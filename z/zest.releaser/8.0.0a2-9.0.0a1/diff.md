# Comparing `tmp/zest.releaser-8.0.0a2.tar.gz` & `tmp/zest.releaser-9.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zest.releaser-8.0.0a2.tar", last modified: Thu Apr  6 15:46:36 2023, max compression
+gzip compressed data, was "zest.releaser-9.0.0a1.tar", last modified: Thu Jul 13 10:09:25 2023, max compression
```

## Comparing `zest.releaser-8.0.0a2.tar` & `zest.releaser-9.0.0a1.tar`

### file list

```diff
@@ -1,88 +1,86 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 15:46:36.353483 zest.releaser-8.0.0a2/
--rw-r--r--   0 maurits    (501) staff       (20)     3034 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1288 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      938 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/CREDITS.rst
--rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      756 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/LICENSE.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    13852 2023-04-06 15:46:36.353715 zest.releaser-8.0.0a2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     8496 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 15:46:36.317024 zest.releaser-8.0.0a2/doc/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 15:46:36.328550 zest.releaser-8.0.0a2/doc/source/
--rw-r--r--   0 maurits    (501) staff       (20)     1804 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/doc/source/assumptions.rst
--rw-r--r--   0 maurits    (501) staff       (20)    50612 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/doc/source/changelog.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6911 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/doc/source/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)       32 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/doc/source/credits.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3355 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/doc/source/developing.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7705 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/doc/source/entrypoints.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1265 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/doc/source/further_reading.rst
--rw-r--r--   0 maurits    (501) staff       (20)      837 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/doc/source/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6754 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/doc/source/options.rst
--rw-r--r--   0 maurits    (501) staff       (20)       30 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/doc/source/overview.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1165 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/doc/source/project.rst
--rw-r--r--   0 maurits    (501) staff       (20)     9536 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/doc/source/uploading.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3360 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/doc/source/versions.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3204 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      340 2023-04-06 15:46:36.354517 zest.releaser-8.0.0a2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)      191 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/setup.py
--rw-r--r--   0 maurits    (501) staff       (20)      229 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/tox.ini
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 15:46:36.328976 zest.releaser-8.0.0a2/zest/
--rw-r--r--   0 maurits    (501) staff       (20)      245 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 15:46:36.340119 zest.releaser-8.0.0a2/zest/releaser/
--rw-r--r--   0 maurits    (501) staff       (20)      398 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3063 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/addchangelogentry.py
--rw-r--r--   0 maurits    (501) staff       (20)    18151 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/baserelease.py
--rw-r--r--   0 maurits    (501) staff       (20)     6267 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/bumpversion.py
--rw-r--r--   0 maurits    (501) staff       (20)     1241 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/choose.py
--rw-r--r--   0 maurits    (501) staff       (20)      962 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/fullrelease.py
--rw-r--r--   0 maurits    (501) staff       (20)     4159 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/git.py
--rw-r--r--   0 maurits    (501) staff       (20)      831 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/lasttagdiff.py
--rw-r--r--   0 maurits    (501) staff       (20)      833 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/lasttaglog.py
--rw-r--r--   0 maurits    (501) staff       (20)     2309 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/longtest.py
--rw-r--r--   0 maurits    (501) staff       (20)     5132 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/postrelease.py
--rw-r--r--   0 maurits    (501) staff       (20)     2146 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/preparedocs.py
--rw-r--r--   0 maurits    (501) staff       (20)     4533 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/prerelease.py
--rw-r--r--   0 maurits    (501) staff       (20)    24132 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/pypi.py
--rw-r--r--   0 maurits    (501) staff       (20)    12986 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/release.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 15:46:36.353155 zest.releaser-8.0.0a2/zest/releaser/tests/
--rw-r--r--   0 maurits    (501) staff       (20)       10 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3657 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/addchangelogentry.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4318 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/baserelease.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4598 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/bumpversion.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1199 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/choose.txt
--rw-r--r--   0 maurits    (501) staff       (20)      121 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/cmd_error.py
--rw-r--r--   0 maurits    (501) staff       (20)    20480 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/example.tar
--rw-r--r--   0 maurits    (501) staff       (20)     3166 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/fullrelease.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4124 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/functional-git.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4200 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/functional-with-hooks.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4336 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/functional.py
--rw-r--r--   0 maurits    (501) staff       (20)     5662 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/git.txt
--rw-r--r--   0 maurits    (501) staff       (20)     9742 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/postrelease.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1891 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/preparedocs.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1172 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/prerelease.txt
--rw-r--r--   0 maurits    (501) staff       (20)    12003 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/pypi.txt
--rw-r--r--   0 maurits    (501) staff       (20)      203 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/pypirc_both.txt
--rw-r--r--   0 maurits    (501) staff       (20)      341 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/pypirc_new.txt
--rw-r--r--   0 maurits    (501) staff       (20)      109 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/pypirc_no_input.txt
--rw-r--r--   0 maurits    (501) staff       (20)      107 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/pypirc_no_release.txt
--rw-r--r--   0 maurits    (501) staff       (20)      123 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/pypirc_old.txt
--rw-r--r--   0 maurits    (501) staff       (20)       37 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/pypirc_simple.txt
--rw-r--r--   0 maurits    (501) staff       (20)      155 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/pypirc_universal_nocreate.txt
--rw-r--r--   0 maurits    (501) staff       (20)      127 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/pypirc_yes_release.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4236 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/pyproject-toml.txt
--rw-r--r--   0 maurits    (501) staff       (20)      400 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)     3118 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/release.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2791 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)    22286 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/utils.txt
--rw-r--r--   0 maurits    (501) staff       (20)     9600 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/tests/vcs.txt
--rw-r--r--   0 maurits    (501) staff       (20)    32636 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)    17236 2023-04-06 15:46:35.000000 zest.releaser-8.0.0a2/zest/releaser/vcs.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 15:46:36.332499 zest.releaser-8.0.0a2/zest.releaser.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    13852 2023-04-06 15:46:36.000000 zest.releaser-8.0.0a2/zest.releaser.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2301 2023-04-06 15:46:36.000000 zest.releaser-8.0.0a2/zest.releaser.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-06 15:46:36.000000 zest.releaser-8.0.0a2/zest.releaser.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)      951 2023-04-06 15:46:36.000000 zest.releaser-8.0.0a2/zest.releaser.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        5 2023-04-06 15:46:36.000000 zest.releaser-8.0.0a2/zest.releaser.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-06 15:46:36.000000 zest.releaser-8.0.0a2/zest.releaser.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      185 2023-04-06 15:46:36.000000 zest.releaser-8.0.0a2/zest.releaser.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        5 2023-04-06 15:46:36.000000 zest.releaser-8.0.0a2/zest.releaser.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 10:09:25.811226 zest.releaser-9.0.0a1/
+-rw-r--r--   0 maurits    (501) staff       (20)     3648 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1288 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      938 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/CREDITS.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      756 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/LICENSE.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    13996 2023-07-13 10:09:25.811405 zest.releaser-9.0.0a1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     8076 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 10:09:25.787601 zest.releaser-9.0.0a1/doc/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 10:09:25.795598 zest.releaser-9.0.0a1/doc/source/
+-rw-r--r--   0 maurits    (501) staff       (20)     2010 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/doc/source/assumptions.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    50612 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/doc/source/changelog.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6910 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/doc/source/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)       32 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/doc/source/credits.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3191 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/doc/source/developing.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     8122 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/doc/source/entrypoints.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1265 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/doc/source/further_reading.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      837 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/doc/source/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     7096 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/doc/source/options.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       30 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/doc/source/overview.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1165 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/doc/source/project.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     9536 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/doc/source/uploading.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3566 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/doc/source/versions.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3386 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      294 2023-07-13 10:09:25.811946 zest.releaser-9.0.0a1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)      146 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)      251 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/tox.ini
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 10:09:25.788069 zest.releaser-9.0.0a1/zest/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 10:09:25.802553 zest.releaser-9.0.0a1/zest/releaser/
+-rw-r--r--   0 maurits    (501) staff       (20)      398 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3063 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/addchangelogentry.py
+-rw-r--r--   0 maurits    (501) staff       (20)    18351 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/baserelease.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6297 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/bumpversion.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1241 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/choose.py
+-rw-r--r--   0 maurits    (501) staff       (20)      962 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/fullrelease.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4178 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/git.py
+-rw-r--r--   0 maurits    (501) staff       (20)      831 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/lasttagdiff.py
+-rw-r--r--   0 maurits    (501) staff       (20)      833 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/lasttaglog.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2315 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/longtest.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5172 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/postrelease.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2146 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/preparedocs.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4590 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/prerelease.py
+-rw-r--r--   0 maurits    (501) staff       (20)    24741 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/pypi.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13543 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/release.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 10:09:25.810987 zest.releaser-9.0.0a1/zest/releaser/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)       10 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3657 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/addchangelogentry.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4446 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/baserelease.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4598 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/bumpversion.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1199 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/choose.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/cmd_error.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17408 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/example.tar
+-rw-r--r--   0 maurits    (501) staff       (20)     3166 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/fullrelease.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3936 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/functional-git.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4444 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/functional-with-hooks.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4311 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/functional.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5662 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/git.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     9742 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/postrelease.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1891 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/preparedocs.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1172 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/prerelease.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    12174 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/pypi.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      203 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/pypirc_both.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      275 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/pypirc_new.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      109 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/pypirc_no_input.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      107 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/pypirc_no_release.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       57 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/pypirc_old.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       37 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/pypirc_simple.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      155 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/pypirc_universal_nocreate.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      127 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/pypirc_yes_release.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4211 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/pyproject-toml.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      400 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)     3118 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/release.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2857 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/test_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)    22286 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/utils.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     9600 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/tests/vcs.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    34197 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)    18452 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest/releaser/vcs.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 10:09:25.797601 zest.releaser-9.0.0a1/zest.releaser.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    13996 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest.releaser.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2238 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest.releaser.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest.releaser.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      951 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest.releaser.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest.releaser.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      223 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest.releaser.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        5 2023-07-13 10:09:25.000000 zest.releaser-9.0.0a1/zest.releaser.egg-info/top_level.txt
```

### Comparing `zest.releaser-8.0.0a2/CHANGES.rst` & `zest.releaser-9.0.0a1/CHANGES.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,33 @@
 Changelog for zest.releaser
 ===========================
 
+9.0.0a1 (2023-07-13)
+--------------------
+
+- Changed build system to pypa/build instead of explicitly using
+  setuptools.
+
+- Zest.releaser's settings can now also be placed in ``pyproject.toml``.
+
+- Use native namespace packages for ``zest.releaser``, instead of
+  deprecated ``pkg_resources`` based ones.
+
+- Added pre-commit config for neater code (black, flake8, isort).
+
+- Dropped support for python 3.7. Together with switching to ``build`` and
+  ``pyproject.toml``, this warrants a major version bump.
+
+
+8.0.0 (2023-05-05)
+------------------
+
+- Make final release, no changes since latest alpha.  [maurits]
+
+
 8.0.0a2 (2023-04-06)
 --------------------
 
 - Always create wheels, except when you explicitly switch this off in the config:
   ``[zest.releaser] create-wheel = no``.
   If the ``wheel`` package is not available, we still do not create wheels.
   Fixes `issue 406 <https://github.com/zestsoftware/zest.releaser/issues/406>`_.
```

### Comparing `zest.releaser-8.0.0a2/CONTRIBUTING.rst` & `zest.releaser-9.0.0a1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/CREDITS.rst` & `zest.releaser-9.0.0a1/CREDITS.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/LICENSE.GPL` & `zest.releaser-9.0.0a1/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/LICENSE.rst` & `zest.releaser-9.0.0a1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/PKG-INFO` & `zest.releaser-9.0.0a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: zest.releaser
-Version: 8.0.0a2
+Version: 9.0.0a1
 Summary: Software releasing made easy and repeatable
 Author-email: Reinout van Rees <reinout@vanrees.org>, Maurits van Rees <maurits@vanrees.org>
 License: GPL
 Project-URL: documentation, https://zestreleaser.readthedocs.io
 Project-URL: repository, https://github.com/zestsoftware/zest.releaser/
 Project-URL: changelog, https://github.com/zestsoftware/zest.releaser/blob/master/CHANGES.rst
 Keywords: releasing,packaging,pypi
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: recommended
 Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 
 Package releasing made easy: zest.releaser overview and installation
 ====================================================================
@@ -71,15 +70,15 @@
 
 Compatibility / Dependencies
 ----------------------------
 
 .. image:: https://img.shields.io/pypi/pyversions/zest.releaser?   :alt: PyPI - Python Version
 .. image:: https://img.shields.io/pypi/implementation/zest.releaser?   :alt: PyPI - Implementation
 
-``zest.releaser`` works on Python 3.7+, including PyPy3.
+``zest.releaser`` works on Python 3.8+, including PyPy3.
 Tested until Python 3.11, but see ``tox.ini`` for the canonical place for that.
 
 To be sure: the packages that you release with ``zest.releaser`` may
 very well work on other Python versions: that totally depends on your
 package.
 
 We depend on:
@@ -93,26 +92,21 @@
 
 Since version 4.0 there is a ``recommended`` extra that you can get by
 installing ``zest.releaser[recommended]`` instead of ``zest.releaser``.  It
 contains a few trusted add-ons that we feel are useful for the great majority
 of ``zest.releaser`` users:
 
 - wheel_ for creating a Python wheel that we upload to PyPI next to
-  the standard source distribution.  Wheels are the new Python package
-  format.  Create or edit ``setup.cfg`` in your project (or globally
-  in your ``~/.pypirc``) and create a section ``[zest.releaser]`` with
-  ``create-wheel = yes`` to create a wheel to upload to PyPI.  See
-  http://pythonwheels.com for deciding whether this is a good idea for
-  your package.  Briefly, if it is a pure Python 2 *or* pure Python 3
-  package: just do it. If it is a pure Python 2 *and* a pure Python 3
-  project, it is known as a "universal" wheel, because one wheel can
-  be installed on all implementations and versions of Python. If you
-  indicate this in ``setup.cfg`` with the section ``[bdist_wheel]``
-  having ``universal = 1``, then we will automatically upload a wheel,
-  unless ``create-wheel`` is explicitly set to false.
+  the standard source distribution.  Wheels are the official binary
+  distribution format for Python.
+  Since version 8.0.0a2 we always create wheels, except when you
+  explicitly switch this off in the config:
+  ``create-wheel = false``.
+  If you are sure you want "universal" wheels, follow the directions from the
+  `wheel documentation <https://wheel.readthedocs.io/en/stable/user_guide.html>`_.
 
 - `check-manifest`_ checks your ``MANIFEST.in`` file for completeness,
   or tells you that you need such a file.  It basically checks if all
   version controlled files are ending up the the distribution that we
   will upload.  This may avoid 'brown bag' releases that are missing
   files.
 
@@ -248,14 +242,37 @@
 
 * `Mateusz Legięcki <https://github.com/Behoston>`_ added a dockerfile for
   much easier testing.
 
 Changelog for zest.releaser
 ===========================
 
+9.0.0a1 (2023-07-13)
+--------------------
+
+- Changed build system to pypa/build instead of explicitly using
+  setuptools.
+
+- Zest.releaser's settings can now also be placed in ``pyproject.toml``.
+
+- Use native namespace packages for ``zest.releaser``, instead of
+  deprecated ``pkg_resources`` based ones.
+
+- Added pre-commit config for neater code (black, flake8, isort).
+
+- Dropped support for python 3.7. Together with switching to ``build`` and
+  ``pyproject.toml``, this warrants a major version bump.
+
+
+8.0.0 (2023-05-05)
+------------------
+
+- Make final release, no changes since latest alpha.  [maurits]
+
+
 8.0.0a2 (2023-04-06)
 --------------------
 
 - Always create wheels, except when you explicitly switch this off in the config:
   ``[zest.releaser] create-wheel = no``.
   If the ``wheel`` package is not available, we still do not create wheels.
   Fixes `issue 406 <https://github.com/zestsoftware/zest.releaser/issues/406>`_.
```

### Comparing `zest.releaser-8.0.0a2/README.rst` & `zest.releaser-9.0.0a1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 Compatibility / Dependencies
 ----------------------------
 
 .. image:: https://img.shields.io/pypi/pyversions/zest.releaser?   :alt: PyPI - Python Version
 .. image:: https://img.shields.io/pypi/implementation/zest.releaser?   :alt: PyPI - Implementation
 
-``zest.releaser`` works on Python 3.7+, including PyPy3.
+``zest.releaser`` works on Python 3.8+, including PyPy3.
 Tested until Python 3.11, but see ``tox.ini`` for the canonical place for that.
 
 To be sure: the packages that you release with ``zest.releaser`` may
 very well work on other Python versions: that totally depends on your
 package.
 
 We depend on:
@@ -63,26 +63,21 @@
 
 Since version 4.0 there is a ``recommended`` extra that you can get by
 installing ``zest.releaser[recommended]`` instead of ``zest.releaser``.  It
 contains a few trusted add-ons that we feel are useful for the great majority
 of ``zest.releaser`` users:
 
 - wheel_ for creating a Python wheel that we upload to PyPI next to
-  the standard source distribution.  Wheels are the new Python package
-  format.  Create or edit ``setup.cfg`` in your project (or globally
-  in your ``~/.pypirc``) and create a section ``[zest.releaser]`` with
-  ``create-wheel = yes`` to create a wheel to upload to PyPI.  See
-  http://pythonwheels.com for deciding whether this is a good idea for
-  your package.  Briefly, if it is a pure Python 2 *or* pure Python 3
-  package: just do it. If it is a pure Python 2 *and* a pure Python 3
-  project, it is known as a "universal" wheel, because one wheel can
-  be installed on all implementations and versions of Python. If you
-  indicate this in ``setup.cfg`` with the section ``[bdist_wheel]``
-  having ``universal = 1``, then we will automatically upload a wheel,
-  unless ``create-wheel`` is explicitly set to false.
+  the standard source distribution.  Wheels are the official binary
+  distribution format for Python.
+  Since version 8.0.0a2 we always create wheels, except when you
+  explicitly switch this off in the config:
+  ``create-wheel = false``.
+  If you are sure you want "universal" wheels, follow the directions from the
+  `wheel documentation <https://wheel.readthedocs.io/en/stable/user_guide.html>`_.
 
 - `check-manifest`_ checks your ``MANIFEST.in`` file for completeness,
   or tells you that you need such a file.  It basically checks if all
   version controlled files are ending up the the distribution that we
   will upload.  This may avoid 'brown bag' releases that are missing
   files.
```

### Comparing `zest.releaser-8.0.0a2/doc/source/assumptions.rst` & `zest.releaser-9.0.0a1/doc/source/assumptions.rst`

 * *Files 5% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 ===========
 
 Zest.releaser originated at `Zest software <https://zestsoftware.nl>`_ so there
 are some assumptions built-in that might or might not fit you.  Lots of people
 are using it in various companies and open source projects, so it'll probably
 fit :-)
 
-- We absolutely need a version. There's a ``version.txt`` or ``setup.py`` in
-  your project. The ``version.txt`` has a single line with the version number
-  (newline optional). The ``setup.py`` should have a single ``version =
-  '0.3'`` line somewhere. You can also have it in the actual ``setup()`` call,
-  on its own line still, as `` version = '0.3',``. Indentation and comma are
-  preserved. If your ``setup.py`` actually reads the version from your
-  ``setup.cfg`` (as `it does automatically
+- We absolutely need a version. There's a ``version.txt``, ``setup.py``, or
+  ``pyproject.toml`` in your project. The ``version.txt`` has a single line
+  with the version number (newline optional). The ``setup.py`` should have a
+  single ``version = '0.3'`` line somewhere. You can also have it in the
+  actual ``setup()`` call, on its own line still, as `` version = '0.3',``.
+  Indentation and comma are preserved. If your ``setup.py`` actually reads
+  the version from your ``setup.cfg`` (as `it does automatically
   <https://setuptools.readthedocs.io/en/latest/setuptools.html#configuring-
   setup-using-setup-cfg-files>`_ using ``setuptools`` since version 30.3.0),
   then the version will be modified there too. If you need something special,
   you can always do a ``version=version`` and put the actual version statement
   in a zest.releaser- friendly format near the top of the file. Reading (in
-  Plone products) a version.txt into setup.py works great, too.
+  Plone products) a version.txt into setup.py works great, too. If you use
+  ``pyproject.toml``, you should put the version under the ``project``
+  metadata section, which also contains the package name, as a single line like
+  ``version = "0.3"``.
 
 - The history/changes file restriction is probably the most severe at the
   moment. zest.releaser searches for a restructuredtext header with
   parenthesis. So something like::
 
     Changelog for xyz
     =================
```

### Comparing `zest.releaser-8.0.0a2/doc/source/changelog.rst` & `zest.releaser-9.0.0a1/doc/source/changelog.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/doc/source/conf.py` & `zest.releaser-9.0.0a1/doc/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 
 # The font size ('10pt', '11pt' or '12pt').
 latex_font_size = "11pt"
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-    ("index", "%s.tex" % project, u"%s Documentation" % project, author, "manual"),
+    ("index", "%s.tex" % project, "%s Documentation" % project, author, "manual"),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
```

### Comparing `zest.releaser-8.0.0a2/doc/source/developing.rst` & `zest.releaser-9.0.0a1/doc/source/developing.rst`

 * *Files 25% similar despite different names*

```diff
@@ -37,59 +37,59 @@
 
 
 Running tests
 -------------
 
 Actually, this should be easy now, because we use tox.
 So ``pip install tox`` somewhere, probably in a virtualenv, maybe the current directory,
-and call it:
+and call it::
 
-    tox
+    $ tox
 
 You probably want to run the tests for all environments in parallel::
 
-    tox -p auto
+    $ tox -p auto
 
 To run a specific environment and a specific test file::
 
-    tox -e py38 -- utils.txt
+    $ tox -e py38 -- utils.txt
+
+
+Code formatting
+---------------
+
+We use black/flake8/isort. To make it easy to configure and run, there's a
+pre-commit config. Enable it with::
+
+    $ pre-commit install
+
+That will run it before every commit. You can also run it periodically when
+developing::
+
+    $ pre-commit run --all
 
 
 Python versions
 ---------------
 
-The tests currently pass on python 3.7-3.11 and PyPy3.
+The tests currently pass on python 3.8-3.11 and PyPy3.
 
 
 Necessary programs
 ------------------
 
 To run the tests, you need to have the supported versioning systems installed.
-Since version 7, we only support ``git``.
-On ubuntu::
-
-  $ sudo apt-get install git
+Since version 7, we only support ``git``, which you already have installed
+probably :-)
 
 There may be test failures when you have different versions of these programs.
-In that case, please investigate as these may be genuine errors.
-In the past, ``git`` commands would give slightly different output.
-If the output of a command changes again, we may need extra compatibility code in ``test_setup.py``
-
-
-Setuptools is needed
---------------------
-
-You also need ``setuptools`` in your system path.  This is because
-we basically call 'sys.executable setup.py egg_info' directly (in the tests
-and in the actual code), which will give an import error on setuptools
-otherwise.  There is a branch with a hack that solves this but it sounds too
-hacky.
-
-TODO: calling ``setup.py`` from the command line is not recommended anymore.
-We should upgrade the code to no longer do that.
+In that case, please investigate as these *may* be genuine errors.  In the
+past, ``git`` commands would give slightly different output.  If the output of
+a command changes again, we may need extra compatibility code in
+``test_setup.py``.
 
 
 Building the documentation locally
 -------------------------------------
 
 If you worked on the documentation, we suggest you verify the markup
 and the result by building the documentation locally and view your
```

### Comparing `zest.releaser-8.0.0a2/doc/source/entrypoints.rst` & `zest.releaser-9.0.0a1/doc/source/entrypoints.rst`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,19 @@
       entry_points={
           #'console_scripts': [
           #    'myscript = my.package.scripts:main'],
           'zest.releaser.prereleaser.middle': [
               'dosomething = my.package.some:some_entrypoint',
               ]},
 
+or like this in your pyproject.toml::
+
+    [project.entry-points."zest.releaser.prereleaser.middle"]
+    dosomething = "my.package.some:some_entrypoint"
+
 Entry-points can also be specified in the setup.cfg file like this
 (The options will be split by white-space and processed in the given
 order.)::
 
     [zest.releaser]
     prereleaser.middle =
        my.package.some.some_entrypoint
@@ -80,14 +85,23 @@
 replace ``prereleaser``
 with the respective command name (`prerelease`, `release`, `postrelease`,
 etc.)
 and ``middle`` with the respective hook name (`before`, `middle`, `after`,
 `after_checkout`, etc.)
 as needed.
 
+Similarly, they can also be placed in the ``tool.zest-releaser`` config section of
+pyproject.toml like this::
+
+    [tool.zest-releaser]
+    prereleaser.middle = [
+        "my.package.some.some_entrypoint",
+        "our.package.other_module.other_function"
+    ]
+
 See the ``setup.py`` of ``zest.releaser`` itself for some real world examples.
 
 You'll have to make sure that the zest.releaser scripts know about your entry
 points, for instance by placing your egg (with entry point) in the same
 zc.recipe.egg section in your buildout as where you placed zest.releaser.  Or,
 if you installed zest.releaser globally, your egg-with-entrypoint has to be
 globally installed, too.
```

### Comparing `zest.releaser-8.0.0a2/doc/source/further_reading.rst` & `zest.releaser-9.0.0a1/doc/source/further_reading.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/doc/source/index.rst` & `zest.releaser-9.0.0a1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/doc/source/options.rst` & `zest.releaser-9.0.0a1/doc/source/options.rst`

 * *Files 12% similar despite different names*

```diff
@@ -64,60 +64,55 @@
 
 Lots of things may be in this file, but zest.releaser looks for a
 ``zest.releaser`` section, like this::
 
   [zest.releaser]
   some-option = some value
 
-For yes/no options, you can use no/false/off/0 or yes/true/on/1 as
+For true/false options, you can use no/false/off/0 or yes/true/on/1 as
 answers; upper, lower or mixed case are all fine.
 
 Various options change the default answer of a question.
 So if you want to use the ``--no-input`` command line option
 or want to press Enter a couple of times without thinking too much,
 see if you can tweak the default answers by setting one of these options
 
 We have these options:
 
-release = yes / no
-    Default: yes.  When this is false, zest.releaser sets ``no`` as
+release = true / false
+    Default: true.  When this is false, zest.releaser sets ``false`` as
     default answer for the question if you want to create a checkout
     of the tag.
 
-create-wheel = yes / no
-    Default: no.  Set to yes if you want zest.releaser to create
-    Python wheels.  You need to install the ``wheel`` package for this
-    to work.
-
-    If the package is a universal wheel, indicated by having
-    ``universal = 1`` in the ``[bdist_wheel]`` section of
-    ``setup.cfg``, then the default for this value is yes.
+create-wheel = true / false
+    Default: true, if the recommended ``wheel`` package is installed.
+    Set to false if you do not want zest.releaser to create Python wheels.
 
 extra-message = [ci skip]
     Extra message to add to each commit (prerelease, postrelease).
 
 prefix-message = [TAG]
     Prefix message to add at the beginning of each commit (prerelease, postrelease).
 
-no-input = yes / no
-    Default: no.  Set this to yes to accept default answers for all
+no-input = true / false
+    Default: false.  Set this to true to accept default answers for all
     questions.
 
-register = yes / no
-    Default: no.  Set this to yes to register a package before uploading.
+register = true / false
+    Default: false.  Set this to true to register a package before uploading.
     On the official Python Package Index registering a package is no longer needed,
     and may even fail.
 
-push-changes = yes / no
-    Default: yes.  When this is false, zest.releaser sets ``no`` as
+push-changes = true / false
+    Default: true.  When this is false, zest.releaser sets ``false`` as
     default answer for the question if you want to push the changes to
     the remote.
 
-less-zeroes = yes / no
-    Default: no.
+less-zeroes = true / false
+    Default: false.
     This influences the version suggested by the bumpversion command.
     When set to true:
 
     - Instead of 1.3.0 we will suggest 1.3.
     - Instead of 2.0.0 we will suggest 2.0.
 
 version-levels = a number
@@ -149,16 +144,16 @@
 
 tag-message = a string
     Default: ``Tagging {version}``
     This formatter defines the commit message passed to the ``tag``
     command of the VCS.
     It must contain ``{version}``.
 
-tag-signing = yes / no
-    Default: no.
+tag-signing = true / false
+    Default: false.
     When set to true, tags are signed using the signing feature of the
     respective vcs. Currently tag-signing is only supported for git.
     Note: When you enable it, everyone releasing the project is
     required to have git tag signing set up correctly.
 
 date-format = a string
     Default: ``%%Y-%%m-%%d``
@@ -179,23 +174,34 @@
   Set this to, for example, ``utf-8`` when the encoding of your ``CHANGES.rst``
   file is not determined correctly.
 
 history_format = a string
   Default: empty.
   Set this to ``md`` to handle changelog entries in Markdown.
 
-run-pre-commit = yes / no
-    Default: no.
+run-pre-commit = true / false
+    Default: false.
     New in version 7.3.0.
     When set to true, pre commit hooks are run.
     This may interfere with releasing when they fail.
 
 
 Per project options
 -------------------
 
 You can change some settings per project by adding instructions for
 zest.releaser in a ``setup.cfg`` file.  This will only work for a
 Python package.
 
 These are the same options as the global ones.  If you set an option
 locally in a project, this will override the global option.
+
+You can also set these options in a ``pyproject.toml`` file. If you do
+so, instead of having a ``[zest.releaser]`` section, you should use a
+``[tool.zest-releaser]`` section. For true/false options in a
+``pyproject.toml``, you must use lowercase true or false; for string
+options like ``extra-message`` or ``prefix-message``, you should put
+the value between double quotes, like this::
+
+  [tool.zest-releaser]
+  create-wheel = false
+  extra-message = "[ci skip]"
```

### Comparing `zest.releaser-8.0.0a2/doc/source/project.rst` & `zest.releaser-9.0.0a1/doc/source/project.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/doc/source/uploading.rst` & `zest.releaser-9.0.0a1/doc/source/uploading.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/doc/source/versions.rst` & `zest.releaser-9.0.0a1/doc/source/versions.rst`

 * *Files 5% similar despite different names*

```diff
@@ -46,16 +46,22 @@
   *which* Python file by adding (or updating) the ``setup.cfg`` file next to
   the ``setup.py``. You need a ``[zest.releaser]`` header and a
   ``python-file-with-version`` option::
 
     [zest.releaser]
     python-file-with-version = mypackage/__init__.py
 
+  Alternatively, in ``pyproject.toml``, you can use the following::
+
+    [tool.zest-releaser]
+    python-file-with-version = "mypackage/__init__.py"
+
   Because you need to configure this explicitly, this option takes precedence
-  over any ``setup.py`` or ``version.txt`` file.
+  over any ``setup.py``, ``setup.cfg`` or ``pyproject.toml`` package version,
+  or ``version.txt`` file.
 
 
 Where is the version number being set?
 --------------------------------------
 
 Of those four locations where the version can come from, only the first one
 found is also set to the new value again. Zest.releaser assumes that there's
```

### Comparing `zest.releaser-8.0.0a2/pyproject.toml` & `zest.releaser-9.0.0a1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 [build-system]
 # See https://snarky.ca/what-the-heck-is-pyproject-toml/
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zest.releaser"
-version = "8.0.0a2"
+version = "9.0.0a1"
 description = "Software releasing made easy and repeatable"
 license = {text = "GPL"}
 authors = [
     {name = "Reinout van Rees", email = "reinout@vanrees.org"},
     {name = "Maurits van Rees", email = "maurits@vanrees.org"},
 ]
 dependencies = [
     "setuptools",
     "colorama",
     "requests",
     "twine >= 1.6.0",
+    "build >= 0.6.0.post1",  # 0.6.0 wasn't compatible with Python 3.7
     "tomli; python_version<'3.11'",
+    "setuptools >= 61.0.0",  # older versions can't read pyproject.toml configurations
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 6 - Mature",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -90,7 +91,11 @@
 
 # Documentation generation
 [project.entry-points."zest.releaser.prereleaser.before"]
 preparedocs = "zest.releaser.preparedocs:prepare_entrypoint_documentation"
 
 [tool.isort]
 profile = "plone"
+
+[tool.zest-releaser]
+extra-message = "[ci skip]"
+tag-signing = true
```

### Comparing `zest.releaser-8.0.0a2/zest/releaser/addchangelogentry.py` & `zest.releaser-9.0.0a1/zest/releaser/addchangelogentry.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/zest/releaser/baserelease.py` & `zest.releaser-9.0.0a1/zest/releaser/baserelease.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,23 +73,26 @@
         }
         self.setup_cfg = pypi.SetupConfig()
         if utils.TESTMODE:
             pypirc_old = pkg_resources.resource_filename(
                 "zest.releaser.tests", "pypirc_old.txt"
             )
             self.pypiconfig = pypi.PypiConfig(pypirc_old)
+            self.zest_releaser_config = pypi.ZestReleaserConfig(
+                pypirc_config_filename=pypirc_old
+            )
         else:
             self.pypiconfig = pypi.PypiConfig()
-        if self.pypiconfig.no_input():
+            self.zest_releaser_config = pypi.ZestReleaserConfig()
+        if self.zest_releaser_config.no_input():
             utils.AUTO_RESPONSE = True
 
     @property
     def history_format(self):
-        default = "rst"
-        config_value = self.pypiconfig.history_format()
+        config_value = self.zest_releaser_config.history_format()
         history_file = self.data.get("history_file") or ""
         return utils.history_format(config_value, history_file)
 
     @property
     def underline_char(self):
         underline_char = "-"
         if self.history_format == "md":
@@ -120,16 +123,16 @@
         """
         self.data["history_lines"] = []
         self.data["history_file"] = None
         self.data["history_encoding"] = None
         self.data["headings"] = []
         self.data["history_last_release"] = ""
         self.data["history_insert_line_here"] = 0
-        default_location = self.pypiconfig.history_file()
-        fallback_encoding = self.pypiconfig.encoding()
+        default_location = self.zest_releaser_config.history_file()
+        fallback_encoding = self.zest_releaser_config.encoding()
         history_file = self.vcs.history_file(location=default_location)
         self.data["history_file"] = history_file
         if not history_file:
             logger.warning("No history file found")
             return
         logger.debug("Checking %s", history_file)
         history_lines, history_encoding = read_text_file(
@@ -273,18 +276,17 @@
             message.encode(orig_encoding)
         except UnicodeEncodeError:
             logger.warning(
                 "Changelog entry does not have the same encoding (%s) as "
                 "the existing file. This might give problems.",
                 orig_encoding,
             )
-            config = self.setup_cfg.config
             fallback_encodings = []
-            if config.has_option("zest.releaser", "encoding"):
-                encoding = config.get("zest.releaser", "encoding")
+            if "encoding" in self.zest_releaser_config:
+                encoding = self.zest_releaser_config["encoding"]
                 if encoding != orig_encoding:
                     fallback_encodings.append(encoding)
             encoding = "utf-8"
             if encoding != orig_encoding:
                 fallback_encodings.append(encoding)
             for encoding in fallback_encodings:
                 try:
@@ -412,23 +414,23 @@
             logger.info(commit)
 
     def _push(self):
         """Offer to push changes, if needed."""
         push_cmds = self.vcs.push_commands()
         if not push_cmds:
             return
-        default_anwer = self.pypiconfig.push_changes()
+        default_anwer = self.zest_releaser_config.push_changes()
         if utils.ask("OK to push commits to the server?", default=default_anwer):
             for push_cmd in push_cmds:
                 output = execute_command(push_cmd)
                 logger.info(output)
 
     def _run_hooks(self, when):
         which_releaser = self.__class__.__name__.lower()
-        utils.run_hooks(self.setup_cfg, which_releaser, when, self.data)
+        utils.run_hooks(self.zest_releaser_config, which_releaser, when, self.data)
 
     def run(self):
         self._run_hooks("before")
         self.prepare()
         self._run_hooks("middle")
         self.execute()
         self._run_hooks("after")
@@ -436,14 +438,14 @@
     def prepare(self):
         raise NotImplementedError()
 
     def execute(self):
         raise NotImplementedError()
 
     def update_commit_message(self, msg):
-        prefix_message = self.pypiconfig.prefix_message()
-        extra_message = self.pypiconfig.extra_message()
+        prefix_message = self.zest_releaser_config.prefix_message()
+        extra_message = self.zest_releaser_config.extra_message()
         if prefix_message:
             msg = "%s %s" % (prefix_message, msg)
         if extra_message:
             msg += "\n\n%s" % extra_message
         return msg
```

### Comparing `zest.releaser-8.0.0a2/zest/releaser/bumpversion.py` & `zest.releaser-9.0.0a1/zest/releaser/bumpversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,17 +105,17 @@
             else:
                 print(f"Last tag: {last_tag_version}")
             print(f"Current version: {original_version}")
             params = dict(
                 feature=feature,
                 breaking=breaking,
                 final=final,
-                less_zeroes=self.pypiconfig.less_zeroes(),
-                levels=self.pypiconfig.version_levels(),
-                dev_marker=self.pypiconfig.development_marker(),
+                less_zeroes=self.zest_releaser_config.less_zeroes(),
+                levels=self.zest_releaser_config.version_levels(),
+                dev_marker=self.zest_releaser_config.development_marker(),
             )
             if final:
                 minimum_version = utils.suggest_version(original_version, **params)
                 if minimum_version is None:
                     print("No version bump needed.")
                     sys.exit(0)
             else:
```

### Comparing `zest.releaser-8.0.0a2/zest/releaser/choose.py` & `zest.releaser-9.0.0a1/zest/releaser/choose.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/zest/releaser/fullrelease.py` & `zest.releaser-9.0.0a1/zest/releaser/fullrelease.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/zest/releaser/git.py` & `zest.releaser-9.0.0a1/zest/releaser/git.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,18 +24,18 @@
             __import__("setuptools_git")
         except ImportError:
             return False
         return True
 
     @property
     def name(self):
-        package_name = self.get_setup_py_name()
+        package_name = self._extract_name()
         if package_name:
             return package_name
-        # No setup.py? With git we can probably only fall back to the directory
+        # No python package name? With git we can probably only fall back to the directory
         # name as there's no svn-url with a usable name in it.
         dir_name = os.path.basename(os.getcwd())
         dir_name = fs_to_text(dir_name)
         return dir_name
 
     def available_tags(self):
         tag_info = execute_command(["git", "tag"])
@@ -64,15 +64,15 @@
         return version
 
     def cmd_diff(self):
         return ["git", "diff"]
 
     def cmd_commit(self, message):
         parts = ["git", "commit", "-a", "-m", message]
-        if not self.pypi_cfg.run_pre_commit():
+        if not self.zest_releaser_config.run_pre_commit():
             parts.append("-n")
         return parts
 
     def cmd_diff_last_commit_against_tag(self, version):
         return ["git", "diff", version]
 
     def cmd_log_since_tag(self, version):
```

### Comparing `zest.releaser-8.0.0a2/zest/releaser/lasttagdiff.py` & `zest.releaser-9.0.0a1/zest/releaser/lasttagdiff.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/zest/releaser/lasttaglog.py` & `zest.releaser-9.0.0a1/zest/releaser/lasttaglog.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/zest/releaser/longtest.py` & `zest.releaser-9.0.0a1/zest/releaser/longtest.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,12 +76,13 @@
 def main():
     parser = utils.base_option_parser()
     parser.add_argument(
         "--headless",
         action="store_true",
         dest="headless",
         default=False,
-        help="Do not open a browser window with the HTML result")
+        help="Do not open a browser window with the HTML result",
+    )
     options = utils.parse_options(parser)
     utils.configure_logging()
     code = show_longdesc(headless=options.headless)
     sys.exit(code)
```

### Comparing `zest.releaser-8.0.0a2/zest/releaser/postrelease.py` & `zest.releaser-9.0.0a1/zest/releaser/postrelease.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         self.data.update(
             dict(
                 breaking=breaking,
                 commit_msg=COMMIT_MSG,
                 feature=feature,
                 final=final,
                 dev_version_template=DEV_VERSION_TEMPLATE,
-                development_marker=self.pypiconfig.development_marker(),
+                development_marker=self.zest_releaser_config.development_marker(),
                 history_header=HISTORY_HEADER,
                 update_history=True,
             )
         )
 
     def prepare(self):
         """Prepare self.data by asking about new dev version"""
@@ -78,17 +78,17 @@
             sys.exit(1)
         # Clean it up to a non-development version.
         current = utils.cleanup_version(current)
         params = dict(
             breaking=self.data["breaking"],
             feature=self.data["feature"],
             final=self.data["final"],
-            less_zeroes=self.pypiconfig.less_zeroes(),
-            levels=self.pypiconfig.version_levels(),
-            dev_marker=self.pypiconfig.development_marker(),
+            less_zeroes=self.zest_releaser_config.less_zeroes(),
+            levels=self.zest_releaser_config.version_levels(),
+            dev_marker=self.zest_releaser_config.development_marker(),
         )
         suggestion = utils.suggest_version(current, **params)
         print("Current version is %s" % current)
         q = (
             "Enter new development version "
             "('%(development_marker)s' will be appended)" % self.data
         )
```

### Comparing `zest.releaser-8.0.0a2/zest/releaser/preparedocs.py` & `zest.releaser-9.0.0a1/zest/releaser/preparedocs.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/zest/releaser/prerelease.py` & `zest.releaser-9.0.0a1/zest/releaser/prerelease.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 try:
     # This is a recommended dependency.
     # Not a core dependency for now, as zest.releaser can also be used for
     # non-Python projects.
     from pep440 import is_canonical
 except ImportError:
+
     def is_canonical(version):
         logger.debug("Using dummy is_canonical that always returns True.")
         return True
 
 
 logger = logging.getLogger(__name__)
 
@@ -41,15 +42,15 @@
     self.data holds data that can optionally be changed by plugins.
 
     """
 
     def __init__(self, vcs=None):
         baserelease.Basereleaser.__init__(self, vcs=vcs)
         # Prepare some defaults for potential overriding.
-        date_format = self.pypiconfig.date_format()
+        date_format = self.zest_releaser_config.date_format()
         self.data.update(
             dict(
                 commit_msg=PRERELEASE_COMMIT_MSG,
                 history_header=HISTORY_HEADER,
                 today=datetime.datetime.today().strftime(date_format),
                 update_history=True,
             )
@@ -105,15 +106,17 @@
             sys.exit(1)
         suggestion = utils.cleanup_version(original_version)
         new_version = None
         if not initial:
             while new_version is None:
                 new_version = utils.ask_version("Enter version", default=suggestion)
                 if not is_canonical(new_version):
-                    logger.warning(f"'{new_version}' is not a canonical Python package version.")
+                    logger.warning(
+                        f"'{new_version}' is not a canonical Python package version."
+                    )
                     question = "Do you want to use this version anyway?"
                     if not utils.ask(question):
                         # Set to None: we will ask to enter a new version.
                         new_version = None
         if not new_version:
             new_version = suggestion
         self.data["original_version"] = original_version
```

### Comparing `zest.releaser-8.0.0a2/zest/releaser/pypi.py` & `zest.releaser-9.0.0a1/zest/releaser/pypi.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,34 @@
+from .utils import extract_zestreleaser_configparser
 from configparser import ConfigParser
 from configparser import NoOptionError
 from configparser import NoSectionError
 
 import logging
 import os
 import pkg_resources
 import sys
 
+
+try:
+    # Python 3.11+
+    import tomllib
+except ImportError:
+    # Python 3.10-
+    import tomli as tomllib
+
 try:
     pkg_resources.get_distribution("wheel")
 except pkg_resources.DistributionNotFound:
     USE_WHEEL = False
 else:
     USE_WHEEL = True
 DIST_CONFIG_FILE = ".pypirc"
 SETUP_CONFIG_FILE = "setup.cfg"
+PYPROJECTTOML_CONFIG_FILE = "pyproject.toml"
 DEFAULT_REPOSITORY = "https://upload.pypi.org/legacy/"
 
 logger = logging.getLogger(__name__)
 
 
 class BaseConfig:
     """Base config class with a few helper methods."""
@@ -38,16 +48,15 @@
             try:
                 result = self.config.getboolean(section, key)
             except (NoSectionError, NoOptionError, ValueError):
                 return result
         return result
 
     def _get_text(self, section, key, default=None, raw=False):
-        """Get a text from the config.
-        """
+        """Get a text from the config."""
         result = default
         if self.config is not None:
             try:
                 result = self.config.get(section, key, raw=raw)
             except (NoSectionError, NoOptionError, ValueError):
                 return result
         return result
@@ -74,15 +83,15 @@
 
     def __init__(self):
         """Grab the configuration (overridable for test purposes)"""
         # If there is a setup.cfg in the package, parse it
         if not os.path.exists(self.config_filename):
             self.config = None
             return
-        self.config = ConfigParser()
+        self.config = ConfigParser(interpolation=None)
         self.config.read(self.config_filename)
 
     def has_bad_commands(self):
         if self.config is None:
             return False
         if not self.config.has_section("egg_info"):
             # bail out early as the main section is not there
@@ -124,82 +133,59 @@
             self.config.write(new_setup)
         finally:
             new_setup.close()
         logger.info("New setup.cfg contents:")
         with open(self.config_filename) as config_file:
             print("".join(config_file.readlines()))
 
-    def python_file_with_version(self):
-        """Return Python filename with ``__version__`` marker, if configured.
-
-        Enable this by adding a ``python-file-with-version`` option::
-
-            [zest.releaser]
-            python-file-with-version = reinout/maurits.py
-
-        Return None when nothing has been configured.
-
-        """
-        default = None
-        if self.config is None:
-            return default
-        try:
-            result = self._get_text(
-                "zest.releaser", "python-file-with-version", default=default
-            )
-        except (NoSectionError, NoOptionError, ValueError):
-            return default
-        return result
+    def zest_releaser_config(self):
+        return extract_zestreleaser_configparser(self.config, self.config_filename)
 
 
 class PypiConfig(BaseConfig):
-    """Wrapper around the pypi config file"""
+    """Wrapper around the pypi config file.
 
-    def __init__(self, config_filename=DIST_CONFIG_FILE, use_setup_cfg=True):
+    Contains functions which return information about
+    the pypi configuration.
+    """
+
+    def __init__(self, config_filename=DIST_CONFIG_FILE):
         """Grab the PyPI configuration.
 
         This is .pypirc in the home directory.  It is overridable for
         test purposes.
-
-        If there is a setup.cfg file in the current directory, we read
-        it too.
         """
         self.config_filename = config_filename
-        self.use_setup_cfg = use_setup_cfg
         self.reload()
 
     def reload(self):
         """Load the config.
 
         Do the initial load of the config.
 
         Or reload it in case of problems: this is needed when a pypi
         upload fails, you edit the .pypirc file to fix the account
         settings, and tell release to retry the command.
         """
-        self._read_configfile(use_setup_cfg=self.use_setup_cfg)
+        self._read_configfile()
 
-    def _read_configfile(self, use_setup_cfg=True):
-        """Read the PyPI config file and store it (when valid).
+    def zest_releaser_config(self):
+        return extract_zestreleaser_configparser(self.config, self.config_filename)
 
-        Usually read the setup.cfg too.
-        """
-        rc = self.config_filename
-        if not os.path.isabs(rc):
-            rc = os.path.join(os.path.expanduser("~"), self.config_filename)
-        filenames = [rc]
-        if use_setup_cfg:
-            # If there is a setup.cfg in the package, parse it
-            filenames.append("setup.cfg")
-        files = [f for f in filenames if os.path.exists(f)]
-        if not files:
+    def _read_configfile(self):
+        """Read the PyPI config file and store it (when valid)."""
+        config_filename = self.config_filename
+        if not os.path.exists(config_filename) and not os.path.isabs(config_filename):
+            # When filename is .pypirc, we look in ~/.pypirc
+            config_filename = os.path.join(os.path.expanduser("~"), config_filename)
+        if not os.path.exists(config_filename):
             self.config = None
             return
-        self.config = ConfigParser()
-        self.config.read(files)
+        self.config = ConfigParser(interpolation=None)
+        self.config.read(config_filename)
 
     def twine_repository(self):
         """Gets the repository from Twine environment variables."""
         return os.getenv("TWINE_REPOSITORY")
 
     def twine_repository_url(self):
         """Gets the repository URL from Twine environment variables."""
@@ -248,118 +234,196 @@
                 # when no explicit pypi section is in the file.
                 return ["pypi"]
             # https://github.com/zestsoftware/zest.releaser/issues/199
             index_servers = ["pypi"]
         # The servers all need to have a section in the config file.
         return [server for server in index_servers if self.config.has_section(server)]
 
+
+class PyprojectTomlConfig(BaseConfig):
+    """Wrapper around the pyproject.toml file if available.
+
+    This is for optional zest.releaser-specific settings::
+
+        [tool.zest-releaser]
+        python-file-with-version = "reinout/maurits.py"
+
+
+    """
+
+    config_filename = PYPROJECTTOML_CONFIG_FILE
+
+    def __init__(self):
+        """Grab the configuration (overridable for test purposes)"""
+        # If there is a pyproject.toml in the package, parse it
+        if not os.path.exists(self.config_filename):
+            self.config = None
+            return
+        with open(self.config_filename, "rb") as tomlconfig:
+            self.config = tomllib.load(tomlconfig)
+
+    def zest_releaser_config(self):
+        if self.config is None:
+            return None
+        try:
+            result = self.config["tool"]["zest-releaser"]
+        except KeyError:
+            logger.debug(
+                f"No [tool.zest-releaser] section found in the {self.config_filename}"
+            )
+            return None
+        return result
+
+
+class ZestReleaserConfig:
+    hooks_filename = None
+
+    def load_configs(self, pypirc_config_filename=DIST_CONFIG_FILE):
+        """Load configs from several files.
+
+        The order is this:
+
+        - ~/.pypirc
+        - setup.cfg
+        - pyproject.toml
+
+        A later config file overwrites keys from an earlier config file.
+        I think this order makes the most sense.
+        Example: extra-message = [ci skip]
+        What I expect, is:
+
+        * Most packages won't have this setting.
+        * If you make releases for lots of packages, you probably set this in
+          your global ~/.pypirc.
+        * A few individual packages will explicitly set this.
+          They will expect this to have the effect that the extra message is
+          added to commits, regardless of who makes a release.
+          So this individual package setting should win.
+        * Finally, pyproject.toml is newer than setup.cfg, so it makes sense
+          that this file has the last say.
+        """
+        setup_config = SetupConfig()
+        pypi_config = PypiConfig(config_filename=pypirc_config_filename)
+        pyproject_config = PyprojectTomlConfig()
+        combined_config = {}
+        config_files = [pypi_config]
+        if not self.omit_package_config_in_test:
+            config_files.extend([setup_config, pyproject_config])
+        for config in config_files:
+            if config.zest_releaser_config() is not None:
+                zest_config = config.zest_releaser_config()
+                assert isinstance(zest_config, dict)
+                combined_config.update(zest_config)
+
+                # store which config file contained entrypoint hooks
+                if any(
+                    [
+                        x
+                        for x in zest_config.keys()
+                        if x.lower().startswith(
+                            ("prereleaser.", "releaser.", "postreleaser.")
+                        )
+                    ]
+                ):
+                    self.hooks_filename = config.config_filename
+        self.config = combined_config
+
+    def __init__(
+        self, pypirc_config_filename=DIST_CONFIG_FILE, omit_package_config_in_test=False
+    ):
+        self.omit_package_config_in_test = omit_package_config_in_test
+        self.load_configs(pypirc_config_filename=pypirc_config_filename)
+
     def want_release(self):
         """Does the user normally want to release this package.
 
         Some colleagues find it irritating to have to remember to
         answer the question "Check out the tag (for tweaks or
         pypi/distutils server upload)" with the non-default 'no' when
         in 99 percent of the cases they just make a release specific
         for a customer, so they always answer 'no' here.  This is
         where an extra config option comes in handy: you can influence
         the default answer so you can just keep hitting 'Enter' until
         zest.releaser is done.
 
-        Either in your ~/.pypirc or in a setup.cfg in a specific
+        Either in your ~/.pypirc or in a setup.cfg or pyproject.toml in a specific
         package, add this when you want the default answer to this
         question to be 'no':
 
         [zest.releaser]
         release = no
 
         The default when this option has not been set is True.
 
         Standard config rules apply, so you can use upper or lower or
         mixed case and specify 0, false, no or off for boolean False,
         and 1, on, true or yes for boolean True.
         """
-        return self._get_boolean("zest.releaser", "release", default=True)
-
-    def __get_message_config__(self, config_name):
-        """
-        Return the value of the message configuration based on its name.
-
-        If the configuration does not exist or can't be retrieved, return an empty string.
-
-        :param config_name: Name of the configuration to obtain from configuration file
-        :return: The configuration value or an empty string
-        """
-        default = ""
-        if self.config is None:
-            return default
-        try:
-            result = self._get_text("zest.releaser", config_name, default=default)
-        except (NoSectionError, NoOptionError, ValueError):
-            return default
-        return result
+        return self.config.get("release", True)
 
     def extra_message(self):
         """Return extra text to be added to commit messages.
 
         This can for example be used to skip CI builds.  This at least
         works for Travis.  See
         http://docs.travis-ci.com/user/how-to-skip-a-build/
 
         Enable this mode by adding a ``extra-message`` option, either in the
         package you want to release, or in your ~/.pypirc::
 
             [zest.releaser]
             extra-message = [ci skip]
         """
-        return self.__get_message_config__("extra-message")
+        return self.config.get("extra-message")
 
     def prefix_message(self):
         """Return extra text to be added before the commit message.
 
         This can for example be used follow internal policies on commit messages.
 
         Enable this mode by adding a ``prefix-message`` option, either in the
         package you want to release, or in your ~/.pypirc::
 
             [zest.releaser]
             prefix-message = [TAG]
         """
-        return self.__get_message_config__("prefix-message")
+        return self.config.get("prefix-message")
 
     def history_file(self):
         """Return path of history file.
 
         Usually zest.releaser can find the correct one on its own.
         But sometimes it may not find anything, or it finds multiple
         and selects the wrong one.
 
         Configure this by adding a ``history-file`` option, either in the
         package you want to release, or in your ~/.pypirc::
 
             [zest.releaser]
             history-file = deep/down/historie.doc
         """
-        default = ""
-        if self.config is None:
-            return default
-        marker = object()
-        try:
-            result = self._get_text("zest.releaser", "history-file", default=marker)
-        except (NoSectionError, NoOptionError, ValueError):
-            return default
-        if result == marker:
-            # We were reading an underscore instead of a dash at first.
-            try:
-                result = self._get_text(
-                    "zest.releaser", "history_file", default=default
-                )
-            except (NoSectionError, NoOptionError, ValueError):
-                return default
+        # we were using an underscore at first
+        result = self.config.get("history_file")
+        # but if they're both defined, the hyphenated key takes precedence
+        result = self.config.get("history-file", result)
         return result
 
+    def python_file_with_version(self):
+        """Return Python filename with ``__version__`` marker, if configured.
+
+        Enable this by adding a ``python-file-with-version`` option::
+
+            [zest-releaser]
+            python-file-with-version = reinout/maurits.py
+
+        Return None when nothing has been configured.
+
+        """
+        return self.config.get("python-file-with-version")
+
     def encoding(self):
         """Return encoding to use for text files.
 
         Mostly the changelog and if needed `setup.py`.
 
         The encoding cannot always be determined correctly.
         This setting is a way to fix that.
@@ -367,45 +431,27 @@
 
         Configure this by adding an ``encoding`` option, either in the
         package you want to release, or in your ~/.pypirc::
 
             [zest.releaser]
             encoding = utf-8
         """
-        default = ""
-        if self.config is None:
-            return default
-        try:
-            result = self._get_text(
-                "zest.releaser", "encoding", default=default, raw=True
-            )
-        except (NoSectionError, NoOptionError, ValueError):
-            return default
-        return result
+        return self.config.get("encoding", "")
 
     def history_format(self):
         """Return the format to be used for Changelog files.
 
         Configure this by adding an ``history_format`` option, either in the
         package you want to release, or in your ~/.pypirc, and using ``rst`` for
         Restructured Text and ``md`` for Markdown::
 
             [zest.releaser]
             history_format = md
         """
-        default = ""
-        if self.config is None:
-            return default
-        try:
-            result = self._get_text(
-                "zest.releaser", "history_format", default=default, raw=True
-            )
-        except (NoSectionError, NoOptionError, ValueError):
-            return default
-        return result
+        return self.config.get("history_format", "")
 
     def create_wheel(self):
         """Should we create a Python wheel for this package?
 
         This is next to the standard source distribution that we always create
         when releasing a Python package.
 
@@ -420,15 +466,15 @@
         [zest.releaser]
         create-wheel = no
         """
         if not USE_WHEEL:
             # If the wheel package is not available, we obviously
             # cannot create wheels.
             return False
-        return self._get_boolean("zest.releaser", "create-wheel", True)
+        return self.config.get("create-wheel", True)
 
     def register_package(self):
         """Should we try to register this package with a package server?
 
         For the standard Python Package Index (PyPI), registering a
         package is no longer needed: this is done automatically when
         uploading a distribution for a package.  In fact, trying to
@@ -445,61 +491,52 @@
         [zest.releaser]
         register = yes
 
         Note that if you have specified multiple package servers, this
         option is used for all of them.  There is no way to register and
         upload to server A, and only upload to server B.
         """
-        return self._get_boolean("zest.releaser", "register")
+        return self.config.get("register", False)
 
     def no_input(self):
         """Return whether the user wants to run in no-input mode.
 
         Enable this mode by adding a ``no-input`` option::
 
             [zest.releaser]
             no-input = yes
 
         The default when this option has not been set is False.
         """
-        return self._get_boolean("zest.releaser", "no-input")
+        return self.config.get("no-input", False)
 
     def development_marker(self):
         """Return development marker to be appended in postrelease.
 
         Override the default ``.dev0`` in ~/.pypirc or setup.cfg using
         a ``development-marker`` option::
 
             [zest.releaser]
             development-marker = .dev1
 
         Returns default of ``.dev0`` when nothing has been configured.
         """
-        default = ".dev0"
-        if self.config is None:
-            return default
-        try:
-            result = self._get_text(
-                "zest.releaser", "development-marker", default=default
-            )
-        except (NoSectionError, NoOptionError, ValueError):
-            return default
-        return result
+        return self.config.get("development-marker", ".dev0")
 
     def push_changes(self):
         """Return whether the user wants to push the changes to the remote.
 
         Configure this mode by adding a ``push-changes`` option::
 
             [zest.releaser]
             push-changes = no
 
         The default when this option has not been set is True.
         """
-        return self._get_boolean("zest.releaser", "push-changes", default=True)
+        return self.config.get("push-changes", True)
 
     def less_zeroes(self):
         """Return whether the user prefers less zeroes at the end of a version.
 
         Configure this mode by adding a ``less-zeroes`` option::
 
             [zest.releaser]
@@ -511,15 +548,15 @@
         - Instead of 1.3.0 we will suggest 1.3.
         - Instead of 2.0.0 we will suggest 2.0.
 
         This only makes sense for the bumpversion command.
         In the postrelease command we read this option too,
         but with the current logic it has no effect there.
         """
-        return self._get_boolean("zest.releaser", "less-zeroes")
+        return self.config.get("less-zeroes", False)
 
     def version_levels(self):
         """How many levels does the user prefer in a version number?
 
         Configure this mode by adding a ``version-levels`` option::
 
             [zest.releaser]
@@ -538,20 +575,15 @@
         If the current version number has more levels, we keep them.
         So next version for 1.2.3.4 with levels=1 is 1.2.3.5.
 
         Tweaking version-levels and less-zeroes should give you the
         version number strategy that you prefer.
         """
         default = 0
-        if self.config is None:
-            return default
-        try:
-            result = self.config.getint("zest.releaser", "version-levels")
-        except (NoSectionError, NoOptionError, ValueError):
-            return default
+        result = self.config.get("version-levels", default)
         if result < 0:
             return default
         return result
 
     _tag_format_deprecated_message = "\n".join(
         line.strip()
         for line in """
@@ -573,22 +605,16 @@
         ``tag-format`` must contain exactly one formatting instruction: for the
         ``version`` key.
 
         Accepts also ``%(version)s`` format for backward compatibility.
 
         The default format, when nothing has been configured, is ``{version}``.
         """
-        fmt = "{version}"
-        if self.config is not None:
-            try:
-                fmt = self._get_text(
-                    "zest.releaser", "tag-format", default=fmt, raw=True
-                )
-            except (NoSectionError, NoOptionError, ValueError):
-                pass
+        default_fmt = "{version}"
+        fmt = self.config.get("tag-format", default_fmt)
         if "{version}" in fmt:
             return fmt.format(version=version)
         # BBB:
         if "%(version)s" in fmt:
             proposed_fmt = fmt.replace("%(version)s", "{version}")
             print(self._tag_format_deprecated_message % proposed_fmt)
             return fmt % {"version": version}
@@ -605,22 +631,16 @@
             tag-message = Creating v{version} tag.
 
         ``tag-message`` must contain exactly one formatting
         instruction: for the ``version`` key.
 
         The default format is ``Tagging {version}``.
         """
-        fmt = "Tagging {version}"
-        if self.config:
-            try:
-                fmt = self._get_text(
-                    "zest.releaser", "tag-message", default=fmt, raw=True
-                )
-            except (NoSectionError, NoOptionError, ValueError):
-                pass
+        default_fmt = "Tagging {version}"
+        fmt = self.config.get("tag-message", default_fmt)
         if "{version}" not in fmt:
             print("{version} needs to be part of 'tag-message': '%s'" % fmt)
             sys.exit(1)
         return fmt.format(version=version)
 
     def tag_signing(self):
         """Return whether the tag should be signed.
@@ -634,15 +654,15 @@
         converted to a boolean. Currently are accepted (case
         insensitively): 0, false, no, off for False, and 1, true, yes,
         on for True).
 
         The default when this option has not been set is False.
 
         """
-        return self._get_boolean("zest.releaser", "tag-signing", default=False)
+        return self.config.get("tag-signing", False)
 
     def date_format(self):
         """Return the string format for the date used in the changelog.
 
         Override the default ``%Y-%m-%d`` in ~/.pypirc or setup.cfg using
         a ``date-format`` option::
 
@@ -651,21 +671,17 @@
 
         Note: the % signs should be doubled for compatibility with other tools
         (i.e. pip) that parse setup.cfg using the interpolating ConfigParser.
 
         Returns default of ``%Y-%m-%d`` when nothing has been configured.
         """
         default = "%Y-%m-%d"
-        if self.config is None:
-            return default
         try:
-            result = self._get_text(
-                "zest.releaser", "date-format", default=default
-            ).replace("%%", "%")
-        except (NoSectionError, NoOptionError, ValueError):
+            result = self.config["date-format"].replace("%%", "%")
+        except (KeyError, ValueError):
             return default
         return result
 
     def run_pre_commit(self):
         """Return whether we should run pre commit hooks.
 
         At least in git you have pre commit hooks.
@@ -683,8 +699,8 @@
         converted to a boolean. Currently are accepted (case
         insensitively): 0, false, no, off for False, and 1, true, yes,
         on for True).
 
         The default when this option has not been set is False.
 
         """
-        return self._get_boolean("zest.releaser", "run-pre-commit", default=False)
+        return self.config.get("run-pre-commit", False)
```

### Comparing `zest.releaser-8.0.0a2/zest/releaser/release.py` & `zest.releaser-9.0.0a1/zest/releaser/release.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # GPL, (c) Reinout van Rees
 
+from build import ProjectBuilder
 from colorama import Fore
 from urllib import request
 from urllib.error import HTTPError
 
 import logging
 import os
 import requests
@@ -54,14 +55,27 @@
         request.urlopen(url)
         return True
     except HTTPError as e:
         logger.debug("Package not found on pypi: %s", e)
         return False
 
 
+def _project_builder_runner(cmd, cwd=None, extra_environ=None):
+    """Run the build command and format warnings and errors.
+
+    It runs the build command in a subprocess.
+    extra_environ will contain for example:
+
+    {'PEP517_BUILD_BACKEND': 'setuptools.build_meta:__legacy__'}
+    """
+    utils.show_interesting_lines(
+        execute_command(cmd, cwd=cwd, extra_environ=extra_environ)
+    )
+
+
 class Releaser(baserelease.Basereleaser):
     """Release the project by tagging it and optionally uploading to pypi."""
 
     def __init__(self, vcs=None):
         baserelease.Basereleaser.__init__(self, vcs=vcs)
         # Prepare some defaults for potential overriding.
         self.data.update(
@@ -69,18 +83,20 @@
                 # Nothing yet
             )
         )
 
     def prepare(self):
         """Collect some data needed for releasing"""
         self._grab_version()
-        tag = self.pypiconfig.tag_format(self.data["version"])
+        tag = self.zest_releaser_config.tag_format(self.data["version"])
         self.data["tag"] = tag
-        self.data["tag-message"] = self.pypiconfig.tag_message(self.data["version"])
-        self.data["tag-signing"] = self.pypiconfig.tag_signing()
+        self.data["tag-message"] = self.zest_releaser_config.tag_message(
+            self.data["version"]
+        )
+        self.data["tag-signing"] = self.zest_releaser_config.tag_signing()
         self.data["tag_already_exists"] = self.vcs.tag_exists(tag)
 
     def execute(self):
         """Do the actual releasing"""
         self._info_if_tag_already_exists()
         self._make_tag()
         self._release()
@@ -127,23 +143,22 @@
         # See if creating an sdist (and maybe a wheel) actually works.
         # Also, this makes the sdist (and wheel) available for plugins.
         # And for twine, who will just upload the created files.
         logger.info(
             "Making a source distribution of a fresh tag checkout (in %s).",
             self.data["tagworkingdir"],
         )
-        result = utils.execute_command(utils.setup_py("sdist"))
-        utils.show_interesting_lines(result)
-        if self.pypiconfig.create_wheel():
+        builder = ProjectBuilder(srcdir=".", runner=_project_builder_runner)
+        builder.build("sdist", "./dist/")
+        if self.zest_releaser_config.create_wheel():
             logger.info(
                 "Making a wheel of a fresh tag checkout (in %s).",
                 self.data["tagworkingdir"],
             )
-            result = utils.execute_command(utils.setup_py("bdist_wheel"))
-        utils.show_interesting_lines(result)
+            builder.build("wheel", "./dist/")
         if not self.pypiconfig.is_pypi_configured():
             logger.error(
                 "You must have a properly configured %s file in "
                 "your home dir to upload to a Python package index.",
                 pypi.DIST_CONFIG_FILE,
             )
             if utils.ask("Do you want to continue without uploading?", default=False):
@@ -154,15 +169,15 @@
         self._run_hooks("before_upload")
 
         # Get list of all files to upload.
         files_in_dist = sorted(
             os.path.join("dist", filename) for filename in os.listdir("dist")
         )
 
-        register = self.pypiconfig.register_package()
+        register = self.zest_releaser_config.register_package()
 
         # If TWINE_REPOSITORY_URL is set, use it.
         if self.pypiconfig.twine_repository_url():
             if not self._ask_upload(
                 package, self.pypiconfig.twine_repository_url(), register
             ):
                 return
@@ -261,21 +276,21 @@
     def _release(self):
         """Upload the release, when desired"""
         # Does the user normally want a real release?  We are
         # interested in getting a sane default answer here, so you can
         # override it in the exceptional case but just hit Enter in
         # the usual case.
         main_files = os.listdir(self.data["workingdir"])
-        if "setup.py" not in main_files and "setup.cfg" not in main_files:
-            # Neither setup.py nor setup.cfg, so this is no python
-            # package, so at least a pypi release is not useful.
+        if not {"setup.py", "setup.cfg", "pyproject.toml"}.intersection(main_files):
+            # No setup.py, setup.cfg, or pyproject.toml, so this is no
+            # python package, so at least a pypi release is not useful.
             # Expected case: this is a buildout directory.
             default_answer = False
         else:
-            default_answer = self.pypiconfig.want_release()
+            default_answer = self.zest_releaser_config.want_release()
 
         if not utils.ask(
             "Check out the tag (for tweaks or pypi/distutils " "server upload)",
             default=default_answer,
         ):
             return
 
@@ -314,15 +329,18 @@
                 # Fix the setup.cfg in the current working directory
                 # so the current release works well.
                 self.setup_cfg.fix_config()
 
         # Run extra entry point
         self._run_hooks("after_checkout")
 
-        if "setup.py" in os.listdir(self.data["tagworkingdir"]):
+        if any(
+            filename in os.listdir(self.data["tagworkingdir"])
+            for filename in ["setup.py", "pyproject.toml"]
+        ):
             self._upload_distributions(package)
 
         # Make sure we are in the expected directory again.
         os.chdir(self.vcs.workingdir)
 
 
 def datacheck(data):
```

### Comparing `zest.releaser-8.0.0a2/zest/releaser/tests/addchangelogentry.txt` & `zest.releaser-9.0.0a1/zest/releaser/tests/addchangelogentry.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/zest/releaser/tests/baserelease.txt` & `zest.releaser-9.0.0a1/zest/releaser/tests/baserelease.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 Change to a git dir:
 
     >>> gitsourcedir
     'TESTTEMP/tha.example-git'
     >>> import os
     >>> os.chdir(gitsourcedir)
 
+We need to set test mode, to avoid reading ~/.pypirc::
+
+    >>> from zest.releaser import utils
+    >>> utils.TESTMODE = True
+
 Init the Basereleaser, which is otherwise only used as a base class.
 
     >>> from zest.releaser import baserelease
     >>> base = baserelease.Basereleaser()
 
 The data dict is initialized.  And a vcs is chosen:
 
@@ -149,8 +154,8 @@
     >>> lines = ["[zest.releaser]", ""]
     >>> with open('setup.cfg', 'w') as f:
     ...     _ = f.write('\n'.join(lines))
     >>> rename_changelog("CHANGES.txt", "CHANGES.md")
     >>> base = baserelease.Basereleaser()
     >>> base._grab_history()
     >>> base.history_format
-    'md'
+    'md'
```

### Comparing `zest.releaser-8.0.0a2/zest/releaser/tests/bumpversion.txt` & `zest.releaser-9.0.0a1/zest/releaser/tests/bumpversion.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/zest/releaser/tests/choose.txt` & `zest.releaser-9.0.0a1/zest/releaser/tests/choose.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/zest/releaser/tests/fullrelease.txt` & `zest.releaser-9.0.0a1/zest/releaser/tests/fullrelease.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/zest/releaser/tests/functional-git.txt` & `zest.releaser-9.0.0a1/zest/releaser/tests/functional-git.txt`

 * *Files 5% similar despite different names*

```diff
@@ -93,16 +93,16 @@
     tag_build =
     tag_svn_revision = false
     <BLANKLINE>
     <BLANKLINE>
     Showing first few lines...
     running sdist
     running egg_info
+    creating src/tha.example.egg-info
     ...
-    creating dist
     Creating ...
     removing 'tha.example-0.1' ...
     Question: Upload to pypi (y/N)?
     Our reply: yes
     MOCK twine dispatch upload ... dist/tha.example-0.1.tar.gz
 
 There is now a tag:
@@ -119,25 +119,19 @@
     Question: Enter new development version ('.dev0' will be appended) [0.2]:
     Our reply: <ENTER>
     Checking data dict
     Question: OK to commit this (Y/n)?
     Our reply: <ENTER>
     Question: OK to push commits to the server? (Y/n)?
     Our reply: n
-
-The commit will contain an extra message with in this case a hint for
-Travis to skip the Continuous Integration build, because our pypirc
-has asked this with the extra-message option::
-
     >>> from zest.releaser import lasttaglog
     >>> lasttaglog.main()
     git log...
         Back to development: 0.2
     <BLANKLINE>
-        [ci skip]...
 
 The changelog and setup.py are at 0.2 and indicate dev mode:
 
     >>> githead('CHANGES.txt')
     Changelog of tha.example
     ========================
     <BLANKLINE>
```

### Comparing `zest.releaser-8.0.0a2/zest/releaser/tests/functional-with-hooks.txt` & `zest.releaser-9.0.0a1/zest/releaser/tests/functional-with-hooks.txt`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,20 @@
     dummy...tweak setup.cfg to enable hooks
       1 file changed, 14 insertions(+)
 
 Run the prerelease script.  Note that pyroma and check-manifest have
 hooks here so they are run too, but the order may differ.  With the
 bin/test script first pyroma is run, then check-manifest.  With tox it
 is the other way around.  So we use ellipsis for that part.
+sys.dont_write_bytecode is set to True to avoid writing .pyc files so
+that check-manifest doesn't complain about differences between the sdist
+directory and the vcs.
 
+    >>> import sys
+    >>> sys.dont_write_bytecode = True
     >>> from zest.releaser import prerelease
     >>> utils.test_answer_book.set_answers(['', '', '', '', ''])
     >>> prerelease.main()
     prereleaser_before
     ...
     Question: Enter version [0.1]:
     Our reply: <ENTER>
@@ -95,16 +100,16 @@
     <BLANKLINE>
     [zest.releaser]
     ...
     releaser_after_checkout
     Showing first few lines...
     running sdist
     running egg_info
+    creating src/tha.example.egg-info
     ...
-    creating dist
     Creating ...
     removing 'tha.example-0.1' ...
     releaser_before_upload
     Question: Upload to pypi (Y/n)?
     Our reply: y
     MOCK twine dispatch upload ... dist/tha.example-0.1.tar.gz
     releaser_after
```

### Comparing `zest.releaser-8.0.0a2/zest/releaser/tests/functional.py` & `zest.releaser-9.0.0a1/zest/releaser/tests/functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Set up functional test fixtures"""
 
-from colorama import Fore
 from io import StringIO
 from urllib import request
 from urllib.error import HTTPError
 from zest.releaser import choose
 from zest.releaser import utils
 from zest.releaser.baserelease import NOTHING_CHANGED_YET
 from zest.releaser.utils import execute_command
@@ -112,15 +111,15 @@
         {
             "tempdir": test.tempdir,
             "gitsourcedir": gitsourcedir,
             "githead": githead,
             "mock_pypi_available": test.mock_pypi_available,
             "add_changelog_entry": add_changelog_entry,
             "commit_all_changes": commit_all_changes,
-            "rename_changelog": rename_changelog
+            "rename_changelog": rename_changelog,
         }
     )
 
 
 def teardown(test):
     sys.exit = test.orig_exit
     request.urlopen = test.orig_urlopen
```

### Comparing `zest.releaser-8.0.0a2/zest/releaser/tests/git.txt` & `zest.releaser-9.0.0a1/zest/releaser/tests/git.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     >>> cmd
     ['git', 'diff']
     >>> print(execute_command(cmd))
     diff --git a/setup.py b/setup.py
     index 9c14143..54fa3b9 100644
     --- a/setup.py
     +++ b/setup.py
-    @@ -42,3 +42,5 @@ setup(name='tha.example',
+    @@ -41,3 +41,5 @@ setup(name='tha.example',
                'console_scripts': [
                ]},
            )
     +
     +a = 2
 
 Commit it:
@@ -113,15 +113,15 @@
     >>> cmd
     ['git', 'diff', '0.1']
     >>> print(execute_command(cmd))
     diff --git a/setup.py b/setup.py
     index 9c14143..54fa3b9 100644
     --- a/setup.py
     +++ b/setup.py
-    @@ -44,3 +44,5 @@ setup(name='tha.example',
+    @@ -43,3 +43,5 @@ setup(name='tha.example',
            )
     <BLANKLINE>
      a = 2
     +
     +b = 3
```

### Comparing `zest.releaser-8.0.0a2/zest/releaser/tests/postrelease.txt` & `zest.releaser-9.0.0a1/zest/releaser/tests/postrelease.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/zest/releaser/tests/preparedocs.txt` & `zest.releaser-9.0.0a1/zest/releaser/tests/preparedocs.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/zest/releaser/tests/prerelease.txt` & `zest.releaser-9.0.0a1/zest/releaser/tests/prerelease.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/zest/releaser/tests/pypi.txt` & `zest.releaser-9.0.0a1/zest/releaser/tests/pypi.txt`

 * *Files 17% similar despite different names*

```diff
@@ -17,31 +17,27 @@
     '.pypirc'
 
 This is the default.  For testing purposes, you *can* pass in a config file's
 name yourself.  We'll do that in the rest of these tests.
 
 A missing file doesn't lead to an error:
 
-    >>> pypiconfig = pypi.PypiConfig(config_filename='non/existing', use_setup_cfg=False)
+    >>> pypiconfig = pypi.PypiConfig(config_filename='non/existing')
     >>> pypiconfig.config is None
     True
 
 There are two styles of ``.pypirc`` files.  The old one just for pypi:
 
     >>> pypirc_old = pkg_resources.resource_filename(
     ...     'zest.releaser.tests', 'pypirc_old.txt')
     >>> with open(pypirc_old) as pypifile:
     ...    print(pypifile.read())
     [server-login]
     username:pipo_de_clown
     password:asjemenou
-    <BLANKLINE>
-    [zest.releaser]
-    extra-message = [ci skip]
-    prefix-message = [TAG]
     >>> pypiconfig = pypi.PypiConfig(config_filename=pypirc_old)
     >>> pypiconfig.distutils_servers()
     ['pypi']
 
 And the new format that allows multiple uploads:
 
     >>> pypirc_new = pkg_resources.resource_filename(
@@ -63,18 +59,14 @@
     username:ploneuser
     password:password
     <BLANKLINE>
     [mycompany]
     repository:http://my.company/products
     username:user
     password:password
-    <BLANKLINE>
-    [zest.releaser]
-    extra-message = [ci skip]
-    prefix-message = [TAG]
     >>> pypiconfig = pypi.PypiConfig(config_filename=pypirc_new)
     >>> from pprint import pprint
     >>> pprint(sorted(pypiconfig.distutils_servers()))
     ['mycompany', 'plone.org', 'pypi']
 
 A file with both is also possible.  The old server-login section is
 used to contain the username and password that are shared among
@@ -123,36 +115,35 @@
 
 Some people hardly ever want to make a full release of a package to
 pypi; a git tag may be enough.  They can tell zest.releaser to
 use a different default answer when it asks to make a checkout for a
 release.  This means you can usually just press Enter on all questions
 that zest.releaser asks.
 
-We try to read a [zest.releaser] section, either in pypirc or
-setup.cfg and look  for a ``release`` option.  We can
-ask for the result like this, which by default is True:
+We try to read a [zest.releaser] section and look  for a ``release``
+option.  We can ask for the result like this, which by default is True:
 
-    >>> pypiconfig = pypi.PypiConfig(config_filename=pypirc_both)
-    >>> pypiconfig.want_release()
+    >>> zestreleaserconfig = pypi.ZestReleaserConfig(pypirc_config_filename=pypirc_both)
+    >>> zestreleaserconfig.want_release()
     True
 
 We have a pypirc for this:
 
     >>> pypirc_no_release = pkg_resources.resource_filename(
     ...     'zest.releaser.tests', 'pypirc_no_release.txt')
-    >>> pypiconfig = pypi.PypiConfig(config_filename=pypirc_no_release)
-    >>> pypiconfig.want_release()
+    >>> zestreleaserconfig = pypi.ZestReleaserConfig(pypirc_config_filename=pypirc_no_release)
+    >>> zestreleaserconfig.want_release()
     False
 
 We can also specify to always do that checkout during a release:
 
     >>> pypirc_yes_release = pkg_resources.resource_filename(
     ...     'zest.releaser.tests', 'pypirc_yes_release.txt')
-    >>> pypiconfig = pypi.PypiConfig(config_filename=pypirc_yes_release)
-    >>> pypiconfig.want_release()
+    >>> zestreleaserconfig = pypi.ZestReleaserConfig(pypirc_config_filename=pypirc_yes_release)
+    >>> zestreleaserconfig.want_release()
     True
 
 
 Creating a wheel
 ----------------
 
 When the ``wheel`` package is installed, we could create shiny new
@@ -161,32 +152,32 @@
 
 If the package is installed, we set a constant:
 
     >>> from zest.releaser.pypi import USE_WHEEL
     >>> USE_WHEEL
     True
 
-We try to read a [zest.releaser] section, either in pypirc or
-setup.cfg and check for a ``create-wheel`` option.  In this case we
-explicitly disable checking for a setup.cfg, because when running the
+We try to read a [zest.releaser] section, in pypirc, setup.cfg or
+pyproject.toml and check for a ``create-wheel`` option.  In this case we
+explicitly disable checking for the files in the package, because when running the
 tests with ``tox`` the current directory is the base directory of
 zest.releaser, which now contains a setup.cfg.
 
 We can ask for the result like this, which by default is True:
 
-    >>> pypiconfig = pypi.PypiConfig(config_filename=pypirc_both, use_setup_cfg=False)
-    >>> pypiconfig.create_wheel()
+    >>> zestreleaserconfig = pypi.ZestReleaserConfig(pypirc_config_filename=pypirc_both, omit_package_config_in_test=True)
+    >>> zestreleaserconfig.create_wheel()
     True
 
 We can also specify to not create the wheel, even when (universal) wheels could be created:
 
-    >>> pypirc_yes_release = pkg_resources.resource_filename(
+    >>> pypirc_no_create = pkg_resources.resource_filename(
     ...     'zest.releaser.tests', 'pypirc_universal_nocreate.txt')
-    >>> pypiconfig = pypi.PypiConfig(config_filename=pypirc_yes_release, use_setup_cfg=False)
-    >>> pypiconfig.create_wheel()
+    >>> zestreleaserconfig = pypi.ZestReleaserConfig(pypirc_config_filename=pypirc_no_create, omit_package_config_in_test=True)
+    >>> zestreleaserconfig.create_wheel()
     False
 
 Fixing setup.cfg
 ----------------
 
 A setup.cfg file can be used to influence the release process.  This
 may contain options that are not advisable in the released package but
@@ -270,41 +261,41 @@
 ``zest.releaser`` by default tags releases in the project version control. The
 format of the tag name can be customized by the ``tag-format`` setting.
 
 By default the tag format is just the version itself:
 
     >>> version = '1.2.3'
     >>> os.remove(pypi.SETUP_CONFIG_FILE)
-    >>> pypiconfig = pypi.PypiConfig()
-    >>> pypiconfig.tag_format(version)
+    >>> zestreleaserconfig = pypi.ZestReleaserConfig()
+    >>> zestreleaserconfig.tag_format(version)
     '1.2.3'
 
 But it can be customized with a format string, as long as it contains
 the string ``{version}``:
 
     >>> SETUP_CFG = """
     ... [zest.releaser]
     ... tag-format = mytag-{version}
     ... """
     >>> with open(pypi.SETUP_CONFIG_FILE, 'w') as f:
     ...     _ = f.write(SETUP_CFG)
-    >>> pypiconfig = pypi.PypiConfig()
-    >>> pypiconfig.tag_format(version)
+    >>> zestreleaserconfig = pypi.ZestReleaserConfig()
+    >>> zestreleaserconfig.tag_format(version)
     'mytag-1.2.3'
 
 Or, for backward compatibility, a Python % interpolation format:
 
     >>> SETUP_CFG = """
     ... [zest.releaser]
     ... tag-format = yourtag-%(version)s
     ... """
     >>> with open(pypi.SETUP_CONFIG_FILE, 'w') as f:
     ...     _ = f.write(SETUP_CFG)
-    >>> pypiconfig = pypi.PypiConfig()
-    >>> pypiconfig.tag_format(version)
+    >>> zestreleaserconfig = pypi.ZestReleaserConfig()
+    >>> zestreleaserconfig.tag_format(version)
     `tag-format` contains deprecated `%(version)s` format. Please change to:
     <BLANKLINE>
     [zest.releaser]
     tag-format = yourtag-{version}
     'yourtag-1.2.3'
 
 
@@ -319,88 +310,88 @@
 The commit message to be used when tagging can be customized by the
 ``tag-message`` setting.
 
 By default the tag message is ``Tagging`` plus the version:
 
     >>> version = '1.2.3'
     >>> os.remove(pypi.SETUP_CONFIG_FILE)
-    >>> pypiconfig = pypi.PypiConfig()
-    >>> pypiconfig.tag_message(version)
+    >>> zestreleaserconfig = pypi.ZestReleaserConfig()
+    >>> zestreleaserconfig.tag_message(version)
     'Tagging 1.2.3'
 
 But it can be customized with a message string, as long as it contains
 the string ``{version}``:
 
     >>> SETUP_CFG = """
     ... [zest.releaser]
     ... tag-message = Creating v{version} tag.
     ... """
     >>> with open(pypi.SETUP_CONFIG_FILE, 'w') as f:
     ...     _ = f.write(SETUP_CFG)
-    >>> pypiconfig = pypi.PypiConfig()
-    >>> pypiconfig.tag_message(version)
+    >>> zestreleaserconfig = pypi.ZestReleaserConfig()
+    >>> zestreleaserconfig.tag_message(version)
     'Creating v1.2.3 tag.'
 
 
 No-input mode
 -------------
 
 In some cases you want no questions asked. Zest.releaser should just do its
 job without asking for versions or confirmations. You can enable this
 behaviour with a ``--no-input`` commandline option, but also by adding
 ``no-input = yes`` to the ``[zest.releaser]`` section in ``.pypirc`` or
 ``setup.cfg``.
 
 The default is False:
 
-    >>> pypiconfig = pypi.PypiConfig(config_filename=pypirc_yes_release, use_setup_cfg=False)
-    >>> pypiconfig.no_input()
+    >>> zestreleaserconfig = pypi.ZestReleaserConfig(pypirc_config_filename=pypirc_yes_release)
+    >>> zestreleaserconfig.no_input()
     False
 
 Enable the option in ``.pypirc``:
 
     >>> pypirc_no_input = pkg_resources.resource_filename(
     ...     'zest.releaser.tests', 'pypirc_no_input.txt')
-    >>> pypiconfig = pypi.PypiConfig(config_filename=pypirc_no_input)
+    >>> zestreleaserconfig = pypi.ZestReleaserConfig(pypirc_config_filename=pypirc_no_input)
 
 Now the option should be set to True:
 
-    >>> pypiconfig.no_input()
+    >>> zestreleaserconfig.no_input()
     True
 
 Let's enable the option also in setup.cfg:
 
     >>> SETUP_CFG = """
     ... [zest.releaser]
     ... no-input = yes
     ... """
     >>> with open(pypi.SETUP_CONFIG_FILE, 'w') as f:
     ...     _ = f.write(SETUP_CFG)
-    >>> pypiconfig = pypi.PypiConfig()
+    >>> zestreleaserconfig = pypi.ZestReleaserConfig()
 
 The option should be set to True here as well:
 
-    >>> pypiconfig.no_input()
+    >>> zestreleaserconfig.no_input()
     True
 
 
 Python version file pointer
 ---------------------------
 
 In some cases you want to point at a Python file with a ``__version__`` marker
 in it. For that, there's the ``python-file-with-version`` option.
 
 The default is None:
 
-    >>> setup_config.python_file_with_version()
+    >>> zestreleaserconfig.python_file_with_version()
 
 Enable the option:
 
     >>> SETUP_CFG = """
     ... [zest.releaser]
     ... python-file-with-version = reinout/maurits.py
     ... """
     >>> with open(pypi.SETUP_CONFIG_FILE, 'w') as f:
     ...    _ = f.write(SETUP_CFG)
-    >>> setup_config = pypi.SetupConfig()
-    >>> setup_config.python_file_with_version()
+    >>> zestreleaserconfig = pypi.ZestReleaserConfig()
+    >>> zestreleaserconfig.python_file_with_version()
     'reinout/maurits.py'
```

### Comparing `zest.releaser-8.0.0a2/zest/releaser/tests/pyproject-toml.txt` & `zest.releaser-9.0.0a1/zest/releaser/tests/pyproject-toml.txt`

 * *Files 6% similar despite different names*

```diff
@@ -84,28 +84,31 @@
     Checking data dict
     Tag needed to proceed, you can use the following command:
     git tag 0.1 -m 'Tagging 0.1'
     Question: Run this command (Y/n)?
     Our reply: y
     <BLANKLINE>
     Question: Check out the tag
-        (for tweaks or pypi/distutils server upload) (y/N)?
+        (for tweaks or pypi/distutils server upload) (Y/n)?
     Our reply: y
     RED Note: ...0.1...
     ...
     RED HEAD is now at ...
     Preparing release 0.1
     <BLANKLINE>
-
-TODO No source distribution or wheel is generated yet!!!!!
-This currently only happens when you have a setup.py.
-One related small thing is that for the question "Check out the tag"
-the default answer is No, instead of Yes.
-So there is much more to do.
-But writing pyproject.toml has worked, which is a start.
+    Showing first few lines...
+    running sdist
+    running egg_info
+    creating src/tha.example.egg-info
+    ...
+    Creating ...
+    removing 'tha.example-0.1' ...
+    Question: Upload to pypi (y/N)?
+    Our reply: yes
+    MOCK twine dispatch upload ... dist/tha.example-0.1.tar.gz
 
 There is now a tag:
 
     >>> print(execute_command(["git", "tag"]))
     0.1
 
 And the postrelease script ups the version:
```

### Comparing `zest.releaser-8.0.0a2/zest/releaser/tests/release.txt` & `zest.releaser-9.0.0a1/zest/releaser/tests/release.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/zest/releaser/tests/test_setup.py` & `zest.releaser-9.0.0a1/zest/releaser/tests/test_setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,22 +43,22 @@
         (re.compile(re.escape(tempfile.gettempdir())), "TMPDIR"),
         # Change in git 2.9.1:
         (
             re.compile(r"nothing to commit, working directory clean"),
             "nothing to commit, working tree clean",
         ),
         # We should ignore coloring by colorama.  Or actually print it
-        # clearly.  This catches Fore.RED and Fore.MAGENTA.
+        # clearly.  This catches Fore.RED, Fore.MAGENTA and Fore.RESET.
         (re.compile(re.escape(Fore.RED)), "RED "),
         (re.compile(re.escape(Fore.MAGENTA)), "MAGENTA "),
+        (re.compile(re.escape(Fore.RESET)), "RESET "),
     ]
 )
 
 
-
 def test_suite():
     """Find .txt files and test code examples in them."""
     suite = unittest.TestSuite()
 
     # These are simple tests without setup.
     simple = [
         "preparedocs.txt",
```

### Comparing `zest.releaser-8.0.0a2/zest/releaser/tests/utils.txt` & `zest.releaser-9.0.0a1/zest/releaser/tests/utils.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/zest/releaser/tests/vcs.txt` & `zest.releaser-9.0.0a1/zest/releaser/tests/vcs.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-8.0.0a2/zest/releaser/utils.py` & `zest.releaser-9.0.0a1/zest/releaser/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,17 @@
         )
         with open(filename, "rb", encoding=encoding) as filehandler:
             data = filehandler.read()
         return splitlines_with_trailing(data), encoding
 
     if fallback_encoding:
         logger.debug(
-            "Decoding file %s from encoding %s from setup.cfg.", filename, fallback_encoding
+            "Decoding file %s from encoding %s from setup.cfg.",
+            filename,
+            fallback_encoding,
         )
         try:
             with open(filename, "rb", encoding=fallback_encoding) as filehandler:
                 data = filehandler.read()
             return splitlines_with_trailing(data), fallback_encoding
         except UnicodeDecodeError:
             logger.warning(
@@ -96,17 +98,15 @@
 
     # tokenize first detects the encoding (looking for encoding hints
     # or an UTF-8 BOM) and opens the file using this encoding.
     # See https://docs.python.org/3/library/tokenize.html
     with tokenize.open(filename) as filehandler:
         data = filehandler.read()
         encoding = filehandler.encoding
-        logger.debug(
-            "Detected encoding of %s with tokenize: %s", filename, encoding
-        )
+        logger.debug("Detected encoding of %s with tokenize: %s", filename, encoding)
     return splitlines_with_trailing(data), encoding
 
 
 def strip_version(version):
     """Strip the version of all whitespace."""
     return version.strip().replace(" ", "")
 
@@ -286,15 +286,15 @@
             answers = []
         self.answers = answers
 
     def get_next_answer(self):
         if self.answers:
             return self.answers.pop(0)
         # Accept the default.
-        return ''
+        return ""
 
 
 test_answer_book = AnswerBook()
 
 
 def get_input(question):
     if not TESTMODE:
@@ -470,15 +470,15 @@
     But: when there are errors or warnings, print everything and ask
     the user if she wants to continue.
     """
     if Fore.RED in result:
         # warnings/errors, print complete result.
         print(result)
         if not ask(
-            "There were errors or warnings. Are you sure " "you want to continue?",
+            "There were errors or warnings. Are you sure you want to continue?",
             default=False,
         ):
             sys.exit(1)
         # User has seen everything and wants to continue.
         return
 
     # No errors or warnings.  Show first and last lines.
@@ -557,48 +557,53 @@
             ret = getattr(ret, part)
         except AttributeError:
             raise ImportError(part)
 
     return ret
 
 
-def run_hooks(setup_cfg, which_releaser, when, data):
+def run_hooks(zest_releaser_config, which_releaser, when, data):
     """Run all release hooks for the given release step, including
     project-specific hooks from setup.cfg, and globally installed entry-points.
 
     which_releaser can be prereleaser, releaser, postreleaser.
 
     when can be before, middle, after.
 
     """
     hook_group = f"{which_releaser}.{when}"
-    config = setup_cfg.config
+    config = zest_releaser_config.config
 
-    if config is not None and config.has_option("zest.releaser", hook_group):
-        # Multiple hooks may be specified, each one separated by whitespace
+    if config is not None and config.get(hook_group):
+        # Multiple hooks may be specified
+        # in setup.cfg or .pypirc each one is separated by whitespace
         # (including newlines)
-        hook_names = config.get("zest.releaser", hook_group).split()
+        if zest_releaser_config.hooks_filename in ["setup.py", "setup.cfg", ".pypirc"]:
+            hook_names = config.get(hook_group).split()
+        # in pyproject.toml, a list is passed with the hooks
+        elif zest_releaser_config.hooks_filename == "pyproject.toml":
+            hook_names = config.get(hook_group)
+        else:
+            hook_names = []
         hooks = []
 
         # The following code is adapted from the 'packaging' package being
         # developed for Python's stdlib:
 
         # add project directory to sys.path, to allow hooks to be
         # distributed with the project
         # an optional package_dir option adds support for source layouts where
         # Python packages are not directly in the root of the source
-        config_dir = os.path.dirname(setup_cfg.config_filename)
-        sys.path.insert(0, os.path.dirname(setup_cfg.config_filename))
+        config_dir = os.path.dirname(zest_releaser_config.hooks_filename)
+        sys.path.insert(0, os.path.dirname(zest_releaser_config.hooks_filename))
 
-        if config.has_option("zest.releaser", "hook_package_dir"):
-            package_dir = config.get("zest.releaser", "hook_package_dir")
+        package_dir = config.get("hook_package_dir")
+        if package_dir:
             package_dir = os.path.join(config_dir, package_dir)
             sys.path.insert(0, package_dir)
-        else:
-            package_dir = None
 
         try:
             for hook_name in hook_names:
                 # Resolve the hook or fail with ImportError.
                 hooks.append(resolve_name(hook_name))
 
             for hook in hooks:
@@ -653,40 +658,42 @@
     Do NOT pass this to subprocess.popen/run.
     See also: https://docs.python.org/3/library/shlex.html#shlex.quote
     """
     args = [shlex.quote(arg) for arg in command]
     return " ".join(args)
 
 
-def _execute_command(command):
+def _execute_command(command, cwd=None, extra_environ=None):
     """Execute a command, returning stdout, plus maybe parts of stderr."""
     # Enforce the command to be a list or arguments.
     assert isinstance(command, (list, tuple))
     logger.debug("Running command: '%s'", format_command(command))
+    env = dict(os.environ, PYTHONPATH=os.pathsep.join(sys.path))
+    if extra_environ is not None:
+        env.update(extra_environ)
+    # By default we show errors, of course.
+    show_stderr = True
     if command[0].startswith(sys.executable):
-        env = dict(os.environ, PYTHONPATH=os.pathsep.join(sys.path))
-        if "upload" in command or "register" in command:
-            # We really do want to see the stderr here, otherwise a
-            # failed upload does not even show up in the output.
-            show_stderr = True
-        else:
-            show_stderr = False
-    else:
-        env = None
-        show_stderr = True
+        # For several Python commands, we do not want to see the stderr:
+        # if we include it for `python setup.py --version`, then the version
+        # may contain all kinds of warnings.
+        show_stderr = False
+        # But we really DO want to see the stderr for some other Python commands,
+        # otherwise for example a failed upload would not even show up in the output.
+        for flag in ("upload", "register", "build_sdist", "build_wheel", "-mbuild"):
+            if flag in command:
+                show_stderr = True
+                break
     process_kwargs = {
         "stdin": subprocess.PIPE,
         "stdout": subprocess.PIPE,
         "stderr": subprocess.PIPE,
+        "cwd": cwd,
         "env": env,
-        # With Python 3.7+ we could use the more understandable 'text' alias
-        # instead of the cryptic 'universal_newlines'.
-        # They do the same: open a file (stdin/out/err) in text mode
-        # instead of binary.  Core Python is better at knowing which encoding to use.
-        "universal_newlines": True,
+        "text": True,
     }
     process = subprocess.run(command, **process_kwargs)
     if process.returncode or show_stderr or "Traceback" in process.stderr:
         # Some error occurred
         return process.stdout + get_errors(process.stderr)
     # Only return the stdout. Stderr only contains possible
     # weird/confusing warnings that might trip up extraction of version
@@ -726,15 +733,17 @@
                 break
         else:
             # Not found in known warnings, so mark it as an error.
             errors.append(Fore.RED + line)
     return "\n".join(errors)
 
 
-def execute_command(command, allow_retry=False, fail_message=""):
+def execute_command(
+    command, allow_retry=False, fail_message="", cwd=None, extra_environ=None
+):
     """Run the command and possibly retry it.
 
     When allow_retry is False, we simply call the base
     _execute_command and return the result.
 
     When allow_retry is True, a few things change.
 
@@ -747,15 +756,15 @@
     - Retry
     - Continue
 
     There is an error when there is a red color in the output.
 
     It might be a warning, but we cannot detect the distinction.
     """
-    result = _execute_command(command)
+    result = _execute_command(command, cwd=cwd, extra_environ=extra_environ)
     if not allow_retry:
         return result
     if Fore.RED not in result:
         show_interesting_lines(result)
         return result
     # There are warnings or errors. Print the complete result.
     print(result)
@@ -974,7 +983,50 @@
     default = "rst"
     history_format = config_value
     if not history_format:
         history_file = history_file or ""
         ext = history_file.split(".")[-1].lower()
         history_format = "md" if ext in ["md", "markdown"] else default
     return history_format
+
+
+def string_to_bool(value):
+    """Reimplementation of configparser.ConfigParser.getboolean()"""
+    if value.isalpha():
+        value = value.lower()
+    if value in ["1", "yes", "true", "on"]:
+        return True
+    elif value in ["0", "no", "false", "off"]:
+        return False
+    else:
+        raise ValueError(f"Cannot convert string '{value}' to a bool")
+
+
+def extract_zestreleaser_configparser(config, config_filename):
+    if not config:
+        return None
+
+    try:
+        result = dict(config["zest.releaser"].items())
+    except KeyError:
+        logger.debug(f"No [zest.releaser] section found in the {config_filename}")
+        return None
+
+    boolean_keys = [
+        "release",
+        "create-wheel",
+        "no-input",
+        "register",
+        "push-changes",
+        "less-zeroes",
+        "tag-signing",
+        "run-pre-commit",
+    ]
+    integer_keys = [
+        "version-levels",
+    ]
+    for key, value in result.items():
+        if key in boolean_keys:
+            result[key] = string_to_bool(value)
+        if key in integer_keys:
+            result[key] = int(value)
+    return result
```

### Comparing `zest.releaser-8.0.0a2/zest/releaser/vcs.py` & `zest.releaser-9.0.0a1/zest/releaser/vcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+from configparser import ConfigParser
 from zest.releaser import pypi
 from zest.releaser import utils
 
 import logging
 import os
+import pkg_resources
 import re
 import sys
 
+
 try:
     # Python 3.11+
     import tomllib
 except ImportError:
     # Python 3.10-
     import tomli as tomllib
 
@@ -60,17 +63,24 @@
         if reporoot is None:
             self.reporoot = self.workingdir
             self.relative_path_in_repo = ""
         else:
             self.reporoot = reporoot
             # Determine relative path from root of repo.
             self.relative_path_in_repo = os.path.relpath(self.workingdir, reporoot)
-        self.setup_cfg = pypi.SetupConfig()
-        self.pypi_cfg = pypi.PypiConfig()
-        self.fallback_encoding = self.pypi_cfg.encoding()
+        if utils.TESTMODE:
+            pypirc_old = pkg_resources.resource_filename(
+                "zest.releaser.tests", "pypirc_old.txt"
+            )
+            self.zest_releaser_config = pypi.ZestReleaserConfig(
+                pypirc_config_filename=pypirc_old
+            )
+        else:
+            self.zest_releaser_config = pypi.ZestReleaserConfig()
+        self.fallback_encoding = self.zest_releaser_config.encoding()
 
     def __repr__(self):
         return "<{} at {} {}>".format(
             self.__class__.__name__, self.reporoot, self.relative_path_in_repo
         )
 
     def is_setuptools_helper_package_installed(self):
@@ -100,26 +110,35 @@
         if os.path.exists("setup.py"):
             # First run egg_info, as that may get rid of some warnings
             # that otherwise end up in the extracted name, like
             # UserWarnings.
             utils.execute_command(utils.setup_py("egg_info"))
             return utils.execute_command(utils.setup_py("--name")).strip()
 
+    def get_setup_cfg_name(self):
+        if os.path.exists("setup.cfg"):
+            setup_cfg = ConfigParser()
+            setup_cfg.read("setup.cfg")
+            try:
+                return setup_cfg["metadata"]["name"]
+            except KeyError:
+                return None
+
     def get_version_txt_version(self):
         filenames = ["version"]
         for extension in TXT_EXTENSIONS:
             filenames.append(".".join(["version", extension]))
         version_file = self.filefind(filenames)
         if version_file:
             with open(version_file) as f:
                 version = f.read()
             return utils.strip_version(version)
 
     def get_python_file_version(self):
-        python_version_file = self.setup_cfg.python_file_with_version()
+        python_version_file = self.zest_releaser_config.python_file_with_version()
         if not python_version_file:
             return
         lines, encoding = utils.read_text_file(
             python_version_file,
             fallback_encoding=self.fallback_encoding,
         )
         encoding  # noqa, unused variable
@@ -136,14 +155,22 @@
         if not os.path.exists("pyproject.toml"):
             return
         with open("pyproject.toml", "rb") as myfile:
             result = tomllib.load(myfile)
         # Might be None, but that is fine.
         return result.get("project", {}).get("version")
 
+    def get_pyproject_toml_name(self):
+        if not os.path.exists("pyproject.toml"):
+            return
+        with open("pyproject.toml", "rb") as myfile:
+            result = tomllib.load(myfile)
+        # Might be None, but that is fine.
+        return result.get("project", {}).get("name")
+
     def filefind(self, names):
         """Return first found file matching name (case-insensitive).
 
         Some packages have docs/HISTORY.txt and
         package/name/HISTORY.txt.  We make sure we only return the one
         in the docs directory if no other can be found.
 
@@ -228,16 +255,24 @@
         return (
             self.get_python_file_version()
             or self.get_pyproject_toml_version()
             or self.get_setup_py_version()
             or self.get_version_txt_version()
         )
 
+    def _extract_name(self):
+        """Extract the package name from setup.py or pyproject.toml or similar."""
+        return (
+            self.get_setup_py_name()
+            or self.get_setup_cfg_name()
+            or self.get_pyproject_toml_name()
+        )
+
     def _update_python_file_version(self, version):
-        filename = self.setup_cfg.python_file_with_version()
+        filename = self.zest_releaser_config.python_file_with_version()
         lines, encoding = utils.read_text_file(
             filename,
             fallback_encoding=self.fallback_encoding,
         )
         good_version = "__version__ = '%s'" % version
         for index, line in enumerate(lines):
             if UNDERSCORED_VERSION_PATTERN.search(line):
```

### Comparing `zest.releaser-8.0.0a2/zest.releaser.egg-info/PKG-INFO` & `zest.releaser-9.0.0a1/zest.releaser.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: zest.releaser
-Version: 8.0.0a2
+Version: 9.0.0a1
 Summary: Software releasing made easy and repeatable
 Author-email: Reinout van Rees <reinout@vanrees.org>, Maurits van Rees <maurits@vanrees.org>
 License: GPL
 Project-URL: documentation, https://zestreleaser.readthedocs.io
 Project-URL: repository, https://github.com/zestsoftware/zest.releaser/
 Project-URL: changelog, https://github.com/zestsoftware/zest.releaser/blob/master/CHANGES.rst
 Keywords: releasing,packaging,pypi
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: recommended
 Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 
 Package releasing made easy: zest.releaser overview and installation
 ====================================================================
@@ -71,15 +70,15 @@
 
 Compatibility / Dependencies
 ----------------------------
 
 .. image:: https://img.shields.io/pypi/pyversions/zest.releaser?   :alt: PyPI - Python Version
 .. image:: https://img.shields.io/pypi/implementation/zest.releaser?   :alt: PyPI - Implementation
 
-``zest.releaser`` works on Python 3.7+, including PyPy3.
+``zest.releaser`` works on Python 3.8+, including PyPy3.
 Tested until Python 3.11, but see ``tox.ini`` for the canonical place for that.
 
 To be sure: the packages that you release with ``zest.releaser`` may
 very well work on other Python versions: that totally depends on your
 package.
 
 We depend on:
@@ -93,26 +92,21 @@
 
 Since version 4.0 there is a ``recommended`` extra that you can get by
 installing ``zest.releaser[recommended]`` instead of ``zest.releaser``.  It
 contains a few trusted add-ons that we feel are useful for the great majority
 of ``zest.releaser`` users:
 
 - wheel_ for creating a Python wheel that we upload to PyPI next to
-  the standard source distribution.  Wheels are the new Python package
-  format.  Create or edit ``setup.cfg`` in your project (or globally
-  in your ``~/.pypirc``) and create a section ``[zest.releaser]`` with
-  ``create-wheel = yes`` to create a wheel to upload to PyPI.  See
-  http://pythonwheels.com for deciding whether this is a good idea for
-  your package.  Briefly, if it is a pure Python 2 *or* pure Python 3
-  package: just do it. If it is a pure Python 2 *and* a pure Python 3
-  project, it is known as a "universal" wheel, because one wheel can
-  be installed on all implementations and versions of Python. If you
-  indicate this in ``setup.cfg`` with the section ``[bdist_wheel]``
-  having ``universal = 1``, then we will automatically upload a wheel,
-  unless ``create-wheel`` is explicitly set to false.
+  the standard source distribution.  Wheels are the official binary
+  distribution format for Python.
+  Since version 8.0.0a2 we always create wheels, except when you
+  explicitly switch this off in the config:
+  ``create-wheel = false``.
+  If you are sure you want "universal" wheels, follow the directions from the
+  `wheel documentation <https://wheel.readthedocs.io/en/stable/user_guide.html>`_.
 
 - `check-manifest`_ checks your ``MANIFEST.in`` file for completeness,
   or tells you that you need such a file.  It basically checks if all
   version controlled files are ending up the the distribution that we
   will upload.  This may avoid 'brown bag' releases that are missing
   files.
 
@@ -248,14 +242,37 @@
 
 * `Mateusz Legięcki <https://github.com/Behoston>`_ added a dockerfile for
   much easier testing.
 
 Changelog for zest.releaser
 ===========================
 
+9.0.0a1 (2023-07-13)
+--------------------
+
+- Changed build system to pypa/build instead of explicitly using
+  setuptools.
+
+- Zest.releaser's settings can now also be placed in ``pyproject.toml``.
+
+- Use native namespace packages for ``zest.releaser``, instead of
+  deprecated ``pkg_resources`` based ones.
+
+- Added pre-commit config for neater code (black, flake8, isort).
+
+- Dropped support for python 3.7. Together with switching to ``build`` and
+  ``pyproject.toml``, this warrants a major version bump.
+
+
+8.0.0 (2023-05-05)
+------------------
+
+- Make final release, no changes since latest alpha.  [maurits]
+
+
 8.0.0a2 (2023-04-06)
 --------------------
 
 - Always create wheels, except when you explicitly switch this off in the config:
   ``[zest.releaser] create-wheel = no``.
   If the ``wheel`` package is not available, we still do not create wheels.
   Fixes `issue 406 <https://github.com/zestsoftware/zest.releaser/issues/406>`_.
```

### Comparing `zest.releaser-8.0.0a2/zest.releaser.egg-info/SOURCES.txt` & `zest.releaser-9.0.0a1/zest.releaser.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -18,20 +18,18 @@
 doc/source/further_reading.rst
 doc/source/index.rst
 doc/source/options.rst
 doc/source/overview.rst
 doc/source/project.rst
 doc/source/uploading.rst
 doc/source/versions.rst
-zest/__init__.py
 zest.releaser.egg-info/PKG-INFO
 zest.releaser.egg-info/SOURCES.txt
 zest.releaser.egg-info/dependency_links.txt
 zest.releaser.egg-info/entry_points.txt
-zest.releaser.egg-info/namespace_packages.txt
 zest.releaser.egg-info/not-zip-safe
 zest.releaser.egg-info/requires.txt
 zest.releaser.egg-info/top_level.txt
 zest/releaser/__init__.py
 zest/releaser/addchangelogentry.py
 zest/releaser/baserelease.py
 zest/releaser/bumpversion.py
```

### Comparing `zest.releaser-8.0.0a2/zest.releaser.egg-info/entry_points.txt` & `zest.releaser-9.0.0a1/zest.releaser.egg-info/entry_points.txt`

 * *Files identical despite different names*

