# Comparing `tmp/elasticsearch_curator-8.0.4.tar.gz` & `tmp/elasticsearch_curator-8.0.5.tar.gz`

## Comparing `elasticsearch_curator-8.0.4.tar` & `elasticsearch_curator-8.0.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/_version.py
--rw-r--r--   0        0        0     9608 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/classdef.py
--rw-r--r--   0        0        0    15002 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/config_utils.py
--rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/curator_cli.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/exceptions.py
--rw-r--r--   0        0        0    56567 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/indexlist.py
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/logtools.py
--rw-r--r--   0        0        0    23556 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/repomgrcli.py
--rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/singletons.py
--rw-r--r--   0        0        0    22898 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/snapshotlist.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/__init__.py
--rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/alias.py
--rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/allocation.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/close.py
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/cluster_routing.py
--rw-r--r--   0        0        0     8770 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/cold2frozen.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/create_index.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/delete_indices.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/forcemerge.py
--rw-r--r--   0        0        0     5603 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/index_settings.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/open.py
--rw-r--r--   0        0        0    17631 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/reindex.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/replicas.py
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/rollover.py
--rw-r--r--   0        0        0    24570 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/shrink.py
--rw-r--r--   0        0        0    21632 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/snapshot.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/__init__.py
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/alias.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/allocation.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/close.py
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/delete.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/forcemerge.py
--rw-r--r--   0        0        0     9687 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/object_class.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/open_indices.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/replicas.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/restore.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/rollover.py
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/show.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/shrink.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/snapshot.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/defaults/__init__.py
--rw-r--r--   0        0        0    11383 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/defaults/filter_elements.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/defaults/filtertypes.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/defaults/logging_defaults.py
--rw-r--r--   0        0        0    18383 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/defaults/option_defaults.py
--rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/defaults/settings.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/helpers/__init__.py
--rw-r--r--   0        0        0    23308 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/helpers/date_ops.py
--rw-r--r--   0        0        0    13903 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/helpers/getters.py
--rw-r--r--   0        0        0    15381 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/helpers/testers.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/helpers/utils.py
--rw-r--r--   0        0        0    12704 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/helpers/waiters.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/validators/__init__.py
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/validators/actions.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/validators/filter_functions.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/validators/logconfig.py
--rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/validators/options.py
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/validators/schemacheck.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/.gitignore
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/LICENSE
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/NOTICE
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/README.rst
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/pyproject.toml
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/PKG-INFO
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/_version.py
+-rw-r--r--   0        0        0     9608 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/classdef.py
+-rw-r--r--   0        0        0    15861 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/config_utils.py
+-rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/curator_cli.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/exceptions.py
+-rw-r--r--   0        0        0    57820 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/indexlist.py
+-rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/logtools.py
+-rw-r--r--   0        0        0    23556 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/repomgrcli.py
+-rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/singletons.py
+-rw-r--r--   0        0        0    22898 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/snapshotlist.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/__init__.py
+-rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/alias.py
+-rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/allocation.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/close.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/cluster_routing.py
+-rw-r--r--   0        0        0     8770 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/cold2frozen.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/create_index.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/delete_indices.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/forcemerge.py
+-rw-r--r--   0        0        0     5603 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/index_settings.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/open.py
+-rw-r--r--   0        0        0    17631 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/reindex.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/replicas.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/rollover.py
+-rw-r--r--   0        0        0    24570 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/shrink.py
+-rw-r--r--   0        0        0    21632 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/snapshot.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/__init__.py
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/alias.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/allocation.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/close.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/delete.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/forcemerge.py
+-rw-r--r--   0        0        0     9687 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/object_class.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/open_indices.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/replicas.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/restore.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/rollover.py
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/show.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/shrink.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/snapshot.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/defaults/__init__.py
+-rw-r--r--   0        0        0    11383 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/defaults/filter_elements.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/defaults/filtertypes.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/defaults/logging_defaults.py
+-rw-r--r--   0        0        0    18383 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/defaults/option_defaults.py
+-rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/defaults/settings.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/helpers/__init__.py
+-rw-r--r--   0        0        0    23308 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/helpers/date_ops.py
+-rw-r--r--   0        0        0    13903 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/helpers/getters.py
+-rw-r--r--   0        0        0    15381 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/helpers/testers.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/helpers/utils.py
+-rw-r--r--   0        0        0    12701 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/helpers/waiters.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/validators/__init__.py
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/validators/actions.py
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/validators/filter_functions.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/validators/logconfig.py
+-rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/validators/options.py
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/validators/schemacheck.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/.gitignore
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/LICENSE
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/NOTICE
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/README.rst
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/PKG-INFO
```

### Comparing `elasticsearch_curator-8.0.4/curator/classdef.py` & `elasticsearch_curator-8.0.5/curator/classdef.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/cli.py` & `elasticsearch_curator-8.0.5/curator/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,48 @@
 """Main CLI for Curator"""
 import sys
 import logging
+import pathlib
 import click
 from es_client.builder import ClientArgs, OtherArgs
 from es_client.helpers.utils import get_yaml, check_config, prune_nones, verify_url_schema
 from curator.exceptions import ClientException
 from curator.classdef import ActionsFile
 from curator.config_utils import check_logging_config, set_logging
 from curator.defaults import settings
 from curator.exceptions import NoIndices, NoSnapshots
 from curator.helpers.getters import get_client
 from curator.helpers.testers import ilm_policy_check
 from curator.cli_singletons.utils import get_width
 from curator._version import __version__
 
+def configfile_callback(ctx, param, value):
+    """Callback to validate whether the provided config file exists and is writeable
+
+    :param ctx: The click context
+    :param param: The click parameter object
+    :param value: The value of the parameter
+
+    :type ctx: Click context
+    :type param: Click object
+    :type value: Any
+
+    :returns: Config file path or None
+    :rtype: str
+    """
+    logger = logging.getLogger(__name__)
+    logger.debug('Click ctx = %s', ctx)
+    logger.debug('Click param = %s', param)
+    logger.debug('Click value = %s', value)
+    path = pathlib.Path(value)
+    if path.is_file():
+        return value
+    logger.warning('Config file not found: %s', value)
+    return None
+
 def override_logging(config, loglevel, logfile, logformat):
     """Get logging config and override from command-line options
 
     :param config: The configuration from file
     :param loglevel: The log level
     :param logfile: The log file to write
     :param logformat: Which log format to use
@@ -234,15 +259,15 @@
         except Exception as err:
             exception_handler(action_def, err)
         logger.info('Action ID: %s, "%s" completed.', idx, action_def.action)
     logger.info('All actions completed.')
 
 # pylint: disable=unused-argument, redefined-builtin
 @click.command(context_settings=get_width())
-@click.option('--config', help='Path to configuration file.', type=click.Path(exists=True), default=settings.config_file())
+@click.option('--config', help='Path to configuration file.', type=str, default=settings.config_file(), callback=configfile_callback)
 @click.option('--hosts', help='Elasticsearch URL to connect to', multiple=True)
 @click.option('--cloud_id', help='Shorthand to connect to Elastic Cloud instance')
 @click.option('--api_token', help='The base64 encoded API Key token', type=str)
 @click.option('--id', help='API Key "id" value', type=str)
 @click.option('--api_key', help='API Key "api_key" value', type=str)
 @click.option('--username', help='Username used to create "basic_auth" tuple')
 @click.option('--password', help='Password used to create "basic_auth" tuple')
@@ -277,17 +302,20 @@
 
     See http://elastic.co/guide/en/elasticsearch/client/curator/current
     """
     client_args = ClientArgs()
     other_args = OtherArgs()
     if config:
         from_yaml = get_yaml(config)
-        raw_config = check_config(from_yaml)
-        client_args.update_settings(raw_config['client'])
-        other_args.update_settings(raw_config['other_settings'])
+    else:
+        # Use empty defaults.
+        from_yaml = {'elasticsearch': {'client': {}, 'other_settings': {}}, 'logging': {}}
+    raw_config = check_config(from_yaml)
+    client_args.update_settings(raw_config['client'])
+    other_args.update_settings(raw_config['other_settings'])
 
     set_logging(check_logging_config(
         {'logging': override_logging(from_yaml, loglevel, logfile, logformat)}))
 
     hostslist = cli_hostslist(hosts)
 
     cli_client = prune_nones({
```

### Comparing `elasticsearch_curator-8.0.4/curator/config_utils.py` & `elasticsearch_curator-8.0.5/curator/config_utils.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/exceptions.py` & `elasticsearch_curator-8.0.5/curator/exceptions.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/indexlist.py` & `elasticsearch_curator-8.0.5/curator/indexlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,16 @@
         """
         self.loggit.debug('Getting all indices')
         self.all_indices = get_indices(self.client)
         self.indices = self.all_indices[:]
         if self.indices:
             for index in self.indices:
                 self.__build_index_info(index)
-            self._get_metadata()
-            self._get_index_stats()
+            self.get_metadata()
+            self.get_index_stats()
 
     def __build_index_info(self, index):
         """
         Ensure that ``index`` is a key in ``index_info``. If not, create a sub-dictionary structure
         under that key.
         """
         self.loggit.debug('Building preliminary index metadata for %s', index)
@@ -109,15 +109,25 @@
             'pattern': self.filter_by_regex,
             'space': self.filter_by_space,
             'shards': self.filter_by_shards,
             'size': self.filter_by_size,
         }
         return methods[ftype]
 
-    def _get_index_stats(self):
+    def __remove_missing(self, err):
+        """
+        Remove missing index found in ``err`` from self.indices and return that name
+        """
+        missing = err.info['error']['index']
+        self.loggit.warning('Index was initiallly present, but now is not: %s', missing)
+        self.loggit.debug('Removing %s from active IndexList')
+        self.indices.remove(missing)
+        return missing
+
+    def get_index_stats(self):
         """
         Populate ``index_info`` with index ``size_in_bytes``, ``primary_size_in_bytes`` and doc
         count information for each index.
         """
         self.loggit.debug('Getting index stats')
         self.empty_list_check()
         # Subroutine to do the dirty work
@@ -139,22 +149,36 @@
         for index in self.working_list():
             if self.index_info[index]['state'] == 'close':
                 working_list.remove(index)
         if working_list:
             index_lists = chunk_index_list(working_list)
             for lst in index_lists:
                 stats_result = {}
-                try:
-                    stats_result.update(self._get_indices_stats(lst))
-                except TransportError as err:
-                    if '413' in err.errors:
-                        self.loggit.debug('Huge Payload 413 Error - Trying to get information with multiple requests')
-                        stats_result = {}
-                        stats_result.update(self._bulk_queries(lst, self._get_indices_stats))
-                iterate_over_stats(stats_result)
+                checking = True
+                while checking:
+                    try:
+                        stats_result.update(self._get_indices_stats(lst))
+                    except NotFoundError as err:
+                        lst.remove(self.__remove_missing(err))
+                        continue
+                    except TransportError as err:
+                        if '413' in err.errors:
+                            msg = (
+                                'Huge Payload 413 Err - '
+                                'Trying to get information via multiple requests'
+                            )
+                            self.loggit.debug(msg)
+                            stats_result = {}
+                            try:
+                                stats_result.update(self._bulk_queries(lst, self._get_indices_stats))
+                            except NotFoundError as err2:
+                                lst.remove(self.__remove_missing(err2))
+                                continue
+                    iterate_over_stats(stats_result)
+                    checking = False
 
     def _get_indices_stats(self, data):
         return self.client.indices.stats(index=to_csv(data), metric='store,docs')
 
     def _bulk_queries(self, data, exec_func):
         slice_number = 10
         query_result = {}
@@ -167,39 +191,43 @@
                 data_sliced = data[num*slice_number:(num+1)*slice_number]
             query_result.update(exec_func(data_sliced))
         return query_result
 
     def _get_cluster_state(self, data):
         return self.client.cluster.state(index=to_csv(data), metric='metadata')['metadata']['indices']
 
-    def _get_metadata(self):
+    def get_metadata(self):
         """
         Populate ``index_info`` with index ``size_in_bytes`` and doc count information for each
         index.
         """
         self.loggit.debug('Getting index metadata')
         self.empty_list_check()
         for lst in chunk_index_list(self.indices):
             working_list = {}
+            # The API called by _get_cluster_state doesn't suffer from the same problems that
+            # _get_indices_stats does. This won't result in an error if an index is suddenly
+            # missing.
             try:
                 working_list.update(self._get_cluster_state(lst))
             except TransportError as err:
                 if '413' in err.errors:
-                    self.loggit.debug('Huge Payload 413 Error - Trying to get information with multiple requests')
+                    msg = 'Huge Payload 413 Err - Trying to get information via multiple requests'
+                    self.loggit.debug(msg)
                     working_list = {}
                     working_list.update(self._bulk_queries(lst, self._get_cluster_state))
             if working_list:
                 for index in list(working_list.keys()):
                     sii = self.index_info[index]
                     wli = working_list[index]
                     sii['age']['creation_date'] = (
                         fix_epoch(wli['settings']['index']['creation_date'])
                     )
-                    sii['number_of_replicas'] = (wli['settings']['index']['number_of_replicas'])
-                    sii['number_of_shards'] = (wli['settings']['index']['number_of_shards'])
+                    sii['number_of_replicas'] = wli['settings']['index']['number_of_replicas']
+                    sii['number_of_shards'] = wli['settings']['index']['number_of_shards']
                     sii['state'] = wli['state']
                     if 'routing' in wli['settings']['index']:
                         sii['routing'] = wli['settings']['index']['routing']
 
     def empty_list_check(self):
         """Raise :py:exc:`~.curator.exceptions.NoIndices` if ``indices`` is empty"""
         self.loggit.debug('Checking for empty list')
```

### Comparing `elasticsearch_curator-8.0.4/curator/logtools.py` & `elasticsearch_curator-8.0.5/curator/logtools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Logging tools"""
 import sys
 import json
 import logging
 import time
+from pathlib import Path
 import ecs_logging
 from curator.exceptions import LoggingException
 
 def de_dot(dot_string, msg):
     """
     Turn message and dotted string into a nested dictionary. Used by :py:class:`LogstashFormatter`
 
@@ -50,14 +51,19 @@
         if isinstance(value, dict):
             node = destination.setdefault(key, {})
             deepmerge(value, node)
         else:
             destination[key] = value
     return destination
 
+def is_docker():
+    """Check if we're running in a docker container"""
+    cgroup = Path('/proc/self/cgroup')
+    return Path('/.dockerenv').is_file() or cgroup.is_file() and 'docker' in cgroup.read_text()
+
 class LogstashFormatter(logging.Formatter):
     """Logstash formatting (JSON)"""
     # The LogRecord attributes we want to carry over to the Logstash message,
     # mapped to the corresponding output key.
     WANTED_ATTRS = {
         'levelname': 'loglevel',
         'funcName': 'function',
@@ -122,15 +128,18 @@
         #: Attribute. The logging format string to use.
         self.format_string = '%(asctime)s %(levelname)-9s %(message)s'
 
         if not isinstance(self.numeric_log_level, int):
             raise ValueError(f"Invalid log level: {cfg['loglevel']}")
 
         #: Attribute. Which logging handler to use
-        self.handler = logging.StreamHandler(stream=sys.stdout)
+        if is_docker():
+            self.handler = logging.FileHandler('/proc/1/fd/1')
+        else:
+            self.handler = logging.StreamHandler(stream=sys.stdout)
         if cfg['logfile']:
             self.handler = logging.FileHandler(cfg['logfile'])
 
         if self.numeric_log_level == 10: # DEBUG
             self.format_string = (
                 '%(asctime)s %(levelname)-9s %(name)22s %(funcName)22s:%(lineno)-4d %(message)s')
```

### Comparing `elasticsearch_curator-8.0.4/curator/repomgrcli.py` & `elasticsearch_curator-8.0.5/curator/repomgrcli.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/singletons.py` & `elasticsearch_curator-8.0.5/curator/singletons.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/snapshotlist.py` & `elasticsearch_curator-8.0.5/curator/snapshotlist.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/actions/__init__.py` & `elasticsearch_curator-8.0.5/curator/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/actions/alias.py` & `elasticsearch_curator-8.0.5/curator/actions/alias.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/actions/allocation.py` & `elasticsearch_curator-8.0.5/curator/actions/allocation.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/actions/close.py` & `elasticsearch_curator-8.0.5/curator/actions/close.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/actions/cluster_routing.py` & `elasticsearch_curator-8.0.5/curator/actions/cluster_routing.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/actions/cold2frozen.py` & `elasticsearch_curator-8.0.5/curator/actions/cold2frozen.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/actions/create_index.py` & `elasticsearch_curator-8.0.5/curator/actions/create_index.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/actions/delete_indices.py` & `elasticsearch_curator-8.0.5/curator/actions/delete_indices.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/actions/forcemerge.py` & `elasticsearch_curator-8.0.5/curator/actions/forcemerge.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/actions/index_settings.py` & `elasticsearch_curator-8.0.5/curator/actions/index_settings.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/actions/open.py` & `elasticsearch_curator-8.0.5/curator/actions/open.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/actions/reindex.py` & `elasticsearch_curator-8.0.5/curator/actions/reindex.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/actions/replicas.py` & `elasticsearch_curator-8.0.5/curator/actions/replicas.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/actions/rollover.py` & `elasticsearch_curator-8.0.5/curator/actions/rollover.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/actions/shrink.py` & `elasticsearch_curator-8.0.5/curator/actions/shrink.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/actions/snapshot.py` & `elasticsearch_curator-8.0.5/curator/actions/snapshot.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/cli_singletons/__init__.py` & `elasticsearch_curator-8.0.5/curator/cli_singletons/__init__.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/cli_singletons/alias.py` & `elasticsearch_curator-8.0.5/curator/cli_singletons/alias.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/cli_singletons/allocation.py` & `elasticsearch_curator-8.0.5/curator/cli_singletons/allocation.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/cli_singletons/close.py` & `elasticsearch_curator-8.0.5/curator/cli_singletons/close.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/cli_singletons/delete.py` & `elasticsearch_curator-8.0.5/curator/cli_singletons/delete.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/cli_singletons/forcemerge.py` & `elasticsearch_curator-8.0.5/curator/cli_singletons/forcemerge.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/cli_singletons/object_class.py` & `elasticsearch_curator-8.0.5/curator/cli_singletons/object_class.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/cli_singletons/open_indices.py` & `elasticsearch_curator-8.0.5/curator/cli_singletons/open_indices.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/cli_singletons/replicas.py` & `elasticsearch_curator-8.0.5/curator/cli_singletons/replicas.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/cli_singletons/restore.py` & `elasticsearch_curator-8.0.5/curator/cli_singletons/restore.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/cli_singletons/rollover.py` & `elasticsearch_curator-8.0.5/curator/cli_singletons/rollover.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/cli_singletons/show.py` & `elasticsearch_curator-8.0.5/curator/cli_singletons/show.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/cli_singletons/shrink.py` & `elasticsearch_curator-8.0.5/curator/cli_singletons/shrink.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/cli_singletons/snapshot.py` & `elasticsearch_curator-8.0.5/curator/cli_singletons/snapshot.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/cli_singletons/utils.py` & `elasticsearch_curator-8.0.5/curator/cli_singletons/utils.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/defaults/filter_elements.py` & `elasticsearch_curator-8.0.5/curator/defaults/filter_elements.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/defaults/filtertypes.py` & `elasticsearch_curator-8.0.5/curator/defaults/filtertypes.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/defaults/logging_defaults.py` & `elasticsearch_curator-8.0.5/curator/defaults/logging_defaults.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/defaults/option_defaults.py` & `elasticsearch_curator-8.0.5/curator/defaults/option_defaults.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/defaults/settings.py` & `elasticsearch_curator-8.0.5/curator/defaults/settings.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/helpers/date_ops.py` & `elasticsearch_curator-8.0.5/curator/helpers/date_ops.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/helpers/getters.py` & `elasticsearch_curator-8.0.5/curator/helpers/getters.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/helpers/testers.py` & `elasticsearch_curator-8.0.5/curator/helpers/testers.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/helpers/utils.py` & `elasticsearch_curator-8.0.5/curator/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/helpers/waiters.py` & `elasticsearch_curator-8.0.5/curator/helpers/waiters.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from datetime import datetime
 from curator.exceptions import (
     ActionTimeout, ConfigurationError, CuratorException, FailedReindex, MissingArgument)
 from curator.helpers.utils import chunk_index_list
 
 def health_check(client, **kwargs):
     """
-    This function calls `client.cluster.` :py:meth:`~.elasticsearch.client.ClusterClient.health` and, based on the
-    params provided, will return ``True`` or ``False`` depending on whether that particular keyword
-    appears in the output, and has the expected value.
+    This function calls `client.cluster.` :py:meth:`~.elasticsearch.client.ClusterClient.health`
+    and, based on the params provided, will return ``True`` or ``False`` depending on whether that
+    particular keyword appears in the output, and has the expected value.
 
     If multiple keys are provided, all must match for a ``True`` response.
 
     :param client: A client connection object
 
     :type client: :py:class:`~.elasticsearch.Elasticsearch`
 
@@ -116,19 +116,19 @@
                 return False
 
     # If we've gotten here, all of the indices have recovered
     return True
 
 def snapshot_check(client, snapshot=None, repository=None):
     """
-    This function calls `client.snapshot.` :py:meth:`~.elasticsearch.client.SnapshotClient.get` and tests to see
-    whether the snapshot is complete, and if so, with what status.  It will log errors according
-    to the result. If the snapshot is still ``IN_PROGRESS``, it will return ``False``.  ``SUCCESS``
-    will be an ``INFO`` level message, ``PARTIAL`` nets a ``WARNING`` message, ``FAILED`` is an
-    ``ERROR``, message, and all others will be a ``WARNING`` level message.
+    This function calls `client.snapshot.` :py:meth:`~.elasticsearch.client.SnapshotClient.get` and
+    tests to see whether the snapshot is complete, and if so, with what status.  It will log errors
+    according to the result. If the snapshot is still ``IN_PROGRESS``, it will return ``False``.
+    ``SUCCESS`` will be an ``INFO`` level message, ``PARTIAL`` nets a ``WARNING`` message,
+    ``FAILED`` is an ``ERROR``, message, and all others will be a ``WARNING`` level message.
 
     :param client: A client connection object
     :param snapshot: The snapshot name
     :param repository: The repository name
 
     :type client: :py:class:`~.elasticsearch.Elasticsearch`
     :type snapshot: str
@@ -196,15 +196,15 @@
                 msg = f'Failures found in reindex response: {response["failures"]}'
                 raise FailedReindex(msg)
     running_time = 0.000000001 * task['running_time_in_nanos']
     logger.debug('Running time: %s seconds', running_time)
     descr = task['description']
 
     if completed:
-        completion_time = ((running_time * 1000) + task['start_time_in_millis'])
+        completion_time = (running_time * 1000) + task['start_time_in_millis']
         time_string = strftime('%Y-%m-%dT%H:%M:%SZ', localtime(completion_time/1000))
         logger.info('Task "%s" completed at %s.', descr, time_string)
         retval = True
     else:
         # Log the task status here.
         logger.debug('Full Task Data: %s', task_data)
         msg = (
```

### Comparing `elasticsearch_curator-8.0.4/curator/validators/actions.py` & `elasticsearch_curator-8.0.5/curator/validators/actions.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/validators/filter_functions.py` & `elasticsearch_curator-8.0.5/curator/validators/filter_functions.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/validators/options.py` & `elasticsearch_curator-8.0.5/curator/validators/options.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/curator/validators/schemacheck.py` & `elasticsearch_curator-8.0.5/curator/validators/schemacheck.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/LICENSE` & `elasticsearch_curator-8.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/NOTICE` & `elasticsearch_curator-8.0.5/NOTICE`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/README.rst` & `elasticsearch_curator-8.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.4/pyproject.toml` & `elasticsearch_curator-8.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 keywords = [
     'elasticsearch',
     'time-series',
     'indexed',
     'index-expiry'
 ]
 dependencies = [
-    "elasticsearch8==8.7.0",
-    "es_client==8.7.0",
-    "ecs-logging==2.0.0",
-    "click==8.1.3",
+    "elasticsearch8==8.8.2",
+    "es_client==8.8.2",
+    "ecs-logging==2.0.2",
+    "click==8.1.4",
     "pyyaml==6.0.0",
     "voluptuous>=0.13.1",
-    "certifi>=2022.12.7",
+    "certifi>=2023.5.7",
     "six>=1.16.0",
 ]
 
 [project.optional-dependencies]
 test = [
     "mock",
     "requests",
@@ -99,15 +99,15 @@
 step4 = "step3 ; echo 'Tests complete! Destroying Docker test environment...' "
 full = "step4 ; $(docker_test/scripts/destroy.sh 2&>1 /dev/null ) ;  exit $EXITCODE"
 run-coverage = "pytest --cov-config=pyproject.toml --cov=curator --cov=tests"
 run = "run-coverage --no-cov"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["3.9", "3.10", "3.11"]
-version = ["8.0.4"]
+version = ["8.0.5"]
 
 [tool.pytest.ini_options]
 pythonpath = [".", "curator"]
 minversion = "7.2"
 addopts = "-ra -q"
 testpaths = [
     "tests/unit",
```

### Comparing `elasticsearch_curator-8.0.4/PKG-INFO` & `elasticsearch_curator-8.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elasticsearch-curator
-Version: 8.0.4
+Version: 8.0.5
 Summary: Tending your Elasticsearch indices and snapshots
 Project-URL: Homepage, https://github.com/elastic/curator
 Project-URL: Bug Tracker, https://github.com/elastic/curator/issues
 Author-email: Elastic <info@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
@@ -15,19 +15,19 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
-Requires-Dist: certifi>=2022.12.7
-Requires-Dist: click==8.1.3
-Requires-Dist: ecs-logging==2.0.0
-Requires-Dist: elasticsearch8==8.7.0
-Requires-Dist: es-client==8.7.0
+Requires-Dist: certifi>=2023.5.7
+Requires-Dist: click==8.1.4
+Requires-Dist: ecs-logging==2.0.2
+Requires-Dist: elasticsearch8==8.8.2
+Requires-Dist: es-client==8.8.2
 Requires-Dist: pyyaml==6.0.0
 Requires-Dist: six>=1.16.0
 Requires-Dist: voluptuous>=0.13.1
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == 'doc'
 Requires-Dist: sphinx-rtd-theme; extra == 'doc'
 Provides-Extra: test
```

