# Comparing `tmp/freva-2303.0.0.tar.gz` & `tmp/freva-2307.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freva-2303.0.0.tar", last modified: Wed Mar  8 07:39:40 2023, max compression
+gzip compressed data, was "freva-2307.0.0.tar", last modified: Thu Jul 13 08:55:23 2023, max compression
```

## Comparing `freva-2303.0.0.tar` & `freva-2307.0.0.tar`

### file list

```diff
@@ -1,140 +1,134 @@
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.033548 freva-2303.0.0/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     1550 2023-03-08 07:38:15.000000 freva-2303.0.0/LICENSE.md
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      110 2023-03-08 07:38:15.000000 freva-2303.0.0/MANIFEST.in
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     6173 2023-03-08 07:39:40.033548 freva-2303.0.0/PKG-INFO
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     4811 2023-03-08 07:38:15.000000 freva-2303.0.0/README.md
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.026881 freva-2303.0.0/assets/
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.020214 freva-2303.0.0/assets/completions/
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.026881 freva-2303.0.0/assets/completions/bash/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     4758 2023-03-08 07:38:15.000000 freva-2303.0.0/assets/completions/bash/freva
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.026881 freva-2303.0.0/assets/completions/fish/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     4555 2023-03-08 07:38:15.000000 freva-2303.0.0/assets/completions/fish/freva.fish
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.026881 freva-2303.0.0/assets/completions/tcsh/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     4619 2023-03-08 07:38:15.000000 freva-2303.0.0/assets/completions/tcsh/tcsh-completion.bash
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.026881 freva-2303.0.0/assets/completions/zsh/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      726 2023-03-08 07:38:15.000000 freva-2303.0.0/assets/completions/zsh/_freva
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       59 2023-03-08 07:38:15.000000 freva-2303.0.0/assets/completions/zsh/_freva_crawl_my_data
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       48 2023-03-08 07:38:15.000000 freva-2303.0.0/assets/completions/zsh/_freva_databrowser
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       41 2023-03-08 07:38:15.000000 freva-2303.0.0/assets/completions/zsh/_freva_esgf
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       47 2023-03-08 07:38:15.000000 freva-2303.0.0/assets/completions/zsh/_freva_history
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       37 2023-03-08 07:38:15.000000 freva-2303.0.0/assets/completions/zsh/_freva_plugin
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     3225 2023-03-08 07:38:15.000000 freva-2303.0.0/assets/completions/zsh/completions.zsh
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      128 2023-03-08 07:38:15.000000 freva-2303.0.0/assets/completions/zsh/source.zsh
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     1056 2023-03-08 07:38:15.000000 freva-2303.0.0/assets/drs_config.toml
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2578 2023-03-08 07:38:15.000000 freva-2303.0.0/assets/evaluation_system.conf
--rwxr-xr-x   0 wilfred   (1000) wilfred   (1001)    15492 2023-03-08 07:38:15.000000 freva-2303.0.0/deploy.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       38 2023-03-08 07:39:40.033548 freva-2303.0.0/setup.cfg
--rwxr-xr-x   0 wilfred   (1000) wilfred   (1001)     7017 2023-03-08 07:38:15.000000 freva-2303.0.0/setup.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.023547 freva-2303.0.0/src/
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.026881 freva-2303.0.0/src/evaluation_system/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     1514 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/__init__.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.026881 freva-2303.0.0/src/evaluation_system/api/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)        1 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/api/__init__.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    35239 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/api/parameters.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    48016 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/api/plugin.py
--rwxr-xr-x   0 wilfred   (1000) wilfred   (1001)    45916 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/api/plugin_manager.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     8767 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/api/user_data.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.026881 freva-2303.0.0/src/evaluation_system/api/workload_manager/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     3509 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/api/workload_manager/__init__.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    12609 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/api/workload_manager/core.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     1995 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/api/workload_manager/local.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     5859 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/api/workload_manager/lsf.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      294 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/api/workload_manager/moab.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     3484 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/api/workload_manager/oar.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2965 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/api/workload_manager/pbs.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     1974 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/api/workload_manager/sge.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2867 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/api/workload_manager/slurm.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.026881 freva-2303.0.0/src/evaluation_system/external/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/external/__init__.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.026881 freva-2303.0.0/src/evaluation_system/external/basePlugin/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     3347 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/external/basePlugin/Logger.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2473 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/external/basePlugin/NCLhelper.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     6666 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/external/basePlugin/ShellScriptHelper.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    44879 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/external/basePlugin/__init__.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.026881 freva-2303.0.0/src/evaluation_system/fuse/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       69 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/fuse/__init__.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     9662 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/fuse/esgf2fs.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     3730 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/fuse/esgf2solr_crawl.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     4289 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/fuse/esgf_crawl_config.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.030214 freva-2303.0.0/src/evaluation_system/misc/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      464 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/misc/__init__.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    12399 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/misc/config.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2186 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/misc/exceptions.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    19289 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/misc/utils.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.030214 freva-2303.0.0/src/evaluation_system/model/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       43 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/model/__init__.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    13347 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/model/db.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    10153 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/model/esgf.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    21455 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/model/file.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.030214 freva-2303.0.0/src/evaluation_system/model/history/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/model/history/__init__.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    13492 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/model/history/models.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.030214 freva-2303.0.0/src/evaluation_system/model/plugins/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/model/plugins/__init__.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     1960 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/model/plugins/models.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2821 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/model/repository.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    10407 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/model/solr.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    16758 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/model/solr_core.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.030214 freva-2303.0.0/src/evaluation_system/model/solr_models/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/model/solr_models/__init__.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      886 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/model/solr_models/models.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    12419 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/model/user.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.030214 freva-2303.0.0/src/evaluation_system/settings/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/settings/__init__.py
--rwxr-xr-x   0 wilfred   (1000) wilfred   (1001)      894 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/settings/database.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.030214 freva-2303.0.0/src/evaluation_system/tests/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      707 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/__init__.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     4635 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/cli_argcomplete_test.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     1873 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/cli_help_test.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    13776 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/conftest.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    13422 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/crawl_my_data_test.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     8863 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/databrowser_test.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     6501 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/db_test.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     4088 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/esgf_test.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2832 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/file_test.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2899 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/history_command_test.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2102 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/history_models_test.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.030214 freva-2303.0.0/src/evaluation_system/tests/mocks/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2332 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/mocks/__init__.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     3647 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/mocks/dummy.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      862 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/mocks/result_tags.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    14786 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/parameters_test.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     5335 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/plugin_command_test.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    13173 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/plugin_manager_test.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    22496 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/plugin_test.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     3384 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/solr_core_test.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2036 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/solr_test.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     6816 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/user_test.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     6126 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/utils_test.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.030214 freva-2303.0.0/src/evaluation_system/tests/workload_manager/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       27 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/workload_manager/__init__.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      253 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/workload_manager/test_core.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     1009 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/workload_manager/test_local.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     6059 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/workload_manager/test_lsf.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2296 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/workload_manager/test_oar.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     3134 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/workload_manager/test_pbs.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      937 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/workload_manager/test_sge.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     3017 2023-03-08 07:38:15.000000 freva-2303.0.0/src/evaluation_system/tests/workload_manager/test_slurm.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.033548 freva-2303.0.0/src/freva/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      418 2023-03-08 07:38:15.000000 freva-2303.0.0/src/freva/__init__.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     9297 2023-03-08 07:38:15.000000 freva-2303.0.0/src/freva/_databrowser.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     3476 2023-03-08 07:38:15.000000 freva-2303.0.0/src/freva/_esgf.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     4054 2023-03-08 07:38:15.000000 freva-2303.0.0/src/freva/_history.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    10554 2023-03-08 07:38:15.000000 freva-2303.0.0/src/freva/_plugin.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    11420 2023-03-08 07:38:15.000000 freva-2303.0.0/src/freva/_user_data.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.033548 freva-2303.0.0/src/freva/cli/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     1608 2023-03-08 07:38:15.000000 freva-2303.0.0/src/freva/cli/__init__.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      333 2023-03-08 07:38:15.000000 freva-2303.0.0/src/freva/cli/__main__.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     5222 2023-03-08 07:38:15.000000 freva-2303.0.0/src/freva/cli/databrowser.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     5122 2023-03-08 07:38:15.000000 freva-2303.0.0/src/freva/cli/esgf.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     3553 2023-03-08 07:38:15.000000 freva-2303.0.0/src/freva/cli/history.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     5304 2023-03-08 07:38:15.000000 freva-2303.0.0/src/freva/cli/plugin.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     8745 2023-03-08 07:38:15.000000 freva-2303.0.0/src/freva/cli/user_data.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)    16899 2023-03-08 07:38:15.000000 freva-2303.0.0/src/freva/cli/utils.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-08 07:39:40.033548 freva-2303.0.0/src/freva.egg-info/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     6173 2023-03-08 07:39:40.000000 freva-2303.0.0/src/freva.egg-info/PKG-INFO
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     4497 2023-03-08 07:39:40.000000 freva-2303.0.0/src/freva.egg-info/SOURCES.txt
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)        1 2023-03-08 07:39:40.000000 freva-2303.0.0/src/freva.egg-info/dependency_links.txt
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      240 2023-03-08 07:39:40.000000 freva-2303.0.0/src/freva.egg-info/entry_points.txt
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      615 2023-03-08 07:39:40.000000 freva-2303.0.0/src/freva.egg-info/requires.txt
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       24 2023-03-08 07:39:40.000000 freva-2303.0.0/src/freva.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.815288 freva-2307.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-13 08:55:09.000000 freva-2307.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-13 08:55:09.000000 freva-2307.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-13 08:55:23.815288 freva-2307.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-13 08:55:09.000000 freva-2307.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.803288 freva-2307.0.0/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.799288 freva-2307.0.0/assets/completions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.803288 freva-2307.0.0/assets/completions/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/bash/freva
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.803288 freva-2307.0.0/assets/completions/fish/
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/fish/freva.fish
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.803288 freva-2307.0.0/assets/completions/tcsh/
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/tcsh/tcsh-completion.bash
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.803288 freva-2307.0.0/assets/completions/zsh/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/zsh/_freva
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/zsh/_freva_crawl_my_data
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/zsh/_freva_databrowser
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/zsh/_freva_esgf
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/zsh/_freva_history
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/zsh/_freva_plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/zsh/completions.zsh
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/zsh/source.zsh
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/drs_config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/evaluation_system.conf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15492 2023-07-13 08:55:09.000000 freva-2307.0.0/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 08:55:23.815288 freva-2307.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7005 2023-07-13 08:55:09.000000 freva-2307.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.803288 freva-2307.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.803288 freva-2307.0.0/src/evaluation_system/
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.807288 freva-2307.0.0/src/evaluation_system/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35205 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48142 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45916 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/user_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.807288 freva-2307.0.0/src/evaluation_system/api/workload_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/workload_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/workload_manager/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/workload_manager/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/workload_manager/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/workload_manager/moab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/workload_manager/oar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/workload_manager/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/workload_manager/sge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/workload_manager/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.807288 freva-2307.0.0/src/evaluation_system/fuse/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/fuse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/fuse/esgf2fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/fuse/esgf2solr_crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/fuse/esgf_crawl_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.807288 freva-2307.0.0/src/evaluation_system/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/misc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/misc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/misc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.807288 freva-2307.0.0/src/evaluation_system/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/esgf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21607 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.807288 freva-2307.0.0/src/evaluation_system/model/history/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/history/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.807288 freva-2307.0.0/src/evaluation_system/model/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/plugins/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10560 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/solr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16938 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/solr_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.811288 freva-2307.0.0/src/evaluation_system/model/solr_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/solr_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/solr_models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.811288 freva-2307.0.0/src/evaluation_system/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/settings/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      894 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/settings/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.811288 freva-2307.0.0/src/evaluation_system/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/cli_argcomplete_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/cli_help_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13776 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/crawl_my_data_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/databrowser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/db_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/esgf_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/history_command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/history_models_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.811288 freva-2307.0.0/src/evaluation_system/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/mocks/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/mocks/dummyfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/mocks/result_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14786 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/parameters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/plugin_command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/plugin_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22496 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/plugin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/solr_core_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/solr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/user_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.811288 freva-2307.0.0/src/evaluation_system/tests/workload_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/workload_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_oar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_sge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.815288 freva-2307.0.0/src/freva/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17406 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/_databrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/_esgf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/_user_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.815288 freva-2307.0.0/src/freva/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/cli/databrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/cli/esgf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/cli/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/cli/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/cli/user_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16899 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.815288 freva-2307.0.0/src/freva.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-13 08:55:23.000000 freva-2307.0.0/src/freva.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-13 08:55:23.000000 freva-2307.0.0/src/freva.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:55:23.000000 freva-2307.0.0/src/freva.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-13 08:55:23.000000 freva-2307.0.0/src/freva.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-13 08:55:23.000000 freva-2307.0.0/src/freva.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 08:55:23.000000 freva-2307.0.0/src/freva.egg-info/top_level.txt
```

### Comparing `freva-2303.0.0/LICENSE.md` & `freva-2307.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/PKG-INFO` & `freva-2307.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freva
-Version: 2303.0.0
+Version: 2307.0.0
 Summary: Free Evaluation and Analysis Framework (Freva) 
 Author: German Climate Computing Centre (DKRZ)
 Maintainer: Climate Informatics and Technology (CLINT)
 License: BSD-3-Clause
 Project-URL: Documentation, https://freva.gitlab-pages.dkrz.de/evaluation_system/sphinx_docs/index.html
 Project-URL: Release notes, https://freva.gitlab-pages.dkrz.de/evaluation_system/sphinx_docs/whats-new.html
 Project-URL: Issues, https://gitlab.dkrz.de/freva/evaluation_system/-/issues
@@ -28,15 +28,15 @@
 Provides-Extra: test
 License-File: LICENSE.md
 
 # Free Evaluation System Framework
 
 [![PyPI version](https://badge.fury.io/py/freva.svg)](https://badge.fury.io/py/freva)
 [![Update](https://anaconda.org/conda-forge/freva/badges/latest_release_date.svg)](https://github.com/FREVA-CLINT/freva)
-[![Conda](https://anaconda.org/conda-forge/freva/badges/installer/conda.svg)](https://anaconda.org/conda-forge/freva)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/freva/badges/version.svg)](https://anaconda.org/conda-forge/freva)
 [![Docs](https://img.shields.io/badge/Freva-Docs-green.svg)](https://freva-clint.github.io/freva)
 [![codecov](https://codecov.io/gh/FREVA-CLINT/freva/branch/main/graph/badge.svg)](https://codecov.io/gh/FREVA-CLINT/freva)
 [![Pipeline](https://github.com/FREVA-CLINT/freva/actions/workflows/ci_job.yml/badge.svg)](https://github.com/FREVA-CLINT/freva/actions)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/FREVA-CLINT/freva/main?labpath=Readme.ipynb)
 [![BSD](https://anaconda.org/conda-forge/freva/badges/license.svg)](https://github.com/FREVA-CLINT/freva)
 
 <img src="docs/source/_static/freva_flowchart-new.jpg" alt="Freva" width="400"/>
```

### Comparing `freva-2303.0.0/README.md` & `freva-2307.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Free Evaluation System Framework
 
 [![PyPI version](https://badge.fury.io/py/freva.svg)](https://badge.fury.io/py/freva)
 [![Update](https://anaconda.org/conda-forge/freva/badges/latest_release_date.svg)](https://github.com/FREVA-CLINT/freva)
-[![Conda](https://anaconda.org/conda-forge/freva/badges/installer/conda.svg)](https://anaconda.org/conda-forge/freva)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/freva/badges/version.svg)](https://anaconda.org/conda-forge/freva)
 [![Docs](https://img.shields.io/badge/Freva-Docs-green.svg)](https://freva-clint.github.io/freva)
 [![codecov](https://codecov.io/gh/FREVA-CLINT/freva/branch/main/graph/badge.svg)](https://codecov.io/gh/FREVA-CLINT/freva)
 [![Pipeline](https://github.com/FREVA-CLINT/freva/actions/workflows/ci_job.yml/badge.svg)](https://github.com/FREVA-CLINT/freva/actions)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/FREVA-CLINT/freva/main?labpath=Readme.ipynb)
 [![BSD](https://anaconda.org/conda-forge/freva/badges/license.svg)](https://github.com/FREVA-CLINT/freva)
 
 <img src="docs/source/_static/freva_flowchart-new.jpg" alt="Freva" width="400"/>
```

### Comparing `freva-2303.0.0/assets/completions/bash/freva` & `freva-2307.0.0/assets/completions/bash/freva`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/assets/completions/fish/freva.fish` & `freva-2307.0.0/assets/completions/fish/freva.fish`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/assets/completions/tcsh/tcsh-completion.bash` & `freva-2307.0.0/assets/completions/tcsh/tcsh-completion.bash`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/assets/completions/zsh/_freva` & `freva-2307.0.0/assets/completions/zsh/_freva`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/assets/completions/zsh/completions.zsh` & `freva-2307.0.0/assets/completions/zsh/completions.zsh`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/assets/drs_config.toml` & `freva-2307.0.0/assets/drs_config.toml`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/assets/evaluation_system.conf` & `freva-2307.0.0/assets/evaluation_system.conf`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/deploy.py` & `freva-2307.0.0/deploy.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/setup.py` & `freva-2307.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,24 +152,24 @@
     setup_requires=["appdirs"],
     extras_require={
         "docs": [
             "bash_kernel",
             "cartopy",
             "cftime",
             "cf_xarray",
+            "furo",
             "ipython",
             "ipykernel",
             "nbsphinx",
             "pint",
             "pint-xarray",
             "recommonmark",
             "sphinx",
             "sphinxcontrib_github_alt",
             "sphinx-execute-code-python3",
-            "sphinx-rtd-theme",
             "xarray",
             "h5netcdf",
         ],
         "test": [
             "allure-pytest",
             "black",
             "django-stubs",
```

### Comparing `freva-2303.0.0/src/evaluation_system/__init__.py` & `freva-2307.0.0/src/evaluation_system/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,9 +26,15 @@
 INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
 BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
 OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED
 OF THE POSSIBILITY OF SUCH DAMAGE.
 """
+import warnings
 
-__version__ = "2303.0.0"
+warnings.filterwarnings(
+    "always", category=PendingDeprecationWarning, module="evaluation_system.*"
+)
+
+
+__version__ = "2307.0.0"
```

### Comparing `freva-2303.0.0/src/evaluation_system/api/parameters.py` & `freva-2307.0.0/src/evaluation_system/api/parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,55 +28,55 @@
 ParameterBaseType = Union[str, int, float, bool, PrintableList]
 """Type definitions of all possible parameter types."""
 
 
 class ParameterType(initOrder):
     """Base class for all prameter types.
 
-     All available parameter types inherit from this class. The class creates
-     a parameter object holding the following user defined information.
+    All available parameter types inherit from this class. The class creates
+    a parameter object holding the following user defined information.
 
-     Parameters
-     ----------
+    Parameters
+    ----------
 
-     name: str
-         Name of the parameter.
-     default: ParameterBaseType, default: str
-         the default value of the given parameter. **Note**: this value must be
-         a *valid* parameter value!
+    name: str
+        Name of the parameter.
+    default: ParameterBaseType, default: str
+        the default value of the given parameter. **Note**: this value must be
+        a *valid* parameter value!
     mandatory: bool, default: False
-         boolean indicating if this parameter is required
-     max_items: int, default: 1
-         If set to > 1 it will cause the values to be returned in a
-         list (even if the user only provided 1). Raises an error if more than
-         than ``max_items`` values are parsed.
-     item_separator: str, default: ,
-         The string used to separate multiple values for this
-         parameter. In some cases (at the shell, web interface, etc) the user have
-         always the option to provide multiple values by re-using the same parameter
-         name (e.g. ``param1=a param1=b`` produces ``{'param1': ['a', 'b']}``). But the
-         configuration file does not allow this at this time. Therefore is better
-         to setup a separator, even though the user might not use it while giving
-         input. It must not be a character, it can be any string
-         (make sure it's not a valid value!!)
-     regex: Optional[str], default: None
-         A regular expression defining valid "string" values before
-         parsing them to their defining classes (e.g. an Integer might define a
-         regex of "[0-9]+" to prevent getting negative numbers). This will be used
-         also on Javascript so don't use fancy expressions or make sure they are
-         understood by both python and Javascript.
-     help: str, default: No help available
-         The help string describing what this parameter is good for.
-     print_format: str, default %s
-         String format used to display parameter values, e.g. ``%.2f`` to
-         display always 2 decimals for floats
-     impact:
-         The impact of the parameter to the output, possible values are
-         Parameter.Impact.affects_values, Parameter.Impact.affects_plots, Parameter.
-         Impact.no_effects
+        boolean indicating if this parameter is required
+    max_items: int, default: 1
+        If set to > 1 it will cause the values to be returned in a
+        list (even if the user only provided 1). Raises an error if more than
+        than ``max_items`` values are parsed.
+    item_separator: str, default: ,
+        The string used to separate multiple values for this
+        parameter. In some cases (at the shell, web interface, etc) the user have
+        always the option to provide multiple values by re-using the same parameter
+        name (e.g. ``param1=a param1=b`` produces ``{'param1': ['a', 'b']}``). But the
+        configuration file does not allow this at this time. Therefore is better
+        to setup a separator, even though the user might not use it while giving
+        input. It must not be a character, it can be any string
+        (make sure it's not a valid value!!)
+    regex: Optional[str], default: None
+        A regular expression defining valid "string" values before
+        parsing them to their defining classes (e.g. an Integer might define a
+        regex of "[0-9]+" to prevent getting negative numbers). This will be used
+        also on Javascript so don't use fancy expressions or make sure they are
+        understood by both python and Javascript.
+    help: str, default: No help available
+        The help string describing what this parameter is good for.
+    print_format: str, default %s
+        String format used to display parameter values, e.g. ``%.2f`` to
+        display always 2 decimals for floats
+    impact: int
+        The impact of the parameter to the output, possible values are
+        Parameter.Impact.affects_values, Parameter.Impact.affects_plots, Parameter.
+        Impact.no_effects
 
 
      Properties
      ----------
 
      base_type:
          Type of this parameter
```

### Comparing `freva-2303.0.0/src/evaluation_system/api/plugin.py` & `freva-2307.0.0/src/evaluation_system/api/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 For this purpose we assume that a plugin core (without Freva) already exists
 - for example as a command line interface tool (cli). Once such a cli has been
 set up a interface to Freva must be defined. This reference will introduce
 the possible definition options below.
 
 Here we assume that the above mentioned cli code is stored in a directory
 name ``/mnt/freva/plugins/new_plugin`` furthermore the actual cli code can be
-excecuted via:
+executed via:
+
     .. code-block:: console
 
         cli/calculate -c 5 -n 6.4 --overwrite --name=Test
 
 With help of this API a Freva plugin can be created in ``/mnt/freva/plugin/new_plugin/plugin.py``
 
 """
@@ -454,23 +455,14 @@
             if isinstance(tmp_param, (Directory, CacheDirectory)) and unique_output:
                 if key in config_dict.keys() and config_dict[key] is not None:
                     config_dict[key] = os.path.join(
                         str(config_dict[key]), str(self.rowid)
                     )
         return config_dict
 
-    def quitnkill(self):
-        """If error occurs quit python and kill child processes by group ID
-
-        :meta private:
-        """
-        PID = os.getpid()
-        self.call(f'setsid nohup bash -c "kill -9 -- -{PID}"  </dev/null &>/dev/null &')
-        raise SystemExit
-
     @deprecated_method("PluginAbstract", "add_output_to_databrowser")
     def linkmydata(self, *args, **kwargs):  # pragma: no cover
         """Deprecated version of the :class:`add_output_to_databrowser` method.
 
         :meta private:
         """
         return self.add_output_to_databrowser(**args, **kwargs)
@@ -483,14 +475,15 @@
         *,
         model: str = "freva",
         institute: Optional[str] = None,
         ensemble: str = "r1i1p1",
         time_frequency: Optional[str] = None,
         variable: Optional[str] = None,
         experiment: Optional[str] = None,
+        index_data: bool = True,
     ) -> Path:
         """Add Plugin output data to the solr database.
 
         This methods crawls the plugin output data directory and adds
         any files that were found to the apache solr database.
 
         ..note::
@@ -498,17 +491,17 @@
             arguments to specify the search facets that are going to be
             added to the solr server for this pluign run. This will help
             users better to better distinguish their plugin result search.
 
         The following facets are fixed:
 
         - project: ``user-<user_name>``
-        - product: ``<plugin_name>``
+        - product: ``<project>.<produc>``
+        - realm: ``<plugin_name>``
         - dataset version: ``<history_id>``
-        - realm: ``plugins``
 
         Parameters
         ----------
         plugin_output: os.PathLike
             Plugin output directory or file created by the files. If a
             directory is given all data files within the sub directories
             will be collected for ingestion.
@@ -533,14 +526,18 @@
             Default time frequency facet. If None is given (default) the time
             frequency will be retrieved from the output files.
         experiment: str, default: freva-plugin
             Default time experiment facet.
         variable: str, default: None
             Default variable facet. If None is given (default) the variable
             will be retrieved from the output files.
+        index_data: bool, default: True
+            Update the freva data browser (default: True). Setting this
+            flag to false can be useful if the data structure should only be
+            created but the databrowser should not be updated yet.
 
         Returns
         -------
             Path: Path to the new directory that containes the data.
         """
         _, plugin_version = repository.get_version(self.wrapper_file)
         plugin_version = plugin_version or "no_plugin_version"
@@ -549,30 +546,33 @@
 
         product_dir = f"{project}.{product}"
         root_dir = DataReader.get_output_directory() / f"user-{self._user.getName()}"
         drs_config = dict(
             project=root_dir.name,
             product=product_dir,
             model=model,
-            experiment=experiment or "frev-plugin",
+            experiment=experiment or "freva-plugin",
             realm=plugin,
             institute=institute or project_name,
             ensemble=ensemble,
             version=f"v{self.rowid}",
         )
         if time_frequency:
             drs_config["time_frequency"] = time_frequency
         if variable:
             drs_config["variable"] = variable
         user_data = DataReader(plugin_output, **drs_config)
         for output_file in user_data:
             new_file = user_data.file_name_from_metdata(output_file)
             new_file.parent.mkdir(exist_ok=True, parents=True, mode=0o2775)
             shutil.copy(str(output_file), str(new_file))
-        SolrCore.load_fs(root_dir / product_dir, drs_type=user_data.drs_specification)
+        if index_data:
+            SolrCore.load_fs(
+                root_dir / product_dir, drs_type=user_data.drs_specification
+            )
         return root_dir / product_dir
 
     @deprecated_method("PluginAbstract", "prepare_output")
     def prepareOutput(self, *args) -> dict[str, dict[str, str]]:
         """Deprecated method for :class:`prepare_output`.
 
         :meta private:
@@ -679,14 +679,15 @@
                 elif ext in ".nc .bin .ascii".split():
                     metadata["type"] = "data"
                 if ext in [".zip"]:
                     metadata["type"] = "pdf"
                     metadata["todo"] = "copy"
                 elif ext in [".html", ".xhtml"]:
                     metadata["todo"] = "copy"
+                    metadata["type"] = "html"
 
     @deprecated_method("PluginAbstract", "get_help")
     def getHelp(self, **kwargs) -> str:
         """Deprecated version of the :class:`get_help` method.
 
         :meta private:
         """
@@ -1189,15 +1190,15 @@
         if caption is not None:
             quote_caption = caption
             quote_caption = caption.replace("\\", "\\\\")
             quote_caption = quote_caption.replace("'", "'\\''")
             cmd_param.append(f"--caption '{quote_caption}'")
 
         # append the unique_output param
-        cmd_param.append(f"--unique_output {unique_output}")
+        cmd_param.append(f"--unique-output {unique_output}")
 
         # a scheduled id overrides the dictionary behavior
         if scheduled_id:
             cmd_param.append(f"--scheduled-id {scheduled_id}")
 
         else:
             # store the section header
```

### Comparing `freva-2303.0.0/src/evaluation_system/api/plugin_manager.py` & `freva-2307.0.0/src/evaluation_system/api/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/api/user_data.py` & `freva-2307.0.0/src/evaluation_system/api/user_data.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/api/workload_manager/__init__.py` & `freva-2307.0.0/src/evaluation_system/api/workload_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/api/workload_manager/core.py` & `freva-2307.0.0/src/evaluation_system/api/workload_manager/core.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/api/workload_manager/local.py` & `freva-2307.0.0/src/evaluation_system/api/workload_manager/local.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/api/workload_manager/lsf.py` & `freva-2307.0.0/src/evaluation_system/api/workload_manager/lsf.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/api/workload_manager/oar.py` & `freva-2307.0.0/src/evaluation_system/api/workload_manager/oar.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/api/workload_manager/pbs.py` & `freva-2307.0.0/src/evaluation_system/api/workload_manager/pbs.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/api/workload_manager/sge.py` & `freva-2307.0.0/src/evaluation_system/api/workload_manager/sge.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/api/workload_manager/slurm.py` & `freva-2307.0.0/src/evaluation_system/api/workload_manager/slurm.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/fuse/esgf2fs.py` & `freva-2307.0.0/src/evaluation_system/fuse/esgf2fs.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/fuse/esgf2solr_crawl.py` & `freva-2307.0.0/src/evaluation_system/fuse/esgf2solr_crawl.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/fuse/esgf_crawl_config.py` & `freva-2307.0.0/src/evaluation_system/fuse/esgf_crawl_config.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/misc/config.py` & `freva-2307.0.0/src/evaluation_system/misc/config.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/misc/exceptions.py` & `freva-2307.0.0/src/evaluation_system/misc/exceptions.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/misc/utils.py` & `freva-2307.0.0/src/evaluation_system/misc/utils.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/model/db.py` & `freva-2307.0.0/src/evaluation_system/model/db.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/model/esgf.py` & `freva-2307.0.0/src/evaluation_system/model/esgf.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/model/file.py` & `freva-2307.0.0/src/evaluation_system/model/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,23 +13,29 @@
     Union,
     Any,
     ClassVar,
     cast,
 )
 from typing_extensions import Literal, TypedDict
 from dataclasses import dataclass, field
-
+import warnings
 import json
 from pathlib import Path
 import os
 import logging
 from evaluation_system.misc import config
 
 log = logging.getLogger(__name__)
 
+
+warnings.warn(
+    "The evaluation_system.model.file module will be removed from v2304.0.0",
+    category=PendingDeprecationWarning,
+)
+
 Activity = str
 """Represents a type of data collection activity for DRS (see Activity from the DRS spec).
 
     This doesn't prevent typing issues beyond what you'd get with `str` but  I think
     it makes the functions that deal with Activities more clear than simply using `str`
 """
```

### Comparing `freva-2303.0.0/src/evaluation_system/model/history/models.py` & `freva-2307.0.0/src/evaluation_system/model/history/models.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/model/plugins/models.py` & `freva-2307.0.0/src/evaluation_system/model/plugins/models.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/model/repository.py` & `freva-2307.0.0/src/evaluation_system/model/repository.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/model/solr.py` & `freva-2307.0.0/src/evaluation_system/model/solr.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 This package encapsulate access to a solr instance
 """
 
 from __future__ import annotations
 import urllib
 from typing import cast, Union, List, NamedTuple
 from typing_extensions import Literal
+import warnings
 
 from evaluation_system.model.solr_core import SolrCore
 from evaluation_system.misc import logger, utils
 
 SolrResponse = NamedTuple(
     "SolrResponse",
     [
@@ -21,14 +22,20 @@
         ("start", int),
         ("exact", bool),
         ("docs", List[str]),
     ],
 )
 
 
+warnings.warn(
+    "The evaluation_system.model.solr module will be removed from v2304.0.0",
+    category=PendingDeprecationWarning,
+)
+
+
 class SolrFindFiles(object):
     """Encapsulate access to Solr like the find files command"""
 
     def __init__(self, core=None, host=None, port=None, get_status=False):
         """Create the connection pointing to the proper solr url and core.
         The default values of these parameters are setup in evaluation_system.model.solr_core.SolrCore
         and read from the configuration file.
```

### Comparing `freva-2303.0.0/src/evaluation_system/model/solr_core.py` & `freva-2307.0.0/src/evaluation_system/model/solr_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,26 @@
 import shutil
 import urllib
 import urllib.request
 import json
 from datetime import datetime
 from pathlib import Path
 from typing import Dict, Iterator, Optional, Tuple
+import warnings
 
 from evaluation_system.model.file import DRSFile
 from evaluation_system.misc import config, logger as log
 from evaluation_system.misc.utils import get_solr_time_range
 from evaluation_system.misc.exceptions import CommandError
 
+warnings.warn(
+    ("The evaluation_system.model.solr_core module will be removed from " "v2304.0.0"),
+    category=PendingDeprecationWarning,
+)
+
 
 class SolrCore:
     """Encapsulate access to a Solr instance"""
 
     def __init__(
         self,
         core=None,
@@ -141,15 +147,16 @@
         """Creates (actually "register") this core. The Core configuration and directories must
         be generated beforehand (not the data one). You may clone an existing one or start from scratch.
 
         :param instance_dir: main directory for this core
         :param data_dir: Data directory for this core (if left unset, a local "data" directory in instance_dir will be used)
         :param config: The configuration file (expected in instance_dir/conf)
         :param schema: The schema file (expected in instance_dir/conf)
-        :param check_if_exist: check for the existence of the instance directorie"""
+        :param check_if_exist: check for the existence of the instance directorie
+        """
         # check basic configuration (it must exists!)
         if instance_dir is None and self.instance_dir is None:
             raise ValueError("No Instance directory defined!")
         elif instance_dir is not None:
             self.instance_dir = instance_dir
         if not os.path.isdir(self.instance_dir) and check_if_exist:
             raise FileNotFoundError(
@@ -181,15 +188,16 @@
         return self.get_json(
             "admin/cores?action=UNLOAD&core=" + self.core, use_core=False
         )
 
     def swap(self, other_core):
         """Will swap this core with the given one (that means rename their references)
 
-        :param other_core: the name of the other core that this will be swapped with."""
+        :param other_core: the name of the other core that this will be swapped with.
+        """
         return self.get_json(
             "admin/cores?action=SWAP&core=%s&other=%s" % (self.core, other_core),
             use_core=False,
         )
 
     def status(self, general=False):
         """Return status information about this core or the whole Solr server.
```

### Comparing `freva-2303.0.0/src/evaluation_system/model/solr_models/models.py` & `freva-2307.0.0/src/evaluation_system/model/solr_models/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 """
 Created on 21.04.2015
 
 @author: sebastian.illing@met.fu-berlin.de
 """
 from django.db import models
 from django.contrib.auth.models import User
+import warnings
+
+warnings.warn(
+    (
+        "The evaluation_system.model.solr_models module will be removed from "
+        "v2304.0.0"
+    ),
+    category=PendingDeprecationWarning,
+)
 
 
 class UserCrawl(models.Model):
     """
     Simple model to track user solr-crawls
     """
```

### Comparing `freva-2303.0.0/src/evaluation_system/model/user.py` & `freva-2307.0.0/src/evaluation_system/model/user.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/settings/database.py` & `freva-2307.0.0/src/evaluation_system/settings/database.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/__init__.py` & `freva-2307.0.0/src/evaluation_system/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/cli_argcomplete_test.py` & `freva-2307.0.0/src/evaluation_system/tests/cli_argcomplete_test.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/cli_help_test.py` & `freva-2307.0.0/src/evaluation_system/tests/cli_help_test.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/conftest.py` & `freva-2307.0.0/src/evaluation_system/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/crawl_my_data_test.py` & `freva-2307.0.0/src/evaluation_system/tests/crawl_my_data_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         valid_data_files, "muh", "mah", experiment="foo"
     )
     assert len(list(freva.databrowser(experiment="foo"))) == len(input_files)
     assert len(list(freva.databrowser(product="muh.mah"))) == len(input_files)
 
 
 def test_add_my_data(valid_data_files, time_mock):
-    from freva import UserData, databrowser
+    from freva import UserData, count_values
     from freva.cli.user_data import main as run
 
     defaults = [
         "--institute",
         "tong",
         "--model",
         "mrfu",
@@ -239,15 +239,15 @@
     input_files = list(valid_data_files.rglob("*.nc"))
     with pytest.raises(SystemExit):
         run(["add", "foo-product", str(valid_data_files)])
     with pytest.raises(ValueError):
         run(["add", "foo-product", str(valid_data_files), "-d"])
 
     user_data = UserData()
-    assert databrowser(product="foo-product", count=True) == len(input_files)
+    assert count_values(product="foo-product") == len(input_files)
     with pytest.raises(ValueError):
         user_data.add("foo-product", valid_data_files, how="foo")
     with pytest.warns(UserWarning):
         user_data.add("foo-product")
 
 
 def test_add_methods():
```

### Comparing `freva-2303.0.0/src/evaluation_system/tests/databrowser_test.py` & `freva-2307.0.0/src/evaluation_system/tests/databrowser_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,38 +6,39 @@
 
 def test_index_len(dummy_solr):
     assert dummy_solr.all_files.status()["index"]["numDocs"] == 5
     assert dummy_solr.latest.status()["index"]["numDocs"] == 3
 
 
 def test_time_subsets(dummy_solr):
-    from freva import databrowser
+    from freva import databrowser, count_values
 
-    files = list(databrowser(project="cmip5"))
-    subset_1 = databrowser(project="cmip5", time="2000-12 to 2012-12", count=True)
-    subset_2 = databrowser(project="cmip5", time="1900 to 1918", count=True)
-    subset_3 = databrowser(project="cmip5", time="2100", count=True)
-    subset_4 = databrowser(
+    subset_1 = count_values(project="cmip5", time="2000-12 to 2012-12")
+    subset_2 = count_values(
+        project="cmip5",
+        time="1900 to 1918",
+    )
+    subset_3 = count_values(project="cmip5", time="2100")
+    subset_4 = count_values(
         project="cmip5",
         time="2000-12 to 2012-12",
-        count=True,
         time_select="strict",
     )
     with pytest.raises(ValueError):
-        databrowser(time="2000-12 to bar", count=True)
+        count_values(time="2000-12 to bar")
     assert subset_1 == 2
     assert subset_2 == 1
     assert subset_3 == 0
     assert subset_4 == 0
     with pytest.raises(ValueError):
         databrowser(time_select="bar")
 
 
 def test_freva_databrowser_method(dummy_solr):
-    from freva import databrowser
+    from freva import databrowser, count_values, facet_search
 
     all_files_output = sorted(
         [
             f"{dummy_solr.tmpdir}/cmip5/output1/MOHC/HadCM3/historical/mon/aerosol/aero/r2i1p1/v20110728/wetso2/wetso2_aero_HadCM3_historical_r2i1p1_190912-193411.nc",
             f"{dummy_solr.tmpdir}/cmip5/output1/MOHC/HadCM3/decadal2009/mon/atmos/Amon/r7i2p1/v20110819/ua/ua_Amon_HadCM3_decadal2009_r7i2p1_200911-201912.nc",
             f"{dummy_solr.tmpdir}/cmip5/output1/MOHC/HadCM3/decadal2008/mon/atmos/Amon/r9i3p1/v20120523/tauu/tauu_Amon_HadCM3_decadal2008_r9i3p1_200811-201812.nc",
         ]
@@ -54,23 +55,23 @@
     )
     res = sorted(databrowser(variable=["ua", "tauu"]))
     assert res == target
     res = list(databrowser(variable=["ua", "tauu"], rows=1))
     assert len(res) == 1
     res = sorted(databrowser(variable=["ua", "tauu", "wetso2"]))
     assert res == all_files_output
-    res = databrowser(variable=["ua", "tauu", "wetso2"], count=True)
+    res = count_values(variable=["ua", "tauu", "wetso2"])
     assert res == len(all_files_output)
     assert databrowser(variable="whhoop", count=True) == 0
     v = "v20110419"
-    res = sorted(databrowser(variable="ua", version=v))
+    res = sorted(databrowser(variable="ua", version=v, multiversion=True))
     assert v in res[0]
     with pytest.raises(TypeError):
         databrowser("badoption")
-    res = databrowser(all_facets=True, relevant_only=True)
+    res = facet_search(facet=None)
     assert isinstance(res, dict)
     target = sorted(
         [
             "cmor_table",
             "product",
             "realm",
             "dataset",
@@ -80,25 +81,15 @@
             "experiment",
             "variable",
             "model",
             "ensemble",
             "fs_type",
         ]
     )
-    relevant = [
-        "cmor_table",
-        "ensemble",
-        "experiment",
-        "realm",
-        "variable",
-    ]
-    res = sorted(databrowser(attributes=True))
-    assert sorted(target) == res
     res = sorted(databrowser(attributes=True, relevant_only=True))
-    assert relevant == res
 
 
 def test_search_files_cmd(dummy_solr, capsys):
     from evaluation_system.misc.exceptions import CommandError
     from freva.cli.databrowser import main as run
 
     cmd = shlex.split("databrowser")
@@ -135,15 +126,15 @@
     assert res == target
     run_cli(cmd + ["variable=ua", "variable=tauu", "variable=wetso2"])
     res = capsys.readouterr().out
     res = [f for f in sorted(res.split("\n")) if f]
     assert res == all_files_output
     # search specific version
     v = "v20110419"
-    run_cli(cmd + ["variable=ua", f"version={v}"])
+    run_cli(cmd + ["variable=ua", f"version={v}", "--multiversion"])
     res = capsys.readouterr().out
     assert v in res
     # test bad input
     with pytest.raises(ValueError):
         run_cli(cmd + ["badoption"])
```

### Comparing `freva-2303.0.0/src/evaluation_system/tests/db_test.py` & `freva-2307.0.0/src/evaluation_system/tests/db_test.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/esgf_test.py` & `freva-2307.0.0/src/evaluation_system/tests/esgf_test.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/file_test.py` & `freva-2307.0.0/src/evaluation_system/tests/file_test.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/history_command_test.py` & `freva-2307.0.0/src/evaluation_system/tests/history_command_test.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/history_models_test.py` & `freva-2307.0.0/src/evaluation_system/tests/history_models_test.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/mocks/__init__.py` & `freva-2307.0.0/src/evaluation_system/tests/mocks/__init__.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/mocks/dummy.py` & `freva-2307.0.0/src/evaluation_system/tests/mocks/dummy.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from evaluation_system.api.plugin import PluginAbstract
 from evaluation_system.api.parameters import (
     ParameterDictionary,
     Integer,
     Float,
     String,
     InputDirectory,
+    Directory,
 )
 
 from evaluation_system.model.user import User
 from evaluation_system.model.db import UserDB
 
 
 class DummyPlugin(PluginAbstract):
```

### Comparing `freva-2303.0.0/src/evaluation_system/tests/mocks/result_tags.py` & `freva-2307.0.0/src/evaluation_system/tests/mocks/result_tags.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/parameters_test.py` & `freva-2307.0.0/src/evaluation_system/tests/parameters_test.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/plugin_command_test.py` & `freva-2307.0.0/src/evaluation_system/tests/plugin_command_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,16 +17,14 @@
     ValidationError,
 )
 
 
 @mock.patch("os.getpid", lambda: 12345)
 def test_cli(dummy_plugin, capsys, dummy_config, caplog):
     from freva.cli.plugin import main as plugin_cli
-    import time
-    from evaluation_system.misc.exceptions import ValidationError
     from evaluation_system.misc import config
 
     with pytest.raises(ValidationError):
         plugin_cli(["dummyplugin"])
     plugin_cli(["dummyplugin", "the_number=13"])
     output = capsys.readouterr().out
     assert "the_number" in output
@@ -52,14 +50,45 @@
     output = capsys.readouterr().out
     assert "tail -f" in output
     out_f = Path([o.split()[-1] for o in output.split("\n") if "tail" in o][0])
     assert out_f.exists()
     with out_f.open() as f:
         assert "pending" in f.read()
 
+    import re, freva
+
+    pattern = r"'outputdir': '([^']*)'"
+
+    plugin_cli(["dummypluginfolders", "variable=pr"])
+    output_str = capsys.readouterr().out
+    match = re.search(pattern, output_str)
+    if match:
+        folder_path = match.group(1)
+    assert str(freva.history()[0]["id"]) in os.path.basename(
+        os.path.normpath(folder_path)
+    )
+
+    plugin_cli(["dummypluginfolders", "variable=pr", "--unique-output", "true"])
+    output_str = capsys.readouterr().out
+    match = re.search(pattern, output_str)
+    if match:
+        folder_path = match.group(1)
+    assert str(freva.history()[0]["id"]) in os.path.basename(
+        os.path.normpath(folder_path)
+    )
+
+    plugin_cli(["dummypluginfolders", "variable=pr", "--unique-output", "false"])
+    output_str = capsys.readouterr().out
+    match = re.search(pattern, output_str)
+    if match:
+        folder_path = match.group(1)
+    assert str(freva.history()[0]["id"]) not in os.path.basename(
+        os.path.normpath(folder_path)
+    )
+
 
 def test_killed_jobs_set_to_broken():
     import freva
 
     proc = mp.Process(
         target=freva.run_plugin,
         args=("dummyplugin",),
```

### Comparing `freva-2303.0.0/src/evaluation_system/tests/plugin_manager_test.py` & `freva-2307.0.0/src/evaluation_system/tests/plugin_manager_test.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/plugin_test.py` & `freva-2307.0.0/src/evaluation_system/tests/plugin_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -570,15 +570,15 @@
     command = dummy_plugin.compose_command(
         config_dict={"the_number": 22}, caption="This is the caption"
     )
     assert similar_string(
         " ".join(command),
         (
             "dummpyplugin the_number=22 something=test other=1.4 variable=tas "
-            "--caption 'This is the caption' --unique_output True"
+            "--caption 'This is the caption' --unique-output true"
         ),
     )
 
 
 @mock.patch("os.getpid", lambda: 12345)
 def test_append_unique_output():
     from evaluation_system.api.parameters import (
```

### Comparing `freva-2303.0.0/src/evaluation_system/tests/solr_core_test.py` & `freva-2307.0.0/src/evaluation_system/tests/solr_core_test.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/solr_test.py` & `freva-2307.0.0/src/evaluation_system/tests/solr_test.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/user_test.py` & `freva-2307.0.0/src/evaluation_system/tests/user_test.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/utils_test.py` & `freva-2307.0.0/src/evaluation_system/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/workload_manager/test_local.py` & `freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_local.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/workload_manager/test_lsf.py` & `freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_lsf.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/workload_manager/test_oar.py` & `freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_oar.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/workload_manager/test_pbs.py` & `freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_pbs.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/workload_manager/test_sge.py` & `freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_sge.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/evaluation_system/tests/workload_manager/test_slurm.py` & `freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_slurm.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/freva/_esgf.py` & `freva-2307.0.0/src/freva/_esgf.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/freva/_history.py` & `freva-2307.0.0/src/freva/_history.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/freva/_plugin.py` & `freva-2307.0.0/src/freva/_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,15 +218,15 @@
     scheduled_id:
         Run a scheduled job from database
     dry_run:
         Perform no computation. Useful for development.
     batchmode:
         Create a Batch job and submit it to the scheduling system.
     unique_output:
-        Append a Freva run id to every output folder
+        Append a Freva run id to the output/cache folder(s).
     return_result:
         Return the plugin result, this can be useful for pipelining.
     repo_version:
         show the version number from the repository.
     tag:
        Use git commit hash to specify a specific versrion of this tool.
```

### Comparing `freva-2303.0.0/src/freva/_user_data.py` & `freva-2307.0.0/src/freva/_user_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,24 +197,23 @@
         """Delete data from the databrowser.
 
         The methods deletes user data from the databrowser.
 
         Parameters
         ----------
 
-         *paths: os.PathLike
+        *paths: os.PathLike
             Filename(s) or Directories that are going to be from  the
             databrowser.
         delete_from_fs: bool, default : False
             Do not only delete the files from the databrowser but also from their
             central location where they have been added to.
 
         Raises
         ------
-
         ValidationError:
             If crawl_dirs do not belong to current user.
 
         Example
         -------
 
         Any data in the central user directory that belongs to the user can
```

### Comparing `freva-2303.0.0/src/freva/cli/__init__.py` & `freva-2307.0.0/src/freva/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/freva/cli/databrowser.py` & `freva-2307.0.0/src/freva/cli/databrowser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 import argparse
 import sys
 from typing import Any, Optional
 
 import lazy_import
 from evaluation_system import __version__
+from evaluation_system.misc import logger
 from .utils import BaseParser, BaseCompleter
 
 freva = lazy_import.lazy_module("freva")
 
 
 class Cli(BaseParser):
     """Class that constructs the Databrowser Argument Parser."""
@@ -47,22 +48,26 @@
         )
         self.parser.add_argument(
             "--attributes",
             default=False,
             action="store_true",
             help=(
                 "Retrieve all possible attributes for the current "
-                "search instead of the files."
+                "search instead of the files. Deprecated, to be removed in "
+                "v2304.0.0"
             ),
         )
         self.parser.add_argument(
             "--all-facets",
             default=False,
             action="store_true",
-            help=("retrieve all facets (attributes & values) instead of " "the files"),
+            help=(
+                "retrieve all facets (attributes & values) instead of "
+                "the files (deprecated, to be removed in v2304.0.0.0)"
+            ),
         )
         self.parser.add_argument(
             "--facet",
             default=None,
             type=str,
             action="append",
             help=("Retrieve values of given facet instead of files"),
@@ -102,21 +107,52 @@
     def run_cmd(
         args: argparse.Namespace,
         other_args: Optional[list[str]] = None,
         **kwargs: Optional[Any],
     ) -> None:
         """Call the databrowser command and print the results."""
         facets: dict[str, Any] = BaseCompleter.arg_to_dict(args.facets, append=True)
+        if args.relevant_only:
+            logger.warning(
+                "The relevant-only flag will be made deprecated",
+            )
+        if args.attributes:
+            logger.warning(
+                "The attributes flag will be made deprecated",
+            )
         facet_limit = kwargs.pop("facet_limit")
-        _ = kwargs.pop("facets")
+        for key in (
+            "facets",
+            "all_facets",
+            "count",
+            "attributes",
+            "relevant_only",
+            "batch_size",
+        ):
+            _ = kwargs.pop(key, "")
         for key, values in facets.items():
             if len(values) == 1:
                 facets[key] = values[0]
         merged_args: dict[str, Any] = {**kwargs, **facets}
-        out = freva.databrowser(**merged_args)
+        if args.all_facets:
+            logger.warning(
+                "The all-facets flag will be made deprecated use"
+                "user --facet '*' or --facet all instead"
+            )
+            args.facet = "*"
+        if args.count:
+            _ = merged_args.pop("facet", "")
+            out = freva.count_values(facet=args.facet, **merged_args)
+        elif args.facet:
+            _ = merged_args.pop("facet", "")
+            out = freva.facet_search(facet=args.facet, **merged_args)
+        elif args.attributes:
+            out = freva.databrowser(attributes=True, **merged_args)
+        else:
+            out = freva.databrowser(batch_size=args.batch_size, **merged_args)
         # flush stderr in case we have something pending
         sys.stderr.flush()
         if isinstance(out, dict):
             # We have facet values as return values
             for att, values in out.items():
                 facet_limit = facet_limit or len(values) + 1
                 try:
```

### Comparing `freva-2303.0.0/src/freva/cli/esgf.py` & `freva-2307.0.0/src/freva/cli/esgf.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/freva/cli/history.py` & `freva-2307.0.0/src/freva/cli/history.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/freva/cli/plugin.py` & `freva-2307.0.0/src/freva/cli/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,18 +87,19 @@
         self.parser.add_argument(
             "--batchmode",
             help="Create a Batch job and submit it to the scheduling system.",
             default=False,
             action="store_true",
         )
         self.parser.add_argument(
+            "--unique-output",
             "--unique_output",
-            help="Append a freva run id to every output folder",
-            default=True,
-            type=bool,
+            choices=["true", "false", "True", "False"],
+            help="Append a Freva run id to the output/cache folder(s).",
+            default="true",
         )
         self.parser.add_argument(
             "--debug",
             "-v",
             "-d",
             "--verbose",
             help="Use verbose output.",
@@ -124,23 +125,27 @@
 
     @staticmethod
     def run_cmd(
         args: argparse.Namespace,
         other_args: Optional[list[str]] = None,
         **kwargs: Any,
     ) -> None:
-        """Call the databrowser command and print the results."""
+        """Call the plugin command and print the results."""
         tool_name = kwargs.pop("tool-name")
         if kwargs.pop("list_tools") or not tool_name:
             print(freva.get_tools_list())
             return
         options: dict[str, Any] = BaseCompleter.arg_to_dict(other_args or [])
         for key, val in options.items():
             if len(val) == 1:
                 options[key] = val[0]
+        if kwargs["unique_output"].lower() == "true":
+            kwargs["unique_output"] = True
+        else:
+            kwargs["unique_output"] = False
         tool_args = {**kwargs, **options}
         try:
             if tool_args.pop("doc"):
                 print(freva.plugin_doc(tool_name))
                 return
             value, out = freva.run_plugin(tool_name or "", **tool_args)
         except (
```

### Comparing `freva-2303.0.0/src/freva/cli/user_data.py` & `freva-2307.0.0/src/freva/cli/user_data.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/freva/cli/utils.py` & `freva-2307.0.0/src/freva/cli/utils.py`

 * *Files identical despite different names*

### Comparing `freva-2303.0.0/src/freva.egg-info/PKG-INFO` & `freva-2307.0.0/src/freva.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freva
-Version: 2303.0.0
+Version: 2307.0.0
 Summary: Free Evaluation and Analysis Framework (Freva) 
 Author: German Climate Computing Centre (DKRZ)
 Maintainer: Climate Informatics and Technology (CLINT)
 License: BSD-3-Clause
 Project-URL: Documentation, https://freva.gitlab-pages.dkrz.de/evaluation_system/sphinx_docs/index.html
 Project-URL: Release notes, https://freva.gitlab-pages.dkrz.de/evaluation_system/sphinx_docs/whats-new.html
 Project-URL: Issues, https://gitlab.dkrz.de/freva/evaluation_system/-/issues
@@ -28,15 +28,15 @@
 Provides-Extra: test
 License-File: LICENSE.md
 
 # Free Evaluation System Framework
 
 [![PyPI version](https://badge.fury.io/py/freva.svg)](https://badge.fury.io/py/freva)
 [![Update](https://anaconda.org/conda-forge/freva/badges/latest_release_date.svg)](https://github.com/FREVA-CLINT/freva)
-[![Conda](https://anaconda.org/conda-forge/freva/badges/installer/conda.svg)](https://anaconda.org/conda-forge/freva)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/freva/badges/version.svg)](https://anaconda.org/conda-forge/freva)
 [![Docs](https://img.shields.io/badge/Freva-Docs-green.svg)](https://freva-clint.github.io/freva)
 [![codecov](https://codecov.io/gh/FREVA-CLINT/freva/branch/main/graph/badge.svg)](https://codecov.io/gh/FREVA-CLINT/freva)
 [![Pipeline](https://github.com/FREVA-CLINT/freva/actions/workflows/ci_job.yml/badge.svg)](https://github.com/FREVA-CLINT/freva/actions)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/FREVA-CLINT/freva/main?labpath=Readme.ipynb)
 [![BSD](https://anaconda.org/conda-forge/freva/badges/license.svg)](https://github.com/FREVA-CLINT/freva)
 
 <img src="docs/source/_static/freva_flowchart-new.jpg" alt="Freva" width="400"/>
```

### Comparing `freva-2303.0.0/src/freva.egg-info/SOURCES.txt` & `freva-2307.0.0/src/freva.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,19 +27,14 @@
 src/evaluation_system/api/workload_manager/local.py
 src/evaluation_system/api/workload_manager/lsf.py
 src/evaluation_system/api/workload_manager/moab.py
 src/evaluation_system/api/workload_manager/oar.py
 src/evaluation_system/api/workload_manager/pbs.py
 src/evaluation_system/api/workload_manager/sge.py
 src/evaluation_system/api/workload_manager/slurm.py
-src/evaluation_system/external/__init__.py
-src/evaluation_system/external/basePlugin/Logger.py
-src/evaluation_system/external/basePlugin/NCLhelper.py
-src/evaluation_system/external/basePlugin/ShellScriptHelper.py
-src/evaluation_system/external/basePlugin/__init__.py
 src/evaluation_system/fuse/__init__.py
 src/evaluation_system/fuse/esgf2fs.py
 src/evaluation_system/fuse/esgf2solr_crawl.py
 src/evaluation_system/fuse/esgf_crawl_config.py
 src/evaluation_system/misc/__init__.py
 src/evaluation_system/misc/config.py
 src/evaluation_system/misc/exceptions.py
@@ -77,14 +72,15 @@
 src/evaluation_system/tests/plugin_test.py
 src/evaluation_system/tests/solr_core_test.py
 src/evaluation_system/tests/solr_test.py
 src/evaluation_system/tests/user_test.py
 src/evaluation_system/tests/utils_test.py
 src/evaluation_system/tests/mocks/__init__.py
 src/evaluation_system/tests/mocks/dummy.py
+src/evaluation_system/tests/mocks/dummyfolder.py
 src/evaluation_system/tests/mocks/result_tags.py
 src/evaluation_system/tests/workload_manager/__init__.py
 src/evaluation_system/tests/workload_manager/test_core.py
 src/evaluation_system/tests/workload_manager/test_local.py
 src/evaluation_system/tests/workload_manager/test_lsf.py
 src/evaluation_system/tests/workload_manager/test_oar.py
 src/evaluation_system/tests/workload_manager/test_pbs.py
```

### Comparing `freva-2303.0.0/src/freva.egg-info/requires.txt` & `freva-2307.0.0/src/freva.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 xarray
 
 [docs]
 bash_kernel
 cartopy
 cftime
 cf_xarray
+furo
 ipython
 ipykernel
 nbsphinx
 pint
 pint-xarray
 recommonmark
 sphinx
 sphinxcontrib_github_alt
 sphinx-execute-code-python3
-sphinx-rtd-theme
 xarray
 h5netcdf
 
 [test]
 allure-pytest
 black
 django-stubs
```

