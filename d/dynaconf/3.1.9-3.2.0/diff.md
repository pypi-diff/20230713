# Comparing `tmp/dynaconf-3.1.9.tar.gz` & `tmp/dynaconf-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynaconf-3.1.9.tar", last modified: Mon Jun  6 18:01:29 2022, max compression
+gzip compressed data, was "dynaconf-3.2.0.tar", last modified: Thu Jul 13 16:33:32 2023, max compression
```

## Comparing `dynaconf-3.1.9.tar` & `dynaconf-3.2.0.tar`

### file list

```diff
@@ -1,128 +1,144 @@
-drwxr-xr-x   0 rochacbruno  (1000) rochacbruno  (1000)        0 2022-06-06 18:01:29.069888 dynaconf-3.1.9/
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     5201 2022-01-03 18:49:36.000000 dynaconf-3.1.9/3.x-release-notes.md
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)   115581 2022-04-15 20:04:17.000000 dynaconf-3.1.9/CHANGELOG.md
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     5703 2022-01-03 18:49:36.000000 dynaconf-3.1.9/CONTRIBUTING.md
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     1700 2022-04-14 14:06:38.000000 dynaconf-3.1.9/CONTRIBUTORS.md
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     1078 2022-01-03 18:49:36.000000 dynaconf-3.1.9/LICENSE
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      110 2022-01-03 18:49:36.000000 dynaconf-3.1.9/MANIFEST.in
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     7777 2022-06-06 18:01:29.069888 dynaconf-3.1.9/PKG-INFO
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     6515 2022-01-03 18:49:36.000000 dynaconf-3.1.9/README.md
-drwxr-xr-x   0 rochacbruno  (1000) rochacbruno  (1000)        0 2022-06-06 18:01:29.059888 dynaconf-3.1.9/dynaconf/
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)        6 2022-06-06 18:01:23.000000 dynaconf-3.1.9/dynaconf/VERSION
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      841 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/__init__.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)    44509 2022-06-02 19:23:07.000000 dynaconf-3.1.9/dynaconf/base.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)    22106 2022-04-14 14:06:38.000000 dynaconf-3.1.9/dynaconf/cli.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     1223 2022-06-02 18:00:53.000000 dynaconf-3.1.9/dynaconf/constants.py
-drwxr-xr-x   0 rochacbruno  (1000) rochacbruno  (1000)        0 2022-06-06 18:01:29.059888 dynaconf-3.1.9/dynaconf/contrib/
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      204 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/contrib/__init__.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     4558 2022-06-02 19:23:07.000000 dynaconf-3.1.9/dynaconf/contrib/django_dynaconf_v2.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     7593 2022-03-30 20:47:51.000000 dynaconf-3.1.9/dynaconf/contrib/flask_dynaconf.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     9084 2022-06-02 19:23:07.000000 dynaconf-3.1.9/dynaconf/default_settings.py
-drwxr-xr-x   0 rochacbruno  (1000) rochacbruno  (1000)        0 2022-06-06 18:01:29.059888 dynaconf-3.1.9/dynaconf/loaders/
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     9340 2022-06-02 19:23:07.000000 dynaconf-3.1.9/dynaconf/loaders/__init__.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     6612 2022-06-02 19:23:07.000000 dynaconf-3.1.9/dynaconf/loaders/base.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     2946 2022-06-02 19:23:07.000000 dynaconf-3.1.9/dynaconf/loaders/env_loader.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     1867 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/loaders/ini_loader.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     2334 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/loaders/json_loader.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     4991 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/loaders/py_loader.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     3493 2022-03-30 20:49:10.000000 dynaconf-3.1.9/dynaconf/loaders/redis_loader.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     2072 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/loaders/toml_loader.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     6372 2022-03-30 20:47:51.000000 dynaconf-3.1.9/dynaconf/loaders/vault_loader.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     2688 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/loaders/yaml_loader.py
-drwxr-xr-x   0 rochacbruno  (1000) rochacbruno  (1000)        0 2022-06-06 18:01:29.059888 dynaconf-3.1.9/dynaconf/strategies/
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)        0 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/strategies/__init__.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      532 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/strategies/filtering.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      134 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/test_settings.py
-drwxr-xr-x   0 rochacbruno  (1000) rochacbruno  (1000)        0 2022-06-06 18:01:29.059888 dynaconf-3.1.9/dynaconf/utils/
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)    13761 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/utils/__init__.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     2999 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/utils/boxing.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     3250 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/utils/files.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     4469 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/utils/functional.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)    11568 2022-06-02 19:23:07.000000 dynaconf-3.1.9/dynaconf/utils/parse_conf.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)    15961 2022-06-02 19:23:07.000000 dynaconf-3.1.9/dynaconf/validator.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     1384 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/validator_conditions.py
-drwxr-xr-x   0 rochacbruno  (1000) rochacbruno  (1000)        0 2022-06-06 18:01:29.059888 dynaconf-3.1.9/dynaconf/vendor/
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)        0 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/__init__.py
-drwxr-xr-x   0 rochacbruno  (1000) rochacbruno  (1000)        0 2022-06-06 18:01:29.059888 dynaconf-3.1.9/dynaconf/vendor/box/
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      246 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/box/__init__.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)    13967 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/box/box.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     5501 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/box/box_list.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     1665 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/box/config_box.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     3165 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/box/converters.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      197 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/box/exceptions.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     1458 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/box/from_file.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      552 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/box/shorthand_box.py
-drwxr-xr-x   0 rochacbruno  (1000) rochacbruno  (1000)        0 2022-06-06 18:01:29.059888 dynaconf-3.1.9/dynaconf/vendor/click/
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     1971 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/click/__init__.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     6415 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/click/_bashcomplete.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     9848 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/click/_compat.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     9605 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/click/_termui_impl.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      704 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/click/_textwrap.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     1659 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/click/_unicodefun.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     4833 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/click/_winconsole.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)    25829 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/click/core.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     8707 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/click/decorators.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     3297 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/click/exceptions.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     3391 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/click/formatting.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      475 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/click/globals.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     5730 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/click/parser.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     5786 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/click/termui.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     4571 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/click/testing.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     9010 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/click/types.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     4360 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/click/utils.py
-drwxr-xr-x   0 rochacbruno  (1000) rochacbruno  (1000)        0 2022-06-06 18:01:29.059888 dynaconf-3.1.9/dynaconf/vendor/dotenv/
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      706 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/dotenv/__init__.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     2285 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/dotenv/cli.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      475 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/dotenv/compat.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      910 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/dotenv/ipython.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     5021 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/dotenv/main.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     3905 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/dotenv/parser.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)       20 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/dotenv/version.py
-drwxr-xr-x   0 rochacbruno  (1000) rochacbruno  (1000)        0 2022-06-06 18:01:29.059888 dynaconf-3.1.9/dynaconf/vendor/ruamel/
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)        0 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/__init__.py
-drwxr-xr-x   0 rochacbruno  (1000) rochacbruno  (1000)        0 2022-06-06 18:01:29.069888 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     1666 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/__init__.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      326 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/anchor.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)    16791 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/comments.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     4466 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/compat.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     4055 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/composer.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      254 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/configobjwalker.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)    40855 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/constructor.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     3261 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/cyaml.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     3517 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/dumper.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)    35864 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/emitter.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     5455 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/error.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     2311 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/events.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     1937 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/loader.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)    28419 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/main.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     1850 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/nodes.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)    16979 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/parser.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     5037 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/reader.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)    29471 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/representer.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     9559 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/resolver.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      729 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/scalarbool.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     2326 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/scalarfloat.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     2362 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/scalarint.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     2414 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/scalarstring.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)    32600 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/scanner.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     4116 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/serializer.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)    19019 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/setup.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      443 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/timestamp.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     3899 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/tokens.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     2067 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/util.py
-drwxr-xr-x   0 rochacbruno  (1000) rochacbruno  (1000)        0 2022-06-06 18:01:29.069888 dynaconf-3.1.9/dynaconf/vendor/toml/
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      586 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/toml/__init__.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)    16429 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/toml/decoder.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     4748 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/toml/encoder.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      299 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/toml/ordered.py
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      435 2022-01-03 18:49:36.000000 dynaconf-3.1.9/dynaconf/vendor/toml/tz.py
-drwxr-xr-x   0 rochacbruno  (1000) rochacbruno  (1000)        0 2022-06-06 18:01:29.059888 dynaconf-3.1.9/dynaconf.egg-info/
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     7777 2022-06-06 18:01:28.000000 dynaconf-3.1.9/dynaconf.egg-info/PKG-INFO
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     3595 2022-06-06 18:01:28.000000 dynaconf-3.1.9/dynaconf.egg-info/SOURCES.txt
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)        1 2022-06-06 18:01:28.000000 dynaconf-3.1.9/dynaconf.egg-info/dependency_links.txt
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)       48 2022-06-06 18:01:28.000000 dynaconf-3.1.9/dynaconf.egg-info/entry_points.txt
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)        1 2022-06-06 18:01:28.000000 dynaconf-3.1.9/dynaconf.egg-info/not-zip-safe
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      326 2022-06-06 18:01:28.000000 dynaconf-3.1.9/dynaconf.egg-info/requires.txt
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)        9 2022-06-06 18:01:28.000000 dynaconf-3.1.9/dynaconf.egg-info/top_level.txt
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)      423 2022-06-06 18:01:29.069888 dynaconf-3.1.9/setup.cfg
--rw-r--r--   0 rochacbruno  (1000) rochacbruno  (1000)     2836 2022-04-15 20:38:07.000000 dynaconf-3.1.9/setup.py
+drwxrwxr-x   0 pedro-psb  (1000) pedro-psb  (1000)        0 2023-07-13 16:33:32.158539 dynaconf-3.2.0/
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     5193 2023-06-30 15:30:10.000000 dynaconf-3.2.0/3.x-release-notes.md
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)   130416 2023-06-30 15:30:10.000000 dynaconf-3.2.0/CHANGELOG.md
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     5724 2023-06-30 15:30:10.000000 dynaconf-3.2.0/CONTRIBUTING.md
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     1700 2023-06-30 15:30:10.000000 dynaconf-3.2.0/CONTRIBUTORS.md
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     1078 2023-03-07 19:53:46.000000 dynaconf-3.2.0/LICENSE
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      147 2023-06-30 15:30:10.000000 dynaconf-3.2.0/MANIFEST.in
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     8157 2023-07-13 16:33:32.162539 dynaconf-3.2.0/PKG-INFO
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     6457 2023-06-30 15:30:10.000000 dynaconf-3.2.0/README.md
+drwxrwxr-x   0 pedro-psb  (1000) pedro-psb  (1000)        0 2023-07-13 16:33:32.142538 dynaconf-3.2.0/dynaconf/
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)        6 2023-07-13 16:32:55.000000 dynaconf-3.2.0/dynaconf/VERSION
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     1035 2023-07-10 15:14:13.000000 dynaconf-3.2.0/dynaconf/__init__.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)    50370 2023-07-13 16:31:12.000000 dynaconf-3.2.0/dynaconf/base.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)    25774 2023-07-13 16:31:12.000000 dynaconf-3.2.0/dynaconf/cli.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     1259 2023-06-30 15:30:10.000000 dynaconf-3.2.0/dynaconf/constants.py
+drwxrwxr-x   0 pedro-psb  (1000) pedro-psb  (1000)        0 2023-07-13 16:33:32.146538 dynaconf-3.2.0/dynaconf/contrib/
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      240 2023-06-30 15:30:10.000000 dynaconf-3.2.0/dynaconf/contrib/__init__.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     4594 2023-07-07 20:48:23.000000 dynaconf-3.2.0/dynaconf/contrib/django_dynaconf_v2.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     7566 2023-07-04 14:48:19.000000 dynaconf-3.2.0/dynaconf/contrib/flask_dynaconf.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     9701 2023-07-07 11:33:57.000000 dynaconf-3.2.0/dynaconf/default_settings.py
+drwxrwxr-x   0 pedro-psb  (1000) pedro-psb  (1000)        0 2023-07-13 16:33:32.146538 dynaconf-3.2.0/dynaconf/loaders/
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)    10737 2023-07-11 19:54:11.000000 dynaconf-3.2.0/dynaconf/loaders/__init__.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     8255 2023-07-13 16:31:12.000000 dynaconf-3.2.0/dynaconf/loaders/base.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     3891 2023-07-04 15:28:07.000000 dynaconf-3.2.0/dynaconf/loaders/env_loader.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     1943 2023-07-04 14:47:10.000000 dynaconf-3.2.0/dynaconf/loaders/ini_loader.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     2407 2023-07-05 20:00:34.000000 dynaconf-3.2.0/dynaconf/loaders/json_loader.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     5770 2023-07-13 16:31:12.000000 dynaconf-3.2.0/dynaconf/loaders/py_loader.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     3990 2023-07-13 16:31:12.000000 dynaconf-3.2.0/dynaconf/loaders/redis_loader.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     4290 2023-07-04 14:47:10.000000 dynaconf-3.2.0/dynaconf/loaders/toml_loader.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     7336 2023-07-13 16:31:12.000000 dynaconf-3.2.0/dynaconf/loaders/vault_loader.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     2858 2023-07-04 15:28:07.000000 dynaconf-3.2.0/dynaconf/loaders/yaml_loader.py
+drwxrwxr-x   0 pedro-psb  (1000) pedro-psb  (1000)        0 2023-07-13 16:33:32.146538 dynaconf-3.2.0/dynaconf/strategies/
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)        0 2023-04-03 19:45:39.000000 dynaconf-3.2.0/dynaconf/strategies/__init__.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      560 2023-06-30 15:30:10.000000 dynaconf-3.2.0/dynaconf/strategies/filtering.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      170 2023-06-30 15:30:10.000000 dynaconf-3.2.0/dynaconf/test_settings.py
+drwxrwxr-x   0 pedro-psb  (1000) pedro-psb  (1000)        0 2023-07-13 16:33:32.146538 dynaconf-3.2.0/dynaconf/utils/
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)    15335 2023-07-12 14:41:02.000000 dynaconf-3.2.0/dynaconf/utils/__init__.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     3031 2023-07-12 15:26:54.000000 dynaconf-3.2.0/dynaconf/utils/boxing.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     3355 2023-07-04 14:34:00.000000 dynaconf-3.2.0/dynaconf/utils/files.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     4505 2023-07-03 20:59:02.000000 dynaconf-3.2.0/dynaconf/utils/functional.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     7002 2023-07-13 16:30:00.000000 dynaconf-3.2.0/dynaconf/utils/inspect.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)    13171 2023-07-12 14:40:41.000000 dynaconf-3.2.0/dynaconf/utils/parse_conf.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)    17795 2023-07-04 15:28:07.000000 dynaconf-3.2.0/dynaconf/validator.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     1526 2023-06-30 15:30:10.000000 dynaconf-3.2.0/dynaconf/validator_conditions.py
+drwxrwxr-x   0 pedro-psb  (1000) pedro-psb  (1000)        0 2023-07-13 16:33:32.146538 dynaconf-3.2.0/dynaconf/vendor/
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)        0 2023-07-13 16:33:00.000000 dynaconf-3.2.0/dynaconf/vendor/__init__.py
+drwxrwxr-x   0 pedro-psb  (1000) pedro-psb  (1000)        0 2023-07-13 16:33:32.150539 dynaconf-3.2.0/dynaconf/vendor/box/
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      268 2023-07-13 16:33:03.000000 dynaconf-3.2.0/dynaconf/vendor/box/__init__.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)    14045 2023-07-13 16:33:01.000000 dynaconf-3.2.0/dynaconf/vendor/box/box.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     5521 2023-07-13 16:33:01.000000 dynaconf-3.2.0/dynaconf/vendor/box/box_list.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     1679 2023-07-13 16:33:01.000000 dynaconf-3.2.0/dynaconf/vendor/box/config_box.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     3192 2023-07-13 16:33:02.000000 dynaconf-3.2.0/dynaconf/vendor/box/converters.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      219 2023-07-13 16:33:02.000000 dynaconf-3.2.0/dynaconf/vendor/box/exceptions.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     1483 2023-07-13 16:33:03.000000 dynaconf-3.2.0/dynaconf/vendor/box/from_file.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      574 2023-07-13 16:33:03.000000 dynaconf-3.2.0/dynaconf/vendor/box/shorthand_box.py
+drwxrwxr-x   0 pedro-psb  (1000) pedro-psb  (1000)        0 2023-07-13 16:33:32.150539 dynaconf-3.2.0/dynaconf/vendor/click/
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     1971 2023-07-13 16:33:07.000000 dynaconf-3.2.0/dynaconf/vendor/click/__init__.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     6407 2023-07-13 16:33:04.000000 dynaconf-3.2.0/dynaconf/vendor/click/_bashcomplete.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     9830 2023-07-13 16:33:04.000000 dynaconf-3.2.0/dynaconf/vendor/click/_compat.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     9600 2023-07-13 16:33:08.000000 dynaconf-3.2.0/dynaconf/vendor/click/_termui_impl.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      704 2023-07-13 16:33:09.000000 dynaconf-3.2.0/dynaconf/vendor/click/_textwrap.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     1659 2023-07-13 16:33:10.000000 dynaconf-3.2.0/dynaconf/vendor/click/_unicodefun.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     4833 2023-07-13 16:33:11.000000 dynaconf-3.2.0/dynaconf/vendor/click/_winconsole.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)    25824 2023-07-13 16:33:05.000000 dynaconf-3.2.0/dynaconf/vendor/click/core.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     8721 2023-07-13 16:33:05.000000 dynaconf-3.2.0/dynaconf/vendor/click/decorators.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     3297 2023-07-13 16:33:06.000000 dynaconf-3.2.0/dynaconf/vendor/click/exceptions.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     3391 2023-07-13 16:33:06.000000 dynaconf-3.2.0/dynaconf/vendor/click/formatting.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      473 2023-07-13 16:33:06.000000 dynaconf-3.2.0/dynaconf/vendor/click/globals.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     5723 2023-07-13 16:33:07.000000 dynaconf-3.2.0/dynaconf/vendor/click/parser.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     5786 2023-07-13 16:33:08.000000 dynaconf-3.2.0/dynaconf/vendor/click/termui.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     4569 2023-07-13 16:33:09.000000 dynaconf-3.2.0/dynaconf/vendor/click/testing.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     9008 2023-07-13 16:33:09.000000 dynaconf-3.2.0/dynaconf/vendor/click/types.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     4362 2023-07-13 16:33:10.000000 dynaconf-3.2.0/dynaconf/vendor/click/utils.py
+drwxrwxr-x   0 pedro-psb  (1000) pedro-psb  (1000)        0 2023-07-13 16:33:32.154539 dynaconf-3.2.0/dynaconf/vendor/dotenv/
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      702 2023-07-13 16:33:12.000000 dynaconf-3.2.0/dynaconf/vendor/dotenv/__init__.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     2285 2023-07-13 16:33:11.000000 dynaconf-3.2.0/dynaconf/vendor/dotenv/cli.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      473 2023-07-13 16:33:11.000000 dynaconf-3.2.0/dynaconf/vendor/dotenv/compat.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      909 2023-07-13 16:33:12.000000 dynaconf-3.2.0/dynaconf/vendor/dotenv/ipython.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     5016 2023-07-13 16:33:12.000000 dynaconf-3.2.0/dynaconf/vendor/dotenv/main.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     3898 2023-07-13 16:33:13.000000 dynaconf-3.2.0/dynaconf/vendor/dotenv/parser.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)       20 2023-07-13 16:33:13.000000 dynaconf-3.2.0/dynaconf/vendor/dotenv/version.py
+drwxrwxr-x   0 pedro-psb  (1000) pedro-psb  (1000)        0 2023-07-13 16:33:32.154539 dynaconf-3.2.0/dynaconf/vendor/ruamel/
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)        0 2023-07-13 16:33:31.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/__init__.py
+drwxrwxr-x   0 pedro-psb  (1000) pedro-psb  (1000)        0 2023-07-13 16:33:32.158539 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     1661 2023-07-13 16:33:19.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/__init__.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      323 2023-07-13 16:33:13.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/anchor.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)    16788 2023-07-13 16:33:14.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/comments.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     4470 2023-07-13 16:33:15.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/compat.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     4052 2023-07-13 16:33:15.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/composer.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      254 2023-07-13 16:33:15.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/configobjwalker.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)    40831 2023-07-13 16:33:16.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/constructor.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     3261 2023-07-13 16:33:16.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/cyaml.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     3517 2023-07-13 16:33:17.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/dumper.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)    35839 2023-07-13 16:33:18.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/emitter.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     5445 2023-07-13 16:33:18.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/error.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     2309 2023-07-13 16:33:18.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/events.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     1937 2023-07-13 16:33:19.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/loader.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)    28409 2023-07-13 16:33:20.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/main.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     1850 2023-07-13 16:33:20.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/nodes.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)    16973 2023-07-13 16:33:21.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/parser.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     5029 2023-07-13 16:33:21.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/reader.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)    29443 2023-07-13 16:33:22.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/representer.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     9554 2023-07-13 16:33:22.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/resolver.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      731 2023-07-13 16:33:23.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/scalarbool.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     2328 2023-07-13 16:33:23.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/scalarfloat.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     2364 2023-07-13 16:33:23.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/scalarint.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     2414 2023-07-13 16:33:24.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/scalarstring.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)    32540 2023-07-13 16:33:24.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/scanner.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     4113 2023-07-13 16:33:25.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/serializer.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)    19019 2023-07-13 16:33:25.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/setup.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      442 2023-07-13 16:33:26.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/timestamp.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     3899 2023-07-13 16:33:26.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/tokens.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     2066 2023-07-13 16:33:27.000000 dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/util.py
+drwxrwxr-x   0 pedro-psb  (1000) pedro-psb  (1000)        0 2023-07-13 16:33:32.158539 dynaconf-3.2.0/dynaconf/vendor/toml/
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      586 2023-07-13 16:33:28.000000 dynaconf-3.2.0/dynaconf/vendor/toml/__init__.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)    16403 2023-07-13 16:33:27.000000 dynaconf-3.2.0/dynaconf/vendor/toml/decoder.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     4738 2023-07-13 16:33:28.000000 dynaconf-3.2.0/dynaconf/vendor/toml/encoder.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      299 2023-07-13 16:33:28.000000 dynaconf-3.2.0/dynaconf/vendor/toml/ordered.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      435 2023-07-13 16:33:29.000000 dynaconf-3.2.0/dynaconf/vendor/toml/tz.py
+drwxrwxr-x   0 pedro-psb  (1000) pedro-psb  (1000)        0 2023-07-13 16:33:32.158539 dynaconf-3.2.0/dynaconf/vendor/tomllib/
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      171 2023-07-13 16:33:29.000000 dynaconf-3.2.0/dynaconf/vendor/tomllib/__init__.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)    11509 2023-07-13 16:33:30.000000 dynaconf-3.2.0/dynaconf/vendor/tomllib/_parser.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     1687 2023-07-13 16:33:30.000000 dynaconf-3.2.0/dynaconf/vendor/tomllib/_re.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)       95 2023-07-13 16:33:30.000000 dynaconf-3.2.0/dynaconf/vendor/tomllib/_types.py
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     3596 2023-07-13 16:33:31.000000 dynaconf-3.2.0/dynaconf/vendor/tomllib/_writer.py
+drwxrwxr-x   0 pedro-psb  (1000) pedro-psb  (1000)        0 2023-07-13 16:33:32.142538 dynaconf-3.2.0/dynaconf.egg-info/
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     8157 2023-07-13 16:33:32.000000 dynaconf-3.2.0/dynaconf.egg-info/PKG-INFO
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     4071 2023-07-13 16:33:32.000000 dynaconf-3.2.0/dynaconf.egg-info/SOURCES.txt
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)        1 2023-07-13 16:33:32.000000 dynaconf-3.2.0/dynaconf.egg-info/dependency_links.txt
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)       47 2023-07-13 16:33:32.000000 dynaconf-3.2.0/dynaconf.egg-info/entry_points.txt
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)        1 2023-07-13 16:33:32.000000 dynaconf-3.2.0/dynaconf.egg-info/not-zip-safe
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      318 2023-07-13 16:33:32.000000 dynaconf-3.2.0/dynaconf.egg-info/requires.txt
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)        9 2023-07-13 16:33:32.000000 dynaconf-3.2.0/dynaconf.egg-info/top_level.txt
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      423 2023-07-13 16:33:32.162539 dynaconf-3.2.0/setup.cfg
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     2950 2023-07-04 14:48:10.000000 dynaconf-3.2.0/setup.py
+drwxrwxr-x   0 pedro-psb  (1000) pedro-psb  (1000)        0 2023-07-13 16:33:32.158539 dynaconf-3.2.0/vendor_licenses/
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     1076 2023-06-30 15:30:10.000000 dynaconf-3.2.0/vendor_licenses/box-LICENSE.txt
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     1475 2023-06-30 15:30:10.000000 dynaconf-3.2.0/vendor_licenses/click-LICENSE.rst
+-rwxrwxr-x   0 pedro-psb  (1000) pedro-psb  (1000)      769 2023-06-30 15:30:10.000000 dynaconf-3.2.0/vendor_licenses/licenses.sh
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     4600 2023-06-30 15:30:10.000000 dynaconf-3.2.0/vendor_licenses/python-dotenv-LICENSE.txt
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     1121 2023-06-30 15:30:10.000000 dynaconf-3.2.0/vendor_licenses/ruamel.yaml-LICENSE.txt
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     1253 2023-06-30 15:30:10.000000 dynaconf-3.2.0/vendor_licenses/toml-LICENSE.txt
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)     1072 2023-06-30 15:30:10.000000 dynaconf-3.2.0/vendor_licenses/tomli-LICENSE.txt
+-rw-rw-r--   0 pedro-psb  (1000) pedro-psb  (1000)      100 2023-07-13 16:33:00.000000 dynaconf-3.2.0/vendor_licenses/vendor_versions.txt
```

### Comparing `dynaconf-3.1.9/3.x-release-notes.md` & `dynaconf-3.2.0/3.x-release-notes.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Dynaconf 3.0.0
 
 In Dynaconf 3.0.0 we introduced some improvements and with
 those improvements it comes some **breaking changes.**
 
-Some of the changes were discussed on the **1st Dynaconf community meeting** [video is available](https://www.twitch.tv/videos/657033043) and [meeting notes #354](https://github.com/rochacbruno/dynaconf/issues/354).
+Some of the changes were discussed on the **1st Dynaconf community meeting** [video is available](https://www.twitch.tv/videos/657033043) and [meeting notes #354](https://github.com/dynaconf/dynaconf/issues/354).
 
 
 ## Improvements
 
-- Validators now implements `|` and `&` operators to allow `Validator() &| Validator()` and has more `operations` available such as `len_eq, len_min, len_max, startswith` [#353](https://github.com/rochacbruno/dynaconf/pull/353).
-- First level variables are now allowed to be `lowercase` it is now possible to access `settings.foo` or `settings.FOO` [#357](https://github.com/rochacbruno/dynaconf/pull/357).
+- Validators now implements `|` and `&` operators to allow `Validator() &| Validator()` and has more `operations` available such as `len_eq, len_min, len_max, startswith` [#353](https://github.com/dynaconf/dynaconf/pull/353).
+- First level variables are now allowed to be `lowercase` it is now possible to access `settings.foo` or `settings.FOO` [#357](https://github.com/dynaconf/dynaconf/pull/357).
 - All Dependencies are now vendored, so when installing Dynaconf is not needed to install any dependency.
 - Dynaconf configuration options are now aliased so when creating an instance of `LazySettings|FlaskDynaconf|DjangoDynaconf` it is now possible to pass instead of `ENVVAR_PREFIX_FOR_DYNACONF` just `envvar_prefix` and this lowercase alias is now accepted.
 - Fixed bugs in `merge` and deprecated the `@reset` token.
 - Added implementation for `__dir__` to allow auto complete for terminal and IDEs.
 - Add option to override mount point for vault server.
 - `LazySettings` is now aliased to `Dynaconf`
 - `Dynaconf` class now accepts a parameter `validators=[Validator, ...]` that will be immediately evaluated when passed.
@@ -62,15 +62,15 @@
 [default]
 key = 'value'
 
 [production]
 key = 'value'
 ```
 
-**Now starting on 3.0.0** the environments are disabled by default, so the same file can be crated as.
+**Now starting on 3.0.0** the environments are disabled by default, so the same file can be created as.
 
 ```toml
 key = 'value'
 ```
 
 And you can still have the environments but only if you explicit specify it when creating your instance.
```

### Comparing `dynaconf-3.1.9/CHANGELOG.md` & `dynaconf-3.2.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,480 @@
 Changelog
 =========
 
 
+3.1.12 (2023-03-02)
+-------------------
+
+Fix
+~~~
+- Envvars.md get `HOME` environment variable (#831) [MicLon]
+
+Other
+~~~~~
+- Release version 3.1.12. [Bruno Rocha]
+
+  Shortlog of commits since last release:
+
+      André "decko" de Brito (2):
+            Removes Codacy Coverage Reporter (#871)
+            Add a namespace property for VAULT_FOR_DYNACONF dict (#870)
+
+      Bruno Rocha (8):
+            Release version 3.1.11
+            bump dev version to 3.1.12
+            Ensure `dynaconf get` returns a valid json string. (#813)
+            [bugfix] Fix access of keys with spaces (#815)
+            hotfix func tests (#816)
+            Add Python 3.11 to CI (#830)
+            fix lint error
+            Fix casting on Validator and improve docs (#873)
+
+      Bryan Weber (1):
+            Fix typos in envvars docs (#840)
+
+      Florian Apolloner (1):
+            Small typo fix. (#822)
+
+      Maxwell G (1):
+            Include license files for vendored deps (#841)
+
+      MicLon (1):
+            fix: envvars.md get `HOME` environment variable (#831)
+
+      Otávio Dantas (1):
+            doc(pt-br): translate flask extension to pt-br (#852)
+
+      Sergio Kef (1):
+            Fix code snippet in docs (#843)
+
+      Tetiana (1):
+            #817 Add note about defining root_path when testing (#818)
+
+      jctanner (1):
+            Handle all failures when pwd does not exist. (#857)
+
+      jmeichle (1):
+            Add support for VAULT_NAMESPACE_FOR_DYNACONF (#854)
+- Fix casting on Validator and improve docs (#873) [Bruno Rocha]
+
+  fix: #823
+  fix: #834
+- Fix lint error. [Bruno Rocha]
+- Small typo fix. (#822) [Bruno Rocha, Florian Apolloner]
+- Fix typos in envvars docs (#840) [Bruno Rocha, Bryan Weber]
+- Include license files for vendored deps (#841) [Bruno Rocha, Maxwell
+  G]
+- Fix code snippet in docs (#843) [Sergio Kef]
+
+  Fix syntax error, missing comma
+- Add a namespace property for VAULT_FOR_DYNACONF dict (#870) [André
+  "decko" de Brito, Bruno Rocha]
+- Removes Codacy Coverage Reporter (#871) [André "decko" de Brito]
+- Add support for VAULT_NAMESPACE_FOR_DYNACONF (#854) [Bruno Rocha,
+  jmeichle]
+
+  * Add support for VAULT_NAMESPACE_FOR_DYNACONF
+
+  * adjusting for linting
+
+  ---------
+- Handle all failures when pwd does not exist. (#857) [jctanner]
+
+  * Handle all failures when pwd does not exist.
+
+  ---------
+- Doc(pt-br): translate flask extension to pt-br (#852) [Otávio Dantas]
+- Add Python 3.11 to CI (#830) [Bruno Rocha, Vicente Marçal]
+
+  Fix a testing error on CI
+- #817 Add note about defining root_path when testing (#818) [Tetiana]
+
+  fix #817
+- Hotfix func tests (#816) [Bruno Rocha]
+- [bugfix] Fix access of keys with spaces (#815) [Bruno Rocha]
+
+  Fix #814
+- Ensure `dynaconf get` returns a valid json string. (#813) [Bruno
+  Rocha]
+- Bump dev version to 3.1.12. [Bruno Rocha]
+- Release version 3.1.11. [Bruno Rocha]
+
+  This release is a hotfix on top of 3.1.10
+
+  Please read changelog from  https://github.com/dynaconf/dynaconf/releases/tag/3.1.10
+
+  Shortlog of commits since last release:
+
+      Bruno Rocha (2):
+            Release version 3.1.10
+            Release hotfix (no need to run coverage or include tests_functional)
+
+
+3.1.11 (2022-09-22)
+-------------------
+- Release version 3.1.11. [Bruno Rocha]
+
+  Shortlog of commits since last release:
+
+      Bruno Rocha (2):
+            Release version 3.1.10
+            Release hotfix (no need to run coverage or include tests_functional)
+- Release hotfix (no need to run coverage or include tests_functional)
+  [Bruno Rocha]
+- Release version 3.1.10. [Bruno Rocha]
+
+  Shortlog of commits since last release:
+
+      Amadou Crookes (1):
+            envars.md typo fix (#786)
+
+      Bruno Rocha (19):
+            Release version 3.1.9
+            Bump dev version to 3.1.10
+            Update badges
+            demo repo will be replaced by a video tutorial soon
+            Fix CI
+            New data key casing must adapt to existing key casing (#795)
+            Add test and docs about includes (#796)
+            Removed vendor_src folder (#798)
+            Replacing rochacbruno/ with dynaconf/ (#800)
+            Fix codecov (#801)
+            Parse negative numbers from envvar Fix #799 and Fix #585 (#802)
+            Fix get command with Django (#804)
+            Add a functional test runner (#805)
+            Test runner docs and styling (#806)
+            Allow merge_unique on lists when merge_enabled=True (#810)
+            Rebind current env when forced for Pytest Fix #728 (#809)
+            AUTO_CAST can be enabled on instance (#811)
+            Ensure pyminify is on release script
+            Add missing tomllib to monify script
+
+      Gaurav Talreja (1):
+            Fix #807 Use client.auth.approle.login instead of client.auth_approle (#808)
+
+      Jitendra Yejare (1):
+            Fix #768 of kv property depreciation from client object (#769)
+
+      Joren Retel (2):
+            Feature/detect casting comb token from converters (#784)
+            Adding documentation and example to makefile. (#791)
+
+      João Gustavo A. Amorim (1):
+            Add pyupgrade hook (#759)
+
+      Kian-Meng Ang (1):
+            Fix typos (#788)
+
+      Lucas Limeira (1):
+            Using filter_strategy in env_loader to fix #760 (#767)
+
+      Nicholas Nadeau, Ph.D., P.Eng (1):
+            fix: typo (#766)
+
+      Oleksii Baranov (2):
+            Bump codecov action version (#775)
+            Fix cli init command for flask (#705) (#774)
+
+      Pedro de Medeiros (1):
+            documentation fixes (#771)
+
+      The Gitter Badger (1):
+            Add a Gitter chat badge to README.md (#776)
+
+      Théo Melo (1):
+            Fixing a typo on the readme file (#763)
+
+      Vicente Marçal (1):
+            docs(pt-br): Docs Translation to brazilian portugues. (#787)
+
+
+3.1.10 (2022-09-22)
+-------------------
+
+Fix
+~~~
+- Typo (#766) [Bruno Rocha, Nicholas Nadeau, Ph.D., P.Eng]
+
+Other
+~~~~~
+- Release version 3.1.10. [Bruno Rocha]
+
+  Shortlog of commits since last release:
+
+      Amadou Crookes (1):
+            envars.md typo fix (#786)
+
+      Bruno Rocha (19):
+            Release version 3.1.9
+            Bump dev version to 3.1.10
+            Update badges
+            demo repo will be replaced by a video tutorial soon
+            Fix CI
+            New data key casing must adapt to existing key casing (#795)
+            Add test and docs about includes (#796)
+            Removed vendor_src folder (#798)
+            Replacing rochacbruno/ with dynaconf/ (#800)
+            Fix codecov (#801)
+            Parse negative numbers from envvar Fix #799 and Fix #585 (#802)
+            Fix get command with Django (#804)
+            Add a functional test runner (#805)
+            Test runner docs and styling (#806)
+            Allow merge_unique on lists when merge_enabled=True (#810)
+            Rebind current env when forced for Pytest Fix #728 (#809)
+            AUTO_CAST can be enabled on instance (#811)
+            Ensure pyminify is on release script
+            Add missing tomllib to monify script
+
+      Gaurav Talreja (1):
+            Fix #807 Use client.auth.approle.login instead of client.auth_approle (#808)
+
+      Jitendra Yejare (1):
+            Fix #768 of kv property depreciation from client object (#769)
+
+      Joren Retel (2):
+            Feature/detect casting comb token from converters (#784)
+            Adding documentation and example to makefile. (#791)
+
+      João Gustavo A. Amorim (1):
+            Add pyupgrade hook (#759)
+
+      Kian-Meng Ang (1):
+            Fix typos (#788)
+
+      Lucas Limeira (1):
+            Using filter_strategy in env_loader to fix #760 (#767)
+
+      Nicholas Nadeau, Ph.D., P.Eng (1):
+            fix: typo (#766)
+
+      Oleksii Baranov (2):
+            Bump codecov action version (#775)
+            Fix cli init command for flask (#705) (#774)
+
+      Pedro de Medeiros (1):
+            documentation fixes (#771)
+
+      The Gitter Badger (1):
+            Add a Gitter chat badge to README.md (#776)
+
+      Théo Melo (1):
+            Fixing a typo on the readme file (#763)
+
+      Vicente Marçal (1):
+            docs(pt-br): Docs Translation to brazilian portugues. (#787)
+- Add missing tomllib to monify script. [Bruno Rocha]
+- Ensure pyminify is on release script. [Bruno Rocha]
+- AUTO_CAST can be enabled on instance (#811) [Bruno Rocha]
+
+  Fix #772
+- Rebind current env when forced for Pytest Fix #728 (#809) [Bruno
+  Rocha]
+- Allow merge_unique on lists when merge_enabled=True (#810) [Bruno
+  Rocha]
+
+  Fix #726
+- Fix #807 Use client.auth.approle.login instead of client.auth_approle
+  (#808) [Gaurav Talreja]
+- Fix typos (#788) [Kian-Meng Ang]
+
+  Found via this command:
+
+      codespell -S "./dynaconf/vendor/*,./docs/pt-br/*,./.mypy_cache/*,*.svg" -L hashi
+- Test runner docs and styling (#806) [Bruno Rocha]
+
+  * Test runner docs and styling
+
+  * No emojis on windows
+- Add a functional test runner (#805) [Bruno Rocha]
+
+  * Add a functional test runner
+
+  * Renamed example/ to tests_functional/
+- Fix get command with Django (#804) [Bruno Rocha]
+
+  Fix #789
+- Parse negative numbers from envvar Fix #799 and Fix #585 (#802) [Bruno
+  Rocha]
+- Fix codecov (#801) [Bruno Rocha]
+
+  * Fix codecov
+
+  * call coverage xml
+- Replacing rochacbruno/ with dynaconf/ (#800) [Bruno Rocha]
+
+  * Replacing rochacbruno/ with dynaconf/
+
+  * xscode doesn't exist anymore
+- Removed vendor_src folder (#798) [Bruno Rocha]
+
+  * Removed vendor_src folder
+
+  Now `vendor` is the source
+  and minification happens during release process.
+
+  * Added tomllib (vendored) as a replacement for toml fix #708
+
+  toml kept as a fallback until 4.0.0 to nor break compatibility
+
+  - toml follows 0.5.0 spec
+  - tomlib follows 1.0.0 spec
+  - toml allows emojis and unicode chars unencoded
+  - tomllib foolows the spec where only encoded chars are allowed
+- Add test and docs about includes (#796) [Bruno Rocha]
+
+  closes #794
+- New data key casing must adapt to existing key casing (#795) [Bruno
+  Rocha]
+
+  Fix #737
+- Docs(pt-br): Docs Translation to brazilian portugues. (#787) [Vicente
+  Marçal]
+- Adding documentation and example to makefile. (#791) [Joren Retel]
+
+  * Adding documentation and example to makefile.
+
+  * Put header one level down in  docs.
+- Feature/detect casting comb token from converters (#784) [Joren Retel]
+- Envars.md typo fix (#786) [Amadou Crookes]
+- Fix CI. [Bruno Rocha]
+- Demo repo will be replaced by a video tutorial soon. [Bruno Rocha]
+- Update badges. [Bruno Rocha]
+- Documentation fixes (#771) [Bruno Rocha, Pedro de Medeiros]
+- Add a Gitter chat badge to README.md (#776) [Bruno Rocha, The Gitter
+  Badger]
+- Fix cli init command for flask (#705) (#774) [Bruno Rocha, Oleksii
+  Baranov]
+- Bump codecov action version (#775) [Oleksii Baranov]
+- Fix #768 of kv property depreciation from client object (#769)
+  [Jitendra Yejare]
+- Using filter_strategy in env_loader to fix #760 (#767) [Lucas Limeira]
+- Fixing a typo on the readme file (#763) [Théo Melo]
+- Add pyupgrade hook (#759) [João Gustavo A. Amorim]
+
+  * update hooks and add pyupgrade
+
+  * updates by pyupgrade
+
+  * remove unused typing imports
+
+  * add `from __future__ import annotations` across the codebase
+
+  * add `from __future__ import annotations` in examples
+- Bump dev version to 3.1.10. [Bruno Rocha]
+- Release version 3.1.9. [Bruno Rocha]
+
+  Shortlog of commits since last release:
+
+      Bruno Rocha (4):
+            Release version 3.1.8
+            Bye py 3.7
+            Multiple fixes for 3.19 (#756)
+            update docs site (#758)
+
+      João Gustavo A. Amorim (1):
+            Organize pre-commit setup (#757)
+
+      dependabot[bot] (1):
+            Bump django from 2.2.27 to 2.2.28 in /example/django_pytest_pure (#743)
+
+
+3.1.9 (2022-06-06)
+------------------
+- Release version 3.1.9. [Bruno Rocha]
+
+  Shortlog of commits since last release:
+
+      Bruno Rocha (4):
+            Release version 3.1.8
+            Bye py 3.7
+            Multiple fixes for 3.19 (#756)
+            update docs site (#758)
+
+      João Gustavo A. Amorim (1):
+            Organize pre-commit setup (#757)
+
+      dependabot[bot] (1):
+            Bump django from 2.2.27 to 2.2.28 in /example/django_pytest_pure (#743)
+- Update docs site (#758) [Bruno Rocha]
+- Organize pre-commit setup (#757) [João Gustavo A. Amorim]
+- Multiple fixes for 3.19 (#756) [Bruno Rocha]
+- Bump django from 2.2.27 to 2.2.28 in /example/django_pytest_pure
+  (#743) [dependabot[bot], dependabot[bot]]
+- Bye py 3.7. [Bruno Rocha]
+- Release version 3.1.8. [Bruno Rocha]
+
+  Shortlog of commits since last release:
+
+      Anderson Sousa (1):
+            Document the usage with python -m (#710)
+
+      Andressa Cabistani (2):
+            Add unique label when merging lists to fix issue #653 (#661)
+            Add new validation to fix issue #585 (#667)
+
+      Armin Berres (1):
+            Fix typo in error message
+
+      Bruno Rocha (7):
+            Release version 3.1.7
+            Found this bug that was duplicating the generated envlist (#663)
+            Add support for Python 3.10 (#665)
+            Attempt to fix #555 (#669)
+            Create update_contributors.yml
+            Fixing pre-coomit and docs CI
+            Added `dynaconf get` command to cli (#730)
+
+      Caneco (2):
+            improvement: add brand new logo to the project (#686)
+            improvement: update socialcard to match the python way (#687)
+
+      EdwardCuiPeacock (2):
+            Feature: add @jinja and @format casting (#704)
+            Combo converter doc (#735)
+
+      Eitan Mosenkis (1):
+            Fix FlaskConfig.setdefault (#706)
+
+      Enderson Menezes (Mr. Enderson) (2):
+            Force PYTHONIOENCODING to utf-8 to fix #664 (#672)
+            edit: move discussions to github tab (#682)
+
+      Eugene Triguba (1):
+            Fix custom prefix link in envvar documentation (#680)
+
+      Gibran Herrera (1):
+            Fix Issue 662 Lazy validation (#675)
+
+      Jitendra Yejare (2):
+            Load vault secrets from environment less stores or which are not written by dynaconf (#725)
+            Use default value when settings is blank (#729)
+
+      Pavel Alimpiev (1):
+            Update docs link (#678)
+
+      Ugo Benassayag (1):
+            Added validate_only_current_env to validator (issue #734) (#736)
+
+      Waylon Walker (1):
+            Docs Fix Spelling (#696)
+
+      dependabot[bot] (3):
+            Bump django from 2.1.5 to 2.2.26 in /example/django_pytest_pure (#711)
+            Bump mkdocs from 1.1.2 to 1.2.3 (#715)
+            Bump django from 2.2.26 to 2.2.27 in /example/django_pytest_pure (#717)
+
+      github-actions[bot] (2):
+            [automated] Update Contributors File (#691)
+            [automated] Update Contributors File (#732)
+
+      lowercase00 (1):
+            Makes Django/Flask kwargs case insensitive (#721)
+
+
 3.1.8 (2022-04-15)
 ------------------
 - Release version 3.1.8. [Bruno Rocha]
 
   Shortlog of commits since last release:
 
       Anderson Sousa (1):
```

### Comparing `dynaconf-3.1.9/CONTRIBUTING.md` & `dynaconf-3.2.0/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 ## Pull Request Process
 
 1. Ensure your local environment is set.
    1. Clone your own fork of this repo
    2. Activate a python3.6+ virtualenv
    3. Code
 2. Update the `docs/guides/` related to your changes.
-3. Update `example/` (editing or adding a new one related to your changes)
+3. Update `tests_functional/` (editing or adding a new one related to your changes)
 4. Ensure tests are passing (see below `make all`)
    1. This project uses `pre-commit` and `Black` for code styling and adequacy tests.
 5. Commit, Push and make a Pull Request!
 
 
 ### Common Workflow:
 
 ```bash
 # clone your fork of this repo
 git clone git@github.com:{$USER}/dynaconf.git
 
 # Add the upstream remote
-git remote add upstream https://github.com/rochacbruno/dynaconf.git
+git remote add upstream https://github.com/dynaconf/dynaconf.git
 
 # Activate your Python Environment
 python3.7 -m venv venv
 source venv/bin/activate
 
 # Install dynaconf for development
 make all
@@ -43,27 +43,27 @@
 code .
 
 # After editing please rebase with upstream
 git fetch upstream; git rebase upstream/master
 # Fix any conflicts if any.
 
 # Update docs/guides/ if needed
-# Edit example/ if needed
-# Create a new app in example/{your_example} and add it to Makefile.
+# Edit tests_functional/ if needed
+# Create a new app in tests_functional/{your_example} and add it to Makefile.
 
 # Then ensure everything is ok
 make all
 
 # Now commit your changes
 git commit -am "Changed XPTO to fix #issue_number"
 
 # Push to your own fork
 git push -u origin HEAD
 
-# Open github.com/rochacbruno/dynaconf and send a Pull Request.
+# Open github.com/dynaconf/dynaconf and send a Pull Request.
 ```
 
 ### Run integration tests
 
 * "make all" do not run integration tests for Redis and Vault.
 * If you want to run integration tests, make sure you have docker installed
```

### Comparing `dynaconf-3.1.9/CONTRIBUTORS.md` & `dynaconf-3.2.0/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `dynaconf-3.1.9/LICENSE` & `dynaconf-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dynaconf-3.1.9/PKG-INFO` & `dynaconf-3.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dynaconf
-Version: 3.1.9
+Version: 3.2.0
 Summary: The dynamic configurator for your Python Project
-Home-page: https://github.com/rochacbruno/dynaconf
+Home-page: https://github.com/dynaconf/dynaconf
 Author: Bruno Rocha
 Author-email: rochacbruno@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Flask
@@ -16,59 +16,61 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: redis
 Provides-Extra: vault
 Provides-Extra: yaml
 Provides-Extra: toml
 Provides-Extra: ini
 Provides-Extra: configobj
 Provides-Extra: all
 Provides-Extra: test
 License-File: LICENSE
+License-File: vendor_licenses/box-LICENSE.txt
+License-File: vendor_licenses/click-LICENSE.rst
+License-File: vendor_licenses/licenses.sh
+License-File: vendor_licenses/python-dotenv-LICENSE.txt
+License-File: vendor_licenses/ruamel.yaml-LICENSE.txt
+License-File: vendor_licenses/toml-LICENSE.txt
+License-File: vendor_licenses/tomli-LICENSE.txt
+License-File: vendor_licenses/vendor_versions.txt
 
 <!-- [![Dynaconf](docs/img/logo_400.svg?sanitize=true)](http://dynaconf.com) -->
 
 <p align="center"><img src="/art/header.png?v2" alt="dynaconf. new logo"></p>
 
 > **dynaconf** - Configuration Management for Python.
 
-[![MIT License](https://img.shields.io/badge/license-MIT-007EC7.svg?style=flat-square)](/LICENSE) [![PyPI](https://img.shields.io/pypi/v/dynaconf.svg)](https://pypi.python.org/pypi/dynaconf) [![PyPI](https://img.shields.io/pypi/pyversions/dynaconf.svg)]() ![PyPI - Downloads](https://img.shields.io/pypi/dm/dynaconf.svg?label=pip%20installs&logo=python) [![CI](https://github.com/rochacbruno/dynaconf/actions/workflows/main.yml/badge.svg)](https://github.com/rochacbruno/dynaconf/actions/workflows/main.yml) [![codecov](https://codecov.io/gh/rochacbruno/dynaconf/branch/master/graph/badge.svg)](https://codecov.io/gh/rochacbruno/dynaconf) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/42d2f11ef0a446808b246c8c69603f6e)](https://www.codacy.com/gh/rochacbruno/dynaconf/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=rochacbruno/dynaconf&amp;utm_campaign=Badge_Grade) ![GitHub issues](https://img.shields.io/github/issues/rochacbruno/dynaconf.svg) ![GitHub stars](https://img.shields.io/github/stars/rochacbruno/dynaconf.svg) ![GitHub Release Date](https://img.shields.io/github/release-date/rochacbruno/dynaconf.svg) ![GitHub commits since latest release](https://img.shields.io/github/commits-since/rochacbruno/dynaconf/latest.svg) ![GitHub last commit](https://img.shields.io/github/last-commit/rochacbruno/dynaconf.svg) [![Code Style Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black/) [![Discussion](https://img.shields.io/badge/chat-discussions-blue.svg?logo=googlechat)](https://github.com/rochacbruno/dynaconf/discussions) [![Discussion](https://img.shields.io/badge/demo-learn-yellow.svg?logo=gnubash)](https://github.com/rochacbruno/learndynaconf)
+[![MIT License](https://img.shields.io/badge/license-MIT-007EC7.svg?style=flat-square)](/LICENSE) [![PyPI](https://img.shields.io/pypi/v/dynaconf.svg)](https://pypi.python.org/pypi/dynaconf) [![PyPI](https://img.shields.io/pypi/pyversions/dynaconf.svg)]() ![PyPI - Downloads](https://img.shields.io/pypi/dm/dynaconf.svg?label=pip%20installs&logo=python) [![CI](https://github.com/dynaconf/dynaconf/actions/workflows/main.yml/badge.svg)](https://github.com/dynaconf/dynaconf/actions/workflows/main.yml) [![codecov](https://codecov.io/gh/dynaconf/dynaconf/branch/master/graph/badge.svg)](https://codecov.io/gh/dynaconf/dynaconf) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/3fb2de98464442f99a7663181803b400)](https://www.codacy.com/gh/dynaconf/dynaconf/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=dynaconf/dynaconf&amp;utm_campaign=Badge_Grade)  ![GitHub stars](https://img.shields.io/github/stars/dynaconf/dynaconf.svg) ![GitHub Release Date](https://img.shields.io/github/release-date/dynaconf/dynaconf.svg) ![GitHub commits since latest release](https://img.shields.io/github/commits-since/dynaconf/dynaconf/latest.svg) ![GitHub last commit](https://img.shields.io/github/last-commit/dynaconf/dynaconf.svg) [![Code Style Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black/)
 
-
-
-[![Foo](https://xscode.com/assets/promo-banner.svg)](https://xscode.com/rochacbruno/dynaconf)
+![GitHub issues](https://img.shields.io/github/issues/dynaconf/dynaconf.svg) [![User Forum](https://img.shields.io/badge/users-forum-blue.svg?logo=googlechat)](https://github.com/dynaconf/dynaconf/discussions) [![Join the chat at https://gitter.im/dynaconf/dev](https://badges.gitter.im/dynaconf/dev.svg)](https://gitter.im/dynaconf/dev?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![ Matrix](https://img.shields.io/badge/dev-room-blue.svg?logo=matrix)](https://matrix.to/#/#dynaconf:matrix.org)
 
 ## Features
 
 - Inspired by the [12-factor application guide](https://12factor.net/config)
 - Settings management (default values, validation, parsing, templating)
 - Protection of sensitive information (passwords/tokens)
 - Multiple file formats `toml|yaml|json|ini|py` and also customizable loaders.
 - Full support for environment variables to override existing settings (dotenv support included).
 - Optional layered system for multi environments `[default, development, testing, production]`
 - Built-in support for Hashicorp Vault and Redis as settings and secrets storage.
 - Built-in extensions for **Django** and **Flask** web frameworks.
 - CLI for common operations such as `init, list, write, validate, export`.
 - full docs on https://dynaconf.com
 
-## Quick start
-
-> **DEMO:** You can see a working demo here: https://github.com/rochacbruno/learndynaconf
-
-
 ### Install
 
 ```bash
 $ pip install dynaconf
 ```
 
 #### Initialize Dynaconf on project root directory
@@ -96,15 +98,15 @@
 
 #### Dynaconf init creates the following files
 
 ```plain
 .
 ├── config.py       # This is from where you import your settings object (required)
 ├── .secrets.toml   # This is to hold sensitive data like passwords and tokens (optional)
-└── settings.toml   # This is to hold your application setttings (optional)
+└── settings.toml   # This is to hold your application settings (optional)
 ```
 
 On the file `config.py` Dynaconf init generates the following boilerpate
 
 ```py
 from dynaconf import Dynaconf
 
@@ -167,15 +169,14 @@
 - Template substitutions
 - etc...
 
 There is a lot more you can do, **read the docs:** http://dynaconf.com
 
 ## Contribute
 
-Main discussions happens on [Discussions Tab](https://github.com/rochacbruno/dynaconf/discussions) learn more about how to get involved on [CONTRIBUTING.md guide](CONTRIBUTING.md)
+Main discussions happens on [Discussions Tab](https://github.com/dynaconf/dynaconf/discussions) learn more about how to get involved on [CONTRIBUTING.md guide](CONTRIBUTING.md)
 
 ## More
 
 If you are looking for something similar to Dynaconf to use in your Rust projects: https://github.com/rubik/hydroconf
 
 And a special thanks to [Caneco](https://twitter.com/caneco) for the logo.
-
```

### Comparing `dynaconf-3.1.9/README.md` & `dynaconf-3.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 <!-- [![Dynaconf](docs/img/logo_400.svg?sanitize=true)](http://dynaconf.com) -->
 
 <p align="center"><img src="/art/header.png?v2" alt="dynaconf. new logo"></p>
 
 > **dynaconf** - Configuration Management for Python.
 
-[![MIT License](https://img.shields.io/badge/license-MIT-007EC7.svg?style=flat-square)](/LICENSE) [![PyPI](https://img.shields.io/pypi/v/dynaconf.svg)](https://pypi.python.org/pypi/dynaconf) [![PyPI](https://img.shields.io/pypi/pyversions/dynaconf.svg)]() ![PyPI - Downloads](https://img.shields.io/pypi/dm/dynaconf.svg?label=pip%20installs&logo=python) [![CI](https://github.com/rochacbruno/dynaconf/actions/workflows/main.yml/badge.svg)](https://github.com/rochacbruno/dynaconf/actions/workflows/main.yml) [![codecov](https://codecov.io/gh/rochacbruno/dynaconf/branch/master/graph/badge.svg)](https://codecov.io/gh/rochacbruno/dynaconf) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/42d2f11ef0a446808b246c8c69603f6e)](https://www.codacy.com/gh/rochacbruno/dynaconf/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=rochacbruno/dynaconf&amp;utm_campaign=Badge_Grade) ![GitHub issues](https://img.shields.io/github/issues/rochacbruno/dynaconf.svg) ![GitHub stars](https://img.shields.io/github/stars/rochacbruno/dynaconf.svg) ![GitHub Release Date](https://img.shields.io/github/release-date/rochacbruno/dynaconf.svg) ![GitHub commits since latest release](https://img.shields.io/github/commits-since/rochacbruno/dynaconf/latest.svg) ![GitHub last commit](https://img.shields.io/github/last-commit/rochacbruno/dynaconf.svg) [![Code Style Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black/) [![Discussion](https://img.shields.io/badge/chat-discussions-blue.svg?logo=googlechat)](https://github.com/rochacbruno/dynaconf/discussions) [![Discussion](https://img.shields.io/badge/demo-learn-yellow.svg?logo=gnubash)](https://github.com/rochacbruno/learndynaconf)
+[![MIT License](https://img.shields.io/badge/license-MIT-007EC7.svg?style=flat-square)](/LICENSE) [![PyPI](https://img.shields.io/pypi/v/dynaconf.svg)](https://pypi.python.org/pypi/dynaconf) [![PyPI](https://img.shields.io/pypi/pyversions/dynaconf.svg)]() ![PyPI - Downloads](https://img.shields.io/pypi/dm/dynaconf.svg?label=pip%20installs&logo=python) [![CI](https://github.com/dynaconf/dynaconf/actions/workflows/main.yml/badge.svg)](https://github.com/dynaconf/dynaconf/actions/workflows/main.yml) [![codecov](https://codecov.io/gh/dynaconf/dynaconf/branch/master/graph/badge.svg)](https://codecov.io/gh/dynaconf/dynaconf) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/3fb2de98464442f99a7663181803b400)](https://www.codacy.com/gh/dynaconf/dynaconf/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=dynaconf/dynaconf&amp;utm_campaign=Badge_Grade)  ![GitHub stars](https://img.shields.io/github/stars/dynaconf/dynaconf.svg) ![GitHub Release Date](https://img.shields.io/github/release-date/dynaconf/dynaconf.svg) ![GitHub commits since latest release](https://img.shields.io/github/commits-since/dynaconf/dynaconf/latest.svg) ![GitHub last commit](https://img.shields.io/github/last-commit/dynaconf/dynaconf.svg) [![Code Style Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black/)
 
-
-
-[![Foo](https://xscode.com/assets/promo-banner.svg)](https://xscode.com/rochacbruno/dynaconf)
+![GitHub issues](https://img.shields.io/github/issues/dynaconf/dynaconf.svg) [![User Forum](https://img.shields.io/badge/users-forum-blue.svg?logo=googlechat)](https://github.com/dynaconf/dynaconf/discussions) [![Join the chat at https://gitter.im/dynaconf/dev](https://badges.gitter.im/dynaconf/dev.svg)](https://gitter.im/dynaconf/dev?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![ Matrix](https://img.shields.io/badge/dev-room-blue.svg?logo=matrix)](https://matrix.to/#/#dynaconf:matrix.org)
 
 ## Features
 
 - Inspired by the [12-factor application guide](https://12factor.net/config)
 - Settings management (default values, validation, parsing, templating)
 - Protection of sensitive information (passwords/tokens)
 - Multiple file formats `toml|yaml|json|ini|py` and also customizable loaders.
 - Full support for environment variables to override existing settings (dotenv support included).
 - Optional layered system for multi environments `[default, development, testing, production]`
 - Built-in support for Hashicorp Vault and Redis as settings and secrets storage.
 - Built-in extensions for **Django** and **Flask** web frameworks.
 - CLI for common operations such as `init, list, write, validate, export`.
 - full docs on https://dynaconf.com
 
-## Quick start
-
-> **DEMO:** You can see a working demo here: https://github.com/rochacbruno/learndynaconf
-
-
 ### Install
 
 ```bash
 $ pip install dynaconf
 ```
 
 #### Initialize Dynaconf on project root directory
@@ -59,15 +52,15 @@
 
 #### Dynaconf init creates the following files
 
 ```plain
 .
 ├── config.py       # This is from where you import your settings object (required)
 ├── .secrets.toml   # This is to hold sensitive data like passwords and tokens (optional)
-└── settings.toml   # This is to hold your application setttings (optional)
+└── settings.toml   # This is to hold your application settings (optional)
 ```
 
 On the file `config.py` Dynaconf init generates the following boilerpate
 
 ```py
 from dynaconf import Dynaconf
 
@@ -130,14 +123,14 @@
 - Template substitutions
 - etc...
 
 There is a lot more you can do, **read the docs:** http://dynaconf.com
 
 ## Contribute
 
-Main discussions happens on [Discussions Tab](https://github.com/rochacbruno/dynaconf/discussions) learn more about how to get involved on [CONTRIBUTING.md guide](CONTRIBUTING.md)
+Main discussions happens on [Discussions Tab](https://github.com/dynaconf/dynaconf/discussions) learn more about how to get involved on [CONTRIBUTING.md guide](CONTRIBUTING.md)
 
 ## More
 
 If you are looking for something similar to Dynaconf to use in your Rust projects: https://github.com/rubik/hydroconf
 
 And a special thanks to [Caneco](https://twitter.com/caneco) for the logo.
```

### Comparing `dynaconf-3.1.9/dynaconf/__init__.py` & `dynaconf-3.2.0/dynaconf/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,36 @@
+from __future__ import annotations
+
 from dynaconf.base import LazySettings  # noqa
 from dynaconf.constants import DEFAULT_SETTINGS_FILES
 from dynaconf.contrib import DjangoDynaconf  # noqa
 from dynaconf.contrib import FlaskDynaconf  # noqa
+from dynaconf.utils.inspect import inspect_settings
+from dynaconf.utils.parse_conf import add_converter  # noqa
 from dynaconf.validator import ValidationError  # noqa
 from dynaconf.validator import Validator  # noqa
 
 settings = LazySettings(
     # This global `settings` is deprecated from v3.0.0+
     # kept here for backwards compatibility
     # To Be Removed in 4.0.x
     warn_dynaconf_global_settings=True,
     environments=True,
     lowercase_read=False,
     load_dotenv=True,
     default_settings_paths=DEFAULT_SETTINGS_FILES,
 )
 
+
 # This is the new recommended base class alias
 Dynaconf = LazySettings  # noqa
 
 __all__ = [
     "Dynaconf",
     "LazySettings",
     "Validator",
     "FlaskDynaconf",
     "ValidationError",
     "DjangoDynaconf",
+    "add_converter",
+    "inspect_settings",
 ]
```

### Comparing `dynaconf-3.1.9/dynaconf/base.py` & `dynaconf-3.2.0/dynaconf/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,50 @@
+from __future__ import annotations
+
 import copy
 import glob
 import importlib
 import inspect
 import os
 import warnings
 from collections import defaultdict
 from contextlib import contextmanager
 from contextlib import suppress
 from pathlib import Path
+from typing import Any
+from typing import Callable
 
 from dynaconf import default_settings
 from dynaconf.loaders import default_loader
 from dynaconf.loaders import enable_external_loaders
 from dynaconf.loaders import env_loader
-from dynaconf.loaders import execute_hooks
+from dynaconf.loaders import execute_instance_hooks
+from dynaconf.loaders import execute_module_hooks
 from dynaconf.loaders import py_loader
 from dynaconf.loaders import settings_loader
 from dynaconf.loaders import yaml_loader
+from dynaconf.loaders.base import SourceMetadata
 from dynaconf.utils import BANNER
 from dynaconf.utils import compat_kwargs
 from dynaconf.utils import ensure_a_list
 from dynaconf.utils import missing
 from dynaconf.utils import object_merge
 from dynaconf.utils import recursively_evaluate_lazy_format
 from dynaconf.utils import RENAMED_VARS
 from dynaconf.utils import upperfy
 from dynaconf.utils.boxing import DynaBox
 from dynaconf.utils.files import find_file
 from dynaconf.utils.functional import empty
 from dynaconf.utils.functional import LazyObject
+from dynaconf.utils.parse_conf import apply_converter
 from dynaconf.utils.parse_conf import converters
-from dynaconf.utils.parse_conf import get_converter
+from dynaconf.utils.parse_conf import Lazy
 from dynaconf.utils.parse_conf import parse_conf_data
 from dynaconf.utils.parse_conf import true_values
+from dynaconf.validator import ValidationError
 from dynaconf.validator import ValidatorList
 from dynaconf.vendor.box.box_list import BoxList
 
 
 class LazySettings(LazyObject):
     """Loads settings lazily from multiple sources::
 
@@ -62,15 +70,15 @@
         self._warn_dynaconf_global_settings = kwargs.pop(
             "warn_dynaconf_global_settings", None
         )  # in 3.0.0 global settings is deprecated
 
         self.__resolve_config_aliases(kwargs)
         compat_kwargs(kwargs)
         self._kwargs = kwargs
-        super(LazySettings, self).__init__()
+        super().__init__()
 
         if wrapped:
             if self._django_override:
                 # This fixes django issue #596
                 self._wrapped = copy.deepcopy(wrapped)
             else:
                 self._wrapped = wrapped
@@ -83,17 +91,17 @@
 
         mispells = {
             "settings_files": "settings_file",
             "SETTINGS_FILES": "SETTINGS_FILE",
             "environment": "environments",
             "ENVIRONMENT": "ENVIRONMENTS",
         }
-        for mispell, correct in mispells.items():
-            if mispell in kwargs:
-                kwargs[correct] = kwargs.pop(mispell)
+        for misspell, correct in mispells.items():
+            if misspell in kwargs:
+                kwargs[correct] = kwargs.pop(misspell)
 
         for_dynaconf_keys = {
             key
             for key in UPPER_DEFAULT_SETTINGS
             if key.endswith("_FOR_DYNACONF")
         }
         aliases = {
@@ -174,15 +182,15 @@
         )
 
     def configure(self, settings_module=None, **kwargs):
         """
         Allows user to reconfigure settings object passing a new settings
         module or separated kwargs
 
-        :param settings_module: defines the setttings file
+        :param settings_module: defines the settings file
         :param kwargs:  override default settings
         """
         default_settings.reload(self._should_load_dotenv)
         environment_var = self._kwargs.get(
             "ENVVAR_FOR_DYNACONF", default_settings.ENVVAR_FOR_DYNACONF
         )
         settings_module = settings_module or os.environ.get(environment_var)
@@ -203,26 +211,26 @@
 
     dynaconf_banner = BANNER
     _store = DynaBox()
 
     def __init__(self, settings_module=None, **kwargs):  # pragma: no cover
         """Execute loaders and custom initialization
 
-        :param settings_module: defines the setttings file
+        :param settings_module: defines the settings file
         :param kwargs:  override default settings
         """
         self._fresh = False
         self._loaded_envs = []
         self._loaded_hooks = defaultdict(dict)
         self._loaded_py_modules = []
         self._loaded_files = []
         self._deleted = set()
         self._store = DynaBox(box_settings=self)
         self._env_cache = {}
-        self._loaded_by_loaders = {}
+        self._loaded_by_loaders: dict[SourceMetadata, Any] = {}
         self._loaders = []
         self._defaults = DynaBox(box_settings=self)
         self.environ = os.environ
         self.SETTINGS_MODULE = None
         self.filter_strategy = kwargs.get("filter_strategy", None)
         self._not_installed_warnings = []
         self._validate_only = kwargs.pop("validate_only", None)
@@ -230,14 +238,17 @@
         self._validate_only_current_env = kwargs.pop(
             "validate_only_current_env", False
         )
 
         self.validators = ValidatorList(
             self, validators=kwargs.pop("validators", None)
         )
+        self._post_hooks: list[Callable] = ensure_a_list(
+            kwargs.get("post_hooks", [])
+        )
 
         compat_kwargs(kwargs)
         if settings_module:
             self.set("SETTINGS_FILE_FOR_DYNACONF", settings_module)
         for key, value in kwargs.items():
             self.set(key, value)
         # execute loaders only after setting defaults got from kwargs
@@ -263,23 +274,23 @@
         """
         return self.get(*args, **kwargs)
 
     def __setattr__(self, name, value):
         """Allow `settings.FOO = 'value'` while keeping internal attrs."""
 
         if name in RESERVED_ATTRS:
-            super(Settings, self).__setattr__(name, value)
+            super().__setattr__(name, value)
         else:
             self.set(name, value)
 
     def __delattr__(self, name):
         """stores reference in `_deleted` for proper error management"""
         self._deleted.add(name)
         if hasattr(self, name):
-            super(Settings, self).__delattr__(name)
+            super().__delattr__(name)
 
     def __contains__(self, item):
         """Respond to `item in settings`"""
         return item.upper() in self.store or item.lower() in self.store
 
     def __getattribute__(self, name):
         if name not in RESERVED_ATTRS and name not in UPPER_DEFAULT_SETTINGS:
@@ -287,15 +298,15 @@
                 # self._store has Lazy values already evaluated
                 if (
                     name.islower()
                     and self._store.get("LOWERCASE_READ_FOR_DYNACONF", empty)
                     is False
                 ):
                     # only matches exact casing, first levels always upper
-                    return self._store.to_dict()[name]
+                    return self._store.__getattribute__(name)
                 # perform lookups for upper, and casefold
                 return self._store[name]
         # in case of RESERVED_ATTRS or KeyError above, keep default behaviour
         return super().__getattribute__(name)
 
     def __getitem__(self, item):
         """Allow getting variables as dict keys `settings['KEY']`"""
@@ -333,41 +344,47 @@
         """Redirects to store object"""
         return self.store.keys()
 
     def values(self):
         """Redirects to store object"""
         return self.store.values()
 
-    def setdefault(self, item, default, apply_default_on_none=False):
+    def setdefault(
+        self, item, default, apply_default_on_none=False, env: str = "unknown"
+    ):
         """Returns value if exists or set it as the given default
 
         apply_default_on_none: if True, default is set when value is None
+        env: used to create the source identifier
         """
         value = self.get(item, empty)
 
-        # Yaml loader reads empty values as None, whould we apply defaults?
+        # Yaml loader reads empty values as None, would we apply defaults?
         global_apply_default = (
             self.get("APPLY_DEFAULT_ON_NONE_FOR_DYNACONF") is not None
         )
         apply_default = default is not empty and (
             value is empty
             or (
                 value is None
                 and (
                     apply_default_on_none is True
                     or global_apply_default is True
                 )
             )
         )
+        loader_identifier = SourceMetadata(
+            "validation_default", "unique", env.lower()
+        )
 
         if apply_default:
             self.set(
                 item,
                 default,
-                loader_identifier="setdefault",
+                loader_identifier=loader_identifier,
                 tomlfy=True,
             )
             return default
 
         return value
 
     def as_dict(self, env=None, internal=False):
@@ -399,15 +416,15 @@
         split_key = dotted_key.split(".")
         name, keys = split_key[0], split_key[1:]
         result = self.get(name, default=default, parent=parent, **kwargs)
 
         # If we've reached the end, or parent key not found, then return result
         if not keys or result == default:
             if cast and cast in converters:
-                return get_converter(cast, result, box_settings=self)
+                return apply_converter(cast, result, box_settings=self)
             elif cast is True:
                 return parse_conf_data(result, tomlfy=True, box_settings=self)
             return result
 
         # If we've still got key elements to traverse, let's do that.
         return self._dotted_get(
             ".".join(keys), default=default, parent=result, cast=cast, **kwargs
@@ -417,29 +434,34 @@
         self,
         key,
         default=None,
         cast=None,
         fresh=False,
         dotted_lookup=empty,
         parent=None,
+        sysenv_fallback=None,
     ):
         """
-        Get a value from settings store, this is the prefered way to access::
+        Get a value from settings store, this is the preferred way to access::
 
             >>> from dynaconf import settings
             >>> settings.get('KEY')
 
         :param key: The name of the setting value, will always be upper case
         :param default: In case of not found it will be returned
         :param cast: Should cast in to @int, @float, @bool or @json ?
         :param fresh: Should reload from loaders store before access?
         :param dotted_lookup: Should perform dotted-path lookup?
         :param parent: Is there a pre-loaded parent in a nested data?
+        :param sysenv_fallback: Should fallback to system environ if not found?
         :return: The value if found, default or None
         """
+        if sysenv_fallback is None:
+            sysenv_fallback = self._store.get("SYSENV_FALLBACK_FOR_DYNACONF")
+
         nested_sep = self._store.get("NESTED_SEPARATOR_FOR_DYNACONF")
         if nested_sep and nested_sep in key:
             # turn FOO__bar__ZAZ in `FOO.bar.ZAZ`
             key = key.replace(nested_sep, ".")
 
         if dotted_lookup is empty:
             dotted_lookup = self._store.get("DOTTED_LOOKUP_FOR_DYNACONF")
@@ -449,43 +471,52 @@
                 dotted_key=key,
                 default=default,
                 cast=cast,
                 fresh=fresh,
                 parent=parent,
             )
 
+        key = upperfy(key)
+
+        # handles system environment fallback
+        if default is None:
+            key_in_sysenv_fallback_list = isinstance(
+                sysenv_fallback, list
+            ) and key in [upperfy(k) for k in sysenv_fallback]
+            if sysenv_fallback is True or key_in_sysenv_fallback_list:
+                default = self.environ.get(key)
+
+        # default values should behave exactly Dynaconf parsed values
         if default is not None:
-            # default values should behave exactly Dynaconf parsed values
             if isinstance(default, list):
                 default = BoxList(default)
             elif isinstance(default, dict):
                 default = DynaBox(default)
 
-        key = upperfy(key)
         if key in self._deleted:
             return default
 
         if (
             fresh
             or self._fresh
             or key in getattr(self, "FRESH_VARS_FOR_DYNACONF", ())
         ) and key not in UPPER_DEFAULT_SETTINGS:
             self.unset(key)
             self.execute_loaders(key=key)
 
         data = (parent or self.store).get(key, default)
         if cast:
-            data = get_converter(cast, data, box_settings=self)
+            data = apply_converter(cast, data, box_settings=self)
         return data
 
     def exists(self, key, fresh=False):
         """Check if key exists
 
         :param key: the name of setting variable
-        :param fresh: if key should be taken from source direclty
+        :param fresh: if key should be taken from source directly
         :return: Boolean
         """
         key = upperfy(key)
         if key in self._deleted:
             return False
         return self.get(key, fresh=fresh, default=missing) is not missing
 
@@ -509,15 +540,15 @@
          or cast must be true to use cast inference
         :return: The value if found, default or None
         """
         key = upperfy(key)
         data = self.environ.get(key, default)
         if data:
             if cast in converters:
-                data = get_converter(cast, data, box_settings=self)
+                data = apply_converter(cast, data, box_settings=self)
             elif cast is True:
                 data = parse_conf_data(data, tomlfy=True, box_settings=self)
         return data
 
     def exists_in_environ(self, key):
         """Return True if env variable is exported"""
         return upperfy(key) in self.environ
@@ -552,14 +583,15 @@
 
     # compat
     loaded_namespaces = loaded_envs
 
     @property
     def loaded_by_loaders(self):
         """Gets the internal mapping of LOADER -> values"""
+        # return {k.loader:data for k, data in self._loaded_by_loaders}
         return self._loaded_by_loaders
 
     def from_env(self, env="", keep=False, **kwargs):
         """Return a new isolated settings object pointing to specified env.
 
         Example of settings.toml::
 
@@ -616,14 +648,18 @@
                 }
             )
 
         new_data.update(kwargs)
         new_data["FORCE_ENV_FOR_DYNACONF"] = env
         new_settings = LazySettings(**new_data)
         self._env_cache[cache_key] = new_settings
+
+        # update source metadata for inspecting
+        self._loaded_by_loaders.update(new_settings._loaded_by_loaders)
+
         return new_settings
 
     @contextmanager
     def using_env(self, env, clean=True, silent=True, filename=None):
         """
         This context manager allows the contextual use of a different env
         Example of settings.toml::
@@ -688,14 +724,15 @@
     def current_env(self):
         """Return the current active env"""
 
         if self.ENVIRONMENTS_FOR_DYNACONF is False:
             return self.MAIN_ENV_FOR_DYNACONF.lower()
 
         if self.FORCE_ENV_FOR_DYNACONF is not None:
+            self.ENV_FOR_DYNACONF = self.FORCE_ENV_FOR_DYNACONF
             return self.FORCE_ENV_FOR_DYNACONF
 
         try:
             return self.loaded_envs[-1]
         except IndexError:
             return self.ENV_FOR_DYNACONF
 
@@ -746,16 +783,16 @@
         :param clean: If preloaded vars should be cleaned
         :param silent: Silence errors
         :param filename: Custom filename to load (optional)
         :return: context
         """
         env = env or self.ENV_FOR_DYNACONF
 
-        if not isinstance(env, str):
-            raise AttributeError("env should be a string")
+        if not isinstance(env, str) or "_" in env or " " in env:
+            raise ValueError("env should be a string without _ or spaces")
 
         env = env.upper()
 
         if env != self.ENV_FOR_DYNACONF:
             self.loaded_envs.append(env)
         else:
             self.loaded_envs = []
@@ -795,137 +832,200 @@
 
         :param keys: a list of keys
         :param force: Bypass default checks and force unset
         """
         for key in keys:
             self.unset(key, force=force)
 
-    def _dotted_set(self, dotted_key, value, tomlfy=False, **kwargs):
+    def _dotted_set(
+        self, dotted_key, value, tomlfy=False, validate=empty, **kwargs
+    ):
         """Sets dotted keys as nested dictionaries.
 
         Dotted set will always reassign the value, to merge use `@merge` token
 
         Arguments:
             dotted_key {str} -- A traversal name e.g: foo.bar.zaz
             value {Any} -- The value to set to the nested value.
 
         Keyword Arguments:
             tomlfy {bool} -- Perform toml parsing (default: {False})
+            validate {bool} --
         """
+        if validate is empty:
+            validate = self.get(
+                "VALIDATE_ON_UPDATE_FOR_DYNACONF"
+            )  # pragma: nocover
 
         split_keys = dotted_key.split(".")
         existing_data = self.get(split_keys[0], {})
         new_data = tree = DynaBox(box_settings=self)
 
         for k in split_keys[:-1]:
             tree = tree.setdefault(k, {})
 
         value = parse_conf_data(value, tomlfy=tomlfy, box_settings=self)
         tree[split_keys[-1]] = value
 
         if existing_data:
+            old_data = DynaBox(
+                {split_keys[0]: existing_data}, box_settings=self
+            )
             new_data = object_merge(
-                old=DynaBox({split_keys[0]: existing_data}),
+                old=old_data,
                 new=new_data,
                 full_path=split_keys,
             )
-        self.update(data=new_data, tomlfy=tomlfy, **kwargs)
+        self.update(data=new_data, tomlfy=tomlfy, validate=validate, **kwargs)
 
     def set(
         self,
         key,
         value,
-        loader_identifier=None,
+        loader_identifier: SourceMetadata | None = None,
         tomlfy=False,
         dotted_lookup=empty,
         is_secret="DeprecatedArgument",  # noqa
-        merge=False,
+        validate=empty,
+        merge=empty,
     ):
         """Set a value storing references for the loader
 
         :param key: The key to store
         :param value: The value to store
         :param loader_identifier: Optional loader name e.g: toml, yaml etc.
         :param tomlfy: Bool define if value is parsed by toml (defaults False)
         :param merge: Bool define if existing nested data will be merged.
+        :param validate: Bool define if validation will be triggered
         """
+        if validate is empty:
+            validate = self.get("VALIDATE_ON_UPDATE_FOR_DYNACONF")
+
         if dotted_lookup is empty:
             dotted_lookup = self.get("DOTTED_LOOKUP_FOR_DYNACONF")
 
         nested_sep = self.get("NESTED_SEPARATOR_FOR_DYNACONF")
         if nested_sep and nested_sep in key:
             # turn FOO__bar__ZAZ in `FOO.bar.ZAZ`
             key = key.replace(nested_sep, ".")
 
         if "." in key and dotted_lookup is True:
             return self._dotted_set(
-                key, value, loader_identifier=loader_identifier, tomlfy=tomlfy
+                key,
+                value,
+                loader_identifier=loader_identifier,
+                tomlfy=tomlfy,
+                validate=validate,
             )
 
+        # Fix for #905
+        # parsed_conf default value was causing duplication
+        value_not_parsed = (
+            value
+            if loader_identifier
+            and loader_identifier.loader == "validation_default"
+            else None
+        )
+
         value = parse_conf_data(value, tomlfy=tomlfy, box_settings=self)
         key = upperfy(key.strip())
-        existing = getattr(self, key, None)
+
+        # Fix for #869 - The call to getattr trigger early evaluation
+        existing = (
+            getattr(self, key, None) if not isinstance(value, Lazy) else None
+        )
 
         if getattr(value, "_dynaconf_del", None):
             # just in case someone use a `@del` in a first level var.
             self.unset(key, force=True)
             return
 
         if getattr(value, "_dynaconf_reset", False):  # pragma: no cover
             # just in case someone use a `@reset` in a first level var.
             value = value.unwrap()
 
         if getattr(value, "_dynaconf_merge_unique", False):
             # just in case someone use a `@merge_unique` in a first level var
             if existing:
+                # update SourceMetadata (for inspecting purposes)
+                loader_identifier = (
+                    loader_identifier._replace(merged=True)
+                    if loader_identifier
+                    else None
+                )
                 value = object_merge(existing, value.unwrap(), unique=True)
             else:
                 value = value.unwrap()
 
         if getattr(value, "_dynaconf_merge", False):
             # just in case someone use a `@merge` in a first level var
             if existing:
+                # update SourceMetadata (for inspecting purposes)
+                loader_identifier = (
+                    loader_identifier._replace(merged=True)
+                    if loader_identifier
+                    else None
+                )
                 value = object_merge(existing, value.unwrap())
             else:
                 value = value.unwrap()
 
         if existing is not None and existing != value:
             # `dynaconf_merge` used in file root `merge=True`
-            if merge:
+            if merge and merge is not empty:
+                loader_identifier = (
+                    loader_identifier._replace(merged=True)
+                    if loader_identifier
+                    else None
+                )
                 value = object_merge(existing, value)
             else:
-                # `dynaconf_merge` may be used within the key structure
-                # Or merge_enabled is set to True
-                value = self._merge_before_set(existing, value)
+                # Fix for #905
+                if (
+                    loader_identifier
+                    and loader_identifier.loader == "validation_default"
+                ):
+                    value = value_not_parsed
+                else:
+                    # `dynaconf_merge` may be used within the key structure
+                    # Or merge_enabled is set to True
+                    value, updated_identifier = self._merge_before_set(
+                        existing, value, loader_identifier, context_merge=merge
+                    )
+                    loader_identifier = updated_identifier
 
-        if isinstance(value, dict):
+        if isinstance(value, dict) and not isinstance(value, DynaBox):
             value = DynaBox(value, box_settings=self)
 
         self.store[key] = value
         self._deleted.discard(key)
-        super(Settings, self).__setattr__(key, value)
+        super().__setattr__(key, value)
 
         # set loader identifiers so cleaners know which keys to clean
-        if loader_identifier and loader_identifier in self.loaded_by_loaders:
-            self.loaded_by_loaders[loader_identifier][key] = value
+        if loader_identifier and loader_identifier in self._loaded_by_loaders:
+            self._loaded_by_loaders[loader_identifier][key] = value
         elif loader_identifier:
-            self.loaded_by_loaders[loader_identifier] = {key: value}
+            self._loaded_by_loaders[loader_identifier] = {key: value}
         elif loader_identifier is None:
             # if .set is called without loader identifier it becomes
             # a default value and goes away only when explicitly unset
             self._defaults[key] = value
 
+        if validate is True:
+            self.validators.validate()
+
     def update(
         self,
         data=None,
         loader_identifier=None,
         tomlfy=False,
-        merge=False,
+        merge=empty,
         is_secret="DeprecatedArgument",  # noqa
         dotted_lookup=empty,
+        validate=empty,
         **kwargs,
     ):
         """
         Update values in the current settings object without saving in stores::
 
             >>> from dynaconf import settings
             >>> print settings.NAME
@@ -936,58 +1036,90 @@
             >>> print settings.OTHER_VALUE
             1
 
         :param data: Data to be updated
         :param loader_identifier: Only to be used by custom loaders
         :param tomlfy: Bool define if value is parsed by toml (defaults False)
         :param merge: Bool define if existing nested data will be merged.
+        :param validate: Bool define if validators will trigger automatically
         :param kwargs: extra values to update
         :return: None
         """
+
+        if validate is empty:
+            validate = self.get("VALIDATE_ON_UPDATE_FOR_DYNACONF")
+
         data = data or {}
         data.update(kwargs)
         for key, value in data.items():
-            self.set(
-                key,
-                value,
-                loader_identifier=loader_identifier,
-                tomlfy=tomlfy,
-                merge=merge,
-                dotted_lookup=dotted_lookup,
-            )
+            # update() will handle validation later
+            with suppress(ValidationError):
+                self.set(
+                    key,
+                    value,
+                    loader_identifier=loader_identifier,
+                    tomlfy=tomlfy,
+                    merge=merge,
+                    dotted_lookup=dotted_lookup,
+                    validate=validate,
+                )
+
+        # handle param `validate`
+        if validate is True:
+            self.validators.validate()
+        elif validate == "all":
+            self.validators.validate_all()
+
+    def _merge_before_set(
+        self,
+        existing,
+        value,
+        identifier: SourceMetadata | None = None,
+        context_merge=empty,
+    ):
+        """
+        Merge the new value being set with the existing value before set
+        Returns the merged value and the updated identifier (for inspecting).
+        """
+        # context_merge may come from file_scope or env_scope
+        if context_merge is empty:
+            context_merge = self.get("MERGE_ENABLED_FOR_DYNACONF")
 
-    def _merge_before_set(self, existing, value):
-        """Merge the new value being set with the existing value before set"""
-        global_merge = getattr(self, "MERGE_ENABLED_FOR_DYNACONF", False)
         if isinstance(value, dict):
             local_merge = value.pop(
                 "dynaconf_merge", value.pop("dynaconf_merge_unique", None)
             )
             if local_merge not in (True, False, None) and not value:
                 # In case `dynaconf_merge:` holds value not boolean - ref #241
                 value = local_merge
 
-            if global_merge or local_merge:
+            if local_merge or (context_merge and local_merge is not False):
+                identifier = (
+                    identifier._replace(merged=True) if identifier else None
+                )
                 value = object_merge(existing, value)
 
         if isinstance(value, (list, tuple)):
-            local_merge = (
-                "dynaconf_merge" in value or "dynaconf_merge_unique" in value
-            )
-            if global_merge or local_merge:
-                value = list(value)
-                unique = False
-                if local_merge:
-                    try:
-                        value.remove("dynaconf_merge")
-                    except ValueError:  # EAFP
-                        value.remove("dynaconf_merge_unique")
-                        unique = True
+            value = list(value)
+            local_merge = None
+            unique = False
+            if "dynaconf_merge" in value:
+                value.remove("dynaconf_merge")
+                local_merge = True
+            elif "dynaconf_merge_unique" in value:
+                value.remove("dynaconf_merge_unique")
+                local_merge = True
+                unique = True
+
+            if local_merge or (context_merge and local_merge is not False):
+                identifier = (
+                    identifier._replace(merged=True) if identifier else None
+                )
                 value = object_merge(existing, value, unique=unique)
-        return value
+        return value, identifier
 
     @property
     def loaders(self):  # pragma: no cover
         """Return available loaders"""
         if self.LOADERS_FOR_DYNACONF in (None, 0, "0", "false", False):
             return []
 
@@ -995,23 +1127,24 @@
             self._loaders = self.LOADERS_FOR_DYNACONF
 
         return [importlib.import_module(loader) for loader in self._loaders]
 
     def reload(self, env=None, silent=None):  # pragma: no cover
         """Clean end Execute all loaders"""
         self.clean()
+        self._loaded_hooks.clear()
         self.execute_loaders(env, silent)
 
     def execute_loaders(
         self, env=None, silent=None, key=None, filename=None, loaders=None
     ):
         """Execute all internal and registered loaders
 
         :param env: The environment to load
-        :param silent: If loading erros is silenced
+        :param silent: If loading errors is silenced
         :param key: if provided load a single key
         :param filename: optional custom filename to load
         :param loaders: optional list of loader modules
         """
         if key is None:
             default_loader(self, self._defaults)
 
@@ -1023,92 +1156,120 @@
             settings_loader(
                 self, env=env, silent=silent, key=key, filename=filename
             )
             self.load_extra_yaml(env, silent, key)  # DEPRECATED
             enable_external_loaders(self)
 
             loaders = self.loaders
-
+        # non setting_file or py_module loaders
         for core_loader in loaders:
             core_loader.load(self, env, silent=silent, key=key)
 
         self.load_includes(env, silent=silent, key=key)
-        execute_hooks("post", self, env, silent=silent, key=key)
+        self._store._box_config["_bypass_evaluation"] = True
+
+        # execute hooks
+        execute_module_hooks("post", self, env, silent=silent, key=key)
+        execute_instance_hooks(self, "post", self._post_hooks)
+
+        self._store._box_config["_bypass_evaluation"] = False
 
     def pre_load(self, env, silent, key):
         """Do we have any file to pre-load before main settings file?"""
         preloads = self.get("PRELOAD_FOR_DYNACONF", [])
         if preloads:
             self.load_file(path=preloads, env=env, silent=silent, key=key)
 
     def load_includes(self, env, silent, key):
         """Do we have any nested includes we need to process?"""
-        includes = self.get("DYNACONF_INCLUDE", [])
+        includes = ensure_a_list(self.get("DYNACONF_INCLUDE"))
         includes.extend(ensure_a_list(self.get("INCLUDES_FOR_DYNACONF")))
         if includes:
             self.load_file(path=includes, env=env, silent=silent, key=key)
             # ensure env vars are the last thing loaded after all includes
             last_loader = self.loaders and self.loaders[-1]
             if last_loader and last_loader == env_loader:
                 last_loader.load(self, env, silent, key)
 
-    def load_file(self, path=None, env=None, silent=True, key=None):
+    def load_file(
+        self, path=None, env=None, silent=True, key=None, validate=empty
+    ):
         """Programmatically load files from ``path``.
 
+        When using relative paths, the basedir fallbacks in this order:
+        - ROOT_PATH_FOR_DYNACONF
+        - Directory of the last loaded file
+        - CWD
+
         :param path: A single filename or a file list
         :param env: Which env to load from file (default current_env)
         :param silent: Should raise errors?
         :param key: Load a single key?
+        :param validate: Should trigger validation?
         """
+        if validate is empty:
+            validate = self.get("VALIDATE_ON_UPDATE_FOR_DYNACONF")
+
         env = (env or self.current_env).upper()
         files = ensure_a_list(path)
         if files:
             already_loaded = set()
             for _filename in files:
 
-                if py_loader.try_to_load_from_py_module_name(
-                    obj=self, name=_filename, silent=True
-                ):
-                    # if it was possible to load from module name
-                    # continue the loop.
-                    continue
+                # load_file() will handle validation later
+                with suppress(ValidationError):
+                    if py_loader.try_to_load_from_py_module_name(
+                        obj=self, name=_filename, silent=True
+                    ):
+                        # if it was possible to load from module name
+                        # continue the loop.
+                        continue
 
-                # python 3.6 does not resolve Pathlib basedirs
-                # issue #494
                 root_dir = str(self._root_path or os.getcwd())
+
+                # Issue #494
                 if (
                     isinstance(_filename, Path)
                     and str(_filename.parent) in root_dir
                 ):  # pragma: no cover
                     filepath = str(_filename)
                 else:
-                    filepath = os.path.join(
-                        self._root_path or os.getcwd(), str(_filename)
-                    )
+                    filepath = os.path.join(root_dir, str(_filename))
 
                 paths = [
                     p
                     for p in sorted(glob.glob(filepath))
                     if ".local." not in p
                 ]
                 local_paths = [
                     p for p in sorted(glob.glob(filepath)) if ".local." in p
                 ]
+
                 # Handle possible *.globs sorted alphanumeric
                 for path in paths + local_paths:
                     if path in already_loaded:  # pragma: no cover
                         continue
-                    settings_loader(
-                        obj=self,
-                        env=env,
-                        silent=silent,
-                        key=key,
-                        filename=path,
-                    )
-                    already_loaded.add(path)
+
+                    # load_file() will handle validation later
+                    with suppress(ValidationError):
+                        settings_loader(
+                            obj=self,
+                            env=env,
+                            silent=silent,
+                            key=key,
+                            filename=path,
+                            validate=validate,
+                        )
+                        already_loaded.add(path)
+
+        # handle param `validate`
+        if validate is True:
+            self.validators.validate()
+        elif validate == "all":
+            self.validators.validate_all()
 
     @property
     def _root_path(self):
         """ROOT_PATH_FOR_DYNACONF or the path of first loaded file or '.'"""
 
         if self.ROOT_PATH_FOR_DYNACONF is not None:
             return self.ROOT_PATH_FOR_DYNACONF
@@ -1195,15 +1356,15 @@
                 setattr(obj, key, value)
 
     def dynaconf_clone(self):
         """Clone the current settings object."""
         try:
             return copy.deepcopy(self)
         except TypeError:
-            # can't deepcopy settings object bacause of module object
+            # can't deepcopy settings object because of module object
             # being set as value in the settings dict
             new_data = self.to_dict(internal=True)
             new_data["dynaconf_skip_loaders"] = True
             new_data["dynaconf_skip_validators"] = True
             return Settings(**new_data)
 
     @property
@@ -1211,15 +1372,15 @@
         """A proxy to access internal methods and attributes
 
         Starting in 3.0.0 Dynaconf now allows first level lower case
         keys that are not reserved keyword, so this is a proxy to
         internal methods and attrs.
         """
 
-        class AttrProxy(object):
+        class AttrProxy:
             def __init__(self, obj):
                 self.obj = obj
 
             def __getattr__(self, name):
                 return getattr(self.obj, f"dynaconf_{name}")
 
         return AttrProxy(self)
@@ -1275,9 +1436,10 @@
         "environ",
         "SETTINGS_MODULE",
         "filter_strategy",
         "validators",
         "_validate_only",
         "_validate_exclude",
         "_validate_only_current_env",
+        "_post_hooks",
     ]
 )
```

### Comparing `dynaconf-3.1.9/dynaconf/cli.py` & `dynaconf-3.2.0/dynaconf/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from __future__ import annotations
+
 import importlib
-import io
+import json
 import os
 import pprint
 import sys
 import warnings
 import webbrowser
 from contextlib import suppress
 from pathlib import Path
+from typing import TYPE_CHECKING
 
 from dynaconf import constants
 from dynaconf import default_settings
 from dynaconf import LazySettings
 from dynaconf import loaders
 from dynaconf import settings as legacy_settings
 from dynaconf.loaders.py_loader import get_module
@@ -19,60 +22,77 @@
 from dynaconf.utils.functional import empty
 from dynaconf.utils.parse_conf import parse_conf_data
 from dynaconf.utils.parse_conf import unparse_conf_data
 from dynaconf.validator import ValidationError
 from dynaconf.validator import Validator
 from dynaconf.vendor import click
 from dynaconf.vendor import toml
+from dynaconf.vendor import tomllib
+
+
+if TYPE_CHECKING:  # pragma: no cover
+    from dynaconf.base import Settings
 
 os.environ["PYTHONIOENCODING"] = "utf-8"
 
-CWD = Path.cwd()
+CWD = None
+with suppress(FileNotFoundError):
+    CWD = Path.cwd()
+
 EXTS = ["ini", "toml", "yaml", "json", "py", "env"]
 WRITERS = ["ini", "toml", "yaml", "json", "py", "redis", "vault", "env"]
 
 ENC = default_settings.ENCODING_FOR_DYNACONF
 
 
 def set_settings(ctx, instance=None):
     """Pick correct settings instance and set it to a global variable."""
-
     global settings
 
     settings = None
 
+    _echo_enabled = ctx.invoked_subcommand not in ["get", None]
+
     if instance is not None:
         if ctx.invoked_subcommand in ["init"]:
             raise click.UsageError(
                 "-i/--instance option is not allowed for `init` command"
             )
         sys.path.insert(0, ".")
         settings = import_settings(instance)
     elif "FLASK_APP" in os.environ:  # pragma: no cover
         with suppress(ImportError, click.UsageError):
             from flask.cli import ScriptInfo  # noqa
+            from dynaconf import FlaskDynaconf
 
             flask_app = ScriptInfo().load_app()
-            settings = flask_app.config
-            click.echo(
-                click.style(
-                    "Flask app detected", fg="white", bg="bright_black"
+            settings = FlaskDynaconf(flask_app, **flask_app.config).settings
+            if _echo_enabled:
+                click.echo(
+                    click.style(
+                        "Flask app detected", fg="white", bg="bright_black"
+                    )
                 )
-            )
     elif "DJANGO_SETTINGS_MODULE" in os.environ:  # pragma: no cover
         sys.path.insert(0, os.path.abspath(os.getcwd()))
         try:
             # Django extension v2
             from django.conf import settings  # noqa
+            import dynaconf
+            import django
+
+            # see https://docs.djangoproject.com/en/4.2/ref/applications/
+            # at #troubleshooting
+            django.setup()
 
             settings.DYNACONF.configure()
         except AttributeError:
             settings = LazySettings()
 
-        if settings is not None:
+        if settings is not None and _echo_enabled:
             click.echo(
                 click.style(
                     "Django app detected", fg="white", bg="bright_black"
                 )
             )
 
     if settings is None:
@@ -92,28 +112,30 @@
         else:
             settings = LazySettings()
 
 
 def import_settings(dotted_path):
     """Import settings instance from python dotted path.
 
-    Last item in dotted path must be settings instace.
+    Last item in dotted path must be settings instance.
 
     Example: import_settings('path.to.settings')
     """
     if "." in dotted_path:
         module, name = dotted_path.rsplit(".", 1)
     else:
         raise click.UsageError(
             f"invalid path to settings instance: {dotted_path}"
         )
     try:
         module = importlib.import_module(module)
     except ImportError as e:
         raise click.UsageError(e)
+    except FileNotFoundError:
+        return
     try:
         return getattr(module, name)
     except AttributeError as e:
         raise click.UsageError(e)
 
 
 def split_vars(_vars):
@@ -156,15 +178,15 @@
 
 def show_banner(ctx, param, value):
     """Shows dynaconf awesome banner"""
     if not value or ctx.resilient_parsing:
         return
     set_settings(ctx)
     click.echo(settings.dynaconf_banner)
-    click.echo("Learn more at: http://github.com/rochacbruno/dynaconf")
+    click.echo("Learn more at: http://github.com/dynaconf/dynaconf")
     ctx.exit()
 
 
 @click.group()
 @click.option(
     "--version",
     is_flag=True,
@@ -240,28 +262,43 @@
     ),
 )
 @click.option("--wg/--no-wg", default=True)
 @click.option("-y", default=False, is_flag=True)
 @click.option("--django", default=os.environ.get("DJANGO_SETTINGS_MODULE"))
 @click.pass_context
 def init(ctx, fileformat, path, env, _vars, _secrets, wg, y, django):
-    """Inits a dynaconf project
+    """
+    Inits a dynaconf project.
+
     By default it creates a settings.toml and a .secrets.toml
     for [default|development|staging|testing|production|global] envs.
 
     The format of the files can be changed passing
     --format=yaml|json|ini|py.
 
     This command must run on the project's root folder or you must pass
     --path=/myproject/root/folder.
 
     The --env/-e is deprecated (kept for compatibility but unused)
     """
     click.echo("⚙️  Configuring your Dynaconf environment")
     click.echo("-" * 42)
+    if "FLASK_APP" in os.environ:  # pragma: no cover
+        click.echo(
+            "⚠️  Flask detected, you can't use `dynaconf init` "
+            "on a flask project, instead go to dynaconf.com/flask/ "
+            "for more information.\n"
+            "Or add the following to your app.py\n"
+            "\n"
+            "from dynaconf import FlaskDynaconf\n"
+            "app = Flask(__name__)\n"
+            "FlaskDynaconf(app)\n"
+        )
+        exit(1)
+
     path = Path(path)
 
     if env is not None:
         click.secho(
             "⚠️ The --env/-e option is deprecated (kept for\n"
             "   compatibility but unused)\n",
             fg="red",
@@ -362,23 +399,22 @@
 
     if secrets_path:
         loader.write(secrets_path, secrets_data, merge=True)
         click.echo(f"🔑 {secrets_path.name} created to hold your secrets.\n")
         ignore_line = ".secrets.*"
         comment = "\n# Ignore dynaconf secret files\n"
         if not gitignore_path.exists():
-            with io.open(str(gitignore_path), "w", encoding=ENC) as f:
+            with open(str(gitignore_path), "w", encoding=ENC) as f:
                 f.writelines([comment, ignore_line, "\n"])
         else:
             existing = (
-                ignore_line
-                in io.open(str(gitignore_path), encoding=ENC).read()
+                ignore_line in open(str(gitignore_path), encoding=ENC).read()
             )
             if not existing:  # pragma: no cover
-                with io.open(str(gitignore_path), "a+", encoding=ENC) as f:
+                with open(str(gitignore_path), "a+", encoding=ENC) as f:
                     f.writelines([comment, ignore_line, "\n"])
 
         click.echo(
             f"🙈 the {secrets_path.name} is also included in `.gitignore` \n"
             "  beware to not push your secrets to a public repo \n"
             "  or use dynaconf builtin support for Vault Servers.\n"
         )
@@ -418,31 +454,41 @@
     "--unparse",
     "-u",
     default=False,
     help="Unparse data by adding markers such as @none, @int etc..",
     is_flag=True,
 )
 def get(key, default, env, unparse):
-    """Returns the raw value for a settings key"""
+    """Returns the raw value for a settings key.
+
+    If result is a dict, list or tuple it is printes as a valid json string.
+    """
     if env:
         env = env.strip()
     if key:
         key = key.strip()
 
     if env:
         settings.setenv(env)
 
     if default is not empty:
         result = settings.get(key, default)
     else:
-        result = settings[key]  # let the keyerror raises
+        try:
+            result = settings[key]
+        except KeyError:
+            click.echo("Key not found", nl=False, err=True)
+            sys.exit(1)
 
     if unparse:
         result = unparse_conf_data(result)
 
+    if isinstance(result, (dict, list, tuple)):
+        result = json.dumps(result, sort_keys=True)
+
     click.echo(result, nl=False)
 
 
 @main.command(name="list")
 @click.option(
     "--env", "-e", default=None, help="Filters the env to get the values"
 )
@@ -479,16 +525,19 @@
     "--output-flat",
     "flat",
     is_flag=True,
     default=False,
     help="Output file is flat (do not include [env] name)",
 )
 def _list(env, key, more, loader, _all=False, output=None, flat=False):
-    """Lists all user defined config values
-    and if `--all` is passed it also shows dynaconf internal variables.
+    """
+    Lists user defined settings or all (including internal configs).
+
+    By default, shows only user defined. If `--all` is passed it also shows
+    dynaconf internal variables aswell.
     """
     if env:
         env = env.strip()
     if key:
         key = key.strip()
     if loader:
         loader = loader.strip()
@@ -547,15 +596,15 @@
 
         try:
             value = settings.get(key, empty)
         except AttributeError:
             value = empty
 
         if value is empty:
-            click.echo(click.style("Key not found", bg="red", fg="white"))
+            click.secho("Key not found", bg="red", fg="white", err=True)
             return
 
         click.echo(format_setting(key, value))
         if output:
             loaders.write(output, {key: value}, env=not flat and cur_env)
 
     if env:
@@ -601,15 +650,15 @@
         "for external sources like Redis and Vault "
         "it will be DYNACONF or the value set in "
         "$ENVVAR_PREFIX_FOR_DYNACONF"
     ),
 )
 @click.option("-y", default=False, is_flag=True)
 def write(to, _vars, _secrets, path, env, y):
-    """Writes data to specific source"""
+    """Writes data to specific source."""
     _vars = split_vars(_vars)
     _secrets = split_vars(_secrets)
     loader = importlib.import_module(f"dynaconf.loaders.{to}_loader")
 
     if to in EXTS:
 
         # Lets write to a file
@@ -674,38 +723,65 @@
 
 
 @main.command()
 @click.option(
     "--path", "-p", default=CWD, help="defaults to current directory"
 )
 def validate(path):  # pragma: no cover
-    """Validates Dynaconf settings based on rules defined in
-    dynaconf_validators.toml"""
+    """
+    Validates Dynaconf settings based on provided rules.
+
+    Rules should be defined in dynaconf_validators.toml
+    """
     # reads the 'dynaconf_validators.toml' from path
     # for each section register the validator for specific env
     # call validate
-
     path = Path(path)
 
     if not str(path).endswith(".toml"):
         path = path / "dynaconf_validators.toml"
 
     if not path.exists():  # pragma: no cover  # noqa
         click.echo(click.style(f"{path} not found", fg="white", bg="red"))
         sys.exit(1)
 
-    validation_data = toml.load(open(str(path)))
+    # parse validator file
+    try:  # try tomlib first
+        validation_data = tomllib.load(open(str(path), "rb"))
+    except UnicodeDecodeError:  # fallback to legacy toml (TBR in 4.0.0)
+        warnings.warn(
+            "TOML files should have only UTF-8 encoded characters. "
+            "starting on 4.0.0 dynaconf will stop allowing invalid chars.",
+        )
+        validation_data = toml.load(
+            open(str(path), encoding=default_settings.ENCODING_FOR_DYNACONF),
+        )
+    except tomllib.TOMLDecodeError as e:
+        click.echo(
+            click.style(
+                f"Error parsing TOML: {e}. Maybe it should be quoted.",
+                fg="white",
+                bg="red",
+            )
+        )
+        sys.exit(1)
+
+    # guarantee there is an environment
+    validation_data = {k.lower(): v for k, v in validation_data.items()}
+    if not validation_data.get("default"):
+        validation_data = {"default": validation_data}
 
     success = True
     for env, name_data in validation_data.items():
         for name, data in name_data.items():
             if not isinstance(data, dict):  # pragma: no cover
                 click.echo(
                     click.style(
-                        f"Invalid rule for parameter '{name}'",
+                        f"Invalid rule for parameter '{name}'"
+                        "(this will be skipped)",
                         fg="white",
                         bg="yellow",
                     )
                 )
             else:
                 data.setdefault("env", env)
                 click.echo(
@@ -726,9 +802,57 @@
     if success:
         click.echo(click.style("Validation success!", fg="white", bg="green"))
     else:
         click.echo(click.style("Validation error!", fg="white", bg="red"))
         sys.exit(1)
 
 
+from dynaconf.utils.inspect import (
+    KeyNotFoundError,
+    builtin_dumpers,
+    inspect_settings,
+    EnvNotFoundError,
+    OutputFormatError,
+)
+
+INSPECT_FORMATS = list(builtin_dumpers.keys())
+
+
+@main.command()
+@click.option("--key", "-k", help="Filters result by key.")
+@click.option("--env", "-e", help="Filters result by environment.", default="")
+@click.option(
+    "--format",
+    "-f",
+    help="The output format.",
+    default="json",
+    type=click.Choice(INSPECT_FORMATS),
+)
+@click.option(
+    "--descending",
+    "-d",
+    help="Set history loading order to 'last-first'",
+    default=False,
+    is_flag=True,
+)
+def inspect(key, env, format, descending):  # pragma: no cover
+    """
+    Inspect the loading history of the given settings instance.
+
+    Filters by key and environement, otherwise shows all.
+    """
+    try:
+        inspect_settings(
+            settings,
+            key_dotted_path=key,
+            env=env,
+            output_format=format,
+            ascending_order=(not descending),
+        )
+        click.echo()
+    except (KeyNotFoundError, EnvNotFoundError, OutputFormatError) as err:
+        click.echo(err)
+        sys.exit(1)
+
+
 if __name__ == "__main__":  # pragma: no cover
     main()
```

### Comparing `dynaconf-3.1.9/dynaconf/constants.py` & `dynaconf-3.2.0/dynaconf/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # pragma: no cover
+from __future__ import annotations
+
 INI_EXTENSIONS = (".ini", ".conf", ".properties")
 TOML_EXTENSIONS = (".toml", ".tml")
 YAML_EXTENSIONS = (".yaml", ".yml")
 JSON_EXTENSIONS = (".json",)
 
 ALL_EXTENSIONS = (
     INI_EXTENSIONS + TOML_EXTENSIONS + YAML_EXTENSIONS + JSON_EXTENSIONS
```

### Comparing `dynaconf-3.1.9/dynaconf/contrib/django_dynaconf_v2.py` & `dynaconf-3.2.0/dynaconf/contrib/django_dynaconf_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Dynaconf django extension
 
-In the `django_project/settings.py` put at the very botton of the file:
+In the `django_project/settings.py` put at the very bottom of the file:
 
 # HERE STARTS DYNACONF EXTENSION LOAD (Keep at the very bottom of settings.py)
 # Read more at https://www.dynaconf.com/django/
 import dynaconf  # noqa
 settings = dynaconf.DjangoDynaconf(__name__)  # noqa
 # HERE ENDS DYNACONF EXTENSION LOAD (No more code below this line)
 
@@ -16,14 +16,16 @@
 
 On your projects root folder now you can start as::
 
     DJANGO_DEBUG='false' \
     DJANGO_ALLOWED_HOSTS='["localhost"]' \
     python manage.py runserver
 """
+from __future__ import annotations
+
 import inspect
 import os
 import sys
 
 import dynaconf
 
 try:  # pragma: no cover
```

### Comparing `dynaconf-3.1.9/dynaconf/contrib/flask_dynaconf.py` & `dynaconf-3.2.0/dynaconf/contrib/flask_dynaconf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from __future__ import annotations
+
 import warnings
 from collections import ChainMap
 from contextlib import suppress
 
 try:
     from flask.config import Config
 
     flask_installed = True
 except ImportError:  # pragma: no cover
     flask_installed = False
     Config = object
 
 
 import dynaconf
-import pkg_resources
+from importlib.metadata import EntryPoint
 
 
 class FlaskDynaconf:
     """The arguments are.
     app = The created app
     dynaconf_args = Extra args to be passed to Dynaconf (validator for example)
 
@@ -65,15 +67,15 @@
     Example::
 
         app = Flask(__name__)
         FlaskDynaconf(
             app,
             ENV='MYSITE',
             SETTINGS_FILE='settings.yml',
-            EXTRA_VALUE='You can add aditional config vars here'
+            EXTRA_VALUE='You can add additional config vars here'
         )
 
     Take a look at examples/flask in Dynaconf repository
 
     """
 
     def __init__(
@@ -87,20 +89,20 @@
         """kwargs holds initial dynaconf configuration"""
         if not flask_installed:  # pragma: no cover
             raise RuntimeError(
                 "To use this extension Flask must be installed "
                 "install it with: pip install flask"
             )
         self.kwargs = {k.upper(): v for k, v in kwargs.items()}
-        kwargs.setdefault("ENVVAR_PREFIX", "FLASK")
-        env_prefix = f"{kwargs['ENVVAR_PREFIX']}_ENV"  # FLASK_ENV
-        kwargs.setdefault("ENV_SWITCHER", env_prefix)
-        kwargs.setdefault("ENVIRONMENTS", True)
-        kwargs.setdefault("load_dotenv", True)
-        kwargs.setdefault(
+        self.kwargs.setdefault("ENVVAR_PREFIX", "FLASK")
+        env_prefix = f"{self.kwargs['ENVVAR_PREFIX']}_ENV"  # FLASK_ENV
+        self.kwargs.setdefault("ENV_SWITCHER", env_prefix)
+        self.kwargs.setdefault("ENVIRONMENTS", True)
+        self.kwargs.setdefault("LOAD_DOTENV", True)
+        self.kwargs.setdefault(
             "default_settings_paths", dynaconf.DEFAULT_SETTINGS_FILES
         )
 
         self.dynaconf_instance = dynaconf_instance
         self.instance_relative_config = instance_relative_config
         self.extensions_list = extensions_list
         if app:
@@ -138,15 +140,15 @@
 class DynaconfConfig(Config):
     """
     Replacement for flask.config_class that responds as a Dynaconf instance.
     """
 
     def __init__(self, _settings, _app, *args, **kwargs):
         """perform the initial load"""
-        super(DynaconfConfig, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
         # Bring Dynaconf instance value to Flask Config
         Config.update(self, _settings.store)
 
         self._settings = _settings
         self._app = _app
 
@@ -214,15 +216,15 @@
             warnings.warn(
                 f"Settings is missing {key} to load Flask Extensions",
                 RuntimeWarning,
             )
             return
 
         for object_reference in app.config[key]:
-            # add a placeholder `name` to create a valid entry point
-            entry_point_spec = f"__name = {object_reference}"
             # parse the entry point specification
-            entry_point = pkg_resources.EntryPoint.parse(entry_point_spec)
+            entry_point = EntryPoint(
+                name=None, group=None, value=object_reference
+            )
             # dynamically resolve the entry point
-            initializer = entry_point.resolve()
+            initializer = entry_point.load()
             # Invoke extension initializer
             initializer(app)
```

### Comparing `dynaconf-3.1.9/dynaconf/default_settings.py` & `dynaconf-3.2.0/dynaconf/default_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import importlib
 import os
 import sys
 import warnings
 
 from dynaconf.utils import RENAMED_VARS
 from dynaconf.utils import upperfy
@@ -80,15 +82,15 @@
 if not SETTINGS_FILE_FOR_DYNACONF and mispelled_files is not None:
     SETTINGS_FILE_FOR_DYNACONF = mispelled_files
 
 # # ENV SETTINGS
 # # In dynaconf 1.0.0 `NAMESPACE` got renamed to `ENV`
 
 
-# If provided environments will be loaded separatelly
+# If provided environments will be loaded separately
 ENVIRONMENTS_FOR_DYNACONF = get("ENVIRONMENTS_FOR_DYNACONF", False)
 MAIN_ENV_FOR_DYNACONF = get("MAIN_ENV_FOR_DYNACONF", "MAIN")
 
 # If False dynaconf will allow access to first level settings only in upper
 LOWERCASE_READ_FOR_DYNACONF = get("LOWERCASE_READ_FOR_DYNACONF", True)
 
 # The environment variable to switch current env
@@ -119,14 +121,16 @@
 # setting this flag to `True` will change this behaviour.
 # Only "known" variables will be considered -- that is variables defined before
 # in settings files (or includes/preloads).
 IGNORE_UNKNOWN_ENVVARS_FOR_DYNACONF = get(
     "IGNORE_UNKNOWN_ENVVARS_FOR_DYNACONF", False
 )
 
+AUTO_CAST_FOR_DYNACONF = get("AUTO_CAST_FOR_DYNACONF", True)
+
 # The default encoding to open settings files
 ENCODING_FOR_DYNACONF = get("ENCODING_FOR_DYNACONF", "utf-8")
 
 # Merge objects on load
 MERGE_ENABLED_FOR_DYNACONF = get("MERGE_ENABLED_FOR_DYNACONF", False)
 
 # Lookup keys considering dots as separators
@@ -164,14 +168,15 @@
     ),
     "token": get("VAULT_TOKEN_FOR_DYNACONF", None),
     "cert": get("VAULT_CERT_FOR_DYNACONF", None),
     "verify": get("VAULT_VERIFY_FOR_DYNACONF", None),
     "timeout": get("VAULT_TIMEOUT_FOR_DYNACONF", None),
     "proxies": get("VAULT_PROXIES_FOR_DYNACONF", None),
     "allow_redirects": get("VAULT_ALLOW_REDIRECTS_FOR_DYNACONF", None),
+    "namespace": get("VAULT_NAMESPACE_FOR_DYNACONF", None),
 }
 VAULT_FOR_DYNACONF = get("VAULT_FOR_DYNACONF", default_vault)
 VAULT_ENABLED_FOR_DYNACONF = get("VAULT_ENABLED_FOR_DYNACONF", False)
 VAULT_PATH_FOR_DYNACONF = get("VAULT_PATH_FOR_DYNACONF", "dynaconf")
 VAULT_MOUNT_POINT_FOR_DYNACONF = get(
     "VAULT_MOUNT_POINT_FOR_DYNACONF", "secret"
 )
@@ -179,14 +184,16 @@
 VAULT_KV_VERSION_FOR_DYNACONF = get("VAULT_KV_VERSION_FOR_DYNACONF", 1)
 VAULT_AUTH_WITH_IAM_FOR_DYNACONF = get(
     "VAULT_AUTH_WITH_IAM_FOR_DYNACONF", False
 )
 VAULT_AUTH_ROLE_FOR_DYNACONF = get("VAULT_AUTH_ROLE_FOR_DYNACONF", None)
 VAULT_ROLE_ID_FOR_DYNACONF = get("VAULT_ROLE_ID_FOR_DYNACONF", None)
 VAULT_SECRET_ID_FOR_DYNACONF = get("VAULT_SECRET_ID_FOR_DYNACONF", None)
+VAULT_USERNAME_FOR_DYNACONF = get("VAULT_USERNAME_FOR_DYNACONF", None)
+VAULT_PASSWORD_FOR_DYNACONF = get("VAULT_PASSWORD_FOR_DYNACONF", None)
 
 # Only core loaders defined on this list will be invoked
 core_loaders = ["YAML", "TOML", "INI", "JSON", "PY"]
 CORE_LOADERS_FOR_DYNACONF = get("CORE_LOADERS_FOR_DYNACONF", core_loaders)
 
 # External Loaders to read vars from different data stores
 default_loaders = [
@@ -237,11 +244,18 @@
 # YAML reads empty vars as None, should dynaconf apply validator defaults?
 # this is set to None, then evaluated on base.Settings.setdefault
 # possible values are True/False
 APPLY_DEFAULT_ON_NONE_FOR_DYNACONF = get(
     "APPLY_DEFAULT_ON_NONE_FOR_DYNACONF", None
 )
 
+# Auto trigger validation when Settings update methods are called directly
+# (set, update, load_file)
+VALIDATE_ON_UPDATE_FOR_DYNACONF = get("VALIDATE_ON_UPDATE_FOR_DYNACONF", False)
+
+# Use system environ as fallback when a setting was not set
+SYSENV_FALLBACK_FOR_DYNACONF = get("SYSENV_FALLBACK_FOR_DYNACONF", False)
+
 
 # Backwards compatibility with renamed variables
 for old, new in RENAMED_VARS.items():
     setattr(sys.modules[__name__], old, locals()[new])
```

### Comparing `dynaconf-3.1.9/dynaconf/loaders/__init__.py` & `dynaconf-3.2.0/dynaconf/loaders/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,30 @@
+from __future__ import annotations
+
 import importlib
 import os
+from typing import Callable
+from typing import TYPE_CHECKING
 
 from dynaconf import constants as ct
 from dynaconf import default_settings
 from dynaconf.loaders import ini_loader
 from dynaconf.loaders import json_loader
 from dynaconf.loaders import py_loader
 from dynaconf.loaders import toml_loader
 from dynaconf.loaders import yaml_loader
 from dynaconf.utils import deduplicate
 from dynaconf.utils import ensure_a_list
 from dynaconf.utils.boxing import DynaBox
 from dynaconf.utils.files import get_local_filename
 from dynaconf.utils.parse_conf import false_values
 
+if TYPE_CHECKING:
+    from dynaconf.base import Settings
+
 
 def default_loader(obj, defaults=None):
     """Loads default settings and check if there are overridings
     exported as environment variables"""
     defaults = defaults or {}
     default_settings_values = {
         key: value
@@ -54,43 +61,24 @@
             default="_not_found",
         )
 
         if env_value != "_not_found":
             obj.set(key, env_value, tomlfy=True)
 
 
-def _run_hook_module(hook, hook_module, obj, key=None):
-    """Run the hook function from the settings obj.
-
-    given a hook name, a hook_module and a settings object
-    load the function and execute if found.
-    """
-    if hook in obj._loaded_hooks.get(hook_module.__file__, {}):
-        # already loaded
-        return
-
-    if hook_module and getattr(hook_module, "_error", False):
-        if not isinstance(hook_module._error, FileNotFoundError):
-            raise hook_module._error
-
-    hook_func = getattr(hook_module, hook, None)
-    if hook_func:
-        hook_dict = hook_func(obj.dynaconf.clone())
-        if hook_dict:
-            merge = hook_dict.pop(
-                "dynaconf_merge", hook_dict.pop("DYNACONF_MERGE", False)
-            )
-            if key and key in hook_dict:
-                obj.set(key, hook_dict[key], tomlfy=False, merge=merge)
-            elif not key:
-                obj.update(hook_dict, tomlfy=False, merge=merge)
-        obj._loaded_hooks[hook_module.__file__][hook] = hook_dict
+def execute_instance_hooks(
+    obj: Settings, hook_type: str, hook_functions: list[Callable]
+):
+    """Execute hooks provided by Setting instance"""
+    hook_source = "instance"
+    for hook_func in hook_functions:
+        _run_hook_function(obj, hook_type, hook_func, hook_source)
 
 
-def execute_hooks(
+def execute_module_hooks(
     hook, obj, env=None, silent=True, key=None, modules=None, files=None
 ):
     """Execute dynaconf_hooks from module or filepath."""
     if hook not in ["post"]:
         raise ValueError(f"hook {hook} not supported yet.")
 
     # try to load hooks using python module __name__
@@ -102,15 +90,15 @@
         try:
             hook_module = importlib.import_module(hook_module_name)
         except (ImportError, TypeError):
             # There was no hook on the same path as a python module
             continue
         else:
             _run_hook_module(
-                hook=hook,
+                hook_type=hook,
                 hook_module=hook_module,
                 obj=obj,
                 key=key,
             )
 
     # Try to load from python filename path
     files = files or obj._loaded_files
@@ -121,23 +109,90 @@
         hook_module = py_loader.import_from_filename(
             obj, hook_file, silent=silent
         )
         if not hook_module:
             # There was no hook on the same path as a python file
             continue
         _run_hook_module(
-            hook=hook,
+            hook_type=hook,
             hook_module=hook_module,
             obj=obj,
             key=key,
         )
 
 
+# alias
+execute_hooks = execute_module_hooks
+
+
+def _run_hook_module(hook_type, hook_module, obj, key=""):
+    """
+    Run a hook function from hook_module.
+
+    Given a @hook_type, a @hook_module and a settings @obj, load the function
+    and execute it if found.
+    """
+    hook_source = hook_module.__file__
+
+    # check if already loaded
+    if hook_type in obj._loaded_hooks.get(hook_source, {}):
+        return
+
+    # check errors
+    if hook_module and getattr(hook_module, "_error", False):
+        if not isinstance(hook_module._error, FileNotFoundError):
+            raise hook_module._error
+
+    # execute hook
+    hook_func = getattr(hook_module, hook_type, None)
+    if hook_func:
+        _run_hook_function(obj, hook_type, hook_func, hook_source, key)
+
+
+def _run_hook_function(
+    obj: Settings,
+    hook_type: str,
+    hook_func: Callable,
+    hook_source: str = "default",
+    key: str = "",
+):
+    """
+    Run a hook function:
+
+    It execute @hook_func, update the results into settings @obj and
+    add it to _loaded_hook registry ([@hook_source][@hook_type])
+    """
+    # optional settings argument
+    try:
+        hook_dict = hook_func(obj.dynaconf.clone())
+    except TypeError:
+        hook_dict = hook_func()
+
+    # update obj settings
+    if hook_dict:
+        merge = hook_dict.pop(
+            "dynaconf_merge", hook_dict.pop("DYNACONF_MERGE", False)
+        )
+        if key and key in hook_dict:
+            obj.set(key, hook_dict[key], tomlfy=False, merge=merge)
+        elif not key:
+            obj.update(hook_dict, tomlfy=False, merge=merge)
+
+    # add to registry
+    obj._loaded_hooks[hook_source][hook_type] = hook_dict
+
+
 def settings_loader(
-    obj, settings_module=None, env=None, silent=True, key=None, filename=None
+    obj,
+    settings_module=None,
+    env=None,
+    silent=True,
+    key=None,
+    filename=None,
+    validate=False,
 ):
     """Loads from defined settings module
 
     :param obj: A dynaconf instance
     :param settings_module: A path or a list of paths e.g settings.toml
     :param env: Env to look for data defaults: development
     :param silent: Boolean to raise loading errors
@@ -195,28 +250,33 @@
 
         for loader in loaders:
             if loader["name"] not in enabled_core_loaders:
                 continue
 
             if mod_file.endswith(loader["ext"]):
                 loader["loader"].load(
-                    obj, filename=mod_file, env=env, silent=silent, key=key
+                    obj,
+                    filename=mod_file,
+                    env=env,
+                    silent=silent,
+                    key=key,
+                    validate=validate,
                 )
                 continue
 
         if mod_file.endswith(ct.ALL_EXTENSIONS):
             continue
 
         if "PY" not in enabled_core_loaders:
             # pyloader is disabled
             continue
 
         # must be Python file or module
         # load from default defined module settings.py or .secrets.py if exists
-        py_loader.load(obj, mod_file, key=key)
+        py_loader.load(obj, mod_file, key=key, validate=validate)
 
         # load from the current env e.g: development_settings.py
         env = env or obj.current_env
         if mod_file.endswith(".py"):
             if ".secrets.py" == mod_file:
                 tmpl = ".{0}_{1}{2}"
                 mod_file = "secrets.py"
@@ -235,19 +295,25 @@
 
         py_loader.load(
             obj,
             env_mod_file,
             identifier=f"py_{env.upper()}",
             silent=True,
             key=key,
+            validate=validate,
         )
 
         # load from global_settings.py
         py_loader.load(
-            obj, global_mod_file, identifier="py_global", silent=True, key=key
+            obj,
+            global_mod_file,
+            identifier="py_global",
+            silent=True,
+            key=key,
+            validate=validate,
         )
 
 
 def enable_external_loaders(obj):
     """Enable external service loaders like `VAULT_` and `REDIS_`
     looks forenv variables like `REDIS_ENABLED_FOR_DYNACONF`
     """
@@ -257,19 +323,19 @@
             enabled
             and enabled not in false_values
             and loader not in obj.LOADERS_FOR_DYNACONF
         ):  # noqa
             obj.LOADERS_FOR_DYNACONF.insert(0, loader)
 
 
-def write(filename, data, env=None):
+def write(filename, data, env=None, merge=False):
     """Writes `data` to `filename` infers format by file extension."""
     loader_name = f"{filename.rpartition('.')[-1]}_loader"
     loader = globals().get(loader_name)
     if not loader:
-        raise IOError(f"{loader_name} cannot be found.")
+        raise OSError(f"{loader_name} cannot be found.")
 
     data = DynaBox(data, box_settings={}).to_dict()
     if loader is not py_loader and env and env not in data:
         data = {env: data}
 
-    loader.write(filename, data, merge=False)
+    loader.write(filename, data, merge=merge)
```

### Comparing `dynaconf-3.1.9/dynaconf/loaders/base.py` & `dynaconf-3.2.0/dynaconf/loaders/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+from __future__ import annotations
+
 import io
 import warnings
+from typing import NamedTuple
 
 from dynaconf.utils import build_env_list
 from dynaconf.utils import ensure_a_list
 from dynaconf.utils import upperfy
+from dynaconf.utils.functional import empty
 
 
 class BaseLoader:
     """Base loader for dynaconf source files.
 
     :param obj: {[LazySettings]} -- [Dynaconf settings]
     :param env: {[string]} -- [the current env to be loaded defaults to
@@ -15,40 +19,53 @@
     :param identifier: {[string]} -- [identifier ini, yaml, json, py, toml]
     :param extensions: {[list]} -- [List of extensions with dots ['.a', '.b']]
     :param file_reader: {[callable]} -- [reads file return dict]
     :param string_reader: {[callable]} -- [reads string return dict]
     """
 
     def __init__(
-        self, obj, env, identifier, extensions, file_reader, string_reader
+        self,
+        obj,
+        env,
+        identifier,
+        extensions,
+        file_reader,
+        string_reader,
+        opener_params=None,
+        validate=False,
     ):
         """Instantiates a loader for different sources"""
         self.obj = obj
         self.env = env or obj.current_env
         self.identifier = identifier
         self.extensions = extensions
         self.file_reader = file_reader
         self.string_reader = string_reader
+        self.opener_params = opener_params or {
+            "mode": "r",
+            "encoding": obj.get("ENCODING_FOR_DYNACONF", "utf-8"),
+        }
+        self.validate = validate
 
     @staticmethod
     def warn_not_installed(obj, identifier):  # pragma: no cover
         if identifier not in obj._not_installed_warnings:
             warnings.warn(
                 f"{identifier} support is not installed in your environment. "
                 f"`pip install dynaconf[{identifier}]`"
             )
         obj._not_installed_warnings.append(identifier)
 
-    def load(self, filename=None, key=None, silent=True):
+    def load(self, filename=None, key=None, silent=True, merge=empty):
         """
         Reads and loads in to `self.obj` a single key or all keys from source
 
         :param filename: Optional filename to load
         :param key: if provided load a single key
-        :param silent: if load erros should be silenced
+        :param silent: if load errors should be silenced
         """
 
         filename = filename or self.obj.get(self.identifier.upper())
         if not filename:
             return
 
         if not isinstance(filename, (list, tuple)):
@@ -71,100 +88,119 @@
         """Reads each file and returns source data for each file
         {"path/to/file.ext": {"key": "value"}}
         """
         data = {}
         for source_file in files:
             if source_file.endswith(self.extensions):
                 try:
-                    with io.open(
-                        source_file,
-                        encoding=self.obj.get(
-                            "ENCODING_FOR_DYNACONF", "utf-8"
-                        ),
-                    ) as open_file:
+                    with open(source_file, **self.opener_params) as open_file:
                         content = self.file_reader(open_file)
                         self.obj._loaded_files.append(source_file)
                         if content:
                             data[source_file] = content
-                except IOError as e:
+                except OSError as e:
                     if ".local." not in source_file:
                         warnings.warn(
                             f"{self.identifier}_loader: {source_file} "
                             f":{str(e)}"
                         )
             else:
                 # for tests it is possible to pass string
                 content = self.string_reader(source_file)
                 if content:
                     data[source_file] = content
         return data
 
     def _envless_load(self, source_data, silent=True, key=None):
         """Load all the keys from each file without env separation"""
-        for file_data in source_data.values():
+        for file_name, file_data in source_data.items():
+            # is there a `dynaconf_merge` on top level of file?
+            file_merge = file_data.get("dynaconf_merge", empty)
+
+            # set source metadata
+            source_metadata = SourceMetadata(
+                self.identifier, file_name, "default"
+            )
+
             self._set_data_to_obj(
                 file_data,
-                self.identifier,
+                source_metadata,
+                file_merge=file_merge,
                 key=key,
             )
 
     def _load_all_envs(self, source_data, silent=True, key=None):
-        """Load configs from files separating by each environment"""
-
-        for file_data in source_data.values():
-
+        """
+        Load configs from files separating by each environment
+        source_data should have format:
+            {
+                "path/to/src": {
+                    "env": {...},
+                    "env2": {...}
+                }
+            }
+        """
+        for file_name, file_data in source_data.items():
             # env name is checked in lower
             file_data = {k.lower(): value for k, value in file_data.items()}
 
             # is there a `dynaconf_merge` on top level of file?
-            file_merge = file_data.get("dynaconf_merge")
+            file_merge = file_data.get("dynaconf_merge", empty)
 
             # is there a flag disabling dotted lookup on file?
             file_dotted_lookup = file_data.get("dynaconf_dotted_lookup")
 
             for env in build_env_list(self.obj, self.env):
                 env = env.lower()  # lower for better comparison
+                # print(self.env, file_data)
+
+                # set source metadata
+                source_metadata = SourceMetadata(
+                    self.identifier, file_name, env
+                )
 
                 try:
                     data = file_data[env] or {}
                 except KeyError:
                     if silent:
                         continue
                     raise
 
                 if not data:
                     continue
 
                 self._set_data_to_obj(
                     data,
-                    f"{self.identifier}_{env}",
+                    source_metadata,
                     file_merge,
                     key,
                     file_dotted_lookup=file_dotted_lookup,
                 )
 
     def _set_data_to_obj(
         self,
         data,
-        identifier,
-        file_merge=None,
+        identifier: SourceMetadata,
+        file_merge=empty,
         key=False,
         file_dotted_lookup=None,
     ):
         """Calls settings.set to add the keys"""
         # data 1st level keys should be transformed to upper case.
         data = {upperfy(k): v for k, v in data.items()}
         if key:
             key = upperfy(key)
 
         if self.obj.filter_strategy:
             data = self.obj.filter_strategy(data)
 
         # is there a `dynaconf_merge` inside an `[env]`?
-        file_merge = file_merge or data.pop("DYNACONF_MERGE", False)
+        env_scope_merge = data.pop("DYNACONF_MERGE", None)
+        if env_scope_merge is not None:
+            file_merge = env_scope_merge
 
         # If not passed or passed as None,
         # look for inner [env] value, or default settings.
         if file_dotted_lookup is None:
             file_dotted_lookup = data.pop(
                 "DYNACONF_DOTTED_LOOKUP",
                 self.obj.get("DOTTED_LOOKUP_FOR_DYNACONF"),
@@ -172,16 +208,36 @@
 
         if not key:
             self.obj.update(
                 data,
                 loader_identifier=identifier,
                 merge=file_merge,
                 dotted_lookup=file_dotted_lookup,
+                validate=self.validate,
             )
         elif key in data:
             self.obj.set(
                 key,
                 data.get(key),
                 loader_identifier=identifier,
                 merge=file_merge,
                 dotted_lookup=file_dotted_lookup,
+                validate=self.validate,
             )
+
+
+class SourceMetadata(NamedTuple):
+    """
+    Usefull metadata about some loaded source (file, envvar, etc).
+
+    Serve as a unique identifier for data from a specific env
+    and a specific source (file, envvar, validationd default, etc)
+
+    Examples:
+        SourceMetadata(loader="envvar", identifier="os", env="global")
+        SourceMetadata(loader="yaml", identifier="path/to/file.yml", env="dev")
+    """
+
+    loader: str
+    identifier: str
+    env: str
+    merged: bool = False
```

### Comparing `dynaconf-3.1.9/dynaconf/loaders/ini_loader.py` & `dynaconf-3.2.0/dynaconf/loaders/ini_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from __future__ import annotations
+
 import io
 from pathlib import Path
 
 from dynaconf import default_settings
 from dynaconf.constants import INI_EXTENSIONS
 from dynaconf.loaders.base import BaseLoader
 from dynaconf.utils import object_merge
 
 try:
     from configobj import ConfigObj
 except ImportError:  # pragma: no cover
     ConfigObj = None
 
 
-def load(obj, env=None, silent=True, key=None, filename=None):
+def load(obj, env=None, silent=True, key=None, filename=None, validate=False):
     """
     Reads and loads in to "obj" a single key or all keys from source file.
 
     :param obj: the settings instance
     :param env: settings current env default='development'
     :param silent: if errors should raise
     :param key: if defined load a single key, else load all in env
@@ -30,14 +32,15 @@
     loader = BaseLoader(
         obj=obj,
         env=env,
         identifier="ini",
         extensions=INI_EXTENSIONS,
         file_reader=lambda fileobj: ConfigObj(fileobj).dict(),
         string_reader=lambda strobj: ConfigObj(strobj.split("\n")).dict(),
+        validate=validate,
     )
     loader.load(
         filename=filename,
         key=key,
         silent=silent,
     )
 
@@ -47,14 +50,14 @@
 
     :param settings_path: the filepath
     :param settings_data: a dictionary with data
     :param merge: boolean if existing file should be merged with new data
     """
     settings_path = Path(settings_path)
     if settings_path.exists() and merge:  # pragma: no cover
-        with io.open(
+        with open(
             str(settings_path), encoding=default_settings.ENCODING_FOR_DYNACONF
         ) as open_file:
             object_merge(ConfigObj(open_file).dict(), settings_data)
     new = ConfigObj()
     new.update(settings_data)
     new.write(open(str(settings_path), "bw"))
```

### Comparing `dynaconf-3.1.9/dynaconf/loaders/json_loader.py` & `dynaconf-3.2.0/dynaconf/loaders/json_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import io
 import json
 from pathlib import Path
 
 from dynaconf import default_settings
 from dynaconf.constants import JSON_EXTENSIONS
 from dynaconf.loaders.base import BaseLoader
@@ -10,15 +12,15 @@
 
 try:  # pragma: no cover
     import commentjson
 except ImportError:  # pragma: no cover
     commentjson = None
 
 
-def load(obj, env=None, silent=True, key=None, filename=None):
+def load(obj, env=None, silent=True, key=None, filename=None, validate=False):
     """
     Reads and loads in to "obj" a single key or all keys from source file.
 
     :param obj: the settings instance
     :param env: settings current env default='development'
     :param silent: if errors should raise
     :param key: if defined load a single key, else load all in env
@@ -37,14 +39,15 @@
     loader = BaseLoader(
         obj=obj,
         env=env,
         identifier="json",
         extensions=JSON_EXTENSIONS,
         file_reader=file_reader,
         string_reader=string_reader,
+        validate=validate,
     )
     loader.load(
         filename=filename,
         key=key,
         silent=silent,
     )
 
@@ -54,20 +57,20 @@
 
     :param settings_path: the filepath
     :param settings_data: a dictionary with data
     :param merge: boolean if existing file should be merged with new data
     """
     settings_path = Path(settings_path)
     if settings_path.exists() and merge:  # pragma: no cover
-        with io.open(
+        with open(
             str(settings_path), encoding=default_settings.ENCODING_FOR_DYNACONF
         ) as open_file:
             object_merge(json.load(open_file), settings_data)
 
-    with io.open(
+    with open(
         str(settings_path),
         "w",
         encoding=default_settings.ENCODING_FOR_DYNACONF,
     ) as open_file:
         json.dump(settings_data, open_file, cls=DynaconfEncoder)
```

### Comparing `dynaconf-3.1.9/dynaconf/loaders/py_loader.py` & `dynaconf-3.2.0/dynaconf/loaders/py_loader.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,105 @@
+from __future__ import annotations
+
 import errno
 import importlib
 import inspect
 import io
 import types
 from contextlib import suppress
 from pathlib import Path
 
 from dynaconf import default_settings
+from dynaconf.loaders.base import SourceMetadata
 from dynaconf.utils import DynaconfDict
 from dynaconf.utils import object_merge
 from dynaconf.utils import upperfy
 from dynaconf.utils.files import find_file
+from dynaconf.utils.functional import empty
+
 
+def load(
+    obj,
+    settings_module,
+    identifier="py",
+    silent=False,
+    key=None,
+    validate=False,
+):
+    """
+    Tries to import a python module
 
-def load(obj, settings_module, identifier="py", silent=False, key=None):
-    """Tries to import a python module"""
+    Notes:
+        It doesn't handle environment namespaces explicitly. Eg
+            [default], [development], etc
+        See tests/test_nested_loading.py sample python file
+    """
     mod, loaded_from = get_module(obj, settings_module, silent)
     if not (mod and loaded_from):
         return
-    load_from_python_object(obj, mod, settings_module, key, identifier)
+
+    # setup SourceMetadata (for inspecting)
+    loader_identifier = SourceMetadata(identifier, mod.__name__, "global")
+
+    load_from_python_object(
+        obj, mod, settings_module, key, loader_identifier, validate=validate
+    )
 
 
 def load_from_python_object(
-    obj, mod, settings_module, key=None, identifier=None
+    obj, mod, settings_module, key=None, identifier=None, validate=False
 ):
-    file_merge = getattr(mod, "dynaconf_merge", False) or getattr(
-        mod, "DYNACONF_MERGE", False
-    )
+    file_merge = getattr(mod, "dynaconf_merge", empty)
+    if file_merge is empty:
+        file_merge = getattr(mod, "DYNACONF_MERGE", empty)
+
     for setting in dir(mod):
         # A setting var in a Python file should start with upper case
         # valid: A_value=1, ABC_value=3 A_BBB__default=1
         # invalid: a_value=1, MyValue=3
         # This is to avoid loading functions, classes and built-ins
         if setting.split("__")[0].isupper():
             if key is None or key == setting:
                 setting_value = getattr(mod, setting)
                 obj.set(
                     setting,
                     setting_value,
                     loader_identifier=identifier,
                     merge=file_merge,
+                    validate=validate,
                 )
 
     obj._loaded_py_modules.append(mod.__name__)
     obj._loaded_files.append(mod.__file__)
 
 
 def try_to_load_from_py_module_name(
-    obj, name, key=None, identifier="py", silent=False
+    obj, name, key=None, identifier="py", silent=False, validate=False
 ):
     """Try to load module by its string name.
 
     Arguments:
         obj {LAzySettings} -- Dynaconf settings instance
         name {str} -- Name of the module e.g: foo.bar.zaz
 
     Keyword Arguments:
         key {str} -- Single key to be loaded (default: {None})
         identifier {str} -- Name of identifier to store (default: 'py')
         silent {bool} -- Weather to raise or silence exceptions.
     """
     ctx = suppress(ImportError, TypeError) if silent else suppress()
 
+    # setup SourceMetadata (for inspecting)
+    loader_identifier = SourceMetadata(identifier, name, "global")
+
     with ctx:
         mod = importlib.import_module(str(name))
-        load_from_python_object(obj, mod, name, key, identifier)
+        load_from_python_object(
+            obj, mod, name, key, loader_identifier, validate=validate
+        )
         return True  # loaded ok!
     # if it reaches this point that means exception occurred, module not found.
     return False
 
 
 def get_module(obj, filename, silent=False):
     try:
@@ -104,20 +135,20 @@
     if filename in default_settings.SETTINGS_FILE_FOR_DYNACONF:
         silent = True
     mod = types.ModuleType(filename.rstrip(".py"))
     mod.__file__ = filename
     mod._is_error = False
     mod._error = None
     try:
-        with io.open(
+        with open(
             _find_file(filename),
             encoding=default_settings.ENCODING_FOR_DYNACONF,
         ) as config_file:
             exec(compile(config_file.read(), filename, "exec"), mod.__dict__)
-    except IOError as e:
+    except OSError as e:
         e.strerror = (
             f"py_loader: error loading file " f"({e.strerror} {filename})\n"
         )
         if silent and e.errno in (errno.ENOENT, errno.EISDIR):
             return
         mod._is_error = True
         mod._error = e
@@ -132,15 +163,15 @@
     :param merge: boolean if existing file should be merged with new data
     """
     settings_path = Path(settings_path)
     if settings_path.exists() and merge:  # pragma: no cover
         existing = DynaconfDict()
         load(existing, str(settings_path))
         object_merge(existing, settings_data)
-    with io.open(
+    with open(
         str(settings_path),
         "w",
         encoding=default_settings.ENCODING_FOR_DYNACONF,
     ) as f:
         f.writelines(
             [f"{upperfy(k)} = {repr(v)}\n" for k, v in settings_data.items()]
         )
```

### Comparing `dynaconf-3.1.9/dynaconf/loaders/redis_loader.py` & `dynaconf-3.2.0/dynaconf/loaders/redis_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+from __future__ import annotations
+
+from dynaconf.loaders.base import SourceMetadata
 from dynaconf.utils import build_env_list
 from dynaconf.utils import upperfy
 from dynaconf.utils.parse_conf import parse_conf_data
 from dynaconf.utils.parse_conf import unparse_conf_data
 
 try:
     from redis import StrictRedis
 except ImportError:
     StrictRedis = None
 
 IDENTIFIER = "redis"
 
 
-def load(obj, env=None, silent=True, key=None):
+def load(obj, env=None, silent=True, key=None, validate=False):
     """Reads and loads in to "settings" a single key or all keys from redis
 
     :param obj: the settings instance
     :param env: settings env default='DYNACONF'
     :param silent: if errors should raise
     :param key: if defined load a single key, else load all in env
     :return: None
@@ -30,29 +33,39 @@
     redis = StrictRedis(**obj.get("REDIS_FOR_DYNACONF"))
     prefix = obj.get("ENVVAR_PREFIX_FOR_DYNACONF")
     # prefix is added to env_list to keep backwards compatibility
     env_list = [prefix] + build_env_list(obj, env or obj.current_env)
     for env_name in env_list:
         holder = f"{prefix.upper()}_{env_name.upper()}"
         try:
+            source_metadata = SourceMetadata(IDENTIFIER, "unique", env_name)
             if key:
                 value = redis.hget(holder.upper(), key)
                 if value:
                     parsed_value = parse_conf_data(
                         value, tomlfy=True, box_settings=obj
                     )
                     if parsed_value:
-                        obj.set(key, parsed_value)
+                        obj.set(
+                            key,
+                            parsed_value,
+                            validate=validate,
+                            loader_identifier=source_metadata,
+                        )
             else:
                 data = {
                     key: parse_conf_data(value, tomlfy=True, box_settings=obj)
                     for key, value in redis.hgetall(holder.upper()).items()
                 }
                 if data:
-                    obj.update(data, loader_identifier=IDENTIFIER)
+                    obj.update(
+                        data,
+                        loader_identifier=source_metadata,
+                        validate=validate,
+                    )
         except Exception:
             if silent:
                 return False
             raise
 
 
 def write(obj, data=None, **kwargs):
@@ -77,15 +90,15 @@
     data = data or {}
     data.update(kwargs)
     if not data:
         raise AttributeError("Data must be provided")
     redis_data = {
         upperfy(key): unparse_conf_data(value) for key, value in data.items()
     }
-    client.hmset(holder.upper(), redis_data)
+    client.hset(holder.upper(), mapping=redis_data)
     load(obj)
 
 
 def delete(obj, key=None):
     """
     Delete a single key if specified, or all env if key is none
     :param obj: settings object
```

### Comparing `dynaconf-3.1.9/dynaconf/loaders/vault_loader.py` & `dynaconf-3.2.0/dynaconf/loaders/vault_loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # docker run -e 'VAULT_DEV_ROOT_TOKEN_ID=myroot' -p 8200:8200 vault
 # pip install hvac
+from __future__ import annotations
+
+from dynaconf.loaders.base import SourceMetadata
 from dynaconf.utils import build_env_list
 from dynaconf.utils.parse_conf import parse_conf_data
 
 try:
     import boto3
 except ImportError:
     boto3 = None
 
 try:
     from hvac import Client
-    from hvac.exceptions import InvalidPath
+    from hvac.exceptions import InvalidPath, Forbidden
 except ImportError:
     raise ImportError(
         "vault package is not installed in your environment. "
         "`pip install dynaconf[vault]` or disable the vault loader with "
         "export VAULT_ENABLED_FOR_DYNACONF=false"
     )
 
@@ -27,20 +30,26 @@
 
 
 def get_client(obj):
     client = Client(
         **{k: v for k, v in obj.VAULT_FOR_DYNACONF.items() if v is not None}
     )
     if obj.VAULT_ROLE_ID_FOR_DYNACONF is not None:
-        client.auth_approle(
+        client.auth.approle.login(
             role_id=obj.VAULT_ROLE_ID_FOR_DYNACONF,
             secret_id=obj.get("VAULT_SECRET_ID_FOR_DYNACONF"),
         )
     elif obj.VAULT_ROOT_TOKEN_FOR_DYNACONF is not None:
         client.token = obj.VAULT_ROOT_TOKEN_FOR_DYNACONF
+    elif obj.VAULT_USERNAME_FOR_DYNACONF is not None:
+        client.auth.userpass.login(
+            username=obj.VAULT_USERNAME_FOR_DYNACONF,
+            password=obj.VAULT_PASSWORD_FOR_DYNACONF,
+        )
+
     elif obj.VAULT_AUTH_WITH_IAM_FOR_DYNACONF:
         if boto3 is None:
             raise ImportError(
                 "boto3 package is not installed in your environment. "
                 "`pip install boto3` or disable the VAULT_AUTH_WITH_IAM"
             )
 
@@ -52,19 +61,19 @@
             credentials.token,
             role=obj.VAULT_AUTH_ROLE_FOR_DYNACONF,
         )
     assert client.is_authenticated(), (
         "Vault authentication error: is VAULT_TOKEN_FOR_DYNACONF or "
         "VAULT_ROLE_ID_FOR_DYNACONF defined?"
     )
-    client.kv.default_kv_version = obj.VAULT_KV_VERSION_FOR_DYNACONF
+    client.secrets.kv.default_kv_version = obj.VAULT_KV_VERSION_FOR_DYNACONF
     return client
 
 
-def load(obj, env=None, silent=None, key=None):
+def load(obj, env=None, silent=None, key=None, validate=False):
     """Reads and loads in to "settings" a single key or all keys from vault
 
     :param obj: the settings instance
     :param env: settings env default='DYNACONF'
     :param silent: if errors should raise
     :param key: if defined load a single key, else load all in env
     :return: None
@@ -80,56 +89,74 @@
             dirs = client.secrets.kv.v1.list_secrets(
                 path=obj.VAULT_PATH_FOR_DYNACONF,
                 mount_point=obj.VAULT_MOUNT_POINT_FOR_DYNACONF,
             )["data"]["keys"]
     except InvalidPath:
         # The given path is not a directory
         dirs = []
+    except Forbidden:
+        # The given token does not have permission to list the given path
+        dirs = []
     # First look for secrets into environments less store
     if not obj.ENVIRONMENTS_FOR_DYNACONF:
         # By adding '', dynaconf will now read secrets from environments-less
         # store which are not written by `dynaconf write` to Vault store
         env_list = [obj.MAIN_ENV_FOR_DYNACONF.lower(), ""]
     # Finally, look for secret into all the environments
     else:
         env_list = dirs + build_env_list(obj, env)
     for env in env_list:
         path = "/".join([obj.VAULT_PATH_FOR_DYNACONF, env])
         try:
             if obj.VAULT_KV_VERSION_FOR_DYNACONF == 2:
                 data = client.secrets.kv.v2.read_secret_version(
-                    path, mount_point=obj.VAULT_MOUNT_POINT_FOR_DYNACONF
+                    path,
+                    mount_point=obj.VAULT_MOUNT_POINT_FOR_DYNACONF,
+                    raise_on_deleted_version=True,  # keep default behavior
                 )
             else:
                 data = client.secrets.kv.read_secret(
                     "data/" + path,
                     mount_point=obj.VAULT_MOUNT_POINT_FOR_DYNACONF,
                 )
         except InvalidPath:
             # If the path doesn't exist, ignore it and set data to None
             data = None
+        except Forbidden:
+            data = None
         if data:
             # There seems to be a data dict within a data dict,
             # extract the inner data
             data = data.get("data", {}).get("data", {})
         try:
+            source_metadata = SourceMetadata(IDENTIFIER, "unique", env)
             if (
                 obj.VAULT_KV_VERSION_FOR_DYNACONF == 2
                 and obj.ENVIRONMENTS_FOR_DYNACONF
                 and data
             ):
                 data = data.get("data", {})
             if data and key:
                 value = parse_conf_data(
                     data.get(key), tomlfy=True, box_settings=obj
                 )
                 if value:
-                    obj.set(key, value)
+                    obj.set(
+                        key,
+                        value,
+                        validate=validate,
+                        loader_identifier=source_metadata,
+                    )
             elif data:
-                obj.update(data, loader_identifier=IDENTIFIER, tomlfy=True)
+                obj.update(
+                    data,
+                    loader_identifier=source_metadata,
+                    tomlfy=True,
+                    validate=validate,
+                )
         except Exception:
             if silent:
                 return False
             raise
 
 
 def write(obj, data=None, **kwargs):
```

### Comparing `dynaconf-3.1.9/dynaconf/loaders/yaml_loader.py` & `dynaconf-3.2.0/dynaconf/loaders/yaml_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,12 @@
-import io
+from __future__ import annotations
+
+import sys
 from pathlib import Path
+from typing import TextIO
 from warnings import warn
 
 from dynaconf import default_settings
 from dynaconf.constants import YAML_EXTENSIONS
 from dynaconf.loaders.base import BaseLoader
 from dynaconf.utils import object_merge
 from dynaconf.utils.parse_conf import try_to_encode
@@ -13,15 +16,15 @@
 yaml.SafeDumper.yaml_representers[
     None
 ] = lambda self, data: yaml.representer.SafeRepresenter.represent_str(
     self, try_to_encode(data)
 )
 
 
-def load(obj, env=None, silent=True, key=None, filename=None):
+def load(obj, env=None, silent=True, key=None, filename=None, validate=False):
     """
     Reads and loads in to "obj" a single key or all keys from source file.
 
     :param obj: the settings instance
     :param env: settings current env default='development'
     :param silent: if errors should raise
     :param key: if defined load a single key, else load all in env
@@ -44,37 +47,39 @@
     loader = BaseLoader(
         obj=obj,
         env=env,
         identifier="yaml",
         extensions=YAML_EXTENSIONS,
         file_reader=yaml_reader,
         string_reader=yaml_reader,
+        validate=validate,
     )
     loader.load(
         filename=filename,
         key=key,
         silent=silent,
     )
 
 
 def write(settings_path, settings_data, merge=True):
     """Write data to a settings file.
 
     :param settings_path: the filepath
     :param settings_data: a dictionary with data
     :param merge: boolean if existing file should be merged with new data
+    :param stdout: boolean if should output to stdout instead of file
     """
     settings_path = Path(settings_path)
     if settings_path.exists() and merge:  # pragma: no cover
-        with io.open(
+        with open(
             str(settings_path), encoding=default_settings.ENCODING_FOR_DYNACONF
         ) as open_file:
             object_merge(yaml.safe_load(open_file), settings_data)
 
-    with io.open(
+    with open(
         str(settings_path),
         "w",
         encoding=default_settings.ENCODING_FOR_DYNACONF,
     ) as open_file:
         yaml.dump(
             settings_data,
             open_file,
```

### Comparing `dynaconf-3.1.9/dynaconf/strategies/filtering.py` & `dynaconf-3.2.0/dynaconf/strategies/filtering.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from __future__ import annotations
+
 from dynaconf.utils import upperfy
 
 
 class PrefixFilter:
     def __init__(self, prefix):
         if not isinstance(prefix, str):
             raise TypeError("`SETTINGS_FILE_PREFIX` must be str")
-        self.prefix = "{}_".format(upperfy(prefix))
+        self.prefix = f"{upperfy(prefix)}_"
 
     def __call__(self, data):
         """Filter incoming data by prefix"""
         len_prefix = len(self.prefix)
         return {
             upperfy(key[len_prefix:]): value
             for key, value in data.items()
```

### Comparing `dynaconf-3.1.9/dynaconf/utils/__init__.py` & `dynaconf-3.2.0/dynaconf/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 from __future__ import annotations
 
 import os
 import warnings
 from collections import defaultdict
 from json import JSONDecoder
 from typing import Any
-from typing import Dict
 from typing import Iterator
-from typing import List
-from typing import Optional
-from typing import Tuple
 from typing import TYPE_CHECKING
-from typing import Union
+from typing import TypeVar
 
 
 if TYPE_CHECKING:  # pragma: no cover
     from dynaconf.utils.boxing import DynaBox
     from dynaconf.base import LazySettings, Settings
 
 
@@ -30,15 +26,15 @@
 
 if os.name == "nt":  # pragma: no cover
     # windows can't handle the above charmap
     BANNER = "DYNACONF"
 
 
 def object_merge(
-    old: Any, new: Any, unique: bool = False, full_path: List[str] = None
+    old: Any, new: Any, unique: bool = False, full_path: list[str] = None
 ) -> Any:
     """
     Recursively merge two data structures, new is mutated in-place.
 
     :param old: The existing data.
     :param new: The new data to get old values merged in to.
     :param unique: When set to True existing list items are not set.
@@ -47,75 +43,99 @@
     if full_path is None:
         full_path = []
     if old == new or old is None or new is None:
         # Nothing to merge
         return new
 
     if isinstance(old, list) and isinstance(new, list):
+
+        # 726: allow local_merge to override global merge on lists
+        if "dynaconf_merge_unique" in new:
+            new.remove("dynaconf_merge_unique")
+            unique = True
+
         for item in old[::-1]:
             if unique and item in new:
                 continue
             new.insert(0, item)
 
     if isinstance(old, dict) and isinstance(new, dict):
-        existing_value = recursive_get(old, full_path)  # doesnt handle None
+        existing_value = recursive_get(old, full_path)  # doesn't handle None
         # Need to make every `None` on `_store` to be an wrapped `LazyNone`
 
-        for key, value in old.items():
+        # data coming from source, in `new` can be mix case: KEY4|key4|Key4
+        # data existing on `old` object has the correct case: key4|KEY4|Key4
+        # So we need to ensure that new keys matches the existing keys
+        for new_key in list(new.keys()):
+            correct_case_key = find_the_correct_casing(new_key, old)
+            if correct_case_key:
+                new[correct_case_key] = new.pop(new_key)
+
+        def safe_items(data):
+            """
+            Get items from DynaBox without triggering recursive evaluation
+            """
+            if data.__class__.__name__ == "DynaBox":
+                return data._safe_items()
+            else:
+                return data.items()
+
+        for old_key, value in safe_items(old):
 
+            # This is for when the dict exists internally
+            # but the new value on the end of full path is the same
             if (
                 existing_value is not None
-                and key.lower() == full_path[-1].lower()
+                and old_key.lower() == full_path[-1].lower()
                 and existing_value is value
             ):
                 # Here Be The Dragons
                 # This comparison needs to be smarter
                 continue
 
-            if key not in new:
-                new[key] = value
+            if old_key not in new:
+                new[old_key] = value
             else:
                 object_merge(
                     value,
-                    new[key],
+                    new[old_key],
                     full_path=full_path[1:] if full_path else None,
                 )
 
         handle_metavalues(old, new)
 
     return new
 
 
 def recursive_get(
-    obj: Union[DynaBox, Dict[str, int], Dict[str, Union[str, int]]],
-    names: Optional[List[str]],
+    obj: DynaBox | dict[str, int] | dict[str, str | int],
+    names: list[str] | None,
 ) -> Any:
     """Given a dot accessible object and a list of names `foo.bar.zaz`
-    gets recursivelly all names one by one obj.foo.bar.zaz.
+    gets recursively all names one by one obj.foo.bar.zaz.
     """
     if not names:
         return
-    head, tail = names[0], names[1:]
+    head, *tail = names
     result = getattr(obj, head, None)
     if not tail:
         return result
     return recursive_get(result, tail)
 
 
 def handle_metavalues(
-    old: Union[DynaBox, Dict[str, int], Dict[str, Union[str, int]]], new: Any
+    old: DynaBox | dict[str, int] | dict[str, str | int], new: Any
 ) -> None:
     """Cleanup of MetaValues on new dict"""
 
     for key in list(new.keys()):
 
         # MetaValue instances
         if getattr(new[key], "_dynaconf_reset", False):  # pragma: no cover
             # a Reset on `new` triggers reasign of existing data
-            # @reset is deprecated on v3.0.0
             new[key] = new[key].unwrap()
         elif getattr(new[key], "_dynaconf_del", False):
             # a Del on `new` triggers deletion of existing data
             new.pop(key, None)
             old.pop(key, None)
         elif getattr(new[key], "_dynaconf_merge", False):
             # a Merge on `new` triggers merge with existing data
@@ -174,15 +194,15 @@
         self._defaults = {}
         self.environ = os.environ
         self.SETTINGS_MODULE = None
         self.filter_strategy = kwargs.get("filter_strategy", None)
         self._not_installed_warnings = []
         self._validate_only = kwargs.pop("validate_only", None)
         self._validate_exclude = kwargs.pop("validate_exclude", None)
-        super(DynaconfDict, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     def set(self, key: str, value: str, *args, **kwargs) -> None:
         self[key] = value
 
     @staticmethod
     def get_environ(key, default=None):  # pragma: no cover
         return os.environ.get(key, default)
@@ -204,15 +224,15 @@
     "DYNACONF_SILENT_ERRORS": "SILENT_ERRORS_FOR_DYNACONF",
     "DYNACONF_ALWAYS_FRESH_VARS": "FRESH_VARS_FOR_DYNACONF",
     "BASE_NAMESPACE_FOR_DYNACONF": "DEFAULT_ENV_FOR_DYNACONF",
     "GLOBAL_ENV_FOR_DYNACONF": "ENVVAR_PREFIX_FOR_DYNACONF",
 }
 
 
-def compat_kwargs(kwargs: Dict[str, Any]) -> None:
+def compat_kwargs(kwargs: dict[str, Any]) -> None:
     """To keep backwards compat change the kwargs to new names"""
     warn_deprecations(kwargs)
     for old, new in RENAMED_VARS.items():
         if old in kwargs:
             kwargs[new] = kwargs[old]
             # update cross references
             for c_old, c_new in RENAMED_VARS.items():
@@ -226,15 +246,15 @@
     situations where `None` is a valid value.
     """
 
     def __bool__(self) -> bool:
         """Respond to boolean duck-typing."""
         return False
 
-    def __eq__(self, other: Union[DynaBox, Missing]) -> bool:
+    def __eq__(self, other: DynaBox | Missing) -> bool:
         """Equality check for a singleton."""
 
         return isinstance(other, self.__class__)
 
     # Ensure compatibility with Python 2.x
     __nonzero__ = __bool__
 
@@ -245,15 +265,15 @@
         """
         return "<dynaconf.missing>"
 
 
 missing = Missing()
 
 
-def deduplicate(list_object: List[str]) -> List[str]:
+def deduplicate(list_object: list[str]) -> list[str]:
     """Rebuild `list_object` removing duplicated and keeping order"""
     new = []
     for item in list_object:
         if item not in new:
             new.append(item)
     return new
 
@@ -265,40 +285,41 @@
                 f"You are using {old} which is a deprecated settings "
                 f"replace it with {new}",
                 DeprecationWarning,
             )
 
 
 def trimmed_split(
-    s: str, seps: Union[str, Tuple[str, str]] = (";", ",")
-) -> List[str]:
+    s: str, seps: str | tuple[str, str] = (";", ",")
+) -> list[str]:
     """Given a string s, split is by one of one of the seps."""
     for sep in seps:
         if sep not in s:
             continue
         data = [item.strip() for item in s.strip().split(sep)]
         return data
     return [s]  # raw un-splitted
 
 
-def ensure_a_list(data: Any) -> Union[List[int], List[str]]:
+T = TypeVar("T")
+
+
+def ensure_a_list(data: T | list[T]) -> list[T]:
     """Ensure data is a list or wrap it in a list"""
     if not data:
         return []
     if isinstance(data, (list, tuple, set)):
         return list(data)
     if isinstance(data, str):
         data = trimmed_split(data)  # settings.toml,other.yaml
         return data
     return [data]
 
 
-def build_env_list(
-    obj: Union[Settings, LazySettings], env: Optional[str]
-) -> List[str]:
+def build_env_list(obj: Settings | LazySettings, env: str | None) -> list[str]:
     """Build env list for loaders to iterate.
 
     Arguments:
         obj {LazySettings} -- A Dynaconf settings instance
         env {str} -- The current env to be loaded
 
     Returns:
@@ -351,15 +372,15 @@
     key = str(key)
     if "__" in key:
         parts = key.split("__")
         return "__".join([parts[0].upper()] + parts[1:])
     return key.upper()
 
 
-def multi_replace(text: str, patterns: Dict[str, str]) -> str:
+def multi_replace(text: str, patterns: dict[str, str]) -> str:
     """Replaces multiple pairs in a string
 
     Arguments:
         text {str} -- A "string text"
         patterns {dict} -- A dict of {"old text": "new text"}
 
     Returns:
@@ -368,15 +389,15 @@
     for old, new in patterns.items():
         text = text.replace(old, new)
     return text
 
 
 def extract_json_objects(
     text: str, decoder: JSONDecoder = JSONDecoder()
-) -> Iterator[Dict[str, Union[int, Dict[Any, Any]]]]:
+) -> Iterator[dict[str, int | dict[Any, Any]]]:
     """Find JSON objects in text, and yield the decoded JSON data
 
     Does not attempt to look for JSON arrays, text, or other JSON types outside
     of a parent JSON object.
 
     """
     pos = 0
@@ -389,30 +410,36 @@
             yield result
             pos = match + index
         except ValueError:
             pos = match + 1
 
 
 def recursively_evaluate_lazy_format(
-    value: Any, settings: Union[Settings, LazySettings]
+    value: Any, settings: Settings | LazySettings
 ) -> Any:
     """Given a value as a data structure, traverse all its members
     to find Lazy values and evaluate it.
 
     For example: Evaluate values inside lists and dicts
     """
+    return _recursively_evaluate_lazy_format(value, settings)
+
 
+def _recursively_evaluate_lazy_format(
+    value: Any, settings: Settings | LazySettings
+) -> Any:
+    """Recursive implementation. Separate for easier debugging."""
     if getattr(value, "_dynaconf_lazy_format", None):
         value = value(settings)
 
     if isinstance(value, list):
         # Keep the original type, can be a BoxList
         value = value.__class__(
             [
-                recursively_evaluate_lazy_format(item, settings)
+                _recursively_evaluate_lazy_format(item, settings)
                 for item in value
             ]
         )
 
     return value
 
 
@@ -427,7 +454,27 @@
     b = t.__bases__
     if len(b) != 1 or b[0] != tuple:
         return False
     f = getattr(t, "_fields", None)
     if not isinstance(f, tuple):
         return False
     return all(type(n) == str for n in f)
+
+
+def find_the_correct_casing(key: str, data: dict[str, Any]) -> str | None:
+    """Given a key, find the proper casing in data
+
+    Arguments:
+        key {str} -- A key to be searched in data
+        data {dict} -- A dict to be searched
+
+    Returns:
+        str -- The proper casing of the key in data
+    """
+    if key in data:
+        return key
+    for k in data.keys():
+        if k.lower() == key.lower():
+            return k
+        if k.replace(" ", "_").lower() == key.lower():
+            return k
+    return None
```

### Comparing `dynaconf-3.1.9/dynaconf/utils/boxing.py` & `dynaconf-3.2.0/dynaconf/utils/boxing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+from __future__ import annotations
+
 import inspect
 from functools import wraps
 
+from dynaconf.utils import find_the_correct_casing
 from dynaconf.utils import recursively_evaluate_lazy_format
-from dynaconf.utils import upperfy
 from dynaconf.utils.functional import empty
 from dynaconf.vendor.box import Box
 
 
 def evaluate_lazy_format(f):
     """Marks a method on Dynabox instance to
     lazily evaluate LazyFormat objects upon access."""
 
     @wraps(f)
     def evaluate(dynabox, item, *args, **kwargs):
+        if dynabox._box_config.get("_bypass_evaluation") is True:
+            return f(dynabox, item, *args, **kwargs)
+
         value = f(dynabox, item, *args, **kwargs)
         settings = dynabox._box_config["box_settings"]
 
         if getattr(value, "_dynaconf_lazy_format", None):
             dynabox._box_config[
                 f"raw_{item.lower()}"
             ] = f"@{value.formatter.token} {value.value}"
@@ -29,55 +34,52 @@
 class DynaBox(Box):
     """Specialized Box for dynaconf
     it allows items/attrs to be found both in upper or lower case"""
 
     @evaluate_lazy_format
     def __getattr__(self, item, *args, **kwargs):
         try:
-            return super(DynaBox, self).__getattr__(item, *args, **kwargs)
+            return super().__getattr__(item, *args, **kwargs)
         except (AttributeError, KeyError):
-            n_item = item.lower() if item.isupper() else upperfy(item)
-            return super(DynaBox, self).__getattr__(n_item, *args, **kwargs)
+            n_item = find_the_correct_casing(item, self) or item
+            return super().__getattr__(n_item, *args, **kwargs)
 
     @evaluate_lazy_format
     def __getitem__(self, item, *args, **kwargs):
         try:
-            return super(DynaBox, self).__getitem__(item, *args, **kwargs)
+            return super().__getitem__(item, *args, **kwargs)
+        except (AttributeError, KeyError):
+            n_item = find_the_correct_casing(item, self) or item
+            return super().__getitem__(n_item, *args, **kwargs)
+
+    def _safe_get(self, item, *args, **kwargs):
+        """Get item bypassing recursive evaluation"""
+        try:
+            return super().__getitem__(item, *args, **kwargs)
         except (AttributeError, KeyError):
-            n_item = item.lower() if item.isupper() else upperfy(item)
-            return super(DynaBox, self).__getitem__(n_item, *args, **kwargs)
+            n_item = find_the_correct_casing(item, self) or item
+            return super().__getitem__(n_item, *args, **kwargs)
 
     def __copy__(self):
         return self.__class__(
             super(Box, self).copy(),
             box_settings=self._box_config.get("box_settings"),
         )
 
     def copy(self):
         return self.__class__(
             super(Box, self).copy(),
             box_settings=self._box_config.get("box_settings"),
         )
 
-    def _case_insensitive_get(self, item, default=None):
-        """adds a bit of overhead but allows case insensitive get
-        See issue: #486
-        """
-        lower_self = {k.casefold(): v for k, v in self.items()}
-        return lower_self.get(item.casefold(), default)
-
     @evaluate_lazy_format
     def get(self, item, default=None, *args, **kwargs):
-        if item not in self:  # toggle case
-            item = item.lower() if item.isupper() else upperfy(item)
-        value = super(DynaBox, self).get(item, empty, *args, **kwargs)
-        if value is empty:
-            # see Issue: #486
-            return self._case_insensitive_get(item, default)
-        return value
+        n_item = find_the_correct_casing(item, self) or item
+        value = super().get(n_item, empty, *args, **kwargs)
+        return value if value is not empty else default
 
     def __dir__(self):
         keys = list(self.keys())
         reserved = [
             item[0]
             for item in inspect.getmembers(DynaBox)
             if not item[0].startswith("__")
```

### Comparing `dynaconf-3.1.9/dynaconf/utils/files.py` & `dynaconf-3.2.0/dynaconf/utils/files.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+from __future__ import annotations
+
 import inspect
-import io
 import os
 
 from dynaconf.utils import deduplicate
 
 
 def _walk_to_root(path, break_at=None):
     """
     Directories starting from the given directory up to the root or break_at
     """
     if not os.path.exists(path):  # pragma: no cover
-        raise IOError("Starting path not found")
+        raise OSError("Starting path not found")
 
     if os.path.isfile(path):  # pragma: no cover
         path = os.path.dirname(path)
 
     last_dir = None
     current_dir = os.path.abspath(path)
     paths = []
@@ -38,26 +39,29 @@
     This function will build a `search_tree` based on:
 
     - Project_root if specified
     - Invoked script location and its parents until root
     - Current working directory
 
     For each path in the `search_tree` it will also look for an
-    aditional `./config` folder.
+    additional `./config` folder.
     """
-    search_tree = []
-    work_dir = os.getcwd()
-    skip_files = skip_files or []
-
     # If filename is an absolute path and exists, just return it
     # if the absolute path does not exist, return empty string so
     # that it can be joined and avoid IoError
     if os.path.isabs(filename):
         return filename if os.path.exists(filename) else ""
 
+    search_tree = []
+    try:
+        work_dir = os.getcwd()
+    except FileNotFoundError:  # pragma: no cover
+        return ""
+    skip_files = skip_files or []
+
     if project_root is not None:
         search_tree.extend(_walk_to_root(project_root, break_at=work_dir))
 
     script_dir = os.path.dirname(os.path.abspath(inspect.stack()[-1].filename))
 
     # Path to invoked script and recursively to root with its ./config dirs
     search_tree.extend(_walk_to_root(script_dir))
@@ -80,15 +84,15 @@
 
     # return empty string if not found so it can still be joined in os.path
     return ""
 
 
 def read_file(path, **kwargs):
     content = ""
-    with io.open(path, **kwargs) as open_file:
+    with open(path, **kwargs) as open_file:
         content = open_file.read().strip()
     return content
 
 
 def get_local_filename(filename):
     """Takes a filename like `settings.toml` and returns `settings.local.toml`
```

### Comparing `dynaconf-3.1.9/dynaconf/utils/functional.py` & `dynaconf-3.2.0/dynaconf/utils/functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import copy
 import operator
 
 
 class Empty:
     def __str__(self):
         return "EMPTY"
```

### Comparing `dynaconf-3.1.9/dynaconf/utils/parse_conf.py` & `dynaconf-3.2.0/dynaconf/utils/parse_conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+from __future__ import annotations
+
 import json
 import os
 import re
 import warnings
 from functools import wraps
 
 from dynaconf.utils import extract_json_objects
 from dynaconf.utils import isnamedtupleinstance
 from dynaconf.utils import multi_replace
 from dynaconf.utils import recursively_evaluate_lazy_format
 from dynaconf.utils.boxing import DynaBox
 from dynaconf.utils.functional import empty
 from dynaconf.vendor import toml
+from dynaconf.vendor import tomllib
 
 try:
     from jinja2 import Environment
 
     jinja_env = Environment()
     for p_method in ("abspath", "realpath", "relpath", "dirname", "basename"):
         jinja_env.filters[p_method] = getattr(os.path, p_method)
@@ -260,29 +263,62 @@
     "@comment": lambda value: None,
     "@null": lambda value: None,
     "@none": lambda value: None,
     "@empty": lambda value: empty,
 }
 
 
-def get_converter(converter_key, value, box_settings):
+def apply_converter(converter_key, value, box_settings):
+    """
+    Get converter and apply it to @value.
+
+    Lazy converters will return Lazy objects for later evaluation.
+    """
     converter = converters[converter_key]
     try:
         converted_value = converter(value, box_settings=box_settings)
     except TypeError:
         converted_value = converter(value)
     return converted_value
 
 
+def add_converter(converter_key, func):
+    """Adds a new converter to the converters dict"""
+    if not converter_key.startswith("@"):
+        converter_key = f"@{converter_key}"
+
+    converters[converter_key] = wraps(func)(
+        lambda value: value.set_casting(func)
+        if isinstance(value, Lazy)
+        else Lazy(
+            value,
+            casting=func,
+            formatter=BaseFormatter(lambda x, **_: x, converter_key),
+        )
+    )
+
+
 def parse_with_toml(data):
     """Uses TOML syntax to parse data"""
-    try:
-        return toml.loads(f"key={data}")["key"]
-    except (toml.TomlDecodeError, KeyError):
-        return data
+    try:  # try tomllib first
+        try:
+            return tomllib.loads(f"key={data}")["key"]
+        except (tomllib.TOMLDecodeError, KeyError):
+            return data
+    except UnicodeDecodeError:  # pragma: no cover
+        # fallback to toml (TBR in 4.0.0)
+        try:
+            return toml.loads(f"key={data}")["key"]
+        except (toml.TomlDecodeError, KeyError):
+            return data
+        warnings.warn(
+            "TOML files should have only UTF-8 encoded characters. "
+            "starting on 4.0.0 dynaconf will stop allowing invalid chars.",
+            DeprecationWarning,
+        )
 
 
 def _parse_conf_data(data, tomlfy=False, box_settings=None):
     """
     @int @bool @float @json (for lists and dicts)
     strings does not need converters
 
@@ -292,81 +328,92 @@
     export DYNACONF_PAGINATION_PER_PAGE='@int 20'
     export DYNACONF_MONGODB_SETTINGS='@json {"DB": "quokka_db"}'
     export DYNACONF_ALLOWED_EXTENSIONS='@json ["jpg", "png"]'
     """
     # not enforced to not break backwards compatibility with custom loaders
     box_settings = box_settings or {}
 
-    cast_toggler = os.environ.get("AUTO_CAST_FOR_DYNACONF", "true").lower()
-    castenabled = cast_toggler not in false_values
+    castenabled = box_settings.get("AUTO_CAST_FOR_DYNACONF", empty)
+    if castenabled is empty:
+        castenabled = (
+            os.environ.get("AUTO_CAST_FOR_DYNACONF", "true").lower()
+            not in false_values
+        )
 
     if (
         castenabled
         and data
         and isinstance(data, str)
         and data.startswith(tuple(converters.keys()))
     ):
         # Check combination token is used
         comb_token = re.match(
-            r"^@(str|int|float|bool|json) @(jinja|format)", data
+            f"^({'|'.join(converters.keys())}) @(jinja|format)",
+            data,
         )
         if comb_token:
             tokens = comb_token.group(0)
             converter_key_list = tokens.split(" ")
             value = data.replace(tokens, "").strip()
         else:
             parts = data.partition(" ")
             converter_key_list = [parts[0]]
             value = parts[-1]
 
         # Parse the converters iteratively
         for converter_key in converter_key_list[::-1]:
-            value = get_converter(converter_key, value, box_settings)
+            value = apply_converter(converter_key, value, box_settings)
     else:
         value = parse_with_toml(data) if tomlfy else data
 
     if isinstance(value, dict):
         value = DynaBox(value, box_settings=box_settings)
 
     return value
 
 
 def parse_conf_data(data, tomlfy=False, box_settings=None):
+    """
+    Apply parsing tokens recursively and return transformed data.
 
-    # fix for https://github.com/rochacbruno/dynaconf/issues/595
+    Strings with lazy parser (e.g, @format) will become Lazy objects.
+    """
+
+    # fix for https://github.com/dynaconf/dynaconf/issues/595
     if isnamedtupleinstance(data):
         return data
 
     # not enforced to not break backwards compatibility with custom loaders
     box_settings = box_settings or {}
 
     if isinstance(data, (tuple, list)):
-
         # recursively parse each sequence item
         return [
             parse_conf_data(item, tomlfy=tomlfy, box_settings=box_settings)
             for item in data
         ]
 
-    if isinstance(data, (dict, DynaBox)):
+    if isinstance(data, DynaBox):
+        # recursively parse inner dict items
+        _parsed = DynaBox({}, box_settings=box_settings)
+        for k, v in data._safe_items():
+            _parsed[str(k)] = parse_conf_data(
+                v, tomlfy=tomlfy, box_settings=box_settings
+            )
+        return _parsed
+
+    if isinstance(data, dict):
         # recursively parse inner dict items
         _parsed = {}
         for k, v in data.items():
-            _parsed[k] = parse_conf_data(
+            _parsed[str(k)] = parse_conf_data(
                 v, tomlfy=tomlfy, box_settings=box_settings
             )
         return _parsed
 
-    if (
-        isinstance(data, str)
-        and data.startswith(("+", "-"))
-        and data[1:].isdigit()
-    ):
-        return data
-
     # return parsed string value
     return _parse_conf_data(data, tomlfy=tomlfy, box_settings=box_settings)
 
 
 def unparse_conf_data(value):
     if isinstance(value, bool):
         return f"@bool {value}"
```

### Comparing `dynaconf-3.1.9/dynaconf/validator.py` & `dynaconf-3.2.0/dynaconf/validator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from itertools import chain
 from types import MappingProxyType
 from typing import Any
 from typing import Callable
-from typing import Dict
-from typing import List
-from typing import Optional
 from typing import Sequence
-from typing import Union
+from typing import TYPE_CHECKING
 
 from dynaconf import validator_conditions
 from dynaconf.utils import ensure_a_list
 from dynaconf.utils.functional import empty
 
+if TYPE_CHECKING:
+    from dynaconf.base import LazySettings, Settings
 
 EQUALITY_ATTRS = (
     "names",
     "must_exist",
     "when",
     "condition",
     "operations",
@@ -101,24 +100,24 @@
             "combined": "combined validators failed {errors}",
         }
     )
 
     def __init__(
         self,
         *names: str,
-        must_exist: Optional[bool] = None,
-        required: Optional[bool] = None,  # alias for `must_exist`
-        condition: Optional[Callable[[Any], bool]] = None,
-        when: Optional[Validator] = None,
-        env: Optional[Union[str, Sequence[str]]] = None,
-        messages: Optional[Dict[str, str]] = None,
-        cast: Optional[Callable[[Any], Any]] = None,
-        default: Optional[Union[Any, Callable[[Any, Validator], Any]]] = empty,
-        description: Optional[str] = None,
-        apply_default_on_none: Optional[bool] = False,
+        must_exist: bool | None = None,
+        required: bool | None = None,  # alias for `must_exist`
+        condition: Callable[[Any], bool] | None = None,
+        when: Validator | None = None,
+        env: str | Sequence[str] | None = None,
+        messages: dict[str, str] | None = None,
+        cast: Callable[[Any], Any] | None = None,
+        default: Any | Callable[[Any, Validator], Any] | None = empty,
+        description: str | None = None,
+        apply_default_on_none: bool | None = False,
         **operations: Any,
     ) -> None:
         # Copy immutable MappingProxyType as a mutable dict
         self.messages = dict(self.default_messages)
         if messages:
             self.messages.update(messages)
 
@@ -132,17 +131,20 @@
         self.must_exist = must_exist if must_exist is not None else required
         self.condition = condition
         self.when = when
         self.cast = cast or (lambda value: value)
         self.operations = operations
         self.default = default
         self.description = description
-        self.envs: Optional[Sequence[str]] = None
+        self.envs: Sequence[str] | None = None
         self.apply_default_on_none = apply_default_on_none
 
+        # See #585
+        self.is_type_of = operations.get("is_type_of")
+
         if isinstance(env, str):
             self.envs = [env]
         elif isinstance(env, (list, tuple)):
             self.envs = env
 
     def __or__(self, other: Validator) -> CombinedValidator:
         return OrValidator(self, other, description=self.description)
@@ -164,17 +166,17 @@
         if all(identical_attrs):
             return True
 
         return False
 
     def validate(
         self,
-        settings: Any,
-        only: Optional[Union[str, Sequence]] = None,
-        exclude: Optional[Union[str, Sequence]] = None,
+        settings: Settings,
+        only: str | Sequence | None = None,
+        exclude: str | Sequence | None = None,
         only_current_env: bool = False,
     ) -> None:
         """Raise ValidationError if invalid"""
         # If only or exclude are not set, this value always passes startswith
         only = ensure_a_list(only or [""])
         if only and not isinstance(only[0], str):
             raise ValueError("'only' must be a string or list of strings.")
@@ -213,24 +215,25 @@
         ):
             self._validate_items(
                 settings, settings.current_env, only=only, exclude=exclude
             )
             return
 
         for env in self.envs:
-            self._validate_items(
-                settings.from_env(env), only=only, exclude=exclude
-            )
+            env_settings: Settings = settings.from_env(env)
+            self._validate_items(env_settings, only=only, exclude=exclude)
+            # merge source metadata into original settings for history inspect
+            settings._loaded_by_loaders.update(env_settings._loaded_by_loaders)
 
     def _validate_items(
         self,
-        settings: Any,
-        env: Optional[str] = None,
-        only: Optional[Union[str, Sequence]] = None,
-        exclude: Optional[Union[str, Sequence]] = None,
+        settings: Settings,
+        env: str | None = None,
+        only: str | Sequence | None = None,
+        exclude: str | Sequence | None = None,
     ) -> None:
         env = env or settings.current_env
         for name in self.names:
             # Skip if only is set and name isn't in the only list
             if only and not any(name.startswith(sub) for sub in only):
                 continue
 
@@ -243,20 +246,33 @@
                     self.default(settings, self)
                     if callable(self.default)
                     else self.default
                 )
             else:
                 default_value = empty
 
-            value = self.cast(
-                settings.setdefault(
-                    name,
-                    default_value,
-                    apply_default_on_none=self.apply_default_on_none,
-                )
+            # THIS IS A FIX FOR #585 in contrast with #799
+            # toml considers signed strings "+-1" as integers
+            # however existing users are passing strings
+            # to default on validator (see #585)
+            # The solution we added on #667 introduced a new problem
+            # This fix here makes it to work for both cases.
+            if (
+                isinstance(default_value, str)
+                and default_value.startswith(("+", "-"))
+                and self.is_type_of is str
+            ):
+                # avoid TOML from parsing "+-1" as integer
+                default_value = f"'{default_value}'"
+
+            value = settings.setdefault(
+                name,
+                default_value,
+                apply_default_on_none=self.apply_default_on_none,
+                env=env,
             )
 
             # is name required but not exists?
             if self.must_exist is True and value is empty:
                 _message = self.messages["must_exist_true"].format(
                     name=name, env=env
                 )
@@ -267,29 +283,57 @@
                     name=name, env=env
                 )
                 raise ValidationError(_message, details=[(self, _message)])
 
             if self.must_exist in (False, None) and value is empty:
                 continue
 
+            # value or default value already set
+            # by settings.setdefault above
+            # however we need to cast it
+            # so we call .set again
+            value = self.cast(settings.get(name))
+            settings.set(name, value, validate=False)
+
             # is there a callable condition?
             if self.condition is not None:
                 if not self.condition(value):
                     _message = self.messages["condition"].format(
                         name=name,
                         function=self.condition.__name__,
                         value=value,
                         env=env,
                     )
                     raise ValidationError(_message, details=[(self, _message)])
 
             # operations
             for op_name, op_value in self.operations.items():
                 op_function = getattr(validator_conditions, op_name)
-                if not op_function(value, op_value):
+                op_succeeded = False
+
+                # 'is_type_of' special error handling - related to #879
+                if op_name == "is_type_of":
+                    # auto transform quoted types
+                    if isinstance(op_value, str):
+                        op_value = __builtins__.get(  # type: ignore
+                            op_value, op_value
+                        )
+
+                    # invalid type (not in __builtins__) may raise TypeError
+                    try:
+                        op_succeeded = op_function(value, op_value)
+                    except TypeError:
+                        raise ValidationError(
+                            f"Invalid type '{op_value}' for condition "
+                            "'is_type_of'. Should provide a valid type"
+                        )
+                else:
+                    op_succeeded = op_function(value, op_value)
+
+                if not op_succeeded:
                     _message = self.messages["operations"].format(
                         name=name,
                         operation=op_function.__name__,
                         op_value=op_value,
                         value=value,
                         env=env,
                     )
@@ -313,31 +357,31 @@
                     getattr(validator, attr) for validator in self.validators
                 )
                 setattr(self, attr, value)
 
     def validate(
         self,
         settings: Any,
-        only: Optional[Union[str, Sequence]] = None,
-        exclude: Optional[Union[str, Sequence]] = None,
+        only: str | Sequence | None = None,
+        exclude: str | Sequence | None = None,
         only_current_env: bool = False,
     ) -> None:  # pragma: no cover
         raise NotImplementedError(
             "subclasses OrValidator or AndValidator implements this method"
         )
 
 
 class OrValidator(CombinedValidator):
     """Evaluates on Validator() | Validator()"""
 
     def validate(
         self,
         settings: Any,
-        only: Optional[Union[str, Sequence]] = None,
-        exclude: Optional[Union[str, Sequence]] = None,
+        only: str | Sequence | None = None,
+        exclude: str | Sequence | None = None,
         only_current_env: bool = False,
     ) -> None:
         """Ensure at least one of the validators are valid"""
         errors = []
         for validator in self.validators:
             try:
                 validator.validate(
@@ -363,16 +407,16 @@
 
 class AndValidator(CombinedValidator):
     """Evaluates on Validator() & Validator()"""
 
     def validate(
         self,
         settings: Any,
-        only: Optional[Union[str, Sequence]] = None,
-        exclude: Optional[Union[str, Sequence]] = None,
+        only: str | Sequence | None = None,
+        exclude: str | Sequence | None = None,
         only_current_env: bool = False,
     ) -> None:
         """Ensure both the validators are valid"""
         errors = []
         for validator in self.validators:
             try:
                 validator.validate(
@@ -394,41 +438,39 @@
             )
             raise ValidationError(_message, details=[(self, _message)])
 
 
 class ValidatorList(list):
     def __init__(
         self,
-        settings: Any,
-        validators: Optional[Sequence[Validator]] = None,
+        settings: Settings,
+        validators: Sequence[Validator] | None = None,
         *args: Validator,
         **kwargs: Any,
     ) -> None:
         if isinstance(validators, (list, tuple)):
             args = list(args) + list(validators)  # type: ignore
         self._only = kwargs.pop("validate_only", None)
         self._exclude = kwargs.pop("validate_exclude", None)
-        super(ValidatorList, self).__init__(args, **kwargs)  # type: ignore
+        super().__init__(args, **kwargs)  # type: ignore
         self.settings = settings
 
     def register(self, *args: Validator, **kwargs: Validator):
-        validators: List[Validator] = list(
+        validators: list[Validator] = list(
             chain.from_iterable(kwargs.values())  # type: ignore
         )
         validators.extend(args)
         for validator in validators:
             if validator and validator not in self:
                 self.append(validator)
 
-    def descriptions(
-        self, flat: bool = False
-    ) -> Dict[str, Union[str, List[str]]]:
+    def descriptions(self, flat: bool = False) -> dict[str, str | list[str]]:
 
         if flat:
-            descriptions: Dict[str, Union[str, List[str]]] = {}
+            descriptions: dict[str, str | list[str]] = {}
         else:
             descriptions = defaultdict(list)
 
         for validator in self:
             for name in validator.names:
                 if isinstance(name, tuple) and len(name) > 0:
                     name = name[0]
@@ -438,30 +480,30 @@
                     descriptions[name].append(  # type: ignore
                         validator.description
                     )
         return descriptions
 
     def validate(
         self,
-        only: Optional[Union[str, Sequence]] = None,
-        exclude: Optional[Union[str, Sequence]] = None,
+        only: str | Sequence | None = None,
+        exclude: str | Sequence | None = None,
         only_current_env: bool = False,
     ) -> None:
         for validator in self:
             validator.validate(
                 self.settings,
                 only=only,
                 exclude=exclude,
                 only_current_env=only_current_env,
             )
 
     def validate_all(
         self,
-        only: Optional[Union[str, Sequence]] = None,
-        exclude: Optional[Union[str, Sequence]] = None,
+        only: str | Sequence | None = None,
+        exclude: str | Sequence | None = None,
         only_current_env: bool = False,
     ) -> None:
         errors = []
         details = []
         for validator in self:
             try:
                 validator.validate(
```

### Comparing `dynaconf-3.1.9/dynaconf/validator_conditions.py` & `dynaconf-3.2.0/dynaconf/validator_conditions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # pragma: no cover
 """
 Implement basic assertions to be used in assertion action
 """
+from __future__ import annotations
 
 
 def eq(value, other):
     """Equal"""
     return value == other
 
 
@@ -71,14 +72,19 @@
 
 def len_min(value, other):
     """Minimum length"""
     return len(value) >= other
 
 
 def len_max(value, other):
-    """Maximum lenght"""
+    """Maximum length"""
     return len(value) <= other
 
 
 def startswith(value, term):
     """returns value.startswith(term) result"""
     return value.startswith(term)
+
+
+def endswith(value, term):
+    """returns value.endswith(term) result"""
+    return value.endswith(term)
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/box/box.py` & `dynaconf-3.2.0/dynaconf/vendor/box/box.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-_Z='keys'
-_Y='box_settings'
-_X='default_box_attr'
-_W='Box is frozen'
-_V='modify_tuples_box'
-_U='box_safe_prefix'
-_T='default_box_none_transform'
-_S='__created'
-_R='box_dots'
-_Q='box_duplicates'
-_P='ignore'
-_O='.'
-_N='strict'
-_M='box_recast'
-_L='box_intact_types'
-_K='default_box'
-_J='_'
+#!/usr/bin/env python
+_W='box_settings'
+_V='default_box_attr'
+_U='Box is frozen'
+_T='modify_tuples_box'
+_S='box_safe_prefix'
+_R='default_box_none_transform'
+_Q='__created'
+_P='box_dots'
+_O='box_duplicates'
+_N='ignore'
+_M='strict'
+_L='box_recast'
+_K='box_intact_types'
+_J='default_box'
 _I='utf-8'
 _H='_box_config'
 _G=True
 _F='camel_killer_box'
 _E='conversion_box'
 _D='frozen_box'
 _C='__safe_keys'
@@ -33,62 +31,62 @@
 from .converters import _to_json,_from_json,_from_toml,_to_toml,_from_yaml,_to_yaml,BOX_PARAMETERS
 from .exceptions import BoxError,BoxKeyError,BoxTypeError,BoxValueError,BoxWarning
 __all__=['Box']
 _first_cap_re=re.compile('(.)([A-Z][a-z]+)')
 _all_cap_re=re.compile('([a-z0-9])([A-Z])')
 _list_pos_re=re.compile('\\[(\\d+)\\]')
 NO_DEFAULT=object()
-def _camel_killer(attr):D='\\1_\\2';A=attr;A=str(A);B=_first_cap_re.sub(D,A);C=_all_cap_re.sub(D,B);return re.sub(' *_+',_J,C.lower())
+def _camel_killer(attr):B='\\1_\\2';A=attr;A=str(A);C=_first_cap_re.sub(B,A);D=_all_cap_re.sub(B,C);return re.sub(' *_+','_',D.lower())
 def _recursive_tuples(iterable,box_class,recreate_tuples=_B,**E):
 	D=recreate_tuples;C=box_class;B=[]
 	for A in iterable:
 		if isinstance(A,dict):B.append(C(A,**E))
 		elif isinstance(A,list)or D and isinstance(A,tuple):B.append(_recursive_tuples(A,C,D,**E))
 		else:B.append(A)
 	return tuple(B)
 def _parse_box_dots(item):
 	A=item
 	for (B,C) in enumerate(A):
 		if C=='[':return A[:B],A[B:]
-		elif C==_O:return A[:B],A[B+1:]
+		elif C=='.':return A[:B],A[B+1:]
 	raise BoxError('Could not split box dots properly')
-def _get_box_config():return{_S:_B,_C:{}}
+def _get_box_config():return{_Q:_B,_C:{}}
 class Box(dict):
-	_protected_keys=['to_dict','to_json','to_yaml','from_yaml','from_json','from_toml','to_toml','merge_update']+[A for A in dir({})if not A.startswith(_J)]
-	def __new__(A,*D,box_settings=_A,default_box=_B,default_box_attr=NO_DEFAULT,default_box_none_transform=_G,frozen_box=_B,camel_killer_box=_B,conversion_box=_G,modify_tuples_box=_B,box_safe_prefix='x',box_duplicates=_P,box_intact_types=(),box_recast=_A,box_dots=_B,**E):C=default_box_attr;B=super(Box,A).__new__(A,*D,**E);B._box_config=_get_box_config();B._box_config.update({_K:default_box,_X:A.__class__ if C is NO_DEFAULT else C,_T:default_box_none_transform,_E:conversion_box,_U:box_safe_prefix,_D:frozen_box,_F:camel_killer_box,_V:modify_tuples_box,_Q:box_duplicates,_L:tuple(box_intact_types),_M:box_recast,_R:box_dots,_Y:box_settings or{}});return B
-	def __init__(A,*B,box_settings=_A,default_box=_B,default_box_attr=NO_DEFAULT,default_box_none_transform=_G,frozen_box=_B,camel_killer_box=_B,conversion_box=_G,modify_tuples_box=_B,box_safe_prefix='x',box_duplicates=_P,box_intact_types=(),box_recast=_A,box_dots=_B,**F):
-		E=default_box_attr;super().__init__();A._box_config=_get_box_config();A._box_config.update({_K:default_box,_X:A.__class__ if E is NO_DEFAULT else E,_T:default_box_none_transform,_E:conversion_box,_U:box_safe_prefix,_D:frozen_box,_F:camel_killer_box,_V:modify_tuples_box,_Q:box_duplicates,_L:tuple(box_intact_types),_M:box_recast,_R:box_dots,_Y:box_settings or{}})
-		if not A._box_config[_E]and A._box_config[_Q]!=_P:raise BoxError('box_duplicates are only for conversion_boxes')
+	_protected_keys=['to_dict','to_json','to_yaml','from_yaml','from_json','from_toml','to_toml','merge_update']+[A for A in dir({})if not A.startswith('_')]
+	def __new__(A,*D,box_settings=_A,default_box=_B,default_box_attr=NO_DEFAULT,default_box_none_transform=_G,frozen_box=_B,camel_killer_box=_B,conversion_box=_G,modify_tuples_box=_B,box_safe_prefix='x',box_duplicates=_N,box_intact_types=(),box_recast=_A,box_dots=_B,**E):C=default_box_attr;B=super(Box,A).__new__(A,*(D),**E);B._box_config=_get_box_config();B._box_config.update({_J:default_box,_V:A.__class__ if C is NO_DEFAULT else C,_R:default_box_none_transform,_E:conversion_box,_S:box_safe_prefix,_D:frozen_box,_F:camel_killer_box,_T:modify_tuples_box,_O:box_duplicates,_K:tuple(box_intact_types),_L:box_recast,_P:box_dots,_W:box_settings or{}});return B
+	def __init__(A,*B,box_settings=_A,default_box=_B,default_box_attr=NO_DEFAULT,default_box_none_transform=_G,frozen_box=_B,camel_killer_box=_B,conversion_box=_G,modify_tuples_box=_B,box_safe_prefix='x',box_duplicates=_N,box_intact_types=(),box_recast=_A,box_dots=_B,**F):
+		E=default_box_attr;super().__init__();A._box_config=_get_box_config();A._box_config.update({_J:default_box,_V:A.__class__ if E is NO_DEFAULT else E,_R:default_box_none_transform,_E:conversion_box,_S:box_safe_prefix,_D:frozen_box,_F:camel_killer_box,_T:modify_tuples_box,_O:box_duplicates,_K:tuple(box_intact_types),_L:box_recast,_P:box_dots,_W:box_settings or{}})
+		if not A._box_config[_E]and A._box_config[_O]!=_N:raise BoxError('box_duplicates are only for conversion_boxes')
 		if len(B)==1:
 			if isinstance(B[0],str):raise BoxValueError('Cannot extrapolate Box from string')
 			if isinstance(B[0],Mapping):
 				for (D,C) in B[0].items():
 					if C is B[0]:C=A
-					if C is _A and A._box_config[_K]and A._box_config[_T]:continue
+					if C is _A and A._box_config[_J]and A._box_config[_R]:continue
 					A.__setitem__(D,C)
 			elif isinstance(B[0],Iterable):
 				for (D,C) in B[0]:A.__setitem__(D,C)
 			else:raise BoxValueError('First argument must be mapping or iterable')
 		elif B:raise BoxTypeError(f"Box expected at most 1 argument, got {len(B)}")
 		for (D,C) in F.items():
 			if B and isinstance(B[0],Mapping)and C is B[0]:C=A
 			A.__setitem__(D,C)
-		A._box_config[_S]=_G
+		A._box_config[_Q]=_G
 	def __add__(C,other):
 		A=other;B=C.copy()
 		if not isinstance(A,dict):raise BoxTypeError(f"Box can only merge two boxes or a box and a dictionary.")
 		B.merge_update(A);return B
 	def __hash__(A):
 		if A._box_config[_D]:
 			B=54321
 			for C in A.items():B^=hash(C)
 			return B
 		raise BoxTypeError('unhashable type: "Box"')
 	def __dir__(B):
-		D=string.ascii_letters+string.digits+_J;C=set(super().__dir__())
+		D=string.ascii_letters+string.digits+'_';C=set(super().__dir__())
 		for A in B.keys():
 			A=str(A)
 			if' 'not in A and A[0]not in string.digits and A not in kwlist:
 				for E in A:
 					if E not in D:break
 				else:C.add(A)
 		for A in B.keys():
@@ -97,123 +95,124 @@
 					A=B._safe_attr(A)
 					if A:C.add(A)
 		return list(C)
 	def get(B,key,default=NO_DEFAULT):
 		C=key;A=default
 		if C not in B:
 			if A is NO_DEFAULT:
-				if B._box_config[_K]and B._box_config[_T]:return B.__get_default(C)
+				if B._box_config[_J]and B._box_config[_R]:return B.__get_default(C)
 				else:return _A
-			if isinstance(A,dict)and not isinstance(A,Box):return Box(A,box_settings=B._box_config.get(_Y))
+			if isinstance(A,dict)and not isinstance(A,Box):return Box(A,box_settings=B._box_config.get(_W))
 			if isinstance(A,list)and not isinstance(A,box.BoxList):return box.BoxList(A)
 			return A
 		return B[C]
 	def copy(A):return Box(super().copy(),**A.__box_config())
 	def __copy__(A):return Box(super().copy(),**A.__box_config())
 	def __deepcopy__(A,memodict=_A):
 		B=memodict;E=A._box_config[_D];D=A.__box_config();D[_D]=_B;C=A.__class__(**D);B=B or{};B[id(A)]=C
 		for (F,G) in A.items():C[copy.deepcopy(F,B)]=copy.deepcopy(G,B)
 		C._box_config[_D]=E;return C
 	def __setstate__(A,state):B=state;A._box_config=B[_H];A.__dict__.update(B)
 	def keys(A):return super().keys()
 	def values(A):return[A[B]for B in A.keys()]
 	def items(A):return[(B,A[B])for B in A.keys()]
+	def _safe_items(A):return[(B,A._safe_get(B))for B in A.keys()]
 	def __get_default(B,item):
-		A=B._box_config[_X]
+		A=B._box_config[_V]
 		if A in(B.__class__,dict):C=B.__class__(**B.__box_config())
 		elif isinstance(A,dict):C=B.__class__(**B.__box_config(),**A)
 		elif isinstance(A,list):C=box.BoxList(**B.__box_config())
 		elif isinstance(A,Callable):C=A()
 		elif hasattr(A,'copy'):C=A.copy()
 		else:C=A
 		B.__convert_and_store(item,C);return C
 	def __box_config(C):
 		A={}
 		for (B,D) in C._box_config.copy().items():
 			if not B.startswith('__'):A[B]=D
 		return A
 	def __recast(A,item,value):
 		C=value;B=item
-		if A._box_config[_M]and B in A._box_config[_M]:
-			try:return A._box_config[_M][B](C)
-			except ValueError:raise BoxValueError(f"Cannot convert {C} to {A._box_config[_M][B]}") from _A
+		if A._box_config[_L]and B in A._box_config[_L]:
+			try:return A._box_config[_L][B](C)
+			except ValueError:raise BoxValueError(f"Cannot convert {C} to {A._box_config[_L][B]}") from _A
 		return C
 	def __convert_and_store(B,item,value):
 		C=item;A=value
 		if B._box_config[_E]:D=B._safe_attr(C);B._box_config[_C][D]=C
 		if isinstance(A,(int,float,str,bytes,bytearray,bool,complex,set,frozenset)):return super().__setitem__(C,A)
-		if B._box_config[_L]and isinstance(A,B._box_config[_L]):return super().__setitem__(C,A)
+		if B._box_config[_K]and isinstance(A,B._box_config[_K]):return super().__setitem__(C,A)
 		if isinstance(A,dict)and not isinstance(A,Box):A=B.__class__(A,**B.__box_config())
 		elif isinstance(A,list)and not isinstance(A,box.BoxList):
-			if B._box_config[_D]:A=_recursive_tuples(A,B.__class__,recreate_tuples=B._box_config[_V],**B.__box_config())
+			if B._box_config[_D]:A=_recursive_tuples(A,B.__class__,recreate_tuples=B._box_config[_T],**B.__box_config())
 			else:A=box.BoxList(A,box_class=B.__class__,**B.__box_config())
-		elif B._box_config[_V]and isinstance(A,tuple):A=_recursive_tuples(A,B.__class__,recreate_tuples=_G,**B.__box_config())
+		elif B._box_config[_T]and isinstance(A,tuple):A=_recursive_tuples(A,B.__class__,recreate_tuples=_G,**B.__box_config())
 		super().__setitem__(C,A)
 	def __getitem__(B,item,_ignore_default=_B):
 		A=item
 		try:return super().__getitem__(A)
 		except KeyError as E:
 			if A==_H:raise BoxKeyError('_box_config should only exist as an attribute and is never defaulted') from _A
-			if B._box_config[_R]and isinstance(A,str)and(_O in A or'['in A):
+			if B._box_config[_P]and isinstance(A,str)and('.'in A or'['in A):
 				C,F=_parse_box_dots(A)
 				if C in B.keys():
 					if hasattr(B[C],'__getitem__'):return B[C][F]
 			if B._box_config[_F]and isinstance(A,str):
 				D=_camel_killer(A)
 				if D in B.keys():return super().__getitem__(D)
-			if B._box_config[_K]and not _ignore_default:return B.__get_default(A)
+			if B._box_config[_J]and not _ignore_default:return B.__get_default(A)
 			raise BoxKeyError(str(E)) from _A
 	def __getattr__(A,item):
 		B=item
 		try:
 			try:C=A.__getitem__(B,_ignore_default=_G)
 			except KeyError:C=object.__getattribute__(A,B)
 		except AttributeError as E:
 			if B=='__getstate__':raise BoxKeyError(B) from _A
 			if B==_H:raise BoxError('_box_config key must exist') from _A
 			if A._box_config[_E]:
 				D=A._safe_attr(B)
 				if D in A._box_config[_C]:return A.__getitem__(A._box_config[_C][D])
-			if A._box_config[_K]:return A.__get_default(B)
+			if A._box_config[_J]:return A.__get_default(B)
 			raise BoxKeyError(str(E)) from _A
 		return C
 	def __setitem__(A,key,value):
 		C=value;B=key
-		if B!=_H and A._box_config[_S]and A._box_config[_D]:raise BoxError(_W)
-		if A._box_config[_R]and isinstance(B,str)and _O in B:
+		if B!=_H and A._box_config[_Q]and A._box_config[_D]:raise BoxError(_U)
+		if A._box_config[_P]and isinstance(B,str)and'.'in B:
 			D,E=_parse_box_dots(B)
 			if D in A.keys():
 				if hasattr(A[D],'__setitem__'):return A[D].__setitem__(E,C)
 		C=A.__recast(B,C)
 		if B not in A.keys()and A._box_config[_F]:
 			if A._box_config[_F]and isinstance(B,str):B=_camel_killer(B)
-		if A._box_config[_E]and A._box_config[_Q]!=_P:A._conversion_checks(B)
+		if A._box_config[_E]and A._box_config[_O]!=_N:A._conversion_checks(B)
 		A.__convert_and_store(B,C)
 	def __setattr__(A,key,value):
 		C=value;B=key
-		if B!=_H and A._box_config[_D]and A._box_config[_S]:raise BoxError(_W)
+		if B!=_H and A._box_config[_D]and A._box_config[_Q]:raise BoxError(_U)
 		if B in A._protected_keys:raise BoxKeyError(f'Key name "{B}" is protected')
 		if B==_H:return object.__setattr__(A,B,C)
 		C=A.__recast(B,C);D=A._safe_attr(B)
 		if D in A._box_config[_C]:B=A._box_config[_C][D]
 		A.__setitem__(B,C)
 	def __delitem__(A,key):
 		B=key
-		if A._box_config[_D]:raise BoxError(_W)
-		if B not in A.keys()and A._box_config[_R]and isinstance(B,str)and _O in B:
-			C,E=B.split(_O,1)
+		if A._box_config[_D]:raise BoxError(_U)
+		if B not in A.keys()and A._box_config[_P]and isinstance(B,str)and'.'in B:
+			C,E=B.split('.',1)
 			if C in A.keys()and isinstance(A[C],dict):return A[C].__delitem__(E)
 		if B not in A.keys()and A._box_config[_F]:
 			if A._box_config[_F]and isinstance(B,str):
 				for D in A:
 					if _camel_killer(B)==D:B=D;break
 		super().__delitem__(B)
 	def __delattr__(A,item):
 		B=item
-		if A._box_config[_D]:raise BoxError(_W)
+		if A._box_config[_D]:raise BoxError(_U)
 		if B==_H:raise BoxError('"_box_config" is protected')
 		if B in A._protected_keys:raise BoxKeyError(f'Key name "{B}" is protected')
 		try:A.__delitem__(B)
 		except KeyError as D:
 			if A._box_config[_E]:
 				C=A._safe_attr(B)
 				if C in A._box_config[_C]:A.__delitem__(A._box_config[_C][C]);del A._box_config[_C][C];return
@@ -245,83 +244,83 @@
 			if B is D:A[C]=A
 			elif isinstance(B,Box):A[C]=B.to_dict()
 			elif isinstance(B,box.BoxList):A[C]=B.to_list()
 		return A
 	def update(C,__m=_A,**D):
 		B=__m
 		if B:
-			if hasattr(B,_Z):
+			if hasattr(B,'keys'):
 				for A in B:C.__convert_and_store(A,B[A])
 			else:
 				for (A,E) in B:C.__convert_and_store(A,E)
 		for A in D:C.__convert_and_store(A,D[A])
 	def merge_update(A,__m=_A,**E):
 		C=__m
 		def D(k,v):
-			B=A._box_config[_L]and isinstance(v,A._box_config[_L])
+			B=A._box_config[_K]and isinstance(v,A._box_config[_K])
 			if isinstance(v,dict)and not B:
 				v=A.__class__(v,**A.__box_config())
 				if k in A and isinstance(A[k],dict):
 					if isinstance(A[k],Box):A[k].merge_update(v)
 					else:A[k].update(v)
 					return
 			if isinstance(v,list)and not B:v=box.BoxList(v,**A.__box_config())
 			A.__setitem__(k,v)
 		if C:
-			if hasattr(C,_Z):
+			if hasattr(C,'keys'):
 				for B in C:D(B,C[B])
 			else:
 				for (B,F) in C:D(B,F)
 		for B in E:D(B,E[B])
 	def setdefault(B,item,default=_A):
 		C=item;A=default
 		if C in B:return B[C]
 		if isinstance(A,dict):A=B.__class__(A,**B.__box_config())
 		if isinstance(A,list):A=box.BoxList(A,box_class=B.__class__,**B.__box_config())
 		B[C]=A;return A
 	def _safe_attr(C,attr):
-		B=attr;G=string.ascii_letters+string.digits+_J
-		if isinstance(B,tuple):B=_J.join([str(A)for A in B])
-		B=B.decode(_I,_P)if isinstance(B,bytes)else str(B)
+		B=attr;G=string.ascii_letters+string.digits+'_'
+		if isinstance(B,tuple):B='_'.join([str(A)for A in B])
+		B=B.decode(_I,_N)if isinstance(B,bytes)else str(B)
 		if C.__box_config()[_F]:B=_camel_killer(B)
 		A=[];D=0
 		for (E,F) in enumerate(B):
 			if F in G:D=E;A.append(F)
 			elif not A:continue
-			elif D==E-1:A.append(_J)
+			elif D==E-1:A.append('_')
 		A=''.join(A)[:D+1]
 		try:int(A[0])
 		except (ValueError,IndexError):pass
-		else:A=f"{C.__box_config()[_U]}{A}"
-		if A in kwlist:A=f"{C.__box_config()[_U]}{A}"
+		else:A=f"{C.__box_config()[_S]}{A}"
+		if A in kwlist:A=f"{C.__box_config()[_S]}{A}"
 		return A
 	def _conversion_checks(A,item):
 		B=A._safe_attr(item)
 		if B in A._box_config[_C]:
 			C=[f"{item}({B})",f"{A._box_config[_C][B]}({B})"]
-			if A._box_config[_Q].startswith('warn'):warnings.warn(f"Duplicate conversion attributes exist: {C}",BoxWarning)
+			if A._box_config[_O].startswith('warn'):warnings.warn(f"Duplicate conversion attributes exist: {C}",BoxWarning)
 			else:raise BoxError(f"Duplicate conversion attributes exist: {C}")
-	def to_json(A,filename=_A,encoding=_I,errors=_N,**B):return _to_json(A.to_dict(),filename=filename,encoding=encoding,errors=errors,**B)
+	def to_json(A,filename=_A,encoding=_I,errors=_M,**B):return _to_json(A.to_dict(),filename=filename,encoding=encoding,errors=errors,**B)
 	@classmethod
-	def from_json(E,json_string=_A,filename=_A,encoding=_I,errors=_N,**A):
+	def from_json(E,json_string=_A,filename=_A,encoding=_I,errors=_M,**A):
 		D={}
 		for B in A.copy():
 			if B in BOX_PARAMETERS:D[B]=A.pop(B)
 		C=_from_json(json_string,filename=filename,encoding=encoding,errors=errors,**A)
 		if not isinstance(C,dict):raise BoxError(f"json data not returned as a dictionary, but rather a {type(C).__name__}")
 		return E(C,**D)
-	def to_yaml(A,filename=_A,default_flow_style=_B,encoding=_I,errors=_N,**B):return _to_yaml(A.to_dict(),filename=filename,default_flow_style=default_flow_style,encoding=encoding,errors=errors,**B)
+	def to_yaml(A,filename=_A,default_flow_style=_B,encoding=_I,errors=_M,**B):return _to_yaml(A.to_dict(),filename=filename,default_flow_style=default_flow_style,encoding=encoding,errors=errors,**B)
 	@classmethod
-	def from_yaml(E,yaml_string=_A,filename=_A,encoding=_I,errors=_N,**A):
+	def from_yaml(E,yaml_string=_A,filename=_A,encoding=_I,errors=_M,**A):
 		D={}
 		for B in A.copy():
 			if B in BOX_PARAMETERS:D[B]=A.pop(B)
 		C=_from_yaml(yaml_string=yaml_string,filename=filename,encoding=encoding,errors=errors,**A)
 		if not isinstance(C,dict):raise BoxError(f"yaml data not returned as a dictionary but rather a {type(C).__name__}")
 		return E(C,**D)
-	def to_toml(A,filename=_A,encoding=_I,errors=_N):return _to_toml(A.to_dict(),filename=filename,encoding=encoding,errors=errors)
+	def to_toml(A,filename=_A,encoding=_I,errors=_M):return _to_toml(A.to_dict(),filename=filename,encoding=encoding,errors=errors)
 	@classmethod
-	def from_toml(D,toml_string=_A,filename=_A,encoding=_I,errors=_N,**B):
+	def from_toml(D,toml_string=_A,filename=_A,encoding=_I,errors=_M,**B):
 		C={}
 		for A in B.copy():
 			if A in BOX_PARAMETERS:C[A]=B.pop(A)
 		E=_from_toml(toml_string=toml_string,filename=filename,encoding=encoding,errors=errors);return D(E,**C)
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/box/box_list.py` & `dynaconf-3.2.0/dynaconf/vendor/box/box_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-_H='toml'
+#!/usr/bin/env python
 _G='box_dots'
 _F='BoxList is frozen'
 _E='frozen_box'
 _D=False
 _C='strict'
 _B='utf-8'
 _A=None
@@ -40,19 +40,19 @@
 		if B.box_options.get(_E):raise BoxError(_F)
 		if B.box_options.get(_G)and isinstance(A,str)and A.startswith('['):
 			D=_list_pos_re.search(A);E=int(D.groups()[0])
 			if len(D.group())==len(A):return super(BoxList,B).__setitem__(E,C)
 			return super(BoxList,B).__getitem__(E).__setitem__(A[len(D.group()):].lstrip('.'),C)
 		super(BoxList,B).__setitem__(A,C)
 	def _is_intact_type(A,obj):
-		C='box_intact_types'
+		B='box_intact_types'
 		try:
-			if A.box_options.get(C)and isinstance(obj,A.box_options[C]):return True
-		except AttributeError as B:
-			if'box_options'in A.__dict__:raise BoxKeyError(B)
+			if A.box_options.get(B)and isinstance(obj,A.box_options[B]):return True
+		except AttributeError as C:
+			if'box_options'in A.__dict__:raise BoxKeyError(C)
 		return _D
 	def append(A,p_object):
 		B=p_object
 		if isinstance(B,dict)and not A._is_intact_type(B):
 			try:B=A.box_class(B,**A.box_options)
 			except AttributeError as C:
 				if'box_class'in A.__dict__:raise BoxKeyError(C)
@@ -66,15 +66,15 @@
 	def insert(B,index,p_object):
 		A=p_object
 		if isinstance(A,dict)and not B._is_intact_type(A):A=B.box_class(A,**B.box_options)
 		elif isinstance(A,list)and not B._is_intact_type(A):A=B if id(A)==B.box_org_ref else BoxList(A)
 		super(BoxList,B).insert(index,A)
 	def __repr__(A):return f"<BoxList: {A.to_list()}>"
 	def __str__(A):return str(A.to_list())
-	def __copy__(A):return BoxList((B for B in A),A.box_class,**A.box_options)
+	def __copy__(A):return BoxList((A for A in A),A.box_class,**A.box_options)
 	def __deepcopy__(B,memo=_A):
 		A=memo;C=B.__class__();A=A or{};A[id(B)]=C
 		for D in B:C.append(copy.deepcopy(D,memo=A))
 		return C
 	def __hash__(A):
 		if A.box_options.get(_E):B=98765;B^=hash(tuple(A));return B
 		raise BoxTypeError("unhashable type: 'BoxList'")
@@ -105,17 +105,17 @@
 	def from_yaml(E,yaml_string=_A,filename=_A,encoding=_B,errors=_C,**A):
 		D={}
 		for B in list(A.keys()):
 			if B in BOX_PARAMETERS:D[B]=A.pop(B)
 		C=_from_yaml(yaml_string=yaml_string,filename=filename,encoding=encoding,errors=errors,**A)
 		if not isinstance(C,list):raise BoxError(f"yaml data not returned as a list but rather a {type(C).__name__}")
 		return E(C,**D)
-	def to_toml(A,filename=_A,key_name=_H,encoding=_B,errors=_C):return _to_toml({key_name:A.to_list()},filename=filename,encoding=encoding,errors=errors)
+	def to_toml(A,filename=_A,key_name='toml',encoding=_B,errors=_C):return _to_toml({key_name:A.to_list()},filename=filename,encoding=encoding,errors=errors)
 	@classmethod
-	def from_toml(F,toml_string=_A,filename=_A,key_name=_H,encoding=_B,errors=_C,**C):
+	def from_toml(F,toml_string=_A,filename=_A,key_name='toml',encoding=_B,errors=_C,**C):
 		A=key_name;D={}
 		for B in list(C.keys()):
 			if B in BOX_PARAMETERS:D[B]=C.pop(B)
 		E=_from_toml(toml_string=toml_string,filename=filename,encoding=encoding,errors=errors)
 		if A not in E:raise BoxError(f"{A} was not found.")
 		return F(E[A],**D)
 	def to_csv(A,filename,encoding=_B,errors=_C):_to_csv(A,filename=filename,encoding=encoding,errors=errors)
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/box/config_box.py` & `dynaconf-3.2.0/dynaconf/vendor/box/config_box.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,28 @@
-_H='getint'
-_G='getfloat'
-_F='getboolean'
-_E='list'
-_D='float'
-_C='int'
-_B='bool'
+#!/usr/bin/env python
+_D='getint'
+_C='getfloat'
+_B='getboolean'
 _A=None
 from dynaconf.vendor.box.box import Box
 class ConfigBox(Box):
-	_protected_keys=dir(Box)+[_B,_C,_D,_E,_F,_G,_H]
+	_protected_keys=dir(Box)+['bool','int','float','list',_B,_C,_D]
 	def __getattr__(A,item):
 		try:return super().__getattr__(item)
 		except AttributeError:return super().__getattr__(item.lower())
-	def __dir__(A):return super().__dir__()+[_B,_C,_D,_E,_F,_G,_H]
-	def bool(C,item,default=_A):
-		E=False;B=default;A=item
-		try:A=C.__getattr__(A)
-		except AttributeError as D:
+	def __dir__(A):return super().__dir__()+['bool','int','float','list',_B,_C,_D]
+	def bool(D,item,default=_A):
+		C=False;B=default;A=item
+		try:A=D.__getattr__(A)
+		except AttributeError as E:
 			if B is not _A:return B
-			raise D
+			raise E
 		if isinstance(A,(bool,int)):return bool(A)
-		if isinstance(A,str)and A.lower()in('n','no','false','f','0'):return E
-		return True if A else E
+		if isinstance(A,str)and A.lower()in('n','no','false','f','0'):return C
+		return True if A else C
 	def int(C,item,default=_A):
 		B=default;A=item
 		try:A=C.__getattr__(A)
 		except AttributeError as D:
 			if B is not _A:return B
 			raise D
 		return int(A)
@@ -39,15 +36,15 @@
 	def list(E,item,default=_A,spliter=',',strip=True,mod=_A):
 		C=strip;B=default;A=item
 		try:A=E.__getattr__(A)
 		except AttributeError as F:
 			if B is not _A:return B
 			raise F
 		if C:A=A.lstrip('[').rstrip(']')
-		D=[B.strip()if C else B for B in A.split(spliter)]
+		D=[A.strip()if C else A for A in A.split(spliter)]
 		if mod:return list(map(mod,D))
 		return D
 	def getboolean(A,item,default=_A):return A.bool(item,default)
 	def getint(A,item,default=_A):return A.int(item,default)
 	def getfloat(A,item,default=_A):return A.float(item,default)
 	def __repr__(A):return '<ConfigBox: {0}>'.format(str(A.to_dict()))
 	def copy(A):return ConfigBox(super().copy())
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/box/converters.py` & `dynaconf-3.2.0/dynaconf/vendor/box/converters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,78 +1,77 @@
-_G='r'
-_F='w'
+#!/usr/bin/env python
 _E=False
 _D=True
 _C='strict'
 _B='utf-8'
 _A=None
 import csv,json,sys,warnings
 from pathlib import Path
 import dynaconf.vendor.ruamel.yaml as yaml
 from dynaconf.vendor.box.exceptions import BoxError,BoxWarning
-from dynaconf.vendor import toml
+from dynaconf.vendor import tomllib as toml
 BOX_PARAMETERS='default_box','default_box_attr','conversion_box','frozen_box','camel_killer_box','box_safe_prefix','box_duplicates','ordered_box','default_box_none_transform','box_dots','modify_tuples_box','box_intact_types','box_recast'
 def _exists(filename,create=_E):
 	A=filename;B=Path(A)
 	if create:
 		try:B.touch(exist_ok=_D)
 		except OSError as C:raise BoxError(f"Could not create file {A} - {C}")
 		else:return
 	if not B.exists():raise BoxError(f'File "{A}" does not exist')
 	if not B.is_file():raise BoxError(f"{A} is not a file")
 def _to_json(obj,filename=_A,encoding=_B,errors=_C,**C):
 	A=filename;B=json.dumps(obj,ensure_ascii=_E,**C)
 	if A:
 		_exists(A,create=_D)
-		with open(A,_F,encoding=encoding,errors=errors)as D:D.write(B if sys.version_info>=(3,0)else B.decode(_B))
+		with open(A,'w',encoding=encoding,errors=errors)as D:D.write(B if sys.version_info>=(3,0)else B.decode(_B))
 	else:return B
 def _from_json(json_string=_A,filename=_A,encoding=_B,errors=_C,multiline=_E,**B):
 	D=json_string;A=filename
 	if A:
 		_exists(A)
-		with open(A,_G,encoding=encoding,errors=errors)as E:
+		with open(A,'r',encoding=encoding,errors=errors)as E:
 			if multiline:C=[json.loads(A.strip(),**B)for A in E if A.strip()and not A.strip().startswith('#')]
 			else:C=json.load(E,**B)
 	elif D:C=json.loads(D,**B)
 	else:raise BoxError('from_json requires a string or filename')
 	return C
 def _to_yaml(obj,filename=_A,default_flow_style=_E,encoding=_B,errors=_C,**C):
 	B=default_flow_style;A=filename
 	if A:
 		_exists(A,create=_D)
-		with open(A,_F,encoding=encoding,errors=errors)as D:yaml.dump(obj,stream=D,default_flow_style=B,**C)
+		with open(A,'w',encoding=encoding,errors=errors)as D:yaml.dump(obj,stream=D,default_flow_style=B,**C)
 	else:return yaml.dump(obj,default_flow_style=B,**C)
 def _from_yaml(yaml_string=_A,filename=_A,encoding=_B,errors=_C,**A):
-	F='Loader';C=yaml_string;B=filename
-	if F not in A:A[F]=yaml.SafeLoader
+	E='Loader';C=yaml_string;B=filename
+	if E not in A:A[E]=yaml.SafeLoader
 	if B:
 		_exists(B)
-		with open(B,_G,encoding=encoding,errors=errors)as E:D=yaml.load(E,**A)
+		with open(B,'r',encoding=encoding,errors=errors)as F:D=yaml.load(F,**A)
 	elif C:D=yaml.load(C,**A)
 	else:raise BoxError('from_yaml requires a string or filename')
 	return D
 def _to_toml(obj,filename=_A,encoding=_B,errors=_C):
 	A=filename
 	if A:
 		_exists(A,create=_D)
-		with open(A,_F,encoding=encoding,errors=errors)as B:toml.dump(obj,B)
+		with open(A,'w',encoding=encoding,errors=errors)as B:toml.dump(obj,B)
 	else:return toml.dumps(obj)
 def _from_toml(toml_string=_A,filename=_A,encoding=_B,errors=_C):
 	B=toml_string;A=filename
 	if A:
 		_exists(A)
-		with open(A,_G,encoding=encoding,errors=errors)as D:C=toml.load(D)
+		with open(A,'r',encoding=encoding,errors=errors)as D:C=toml.load(D)
 	elif B:C=toml.loads(B)
 	else:raise BoxError('from_toml requires a string or filename')
 	return C
 def _to_csv(box_list,filename,encoding=_B,errors=_C):
 	B=filename;A=box_list;C=list(A[0].keys())
 	for E in A:
 		if list(E.keys())!=C:raise BoxError('BoxList must contain the same dictionary structure for every item to convert to csv')
 	if B:
 		_exists(B,create=_D)
-		with open(B,_F,encoding=encoding,errors=errors,newline='')as F:
+		with open(B,'w',encoding=encoding,errors=errors,newline='')as F:
 			D=csv.DictWriter(F,fieldnames=C);D.writeheader()
 			for G in A:D.writerow(G)
 def _from_csv(filename,encoding=_B,errors=_C):
 	A=filename;_exists(A)
-	with open(A,_G,encoding=encoding,errors=errors,newline='')as B:C=csv.DictReader(B);return[A for A in C]
+	with open(A,'r',encoding=encoding,errors=errors,newline='')as B:C=csv.DictReader(B);return[A for A in C]
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/box/from_file.py` & `dynaconf-3.2.0/dynaconf/vendor/box/from_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+#!/usr/bin/env python
 from json import JSONDecodeError
 from pathlib import Path
 from typing import Union
-from dynaconf.vendor.toml import TomlDecodeError
+from dynaconf.vendor.tomllib import TOMLDecodeError
 from dynaconf.vendor.ruamel.yaml import YAMLError
 from .exceptions import BoxError
 from .box import Box
 from .box_list import BoxList
 __all__=['box_from_file']
 def _to_json(data):
 	try:return Box.from_json(data)
@@ -13,15 +14,15 @@
 	except BoxError:return BoxList.from_json(data)
 def _to_yaml(data):
 	try:return Box.from_yaml(data)
 	except YAMLError:raise BoxError('File is not YAML as expected')
 	except BoxError:return BoxList.from_yaml(data)
 def _to_toml(data):
 	try:return Box.from_toml(data)
-	except TomlDecodeError:raise BoxError('File is not TOML as expected')
+	except TOMLDecodeError:raise BoxError('File is not TOML as expected')
 def box_from_file(file,file_type=None,encoding='utf-8',errors='strict'):
 	C=file_type;A=file
 	if not isinstance(A,Path):A=Path(A)
 	if not A.exists():raise BoxError(f'file "{A}" does not exist')
 	B=A.read_text(encoding=encoding,errors=errors)
 	if C:
 		if C.lower()=='json':return _to_json(B)
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/box/shorthand_box.py` & `dynaconf-3.2.0/dynaconf/vendor/box/shorthand_box.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python
 from dynaconf.vendor.box.box import Box
 class SBox(Box):
 	_protected_keys=dir({})+['to_dict','to_json','to_yaml','json','yaml','from_yaml','from_json','dict','toml','from_toml','to_toml']
 	@property
 	def dict(self):return self.to_dict()
 	@property
 	def json(self):return self.to_json()
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/click/__init__.py` & `dynaconf-3.2.0/dynaconf/vendor/click/__init__.py`

 * *Files identical despite different names*

### Comparing `dynaconf-3.1.9/dynaconf/vendor/click/_bashcomplete.py` & `dynaconf-3.2.0/dynaconf/vendor/click/_bashcomplete.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-_I='COMP_CWORD'
-_H='COMP_WORDS'
-_G='fish'
-_F='zsh'
-_E='bash'
-_D='_'
+_G='COMP_CWORD'
+_F='COMP_WORDS'
+_E='zsh'
+_D='bash'
 _C=False
 _B=None
 _A=True
 import copy,os,re
 from collections import abc
 from .core import Argument
 from .core import MultiCommand
@@ -15,17 +13,17 @@
 from .parser import split_arg_string
 from .types import Choice
 from .utils import echo
 WORDBREAK='='
 COMPLETION_SCRIPT_BASH='\n%(complete_func)s() {\n    local IFS=$\'\n\'\n    COMPREPLY=( $( env COMP_WORDS="${COMP_WORDS[*]}" \\\n                   COMP_CWORD=$COMP_CWORD \\\n                   %(autocomplete_var)s=complete $1 ) )\n    return 0\n}\n\n%(complete_func)setup() {\n    local COMPLETION_OPTIONS=""\n    local BASH_VERSION_ARR=(${BASH_VERSION//./ })\n    # Only BASH version 4.4 and later have the nosort option.\n    if [ ${BASH_VERSION_ARR[0]} -gt 4 ] || ([ ${BASH_VERSION_ARR[0]} -eq 4 ] && [ ${BASH_VERSION_ARR[1]} -ge 4 ]); then\n        COMPLETION_OPTIONS="-o nosort"\n    fi\n\n    complete $COMPLETION_OPTIONS -F %(complete_func)s %(script_names)s\n}\n\n%(complete_func)setup\n'
 COMPLETION_SCRIPT_ZSH='\n#compdef %(script_names)s\n\n%(complete_func)s() {\n    local -a completions\n    local -a completions_with_descriptions\n    local -a response\n    (( ! $+commands[%(script_names)s] )) && return 1\n\n    response=("${(@f)$( env COMP_WORDS="${words[*]}" \\\n                        COMP_CWORD=$((CURRENT-1)) \\\n                        %(autocomplete_var)s="complete_zsh" \\\n                        %(script_names)s )}")\n\n    for key descr in ${(kv)response}; do\n      if [[ "$descr" == "_" ]]; then\n          completions+=("$key")\n      else\n          completions_with_descriptions+=("$key":"$descr")\n      fi\n    done\n\n    if [ -n "$completions_with_descriptions" ]; then\n        _describe -V unsorted completions_with_descriptions -U\n    fi\n\n    if [ -n "$completions" ]; then\n        compadd -U -V unsorted -a completions\n    fi\n    compstate[insert]="automenu"\n}\n\ncompdef %(complete_func)s %(script_names)s\n'
 COMPLETION_SCRIPT_FISH='complete --no-files --command %(script_names)s --arguments "(env %(autocomplete_var)s=complete_fish COMP_WORDS=(commandline -cp) COMP_CWORD=(commandline -t) %(script_names)s)"'
-_completion_scripts={_E:COMPLETION_SCRIPT_BASH,_F:COMPLETION_SCRIPT_ZSH,_G:COMPLETION_SCRIPT_FISH}
+_completion_scripts={_D:COMPLETION_SCRIPT_BASH,_E:COMPLETION_SCRIPT_ZSH,'fish':COMPLETION_SCRIPT_FISH}
 _invalid_ident_char_re=re.compile('[^a-zA-Z0-9_]')
-def get_completion_script(prog_name,complete_var,shell):A=prog_name;B=_invalid_ident_char_re.sub('',A.replace('-',_D));C=_completion_scripts.get(shell,COMPLETION_SCRIPT_BASH);return (C%{'complete_func':f"_{B}_completion",'script_names':A,'autocomplete_var':complete_var}).strip()+';'
+def get_completion_script(prog_name,complete_var,shell):A=prog_name;B=_invalid_ident_char_re.sub('',A.replace('-','_'));C=_completion_scripts.get(shell,COMPLETION_SCRIPT_BASH);return (C%{'complete_func':f"_{B}_completion",'script_names':A,'autocomplete_var':complete_var}).strip()+';'
 def resolve_ctx(cli,prog_name,args):
 	B=args;A=cli.make_context(prog_name,B,resilient_parsing=_A);B=A.protected_args+A.args
 	while B:
 		if isinstance(A.command,MultiCommand):
 			if not A.command.chain:
 				E,C,B=A.command.resolve_command(A,B)
 				if C is _B:return A
@@ -54,29 +52,29 @@
 	B=current_params[A.name]
 	if B is _B:return _A
 	if A.nargs==-1:return _A
 	if isinstance(B,abc.Iterable)and A.nargs>1 and len(B)<A.nargs:return _A
 	return _C
 def get_user_autocompletions(ctx,args,incomplete,cmd_param):
 	C=incomplete;A=cmd_param;B=[]
-	if isinstance(A.type,Choice):B=[(B,_B)for B in A.type.choices if str(B).startswith(C)]
+	if isinstance(A.type,Choice):B=[(A,_B)for A in A.type.choices if str(A).startswith(C)]
 	elif A.autocompletion is not _B:D=A.autocompletion(ctx=ctx,args=args,incomplete=C);B=[A if isinstance(A,tuple)else(A,_B)for A in D]
 	return B
 def get_visible_commands_starting_with(ctx,starts_with):
 	A=ctx
 	for B in A.command.list_commands(A):
 		if B.startswith(starts_with):
 			C=A.command.get_command(A,B)
 			if not C.hidden:yield C
 def add_subcommand_completions(ctx,incomplete,completions_out):
 	C=completions_out;B=incomplete;A=ctx
-	if isinstance(A.command,MultiCommand):C.extend([(C.name,C.get_short_help_str())for C in get_visible_commands_starting_with(A,B)])
+	if isinstance(A.command,MultiCommand):C.extend([(A.name,A.get_short_help_str())for A in get_visible_commands_starting_with(A,B)])
 	while A.parent is not _B:
 		A=A.parent
-		if isinstance(A.command,MultiCommand)and A.command.chain:D=[C for C in get_visible_commands_starting_with(A,B)if C.name not in A.protected_args];C.extend([(A.name,A.get_short_help_str())for A in D])
+		if isinstance(A.command,MultiCommand)and A.command.chain:D=[B for B in get_visible_commands_starting_with(A,B)if B.name not in A.protected_args];C.extend([(A.name,A.get_short_help_str())for A in D])
 def get_choices(cli,prog_name,args,incomplete):
 	B=incomplete;D=copy.deepcopy(args);C=resolve_ctx(cli,prog_name,args)
 	if C is _B:return[]
 	G='--'in D
 	if start_of_option(B)and WORDBREAK in B:F=B.partition(WORDBREAK);D.append(F[0]);B=F[2]
 	elif B==WORDBREAK:B=''
 	E=[]
@@ -86,29 +84,29 @@
 		return E
 	for A in C.command.params:
 		if is_incomplete_option(D,A):return get_user_autocompletions(C,D,B,A)
 	for A in C.command.params:
 		if is_incomplete_argument(C.params,A):return get_user_autocompletions(C,D,B,A)
 	add_subcommand_completions(C,B,E);return sorted(E)
 def do_complete(cli,prog_name,include_descriptions):
-	B=split_arg_string(os.environ[_H]);C=int(os.environ[_I]);E=B[1:C]
+	B=split_arg_string(os.environ[_F]);C=int(os.environ[_G]);E=B[1:C]
 	try:D=B[C]
 	except IndexError:D=''
 	for A in get_choices(cli,prog_name,E,D):
 		echo(A[0])
-		if include_descriptions:echo(A[1]if A[1]else _D)
+		if include_descriptions:echo(A[1]if A[1]else'_')
 	return _A
 def do_complete_fish(cli,prog_name):
-	B=split_arg_string(os.environ[_H]);C=os.environ[_I];D=B[1:]
+	B=split_arg_string(os.environ[_F]);C=os.environ[_G];D=B[1:]
 	for A in get_choices(cli,prog_name,D,C):
 		if A[1]:echo(f"{A[0]}\t{A[1]}")
 		else:echo(A[0])
 	return _A
 def bashcomplete(cli,prog_name,complete_var,complete_instr):
 	C=complete_instr;B=prog_name
-	if _D in C:D,A=C.split(_D,1)
-	else:D=C;A=_E
+	if'_'in C:D,A=C.split('_',1)
+	else:D=C;A=_D
 	if D=='source':echo(get_completion_script(B,complete_var,A));return _A
 	elif D=='complete':
-		if A==_G:return do_complete_fish(cli,B)
-		elif A in{_E,_F}:return do_complete(cli,B,A==_F)
+		if A=='fish':return do_complete_fish(cli,B)
+		elif A in{_D,_E}:return do_complete(cli,B,A==_E)
 	return _C
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/click/_compat.py` & `dynaconf-3.2.0/dynaconf/vendor/click/_compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-_L='stderr'
-_K='stdout'
-_J='stdin'
-_I='buffer'
-_H='ascii'
-_G='win'
+_I='stderr'
+_H='stdout'
+_G='buffer'
 _F='utf-8'
 _E='encoding'
 _D='replace'
 _C=True
 _B=False
 _A=None
 import codecs,io,os,re,sys
 from weakref import WeakKeyDictionary
 CYGWIN=sys.platform.startswith('cygwin')
-MSYS2=sys.platform.startswith(_G)and'GCC'in sys.version
+MSYS2=sys.platform.startswith('win')and'GCC'in sys.version
 APP_ENGINE='APPENGINE_RUNTIME'in os.environ and'Development/'in os.environ.get('SERVER_SOFTWARE','')
-WIN=sys.platform.startswith(_G)and not APP_ENGINE and not MSYS2
+WIN=sys.platform.startswith('win')and not APP_ENGINE and not MSYS2
 DEFAULT_COLUMNS=80
 auto_wrap_for_ansi=_A
 colorama=_A
 get_winterm_size=_A
 _ansi_re=re.compile('\\033\\[[;?0-9]*[a-zA-Z]')
 def get_filesystem_encoding():return sys.getfilesystemencoding()or sys.getdefaultencoding()
 def _make_text_stream(stream,encoding,errors,force_readable=_B,force_writable=_B):
 	C=stream;B=errors;A=encoding
 	if A is _A:A=get_best_encoding(C)
 	if B is _A:B=_D
 	return _NonClosingTextIOWrapper(C,A,B,line_buffering=_C,force_readable=force_readable,force_writable=force_writable)
 def is_ascii_encoding(encoding):
-	try:return codecs.lookup(encoding).name==_H
+	try:return codecs.lookup(encoding).name=='ascii'
 	except LookupError:return _B
 def get_best_encoding(stream):
 	A=getattr(stream,_E,_A)or sys.getdefaultencoding()
 	if is_ascii_encoding(A):return _F
 	return A
 class _NonClosingTextIOWrapper(io.TextIOWrapper):
 	def __init__(B,stream,encoding,errors,force_readable=_B,force_writable=_B,**C):A=stream;B._stream=A=_FixupStream(A,force_readable,force_writable);super().__init__(A,encoding,errors,**C)
@@ -80,22 +77,22 @@
 		try:A.write('');return _B
 		except Exception:pass
 		return default
 	return _C
 def _find_binary_reader(stream):
 	A=stream
 	if _is_binary_reader(A,_B):return A
-	B=getattr(A,_I,_A)
+	B=getattr(A,_G,_A)
 	if B is not _A and _is_binary_reader(B,_C):return B
 def _find_binary_writer(stream):
 	A=stream
 	if _is_binary_writer(A,_B):return A
-	B=getattr(A,_I,_A)
+	B=getattr(A,_G,_A)
 	if B is not _A and _is_binary_writer(B,_C):return B
-def _stream_is_misconfigured(stream):return is_ascii_encoding(getattr(stream,_E,_A)or _H)
+def _stream_is_misconfigured(stream):return is_ascii_encoding(getattr(stream,_E,_A)or'ascii')
 def _is_compat_stream_attr(stream,attr,value):A=value;B=getattr(stream,attr,_A);return B==A or A is _A and B is not _A
 def _is_compatible_text_stream(stream,encoding,errors):A=stream;return _is_compat_stream_attr(A,_E,encoding)and _is_compat_stream_attr(A,'errors',errors)
 def _force_correct_text_stream(text_stream,encoding,errors,is_binary,find_binary,force_readable=_B,force_writable=_B):
 	C=encoding;B=errors;A=text_stream
 	if is_binary(A,_B):D=A
 	else:
 		if _is_compatible_text_stream(A,C,B)and not(C is _A and _stream_is_misconfigured(A)):return A
@@ -142,25 +139,25 @@
 	if isinstance(A,bytes):A=A.decode(_F,_D)
 	return A
 def _wrap_io_open(file,mode,encoding,errors):
 	A=mode
 	if'b'in A:return open(file,A)
 	return open(file,A,encoding=encoding,errors=errors)
 def open_stream(filename,mode='r',encoding=_A,errors='strict',atomic=_B):
-	P='x';O='a';N='w';E=errors;D=encoding;B=filename;A=mode;G='b'in A
+	E=errors;D=encoding;B=filename;A=mode;G='b'in A
 	if B=='-':
-		if any((B in A for B in[N,O,P])):
+		if any((B in A for B in['w','a','x'])):
 			if G:return get_binary_stdout(),_B
 			return get_text_stdout(encoding=D,errors=E),_B
 		if G:return get_binary_stdin(),_B
 		return get_text_stdin(encoding=D,errors=E),_B
 	if not atomic:return _wrap_io_open(B,A,D,E),_C
-	if O in A:raise ValueError("Appending to an existing file is not supported, because that would involve an expensive `copy`-operation to a temporary file. Open the file in normal `w`-mode and copy explicitly if that's what you're after.")
-	if P in A:raise ValueError('Use the `overwrite`-parameter instead.')
-	if N not in A:raise ValueError('Atomic writes only make sense with `w`-mode.')
+	if'a'in A:raise ValueError("Appending to an existing file is not supported, because that would involve an expensive `copy`-operation to a temporary file. Open the file in normal `w`-mode and copy explicitly if that's what you're after.")
+	if'x'in A:raise ValueError('Use the `overwrite`-parameter instead.')
+	if'w'not in A:raise ValueError('Atomic writes only make sense with `w`-mode.')
 	import errno as I,random as K
 	try:C=os.stat(B).st_mode
 	except OSError:C=_A
 	J=os.O_RDWR|os.O_CREAT|os.O_EXCL
 	if G:J|=getattr(os,'O_BINARY',0)
 	while _C:
 		H=os.path.join(os.path.dirname(B),f".__atomic-write{K.randrange(1<<32):08x}")
@@ -232,9 +229,9 @@
 		try:B=C();D[B]=A
 		except Exception:pass
 		return A
 	return A
 _default_text_stdin=_make_cached_stream_func(lambda:sys.stdin,get_text_stdin)
 _default_text_stdout=_make_cached_stream_func(lambda:sys.stdout,get_text_stdout)
 _default_text_stderr=_make_cached_stream_func(lambda:sys.stderr,get_text_stderr)
-binary_streams={_J:get_binary_stdin,_K:get_binary_stdout,_L:get_binary_stderr}
-text_streams={_J:get_text_stdin,_K:get_text_stdout,_L:get_text_stderr}
+binary_streams={'stdin':get_binary_stdin,_H:get_binary_stdout,_I:get_binary_stderr}
+text_streams={'stdin':get_text_stdin,_H:get_text_stdout,_I:get_text_stderr}
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/click/_termui_impl.py` & `dynaconf-3.2.0/dynaconf/vendor/click/_termui_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-_H='replace'
-_G='less'
-_F='You need to use progress bars in a with block.'
-_E=' '
+_F='replace'
+_E='You need to use progress bars in a with block.'
 _D='\n'
 _C=False
 _B=True
 _A=None
 import contextlib,math,os,sys,time
 from ._compat import _default_text_stdout,CYGWIN,get_best_encoding,isatty,open_stream,strip_ansi,term_len,WIN
 from .exceptions import ClickException
@@ -19,27 +17,27 @@
 		try:C=type(B).__length_hint__
 		except AttributeError:return _A
 		try:A=C(B)
 		except TypeError:return _A
 		if A is NotImplemented or not isinstance(A,int)or A<0:return _A
 		return A
 class ProgressBar:
-	def __init__(A,iterable,length=_A,fill_char='#',empty_char=_E,bar_template='%(bar)s',info_sep='  ',show_eta=_B,show_percent=_A,show_pos=_C,item_show_func=_A,label=_A,file=_A,color=_A,width=30):
+	def __init__(A,iterable,length=_A,fill_char='#',empty_char=' ',bar_template='%(bar)s',info_sep='  ',show_eta=_B,show_percent=_A,show_pos=_C,item_show_func=_A,label=_A,file=_A,color=_A,width=30):
 		E=width;D=file;C=iterable;B=length;A.fill_char=fill_char;A.empty_char=empty_char;A.bar_template=bar_template;A.info_sep=info_sep;A.show_eta=show_eta;A.show_percent=show_percent;A.show_pos=show_pos;A.item_show_func=item_show_func;A.label=label or''
 		if D is _A:D=_default_text_stdout()
 		A.file=D;A.color=color;A.width=E;A.autowidth=E==0
 		if B is _A:B=_length_hint(C)
 		if C is _A:
 			if B is _A:raise TypeError('iterable or length is required')
 			C=range(B)
 		A.iter=iter(C);A.length=B;A.length_known=B is not _A;A.pos=0;A.avg=[];A.start=A.last_eta=time.time();A.eta_known=_C;A.finished=_C;A.max_width=_A;A.entered=_C;A.current_item=_A;A.is_hidden=not isatty(A.file);A._last_line=_A;A.short_limit=0.5
 	def __enter__(A):A.entered=_B;A.render_progress();return A
 	def __exit__(A,exc_type,exc_value,tb):A.render_finish()
 	def __iter__(A):
-		if not A.entered:raise RuntimeError(_F)
+		if not A.entered:raise RuntimeError(_E)
 		A.render_progress();return A.generator()
 	def __next__(A):return next(iter(A))
 	def is_fast(A):return time.time()-A.start<=A.short_limit
 	def render_finish(A):
 		if A.is_hidden or A.is_fast():return
 		A.file.write(AFTER_BAR);A.file.flush()
 	@property
@@ -88,21 +86,21 @@
 		return (A.bar_template%{'label':A.label,'bar':A.format_bar(),'info':A.info_sep.join(B)}).rstrip()
 	def render_progress(A):
 		from .termui import get_terminal_size as G
 		if A.is_hidden:return
 		B=[]
 		if A.autowidth:
 			H=A.width;A.width=0;I=term_len(A.format_progress_line());D=max(0,G()[0]-I)
-			if D<H:B.append(BEFORE_BAR);B.append(_E*A.max_width);A.max_width=D
+			if D<H:B.append(BEFORE_BAR);B.append(' '*A.max_width);A.max_width=D
 			A.width=D
 		F=A.width
 		if A.max_width is not _A:F=A.max_width
 		B.append(BEFORE_BAR);C=A.format_progress_line();E=term_len(C)
 		if A.max_width is _A or A.max_width<E:A.max_width=E
-		B.append(C);B.append(_E*(F-E));C=''.join(B)
+		B.append(C);B.append(' '*(F-E));C=''.join(B)
 		if C!=A._last_line and not A.is_fast():A._last_line=C;echo(C,file=A.file,color=A.color,nl=_C);A.file.flush()
 	def make_step(A,n_steps):
 		A.pos+=n_steps
 		if A.length_known and A.pos>=A.length:A.finished=_B
 		if time.time()-A.last_eta<1.0:return
 		A.last_eta=time.time()
 		if A.pos:B=(time.time()-A.start)/A.pos
@@ -110,45 +108,45 @@
 		A.avg=A.avg[-6:]+[B];A.eta_known=A.length_known
 	def update(A,n_steps,current_item=_A):
 		B=current_item;A.make_step(n_steps)
 		if B is not _A:A.current_item=B
 		A.render_progress()
 	def finish(A):A.eta_known=0;A.current_item=_A;A.finished=_B
 	def generator(A):
-		if not A.entered:raise RuntimeError(_F)
+		if not A.entered:raise RuntimeError(_E)
 		if A.is_hidden:yield from A.iter
 		else:
 			for B in A.iter:A.current_item=B;yield B;A.update(1)
 			A.finish();A.render_progress()
 def pager(generator,color=_A):
-	H='system';B=color;A=generator;C=_default_text_stdout()
+	F='system';B=color;A=generator;C=_default_text_stdout()
 	if not isatty(sys.stdin)or not isatty(C):return _nullpager(C,A,B)
 	D=(os.environ.get('PAGER',_A)or'').strip()
 	if D:
 		if WIN:return _tempfilepager(A,D,B)
 		return _pipepager(A,D,B)
 	if os.environ.get('TERM')in('dumb','emacs'):return _nullpager(C,A,B)
 	if WIN or sys.platform.startswith('os2'):return _tempfilepager(A,'more <',B)
-	if hasattr(os,H)and os.system('(less) 2>/dev/null')==0:return _pipepager(A,_G,B)
-	import tempfile as F;G,E=F.mkstemp();os.close(G)
+	if hasattr(os,F)and os.system('(less) 2>/dev/null')==0:return _pipepager(A,'less',B)
+	import tempfile as G;H,E=G.mkstemp();os.close(H)
 	try:
-		if hasattr(os,H)and os.system(f'more "{E}"')==0:return _pipepager(A,'more',B)
+		if hasattr(os,F)and os.system(f'more "{E}"')==0:return _pipepager(A,'more',B)
 		return _nullpager(C,A,B)
 	finally:os.unlink(E)
 def _pipepager(generator,cmd,color):
-	I='LESS';A=color;import subprocess as E;F=dict(os.environ);G=cmd.rsplit('/',1)[-1].split()
-	if A is _A and G[0]==_G:
-		C=f"{os.environ.get(I,'')}{_E.join(G[1:])}"
-		if not C:F[I]='-R';A=_B
+	H='LESS';A=color;import subprocess as E;F=dict(os.environ);G=cmd.rsplit('/',1)[-1].split()
+	if A is _A and G[0]=='less':
+		C=f"{os.environ.get(H,'')}{' '.join(G[1:])}"
+		if not C:F[H]='-R';A=_B
 		elif'r'in C or'R'in C:A=_B
-	B=E.Popen(cmd,shell=_B,stdin=E.PIPE,env=F);H=get_best_encoding(B.stdin)
+	B=E.Popen(cmd,shell=_B,stdin=E.PIPE,env=F);I=get_best_encoding(B.stdin)
 	try:
 		for D in generator:
 			if not A:D=strip_ansi(D)
-			B.stdin.write(D.encode(H,_H))
+			B.stdin.write(D.encode(I,_F))
 	except (OSError,KeyboardInterrupt):pass
 	else:B.stdin.close()
 	while _B:
 		try:B.wait()
 		except KeyboardInterrupt:pass
 		else:break
 def _tempfilepager(generator,cmd,color):
@@ -178,29 +176,29 @@
 		if A.env:C=os.environ.copy();C.update(A.env)
 		else:C=_A
 		try:
 			E=D.Popen(f'{B} "{filename}"',env=C,shell=_B);F=E.wait()
 			if F!=0:raise ClickException(f"{B}: Editing failed!")
 		except OSError as G:raise ClickException(f"{B}: Editing failed: {G}")
 	def edit(D,text):
-		L='\r\n';K='utf-8-sig';A=text;import tempfile as H;A=A or'';E=type(A)in[bytes,bytearray]
+		I='\r\n';H='utf-8-sig';A=text;import tempfile as J;A=A or'';E=type(A)in[bytes,bytearray]
 		if not E and A and not A.endswith(_D):A+=_D
-		I,B=H.mkstemp(prefix='editor-',suffix=D.extension)
+		K,B=J.mkstemp(prefix='editor-',suffix=D.extension)
 		try:
 			if not E:
-				if WIN:F=K;A=A.replace(_D,L)
+				if WIN:F=H;A=A.replace(_D,I)
 				else:F='utf-8'
 				A=A.encode(F)
-			C=os.fdopen(I,'wb');C.write(A);C.close();J=os.path.getmtime(B);D.edit_file(B)
-			if D.require_save and os.path.getmtime(B)==J:return _A
+			C=os.fdopen(K,'wb');C.write(A);C.close();L=os.path.getmtime(B);D.edit_file(B)
+			if D.require_save and os.path.getmtime(B)==L:return _A
 			C=open(B,'rb')
 			try:G=C.read()
 			finally:C.close()
 			if E:return G
-			else:return G.decode(K).replace(L,_D)
+			else:return G.decode(H).replace(I,_D)
 		finally:os.unlink(B)
 def open_url(url,wait=_C,locate=_C):
 	F='"';D=locate;C=wait;A=url;import subprocess as G
 	def E(url):
 		A=url;import urllib as B
 		if A.startswith('file://'):A=B.unquote(A[7:])
 		return A
@@ -253,10 +251,10 @@
 			try:tty.setraw(A);yield A
 			finally:
 				termios.tcsetattr(A,termios.TCSADRAIN,C);sys.stdout.flush()
 				if B is not _A:B.close()
 		except termios.error:pass
 	def getchar(echo):
 		with raw_terminal()as B:
-			A=os.read(B,32);A=A.decode(get_best_encoding(sys.stdin),_H)
+			A=os.read(B,32);A=A.decode(get_best_encoding(sys.stdin),_F)
 			if echo and isatty(sys.stdout):sys.stdout.write(A)
 			_translate_ch_to_exc(A);return A
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/click/_textwrap.py` & `dynaconf-3.2.0/dynaconf/vendor/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `dynaconf-3.1.9/dynaconf/vendor/click/_unicodefun.py` & `dynaconf-3.2.0/dynaconf/vendor/click/_unicodefun.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import codecs,os
 def _verify_python_env():
-	M='.utf8';L='.utf-8';J=None;I='ascii'
-	try:import locale as A;G=codecs.lookup(A.getpreferredencoding()).name
-	except Exception:G=I
-	if G!=I:return
+	L='.utf8';K='.utf-8';H=None;G='ascii'
+	try:import locale as A;I=codecs.lookup(A.getpreferredencoding()).name
+	except Exception:I=G
+	if I!=G:return
 	B=''
 	if os.name=='posix':
 		import subprocess as D
 		try:C=D.Popen(['locale','-a'],stdout=D.PIPE,stderr=D.PIPE).communicate()[0]
 		except OSError:C=b''
-		E=set();H=False
-		if isinstance(C,bytes):C=C.decode(I,'replace')
-		for K in C.splitlines():
-			A=K.strip()
-			if A.lower().endswith((L,M)):
+		E=set();J=False
+		if isinstance(C,bytes):C=C.decode(G,'replace')
+		for M in C.splitlines():
+			A=M.strip()
+			if A.lower().endswith((K,L)):
 				E.add(A)
-				if A.lower()in('c.utf8','c.utf-8'):H=True
+				if A.lower()in('c.utf8','c.utf-8'):J=True
 		B+='\n\n'
 		if not E:B+='Additional information: on this system no suitable UTF-8 locales were discovered. This most likely requires resolving by reconfiguring the locale system.'
-		elif H:B+='This system supports the C.UTF-8 locale which is recommended. You might be able to resolve your issue by exporting the following environment variables:\n\n    export LC_ALL=C.UTF-8\n    export LANG=C.UTF-8'
+		elif J:B+='This system supports the C.UTF-8 locale which is recommended. You might be able to resolve your issue by exporting the following environment variables:\n\n    export LC_ALL=C.UTF-8\n    export LANG=C.UTF-8'
 		else:B+=f"This system lists some UTF-8 supporting locales that you can pick from. The following suitable locales were discovered: {', '.join(sorted(E))}"
-		F=J
+		F=H
 		for A in (os.environ.get('LC_ALL'),os.environ.get('LANG')):
-			if A and A.lower().endswith((L,M)):F=A
-			if A is not J:break
-		if F is not J:B+=f"\n\nClick discovered that you exported a UTF-8 locale but the locale system could not pick up from it because it does not exist. The exported locale is {F!r} but it is not supported"
+			if A and A.lower().endswith((K,L)):F=A
+			if A is not H:break
+		if F is not H:B+=f"\n\nClick discovered that you exported a UTF-8 locale but the locale system could not pick up from it because it does not exist. The exported locale is {F!r} but it is not supported"
 	raise RuntimeError(f"Click will abort further execution because Python was configured to use ASCII as encoding for the environment. Consult https://click.palletsprojects.com/unicode-support/ for mitigation steps.{B}")
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/click/_winconsole.py` & `dynaconf-3.2.0/dynaconf/vendor/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `dynaconf-3.1.9/dynaconf/vendor/click/core.py` & `dynaconf-3.2.0/dynaconf/vendor/click/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-_I='default'
-_H=' / '
-_G='...'
-_F='nargs'
-_E='-'
-_D='_'
+_E='default'
+_D='nargs'
 _C=True
 _B=False
 _A=None
 import errno,inspect,os,sys
 from contextlib import contextmanager
 from functools import update_wrapper
 from itertools import repeat
@@ -40,15 +36,15 @@
 DEPRECATED_HELP_NOTICE=' (DEPRECATED)'
 DEPRECATED_INVOKE_NOTICE='DeprecationWarning: The command {name} is deprecated.'
 def _maybe_show_deprecated_notice(cmd):
 	if cmd.deprecated:echo(style(DEPRECATED_INVOKE_NOTICE.format(name=cmd.name),fg='red'),err=_C)
 def fast_exit(code):sys.stdout.flush();sys.stderr.flush();os._exit(code)
 def _bashcomplete(cmd,prog_name,complete_var=_A):
 	B=prog_name;A=complete_var
-	if A is _A:A=f"_{B}_COMPLETE".replace(_E,_D).upper()
+	if A is _A:A=f"_{B}_COMPLETE".replace('-','_').upper()
 	C=os.environ.get(A)
 	if not C:return
 	from ._bashcomplete import bashcomplete as D
 	if D(cmd,B,A,C):fast_exit(1)
 def _check_multicommand(base_command,cmd_name,cmd,register=_B):
 	B=cmd_name;A=base_command
 	if not A.chain or not isinstance(cmd,MultiCommand):return
@@ -101,15 +97,15 @@
 			else:E=['--help']
 		A.help_option_names=E
 		if M is _A and B is not _A:M=B.token_normalize_func
 		A.token_normalize_func=M;A.resilient_parsing=resilient_parsing
 		if C is _A:
 			if B is not _A and B.auto_envvar_prefix is not _A and A.info_name is not _A:C=f"{B.auto_envvar_prefix}_{A.info_name.upper()}"
 		else:C=C.upper()
-		if C is not _A:C=C.replace(_E,_D)
+		if C is not _A:C=C.replace('-','_')
 		A.auto_envvar_prefix=C
 		if N is _A and B is not _A:N=B.color
 		A.color=N;A.show_default=show_default;A._close_callbacks=[];A._depth=0;A._source_by_paramname={}
 	def __enter__(A):A._depth+=1;push_context(A);return A
 	def __exit__(A,exc_type,exc_value,tb):
 		A._depth-=1
 		if A._depth==0:A.close()
@@ -163,15 +159,15 @@
 		if isinstance(A,Command):
 			C=A;A=C.callback;G=Context(C,info_name=C.name,parent=F)
 			if A is _A:raise TypeError('The given command does not have a callback that can be invoked.')
 			for D in C.params:
 				if D.name not in E and D.expose_value:E[D.name]=D.get_default(G)
 		B=B[2:]
 		with augment_usage_errors(F):
-			with G:return A(*B,**E)
+			with G:return A(*(B),**E)
 	def forward(*E,**A):
 		B,D=E[:2]
 		if not isinstance(D,Command):raise TypeError('Callback is not a command.')
 		for C in B.params:
 			if C not in A:A[C]=B.params[C]
 		return B.invoke(D,**A)
 	def set_parameter_source(B,name,source):A=source;ParameterSource.validate(A);B._source_by_paramname[name]=A
@@ -214,15 +210,15 @@
 				else:raise
 		except Exit as A:
 			if D:sys.exit(A.exit_code)
 			else:return A.exit_code
 		except Abort:
 			if not D:raise
 			echo('Aborted!',file=sys.stderr);sys.exit(1)
-	def __call__(A,*B,**C):return A.main(*B,**C)
+	def __call__(A,*B,**C):return A.main(*(B),**C)
 class Command(BaseCommand):
 	def __init__(A,name,context_settings=_A,callback=_A,params=_A,help=_A,epilog=_A,short_help=_A,options_metavar='[OPTIONS]',add_help_option=_C,no_args_is_help=_B,hidden=_B,deprecated=_B):
 		B='\x0c';BaseCommand.__init__(A,name,context_settings);A.callback=callback;A.params=params or[]
 		if help and B in help:help=help.split(B,1)[0]
 		A.help=help;A.epilog=epilog;A.options_metavar=options_metavar;A.short_help=short_help;A.add_help_option=add_help_option;A.no_args_is_help=no_args_is_help;A.hidden=hidden;A.deprecated=deprecated
 	def __repr__(A):return f"<{A.__class__.__name__} {A.name}>"
 	def get_usage(B,ctx):A=ctx.make_formatter();B.format_usage(ctx,A);return A.getvalue().rstrip('\n')
@@ -301,15 +297,15 @@
 				if isinstance(F,Argument)and not F.required:raise RuntimeError('Multi commands in chain mode cannot have optional arguments.')
 	def collect_usage_pieces(A,ctx):B=Command.collect_usage_pieces(A,ctx);B.append(A.subcommand_metavar);return B
 	def format_options(A,ctx,formatter):B=formatter;Command.format_options(A,ctx,B);A.format_commands(ctx,B)
 	def resultcallback(A,replace=_B):
 		def B(f):
 			B=A.result_callback
 			if B is _A or replace:A.result_callback=f;return f
-			def C(__value,*A,**C):return f(B(__value,*A,**C),*A,**C)
+			def C(__value,*A,**C):return f(B(__value,*(A),**C),*(A),**C)
 			A.result_callback=D=update_wrapper(C,f);return D
 		return B
 	def format_commands(F,ctx,formatter):
 		D=formatter;B=[]
 		for C in F.list_commands(ctx):
 			A=F.get_command(ctx,C)
 			if A is _A:continue
@@ -363,19 +359,19 @@
 	def __init__(A,name=_A,commands=_A,**B):MultiCommand.__init__(A,name,**B);A.commands=commands or{}
 	def add_command(C,cmd,name=_A):
 		B=cmd;A=name;A=A or B.name
 		if A is _A:raise TypeError('Command has no name.')
 		_check_multicommand(C,A,B,register=_C);C.commands[A]=B
 	def command(B,*C,**D):
 		from .decorators import command as E
-		def A(f):A=E(*C,**D)(f);B.add_command(A);return A
+		def A(f):A=E(*(C),**D)(f);B.add_command(A);return A
 		return A
 	def group(B,*C,**D):
 		from .decorators import group
-		def A(f):A=group(*C,**D)(f);B.add_command(A);return A
+		def A(f):A=group(*(C),**D)(f);B.add_command(A);return A
 		return A
 	def get_command(A,ctx,cmd_name):return A.commands.get(cmd_name)
 	def list_commands(A,ctx):return sorted(A.commands)
 class CommandCollection(MultiCommand):
 	def __init__(A,name=_A,sources=_A,**B):MultiCommand.__init__(A,name,**B);A.sources=sources or[]
 	def add_source(A,multi_cmd):A.sources.append(multi_cmd)
 	def get_command(A,ctx,cmd_name):
@@ -400,15 +396,15 @@
 	def __repr__(A):return f"<{A.__class__.__name__} {A.name}>"
 	@property
 	def human_readable_name(self):return self.name
 	def make_metavar(A):
 		if A.metavar is not _A:return A.metavar
 		B=A.type.get_metavar(A)
 		if B is _A:B=A.type.name.upper()
-		if A.nargs!=1:B+=_G
+		if A.nargs!=1:B+='...'
 		return B
 	def get_default(A,ctx):
 		if callable(A.default):B=A.default()
 		else:B=A.default
 		return A.type_cast_value(ctx,B)
 	def add_to_parser(A,parser,ctx):0
 	def consume_value(B,ctx,opts):
@@ -417,15 +413,15 @@
 		if A is _A:A=C.lookup_default(B.name);D=ParameterSource.DEFAULT_MAP
 		if A is not _A:C.set_parameter_source(B.name,D)
 		return A
 	def type_cast_value(A,ctx,value):
 		C=value;B=ctx
 		if A.type.is_composite:
 			if A.nargs<=1:raise TypeError(f"Attempted to invoke composite type but nargs has been set to {A.nargs}. This is not supported; nargs needs to be set to a fixed value > 1.")
-			if A.multiple:return tuple((A.type(D or(),A,B)for D in C or()))
+			if A.multiple:return tuple((A.type(C or(),A,B)for C in C or()))
 			return A.type(C or(),A,B)
 		def D(value,level):
 			E=level;C=value
 			if E==0:return A.type(C,A,B)
 			return tuple((D(A,E-1)for A in C or()))
 		return D(C,(A.nargs!=1)+bool(A.multiple))
 	def process_value(B,ctx,value):
@@ -468,20 +464,20 @@
 				try:C=A.callback(B,A,C)
 				except Exception:
 					if not B.resilient_parsing:raise
 		if A.expose_value:B.params[A.name]=C
 		return C,args
 	def get_help_record(A,ctx):0
 	def get_usage_pieces(A,ctx):return[]
-	def get_error_hint(A,ctx):B=A.opts or[A.human_readable_name];return _H.join((repr(A)for A in B))
+	def get_error_hint(A,ctx):B=A.opts or[A.human_readable_name];return ' / '.join((repr(A)for A in B))
 class Option(Parameter):
 	param_type_name='option'
 	def __init__(A,param_decls=_A,show_default=_B,prompt=_B,confirmation_prompt=_B,hide_input=_B,is_flag=_A,flag_value=_A,multiple=_B,count=_B,allow_from_autoenv=_C,type=_A,help=_A,hidden=_B,show_choices=_C,show_envvar=_B,**G):
-		F=count;D=prompt;C=flag_value;B=is_flag;H=G.get(_I,_missing)is _missing;Parameter.__init__(A,param_decls,type=type,**G)
-		if D is _C:E=A.name.replace(_D,' ').capitalize()
+		F=count;D=prompt;C=flag_value;B=is_flag;H=G.get(_E,_missing)is _missing;Parameter.__init__(A,param_decls,type=type,**G)
+		if D is _C:E=A.name.replace('_',' ').capitalize()
 		elif D is _B:E=_A
 		else:E=D
 		A.prompt=E;A.confirmation_prompt=confirmation_prompt;A.hide_input=hide_input;A.hidden=hidden
 		if B is _A:
 			if C is not _A:B=_C
 			else:B=bool(A.secondary_opts)
 		if B and H:A.default=_B
@@ -498,72 +494,72 @@
 			if A.nargs<0:raise TypeError('Options cannot have nargs < 0')
 			if A.prompt and A.is_flag and not A.is_bool_flag:raise TypeError('Cannot prompt for flags that are not bools.')
 			if not A.is_bool_flag and A.secondary_opts:raise TypeError('Got secondary option for non boolean flag.')
 			if A.is_bool_flag and A.hide_input and A.prompt is not _A:raise TypeError('Hidden input does not work with boolean flag prompts.')
 			if A.count:
 				if A.multiple:raise TypeError('Options cannot be multiple and count at the same time.')
 				elif A.is_flag:raise TypeError('Options cannot be count and flags at the same time.')
-	def _parse_decls(J,decls,expose_value):
-		I='/';C=[];F=[];A=_A;D=[]
+	def _parse_decls(I,decls,expose_value):
+		C=[];F=[];A=_A;D=[]
 		for B in decls:
 			if B.isidentifier():
 				if A is not _A:raise TypeError('Name defined twice')
 				A=B
 			else:
-				H=';'if B[:1]==I else I
+				H=';'if B[:1]=='/'else'/'
 				if H in B:
 					E,G=B.split(H,1);E=E.rstrip()
 					if E:D.append(split_opt(E));C.append(E)
 					G=G.lstrip()
 					if G:F.append(G.lstrip())
 				else:D.append(split_opt(B));C.append(B)
 		if A is _A and D:
-			D.sort(key=lambda x:-len(x[0]));A=D[0][1].replace(_E,_D).lower()
+			D.sort(key=lambda x:-len(x[0]));A=D[0][1].replace('-','_').lower()
 			if not A.isidentifier():A=_A
 		if A is _A:
 			if not expose_value:return _A,C,F
 			raise TypeError('Could not determine name for option')
 		if not C and not F:raise TypeError(f"No options defined but a name was passed ({A}). Did you mean to declare an argument instead of an option?")
 		return A,C,F
 	def add_to_parser(A,parser,ctx):
-		C=parser;B={'dest':A.name,_F:A.nargs,'obj':A}
+		C=parser;B={'dest':A.name,_D:A.nargs,'obj':A}
 		if A.multiple:D='append'
 		elif A.count:D='count'
 		else:D='store'
 		if A.is_flag:
-			B.pop(_F,_A);E=f"{D}_const"
+			B.pop(_D,_A);E=f"{D}_const"
 			if A.is_bool_flag and A.secondary_opts:C.add_option(A.opts,action=E,const=_C,**B);C.add_option(A.secondary_opts,action=E,const=_B,**B)
 			else:C.add_option(A.opts,action=E,const=A.flag_value,**B)
 		else:B['action']=D;C.add_option(A.opts,**B)
 	def get_help_record(A,ctx):
-		K=', ';E=ctx
+		E=ctx
 		if A.hidden:return
 		F=[]
 		def G(opts):
 			B,C=join_options(opts)
 			if C:F[:]=[_C]
 			if not A.is_flag and not A.count:B+=f" {A.make_metavar()}"
 			return B
 		H=[G(A.opts)]
 		if A.secondary_opts:H.append(G(A.secondary_opts))
 		help=A.help or'';C=[]
 		if A.show_envvar:
 			B=A.envvar
 			if B is _A:
 				if A.allow_from_autoenv and E.auto_envvar_prefix is not _A:B=f"{E.auto_envvar_prefix}_{A.name.upper()}"
-			if B is not _A:J=K.join((str(A)for A in B))if isinstance(B,(list,tuple))else B;C.append(f"env var: {J}")
+			if B is not _A:J=', '.join((str(A)for A in B))if isinstance(B,(list,tuple))else B;C.append(f"env var: {J}")
 		if A.default is not _A and(A.show_default or E.show_default):
 			if isinstance(A.show_default,str):D=f"({A.show_default})"
-			elif isinstance(A.default,(list,tuple)):D=K.join((str(B)for B in A.default))
+			elif isinstance(A.default,(list,tuple)):D=', '.join((str(A)for A in A.default))
 			elif inspect.isfunction(A.default):D='(dynamic)'
 			else:D=A.default
 			C.append(f"default: {D}")
 		if A.required:C.append('required')
 		if C:I=';'.join(C);help=f"{help}  [{I}]"if help else f"[{I}]"
-		return ('; 'if F else _H).join(H),help
+		return ('; 'if F else' / ').join(H),help
 	def get_default(A,ctx):
 		if A.is_flag and not A.is_bool_flag:
 			for B in ctx.command.params:
 				if B.name==A.name and B.default:return B.flag_value
 			return _A
 		return Parameter.get_default(A,ctx)
 	def prompt_for_value(A,ctx):
@@ -587,34 +583,34 @@
 		if C is _A and A.prompt is not _A and not B.resilient_parsing:return A.prompt_for_value(B)
 		return Parameter.full_process_value(A,B,C)
 class Argument(Parameter):
 	param_type_name='argument'
 	def __init__(B,param_decls,required=_A,**C):
 		A=required
 		if A is _A:
-			if C.get(_I)is not _A:A=_B
-			else:A=C.get(_F,1)>0
+			if C.get(_E)is not _A:A=_B
+			else:A=C.get(_D,1)>0
 		Parameter.__init__(B,param_decls,required=A,**C)
 		if B.default is not _A and B.nargs<0:raise TypeError('nargs=-1 in combination with a default value is not supported.')
 	@property
 	def human_readable_name(self):
 		A=self
 		if A.metavar is not _A:return A.metavar
 		return A.name.upper()
 	def make_metavar(A):
 		if A.metavar is not _A:return A.metavar
 		B=A.type.get_metavar(A)
 		if not B:B=A.name.upper()
 		if not A.required:B=f"[{B}]"
-		if A.nargs!=1:B+=_G
+		if A.nargs!=1:B+='...'
 		return B
 	def _parse_decls(D,decls,expose_value):
 		A=decls
 		if not A:
 			if not expose_value:return _A,[],[]
 			raise TypeError('Could not determine name for argument')
-		if len(A)==1:B=C=A[0];B=B.replace(_E,_D).lower()
+		if len(A)==1:B=C=A[0];B=B.replace('-','_').lower()
 		else:raise TypeError(f"Arguments take exactly one parameter declaration, got {len(A)}.")
 		return B,[C],[]
 	def get_usage_pieces(A,ctx):return[A.make_metavar()]
 	def get_error_hint(A,ctx):return repr(A.make_metavar())
 	def add_to_parser(A,parser,ctx):parser.add_argument(dest=A.name,nargs=A.nargs,obj=A)
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/click/decorators.py` & `dynaconf-3.2.0/dynaconf/vendor/click/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,29 +14,29 @@
 from .core import Command
 from .core import Group
 from .core import Option
 from .globals import get_current_context
 from .utils import echo
 def pass_context(f):
 	'Marks a callback as wanting to receive the current context\n    object as first argument.\n    '
-	def A(*A,**B):return f(get_current_context(),*A,**B)
+	def A(*A,**B):return f(get_current_context(),*(A),**B)
 	return update_wrapper(A,f)
 def pass_obj(f):
 	'Similar to :func:`pass_context`, but only pass the object on the\n    context onwards (:attr:`Context.obj`).  This is useful if that object\n    represents the state of a nested system.\n    '
-	def A(*A,**B):return f(get_current_context().obj,*A,**B)
+	def A(*A,**B):return f(get_current_context().obj,*(A),**B)
 	return update_wrapper(A,f)
 def make_pass_decorator(object_type,ensure=_D):
 	"Given an object type this creates a decorator that will work\n    similar to :func:`pass_obj` but instead of passing the object of the\n    current context, it will find the innermost context of type\n    :func:`object_type`.\n\n    This generates a decorator that works roughly like this::\n\n        from functools import update_wrapper\n\n        def decorator(f):\n            @pass_context\n            def new_func(ctx, *args, **kwargs):\n                obj = ctx.find_object(object_type)\n                return ctx.invoke(f, obj, *args, **kwargs)\n            return update_wrapper(new_func, f)\n        return decorator\n\n    :param object_type: the type of the object to pass.\n    :param ensure: if set to `True`, a new object will be created and\n                   remembered on the context if it's not there yet.\n    ";A=object_type
 	def B(f):
 		def B(*D,**E):
 			B=get_current_context()
 			if ensure:C=B.ensure_object(A)
 			else:C=B.find_object(A)
 			if C is _A:raise RuntimeError(f"Managed to invoke callback without a context object of type {A.__name__!r} existing.")
-			return B.invoke(f,C,*D,**E)
+			return B.invoke(f,C,*(D),**E)
 		return update_wrapper(B,f)
 	return B
 def _make_command(f,name,attrs,cls):
 	A=attrs
 	if isinstance(f,Command):raise TypeError('Attempted to convert a callback into a command twice.')
 	try:B=f.__click_params__;B.reverse();del f.__click_params__
 	except AttributeError:B=[]
@@ -70,19 +70,19 @@
 		D=A.pop(_E,Option);_param_memo(f,D(B,**A));return f
 	return A
 def confirmation_option(*B,**A):
 	"Shortcut for confirmation prompts that can be ignored by passing\n    ``--yes`` as parameter.\n\n    This is equivalent to decorating a function with :func:`option` with\n    the following parameters::\n\n        def callback(ctx, param, value):\n            if not value:\n                ctx.abort()\n\n        @click.command()\n        @click.option('--yes', is_flag=True, callback=callback,\n                      expose_value=False, prompt='Do you want to continue?')\n        def dropdb():\n            pass\n    "
 	def C(f):
 		def C(ctx,param,value):
 			if not value:ctx.abort()
-		A.setdefault(_F,_C);A.setdefault(_G,C);A.setdefault(_H,_D);A.setdefault(_I,'Do you want to continue?');A.setdefault(_B,'Confirm the action without prompting.');return option(*B or('--yes',),**A)(f)
+		A.setdefault(_F,_C);A.setdefault(_G,C);A.setdefault(_H,_D);A.setdefault(_I,'Do you want to continue?');A.setdefault(_B,'Confirm the action without prompting.');return option(*(B or('--yes',)),**A)(f)
 	return C
 def password_option(*B,**A):
 	"Shortcut for password prompts.\n\n    This is equivalent to decorating a function with :func:`option` with\n    the following parameters::\n\n        @click.command()\n        @click.option('--password', prompt=True, confirmation_prompt=True,\n                      hide_input=True)\n        def changeadmin(password):\n            pass\n    "
-	def C(f):A.setdefault(_I,_C);A.setdefault('confirmation_prompt',_C);A.setdefault('hide_input',_C);return option(*B or('--password',),**A)(f)
+	def C(f):A.setdefault(_I,_C);A.setdefault('confirmation_prompt',_C);A.setdefault('hide_input',_C);return option(*(B or('--password',)),**A)(f)
 	return C
 def version_option(version=_A,*B,**A):
 	"Adds a ``--version`` option which immediately ends the program\n    printing out the version number.  This is implemented as an eager\n    option that prints the version and exits the program in the callback.\n\n    :param version: the version number to show.  If not provided Click\n                    attempts an auto discovery via setuptools.\n    :param prog_name: the name of the program (defaults to autodetection)\n    :param message: custom message to show instead of the default\n                    (``'%(prog)s, version %(version)s'``)\n    :param others: everything else is forwarded to :func:`option`.\n    ";D=version
 	if D is _A:
 		if hasattr(sys,'_getframe'):E=sys._getframe(1).f_globals.get('__name__')
 		else:E=''
 	def C(f):
@@ -99,17 +99,17 @@
 				else:
 					for F in I.working_set:
 						J=F.get_entry_map().get('console_scripts')or{}
 						for K in J.values():
 							if K.module_name==E:B=F.version;break
 				if B is _A:raise RuntimeError('Could not determine version')
 			echo(H%{'prog':C,'version':B},color=A.color);A.exit()
-		A.setdefault(_F,_C);A.setdefault(_H,_D);A.setdefault(_J,_C);A.setdefault(_B,'Show the version and exit.');A[_G]=C;return option(*B or('--version',),**A)(f)
+		A.setdefault(_F,_C);A.setdefault(_H,_D);A.setdefault(_J,_C);A.setdefault(_B,'Show the version and exit.');A[_G]=C;return option(*(B or('--version',)),**A)(f)
 	return C
 def help_option(*B,**A):
 	'Adds a ``--help`` option which immediately ends the program\n    printing out the help page.  This is usually unnecessary to add as\n    this is added by default to all commands unless suppressed.\n\n    Like :func:`version_option`, this is implemented as eager option that\n    prints in the callback and exits.\n\n    All arguments are forwarded to :func:`option`.\n    '
 	def C(f):
 		def C(ctx,param,value):
 			A=ctx
 			if value and not A.resilient_parsing:echo(A.get_help(),color=A.color);A.exit()
-		A.setdefault(_F,_C);A.setdefault(_H,_D);A.setdefault(_B,'Show this message and exit.');A.setdefault(_J,_C);A[_G]=C;return option(*B or('--help',),**A)(f)
+		A.setdefault(_F,_C);A.setdefault(_H,_D);A.setdefault(_B,'Show this message and exit.');A.setdefault(_J,_C);A[_G]=C;return option(*(B or('--help',)),**A)(f)
 	return C
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/click/exceptions.py` & `dynaconf-3.2.0/dynaconf/vendor/click/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 _A=None
 from ._compat import filename_to_ui,get_text_stderr
 from .utils import echo
 def _join_param_hints(param_hint):
 	A=param_hint
-	if isinstance(A,(tuple,list)):return ' / '.join((repr(B)for B in A))
+	if isinstance(A,(tuple,list)):return ' / '.join((repr(A)for A in A))
 	return A
 class ClickException(Exception):
 	exit_code=1
 	def __init__(B,message):A=message;super().__init__(A);B.message=A
 	def format_message(A):return A.message
 	def __str__(A):return A.message
 	def show(B,file=_A):
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/click/formatting.py` & `dynaconf-3.2.0/dynaconf/vendor/click/formatting.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .parser import split_opt
 from .termui import get_terminal_size
 FORCED_WIDTH=_A
 def measure_table(rows):
 	A={}
 	for C in rows:
 		for (B,D) in enumerate(C):A[B]=max(A.get(B,0),term_len(D))
-	return tuple((B for(C,B)in sorted(A.items())))
+	return tuple((A for(B,A)in sorted(A.items())))
 def iter_rows(rows,col_count):
 	for A in rows:A=tuple(A);yield A+('',)*(col_count-len(A))
 def wrap_text(text,width=78,initial_indent='',subsequent_indent='',preserve_paragraphs=_D):
 	A=text;from ._textwrap import TextWrapper as I;A=A.expandtabs();E=I(width,initial_indent=initial_indent,subsequent_indent=subsequent_indent,replace_whitespace=_D)
 	if not preserve_paragraphs:return E.fill(A)
 	F=[];C=[];B=_A
 	def H():
@@ -83,8 +83,8 @@
 	def getvalue(A):return ''.join(A.buffer)
 def join_options(options):
 	A=[];B=_D
 	for C in options:
 		D=split_opt(C)[0]
 		if D=='/':B=_E
 		A.append((len(D),C))
-	A.sort(key=lambda x:x[0]);A=', '.join((B[1]for B in A));return A,B
+	A.sort(key=lambda x:x[0]);A=', '.join((A[1]for A in A));return A,B
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/click/parser.py` & `dynaconf-3.2.0/dynaconf/vendor/click/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-_D=False
 _C='append'
 _B='store'
 _A=None
 import re
 from collections import deque
 from .exceptions import BadArgumentUsage
 from .exceptions import BadOptionUsage
@@ -80,15 +79,15 @@
 			if D==len(B):B=_A
 			elif D!=0:raise BadArgumentUsage(f"argument {A.dest} takes {A.nargs} values")
 		C.opts[A.dest]=B;C.order.append(A.obj)
 class ParsingState:
 	def __init__(A,rargs):A.opts={};A.largs=[];A.rargs=rargs;A.order=[]
 class OptionParser:
 	def __init__(A,ctx=_A):
-		B=ctx;A.ctx=B;A.allow_interspersed_args=True;A.ignore_unknown_options=_D
+		B=ctx;A.ctx=B;A.allow_interspersed_args=True;A.ignore_unknown_options=False
 		if B is not _A:A.allow_interspersed_args=B.allow_interspersed_args;A.ignore_unknown_options=B.ignore_unknown_options
 		A._short_opt={};A._long_opt={};A._opt_prefixes={'-','--'};A._args=[]
 	def add_option(B,opts,dest,action=_A,nargs=1,const=_A,obj=_A):
 		D=obj;C=opts
 		if D is _A:D=dest
 		C=[normalize_opt(A,B.ctx)for A in C];A=Option(C,dest,action=action,nargs=nargs,const=const,obj=D);B._opt_prefixes.update(A.prefixes)
 		for E in A._short_opts:B._short_opt[E]=A
@@ -125,15 +124,15 @@
 			if len(B.rargs)<C:_error_opt_args(C,A)
 			elif C==1:G=B.rargs.pop(0)
 			else:G=tuple(B.rargs[:C]);del B.rargs[:C]
 		elif E is not _A:raise BadOptionUsage(A,f"{A} option does not take a value")
 		else:G=_A
 		F.process(G,B)
 	def _match_short_opt(B,arg,state):
-		D=arg;A=state;J=_D;F=1;K=D[0];G=[]
+		D=arg;A=state;J=False;F=1;K=D[0];G=[]
 		for L in D[1:]:
 			H=normalize_opt(f"{K}{L}",B.ctx);E=B._short_opt.get(H);F+=1
 			if not E:
 				if B.ignore_unknown_options:G.append(L);continue
 				raise NoSuchOption(H,ctx=B.ctx)
 			if E.takes_value:
 				if F<len(D):A.rargs.insert(0,D[F:]);J=True
@@ -142,16 +141,16 @@
 				elif C==1:I=A.rargs.pop(0)
 				else:I=tuple(A.rargs[:C]);del A.rargs[:C]
 			else:I=_A
 			E.process(I,A)
 			if J:break
 		if B.ignore_unknown_options and G:A.largs.append(f"{K}{''.join(G)}")
 	def _process_opts(B,arg,state):
-		G='=';C=state;A=arg;D=_A
-		if G in A:E,D=A.split(G,1)
+		C=state;A=arg;D=_A
+		if'='in A:E,D=A.split('=',1)
 		else:E=A
 		F=normalize_opt(E,B.ctx)
 		try:B._match_long_opt(F,D,C)
 		except NoSuchOption:
 			if A[:2]not in B._opt_prefixes:return B._match_short_opt(A,C)
 			if not B.ignore_unknown_options:raise
 			C.largs.append(A)
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/click/termui.py` & `dynaconf-3.2.0/dynaconf/vendor/click/termui.py`

 * *Files identical despite different names*

### Comparing `dynaconf-3.1.9/dynaconf/vendor/click/testing.py` & `dynaconf-3.2.0/dynaconf/vendor/click/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-_E='replace'
-_D=False
-_C='\n'
+_D='replace'
+_C=False
 _B='\r\n'
 _A=None
 import contextlib,io,os,shlex,shutil,sys,tempfile
 from .  import formatting,termui,utils
 from ._compat import _find_binary_reader
 class EchoingStdin:
 	def __init__(A,input,output):A._input=input;A._output=output
@@ -24,30 +23,30 @@
 	elif not isinstance(input,bytes):input=input.encode(charset)
 	return io.BytesIO(input)
 class Result:
 	def __init__(A,runner,stdout_bytes,stderr_bytes,exit_code,exception,exc_info=_A):A.runner=runner;A.stdout_bytes=stdout_bytes;A.stderr_bytes=stderr_bytes;A.exit_code=exit_code;A.exception=exception;A.exc_info=exc_info
 	@property
 	def output(self):return self.stdout
 	@property
-	def stdout(self):return self.stdout_bytes.decode(self.runner.charset,_E).replace(_B,_C)
+	def stdout(self):return self.stdout_bytes.decode(self.runner.charset,_D).replace(_B,'\n')
 	@property
 	def stderr(self):
 		A=self
 		if A.stderr_bytes is _A:raise ValueError('stderr not separately captured')
-		return A.stderr_bytes.decode(A.runner.charset,_E).replace(_B,_C)
+		return A.stderr_bytes.decode(A.runner.charset,_D).replace(_B,'\n')
 	def __repr__(A):B=repr(A.exception)if A.exception else'okay';return f"<{type(A).__name__} {B}>"
 class CliRunner:
-	def __init__(A,charset='utf-8',env=_A,echo_stdin=_D,mix_stderr=True):A.charset=charset;A.env=env or{};A.echo_stdin=echo_stdin;A.mix_stderr=mix_stderr
+	def __init__(A,charset='utf-8',env=_A,echo_stdin=_C,mix_stderr=True):A.charset=charset;A.env=env or{};A.echo_stdin=echo_stdin;A.mix_stderr=mix_stderr
 	def get_default_prog_name(A,cli):return cli.name or'root'
 	def make_env(C,overrides=_A):
 		A=overrides;B=dict(C.env)
 		if A:B.update(A)
 		return B
 	@contextlib.contextmanager
-	def isolation(self,input=_A,env=_A,color=_D):
+	def isolation(self,input=_A,env=_A,color=_C):
 		D=env;A=self;input=make_input_stream(input,A.charset);H=sys.stdin;I=sys.stdout;J=sys.stderr;K=formatting.FORCED_WIDTH;formatting.FORCED_WIDTH=80;D=A.make_env(D);E=io.BytesIO()
 		if A.echo_stdin:input=EchoingStdin(input,E)
 		input=io.TextIOWrapper(input,encoding=A.charset);sys.stdout=io.TextIOWrapper(E,encoding=A.charset)
 		if not A.mix_stderr:F=io.BytesIO();sys.stderr=io.TextIOWrapper(F,encoding=A.charset)
 		if A.mix_stderr:sys.stderr=sys.stdout
 		sys.stdin=input
 		def L(prompt=_A):sys.stdout.write(prompt or'');A=input.readline().rstrip(_B);sys.stdout.write(f"{A}\n");sys.stdout.flush();return A
@@ -73,27 +72,27 @@
 		finally:
 			for (B,C) in G.items():
 				if C is _A:
 					try:del os.environ[B]
 					except Exception:pass
 				else:os.environ[B]=C
 			sys.stdout=I;sys.stderr=J;sys.stdin=H;termui.visible_prompt_func=Q;termui.hidden_prompt_func=R;termui._getchar=S;utils.should_strip_ansi=T;formatting.FORCED_WIDTH=K
-	def invoke(B,cli,args=_A,input=_A,env=_A,catch_exceptions=True,color=_D,**G):
+	def invoke(B,cli,args=_A,input=_A,env=_A,catch_exceptions=True,color=_C,**G):
 		C=args;E=_A
 		with B.isolation(input=input,env=env,color=color)as H:
 			F=_A;A=0
 			if isinstance(C,str):C=shlex.split(C)
 			try:I=G.pop('prog_name')
 			except KeyError:I=B.get_default_prog_name(cli)
 			try:cli.main(args=C or(),prog_name=I,**G)
 			except SystemExit as D:
 				E=sys.exc_info();A=D.code
 				if A is _A:A=0
 				if A!=0:F=D
-				if not isinstance(A,int):sys.stdout.write(str(A));sys.stdout.write(_C);A=1
+				if not isinstance(A,int):sys.stdout.write(str(A));sys.stdout.write('\n');A=1
 			except Exception as D:
 				if not catch_exceptions:raise
 				F=D;A=1;E=sys.exc_info()
 			finally:
 				sys.stdout.flush();K=H[0].getvalue()
 				if B.mix_stderr:J=_A
 				else:J=H[1].getvalue()
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/click/types.py` & `dynaconf-3.2.0/dynaconf/vendor/click/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-_F='text'
 _E='replace'
 _D='utf-8'
 _C=True
 _B=False
 _A=None
 import os,stat
 from datetime import datetime
@@ -34,19 +33,19 @@
 		A=value
 		try:return B.func(A)
 		except ValueError:
 			try:A=str(A)
 			except UnicodeError:A=A.decode(_D,_E)
 			B.fail(A,param,ctx)
 class UnprocessedParamType(ParamType):
-	name=_F
+	name='text'
 	def convert(A,value,param,ctx):return value
 	def __repr__(A):return'UNPROCESSED'
 class StringParamType(ParamType):
-	name=_F
+	name='text'
 	def convert(D,value,param,ctx):
 		A=value
 		if isinstance(A,bytes):
 			B=_get_argv_encoding()
 			try:A=A.decode(B)
 			except UnicodeError:
 				C=get_filesystem_encoding()
@@ -60,16 +59,16 @@
 class Choice(ParamType):
 	name='choice'
 	def __init__(A,choices,case_sensitive=_C):A.choices=choices;A.case_sensitive=case_sensitive
 	def get_metavar(A,param):return f"[{'|'.join(A.choices)}]"
 	def get_missing_message(A,param):B=',\n\t'.join(A.choices);return f"Choose from:\n\t{B}"
 	def convert(D,value,param,ctx):
 		E=value;B=ctx;C=E;A={A:A for A in D.choices}
-		if B is not _A and B.token_normalize_func is not _A:C=B.token_normalize_func(E);A={B.token_normalize_func(C):D for(C,D)in A.items()}
-		if not D.case_sensitive:C=C.casefold();A={B.casefold():C for(B,C)in A.items()}
+		if B is not _A and B.token_normalize_func is not _A:C=B.token_normalize_func(E);A={B.token_normalize_func(A):C for(A,C)in A.items()}
+		if not D.case_sensitive:C=C.casefold();A={A.casefold():B for(A,B)in A.items()}
 		if C in A:return A[C]
 		D.fail(f"invalid choice: {E}. (choose from {', '.join(D.choices)})",param,B)
 	def __repr__(A):return f"Choice({list(A.choices)})"
 class DateTime(ParamType):
 	name='datetime'
 	def __init__(A,formats=_A):A.formats=formats or['%Y-%m-%d','%Y-%m-%dT%H:%M:%S','%Y-%m-%d %H:%M:%S']
 	def get_metavar(A,param):return f"[{'|'.join(A.formats)}]"
@@ -196,15 +195,15 @@
 	@property
 	def name(self):return f"<{' '.join((A.name for A in self.types))}>"
 	@property
 	def arity(self):return len(self.types)
 	def convert(A,value,param,ctx):
 		B=value
 		if len(B)!=len(A.types):raise TypeError('It would appear that nargs is set to conflict with the composite type arity.')
-		return tuple((C(D,param,ctx)for(C,D)in zip(A.types,B)))
+		return tuple((A(B,param,ctx)for(A,B)in zip(A.types,B)))
 def convert_type(ty,default=_A):
 	B=default;A=ty;C=_B
 	if A is _A and B is not _A:
 		if isinstance(B,tuple):A=tuple(map(type,B))
 		else:A=type(B)
 		C=_C
 	if isinstance(A,tuple):return Tuple(A)
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/click/utils.py` & `dynaconf-3.2.0/dynaconf/vendor/click/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os,sys
 from ._compat import _default_text_stderr,_default_text_stdout,_find_binary_writer,auto_wrap_for_ansi,binary_streams,filename_to_ui,get_filesystem_encoding,get_strerror,is_bytes,open_stream,should_strip_ansi,strip_ansi,text_streams,WIN
 from .globals import resolve_color_default
 echo_native_types=str,bytes,bytearray
 def _posixify(name):return '-'.join(name.split()).lower()
 def safecall(func):
 	def A(*A,**B):
-		try:return func(*A,**B)
+		try:return func(*(A),**B)
 		except Exception:pass
 	return A
 def make_str(value):
 	A=value
 	if isinstance(A,bytes):
 		try:return A.decode(get_filesystem_encoding())
 		except UnicodeError:return A.decode('utf-8','replace')
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/dotenv/__init__.py` & `dynaconf-3.2.0/dynaconf/vendor/dotenv/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 _A=None
 from .compat import IS_TYPE_CHECKING
 from .main import load_dotenv,get_key,set_key,unset_key,find_dotenv,dotenv_values
 if IS_TYPE_CHECKING:from typing import Any,Optional
 def load_ipython_extension(ipython):from .ipython import load_ipython_extension as A;A(ipython)
 def get_cli_string(path=_A,action=_A,key=_A,value=_A,quote=_A):
-	E=' ';D=quote;C=action;B=value;A=['dotenv']
+	D=quote;C=action;B=value;A=['dotenv']
 	if D:A.append('-q %s'%D)
 	if path:A.append('-f %s'%path)
 	if C:
 		A.append(C)
 		if key:
 			A.append(key)
 			if B:
-				if E in B:A.append('"%s"'%B)
+				if' 'in B:A.append('"%s"'%B)
 				else:A.append(B)
-	return E.join(A).strip()
+	return ' '.join(A).strip()
 __all__=['get_cli_string','load_dotenv','dotenv_values','get_key','set_key','unset_key','find_dotenv','load_ipython_extension']
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/dotenv/cli.py` & `dynaconf-3.2.0/dynaconf/vendor/dotenv/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,12 +45,12 @@
 	A=key;B=ctx.obj[_B];C=ctx.obj[_C];D,A=unset_key(B,A,C)
 	if D:click.echo('Successfully removed %s'%A)
 	else:exit(1)
 @cli.command(context_settings={'ignore_unknown_options':_A})
 @click.pass_context
 @click.argument('commandline',nargs=-1,type=click.UNPROCESSED)
 def run(ctx,commandline):
-	A=commandline;B=ctx.obj[_B];C={to_env(C):to_env(A)for(C,A)in dotenv_values(B).items()if A is not None}
+	A=commandline;B=ctx.obj[_B];C={to_env(B):to_env(A)for(B,A)in dotenv_values(B).items()if A is not None}
 	if not A:click.echo('No command given.');exit(1)
 	D=run_command(A,C);exit(D)
 def run_command(command,env):A=os.environ.copy();A.update(env);B=Popen(command,universal_newlines=_A,bufsize=0,shell=False,env=A);C,C=B.communicate();return B.returncode
 if __name__=='__main__':cli()
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/dotenv/ipython.py` & `dynaconf-3.2.0/dynaconf/vendor/dotenv/ipython.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 class IPythonDotEnv(Magics):
 	@magic_arguments()
 	@argument('-o','--override',action=_A,help='Indicate to override existing variables')
 	@argument('-v','--verbose',action=_A,help='Indicate function calls to be verbose')
 	@argument('dotenv_path',nargs='?',type=str,default='.env',help='Search in increasingly higher folders for the `dotenv_path`')
 	@line_magic
 	def dotenv(self,line):
-		C=True;A=parse_argstring(self.dotenv,line);B=A.dotenv_path
-		try:B=find_dotenv(B,C,C)
+		A=parse_argstring(self.dotenv,line);B=A.dotenv_path
+		try:B=find_dotenv(B,True,True)
 		except IOError:print('cannot find .env file');return
 		load_dotenv(B,verbose=A.verbose,override=A.override)
 def load_ipython_extension(ipython):ipython.register_magics(IPythonDotEnv)
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/dotenv/main.py` & `dynaconf-3.2.0/dynaconf/vendor/dotenv/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from __future__ import absolute_import,print_function,unicode_literals
-_E='.env'
 _D='always'
 _C=True
 _B=False
 _A=None
 import io,logging,os,re,shutil,sys,tempfile
 from collections import OrderedDict
 from contextlib import contextmanager
@@ -26,15 +25,15 @@
 	@contextmanager
 	def _get_stream(self):
 		A=self
 		if isinstance(A.dotenv_path,StringIO):yield A.dotenv_path
 		elif os.path.isfile(A.dotenv_path):
 			with io.open(A.dotenv_path,encoding=A.encoding)as B:yield B
 		else:
-			if A.verbose:logger.info('Python-dotenv could not find configuration file %s.',A.dotenv_path or _E)
+			if A.verbose:logger.info('Python-dotenv could not find configuration file %s.',A.dotenv_path or'.env')
 			yield StringIO('')
 	def dict(A):
 		if A._dict:return A._dict
 		B=OrderedDict(A.parse());A._dict=resolve_nested_variables(B)if A.interpolate else B;return A._dict
 	def parse(B):
 		with B._get_stream()as C:
 			for A in with_warn_for_invalid_lines(parse_stream(C)):
@@ -56,18 +55,18 @@
 		with tempfile.NamedTemporaryFile(mode='w+',delete=_B)as A:
 			with io.open(path)as B:yield(B,A)
 	except BaseException:
 		if os.path.isfile(A.name):os.unlink(A.name)
 		raise
 	else:shutil.move(A.name,path)
 def set_key(dotenv_path,key_to_set,value_to_set,quote_mode=_D):
-	K='"';E=quote_mode;C=dotenv_path;B=key_to_set;A=value_to_set;A=A.strip("'").strip(K)
+	E=quote_mode;C=dotenv_path;B=key_to_set;A=value_to_set;A=A.strip("'").strip('"')
 	if not os.path.exists(C):logger.warning("Can't write to %s - it doesn't exist.",C);return _A,B,A
 	if' 'in A:E=_D
-	if E==_D:F='"{}"'.format(A.replace(K,'\\"'))
+	if E==_D:F='"{}"'.format(A.replace('"','\\"'))
 	else:F=A
 	G='{}={}\n'.format(B,F)
 	with rewrite(C)as(J,D):
 		H=_B
 		for I in with_warn_for_invalid_lines(parse_stream(J)):
 			if I.key==B:D.write(G);H=_C
 			else:D.write(I.original.string)
@@ -91,24 +90,24 @@
 	return B
 def _walk_to_root(path):
 	A=path
 	if not os.path.exists(A):raise IOError('Starting path not found')
 	if os.path.isfile(A):A=os.path.dirname(A)
 	C=_A;B=os.path.abspath(A)
 	while C!=B:yield B;D=os.path.abspath(os.path.join(B,os.path.pardir));C,B=B,D
-def find_dotenv(filename=_E,raise_error_if_not_found=_B,usecwd=_B):
-	H='.py'
-	def E():B='__file__';A=__import__('__main__',_A,_A,fromlist=[B]);return not hasattr(A,B)
-	if usecwd or E()or getattr(sys,'frozen',_B):B=os.getcwd()
+def find_dotenv(filename='.env',raise_error_if_not_found=_B,usecwd=_B):
+	E='.py'
+	def F():A='__file__';B=__import__('__main__',_A,_A,fromlist=[A]);return not hasattr(B,A)
+	if usecwd or F()or getattr(sys,'frozen',_B):B=os.getcwd()
 	else:
 		A=sys._getframe()
-		if PY2 and not __file__.endswith(H):C=__file__.rsplit('.',1)[0]+H
+		if PY2 and not __file__.endswith(E):C=__file__.rsplit('.',1)[0]+E
 		else:C=__file__
 		while A.f_code.co_filename==C:assert A.f_back is not _A;A=A.f_back
-		F=A.f_code.co_filename;B=os.path.dirname(os.path.abspath(F))
-	for G in _walk_to_root(B):
-		D=os.path.join(G,filename)
+		G=A.f_code.co_filename;B=os.path.dirname(os.path.abspath(G))
+	for H in _walk_to_root(B):
+		D=os.path.join(H,filename)
 		if os.path.isfile(D):return D
 	if raise_error_if_not_found:raise IOError('File not found')
 	return''
 def load_dotenv(dotenv_path=_A,stream=_A,verbose=_B,override=_B,interpolate=_C,**A):B=dotenv_path or stream or find_dotenv();return DotEnv(B,verbose=verbose,interpolate=interpolate,**A).set_as_environment_variables(override=override)
 def dotenv_values(dotenv_path=_A,stream=_A,verbose=_B,interpolate=_C,**A):B=dotenv_path or stream or find_dotenv();return DotEnv(B,verbose=verbose,interpolate=interpolate,**A).dict()
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/dotenv/parser.py` & `dynaconf-3.2.0/dynaconf/vendor/dotenv/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-_I='error'
-_H='original'
-_G='value'
-_F='key'
-_E='Binding'
-_D='line'
+_E='original'
+_D='Binding'
 _C='string'
 _B='Original'
 _A=None
 import codecs,re
 from .compat import IS_TYPE_CHECKING,to_text
 if IS_TYPE_CHECKING:from typing import IO,Iterator,Match,NamedTuple,Optional,Pattern,Sequence,Text,Tuple
 def make_regex(string,extra_flags=0):return re.compile(to_text(string),re.UNICODE|extra_flags)
@@ -22,16 +18,16 @@
 _double_quoted_value=make_regex('"((?:\\\\"|[^"])*)"')
 _unquoted_value_part=make_regex('([^ \\r\\n]*)')
 _comment=make_regex('(?:[^\\S\\r\\n]*#[^\\r\\n]*)?')
 _end_of_line=make_regex('[^\\S\\r\\n]*(?:\\r\\n|\\n|\\r|$)')
 _rest_of_line=make_regex('[^\\r\\n]*(?:\\r|\\n|\\r\\n)?')
 _double_quote_escapes=make_regex('\\\\[\\\\\'\\"abfnrtv]')
 _single_quote_escapes=make_regex("\\\\[\\\\']")
-try:import typing;Original=typing.NamedTuple(_B,[(_C,typing.Text),(_D,int)]);Binding=typing.NamedTuple(_E,[(_F,typing.Optional[typing.Text]),(_G,typing.Optional[typing.Text]),(_H,Original),(_I,bool)])
-except ImportError:from collections import namedtuple;Original=namedtuple(_B,[_C,_D]);Binding=namedtuple(_E,[_F,_G,_H,_I])
+try:import typing;Original=typing.NamedTuple(_B,[(_C,typing.Text),('line',int)]);Binding=typing.NamedTuple(_D,[('key',typing.Optional[typing.Text]),('value',typing.Optional[typing.Text]),(_E,Original),('error',bool)])
+except ImportError:from collections import namedtuple;Original=namedtuple(_B,[_C,'line']);Binding=namedtuple(_D,['key','value',_E,'error'])
 class Position:
 	def __init__(A,chars,line):A.chars=chars;A.line=line
 	@classmethod
 	def start(A):return A(chars=0,line=1)
 	def set(A,other):B=other;A.chars=B.chars;A.line=B.line
 	def advance(A,string):B=string;A.chars+=len(B);A.line+=len(re.findall(_newline,B))
 class Error(Exception):0
@@ -67,19 +63,19 @@
 def parse_value(reader):
 	A=reader;B=A.peek(1)
 	if B=="'":C,=A.read_regex(_single_quoted_value);return decode_escapes(_single_quote_escapes,C)
 	elif B=='"':C,=A.read_regex(_double_quoted_value);return decode_escapes(_double_quote_escapes,C)
 	elif B in('','\n','\r'):return''
 	else:return parse_unquoted_value(A)
 def parse_binding(reader):
-	D=False;A=reader;A.set_mark()
+	C=False;A=reader;A.set_mark()
 	try:
 		A.read_regex(_multiline_whitespace)
-		if not A.has_next():return Binding(key=_A,value=_A,original=A.get_marked(),error=D)
-		A.read_regex(_export);C=parse_key(A);A.read_regex(_whitespace)
+		if not A.has_next():return Binding(key=_A,value=_A,original=A.get_marked(),error=C)
+		A.read_regex(_export);D=parse_key(A);A.read_regex(_whitespace)
 		if A.peek(1)=='=':A.read_regex(_equal_sign);B=parse_value(A)
 		else:B=_A
-		A.read_regex(_comment);A.read_regex(_end_of_line);return Binding(key=C,value=B,original=A.get_marked(),error=D)
+		A.read_regex(_comment);A.read_regex(_end_of_line);return Binding(key=D,value=B,original=A.get_marked(),error=C)
 	except Error:A.read_regex(_rest_of_line);return Binding(key=_A,value=_A,original=A.get_marked(),error=True)
 def parse_stream(stream):
 	A=Reader(stream)
 	while A.has_next():yield parse_binding(A)
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/__init__.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from __future__ import print_function,absolute_import,division,unicode_literals
-_B='yaml'
-_A=False
-if _A:from typing import Dict,Any
-_package_data=dict(full_package_name='ruamel.yaml',version_info=(0,16,10),__version__='0.16.10',author='Anthon van der Neut',author_email='a.van.der.neut@ruamel.eu',description='ruamel.yaml is a YAML parser/emitter that supports roundtrip preservation of comments, seq/map flow style, and map key order',entry_points=None,since=2014,extras_require={':platform_python_implementation=="CPython" and python_version<="2.7"':['ruamel.ordereddict'],':platform_python_implementation=="CPython" and python_version<"3.9"':['ruamel.yaml.clib>=0.1.2'],'jinja2':['ruamel.yaml.jinja2>=0.2'],'docs':['ryd']},classifiers=['Programming Language :: Python :: 2.7','Programming Language :: Python :: 3.5','Programming Language :: Python :: 3.6','Programming Language :: Python :: 3.7','Programming Language :: Python :: 3.8','Programming Language :: Python :: Implementation :: CPython','Programming Language :: Python :: Implementation :: PyPy','Programming Language :: Python :: Implementation :: Jython','Topic :: Software Development :: Libraries :: Python Modules','Topic :: Text Processing :: Markup','Typing :: Typed'],keywords='yaml 1.2 parser round-trip preserve quotes order config',read_the_docs=_B,supported=[(2,7),(3,5)],tox=dict(env='*',deps='ruamel.std.pathlib',fl8excl='_test/lib'),universal=True,rtfd=_B)
+if False:from typing import Dict,Any
+_package_data=dict(full_package_name='ruamel.yaml',version_info=(0,16,10),__version__='0.16.10',author='Anthon van der Neut',author_email='a.van.der.neut@ruamel.eu',description='ruamel.yaml is a YAML parser/emitter that supports roundtrip preservation of comments, seq/map flow style, and map key order',entry_points=None,since=2014,extras_require={':platform_python_implementation=="CPython" and python_version<="2.7"':['ruamel.ordereddict'],':platform_python_implementation=="CPython" and python_version<"3.9"':['ruamel.yaml.clib>=0.1.2'],'jinja2':['ruamel.yaml.jinja2>=0.2'],'docs':['ryd']},classifiers=['Programming Language :: Python :: 2.7','Programming Language :: Python :: 3.5','Programming Language :: Python :: 3.6','Programming Language :: Python :: 3.7','Programming Language :: Python :: 3.8','Programming Language :: Python :: Implementation :: CPython','Programming Language :: Python :: Implementation :: PyPy','Programming Language :: Python :: Implementation :: Jython','Topic :: Software Development :: Libraries :: Python Modules','Topic :: Text Processing :: Markup','Typing :: Typed'],keywords='yaml 1.2 parser round-trip preserve quotes order config',read_the_docs='yaml',supported=[(2,7),(3,5)],tox=dict(env='*',deps='ruamel.std.pathlib',fl8excl='_test/lib'),universal=True,rtfd='yaml')
 version_info=_package_data['version_info']
 __version__=_package_data['__version__']
 try:from .cyaml import *;__with_libyaml__=True
-except (ImportError,ValueError):__with_libyaml__=_A
+except (ImportError,ValueError):__with_libyaml__=False
 from dynaconf.vendor.ruamel.yaml.main import *
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/comments.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/comments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from __future__ import absolute_import,print_function
-_G='_od'
-_F='CommentedMap'
-_E='# '
+_E='CommentedMap'
 _D=True
 _C='\n'
 _B=False
 _A=None
 import sys,copy
 from .compat import ordereddict
 from .compat import PY2,string_types,MutableSliceableSequence
 from .scalarstring import ScalarString
 from .anchor import Anchor
 if PY2:from collections import MutableSet,Sized,Set,Mapping
 else:from collections.abc import MutableSet,Sized,Set,Mapping
 if _B:from typing import Any,Dict,Optional,List,Union,Optional,Iterator
-__all__=['CommentedSeq','CommentedKeySeq',_F,'CommentedOrderedMap','CommentedSet','comment_attrib','merge_attrib']
+__all__=['CommentedSeq','CommentedKeySeq',_E,'CommentedOrderedMap','CommentedSet','comment_attrib','merge_attrib']
 comment_attrib='_yaml_comment'
 format_attrib='_yaml_format'
 line_col_attrib='_yaml_line_col'
 merge_attrib='_yaml_merge'
 tag_attrib='_yaml_tag'
 class Comment:
 	__slots__='comment','_items','_end','_start';attrib=comment_attrib
@@ -92,18 +90,18 @@
 			B[3]=A[1]
 		else:B[3].extend(A[0])
 		B[2]=A[0]
 	def yaml_set_start_comment(B,comment,indent=0):
 		A=comment;from .error import CommentMark as C;from .tokens import CommentToken as D;E=B._yaml_get_pre_comment()
 		if A[-1]==_C:A=A[:-1]
 		F=C(indent)
-		for G in A.split(_C):E.append(D(_E+G+_C,F,_A))
+		for G in A.split(_C):E.append(D('# '+G+_C,F,_A))
 	def yaml_set_comment_before_after_key(J,key,before=_A,indent=0,after=_A,after_indent=_A):
 		H=indent;E=after_indent;B=after;A=before;from dynaconf.vendor.ruamel.yaml.error import CommentMark as I;from dynaconf.vendor.ruamel.yaml.tokens import CommentToken as K
-		def F(s,mark):return K((_E if s else'')+s+_C,mark,_A)
+		def F(s,mark):return K(('# 'if s else'')+s+_C,mark,_A)
 		if E is _A:E=H+2
 		if A and len(A)>1 and A[-1]==_C:A=A[:-1]
 		if B and B[-1]==_C:B=B[:-1]
 		D=I(H);C=J.ca.items.setdefault(key,[_A,[],_A,_A])
 		if A==_C:C[1].append(F('',D))
 		elif A:
 			for G in A.split(_C):C[1].append(F(G,D))
@@ -113,21 +111,21 @@
 			for G in B.split(_C):C[3].append(F(G,D))
 	@property
 	def fa(self):
 		A=self
 		if not hasattr(A,Format.attrib):setattr(A,Format.attrib,Format())
 		return getattr(A,Format.attrib)
 	def yaml_add_eol_comment(C,comment,key=NoComment,column=_A):
-		H='#';B=column;A=comment;from .tokens import CommentToken as D;from .error import CommentMark as E
+		B=column;A=comment;from .tokens import CommentToken as D;from .error import CommentMark as E
 		if B is _A:
 			try:B=C._yaml_get_column(key)
 			except AttributeError:B=0
-		if A[0]!=H:A=_E+A
+		if A[0]!='#':A='# '+A
 		if B is _A:
-			if A[0]==H:A=' '+A;B=0
+			if A[0]=='#':A=' '+A;B=0
 		F=E(B);G=[D(A,F,_A),_A];C._yaml_add_eol_comment(G,key=key)
 	@property
 	def lc(self):
 		A=self
 		if not hasattr(A,LineCol.attrib):setattr(A,LineCol.attrib,LineCol())
 		return getattr(A,LineCol.attrib)
 	def _yaml_set_line_col(A,line,col):A.lc.line=line;A.lc.col=col
@@ -154,15 +152,15 @@
 				if memo is not _A:setattr(t,A,copy.deepcopy(getattr(B,A,memo)))
 				else:setattr(t,A,getattr(B,A))
 	def _yaml_add_eol_comment(A,comment,key):raise NotImplementedError
 	def _yaml_get_pre_comment(A):raise NotImplementedError
 	def _yaml_get_column(A,key):raise NotImplementedError
 class CommentedSeq(MutableSliceableSequence,list,CommentedBase):
 	__slots__=Comment.attrib,'_lst'
-	def __init__(A,*B,**C):list.__init__(A,*B,**C)
+	def __init__(A,*B,**C):list.__init__(A,*(B),**C)
 	def __getsingleitem__(A,idx):return list.__getitem__(A,idx)
 	def __setsingleitem__(B,idx,value):
 		C=idx;A=value
 		if C<len(B):
 			if isinstance(A,string_types)and not isinstance(A,ScalarString)and isinstance(B[C],ScalarString):A=type(B[C])(A)
 		list.__setitem__(B,C,A)
 	def __delsingleitem__(A,idx=_A):
@@ -204,15 +202,15 @@
 		C=memo;B=A.__class__();C[id(A)]=B
 		for D in A:B.append(copy.deepcopy(D,C));A.copy_attributes(B,memo=C)
 		return B
 	def __add__(A,other):return list.__add__(A,other)
 	def sort(A,key=_A,reverse=_B):
 		C=reverse
 		if key is _A:B=sorted(zip(A,range(len(A))),reverse=C);list.__init__(A,[A[0]for A in B])
-		else:B=sorted(zip(map(key,list.__iter__(A)),range(len(A))),reverse=C);list.__init__(A,[list.__getitem__(A,C[1])for C in B])
+		else:B=sorted(zip(map(key,list.__iter__(A)),range(len(A))),reverse=C);list.__init__(A,[list.__getitem__(A,B[1])for B in B])
 		D=A.ca.items;A.ca._items={}
 		for (F,G) in enumerate(B):
 			E=G[1]
 			if E in D:A.ca.items[F]=D[E]
 	def __repr__(A):return list.__repr__(A)
 class CommentedKeySeq(tuple,CommentedBase):
 	def _yaml_add_comment(A,comment,key=NoComment):
@@ -265,15 +263,15 @@
 		for B in A._mapping:
 			if value==A._mapping[B]:return _D
 		return _B
 	def __iter__(A):
 		for B in A._mapping._keys():yield A._mapping[B]
 class CommentedMap(ordereddict,CommentedBase):
 	__slots__=Comment.attrib,'_ok','_ref'
-	def __init__(A,*B,**C):A._ok=set();A._ref=[];ordereddict.__init__(A,*B,**C)
+	def __init__(A,*B,**C):A._ok=set();A._ref=[];ordereddict.__init__(A,*(B),**C)
 	def _yaml_add_comment(A,comment,key=NoComment,value=NoComment):
 		C=value;B=comment
 		if key is not NoComment:A.yaml_key_comment_extend(key,B);return
 		if C is not NoComment:A.yaml_value_comment_extend(C,B)
 		else:A.ca.comment=B
 	def _yaml_add_eol_comment(A,comment,key):A._yaml_add_comment(comment,value=key)
 	def _yaml_get_columnX(A,key):return A.ca.items[key][2].start_mark.column
@@ -338,15 +336,15 @@
 	def _unmerged_contains(A,key):
 		if key in A._ok:return _D
 		return _A
 	def __contains__(A,key):return bool(ordereddict.__contains__(A,key))
 	def get(A,key,default=_A):
 		try:return A.__getitem__(key)
 		except:return default
-	def __repr__(A):return ordereddict.__repr__(A).replace(_F,'ordereddict')
+	def __repr__(A):return ordereddict.__repr__(A).replace(_E,'ordereddict')
 	def non_merged_items(A):
 		for B in ordereddict.__iter__(A):
 			if B in A._ok:yield(B,ordereddict.__getitem__(A,B))
 	def __delitem__(A,key):
 		B=key;A._ok.discard(B);ordereddict.__delitem__(A,B)
 		for C in A._ref:C.update_key_value(B)
 	def __iter__(A):
@@ -405,18 +403,18 @@
 	def __deepcopy__(A,memo):
 		C=memo;B=A.__class__();C[id(A)]=B
 		for D in A:B[D]=copy.deepcopy(A[D],C)
 		A.copy_attributes(B,memo=C);return B
 @classmethod
 def raise_immutable(cls,*A,**B):raise TypeError('{} objects are immutable'.format(cls.__name__))
 class CommentedKeyMap(CommentedBase,Mapping):
-	__slots__=Comment.attrib,_G
+	__slots__=Comment.attrib,'_od'
 	def __init__(A,*B,**C):
-		if hasattr(A,_G):raise_immutable(A)
-		try:A._od=ordereddict(*B,**C)
+		if hasattr(A,'_od'):raise_immutable(A)
+		try:A._od=ordereddict(*(B),**C)
 		except TypeError:
 			if PY2:A._od=ordereddict(B[0].items())
 			else:raise
 	__delitem__=__setitem__=clear=pop=popitem=setdefault=update=raise_immutable
 	def __getitem__(A,index):return A._od[index]
 	def __iter__(A):
 		for B in A._od.__iter__():yield B
@@ -470,16 +468,16 @@
 	def __repr__(A):return 'set({0!r})'.format(A.odict.keys())
 class TaggedScalar(CommentedBase):
 	def __init__(A,value=_A,style=_A,tag=_A):
 		A.value=value;A.style=style
 		if tag is not _A:A.yaml_set_tag(tag)
 	def __str__(A):return A.value
 def dump_comments(d,name='',sep='.',out=sys.stdout):
-	G='ca';E='{}\n';D=out;C=sep;A=name
-	if isinstance(d,dict)and hasattr(d,G):
+	E='{}\n';D=out;C=sep;A=name
+	if isinstance(d,dict)and hasattr(d,'ca'):
 		if A:sys.stdout.write(E.format(A))
 		D.write(E.format(d.ca))
 		for B in d:dump_comments(d[B],name=A+C+B if A else B,sep=C,out=D)
-	elif isinstance(d,list)and hasattr(d,G):
+	elif isinstance(d,list)and hasattr(d,'ca'):
 		if A:sys.stdout.write(E.format(A))
 		D.write(E.format(d.ca))
 		for (F,B) in enumerate(d):dump_comments(B,name=A+C+str(F)if A else str(F),sep=C,out=D)
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/compat.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 		else:_debug=int(A)
 	if val is _A:return _debug
 	return _debug&val
 class Nprint:
 	def __init__(A,file_name=_A):A._max_print=_A;A._count=_A;A._file_name=file_name
 	def __call__(A,*E,**F):
 		if not bool(_debug):return
-		B=sys.stdout if A._file_name is _A else open(A._file_name,'a');C=print;D=F.copy();D['file']=B;C(*E,**D);B.flush()
+		B=sys.stdout if A._file_name is _A else open(A._file_name,'a');C=print;D=F.copy();D['file']=B;C(*(E),**D);B.flush()
 		if A._max_print is not _A:
 			if A._count is _A:A._count=A._max_print
 			A._count-=1
 			if A._count==0:C('forced exit\n');traceback.print_stack();B.flush();sys.exit(0)
 		if A._file_name:B.close()
 	def set_max_print(A,i):A._max_print=i;A._count=_A
 nprint=Nprint()
@@ -91,27 +91,27 @@
 	if t2 is not _A and A<t2:return _A
 	return _B
 class MutableSliceableSequence(MutableSequence):
 	__slots__=()
 	def __getitem__(A,index):
 		B=index
 		if not isinstance(B,slice):return A.__getsingleitem__(B)
-		return type(A)([A[C]for C in range(*B.indices(len(A)))])
+		return type(A)([A[B]for B in range(*B.indices(len(A)))])
 	def __setitem__(C,index,value):
 		B=value;A=index
 		if not isinstance(A,slice):return C.__setsingleitem__(A,B)
 		assert iter(B)
 		if A.step is _A:
 			del C[A.start:A.stop]
 			for F in reversed(B):C.insert(0 if A.start is _A else A.start,F)
 		else:
 			D=A.indices(len(C));E=(D[1]-D[0]-1)//D[2]+1
 			if E<len(B):raise TypeError('too many elements in value {} < {}'.format(E,len(B)))
 			elif E>len(B):raise TypeError('not enough elements in value {} > {}'.format(E,len(B)))
-			for (G,H) in enumerate(range(*D)):C[H]=B[G]
+			for (G,H) in enumerate(range(*(D))):C[H]=B[G]
 	def __delitem__(A,index):
 		B=index
 		if not isinstance(B,slice):return A.__delsingleitem__(B)
 		for C in reversed(range(*B.indices(len(A)))):del A[C]
 	@abstractmethod
 	def __getsingleitem__(self,index):raise IndexError
 	@abstractmethod
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/composer.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/composer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from __future__ import absolute_import,print_function
-_B='typ'
 _A=None
 import warnings
 from .error import MarkedYAMLError,ReusedAnchorWarning
 from .compat import utf8,nprint,nprintf
 from .events import StreamStartEvent,StreamEndEvent,MappingStartEvent,MappingEndEvent,SequenceStartEvent,SequenceEndEvent,AliasEvent,ScalarEvent
 from .nodes import MappingNode,ScalarNode,SequenceNode
 if False:from typing import Any,Dict,Optional,List
@@ -13,20 +12,20 @@
 	def __init__(A,loader=_A):
 		A.loader=loader
 		if A.loader is not _A and getattr(A.loader,'_composer',_A)is _A:A.loader._composer=A
 		A.anchors={}
 	@property
 	def parser(self):
 		A=self
-		if hasattr(A.loader,_B):A.loader.parser
+		if hasattr(A.loader,'typ'):A.loader.parser
 		return A.loader._parser
 	@property
 	def resolver(self):
 		A=self
-		if hasattr(A.loader,_B):A.loader.resolver
+		if hasattr(A.loader,'typ'):A.loader.resolver
 		return A.loader._resolver
 	def check_node(A):
 		if A.parser.check_event(StreamStartEvent):A.parser.get_event()
 		return not A.parser.check_event(StreamEndEvent)
 	def get_node(A):
 		if not A.parser.check_event(StreamEndEvent):return A.compose_document()
 	def get_single_node(A):
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/constructor.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/constructor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,65 +1,57 @@
 from __future__ import print_function,absolute_import,division
-_AD='expected the empty value, but found %r'
-_AC='cannot find module %r (%s)'
-_AB='expected non-empty name appended to the tag'
-_AA='tag:yaml.org,2002:map'
-_A9='tag:yaml.org,2002:seq'
-_A8='tag:yaml.org,2002:set'
-_A7='tag:yaml.org,2002:pairs'
-_A6='tag:yaml.org,2002:omap'
-_A5='tag:yaml.org,2002:timestamp'
-_A4='tag:yaml.org,2002:binary'
-_A3='tag:yaml.org,2002:float'
-_A2='tag:yaml.org,2002:int'
-_A1='tag:yaml.org,2002:bool'
-_A0='tag:yaml.org,2002:null'
-_z='could not determine a constructor for the tag %r'
-_y='second'
-_x='minute'
-_w='day'
-_v='month'
-_u='year'
-_t='failed to construct timestamp from "{}"'
-_s='decodebytes'
-_r='failed to convert base64 data into ascii: %s'
-_q='.nan'
-_p='.inf'
-_o='expected a mapping or list of mappings for merging, but found %s'
-_n='expected a mapping for merging, but found %s'
-_m='                        Duplicate keys will become an error in future releases, and are errors\n                        by default when using the new API.\n                        '
-_l='\n                        To suppress this check see:\n                           http://yaml.readthedocs.io/en/latest/api.html#duplicate-keys\n                        '
-_k='tag:yaml.org,2002:merge'
-_j='                    Duplicate keys will become an error in future releases, and are errors\n                    by default when using the new API.\n                    '
-_i='\n                    To suppress this check see:\n                        http://yaml.readthedocs.io/en/latest/api.html#duplicate-keys\n                    '
-_h='expected a sequence node, but found %s'
-_g='expected a scalar node, but found %s'
-_f='typ'
-_e='while constructing a Python module'
-_d='expected a single mapping item, but found %d items'
-_c='expected a mapping of length 1, but found %s'
-_b='expected a sequence, but found %s'
-_a='failed to decode base64 data: %s'
-_Z='tag:yaml.org,2002:value'
-_Y='found duplicate key "{}"'
-_X='found unhashable key'
-_W='found unacceptable key (%s)'
-_V='__setstate__'
-_U='tz_hour'
-_T='hour'
-_S='ascii'
-_R='tag:yaml.org,2002:str'
-_Q='utf-8'
-_P='expected a mapping node, but found %s'
-_O='tz_minute'
-_N='e'
-_M='+-'
-_L='while constructing an ordered map'
-_K='tz_sign'
-_J='-'
+_A5='expected the empty value, but found %r'
+_A4='cannot find module %r (%s)'
+_A3='expected non-empty name appended to the tag'
+_A2='tag:yaml.org,2002:map'
+_A1='tag:yaml.org,2002:seq'
+_A0='tag:yaml.org,2002:set'
+_z='tag:yaml.org,2002:pairs'
+_y='tag:yaml.org,2002:omap'
+_x='tag:yaml.org,2002:timestamp'
+_w='tag:yaml.org,2002:binary'
+_v='tag:yaml.org,2002:float'
+_u='tag:yaml.org,2002:int'
+_t='tag:yaml.org,2002:bool'
+_s='tag:yaml.org,2002:null'
+_r='could not determine a constructor for the tag %r'
+_q='second'
+_p='minute'
+_o='failed to construct timestamp from "{}"'
+_n='decodebytes'
+_m='failed to convert base64 data into ascii: %s'
+_l='expected a mapping or list of mappings for merging, but found %s'
+_k='expected a mapping for merging, but found %s'
+_j='                        Duplicate keys will become an error in future releases, and are errors\n                        by default when using the new API.\n                        '
+_i='\n                        To suppress this check see:\n                           http://yaml.readthedocs.io/en/latest/api.html#duplicate-keys\n                        '
+_h='tag:yaml.org,2002:merge'
+_g='                    Duplicate keys will become an error in future releases, and are errors\n                    by default when using the new API.\n                    '
+_f='\n                    To suppress this check see:\n                        http://yaml.readthedocs.io/en/latest/api.html#duplicate-keys\n                    '
+_e='expected a sequence node, but found %s'
+_d='expected a scalar node, but found %s'
+_c='while constructing a Python module'
+_b='expected a single mapping item, but found %d items'
+_a='expected a mapping of length 1, but found %s'
+_Z='expected a sequence, but found %s'
+_Y='failed to decode base64 data: %s'
+_X='tag:yaml.org,2002:value'
+_W='found duplicate key "{}"'
+_V='found unhashable key'
+_U='found unacceptable key (%s)'
+_T='__setstate__'
+_S='tz_hour'
+_R='hour'
+_Q='ascii'
+_P='tag:yaml.org,2002:str'
+_O='utf-8'
+_N='expected a mapping node, but found %s'
+_M='tz_minute'
+_L='+-'
+_K='while constructing an ordered map'
+_J='tz_sign'
 _I='fraction'
 _H='.'
 _G=':'
 _F='0'
 _E='while constructing a mapping'
 _D='_'
 _C=True
@@ -89,20 +81,20 @@
 	yaml_constructors={};yaml_multi_constructors={}
 	def __init__(self,preserve_quotes=_A,loader=_A):
 		self.loader=loader
 		if self.loader is not _A and getattr(self.loader,'_constructor',_A)is _A:self.loader._constructor=self
 		self.loader=loader;self.yaml_base_dict_type=dict;self.yaml_base_list_type=list;self.constructed_objects={};self.recursive_objects={};self.state_generators=[];self.deep_construct=_B;self._preserve_quotes=preserve_quotes;self.allow_duplicate_keys=version_tnf((0,15,1),(0,16))
 	@property
 	def composer(self):
-		if hasattr(self.loader,_f):return self.loader.composer
+		if hasattr(self.loader,'typ'):return self.loader.composer
 		try:return self.loader._composer
 		except AttributeError:sys.stdout.write('slt {}\n'.format(type(self)));sys.stdout.write('slc {}\n'.format(self.loader._composer));sys.stdout.write('{}\n'.format(dir(self)));raise
 	@property
 	def resolver(self):
-		if hasattr(self.loader,_f):return self.loader.resolver
+		if hasattr(self.loader,'typ'):return self.loader.resolver
 		return self.loader._resolver
 	def check_data(self):return self.composer.check_node()
 	def get_data(self):
 		if self.composer.check_node():return self.construct_document(self.composer.get_node())
 	def get_single_data(self):
 		node=self.composer.get_single_node()
 		if node is not _A:return self.construct_document(node)
@@ -139,63 +131,63 @@
 		if isinstance(data,types.GeneratorType):
 			generator=data;data=next(generator)
 			if self.deep_construct:
 				for _dummy in generator:0
 			else:self.state_generators.append(generator)
 		return data
 	def construct_scalar(self,node):
-		if not isinstance(node,ScalarNode):raise ConstructorError(_A,_A,_g%node.id,node.start_mark)
+		if not isinstance(node,ScalarNode):raise ConstructorError(_A,_A,_d%node.id,node.start_mark)
 		return node.value
 	def construct_sequence(self,node,deep=_B):
-		if not isinstance(node,SequenceNode):raise ConstructorError(_A,_A,_h%node.id,node.start_mark)
+		if not isinstance(node,SequenceNode):raise ConstructorError(_A,_A,_e%node.id,node.start_mark)
 		return[self.construct_object(child,deep=deep)for child in node.value]
 	def construct_mapping(self,node,deep=_B):
-		if not isinstance(node,MappingNode):raise ConstructorError(_A,_A,_P%node.id,node.start_mark)
+		if not isinstance(node,MappingNode):raise ConstructorError(_A,_A,_N%node.id,node.start_mark)
 		total_mapping=self.yaml_base_dict_type()
 		if getattr(node,'merge',_A)is not _A:todo=[(node.merge,_B),(node.value,_B)]
 		else:todo=[(node.value,_C)]
 		for (values,check) in todo:
 			mapping=self.yaml_base_dict_type()
 			for (key_node,value_node) in values:
 				key=self.construct_object(key_node,deep=_C)
 				if not isinstance(key,Hashable):
 					if isinstance(key,list):key=tuple(key)
 				if PY2:
 					try:hash(key)
-					except TypeError as exc:raise ConstructorError(_E,node.start_mark,_W%exc,key_node.start_mark)
-				elif not isinstance(key,Hashable):raise ConstructorError(_E,node.start_mark,_X,key_node.start_mark)
+					except TypeError as exc:raise ConstructorError(_E,node.start_mark,_U%exc,key_node.start_mark)
+				elif not isinstance(key,Hashable):raise ConstructorError(_E,node.start_mark,_V,key_node.start_mark)
 				value=self.construct_object(value_node,deep=deep)
 				if check:
 					if self.check_mapping_key(node,key_node,mapping,key,value):mapping[key]=value
 				else:mapping[key]=value
 			total_mapping.update(mapping)
 		return total_mapping
 	def check_mapping_key(self,node,key_node,mapping,key,value):
 		if key in mapping:
 			if not self.allow_duplicate_keys:
 				mk=mapping.get(key)
 				if PY2:
-					if isinstance(key,unicode):key=key.encode(_Q)
-					if isinstance(value,unicode):value=value.encode(_Q)
-					if isinstance(mk,unicode):mk=mk.encode(_Q)
-				args=[_E,node.start_mark,'found duplicate key "{}" with value "{}" (original value: "{}")'.format(key,value,mk),key_node.start_mark,_i,_j]
-				if self.allow_duplicate_keys is _A:warnings.warn(DuplicateKeyFutureWarning(*args))
-				else:raise DuplicateKeyError(*args)
+					if isinstance(key,unicode):key=key.encode(_O)
+					if isinstance(value,unicode):value=value.encode(_O)
+					if isinstance(mk,unicode):mk=mk.encode(_O)
+				args=[_E,node.start_mark,'found duplicate key "{}" with value "{}" (original value: "{}")'.format(key,value,mk),key_node.start_mark,_f,_g]
+				if self.allow_duplicate_keys is _A:warnings.warn(DuplicateKeyFutureWarning(*(args)))
+				else:raise DuplicateKeyError(*(args))
 			return _B
 		return _C
 	def check_set_key(self,node,key_node,setting,key):
 		if key in setting:
 			if not self.allow_duplicate_keys:
 				if PY2:
-					if isinstance(key,unicode):key=key.encode(_Q)
-				args=['while constructing a set',node.start_mark,_Y.format(key),key_node.start_mark,_i,_j]
-				if self.allow_duplicate_keys is _A:warnings.warn(DuplicateKeyFutureWarning(*args))
-				else:raise DuplicateKeyError(*args)
+					if isinstance(key,unicode):key=key.encode(_O)
+				args=['while constructing a set',node.start_mark,_W.format(key),key_node.start_mark,_f,_g]
+				if self.allow_duplicate_keys is _A:warnings.warn(DuplicateKeyFutureWarning(*(args)))
+				else:raise DuplicateKeyError(*(args))
 	def construct_pairs(self,node,deep=_B):
-		if not isinstance(node,MappingNode):raise ConstructorError(_A,_A,_P%node.id,node.start_mark)
+		if not isinstance(node,MappingNode):raise ConstructorError(_A,_A,_N%node.id,node.start_mark)
 		pairs=[]
 		for (key_node,value_node) in node.value:key=self.construct_object(key_node,deep=deep);value=self.construct_object(value_node,deep=deep);pairs.append((key,value))
 		return pairs
 	@classmethod
 	def add_constructor(cls,tag,constructor):
 		if'yaml_constructors'not in cls.__dict__:cls.yaml_constructors=cls.yaml_constructors.copy()
 		cls.yaml_constructors[tag]=constructor
@@ -203,49 +195,49 @@
 	def add_multi_constructor(cls,tag_prefix,multi_constructor):
 		if'yaml_multi_constructors'not in cls.__dict__:cls.yaml_multi_constructors=cls.yaml_multi_constructors.copy()
 		cls.yaml_multi_constructors[tag_prefix]=multi_constructor
 class SafeConstructor(BaseConstructor):
 	def construct_scalar(self,node):
 		if isinstance(node,MappingNode):
 			for (key_node,value_node) in node.value:
-				if key_node.tag==_Z:return self.construct_scalar(value_node)
+				if key_node.tag==_X:return self.construct_scalar(value_node)
 		return BaseConstructor.construct_scalar(self,node)
 	def flatten_mapping(self,node):
 		merge=[];index=0
 		while index<len(node.value):
 			key_node,value_node=node.value[index]
-			if key_node.tag==_k:
+			if key_node.tag==_h:
 				if merge:
 					if self.allow_duplicate_keys:del node.value[index];index+=1;continue
-					args=[_E,node.start_mark,_Y.format(key_node.value),key_node.start_mark,_l,_m]
-					if self.allow_duplicate_keys is _A:warnings.warn(DuplicateKeyFutureWarning(*args))
-					else:raise DuplicateKeyError(*args)
+					args=[_E,node.start_mark,_W.format(key_node.value),key_node.start_mark,_i,_j]
+					if self.allow_duplicate_keys is _A:warnings.warn(DuplicateKeyFutureWarning(*(args)))
+					else:raise DuplicateKeyError(*(args))
 				del node.value[index]
 				if isinstance(value_node,MappingNode):self.flatten_mapping(value_node);merge.extend(value_node.value)
 				elif isinstance(value_node,SequenceNode):
 					submerge=[]
 					for subnode in value_node.value:
-						if not isinstance(subnode,MappingNode):raise ConstructorError(_E,node.start_mark,_n%subnode.id,subnode.start_mark)
+						if not isinstance(subnode,MappingNode):raise ConstructorError(_E,node.start_mark,_k%subnode.id,subnode.start_mark)
 						self.flatten_mapping(subnode);submerge.append(subnode.value)
 					submerge.reverse()
 					for value in submerge:merge.extend(value)
-				else:raise ConstructorError(_E,node.start_mark,_o%value_node.id,value_node.start_mark)
-			elif key_node.tag==_Z:key_node.tag=_R;index+=1
+				else:raise ConstructorError(_E,node.start_mark,_l%value_node.id,value_node.start_mark)
+			elif key_node.tag==_X:key_node.tag=_P;index+=1
 			else:index+=1
 		if bool(merge):node.merge=merge;node.value=merge+node.value
 	def construct_mapping(self,node,deep=_B):
 		if isinstance(node,MappingNode):self.flatten_mapping(node)
 		return BaseConstructor.construct_mapping(self,node,deep=deep)
 	def construct_yaml_null(self,node):self.construct_scalar(node);return _A
 	bool_values={'yes':_C,'no':_B,'y':_C,'n':_B,'true':_C,'false':_B,'on':_C,'off':_B}
 	def construct_yaml_bool(self,node):value=self.construct_scalar(node);return self.bool_values[value.lower()]
 	def construct_yaml_int(self,node):
 		value_s=to_str(self.construct_scalar(node));value_s=value_s.replace(_D,'');sign=+1
-		if value_s[0]==_J:sign=-1
-		if value_s[0]in _M:value_s=value_s[1:]
+		if value_s[0]=='-':sign=-1
+		if value_s[0]in _L:value_s=value_s[1:]
 		if value_s==_F:return 0
 		elif value_s.startswith('0b'):return sign*int(value_s[2:],2)
 		elif value_s.startswith('0x'):return sign*int(value_s[2:],16)
 		elif value_s.startswith('0o'):return sign*int(value_s[2:],8)
 		elif self.resolver.processing_version==(1,1)and value_s[0]==_F:return sign*int(value_s,8)
 		elif self.resolver.processing_version==(1,1)and _G in value_s:
 			digits=[int(part)for part in value_s.split(_G)];digits.reverse();base=1;value=0
@@ -253,170 +245,170 @@
 			return sign*value
 		else:return sign*int(value_s)
 	inf_value=1e+300
 	while inf_value!=inf_value*inf_value:inf_value*=inf_value
 	nan_value=-inf_value/inf_value
 	def construct_yaml_float(self,node):
 		value_so=to_str(self.construct_scalar(node));value_s=value_so.replace(_D,'').lower();sign=+1
-		if value_s[0]==_J:sign=-1
-		if value_s[0]in _M:value_s=value_s[1:]
-		if value_s==_p:return sign*self.inf_value
-		elif value_s==_q:return self.nan_value
+		if value_s[0]=='-':sign=-1
+		if value_s[0]in _L:value_s=value_s[1:]
+		if value_s=='.inf':return sign*self.inf_value
+		elif value_s=='.nan':return self.nan_value
 		elif self.resolver.processing_version!=(1,2)and _G in value_s:
 			digits=[float(part)for part in value_s.split(_G)];digits.reverse();base=1;value=0.0
 			for digit in digits:value+=digit*base;base*=60
 			return sign*value
 		else:
-			if self.resolver.processing_version!=(1,2)and _N in value_s:
-				mantissa,exponent=value_s.split(_N)
+			if self.resolver.processing_version!=(1,2)and'e'in value_s:
+				mantissa,exponent=value_s.split('e')
 				if _H not in mantissa:warnings.warn(MantissaNoDotYAML1_1Warning(node,value_so))
 			return sign*float(value_s)
 	if PY3:
 		def construct_yaml_binary(self,node):
-			try:value=self.construct_scalar(node).encode(_S)
-			except UnicodeEncodeError as exc:raise ConstructorError(_A,_A,_r%exc,node.start_mark)
+			try:value=self.construct_scalar(node).encode(_Q)
+			except UnicodeEncodeError as exc:raise ConstructorError(_A,_A,_m%exc,node.start_mark)
 			try:
-				if hasattr(base64,_s):return base64.decodebytes(value)
+				if hasattr(base64,_n):return base64.decodebytes(value)
 				else:return base64.decodestring(value)
-			except binascii.Error as exc:raise ConstructorError(_A,_A,_a%exc,node.start_mark)
+			except binascii.Error as exc:raise ConstructorError(_A,_A,_Y%exc,node.start_mark)
 	else:
 		def construct_yaml_binary(self,node):
 			value=self.construct_scalar(node)
 			try:return to_str(value).decode('base64')
-			except (binascii.Error,UnicodeEncodeError)as exc:raise ConstructorError(_A,_A,_a%exc,node.start_mark)
+			except (binascii.Error,UnicodeEncodeError)as exc:raise ConstructorError(_A,_A,_Y%exc,node.start_mark)
 	timestamp_regexp=RegExp('^(?P<year>[0-9][0-9][0-9][0-9])\n          -(?P<month>[0-9][0-9]?)\n          -(?P<day>[0-9][0-9]?)\n          (?:((?P<t>[Tt])|[ \\t]+)   # explictly not retaining extra spaces\n          (?P<hour>[0-9][0-9]?)\n          :(?P<minute>[0-9][0-9])\n          :(?P<second>[0-9][0-9])\n          (?:\\.(?P<fraction>[0-9]*))?\n          (?:[ \\t]*(?P<tz>Z|(?P<tz_sign>[-+])(?P<tz_hour>[0-9][0-9]?)\n          (?::(?P<tz_minute>[0-9][0-9]))?))?)?$',re.X)
 	def construct_yaml_timestamp(self,node,values=_A):
 		if values is _A:
 			try:match=self.timestamp_regexp.match(node.value)
 			except TypeError:match=_A
-			if match is _A:raise ConstructorError(_A,_A,_t.format(node.value),node.start_mark)
+			if match is _A:raise ConstructorError(_A,_A,_o.format(node.value),node.start_mark)
 			values=match.groupdict()
-		year=int(values[_u]);month=int(values[_v]);day=int(values[_w])
-		if not values[_T]:return datetime.date(year,month,day)
-		hour=int(values[_T]);minute=int(values[_x]);second=int(values[_y]);fraction=0
+		year=int(values['year']);month=int(values['month']);day=int(values['day'])
+		if not values[_R]:return datetime.date(year,month,day)
+		hour=int(values[_R]);minute=int(values[_p]);second=int(values[_q]);fraction=0
 		if values[_I]:
 			fraction_s=values[_I][:6]
 			while len(fraction_s)<6:fraction_s+=_F
 			fraction=int(fraction_s)
 			if len(values[_I])>6 and int(values[_I][6])>4:fraction+=1
 		delta=_A
-		if values[_K]:
-			tz_hour=int(values[_U]);minutes=values[_O];tz_minute=int(minutes)if minutes else 0;delta=datetime.timedelta(hours=tz_hour,minutes=tz_minute)
-			if values[_K]==_J:delta=-delta
+		if values[_J]:
+			tz_hour=int(values[_S]);minutes=values[_M];tz_minute=int(minutes)if minutes else 0;delta=datetime.timedelta(hours=tz_hour,minutes=tz_minute)
+			if values[_J]=='-':delta=-delta
 		data=datetime.datetime(year,month,day,hour,minute,second,fraction)
 		if delta:data-=delta
 		return data
 	def construct_yaml_omap(self,node):
 		omap=ordereddict();yield omap
-		if not isinstance(node,SequenceNode):raise ConstructorError(_L,node.start_mark,_b%node.id,node.start_mark)
+		if not isinstance(node,SequenceNode):raise ConstructorError(_K,node.start_mark,_Z%node.id,node.start_mark)
 		for subnode in node.value:
-			if not isinstance(subnode,MappingNode):raise ConstructorError(_L,node.start_mark,_c%subnode.id,subnode.start_mark)
-			if len(subnode.value)!=1:raise ConstructorError(_L,node.start_mark,_d%len(subnode.value),subnode.start_mark)
+			if not isinstance(subnode,MappingNode):raise ConstructorError(_K,node.start_mark,_a%subnode.id,subnode.start_mark)
+			if len(subnode.value)!=1:raise ConstructorError(_K,node.start_mark,_b%len(subnode.value),subnode.start_mark)
 			key_node,value_node=subnode.value[0];key=self.construct_object(key_node);assert key not in omap;value=self.construct_object(value_node);omap[key]=value
 	def construct_yaml_pairs(self,node):
 		A='while constructing pairs';pairs=[];yield pairs
-		if not isinstance(node,SequenceNode):raise ConstructorError(A,node.start_mark,_b%node.id,node.start_mark)
+		if not isinstance(node,SequenceNode):raise ConstructorError(A,node.start_mark,_Z%node.id,node.start_mark)
 		for subnode in node.value:
-			if not isinstance(subnode,MappingNode):raise ConstructorError(A,node.start_mark,_c%subnode.id,subnode.start_mark)
-			if len(subnode.value)!=1:raise ConstructorError(A,node.start_mark,_d%len(subnode.value),subnode.start_mark)
+			if not isinstance(subnode,MappingNode):raise ConstructorError(A,node.start_mark,_a%subnode.id,subnode.start_mark)
+			if len(subnode.value)!=1:raise ConstructorError(A,node.start_mark,_b%len(subnode.value),subnode.start_mark)
 			key_node,value_node=subnode.value[0];key=self.construct_object(key_node);value=self.construct_object(value_node);pairs.append((key,value))
 	def construct_yaml_set(self,node):data=set();yield data;value=self.construct_mapping(node);data.update(value)
 	def construct_yaml_str(self,node):
 		value=self.construct_scalar(node)
 		if PY3:return value
-		try:return value.encode(_S)
+		try:return value.encode(_Q)
 		except UnicodeEncodeError:return value
 	def construct_yaml_seq(self,node):data=self.yaml_base_list_type();yield data;data.extend(self.construct_sequence(node))
 	def construct_yaml_map(self,node):data=self.yaml_base_dict_type();yield data;value=self.construct_mapping(node);data.update(value)
 	def construct_yaml_object(self,node,cls):
 		data=cls.__new__(cls);yield data
-		if hasattr(data,_V):state=self.construct_mapping(node,deep=_C);data.__setstate__(state)
+		if hasattr(data,_T):state=self.construct_mapping(node,deep=_C);data.__setstate__(state)
 		else:state=self.construct_mapping(node);data.__dict__.update(state)
-	def construct_undefined(self,node):raise ConstructorError(_A,_A,_z%utf8(node.tag),node.start_mark)
-SafeConstructor.add_constructor(_A0,SafeConstructor.construct_yaml_null)
-SafeConstructor.add_constructor(_A1,SafeConstructor.construct_yaml_bool)
-SafeConstructor.add_constructor(_A2,SafeConstructor.construct_yaml_int)
-SafeConstructor.add_constructor(_A3,SafeConstructor.construct_yaml_float)
-SafeConstructor.add_constructor(_A4,SafeConstructor.construct_yaml_binary)
-SafeConstructor.add_constructor(_A5,SafeConstructor.construct_yaml_timestamp)
-SafeConstructor.add_constructor(_A6,SafeConstructor.construct_yaml_omap)
-SafeConstructor.add_constructor(_A7,SafeConstructor.construct_yaml_pairs)
-SafeConstructor.add_constructor(_A8,SafeConstructor.construct_yaml_set)
-SafeConstructor.add_constructor(_R,SafeConstructor.construct_yaml_str)
-SafeConstructor.add_constructor(_A9,SafeConstructor.construct_yaml_seq)
-SafeConstructor.add_constructor(_AA,SafeConstructor.construct_yaml_map)
+	def construct_undefined(self,node):raise ConstructorError(_A,_A,_r%utf8(node.tag),node.start_mark)
+SafeConstructor.add_constructor(_s,SafeConstructor.construct_yaml_null)
+SafeConstructor.add_constructor(_t,SafeConstructor.construct_yaml_bool)
+SafeConstructor.add_constructor(_u,SafeConstructor.construct_yaml_int)
+SafeConstructor.add_constructor(_v,SafeConstructor.construct_yaml_float)
+SafeConstructor.add_constructor(_w,SafeConstructor.construct_yaml_binary)
+SafeConstructor.add_constructor(_x,SafeConstructor.construct_yaml_timestamp)
+SafeConstructor.add_constructor(_y,SafeConstructor.construct_yaml_omap)
+SafeConstructor.add_constructor(_z,SafeConstructor.construct_yaml_pairs)
+SafeConstructor.add_constructor(_A0,SafeConstructor.construct_yaml_set)
+SafeConstructor.add_constructor(_P,SafeConstructor.construct_yaml_str)
+SafeConstructor.add_constructor(_A1,SafeConstructor.construct_yaml_seq)
+SafeConstructor.add_constructor(_A2,SafeConstructor.construct_yaml_map)
 SafeConstructor.add_constructor(_A,SafeConstructor.construct_undefined)
 if PY2:
 	class classobj:0
 class Constructor(SafeConstructor):
 	def construct_python_str(self,node):return utf8(self.construct_scalar(node))
 	def construct_python_unicode(self,node):return self.construct_scalar(node)
 	if PY3:
 		def construct_python_bytes(self,node):
-			try:value=self.construct_scalar(node).encode(_S)
-			except UnicodeEncodeError as exc:raise ConstructorError(_A,_A,_r%exc,node.start_mark)
+			try:value=self.construct_scalar(node).encode(_Q)
+			except UnicodeEncodeError as exc:raise ConstructorError(_A,_A,_m%exc,node.start_mark)
 			try:
-				if hasattr(base64,_s):return base64.decodebytes(value)
+				if hasattr(base64,_n):return base64.decodebytes(value)
 				else:return base64.decodestring(value)
-			except binascii.Error as exc:raise ConstructorError(_A,_A,_a%exc,node.start_mark)
+			except binascii.Error as exc:raise ConstructorError(_A,_A,_Y%exc,node.start_mark)
 	def construct_python_long(self,node):
 		val=self.construct_yaml_int(node)
 		if PY3:return val
 		return int(val)
 	def construct_python_complex(self,node):return complex(self.construct_scalar(node))
 	def construct_python_tuple(self,node):return tuple(self.construct_sequence(node))
 	def find_python_module(self,name,mark):
-		if not name:raise ConstructorError(_e,mark,_AB,mark)
+		if not name:raise ConstructorError(_c,mark,_A3,mark)
 		try:__import__(name)
-		except ImportError as exc:raise ConstructorError(_e,mark,_AC%(utf8(name),exc),mark)
+		except ImportError as exc:raise ConstructorError(_c,mark,_A4%(utf8(name),exc),mark)
 		return sys.modules[name]
 	def find_python_name(self,name,mark):
 		A='while constructing a Python object'
-		if not name:raise ConstructorError(A,mark,_AB,mark)
+		if not name:raise ConstructorError(A,mark,_A3,mark)
 		if _H in name:
 			lname=name.split(_H);lmodule_name=lname;lobject_name=[]
 			while len(lmodule_name)>1:
 				lobject_name.insert(0,lmodule_name.pop());module_name=_H.join(lmodule_name)
 				try:__import__(module_name);break
 				except ImportError:continue
 		else:module_name=builtins_module;lobject_name=[name]
 		try:__import__(module_name)
-		except ImportError as exc:raise ConstructorError(A,mark,_AC%(utf8(module_name),exc),mark)
+		except ImportError as exc:raise ConstructorError(A,mark,_A4%(utf8(module_name),exc),mark)
 		module=sys.modules[module_name];object_name=_H.join(lobject_name);obj=module
 		while lobject_name:
 			if not hasattr(obj,lobject_name[0]):raise ConstructorError(A,mark,'cannot find %r in the module %r'%(utf8(object_name),module.__name__),mark)
 			obj=getattr(obj,lobject_name.pop(0))
 		return obj
 	def construct_python_name(self,suffix,node):
 		value=self.construct_scalar(node)
-		if value:raise ConstructorError('while constructing a Python name',node.start_mark,_AD%utf8(value),node.start_mark)
+		if value:raise ConstructorError('while constructing a Python name',node.start_mark,_A5%utf8(value),node.start_mark)
 		return self.find_python_name(suffix,node.start_mark)
 	def construct_python_module(self,suffix,node):
 		value=self.construct_scalar(node)
-		if value:raise ConstructorError(_e,node.start_mark,_AD%utf8(value),node.start_mark)
+		if value:raise ConstructorError(_c,node.start_mark,_A5%utf8(value),node.start_mark)
 		return self.find_python_module(suffix,node.start_mark)
 	def make_python_instance(self,suffix,node,args=_A,kwds=_A,newobj=_B):
 		if not args:args=[]
 		if not kwds:kwds={}
 		cls=self.find_python_name(suffix,node.start_mark)
 		if PY3:
-			if newobj and isinstance(cls,type):return cls.__new__(cls,*args,**kwds)
-			else:return cls(*args,**kwds)
+			if newobj and isinstance(cls,type):return cls.__new__(cls,*(args),**kwds)
+			else:return cls(*(args),**kwds)
 		elif newobj and isinstance(cls,type(classobj))and not args and not kwds:instance=classobj();instance.__class__=cls;return instance
-		elif newobj and isinstance(cls,type):return cls.__new__(cls,*args,**kwds)
-		else:return cls(*args,**kwds)
+		elif newobj and isinstance(cls,type):return cls.__new__(cls,*(args),**kwds)
+		else:return cls(*(args),**kwds)
 	def set_python_instance_state(self,instance,state):
-		if hasattr(instance,_V):instance.__setstate__(state)
+		if hasattr(instance,_T):instance.__setstate__(state)
 		else:
 			slotstate={}
 			if isinstance(state,tuple)and len(state)==2:state,slotstate=state
 			if hasattr(instance,'__dict__'):instance.__dict__.update(state)
 			elif state:slotstate.update(state)
 			for (key,value) in slotstate.items():setattr(instance,key,value)
-	def construct_python_object(self,suffix,node):instance=self.make_python_instance(suffix,node,newobj=_C);self.recursive_objects[node]=instance;yield instance;deep=hasattr(instance,_V);state=self.construct_mapping(node,deep=deep);self.set_python_instance_state(instance,state)
+	def construct_python_object(self,suffix,node):instance=self.make_python_instance(suffix,node,newobj=_C);self.recursive_objects[node]=instance;yield instance;deep=hasattr(instance,_T);state=self.construct_mapping(node,deep=deep);self.set_python_instance_state(instance,state)
 	def construct_python_object_apply(self,suffix,node,newobj=_B):
 		if isinstance(node,SequenceNode):args=self.construct_sequence(node,deep=_C);kwds={};state={};listitems=[];dictitems={}
 		else:value=self.construct_mapping(node,deep=_C);args=value.get('args',[]);kwds=value.get('kwds',{});state=value.get('state',{});listitems=value.get('listitems',[]);dictitems=value.get('dictitems',{})
 		instance=self.make_python_instance(suffix,node,args,kwds,newobj)
 		if bool(state):self.set_python_instance_state(instance,state)
 		if bool(listitems):instance.extend(listitems)
 		if bool(dictitems):
@@ -439,15 +431,15 @@
 Constructor.add_multi_constructor('tag:yaml.org,2002:python/module:',Constructor.construct_python_module)
 Constructor.add_multi_constructor('tag:yaml.org,2002:python/object:',Constructor.construct_python_object)
 Constructor.add_multi_constructor('tag:yaml.org,2002:python/object/apply:',Constructor.construct_python_object_apply)
 Constructor.add_multi_constructor('tag:yaml.org,2002:python/object/new:',Constructor.construct_python_object_new)
 class RoundTripConstructor(SafeConstructor):
 	def construct_scalar(self,node):
 		A='\x07'
-		if not isinstance(node,ScalarNode):raise ConstructorError(_A,_A,_g%node.id,node.start_mark)
+		if not isinstance(node,ScalarNode):raise ConstructorError(_A,_A,_d%node.id,node.start_mark)
 		if node.style=='|'and isinstance(node.value,text_type):
 			lss=LiteralScalarString(node.value,anchor=node.anchor)
 			if node.comment and node.comment[1]:lss.comment=node.comment[1][0]
 			return lss
 		if node.style=='>'and isinstance(node.value,text_type):
 			fold_positions=[];idx=-1
 			while _C:
@@ -465,16 +457,16 @@
 		return node.value
 	def construct_yaml_int(self,node):
 		width=_A;value_su=to_str(self.construct_scalar(node))
 		try:sx=value_su.rstrip(_D);underscore=[len(sx)-sx.rindex(_D)-1,_B,_B]
 		except ValueError:underscore=_A
 		except IndexError:underscore=_A
 		value_s=value_su.replace(_D,'');sign=+1
-		if value_s[0]==_J:sign=-1
-		if value_s[0]in _M:value_s=value_s[1:]
+		if value_s[0]=='-':sign=-1
+		if value_s[0]in _L:value_s=value_s[1:]
 		if value_s==_F:return 0
 		elif value_s.startswith('0b'):
 			if self.resolver.processing_version>(1,1)and value_s[2]==_F:width=len(value_s[2:])
 			if underscore is not _A:underscore[1]=value_su[2]==_D;underscore[2]=len(value_su[2:])>1 and value_su[-1]==_D
 			return BinaryInt(sign*int(value_s[2:],2),width=width,underscore=underscore,anchor=node.anchor)
 		elif value_s.startswith('0x'):
 			if self.resolver.processing_version>(1,1)and value_s[2]==_F:width=len(value_s[2:])
@@ -496,48 +488,47 @@
 		elif self.resolver.processing_version>(1,1)and value_s[0]==_F:
 			if underscore is not _A:underscore[2]=len(value_su)>1 and value_su[-1]==_D
 			return ScalarInt(sign*int(value_s),width=len(value_s),underscore=underscore)
 		elif underscore:underscore[2]=len(value_su)>1 and value_su[-1]==_D;return ScalarInt(sign*int(value_s),width=_A,underscore=underscore,anchor=node.anchor)
 		elif node.anchor:return ScalarInt(sign*int(value_s),width=_A,anchor=node.anchor)
 		else:return sign*int(value_s)
 	def construct_yaml_float(self,node):
-		A='E'
 		def leading_zeros(v):
 			lead0=0;idx=0
 			while idx<len(v)and v[idx]in'0.':
 				if v[idx]==_F:lead0+=1
 				idx+=1
 			return lead0
 		m_sign=_B;value_so=to_str(self.construct_scalar(node));value_s=value_so.replace(_D,'').lower();sign=+1
-		if value_s[0]==_J:sign=-1
-		if value_s[0]in _M:m_sign=value_s[0];value_s=value_s[1:]
-		if value_s==_p:return sign*self.inf_value
-		if value_s==_q:return self.nan_value
+		if value_s[0]=='-':sign=-1
+		if value_s[0]in _L:m_sign=value_s[0];value_s=value_s[1:]
+		if value_s=='.inf':return sign*self.inf_value
+		if value_s=='.nan':return self.nan_value
 		if self.resolver.processing_version!=(1,2)and _G in value_s:
 			digits=[float(part)for part in value_s.split(_G)];digits.reverse();base=1;value=0.0
 			for digit in digits:value+=digit*base;base*=60
 			return sign*value
-		if _N in value_s:
-			try:mantissa,exponent=value_so.split(_N);exp=_N
-			except ValueError:mantissa,exponent=value_so.split(A);exp=A
+		if'e'in value_s:
+			try:mantissa,exponent=value_so.split('e');exp='e'
+			except ValueError:mantissa,exponent=value_so.split('E');exp='E'
 			if self.resolver.processing_version!=(1,2):
 				if _H not in mantissa:warnings.warn(MantissaNoDotYAML1_1Warning(node,value_so))
 			lead0=leading_zeros(mantissa);width=len(mantissa);prec=mantissa.find(_H)
 			if m_sign:width-=1
-			e_width=len(exponent);e_sign=exponent[0]in _M;return ScalarFloat(sign*float(value_s),width=width,prec=prec,m_sign=m_sign,m_lead0=lead0,exp=exp,e_width=e_width,e_sign=e_sign,anchor=node.anchor)
+			e_width=len(exponent);e_sign=exponent[0]in _L;return ScalarFloat(sign*float(value_s),width=width,prec=prec,m_sign=m_sign,m_lead0=lead0,exp=exp,e_width=e_width,e_sign=e_sign,anchor=node.anchor)
 		width=len(value_so);prec=value_so.index(_H);lead0=leading_zeros(value_so);return ScalarFloat(sign*float(value_s),width=width,prec=prec,m_sign=m_sign,m_lead0=lead0,anchor=node.anchor)
 	def construct_yaml_str(self,node):
 		value=self.construct_scalar(node)
 		if isinstance(value,ScalarString):return value
 		if PY3:return value
-		try:return value.encode(_S)
+		try:return value.encode(_Q)
 		except AttributeError:return value
 		except UnicodeEncodeError:return value
 	def construct_rt_sequence(self,node,seqtyp,deep=_B):
-		if not isinstance(node,SequenceNode):raise ConstructorError(_A,_A,_h%node.id,node.start_mark)
+		if not isinstance(node,SequenceNode):raise ConstructorError(_A,_A,_e%node.id,node.start_mark)
 		ret_val=[]
 		if node.comment:
 			seqtyp._yaml_add_comment(node.comment[:2])
 			if len(node.comment)>2:seqtyp.yaml_end_comment_extend(node.comment[2],clear=_C)
 		if node.anchor:
 			from dynaconf.vendor.ruamel.yaml.serializer import templated_id
 			if not templated_id(node.anchor):seqtyp.yaml_set_anchor(node.anchor)
@@ -549,33 +540,33 @@
 		def constructed(value_node):
 			if value_node in self.constructed_objects:value=self.constructed_objects[value_node]
 			else:value=self.construct_object(value_node,deep=_B)
 			return value
 		merge_map_list=[];index=0
 		while index<len(node.value):
 			key_node,value_node=node.value[index]
-			if key_node.tag==_k:
+			if key_node.tag==_h:
 				if merge_map_list:
 					if self.allow_duplicate_keys:del node.value[index];index+=1;continue
-					args=[_E,node.start_mark,_Y.format(key_node.value),key_node.start_mark,_l,_m]
-					if self.allow_duplicate_keys is _A:warnings.warn(DuplicateKeyFutureWarning(*args))
-					else:raise DuplicateKeyError(*args)
+					args=[_E,node.start_mark,_W.format(key_node.value),key_node.start_mark,_i,_j]
+					if self.allow_duplicate_keys is _A:warnings.warn(DuplicateKeyFutureWarning(*(args)))
+					else:raise DuplicateKeyError(*(args))
 				del node.value[index]
 				if isinstance(value_node,MappingNode):merge_map_list.append((index,constructed(value_node)))
 				elif isinstance(value_node,SequenceNode):
 					for subnode in value_node.value:
-						if not isinstance(subnode,MappingNode):raise ConstructorError(_E,node.start_mark,_n%subnode.id,subnode.start_mark)
+						if not isinstance(subnode,MappingNode):raise ConstructorError(_E,node.start_mark,_k%subnode.id,subnode.start_mark)
 						merge_map_list.append((index,constructed(subnode)))
-				else:raise ConstructorError(_E,node.start_mark,_o%value_node.id,value_node.start_mark)
-			elif key_node.tag==_Z:key_node.tag=_R;index+=1
+				else:raise ConstructorError(_E,node.start_mark,_l%value_node.id,value_node.start_mark)
+			elif key_node.tag==_X:key_node.tag=_P;index+=1
 			else:index+=1
 		return merge_map_list
 	def _sentinel(self):0
 	def construct_mapping(self,node,maptyp,deep=_B):
-		if not isinstance(node,MappingNode):raise ConstructorError(_A,_A,_P%node.id,node.start_mark)
+		if not isinstance(node,MappingNode):raise ConstructorError(_A,_A,_N%node.id,node.start_mark)
 		merge_map=self.flatten_mapping(node)
 		if node.comment:
 			maptyp._yaml_add_comment(node.comment[:2])
 			if len(node.comment)>2:maptyp.yaml_end_comment_extend(node.comment[2],clear=_C)
 		if node.anchor:
 			from dynaconf.vendor.ruamel.yaml.serializer import templated_id
 			if not templated_id(node.anchor):maptyp.yaml_set_anchor(node.anchor)
@@ -591,42 +582,42 @@
 				elif isinstance(key,MutableMapping):
 					key_m=CommentedKeyMap(key)
 					if key_node.flow_style is _C:key_m.fa.set_flow_style()
 					elif key_node.flow_style is _B:key_m.fa.set_block_style()
 					key=key_m
 			if PY2:
 				try:hash(key)
-				except TypeError as exc:raise ConstructorError(_E,node.start_mark,_W%exc,key_node.start_mark)
-			elif not isinstance(key,Hashable):raise ConstructorError(_E,node.start_mark,_X,key_node.start_mark)
+				except TypeError as exc:raise ConstructorError(_E,node.start_mark,_U%exc,key_node.start_mark)
+			elif not isinstance(key,Hashable):raise ConstructorError(_E,node.start_mark,_V,key_node.start_mark)
 			value=self.construct_object(value_node,deep=deep)
 			if self.check_mapping_key(node,key_node,maptyp,key,value):
 				if key_node.comment and len(key_node.comment)>4 and key_node.comment[4]:
 					if last_value is _A:key_node.comment[0]=key_node.comment.pop(4);maptyp._yaml_add_comment(key_node.comment,value=last_key)
 					else:key_node.comment[2]=key_node.comment.pop(4);maptyp._yaml_add_comment(key_node.comment,key=key)
 					key_node.comment=_A
 				if key_node.comment:maptyp._yaml_add_comment(key_node.comment,key=key)
 				if value_node.comment:maptyp._yaml_add_comment(value_node.comment,value=key)
 				maptyp._yaml_set_kv_line_col(key,[key_node.start_mark.line,key_node.start_mark.column,value_node.start_mark.line,value_node.start_mark.column]);maptyp[key]=value;last_key,last_value=key,value
 		if merge_map:maptyp.add_yaml_merge(merge_map)
 	def construct_setting(self,node,typ,deep=_B):
-		if not isinstance(node,MappingNode):raise ConstructorError(_A,_A,_P%node.id,node.start_mark)
+		if not isinstance(node,MappingNode):raise ConstructorError(_A,_A,_N%node.id,node.start_mark)
 		if node.comment:
 			typ._yaml_add_comment(node.comment[:2])
 			if len(node.comment)>2:typ.yaml_end_comment_extend(node.comment[2],clear=_C)
 		if node.anchor:
 			from dynaconf.vendor.ruamel.yaml.serializer import templated_id
 			if not templated_id(node.anchor):typ.yaml_set_anchor(node.anchor)
 		for (key_node,value_node) in node.value:
 			key=self.construct_object(key_node,deep=_C)
 			if not isinstance(key,Hashable):
 				if isinstance(key,list):key=tuple(key)
 			if PY2:
 				try:hash(key)
-				except TypeError as exc:raise ConstructorError(_E,node.start_mark,_W%exc,key_node.start_mark)
-			elif not isinstance(key,Hashable):raise ConstructorError(_E,node.start_mark,_X,key_node.start_mark)
+				except TypeError as exc:raise ConstructorError(_E,node.start_mark,_U%exc,key_node.start_mark)
+			elif not isinstance(key,Hashable):raise ConstructorError(_E,node.start_mark,_V,key_node.start_mark)
 			value=self.construct_object(value_node,deep=deep);self.check_set_key(node,key_node,typ,key)
 			if key_node.comment:typ._yaml_add_comment(key_node.comment,key=key)
 			if value_node.comment:typ._yaml_add_comment(value_node.comment,value=key)
 			typ.add(key)
 	def construct_yaml_seq(self,node):
 		data=CommentedSeq();data._yaml_set_line_col(node.start_mark.line,node.start_mark.column)
 		if node.comment:data._yaml_add_comment(node.comment)
@@ -634,28 +625,28 @@
 	def construct_yaml_map(self,node):data=CommentedMap();data._yaml_set_line_col(node.start_mark.line,node.start_mark.column);yield data;self.construct_mapping(node,data,deep=_C);self.set_collection_style(data,node)
 	def set_collection_style(self,data,node):
 		if len(data)==0:return
 		if node.flow_style is _C:data.fa.set_flow_style()
 		elif node.flow_style is _B:data.fa.set_block_style()
 	def construct_yaml_object(self,node,cls):
 		data=cls.__new__(cls);yield data
-		if hasattr(data,_V):state=SafeConstructor.construct_mapping(self,node,deep=_C);data.__setstate__(state)
+		if hasattr(data,_T):state=SafeConstructor.construct_mapping(self,node,deep=_C);data.__setstate__(state)
 		else:state=SafeConstructor.construct_mapping(self,node);data.__dict__.update(state)
 	def construct_yaml_omap(self,node):
 		omap=CommentedOrderedMap();omap._yaml_set_line_col(node.start_mark.line,node.start_mark.column)
 		if node.flow_style is _C:omap.fa.set_flow_style()
 		elif node.flow_style is _B:omap.fa.set_block_style()
 		yield omap
 		if node.comment:
 			omap._yaml_add_comment(node.comment[:2])
 			if len(node.comment)>2:omap.yaml_end_comment_extend(node.comment[2],clear=_C)
-		if not isinstance(node,SequenceNode):raise ConstructorError(_L,node.start_mark,_b%node.id,node.start_mark)
+		if not isinstance(node,SequenceNode):raise ConstructorError(_K,node.start_mark,_Z%node.id,node.start_mark)
 		for subnode in node.value:
-			if not isinstance(subnode,MappingNode):raise ConstructorError(_L,node.start_mark,_c%subnode.id,subnode.start_mark)
-			if len(subnode.value)!=1:raise ConstructorError(_L,node.start_mark,_d%len(subnode.value),subnode.start_mark)
+			if not isinstance(subnode,MappingNode):raise ConstructorError(_K,node.start_mark,_a%subnode.id,subnode.start_mark)
+			if len(subnode.value)!=1:raise ConstructorError(_K,node.start_mark,_b%len(subnode.value),subnode.start_mark)
 			key_node,value_node=subnode.value[0];key=self.construct_object(key_node);assert key not in omap;value=self.construct_object(value_node)
 			if key_node.comment:omap._yaml_add_comment(key_node.comment,key=key)
 			if subnode.comment:omap._yaml_add_comment(subnode.comment,key=key)
 			if value_node.comment:omap._yaml_add_comment(value_node.comment,value=key)
 			omap[key]=value
 	def construct_yaml_set(self,node):data=CommentedSet();data._yaml_set_line_col(node.start_mark.line,node.start_mark.column);yield data;self.construct_setting(node,data)
 	def construct_undefined(self,node):
@@ -675,54 +666,54 @@
 				data3=CommentedSeq();data3._yaml_set_line_col(node.start_mark.line,node.start_mark.column)
 				if node.flow_style is _C:data3.fa.set_flow_style()
 				elif node.flow_style is _B:data3.fa.set_block_style()
 				data3.yaml_set_tag(node.tag);yield data3
 				if node.anchor:data3.yaml_set_anchor(node.anchor)
 				data3.extend(self.construct_sequence(node));return
 		except:pass
-		raise ConstructorError(_A,_A,_z%utf8(node.tag),node.start_mark)
+		raise ConstructorError(_A,_A,_r%utf8(node.tag),node.start_mark)
 	def construct_yaml_timestamp(self,node,values=_A):
 		B='t';A='tz'
 		try:match=self.timestamp_regexp.match(node.value)
 		except TypeError:match=_A
-		if match is _A:raise ConstructorError(_A,_A,_t.format(node.value),node.start_mark)
+		if match is _A:raise ConstructorError(_A,_A,_o.format(node.value),node.start_mark)
 		values=match.groupdict()
-		if not values[_T]:return SafeConstructor.construct_yaml_timestamp(self,node,values)
-		for part in [B,_K,_U,_O]:
+		if not values[_R]:return SafeConstructor.construct_yaml_timestamp(self,node,values)
+		for part in [B,_J,_S,_M]:
 			if values[part]:break
 		else:return SafeConstructor.construct_yaml_timestamp(self,node,values)
-		year=int(values[_u]);month=int(values[_v]);day=int(values[_w]);hour=int(values[_T]);minute=int(values[_x]);second=int(values[_y]);fraction=0
+		year=int(values['year']);month=int(values['month']);day=int(values['day']);hour=int(values[_R]);minute=int(values[_p]);second=int(values[_q]);fraction=0
 		if values[_I]:
 			fraction_s=values[_I][:6]
 			while len(fraction_s)<6:fraction_s+=_F
 			fraction=int(fraction_s)
 			if len(values[_I])>6 and int(values[_I][6])>4:fraction+=1
 		delta=_A
-		if values[_K]:
-			tz_hour=int(values[_U]);minutes=values[_O];tz_minute=int(minutes)if minutes else 0;delta=datetime.timedelta(hours=tz_hour,minutes=tz_minute)
-			if values[_K]==_J:delta=-delta
+		if values[_J]:
+			tz_hour=int(values[_S]);minutes=values[_M];tz_minute=int(minutes)if minutes else 0;delta=datetime.timedelta(hours=tz_hour,minutes=tz_minute)
+			if values[_J]=='-':delta=-delta
 		if delta:
-			dt=datetime.datetime(year,month,day,hour,minute);dt-=delta;data=TimeStamp(dt.year,dt.month,dt.day,dt.hour,dt.minute,second,fraction);data._yaml['delta']=delta;tz=values[_K]+values[_U]
-			if values[_O]:tz+=_G+values[_O]
+			dt=datetime.datetime(year,month,day,hour,minute);dt-=delta;data=TimeStamp(dt.year,dt.month,dt.day,dt.hour,dt.minute,second,fraction);data._yaml['delta']=delta;tz=values[_J]+values[_S]
+			if values[_M]:tz+=_G+values[_M]
 			data._yaml[A]=tz
 		else:
 			data=TimeStamp(year,month,day,hour,minute,second,fraction)
 			if values[A]:data._yaml[A]=values[A]
 		if values[B]:data._yaml[B]=_C
 		return data
 	def construct_yaml_bool(self,node):
 		b=SafeConstructor.construct_yaml_bool(self,node)
 		if node.anchor:return ScalarBoolean(b,anchor=node.anchor)
 		return b
-RoundTripConstructor.add_constructor(_A0,RoundTripConstructor.construct_yaml_null)
-RoundTripConstructor.add_constructor(_A1,RoundTripConstructor.construct_yaml_bool)
-RoundTripConstructor.add_constructor(_A2,RoundTripConstructor.construct_yaml_int)
-RoundTripConstructor.add_constructor(_A3,RoundTripConstructor.construct_yaml_float)
-RoundTripConstructor.add_constructor(_A4,RoundTripConstructor.construct_yaml_binary)
-RoundTripConstructor.add_constructor(_A5,RoundTripConstructor.construct_yaml_timestamp)
-RoundTripConstructor.add_constructor(_A6,RoundTripConstructor.construct_yaml_omap)
-RoundTripConstructor.add_constructor(_A7,RoundTripConstructor.construct_yaml_pairs)
-RoundTripConstructor.add_constructor(_A8,RoundTripConstructor.construct_yaml_set)
-RoundTripConstructor.add_constructor(_R,RoundTripConstructor.construct_yaml_str)
-RoundTripConstructor.add_constructor(_A9,RoundTripConstructor.construct_yaml_seq)
-RoundTripConstructor.add_constructor(_AA,RoundTripConstructor.construct_yaml_map)
+RoundTripConstructor.add_constructor(_s,RoundTripConstructor.construct_yaml_null)
+RoundTripConstructor.add_constructor(_t,RoundTripConstructor.construct_yaml_bool)
+RoundTripConstructor.add_constructor(_u,RoundTripConstructor.construct_yaml_int)
+RoundTripConstructor.add_constructor(_v,RoundTripConstructor.construct_yaml_float)
+RoundTripConstructor.add_constructor(_w,RoundTripConstructor.construct_yaml_binary)
+RoundTripConstructor.add_constructor(_x,RoundTripConstructor.construct_yaml_timestamp)
+RoundTripConstructor.add_constructor(_y,RoundTripConstructor.construct_yaml_omap)
+RoundTripConstructor.add_constructor(_z,RoundTripConstructor.construct_yaml_pairs)
+RoundTripConstructor.add_constructor(_A0,RoundTripConstructor.construct_yaml_set)
+RoundTripConstructor.add_constructor(_P,RoundTripConstructor.construct_yaml_str)
+RoundTripConstructor.add_constructor(_A1,RoundTripConstructor.construct_yaml_seq)
+RoundTripConstructor.add_constructor(_A2,RoundTripConstructor.construct_yaml_map)
 RoundTripConstructor.add_constructor(_A,RoundTripConstructor.construct_undefined)
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/cyaml.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/dumper.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/emitter.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/emitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 from __future__ import absolute_import,print_function
-_a='\x07'
-_Z='\ufeff'
-_Y='\ue000'
-_X='\ud7ff'
-_W='\x85'
-_V='%%%02X'
-_U='version'
-_T="-;/?:@&=+$,_.~*'()[]"
-_S='---'
-_R=' \n\x85\u2028\u2029'
-_Q='\xa0'
-_P='a'
-_O='0'
-_N=','
-_M='...'
-_L='\\'
-_K='['
+_T='\ufeff'
+_S='\ue000'
+_R='\ud7ff'
+_Q='%%%02X'
+_P='version'
+_O="-;/?:@&=+$,_.~*'()[]"
+_N=' \n\x85\u2028\u2029'
+_M='\xa0'
+_L='...'
+_K='\\'
 _J="'"
 _I='?'
 _H='"'
 _G='!'
 _F='\n\x85\u2028\u2029'
 _E='\n'
 _D=' '
@@ -109,33 +102,33 @@
 			elif self.event.encoding and not hasattr(self.stream,A):self.encoding=self.event.encoding
 			self.write_stream_start();self.state=self.expect_first_document_start
 		else:raise EmitterError('expected StreamStartEvent, but got %s'%(self.event,))
 	def expect_nothing(self):raise EmitterError('expected nothing, but got %s'%(self.event,))
 	def expect_first_document_start(self):return self.expect_document_start(first=_A)
 	def expect_document_start(self,first=_C):
 		if isinstance(self.event,DocumentStartEvent):
-			if(self.event.version or self.event.tags)and self.open_ended:self.write_indicator(_M,_A);self.write_indent()
+			if(self.event.version or self.event.tags)and self.open_ended:self.write_indicator(_L,_A);self.write_indent()
 			if self.event.version:version_text=self.prepare_version(self.event.version);self.write_version_directive(version_text)
 			self.tag_prefixes=self.DEFAULT_TAG_PREFIXES.copy()
 			if self.event.tags:
 				handles=sorted(self.event.tags.keys())
 				for handle in handles:prefix=self.event.tags[handle];self.tag_prefixes[prefix]=handle;handle_text=self.prepare_tag_handle(handle);prefix_text=self.prepare_tag_prefix(prefix);self.write_tag_directive(handle_text,prefix_text)
 			implicit=first and not self.event.explicit and not self.canonical and not self.event.version and not self.event.tags and not self.check_empty_document()
 			if not implicit:
-				self.write_indent();self.write_indicator(_S,_A)
+				self.write_indent();self.write_indicator('---',_A)
 				if self.canonical:self.write_indent()
 			self.state=self.expect_document_root
 		elif isinstance(self.event,StreamEndEvent):
-			if self.open_ended:self.write_indicator(_M,_A);self.write_indent()
+			if self.open_ended:self.write_indicator(_L,_A);self.write_indent()
 			self.write_stream_end();self.state=self.expect_nothing
 		else:raise EmitterError('expected DocumentStartEvent, but got %s'%(self.event,))
 	def expect_document_end(self):
 		if isinstance(self.event,DocumentEndEvent):
 			self.write_indent()
-			if self.event.explicit:self.write_indicator(_M,_A);self.write_indent()
+			if self.event.explicit:self.write_indicator(_L,_A);self.write_indent()
 			self.flush_stream();self.state=self.expect_document_start
 		else:raise EmitterError('expected DocumentEndEvent, but got %s'%(self.event,))
 	def expect_document_root(self):self.states.append(self.expect_document_end);self.expect_node(root=_A)
 	def expect_node(self,root=_C,sequence=_C,mapping=_C,simple_key=_C):
 		self.root_context=root;self.sequence_context=sequence;self.mapping_context=mapping;self.simple_key_context=simple_key
 		if isinstance(self.event,AliasEvent):self.expect_alias()
 		elif isinstance(self.event,(ScalarEvent,CollectionStartEvent)):
@@ -157,60 +150,60 @@
 				if self.flow_level or self.canonical or self.event.flow_style or self.check_empty_mapping():self.expect_flow_mapping(single=self.event.nr_items==1)
 				else:self.expect_block_mapping()
 		else:raise EmitterError('expected NodeEvent, but got %s'%(self.event,))
 	def expect_alias(self):
 		if self.event.anchor is _B:raise EmitterError('anchor is not specified for alias')
 		self.process_anchor('*');self.state=self.states.pop()
 	def expect_scalar(self):self.increase_indent(flow=_A);self.process_scalar();self.indent=self.indents.pop();self.state=self.states.pop()
-	def expect_flow_sequence(self):ind=self.indents.seq_flow_align(self.best_sequence_indent,self.column);self.write_indicator(_D*ind+_K,_A,whitespace=_A);self.increase_indent(flow=_A,sequence=_A);self.flow_context.append(_K);self.state=self.expect_first_flow_sequence_item
+	def expect_flow_sequence(self):ind=self.indents.seq_flow_align(self.best_sequence_indent,self.column);self.write_indicator(_D*ind+'[',_A,whitespace=_A);self.increase_indent(flow=_A,sequence=_A);self.flow_context.append('[');self.state=self.expect_first_flow_sequence_item
 	def expect_first_flow_sequence_item(self):
 		if isinstance(self.event,SequenceEndEvent):
-			self.indent=self.indents.pop();popped=self.flow_context.pop();assert popped==_K;self.write_indicator(']',_C)
+			self.indent=self.indents.pop();popped=self.flow_context.pop();assert popped=='[';self.write_indicator(']',_C)
 			if self.event.comment and self.event.comment[0]:self.write_post_comment(self.event)
 			elif self.flow_level==0:self.write_line_break()
 			self.state=self.states.pop()
 		else:
 			if self.canonical or self.column>self.best_width:self.write_indent()
 			self.states.append(self.expect_flow_sequence_item);self.expect_node(sequence=_A)
 	def expect_flow_sequence_item(self):
 		if isinstance(self.event,SequenceEndEvent):
-			self.indent=self.indents.pop();popped=self.flow_context.pop();assert popped==_K
-			if self.canonical:self.write_indicator(_N,_C);self.write_indent()
+			self.indent=self.indents.pop();popped=self.flow_context.pop();assert popped=='['
+			if self.canonical:self.write_indicator(',',_C);self.write_indent()
 			self.write_indicator(']',_C)
 			if self.event.comment and self.event.comment[0]:self.write_post_comment(self.event)
 			else:self.no_newline=_C
 			self.state=self.states.pop()
 		else:
-			self.write_indicator(_N,_C)
+			self.write_indicator(',',_C)
 			if self.canonical or self.column>self.best_width:self.write_indent()
 			self.states.append(self.expect_flow_sequence_item);self.expect_node(sequence=_A)
 	def expect_flow_mapping(self,single=_C):
 		ind=self.indents.seq_flow_align(self.best_sequence_indent,self.column);map_init='{'
-		if single and self.flow_level and self.flow_context[-1]==_K and not self.canonical and not self.brace_single_entry_mapping_in_flow_sequence:map_init=''
+		if single and self.flow_level and self.flow_context[-1]=='['and not self.canonical and not self.brace_single_entry_mapping_in_flow_sequence:map_init=''
 		self.write_indicator(_D*ind+map_init,_A,whitespace=_A);self.flow_context.append(map_init);self.increase_indent(flow=_A,sequence=_C);self.state=self.expect_first_flow_mapping_key
 	def expect_first_flow_mapping_key(self):
 		if isinstance(self.event,MappingEndEvent):
 			self.indent=self.indents.pop();popped=self.flow_context.pop();assert popped=='{';self.write_indicator('}',_C)
 			if self.event.comment and self.event.comment[0]:self.write_post_comment(self.event)
 			elif self.flow_level==0:self.write_line_break()
 			self.state=self.states.pop()
 		else:
 			if self.canonical or self.column>self.best_width:self.write_indent()
 			if not self.canonical and self.check_simple_key():self.states.append(self.expect_flow_mapping_simple_value);self.expect_node(mapping=_A,simple_key=_A)
 			else:self.write_indicator(_I,_A);self.states.append(self.expect_flow_mapping_value);self.expect_node(mapping=_A)
 	def expect_flow_mapping_key(self):
 		if isinstance(self.event,MappingEndEvent):
 			self.indent=self.indents.pop();popped=self.flow_context.pop();assert popped in['{','']
-			if self.canonical:self.write_indicator(_N,_C);self.write_indent()
+			if self.canonical:self.write_indicator(',',_C);self.write_indent()
 			if popped!='':self.write_indicator('}',_C)
 			if self.event.comment and self.event.comment[0]:self.write_post_comment(self.event)
 			else:self.no_newline=_C
 			self.state=self.states.pop()
 		else:
-			self.write_indicator(_N,_C)
+			self.write_indicator(',',_C)
 			if self.canonical or self.column>self.best_width:self.write_indent()
 			if not self.canonical and self.check_simple_key():self.states.append(self.expect_flow_mapping_simple_value);self.expect_node(mapping=_A,simple_key=_A)
 			else:self.write_indicator(_I,_A);self.states.append(self.expect_flow_mapping_value);self.expect_node(mapping=_A)
 	def expect_flow_mapping_simple_value(self):self.write_indicator(self.prefixed_colon,_C);self.states.append(self.expect_flow_mapping_key);self.expect_node(mapping=_A)
 	def expect_flow_mapping_value(self):
 		if self.canonical or self.column>self.best_width:self.write_indent()
 		self.write_indicator(self.prefixed_colon,_A);self.states.append(self.expect_flow_mapping_key);self.expect_node(mapping=_A)
@@ -320,64 +313,64 @@
 		major,minor=version
 		if major!=1:raise EmitterError('unsupported YAML version: %d.%d'%(major,minor))
 		return'%d.%d'%(major,minor)
 	def prepare_tag_handle(self,handle):
 		if not handle:raise EmitterError('tag handle must not be empty')
 		if handle[0]!=_G or handle[-1]!=_G:raise EmitterError("tag handle must start and end with '!': %r"%utf8(handle))
 		for ch in handle[1:-1]:
-			if not(_O<=ch<='9'or'A'<=ch<='Z'or _P<=ch<='z'or ch in'-_'):raise EmitterError('invalid character %r in the tag handle: %r'%(utf8(ch),utf8(handle)))
+			if not('0'<=ch<='9'or'A'<=ch<='Z'or'a'<=ch<='z'or ch in'-_'):raise EmitterError('invalid character %r in the tag handle: %r'%(utf8(ch),utf8(handle)))
 		return handle
 	def prepare_tag_prefix(self,prefix):
 		if not prefix:raise EmitterError('tag prefix must not be empty')
 		chunks=[];start=end=0
 		if prefix[0]==_G:end=1
-		ch_set=_T
+		ch_set=_O
 		if self.dumper:
-			version=getattr(self.dumper,_U,(1,2))
+			version=getattr(self.dumper,_P,(1,2))
 			if version is _B or version>=(1,2):ch_set+='#'
 		while end<len(prefix):
 			ch=prefix[end]
-			if _O<=ch<='9'or'A'<=ch<='Z'or _P<=ch<='z'or ch in ch_set:end+=1
+			if'0'<=ch<='9'or'A'<=ch<='Z'or'a'<=ch<='z'or ch in ch_set:end+=1
 			else:
 				if start<end:chunks.append(prefix[start:end])
 				start=end=end+1;data=utf8(ch)
-				for ch in data:chunks.append(_V%ord(ch))
+				for ch in data:chunks.append(_Q%ord(ch))
 		if start<end:chunks.append(prefix[start:end])
 		return ''.join(chunks)
 	def prepare_tag(self,tag):
 		if not tag:raise EmitterError('tag must not be empty')
 		if tag==_G:return tag
 		handle=_B;suffix=tag;prefixes=sorted(self.tag_prefixes.keys())
 		for prefix in prefixes:
 			if tag.startswith(prefix)and(prefix==_G or len(prefix)<len(tag)):handle=self.tag_prefixes[prefix];suffix=tag[len(prefix):]
-		chunks=[];start=end=0;ch_set=_T
+		chunks=[];start=end=0;ch_set=_O
 		if self.dumper:
-			version=getattr(self.dumper,_U,(1,2))
+			version=getattr(self.dumper,_P,(1,2))
 			if version is _B or version>=(1,2):ch_set+='#'
 		while end<len(suffix):
 			ch=suffix[end]
-			if _O<=ch<='9'or'A'<=ch<='Z'or _P<=ch<='z'or ch in ch_set or ch==_G and handle!=_G:end+=1
+			if'0'<=ch<='9'or'A'<=ch<='Z'or'a'<=ch<='z'or ch in ch_set or ch==_G and handle!=_G:end+=1
 			else:
 				if start<end:chunks.append(suffix[start:end])
 				start=end=end+1;data=utf8(ch)
-				for ch in data:chunks.append(_V%ord(ch))
+				for ch in data:chunks.append(_Q%ord(ch))
 		if start<end:chunks.append(suffix[start:end])
 		suffix_text=''.join(chunks)
 		if handle:return'%s%s'%(handle,suffix_text)
 		else:return'!<%s>'%suffix_text
 	def prepare_anchor(self,anchor):
 		if not anchor:raise EmitterError('anchor must not be empty')
 		for ch in anchor:
 			if not check_anchorname_char(ch):raise EmitterError('invalid character %r in the anchor: %r'%(utf8(ch),utf8(anchor)))
 		return anchor
 	def analyze_scalar(self,scalar):
 		A='\x00 \t\r\n\x85\u2028\u2029'
 		if not scalar:return ScalarAnalysis(scalar=scalar,empty=_A,multiline=_C,allow_flow_plain=_C,allow_block_plain=_A,allow_single_quoted=_A,allow_double_quoted=_A,allow_block=_C)
 		block_indicators=_C;flow_indicators=_C;line_breaks=_C;special_characters=_C;leading_space=_C;leading_break=_C;trailing_space=_C;trailing_break=_C;break_space=_C;space_break=_C
-		if scalar.startswith(_S)or scalar.startswith(_M):block_indicators=_A;flow_indicators=_A
+		if scalar.startswith('---')or scalar.startswith(_L):block_indicators=_A;flow_indicators=_A
 		preceeded_by_whitespace=_A;followed_by_whitespace=len(scalar)==1 or scalar[1]in A;previous_space=_C;previous_break=_C;index=0
 		while index<len(scalar):
 			ch=scalar[index]
 			if index==0:
 				if ch in'#,[]{}&*!|>\'"%@`':flow_indicators=_A;block_indicators=_A
 				if ch in'?:':
 					if self.serializer.use_version==(1,1):flow_indicators=_A
@@ -388,15 +381,15 @@
 				if ch in',[]{}':flow_indicators=_A
 				if ch==_I and self.serializer.use_version==(1,1):flow_indicators=_A
 				if ch==':':
 					if followed_by_whitespace:flow_indicators=_A;block_indicators=_A
 				if ch=='#'and preceeded_by_whitespace:flow_indicators=_A;block_indicators=_A
 			if ch in _F:line_breaks=_A
 			if not(ch==_E or _D<=ch<='~'):
-				if(ch==_W or _Q<=ch<=_X or _Y<=ch<='�'or self.unicode_supplementary and'𐀀'<=ch<='\U0010ffff')and ch!=_Z:
+				if(ch=='\x85'or _M<=ch<=_R or _S<=ch<='�'or self.unicode_supplementary and'𐀀'<=ch<='\U0010ffff')and ch!=_T:
 					if not self.allow_unicode:special_characters=_A
 				else:special_characters=_A
 			if ch==_D:
 				if index==0:leading_space=_A
 				if index==len(scalar)-1:trailing_space=_A
 				if previous_break:break_space=_A
 				previous_space=_A;previous_break=_C
@@ -418,15 +411,15 @@
 		if line_breaks:allow_flow_plain=allow_block_plain=_C
 		if flow_indicators:allow_flow_plain=_C
 		if block_indicators:allow_block_plain=_C
 		return ScalarAnalysis(scalar=scalar,empty=_C,multiline=line_breaks,allow_flow_plain=allow_flow_plain,allow_block_plain=allow_block_plain,allow_single_quoted=allow_single_quoted,allow_double_quoted=allow_double_quoted,allow_block=allow_block)
 	def flush_stream(self):
 		if hasattr(self.stream,'flush'):self.stream.flush()
 	def write_stream_start(self):
-		if self.encoding and self.encoding.startswith('utf-16'):self.stream.write(_Z.encode(self.encoding))
+		if self.encoding and self.encoding.startswith('utf-16'):self.stream.write(_T.encode(self.encoding))
 	def write_stream_end(self):self.flush_stream()
 	def write_indicator(self,indicator,need_whitespace,whitespace=_C,indention=_C):
 		if self.whitespace or not need_whitespace:data=indicator
 		else:data=_D+indicator
 		self.whitespace=whitespace;self.indention=self.indention and indention;self.column+=len(data);self.open_ended=_C
 		if bool(self.encoding):data=data.encode(self.encoding)
 		self.stream.write(data)
@@ -472,65 +465,65 @@
 			elif breaks:
 				if ch is _B or ch not in _F:
 					if text[start]==_E:self.write_line_break()
 					for br in text[start:end]:
 						if br==_E:self.write_line_break()
 						else:self.write_line_break(br)
 					self.write_indent();start=end
-			elif ch is _B or ch in _R or ch==_J:
+			elif ch is _B or ch in _N or ch==_J:
 				if start<end:
 					data=text[start:end];self.column+=len(data)
 					if bool(self.encoding):data=data.encode(self.encoding)
 					self.stream.write(data);start=end
 			if ch==_J:
 				data="''";self.column+=2
 				if bool(self.encoding):data=data.encode(self.encoding)
 				self.stream.write(data);start=end+1
 			if ch is not _B:spaces=ch==_D;breaks=ch in _F
 			end+=1
 		self.write_indicator(_J,_C)
-	ESCAPE_REPLACEMENTS={'\x00':_O,_a:_P,'\x08':'b','\t':'t',_E:'n','\x0b':'v','\x0c':'f','\r':'r','\x1b':'e',_H:_H,_L:_L,_W:'N',_Q:'_','\u2028':'L','\u2029':'P'}
+	ESCAPE_REPLACEMENTS={'\x00':'0','\x07':'a','\x08':'b','\t':'t',_E:'n','\x0b':'v','\x0c':'f','\r':'r','\x1b':'e',_H:_H,_K:_K,'\x85':'N',_M:'_','\u2028':'L','\u2029':'P'}
 	def write_double_quoted(self,text,split=_A):
 		if self.root_context:
 			if self.requested_indent is not _B:
 				self.write_line_break()
 				if self.requested_indent!=0:self.write_indent()
 		self.write_indicator(_H,_A);start=end=0
 		while end<=len(text):
 			ch=_B
 			if end<len(text):ch=text[end]
-			if ch is _B or ch in'"\\\x85\u2028\u2029\ufeff'or not(_D<=ch<='~'or self.allow_unicode and(_Q<=ch<=_X or _Y<=ch<='�')):
+			if ch is _B or ch in'"\\\x85\u2028\u2029\ufeff'or not(_D<=ch<='~'or self.allow_unicode and(_M<=ch<=_R or _S<=ch<='�')):
 				if start<end:
 					data=text[start:end];self.column+=len(data)
 					if bool(self.encoding):data=data.encode(self.encoding)
 					self.stream.write(data);start=end
 				if ch is not _B:
-					if ch in self.ESCAPE_REPLACEMENTS:data=_L+self.ESCAPE_REPLACEMENTS[ch]
+					if ch in self.ESCAPE_REPLACEMENTS:data=_K+self.ESCAPE_REPLACEMENTS[ch]
 					elif ch<='ÿ':data='\\x%02X'%ord(ch)
 					elif ch<='\uffff':data='\\u%04X'%ord(ch)
 					else:data='\\U%08X'%ord(ch)
 					self.column+=len(data)
 					if bool(self.encoding):data=data.encode(self.encoding)
 					self.stream.write(data);start=end+1
 			if 0<end<len(text)-1 and(ch==_D or start>=end)and self.column+(end-start)>self.best_width and split:
-				data=text[start:end]+_L
+				data=text[start:end]+_K
 				if start<end:start=end
 				self.column+=len(data)
 				if bool(self.encoding):data=data.encode(self.encoding)
 				self.stream.write(data);self.write_indent();self.whitespace=_C;self.indention=_C
 				if text[start]==_D:
-					data=_L;self.column+=len(data)
+					data=_K;self.column+=len(data)
 					if bool(self.encoding):data=data.encode(self.encoding)
 					self.stream.write(data)
 			end+=1
 		self.write_indicator(_H,_C)
 	def determine_block_hints(self,text):
 		indent=0;indicator='';hints=''
 		if text:
-			if text[0]in _R:indent=self.best_sequence_indent;hints+=text_type(indent)
+			if text[0]in _N:indent=self.best_sequence_indent;hints+=text_type(indent)
 			elif self.root_context:
 				for end in ['\n---','\n...']:
 					pos=0
 					while _A:
 						pos=text.find(end,pos)
 						if pos==-1:break
 						try:
@@ -566,15 +559,15 @@
 						if bool(self.encoding):data=data.encode(self.encoding)
 						self.stream.write(data)
 					start=end
 			elif ch is _B or ch in' \n\x85\u2028\u2029\x07':
 				data=text[start:end];self.column+=len(data)
 				if bool(self.encoding):data=data.encode(self.encoding)
 				self.stream.write(data)
-				if ch==_a:
+				if ch=='\x07':
 					if end<len(text)-1 and not text[end+2].isspace():self.write_line_break();self.write_indent();end+=2
 					else:raise EmitterError('unexcpected fold indicator \\a before space')
 				if ch is _B:self.write_line_break()
 				start=end
 			if ch is not _B:breaks=ch in _F;spaces=ch==_D
 			end+=1
 	def write_literal(self,text,comment=_B):
@@ -631,15 +624,15 @@
 			elif breaks:
 				if ch not in _F:
 					if text[start]==_E:self.write_line_break()
 					for br in text[start:end]:
 						if br==_E:self.write_line_break()
 						else:self.write_line_break(br)
 					self.write_indent();self.whitespace=_C;self.indention=_C;start=end
-			elif ch is _B or ch in _R:
+			elif ch is _B or ch in _N:
 				data=text[start:end];self.column+=len(data)
 				if self.encoding:data=data.encode(self.encoding)
 				try:self.stream.write(data)
 				except:sys.stdout.write(repr(data)+_E);raise
 				start=end
 			if ch is not _B:spaces=ch==_D;breaks=ch in _F
 			end+=1
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/error.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 from __future__ import absolute_import
-_I='once'
-_H='  in "%s", line %d, column %d'
-_G='line'
-_F='index'
-_E='name'
+_E='  in "%s", line %d, column %d'
 _D='column'
 _C=False
 _B='\n'
 _A=None
 import warnings,textwrap
 from .compat import utf8
 if _C:from typing import Any,Dict,Optional,List,Text
 __all__=['FileMark','StringMark','CommentMark','YAMLError','MarkedYAMLError','ReusedAnchorWarning','UnsafeLoaderWarning','MarkedYAMLWarning','MarkedYAMLFutureWarning']
 class StreamMark:
-	__slots__=_E,_F,_G,_D
+	__slots__='name','index','line',_D
 	def __init__(A,name,index,line,column):A.name=name;A.index=index;A.line=line;A.column=column
-	def __str__(A):B=_H%(A.name,A.line+1,A.column+1);return B
+	def __str__(A):B=_E%(A.name,A.line+1,A.column+1);return B
 	def __eq__(A,other):
 		B=other
 		if A.line!=B.line or A.column!=B.column:return _C
 		if A.name!=B.name or A.index!=B.index:return _C
 		return True
 	def __ne__(A,other):return not A.__eq__(other)
 class FileMark(StreamMark):__slots__=()
 class StringMark(StreamMark):
-	__slots__=_E,_F,_G,_D,'buffer','pointer'
+	__slots__='name','index','line',_D,'buffer','pointer'
 	def __init__(A,name,index,line,column,buffer,pointer):StreamMark.__init__(A,name,index,line,column);A.buffer=buffer;A.pointer=pointer
 	def get_snippet(A,indent=4,max_length=75):
-		L=' ';K=' ... ';J='\x00\r\n\x85\u2028\u2029';F=max_length;E=indent
+		J=' ... ';I='\x00\r\n\x85\u2028\u2029';F=max_length;E=indent
 		if A.buffer is _A:return _A
 		D='';B=A.pointer
-		while B>0 and A.buffer[B-1]not in J:
+		while B>0 and A.buffer[B-1]not in I:
 			B-=1
-			if A.pointer-B>F/2-1:D=K;B+=5;break
+			if A.pointer-B>F/2-1:D=J;B+=5;break
 		G='';C=A.pointer
-		while C<len(A.buffer)and A.buffer[C]not in J:
+		while C<len(A.buffer)and A.buffer[C]not in I:
 			C+=1
-			if C-A.pointer>F/2-1:G=K;C-=5;break
-		I=utf8(A.buffer[B:C]);H='^';H='^ (line: {})'.format(A.line+1);return L*E+D+I+G+_B+L*(E+A.pointer-B+len(D))+H
+			if C-A.pointer>F/2-1:G=J;C-=5;break
+		K=utf8(A.buffer[B:C]);H='^';H='^ (line: {})'.format(A.line+1);return' '*E+D+K+G+_B+' '*(E+A.pointer-B+len(D))+H
 	def __str__(A):
-		B=A.get_snippet();C=_H%(A.name,A.line+1,A.column+1)
+		B=A.get_snippet();C=_E%(A.name,A.line+1,A.column+1)
 		if B is not _A:C+=':\n'+B
 		return C
 class CommentMark:
 	__slots__=_D,
 	def __init__(A,column):A.column=column
 class YAMLError(Exception):0
 class MarkedYAMLError(YAMLError):
@@ -67,19 +63,19 @@
 		if A.problem is not _A:B.append(A.problem)
 		if A.problem_mark is not _A:B.append(str(A.problem_mark))
 		if A.note is not _A and A.note:C=textwrap.dedent(A.note);B.append(C)
 		if A.warn is not _A and A.warn:D=textwrap.dedent(A.warn);B.append(D)
 		return _B.join(B)
 class ReusedAnchorWarning(YAMLWarning):0
 class UnsafeLoaderWarning(YAMLWarning):text="\nThe default 'Loader' for 'load(stream)' without further arguments can be unsafe.\nUse 'load(stream, Loader=ruamel.yaml.Loader)' explicitly if that is OK.\nAlternatively include the following in your code:\n\n  import warnings\n  warnings.simplefilter('ignore', ruamel.yaml.error.UnsafeLoaderWarning)\n\nIn most other cases you should consider using 'safe_load(stream)'"
-warnings.simplefilter(_I,UnsafeLoaderWarning)
+warnings.simplefilter('once',UnsafeLoaderWarning)
 class MantissaNoDotYAML1_1Warning(YAMLWarning):
 	def __init__(A,node,flt_str):A.node=node;A.flt=flt_str
 	def __str__(A):B=A.node.start_mark.line;C=A.node.start_mark.column;return '\nIn YAML 1.1 floating point values should have a dot (\'.\') in their mantissa.\nSee the Floating-Point Language-Independent Type for YAML™ Version 1.1 specification\n( http://yaml.org/type/float.html ). This dot is not required for JSON nor for YAML 1.2\n\nCorrect your float: "{}" on line: {}, column: {}\n\nor alternatively include the following in your code:\n\n  import warnings\n  warnings.simplefilter(\'ignore\', ruamel.yaml.error.MantissaNoDotYAML1_1Warning)\n\n'.format(A.flt,B,C)
-warnings.simplefilter(_I,MantissaNoDotYAML1_1Warning)
+warnings.simplefilter('once',MantissaNoDotYAML1_1Warning)
 class YAMLFutureWarning(Warning):0
 class MarkedYAMLFutureWarning(YAMLFutureWarning):
 	def __init__(A,context=_A,context_mark=_A,problem=_A,problem_mark=_A,note=_A,warn=_A):A.context=context;A.context_mark=context_mark;A.problem=problem;A.problem_mark=problem_mark;A.note=note;A.warn=warn
 	def __str__(A):
 		B=[]
 		if A.context is not _A:B.append(A.context)
 		if A.context_mark is not _A and(A.problem is _A or A.problem_mark is _A or A.context_mark.name!=A.problem_mark.name or A.context_mark.line!=A.problem_mark.line or A.context_mark.column!=A.problem_mark.column):B.append(str(A.context_mark))
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/events.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/events.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,43 @@
-_H='explicit'
-_G='style'
-_F='flow_style'
-_E='value'
+_F='explicit'
+_E='flow_style'
 _D='anchor'
 _C='implicit'
 _B='tag'
 _A=None
 if False:from typing import Any,Dict,Optional,List
 def CommentCheck():0
 class Event:
 	__slots__='start_mark','end_mark','comment'
 	def __init__(A,start_mark=_A,end_mark=_A,comment=CommentCheck):
 		B=comment;A.start_mark=start_mark;A.end_mark=end_mark
 		if B is CommentCheck:B=_A
 		A.comment=B
 	def __repr__(A):
-		C=[B for B in[_D,_B,_C,_E,_F,_G]if hasattr(A,B)];B=', '.join(['%s=%r'%(B,getattr(A,B))for B in C])
+		C=[B for B in[_D,_B,_C,'value',_E,'style']if hasattr(A,B)];B=', '.join(['%s=%r'%(B,getattr(A,B))for B in C])
 		if A.comment not in[_A,CommentCheck]:B+=', comment={!r}'.format(A.comment)
 		return'%s(%s)'%(A.__class__.__name__,B)
 class NodeEvent(Event):
 	__slots__=_D,
 	def __init__(A,anchor,start_mark=_A,end_mark=_A,comment=_A):Event.__init__(A,start_mark,end_mark,comment);A.anchor=anchor
 class CollectionStartEvent(NodeEvent):
-	__slots__=_B,_C,_F,'nr_items'
+	__slots__=_B,_C,_E,'nr_items'
 	def __init__(A,anchor,tag,implicit,start_mark=_A,end_mark=_A,flow_style=_A,comment=_A,nr_items=_A):NodeEvent.__init__(A,anchor,start_mark,end_mark,comment);A.tag=tag;A.implicit=implicit;A.flow_style=flow_style;A.nr_items=nr_items
 class CollectionEndEvent(Event):__slots__=()
 class StreamStartEvent(Event):
 	__slots__='encoding',
 	def __init__(A,start_mark=_A,end_mark=_A,encoding=_A,comment=_A):Event.__init__(A,start_mark,end_mark,comment);A.encoding=encoding
 class StreamEndEvent(Event):__slots__=()
 class DocumentStartEvent(Event):
-	__slots__=_H,'version','tags'
+	__slots__=_F,'version','tags'
 	def __init__(A,start_mark=_A,end_mark=_A,explicit=_A,version=_A,tags=_A,comment=_A):Event.__init__(A,start_mark,end_mark,comment);A.explicit=explicit;A.version=version;A.tags=tags
 class DocumentEndEvent(Event):
-	__slots__=_H,
+	__slots__=_F,
 	def __init__(A,start_mark=_A,end_mark=_A,explicit=_A,comment=_A):Event.__init__(A,start_mark,end_mark,comment);A.explicit=explicit
 class AliasEvent(NodeEvent):__slots__=()
 class ScalarEvent(NodeEvent):
-	__slots__=_B,_C,_E,_G
+	__slots__=_B,_C,'value','style'
 	def __init__(A,anchor,tag,implicit,value,start_mark=_A,end_mark=_A,style=_A,comment=_A):NodeEvent.__init__(A,anchor,start_mark,end_mark,comment);A.tag=tag;A.implicit=implicit;A.value=value;A.style=style
 class SequenceStartEvent(CollectionStartEvent):__slots__=()
 class SequenceEndEvent(CollectionEndEvent):__slots__=()
 class MappingStartEvent(CollectionStartEvent):__slots__=()
 class MappingEndEvent(CollectionEndEvent):__slots__=()
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/loader.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/main.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 from __future__ import absolute_import,unicode_literals,print_function
-_Q='_emitter'
-_P='_serializer'
-_O='write'
-_N='{}.dump(_all) takes two positional argument but at least three were given ({!r})'
-_M='read'
-_L='_stream'
-_K='typ'
-_J='utf-8'
-_I='base'
+_L='_emitter'
+_K='_serializer'
+_J='{}.dump(_all) takes two positional argument but at least three were given ({!r})'
+_I='_stream'
 _H='{}.__init__() takes no positional argument but at least one was given ({!r})'
 _G='yaml_tag'
 _F='open'
 _E='rt'
 _D='_'
 _C=True
 _B=False
@@ -41,36 +36,36 @@
 	def __init__(self,_kw=enforce,typ=_A,pure=_B,output=_A,plug_ins=_A):
 		if _kw is not enforce:raise TypeError(_H.format(self.__class__.__name__,_kw))
 		self.typ=[_E]if typ is _A else typ if isinstance(typ,list)else[typ];self.pure=pure;self._output=output;self._context_manager=_A;self.plug_ins=[]
 		for pu in ([]if plug_ins is _A else plug_ins)+self.official_plug_ins():file_name=pu.replace(os.sep,'.');self.plug_ins.append(import_module(file_name))
 		self.Resolver=ruamel.yaml.resolver.VersionedResolver;self.allow_unicode=_C;self.Reader=_A;self.Representer=_A;self.Constructor=_A;self.Scanner=_A;self.Serializer=_A;self.default_flow_style=_A;typ_found=1;setup_rt=_B
 		if _E in self.typ:setup_rt=_C
 		elif'safe'in self.typ:self.Emitter=ruamel.yaml.emitter.Emitter if pure or CEmitter is _A else CEmitter;self.Representer=ruamel.yaml.representer.SafeRepresenter;self.Parser=ruamel.yaml.parser.Parser if pure or CParser is _A else CParser;self.Composer=ruamel.yaml.composer.Composer;self.Constructor=ruamel.yaml.constructor.SafeConstructor
-		elif _I in self.typ:self.Emitter=ruamel.yaml.emitter.Emitter;self.Representer=ruamel.yaml.representer.BaseRepresenter;self.Parser=ruamel.yaml.parser.Parser if pure or CParser is _A else CParser;self.Composer=ruamel.yaml.composer.Composer;self.Constructor=ruamel.yaml.constructor.BaseConstructor
+		elif'base'in self.typ:self.Emitter=ruamel.yaml.emitter.Emitter;self.Representer=ruamel.yaml.representer.BaseRepresenter;self.Parser=ruamel.yaml.parser.Parser if pure or CParser is _A else CParser;self.Composer=ruamel.yaml.composer.Composer;self.Constructor=ruamel.yaml.constructor.BaseConstructor
 		elif'unsafe'in self.typ:self.Emitter=ruamel.yaml.emitter.Emitter if pure or CEmitter is _A else CEmitter;self.Representer=ruamel.yaml.representer.Representer;self.Parser=ruamel.yaml.parser.Parser if pure or CParser is _A else CParser;self.Composer=ruamel.yaml.composer.Composer;self.Constructor=ruamel.yaml.constructor.Constructor
 		else:setup_rt=_C;typ_found=0
 		if setup_rt:self.default_flow_style=_B;self.Emitter=ruamel.yaml.emitter.Emitter;self.Serializer=ruamel.yaml.serializer.Serializer;self.Representer=ruamel.yaml.representer.RoundTripRepresenter;self.Scanner=ruamel.yaml.scanner.RoundTripScanner;self.Parser=ruamel.yaml.parser.RoundTripParser;self.Composer=ruamel.yaml.composer.Composer;self.Constructor=ruamel.yaml.constructor.RoundTripConstructor
-		del setup_rt;self.stream=_A;self.canonical=_A;self.old_indent=_A;self.width=_A;self.line_break=_A;self.map_indent=_A;self.sequence_indent=_A;self.sequence_dash_offset=0;self.compact_seq_seq=_A;self.compact_seq_map=_A;self.sort_base_mapping_type_on_output=_A;self.top_level_colon_align=_A;self.prefix_colon=_A;self.version=_A;self.preserve_quotes=_A;self.allow_duplicate_keys=_B;self.encoding=_J;self.explicit_start=_A;self.explicit_end=_A;self.tags=_A;self.default_style=_A;self.top_level_block_style_scalar_no_indent_error_1_1=_B;self.scalar_after_indicator=_A;self.brace_single_entry_mapping_in_flow_sequence=_B
+		del setup_rt;self.stream=_A;self.canonical=_A;self.old_indent=_A;self.width=_A;self.line_break=_A;self.map_indent=_A;self.sequence_indent=_A;self.sequence_dash_offset=0;self.compact_seq_seq=_A;self.compact_seq_map=_A;self.sort_base_mapping_type_on_output=_A;self.top_level_colon_align=_A;self.prefix_colon=_A;self.version=_A;self.preserve_quotes=_A;self.allow_duplicate_keys=_B;self.encoding='utf-8';self.explicit_start=_A;self.explicit_end=_A;self.tags=_A;self.default_style=_A;self.top_level_block_style_scalar_no_indent_error_1_1=_B;self.scalar_after_indicator=_A;self.brace_single_entry_mapping_in_flow_sequence=_B
 		for module in self.plug_ins:
-			if getattr(module,_K,_A)in self.typ:typ_found+=1;module.init_typ(self);break
+			if getattr(module,'typ',_A)in self.typ:typ_found+=1;module.init_typ(self);break
 		if typ_found==0:raise NotImplementedError('typ "{}"not recognised (need to install plug-in?)'.format(self.typ))
 	@property
 	def reader(self):
 		try:return self._reader
 		except AttributeError:self._reader=self.Reader(_A,loader=self);return self._reader
 	@property
 	def scanner(self):
 		try:return self._scanner
 		except AttributeError:self._scanner=self.Scanner(loader=self);return self._scanner
 	@property
 	def parser(self):
 		attr=_D+sys._getframe().f_code.co_name
 		if not hasattr(self,attr):
 			if self.Parser is not CParser:setattr(self,attr,self.Parser(loader=self))
-			elif getattr(self,_L,_A)is _A:return _A
+			elif getattr(self,_I,_A)is _A:return _A
 			else:setattr(self,attr,CParser(self._stream))
 		return getattr(self,attr)
 	@property
 	def composer(self):
 		attr=_D+sys._getframe().f_code.co_name
 		if not hasattr(self,attr):setattr(self,attr,self.Composer(loader=self))
 		return getattr(self,attr)
@@ -92,15 +87,15 @@
 				_emitter=self.Emitter(_A,canonical=self.canonical,indent=self.old_indent,width=self.width,allow_unicode=self.allow_unicode,line_break=self.line_break,prefix_colon=self.prefix_colon,brace_single_entry_mapping_in_flow_sequence=self.brace_single_entry_mapping_in_flow_sequence,dumper=self);setattr(self,attr,_emitter)
 				if self.map_indent is not _A:_emitter.best_map_indent=self.map_indent
 				if self.sequence_indent is not _A:_emitter.best_sequence_indent=self.sequence_indent
 				if self.sequence_dash_offset is not _A:_emitter.sequence_dash_offset=self.sequence_dash_offset
 				if self.compact_seq_seq is not _A:_emitter.compact_seq_seq=self.compact_seq_seq
 				if self.compact_seq_map is not _A:_emitter.compact_seq_map=self.compact_seq_map
 			else:
-				if getattr(self,_L,_A)is _A:return _A
+				if getattr(self,_I,_A)is _A:return _A
 				return _A
 		return getattr(self,attr)
 	@property
 	def serializer(self):
 		attr=_D+sys._getframe().f_code.co_name
 		if not hasattr(self,attr):setattr(self,attr,self.Serializer(encoding=self.encoding,explicit_start=self.explicit_start,explicit_end=self.explicit_end,version=self.version,tags=self.tags,dumper=self))
 		return getattr(self,attr)
@@ -109,27 +104,27 @@
 		attr=_D+sys._getframe().f_code.co_name
 		if not hasattr(self,attr):
 			repres=self.Representer(default_style=self.default_style,default_flow_style=self.default_flow_style,dumper=self)
 			if self.sort_base_mapping_type_on_output is not _A:repres.sort_base_mapping_type_on_output=self.sort_base_mapping_type_on_output
 			setattr(self,attr,repres)
 		return getattr(self,attr)
 	def load(self,stream):
-		if not hasattr(stream,_M)and hasattr(stream,_F):
+		if not hasattr(stream,'read')and hasattr(stream,_F):
 			with stream.open('rb')as fp:return self.load(fp)
 		constructor,parser=self.get_constructor_parser(stream)
 		try:return constructor.get_single_data()
 		finally:
 			parser.dispose()
 			try:self._reader.reset_reader()
 			except AttributeError:pass
 			try:self._scanner.reset_scanner()
 			except AttributeError:pass
 	def load_all(self,stream,_kw=enforce):
 		if _kw is not enforce:raise TypeError(_H.format(self.__class__.__name__,_kw))
-		if not hasattr(stream,_M)and hasattr(stream,_F):
+		if not hasattr(stream,'read')and hasattr(stream,_F):
 			with stream.open('r')as fp:
 				for d in self.load_all(fp,_kw=enforce):yield d
 				return
 		constructor,parser=self.get_constructor_parser(stream)
 		try:
 			while constructor.check_data():yield constructor.get_data()
 		finally:
@@ -162,22 +157,22 @@
 			if transform is not _A:raise TypeError('{}.dump() in the context manager cannot have transform keyword '.format(self.__class__.__name__))
 			self._context_manager.dump(data)
 		else:
 			if stream is _A:raise TypeError('Need a stream argument when not dumping from context manager')
 			return self.dump_all([data],stream,_kw,transform=transform)
 	def dump_all(self,documents,stream,_kw=enforce,transform=_A):
 		if self._context_manager:raise NotImplementedError
-		if _kw is not enforce:raise TypeError(_N.format(self.__class__.__name__,_kw))
+		if _kw is not enforce:raise TypeError(_J.format(self.__class__.__name__,_kw))
 		self._output=stream;self._context_manager=YAMLContextManager(self,transform=transform)
 		for data in documents:self._context_manager.dump(data)
 		self._context_manager.teardown_output();self._output=_A;self._context_manager=_A
 	def Xdump_all(self,documents,stream,_kw=enforce,transform=_A):
-		if not hasattr(stream,_O)and hasattr(stream,_F):
+		if not hasattr(stream,'write')and hasattr(stream,_F):
 			with stream.open('w')as fp:return self.dump_all(documents,fp,_kw,transform=transform)
-		if _kw is not enforce:raise TypeError(_N.format(self.__class__.__name__,_kw))
+		if _kw is not enforce:raise TypeError(_J.format(self.__class__.__name__,_kw))
 		if self.top_level_colon_align is _C:tlca=max([len(str(x))for x in documents[0]])
 		else:tlca=self.top_level_colon_align
 		if transform is not _A:
 			fstream=stream
 			if self.encoding is _A:stream=StringIO()
 			else:stream=BytesIO()
 		serializer,representer,emitter=self.get_serializer_representer_emitter(stream,tlca)
@@ -186,15 +181,15 @@
 			for data in documents:
 				try:self.representer.represent(data)
 				except AttributeError:raise
 			self.serializer.close()
 		finally:
 			try:self.emitter.dispose()
 			except AttributeError:raise
-			delattr(self,_P);delattr(self,_Q)
+			delattr(self,_K);delattr(self,_L)
 		if transform:
 			val=stream.getvalue()
 			if self.encoding:val=val.decode(self.encoding)
 			if fstream is _A:transform(val)
 			else:fstream.write(transform(val))
 		return _A
 	def get_serializer_representer_emitter(self,stream,tlca):
@@ -203,24 +198,24 @@
 			self.emitter.stream=stream;self.emitter.top_level_colon_align=tlca
 			if self.scalar_after_indicator is not _A:self.emitter.scalar_after_indicator=self.scalar_after_indicator
 			return self.serializer,self.representer,self.emitter
 		if self.Serializer is not _A:
 			self.Emitter=ruamel.yaml.emitter.Emitter;self.emitter.stream=stream;self.emitter.top_level_colon_align=tlca
 			if self.scalar_after_indicator is not _A:self.emitter.scalar_after_indicator=self.scalar_after_indicator
 			return self.serializer,self.representer,self.emitter
-		rslvr=ruamel.yaml.resolver.BaseResolver if _I in self.typ else ruamel.yaml.resolver.Resolver
+		rslvr=ruamel.yaml.resolver.BaseResolver if'base'in self.typ else ruamel.yaml.resolver.Resolver
 		class XDumper(CEmitter,self.Representer,rslvr):
 			def __init__(selfx,stream,default_style=_A,default_flow_style=_A,canonical=_A,indent=_A,width=_A,allow_unicode=_A,line_break=_A,encoding=_A,explicit_start=_A,explicit_end=_A,version=_A,tags=_A,block_seq_indent=_A,top_level_colon_align=_A,prefix_colon=_A):CEmitter.__init__(selfx,stream,canonical=canonical,indent=indent,width=width,encoding=encoding,allow_unicode=allow_unicode,line_break=line_break,explicit_start=explicit_start,explicit_end=explicit_end,version=version,tags=tags);selfx._emitter=selfx._serializer=selfx._representer=selfx;self.Representer.__init__(selfx,default_style=default_style,default_flow_style=default_flow_style);rslvr.__init__(selfx)
 		self._stream=stream;dumper=XDumper(stream,default_style=self.default_style,default_flow_style=self.default_flow_style,canonical=self.canonical,indent=self.old_indent,width=self.width,allow_unicode=self.allow_unicode,line_break=self.line_break,explicit_start=self.explicit_start,explicit_end=self.explicit_end,version=self.version,tags=self.tags);self._emitter=self._serializer=dumper;return dumper,dumper,dumper
 	def map(self,**kw):
 		if _E in self.typ:from dynaconf.vendor.ruamel.yaml.comments import CommentedMap;return CommentedMap(**kw)
 		else:return dict(**kw)
 	def seq(self,*args):
-		if _E in self.typ:from dynaconf.vendor.ruamel.yaml.comments import CommentedSeq;return CommentedSeq(*args)
-		else:return list(*args)
+		if _E in self.typ:from dynaconf.vendor.ruamel.yaml.comments import CommentedSeq;return CommentedSeq(*(args))
+		else:return list(*(args))
 	def official_plug_ins(self):bd=os.path.dirname(__file__);gpbd=os.path.dirname(os.path.dirname(bd));res=[x.replace(gpbd,'')[1:-3]for x in glob.glob(bd+'/*/__plug_in__.py')];return res
 	def register_class(self,cls):
 		tag=getattr(cls,_G,'!'+cls.__name__)
 		try:self.representer.add_representer(cls,cls.to_yaml)
 		except AttributeError:
 			def t_y(representer,data):return representer.represent_yaml_object(tag,data,cls,flow_style=representer.default_flow_style)
 			self.representer.add_representer(cls,t_y)
@@ -237,15 +232,15 @@
 			parser.dispose()
 			try:self._reader.reset_reader()
 			except AttributeError:pass
 			try:self._scanner.reset_scanner()
 			except AttributeError:pass
 	def __enter__(self):self._context_manager=YAMLContextManager(self);return self
 	def __exit__(self,typ,value,traceback):
-		if typ:nprint(_K,typ)
+		if typ:nprint('typ',typ)
 		self._context_manager.teardown_output();self._context_manager=_A
 	def _indent(self,mapping=_A,sequence=_A,offset=_A):
 		if mapping is not _A:self.map_indent=mapping
 		if sequence is not _A:self.sequence_indent=sequence
 		if offset is not _A:self.sequence_dash_offset=offset
 	@property
 	def indent(self):return self._indent
@@ -255,25 +250,25 @@
 	def block_seq_indent(self):return self.sequence_dash_offset
 	@block_seq_indent.setter
 	def block_seq_indent(self,val):self.sequence_dash_offset=val
 	def compact(self,seq_seq=_A,seq_map=_A):self.compact_seq_seq=seq_seq;self.compact_seq_map=seq_map
 class YAMLContextManager:
 	def __init__(self,yaml,transform=_A):
 		self._yaml=yaml;self._output_inited=_B;self._output_path=_A;self._output=self._yaml._output;self._transform=transform
-		if not hasattr(self._output,_O)and hasattr(self._output,_F):self._output_path=self._output;self._output=self._output_path.open('w')
+		if not hasattr(self._output,'write')and hasattr(self._output,_F):self._output_path=self._output;self._output=self._output_path.open('w')
 		if self._transform is not _A:
 			self._fstream=self._output
 			if self._yaml.encoding is _A:self._output=StringIO()
 			else:self._output=BytesIO()
 	def teardown_output(self):
 		if self._output_inited:self._yaml.serializer.close()
 		else:return
 		try:self._yaml.emitter.dispose()
 		except AttributeError:raise
-		try:delattr(self._yaml,_P);delattr(self._yaml,_Q)
+		try:delattr(self._yaml,_K);delattr(self._yaml,_L)
 		except AttributeError:raise
 		if self._transform:
 			val=self._output.getvalue()
 			if self._yaml.encoding:val=val.decode(self._yaml.encoding)
 			if self._fstream is _A:self._transform(val)
 			else:self._fstream.write(self._transform(val));self._fstream.flush();self._output=self._fstream
 		if self._output_path is not _A:self._output.close()
@@ -348,15 +343,15 @@
 	dumper=Dumper(stream,canonical=canonical,indent=indent,width=width,allow_unicode=allow_unicode,line_break=line_break)
 	try:
 		for event in events:dumper.emit(event)
 	finally:
 		try:dumper._emitter.dispose()
 		except AttributeError:raise;dumper.dispose()
 	if getvalue is not _A:return getvalue()
-enc=_A if PY3 else _J
+enc=_A if PY3 else'utf-8'
 def serialize_all(nodes,stream=_A,Dumper=Dumper,canonical=_A,indent=_A,width=_A,allow_unicode=_A,line_break=_A,encoding=enc,explicit_start=_A,explicit_end=_A,version=_A,tags=_A):
 	getvalue=_A
 	if stream is _A:
 		if encoding is _A:stream=StringIO()
 		else:stream=BytesIO()
 		getvalue=stream.getvalue
 	dumper=Dumper(stream,canonical=canonical,indent=indent,width=width,allow_unicode=allow_unicode,line_break=line_break,encoding=encoding,version=version,tags=tags,explicit_start=explicit_start,explicit_end=explicit_end)
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/nodes.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/nodes.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 from .compat import string_types
 if False:from typing import Dict,Any,Text
 class Node:
 	__slots__='tag','value','start_mark','end_mark','comment','anchor'
 	def __init__(A,tag,value,start_mark,end_mark,comment=_A,anchor=_A):A.tag=tag;A.value=value;A.start_mark=start_mark;A.end_mark=end_mark;A.comment=comment;A.anchor=anchor
 	def __repr__(A):B=A.value;B=repr(B);return'%s(tag=%r, value=%s)'%(A.__class__.__name__,A.tag,B)
 	def dump(A,indent=0):
-		F='    {}comment: {})\n';D='  ';B=indent
+		E='    {}comment: {})\n';D='  ';B=indent
 		if isinstance(A.value,string_types):
 			sys.stdout.write('{}{}(tag={!r}, value={!r})\n'.format(D*B,A.__class__.__name__,A.tag,A.value))
-			if A.comment:sys.stdout.write(F.format(D*B,A.comment))
+			if A.comment:sys.stdout.write(E.format(D*B,A.comment))
 			return
 		sys.stdout.write('{}{}(tag={!r})\n'.format(D*B,A.__class__.__name__,A.tag))
-		if A.comment:sys.stdout.write(F.format(D*B,A.comment))
+		if A.comment:sys.stdout.write(E.format(D*B,A.comment))
 		for C in A.value:
 			if isinstance(C,tuple):
-				for E in C:E.dump(B+1)
+				for F in C:F.dump(B+1)
 			elif isinstance(C,Node):C.dump(B+1)
 			else:sys.stdout.write('Node value type? {}\n'.format(type(C)))
 class ScalarNode(Node):
 	__slots__='style',;id='scalar'
 	def __init__(A,tag,value,start_mark=_A,end_mark=_A,style=_A,comment=_A,anchor=_A):Node.__init__(A,tag,value,start_mark,end_mark,comment=comment,anchor=anchor);A.style=style
 class CollectionNode(Node):
 	__slots__='flow_style',
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/parser.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 from __future__ import absolute_import
-_F='expected <block end>, but found %r'
-_E='typ'
-_D='!'
+_D='expected <block end>, but found %r'
 _C=True
 _B=False
 _A=None
 from .error import MarkedYAMLError
 from .tokens import *
 from .events import *
 from .scanner import Scanner,RoundTripScanner,ScannerError
 from .compat import utf8,nprint,nprintf
 if _B:from typing import Any,Dict,Optional,List
 __all__=['Parser','RoundTripParser','ParserError']
 class ParserError(MarkedYAMLError):0
 class Parser:
-	DEFAULT_TAGS={_D:_D,'!!':'tag:yaml.org,2002:'}
+	DEFAULT_TAGS={'!':'!','!!':'tag:yaml.org,2002:'}
 	def __init__(self,loader):
 		self.loader=loader
 		if self.loader is not _A and getattr(self.loader,'_parser',_A)is _A:self.loader._parser=self
 		self.reset_parser()
 	def reset_parser(self):self.current_event=_A;self.tag_handles={};self.states=[];self.marks=[];self.state=self.parse_stream_start
 	def dispose(self):self.reset_parser()
 	@property
 	def scanner(self):
-		if hasattr(self.loader,_E):return self.loader.scanner
+		if hasattr(self.loader,'typ'):return self.loader.scanner
 		return self.loader._scanner
 	@property
 	def resolver(self):
-		if hasattr(self.loader,_E):return self.loader.resolver
+		if hasattr(self.loader,'typ'):return self.loader.resolver
 		return self.loader._resolver
 	def check_event(self,*choices):
 		if self.current_event is _A:
 			if self.state:self.current_event=self.state()
 		if self.current_event is not _A:
 			if not choices:return _C
 			for choice in choices:
@@ -105,22 +103,22 @@
 		if tag is not _A:
 			handle,suffix=tag
 			if handle is not _A:
 				if handle not in self.tag_handles:raise ParserError('while parsing a node',start_mark,'found undefined tag handle %r'%utf8(handle),tag_mark)
 				tag=self.transform_tag(handle,suffix)
 			else:tag=suffix
 		if start_mark is _A:start_mark=end_mark=self.scanner.peek_token().start_mark
-		event=_A;implicit=tag is _A or tag==_D
+		event=_A;implicit=tag is _A or tag=='!'
 		if indentless_sequence and self.scanner.check_token(BlockEntryToken):
 			comment=_A;pt=self.scanner.peek_token()
 			if pt.comment and pt.comment[0]:comment=[pt.comment[0],[]];pt.comment[0]=_A
 			end_mark=self.scanner.peek_token().end_mark;event=SequenceStartEvent(anchor,tag,implicit,start_mark,end_mark,flow_style=_B,comment=comment);self.state=self.parse_indentless_sequence_entry;return event
 		if self.scanner.check_token(ScalarToken):
 			token=self.scanner.get_token();end_mark=token.end_mark
-			if token.plain and tag is _A or tag==_D:implicit=_C,_B
+			if token.plain and tag is _A or tag=='!':implicit=_C,_B
 			elif tag is _A:implicit=_B,_C
 			else:implicit=_B,_B
 			event=ScalarEvent(anchor,tag,implicit,token.value,start_mark,end_mark,style=token.style,comment=token.comment);self.state=self.states.pop()
 		elif self.scanner.check_token(FlowSequenceStartToken):pt=self.scanner.peek_token();end_mark=pt.end_mark;event=SequenceStartEvent(anchor,tag,implicit,start_mark,end_mark,flow_style=_C,comment=pt.comment);self.state=self.parse_flow_sequence_first_entry
 		elif self.scanner.check_token(FlowMappingStartToken):pt=self.scanner.peek_token();end_mark=pt.end_mark;event=MappingStartEvent(anchor,tag,implicit,start_mark,end_mark,flow_style=_C,comment=pt.comment);self.state=self.parse_flow_mapping_first_key
 		elif block and self.scanner.check_token(BlockSequenceStartToken):
 			end_mark=self.scanner.peek_token().start_mark;pt=self.scanner.peek_token();comment=pt.comment
@@ -135,30 +133,30 @@
 		return event
 	def parse_block_sequence_first_entry(self):token=self.scanner.get_token();self.marks.append(token.start_mark);return self.parse_block_sequence_entry()
 	def parse_block_sequence_entry(self):
 		if self.scanner.check_token(BlockEntryToken):
 			token=self.scanner.get_token();token.move_comment(self.scanner.peek_token())
 			if not self.scanner.check_token(BlockEntryToken,BlockEndToken):self.states.append(self.parse_block_sequence_entry);return self.parse_block_node()
 			else:self.state=self.parse_block_sequence_entry;return self.process_empty_scalar(token.end_mark)
-		if not self.scanner.check_token(BlockEndToken):token=self.scanner.peek_token();raise ParserError('while parsing a block collection',self.marks[-1],_F%token.id,token.start_mark)
+		if not self.scanner.check_token(BlockEndToken):token=self.scanner.peek_token();raise ParserError('while parsing a block collection',self.marks[-1],_D%token.id,token.start_mark)
 		token=self.scanner.get_token();event=SequenceEndEvent(token.start_mark,token.end_mark,comment=token.comment);self.state=self.states.pop();self.marks.pop();return event
 	def parse_indentless_sequence_entry(self):
 		if self.scanner.check_token(BlockEntryToken):
 			token=self.scanner.get_token();token.move_comment(self.scanner.peek_token())
 			if not self.scanner.check_token(BlockEntryToken,KeyToken,ValueToken,BlockEndToken):self.states.append(self.parse_indentless_sequence_entry);return self.parse_block_node()
 			else:self.state=self.parse_indentless_sequence_entry;return self.process_empty_scalar(token.end_mark)
 		token=self.scanner.peek_token();event=SequenceEndEvent(token.start_mark,token.start_mark,comment=token.comment);self.state=self.states.pop();return event
 	def parse_block_mapping_first_key(self):token=self.scanner.get_token();self.marks.append(token.start_mark);return self.parse_block_mapping_key()
 	def parse_block_mapping_key(self):
 		if self.scanner.check_token(KeyToken):
 			token=self.scanner.get_token();token.move_comment(self.scanner.peek_token())
 			if not self.scanner.check_token(KeyToken,ValueToken,BlockEndToken):self.states.append(self.parse_block_mapping_value);return self.parse_block_node_or_indentless_sequence()
 			else:self.state=self.parse_block_mapping_value;return self.process_empty_scalar(token.end_mark)
 		if self.resolver.processing_version>(1,1)and self.scanner.check_token(ValueToken):self.state=self.parse_block_mapping_value;return self.process_empty_scalar(self.scanner.peek_token().start_mark)
-		if not self.scanner.check_token(BlockEndToken):token=self.scanner.peek_token();raise ParserError('while parsing a block mapping',self.marks[-1],_F%token.id,token.start_mark)
+		if not self.scanner.check_token(BlockEndToken):token=self.scanner.peek_token();raise ParserError('while parsing a block mapping',self.marks[-1],_D%token.id,token.start_mark)
 		token=self.scanner.get_token();token.move_comment(self.scanner.peek_token());event=MappingEndEvent(token.start_mark,token.end_mark,comment=token.comment);self.state=self.states.pop();self.marks.pop();return event
 	def parse_block_mapping_value(self):
 		if self.scanner.check_token(ValueToken):
 			token=self.scanner.get_token()
 			if self.scanner.check_token(ValueToken):token.move_comment(self.scanner.peek_token())
 			elif not self.scanner.check_token(KeyToken):token.move_comment(self.scanner.peek_token(),empty=_C)
 			if not self.scanner.check_token(KeyToken,ValueToken,BlockEndToken):self.states.append(self.parse_block_mapping_key);return self.parse_block_node_or_indentless_sequence()
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/reader.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from __future__ import absolute_import
-_F='\ufeff'
-_E='\x00'
-_D=False
-_C='ascii'
-_B='\n'
+_C='\ufeff'
+_B='ascii'
 _A=None
 import codecs
 from .error import YAMLError,FileMark,StringMark,YAMLStreamError
 from .compat import text_type,binary_type,PY3,UNICODE_SIZE
 from .util import RegExp
-if _D:from typing import Any,Dict,Optional,List,Union,Text,Tuple,Optional
+if False:from typing import Any,Dict,Optional,List,Union,Text,Tuple,Optional
 __all__=['Reader','ReaderError']
 class ReaderError(YAMLError):
 	def __init__(A,name,position,character,encoding,reason):A.name=name;A.character=character;A.position=position;A.encoding=encoding;A.reason=reason
 	def __str__(A):
 		if isinstance(A.character,binary_type):return'\'%s\' codec can\'t decode byte #x%02x: %s\n  in "%s", position %d'%(A.encoding,ord(A.character),A.reason,A.name,A.position)
 		else:return'unacceptable character #x%04x: %s\n  in "%s", position %d'%(A.character,A.reason,A.name,A.position)
 class Reader:
@@ -27,61 +24,61 @@
 		try:return self._stream
 		except AttributeError:raise YAMLStreamError('input stream needs to specified')
 	@stream.setter
 	def stream(self,val):
 		B=val;A=self
 		if B is _A:return
 		A._stream=_A
-		if isinstance(B,text_type):A.name='<unicode string>';A.check_printable(B);A.buffer=B+_E
+		if isinstance(B,text_type):A.name='<unicode string>';A.check_printable(B);A.buffer=B+'\x00'
 		elif isinstance(B,binary_type):A.name='<byte string>';A.raw_buffer=B;A.determine_encoding()
 		else:
 			if not hasattr(B,'read'):raise YAMLStreamError('stream argument needs to have a read() method')
-			A._stream=B;A.name=getattr(A.stream,'name','<file>');A.eof=_D;A.raw_buffer=_A;A.determine_encoding()
+			A._stream=B;A.name=getattr(A.stream,'name','<file>');A.eof=False;A.raw_buffer=_A;A.determine_encoding()
 	def peek(A,index=0):
 		B=index
 		try:return A.buffer[A.pointer+B]
 		except IndexError:A.update(B+1);return A.buffer[A.pointer+B]
 	def prefix(A,length=1):
 		B=length
 		if A.pointer+B>=len(A.buffer):A.update(B)
 		return A.buffer[A.pointer:A.pointer+B]
 	def forward_1_1(A,length=1):
 		B=length
 		if A.pointer+B+1>=len(A.buffer):A.update(B+1)
 		while B!=0:
 			C=A.buffer[A.pointer];A.pointer+=1;A.index+=1
-			if C in'\n\x85\u2028\u2029'or C=='\r'and A.buffer[A.pointer]!=_B:A.line+=1;A.column=0
-			elif C!=_F:A.column+=1
+			if C in'\n\x85\u2028\u2029'or C=='\r'and A.buffer[A.pointer]!='\n':A.line+=1;A.column=0
+			elif C!=_C:A.column+=1
 			B-=1
 	def forward(A,length=1):
 		B=length
 		if A.pointer+B+1>=len(A.buffer):A.update(B+1)
 		while B!=0:
 			C=A.buffer[A.pointer];A.pointer+=1;A.index+=1
-			if C==_B or C=='\r'and A.buffer[A.pointer]!=_B:A.line+=1;A.column=0
-			elif C!=_F:A.column+=1
+			if C=='\n'or C=='\r'and A.buffer[A.pointer]!='\n':A.line+=1;A.column=0
+			elif C!=_C:A.column+=1
 			B-=1
 	def get_mark(A):
 		if A.stream is _A:return StringMark(A.name,A.index,A.line,A.column,A.buffer,A.pointer)
 		else:return FileMark(A.name,A.index,A.line,A.column)
 	def determine_encoding(A):
 		while not A.eof and(A.raw_buffer is _A or len(A.raw_buffer)<2):A.update_raw()
 		if isinstance(A.raw_buffer,binary_type):
 			if A.raw_buffer.startswith(codecs.BOM_UTF16_LE):A.raw_decode=codecs.utf_16_le_decode;A.encoding='utf-16-le'
 			elif A.raw_buffer.startswith(codecs.BOM_UTF16_BE):A.raw_decode=codecs.utf_16_be_decode;A.encoding='utf-16-be'
 			else:A.raw_decode=codecs.utf_8_decode;A.encoding='utf-8'
 		A.update(1)
 	if UNICODE_SIZE==2:NON_PRINTABLE=RegExp('[^\t\n\r -~\x85\xa0-\ud7ff\ue000-�]')
 	else:NON_PRINTABLE=RegExp('[^\t\n\r -~\x85\xa0-\ud7ff\ue000-�𐀀-\U0010ffff]')
-	_printable_ascii=('\t\n\r'+''.join(map(chr,range(32,127)))).encode(_C)
+	_printable_ascii=('\t\n\r'+''.join(map(chr,range(32,127)))).encode(_B)
 	@classmethod
 	def _get_non_printable_ascii(D,data):
-		A=data.encode(_C);B=A.translate(_A,D._printable_ascii)
+		A=data.encode(_B);B=A.translate(_A,D._printable_ascii)
 		if not B:return _A
-		C=B[:1];return A.index(C),C.decode(_C)
+		C=B[:1];return A.index(C),C.decode(_B)
 	@classmethod
 	def _get_non_printable_regex(B,data):
 		A=B.NON_PRINTABLE.search(data)
 		if not bool(A):return _A
 		return A.start(),A.group()
 	@classmethod
 	def _get_non_printable(A,data):
@@ -102,15 +99,15 @@
 					else:F=B.object[B.start]
 					if A.stream is not _A:D=A.stream_pointer-len(A.raw_buffer)+B.start
 					elif A.stream is not _A:D=A.stream_pointer-len(A.raw_buffer)+B.start
 					else:D=B.start
 					raise ReaderError(A.name,D,F,B.encoding,B.reason)
 			else:C=A.raw_buffer;E=len(C)
 			A.check_printable(C);A.buffer+=C;A.raw_buffer=A.raw_buffer[E:]
-			if A.eof:A.buffer+=_E;A.raw_buffer=_A;break
+			if A.eof:A.buffer+='\x00';A.raw_buffer=_A;break
 	def update_raw(A,size=_A):
 		C=size
 		if C is _A:C=4096 if PY3 else 1024
 		B=A.stream.read(C)
 		if A.raw_buffer is _A:A.raw_buffer=B
 		else:A.raw_buffer+=B
 		A.stream_pointer+=len(B)
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/representer.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/representer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,21 @@
 from __future__ import print_function,absolute_import,division
-_e='tag:yaml.org,2002:'
-_d='state'
-_c='args'
-_b='tag:yaml.org,2002:python/object:'
-_a='__getstate__'
-_Z='tag:yaml.org,2002:set'
-_Y='-.inf'
-_X='.inf'
-_W='.nan'
-_V='base64'
-_U='utf-8'
-_T='null'
-_S='typ'
-_R='tag:yaml.org,2002:python/object/new:'
-_Q='tag:yaml.org,2002:timestamp'
-_P='tag:yaml.org,2002:map'
-_O='tag:yaml.org,2002:seq'
-_N='tag:yaml.org,2002:float'
-_M='tag:yaml.org,2002:binary'
-_L='tag:yaml.org,2002:null'
-_K=0.0
-_J='|'
-_I='%s.%s'
-_H='.'
+_T='tag:yaml.org,2002:'
+_S='tag:yaml.org,2002:python/object:'
+_R='__getstate__'
+_Q='tag:yaml.org,2002:set'
+_P='base64'
+_O='tag:yaml.org,2002:python/object/new:'
+_N='tag:yaml.org,2002:timestamp'
+_M='tag:yaml.org,2002:map'
+_L='tag:yaml.org,2002:seq'
+_K='tag:yaml.org,2002:float'
+_J='tag:yaml.org,2002:binary'
+_I='tag:yaml.org,2002:null'
+_H='%s.%s'
 _G='tag:yaml.org,2002:int'
 _F='comment'
 _E='ascii'
 _D='tag:yaml.org,2002:str'
 _C=False
 _B=True
 _A=None
@@ -56,15 +45,15 @@
 	def __init__(self,default_style=_A,default_flow_style=_A,dumper=_A):
 		self.dumper=dumper
 		if self.dumper is not _A:self.dumper._representer=self
 		self.default_style=default_style;self.default_flow_style=default_flow_style;self.represented_objects={};self.object_keeper=[];self.alias_key=_A;self.sort_base_mapping_type_on_output=_B
 	@property
 	def serializer(self):
 		try:
-			if hasattr(self.dumper,_S):return self.dumper.serializer
+			if hasattr(self.dumper,'typ'):return self.dumper.serializer
 			return self.dumper._serializer
 		except AttributeError:return self
 	def represent(self,data):node=self.represent_data(data);self.serializer.serialize(node);self.represented_objects={};self.object_keeper=[];self.alias_key=_A
 	def represent_data(self,data):
 		if self.ignore_aliases(data):self.alias_key=_A
 		else:self.alias_key=id(data)
 		if self.alias_key is not _A:
@@ -141,61 +130,61 @@
 		return node
 	def ignore_aliases(self,data):return _C
 class SafeRepresenter(BaseRepresenter):
 	def ignore_aliases(self,data):
 		if data is _A or isinstance(data,tuple)and data==():return _B
 		if isinstance(data,(binary_type,text_type,bool,int,float)):return _B
 		return _C
-	def represent_none(self,data):return self.represent_scalar(_L,_T)
+	def represent_none(self,data):return self.represent_scalar(_I,'null')
 	if PY3:
 		def represent_str(self,data):return self.represent_scalar(_D,data)
 		def represent_binary(self,data):
 			if hasattr(base64,'encodebytes'):data=base64.encodebytes(data).decode(_E)
 			else:data=base64.encodestring(data).decode(_E)
-			return self.represent_scalar(_M,data,style=_J)
+			return self.represent_scalar(_J,data,style='|')
 	else:
 		def represent_str(self,data):
 			tag=_A;style=_A
 			try:data=unicode(data,_E);tag=_D
 			except UnicodeDecodeError:
-				try:data=unicode(data,_U);tag=_D
-				except UnicodeDecodeError:data=data.encode(_V);tag=_M;style=_J
+				try:data=unicode(data,'utf-8');tag=_D
+				except UnicodeDecodeError:data=data.encode(_P);tag=_J;style='|'
 			return self.represent_scalar(tag,data,style=style)
 		def represent_unicode(self,data):return self.represent_scalar(_D,data)
 	def represent_bool(self,data,anchor=_A):
 		try:value=self.dumper.boolean_representation[bool(data)]
 		except AttributeError:
 			if data:value='true'
 			else:value='false'
 		return self.represent_scalar('tag:yaml.org,2002:bool',value,anchor=anchor)
 	def represent_int(self,data):return self.represent_scalar(_G,text_type(data))
 	if PY2:
 		def represent_long(self,data):return self.represent_scalar(_G,text_type(data))
 	inf_value=1e+300
 	while repr(inf_value)!=repr(inf_value*inf_value):inf_value*=inf_value
 	def represent_float(self,data):
-		if data!=data or data==_K and data==1.0:value=_W
-		elif data==self.inf_value:value=_X
-		elif data==-self.inf_value:value=_Y
+		if data!=data or data==0.0 and data==1.0:value='.nan'
+		elif data==self.inf_value:value='.inf'
+		elif data==-self.inf_value:value='-.inf'
 		else:
 			value=to_unicode(repr(data)).lower()
 			if getattr(self.serializer,'use_version',_A)==(1,1):
-				if _H not in value and'e'in value:value=value.replace('e','.0e',1)
-		return self.represent_scalar(_N,value)
-	def represent_list(self,data):return self.represent_sequence(_O,data)
-	def represent_dict(self,data):return self.represent_mapping(_P,data)
+				if'.'not in value and'e'in value:value=value.replace('e','.0e',1)
+		return self.represent_scalar(_K,value)
+	def represent_list(self,data):return self.represent_sequence(_L,data)
+	def represent_dict(self,data):return self.represent_mapping(_M,data)
 	def represent_ordereddict(self,data):return self.represent_omap('tag:yaml.org,2002:omap',data)
 	def represent_set(self,data):
 		value={}
 		for key in data:value[key]=_A
-		return self.represent_mapping(_Z,value)
-	def represent_date(self,data):value=to_unicode(data.isoformat());return self.represent_scalar(_Q,value)
-	def represent_datetime(self,data):value=to_unicode(data.isoformat(' '));return self.represent_scalar(_Q,value)
+		return self.represent_mapping(_Q,value)
+	def represent_date(self,data):value=to_unicode(data.isoformat());return self.represent_scalar(_N,value)
+	def represent_datetime(self,data):value=to_unicode(data.isoformat(' '));return self.represent_scalar(_N,value)
 	def represent_yaml_object(self,tag,data,cls,flow_style=_A):
-		if hasattr(data,_a):state=data.__getstate__()
+		if hasattr(data,_R):state=data.__getstate__()
 		else:state=data.__dict__.copy()
 		return self.represent_mapping(tag,state,flow_style=flow_style)
 	def represent_undefined(self,data):raise RepresenterError('cannot represent an object: %s'%(data,))
 SafeRepresenter.add_representer(type(_A),SafeRepresenter.represent_none)
 SafeRepresenter.add_representer(str,SafeRepresenter.represent_str)
 if PY2:SafeRepresenter.add_representer(unicode,SafeRepresenter.represent_unicode)
 else:SafeRepresenter.add_representer(bytes,SafeRepresenter.represent_binary)
@@ -214,68 +203,68 @@
 SafeRepresenter.add_representer(_A,SafeRepresenter.represent_undefined)
 class Representer(SafeRepresenter):
 	if PY2:
 		def represent_str(self,data):
 			tag=_A;style=_A
 			try:data=unicode(data,_E);tag=_D
 			except UnicodeDecodeError:
-				try:data=unicode(data,_U);tag='tag:yaml.org,2002:python/str'
-				except UnicodeDecodeError:data=data.encode(_V);tag=_M;style=_J
+				try:data=unicode(data,'utf-8');tag='tag:yaml.org,2002:python/str'
+				except UnicodeDecodeError:data=data.encode(_P);tag=_J;style='|'
 			return self.represent_scalar(tag,data,style=style)
 		def represent_unicode(self,data):
 			tag=_A
 			try:data.encode(_E);tag='tag:yaml.org,2002:python/unicode'
 			except UnicodeEncodeError:tag=_D
 			return self.represent_scalar(tag,data)
 		def represent_long(self,data):
 			tag=_G
 			if int(data)is not data:tag='tag:yaml.org,2002:python/long'
 			return self.represent_scalar(tag,to_unicode(data))
 	def represent_complex(self,data):
-		if data.imag==_K:data='%r'%data.real
-		elif data.real==_K:data='%rj'%data.imag
+		if data.imag==0.0:data='%r'%data.real
+		elif data.real==0.0:data='%rj'%data.imag
 		elif data.imag>0:data='%r+%rj'%(data.real,data.imag)
 		else:data='%r%rj'%(data.real,data.imag)
 		return self.represent_scalar('tag:yaml.org,2002:python/complex',data)
 	def represent_tuple(self,data):return self.represent_sequence('tag:yaml.org,2002:python/tuple',data)
 	def represent_name(self,data):
-		try:name=_I%(data.__module__,data.__qualname__)
-		except AttributeError:name=_I%(data.__module__,data.__name__)
+		try:name=_H%(data.__module__,data.__qualname__)
+		except AttributeError:name=_H%(data.__module__,data.__name__)
 		return self.represent_scalar('tag:yaml.org,2002:python/name:'+name,'')
 	def represent_module(self,data):return self.represent_scalar('tag:yaml.org,2002:python/module:'+data.__name__,'')
 	if PY2:
 		def represent_instance(self,data):
-			cls=data.__class__;class_name=_I%(cls.__module__,cls.__name__);args=_A;state=_A
+			cls=data.__class__;class_name=_H%(cls.__module__,cls.__name__);args=_A;state=_A
 			if hasattr(data,'__getinitargs__'):args=list(data.__getinitargs__())
-			if hasattr(data,_a):state=data.__getstate__()
+			if hasattr(data,_R):state=data.__getstate__()
 			else:state=data.__dict__
-			if args is _A and isinstance(state,dict):return self.represent_mapping(_b+class_name,state)
-			if isinstance(state,dict)and not state:return self.represent_sequence(_R+class_name,args)
+			if args is _A and isinstance(state,dict):return self.represent_mapping(_S+class_name,state)
+			if isinstance(state,dict)and not state:return self.represent_sequence(_O+class_name,args)
 			value={}
-			if bool(args):value[_c]=args
-			value[_d]=state;return self.represent_mapping(_R+class_name,value)
+			if bool(args):value['args']=args
+			value['state']=state;return self.represent_mapping(_O+class_name,value)
 	def represent_object(self,data):
 		cls=type(data)
 		if cls in copyreg.dispatch_table:reduce=copyreg.dispatch_table[cls](data)
 		elif hasattr(data,'__reduce_ex__'):reduce=data.__reduce_ex__(2)
 		elif hasattr(data,'__reduce__'):reduce=data.__reduce__()
 		else:raise RepresenterError('cannot represent object: %r'%(data,))
 		reduce=(list(reduce)+[_A]*5)[:5];function,args,state,listitems,dictitems=reduce;args=list(args)
 		if state is _A:state={}
 		if listitems is not _A:listitems=list(listitems)
 		if dictitems is not _A:dictitems=dict(dictitems)
-		if function.__name__=='__newobj__':function=args[0];args=args[1:];tag=_R;newobj=_B
+		if function.__name__=='__newobj__':function=args[0];args=args[1:];tag=_O;newobj=_B
 		else:tag='tag:yaml.org,2002:python/object/apply:';newobj=_C
-		try:function_name=_I%(function.__module__,function.__qualname__)
-		except AttributeError:function_name=_I%(function.__module__,function.__name__)
-		if not args and not listitems and not dictitems and isinstance(state,dict)and newobj:return self.represent_mapping(_b+function_name,state)
+		try:function_name=_H%(function.__module__,function.__qualname__)
+		except AttributeError:function_name=_H%(function.__module__,function.__name__)
+		if not args and not listitems and not dictitems and isinstance(state,dict)and newobj:return self.represent_mapping(_S+function_name,state)
 		if not listitems and not dictitems and isinstance(state,dict)and not state:return self.represent_sequence(tag+function_name,args)
 		value={}
-		if args:value[_c]=args
-		if state or not isinstance(state,dict):value[_d]=state
+		if args:value['args']=args
+		if state or not isinstance(state,dict):value['state']=state
 		if listitems:value['listitems']=listitems
 		if dictitems:value['dictitems']=dictitems
 		return self.represent_mapping(tag+function_name,value)
 if PY2:Representer.add_representer(str,Representer.represent_str);Representer.add_representer(unicode,Representer.represent_unicode);Representer.add_representer(long,Representer.represent_long)
 Representer.add_representer(complex,Representer.represent_complex)
 Representer.add_representer(tuple,Representer.represent_tuple)
 Representer.add_representer(type,Representer.represent_name)
@@ -285,26 +274,26 @@
 Representer.add_representer(types.ModuleType,Representer.represent_module)
 if PY2:Representer.add_multi_representer(types.InstanceType,Representer.represent_instance)
 Representer.add_multi_representer(object,Representer.represent_object)
 Representer.add_multi_representer(type,Representer.represent_name)
 from .comments import CommentedMap,CommentedOrderedMap,CommentedSeq,CommentedKeySeq,CommentedKeyMap,CommentedSet,comment_attrib,merge_attrib,TaggedScalar
 class RoundTripRepresenter(SafeRepresenter):
 	def __init__(self,default_style=_A,default_flow_style=_A,dumper=_A):
-		if not hasattr(dumper,_S)and default_flow_style is _A:default_flow_style=_C
+		if not hasattr(dumper,'typ')and default_flow_style is _A:default_flow_style=_C
 		SafeRepresenter.__init__(self,default_style=default_style,default_flow_style=default_flow_style,dumper=dumper)
 	def ignore_aliases(self,data):
 		try:
 			if data.anchor is not _A and data.anchor.value is not _A:return _C
 		except AttributeError:pass
 		return SafeRepresenter.ignore_aliases(self,data)
 	def represent_none(self,data):
-		if len(self.represented_objects)==0 and not self.serializer.use_explicit_start:return self.represent_scalar(_L,_T)
-		return self.represent_scalar(_L,'')
+		if len(self.represented_objects)==0 and not self.serializer.use_explicit_start:return self.represent_scalar(_I,'null')
+		return self.represent_scalar(_I,'')
 	def represent_literal_scalarstring(self,data):
-		tag=_A;style=_J;anchor=data.yaml_anchor(any=_B)
+		tag=_A;style='|';anchor=data.yaml_anchor(any=_B)
 		if PY2 and not isinstance(data,unicode):data=unicode(data,_E)
 		tag=_D;return self.represent_scalar(tag,data,style=style,anchor=anchor)
 	represent_preserved_scalarstring=represent_literal_scalarstring
 	def represent_folded_scalarstring(self,data):
 		tag=_A;style='>';anchor=data.yaml_anchor(any=_B)
 		for fold_pos in reversed(getattr(data,'fold_pos',[])):
 			if data[fold_pos]==' 'and(fold_pos>0 and not data[fold_pos-1].isspace())and(fold_pos<len(data)and not data[fold_pos+1].isspace()):data=data[:fold_pos]+'\x07'+data[fold_pos:]
@@ -349,43 +338,43 @@
 		else:s=format(data,'x')
 		anchor=data.yaml_anchor(any=_B);return self.insert_underscore('0x',s,data._underscore,anchor=anchor)
 	def represent_hex_caps_int(self,data):
 		if data._width is not _A:s='{:0{}X}'.format(data,data._width)
 		else:s=format(data,'X')
 		anchor=data.yaml_anchor(any=_B);return self.insert_underscore('0x',s,data._underscore,anchor=anchor)
 	def represent_scalar_float(self,data):
-		C='+';B='{:{}0{}d}';A='0';value=_A;anchor=data.yaml_anchor(any=_B)
-		if data!=data or data==_K and data==1.0:value=_W
-		elif data==self.inf_value:value=_X
-		elif data==-self.inf_value:value=_Y
-		if value:return self.represent_scalar(_N,value,anchor=anchor)
+		B='{:{}0{}d}';A='0';value=_A;anchor=data.yaml_anchor(any=_B)
+		if data!=data or data==0.0 and data==1.0:value='.nan'
+		elif data==self.inf_value:value='.inf'
+		elif data==-self.inf_value:value='-.inf'
+		if value:return self.represent_scalar(_K,value,anchor=anchor)
 		if data._exp is _A and data._prec>0 and data._prec==data._width-1:value='{}{:d}.'.format(data._m_sign if data._m_sign else'',abs(int(data)))
 		elif data._exp is _A:
 			prec=data._prec;ms=data._m_sign if data._m_sign else'';value='{}{:0{}.{}f}'.format(ms,abs(data),data._width-len(ms),data._width-prec-1)
-			if prec==0 or prec==1 and ms!='':value=value.replace('0.',_H)
+			if prec==0 or prec==1 and ms!='':value=value.replace('0.','.')
 			while len(value)<data._width:value+=A
 		else:
 			m,es='{:{}.{}e}'.format(data,data._width,data._width+(1 if data._m_sign else 0)).split('e');w=data._width if data._prec>0 else data._width+1
 			if data<0:w+=1
-			m=m[:w];e=int(es);m1,m2=m.split(_H)
+			m=m[:w];e=int(es);m1,m2=m.split('.')
 			while len(m1)+len(m2)<data._width-(1 if data._prec>=0 else 0):m2+=A
-			if data._m_sign and data>0:m1=C+m1
-			esgn=C if data._e_sign else''
+			if data._m_sign and data>0:m1='+'+m1
+			esgn='+'if data._e_sign else''
 			if data._prec<0:
 				if m2!=A:e-=len(m2)
 				else:m2=''
 				while len(m1)+len(m2)-(1 if data._m_sign else 0)<data._width:m2+=A;e-=1
 				value=m1+m2+data._exp+B.format(e,esgn,data._e_width)
-			elif data._prec==0:e-=len(m2);value=m1+m2+_H+data._exp+B.format(e,esgn,data._e_width)
+			elif data._prec==0:e-=len(m2);value=m1+m2+'.'+data._exp+B.format(e,esgn,data._e_width)
 			else:
 				if data._m_lead0>0:m2=A*(data._m_lead0-1)+m1+m2;m1=A;m2=m2[:-data._m_lead0];e+=data._m_lead0
 				while len(m1)<data._prec:m1+=m2[0];m2=m2[1:];e-=1
-				value=m1+_H+m2+data._exp+B.format(e,esgn,data._e_width)
+				value=m1+'.'+m2+data._exp+B.format(e,esgn,data._e_width)
 		if value is _A:value=to_unicode(repr(data)).lower()
-		return self.represent_scalar(_N,value,anchor=anchor)
+		return self.represent_scalar(_K,value,anchor=anchor)
 	def represent_sequence(self,tag,sequence,flow_style=_A):
 		value=[]
 		try:flow_style=sequence.fa.flow_style(flow_style)
 		except AttributeError:flow_style=flow_style
 		try:anchor=sequence.yaml_anchor()
 		except AttributeError:anchor=_A
 		node=SequenceNode(tag,value,flow_style=flow_style,anchor=anchor)
@@ -416,16 +405,16 @@
 		if getattr(node,_F,_A)is not _A:
 			for (idx,val) in enumerate(comments):
 				if idx>=len(node.comment):continue
 				nc=node.comment[idx]
 				if nc is not _A:assert val is _A or val==nc;comments[idx]=nc
 		node.comment=comments;return node
 	def represent_key(self,data):
-		if isinstance(data,CommentedKeySeq):self.alias_key=_A;return self.represent_sequence(_O,data,flow_style=_B)
-		if isinstance(data,CommentedKeyMap):self.alias_key=_A;return self.represent_mapping(_P,data,flow_style=_B)
+		if isinstance(data,CommentedKeySeq):self.alias_key=_A;return self.represent_sequence(_L,data,flow_style=_B)
+		if isinstance(data,CommentedKeyMap):self.alias_key=_A;return self.represent_mapping(_M,data,flow_style=_B)
 		return SafeRepresenter.represent_key(self,data)
 	def represent_mapping(self,tag,mapping,flow_style=_A):
 		value=[]
 		try:flow_style=mapping.fa.flow_style(flow_style)
 		except AttributeError:flow_style=flow_style
 		try:anchor=mapping.yaml_anchor()
 		except AttributeError:anchor=_A
@@ -495,15 +484,15 @@
 				else:node_item.value[0][1].comment=item_comment[2:]
 			value.append(node_item)
 		if flow_style is _A:
 			if self.default_flow_style is not _A:node.flow_style=self.default_flow_style
 			else:node.flow_style=best_style
 		return node
 	def represent_set(self,setting):
-		flow_style=_C;tag=_Z;value=[];flow_style=setting.fa.flow_style(flow_style)
+		flow_style=_C;tag=_Q;value=[];flow_style=setting.fa.flow_style(flow_style)
 		try:anchor=setting.yaml_anchor()
 		except AttributeError:anchor=_A
 		node=MappingNode(tag,value,flow_style=flow_style,anchor=anchor)
 		if self.alias_key is not _A:self.represented_objects[self.alias_key]=node
 		best_style=_B
 		try:
 			comment=getattr(setting,comment_attrib);node.comment=comment.comment
@@ -524,32 +513,32 @@
 			if not(isinstance(node_value,ScalarNode)and not node_value.style):best_style=_C
 			value.append((node_key,node_value))
 		best_style=best_style;return node
 	def represent_dict(self,data):
 		try:t=data.tag.value
 		except AttributeError:t=_A
 		if t:
-			if t.startswith('!!'):tag=_e+t[2:]
+			if t.startswith('!!'):tag=_T+t[2:]
 			else:tag=t
-		else:tag=_P
+		else:tag=_M
 		return self.represent_mapping(tag,data)
 	def represent_list(self,data):
 		try:t=data.tag.value
 		except AttributeError:t=_A
 		if t:
-			if t.startswith('!!'):tag=_e+t[2:]
+			if t.startswith('!!'):tag=_T+t[2:]
 			else:tag=t
-		else:tag=_O
+		else:tag=_L
 		return self.represent_sequence(tag,data)
 	def represent_datetime(self,data):
-		B='tz';A='delta';inter='T'if data._yaml['t']else' ';_yaml=data._yaml
+		A='delta';inter='T'if data._yaml['t']else' ';_yaml=data._yaml
 		if _yaml[A]:data+=_yaml[A];value=data.isoformat(inter)
 		else:value=data.isoformat(inter)
-		if _yaml[B]:value+=_yaml[B]
-		return self.represent_scalar(_Q,to_unicode(value))
+		if _yaml['tz']:value+=_yaml['tz']
+		return self.represent_scalar(_N,to_unicode(value))
 	def represent_tagged_scalar(self,data):
 		try:tag=data.tag.value
 		except AttributeError:tag=_A
 		try:anchor=data.yaml_anchor()
 		except AttributeError:anchor=_A
 		return self.represent_scalar(tag,data.value,style=data.style,anchor=anchor)
 	def represent_scalar_bool(self,data):
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/resolver.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/resolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,56 @@
 from __future__ import absolute_import
-_J='yaml_implicit_resolvers'
-_I='typ'
-_H='-+0123456789'
-_G='tag:yaml.org,2002:int'
-_F='-+0123456789.'
-_E='tag:yaml.org,2002:float'
-_D='tag:yaml.org,2002:bool'
-_C=True
+_H='yaml_implicit_resolvers'
+_G='-+0123456789'
+_F='tag:yaml.org,2002:int'
+_E='-+0123456789.'
+_D='tag:yaml.org,2002:float'
+_C='tag:yaml.org,2002:bool'
 _B=False
 _A=None
 import re
 if _B:from typing import Any,Dict,List,Union,Text,Optional;from .compat import VersionType
 from .compat import string_types,_DEFAULT_YAML_VERSION
 from .error import *
 from .nodes import MappingNode,ScalarNode,SequenceNode
 from .util import RegExp
 __all__=['BaseResolver','Resolver','VersionedResolver']
-implicit_resolvers=[([(1,2)],_D,RegExp('^(?:true|True|TRUE|false|False|FALSE)$',re.X),list('tTfF')),([(1,1)],_D,RegExp('^(?:y|Y|yes|Yes|YES|n|N|no|No|NO\n        |true|True|TRUE|false|False|FALSE\n        |on|On|ON|off|Off|OFF)$',re.X),list('yYnNtTfFoO')),([(1,2)],_E,RegExp('^(?:\n         [-+]?(?:[0-9][0-9_]*)\\.[0-9_]*(?:[eE][-+]?[0-9]+)?\n        |[-+]?(?:[0-9][0-9_]*)(?:[eE][-+]?[0-9]+)\n        |[-+]?\\.[0-9_]+(?:[eE][-+][0-9]+)?\n        |[-+]?\\.(?:inf|Inf|INF)\n        |\\.(?:nan|NaN|NAN))$',re.X),list(_F)),([(1,1)],_E,RegExp('^(?:\n         [-+]?(?:[0-9][0-9_]*)\\.[0-9_]*(?:[eE][-+]?[0-9]+)?\n        |[-+]?(?:[0-9][0-9_]*)(?:[eE][-+]?[0-9]+)\n        |\\.[0-9_]+(?:[eE][-+][0-9]+)?\n        |[-+]?[0-9][0-9_]*(?::[0-5]?[0-9])+\\.[0-9_]*  # sexagesimal float\n        |[-+]?\\.(?:inf|Inf|INF)\n        |\\.(?:nan|NaN|NAN))$',re.X),list(_F)),([(1,2)],_G,RegExp('^(?:[-+]?0b[0-1_]+\n        |[-+]?0o?[0-7_]+\n        |[-+]?[0-9_]+\n        |[-+]?0x[0-9a-fA-F_]+)$',re.X),list(_H)),([(1,1)],_G,RegExp('^(?:[-+]?0b[0-1_]+\n        |[-+]?0?[0-7_]+\n        |[-+]?(?:0|[1-9][0-9_]*)\n        |[-+]?0x[0-9a-fA-F_]+\n        |[-+]?[1-9][0-9_]*(?::[0-5]?[0-9])+)$',re.X),list(_H)),([(1,2),(1,1)],'tag:yaml.org,2002:merge',RegExp('^(?:<<)$'),['<']),([(1,2),(1,1)],'tag:yaml.org,2002:null',RegExp('^(?: ~\n        |null|Null|NULL\n        | )$',re.X),['~','n','N','']),([(1,2),(1,1)],'tag:yaml.org,2002:timestamp',RegExp('^(?:[0-9][0-9][0-9][0-9]-[0-9][0-9]-[0-9][0-9]\n        |[0-9][0-9][0-9][0-9] -[0-9][0-9]? -[0-9][0-9]?\n        (?:[Tt]|[ \\t]+)[0-9][0-9]?\n        :[0-9][0-9] :[0-9][0-9] (?:\\.[0-9]*)?\n        (?:[ \\t]*(?:Z|[-+][0-9][0-9]?(?::[0-9][0-9])?))?)$',re.X),list('0123456789')),([(1,2),(1,1)],'tag:yaml.org,2002:value',RegExp('^(?:=)$'),['=']),([(1,2),(1,1)],'tag:yaml.org,2002:yaml',RegExp('^(?:!|&|\\*)$'),list('!&*'))]
+implicit_resolvers=[([(1,2)],_C,RegExp('^(?:true|True|TRUE|false|False|FALSE)$',re.X),list('tTfF')),([(1,1)],_C,RegExp('^(?:y|Y|yes|Yes|YES|n|N|no|No|NO\n        |true|True|TRUE|false|False|FALSE\n        |on|On|ON|off|Off|OFF)$',re.X),list('yYnNtTfFoO')),([(1,2)],_D,RegExp('^(?:\n         [-+]?(?:[0-9][0-9_]*)\\.[0-9_]*(?:[eE][-+]?[0-9]+)?\n        |[-+]?(?:[0-9][0-9_]*)(?:[eE][-+]?[0-9]+)\n        |[-+]?\\.[0-9_]+(?:[eE][-+][0-9]+)?\n        |[-+]?\\.(?:inf|Inf|INF)\n        |\\.(?:nan|NaN|NAN))$',re.X),list(_E)),([(1,1)],_D,RegExp('^(?:\n         [-+]?(?:[0-9][0-9_]*)\\.[0-9_]*(?:[eE][-+]?[0-9]+)?\n        |[-+]?(?:[0-9][0-9_]*)(?:[eE][-+]?[0-9]+)\n        |\\.[0-9_]+(?:[eE][-+][0-9]+)?\n        |[-+]?[0-9][0-9_]*(?::[0-5]?[0-9])+\\.[0-9_]*  # sexagesimal float\n        |[-+]?\\.(?:inf|Inf|INF)\n        |\\.(?:nan|NaN|NAN))$',re.X),list(_E)),([(1,2)],_F,RegExp('^(?:[-+]?0b[0-1_]+\n        |[-+]?0o?[0-7_]+\n        |[-+]?[0-9_]+\n        |[-+]?0x[0-9a-fA-F_]+)$',re.X),list(_G)),([(1,1)],_F,RegExp('^(?:[-+]?0b[0-1_]+\n        |[-+]?0?[0-7_]+\n        |[-+]?(?:0|[1-9][0-9_]*)\n        |[-+]?0x[0-9a-fA-F_]+\n        |[-+]?[1-9][0-9_]*(?::[0-5]?[0-9])+)$',re.X),list(_G)),([(1,2),(1,1)],'tag:yaml.org,2002:merge',RegExp('^(?:<<)$'),['<']),([(1,2),(1,1)],'tag:yaml.org,2002:null',RegExp('^(?: ~\n        |null|Null|NULL\n        | )$',re.X),['~','n','N','']),([(1,2),(1,1)],'tag:yaml.org,2002:timestamp',RegExp('^(?:[0-9][0-9][0-9][0-9]-[0-9][0-9]-[0-9][0-9]\n        |[0-9][0-9][0-9][0-9] -[0-9][0-9]? -[0-9][0-9]?\n        (?:[Tt]|[ \\t]+)[0-9][0-9]?\n        :[0-9][0-9] :[0-9][0-9] (?:\\.[0-9]*)?\n        (?:[ \\t]*(?:Z|[-+][0-9][0-9]?(?::[0-9][0-9])?))?)$',re.X),list('0123456789')),([(1,2),(1,1)],'tag:yaml.org,2002:value',RegExp('^(?:=)$'),['=']),([(1,2),(1,1)],'tag:yaml.org,2002:yaml',RegExp('^(?:!|&|\\*)$'),list('!&*'))]
 class ResolverError(YAMLError):0
 class BaseResolver:
 	DEFAULT_SCALAR_TAG='tag:yaml.org,2002:str';DEFAULT_SEQUENCE_TAG='tag:yaml.org,2002:seq';DEFAULT_MAPPING_TAG='tag:yaml.org,2002:map';yaml_implicit_resolvers={};yaml_path_resolvers={}
 	def __init__(self,loadumper=_A):
 		self.loadumper=loadumper
 		if self.loadumper is not _A and getattr(self.loadumper,'_resolver',_A)is _A:self.loadumper._resolver=self.loadumper
 		self._loader_version=_A;self.resolver_exact_paths=[];self.resolver_prefix_paths=[]
 	@property
 	def parser(self):
 		if self.loadumper is not _A:
-			if hasattr(self.loadumper,_I):return self.loadumper.parser
+			if hasattr(self.loadumper,'typ'):return self.loadumper.parser
 			return self.loadumper._parser
 		return _A
 	@classmethod
 	def add_implicit_resolver_base(cls,tag,regexp,first):
-		if _J not in cls.__dict__:cls.yaml_implicit_resolvers=dict(((k,cls.yaml_implicit_resolvers[k][:])for k in cls.yaml_implicit_resolvers))
+		if _H not in cls.__dict__:cls.yaml_implicit_resolvers=dict(((k,cls.yaml_implicit_resolvers[k][:])for k in cls.yaml_implicit_resolvers))
 		if first is _A:first=[_A]
 		for ch in first:cls.yaml_implicit_resolvers.setdefault(ch,[]).append((tag,regexp))
 	@classmethod
 	def add_implicit_resolver(cls,tag,regexp,first):
-		if _J not in cls.__dict__:cls.yaml_implicit_resolvers=dict(((k,cls.yaml_implicit_resolvers[k][:])for k in cls.yaml_implicit_resolvers))
+		if _H not in cls.__dict__:cls.yaml_implicit_resolvers=dict(((k,cls.yaml_implicit_resolvers[k][:])for k in cls.yaml_implicit_resolvers))
 		if first is _A:first=[_A]
 		for ch in first:cls.yaml_implicit_resolvers.setdefault(ch,[]).append((tag,regexp))
 		implicit_resolvers.append(([(1,2),(1,1)],tag,regexp,first))
 	@classmethod
 	def add_path_resolver(cls,tag,path,kind=_A):
 		if'yaml_path_resolvers'not in cls.__dict__:cls.yaml_path_resolvers=cls.yaml_path_resolvers.copy()
 		new_path=[]
 		for element in path:
 			if isinstance(element,(list,tuple)):
 				if len(element)==2:node_check,index_check=element
-				elif len(element)==1:node_check=element[0];index_check=_C
+				elif len(element)==1:node_check=element[0];index_check=True
 				else:raise ResolverError('Invalid path element: %s'%(element,))
 			else:node_check=_A;index_check=element
 			if node_check is str:node_check=ScalarNode
 			elif node_check is list:node_check=SequenceNode
 			elif node_check is dict:node_check=MappingNode
 			elif node_check not in[ScalarNode,SequenceNode,MappingNode]and not isinstance(node_check,string_types)and node_check is not _A:raise ResolverError('Invalid node checker: %s'%(node_check,))
 			if not isinstance(index_check,(string_types,int))and index_check is not _A:raise ResolverError('Invalid index checker: %s'%(index_check,))
@@ -81,21 +79,21 @@
 		self.resolver_exact_paths.pop();self.resolver_prefix_paths.pop()
 	def check_resolver_prefix(self,depth,path,kind,current_node,current_index):
 		node_check,index_check=path[depth-1]
 		if isinstance(node_check,string_types):
 			if current_node.tag!=node_check:return _B
 		elif node_check is not _A:
 			if not isinstance(current_node,node_check):return _B
-		if index_check is _C and current_index is not _A:return _B
+		if index_check is True and current_index is not _A:return _B
 		if(index_check is _B or index_check is _A)and current_index is _A:return _B
 		if isinstance(index_check,string_types):
 			if not(isinstance(current_index,ScalarNode)and index_check==current_index.value):return _B
 		elif isinstance(index_check,int)and not isinstance(index_check,bool):
 			if index_check!=current_index:return _B
-		return _C
+		return True
 	def resolve(self,kind,value,implicit):
 		if kind is ScalarNode and implicit[0]:
 			if value=='':resolvers=self.yaml_implicit_resolvers.get('',[])
 			else:resolvers=self.yaml_implicit_resolvers.get(value[0],[])
 			resolvers+=self.yaml_implicit_resolvers.get(_A,[])
 			for (tag,regexp) in resolvers:
 				if regexp.match(value):return tag
@@ -147,14 +145,14 @@
 		elif kind is SequenceNode:return self.DEFAULT_SEQUENCE_TAG
 		elif kind is MappingNode:return self.DEFAULT_MAPPING_TAG
 	@property
 	def processing_version(self):
 		try:version=self.loadumper._scanner.yaml_version
 		except AttributeError:
 			try:
-				if hasattr(self.loadumper,_I):version=self.loadumper.version
+				if hasattr(self.loadumper,'typ'):version=self.loadumper.version
 				else:version=self.loadumper._serializer.use_version
 			except AttributeError:version=_A
 		if version is _A:
 			version=self._loader_version
 			if version is _A:version=_DEFAULT_YAML_VERSION
 		return version
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/scalarbool.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/scalarbool.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 _B=False
 _A=None
 from .anchor import Anchor
 if _B:from typing import Text,Any,Dict,List
 __all__=['ScalarBoolean']
 class ScalarBoolean(int):
 	def __new__(D,*E,**A):
-		B=A.pop('anchor',_A);C=int.__new__(D,*E,**A)
+		B=A.pop('anchor',_A);C=int.__new__(D,*(E),**A)
 		if B is not _A:C.yaml_set_anchor(B,always_dump=True)
 		return C
 	@property
 	def anchor(self):
 		A=self
 		if not hasattr(A,Anchor.attrib):setattr(A,Anchor.attrib,Anchor())
 		return getattr(A,Anchor.attrib)
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/scalarfloat.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/scalarfloat.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 from .compat import no_limit_int
 from .anchor import Anchor
 if _B:from typing import Text,Any,Dict,List
 __all__=['ScalarFloat','ExponentialFloat','ExponentialCapsFloat']
 class ScalarFloat(float):
 	def __new__(D,*E,**A):
-		F=A.pop('width',_A);G=A.pop('prec',_A);H=A.pop('m_sign',_A);I=A.pop('m_lead0',0);J=A.pop('exp',_A);K=A.pop('e_width',_A);L=A.pop('e_sign',_A);M=A.pop('underscore',_A);C=A.pop('anchor',_A);B=float.__new__(D,*E,**A);B._width=F;B._prec=G;B._m_sign=H;B._m_lead0=I;B._exp=J;B._e_width=K;B._e_sign=L;B._underscore=M
+		F=A.pop('width',_A);G=A.pop('prec',_A);H=A.pop('m_sign',_A);I=A.pop('m_lead0',0);J=A.pop('exp',_A);K=A.pop('e_width',_A);L=A.pop('e_sign',_A);M=A.pop('underscore',_A);C=A.pop('anchor',_A);B=float.__new__(D,*(E),**A);B._width=F;B._prec=G;B._m_sign=H;B._m_lead0=I;B._exp=J;B._e_width=K;B._e_sign=L;B._underscore=M
 		if C is not _A:B.yaml_set_anchor(C,always_dump=True)
 		return B
 	def __iadd__(A,a):return float(A)+a;B=type(A)(A+a);B._width=A._width;B._underscore=A._underscore[:]if A._underscore is not _A else _A;return B
 	def __ifloordiv__(A,a):return float(A)//a;B=type(A)(A//a);B._width=A._width;B._underscore=A._underscore[:]if A._underscore is not _A else _A;return B
 	def __imul__(A,a):return float(A)*a;B=type(A)(A*a);B._width=A._width;B._underscore=A._underscore[:]if A._underscore is not _A else _A;B._prec=A._prec;return B
 	def __ipow__(A,a):return float(A)**a;B=type(A)(A**a);B._width=A._width;B._underscore=A._underscore[:]if A._underscore is not _A else _A;return B
 	def __isub__(A,a):return float(A)-a;B=type(A)(A-a);B._width=A._width;B._underscore=A._underscore[:]if A._underscore is not _A else _A;return B
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/scalarint.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/scalarint.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 _A=None
 from .compat import no_limit_int
 from .anchor import Anchor
 if _B:from typing import Text,Any,Dict,List
 __all__=['ScalarInt','BinaryInt','OctalInt','HexInt','HexCapsInt','DecimalInt']
 class ScalarInt(no_limit_int):
 	def __new__(D,*E,**A):
-		F=A.pop('width',_A);G=A.pop('underscore',_A);C=A.pop('anchor',_A);B=no_limit_int.__new__(D,*E,**A);B._width=F;B._underscore=G
+		F=A.pop('width',_A);G=A.pop('underscore',_A);C=A.pop('anchor',_A);B=no_limit_int.__new__(D,*(E),**A);B._width=F;B._underscore=G
 		if C is not _A:B.yaml_set_anchor(C,always_dump=True)
 		return B
 	def __iadd__(A,a):B=type(A)(A+a);B._width=A._width;B._underscore=A._underscore[:]if A._underscore is not _A else _A;return B
 	def __ifloordiv__(A,a):B=type(A)(A//a);B._width=A._width;B._underscore=A._underscore[:]if A._underscore is not _A else _A;return B
 	def __imul__(A,a):B=type(A)(A*a);B._width=A._width;B._underscore=A._underscore[:]if A._underscore is not _A else _A;return B
 	def __ipow__(A,a):B=type(A)(A**a);B._width=A._width;B._underscore=A._underscore[:]if A._underscore is not _A else _A;return B
 	def __isub__(A,a):B=type(A)(A-a);B._width=A._width;B._underscore=A._underscore[:]if A._underscore is not _A else _A;return B
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/scalarstring.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/scalarstring.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 from __future__ import print_function,absolute_import,division,unicode_literals
-_D='comment'
-_C='\n'
+_C='comment'
 _B=False
 _A=None
 from .compat import text_type
 from .anchor import Anchor
 if _B:from typing import Text,Any,Dict,List
 __all__=['ScalarString','LiteralScalarString','FoldedScalarString','SingleQuotedScalarString','DoubleQuotedScalarString','PlainScalarString','PreservedScalarString']
 class ScalarString(text_type):
 	__slots__=Anchor.attrib
 	def __new__(D,*E,**A):
-		B=A.pop('anchor',_A);C=text_type.__new__(D,*E,**A)
+		B=A.pop('anchor',_A);C=text_type.__new__(D,*(E),**A)
 		if B is not _A:C.yaml_set_anchor(B,always_dump=True)
 		return C
 	def replace(A,old,new,maxreplace=-1):return type(A)(text_type.replace(A,old,new,maxreplace))
 	@property
 	def anchor(self):
 		A=self
 		if not hasattr(A,Anchor.attrib):setattr(A,Anchor.attrib,Anchor())
 		return getattr(A,Anchor.attrib)
 	def yaml_anchor(A,any=_B):
 		if not hasattr(A,Anchor.attrib):return _A
 		if any or A.anchor.always_dump:return A.anchor
 		return _A
 	def yaml_set_anchor(A,value,always_dump=_B):A.anchor.value=value;A.anchor.always_dump=always_dump
 class LiteralScalarString(ScalarString):
-	__slots__=_D;style='|'
+	__slots__=_C;style='|'
 	def __new__(A,value,anchor=_A):return ScalarString.__new__(A,value,anchor=anchor)
 PreservedScalarString=LiteralScalarString
 class FoldedScalarString(ScalarString):
-	__slots__='fold_pos',_D;style='>'
+	__slots__='fold_pos',_C;style='>'
 	def __new__(A,value,anchor=_A):return ScalarString.__new__(A,value,anchor=anchor)
 class SingleQuotedScalarString(ScalarString):
 	__slots__=();style="'"
 	def __new__(A,value,anchor=_A):return ScalarString.__new__(A,value,anchor=anchor)
 class DoubleQuotedScalarString(ScalarString):
 	__slots__=();style='"'
 	def __new__(A,value,anchor=_A):return ScalarString.__new__(A,value,anchor=anchor)
 class PlainScalarString(ScalarString):
 	__slots__=();style=''
 	def __new__(A,value,anchor=_A):return ScalarString.__new__(A,value,anchor=anchor)
-def preserve_literal(s):return LiteralScalarString(s.replace('\r\n',_C).replace('\r',_C))
+def preserve_literal(s):return LiteralScalarString(s.replace('\r\n','\n').replace('\r','\n'))
 def walk_tree(base,map=_A):
 	A=base;from dynaconf.vendor.ruamel.yaml.compat import string_types as E,MutableMapping as G,MutableSequence as H
-	if map is _A:map={_C:preserve_literal}
+	if map is _A:map={'\n':preserve_literal}
 	if isinstance(A,G):
 		for F in A:
 			C=A[F]
 			if isinstance(C,E):
 				for B in map:
 					if B in C:A[F]=map[B](C);break
 			else:walk_tree(C)
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/scanner.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/scanner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,27 @@
 from __future__ import print_function,absolute_import,division,unicode_literals
-_o='\u2028\u2029'
-_n='\r\n'
-_m='\r\n\x85'
-_l='while scanning a quoted scalar'
-_k='0123456789ABCDEFabcdef'
-_j=' \r\n\x85\u2028\u2029'
-_i='\x07'
-_h='expected a comment or a line break, but found %r'
-_g='directive'
-_f='\ufeff'
-_e="could not find expected ':'"
-_d='while scanning a simple key'
-_c='typ'
-_b='\\'
-_a='\t'
-_Z="expected ' ', but found %r"
-_Y='while scanning a %s'
-_X='\r\n\x85\u2028\u2029'
-_W='while scanning a block scalar'
-_V='expected alphabetic or numeric character, but found %r'
-_U='a'
-_T='...'
-_S='---'
-_R='>'
-_Q='9'
-_P='"'
-_O=':'
-_N='-'
-_M=' \t'
-_L='\x00 \r\n\x85\u2028\u2029'
-_K='0'
-_J="'"
+_b='\u2028\u2029'
+_a='\r\n\x85'
+_Z='while scanning a quoted scalar'
+_Y='0123456789ABCDEFabcdef'
+_X=' \r\n\x85\u2028\u2029'
+_W='expected a comment or a line break, but found %r'
+_V='directive'
+_U='\ufeff'
+_T="could not find expected ':'"
+_S='while scanning a simple key'
+_R="expected ' ', but found %r"
+_Q='while scanning a %s'
+_P='\r\n\x85\u2028\u2029'
+_O='while scanning a block scalar'
+_N='expected alphabetic or numeric character, but found %r'
+_M='...'
+_L='---'
+_K=' \t'
+_J='\x00 \r\n\x85\u2028\u2029'
 _I='\x00'
 _H='!'
 _G='while scanning a directive'
 _F='#'
 _E='\n'
 _D=' '
 _C=None
@@ -43,15 +30,15 @@
 from .error import MarkedYAMLError
 from .tokens import *
 from .compat import utf8,unichr,PY3,check_anchorname_char,nprint
 if _B:from typing import Any,Dict,Optional,List,Union,Text;from .compat import VersionType
 __all__=['Scanner','RoundTripScanner','ScannerError']
 _THE_END='\n\x00\r\x85\u2028\u2029'
 _THE_END_SPACE_TAB=' \n\x00\t\r\x85\u2028\u2029'
-_SPACE_TAB=_M
+_SPACE_TAB=_K
 class ScannerError(MarkedYAMLError):0
 class SimpleKey:
 	def __init__(self,token_number,required,index,line,column,mark):self.token_number=token_number;self.required=required;self.index=index;self.line=line;self.column=column;self.mark=mark
 class Scanner:
 	def __init__(self,loader=_C):
 		self.loader=loader
 		if self.loader is not _C and getattr(self.loader,'_scanner',_C)is _C:self.loader._scanner=self
@@ -59,20 +46,20 @@
 	@property
 	def flow_level(self):return len(self.flow_context)
 	def reset_scanner(self):self.done=_B;self.flow_context=[];self.tokens=[];self.fetch_stream_start();self.tokens_taken=0;self.indent=-1;self.indents=[];self.allow_simple_key=_A;self.possible_simple_keys={}
 	@property
 	def reader(self):
 		try:return self._scanner_reader
 		except AttributeError:
-			if hasattr(self.loader,_c):self._scanner_reader=self.loader.reader
+			if hasattr(self.loader,'typ'):self._scanner_reader=self.loader.reader
 			else:self._scanner_reader=self.loader._reader
 			return self._scanner_reader
 	@property
 	def scanner_processing_version(self):
-		if hasattr(self.loader,_c):return self.loader.resolver.processing_version
+		if hasattr(self.loader,'typ'):return self.loader.resolver.processing_version
 		return self.loader.processing_version
 	def check_token(self,*choices):
 		while self.need_more_tokens():self.fetch_more_tokens()
 		if bool(self.tokens):
 			if not choices:return _A
 			for choice in choices:
 				if isinstance(self.tokens[0],choice):return _A
@@ -92,52 +79,52 @@
 	def fetch_comment(self,comment):raise NotImplementedError
 	def fetch_more_tokens(self):
 		comment=self.scan_to_next_token()
 		if comment is not _C:return self.fetch_comment(comment)
 		self.stale_possible_simple_keys();self.unwind_indent(self.reader.column);ch=self.reader.peek()
 		if ch==_I:return self.fetch_stream_end()
 		if ch=='%'and self.check_directive():return self.fetch_directive()
-		if ch==_N and self.check_document_start():return self.fetch_document_start()
+		if ch=='-'and self.check_document_start():return self.fetch_document_start()
 		if ch=='.'and self.check_document_end():return self.fetch_document_end()
 		if ch=='[':return self.fetch_flow_sequence_start()
 		if ch=='{':return self.fetch_flow_mapping_start()
 		if ch==']':return self.fetch_flow_sequence_end()
 		if ch=='}':return self.fetch_flow_mapping_end()
 		if ch==',':return self.fetch_flow_entry()
-		if ch==_N and self.check_block_entry():return self.fetch_block_entry()
+		if ch=='-'and self.check_block_entry():return self.fetch_block_entry()
 		if ch=='?'and self.check_key():return self.fetch_key()
-		if ch==_O and self.check_value():return self.fetch_value()
+		if ch==':'and self.check_value():return self.fetch_value()
 		if ch=='*':return self.fetch_alias()
 		if ch=='&':return self.fetch_anchor()
 		if ch==_H:return self.fetch_tag()
 		if ch=='|'and not self.flow_level:return self.fetch_literal()
-		if ch==_R and not self.flow_level:return self.fetch_folded()
-		if ch==_J:return self.fetch_single()
-		if ch==_P:return self.fetch_double()
+		if ch=='>'and not self.flow_level:return self.fetch_folded()
+		if ch=="'":return self.fetch_single()
+		if ch=='"':return self.fetch_double()
 		if self.check_plain():return self.fetch_plain()
 		raise ScannerError('while scanning for the next token',_C,'found character %r that cannot start any token'%utf8(ch),self.reader.get_mark())
 	def next_possible_simple_key(self):
 		min_token_number=_C
 		for level in self.possible_simple_keys:
 			key=self.possible_simple_keys[level]
 			if min_token_number is _C or key.token_number<min_token_number:min_token_number=key.token_number
 		return min_token_number
 	def stale_possible_simple_keys(self):
 		for level in list(self.possible_simple_keys):
 			key=self.possible_simple_keys[level]
 			if key.line!=self.reader.line or self.reader.index-key.index>1024:
-				if key.required:raise ScannerError(_d,key.mark,_e,self.reader.get_mark())
+				if key.required:raise ScannerError(_S,key.mark,_T,self.reader.get_mark())
 				del self.possible_simple_keys[level]
 	def save_possible_simple_key(self):
 		required=not self.flow_level and self.indent==self.reader.column
 		if self.allow_simple_key:self.remove_possible_simple_key();token_number=self.tokens_taken+len(self.tokens);key=SimpleKey(token_number,required,self.reader.index,self.reader.line,self.reader.column,self.reader.get_mark());self.possible_simple_keys[self.flow_level]=key
 	def remove_possible_simple_key(self):
 		if self.flow_level in self.possible_simple_keys:
 			key=self.possible_simple_keys[self.flow_level]
-			if key.required:raise ScannerError(_d,key.mark,_e,self.reader.get_mark())
+			if key.required:raise ScannerError(_S,key.mark,_T,self.reader.get_mark())
 			del self.possible_simple_keys[self.flow_level]
 	def unwind_indent(self,column):
 		if bool(self.flow_level):return
 		while self.indent>column:mark=self.reader.get_mark();self.indent=self.indents.pop();self.tokens.append(BlockEndToken(mark,mark))
 	def add_indent(self,column):
 		if self.indent<column:self.indents.append(self.indent);self.indent=column;return _A
 		return _B
@@ -182,30 +169,30 @@
 				if self.add_indent(self.reader.column):mark=self.reader.get_mark();self.tokens.append(BlockMappingStartToken(mark,mark))
 			self.allow_simple_key=not self.flow_level;self.remove_possible_simple_key()
 		start_mark=self.reader.get_mark();self.reader.forward();end_mark=self.reader.get_mark();self.tokens.append(ValueToken(start_mark,end_mark))
 	def fetch_alias(self):self.save_possible_simple_key();self.allow_simple_key=_B;self.tokens.append(self.scan_anchor(AliasToken))
 	def fetch_anchor(self):self.save_possible_simple_key();self.allow_simple_key=_B;self.tokens.append(self.scan_anchor(AnchorToken))
 	def fetch_tag(self):self.save_possible_simple_key();self.allow_simple_key=_B;self.tokens.append(self.scan_tag())
 	def fetch_literal(self):self.fetch_block_scalar(style='|')
-	def fetch_folded(self):self.fetch_block_scalar(style=_R)
+	def fetch_folded(self):self.fetch_block_scalar(style='>')
 	def fetch_block_scalar(self,style):self.allow_simple_key=_A;self.remove_possible_simple_key();self.tokens.append(self.scan_block_scalar(style))
-	def fetch_single(self):self.fetch_flow_scalar(style=_J)
-	def fetch_double(self):self.fetch_flow_scalar(style=_P)
+	def fetch_single(self):self.fetch_flow_scalar(style="'")
+	def fetch_double(self):self.fetch_flow_scalar(style='"')
 	def fetch_flow_scalar(self,style):self.save_possible_simple_key();self.allow_simple_key=_B;self.tokens.append(self.scan_flow_scalar(style))
 	def fetch_plain(self):self.save_possible_simple_key();self.allow_simple_key=_B;self.tokens.append(self.scan_plain())
 	def check_directive(self):
 		if self.reader.column==0:return _A
 		return _C
 	def check_document_start(self):
 		if self.reader.column==0:
-			if self.reader.prefix(3)==_S and self.reader.peek(3)in _THE_END_SPACE_TAB:return _A
+			if self.reader.prefix(3)==_L and self.reader.peek(3)in _THE_END_SPACE_TAB:return _A
 		return _C
 	def check_document_end(self):
 		if self.reader.column==0:
-			if self.reader.prefix(3)==_T and self.reader.peek(3)in _THE_END_SPACE_TAB:return _A
+			if self.reader.prefix(3)==_M and self.reader.peek(3)in _THE_END_SPACE_TAB:return _A
 		return _C
 	def check_block_entry(self):return self.reader.peek(1)in _THE_END_SPACE_TAB
 	def check_key(self):
 		if bool(self.flow_level):return _A
 		return self.reader.peek(1)in _THE_END_SPACE_TAB
 	def check_value(self):
 		if self.scanner_processing_version==(1,1):
@@ -214,24 +201,24 @@
 			if self.flow_context[-1]=='[':
 				if self.reader.peek(1)not in _THE_END_SPACE_TAB:return _B
 			elif self.tokens and isinstance(self.tokens[-1],ValueToken):
 				if self.reader.peek(1)not in _THE_END_SPACE_TAB:return _B
 			return _A
 		return self.reader.peek(1)in _THE_END_SPACE_TAB
 	def check_plain(self):
-		B='?:';A='\x00 \t\r\n\x85\u2028\u2029-?:,[]{}#&*!|>\'"%@`';srp=self.reader.peek;ch=srp()
-		if self.scanner_processing_version==(1,1):return ch not in A or srp(1)not in _THE_END_SPACE_TAB and(ch==_N or not self.flow_level and ch in B)
+		A='\x00 \t\r\n\x85\u2028\u2029-?:,[]{}#&*!|>\'"%@`';srp=self.reader.peek;ch=srp()
+		if self.scanner_processing_version==(1,1):return ch not in A or srp(1)not in _THE_END_SPACE_TAB and(ch=='-'or not self.flow_level and ch in'?:')
 		if ch not in A:return _A
 		ch1=srp(1)
-		if ch==_N and ch1 not in _THE_END_SPACE_TAB:return _A
-		if ch==_O and bool(self.flow_level)and ch1 not in _SPACE_TAB:return _A
-		return srp(1)not in _THE_END_SPACE_TAB and(ch==_N or not self.flow_level and ch in B)
+		if ch=='-'and ch1 not in _THE_END_SPACE_TAB:return _A
+		if ch==':'and bool(self.flow_level)and ch1 not in _SPACE_TAB:return _A
+		return srp(1)not in _THE_END_SPACE_TAB and(ch=='-'or not self.flow_level and ch in'?:')
 	def scan_to_next_token(self):
 		srp=self.reader.peek;srf=self.reader.forward
-		if self.reader.index==0 and srp()==_f:srf()
+		if self.reader.index==0 and srp()==_U:srf()
 		found=_B;_the_end=_THE_END
 		while not found:
 			while srp()==_D:srf()
 			if srp()==_F:
 				while srp()not in _the_end:srf()
 			if self.scan_line_break():
 				if not self.flow_level:self.allow_simple_key=_A
@@ -243,105 +230,105 @@
 		elif name=='TAG':value=self.scan_tag_directive_value(start_mark);end_mark=self.reader.get_mark()
 		else:
 			end_mark=self.reader.get_mark()
 			while srp()not in _THE_END:srf()
 		self.scan_directive_ignored_line(start_mark);return DirectiveToken(name,value,start_mark,end_mark)
 	def scan_directive_name(self,start_mark):
 		length=0;srp=self.reader.peek;ch=srp(length)
-		while _K<=ch<=_Q or'A'<=ch<='Z'or _U<=ch<='z'or ch in'-_:.':length+=1;ch=srp(length)
-		if not length:raise ScannerError(_G,start_mark,_V%utf8(ch),self.reader.get_mark())
+		while '0'<=ch<='9'or'A'<=ch<='Z'or'a'<=ch<='z'or ch in'-_:.':length+=1;ch=srp(length)
+		if not length:raise ScannerError(_G,start_mark,_N%utf8(ch),self.reader.get_mark())
 		value=self.reader.prefix(length);self.reader.forward(length);ch=srp()
-		if ch not in _L:raise ScannerError(_G,start_mark,_V%utf8(ch),self.reader.get_mark())
+		if ch not in _J:raise ScannerError(_G,start_mark,_N%utf8(ch),self.reader.get_mark())
 		return value
 	def scan_yaml_directive_value(self,start_mark):
 		srp=self.reader.peek;srf=self.reader.forward
 		while srp()==_D:srf()
 		major=self.scan_yaml_directive_number(start_mark)
 		if srp()!='.':raise ScannerError(_G,start_mark,"expected a digit or '.', but found %r"%utf8(srp()),self.reader.get_mark())
 		srf();minor=self.scan_yaml_directive_number(start_mark)
-		if srp()not in _L:raise ScannerError(_G,start_mark,"expected a digit or ' ', but found %r"%utf8(srp()),self.reader.get_mark())
+		if srp()not in _J:raise ScannerError(_G,start_mark,"expected a digit or ' ', but found %r"%utf8(srp()),self.reader.get_mark())
 		self.yaml_version=major,minor;return self.yaml_version
 	def scan_yaml_directive_number(self,start_mark):
 		srp=self.reader.peek;srf=self.reader.forward;ch=srp()
-		if not _K<=ch<=_Q:raise ScannerError(_G,start_mark,'expected a digit, but found %r'%utf8(ch),self.reader.get_mark())
+		if not'0'<=ch<='9':raise ScannerError(_G,start_mark,'expected a digit, but found %r'%utf8(ch),self.reader.get_mark())
 		length=0
-		while _K<=srp(length)<=_Q:length+=1
+		while '0'<=srp(length)<='9':length+=1
 		value=int(self.reader.prefix(length));srf(length);return value
 	def scan_tag_directive_value(self,start_mark):
 		srp=self.reader.peek;srf=self.reader.forward
 		while srp()==_D:srf()
 		handle=self.scan_tag_directive_handle(start_mark)
 		while srp()==_D:srf()
 		prefix=self.scan_tag_directive_prefix(start_mark);return handle,prefix
 	def scan_tag_directive_handle(self,start_mark):
-		value=self.scan_tag_handle(_g,start_mark);ch=self.reader.peek()
-		if ch!=_D:raise ScannerError(_G,start_mark,_Z%utf8(ch),self.reader.get_mark())
+		value=self.scan_tag_handle(_V,start_mark);ch=self.reader.peek()
+		if ch!=_D:raise ScannerError(_G,start_mark,_R%utf8(ch),self.reader.get_mark())
 		return value
 	def scan_tag_directive_prefix(self,start_mark):
-		value=self.scan_tag_uri(_g,start_mark);ch=self.reader.peek()
-		if ch not in _L:raise ScannerError(_G,start_mark,_Z%utf8(ch),self.reader.get_mark())
+		value=self.scan_tag_uri(_V,start_mark);ch=self.reader.peek()
+		if ch not in _J:raise ScannerError(_G,start_mark,_R%utf8(ch),self.reader.get_mark())
 		return value
 	def scan_directive_ignored_line(self,start_mark):
 		srp=self.reader.peek;srf=self.reader.forward
 		while srp()==_D:srf()
 		if srp()==_F:
 			while srp()not in _THE_END:srf()
 		ch=srp()
-		if ch not in _THE_END:raise ScannerError(_G,start_mark,_h%utf8(ch),self.reader.get_mark())
+		if ch not in _THE_END:raise ScannerError(_G,start_mark,_W%utf8(ch),self.reader.get_mark())
 		self.scan_line_break()
 	def scan_anchor(self,TokenClass):
 		A='while scanning an %s';srp=self.reader.peek;start_mark=self.reader.get_mark();indicator=srp()
 		if indicator=='*':name='alias'
 		else:name='anchor'
 		self.reader.forward();length=0;ch=srp(length)
 		while check_anchorname_char(ch):length+=1;ch=srp(length)
-		if not length:raise ScannerError(A%(name,),start_mark,_V%utf8(ch),self.reader.get_mark())
+		if not length:raise ScannerError(A%(name,),start_mark,_N%utf8(ch),self.reader.get_mark())
 		value=self.reader.prefix(length);self.reader.forward(length)
-		if ch not in'\x00 \t\r\n\x85\u2028\u2029?:,[]{}%@`':raise ScannerError(A%(name,),start_mark,_V%utf8(ch),self.reader.get_mark())
+		if ch not in'\x00 \t\r\n\x85\u2028\u2029?:,[]{}%@`':raise ScannerError(A%(name,),start_mark,_N%utf8(ch),self.reader.get_mark())
 		end_mark=self.reader.get_mark();return TokenClass(value,start_mark,end_mark)
 	def scan_tag(self):
 		A='tag';srp=self.reader.peek;start_mark=self.reader.get_mark();ch=srp(1)
 		if ch=='<':
 			handle=_C;self.reader.forward(2);suffix=self.scan_tag_uri(A,start_mark)
-			if srp()!=_R:raise ScannerError('while parsing a tag',start_mark,"expected '>', but found %r"%utf8(srp()),self.reader.get_mark())
+			if srp()!='>':raise ScannerError('while parsing a tag',start_mark,"expected '>', but found %r"%utf8(srp()),self.reader.get_mark())
 			self.reader.forward()
 		elif ch in _THE_END_SPACE_TAB:handle=_C;suffix=_H;self.reader.forward()
 		else:
 			length=1;use_handle=_B
-			while ch not in _L:
+			while ch not in _J:
 				if ch==_H:use_handle=_A;break
 				length+=1;ch=srp(length)
 			handle=_H
 			if use_handle:handle=self.scan_tag_handle(A,start_mark)
 			else:handle=_H;self.reader.forward()
 			suffix=self.scan_tag_uri(A,start_mark)
 		ch=srp()
-		if ch not in _L:raise ScannerError('while scanning a tag',start_mark,_Z%utf8(ch),self.reader.get_mark())
+		if ch not in _J:raise ScannerError('while scanning a tag',start_mark,_R%utf8(ch),self.reader.get_mark())
 		value=handle,suffix;end_mark=self.reader.get_mark();return TagToken(value,start_mark,end_mark)
 	def scan_block_scalar(self,style,rt=_B):
-		A='|>';srp=self.reader.peek
-		if style==_R:folded=_A
+		srp=self.reader.peek
+		if style=='>':folded=_A
 		else:folded=_B
 		chunks=[];start_mark=self.reader.get_mark();self.reader.forward();chomping,increment=self.scan_block_scalar_indicators(start_mark);block_scalar_comment=self.scan_block_scalar_ignored_line(start_mark);min_indent=self.indent+1
 		if increment is _C:
-			if min_indent<1 and(style not in A or self.scanner_processing_version==(1,1)and getattr(self.loader,'top_level_block_style_scalar_no_indent_error_1_1',_B)):min_indent=1
+			if min_indent<1 and(style not in'|>'or self.scanner_processing_version==(1,1)and getattr(self.loader,'top_level_block_style_scalar_no_indent_error_1_1',_B)):min_indent=1
 			breaks,max_indent,end_mark=self.scan_block_scalar_indentation();indent=max(min_indent,max_indent)
 		else:
 			if min_indent<1:min_indent=1
 			indent=min_indent+increment-1;breaks,end_mark=self.scan_block_scalar_breaks(indent)
 		line_break=''
 		while self.reader.column==indent and srp()!=_I:
-			chunks.extend(breaks);leading_non_space=srp()not in _M;length=0
+			chunks.extend(breaks);leading_non_space=srp()not in _K;length=0
 			while srp(length)not in _THE_END:length+=1
 			chunks.append(self.reader.prefix(length));self.reader.forward(length);line_break=self.scan_line_break();breaks,end_mark=self.scan_block_scalar_breaks(indent)
-			if style in A and min_indent==0:
+			if style in'|>'and min_indent==0:
 				if self.check_document_start()or self.check_document_end():break
 			if self.reader.column==indent and srp()!=_I:
-				if rt and folded and line_break==_E:chunks.append(_i)
-				if folded and line_break==_E and leading_non_space and srp()not in _M:
+				if rt and folded and line_break==_E:chunks.append('\x07')
+				if folded and line_break==_E and leading_non_space and srp()not in _K:
 					if not breaks:chunks.append(_D)
 				else:chunks.append(line_break)
 			else:break
 		trailing=[]
 		if chomping in[_C,_A]:chunks.append(line_break)
 		if chomping is _A:chunks.extend(breaks)
 		elif chomping in[_C,_B]:trailing.extend(breaks)
@@ -349,180 +336,180 @@
 		if block_scalar_comment is not _C:token.add_pre_comments([block_scalar_comment])
 		if len(trailing)>0:
 			comment=self.scan_to_next_token()
 			while comment:trailing.append(_D*comment[1].column+comment[0]);comment=self.scan_to_next_token()
 			comment_end_mark=self.reader.get_mark();comment=CommentToken(''.join(trailing),end_mark,comment_end_mark);token.add_post_comment(comment)
 		return token
 	def scan_block_scalar_indicators(self,start_mark):
-		D='expected indentation indicator in the range 1-9, but found 0';C='0123456789';B='+';A='+-';srp=self.reader.peek;chomping=_C;increment=_C;ch=srp()
-		if ch in A:
-			if ch==B:chomping=_A
+		B='expected indentation indicator in the range 1-9, but found 0';A='0123456789';srp=self.reader.peek;chomping=_C;increment=_C;ch=srp()
+		if ch in'+-':
+			if ch=='+':chomping=_A
 			else:chomping=_B
 			self.reader.forward();ch=srp()
-			if ch in C:
+			if ch in A:
 				increment=int(ch)
-				if increment==0:raise ScannerError(_W,start_mark,D,self.reader.get_mark())
+				if increment==0:raise ScannerError(_O,start_mark,B,self.reader.get_mark())
 				self.reader.forward()
-		elif ch in C:
+		elif ch in A:
 			increment=int(ch)
-			if increment==0:raise ScannerError(_W,start_mark,D,self.reader.get_mark())
+			if increment==0:raise ScannerError(_O,start_mark,B,self.reader.get_mark())
 			self.reader.forward();ch=srp()
-			if ch in A:
-				if ch==B:chomping=_A
+			if ch in'+-':
+				if ch=='+':chomping=_A
 				else:chomping=_B
 				self.reader.forward()
 		ch=srp()
-		if ch not in _L:raise ScannerError(_W,start_mark,'expected chomping or indentation indicators, but found %r'%utf8(ch),self.reader.get_mark())
+		if ch not in _J:raise ScannerError(_O,start_mark,'expected chomping or indentation indicators, but found %r'%utf8(ch),self.reader.get_mark())
 		return chomping,increment
 	def scan_block_scalar_ignored_line(self,start_mark):
 		srp=self.reader.peek;srf=self.reader.forward;prefix='';comment=_C
 		while srp()==_D:prefix+=srp();srf()
 		if srp()==_F:
 			comment=prefix
 			while srp()not in _THE_END:comment+=srp();srf()
 		ch=srp()
-		if ch not in _THE_END:raise ScannerError(_W,start_mark,_h%utf8(ch),self.reader.get_mark())
+		if ch not in _THE_END:raise ScannerError(_O,start_mark,_W%utf8(ch),self.reader.get_mark())
 		self.scan_line_break();return comment
 	def scan_block_scalar_indentation(self):
 		srp=self.reader.peek;srf=self.reader.forward;chunks=[];max_indent=0;end_mark=self.reader.get_mark()
-		while srp()in _j:
+		while srp()in _X:
 			if srp()!=_D:chunks.append(self.scan_line_break());end_mark=self.reader.get_mark()
 			else:
 				srf()
 				if self.reader.column>max_indent:max_indent=self.reader.column
 		return chunks,max_indent,end_mark
 	def scan_block_scalar_breaks(self,indent):
 		chunks=[];srp=self.reader.peek;srf=self.reader.forward;end_mark=self.reader.get_mark()
 		while self.reader.column<indent and srp()==_D:srf()
-		while srp()in _X:
+		while srp()in _P:
 			chunks.append(self.scan_line_break());end_mark=self.reader.get_mark()
 			while self.reader.column<indent and srp()==_D:srf()
 		return chunks,end_mark
 	def scan_flow_scalar(self,style):
-		if style==_P:double=_A
+		if style=='"':double=_A
 		else:double=_B
 		srp=self.reader.peek;chunks=[];start_mark=self.reader.get_mark();quote=srp();self.reader.forward();chunks.extend(self.scan_flow_scalar_non_spaces(double,start_mark))
 		while srp()!=quote:chunks.extend(self.scan_flow_scalar_spaces(double,start_mark));chunks.extend(self.scan_flow_scalar_non_spaces(double,start_mark))
 		self.reader.forward();end_mark=self.reader.get_mark();return ScalarToken(''.join(chunks),_B,start_mark,end_mark,style)
-	ESCAPE_REPLACEMENTS={_K:_I,_U:_i,'b':'\x08','t':_a,_a:_a,'n':_E,'v':'\x0b','f':'\x0c','r':'\r','e':'\x1b',_D:_D,_P:_P,'/':'/',_b:_b,'N':'\x85','_':'\xa0','L':'\u2028','P':'\u2029'};ESCAPE_CODES={'x':2,'u':4,'U':8}
+	ESCAPE_REPLACEMENTS={'0':_I,'a':'\x07','b':'\x08','t':'\t','\t':'\t','n':_E,'v':'\x0b','f':'\x0c','r':'\r','e':'\x1b',_D:_D,'"':'"','/':'/','\\':'\\','N':'\x85','_':'\xa0','L':'\u2028','P':'\u2029'};ESCAPE_CODES={'x':2,'u':4,'U':8}
 	def scan_flow_scalar_non_spaces(self,double,start_mark):
 		A='while scanning a double-quoted scalar';chunks=[];srp=self.reader.peek;srf=self.reader.forward
 		while _A:
 			length=0
 			while srp(length)not in' \n\'"\\\x00\t\r\x85\u2028\u2029':length+=1
 			if length!=0:chunks.append(self.reader.prefix(length));srf(length)
 			ch=srp()
-			if not double and ch==_J and srp(1)==_J:chunks.append(_J);srf(2)
-			elif double and ch==_J or not double and ch in'"\\':chunks.append(ch);srf()
-			elif double and ch==_b:
+			if not double and ch=="'"and srp(1)=="'":chunks.append("'");srf(2)
+			elif double and ch=="'"or not double and ch in'"\\':chunks.append(ch);srf()
+			elif double and ch=='\\':
 				srf();ch=srp()
 				if ch in self.ESCAPE_REPLACEMENTS:chunks.append(self.ESCAPE_REPLACEMENTS[ch]);srf()
 				elif ch in self.ESCAPE_CODES:
 					length=self.ESCAPE_CODES[ch];srf()
 					for k in range(length):
-						if srp(k)not in _k:raise ScannerError(A,start_mark,'expected escape sequence of %d hexdecimal numbers, but found %r'%(length,utf8(srp(k))),self.reader.get_mark())
+						if srp(k)not in _Y:raise ScannerError(A,start_mark,'expected escape sequence of %d hexdecimal numbers, but found %r'%(length,utf8(srp(k))),self.reader.get_mark())
 					code=int(self.reader.prefix(length),16);chunks.append(unichr(code));srf(length)
 				elif ch in'\n\r\x85\u2028\u2029':self.scan_line_break();chunks.extend(self.scan_flow_scalar_breaks(double,start_mark))
 				else:raise ScannerError(A,start_mark,'found unknown escape character %r'%utf8(ch),self.reader.get_mark())
 			else:return chunks
 	def scan_flow_scalar_spaces(self,double,start_mark):
 		srp=self.reader.peek;chunks=[];length=0
-		while srp(length)in _M:length+=1
+		while srp(length)in _K:length+=1
 		whitespaces=self.reader.prefix(length);self.reader.forward(length);ch=srp()
-		if ch==_I:raise ScannerError(_l,start_mark,'found unexpected end of stream',self.reader.get_mark())
-		elif ch in _X:
+		if ch==_I:raise ScannerError(_Z,start_mark,'found unexpected end of stream',self.reader.get_mark())
+		elif ch in _P:
 			line_break=self.scan_line_break();breaks=self.scan_flow_scalar_breaks(double,start_mark)
 			if line_break!=_E:chunks.append(line_break)
 			elif not breaks:chunks.append(_D)
 			chunks.extend(breaks)
 		else:chunks.append(whitespaces)
 		return chunks
 	def scan_flow_scalar_breaks(self,double,start_mark):
 		chunks=[];srp=self.reader.peek;srf=self.reader.forward
 		while _A:
 			prefix=self.reader.prefix(3)
-			if(prefix==_S or prefix==_T)and srp(3)in _THE_END_SPACE_TAB:raise ScannerError(_l,start_mark,'found unexpected document separator',self.reader.get_mark())
-			while srp()in _M:srf()
-			if srp()in _X:chunks.append(self.scan_line_break())
+			if(prefix==_L or prefix==_M)and srp(3)in _THE_END_SPACE_TAB:raise ScannerError(_Z,start_mark,'found unexpected document separator',self.reader.get_mark())
+			while srp()in _K:srf()
+			if srp()in _P:chunks.append(self.scan_line_break())
 			else:return chunks
 	def scan_plain(self):
 		srp=self.reader.peek;srf=self.reader.forward;chunks=[];start_mark=self.reader.get_mark();end_mark=start_mark;indent=self.indent+1;spaces=[]
 		while _A:
 			length=0
 			if srp()==_F:break
 			while _A:
 				ch=srp(length)
-				if ch==_O and srp(length+1)not in _THE_END_SPACE_TAB:0
+				if ch==':'and srp(length+1)not in _THE_END_SPACE_TAB:0
 				elif ch=='?'and self.scanner_processing_version!=(1,1):0
-				elif ch in _THE_END_SPACE_TAB or not self.flow_level and ch==_O and srp(length+1)in _THE_END_SPACE_TAB or self.flow_level and ch in',:?[]{}':break
+				elif ch in _THE_END_SPACE_TAB or not self.flow_level and ch==':'and srp(length+1)in _THE_END_SPACE_TAB or self.flow_level and ch in',:?[]{}':break
 				length+=1
-			if self.flow_level and ch==_O and srp(length+1)not in'\x00 \t\r\n\x85\u2028\u2029,[]{}':srf(length);raise ScannerError('while scanning a plain scalar',start_mark,"found unexpected ':'",self.reader.get_mark(),'Please check http://pyyaml.org/wiki/YAMLColonInFlowContext for details.')
+			if self.flow_level and ch==':'and srp(length+1)not in'\x00 \t\r\n\x85\u2028\u2029,[]{}':srf(length);raise ScannerError('while scanning a plain scalar',start_mark,"found unexpected ':'",self.reader.get_mark(),'Please check http://pyyaml.org/wiki/YAMLColonInFlowContext for details.')
 			if length==0:break
 			self.allow_simple_key=_B;chunks.extend(spaces);chunks.append(self.reader.prefix(length));srf(length);end_mark=self.reader.get_mark();spaces=self.scan_plain_spaces(indent,start_mark)
 			if not spaces or srp()==_F or not self.flow_level and self.reader.column<indent:break
 		token=ScalarToken(''.join(chunks),_A,start_mark,end_mark)
 		if spaces and spaces[0]==_E:comment=CommentToken(''.join(spaces)+_E,start_mark,end_mark);token.add_post_comment(comment)
 		return token
 	def scan_plain_spaces(self,indent,start_mark):
 		srp=self.reader.peek;srf=self.reader.forward;chunks=[];length=0
 		while srp(length)in _D:length+=1
 		whitespaces=self.reader.prefix(length);self.reader.forward(length);ch=srp()
-		if ch in _X:
+		if ch in _P:
 			line_break=self.scan_line_break();self.allow_simple_key=_A;prefix=self.reader.prefix(3)
-			if(prefix==_S or prefix==_T)and srp(3)in _THE_END_SPACE_TAB:return
+			if(prefix==_L or prefix==_M)and srp(3)in _THE_END_SPACE_TAB:return
 			breaks=[]
-			while srp()in _j:
+			while srp()in _X:
 				if srp()==_D:srf()
 				else:
 					breaks.append(self.scan_line_break());prefix=self.reader.prefix(3)
-					if(prefix==_S or prefix==_T)and srp(3)in _THE_END_SPACE_TAB:return
+					if(prefix==_L or prefix==_M)and srp(3)in _THE_END_SPACE_TAB:return
 			if line_break!=_E:chunks.append(line_break)
 			elif not breaks:chunks.append(_D)
 			chunks.extend(breaks)
 		elif whitespaces:chunks.append(whitespaces)
 		return chunks
 	def scan_tag_handle(self,name,start_mark):
 		A="expected '!', but found %r";srp=self.reader.peek;ch=srp()
-		if ch!=_H:raise ScannerError(_Y%(name,),start_mark,A%utf8(ch),self.reader.get_mark())
+		if ch!=_H:raise ScannerError(_Q%(name,),start_mark,A%utf8(ch),self.reader.get_mark())
 		length=1;ch=srp(length)
 		if ch!=_D:
-			while _K<=ch<=_Q or'A'<=ch<='Z'or _U<=ch<='z'or ch in'-_':length+=1;ch=srp(length)
-			if ch!=_H:self.reader.forward(length);raise ScannerError(_Y%(name,),start_mark,A%utf8(ch),self.reader.get_mark())
+			while '0'<=ch<='9'or'A'<=ch<='Z'or'a'<=ch<='z'or ch in'-_':length+=1;ch=srp(length)
+			if ch!=_H:self.reader.forward(length);raise ScannerError(_Q%(name,),start_mark,A%utf8(ch),self.reader.get_mark())
 			length+=1
 		value=self.reader.prefix(length);self.reader.forward(length);return value
 	def scan_tag_uri(self,name,start_mark):
 		srp=self.reader.peek;chunks=[];length=0;ch=srp(length)
-		while _K<=ch<=_Q or'A'<=ch<='Z'or _U<=ch<='z'or ch in"-;/?:@&=+$,_.!~*'()[]%"or self.scanner_processing_version>(1,1)and ch==_F:
+		while '0'<=ch<='9'or'A'<=ch<='Z'or'a'<=ch<='z'or ch in"-;/?:@&=+$,_.!~*'()[]%"or self.scanner_processing_version>(1,1)and ch==_F:
 			if ch=='%':chunks.append(self.reader.prefix(length));self.reader.forward(length);length=0;chunks.append(self.scan_uri_escapes(name,start_mark))
 			else:length+=1
 			ch=srp(length)
 		if length!=0:chunks.append(self.reader.prefix(length));self.reader.forward(length);length=0
 		if not chunks:raise ScannerError('while parsing a %s'%(name,),start_mark,'expected URI, but found %r'%utf8(ch),self.reader.get_mark())
 		return ''.join(chunks)
 	def scan_uri_escapes(self,name,start_mark):
 		A='utf-8';srp=self.reader.peek;srf=self.reader.forward;code_bytes=[];mark=self.reader.get_mark()
 		while srp()=='%':
 			srf()
 			for k in range(2):
-				if srp(k)not in _k:raise ScannerError(_Y%(name,),start_mark,'expected URI escape sequence of 2 hexdecimal numbers, but found %r'%utf8(srp(k)),self.reader.get_mark())
+				if srp(k)not in _Y:raise ScannerError(_Q%(name,),start_mark,'expected URI escape sequence of 2 hexdecimal numbers, but found %r'%utf8(srp(k)),self.reader.get_mark())
 			if PY3:code_bytes.append(int(self.reader.prefix(2),16))
 			else:code_bytes.append(chr(int(self.reader.prefix(2),16)))
 			srf(2)
 		try:
 			if PY3:value=bytes(code_bytes).decode(A)
 			else:value=unicode(b''.join(code_bytes),A)
-		except UnicodeDecodeError as exc:raise ScannerError(_Y%(name,),start_mark,str(exc),mark)
+		except UnicodeDecodeError as exc:raise ScannerError(_Q%(name,),start_mark,str(exc),mark)
 		return value
 	def scan_line_break(self):
 		ch=self.reader.peek()
-		if ch in _m:
-			if self.reader.prefix(2)==_n:self.reader.forward(2)
+		if ch in _a:
+			if self.reader.prefix(2)=='\r\n':self.reader.forward(2)
 			else:self.reader.forward()
 			return _E
-		elif ch in _o:self.reader.forward();return ch
+		elif ch in _b:self.reader.forward();return ch
 		return''
 class RoundTripScanner(Scanner):
 	def check_token(self,*choices):
 		while self.need_more_tokens():self.fetch_more_tokens()
 		self._gather_comments()
 		if bool(self.tokens):
 			if not choices:return _A
@@ -559,15 +546,15 @@
 		return _C
 	def fetch_comment(self,comment):
 		value,start_mark,end_mark=comment
 		while value and value[-1]==_D:value=value[:-1]
 		self.tokens.append(CommentToken(value,start_mark,end_mark))
 	def scan_to_next_token(self):
 		srp=self.reader.peek;srf=self.reader.forward
-		if self.reader.index==0 and srp()==_f:srf()
+		if self.reader.index==0 and srp()==_U:srf()
 		found=_B
 		while not found:
 			while srp()==_D:srf()
 			ch=srp()
 			if ch==_F:
 				start_mark=self.reader.get_mark();comment=ch;srf()
 				while ch not in _THE_END:
@@ -588,15 +575,15 @@
 					while ch:ch=self.scan_line_break(empty_line=_A);comment+=ch
 					if srp()==_F:comment=comment.rsplit(_E,1)[0]+_E
 					end_mark=self.reader.get_mark();return comment,start_mark,end_mark
 			else:found=_A
 		return _C
 	def scan_line_break(self,empty_line=_B):
 		ch=self.reader.peek()
-		if ch in _m:
-			if self.reader.prefix(2)==_n:self.reader.forward(2)
+		if ch in _a:
+			if self.reader.prefix(2)=='\r\n':self.reader.forward(2)
 			else:self.reader.forward()
 			return _E
-		elif ch in _o:self.reader.forward();return ch
+		elif ch in _b:self.reader.forward();return ch
 		elif empty_line and ch in'\t ':self.reader.forward();return ch
 		return''
 	def scan_block_scalar(self,style,rt=_A):return Scanner.scan_block_scalar(self,style,rt=rt)
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/serializer.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/serializer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import absolute_import
-_F='serializer is not opened'
-_E='serializer is closed'
-_D='typ'
+_E='serializer is not opened'
+_D='serializer is closed'
 _C=False
 _B=True
 _A=None
 from .error import YAMLError
 from .compat import nprint,DBG_NODE,dbg,string_types,nprintf
 from .util import RegExp
 from .events import StreamStartEvent,StreamEndEvent,MappingStartEvent,MappingEndEvent,SequenceStartEvent,SequenceEndEvent,AliasEvent,ScalarEvent,DocumentStartEvent,DocumentEndEvent
@@ -21,33 +20,33 @@
 		A.use_encoding=encoding;A.use_explicit_start=explicit_start;A.use_explicit_end=explicit_end
 		if isinstance(B,string_types):A.use_version=tuple(map(int,B.split('.')))
 		else:A.use_version=B
 		A.use_tags=tags;A.serialized_nodes={};A.anchors={};A.last_anchor_id=0;A.closed=_A;A._templated_id=_A
 	@property
 	def emitter(self):
 		A=self
-		if hasattr(A.dumper,_D):return A.dumper.emitter
+		if hasattr(A.dumper,'typ'):return A.dumper.emitter
 		return A.dumper._emitter
 	@property
 	def resolver(self):
 		A=self
-		if hasattr(A.dumper,_D):A.dumper.resolver
+		if hasattr(A.dumper,'typ'):A.dumper.resolver
 		return A.dumper._resolver
 	def open(A):
 		if A.closed is _A:A.emitter.emit(StreamStartEvent(encoding=A.use_encoding));A.closed=_C
-		elif A.closed:raise SerializerError(_E)
+		elif A.closed:raise SerializerError(_D)
 		else:raise SerializerError('serializer is already opened')
 	def close(A):
-		if A.closed is _A:raise SerializerError(_F)
+		if A.closed is _A:raise SerializerError(_E)
 		elif not A.closed:A.emitter.emit(StreamEndEvent());A.closed=_B
 	def serialize(A,node):
 		B=node
 		if dbg(DBG_NODE):nprint('Serializing nodes');B.dump()
-		if A.closed is _A:raise SerializerError(_F)
-		elif A.closed:raise SerializerError(_E)
+		if A.closed is _A:raise SerializerError(_E)
+		elif A.closed:raise SerializerError(_D)
 		A.emitter.emit(DocumentStartEvent(explicit=A.use_explicit_start,version=A.use_version,tags=A.use_tags));A.anchor_node(B);A.serialize_node(B,_A,_A);A.emitter.emit(DocumentEndEvent(explicit=A.use_explicit_end));A.serialized_nodes={};A.anchors={};A.last_anchor_id=0
 	def anchor_node(B,node):
 		A=node
 		if A in B.anchors:
 			if B.anchors[A]is _A:B.anchors[A]=B.generate_anchor(A)
 		else:
 			C=_A
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/setup.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from __future__ import print_function,absolute_import,division,unicode_literals
-_V='bdist_wheel'
-_U='--version'
-_T='extra_packages'
-_S='universal'
-_R='nested'
-_Q='setting  distdir {}/{}'
-_P='nsp'
-_O='PYDISTBASE'
-_N='True'
+_T='bdist_wheel'
+_S='--version'
+_R='extra_packages'
+_Q='universal'
+_P='nested'
+_O='setting  distdir {}/{}'
+_N='PYDISTBASE'
 _M='DVDEBUG'
 _L='LICENSE'
 _K='Jython'
 _J='install'
 _I='full_package_name'
 _H='__init__.py'
 _G='python'
@@ -43,17 +41,17 @@
 else:open_kw=dict(encoding=_E)
 if sys.version_info<(2,7)or platform.python_implementation()==_K:
 	class Set:0
 if os.environ.get(_M,'')=='':
 	def debug(*args,**kw):0
 else:
 	def debug(*args,**kw):
-		with open(os.environ[_M],'a')as fp:kw1=kw.copy();kw1['file']=fp;print('{:%Y-%d-%mT%H:%M:%S}'.format(datetime.datetime.now()),file=fp,end=' ');print(*args,**kw1)
+		with open(os.environ[_M],'a')as fp:kw1=kw.copy();kw1['file']=fp;print('{:%Y-%d-%mT%H:%M:%S}'.format(datetime.datetime.now()),file=fp,end=' ');print(*(args),**kw1)
 def literal_eval(node_or_string):
-	_safe_names={'None':_A,_N:_D,'False':_C}
+	_safe_names={'None':_A,'True':_D,'False':_C}
 	if isinstance(node_or_string,string_type):node_or_string=parse(node_or_string,mode='eval')
 	if isinstance(node_or_string,Expression):node_or_string=node_or_string.body
 	else:raise TypeError('only string or AST nodes supported')
 	def _convert(node):
 		if isinstance(node,Str):
 			if sys.version_info<(3,)and not isinstance(node.s,unicode):return node.s.decode(_E)
 			return node.s
@@ -74,16 +72,16 @@
 			left=_convert(node.left);right=_convert(node.right)
 			if isinstance(node.op,Add):return left+right
 			else:return left-right
 		elif isinstance(node,Call):
 			func_id=getattr(node.func,'id',_A)
 			if func_id=='dict':return dict(((k.arg,_convert(k.value))for k in node.keywords))
 			elif func_id=='set':return set(_convert(node.args[0]))
-			elif func_id=='date':return datetime.date(*[_convert(k)for k in node.args])
-			elif func_id=='datetime':return datetime.datetime(*[_convert(k)for k in node.args])
+			elif func_id=='date':return datetime.date(*([_convert(k)for k in node.args]))
+			elif func_id=='datetime':return datetime.datetime(*([_convert(k)for k in node.args]))
 		err=SyntaxError('malformed node or string: '+repr(node));err.filename='<string>';err.lineno=node.lineno;err.offset=node.col_offset;err.text=repr(node);err.node=node;raise err
 	return _convert(node_or_string)
 def _package_data(fn):
 	data={}
 	with open(fn,**open_kw)as fp:
 		parsing=_C;lines=[]
 		for line in fp.readlines():
@@ -134,33 +132,33 @@
 		for x in outfiles:
 			for full_exclude_file in full_exclude_files:
 				if full_exclude_file in x:os.remove(x);break
 			else:alt_files.append(x)
 		return alt_files
 class MySdist(_sdist):
 	def initialize_options(self):
-		_sdist.initialize_options(self);dist_base=os.environ.get(_O);fpn=getattr(getattr(self,_P,self),_I,_A)
-		if fpn and dist_base:print(_Q.format(dist_base,fpn));self.dist_dir=os.path.join(dist_base,fpn)
+		_sdist.initialize_options(self);dist_base=os.environ.get(_N);fpn=getattr(getattr(self,'nsp',self),_I,_A)
+		if fpn and dist_base:print(_O.format(dist_base,fpn));self.dist_dir=os.path.join(dist_base,fpn)
 try:
 	from wheel.bdist_wheel import bdist_wheel as _bdist_wheel
 	class MyBdistWheel(_bdist_wheel):
 		def initialize_options(self):
-			_bdist_wheel.initialize_options(self);dist_base=os.environ.get(_O);fpn=getattr(getattr(self,_P,self),_I,_A)
-			if fpn and dist_base:print(_Q.format(dist_base,fpn));self.dist_dir=os.path.join(dist_base,fpn)
+			_bdist_wheel.initialize_options(self);dist_base=os.environ.get(_N);fpn=getattr(getattr(self,'nsp',self),_I,_A)
+			if fpn and dist_base:print(_O.format(dist_base,fpn));self.dist_dir=os.path.join(dist_base,fpn)
 	_bdist_wheel_available=_D
 except ImportError:_bdist_wheel_available=_C
 class NameSpacePackager:
 	def __init__(self,pkg_data):
-		assert isinstance(pkg_data,dict);self._pkg_data=pkg_data;self.full_package_name=self.pn(self._pkg_data[_I]);self._split=_A;self.depth=self.full_package_name.count(_B);self.nested=self._pkg_data.get(_R,_C)
+		assert isinstance(pkg_data,dict);self._pkg_data=pkg_data;self.full_package_name=self.pn(self._pkg_data[_I]);self._split=_A;self.depth=self.full_package_name.count(_B);self.nested=self._pkg_data.get(_P,_C)
 		if self.nested:NameSpaceInstaller.install_namespaces=lambda x:_A
 		self.command=_A;self.python_version();self._pkg=[_A,_A]
 		if sys.argv[0]==_F and sys.argv[1]==_J and'--single-version-externally-managed'not in sys.argv:
-			if os.environ.get('READTHEDOCS',_A)==_N:os.system('pip install .');sys.exit(0)
+			if os.environ.get('READTHEDOCS',_A)=='True':os.system('pip install .');sys.exit(0)
 			if not os.environ.get('RUAMEL_NO_PIP_INSTALL_CHECK',_C):print('error: you have to install with "pip install ."');sys.exit(1)
-		if self._pkg_data.get(_S):Distribution.is_pure=lambda *args:_D
+		if self._pkg_data.get(_Q):Distribution.is_pure=lambda *args:_D
 		else:Distribution.is_pure=lambda *args:_C
 		for x in sys.argv:
 			if x[0]=='-'or x==_F:continue
 			self.command=x;break
 	def pn(self,s):
 		if sys.version_info<(3,)and isinstance(s,unicode):return s.encode(_E)
 		return s
@@ -171,15 +169,15 @@
 			fpn=self.full_package_name.split(_B);self._split=[]
 			while fpn:self._split.insert(0,_B.join(fpn));fpn=fpn[:-1]
 			for d in sorted(os.listdir(_B)):
 				if not os.path.isdir(d)or d==self._split[0]or d[0]in'._':continue
 				x=os.path.join(d,_H)
 				if os.path.exists(x):
 					pd=_package_data(x)
-					if pd.get(_R,_C):skip.append(d);continue
+					if pd.get(_P,_C):skip.append(d);continue
 					self._split.append(self.full_package_name+_B+d)
 			if sys.version_info<(3,):self._split=[y.encode(_E)if isinstance(y,unicode)else y for y in self._split]
 		if skip:0
 		return self._split
 	@property
 	def namespace_packages(self):return self.split[:self.depth]
 	def namespace_directories(self,depth=_A):
@@ -187,15 +185,15 @@
 		for (index,d) in enumerate(self.split[:depth]):
 			if index>0:d=os.path.join(*d.split(_B))
 			res.append(_B+d)
 		return res
 	@property
 	def package_dir(self):
 		d={self.full_package_name:_B}
-		if _T in self._pkg_data:return d
+		if _R in self._pkg_data:return d
 		if len(self.split)>1:d[self.split[0]]=self.namespace_directories(1)[0]
 		return d
 	def create_dirs(self):
 		directories=self.namespace_directories(self.depth)
 		if not directories:return
 		if not os.path.exists(directories[0]):
 			for d in directories:
@@ -262,17 +260,17 @@
 		if lic is _A:return'MIT license'
 		return lic
 	def has_mit_lic(self):return'MIT'in self.license
 	@property
 	def description(self):return self._pkg_data['description']
 	@property
 	def status(self):
-		A='β';status=self._pkg_data.get('status',A).lower()
+		status=self._pkg_data.get('status','β').lower()
 		if status in['α','alpha']:return 3,'Alpha'
-		elif status in[A,'beta']:return 4,'Beta'
+		elif status in['β','beta']:return 4,'Beta'
 		elif'stable'in status.lower():return 5,'Production/Stable'
 		raise NotImplementedError
 	@property
 	def classifiers(self):
 		attr='_'+sys._getframe().f_code.co_name
 		if not hasattr(self,attr):setattr(self,attr,self._setup_classifiers())
 		return getattr(self,attr)
@@ -315,22 +313,22 @@
 		pd=self._pkg_data.get('package_data',{})
 		if df:pd[self.full_package_name]=df
 		if sys.version_info<(3,):
 			for k in pd:
 				if isinstance(k,unicode):pd[str(k)]=pd.pop(k)
 		return pd
 	@property
-	def packages(self):s=self.split;return s+self._pkg_data.get(_T,[])
+	def packages(self):s=self.split;return s+self._pkg_data.get(_R,[])
 	@property
 	def python_requires(self):return self._pkg_data.get('python_requires',_A)
 	@property
 	def ext_modules(self):
 		I='Exception:';H='link error';G='compile error:';F='Windows';E='lib';D='src';C='ext_modules';B='test';A='name'
 		if hasattr(self,'_ext_modules'):return self._ext_modules
-		if _U in sys.argv:return _A
+		if _S in sys.argv:return _A
 		if platform.python_implementation()==_K:return _A
 		try:
 			plat=sys.argv.index('--plat-name')
 			if'win'in sys.argv[plat+1]:return _A
 		except ValueError:pass
 		self._ext_modules=[];no_test_compile=_C
 		if'--restructuredtext'in sys.argv:no_test_compile=_D
@@ -359,34 +357,34 @@
 				debug(I,e);print(I,e)
 				if sys.version_info[:2]==(3,4)and platform.system()==F:traceback.print_exc()
 			finally:shutil.rmtree(tmp_dir)
 		return self._ext_modules
 	@property
 	def test_suite(self):return self._pkg_data.get('test_suite')
 	def wheel(self,kw,setup):
-		if _V not in sys.argv:return _C
+		if _T not in sys.argv:return _C
 		file_name='setup.cfg'
 		if os.path.exists(file_name):return _C
 		with open(file_name,'w')as fp:
 			if os.path.exists(_L):fp.write('[metadata]\nlicense-file = LICENSE\n')
 			else:print('\n\n>>>>>> LICENSE file not found <<<<<\n\n')
-			if self._pkg_data.get(_S):fp.write('[bdist_wheel]\nuniversal = 1\n')
+			if self._pkg_data.get(_Q):fp.write('[bdist_wheel]\nuniversal = 1\n')
 		try:setup(**kw)
 		except Exception:raise
 		finally:os.remove(file_name)
 		return _D
 def main():
 	A='tarfmt';dump_kw='--dump-kw'
 	if dump_kw in sys.argv:import wheel,distutils,setuptools;print('python:    ',sys.version);print('setuptools:',setuptools.__version__);print('distutils: ',distutils.__version__);print('wheel:     ',wheel.__version__)
 	nsp=NameSpacePackager(pkg_data);nsp.check();nsp.create_dirs();MySdist.nsp=nsp
 	if pkg_data.get(A):MySdist.tarfmt=pkg_data.get(A)
 	cmdclass=dict(install_lib=MyInstallLib,sdist=MySdist)
-	if _bdist_wheel_available:MyBdistWheel.nsp=nsp;cmdclass[_V]=MyBdistWheel
+	if _bdist_wheel_available:MyBdistWheel.nsp=nsp;cmdclass[_T]=MyBdistWheel
 	kw=dict(name=nsp.full_package_name,namespace_packages=nsp.namespace_packages,version=version_str,packages=nsp.packages,python_requires=nsp.python_requires,url=nsp.url,author=nsp.author,author_email=nsp.author_email,cmdclass=cmdclass,package_dir=nsp.package_dir,entry_points=nsp.entry_points(),description=nsp.description,install_requires=nsp.install_requires,extras_require=nsp.extras_require,license=nsp.license,classifiers=nsp.classifiers,keywords=nsp.keywords,package_data=nsp.package_data,ext_modules=nsp.ext_modules,test_suite=nsp.test_suite)
-	if _U not in sys.argv and('--verbose'in sys.argv or dump_kw in sys.argv):
+	if _S not in sys.argv and('--verbose'in sys.argv or dump_kw in sys.argv):
 		for k in sorted(kw):v=kw[k];print('  "{0}": "{1}",'.format(k,v))
 	if dump_kw in sys.argv:sys.argv.remove(dump_kw)
 	try:
 		with open('README.rst')as fp:kw['long_description']=fp.read();kw['long_description_content_type']='text/x-rst'
 	except Exception:pass
 	if nsp.wheel(kw,setup):return
 	for x in ['-c','egg_info','--egg-base','pip-egg-info']:
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/tokens.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 _A=None
 if _D:from typing import Text,Any,Dict,Optional,List;from .error import StreamMark
 SHOWLINES=True
 class Token:
 	__slots__='start_mark','end_mark',_B
 	def __init__(A,start_mark,end_mark):A.start_mark=start_mark;A.end_mark=end_mark
 	def __repr__(A):
-		C=[B for B in A.__slots__ if not B.endswith('_mark')];C.sort();B=', '.join(['%s=%r'%(B,getattr(A,B))for B in C])
+		C=[A for A in A.__slots__ if not A.endswith('_mark')];C.sort();B=', '.join(['%s=%r'%(B,getattr(A,B))for B in C])
 		if SHOWLINES:
 			try:B+=_F+str(A.start_mark.line)
 			except:pass
 		try:B+=', comment: '+str(A._comment)
 		except:pass
 		return '{}({})'.format(A.__class__.__name__,B)
 	def add_post_comment(A,comment):
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/ruamel/yaml/util.py` & `dynaconf-3.2.0/dynaconf/vendor/ruamel/yaml/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,68 @@
 from __future__ import absolute_import,print_function
-_B='lazy_self'
-_A=' '
+_A='lazy_self'
 from functools import partial
 import re
 from .compat import text_type,binary_type
 if False:from typing import Any,Dict,Optional,List,Text;from .compat import StreamTextType
 class LazyEval:
 	def __init__(A,func,*C,**D):
-		def B():B=func(*C,**D);object.__setattr__(A,_B,lambda:B);return B
-		object.__setattr__(A,_B,B)
+		def B():B=func(*(C),**D);object.__setattr__(A,_A,lambda:B);return B
+		object.__setattr__(A,_A,B)
 	def __getattribute__(B,name):
-		A=object.__getattribute__(B,_B)
-		if name==_B:return A
+		A=object.__getattribute__(B,_A)
+		if name==_A:return A
 		return getattr(A(),name)
 	def __setattr__(A,name,value):setattr(A.lazy_self(),name,value)
 RegExp=partial(LazyEval,re.compile)
 def load_yaml_guess_indent(stream,**N):
 	D=stream;B=None;from .main import round_trip_load as O
 	def K(l):
 		A=0
-		while A<len(l)and l[A]==_A:A+=1
+		while A<len(l)and l[A]==' ':A+=1
 		return A
 	if isinstance(D,text_type):F=D
 	elif isinstance(D,binary_type):F=D.decode('utf-8')
 	else:F=D.read()
 	G=B;H=B;L=B;E=B;I=0
 	for C in F.splitlines():
 		J=C.rstrip();P=J.lstrip()
 		if P.startswith('- '):
 			M=K(C);L=M-I;A=M+1
-			while C[A]==_A:A+=1
+			while C[A]==' ':A+=1
 			if C[A]=='#':continue
 			H=A-I;break
 		if G is B and E is not B and J:
 			A=0
 			while C[A]in' -':A+=1
 			if A>E:G=A-E
 		if J.endswith(':'):
 			I=K(C);A=0
-			while C[A]==_A:A+=1
+			while C[A]==' ':A+=1
 			E=A;continue
 		E=B
 	if H is B and G is not B:H=G
 	return O(F,**N),H,L
 def configobj_walker(cfg):
 	B=cfg;from configobj import ConfigObj as D;assert isinstance(B,D)
 	for A in B.initial_comment:
 		if A.strip():yield A
 	for C in _walk_section(B):
 		if C.strip():yield C
 	for A in B.final_comment:
 		if A.strip():yield A
 def _walk_section(s,level=0):
-	L='  ';I="'";H='\n';F=level;from configobj import Section as J;assert isinstance(s,J);D=L*F
+	H=level;G="'";F='\n';from configobj import Section as J;assert isinstance(s,J);D='  '*H
 	for A in s.scalars:
 		for B in s.comments[A]:yield D+B.strip()
 		C=s[A]
-		if H in C:G=D+L;C='|\n'+G+C.strip().replace(H,H+G)
-		elif':'in C:C=I+C.replace(I,"''")+I
+		if F in C:I=D+'  ';C='|\n'+I+C.strip().replace(F,F+I)
+		elif':'in C:C=G+C.replace(G,"''")+G
 		E='{0}{1}: {2}'.format(D,A,C);B=s.inline_comments[A]
-		if B:E+=_A+B
+		if B:E+=' '+B
 		yield E
 	for A in s.sections:
 		for B in s.comments[A]:yield D+B.strip()
 		E='{0}{1}:'.format(D,A);B=s.inline_comments[A]
-		if B:E+=_A+B
+		if B:E+=' '+B
 		yield E
-		for K in _walk_section(s[A],level=F+1):yield K
+		for K in _walk_section(s[A],level=H+1):yield K
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/toml/__init__.py` & `dynaconf-3.2.0/dynaconf/vendor/toml/__init__.py`

 * *Files identical despite different names*

### Comparing `dynaconf-3.1.9/dynaconf/vendor/toml/decoder.py` & `dynaconf-3.2.0/dynaconf/vendor/toml/decoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,10 @@
-_W='Reserved escape sequence used'
-_V='\\U'
-_U='false'
-_T='true'
-_S='\t'
-_R='}'
-_Q='+'
-_P='_'
-_O='-'
+_Q='Reserved escape sequence used'
+_P='false'
+_O='true'
 _N=','
 _M=']'
 _L=' '
 _K='{'
 _J='='
 _I='['
 _H='\\'
@@ -52,20 +46,20 @@
 	def dump(A,dump_value_func):
 		B=dump_value_func(A.val)
 		if isinstance(A.val,A._dict):return A.comment+_G+unicode(B)
 		else:return unicode(B)+A.comment
 def _strictly_valid_num(n):
 	n=n.strip()
 	if not n:return _A
-	if n[0]==_P:return _A
-	if n[-1]==_P:return _A
+	if n[0]=='_':return _A
+	if n[-1]=='_':return _A
 	if'_.'in n or'._'in n:return _A
 	if len(n)==1:return _B
 	if n[0]=='0'and n[1]not in[_F,'o','b','x']:return _A
-	if n[0]==_Q or n[0]==_O:
+	if n[0]=='+'or n[0]=='-':
 		n=n[1:]
 		if len(n)>1 and n[0]=='0'and n[1]!=_F:return _A
 	if'__'in n:return _A
 	return _B
 def load(f,_dict=dict,decoder=_E):
 	B=_dict;A=decoder
 	if _ispath(f):
@@ -80,15 +74,15 @@
 			else:warn('Non-existent filename in list with at least one valid filename')
 		return E
 	else:
 		try:return loads(f.read(),B,A)
 		except AttributeError:raise TypeError('You can only load a file descriptor, filename or list')
 _groupname_re=re.compile('^[A-Za-z0-9_-]+$')
 def loads(s,_dict=dict,decoder=_E):
-	q="Invalid group name '";K=decoder;d=[]
+	o="Invalid group name '";K=decoder;d=[]
 	if K is _E:K=TomlDecoder(_dict)
 	e=K.get_empty_table();G=e
 	if not isinstance(s,basestring):raise TypeError('Expecting something like a string')
 	if not isinstance(s,unicode):s=s.decode('utf8')
 	I=s;B=list(s);b=0;J=_A;Q='';D=_A;L=_A;V=_B;U=_A;W=_A;O=0;c='';j='';k=1
 	for (A,E) in enumerate(B):
 		if E=='\r'and B[A+1]==_G:B[A]=_L;continue
@@ -100,15 +94,15 @@
 					S=_A;F=1
 					while A>=F and B[A-F]==_H:S=not S;F+=1
 					if not S:O=2;J=_A;Q=''
 				continue
 			elif O==1:
 				if E.isspace():O=2;continue
 				elif E==_F:W=_B;continue
-				elif E.isalnum()or E==_P or E==_O:continue
+				elif E.isalnum()or E=='_'or E=='-':continue
 				elif W and B[A-1]==_F and(E==_C or E==_D):J=_B;Q=E;continue
 			elif O==2:
 				if E.isspace():
 					if W:
 						X=B[A+1]
 						if not X.isspace()and X!=_F:O=1
 					continue
@@ -164,15 +158,15 @@
 				if not D:raise TomlDecodeError('Unbalanced quotes',I,A)
 				if(B[A-1]==_D or B[A-1]==_C)and B[A-2]==B[A-1]:
 					B[A]=B[A-1]
 					if B[A-3]==B[A-1]:B[A-3]=_L
 			elif b:B[A]=_L
 			else:V=_B
 			k+=1
-		elif V and B[A]!=_L and B[A]!=_S:
+		elif V and B[A]!=_L and B[A]!='\t':
 			V=_A
 			if not U and not L:
 				if B[A]==_J:raise TomlDecodeError('Found empty keyname. ',I,A)
 				O=1;c+=E
 	if O:raise TomlDecodeError('Key name found without value. Reached end of file.',I,len(s))
 	if J:raise TomlDecodeError('Unterminated string found. Reached end of file.',I,len(s))
 	s=''.join(B);s=s.split(_G);T=_E;D='';P=_A;N=0
@@ -184,45 +178,45 @@
 		if T:
 			if P:D+=C
 			else:D+=C
 			P=_A;h=_A
 			if D[0]==_I:h=C[-1]==_M
 			elif len(C)>2:h=C[-1]==D[0]and C[-2]==D[0]and C[-3]==D[0]
 			if h:
-				try:o,r=K.load_value(D)
+				try:p,r=K.load_value(D)
 				except ValueError as Y:raise TomlDecodeError(str(Y),I,N)
-				G[T]=o;T=_E;D=''
+				G[T]=p;T=_E;D=''
 			else:
 				F=len(D)-1
 				while F>-1 and D[F]==_H:P=not P;F-=1
 				if P:D=D[:-1]
 				else:D+=_G
 			continue
 		if C[0]==_I:
 			L=_A
 			if len(C)==1:raise TomlDecodeError('Opening key group bracket on line by itself.',I,N)
 			if C[1]==_I:L=_B;C=C[2:];Z=']]'
 			else:C=C[1:];Z=_M
-			A=1;p=K._get_split_on_quotes(C);i=_A
-			for m in p:
+			A=1;q=K._get_split_on_quotes(C);i=_A
+			for m in q:
 				if not i and Z in m:break
 				A+=m.count(Z);i=not i
 			C=C.split(Z,A)
 			if len(C)<A+1 or C[-1].strip()!='':raise TomlDecodeError('Key group not on a line by itself.',I,N)
 			H=Z.join(C[:-1]).split(_F);A=0
 			while A<len(H):
 				H[A]=H[A].strip()
 				if len(H[A])>0 and(H[A][0]==_C or H[A][0]==_D):
 					a=H[A];R=A+1
 					while not a[0]==a[-1]:
 						R+=1
-						if R>len(H)+2:raise TomlDecodeError(q+a+"' Something "+'went wrong.',I,N)
+						if R>len(H)+2:raise TomlDecodeError(o+a+"' Something "+'went wrong.',I,N)
 						a=_F.join(H[A:R]).strip()
 					H[A]=a[1:-1];H[A+1:R]=[]
-				elif not _groupname_re.match(H[A]):raise TomlDecodeError(q+H[A]+"'. Try quoting it.",I,N)
+				elif not _groupname_re.match(H[A]):raise TomlDecodeError(o+H[A]+"'. Try quoting it.",I,N)
 				A+=1
 			G=e
 			for A in _range(len(H)):
 				M=H[A]
 				if M=='':raise TomlDecodeError("Can't have a keygroup with an empty name",I,N)
 				try:
 					G[M]
@@ -242,70 +236,70 @@
 					G[M]=K.get_empty_table()
 					if A==len(H)-1 and L:G[M]=[K.get_empty_table()]
 				G=G[M]
 				if L:
 					try:G=G[-1]
 					except KeyError:pass
 		elif C[0]==_K:
-			if C[-1]!=_R:raise TomlDecodeError('Line breaks are not allowed in inlineobjects',I,N)
+			if C[-1]!='}':raise TomlDecodeError('Line breaks are not allowed in inlineobjects',I,N)
 			try:K.load_inline_object(C,G,T,P)
 			except ValueError as Y:raise TomlDecodeError(str(Y),I,N)
 		elif _J in C:
 			try:n=K.load_line(C,G,T,P)
 			except ValueError as Y:raise TomlDecodeError(str(Y),I,N)
 			if n is not _E:T,D,P=n
 	return e
 def _load_date(val):
-	I='Z';A=val;G=0;F=_E
+	A=val;G=0;F=_E
 	try:
 		if len(A)>19:
 			if A[19]==_F:
-				if A[-1].upper()==I:C=A[20:-1];D=I
+				if A[-1].upper()=='Z':C=A[20:-1];D='Z'
 				else:
 					B=A[20:]
-					if _Q in B:E=B.index(_Q);C=B[:E];D=B[E:]
-					elif _O in B:E=B.index(_O);C=B[:E];D=B[E:]
+					if'+'in B:E=B.index('+');C=B[:E];D=B[E:]
+					elif'-'in B:E=B.index('-');C=B[:E];D=B[E:]
 					else:D=_E;C=B
 				if D is not _E:F=TomlTz(D)
 				G=int(int(C)*10**(6-len(C)))
 			else:F=TomlTz(A[19:])
 	except ValueError:F=_E
-	if _O not in A[1:]:return _E
+	if'-'not in A[1:]:return _E
 	try:
 		if len(A)==10:H=datetime.date(int(A[:4]),int(A[5:7]),int(A[8:10]))
 		else:H=datetime.datetime(int(A[:4]),int(A[5:7]),int(A[8:10]),int(A[11:13]),int(A[14:16]),int(A[17:19]),G,F)
 	except ValueError:return _E
 	return H
 def _load_unicode_escapes(v,hexbytes,prefix):
 	G='Invalid escape sequence: ';E=prefix;C=_A;A=len(v)-1
 	while A>-1 and v[A]==_H:C=not C;A-=1
 	for D in hexbytes:
 		if C:
 			C=_A;A=len(D)-1
 			while A>-1 and D[A]==_H:C=not C;A-=1
 			v+=E;v+=D;continue
 		B='';A=0;F=4
-		if E==_V:F=8
+		if E=='\\U':F=8
 		B=''.join(D[A:A+F]).lower()
 		if B.strip('0123456789abcdef'):raise ValueError(G+B)
 		if B[0]=='d'and B[1].strip('01234567'):raise ValueError(G+B+'. Only scalar unicode points are allowed.')
 		v+=unichr(int(B,16));v+=unicode(D[len(B):])
 	return v
 _escapes=['0','b','f','n','r','t',_C]
-_escapedchars=['\x00','\x08','\x0c',_G,'\r',_S,_C]
+_escapedchars=['\x00','\x08','\x0c',_G,'\r','\t',_C]
 _escape_to_escapedchars=dict(zip(_escapes,_escapedchars))
 def _unescape(v):
 	A=0;B=_A
 	while A<len(v):
 		if B:
 			B=_A
 			if v[A]in _escapes:v=v[:A-1]+_escape_to_escapedchars[v[A]]+v[A+1:]
 			elif v[A]==_H:v=v[:A-1]+v[A:]
 			elif v[A]=='u'or v[A]=='U':A+=1
-			else:raise ValueError(_W)
+			else:raise ValueError(_Q)
 			continue
 		elif v[A]==_H:B=_B
 		A+=1
 	return v
 class InlineTableDict:0
 class TomlDecoder:
 	def __init__(A,_dict=dict):A._dict=_dict
@@ -317,15 +311,15 @@
 		B=line[1:-1].split(_N);D=[]
 		if len(B)==1 and not B[0].strip():B.pop()
 		while len(B)>0:
 			C=B.pop(0)
 			try:H,A=C.split(_J,1)
 			except ValueError:raise ValueError('Invalid inline table encountered')
 			A=A.strip()
-			if A[0]==A[-1]and A[0]in(_C,_D)or(A[0]in'-0123456789'or A in(_T,_U)or A[0]==_I and A[-1]==_M or A[0]==_K and A[-1]==_R):D.append(C)
+			if A[0]==A[-1]and A[0]in(_C,_D)or(A[0]in'-0123456789'or A in(_O,_P)or A[0]==_I and A[-1]==_M or A[0]==_K and A[-1]=='}'):D.append(C)
 			elif len(B)>0:B[0]=C+_N+B[0]
 			else:raise ValueError('Invalid inline table value encountered')
 		for F in D:
 			G=E.load_line(F,currentlevel,multikey,multibackslash)
 			if G is not _E:break
 	def _get_split_on_quotes(F,line):
 		A=line.split(_C);D=_A;C=[]
@@ -336,27 +330,27 @@
 				if _D in B[-1]:B=B[:-1]+B[-1].split(_D)
 			C+=B
 		for E in A:
 			if D:C.append(E)
 			else:C+=E.split(_D);D=not D
 		return C
 	def load_line(E,line,currentlevel,multikey,multibackslash):
-		S='Duplicate keys!';L=multikey;K=line;G=multibackslash;D=currentlevel;H=1;M=E._get_split_on_quotes(K);C=_A
+		P='Duplicate keys!';L=multikey;K=line;G=multibackslash;D=currentlevel;H=1;M=E._get_split_on_quotes(K);C=_A
 		for F in M:
 			if not C and _J in F:break
 			H+=F.count(_J);C=not C
 		A=K.split(_J,H);N=_strictly_valid_num(A[-1])
-		if _number_with_underscores.match(A[-1]):A[-1]=A[-1].replace(_P,'')
-		while len(A[-1])and(A[-1][0]!=_L and A[-1][0]!=_S and A[-1][0]!=_D and A[-1][0]!=_C and A[-1][0]!=_I and A[-1][0]!=_K and A[-1].strip()!=_T and A[-1].strip()!=_U):
+		if _number_with_underscores.match(A[-1]):A[-1]=A[-1].replace('_','')
+		while len(A[-1])and(A[-1][0]!=_L and A[-1][0]!='\t'and A[-1][0]!=_D and A[-1][0]!=_C and A[-1][0]!=_I and A[-1][0]!=_K and A[-1].strip()!=_O and A[-1].strip()!=_P):
 			try:float(A[-1]);break
 			except ValueError:pass
 			if _load_date(A[-1])is not _E:break
 			if TIME_RE.match(A[-1]):break
-			H+=1;P=A[-1];A=K.split(_J,H)
-			if P==A[-1]:raise ValueError('Invalid date or number')
+			H+=1;Q=A[-1];A=K.split(_J,H)
+			if Q==A[-1]:raise ValueError('Invalid date or number')
 			if N:N=_strictly_valid_num(A[-1])
 		A=[_J.join(A[:-1]).strip(),A[-1].strip()]
 		if _F in A[0]:
 			if _C in A[0]or _D in A[0]:
 				M=E._get_split_on_quotes(A[0]);C=_A;B=[]
 				for F in M:
 					if C:B.append(F)
@@ -366,42 +360,42 @@
 			while B[-1]=='':B=B[:-1]
 			for I in B[:-1]:
 				if I=='':continue
 				if I not in D:D[I]=E.get_empty_table()
 				D=D[I]
 			A[0]=B[-1].strip()
 		elif(A[0][0]==_C or A[0][0]==_D)and A[0][-1]==A[0][0]:A[0]=_unescape(A[0][1:-1])
-		J,Q=E._load_line_multiline_str(A[1])
+		J,R=E._load_line_multiline_str(A[1])
 		if J>-1:
-			while J>-1 and A[1][J+Q]==_H:G=not G;J-=1
+			while J>-1 and A[1][J+R]==_H:G=not G;J-=1
 			if G:O=A[1][:-1]
 			else:O=A[1]+_G
 			L=A[0]
-		else:R,T=E.load_value(A[1],N)
-		try:D[A[0]];raise ValueError(S)
-		except TypeError:raise ValueError(S)
+		else:S,T=E.load_value(A[1],N)
+		try:D[A[0]];raise ValueError(P)
+		except TypeError:raise ValueError(P)
 		except KeyError:
 			if L:return L,O,G
-			else:D[A[0]]=R
+			else:D[A[0]]=S
 	def _load_line_multiline_str(C,p):
 		B=0
 		if len(p)<3:return-1,B
 		if p[0]==_I and(p.strip()[-1]!=_M and C._load_array_isstrarray(p)):
 			A=p[1:].strip().split(_N)
 			while len(A)>1 and A[-1][0]!=_C and A[-1][0]!=_D:A=A[:-2]+[A[-2]+_N+A[-1]]
 			A=A[-1];B=len(p)-len(A);p=A
 		if p[0]!=_C and p[0]!=_D:return-1,B
 		if p[1]!=p[0]or p[2]!=p[0]:return-1,B
 		if len(p)>5 and p[-1]==p[0]and p[-2]==p[0]and p[-3]==p[0]:return-1,B
 		return len(p)-1,B
 	def load_value(E,v,strictly_valid=_B):
-		a='float';Z='int';Y='bool'
+		V='float';U='int';T='bool'
 		if not v:raise ValueError('Empty value is invalid')
-		if v==_T:return _B,Y
-		elif v==_U:return _A,Y
+		if v==_O:return _B,T
+		elif v==_P:return _A,T
 		elif v[0]==_C or v[0]==_D:
 			F=v[0];B=v[1:].split(F);G=_A;H=0
 			if len(B)>1 and B[0]==''and B[1]=='':B=B[2:];G=_B
 			I=_A
 			for J in B:
 				if J=='':
 					if G:H+=1
@@ -413,42 +407,42 @@
 						while N==_H:K=not K;A-=1;N=J[A]
 					except IndexError:pass
 					if not K:
 						if I:raise ValueError('Found tokens after a closed '+'string. Invalid TOML.')
 						elif not G or H>1:I=_B
 						else:H=0
 			if F==_C:
-				T=v.split(_H)[1:];C=_A
-				for A in T:
+				W=v.split(_H)[1:];C=_A
+				for A in W:
 					if A=='':C=not C
 					else:
-						if A[0]not in _escapes and(A[0]!='u'and A[0]!='U'and not C):raise ValueError(_W)
+						if A[0]not in _escapes and(A[0]!='u'and A[0]!='U'and not C):raise ValueError(_Q)
 						if C:C=_A
-				for L in ['\\u',_V]:
+				for L in ['\\u','\\U']:
 					if L in v:O=v.split(L);v=_load_unicode_escapes(O[0],O[1:],L)
 				v=_unescape(v)
 			if len(v)>1 and v[1]==F and(len(v)<3 or v[1]==v[2]):v=v[2:-2]
 			return v[1:-1],'str'
 		elif v[0]==_I:return E.load_array(v),'array'
 		elif v[0]==_K:P=E.get_empty_inline_table();E.load_inline_object(v,P);return P,'inline_object'
-		elif TIME_RE.match(v):U,V,W,b,Q=TIME_RE.match(v).groups();X=datetime.time(int(U),int(V),int(W),int(Q)if Q else 0);return X,'time'
+		elif TIME_RE.match(v):X,Y,Z,b,Q=TIME_RE.match(v).groups();a=datetime.time(int(X),int(Y),int(Z),int(Q)if Q else 0);return a,'time'
 		else:
 			R=_load_date(v)
 			if R is not _E:return R,'date'
 			if not strictly_valid:raise ValueError('Weirdness with leading zeroes or underscores in your number.')
-			D=Z;S=_A
-			if v[0]==_O:S=_B;v=v[1:]
-			elif v[0]==_Q:v=v[1:]
-			v=v.replace(_P,'');M=v.lower()
+			D=U;S=_A
+			if v[0]=='-':S=_B;v=v[1:]
+			elif v[0]=='+':v=v[1:]
+			v=v.replace('_','');M=v.lower()
 			if _F in v or'x'not in v and('e'in v or'E'in v):
 				if _F in v and v.split(_F,1)[1]=='':raise ValueError('This float is missing digits after the point')
 				if v[0]not in'0123456789':raise ValueError("This float doesn't have a leading digit")
-				v=float(v);D=a
-			elif len(M)==3 and(M=='inf'or M=='nan'):v=float(v);D=a
-			if D==Z:v=int(v,0)
+				v=float(v);D=V
+			elif len(M)==3 and(M=='inf'or M=='nan'):v=float(v);D=V
+			if D==U:v=int(v,0)
 			if S:return 0-v,D
 			return v,D
 	def bounded_string(C,s):
 		if len(s)==0:return _B
 		if s[-1]!=s[0]:return _A
 		A=-2;B=_A
 		while len(s)+A>0:
@@ -469,16 +463,16 @@
 				while A<len(a[1:]):
 					if a[A]==_C or a[A]==_D:
 						if F:
 							K=A-1
 							while K>-1 and a[K]==_H:F=not F;K-=1
 						F=not F
 					if not F and a[A]==_K:J+=1
-					if F or a[A]!=_R:A+=1;continue
-					elif a[A]==_R and J>1:J-=1;A+=1;continue
+					if F or a[A]!='}':A+=1;continue
+					elif a[A]=='}'and J>1:J-=1;A+=1;continue
 					A+=1;O.append(a[E:A]);E=A+1
 					while E<len(a[1:])and a[E]!=_K:E+=1
 					A=E+1
 				a=O
 			B=0
 			if Q:
 				while B<len(a)-1:
```

### Comparing `dynaconf-3.1.9/dynaconf/vendor/toml/encoder.py` & `dynaconf-3.2.0/dynaconf/vendor/toml/encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-_G=']\n'
-_F=' = '
-_E='\n'
-_D=False
-_C='['
-_B='.'
+_C=' = '
+_B=False
 _A=None
 import datetime,re,sys
 from decimal import Decimal
 from .decoder import InlineTableDict
 if sys.version_info>=(3,):unicode=str
 def dump(o,f,encoder=_A):
 	if not f.write:raise TypeError('You can only dump an object to a file descriptor')
@@ -20,115 +16,115 @@
 		H=[id(A)for A in D]
 		for K in G:
 			if K in H:raise ValueError('Circular reference detected')
 		G+=H;I=C.get_empty_table()
 		for E in D:
 			B,F=C.dump_sections(D[E],E)
 			if B or not B and not F:
-				if A and A[-2:]!='\n\n':A+=_E
-				A+=_C+E+_G
+				if A and A[-2:]!='\n\n':A+='\n'
+				A+='['+E+']\n'
 				if B:A+=B
-			for J in F:I[E+_B+J]=F[J]
+			for J in F:I[E+'.'+J]=F[J]
 		D=I
 	return A
 def _dump_str(v):
-	G="'";F='\\';C='"'
+	D='\\';B='"'
 	if sys.version_info<(3,)and hasattr(v,'decode')and isinstance(v,str):v=v.decode('utf-8')
 	v='%r'%v
 	if v[0]=='u':v=v[1:]
-	D=v.startswith(G)
-	if D or v.startswith(C):v=v[1:-1]
-	if D:v=v.replace("\\'",G);v=v.replace(C,'\\"')
+	E=v.startswith("'")
+	if E or v.startswith(B):v=v[1:-1]
+	if E:v=v.replace("\\'","'");v=v.replace(B,'\\"')
 	v=v.split('\\x')
 	while len(v)>1:
 		A=-1
 		if not v[0]:v=v[1:]
-		v[0]=v[0].replace('\\\\',F);B=v[0][A]!=F
-		while v[0][:A]and v[0][A]==F:B=not B;A-=1
-		if B:E='x'
-		else:E='u00'
-		v=[v[0]+E+v[1]]+v[2:]
-	return unicode(C+v[0]+C)
+		v[0]=v[0].replace('\\\\',D);C=v[0][A]!=D
+		while v[0][:A]and v[0][A]==D:C=not C;A-=1
+		if C:F='x'
+		else:F='u00'
+		v=[v[0]+F+v[1]]+v[2:]
+	return unicode(B+v[0]+B)
 def _dump_float(v):return '{}'.format(v).replace('e+0','e+').replace('e-0','e-')
 def _dump_time(v):
 	A=v.utcoffset()
 	if A is _A:return v.isoformat()
 	return v.isoformat()[:-6]
 class TomlEncoder:
-	def __init__(A,_dict=dict,preserve=_D):A._dict=_dict;A.preserve=preserve;A.dump_funcs={str:_dump_str,unicode:_dump_str,list:A.dump_list,bool:lambda v:unicode(v).lower(),int:lambda v:v,float:_dump_float,Decimal:_dump_float,datetime.datetime:lambda v:v.isoformat().replace('+00:00','Z'),datetime.time:_dump_time,datetime.date:lambda v:v.isoformat()}
+	def __init__(A,_dict=dict,preserve=_B):A._dict=_dict;A.preserve=preserve;A.dump_funcs={str:_dump_str,unicode:_dump_str,list:A.dump_list,bool:lambda v:unicode(v).lower(),int:lambda v:v,float:_dump_float,Decimal:_dump_float,datetime.datetime:lambda v:v.isoformat().replace('+00:00','Z'),datetime.time:_dump_time,datetime.date:lambda v:v.isoformat()}
 	def get_empty_table(A):return A._dict()
 	def dump_list(B,v):
-		A=_C
+		A='['
 		for C in v:A+=' '+unicode(B.dump_value(C))+','
 		A+=']';return A
 	def dump_inline_table(B,section):
 		A=section;C=''
 		if isinstance(A,dict):
 			D=[]
-			for (E,F) in A.items():G=B.dump_inline_table(F);D.append(E+_F+G)
+			for (E,F) in A.items():G=B.dump_inline_table(F);D.append(E+_C+G)
 			C+='{ '+', '.join(D)+' }\n';return C
 		else:return unicode(B.dump_value(A))
 	def dump_value(B,v):
 		A=B.dump_funcs.get(type(v))
 		if A is _A and hasattr(v,'__iter__'):A=B.dump_funcs[list]
 		return A(v)if A is not _A else B.dump_funcs[str](v)
 	def dump_sections(C,o,sup):
 		D=sup;F=''
-		if D!=''and D[-1]!=_B:D+=_B
+		if D!=''and D[-1]!='.':D+='.'
 		M=C._dict();G=''
 		for A in o:
 			A=unicode(A);B=A
 			if not re.match('^[A-Za-z0-9_-]+$',A):B=_dump_str(A)
 			if not isinstance(o[A],dict):
-				N=_D
+				N=_B
 				if isinstance(o[A],list):
 					for L in o[A]:
 						if isinstance(L,dict):N=True
 				if N:
 					for L in o[A]:
-						H=_E;G+='[['+D+B+']]\n';I,J=C.dump_sections(L,D+B)
+						H='\n';G+='[['+D+B+']]\n';I,J=C.dump_sections(L,D+B)
 						if I:
-							if I[0]==_C:H+=I
+							if I[0]=='[':H+=I
 							else:G+=I
 						while J:
 							O=C._dict()
 							for K in J:
-								E,P=C.dump_sections(J[K],D+B+_B+K)
-								if E:H+=_C+D+B+_B+K+_G;H+=E
-								for E in P:O[K+_B+E]=P[E]
+								E,P=C.dump_sections(J[K],D+B+'.'+K)
+								if E:H+='['+D+B+'.'+K+']\n';H+=E
+								for E in P:O[K+'.'+E]=P[E]
 							J=O
 						G+=H
-				elif o[A]is not _A:F+=B+_F+unicode(C.dump_value(o[A]))+_E
-			elif C.preserve and isinstance(o[A],InlineTableDict):F+=B+_F+C.dump_inline_table(o[A])
+				elif o[A]is not _A:F+=B+_C+unicode(C.dump_value(o[A]))+'\n'
+			elif C.preserve and isinstance(o[A],InlineTableDict):F+=B+_C+C.dump_inline_table(o[A])
 			else:M[B]=o[A]
 		F+=G;return F,M
 class TomlPreserveInlineDictEncoder(TomlEncoder):
 	def __init__(A,_dict=dict):super(TomlPreserveInlineDictEncoder,A).__init__(_dict,True)
 class TomlArraySeparatorEncoder(TomlEncoder):
-	def __init__(B,_dict=dict,preserve=_D,separator=','):
+	def __init__(B,_dict=dict,preserve=_B,separator=','):
 		A=separator;super(TomlArraySeparatorEncoder,B).__init__(_dict,preserve)
 		if A.strip()=='':A=','+A
 		elif A.strip(' \t\n\r,'):raise ValueError('Invalid separator for arrays')
 		B.separator=A
 	def dump_list(D,v):
-		B=[];C=_C
+		B=[];C='['
 		for A in v:B.append(D.dump_value(A))
 		while B!=[]:
 			E=[]
 			for A in B:
 				if isinstance(A,list):
 					for F in A:E.append(F)
 				else:C+=' '+unicode(A)+D.separator
 			B=E
 		C+=']';return C
 class TomlNumpyEncoder(TomlEncoder):
-	def __init__(A,_dict=dict,preserve=_D):import numpy as B;super(TomlNumpyEncoder,A).__init__(_dict,preserve);A.dump_funcs[B.float16]=_dump_float;A.dump_funcs[B.float32]=_dump_float;A.dump_funcs[B.float64]=_dump_float;A.dump_funcs[B.int16]=A._dump_int;A.dump_funcs[B.int32]=A._dump_int;A.dump_funcs[B.int64]=A._dump_int
+	def __init__(A,_dict=dict,preserve=_B):import numpy as B;super(TomlNumpyEncoder,A).__init__(_dict,preserve);A.dump_funcs[B.float16]=_dump_float;A.dump_funcs[B.float32]=_dump_float;A.dump_funcs[B.float64]=_dump_float;A.dump_funcs[B.int16]=A._dump_int;A.dump_funcs[B.int32]=A._dump_int;A.dump_funcs[B.int64]=A._dump_int
 	def _dump_int(A,v):return '{}'.format(int(v))
 class TomlPreserveCommentEncoder(TomlEncoder):
-	def __init__(A,_dict=dict,preserve=_D):from dynaconf.vendor.toml.decoder import CommentValue as B;super(TomlPreserveCommentEncoder,A).__init__(_dict,preserve);A.dump_funcs[B]=lambda v:v.dump(A.dump_value)
+	def __init__(A,_dict=dict,preserve=_B):from dynaconf.vendor.toml.decoder import CommentValue as B;super(TomlPreserveCommentEncoder,A).__init__(_dict,preserve);A.dump_funcs[B]=lambda v:v.dump(A.dump_value)
 class TomlPathlibEncoder(TomlEncoder):
 	def _dump_pathlib_path(A,v):return _dump_str(str(v))
 	def dump_value(A,v):
 		if(3,4)<=sys.version_info:
 			import pathlib as B
 			if isinstance(v,B.PurePath):v=str(v)
 		return super(TomlPathlibEncoder,A).dump_value(v)
```

### Comparing `dynaconf-3.1.9/dynaconf.egg-info/PKG-INFO` & `dynaconf-3.2.0/dynaconf.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dynaconf
-Version: 3.1.9
+Version: 3.2.0
 Summary: The dynamic configurator for your Python Project
-Home-page: https://github.com/rochacbruno/dynaconf
+Home-page: https://github.com/dynaconf/dynaconf
 Author: Bruno Rocha
 Author-email: rochacbruno@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Flask
@@ -16,59 +16,61 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: redis
 Provides-Extra: vault
 Provides-Extra: yaml
 Provides-Extra: toml
 Provides-Extra: ini
 Provides-Extra: configobj
 Provides-Extra: all
 Provides-Extra: test
 License-File: LICENSE
+License-File: vendor_licenses/box-LICENSE.txt
+License-File: vendor_licenses/click-LICENSE.rst
+License-File: vendor_licenses/licenses.sh
+License-File: vendor_licenses/python-dotenv-LICENSE.txt
+License-File: vendor_licenses/ruamel.yaml-LICENSE.txt
+License-File: vendor_licenses/toml-LICENSE.txt
+License-File: vendor_licenses/tomli-LICENSE.txt
+License-File: vendor_licenses/vendor_versions.txt
 
 <!-- [![Dynaconf](docs/img/logo_400.svg?sanitize=true)](http://dynaconf.com) -->
 
 <p align="center"><img src="/art/header.png?v2" alt="dynaconf. new logo"></p>
 
 > **dynaconf** - Configuration Management for Python.
 
-[![MIT License](https://img.shields.io/badge/license-MIT-007EC7.svg?style=flat-square)](/LICENSE) [![PyPI](https://img.shields.io/pypi/v/dynaconf.svg)](https://pypi.python.org/pypi/dynaconf) [![PyPI](https://img.shields.io/pypi/pyversions/dynaconf.svg)]() ![PyPI - Downloads](https://img.shields.io/pypi/dm/dynaconf.svg?label=pip%20installs&logo=python) [![CI](https://github.com/rochacbruno/dynaconf/actions/workflows/main.yml/badge.svg)](https://github.com/rochacbruno/dynaconf/actions/workflows/main.yml) [![codecov](https://codecov.io/gh/rochacbruno/dynaconf/branch/master/graph/badge.svg)](https://codecov.io/gh/rochacbruno/dynaconf) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/42d2f11ef0a446808b246c8c69603f6e)](https://www.codacy.com/gh/rochacbruno/dynaconf/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=rochacbruno/dynaconf&amp;utm_campaign=Badge_Grade) ![GitHub issues](https://img.shields.io/github/issues/rochacbruno/dynaconf.svg) ![GitHub stars](https://img.shields.io/github/stars/rochacbruno/dynaconf.svg) ![GitHub Release Date](https://img.shields.io/github/release-date/rochacbruno/dynaconf.svg) ![GitHub commits since latest release](https://img.shields.io/github/commits-since/rochacbruno/dynaconf/latest.svg) ![GitHub last commit](https://img.shields.io/github/last-commit/rochacbruno/dynaconf.svg) [![Code Style Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black/) [![Discussion](https://img.shields.io/badge/chat-discussions-blue.svg?logo=googlechat)](https://github.com/rochacbruno/dynaconf/discussions) [![Discussion](https://img.shields.io/badge/demo-learn-yellow.svg?logo=gnubash)](https://github.com/rochacbruno/learndynaconf)
+[![MIT License](https://img.shields.io/badge/license-MIT-007EC7.svg?style=flat-square)](/LICENSE) [![PyPI](https://img.shields.io/pypi/v/dynaconf.svg)](https://pypi.python.org/pypi/dynaconf) [![PyPI](https://img.shields.io/pypi/pyversions/dynaconf.svg)]() ![PyPI - Downloads](https://img.shields.io/pypi/dm/dynaconf.svg?label=pip%20installs&logo=python) [![CI](https://github.com/dynaconf/dynaconf/actions/workflows/main.yml/badge.svg)](https://github.com/dynaconf/dynaconf/actions/workflows/main.yml) [![codecov](https://codecov.io/gh/dynaconf/dynaconf/branch/master/graph/badge.svg)](https://codecov.io/gh/dynaconf/dynaconf) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/3fb2de98464442f99a7663181803b400)](https://www.codacy.com/gh/dynaconf/dynaconf/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=dynaconf/dynaconf&amp;utm_campaign=Badge_Grade)  ![GitHub stars](https://img.shields.io/github/stars/dynaconf/dynaconf.svg) ![GitHub Release Date](https://img.shields.io/github/release-date/dynaconf/dynaconf.svg) ![GitHub commits since latest release](https://img.shields.io/github/commits-since/dynaconf/dynaconf/latest.svg) ![GitHub last commit](https://img.shields.io/github/last-commit/dynaconf/dynaconf.svg) [![Code Style Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black/)
 
-
-
-[![Foo](https://xscode.com/assets/promo-banner.svg)](https://xscode.com/rochacbruno/dynaconf)
+![GitHub issues](https://img.shields.io/github/issues/dynaconf/dynaconf.svg) [![User Forum](https://img.shields.io/badge/users-forum-blue.svg?logo=googlechat)](https://github.com/dynaconf/dynaconf/discussions) [![Join the chat at https://gitter.im/dynaconf/dev](https://badges.gitter.im/dynaconf/dev.svg)](https://gitter.im/dynaconf/dev?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![ Matrix](https://img.shields.io/badge/dev-room-blue.svg?logo=matrix)](https://matrix.to/#/#dynaconf:matrix.org)
 
 ## Features
 
 - Inspired by the [12-factor application guide](https://12factor.net/config)
 - Settings management (default values, validation, parsing, templating)
 - Protection of sensitive information (passwords/tokens)
 - Multiple file formats `toml|yaml|json|ini|py` and also customizable loaders.
 - Full support for environment variables to override existing settings (dotenv support included).
 - Optional layered system for multi environments `[default, development, testing, production]`
 - Built-in support for Hashicorp Vault and Redis as settings and secrets storage.
 - Built-in extensions for **Django** and **Flask** web frameworks.
 - CLI for common operations such as `init, list, write, validate, export`.
 - full docs on https://dynaconf.com
 
-## Quick start
-
-> **DEMO:** You can see a working demo here: https://github.com/rochacbruno/learndynaconf
-
-
 ### Install
 
 ```bash
 $ pip install dynaconf
 ```
 
 #### Initialize Dynaconf on project root directory
@@ -96,15 +98,15 @@
 
 #### Dynaconf init creates the following files
 
 ```plain
 .
 ├── config.py       # This is from where you import your settings object (required)
 ├── .secrets.toml   # This is to hold sensitive data like passwords and tokens (optional)
-└── settings.toml   # This is to hold your application setttings (optional)
+└── settings.toml   # This is to hold your application settings (optional)
 ```
 
 On the file `config.py` Dynaconf init generates the following boilerpate
 
 ```py
 from dynaconf import Dynaconf
 
@@ -167,15 +169,14 @@
 - Template substitutions
 - etc...
 
 There is a lot more you can do, **read the docs:** http://dynaconf.com
 
 ## Contribute
 
-Main discussions happens on [Discussions Tab](https://github.com/rochacbruno/dynaconf/discussions) learn more about how to get involved on [CONTRIBUTING.md guide](CONTRIBUTING.md)
+Main discussions happens on [Discussions Tab](https://github.com/dynaconf/dynaconf/discussions) learn more about how to get involved on [CONTRIBUTING.md guide](CONTRIBUTING.md)
 
 ## More
 
 If you are looking for something similar to Dynaconf to use in your Rust projects: https://github.com/rubik/hydroconf
 
 And a special thanks to [Caneco](https://twitter.com/caneco) for the logo.
-
```

### Comparing `dynaconf-3.1.9/dynaconf.egg-info/SOURCES.txt` & `dynaconf-3.2.0/dynaconf.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 dynaconf/loaders/yaml_loader.py
 dynaconf/strategies/__init__.py
 dynaconf/strategies/filtering.py
 dynaconf/utils/__init__.py
 dynaconf/utils/boxing.py
 dynaconf/utils/files.py
 dynaconf/utils/functional.py
+dynaconf/utils/inspect.py
 dynaconf/utils/parse_conf.py
 dynaconf/vendor/__init__.py
 dynaconf/vendor/box/__init__.py
 dynaconf/vendor/box/box.py
 dynaconf/vendor/box/box_list.py
 dynaconf/vendor/box/config_box.py
 dynaconf/vendor/box/converters.py
@@ -106,8 +107,21 @@
 dynaconf/vendor/ruamel/yaml/timestamp.py
 dynaconf/vendor/ruamel/yaml/tokens.py
 dynaconf/vendor/ruamel/yaml/util.py
 dynaconf/vendor/toml/__init__.py
 dynaconf/vendor/toml/decoder.py
 dynaconf/vendor/toml/encoder.py
 dynaconf/vendor/toml/ordered.py
-dynaconf/vendor/toml/tz.py
+dynaconf/vendor/toml/tz.py
+dynaconf/vendor/tomllib/__init__.py
+dynaconf/vendor/tomllib/_parser.py
+dynaconf/vendor/tomllib/_re.py
+dynaconf/vendor/tomllib/_types.py
+dynaconf/vendor/tomllib/_writer.py
+vendor_licenses/box-LICENSE.txt
+vendor_licenses/click-LICENSE.rst
+vendor_licenses/licenses.sh
+vendor_licenses/python-dotenv-LICENSE.txt
+vendor_licenses/ruamel.yaml-LICENSE.txt
+vendor_licenses/toml-LICENSE.txt
+vendor_licenses/tomli-LICENSE.txt
+vendor_licenses/vendor_versions.txt
```

### Comparing `dynaconf-3.1.9/setup.py` & `dynaconf-3.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import io
+from __future__ import annotations
+
 import os
-import sys
 
 from setuptools import find_packages
 from setuptools import setup
 
 
 def read(*names, **kwargs):
     """Read a file."""
     content = ""
-    with io.open(
+    with open(
         os.path.join(os.path.dirname(__file__), *names),
         encoding=kwargs.get("encoding", "utf8"),
     ) as open_file:
         content = open_file.read().strip()
     return content
 
 
@@ -28,37 +28,37 @@
     "flake8-print",
     "flake8-todo",
     "radon",
     "flask>=0.12",
     "django",
     "python-dotenv",
     "toml",
-    "codecov",
     "redis",
     "hvac",
     "configobj",
 ]
 
 
 setup(
     name="dynaconf",
     version=read("dynaconf", "VERSION"),
-    url="https://github.com/rochacbruno/dynaconf",
+    url="https://github.com/dynaconf/dynaconf",
     license="MIT",
+    license_files=["LICENSE", "vendor_licenses/*"],
     author="Bruno Rocha",
     author_email="rochacbruno@gmail.com",
     description="The dynamic configurator for your Python Project",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     packages=find_packages(
         exclude=[
             "tests",
             "tests.*",
-            "example",
-            "example.*",
+            "tests_functional",
+            "tests_functional.*",
             "docs",
             "legacy_docs",
             "legacy_docs.*",
             "docs.*",
             "build",
             "build.*",
             "dynaconf.vendor_src",
@@ -77,15 +77,15 @@
         "yaml": ["ruamel.yaml"],
         "toml": ["toml"],
         "ini": ["configobj"],
         "configobj": ["configobj"],
         "all": ["redis", "ruamel.yaml", "configobj", "hvac"],
         "test": test_requirements,
     },
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     entry_points={"console_scripts": ["dynaconf=dynaconf.cli:main"]},
     setup_requires=["setuptools>=38.6.0"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Framework :: Django",
         "Framework :: Flask",
         "Intended Audience :: Developers",
@@ -94,12 +94,13 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Utilities",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

