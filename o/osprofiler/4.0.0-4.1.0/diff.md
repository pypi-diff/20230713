# Comparing `tmp/osprofiler-4.0.0.tar.gz` & `tmp/osprofiler-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osprofiler-4.0.0.tar", last modified: Wed Jun 21 11:15:26 2023, max compression
+gzip compressed data, was "osprofiler-4.1.0.tar", last modified: Thu Jul 13 15:46:48 2023, max compression
```

## Comparing `osprofiler-4.0.0.tar` & `osprofiler-4.1.0.tar`

### file list

```diff
@@ -1,150 +1,152 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.224339 osprofiler-4.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-06-21 11:14:46.000000 osprofiler-4.0.0/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-06-21 11:14:46.000000 osprofiler-4.0.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2023-06-21 11:14:46.000000 osprofiler-4.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3504 2023-06-21 11:15:26.000000 osprofiler-4.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      543 2023-06-21 11:14:46.000000 osprofiler-4.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14425 2023-06-21 11:15:26.000000 osprofiler-4.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10273 2023-06-21 11:14:46.000000 osprofiler-4.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2424 2023-06-21 11:15:26.224339 osprofiler-4.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1279 2023-06-21 11:14:46.000000 osprofiler-4.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-06-21 11:14:46.000000 osprofiler-4.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.204339 osprofiler-4.0.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3499 2023-06-21 11:14:46.000000 osprofiler-4.0.0/devstack/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.204339 osprofiler-4.0.0/devstack/lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4925 2023-06-21 11:14:46.000000 osprofiler-4.0.0/devstack/lib/osprofiler
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      837 2023-06-21 11:14:46.000000 osprofiler-4.0.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2023-06-21 11:14:46.000000 osprofiler-4.0.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.204339 osprofiler-4.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.204339 osprofiler-4.0.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6778 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/source/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4180 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      738 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.208339 osprofiler-4.0.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7211 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/source/user/api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1215 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/source/user/background.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2890 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/source/user/collectors.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/source/user/history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5293 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/source/user/integration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      533 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/source/user/similar_projects.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.208339 osprofiler-4.0.0/doc/specs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/specs/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.208339 osprofiler-4.0.0/doc/specs/implemented/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/specs/implemented/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2403 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/specs/implemented/make_paste_ini_config_optional.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2656 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/specs/implemented/multi_backend_support.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.208339 osprofiler-4.0.0/doc/specs/in-progress/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/specs/in-progress/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1451 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/specs/in-progress/better_devstack_integration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1601 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/specs/in-progress/integration_testing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2397 2023-06-21 11:14:46.000000 osprofiler-4.0.0/doc/specs/template.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      469 2023-06-21 11:14:46.000000 osprofiler-4.0.0/lower-constraints.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.212339 osprofiler-4.0.0/osprofiler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5826 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.212339 osprofiler-4.0.0/osprofiler/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1731 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/cmd/cliutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7734 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/cmd/commands.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2950 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/cmd/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13940 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/cmd/template.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.216339 osprofiler-4.0.0/osprofiler/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10891 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/drivers/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6810 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/drivers/elasticsearch_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5850 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/drivers/jaeger.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9699 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/drivers/loginsight.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7412 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/drivers/messaging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4377 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/drivers/mongodb.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6841 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/drivers/otlp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8270 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/drivers/redis_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5617 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/drivers/sqlalchemy_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      941 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/exc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.216339 osprofiler-4.0.0/osprofiler/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13136 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/hacking/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1474 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/initializer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2635 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8572 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16071 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/profiler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/sqlalchemy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.216339 osprofiler-4.0.0/osprofiler/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.216339 osprofiler-4.0.0/osprofiler/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/functional/config.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5268 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/functional/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1008 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/test.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.216339 osprofiler-4.0.0/osprofiler/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.216339 osprofiler-4.0.0/osprofiler/tests/unit/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6136 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/cmd/test_shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.216339 osprofiler-4.0.0/osprofiler/tests/unit/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/doc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4501 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/doc/test_specs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.220339 osprofiler-4.0.0/osprofiler/tests/unit/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4137 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4405 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_elasticsearch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3788 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_jaeger.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12953 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_loginsight.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2488 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_messaging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13596 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_mongodb.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2736 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_otlp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14002 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_redis_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1644 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/test_initializer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/test_notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2896 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/test_opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21169 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/test_profiler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6550 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/test_sqlalchemy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5306 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11622 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/tests/unit/test_web.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4519 2023-06-21 11:14:46.000000 osprofiler-4.0.0/osprofiler/web.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.212339 osprofiler-4.0.0/osprofiler.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2424 2023-06-21 11:15:26.000000 osprofiler-4.0.0/osprofiler.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3905 2023-06-21 11:15:26.000000 osprofiler-4.0.0/osprofiler.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-21 11:15:26.000000 osprofiler-4.0.0/osprofiler.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-06-21 11:15:26.000000 osprofiler-4.0.0/osprofiler.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-21 11:15:26.000000 osprofiler-4.0.0/osprofiler.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-06-21 11:15:26.000000 osprofiler-4.0.0/osprofiler.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2023-06-21 11:15:26.000000 osprofiler-4.0.0/osprofiler.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-06-21 11:15:26.000000 osprofiler-4.0.0/osprofiler.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.220339 osprofiler-4.0.0/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1911 2023-06-21 11:14:46.000000 osprofiler-4.0.0/playbooks/osprofiler-post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.200339 osprofiler-4.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.220339 osprofiler-4.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/notes/add-reno-996dd44974d53238.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/notes/drop-jaeger-container-when-unstacking-e8fcdc036f80158a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/notes/jaeger-add-process-tags-79d5f5d7a0b049ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/notes/jaeger-service-name-prefix-72878a930f700878.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/notes/otlp-driver-cb932038ad580ac2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/notes/redis-improvement-d4c91683fc89f570.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/notes/remove-strict-redis-9eb43d30c9c1fc43.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.220339 osprofiler-4.0.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.220339 osprofiler-4.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.224339 osprofiler-4.0.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9011 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-06-21 11:14:46.000000 osprofiler-4.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2023-06-21 11:14:46.000000 osprofiler-4.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2023-06-21 11:15:26.224339 osprofiler-4.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2023-06-21 11:14:46.000000 osprofiler-4.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      584 2023-06-21 11:14:46.000000 osprofiler-4.0.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-21 11:15:26.224339 osprofiler-4.0.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2023-06-21 11:14:46.000000 osprofiler-4.0.0/tools/lint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1615 2023-06-21 11:14:46.000000 osprofiler-4.0.0/tools/patch_tox_venv.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2588 2023-06-21 11:14:46.000000 osprofiler-4.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.871940 osprofiler-4.1.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-07-13 15:46:21.000000 osprofiler-4.1.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-07-13 15:46:21.000000 osprofiler-4.1.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2023-07-13 15:46:21.000000 osprofiler-4.1.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3504 2023-07-13 15:46:48.000000 osprofiler-4.1.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      543 2023-07-13 15:46:21.000000 osprofiler-4.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14479 2023-07-13 15:46:48.000000 osprofiler-4.1.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10273 2023-07-13 15:46:21.000000 osprofiler-4.1.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2424 2023-07-13 15:46:48.875940 osprofiler-4.1.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1279 2023-07-13 15:46:21.000000 osprofiler-4.1.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-07-13 15:46:21.000000 osprofiler-4.1.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.843941 osprofiler-4.1.0/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3499 2023-07-13 15:46:21.000000 osprofiler-4.1.0/devstack/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.843941 osprofiler-4.1.0/devstack/lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4925 2023-07-13 15:46:21.000000 osprofiler-4.1.0/devstack/lib/osprofiler
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      837 2023-07-13 15:46:21.000000 osprofiler-4.1.0/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2023-07-13 15:46:21.000000 osprofiler-4.1.0/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.843941 osprofiler-4.1.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2023-07-13 15:46:21.000000 osprofiler-4.1.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.843941 osprofiler-4.1.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6778 2023-07-13 15:46:21.000000 osprofiler-4.1.0/doc/source/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4180 2023-07-13 15:46:21.000000 osprofiler-4.1.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      738 2023-07-13 15:46:21.000000 osprofiler-4.1.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.847941 osprofiler-4.1.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7211 2023-07-13 15:46:21.000000 osprofiler-4.1.0/doc/source/user/api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1215 2023-07-13 15:46:21.000000 osprofiler-4.1.0/doc/source/user/background.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2890 2023-07-13 15:46:21.000000 osprofiler-4.1.0/doc/source/user/collectors.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-07-13 15:46:21.000000 osprofiler-4.1.0/doc/source/user/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2023-07-13 15:46:21.000000 osprofiler-4.1.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5550 2023-07-13 15:46:21.000000 osprofiler-4.1.0/doc/source/user/integration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      533 2023-07-13 15:46:21.000000 osprofiler-4.1.0/doc/source/user/similar_projects.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.847941 osprofiler-4.1.0/doc/specs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2023-07-13 15:46:21.000000 osprofiler-4.1.0/doc/specs/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.847941 osprofiler-4.1.0/doc/specs/implemented/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2023-07-13 15:46:21.000000 osprofiler-4.1.0/doc/specs/implemented/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2403 2023-07-13 15:46:21.000000 osprofiler-4.1.0/doc/specs/implemented/make_paste_ini_config_optional.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2656 2023-07-13 15:46:21.000000 osprofiler-4.1.0/doc/specs/implemented/multi_backend_support.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.851940 osprofiler-4.1.0/doc/specs/in-progress/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-07-13 15:46:21.000000 osprofiler-4.1.0/doc/specs/in-progress/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1451 2023-07-13 15:46:21.000000 osprofiler-4.1.0/doc/specs/in-progress/better_devstack_integration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1601 2023-07-13 15:46:21.000000 osprofiler-4.1.0/doc/specs/in-progress/integration_testing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2397 2023-07-13 15:46:21.000000 osprofiler-4.1.0/doc/specs/template.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      469 2023-07-13 15:46:21.000000 osprofiler-4.1.0/lower-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.851940 osprofiler-4.1.0/osprofiler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5826 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.855940 osprofiler-4.1.0/osprofiler/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1731 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/cmd/cliutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7734 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/cmd/commands.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2950 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/cmd/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13940 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/cmd/template.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.859940 osprofiler-4.1.0/osprofiler/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10891 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/drivers/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6810 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/drivers/elasticsearch_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5850 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/drivers/jaeger.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9699 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/drivers/loginsight.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7412 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/drivers/messaging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4377 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/drivers/mongodb.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7625 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/drivers/otlp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8270 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/drivers/redis_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5617 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/drivers/sqlalchemy_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      941 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/exc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.859940 osprofiler-4.1.0/osprofiler/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13136 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1569 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/initializer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2635 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8884 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16071 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/profiler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2194 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/requests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/sqlalchemy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.859940 osprofiler-4.1.0/osprofiler/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.859940 osprofiler-4.1.0/osprofiler/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/functional/config.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5268 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/functional/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1008 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/test.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.863940 osprofiler-4.1.0/osprofiler/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.863940 osprofiler-4.1.0/osprofiler/tests/unit/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6136 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/cmd/test_shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.863940 osprofiler-4.1.0/osprofiler/tests/unit/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/doc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4501 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/doc/test_specs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.867940 osprofiler-4.1.0/osprofiler/tests/unit/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4137 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/drivers/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4405 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/drivers/test_elasticsearch.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3788 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/drivers/test_jaeger.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12953 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/drivers/test_loginsight.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2488 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/drivers/test_messaging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13596 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/drivers/test_mongodb.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2736 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/drivers/test_otlp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14002 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/drivers/test_redis_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1644 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/test_initializer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/test_notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2896 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/test_opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21169 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/test_profiler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6550 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/test_sqlalchemy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5306 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11622 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/tests/unit/test_web.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4519 2023-07-13 15:46:21.000000 osprofiler-4.1.0/osprofiler/web.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.855940 osprofiler-4.1.0/osprofiler.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2424 2023-07-13 15:46:48.000000 osprofiler-4.1.0/osprofiler.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3992 2023-07-13 15:46:48.000000 osprofiler-4.1.0/osprofiler.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-13 15:46:48.000000 osprofiler-4.1.0/osprofiler.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-07-13 15:46:48.000000 osprofiler-4.1.0/osprofiler.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-13 15:46:48.000000 osprofiler-4.1.0/osprofiler.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-07-13 15:46:48.000000 osprofiler-4.1.0/osprofiler.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2023-07-13 15:46:48.000000 osprofiler-4.1.0/osprofiler.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-07-13 15:46:48.000000 osprofiler-4.1.0/osprofiler.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.867940 osprofiler-4.1.0/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1911 2023-07-13 15:46:21.000000 osprofiler-4.1.0/playbooks/osprofiler-post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.839941 osprofiler-4.1.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.871940 osprofiler-4.1.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/notes/add-reno-996dd44974d53238.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/notes/add-requests-profiling-761e09f243d36966.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/notes/drop-jaeger-container-when-unstacking-e8fcdc036f80158a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/notes/jaeger-add-process-tags-79d5f5d7a0b049ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/notes/jaeger-service-name-prefix-72878a930f700878.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/notes/otlp-driver-cb932038ad580ac2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/notes/redis-improvement-d4c91683fc89f570.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/notes/remove-strict-redis-9eb43d30c9c1fc43.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.871940 osprofiler-4.1.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.871940 osprofiler-4.1.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.871940 osprofiler-4.1.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9011 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-07-13 15:46:21.000000 osprofiler-4.1.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2023-07-13 15:46:21.000000 osprofiler-4.1.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2023-07-13 15:46:48.875940 osprofiler-4.1.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2023-07-13 15:46:21.000000 osprofiler-4.1.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      584 2023-07-13 15:46:21.000000 osprofiler-4.1.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-13 15:46:48.871940 osprofiler-4.1.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2023-07-13 15:46:21.000000 osprofiler-4.1.0/tools/lint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1615 2023-07-13 15:46:21.000000 osprofiler-4.1.0/tools/patch_tox_venv.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2588 2023-07-13 15:46:21.000000 osprofiler-4.1.0/tox.ini
```

### Comparing `osprofiler-4.0.0/.pre-commit-config.yaml` & `osprofiler-4.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/.zuul.yaml` & `osprofiler-4.1.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/AUTHORS` & `osprofiler-4.1.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/CONTRIBUTING.rst` & `osprofiler-4.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/ChangeLog` & `osprofiler-4.1.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+4.1.0
+-----
+
+* profiler: add python requests profile
+
 4.0.0
 -----
 
 * add support of otlp exporter
 * devstack: remove jaeger container on unstack
 * [profiler] hmac\_key should be secret
 * jaeger: introduce process tags' option for tracer
```

### Comparing `osprofiler-4.0.0/LICENSE` & `osprofiler-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/PKG-INFO` & `osprofiler-4.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osprofiler
-Version: 4.0.0
+Version: 4.1.0
 Summary: OpenStack Profiler Library
 Home-page: https://docs.openstack.org/osprofiler/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===================================================
          OSProfiler -- Library for cross-project profiling
```

### Comparing `osprofiler-4.0.0/README.rst` & `osprofiler-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/devstack/README.rst` & `osprofiler-4.1.0/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/devstack/lib/osprofiler` & `osprofiler-4.1.0/devstack/lib/osprofiler`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/devstack/plugin.sh` & `osprofiler-4.1.0/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/doc/source/Makefile` & `osprofiler-4.1.0/doc/source/Makefile`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/doc/source/conf.py` & `osprofiler-4.1.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/doc/source/index.rst` & `osprofiler-4.1.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/doc/source/user/api.rst` & `osprofiler-4.1.0/doc/source/user/api.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/doc/source/user/background.rst` & `osprofiler-4.1.0/doc/source/user/background.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/doc/source/user/collectors.rst` & `osprofiler-4.1.0/doc/source/user/collectors.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/doc/source/user/index.rst` & `osprofiler-4.1.0/doc/source/user/index.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/doc/source/user/integration.rst` & `osprofiler-4.1.0/doc/source/user/integration.rst`

 * *Files 3% similar despite different names*

```diff
@@ -83,14 +83,18 @@
   processed. This ensures that trace info that is sent in that
   does **not** pass the HMAC validation will be discarded. **NOTE:** The
   application of many possible *validation* keys makes it possible to
   roll out a key upgrade in a non-impactful manner (by adding a key into
   the list and rolling out that change and then removing the older key at
   some time in the future).
 
+  * Optionally you can enable client tracing using `requests`_,
+    Currently only supported by OTLP driver, this will add client call
+    tracing. see `profiler/trace_requests`'s option.
+
 * RPC API
 
   RPC calls are used for interaction between services of one project.
   It's well known that projects are using `oslo.messaging`_ to deal with
   RPC. It's very good, because projects deal with RPC in similar way.
 
   So there are 2 required changes:
@@ -128,7 +132,8 @@
 
 .. _CONF: https://docs.openstack.org/oslo.config/latest/
 .. _HMAC: https://en.wikipedia.org/wiki/Hash-based_message_authentication_code
 .. _OpenStack: https://www.openstack.org/
 .. _Ceilometer: https://wiki.openstack.org/wiki/Ceilometer
 .. _oslo.messaging: https://pypi.org/project/oslo.messaging
 .. _OSprofiler WSGI middleware: https://github.com/openstack/osprofiler/blob/master/osprofiler/web.py
+.. _requests: https://docs.python-requests.org/en/latest/index.html
```

### Comparing `osprofiler-4.0.0/doc/source/user/similar_projects.rst` & `osprofiler-4.1.0/doc/source/user/similar_projects.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/doc/specs/implemented/make_paste_ini_config_optional.rst` & `osprofiler-4.1.0/doc/specs/implemented/make_paste_ini_config_optional.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/doc/specs/implemented/multi_backend_support.rst` & `osprofiler-4.1.0/doc/specs/implemented/multi_backend_support.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/doc/specs/in-progress/better_devstack_integration.rst` & `osprofiler-4.1.0/doc/specs/in-progress/better_devstack_integration.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/doc/specs/in-progress/integration_testing.rst` & `osprofiler-4.1.0/doc/specs/in-progress/integration_testing.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/doc/specs/template.rst` & `osprofiler-4.1.0/doc/specs/template.rst`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/__init__.py` & `osprofiler-4.1.0/osprofiler/__init__.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/_utils.py` & `osprofiler-4.1.0/osprofiler/_utils.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/cmd/cliutils.py` & `osprofiler-4.1.0/osprofiler/cmd/cliutils.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/cmd/commands.py` & `osprofiler-4.1.0/osprofiler/cmd/commands.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/cmd/shell.py` & `osprofiler-4.1.0/osprofiler/cmd/shell.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/cmd/template.html` & `osprofiler-4.1.0/osprofiler/cmd/template.html`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/drivers/base.py` & `osprofiler-4.1.0/osprofiler/drivers/base.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/drivers/elasticsearch_driver.py` & `osprofiler-4.1.0/osprofiler/drivers/elasticsearch_driver.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/drivers/jaeger.py` & `osprofiler-4.1.0/osprofiler/drivers/jaeger.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/drivers/loginsight.py` & `osprofiler-4.1.0/osprofiler/drivers/loginsight.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/drivers/messaging.py` & `osprofiler-4.1.0/osprofiler/drivers/messaging.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/drivers/mongodb.py` & `osprofiler-4.1.0/osprofiler/drivers/mongodb.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/drivers/otlp.py` & `osprofiler-4.1.0/osprofiler/drivers/otlp.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,26 +77,29 @@
     @classmethod
     def get_name(cls):
         return "otlp"
 
     def _kind(self, name):
         if "wsgi" in name:
             return self.trace_api.SpanKind.SERVER
-        elif ("db" in name or "http_client" in name or "api" in name):
+        elif ("db" in name or "http" in name or "api" in name):
             return self.trace_api.SpanKind.CLIENT
         return self.trace_api.SpanKind.INTERNAL
 
     def _name(self, payload):
         info = payload["info"]
         if info.get("request"):
-            return "{}_{}".format(
+            return "WSGI_{}_{}".format(
                 info["request"]["method"], info["request"]["path"])
         elif info.get("db"):
             return "SQL_{}".format(
                 info["db"]["statement"].split(' ', 1)[0].upper())
+        elif info.get("requests"):
+            return "REQUESTS_{}_{}".format(
+                info["requests"]["method"], info["requests"]["hostname"])
         return payload["name"].rstrip("-start")
 
     def notify(self, payload):
         if payload["name"].endswith("start"):
             parent = self.trace_api.SpanContext(
                 trace_id=utils.uuid_to_int128(payload["base_id"]),
                 span_id=utils.shorten_id(payload["parent_id"]),
@@ -126,14 +129,18 @@
             span = self.spans.pop()
 
             # Store result of db call and function call
             for call in ("db", "function"):
                 if payload.get("info", {}).get(call):
                     span.set_attribute(
                         "result", payload["info"][call]["result"])
+            # Store result of requests
+            if payload.get("info", {}).get("requests"):
+                span.set_attribute(
+                    "status_code", payload["info"]["requests"]["status_code"])
             # Span error tag and log
             if payload["info"].get("etype"):
                 span.set_attribute("error", True)
                 span.add_event("log", {
                     "error.kind": payload["info"]["etype"],
                     "message": payload["info"]["message"]})
             span.end()
@@ -164,14 +171,22 @@
             tags["db.params"] = jsonutils.dumps(info["db"]["params"])
         elif info.get("request"):
             # WSGI call
             tags["http.path"] = info["request"]["path"]
             tags["http.query"] = info["request"]["query"]
             tags["http.method"] = info["request"]["method"]
             tags["http.scheme"] = info["request"]["scheme"]
+        elif info.get("requests"):
+            # requests call
+            tags["http.path"] = info["requests"]["path"]
+            tags["http.query"] = info["requests"]["query"]
+            tags["http.method"] = info["requests"]["method"]
+            tags["http.scheme"] = info["requests"]["scheme"]
+            tags["http.hostname"] = info["requests"]["hostname"]
+            tags["http.port"] = info["requests"]["port"]
         elif info.get("function"):
             # RPC, function calls
             if "args" in info["function"]:
                 tags["args"] = info["function"]["args"]
             if "kwargs" in info["function"]:
                 tags["kwargs"] = info["function"]["kwargs"]
             tags["name"] = info["function"]["name"]
```

### Comparing `osprofiler-4.0.0/osprofiler/drivers/redis_driver.py` & `osprofiler-4.1.0/osprofiler/drivers/redis_driver.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/drivers/sqlalchemy_driver.py` & `osprofiler-4.1.0/osprofiler/drivers/sqlalchemy_driver.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/exc.py` & `osprofiler-4.1.0/osprofiler/exc.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/hacking/checks.py` & `osprofiler-4.1.0/osprofiler/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/initializer.py` & `osprofiler-4.1.0/osprofiler/initializer.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from osprofiler import notifier
+from osprofiler import requests
 from osprofiler import web
 
 
 def init_from_conf(conf, context, project, service, host, **kwargs):
     """Initialize notifier from service configuration
 
     :param conf: service configuration
@@ -35,7 +36,9 @@
         project=project,
         service=service,
         host=host,
         conf=conf,
         **kwargs)
     notifier.set(_notifier)
     web.enable(conf.profiler.hmac_keys)
+    if conf.profiler.trace_requests:
+        requests.enable()
```

### Comparing `osprofiler-4.0.0/osprofiler/notifier.py` & `osprofiler-4.1.0/osprofiler/notifier.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/opts.py` & `osprofiler-4.1.0/osprofiler/opts.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,30 @@
 
 * True: Enables SQL requests profiling. Each SQL query will be part of the
   trace and can the be analyzed by how much time was spent for that.
 * False: Disables SQL requests profiling. The spent time is only shown on a
   higher level of operations. Single SQL queries cannot be analyzed this way.
 """)
 
+_trace_requests_opt = cfg.BoolOpt(
+    "trace_requests",
+    default=False,
+    help="""
+Enable python requests package profiling.
+
+Supported drivers: jaeger+otlp
+
+Default value is False.
+
+Possible values:
+
+* True: Enables requests profiling.
+* False: Disables requests profiling.
+""")
+
 _hmac_keys_opt = cfg.StrOpt(
     "hmac_keys",
     default="SECRET_KEY",
     secret=True,
     help="""
 Secret key(s) to use for encrypting context data for performance profiling.
 
@@ -155,14 +171,15 @@
 * True: Enable filter traces that contain error/exception.
 * False: Disable the filter.
 """)
 
 _PROFILER_OPTS = [
     _enabled_opt,
     _trace_sqlalchemy_opt,
+    _trace_requests_opt,
     _hmac_keys_opt,
     _connection_string_opt,
     _es_doc_type_opt,
     _es_scroll_time_opt,
     _es_scroll_size_opt,
     _socket_timeout_opt,
     _sentinel_service_name_opt,
```

### Comparing `osprofiler-4.0.0/osprofiler/profiler.py` & `osprofiler-4.1.0/osprofiler/profiler.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/sqlalchemy.py` & `osprofiler-4.1.0/osprofiler/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/tests/functional/test_driver.py` & `osprofiler-4.1.0/osprofiler/tests/functional/test_driver.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/tests/test.py` & `osprofiler-4.1.0/osprofiler/tests/test.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/tests/unit/cmd/test_shell.py` & `osprofiler-4.1.0/osprofiler/tests/unit/cmd/test_shell.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/tests/unit/doc/test_specs.py` & `osprofiler-4.1.0/osprofiler/tests/unit/doc/test_specs.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_base.py` & `osprofiler-4.1.0/osprofiler/tests/unit/drivers/test_base.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_elasticsearch.py` & `osprofiler-4.1.0/osprofiler/tests/unit/drivers/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_jaeger.py` & `osprofiler-4.1.0/osprofiler/tests/unit/drivers/test_jaeger.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_loginsight.py` & `osprofiler-4.1.0/osprofiler/tests/unit/drivers/test_loginsight.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_messaging.py` & `osprofiler-4.1.0/osprofiler/tests/unit/drivers/test_messaging.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_mongodb.py` & `osprofiler-4.1.0/osprofiler/tests/unit/drivers/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_otlp.py` & `osprofiler-4.1.0/osprofiler/tests/unit/drivers/test_otlp.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/tests/unit/drivers/test_redis_driver.py` & `osprofiler-4.1.0/osprofiler/tests/unit/drivers/test_redis_driver.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/tests/unit/test_initializer.py` & `osprofiler-4.1.0/osprofiler/tests/unit/test_initializer.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/tests/unit/test_notifier.py` & `osprofiler-4.1.0/osprofiler/tests/unit/test_notifier.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/tests/unit/test_opts.py` & `osprofiler-4.1.0/osprofiler/tests/unit/test_opts.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/tests/unit/test_profiler.py` & `osprofiler-4.1.0/osprofiler/tests/unit/test_profiler.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/tests/unit/test_sqlalchemy.py` & `osprofiler-4.1.0/osprofiler/tests/unit/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/tests/unit/test_utils.py` & `osprofiler-4.1.0/osprofiler/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/tests/unit/test_web.py` & `osprofiler-4.1.0/osprofiler/tests/unit/test_web.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler/web.py` & `osprofiler-4.1.0/osprofiler/web.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/osprofiler.egg-info/PKG-INFO` & `osprofiler-4.1.0/osprofiler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osprofiler
-Version: 4.0.0
+Version: 4.1.0
 Summary: OpenStack Profiler Library
 Home-page: https://docs.openstack.org/osprofiler/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===================================================
          OSProfiler -- Library for cross-project profiling
```

### Comparing `osprofiler-4.0.0/osprofiler.egg-info/SOURCES.txt` & `osprofiler-4.1.0/osprofiler.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 osprofiler/__init__.py
 osprofiler/_utils.py
 osprofiler/exc.py
 osprofiler/initializer.py
 osprofiler/notifier.py
 osprofiler/opts.py
 osprofiler/profiler.py
+osprofiler/requests.py
 osprofiler/sqlalchemy.py
 osprofiler/web.py
 osprofiler.egg-info/PKG-INFO
 osprofiler.egg-info/SOURCES.txt
 osprofiler.egg-info/dependency_links.txt
 osprofiler.egg-info/entry_points.txt
 osprofiler.egg-info/not-zip-safe
@@ -94,14 +95,15 @@
 osprofiler/tests/unit/drivers/test_loginsight.py
 osprofiler/tests/unit/drivers/test_messaging.py
 osprofiler/tests/unit/drivers/test_mongodb.py
 osprofiler/tests/unit/drivers/test_otlp.py
 osprofiler/tests/unit/drivers/test_redis_driver.py
 playbooks/osprofiler-post.yaml
 releasenotes/notes/add-reno-996dd44974d53238.yaml
+releasenotes/notes/add-requests-profiling-761e09f243d36966.yaml
 releasenotes/notes/drop-jaeger-container-when-unstacking-e8fcdc036f80158a.yaml
 releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
 releasenotes/notes/jaeger-add-process-tags-79d5f5d7a0b049ef.yaml
 releasenotes/notes/jaeger-service-name-prefix-72878a930f700878.yaml
 releasenotes/notes/otlp-driver-cb932038ad580ac2.yaml
 releasenotes/notes/redis-improvement-d4c91683fc89f570.yaml
 releasenotes/notes/remove-strict-redis-9eb43d30c9c1fc43.yaml
```

### Comparing `osprofiler-4.0.0/osprofiler.egg-info/requires.txt` & `osprofiler-4.1.0/osprofiler.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/playbooks/osprofiler-post.yaml` & `osprofiler-4.1.0/playbooks/osprofiler-post.yaml`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/releasenotes/notes/redis-improvement-d4c91683fc89f570.yaml` & `osprofiler-4.1.0/releasenotes/notes/redis-improvement-d4c91683fc89f570.yaml`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/releasenotes/source/conf.py` & `osprofiler-4.1.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/setup.cfg` & `osprofiler-4.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/setup.py` & `osprofiler-4.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/test-requirements.txt` & `osprofiler-4.1.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/tools/lint.py` & `osprofiler-4.1.0/tools/lint.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/tools/patch_tox_venv.py` & `osprofiler-4.1.0/tools/patch_tox_venv.py`

 * *Files identical despite different names*

### Comparing `osprofiler-4.0.0/tox.ini` & `osprofiler-4.1.0/tox.ini`

 * *Files identical despite different names*

