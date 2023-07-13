# Comparing `tmp/specfile-0.9.0.tar.gz` & `tmp/specfile-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specfile-0.9.0.tar", last modified: Tue Oct 25 17:06:48 2022, max compression
+gzip compressed data, was "specfile-0.9.1.tar", last modified: Sat Nov 12 14:35:18 2022, max compression
```

## Comparing `specfile-0.9.0.tar` & `specfile-0.9.1.tar`

### file list

```diff
@@ -1,147 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.976166 specfile-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.968166 specfile-0.9.0/.fmf/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-10-25 17:06:38.000000 specfile-0.9.0/.fmf/version
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-25 17:06:38.000000 specfile-0.9.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-10-25 17:06:38.000000 specfile-0.9.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.964166 specfile-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.968166 specfile-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-10-25 17:06:38.000000 specfile-0.9.0/.github/workflows/do-release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-10-25 17:06:38.000000 specfile-0.9.0/.github/workflows/opened-issues-to-the-board.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-10-25 17:06:38.000000 specfile-0.9.0/.github/workflows/prepare-release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-10-25 17:06:38.000000 specfile-0.9.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4967 2022-10-25 17:06:38.000000 specfile-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2718 2022-10-25 17:06:38.000000 specfile-0.9.0/.packit.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1720 2022-10-25 17:06:38.000000 specfile-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-10-25 17:06:38.000000 specfile-0.9.0/.zuul.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3130 2022-10-25 17:06:38.000000 specfile-0.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-10-25 17:06:38.000000 specfile-0.9.0/Containerfile.tests
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-10-25 17:06:38.000000 specfile-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-10-25 17:06:38.000000 specfile-0.9.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     8640 2022-10-25 17:06:48.976166 specfile-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7671 2022-10-25 17:06:38.000000 specfile-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.968166 specfile-0.9.0/fedora/
--rw-r--r--   0 runner    (1001) docker     (121)     2223 2022-10-25 17:06:38.000000 specfile-0.9.0/fedora/python-specfile.spec
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.968166 specfile-0.9.0/files/
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-10-25 17:06:38.000000 specfile-0.9.0/files/install-requirements-pip.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-10-25 17:06:38.000000 specfile-0.9.0/files/install-requirements-rpms.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-10-25 17:06:38.000000 specfile-0.9.0/files/local-tests-requirements.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.968166 specfile-0.9.0/files/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-10-25 17:06:38.000000 specfile-0.9.0/files/tasks/build-rpm-deps.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-10-25 17:06:38.000000 specfile-0.9.0/files/tasks/generic-dnf-requirements.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-10-25 17:06:38.000000 specfile-0.9.0/files/tasks/project-dir.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-10-25 17:06:38.000000 specfile-0.9.0/files/tasks/rpm-deps.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-10-25 17:06:38.000000 specfile-0.9.0/files/tasks/rpm-test-deps.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-10-25 17:06:38.000000 specfile-0.9.0/files/zuul-tests.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.968166 specfile-0.9.0/plans/
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-10-25 17:06:38.000000 specfile-0.9.0/plans/full.fmf
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-10-25 17:06:38.000000 specfile-0.9.0/plans/git_reference.py
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-25 17:06:38.000000 specfile-0.9.0/plans/main.fmf
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-10-25 17:06:38.000000 specfile-0.9.0/plans/smoke.fmf
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-10-25 17:06:48.976166 specfile-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-10-25 17:06:38.000000 specfile-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.968166 specfile-0.9.0/specfile/
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-10-25 17:06:38.000000 specfile-0.9.0/specfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10488 2022-10-25 17:06:38.000000 specfile-0.9.0/specfile/changelog.py
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-10-25 17:06:38.000000 specfile-0.9.0/specfile/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7293 2022-10-25 17:06:38.000000 specfile-0.9.0/specfile/macro_definitions.py
--rw-r--r--   0 runner    (1001) docker     (121)    17764 2022-10-25 17:06:38.000000 specfile-0.9.0/specfile/macro_options.py
--rw-r--r--   0 runner    (1001) docker     (121)    11773 2022-10-25 17:06:38.000000 specfile-0.9.0/specfile/prep.py
--rw-r--r--   0 runner    (1001) docker     (121)    10003 2022-10-25 17:06:38.000000 specfile-0.9.0/specfile/rpm.py
--rw-r--r--   0 runner    (1001) docker     (121)     5713 2022-10-25 17:06:38.000000 specfile-0.9.0/specfile/sections.py
--rw-r--r--   0 runner    (1001) docker     (121)     4457 2022-10-25 17:06:38.000000 specfile-0.9.0/specfile/sourcelist.py
--rw-r--r--   0 runner    (1001) docker     (121)    19757 2022-10-25 17:06:38.000000 specfile-0.9.0/specfile/sources.py
--rw-r--r--   0 runner    (1001) docker     (121)    22964 2022-10-25 17:06:38.000000 specfile-0.9.0/specfile/specfile.py
--rw-r--r--   0 runner    (1001) docker     (121)    14738 2022-10-25 17:06:38.000000 specfile-0.9.0/specfile/tags.py
--rw-r--r--   0 runner    (1001) docker     (121)     2993 2022-10-25 17:06:38.000000 specfile-0.9.0/specfile/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    14115 2022-10-25 17:06:38.000000 specfile-0.9.0/specfile/value_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.968166 specfile-0.9.0/specfile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8640 2022-10-25 17:06:48.000000 specfile-0.9.0/specfile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3837 2022-10-25 17:06:48.000000 specfile-0.9.0/specfile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 17:06:48.000000 specfile-0.9.0/specfile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-10-25 17:06:48.000000 specfile-0.9.0/specfile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-25 17:06:48.000000 specfile-0.9.0/specfile.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.968166 specfile-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.964166 specfile-0.9.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.972166 specfile-0.9.0/tests/data/spec_autopatch/
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_autopatch/patch0.patch
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_autopatch/patch1.patch
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_autopatch/patch2.patch
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_autopatch/patch3.patch
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_autopatch/patch4.patch
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_autopatch/patch5.patch
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_autopatch/patch6.patch
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_autopatch/test-0.1.tar.xz
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_autopatch/test.spec
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.972166 specfile-0.9.0/tests/data/spec_autosetup/
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_autosetup/patch0.patch
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_autosetup/patch1.patch
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_autosetup/patch2.patch
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_autosetup/test-0.1.tar.xz
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_autosetup/test.spec
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.972166 specfile-0.9.0/tests/data/spec_commented_patches/
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_commented_patches/patch0.patch
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_commented_patches/patch1.patch
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_commented_patches/patch2.patch
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_commented_patches/patch3.patch
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_commented_patches/patch4.patch
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_commented_patches/patch5.patch
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_commented_patches/patch6.patch
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_commented_patches/test-0.1.tar.xz
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_commented_patches/test.spec
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.972166 specfile-0.9.0/tests/data/spec_macros/
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_macros/patch0.patch
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_macros/patch1.patch
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_macros/patch2.patch
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_macros/test-v0.1.2~rc2.tar.xz
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_macros/test.spec
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_macros/tests-01.tar.xz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.972166 specfile-0.9.0/tests/data/spec_minimal/
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_minimal/test.spec
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.972166 specfile-0.9.0/tests/data/spec_multiple_sources/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_multiple_sources/test.7z
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_multiple_sources/test.spec
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_multiple_sources/test.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_multiple_sources/test.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_multiple_sources/test.tar.lrz
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_multiple_sources/test.tar.lz
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_multiple_sources/test.tar.xz
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_multiple_sources/test.tar.zst
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_multiple_sources/test.txt
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_multiple_sources/test.zip
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.972166 specfile-0.9.0/tests/data/spec_patchlist/
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_patchlist/patch0.patch
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_patchlist/patch1.patch
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_patchlist/patch2.patch
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_patchlist/test-0.1.tar.xz
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_patchlist/test.spec
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.972166 specfile-0.9.0/tests/data/spec_rpmautospec/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_rpmautospec/test.spec
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.976166 specfile-0.9.0/tests/data/spec_traditional/
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_traditional/patch0.patch
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_traditional/patch1.patch
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_traditional/patch2.patch
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_traditional/test-0.1.tar.xz
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/data/spec_traditional/test.spec
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/full.fmf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.976166 specfile-0.9.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2143 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    11897 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/integration/test_specfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/smoke.fmf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:06:48.976166 specfile-0.9.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8372 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/unit/test_changelog.py
--rw-r--r--   0 runner    (1001) docker     (121)     3822 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/unit/test_macro_definitions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7305 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/unit/test_macro_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     3372 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/unit/test_prep.py
--rw-r--r--   0 runner    (1001) docker     (121)     4078 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/unit/test_rpm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1831 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/unit/test_sections.py
--rw-r--r--   0 runner    (1001) docker     (121)     1281 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/unit/test_sourcelist.py
--rw-r--r--   0 runner    (1001) docker     (121)    12695 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/unit/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/unit/test_specfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     3568 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/unit/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)     2602 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-10-25 17:06:38.000000 specfile-0.9.0/tests/unit/test_value_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.202503 specfile-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.190503 specfile-0.9.1/.fmf/
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2022-11-12 14:35:08.000000 specfile-0.9.1/.fmf/version
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-12 14:35:08.000000 specfile-0.9.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-11-12 14:35:08.000000 specfile-0.9.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.190503 specfile-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.194503 specfile-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      953 2022-11-12 14:35:08.000000 specfile-0.9.1/.github/workflows/do-release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-11-12 14:35:08.000000 specfile-0.9.1/.github/workflows/opened-issues-to-the-board.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-11-12 14:35:08.000000 specfile-0.9.1/.github/workflows/prepare-release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      827 2022-11-12 14:35:08.000000 specfile-0.9.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     4967 2022-11-12 14:35:08.000000 specfile-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     2718 2022-11-12 14:35:08.000000 specfile-0.9.1/.packit.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1720 2022-11-12 14:35:08.000000 specfile-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-11-12 14:35:08.000000 specfile-0.9.1/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (121)      577 2022-11-12 14:35:08.000000 specfile-0.9.1/.zuul.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     3351 2022-11-12 14:35:08.000000 specfile-0.9.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2022-11-12 14:35:08.000000 specfile-0.9.1/Containerfile.tests
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-11-12 14:35:08.000000 specfile-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-11-12 14:35:08.000000 specfile-0.9.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     8640 2022-11-12 14:35:18.202503 specfile-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7671 2022-11-12 14:35:08.000000 specfile-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.194503 specfile-0.9.1/fedora/
+-rw-r--r--   0 runner    (1001) docker     (121)     2312 2022-11-12 14:35:08.000000 specfile-0.9.1/fedora/python-specfile.spec
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.194503 specfile-0.9.1/files/
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2022-11-12 14:35:08.000000 specfile-0.9.1/files/install-requirements-pip.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-12 14:35:08.000000 specfile-0.9.1/files/install-requirements-rpms.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-11-12 14:35:08.000000 specfile-0.9.1/files/local-tests-requirements.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.194503 specfile-0.9.1/files/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-11-12 14:35:08.000000 specfile-0.9.1/files/tasks/build-rpm-deps.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-11-12 14:35:08.000000 specfile-0.9.1/files/tasks/generic-dnf-requirements.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      398 2022-11-12 14:35:08.000000 specfile-0.9.1/files/tasks/project-dir.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-11-12 14:35:08.000000 specfile-0.9.1/files/tasks/rpm-deps.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-11-12 14:35:08.000000 specfile-0.9.1/files/tasks/rpm-test-deps.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-12 14:35:08.000000 specfile-0.9.1/files/zuul-tests.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.194503 specfile-0.9.1/plans/
+-rw-r--r--   0 runner    (1001) docker     (121)      366 2022-11-12 14:35:08.000000 specfile-0.9.1/plans/full.fmf
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-11-12 14:35:08.000000 specfile-0.9.1/plans/git_reference.py
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-12 14:35:08.000000 specfile-0.9.1/plans/main.fmf
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-12 14:35:08.000000 specfile-0.9.1/plans/smoke.fmf
+-rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-11-12 14:35:18.202503 specfile-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-11-12 14:35:08.000000 specfile-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.194503 specfile-0.9.1/specfile/
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-11-12 14:35:08.000000 specfile-0.9.1/specfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10488 2022-11-12 14:35:08.000000 specfile-0.9.1/specfile/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-11-12 14:35:08.000000 specfile-0.9.1/specfile/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7293 2022-11-12 14:35:08.000000 specfile-0.9.1/specfile/macro_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17764 2022-11-12 14:35:08.000000 specfile-0.9.1/specfile/macro_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11773 2022-11-12 14:35:08.000000 specfile-0.9.1/specfile/prep.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15159 2022-11-12 14:35:08.000000 specfile-0.9.1/specfile/rpm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6006 2022-11-12 14:35:08.000000 specfile-0.9.1/specfile/sections.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4457 2022-11-12 14:35:08.000000 specfile-0.9.1/specfile/sourcelist.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19757 2022-11-12 14:35:08.000000 specfile-0.9.1/specfile/sources.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24043 2022-11-12 14:35:08.000000 specfile-0.9.1/specfile/specfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15508 2022-11-12 14:35:08.000000 specfile-0.9.1/specfile/tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2993 2022-11-12 14:35:08.000000 specfile-0.9.1/specfile/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14115 2022-11-12 14:35:08.000000 specfile-0.9.1/specfile/value_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.194503 specfile-0.9.1/specfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8640 2022-11-12 14:35:18.000000 specfile-0.9.1/specfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4146 2022-11-12 14:35:18.000000 specfile-0.9.1/specfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-12 14:35:18.000000 specfile-0.9.1/specfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-12 14:35:18.000000 specfile-0.9.1/specfile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-12 14:35:18.000000 specfile-0.9.1/specfile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.194503 specfile-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.190503 specfile-0.9.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.198503 specfile-0.9.1/tests/data/spec_autopatch/
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_autopatch/patch0.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_autopatch/patch1.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_autopatch/patch2.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_autopatch/patch3.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_autopatch/patch4.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_autopatch/patch5.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_autopatch/patch6.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_autopatch/test-0.1.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_autopatch/test.spec
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.198503 specfile-0.9.1/tests/data/spec_autosetup/
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_autosetup/patch0.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_autosetup/patch1.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_autosetup/patch2.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_autosetup/test-0.1.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_autosetup/test.spec
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.198503 specfile-0.9.1/tests/data/spec_commented_patches/
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_commented_patches/patch0.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_commented_patches/patch1.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_commented_patches/patch2.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_commented_patches/patch3.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_commented_patches/patch4.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_commented_patches/patch5.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_commented_patches/patch6.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_commented_patches/test-0.1.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (121)      700 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_commented_patches/test.spec
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.198503 specfile-0.9.1/tests/data/spec_includes/
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_includes/description.inc
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_includes/patch0.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_includes/patch1.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_includes/patch2.patch
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_includes/patches.inc
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_includes/test-0.1.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_includes/test.spec
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.198503 specfile-0.9.1/tests/data/spec_macros/
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_macros/patch0.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_macros/patch1.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_macros/patch2.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_macros/test-v0.1.2~rc2.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_macros/test.spec
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_macros/tests-01.tar.xz
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.198503 specfile-0.9.1/tests/data/spec_minimal/
+-rw-r--r--   0 runner    (1001) docker     (121)      234 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_minimal/test.spec
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.198503 specfile-0.9.1/tests/data/spec_multiple_sources/
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_multiple_sources/test.7z
+-rw-r--r--   0 runner    (1001) docker     (121)      702 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_multiple_sources/test.spec
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_multiple_sources/test.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_multiple_sources/test.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (121)      217 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_multiple_sources/test.tar.lrz
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_multiple_sources/test.tar.lz
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_multiple_sources/test.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_multiple_sources/test.tar.zst
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_multiple_sources/test.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_multiple_sources/test.zip
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.202503 specfile-0.9.1/tests/data/spec_patchlist/
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_patchlist/patch0.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_patchlist/patch1.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_patchlist/patch2.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_patchlist/test-0.1.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_patchlist/test.spec
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.202503 specfile-0.9.1/tests/data/spec_rpmautospec/
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_rpmautospec/test.spec
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.202503 specfile-0.9.1/tests/data/spec_shell_expansions/
+-rw-r--r--   0 runner    (1001) docker     (121)      398 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_shell_expansions/test.spec
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.202503 specfile-0.9.1/tests/data/spec_traditional/
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_traditional/patch0.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_traditional/patch1.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_traditional/patch2.patch
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_traditional/test-0.1.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (121)      418 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/data/spec_traditional/test.spec
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/full.fmf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.202503 specfile-0.9.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2597 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12936 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/integration/test_specfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/smoke.fmf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 14:35:18.202503 specfile-0.9.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8372 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/unit/test_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3822 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/unit/test_macro_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7305 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/unit/test_macro_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3372 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/unit/test_prep.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4107 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/unit/test_rpm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2252 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/unit/test_sections.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1281 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/unit/test_sourcelist.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12695 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/unit/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/unit/test_specfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4168 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/unit/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2602 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-11-12 14:35:08.000000 specfile-0.9.1/tests/unit/test_value_parser.py
```

### Comparing `specfile-0.9.0/.github/workflows/do-release.yml` & `specfile-0.9.1/.github/workflows/do-release.yml`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/.github/workflows/prepare-release.yml` & `specfile-0.9.1/.github/workflows/prepare-release.yml`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/.github/workflows/pypi-publish.yml` & `specfile-0.9.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/.gitignore` & `specfile-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/.packit.yaml` & `specfile-0.9.1/.packit.yaml`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/.pre-commit-config.yaml` & `specfile-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/.zuul.yaml` & `specfile-0.9.1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/CHANGELOG.md` & `specfile-0.9.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# 0.9.1
+
+- `specfile` now supports localized tags (e.g. `Summary(fr)`) and tags with qualifiers (e.g. `Requires(post)`).
+  It also follows more closely rpm parsing logic and doesn't fail on invalid section names. (#132)
+
 # 0.9.0
 
 - Added utility classes for working with (N)EVR. (#113)
 - Fixed an issue with multiple instances of `Specfile` not expanding macros in the right context. (#117)
 
 # 0.8.0
```

### Comparing `specfile-0.9.0/LICENSE` & `specfile-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/Makefile` & `specfile-0.9.1/Makefile`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/PKG-INFO` & `specfile-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specfile
-Version: 0.9.0
+Version: 0.9.1
 Summary: A library for parsing and manipulating RPM spec files.
 Home-page: https://github.com/packit/specfile
 Author: Red Hat
 Author-email: user-cont-team@redhat.com
 License: MIT
 Keywords: packaging,fedora,rpm,spec
 Classifier: Development Status :: 4 - Beta
```

### Comparing `specfile-0.9.0/README.md` & `specfile-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/fedora/python-specfile.spec` & `specfile-0.9.1/fedora/python-specfile.spec`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 %global desc %{expand:
 Python library for parsing and manipulating RPM spec files.
 Main focus is on modifying existing spec files, any change should result
 in a minimal diff.}
 
 
 Name:           python-specfile
-Version:        0.9.0
+Version:        0.9.1
 Release:        1%{?dist}
 
 Summary:        A library for parsing and manipulating RPM spec files
 License:        MIT
 URL:            https://github.com/packit/specfile
 
 Source0:        %{pypi_source specfile}
@@ -65,14 +65,17 @@
 
 
 %files -n python%{python3_pkgversion}-specfile -f %{pyproject_files}
 %doc README.md
 
 
 %changelog
+* Fri Nov 11 2022 Packit Team <hello@packit.dev> - 0.9.1-1
+- New upstream release 0.9.1
+
 * Tue Oct 25 2022 Packit Team <hello@packit.dev> - 0.9.0-1
 - New upstream release 0.9.0
 
 * Fri Oct 14 2022 Packit Team <hello@packit.dev> - 0.8.0-1
 - New upstream release 0.8.0
 
 * Fri Oct 07 2022 Packit Team <hello@packit.dev> - 0.7.0-1
```

### Comparing `specfile-0.9.0/setup.cfg` & `specfile-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/specfile/changelog.py` & `specfile-0.9.1/specfile/changelog.py`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/specfile/exceptions.py` & `specfile-0.9.1/specfile/exceptions.py`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/specfile/macro_definitions.py` & `specfile-0.9.1/specfile/macro_definitions.py`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/specfile/macro_options.py` & `specfile-0.9.1/specfile/macro_options.py`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/specfile/prep.py` & `specfile-0.9.1/specfile/prep.py`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/specfile/rpm.py` & `specfile-0.9.1/specfile/rpm.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright Contributors to the Packit project.
 # SPDX-License-Identifier: MIT
 
 import collections
 import contextlib
 import io
+import logging
 import os
 import re
 import sys
 import tempfile
 from enum import IntEnum
 from pathlib import Path
 from typing import Iterator, List, Optional, Tuple
@@ -15,14 +16,16 @@
 import rpm
 
 from specfile.exceptions import MacroRemovalException, RPMException
 from specfile.utils import get_filename_from_location
 
 MAX_REMOVAL_RETRIES = 20
 
+logger = logging.getLogger(__name__)
+
 
 @contextlib.contextmanager
 def capture_stderr() -> Iterator[List[bytes]]:
     """
     Context manager for capturing output to stderr. A stderr output of anything run
     in its context will be captured in the target variable of the with statement.
 
@@ -233,25 +236,54 @@
         # reset everything, including macros
         rpm.reloadConfig()
         for macro in cls.dump():
             if macro.level > level_threshold:
                 cls.remove(macro.name)
 
 
-class RPM:
-    @staticmethod
+class SpecParser:
+    """
+    Class that represents a spec file parser.
+
+    Attributes:
+        sourcedir: Path to sources and patches.
+        macros: List of extra macro definitions.
+        ignore_missing_includes: Whether to attempt to parse the spec file even if one
+          or more files to be included using the %include directive are not available.
+        spec: `rpm.spec` instance representing parsed spec file.
+        tainted: Indication that the spec file wasn't parsed completely and at least
+          one file to be included was ignored.
+    """
+
+    def __init__(
+        self,
+        sourcedir: Path,
+        macros: Optional[List[Tuple[str, str]]] = None,
+        ignore_missing_includes: bool = False,
+    ) -> None:
+        self.sourcedir = sourcedir
+        self.macros = macros.copy() if macros is not None else []
+        self.ignore_missing_includes = ignore_missing_includes
+        self.spec = None
+        self.tainted = False
+
+    def __repr__(self) -> str:
+        sourcedir = repr(self.sourcedir)
+        macros = repr(self.macros)
+        ignore_missing_includes = repr(self.ignore_missing_includes)
+        return f"SpecParser({sourcedir}, {macros}, {ignore_missing_includes})"
+
     @contextlib.contextmanager
-    def make_dummy_sources(sources: List[str], sourcedir: Path) -> Iterator[List[Path]]:
+    def _make_dummy_sources(self, sources: List[str]) -> Iterator[List[Path]]:
         """
         Context manager for creating temporary dummy sources to enable a spec file
         to be fully parsed by RPM.
 
         Args:
             sources: List of all sources (including patches) in a spec file.
-            sourcedir: Path to sources and patches.
 
         Yields:
             List of paths to each created dummy source.
         """
         # based on rpmFileIsCompressed() in rpmio/rpmfileutil.c in RPM source
         SIGNATURES = [
             (".bz2", b"BZh"),
@@ -266,61 +298,164 @@
         # number of bytes that RPM reads to determine the file type
         MAGIC_LENGTH = 13
         dummy_sources = []
         for source in sources:
             filename = get_filename_from_location(source)
             if not filename:
                 continue
-            path = sourcedir / filename
+            path = self.sourcedir / filename
             if path.is_file():
                 continue
             dummy_sources.append(path)
             for ext, magic in SIGNATURES:
                 if filename.endswith(ext):
                     path.write_bytes(magic.ljust(MAGIC_LENGTH, b"\x00"))
                     break
             else:
                 path.write_bytes(MAGIC_LENGTH * b"\x00")
         yield dummy_sources
         for path in dummy_sources:
             path.unlink()
 
-    @staticmethod
-    def parse(
-        content: str, sourcedir: Path, macros: Optional[List[Tuple[str, str]]] = None
-    ) -> rpm.spec:
+    @contextlib.contextmanager
+    def _sanitize_environment(self) -> Iterator[os._Environ]:
+        """
+        Context manager for sanitizing the environment for shell expansions.
+
+        Temporarily sets LANG and LC_ALL to C.UTF-8 locale.
+
+        Yields:
+            Sanitized environment.
+        """
+        env = os.environ.copy()
+
+        def restore(key):
+            try:
+                os.environ[key] = env[key]
+            except KeyError:
+                del os.environ[key]
+
+        keys = ["LANG", "LC_ALL"]
+        for key in keys:
+            os.environ[key] = "C.UTF-8"
+        try:
+            yield os.environ
+        finally:
+            for key in keys:
+                restore(key)
+
+    def _do_parse(
+        self, content: str, extra_macros: Optional[List[Tuple[str, str]]] = None
+    ) -> Tuple[rpm.spec, bool]:
         """
         Parses the content of a spec file.
 
         Args:
             content: String representing the content of a spec file.
-            sourcedir: Path to sources and patches.
-            macros: List of macro definitions that will be applied before parsing.
+            extra_macros: List of extra macro definitions.
 
         Returns:
-            Parsed spec file as `rpm.spec` instance.
+            Tuple of (parsed spec file as `rpm.spec` instance, indication whether
+              at least one file to be included was ignored).
 
         Raises:
             RPMException, if parsing error occurs.
         """
 
-        def reinit_macros():
+        def get_rpm_spec(content, flags):
             Macros.reinit()
-            for name, value in macros or []:
+            for name, value in self.macros + (extra_macros or []):
                 Macros.define(name, value)
-            Macros.define("_sourcedir", str(sourcedir))
+            Macros.define("_sourcedir", str(self.sourcedir))
+            with tempfile.NamedTemporaryFile() as tmp:
+                tmp.write(content.encode())
+                tmp.flush()
+                try:
+                    with self._sanitize_environment():
+                        with capture_stderr() as stderr:
+                            return rpm.spec(tmp.name, flags)
+                except ValueError as e:
+                    raise RPMException(stderr=stderr) from e
+
+        def get_included_sources(content):
+            include_regex = re.compile(r"^\s*%include\s+(.*)$")
+            lines = content.splitlines()
+            sources = []
+            while lines:
+                line = lines.pop(0)
+                m = include_regex.match(line)
+                if not m:
+                    continue
+                arg = m.group(1)
+                while line.endswith("\\"):
+                    line = lines.pop(0)
+                    arg = arg[:-1] + line
+                # we can expand macros here because the first non-build parse,
+                # even though it failed, populated the macro context
+                source = Path(Macros.expand(arg))
+                # ignore files outside of sourcedir
+                if source.parent.samefile(self.sourcedir):
+                    sources.append(source.name)
+            return sources
 
-        with tempfile.NamedTemporaryFile() as tmp:
-            tmp.write(content.encode())
-            tmp.flush()
-            try:
-                reinit_macros()
-                with capture_stderr() as stderr:
-                    # do a non-build parse first
-                    spec = rpm.spec(tmp.name, rpm.RPMSPEC_ANYARCH | rpm.RPMSPEC_FORCE)
-                reinit_macros()
-                with RPM.make_dummy_sources([s for s, _, _ in spec.sources], sourcedir):
-                    with capture_stderr() as stderr:
-                        # do a full parse with dummy sources
-                        return rpm.spec(tmp.name, rpm.RPMSPEC_ANYARCH)
-            except ValueError as e:
-                raise RPMException(stderr=stderr) from e
+        tainted = False
+        try:
+            # do a non-build parse first, to get a list of sources
+            spec = get_rpm_spec(content, rpm.RPMSPEC_ANYARCH | rpm.RPMSPEC_FORCE)
+            sources = [s for s, _, _ in spec.sources]
+        except RPMException:
+            if self.ignore_missing_includes:
+                sources = get_included_sources(content)
+                if not sources:
+                    # no point in trying again
+                    raise
+                with self._make_dummy_sources(sources) as dummy_sources:
+                    if dummy_sources:
+                        logger.warning(
+                            "Created dummy sources for nonexistent includes:\n"
+                            "\n".join(str(ds) for ds in dummy_sources)
+                        )
+                    # do a non-build parse again with dummy included sources
+                    spec = get_rpm_spec(
+                        content, rpm.RPMSPEC_ANYARCH | rpm.RPMSPEC_FORCE
+                    )
+                    sources = [s for s, _, _ in spec.sources]
+                tainted = True
+            else:
+                raise
+
+        # workaround RPM lua tables feature/bug
+        #
+        # RPM lua tables are a global storage that is used by lua macros and in turn
+        # also by standard %sources and %patches macros
+        #
+        # they are initialized when a rpm.spec instance is created and destroyed
+        # when a rpm.spec instance is deleted
+        #
+        # when a variable that holds a rpm.spec instance is assigned a new rpm.spec
+        # instance, the old instance is garbage collected afterwards and that destroys
+        # lua tables that were (re)initialized when the new instance was created
+        #
+        # explicitly deleting the old instance before creating a new one prevents this
+        del spec
+
+        with self._make_dummy_sources(sources):
+            # do a full parse with dummy sources
+            return get_rpm_spec(content, rpm.RPMSPEC_ANYARCH), tainted
+
+    def parse(
+        self, content: str, extra_macros: Optional[List[Tuple[str, str]]] = None
+    ) -> None:
+        """
+        Parses the content of a spec file and updates the `spec` and `tainted` attributes.
+
+        Args:
+            content: String representing the content of a spec file.
+            extra_macros: List of extra macro definitions.
+
+        Raises:
+            RPMException, if parsing error occurs.
+        """
+        if self.spec:
+            # workaround RPM lua tables feature/bug, see above for details
+            del self.spec
+        self.spec, self.tainted = self._do_parse(content, extra_macros)
```

### Comparing `specfile-0.9.0/specfile/sections.py` & `specfile-0.9.1/specfile/sections.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright Contributors to the Packit project.
 # SPDX-License-Identifier: MIT
 
 import collections
 import re
-from typing import List, Optional, SupportsIndex, Union, overload
+from typing import List, Optional, SupportsIndex, Union, cast, overload
 
 # valid section names as defined in build/parseSpec.c in RPM source
 SECTION_NAMES = {
     "package",
     "prep",
     "generate_buildrequires",
     "conf",
@@ -131,35 +131,43 @@
     def __repr__(self) -> str:
         data = repr(self.data)
         return f"Sections({data})"
 
     def __copy__(self) -> "Sections":
         return Sections(self.data)
 
+    def __contains__(self, name: object) -> bool:
+        try:
+            # use parent's __getattribute__() so this method can be called from __getattr__()
+            data = super().__getattribute__("data")
+        except AttributeError:
+            return False
+        return any(s.name.lower() == cast(str, name).split()[0].lower() for s in data)
+
     def __getattr__(self, name: str) -> Section:
-        if name.split()[0].lower() not in SECTION_NAMES:
+        if name not in self:
             return super().__getattribute__(name)
         try:
             return self.get(name)
         except ValueError:
             raise AttributeError(name)
 
     def __setattr__(self, name: str, value: Union[Section, List[str]]) -> None:
-        if name.split()[0].lower() not in SECTION_NAMES:
+        if name not in self:
             return super().__setattr__(name, value)
         try:
             if isinstance(value, Section):
                 self.data[self.find(name)] = value
             else:
                 self.data[self.find(name)].data = value
         except ValueError:
             raise AttributeError(name)
 
     def __delattr__(self, name: str) -> None:
-        if name.split()[0].lower() not in SECTION_NAMES:
+        if name not in self:
             return super().__delattr__(name)
         try:
             del self.data[self.find(name)]
         except ValueError:
             raise AttributeError(name)
 
     def get(self, name: str) -> Section:
@@ -180,15 +188,16 @@
         Args:
             lines: Lines to parse.
 
         Returns:
             Constructed instance of `Sections` class.
         """
         section_name_regexes = [
-            re.compile(rf"^%{re.escape(n)}\b.*", re.IGNORECASE) for n in SECTION_NAMES
+            re.compile(rf"^%{re.escape(n)}(\s+.*$|$)", re.IGNORECASE)
+            for n in SECTION_NAMES
         ]
         section_starts = []
         for i, line in enumerate(lines):
             if line.startswith("%"):
                 for r in section_name_regexes:
                     if r.match(line):
                         section_starts.append(i)
```

### Comparing `specfile-0.9.0/specfile/sourcelist.py` & `specfile-0.9.1/specfile/sourcelist.py`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/specfile/sources.py` & `specfile-0.9.1/specfile/sources.py`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/specfile/specfile.py` & `specfile-0.9.1/specfile/specfile.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pathlib import Path
 from typing import Iterator, List, Optional, Tuple, Type, Union
 
 from specfile.changelog import Changelog, ChangelogEntry
 from specfile.exceptions import SourceNumberException, SpecfileException
 from specfile.macro_definitions import MacroDefinition, MacroDefinitions
 from specfile.prep import Prep
-from specfile.rpm import RPM, Macros
+from specfile.rpm import Macros, SpecParser
 from specfile.sections import Section, Sections
 from specfile.sourcelist import Sourcelist
 from specfile.sources import Patches, Sources
 from specfile.tags import Tag, Tags
 from specfile.value_parser import SUBSTITUTION_GROUP_PREFIX, ValueParser
 
 
@@ -27,36 +27,41 @@
     Class that represents a spec file.
 
     Attributes:
         path: Path to the spec file.
         sourcedir: Path to sources and patches.
         autosave: Whether to automatically save any changes made.
         macros: List of extra macro definitions.
+        ignore_missing_includes: Whether to attempt to parse the spec file even if one
+          or more files to be included using the %include directive are not available.
     """
 
     def __init__(
         self,
         path: Union[Path, str],
         sourcedir: Optional[Union[Path, str]] = None,
         autosave: bool = False,
         macros: Optional[List[Tuple[str, str]]] = None,
+        ignore_missing_includes: bool = False,
     ) -> None:
         self.path = Path(path)
-        self.sourcedir = Path(sourcedir or self.path.parent)
         self.autosave = autosave
-        self.macros = macros.copy() if macros is not None else []
         self._lines = self.path.read_text().splitlines()
-        self._spec = RPM.parse(str(self), self.sourcedir, self.macros)
+        self._parser = SpecParser(
+            Path(sourcedir or self.path.parent), macros, ignore_missing_includes
+        )
+        self._parser.parse(str(self))
 
     def __repr__(self) -> str:
         path = repr(self.path)
-        sourcedir = repr(self.sourcedir)
+        sourcedir = repr(self._parser.sourcedir)
         autosave = repr(self.autosave)
-        macros = repr(self.macros)
-        return f"Specfile({path}, {sourcedir}, {autosave}, {macros})"
+        macros = repr(self._parser.macros)
+        ignore_missing_includes = repr(self._parser.ignore_missing_includes)
+        return f"Specfile({path}, {sourcedir}, {autosave}, {macros}, {ignore_missing_includes})"
 
     def __str__(self) -> str:
         return "\n".join(self._lines) + "\n"
 
     def __enter__(self) -> "Specfile":
         return self
 
@@ -64,18 +69,44 @@
         self,
         exc_type: Optional[Type[BaseException]],
         exc_value: Optional[BaseException],
         traceback: Optional[types.TracebackType],
     ) -> None:
         self.save()
 
+    @property
+    def sourcedir(self) -> Path:
+        """Path to sources and patches."""
+        return self._parser.sourcedir
+
+    @property
+    def macros(self) -> List[Tuple[str, str]]:
+        """List of extra macro definitions."""
+        return self._parser.macros
+
+    @property
+    def ignore_missing_includes(self) -> bool:
+        """
+        Whether to attempt to parse the spec file even if one or more files
+        to be included using the %include directive are not available.
+        """
+        return self._parser.ignore_missing_includes
+
+    @property
+    def tainted(self) -> bool:
+        """
+        Indication that the spec file wasn't parsed completely and at least
+        one file to be included was ignored.
+        """
+        return self._parser.tainted
+
     def reload(self) -> None:
         """Reload the spec file content."""
         self._lines = self.path.read_text().splitlines()
-        self._spec = RPM.parse(str(self), self.sourcedir, self.macros)
+        self._parser.parse(str(self))
 
     def save(self) -> None:
         """Save the spec file content."""
         self.path.write_text(str(self))
 
     def expand(
         self, expression: str, extra_macros: Optional[List[Tuple[str, str]]] = None
@@ -86,29 +117,29 @@
         Args:
             expression: Expression to expand.
             extra_macros: Extra macros to be defined before expansion is performed.
 
         Returns:
             Expanded expression.
         """
-        RPM.parse(str(self), self.sourcedir, self.macros + (extra_macros or []))
+        self._parser.parse(str(self), extra_macros)
         return Macros.expand(expression)
 
     @contextlib.contextmanager
     def lines(self) -> Iterator[List[str]]:
         """
         Context manager for accessing spec file lines.
 
         Yields:
             Spec file lines as list of strings.
         """
         try:
             yield self._lines
         finally:
-            self._spec = RPM.parse(str(self), self.sourcedir, self.macros)
+            self._parser.parse(str(self))
             if self.autosave:
                 self.save()
 
     @contextlib.contextmanager
     def macro_definitions(self) -> Iterator[MacroDefinitions]:
         """
         Context manager for accessing macro definitions.
@@ -135,17 +166,19 @@
             sections = Sections.parse(lines)
             try:
                 yield sections
             finally:
                 lines[:] = sections.get_raw_data()
 
     @property
-    def parsed_sections(self) -> Sections:
+    def parsed_sections(self) -> Optional[Sections]:
         """Parsed spec file sections."""
-        return Sections.parse(self._spec.parsed.splitlines())
+        if not self._parser.spec:
+            return None
+        return Sections.parse(self._parser.spec.parsed.splitlines())
 
     @contextlib.contextmanager
     def tags(self, section: Union[str, Section] = "package") -> Iterator[Tags]:
         """
         Context manager for accessing tags in a specified section.
 
         Args:
```

### Comparing `specfile-0.9.0/specfile/tags.py` & `specfile-0.9.1/specfile/tags.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright Contributors to the Packit project.
 # SPDX-License-Identifier: MIT
 
 import collections
 import itertools
 import re
-from typing import Any, Iterable, List, Optional, SupportsIndex, Union, overload
+from typing import Any, Iterable, List, Optional, SupportsIndex, Union, cast, overload
 
 from specfile.sections import Section
 
 # valid tag names as defined in build/parsePreamble.c in RPM source
 TAG_NAMES = {
     "name",
     "version",
@@ -58,14 +58,33 @@
     "translationurl",
     "upstreamreleases",
     "orderwithrequires",
     "removepathpostfixes",
     "modularitylabel",
 }
 
+# tags that can optionally have an argument (language or qualifier)
+TAGS_WITH_ARG = {
+    "summary",
+    "group",
+    "requires",
+    "prereq",
+    "orderwithrequires",
+}
+
+
+def get_tag_name_regex(name: str) -> str:
+    """Contructs regex corresponding to the specified tag name."""
+    regex = re.escape(name)
+    if name in TAGS_WITH_ARG:
+        regex += r"(?:\s*\(\s*[^\s)]*\s*\))?"
+    elif name in ["source", "patch"]:
+        regex += r"\d*"
+    return regex
+
 
 class Comment:
     """
     Class that represents a comment.
 
     Attributes:
         text: Text of the comment.
@@ -245,15 +264,18 @@
               Separator between name and literal value (colon usually surrounded by some
               amount of whitespace).
             comments: List of comments associated with the tag.
 
         Returns:
             Constructed instance of `Tag` class.
         """
-        if not name or name.lower().rstrip("0123456789") not in TAG_NAMES:
+        name_regexes = [
+            re.compile(get_tag_name_regex(t), re.IGNORECASE) for t in TAG_NAMES
+        ]
+        if not name or not any(r.match(name) for r in name_regexes):
             raise ValueError(f"Invalid tag name: '{name}'")
         self.name = name
         self.value = value
         self._expanded_value = expanded_value
         self._separator = separator
         self.comments = comments.copy()
 
@@ -371,35 +393,43 @@
 
         if isinstance(i, slice):
             for index in reversed(range(len(self.data))[i]):
                 delete(index)
         else:
             delete(i)
 
+    def __contains__(self, name: object) -> bool:
+        try:
+            # use parent's __getattribute__() so this method can be called from __getattr__()
+            data = super().__getattribute__("data")
+        except AttributeError:
+            return False
+        return any(t.name.lower() == cast(str, name).lower() for t in data)
+
     def __getattr__(self, name: str) -> Tag:
-        if name.lower().rstrip("0123456789") not in TAG_NAMES:
+        if name not in self:
             return super().__getattribute__(name)
         try:
             return self.data[self.find(name)]
         except ValueError:
             raise AttributeError(name)
 
     def __setattr__(self, name: str, value: Union[Tag, str]) -> None:
-        if name.lower().rstrip("0123456789") not in TAG_NAMES:
+        if name not in self:
             return super().__setattr__(name, value)
         try:
             if isinstance(value, Tag):
                 self.data[self.find(name)] = value
             else:
                 self.data[self.find(name)].value = value
         except ValueError:
             raise AttributeError(name)
 
     def __delattr__(self, name: str) -> None:
-        if name.lower().rstrip("0123456789") not in TAG_NAMES:
+        if name not in self:
             return super().__delattr__(name)
         try:
             del self.data[self.find(name)]
         except ValueError:
             raise AttributeError(name)
 
     def copy(self) -> "Tags":
@@ -439,17 +469,16 @@
             parsed_section: The same section after parsing.
 
         Returns:
             Constructed instance of `Tags` class.
         """
 
         def regex_pattern(tag):
-            name = re.escape(tag)
-            index = r"\d*" if tag in ["source", "patch"] else ""
-            return rf"^(?P<n>{name}{index})(?P<s>\s*:\s*)(?P<v>.+)"
+            name_regex = get_tag_name_regex(tag)
+            return rf"^(?P<n>{name_regex})(?P<s>\s*:\s*)(?P<v>.+)"
 
         tag_regexes = [re.compile(regex_pattern(t), re.IGNORECASE) for t in TAG_NAMES]
         data = []
         buffer: List[str] = []
         for line in raw_section:
             # find out if there is a match for one of the tag regexes
             m = next((m for m in (r.match(line) for r in tag_regexes) if m), None)
```

### Comparing `specfile-0.9.0/specfile/utils.py` & `specfile-0.9.1/specfile/utils.py`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/specfile/value_parser.py` & `specfile-0.9.1/specfile/value_parser.py`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/specfile.egg-info/PKG-INFO` & `specfile-0.9.1/specfile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specfile
-Version: 0.9.0
+Version: 0.9.1
 Summary: A library for parsing and manipulating RPM spec files.
 Home-page: https://github.com/packit/specfile
 Author: Red Hat
 Author-email: user-cont-team@redhat.com
 License: MIT
 Keywords: packaging,fedora,rpm,spec
 Classifier: Development Status :: 4 - Beta
```

### Comparing `specfile-0.9.0/specfile.egg-info/SOURCES.txt` & `specfile-0.9.1/specfile.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .git_archival.txt
 .gitattributes
 .gitignore
 .packit.yaml
 .pre-commit-config.yaml
+.prettierignore
 .zuul.yaml
 CHANGELOG.md
 Containerfile.tests
 LICENSE
 Makefile
 README.md
 setup.cfg
@@ -46,15 +47,14 @@
 specfile/value_parser.py
 specfile.egg-info/PKG-INFO
 specfile.egg-info/SOURCES.txt
 specfile.egg-info/dependency_links.txt
 specfile.egg-info/requires.txt
 specfile.egg-info/top_level.txt
 tests/__init__.py
-tests/conftest.py
 tests/constants.py
 tests/full.fmf
 tests/smoke.fmf
 tests/data/spec_autopatch/patch0.patch
 tests/data/spec_autopatch/patch1.patch
 tests/data/spec_autopatch/patch2.patch
 tests/data/spec_autopatch/patch3.patch
@@ -73,14 +73,21 @@
 tests/data/spec_commented_patches/patch2.patch
 tests/data/spec_commented_patches/patch3.patch
 tests/data/spec_commented_patches/patch4.patch
 tests/data/spec_commented_patches/patch5.patch
 tests/data/spec_commented_patches/patch6.patch
 tests/data/spec_commented_patches/test-0.1.tar.xz
 tests/data/spec_commented_patches/test.spec
+tests/data/spec_includes/description.inc
+tests/data/spec_includes/patch0.patch
+tests/data/spec_includes/patch1.patch
+tests/data/spec_includes/patch2.patch
+tests/data/spec_includes/patches.inc
+tests/data/spec_includes/test-0.1.tar.xz
+tests/data/spec_includes/test.spec
 tests/data/spec_macros/patch0.patch
 tests/data/spec_macros/patch1.patch
 tests/data/spec_macros/patch2.patch
 tests/data/spec_macros/test-v0.1.2~rc2.tar.xz
 tests/data/spec_macros/test.spec
 tests/data/spec_macros/tests-01.tar.xz
 tests/data/spec_minimal/test.spec
@@ -96,14 +103,15 @@
 tests/data/spec_multiple_sources/test.zip
 tests/data/spec_patchlist/patch0.patch
 tests/data/spec_patchlist/patch1.patch
 tests/data/spec_patchlist/patch2.patch
 tests/data/spec_patchlist/test-0.1.tar.xz
 tests/data/spec_patchlist/test.spec
 tests/data/spec_rpmautospec/test.spec
+tests/data/spec_shell_expansions/test.spec
 tests/data/spec_traditional/patch0.patch
 tests/data/spec_traditional/patch1.patch
 tests/data/spec_traditional/patch2.patch
 tests/data/spec_traditional/test-0.1.tar.xz
 tests/data/spec_traditional/test.spec
 tests/integration/__init__.py
 tests/integration/conftest.py
```

### Comparing `specfile-0.9.0/tests/constants.py` & `specfile-0.9.1/tests/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,12 +7,14 @@
 DATA_DIR = TESTS_DIR / "data"
 SPEC_MINIMAL = DATA_DIR / "spec_minimal"
 SPEC_RPMAUTOSPEC = DATA_DIR / "spec_rpmautospec"
 SPEC_TRADITIONAL = DATA_DIR / "spec_traditional"
 SPEC_AUTOSETUP = DATA_DIR / "spec_autosetup"
 SPEC_AUTOPATCH = DATA_DIR / "spec_autopatch"
 SPEC_PATCHLIST = DATA_DIR / "spec_patchlist"
+SPEC_INCLUDES = DATA_DIR / "spec_includes"
 SPEC_MACROS = DATA_DIR / "spec_macros"
 SPEC_MULTIPLE_SOURCES = DATA_DIR / "spec_multiple_sources"
 SPEC_COMMENTED_PATCHES = DATA_DIR / "spec_commented_patches"
+SPEC_SHELL_EXPANSIONS = DATA_DIR / "spec_shell_expansions"
 
 SPECFILE = "test.spec"
```

### Comparing `specfile-0.9.0/tests/data/spec_autopatch/test.spec` & `specfile-0.9.1/tests/data/spec_autopatch/test.spec`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/tests/data/spec_commented_patches/test.spec` & `specfile-0.9.1/tests/data/spec_commented_patches/test.spec`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/tests/data/spec_macros/test.spec` & `specfile-0.9.1/tests/data/spec_macros/test.spec`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/tests/data/spec_multiple_sources/test.spec` & `specfile-0.9.1/tests/data/spec_multiple_sources/test.spec`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/tests/integration/conftest.py` & `specfile-0.9.1/tests/integration/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,128 +7,157 @@
 00000060: 6d70 6f72 7420 7079 7465 7374 0a0a 6672  mport pytest..fr
 00000070: 6f6d 2074 6573 7473 2e63 6f6e 7374 616e  om tests.constan
 00000080: 7473 2069 6d70 6f72 7420 280a 2020 2020  ts import (.    
 00000090: 5350 4543 5f41 5554 4f50 4154 4348 2c0a  SPEC_AUTOPATCH,.
 000000a0: 2020 2020 5350 4543 5f41 5554 4f53 4554      SPEC_AUTOSET
 000000b0: 5550 2c0a 2020 2020 5350 4543 5f43 4f4d  UP,.    SPEC_COM
 000000c0: 4d45 4e54 4544 5f50 4154 4348 4553 2c0a  MENTED_PATCHES,.
-000000d0: 2020 2020 5350 4543 5f4d 4143 524f 532c      SPEC_MACROS,
-000000e0: 0a20 2020 2053 5045 435f 4d49 4e49 4d41  .    SPEC_MINIMA
-000000f0: 4c2c 0a20 2020 2053 5045 435f 4d55 4c54  L,.    SPEC_MULT
-00000100: 4950 4c45 5f53 4f55 5243 4553 2c0a 2020  IPLE_SOURCES,.  
-00000110: 2020 5350 4543 5f50 4154 4348 4c49 5354    SPEC_PATCHLIST
-00000120: 2c0a 2020 2020 5350 4543 5f52 504d 4155  ,.    SPEC_RPMAU
-00000130: 544f 5350 4543 2c0a 2020 2020 5350 4543  TOSPEC,.    SPEC
-00000140: 5f54 5241 4449 5449 4f4e 414c 2c0a 2020  _TRADITIONAL,.  
-00000150: 2020 5350 4543 4649 4c45 2c0a 290a 0a0a    SPECFILE,.)...
-00000160: 4070 7974 6573 742e 6669 7874 7572 6528  @pytest.fixture(
-00000170: 7363 6f70 653d 2266 756e 6374 696f 6e22  scope="function"
-00000180: 290a 6465 6620 7370 6563 5f6d 696e 696d  ).def spec_minim
-00000190: 616c 2874 6d70 5f70 6174 6829 3a0a 2020  al(tmp_path):.  
-000001a0: 2020 7370 6563 6669 6c65 5f70 6174 6820    specfile_path 
-000001b0: 3d20 746d 705f 7061 7468 202f 2053 5045  = tmp_path / SPE
-000001c0: 4346 494c 450a 2020 2020 7368 7574 696c  CFILE.    shutil
-000001d0: 2e63 6f70 7966 696c 6528 5350 4543 5f4d  .copyfile(SPEC_M
-000001e0: 494e 494d 414c 202f 2053 5045 4346 494c  INIMAL / SPECFIL
-000001f0: 452c 2073 7065 6366 696c 655f 7061 7468  E, specfile_path
-00000200: 290a 2020 2020 7265 7475 726e 2073 7065  ).    return spe
-00000210: 6366 696c 655f 7061 7468 0a0a 0a40 7079  cfile_path...@py
-00000220: 7465 7374 2e66 6978 7475 7265 2873 636f  test.fixture(sco
-00000230: 7065 3d22 6675 6e63 7469 6f6e 2229 0a64  pe="function").d
-00000240: 6566 2073 7065 635f 7270 6d61 7574 6f73  ef spec_rpmautos
-00000250: 7065 6328 746d 705f 7061 7468 293a 0a20  pec(tmp_path):. 
-00000260: 2020 2073 7065 6366 696c 655f 7061 7468     specfile_path
-00000270: 203d 2074 6d70 5f70 6174 6820 2f20 5350   = tmp_path / SP
-00000280: 4543 4649 4c45 0a20 2020 2073 6875 7469  ECFILE.    shuti
-00000290: 6c2e 636f 7079 6669 6c65 2853 5045 435f  l.copyfile(SPEC_
-000002a0: 5250 4d41 5554 4f53 5045 4320 2f20 5350  RPMAUTOSPEC / SP
-000002b0: 4543 4649 4c45 2c20 7370 6563 6669 6c65  ECFILE, specfile
-000002c0: 5f70 6174 6829 0a20 2020 2072 6574 7572  _path).    retur
-000002d0: 6e20 7370 6563 6669 6c65 5f70 6174 680a  n specfile_path.
-000002e0: 0a0a 4070 7974 6573 742e 6669 7874 7572  ..@pytest.fixtur
-000002f0: 6528 7363 6f70 653d 2266 756e 6374 696f  e(scope="functio
-00000300: 6e22 290a 6465 6620 7370 6563 5f74 7261  n").def spec_tra
-00000310: 6469 7469 6f6e 616c 2874 6d70 5f70 6174  ditional(tmp_pat
-00000320: 6829 3a0a 2020 2020 6465 7374 696e 6174  h):.    destinat
-00000330: 696f 6e20 3d20 746d 705f 7061 7468 202f  ion = tmp_path /
-00000340: 2022 7370 6563 5f74 7261 6469 7469 6f6e   "spec_tradition
-00000350: 616c 220a 2020 2020 7368 7574 696c 2e63  al".    shutil.c
-00000360: 6f70 7974 7265 6528 5350 4543 5f54 5241  opytree(SPEC_TRA
-00000370: 4449 5449 4f4e 414c 2c20 6465 7374 696e  DITIONAL, destin
-00000380: 6174 696f 6e29 0a20 2020 2072 6574 7572  ation).    retur
-00000390: 6e20 6465 7374 696e 6174 696f 6e20 2f20  n destination / 
-000003a0: 5350 4543 4649 4c45 0a0a 0a40 7079 7465  SPECFILE...@pyte
-000003b0: 7374 2e66 6978 7475 7265 2873 636f 7065  st.fixture(scope
-000003c0: 3d22 6675 6e63 7469 6f6e 2229 0a64 6566  ="function").def
-000003d0: 2073 7065 635f 6175 746f 7365 7475 7028   spec_autosetup(
-000003e0: 746d 705f 7061 7468 293a 0a20 2020 2064  tmp_path):.    d
-000003f0: 6573 7469 6e61 7469 6f6e 203d 2074 6d70  estination = tmp
-00000400: 5f70 6174 6820 2f20 2273 7065 635f 6175  _path / "spec_au
-00000410: 746f 7365 7475 7022 0a20 2020 2073 6875  tosetup".    shu
-00000420: 7469 6c2e 636f 7079 7472 6565 2853 5045  til.copytree(SPE
-00000430: 435f 4155 544f 5345 5455 502c 2064 6573  C_AUTOSETUP, des
-00000440: 7469 6e61 7469 6f6e 290a 2020 2020 7265  tination).    re
-00000450: 7475 726e 2064 6573 7469 6e61 7469 6f6e  turn destination
-00000460: 202f 2053 5045 4346 494c 450a 0a0a 4070   / SPECFILE...@p
-00000470: 7974 6573 742e 6669 7874 7572 6528 7363  ytest.fixture(sc
-00000480: 6f70 653d 2266 756e 6374 696f 6e22 290a  ope="function").
-00000490: 6465 6620 7370 6563 5f61 7574 6f70 6174  def spec_autopat
-000004a0: 6368 2874 6d70 5f70 6174 6829 3a0a 2020  ch(tmp_path):.  
-000004b0: 2020 6465 7374 696e 6174 696f 6e20 3d20    destination = 
-000004c0: 746d 705f 7061 7468 202f 2022 7370 6563  tmp_path / "spec
-000004d0: 5f61 7574 6f70 6174 6368 220a 2020 2020  _autopatch".    
-000004e0: 7368 7574 696c 2e63 6f70 7974 7265 6528  shutil.copytree(
-000004f0: 5350 4543 5f41 5554 4f50 4154 4348 2c20  SPEC_AUTOPATCH, 
-00000500: 6465 7374 696e 6174 696f 6e29 0a20 2020  destination).   
-00000510: 2072 6574 7572 6e20 6465 7374 696e 6174   return destinat
-00000520: 696f 6e20 2f20 5350 4543 4649 4c45 0a0a  ion / SPECFILE..
-00000530: 0a40 7079 7465 7374 2e66 6978 7475 7265  .@pytest.fixture
-00000540: 2873 636f 7065 3d22 6675 6e63 7469 6f6e  (scope="function
-00000550: 2229 0a64 6566 2073 7065 635f 7061 7463  ").def spec_patc
-00000560: 686c 6973 7428 746d 705f 7061 7468 293a  hlist(tmp_path):
-00000570: 0a20 2020 2064 6573 7469 6e61 7469 6f6e  .    destination
-00000580: 203d 2074 6d70 5f70 6174 6820 2f20 2273   = tmp_path / "s
-00000590: 7065 635f 7061 7463 686c 6973 7422 0a20  pec_patchlist". 
-000005a0: 2020 2073 6875 7469 6c2e 636f 7079 7472     shutil.copytr
-000005b0: 6565 2853 5045 435f 5041 5443 484c 4953  ee(SPEC_PATCHLIS
-000005c0: 542c 2064 6573 7469 6e61 7469 6f6e 290a  T, destination).
-000005d0: 2020 2020 7265 7475 726e 2064 6573 7469      return desti
-000005e0: 6e61 7469 6f6e 202f 2053 5045 4346 494c  nation / SPECFIL
-000005f0: 450a 0a0a 4070 7974 6573 742e 6669 7874  E...@pytest.fixt
-00000600: 7572 6528 7363 6f70 653d 2266 756e 6374  ure(scope="funct
-00000610: 696f 6e22 290a 6465 6620 7370 6563 5f6d  ion").def spec_m
-00000620: 6163 726f 7328 746d 705f 7061 7468 293a  acros(tmp_path):
-00000630: 0a20 2020 2064 6573 7469 6e61 7469 6f6e  .    destination
-00000640: 203d 2074 6d70 5f70 6174 6820 2f20 2273   = tmp_path / "s
-00000650: 7065 635f 6d61 6372 6f73 220a 2020 2020  pec_macros".    
-00000660: 7368 7574 696c 2e63 6f70 7974 7265 6528  shutil.copytree(
-00000670: 5350 4543 5f4d 4143 524f 532c 2064 6573  SPEC_MACROS, des
-00000680: 7469 6e61 7469 6f6e 290a 2020 2020 7265  tination).    re
-00000690: 7475 726e 2064 6573 7469 6e61 7469 6f6e  turn destination
-000006a0: 202f 2053 5045 4346 494c 450a 0a0a 4070   / SPECFILE...@p
-000006b0: 7974 6573 742e 6669 7874 7572 6528 7363  ytest.fixture(sc
-000006c0: 6f70 653d 2266 756e 6374 696f 6e22 290a  ope="function").
-000006d0: 6465 6620 7370 6563 5f6d 756c 7469 706c  def spec_multipl
-000006e0: 655f 736f 7572 6365 7328 746d 705f 7061  e_sources(tmp_pa
-000006f0: 7468 293a 0a20 2020 2064 6573 7469 6e61  th):.    destina
-00000700: 7469 6f6e 203d 2074 6d70 5f70 6174 6820  tion = tmp_path 
-00000710: 2f20 2273 7065 635f 6d75 6c74 6970 6c65  / "spec_multiple
-00000720: 5f73 6f75 7263 6573 220a 2020 2020 7368  _sources".    sh
-00000730: 7574 696c 2e63 6f70 7974 7265 6528 5350  util.copytree(SP
-00000740: 4543 5f4d 554c 5449 504c 455f 534f 5552  EC_MULTIPLE_SOUR
-00000750: 4345 532c 2064 6573 7469 6e61 7469 6f6e  CES, destination
-00000760: 290a 2020 2020 7265 7475 726e 2064 6573  ).    return des
-00000770: 7469 6e61 7469 6f6e 202f 2053 5045 4346  tination / SPECF
-00000780: 494c 450a 0a0a 4070 7974 6573 742e 6669  ILE...@pytest.fi
-00000790: 7874 7572 6528 7363 6f70 653d 2266 756e  xture(scope="fun
-000007a0: 6374 696f 6e22 290a 6465 6620 7370 6563  ction").def spec
-000007b0: 5f63 6f6d 6d65 6e74 6564 5f70 6174 6368  _commented_patch
-000007c0: 6573 2874 6d70 5f70 6174 6829 3a0a 2020  es(tmp_path):.  
-000007d0: 2020 6465 7374 696e 6174 696f 6e20 3d20    destination = 
-000007e0: 746d 705f 7061 7468 202f 2022 7370 6563  tmp_path / "spec
-000007f0: 5f63 6f6d 6d65 6e74 6564 5f70 6174 6368  _commented_patch
-00000800: 6573 220a 2020 2020 7368 7574 696c 2e63  es".    shutil.c
-00000810: 6f70 7974 7265 6528 5350 4543 5f43 4f4d  opytree(SPEC_COM
-00000820: 4d45 4e54 4544 5f50 4154 4348 4553 2c20  MENTED_PATCHES, 
-00000830: 6465 7374 696e 6174 696f 6e29 0a20 2020  destination).   
-00000840: 2072 6574 7572 6e20 6465 7374 696e 6174   return destinat
-00000850: 696f 6e20 2f20 5350 4543 4649 4c45 0a    ion / SPECFILE.
+000000d0: 2020 2020 5350 4543 5f49 4e43 4c55 4445      SPEC_INCLUDE
+000000e0: 532c 0a20 2020 2053 5045 435f 4d41 4352  S,.    SPEC_MACR
+000000f0: 4f53 2c0a 2020 2020 5350 4543 5f4d 494e  OS,.    SPEC_MIN
+00000100: 494d 414c 2c0a 2020 2020 5350 4543 5f4d  IMAL,.    SPEC_M
+00000110: 554c 5449 504c 455f 534f 5552 4345 532c  ULTIPLE_SOURCES,
+00000120: 0a20 2020 2053 5045 435f 5041 5443 484c  .    SPEC_PATCHL
+00000130: 4953 542c 0a20 2020 2053 5045 435f 5250  IST,.    SPEC_RP
+00000140: 4d41 5554 4f53 5045 432c 0a20 2020 2053  MAUTOSPEC,.    S
+00000150: 5045 435f 5348 454c 4c5f 4558 5041 4e53  PEC_SHELL_EXPANS
+00000160: 494f 4e53 2c0a 2020 2020 5350 4543 5f54  IONS,.    SPEC_T
+00000170: 5241 4449 5449 4f4e 414c 2c0a 2020 2020  RADITIONAL,.    
+00000180: 5350 4543 4649 4c45 2c0a 290a 0a0a 4070  SPECFILE,.)...@p
+00000190: 7974 6573 742e 6669 7874 7572 6528 7363  ytest.fixture(sc
+000001a0: 6f70 653d 2266 756e 6374 696f 6e22 290a  ope="function").
+000001b0: 6465 6620 7370 6563 5f6d 696e 696d 616c  def spec_minimal
+000001c0: 2874 6d70 5f70 6174 6829 3a0a 2020 2020  (tmp_path):.    
+000001d0: 7370 6563 6669 6c65 5f70 6174 6820 3d20  specfile_path = 
+000001e0: 746d 705f 7061 7468 202f 2053 5045 4346  tmp_path / SPECF
+000001f0: 494c 450a 2020 2020 7368 7574 696c 2e63  ILE.    shutil.c
+00000200: 6f70 7966 696c 6528 5350 4543 5f4d 494e  opyfile(SPEC_MIN
+00000210: 494d 414c 202f 2053 5045 4346 494c 452c  IMAL / SPECFILE,
+00000220: 2073 7065 6366 696c 655f 7061 7468 290a   specfile_path).
+00000230: 2020 2020 7265 7475 726e 2073 7065 6366      return specf
+00000240: 696c 655f 7061 7468 0a0a 0a40 7079 7465  ile_path...@pyte
+00000250: 7374 2e66 6978 7475 7265 2873 636f 7065  st.fixture(scope
+00000260: 3d22 6675 6e63 7469 6f6e 2229 0a64 6566  ="function").def
+00000270: 2073 7065 635f 7270 6d61 7574 6f73 7065   spec_rpmautospe
+00000280: 6328 746d 705f 7061 7468 293a 0a20 2020  c(tmp_path):.   
+00000290: 2073 7065 6366 696c 655f 7061 7468 203d   specfile_path =
+000002a0: 2074 6d70 5f70 6174 6820 2f20 5350 4543   tmp_path / SPEC
+000002b0: 4649 4c45 0a20 2020 2073 6875 7469 6c2e  FILE.    shutil.
+000002c0: 636f 7079 6669 6c65 2853 5045 435f 5250  copyfile(SPEC_RP
+000002d0: 4d41 5554 4f53 5045 4320 2f20 5350 4543  MAUTOSPEC / SPEC
+000002e0: 4649 4c45 2c20 7370 6563 6669 6c65 5f70  FILE, specfile_p
+000002f0: 6174 6829 0a20 2020 2072 6574 7572 6e20  ath).    return 
+00000300: 7370 6563 6669 6c65 5f70 6174 680a 0a0a  specfile_path...
+00000310: 4070 7974 6573 742e 6669 7874 7572 6528  @pytest.fixture(
+00000320: 7363 6f70 653d 2266 756e 6374 696f 6e22  scope="function"
+00000330: 290a 6465 6620 7370 6563 5f74 7261 6469  ).def spec_tradi
+00000340: 7469 6f6e 616c 2874 6d70 5f70 6174 6829  tional(tmp_path)
+00000350: 3a0a 2020 2020 6465 7374 696e 6174 696f  :.    destinatio
+00000360: 6e20 3d20 746d 705f 7061 7468 202f 2022  n = tmp_path / "
+00000370: 7370 6563 5f74 7261 6469 7469 6f6e 616c  spec_traditional
+00000380: 220a 2020 2020 7368 7574 696c 2e63 6f70  ".    shutil.cop
+00000390: 7974 7265 6528 5350 4543 5f54 5241 4449  ytree(SPEC_TRADI
+000003a0: 5449 4f4e 414c 2c20 6465 7374 696e 6174  TIONAL, destinat
+000003b0: 696f 6e29 0a20 2020 2072 6574 7572 6e20  ion).    return 
+000003c0: 6465 7374 696e 6174 696f 6e20 2f20 5350  destination / SP
+000003d0: 4543 4649 4c45 0a0a 0a40 7079 7465 7374  ECFILE...@pytest
+000003e0: 2e66 6978 7475 7265 2873 636f 7065 3d22  .fixture(scope="
+000003f0: 6675 6e63 7469 6f6e 2229 0a64 6566 2073  function").def s
+00000400: 7065 635f 6175 746f 7365 7475 7028 746d  pec_autosetup(tm
+00000410: 705f 7061 7468 293a 0a20 2020 2064 6573  p_path):.    des
+00000420: 7469 6e61 7469 6f6e 203d 2074 6d70 5f70  tination = tmp_p
+00000430: 6174 6820 2f20 2273 7065 635f 6175 746f  ath / "spec_auto
+00000440: 7365 7475 7022 0a20 2020 2073 6875 7469  setup".    shuti
+00000450: 6c2e 636f 7079 7472 6565 2853 5045 435f  l.copytree(SPEC_
+00000460: 4155 544f 5345 5455 502c 2064 6573 7469  AUTOSETUP, desti
+00000470: 6e61 7469 6f6e 290a 2020 2020 7265 7475  nation).    retu
+00000480: 726e 2064 6573 7469 6e61 7469 6f6e 202f  rn destination /
+00000490: 2053 5045 4346 494c 450a 0a0a 4070 7974   SPECFILE...@pyt
+000004a0: 6573 742e 6669 7874 7572 6528 7363 6f70  est.fixture(scop
+000004b0: 653d 2266 756e 6374 696f 6e22 290a 6465  e="function").de
+000004c0: 6620 7370 6563 5f61 7574 6f70 6174 6368  f spec_autopatch
+000004d0: 2874 6d70 5f70 6174 6829 3a0a 2020 2020  (tmp_path):.    
+000004e0: 6465 7374 696e 6174 696f 6e20 3d20 746d  destination = tm
+000004f0: 705f 7061 7468 202f 2022 7370 6563 5f61  p_path / "spec_a
+00000500: 7574 6f70 6174 6368 220a 2020 2020 7368  utopatch".    sh
+00000510: 7574 696c 2e63 6f70 7974 7265 6528 5350  util.copytree(SP
+00000520: 4543 5f41 5554 4f50 4154 4348 2c20 6465  EC_AUTOPATCH, de
+00000530: 7374 696e 6174 696f 6e29 0a20 2020 2072  stination).    r
+00000540: 6574 7572 6e20 6465 7374 696e 6174 696f  eturn destinatio
+00000550: 6e20 2f20 5350 4543 4649 4c45 0a0a 0a40  n / SPECFILE...@
+00000560: 7079 7465 7374 2e66 6978 7475 7265 2873  pytest.fixture(s
+00000570: 636f 7065 3d22 6675 6e63 7469 6f6e 2229  cope="function")
+00000580: 0a64 6566 2073 7065 635f 7061 7463 686c  .def spec_patchl
+00000590: 6973 7428 746d 705f 7061 7468 293a 0a20  ist(tmp_path):. 
+000005a0: 2020 2064 6573 7469 6e61 7469 6f6e 203d     destination =
+000005b0: 2074 6d70 5f70 6174 6820 2f20 2273 7065   tmp_path / "spe
+000005c0: 635f 7061 7463 686c 6973 7422 0a20 2020  c_patchlist".   
+000005d0: 2073 6875 7469 6c2e 636f 7079 7472 6565   shutil.copytree
+000005e0: 2853 5045 435f 5041 5443 484c 4953 542c  (SPEC_PATCHLIST,
+000005f0: 2064 6573 7469 6e61 7469 6f6e 290a 2020   destination).  
+00000600: 2020 7265 7475 726e 2064 6573 7469 6e61    return destina
+00000610: 7469 6f6e 202f 2053 5045 4346 494c 450a  tion / SPECFILE.
+00000620: 0a0a 4070 7974 6573 742e 6669 7874 7572  ..@pytest.fixtur
+00000630: 6528 7363 6f70 653d 2266 756e 6374 696f  e(scope="functio
+00000640: 6e22 290a 6465 6620 7370 6563 5f69 6e63  n").def spec_inc
+00000650: 6c75 6465 7328 746d 705f 7061 7468 293a  ludes(tmp_path):
+00000660: 0a20 2020 2064 6573 7469 6e61 7469 6f6e  .    destination
+00000670: 203d 2074 6d70 5f70 6174 6820 2f20 2273   = tmp_path / "s
+00000680: 7065 635f 696e 636c 7564 6573 220a 2020  pec_includes".  
+00000690: 2020 7368 7574 696c 2e63 6f70 7974 7265    shutil.copytre
+000006a0: 6528 5350 4543 5f49 4e43 4c55 4445 532c  e(SPEC_INCLUDES,
+000006b0: 2064 6573 7469 6e61 7469 6f6e 290a 2020   destination).  
+000006c0: 2020 7265 7475 726e 2064 6573 7469 6e61    return destina
+000006d0: 7469 6f6e 202f 2053 5045 4346 494c 450a  tion / SPECFILE.
+000006e0: 0a0a 4070 7974 6573 742e 6669 7874 7572  ..@pytest.fixtur
+000006f0: 6528 7363 6f70 653d 2266 756e 6374 696f  e(scope="functio
+00000700: 6e22 290a 6465 6620 7370 6563 5f6d 6163  n").def spec_mac
+00000710: 726f 7328 746d 705f 7061 7468 293a 0a20  ros(tmp_path):. 
+00000720: 2020 2064 6573 7469 6e61 7469 6f6e 203d     destination =
+00000730: 2074 6d70 5f70 6174 6820 2f20 2273 7065   tmp_path / "spe
+00000740: 635f 6d61 6372 6f73 220a 2020 2020 7368  c_macros".    sh
+00000750: 7574 696c 2e63 6f70 7974 7265 6528 5350  util.copytree(SP
+00000760: 4543 5f4d 4143 524f 532c 2064 6573 7469  EC_MACROS, desti
+00000770: 6e61 7469 6f6e 290a 2020 2020 7265 7475  nation).    retu
+00000780: 726e 2064 6573 7469 6e61 7469 6f6e 202f  rn destination /
+00000790: 2053 5045 4346 494c 450a 0a0a 4070 7974   SPECFILE...@pyt
+000007a0: 6573 742e 6669 7874 7572 6528 7363 6f70  est.fixture(scop
+000007b0: 653d 2266 756e 6374 696f 6e22 290a 6465  e="function").de
+000007c0: 6620 7370 6563 5f6d 756c 7469 706c 655f  f spec_multiple_
+000007d0: 736f 7572 6365 7328 746d 705f 7061 7468  sources(tmp_path
+000007e0: 293a 0a20 2020 2064 6573 7469 6e61 7469  ):.    destinati
+000007f0: 6f6e 203d 2074 6d70 5f70 6174 6820 2f20  on = tmp_path / 
+00000800: 2273 7065 635f 6d75 6c74 6970 6c65 5f73  "spec_multiple_s
+00000810: 6f75 7263 6573 220a 2020 2020 7368 7574  ources".    shut
+00000820: 696c 2e63 6f70 7974 7265 6528 5350 4543  il.copytree(SPEC
+00000830: 5f4d 554c 5449 504c 455f 534f 5552 4345  _MULTIPLE_SOURCE
+00000840: 532c 2064 6573 7469 6e61 7469 6f6e 290a  S, destination).
+00000850: 2020 2020 7265 7475 726e 2064 6573 7469      return desti
+00000860: 6e61 7469 6f6e 202f 2053 5045 4346 494c  nation / SPECFIL
+00000870: 450a 0a0a 4070 7974 6573 742e 6669 7874  E...@pytest.fixt
+00000880: 7572 6528 7363 6f70 653d 2266 756e 6374  ure(scope="funct
+00000890: 696f 6e22 290a 6465 6620 7370 6563 5f63  ion").def spec_c
+000008a0: 6f6d 6d65 6e74 6564 5f70 6174 6368 6573  ommented_patches
+000008b0: 2874 6d70 5f70 6174 6829 3a0a 2020 2020  (tmp_path):.    
+000008c0: 6465 7374 696e 6174 696f 6e20 3d20 746d  destination = tm
+000008d0: 705f 7061 7468 202f 2022 7370 6563 5f63  p_path / "spec_c
+000008e0: 6f6d 6d65 6e74 6564 5f70 6174 6368 6573  ommented_patches
+000008f0: 220a 2020 2020 7368 7574 696c 2e63 6f70  ".    shutil.cop
+00000900: 7974 7265 6528 5350 4543 5f43 4f4d 4d45  ytree(SPEC_COMME
+00000910: 4e54 4544 5f50 4154 4348 4553 2c20 6465  NTED_PATCHES, de
+00000920: 7374 696e 6174 696f 6e29 0a20 2020 2072  stination).    r
+00000930: 6574 7572 6e20 6465 7374 696e 6174 696f  eturn destinatio
+00000940: 6e20 2f20 5350 4543 4649 4c45 0a0a 0a40  n / SPECFILE...@
+00000950: 7079 7465 7374 2e66 6978 7475 7265 2873  pytest.fixture(s
+00000960: 636f 7065 3d22 6675 6e63 7469 6f6e 2229  cope="function")
+00000970: 0a64 6566 2073 7065 635f 7368 656c 6c5f  .def spec_shell_
+00000980: 6578 7061 6e73 696f 6e73 2874 6d70 5f70  expansions(tmp_p
+00000990: 6174 6829 3a0a 2020 2020 6465 7374 696e  ath):.    destin
+000009a0: 6174 696f 6e20 3d20 746d 705f 7061 7468  ation = tmp_path
+000009b0: 202f 2022 7370 6563 5f73 6865 6c6c 5f65   / "spec_shell_e
+000009c0: 7870 616e 7369 6f6e 7322 0a20 2020 2073  xpansions".    s
+000009d0: 6875 7469 6c2e 636f 7079 7472 6565 2853  hutil.copytree(S
+000009e0: 5045 435f 5348 454c 4c5f 4558 5041 4e53  PEC_SHELL_EXPANS
+000009f0: 494f 4e53 2c20 6465 7374 696e 6174 696f  IONS, destinatio
+00000a00: 6e29 0a20 2020 2072 6574 7572 6e20 6465  n).    return de
+00000a10: 7374 696e 6174 696f 6e20 2f20 5350 4543  stination / SPEC
+00000a20: 4649 4c45 0a                             FILE.
```

### Comparing `specfile-0.9.0/tests/integration/test_specfile.py` & `specfile-0.9.1/tests/integration/test_specfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 import datetime
 import subprocess
 
 import pytest
 import rpm
 from flexmock import flexmock
 
-from specfile.exceptions import SpecfileException
+from specfile.exceptions import RPMException, SpecfileException
 from specfile.prep import AutopatchMacro, AutosetupMacro, PatchMacro, SetupMacro
 from specfile.sections import Section
 from specfile.specfile import Specfile
 
 
 def test_parse(spec_multiple_sources):
     spec = Specfile(spec_multiple_sources)
-    prep = spec._spec.prep
+    prep = spec._parser.spec.prep
     # remove all sources
     for path in spec.sourcedir.iterdir():
         if not path.samefile(spec.path):
             path.unlink()
     spec = Specfile(spec_multiple_sources)
-    assert spec._spec.prep == prep
+    assert spec._parser.spec.prep == prep
 
 
 def test_prep_traditional(spec_traditional):
     spec = Specfile(spec_traditional)
     with spec.prep() as prep:
         assert AutosetupMacro not in prep.macros
         assert AutopatchMacro not in prep.macros
@@ -208,20 +208,24 @@
     spec.set_version_and_release(version, release)
     assert spec.version == version
     assert spec.release == release
     assert spec.raw_release.startswith(release)
     with spec.tags() as tags:
         assert tags.version.value == spec.version
         assert tags.release.value == spec.raw_release
-    assert spec._spec.sourceHeader[rpm.RPMTAG_VERSION] == spec.expanded_version
-    assert spec._spec.sourceHeader[rpm.RPMTAG_RELEASE] == spec.expanded_raw_release
+    assert spec._parser.spec.sourceHeader[rpm.RPMTAG_VERSION] == spec.expanded_version
+    assert (
+        spec._parser.spec.sourceHeader[rpm.RPMTAG_RELEASE] == spec.expanded_raw_release
+    )
     spec.raw_release = release
     with spec.tags() as tags:
         assert tags.release.value == release
-    assert spec._spec.sourceHeader[rpm.RPMTAG_RELEASE] == spec.expanded_raw_release
+    assert (
+        spec._parser.spec.sourceHeader[rpm.RPMTAG_RELEASE] == spec.expanded_raw_release
+    )
 
 
 @pytest.mark.parametrize(
     "location, number, comment",
     [
         ("patchX.patch", None, None),
         ("patchX.patch", 0, None),
@@ -340,7 +344,34 @@
     spec2 = Specfile(spec_autosetup)
     spec1.version = "14.2"
     assert spec2.expanded_version == "0.1"
     with spec2.sources() as sources:
         assert sources[0].expanded_location == "test-0.1.tar.xz"
         sources.append("tests-%{version}.tar.xz")
         assert sources[1].expanded_location == "tests-0.1.tar.xz"
+
+
+def test_includes(spec_includes):
+    spec = Specfile(spec_includes)
+    assert not spec.tainted
+    with spec.patches() as patches:
+        assert not patches
+    assert spec.expand("%patches")
+    with spec.sections() as sections:
+        assert sections.description[0] == "%include %{SOURCE2}"
+    for inc in ["patches.inc", "description.inc"]:
+        (spec.sourcedir / inc).unlink()
+    with pytest.raises(RPMException):
+        spec = Specfile(spec_includes)
+    spec = Specfile(spec_includes, ignore_missing_includes=True)
+    assert spec.tainted
+    with spec.patches() as patches:
+        assert not patches
+    assert not spec.expand("%patches")
+    with spec.sections() as sections:
+        assert sections.description[0] == "%include %{SOURCE2}"
+
+
+def test_shell_expansions(spec_shell_expansions):
+    spec = Specfile(spec_shell_expansions)
+    assert spec.expanded_version == "1035.4200"
+    assert "C.UTF-8" in spec.expand("%numeric_locale")
```

### Comparing `specfile-0.9.0/tests/unit/test_changelog.py` & `specfile-0.9.1/tests/unit/test_changelog.py`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/tests/unit/test_macro_definitions.py` & `specfile-0.9.1/tests/unit/test_macro_definitions.py`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/tests/unit/test_macro_options.py` & `specfile-0.9.1/tests/unit/test_macro_options.py`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/tests/unit/test_prep.py` & `specfile-0.9.1/tests/unit/test_prep.py`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/tests/unit/test_rpm.py` & `specfile-0.9.1/tests/unit/test_rpm.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 import pytest
 import rpm
 from flexmock import flexmock
 
 from specfile.exceptions import MacroRemovalException
-from specfile.rpm import RPM, Macro, MacroLevel, Macros
+from specfile.rpm import Macro, MacroLevel, Macros, SpecParser
 
 
 def test_macros_parse():
     assert Macros._parse(
         [
             "-20= dump\t<builtin>\n",
             "-20: echo\t<builtin>\n",
@@ -105,28 +105,27 @@
 
 
 def test_macros_reinit():
     Macros.reinit(MacroLevel.BUILTIN)
     assert all(m.level == MacroLevel.BUILTIN for m in Macros.dump())
 
 
-def test_rpm_parse():
-    spec = RPM.parse(
+def test_spec_parser_do_parse():
+    parser = SpecParser(Path("."), [("dist", ".fc35")])
+    spec, _ = parser._do_parse(
         (
             "Name:           test\n"
             "Version:        0.1\n"
             "Release:        1%{?dist}\n"
             "Summary:        Test package\n"
             "License:        MIT\n"
             "\n"
             "%description\n"
             "Test package\n"
         ),
-        Path("."),
-        macros=[("dist", ".fc35")],
     )
     assert spec.sourceHeader[rpm.RPMTAG_NAME] == "test"
     assert spec.sourceHeader[rpm.RPMTAG_VERSION] == "0.1"
     assert spec.sourceHeader[rpm.RPMTAG_RELEASE] == "1.fc35"
     assert spec.sourceHeader[rpm.RPMTAG_SUMMARY] == "Test package"
     assert spec.sourceHeader[rpm.RPMTAG_LICENSE] == "MIT"
     assert spec.prep is None
```

### Comparing `specfile-0.9.0/tests/unit/test_sections.py` & `specfile-0.9.1/tests/unit/test_sections.py`

 * *Files 26% similar despite different names*

```diff
@@ -63,11 +63,27 @@
     assert sections[0][0] == "0"
     assert sections[1].name == "Prep"
     assert sections.prep == ["0", "1", "2", ""]
     assert sections[2].name == "pAckage x"
     assert sections[2] == ["Requires: bar"]
 
 
+def test_parse_invalid_name():
+    sections = Sections.parse(
+        [
+            "%description",
+            "This is a description.",
+            "",
+            "%description(fr)",
+            "Ceci est une description.",
+            "",
+        ]
+    )
+    assert len(sections) == 2  # including empty preamble
+    assert sections[1].name == "description"
+    assert sections.description[2] == "%description(fr)"
+
+
 def test_copy_sections():
     sections = Sections([Section("package"), Section("package bar")])
     sections_copy = copy.deepcopy(sections)
     assert sections == sections_copy
```

### Comparing `specfile-0.9.0/tests/unit/test_sourcelist.py` & `specfile-0.9.1/tests/unit/test_sourcelist.py`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/tests/unit/test_sources.py` & `specfile-0.9.1/tests/unit/test_sources.py`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/tests/unit/test_specfile.py` & `specfile-0.9.1/tests/unit/test_specfile.py`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/tests/unit/test_tags.py` & `specfile-0.9.1/tests/unit/test_tags.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,14 +36,17 @@
                 "Version: %{ver_major}.%{ver_minor}",
                 "  # this is a valid comment",
                 "Release: 1%{?dist}",
                 "",
                 "%if 0",
                 "Epoch:   1",
                 "%endif",
+                "",
+                "Requires:          make",
+                "Requires(post):    bash",
             ],
         ),
         Section(
             "package",
             [
                 "",
                 "",
@@ -54,28 +57,34 @@
                 "Version: 1.0",
                 "  # this is a valid comment",
                 "Release: 1.fc35",
                 "",
                 "",
                 "",
                 "",
+                "",
+                "Requires:          make",
+                "Requires(post):    bash",
             ],
         ),
     )
     assert tags[0].name == "Name"
     assert tags[0].comments[0].text == "this is a test package"
     assert tags[0].comments[1].text == "not to be used in production"
     assert tags[1].name == "Version"
     assert tags[1].value == "%{ver_major}.%{ver_minor}"
     assert tags[1].valid
     assert tags[1].expanded_value == "1.0"
     assert not tags[1].comments
     assert tags.release.comments[0].prefix == "  # "
     assert tags.epoch.name == "Epoch"
     assert not tags.epoch.valid
+    assert tags.requires.value == "make"
+    assert "requires(post)" in tags
+    assert tags[-1].name == "Requires(post)"
 
 
 def test_get_raw_section_data():
     tags = Tags(
         [
             Tag(
                 "Name",
@@ -95,16 +104,20 @@
                 "Release",
                 "1%{?dist}",
                 "1.fc35",
                 ": ",
                 Comments([Comment("this is a valid comment", "  # ")]),
             ),
             Tag("Epoch", "1", "", ":   ", Comments([], ["", "%if 0"])),
+            Tag(
+                "Requires", "make", "make", ":          ", Comments([], ["%endif", ""])
+            ),
+            Tag("Requires(post)", "bash", "bash", ":    ", Comments()),
         ],
-        ["%endif"],
+        [],
     )
     assert tags.get_raw_section_data() == [
         "%global ver_major 1",
         "%global ver_minor 0",
         "",
         "# this is a test package",
         "# not to be used in production",
@@ -112,14 +125,17 @@
         "Version: %{ver_major}.%{ver_minor}",
         "  # this is a valid comment",
         "Release: 1%{?dist}",
         "",
         "%if 0",
         "Epoch:   1",
         "%endif",
+        "",
+        "Requires:          make",
+        "Requires(post):    bash",
     ]
 
 
 def test_copy_tags():
     tags = Tags(
         [
             Tag("Name", "test", "test", ": ", Comments()),
```

### Comparing `specfile-0.9.0/tests/unit/test_utils.py` & `specfile-0.9.1/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `specfile-0.9.0/tests/unit/test_value_parser.py` & `specfile-0.9.1/tests/unit/test_value_parser.py`

 * *Files identical despite different names*

