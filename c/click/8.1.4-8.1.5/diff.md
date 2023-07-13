# Comparing `tmp/click-8.1.4.tar.gz` & `tmp/click-8.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click-8.1.4.tar", last modified: Thu Jul  6 18:22:39 2023, max compression
+gzip compressed data, was "click-8.1.5.tar", last modified: Thu Jul 13 15:02:51 2023, max compression
```

## Comparing `click-8.1.4.tar` & `click-8.1.5.tar`

### file list

```diff
@@ -1,147 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.659953 click-8.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    46244 2023-07-06 18:22:30.000000 click-8.1.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-06 18:22:30.000000 click-8.1.4/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-06 18:22:30.000000 click-8.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-06 18:22:39.659953 click-8.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-06 18:22:30.000000 click-8.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.643953 click-8.1.4/artwork/
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-07-06 18:22:30.000000 click-8.1.4/artwork/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.647953 click-8.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-06 18:22:30.000000 click-8.1.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.647953 click-8.1.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-06 18:22:30.000000 click-8.1.4/docs/_static/click-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-07-06 18:22:30.000000 click-8.1.4/docs/_static/click-logo-sidebar.png
--rw-r--r--   0 runner    (1001) docker     (123)    26081 2023-07-06 18:22:30.000000 click-8.1.4/docs/_static/click-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    17515 2023-07-06 18:22:30.000000 click-8.1.4/docs/advanced.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-06 18:22:30.000000 click-8.1.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-07-06 18:22:30.000000 click-8.1.4/docs/arguments.rst
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-06 18:22:30.000000 click-8.1.4/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18928 2023-07-06 18:22:30.000000 click-8.1.4/docs/commands.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-07-06 18:22:30.000000 click-8.1.4/docs/complex.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-06 18:22:30.000000 click-8.1.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-06 18:22:30.000000 click-8.1.4/docs/contrib.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-07-06 18:22:30.000000 click-8.1.4/docs/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-06 18:22:30.000000 click-8.1.4/docs/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-06 18:22:30.000000 click-8.1.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-06 18:22:30.000000 click-8.1.4/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-06 18:22:30.000000 click-8.1.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    26719 2023-07-06 18:22:30.000000 click-8.1.4/docs/options.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-06 18:22:30.000000 click-8.1.4/docs/parameters.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-06 18:22:30.000000 click-8.1.4/docs/prompts.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-06 18:22:30.000000 click-8.1.4/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-07-06 18:22:30.000000 click-8.1.4/docs/setuptools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-07-06 18:22:30.000000 click-8.1.4/docs/shell-completion.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-06 18:22:30.000000 click-8.1.4/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-06 18:22:30.000000 click-8.1.4/docs/unicode-support.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-06 18:22:30.000000 click-8.1.4/docs/upgrading.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12792 2023-07-06 18:22:30.000000 click-8.1.4/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-07-06 18:22:30.000000 click-8.1.4/docs/why.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-06 18:22:30.000000 click-8.1.4/docs/wincmd.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.647953 click-8.1.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-06 18:22:30.000000 click-8.1.4/examples/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.647953 click-8.1.4/examples/aliases/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-06 18:22:30.000000 click-8.1.4/examples/aliases/README
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 18:22:30.000000 click-8.1.4/examples/aliases/aliases.ini
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-06 18:22:30.000000 click-8.1.4/examples/aliases/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-06 18:22:30.000000 click-8.1.4/examples/aliases/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.647953 click-8.1.4/examples/colors/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-06 18:22:30.000000 click-8.1.4/examples/colors/README
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-06 18:22:30.000000 click-8.1.4/examples/colors/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-06 18:22:30.000000 click-8.1.4/examples/colors/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.647953 click-8.1.4/examples/completion/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-06 18:22:30.000000 click-8.1.4/examples/completion/README
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-06 18:22:30.000000 click-8.1.4/examples/completion/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-06 18:22:30.000000 click-8.1.4/examples/completion/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.647953 click-8.1.4/examples/complex/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-06 18:22:30.000000 click-8.1.4/examples/complex/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.647953 click-8.1.4/examples/complex/complex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:30.000000 click-8.1.4/examples/complex/complex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-06 18:22:30.000000 click-8.1.4/examples/complex/complex/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.651953 click-8.1.4/examples/complex/complex/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:30.000000 click-8.1.4/examples/complex/complex/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-06 18:22:30.000000 click-8.1.4/examples/complex/complex/commands/cmd_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-06 18:22:30.000000 click-8.1.4/examples/complex/complex/commands/cmd_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-06 18:22:30.000000 click-8.1.4/examples/complex/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.651953 click-8.1.4/examples/imagepipe/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 18:22:30.000000 click-8.1.4/examples/imagepipe/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-06 18:22:30.000000 click-8.1.4/examples/imagepipe/README
--rw-r--r--   0 runner    (1001) docker     (123)    51677 2023-07-06 18:22:30.000000 click-8.1.4/examples/imagepipe/example01.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    39106 2023-07-06 18:22:30.000000 click-8.1.4/examples/imagepipe/example02.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-07-06 18:22:30.000000 click-8.1.4/examples/imagepipe/imagepipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-06 18:22:30.000000 click-8.1.4/examples/imagepipe/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.651953 click-8.1.4/examples/inout/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-06 18:22:30.000000 click-8.1.4/examples/inout/README
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-06 18:22:30.000000 click-8.1.4/examples/inout/inout.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-06 18:22:30.000000 click-8.1.4/examples/inout/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.651953 click-8.1.4/examples/naval/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-06 18:22:30.000000 click-8.1.4/examples/naval/README
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-06 18:22:30.000000 click-8.1.4/examples/naval/naval.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-06 18:22:30.000000 click-8.1.4/examples/naval/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.651953 click-8.1.4/examples/repo/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-06 18:22:30.000000 click-8.1.4/examples/repo/README
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-06 18:22:30.000000 click-8.1.4/examples/repo/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-06 18:22:30.000000 click-8.1.4/examples/repo/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.651953 click-8.1.4/examples/termui/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-06 18:22:30.000000 click-8.1.4/examples/termui/README
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-06 18:22:30.000000 click-8.1.4/examples/termui/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-06 18:22:30.000000 click-8.1.4/examples/termui/termui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.651953 click-8.1.4/examples/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-06 18:22:30.000000 click-8.1.4/examples/validation/README
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-06 18:22:30.000000 click-8.1.4/examples/validation/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-06 18:22:30.000000 click-8.1.4/examples/validation/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.651953 click-8.1.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-06 18:22:30.000000 click-8.1.4/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-06 18:22:30.000000 click-8.1.4/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-06 18:22:30.000000 click-8.1.4/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-06 18:22:30.000000 click-8.1.4/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-06 18:22:30.000000 click-8.1.4/requirements/typing.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-06 18:22:39.659953 click-8.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-06 18:22:30.000000 click-8.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.643953 click-8.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.655953 click-8.1.4/src/click/
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-06 18:22:30.000000 click-8.1.4/src/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-07-06 18:22:30.000000 click-8.1.4/src/click/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    24069 2023-07-06 18:22:30.000000 click-8.1.4/src/click/_termui_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-06 18:22:30.000000 click-8.1.4/src/click/_textwrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-07-06 18:22:30.000000 click-8.1.4/src/click/_winconsole.py
--rw-r--r--   0 runner    (1001) docker     (123)   114086 2023-07-06 18:22:30.000000 click-8.1.4/src/click/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    19485 2023-07-06 18:22:30.000000 click-8.1.4/src/click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-07-06 18:22:30.000000 click-8.1.4/src/click/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-07-06 18:22:30.000000 click-8.1.4/src/click/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-06 18:22:30.000000 click-8.1.4/src/click/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    19067 2023-07-06 18:22:30.000000 click-8.1.4/src/click/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:30.000000 click-8.1.4/src/click/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18396 2023-07-06 18:22:30.000000 click-8.1.4/src/click/shell_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)    28324 2023-07-06 18:22:30.000000 click-8.1.4/src/click/termui.py
--rw-r--r--   0 runner    (1001) docker     (123)    16084 2023-07-06 18:22:30.000000 click-8.1.4/src/click/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    36391 2023-07-06 18:22:30.000000 click-8.1.4/src/click/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    20298 2023-07-06 18:22:30.000000 click-8.1.4/src/click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.655953 click-8.1.4/src/click.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-06 18:22:39.000000 click-8.1.4/src/click.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-06 18:22:39.000000 click-8.1.4/src/click.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:22:39.000000 click-8.1.4/src/click.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-06 18:22:39.000000 click-8.1.4/src/click.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 18:22:39.000000 click-8.1.4/src/click.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:22:39.659953 click-8.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-06 18:22:30.000000 click-8.1.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_command_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_custom_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_info_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    28531 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    14101 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_shell_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_termui.py
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    16173 2023-07-06 18:22:30.000000 click-8.1.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-06 18:22:30.000000 click-8.1.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.483176 click-8.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    46440 2023-07-13 15:02:39.000000 click-8.1.5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-13 15:02:39.000000 click-8.1.5/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-13 15:02:39.000000 click-8.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-13 15:02:51.483176 click-8.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-13 15:02:39.000000 click-8.1.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.463170 click-8.1.5/artwork/
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-07-13 15:02:39.000000 click-8.1.5/artwork/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.467171 click-8.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-13 15:02:39.000000 click-8.1.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.467171 click-8.1.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-13 15:02:39.000000 click-8.1.5/docs/_static/click-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-07-13 15:02:39.000000 click-8.1.5/docs/_static/click-logo-sidebar.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26081 2023-07-13 15:02:39.000000 click-8.1.5/docs/_static/click-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17515 2023-07-13 15:02:39.000000 click-8.1.5/docs/advanced.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-13 15:02:39.000000 click-8.1.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-07-13 15:02:39.000000 click-8.1.5/docs/arguments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 15:02:39.000000 click-8.1.5/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18928 2023-07-13 15:02:39.000000 click-8.1.5/docs/commands.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-07-13 15:02:39.000000 click-8.1.5/docs/complex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-13 15:02:39.000000 click-8.1.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-13 15:02:39.000000 click-8.1.5/docs/contrib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-07-13 15:02:39.000000 click-8.1.5/docs/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-13 15:02:39.000000 click-8.1.5/docs/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-13 15:02:39.000000 click-8.1.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-13 15:02:39.000000 click-8.1.5/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-13 15:02:39.000000 click-8.1.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    26719 2023-07-13 15:02:39.000000 click-8.1.5/docs/options.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-13 15:02:39.000000 click-8.1.5/docs/parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-13 15:02:39.000000 click-8.1.5/docs/prompts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-13 15:02:39.000000 click-8.1.5/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-07-13 15:02:39.000000 click-8.1.5/docs/setuptools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-07-13 15:02:39.000000 click-8.1.5/docs/shell-completion.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-13 15:02:39.000000 click-8.1.5/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-13 15:02:39.000000 click-8.1.5/docs/unicode-support.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-13 15:02:39.000000 click-8.1.5/docs/upgrading.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12792 2023-07-13 15:02:39.000000 click-8.1.5/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-07-13 15:02:39.000000 click-8.1.5/docs/why.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-13 15:02:39.000000 click-8.1.5/docs/wincmd.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.467171 click-8.1.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-13 15:02:39.000000 click-8.1.5/examples/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.467171 click-8.1.5/examples/aliases/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-13 15:02:39.000000 click-8.1.5/examples/aliases/README
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 15:02:39.000000 click-8.1.5/examples/aliases/aliases.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-13 15:02:39.000000 click-8.1.5/examples/aliases/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-13 15:02:39.000000 click-8.1.5/examples/aliases/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.467171 click-8.1.5/examples/colors/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-13 15:02:39.000000 click-8.1.5/examples/colors/README
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-13 15:02:39.000000 click-8.1.5/examples/colors/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-13 15:02:39.000000 click-8.1.5/examples/colors/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.471172 click-8.1.5/examples/completion/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-13 15:02:39.000000 click-8.1.5/examples/completion/README
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-13 15:02:39.000000 click-8.1.5/examples/completion/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-13 15:02:39.000000 click-8.1.5/examples/completion/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.471172 click-8.1.5/examples/complex/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-13 15:02:39.000000 click-8.1.5/examples/complex/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.471172 click-8.1.5/examples/complex/complex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:39.000000 click-8.1.5/examples/complex/complex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-13 15:02:39.000000 click-8.1.5/examples/complex/complex/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.471172 click-8.1.5/examples/complex/complex/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:39.000000 click-8.1.5/examples/complex/complex/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-13 15:02:39.000000 click-8.1.5/examples/complex/complex/commands/cmd_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-13 15:02:39.000000 click-8.1.5/examples/complex/complex/commands/cmd_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-13 15:02:39.000000 click-8.1.5/examples/complex/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.471172 click-8.1.5/examples/imagepipe/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 15:02:39.000000 click-8.1.5/examples/imagepipe/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-13 15:02:39.000000 click-8.1.5/examples/imagepipe/README
+-rw-r--r--   0 runner    (1001) docker     (123)    51677 2023-07-13 15:02:39.000000 click-8.1.5/examples/imagepipe/example01.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    39106 2023-07-13 15:02:39.000000 click-8.1.5/examples/imagepipe/example02.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-07-13 15:02:39.000000 click-8.1.5/examples/imagepipe/imagepipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-13 15:02:39.000000 click-8.1.5/examples/imagepipe/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.471172 click-8.1.5/examples/inout/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-13 15:02:39.000000 click-8.1.5/examples/inout/README
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-13 15:02:39.000000 click-8.1.5/examples/inout/inout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-13 15:02:39.000000 click-8.1.5/examples/inout/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.475174 click-8.1.5/examples/naval/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-13 15:02:39.000000 click-8.1.5/examples/naval/README
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-13 15:02:39.000000 click-8.1.5/examples/naval/naval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-13 15:02:39.000000 click-8.1.5/examples/naval/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.475174 click-8.1.5/examples/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-13 15:02:39.000000 click-8.1.5/examples/repo/README
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-13 15:02:39.000000 click-8.1.5/examples/repo/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-13 15:02:39.000000 click-8.1.5/examples/repo/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.475174 click-8.1.5/examples/termui/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-13 15:02:39.000000 click-8.1.5/examples/termui/README
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-13 15:02:39.000000 click-8.1.5/examples/termui/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-13 15:02:39.000000 click-8.1.5/examples/termui/termui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.475174 click-8.1.5/examples/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-13 15:02:39.000000 click-8.1.5/examples/validation/README
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-13 15:02:39.000000 click-8.1.5/examples/validation/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-13 15:02:39.000000 click-8.1.5/examples/validation/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.475174 click-8.1.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 15:02:39.000000 click-8.1.5/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-13 15:02:39.000000 click-8.1.5/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-13 15:02:39.000000 click-8.1.5/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-13 15:02:39.000000 click-8.1.5/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-13 15:02:39.000000 click-8.1.5/requirements/typing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-13 15:02:51.483176 click-8.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-13 15:02:39.000000 click-8.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.463170 click-8.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.479175 click-8.1.5/src/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-13 15:02:39.000000 click-8.1.5/src/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-07-13 15:02:39.000000 click-8.1.5/src/click/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24069 2023-07-13 15:02:39.000000 click-8.1.5/src/click/_termui_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-13 15:02:39.000000 click-8.1.5/src/click/_textwrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-07-13 15:02:39.000000 click-8.1.5/src/click/_winconsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114086 2023-07-13 15:02:39.000000 click-8.1.5/src/click/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19096 2023-07-13 15:02:39.000000 click-8.1.5/src/click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-07-13 15:02:39.000000 click-8.1.5/src/click/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-07-13 15:02:39.000000 click-8.1.5/src/click/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-13 15:02:39.000000 click-8.1.5/src/click/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19067 2023-07-13 15:02:39.000000 click-8.1.5/src/click/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:39.000000 click-8.1.5/src/click/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18396 2023-07-13 15:02:39.000000 click-8.1.5/src/click/shell_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28324 2023-07-13 15:02:39.000000 click-8.1.5/src/click/termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16084 2023-07-13 15:02:39.000000 click-8.1.5/src/click/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36391 2023-07-13 15:02:39.000000 click-8.1.5/src/click/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20298 2023-07-13 15:02:39.000000 click-8.1.5/src/click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.479175 click-8.1.5/src/click.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-13 15:02:51.000000 click-8.1.5/src/click.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-13 15:02:51.000000 click-8.1.5/src/click.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:02:51.000000 click-8.1.5/src/click.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-13 15:02:51.000000 click-8.1.5/src/click.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 15:02:51.000000 click-8.1.5/src/click.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.483176 click-8.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-13 15:02:39.000000 click-8.1.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-07-13 15:02:39.000000 click-8.1.5/tests/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-07-13 15:02:39.000000 click-8.1.5/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-13 15:02:39.000000 click-8.1.5/tests/test_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-13 15:02:39.000000 click-8.1.5/tests/test_command_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-07-13 15:02:39.000000 click-8.1.5/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-13 15:02:39.000000 click-8.1.5/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-07-13 15:02:39.000000 click-8.1.5/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-13 15:02:39.000000 click-8.1.5/tests/test_custom_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-13 15:02:39.000000 click-8.1.5/tests/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-07-13 15:02:39.000000 click-8.1.5/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-13 15:02:39.000000 click-8.1.5/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-07-13 15:02:39.000000 click-8.1.5/tests/test_info_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-13 15:02:39.000000 click-8.1.5/tests/test_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28531 2023-07-13 15:02:39.000000 click-8.1.5/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-13 15:02:39.000000 click-8.1.5/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14101 2023-07-13 15:02:39.000000 click-8.1.5/tests/test_shell_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-07-13 15:02:39.000000 click-8.1.5/tests/test_termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-07-13 15:02:39.000000 click-8.1.5/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-07-13 15:02:39.000000 click-8.1.5/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16173 2023-07-13 15:02:39.000000 click-8.1.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:02:51.483176 click-8.1.5/tests/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-13 15:02:39.000000 click-8.1.5/tests/typing/typing_aliased_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-13 15:02:39.000000 click-8.1.5/tests/typing/typing_confirmation_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-13 15:02:39.000000 click-8.1.5/tests/typing/typing_help_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-13 15:02:39.000000 click-8.1.5/tests/typing/typing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-13 15:02:39.000000 click-8.1.5/tests/typing/typing_password_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-13 15:02:39.000000 click-8.1.5/tests/typing/typing_simple_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-13 15:02:39.000000 click-8.1.5/tests/typing/typing_version_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-13 15:02:39.000000 click-8.1.5/tox.ini
```

### Comparing `click-8.1.4/CHANGES.rst` & `click-8.1.5/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 .. currentmodule:: click
 
+Version 8.1.5
+-------------
+
+Released 2023-07-13
+
+-   Fix an issue with type hints for ``@click.command()``, ``@click.option()``, and
+    other decorators. Introduce typing tests. :issue:`2558`
+
+
 Version 8.1.4
 -------------
 
 Released 2023-07-06
 
 -   Replace all ``typing.Dict`` occurrences to ``typing.MutableMapping`` for
     parameter hints. :issue:`2255`
```

### Comparing `click-8.1.4/LICENSE.rst` & `click-8.1.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/PKG-INFO` & `click-8.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click
-Version: 8.1.4
+Version: 8.1.5
 Summary: Composable command line interface toolkit
 Home-page: https://palletsprojects.com/p/click/
 Maintainer: Pallets
 Maintainer-email: contact@palletsprojects.com
 License: BSD-3-Clause
 Project-URL: Donate, https://palletsprojects.com/donate
 Project-URL: Documentation, https://click.palletsprojects.com/
```

### Comparing `click-8.1.4/README.rst` & `click-8.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/artwork/logo.svg` & `click-8.1.5/artwork/logo.svg`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/Makefile` & `click-8.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/_static/click-icon.png` & `click-8.1.5/docs/_static/click-icon.png`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/_static/click-logo-sidebar.png` & `click-8.1.5/docs/_static/click-logo-sidebar.png`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/_static/click-logo.png` & `click-8.1.5/docs/_static/click-logo.png`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/advanced.rst` & `click-8.1.5/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/api.rst` & `click-8.1.5/docs/api.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/arguments.rst` & `click-8.1.5/docs/arguments.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/commands.rst` & `click-8.1.5/docs/commands.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/complex.rst` & `click-8.1.5/docs/complex.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/conf.py` & `click-8.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/contrib.rst` & `click-8.1.5/docs/contrib.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/documentation.rst` & `click-8.1.5/docs/documentation.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/exceptions.rst` & `click-8.1.5/docs/exceptions.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/index.rst` & `click-8.1.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/make.bat` & `click-8.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/options.rst` & `click-8.1.5/docs/options.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/parameters.rst` & `click-8.1.5/docs/parameters.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/prompts.rst` & `click-8.1.5/docs/prompts.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/quickstart.rst` & `click-8.1.5/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/setuptools.rst` & `click-8.1.5/docs/setuptools.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/shell-completion.rst` & `click-8.1.5/docs/shell-completion.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/testing.rst` & `click-8.1.5/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/unicode-support.rst` & `click-8.1.5/docs/unicode-support.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/upgrading.rst` & `click-8.1.5/docs/upgrading.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/utils.rst` & `click-8.1.5/docs/utils.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/why.rst` & `click-8.1.5/docs/why.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/docs/wincmd.rst` & `click-8.1.5/docs/wincmd.rst`

 * *Files identical despite different names*

### Comparing `click-8.1.4/examples/aliases/aliases.py` & `click-8.1.5/examples/aliases/aliases.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/examples/colors/colors.py` & `click-8.1.5/examples/colors/colors.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/examples/completion/completion.py` & `click-8.1.5/examples/completion/completion.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/examples/complex/complex/cli.py` & `click-8.1.5/examples/complex/complex/cli.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/examples/imagepipe/example01.jpg` & `click-8.1.5/examples/imagepipe/example01.jpg`

 * *Files identical despite different names*

### Comparing `click-8.1.4/examples/imagepipe/example02.jpg` & `click-8.1.5/examples/imagepipe/example02.jpg`

 * *Files identical despite different names*

### Comparing `click-8.1.4/examples/imagepipe/imagepipe.py` & `click-8.1.5/examples/imagepipe/imagepipe.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/examples/inout/inout.py` & `click-8.1.5/examples/inout/inout.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/examples/naval/naval.py` & `click-8.1.5/examples/naval/naval.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/examples/repo/repo.py` & `click-8.1.5/examples/repo/repo.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/examples/termui/termui.py` & `click-8.1.5/examples/termui/termui.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/examples/validation/validation.py` & `click-8.1.5/examples/validation/validation.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/requirements/dev.txt` & `click-8.1.5/requirements/dev.txt`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,14 @@
     # via virtualenv
 filelock==3.12.2
     # via
     #   tox
     #   virtualenv
 identify==2.5.24
     # via pre-commit
-nodeenv==1.8.0
-    # via pre-commit
 pip-compile-multi==2.6.3
     # via -r requirements/dev.in
 pip-tools==6.13.0
     # via pip-compile-multi
 platformdirs==3.8.0
     # via
     #   tox
```

### Comparing `click-8.1.4/requirements/docs.txt` & `click-8.1.5/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `click-8.1.4/setup.cfg` & `click-8.1.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 	B028
 	B907
 max-line-length = 80
 per-file-ignores = 
 	src/click/__init__.py: F401
 
 [mypy]
-files = src/click
+files = src/click, tests/typing
 python_version = 3.7
 show_error_codes = True
 disallow_subclassing_any = True
 disallow_untyped_calls = True
 disallow_untyped_defs = True
 disallow_incomplete_defs = True
 disallow_any_generics = True
```

### Comparing `click-8.1.4/src/click/__init__.py` & `click-8.1.5/src/click/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,8 +66,8 @@
 from .utils import echo as echo
 from .utils import format_filename as format_filename
 from .utils import get_app_dir as get_app_dir
 from .utils import get_binary_stream as get_binary_stream
 from .utils import get_text_stream as get_text_stream
 from .utils import open_file as open_file
 
-__version__ = "8.1.4"
+__version__ = "8.1.5"
```

### Comparing `click-8.1.4/src/click/_compat.py` & `click-8.1.5/src/click/_compat.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/src/click/_termui_impl.py` & `click-8.1.5/src/click/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/src/click/_textwrap.py` & `click-8.1.5/src/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/src/click/_winconsole.py` & `click-8.1.5/src/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/src/click/core.py` & `click-8.1.5/src/click/core.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/src/click/decorators.py` & `click-8.1.5/src/click/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     import typing_extensions as te
 
     P = te.ParamSpec("P")
 
 R = t.TypeVar("R")
 T = t.TypeVar("T")
 _AnyCallable = t.Callable[..., t.Any]
-_Decorator: "te.TypeAlias" = t.Callable[[T], T]
 FC = t.TypeVar("FC", bound=t.Union[_AnyCallable, Command])
 
 
 def pass_context(f: "t.Callable[te.Concatenate[Context, P], R]") -> "t.Callable[P, R]":
     """Marks a callback as wanting to receive the current context
     object as first argument.
     """
@@ -146,24 +145,20 @@
     name: t.Optional[str],
     cls: t.Type[CmdType],
     **attrs: t.Any,
 ) -> t.Callable[[_AnyCallable], CmdType]:
     ...
 
 
-# variant: name omitted, cls _must_ be a keyword argument, @command(cmd=CommandCls, ...)
-# The correct way to spell this overload is to use keyword-only argument syntax:
-# def command(*, cls: t.Type[CmdType], **attrs: t.Any) -> ...
-# However, mypy thinks this doesn't fit the overloaded function. Pyright does
-# accept that spelling, and the following work-around makes pyright issue a
-# warning that CmdType could be left unsolved, but mypy sees it as fine. *shrug*
+# variant: name omitted, cls _must_ be a keyword argument, @command(cls=CommandCls, ...)
 @t.overload
 def command(
     name: None = None,
-    cls: t.Type[CmdType] = ...,
+    *,
+    cls: t.Type[CmdType],
     **attrs: t.Any,
 ) -> t.Callable[[_AnyCallable], CmdType]:
     ...
 
 
 # variant: with optional string name, no cls argument provided.
 @t.overload
@@ -327,15 +322,15 @@
             f.__click_params__ = []  # type: ignore
 
         f.__click_params__.append(param)  # type: ignore
 
 
 def argument(
     *param_decls: str, cls: t.Optional[t.Type[Argument]] = None, **attrs: t.Any
-) -> _Decorator[FC]:
+) -> t.Callable[[FC], FC]:
     """Attaches an argument to the command.  All positional arguments are
     passed as parameter declarations to :class:`Argument`; all keyword
     arguments are forwarded unchanged (except ``cls``).
     This is equivalent to creating an :class:`Argument` instance manually
     and attaching it to the :attr:`Command.params` list.
 
     For the default argument class, refer to :class:`Argument` and
@@ -355,15 +350,15 @@
         return f
 
     return decorator
 
 
 def option(
     *param_decls: str, cls: t.Optional[t.Type[Option]] = None, **attrs: t.Any
-) -> _Decorator[FC]:
+) -> t.Callable[[FC], FC]:
     """Attaches an option to the command.  All positional arguments are
     passed as parameter declarations to :class:`Option`; all keyword
     arguments are forwarded unchanged (except ``cls``).
     This is equivalent to creating an :class:`Option` instance manually
     and attaching it to the :attr:`Command.params` list.
 
     For the default option class, refer to :class:`Option` and
@@ -381,15 +376,15 @@
     def decorator(f: FC) -> FC:
         _param_memo(f, cls(param_decls, **attrs))
         return f
 
     return decorator
 
 
-def confirmation_option(*param_decls: str, **kwargs: t.Any) -> _Decorator[FC]:
+def confirmation_option(*param_decls: str, **kwargs: t.Any) -> t.Callable[[FC], FC]:
     """Add a ``--yes`` option which shows a prompt before continuing if
     not passed. If the prompt is declined, the program will exit.
 
     :param param_decls: One or more option names. Defaults to the single
         value ``"--yes"``.
     :param kwargs: Extra arguments are passed to :func:`option`.
     """
@@ -405,15 +400,15 @@
     kwargs.setdefault("callback", callback)
     kwargs.setdefault("expose_value", False)
     kwargs.setdefault("prompt", "Do you want to continue?")
     kwargs.setdefault("help", "Confirm the action without prompting.")
     return option(*param_decls, **kwargs)
 
 
-def password_option(*param_decls: str, **kwargs: t.Any) -> _Decorator[FC]:
+def password_option(*param_decls: str, **kwargs: t.Any) -> t.Callable[[FC], FC]:
     """Add a ``--password`` option which prompts for a password, hiding
     input and asking to enter the value again for confirmation.
 
     :param param_decls: One or more option names. Defaults to the single
         value ``"--password"``.
     :param kwargs: Extra arguments are passed to :func:`option`.
     """
@@ -429,15 +424,15 @@
 def version_option(
     version: t.Optional[str] = None,
     *param_decls: str,
     package_name: t.Optional[str] = None,
     prog_name: t.Optional[str] = None,
     message: t.Optional[str] = None,
     **kwargs: t.Any,
-) -> _Decorator[FC]:
+) -> t.Callable[[FC], FC]:
     """Add a ``--version`` option which immediately prints the version
     number and exits the program.
 
     If ``version`` is not provided, Click will try to detect it using
     :func:`importlib.metadata.version` to get the version for the
     ``package_name``. On Python < 3.8, the ``importlib_metadata``
     backport must be installed.
@@ -535,15 +530,15 @@
     kwargs.setdefault("expose_value", False)
     kwargs.setdefault("is_eager", True)
     kwargs.setdefault("help", _("Show the version and exit."))
     kwargs["callback"] = callback
     return option(*param_decls, **kwargs)
 
 
-def help_option(*param_decls: str, **kwargs: t.Any) -> _Decorator[FC]:
+def help_option(*param_decls: str, **kwargs: t.Any) -> t.Callable[[FC], FC]:
     """Add a ``--help`` option which immediately prints the help page
     and exits the program.
 
     This is usually unnecessary, as the ``--help`` option is added to
     each command automatically unless ``add_help_option=False`` is
     passed.
```

### Comparing `click-8.1.4/src/click/exceptions.py` & `click-8.1.5/src/click/exceptions.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/src/click/formatting.py` & `click-8.1.5/src/click/formatting.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/src/click/globals.py` & `click-8.1.5/src/click/globals.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/src/click/parser.py` & `click-8.1.5/src/click/parser.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/src/click/shell_completion.py` & `click-8.1.5/src/click/shell_completion.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/src/click/termui.py` & `click-8.1.5/src/click/termui.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/src/click/testing.py` & `click-8.1.5/src/click/testing.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/src/click/types.py` & `click-8.1.5/src/click/types.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/src/click/utils.py` & `click-8.1.5/src/click/utils.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/src/click.egg-info/PKG-INFO` & `click-8.1.5/src/click.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click
-Version: 8.1.4
+Version: 8.1.5
 Summary: Composable command line interface toolkit
 Home-page: https://palletsprojects.com/p/click/
 Maintainer: Pallets
 Maintainer-email: contact@palletsprojects.com
 License: BSD-3-Clause
 Project-URL: Donate, https://palletsprojects.com/donate
 Project-URL: Documentation, https://click.palletsprojects.com/
```

### Comparing `click-8.1.4/src/click.egg-info/SOURCES.txt` & `click-8.1.5/src/click.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -117,8 +117,15 @@
 tests/test_normalization.py
 tests/test_options.py
 tests/test_parser.py
 tests/test_shell_completion.py
 tests/test_termui.py
 tests/test_testing.py
 tests/test_types.py
-tests/test_utils.py
+tests/test_utils.py
+tests/typing/typing_aliased_group.py
+tests/typing/typing_confirmation_option.py
+tests/typing/typing_help_option.py
+tests/typing/typing_options.py
+tests/typing/typing_password_option.py
+tests/typing/typing_simple_example.py
+tests/typing/typing_version_option.py
```

### Comparing `click-8.1.4/tests/test_arguments.py` & `click-8.1.5/tests/test_arguments.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/tests/test_basic.py` & `click-8.1.5/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/tests/test_chain.py` & `click-8.1.5/tests/test_chain.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/tests/test_command_decorators.py` & `click-8.1.5/tests/test_command_decorators.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/tests/test_commands.py` & `click-8.1.5/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/tests/test_context.py` & `click-8.1.5/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/tests/test_custom_classes.py` & `click-8.1.5/tests/test_custom_classes.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/tests/test_defaults.py` & `click-8.1.5/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/tests/test_formatting.py` & `click-8.1.5/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/tests/test_imports.py` & `click-8.1.5/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/tests/test_info_dict.py` & `click-8.1.5/tests/test_info_dict.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/tests/test_normalization.py` & `click-8.1.5/tests/test_normalization.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/tests/test_options.py` & `click-8.1.5/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/tests/test_parser.py` & `click-8.1.5/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/tests/test_shell_completion.py` & `click-8.1.5/tests/test_shell_completion.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/tests/test_termui.py` & `click-8.1.5/tests/test_termui.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/tests/test_testing.py` & `click-8.1.5/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/tests/test_types.py` & `click-8.1.5/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/tests/test_utils.py` & `click-8.1.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `click-8.1.4/tox.ini` & `click-8.1.5/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -16,12 +16,15 @@
 [testenv:style]
 deps = pre-commit
 skip_install = true
 commands = pre-commit run --all-files
 
 [testenv:typing]
 deps = -r requirements/typing.txt
-commands = mypy
+commands =
+    mypy
+    pyright --verifytypes click
+    pyright tests/typing
 
 [testenv:docs]
 deps = -r requirements/docs.txt
 commands = sphinx-build -W -b html -d {envtmpdir}/doctrees docs {envtmpdir}/html
```

