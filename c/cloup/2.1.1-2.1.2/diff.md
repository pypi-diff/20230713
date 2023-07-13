# Comparing `tmp/cloup-2.1.1.tar.gz` & `tmp/cloup-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cloup/cloup/dist/.tmp-gwe3sspa/cloup-2.1.1.tar", last modified: Sat Jun  3 14:20:39 2023, max compression
+gzip compressed data, was "/home/runner/work/cloup/cloup/dist/.tmp-p7cmlzgt/cloup-2.1.2.tar", last modified: Thu Jul 13 18:09:55 2023, max compression
```

## Comparing `cloup-2.1.1.tar` & `cloup-2.1.2.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-03 14:20:28.000000 cloup-2.1.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 14:20:28.000000 cloup-2.1.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-03 14:20:28.000000 cloup-2.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-03 14:20:28.000000 cloup-2.1.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-03 14:20:28.000000 cloup-2.1.1/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-03 14:20:28.000000 cloup-2.1.1/.github/ISSUE_TEMPLATE/other.md
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-03 14:20:28.000000 cloup-2.1.1/.github/release.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-03 14:20:28.000000 cloup-2.1.1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-03 14:20:28.000000 cloup-2.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-03 14:20:28.000000 cloup-2.1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-06-03 14:20:28.000000 cloup-2.1.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-03 14:20:28.000000 cloup-2.1.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-03 14:20:28.000000 cloup-2.1.1/CREDITS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-03 14:20:28.000000 cloup-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-03 14:20:28.000000 cloup-2.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-06-03 14:20:39.000000 cloup-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-06-03 14:20:28.000000 cloup-2.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup/
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29113 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/_option_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/_params.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/_sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/constraints/_conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/constraints/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/constraints/_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/constraints/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/constraints/conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/constraints/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup/formatting/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17385 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/formatting/_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/formatting/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/formatting/sep.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/styling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-03 14:20:28.000000 cloup-2.1.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/docs/_autoapi_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/docs/_autoapi_templates/python/
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/_autoapi_templates/python/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    57493 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/_static/basic-example.png
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/_static/logo-dark-mode.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/_static/logo-on-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/docs/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/_static/styles/extensions-overrides.css
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/_static/styles/theme-overrides.css
--rw-r--r--   0 runner    (1001) docker     (123)    62855 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/_static/theme-elems.png
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/docs/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/aliases.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/arguments.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    20026 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/constraints.rst
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/credits.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13553 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/formatting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/misc.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/option-groups.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/sections.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-03 14:20:28.000000 cloup-2.1.1/examples/arguments_with_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-03 14:20:28.000000 cloup-2.1.1/examples/default_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-03 14:20:28.000000 cloup-2.1.1/examples/flat_option_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-06-03 14:20:28.000000 cloup-2.1.1/examples/git_sections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/examples/manim/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-03 14:20:28.000000 cloup-2.1.1/examples/manim/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-03 14:20:28.000000 cloup-2.1.1/examples/manim/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-03 14:20:28.000000 cloup-2.1.1/examples/manim/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-03 14:20:28.000000 cloup-2.1.1/examples/option_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 14:20:28.000000 cloup-2.1.1/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-06-03 14:20:28.000000 cloup-2.1.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-03 14:20:28.000000 cloup-2.1.1/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-03 14:20:28.000000 cloup-2.1.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 14:20:28.000000 cloup-2.1.1/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-03 14:20:28.000000 cloup-2.1.1/requirements/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-03 14:20:28.000000 cloup-2.1.1/scripts/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-03 14:20:28.000000 cloup-2.1.1/scripts/copytree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-06-03 14:20:28.000000 cloup-2.1.1/scripts/generate_git_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-03 14:20:28.000000 cloup-2.1.1/scripts/make-help.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-03 14:20:28.000000 cloup-2.1.1/scripts/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-03 14:20:39.000000 cloup-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-03 14:20:28.000000 cloup-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/tests/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/constraints/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/constraints/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/constraints/test_conditional_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    14505 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/constraints/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/constraints/test_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/example_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/example_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/test_aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/test_option_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/test_sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/test_sep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/test_styling.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-03 14:20:28.000000 cloup-2.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:55.000000 cloup-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-13 18:09:42.000000 cloup-2.1.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 18:09:42.000000 cloup-2.1.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:55.000000 cloup-2.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:55.000000 cloup-2.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-13 18:09:42.000000 cloup-2.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-13 18:09:42.000000 cloup-2.1.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-13 18:09:42.000000 cloup-2.1.2/.github/ISSUE_TEMPLATE/enhancement.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 18:09:42.000000 cloup-2.1.2/.github/ISSUE_TEMPLATE/other.md
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-13 18:09:42.000000 cloup-2.1.2/.github/release.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:55.000000 cloup-2.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-13 18:09:42.000000 cloup-2.1.2/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-13 18:09:42.000000 cloup-2.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-13 18:09:42.000000 cloup-2.1.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-07-13 18:09:42.000000 cloup-2.1.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-13 18:09:42.000000 cloup-2.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-13 18:09:42.000000 cloup-2.1.2/CREDITS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-13 18:09:42.000000 cloup-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-13 18:09:42.000000 cloup-2.1.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-07-13 18:09:55.000000 cloup-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-07-13 18:09:42.000000 cloup-2.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:55.000000 cloup-2.1.2/cloup/
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29445 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/_option_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/_params.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/_sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 18:09:55.000000 cloup-2.1.2/cloup/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:55.000000 cloup-2.1.2/cloup/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/constraints/_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/constraints/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/constraints/_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/constraints/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/constraints/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/constraints/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:55.000000 cloup-2.1.2/cloup/formatting/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17385 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/formatting/_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/formatting/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/formatting/sep.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/styling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-13 18:09:42.000000 cloup-2.1.2/cloup/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:55.000000 cloup-2.1.2/cloup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-07-13 18:09:55.000000 cloup-2.1.2/cloup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-13 18:09:55.000000 cloup-2.1.2/cloup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:09:55.000000 cloup-2.1.2/cloup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:09:55.000000 cloup-2.1.2/cloup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-13 18:09:55.000000 cloup-2.1.2/cloup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 18:09:55.000000 cloup-2.1.2/cloup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-13 18:09:42.000000 cloup-2.1.2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:55.000000 cloup-2.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:55.000000 cloup-2.1.2/docs/_autoapi_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:55.000000 cloup-2.1.2/docs/_autoapi_templates/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/_autoapi_templates/python/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:55.000000 cloup-2.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    57493 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/_static/basic-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/_static/logo-dark-mode.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/_static/logo-on-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:55.000000 cloup-2.1.2/docs/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/_static/styles/extensions-overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/_static/styles/theme-overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)    62855 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/_static/theme-elems.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:55.000000 cloup-2.1.2/docs/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/pages/aliases.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/pages/arguments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/pages/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20026 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/pages/constraints.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/pages/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/pages/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13553 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/pages/formatting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/pages/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/pages/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/pages/option-groups.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-07-13 18:09:42.000000 cloup-2.1.2/docs/pages/sections.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:55.000000 cloup-2.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-13 18:09:42.000000 cloup-2.1.2/examples/arguments_with_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-13 18:09:42.000000 cloup-2.1.2/examples/default_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-13 18:09:42.000000 cloup-2.1.2/examples/flat_option_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-13 18:09:42.000000 cloup-2.1.2/examples/git_sections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:55.000000 cloup-2.1.2/examples/manim/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-13 18:09:42.000000 cloup-2.1.2/examples/manim/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-13 18:09:42.000000 cloup-2.1.2/examples/manim/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-13 18:09:42.000000 cloup-2.1.2/examples/manim/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-13 18:09:42.000000 cloup-2.1.2/examples/option_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:55.000000 cloup-2.1.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 18:09:42.000000 cloup-2.1.2/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-13 18:09:42.000000 cloup-2.1.2/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-13 18:09:42.000000 cloup-2.1.2/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-13 18:09:42.000000 cloup-2.1.2/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 18:09:42.000000 cloup-2.1.2/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-13 18:09:42.000000 cloup-2.1.2/requirements/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:55.000000 cloup-2.1.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-13 18:09:42.000000 cloup-2.1.2/scripts/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-13 18:09:42.000000 cloup-2.1.2/scripts/copytree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-07-13 18:09:42.000000 cloup-2.1.2/scripts/generate_git_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-13 18:09:42.000000 cloup-2.1.2/scripts/make-help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-13 18:09:42.000000 cloup-2.1.2/scripts/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-13 18:09:55.000000 cloup-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-13 18:09:42.000000 cloup-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:55.000000 cloup-2.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:55.000000 cloup-2.1.2/tests/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/constraints/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/constraints/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/constraints/test_conditional_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14505 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/constraints/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/constraints/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/example_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/example_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/test_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/test_option_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/test_sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/test_sep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/test_styling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-13 18:09:42.000000 cloup-2.1.2/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-13 18:09:42.000000 cloup-2.1.2/tox.ini
```

### Comparing `cloup-2.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `cloup-2.1.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/.github/workflows/tests.yaml` & `cloup-2.1.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/.gitignore` & `cloup-2.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/CHANGELOG.rst` & `cloup-2.1.2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/CONTRIBUTING.rst` & `cloup-2.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/CREDITS.rst` & `cloup-2.1.2/CREDITS.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/LICENSE` & `cloup-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/Makefile` & `cloup-2.1.2/Makefile`

 * *Files 18% similar despite different names*

```diff
@@ -104,25 +104,27 @@
 release: dist ## package and upload a release
 	twine upload dist/*
 
 .PHONY: test-release
 test-release: dist   ## package and upload a release
 	twine upload --repository testpypi dist/*
 
+PIP_COMPILE := pip-compile --resolver=backtracking
+
 .PHONY: pip-compile
 pip-compile:  ## pin dependencies in requirements/ using the current env
-	pip-compile requirements/test.in
-	pip-compile requirements/docs.in
-	pip-compile requirements/dev.in
+	$(PIP_COMPILE) requirements/test.in
+	$(PIP_COMPILE) requirements/docs.in
+	$(PIP_COMPILE) requirements/dev.in
 
 .PHONY: pip-upgrade
 pip-upgrade:   ## upgrade pip and dependencies
 	python -m pip install -U pip
-	pip-compile --upgrade requirements/test.in
-	pip-compile --upgrade requirements/docs.in
-	pip-compile --upgrade requirements/dev.in
+	$(PIP_COMPILE) --upgrade requirements/test.in
+	# $(PIP_COMPILE) --upgrade requirements/docs.in
+	$(PIP_COMPILE) --upgrade requirements/dev.in
 
 .PHONY: pip-sync
 pip-sync:  ## sync development environment with requirements/dev.txt
 	pip install -U pip-tools
 	pip-sync requirements/dev.txt
 	pip install -e .
```

### Comparing `cloup-2.1.1/PKG-INFO` & `cloup-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloup
-Version: 2.1.1
+Version: 2.1.2
 Summary: Adds features to Click: option groups, constraints, subcommand sections and help themes.
 Home-page: https://github.com/janLuke/cloup
 Author: Gianluca Gippetto
 Author-email: gianluca.gippetto@gmail.com
 License: BSD 3-Clause
 Keywords: CLI,click,argument groups,option groups,constraints,help colors,help themes,help styles
 Classifier: Intended Audience :: Developers
```

### Comparing `cloup-2.1.1/README.rst` & `cloup-2.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup/__init__.py` & `cloup-2.1.2/cloup/__init__.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup/_commands.py` & `cloup-2.1.2/cloup/_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,38 +13,39 @@
 https://github.com/python/mypy/issues/3737.
 So I had to resort to a workaround using @overload which makes things more
 verbose. The ``@overload`` is on the ``cls`` argument:
 
 - in one signature, ``cls`` has type ``None`` and it's set to ``None``; in this
   case the type of the instantiated command is ``cloup.Command`` for ``@command``
   and ``cloup.Group`` for ``@group``
-- in the other signature, there's ``cls: ClickCommand`` without a default, where
-  ``ClickCommand`` is a type variable.
+- in the other signature, there's ``cls: C`` without a default, where ``C`` is
+  a type variable; in this case the type of the instantiated command is ``C``.
 
 When and if the MyPy issue is resolved, the overloads will be removed.
 """
 import inspect
 from typing import (
     Any, Callable, Dict, Iterable, List, NamedTuple, Optional, Sequence, Tuple,
-    Type, TypeVar, Union, cast, overload,
+    Type, TypeVar, Union, cast, overload
 )
 
 import click
 
 import cloup
 from ._context import Context
 from ._option_groups import OptionGroupMixin
 from ._sections import Section, SectionMixin
 from ._util import click_version_ge_8_1, first_bool, reindent
 from .constraints import ConstraintMixin
 from .styling import DEFAULT_THEME
 from .typing import AnyCallable
 
-ClickCommand = TypeVar('ClickCommand', bound=click.Command)
-ClickGroup = TypeVar('ClickGroup', bound=click.Group)
+# Generic types of ``cls`` args of ``@command`` and ``@group``
+C = TypeVar('C', bound=click.Command)
+G = TypeVar('G', bound=click.Group)
 
 
 class Command(ConstraintMixin, OptionGroupMixin, click.Command):
     """A ``click.Command`` supporting option groups and constraints.
 
     Refer to superclasses for the documentation of all accepted parameters:
 
@@ -252,74 +253,77 @@
     # The supertype signature is (*args, **kwargs), which is compatible with
     # this provided that you pass all arguments (expect "name") as keyword arg.
     @overload  # type: ignore
     def command(  # Why overloading? Refer to module docstring.
         self, name: Optional[str] = None,
         *,
         aliases: Optional[Iterable[str]] = None,
-        cls: None = None,  # Command is cloup.Command
+        cls: None = None,  # default to Group.command_class or cloup.Command
         section: Optional[Section] = None,
         context_settings: Optional[Dict[str, Any]] = None,
         formatter_settings: Optional[Dict[str, Any]] = None,
         help: Optional[str] = None,
         epilog: Optional[str] = None,
         short_help: Optional[str] = None,
         options_metavar: Optional[str] = "[OPTIONS]",
         add_help_option: bool = True,
         no_args_is_help: bool = False,
         hidden: bool = False,
         deprecated: bool = False,
         align_option_groups: Optional[bool] = None,
         show_constraints: Optional[bool] = None,
         params: Optional[List[click.Parameter]] = None,
-    ) -> Callable[[AnyCallable], Command]:
+    ) -> Callable[[AnyCallable], click.Command]:
         ...
 
     @overload
     def command(  # Why overloading? Refer to module docstring.
         self, name: Optional[str] = None,
         *,
         aliases: Optional[Iterable[str]] = None,
-        cls: Type[ClickCommand],
+        cls: Type[C],
         section: Optional[Section] = None,
         context_settings: Optional[Dict[str, Any]] = None,
         help: Optional[str] = None,
         epilog: Optional[str] = None,
         short_help: Optional[str] = None,
         options_metavar: Optional[str] = "[OPTIONS]",
         add_help_option: bool = True,
         no_args_is_help: bool = False,
         hidden: bool = False,
         deprecated: bool = False,
         params: Optional[List[click.Parameter]] = None,
         **kwargs: Any,
-    ) -> Callable[[AnyCallable], ClickCommand]:
+    ) -> Callable[[AnyCallable], C]:
         ...
 
     def command(
         self, name: Optional[str] = None, *,
         aliases: Optional[Iterable[str]] = None,
-        cls: Optional[Type[ClickCommand]] = None,
+        cls: Optional[Type[C]] = None,
         section: Optional[Section] = None,
         **kwargs: Any
-    ) -> Callable[[AnyCallable], Union[Command, ClickCommand]]:
+    ) -> Callable[[AnyCallable], Union[click.Command, C]]:
         """Return a decorator that creates a new subcommand of this ``Group``
         using the decorated function as callback.
 
         It takes the same arguments of :func:`command` plus:
 
         ``section``: ``Optional[Section]``
             if provided, put the subcommand in this section.
 
         .. versionchanged:: 0.10.0
             all arguments but ``name`` are now keyword-only.
         """
-        make_command = command(name=name, cls=cls, aliases=aliases, **kwargs)
+        make_command = command(
+            name=name, cls=(self.command_class if cls is None else cls),
+            aliases=aliases, **kwargs
+        )
 
-        def decorator(f: AnyCallable) -> Union[Command, ClickCommand]:
+        def decorator(f: AnyCallable) -> click.Command:
             cmd = make_command(f)
             self.add_command(cmd, section=section)
             return cmd
 
         return decorator
 
     # MyPy complains because "Signature of "group" incompatible with supertype".
@@ -343,22 +347,22 @@
         short_help: Optional[str] = None,
         options_metavar: Optional[str] = "[OPTIONS]",
         subcommand_metavar: Optional[str] = None,
         add_help_option: bool = True,
         chain: bool = False,
         hidden: bool = False,
         deprecated: bool = False,
-    ) -> Callable[[AnyCallable], 'Group']:
+    ) -> Callable[[AnyCallable], click.Group]:
         ...
 
     @overload
     def group(  # Why overloading? Refer to module docstring.
         self, name: Optional[str] = None, *,
         aliases: Optional[Iterable[str]] = None,
-        cls: Type[ClickGroup],
+        cls: Optional[Type[G]] = None,
         section: Optional[Section] = None,
         invoke_without_command: bool = False,
         no_args_is_help: bool = False,
         context_settings: Optional[Dict[str, Any]] = None,
         help: Optional[str] = None,
         epilog: Optional[str] = None,
         short_help: Optional[str] = None,
@@ -366,45 +370,56 @@
         subcommand_metavar: Optional[str] = None,
         add_help_option: bool = True,
         chain: bool = False,
         hidden: bool = False,
         deprecated: bool = False,
         params: Optional[List[click.Parameter]] = None,
         **kwargs: Any
-    ) -> Callable[[AnyCallable], ClickGroup]:
+    ) -> Callable[[AnyCallable], G]:
         ...
 
     def group(  # type: ignore
         self, name: Optional[None] = None,
         *,
-        cls: Optional[Type[ClickGroup]] = None,
+        cls: Optional[Type[G]] = None,
         aliases: Optional[Iterable[str]] = None,
         section: Optional[Section] = None,
         **kwargs: Any
-    ) -> Callable[[AnyCallable], Union["Group", ClickGroup]]:
+    ) -> Callable[[AnyCallable], Union[click.Group, G]]:
         """Return a decorator that creates a new subcommand of this ``Group``
         using the decorated function as callback.
 
         It takes the same argument of :func:`group` plus:
 
         ``section``: ``Optional[Section]``
             if provided, put the subcommand in this section.
 
         .. versionchanged:: 0.10.0
             all arguments but ``name`` are now keyword-only.
         """
-        make_group = group(name=name, cls=cls, aliases=aliases, **kwargs)
+        make_group = group(
+            name=name, cls=cls or self._default_group_class(), aliases=aliases, **kwargs
+        )
 
-        def decorator(f: AnyCallable) -> Union["Group", ClickGroup]:
+        def decorator(f: AnyCallable) -> Union[click.Group, G]:
             cmd = make_group(f)
             self.add_command(cmd, section=section)
             return cmd
 
         return decorator
 
+    @classmethod
+    def _default_group_class(cls) -> Optional[Type[click.Group]]:
+        if cls.group_class is None:
+            return None
+        if cls.group_class is type:
+            return cls
+        else:
+            return cast(Type[click.Group], cls.group_class)
+
 
 # Why overloading? Refer to module docstring.
 @overload  # In this overload: "cls: None = None"
 def command(
     name: Optional[str] = None,
     *,
     aliases: Optional[Iterable[str]] = None,
@@ -427,37 +442,37 @@
 
 
 @overload
 def command(  # In this overload: "cls: ClickCommand"
     name: Optional[str] = None,
     *,
     aliases: Optional[Iterable[str]] = None,
-    cls: Type[ClickCommand],
+    cls: Type[C],
     context_settings: Optional[Dict[str, Any]] = None,
     help: Optional[str] = None,
     short_help: Optional[str] = None,
     epilog: Optional[str] = None,
     options_metavar: Optional[str] = "[OPTIONS]",
     add_help_option: bool = True,
     no_args_is_help: bool = False,
     hidden: bool = False,
     deprecated: bool = False,
     params: Optional[List[click.Parameter]] = None,
     **kwargs: Any
-) -> Callable[[AnyCallable], ClickCommand]:
+) -> Callable[[AnyCallable], C]:
     ...
 
 
 # noinspection PyIncorrectDocstring
 def command(
     name: Optional[str] = None, *,
     aliases: Optional[Iterable[str]] = None,
-    cls: Optional[Type[ClickCommand]] = None,
+    cls: Optional[Type[C]] = None,
     **kwargs: Any
-) -> Callable[[AnyCallable], Union[Command, ClickCommand]]:
+) -> Callable[[AnyCallable], Union[Command, C]]:
     """
     Return a decorator that creates a new command using the decorated function
     as callback.
 
     The only differences with respect to ``click.command`` are:
 
     - the default command class is :class:`cloup.Command`
@@ -534,27 +549,27 @@
     """
     if callable(name):
         raise Exception(
             f"you forgot parenthesis in the command decorator for `{name.__name__}`. "
             f"While parenthesis are optional in Click >= 8.1, they are required in Cloup."
         )
 
-    def decorator(f: AnyCallable) -> ClickCommand:
+    def decorator(f: AnyCallable) -> C:
         if hasattr(f, '__cloup_constraints__'):
             if cls and not issubclass(cls, ConstraintMixin):
                 raise TypeError(
                     f"a `Command` must inherit from `cloup.ConstraintMixin` to support "
                     f"constraints; `{cls}` doesn't")
             constraints = tuple(reversed(f.__cloup_constraints__))
             del f.__cloup_constraints__
             kwargs['constraints'] = constraints
 
         cmd_cls = cls if cls is not None else Command
         try:
-            cmd = cast(ClickCommand, click.command(name, cls=cmd_cls, **kwargs)(f))
+            cmd = cast(C, click.command(name, cls=cmd_cls, **kwargs)(f))
             if aliases:
                 cmd.aliases = list(aliases)  # type: ignore
             return cmd
         except TypeError as error:
             raise _process_unexpected_kwarg_error(error, _ARGS_INFO, cmd_cls)
 
     return decorator
@@ -586,15 +601,15 @@
     ...
 
 
 @overload
 def group(
     name: Optional[str] = None,
     *,
-    cls: Type[ClickGroup],
+    cls: Type[G],
     aliases: Optional[Iterable[str]] = None,
     invoke_without_command: bool = False,
     no_args_is_help: bool = False,
     context_settings: Optional[Dict[str, Any]] = None,
     help: Optional[str] = None,
     short_help: Optional[str] = None,
     epilog: Optional[str] = None,
@@ -602,20 +617,20 @@
     subcommand_metavar: Optional[str] = None,
     add_help_option: bool = True,
     chain: bool = False,
     hidden: bool = False,
     deprecated: bool = False,
     params: Optional[List[click.Parameter]] = None,
     **kwargs: Any
-) -> Callable[[AnyCallable], ClickGroup]:
+) -> Callable[[AnyCallable], G]:
     ...
 
 
 def group(
-    name: Optional[str] = None, *, cls: Optional[Type[ClickGroup]] = None, **kwargs: Any
+    name: Optional[str] = None, *, cls: Optional[Type[G]] = None, **kwargs: Any
 ) -> Callable[[AnyCallable], click.Group]:
     """
     Return a decorator that instantiates a ``Group`` (or a subclass of it)
     using the decorated function as callback.
 
     .. versionchanged:: 0.10.0
         the ``cls`` argument can now be any ``click.Group`` (previously had to
```

### Comparing `cloup-2.1.1/cloup/_context.py` & `cloup-2.1.2/cloup/_context.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup/_option_groups.py` & `cloup-2.1.2/cloup/_option_groups.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup/_params.py` & `cloup-2.1.2/cloup/_params.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup/_params.pyi` & `cloup-2.1.2/cloup/_params.pyi`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup/_sections.py` & `cloup-2.1.2/cloup/_sections.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup/_util.py` & `cloup-2.1.2/cloup/_util.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup/constraints/__init__.py` & `cloup-2.1.2/cloup/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup/constraints/_conditional.py` & `cloup-2.1.2/cloup/constraints/_conditional.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup/constraints/_core.py` & `cloup-2.1.2/cloup/constraints/_core.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup/constraints/_support.py` & `cloup-2.1.2/cloup/constraints/_support.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup/constraints/common.py` & `cloup-2.1.2/cloup/constraints/common.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup/constraints/conditions.py` & `cloup-2.1.2/cloup/constraints/conditions.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup/constraints/exceptions.py` & `cloup-2.1.2/cloup/constraints/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup/formatting/_formatter.py` & `cloup-2.1.2/cloup/formatting/_formatter.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup/formatting/_util.py` & `cloup-2.1.2/cloup/formatting/_util.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup/formatting/sep.py` & `cloup-2.1.2/cloup/formatting/sep.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup/styling.py` & `cloup-2.1.2/cloup/styling.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup/types.py` & `cloup-2.1.2/cloup/types.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup/typing.py` & `cloup-2.1.2/cloup/typing.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/cloup.egg-info/PKG-INFO` & `cloup-2.1.2/cloup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloup
-Version: 2.1.1
+Version: 2.1.2
 Summary: Adds features to Click: option groups, constraints, subcommand sections and help themes.
 Home-page: https://github.com/janLuke/cloup
 Author: Gianluca Gippetto
 Author-email: gianluca.gippetto@gmail.com
 License: BSD 3-Clause
 Keywords: CLI,click,argument groups,option groups,constraints,help colors,help themes,help styles
 Classifier: Intended Audience :: Developers
```

### Comparing `cloup-2.1.1/cloup.egg-info/SOURCES.txt` & `cloup-2.1.2/cloup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/docs/Makefile` & `cloup-2.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/docs/_autoapi_templates/python/module.rst` & `cloup-2.1.2/docs/_autoapi_templates/python/module.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/docs/_static/basic-example.png` & `cloup-2.1.2/docs/_static/basic-example.png`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/docs/_static/logo-dark-mode.svg` & `cloup-2.1.2/docs/_static/logo-dark-mode.svg`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/docs/_static/logo-on-white.svg` & `cloup-2.1.2/docs/_static/logo-on-white.svg`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/docs/_static/logo.svg` & `cloup-2.1.2/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/docs/_static/styles/extensions-overrides.css` & `cloup-2.1.2/docs/_static/styles/extensions-overrides.css`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/docs/_static/styles/theme-overrides.css` & `cloup-2.1.2/docs/_static/styles/theme-overrides.css`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/docs/_static/theme-elems.png` & `cloup-2.1.2/docs/_static/theme-elems.png`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/docs/conf.py` & `cloup-2.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/docs/index.rst` & `cloup-2.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/docs/make.bat` & `cloup-2.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/docs/pages/aliases.rst` & `cloup-2.1.2/docs/pages/aliases.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/docs/pages/arguments.rst` & `cloup-2.1.2/docs/pages/arguments.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/docs/pages/constraints.rst` & `cloup-2.1.2/docs/pages/constraints.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/docs/pages/formatting.rst` & `cloup-2.1.2/docs/pages/formatting.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/docs/pages/installation.rst` & `cloup-2.1.2/docs/pages/installation.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/docs/pages/option-groups.rst` & `cloup-2.1.2/docs/pages/option-groups.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/docs/pages/sections.rst` & `cloup-2.1.2/docs/pages/sections.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/examples/arguments_with_help.py` & `cloup-2.1.2/examples/arguments_with_help.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/examples/default_command.py` & `cloup-2.1.2/examples/default_command.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/examples/flat_option_groups.py` & `cloup-2.1.2/examples/flat_option_groups.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/examples/git_sections.py` & `cloup-2.1.2/examples/git_sections.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/examples/manim/config.py` & `cloup-2.1.2/examples/manim/config.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/examples/manim/main.py` & `cloup-2.1.2/examples/manim/main.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/examples/manim/render.py` & `cloup-2.1.2/examples/manim/render.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/examples/option_groups.py` & `cloup-2.1.2/examples/option_groups.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/requirements/dev.txt` & `cloup-2.1.2/requirements/dev.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,277 +1,277 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
-#    pip-compile 'requirements\dev.in'
+#    pip-compile --resolver=backtracking requirements/dev.in
 #
-alabaster==0.7.12
+alabaster==0.7.13
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   sphinx
-astroid==2.12.2
+astroid==2.15.6
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   sphinx-autoapi
-atomicwrites==1.4.1
+babel==2.12.1
     # via
-    #   -r requirements\test.txt
-    #   pytest
-attrs==21.4.0
-    # via
-    #   -r requirements\test.txt
-    #   pytest
-babel==2.10.3
-    # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   sphinx
-beautifulsoup4==4.11.1
+beautifulsoup4==4.12.2
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   furo
-bleach==5.0.1
+bleach==6.0.0
     # via readme-renderer
-certifi==2022.6.15
+certifi==2023.5.7
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   requests
-charset-normalizer==2.1.0
+cffi==1.15.1
+    # via cryptography
+charset-normalizer==3.2.0
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   requests
-colorama==0.4.5
-    # via
-    #   -r requirements\docs.txt
-    #   -r requirements\test.txt
-    #   pytest
-    #   sphinx
-    #   sphinx-autobuild
-    #   tox
-commonmark==0.9.1
-    # via rich
-coverage[toml]==6.4.2
+colorama==0.4.6
+    # via sphinx-autobuild
+coverage[toml]==7.2.7
     # via
-    #   -r requirements\test.txt
+    #   -r requirements/test.txt
     #   pytest-cov
-distlib==0.3.5
+cryptography==41.0.2
+    # via secretstorage
+distlib==0.3.6
     # via virtualenv
 docutils==0.16
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   readme-renderer
     #   sphinx
     #   sphinx-panels
-filelock==3.7.1
+exceptiongroup==1.1.2
+    # via
+    #   -r requirements/test.txt
+    #   pytest
+filelock==3.12.2
     # via
     #   tox
     #   virtualenv
-flake8==4.0.1
-    # via -r requirements\dev.in
+flake8==6.0.0
+    # via -r requirements/dev.in
 furo==2021.4.11b34
-    # via -r requirements\docs.txt
-idna==3.3
+    # via -r requirements/docs.txt
+idna==3.4
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   requests
 imagesize==1.4.1
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   sphinx
-importlib-metadata==4.12.0
+importlib-metadata==6.8.0
     # via
     #   keyring
     #   twine
-iniconfig==1.1.1
+importlib-resources==6.0.0
+    # via keyring
+iniconfig==2.0.0
     # via
-    #   -r requirements\test.txt
+    #   -r requirements/test.txt
     #   pytest
+jaraco-classes==3.3.0
+    # via keyring
+jeepney==0.8.0
+    # via
+    #   keyring
+    #   secretstorage
 jinja2==3.0.3
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   sphinx
     #   sphinx-autoapi
-keyring==23.7.0
+keyring==24.2.0
     # via twine
-lazy-object-proxy==1.7.1
+lazy-object-proxy==1.9.0
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   astroid
 livereload==2.6.3
     # via sphinx-autobuild
-markupsafe==2.1.1
+markdown-it-py==3.0.0
+    # via rich
+markupsafe==2.1.3
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   jinja2
-mccabe==0.6.1
+mccabe==0.7.0
     # via flake8
-mypy==0.961
-    # via -r requirements\dev.in
-mypy-extensions==0.4.3
+mdurl==0.1.2
+    # via markdown-it-py
+more-itertools==9.1.0
+    # via jaraco-classes
+mypy==1.4.1
+    # via -r requirements/dev.in
+mypy-extensions==1.0.0
     # via mypy
-packaging==21.3
+packaging==23.1
     # via
-    #   -r requirements\docs.txt
-    #   -r requirements\test.txt
+    #   -r requirements/docs.txt
+    #   -r requirements/test.txt
     #   pytest
     #   sphinx
     #   tox
-pkginfo==1.8.3
+pkginfo==1.9.6
     # via twine
-platformdirs==2.5.2
+platformdirs==3.8.1
     # via virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via
-    #   -r requirements\test.txt
+    #   -r requirements/test.txt
     #   pytest
     #   tox
 py==1.11.0
-    # via
-    #   -r requirements\test.txt
-    #   pytest
-    #   tox
-pycodestyle==2.8.0
+    # via tox
+pycodestyle==2.10.0
     # via flake8
-pyflakes==2.4.0
+pycparser==2.21
+    # via cffi
+pyflakes==3.0.1
     # via flake8
-pygments==2.12.0
+pygments==2.15.1
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   readme-renderer
     #   rich
     #   sphinx
-pyparsing==3.0.9
+pytest==7.4.0
     # via
-    #   -r requirements\docs.txt
-    #   -r requirements\test.txt
-    #   packaging
-pytest==7.1.2
-    # via
-    #   -r requirements\test.txt
+    #   -r requirements/test.txt
     #   pytest-cov
-pytest-cov==3.0.0
-    # via -r requirements\test.txt
-pytz==2022.1
+pytest-cov==4.1.0
+    # via -r requirements/test.txt
+pytz==2023.3
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   babel
-pywin32-ctypes==0.2.0
-    # via keyring
 pyyaml==6.0
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   sphinx-autoapi
-readme-renderer==35.0
+readme-renderer==40.0
     # via twine
-requests==2.28.1
+requests==2.31.0
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   requests-toolbelt
     #   sphinx
     #   twine
-requests-toolbelt==0.9.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==12.5.1
+rich==13.4.2
     # via twine
+secretstorage==3.3.3
+    # via keyring
 six==1.16.0
     # via
     #   bleach
     #   livereload
     #   tox
-    #   virtualenv
 snowballstemmer==2.2.0
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   sphinx
-soupsieve==2.3.2.post1
+soupsieve==2.4.1
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   beautifulsoup4
 sphinx==3.5.4
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   furo
     #   sphinx-autoapi
     #   sphinx-autobuild
     #   sphinx-copybutton
     #   sphinx-issues
     #   sphinx-panels
     #   sphinx-version-warning
 sphinx-autoapi==1.8.4
-    # via -r requirements\docs.txt
+    # via -r requirements/docs.txt
 sphinx-autobuild==2021.3.14
-    # via -r requirements\dev.in
-sphinx-copybutton==0.5.0
-    # via -r requirements\docs.txt
+    # via -r requirements/dev.in
+sphinx-copybutton==0.5.2
+    # via -r requirements/docs.txt
 sphinx-issues==3.0.1
-    # via -r requirements\docs.txt
+    # via -r requirements/docs.txt
 sphinx-panels==0.6.0
-    # via -r requirements\docs.txt
+    # via -r requirements/docs.txt
 sphinx-version-warning==1.1.2
-    # via -r requirements\docs.txt
-sphinxcontrib-applehelp==1.0.2
+    # via -r requirements/docs.txt
+sphinxcontrib-applehelp==1.0.4
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   sphinx
 sphinxcontrib-devhelp==1.0.2
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   sphinx
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.1
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   sphinx
 sphinxcontrib-jsmath==1.0.1
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   sphinx
 sphinxcontrib-qthelp==1.0.3
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   sphinx
-toml==0.10.2
-    # via tox
 tomli==2.0.1
     # via
-    #   -r requirements\test.txt
+    #   -r requirements/test.txt
     #   coverage
     #   mypy
     #   pytest
-tornado==6.2
+    #   tox
+tornado==6.3.2
     # via livereload
-tox==3.25.1
-    # via -r requirements\dev.in
-twine==4.0.1
-    # via -r requirements\dev.in
-typing-extensions==4.3.0
+tox==3.28.0
+    # via -r requirements/dev.in
+twine==4.0.2
+    # via -r requirements/dev.in
+typing-extensions==4.7.1
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   astroid
     #   mypy
     #   rich
-unidecode==1.3.4
+unidecode==1.3.6
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   sphinx-autoapi
-urllib3==1.26.10
+urllib3==2.0.3
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   requests
     #   twine
-virtualenv==20.14.1
+virtualenv==20.23.1
     # via tox
 webencodings==0.5.1
     # via bleach
-wrapt==1.14.1
+wrapt==1.15.0
     # via
-    #   -r requirements\docs.txt
+    #   -r requirements/docs.txt
     #   astroid
-zipp==3.8.1
-    # via importlib-metadata
+zipp==3.16.1
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `cloup-2.1.1/requirements/docs.txt` & `cloup-2.1.2/requirements/docs.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,96 +1,93 @@
 #
-# This file is autogenerated by pip-compile
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
-#    pip-compile requirements/docs.in
+#    pip-compile --resolver=backtracking requirements/docs.in
 #
-alabaster==0.7.12
+alabaster==0.7.13
     # via sphinx
-astroid==2.12.2
+astroid==2.15.6
     # via sphinx-autoapi
-babel==2.10.3
+babel==2.12.1
     # via sphinx
-beautifulsoup4==4.11.1
+beautifulsoup4==4.12.2
     # via furo
-certifi==2022.6.15
+certifi==2023.5.7
     # via requests
-charset-normalizer==2.1.0
+charset-normalizer==3.2.0
     # via requests
-colorama==0.4.5
-    # via sphinx
 docutils==0.16
     # via
     #   sphinx
     #   sphinx-panels
 furo==2021.4.11b34
     # via -r requirements/docs.in
-idna==3.3
+idna==3.4
     # via requests
 imagesize==1.4.1
     # via sphinx
 jinja2==3.0.3
     # via
+    #   -r requirements/docs.in
     #   sphinx
     #   sphinx-autoapi
-lazy-object-proxy==1.7.1
+lazy-object-proxy==1.9.0
     # via astroid
-markupsafe==2.1.1
+markupsafe==2.1.3
     # via jinja2
-packaging==21.3
+packaging==23.1
     # via sphinx
-pygments==2.12.0
+pygments==2.15.1
     # via sphinx
-pyparsing==3.0.9
-    # via packaging
-pytz==2022.1
+pytz==2023.3
     # via babel
 pyyaml==6.0
     # via sphinx-autoapi
-requests==2.28.1
+requests==2.31.0
     # via sphinx
 snowballstemmer==2.2.0
     # via sphinx
-soupsieve==2.3.2.post1
+soupsieve==2.4.1
     # via beautifulsoup4
-sphinx-autoapi==1.8.4
-    # via -r requirements/docs.in
-sphinx-copybutton==0.5.0
-    # via -r requirements/docs.in
-sphinx-issues==3.0.1
-    # via -r requirements/docs.in
-sphinx-panels==0.6.0
-    # via -r requirements/docs.in
-sphinx-version-warning==1.1.2
-    # via -r requirements/docs.in
 sphinx==3.5.4
     # via
     #   -r requirements/docs.in
     #   furo
     #   sphinx-autoapi
     #   sphinx-copybutton
     #   sphinx-issues
     #   sphinx-panels
     #   sphinx-version-warning
-sphinxcontrib-applehelp==1.0.2
+sphinx-autoapi==1.8.4
+    # via -r requirements/docs.in
+sphinx-copybutton==0.5.2
+    # via -r requirements/docs.in
+sphinx-issues==3.0.1
+    # via -r requirements/docs.in
+sphinx-panels==0.6.0
+    # via -r requirements/docs.in
+sphinx-version-warning==1.1.2
+    # via -r requirements/docs.in
+sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-typing-extensions==4.3.0
+typing-extensions==4.7.1
     # via astroid
-unidecode==1.3.4
+unidecode==1.3.6
     # via sphinx-autoapi
-urllib3==1.26.10
+urllib3==2.0.3
     # via requests
-wrapt==1.14.1
+wrapt==1.15.0
     # via astroid
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `cloup-2.1.1/scripts/generate_git_example.py` & `cloup-2.1.2/scripts/generate_git_example.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/scripts/remove.py` & `cloup-2.1.2/scripts/remove.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/setup.py` & `cloup-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/tests/conftest.py` & `cloup-2.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/tests/constraints/conftest.py` & `cloup-2.1.2/tests/constraints/conftest.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/tests/constraints/test_common.py` & `cloup-2.1.2/tests/constraints/test_common.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/tests/constraints/test_conditional_constraints.py` & `cloup-2.1.2/tests/constraints/test_conditional_constraints.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/tests/constraints/test_constraints.py` & `cloup-2.1.2/tests/constraints/test_constraints.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/tests/constraints/test_support.py` & `cloup-2.1.2/tests/constraints/test_support.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/tests/example_command.py` & `cloup-2.1.2/tests/example_command.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/tests/example_group.py` & `cloup-2.1.2/tests/example_group.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/tests/test_aliases.py` & `cloup-2.1.2/tests/test_aliases.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/tests/test_commands.py` & `cloup-2.1.2/tests/test_commands.py`

 * *Files 22% similar despite different names*

```diff
@@ -116,7 +116,64 @@
         def subgroup():
             pass
 
     with pytest.raises(Exception, match="parenthesis"):
         @root.command
         def subcommand():
             pass
+
+
+def test_group_command_class_is_used_to_create_subcommands(runner):
+    class CustomCommand(cloup.Command):
+
+        def __init__(self, *args, **kwargs):
+            kwargs.setdefault("context_settings", {"help_option_names": ("--help", "-h")})
+            super().__init__(*args, **kwargs)
+
+    class CustomGroup(cloup.Group):
+        command_class = CustomCommand
+
+    @cloup.group("cli", cls=CustomGroup)
+    def my_cli():
+        pass
+
+    @my_cli.command()
+    def subcommand():
+        pass
+
+    assert isinstance(subcommand, CustomCommand)
+
+    res = runner.invoke(my_cli, ["subcommand", "--help"])
+    assert res.output == reindent("""
+        Usage: cli subcommand [OPTIONS]
+
+        Options:
+          -h, --help  Show this message and exit.
+    """)
+
+
+def test_group_class_is_used_to_create_subgroups(runner):
+    class CustomGroup(cloup.Group):
+        group_class = type
+
+    class OtherCustomGroup(cloup.Group):
+        group_class = cloup.Group
+
+    @cloup.group("cli", cls=CustomGroup)
+    def my_cli():
+        pass
+
+    @my_cli.group()
+    def sub_group():
+        pass
+
+    @my_cli.group(cls=OtherCustomGroup)
+    def other_group():
+        pass
+
+    @other_group.group()
+    def other_sub_group():
+        pass
+
+    assert isinstance(sub_group, CustomGroup)
+    assert isinstance(other_group, OtherCustomGroup)
+    assert isinstance(other_sub_group, cloup.Group)
```

### Comparing `cloup-2.1.1/tests/test_context.py` & `cloup-2.1.2/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/tests/test_formatting.py` & `cloup-2.1.2/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/tests/test_option_groups.py` & `cloup-2.1.2/tests/test_option_groups.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/tests/test_sections.py` & `cloup-2.1.2/tests/test_sections.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/tests/test_sep.py` & `cloup-2.1.2/tests/test_sep.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/tests/test_styling.py` & `cloup-2.1.2/tests/test_styling.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/tests/test_util.py` & `cloup-2.1.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/tests/util.py` & `cloup-2.1.2/tests/util.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.1/tox.ini` & `cloup-2.1.2/tox.ini`

 * *Files identical despite different names*

