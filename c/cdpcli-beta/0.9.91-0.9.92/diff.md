# Comparing `tmp/cdpcli-beta-0.9.91.tar.gz` & `tmp/cdpcli-beta-0.9.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdpcli-beta-0.9.91.tar", last modified: Wed Jun 28 19:35:59 2023, max compression
+gzip compressed data, was "cdpcli-beta-0.9.92.tar", last modified: Thu Jul 13 16:50:38 2023, max compression
```

## Comparing `cdpcli-beta-0.9.91.tar` & `cdpcli-beta-0.9.92.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.339583 cdpcli-beta-0.9.91/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/LICENSE.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/MANIFEST.in
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-06-28 19:35:59.339583 cdpcli-beta-0.9.91/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/README.md
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.339583 cdpcli-beta-0.9.91/cdpcli/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-06-28 19:35:59.339583 cdpcli-beta-0.9.91/cdpcli/_version.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/cdprequest.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/clicommand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/clidriver.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/compat.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/config.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/configloader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/credentials.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.323583 cdpcli-beta-0.9.91/cdpcli/data/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/data/_retry.json
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      246 2023-06-28 19:35:58.000000 cdpcli-beta-0.9.91/cdpcli/data/aliases.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.327583 cdpcli-beta-0.9.91/cdpcli/data/audit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-06-28 19:35:58.000000 cdpcli-beta-0.9.91/cdpcli/data/audit/audit.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/data/cli.json
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.327583 cdpcli-beta-0.9.91/cdpcli/data/cloudprivatelinks/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8803 2023-06-28 19:35:55.000000 cdpcli-beta-0.9.91/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.327583 cdpcli-beta-0.9.91/cdpcli/data/compute/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    97819 2023-06-28 19:35:54.000000 cdpcli-beta-0.9.91/cdpcli/data/compute/compute.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.327583 cdpcli-beta-0.9.91/cdpcli/data/datacatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-06-28 19:35:58.000000 cdpcli-beta-0.9.91/cdpcli/data/datacatalog/datacatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.327583 cdpcli-beta-0.9.91/cdpcli/data/datahub/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   150970 2023-06-28 19:35:56.000000 cdpcli-beta-0.9.91/cdpcli/data/datahub/datahub.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.327583 cdpcli-beta-0.9.91/cdpcli/data/datalake/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   105695 2023-06-28 19:35:55.000000 cdpcli-beta-0.9.91/cdpcli/data/datalake/datalake.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.327583 cdpcli-beta-0.9.91/cdpcli/data/de/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    32532 2023-06-28 19:35:57.000000 cdpcli-beta-0.9.91/cdpcli/data/de/de.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.327583 cdpcli-beta-0.9.91/cdpcli/data/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    93690 2023-06-28 19:35:56.000000 cdpcli-beta-0.9.91/cdpcli/data/df/df.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.327583 cdpcli-beta-0.9.91/cdpcli/data/dfworkload/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    82316 2023-06-28 19:35:57.000000 cdpcli-beta-0.9.91/cdpcli/data/dfworkload/dfworkload.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.327583 cdpcli-beta-0.9.91/cdpcli/data/drscp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-06-28 19:35:55.000000 cdpcli-beta-0.9.91/cdpcli/data/drscp/drscp.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.327583 cdpcli-beta-0.9.91/cdpcli/data/dw/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   193413 2023-06-28 19:35:55.000000 cdpcli-beta-0.9.91/cdpcli/data/dw/dw.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.327583 cdpcli-beta-0.9.91/cdpcli/data/environments/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   181297 2023-06-28 19:35:54.000000 cdpcli-beta-0.9.91/cdpcli/data/environments/environments.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.327583 cdpcli-beta-0.9.91/cdpcli/data/iam/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   149065 2023-06-28 19:35:56.000000 cdpcli-beta-0.9.91/cdpcli/data/iam/iam.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.327583 cdpcli-beta-0.9.91/cdpcli/data/imagecatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    25663 2023-06-28 19:35:55.000000 cdpcli-beta-0.9.91/cdpcli/data/imagecatalog/imagecatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.327583 cdpcli-beta-0.9.91/cdpcli/data/ml/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    56972 2023-06-28 19:35:57.000000 cdpcli-beta-0.9.91/cdpcli/data/ml/ml.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.327583 cdpcli-beta-0.9.91/cdpcli/data/opdb/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    73060 2023-06-28 19:35:57.000000 cdpcli-beta-0.9.91/cdpcli/data/opdb/opdb.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        4 2023-06-28 19:35:58.000000 cdpcli-beta-0.9.91/cdpcli/data/release.txt
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.327583 cdpcli-beta-0.9.91/cdpcli/data/replicationmanager/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    52335 2023-06-28 19:35:58.000000 cdpcli-beta-0.9.91/cdpcli/data/replicationmanager/replicationmanager.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.327583 cdpcli-beta-0.9.91/cdpcli/doc/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/doc/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/doc/docstringparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/doc/restdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/doc/style.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/endpoint.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.319583 cdpcli-beta-0.9.91/cdpcli/examples/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.327583 cdpcli-beta-0.9.91/cdpcli/examples/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/examples/configure/_description.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.327583 cdpcli-beta-0.9.91/cdpcli/examples/configure/get/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/examples/configure/get/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/examples/configure/get/_examples.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.331583 cdpcli-beta-0.9.91/cdpcli/examples/configure/set/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/examples/configure/set/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/examples/configure/set/_examples.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/exceptions.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.331583 cdpcli-beta-0.9.91/cdpcli/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/commands.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.331583 cdpcli-beta-0.9.91/cdpcli/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/configure/classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/configure/configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/configure/get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/configure/list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/configure/set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.331583 cdpcli-beta-0.9.91/cdpcli/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    29050 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/df/createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/df/register.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/refdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/extensions/writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/loader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/main.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/paramformfactor.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/parser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/schema.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/serialize.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/table.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/text.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/textwriter.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.331583 cdpcli-beta-0.9.91/cdpcli/thirdparty/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/thirdparty/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/thirdparty/six.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/translate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/cdpcli/validate.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.331583 cdpcli-beta-0.9.91/cdpcli_beta.egg-info/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-06-28 19:35:58.000000 cdpcli-beta-0.9.91/cdpcli_beta.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4297 2023-06-28 19:35:58.000000 cdpcli-beta-0.9.91/cdpcli_beta.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-06-28 19:35:58.000000 cdpcli-beta-0.9.91/cdpcli_beta.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-06-28 19:35:58.000000 cdpcli-beta-0.9.91/cdpcli_beta.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-06-28 19:35:58.000000 cdpcli-beta-0.9.91/cdpcli_beta.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-06-28 19:35:58.000000 cdpcli-beta-0.9.91/cdpcli_beta.egg-info/top_level.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-06-28 19:35:59.339583 cdpcli-beta-0.9.91/setup.cfg
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1429 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/setup.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/setup_common.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.319583 cdpcli-beta-0.9.91/tests/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.335583 cdpcli-beta-0.9.91/tests/unit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.335583 cdpcli-beta-0.9.91/tests/unit/cdp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/cdp/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.335583 cdpcli-beta-0.9.91/tests/unit/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/extensions/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.335583 cdpcli-beta-0.9.91/tests/unit/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/extensions/configure/test_classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/extensions/configure/test_configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/extensions/configure/test_get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/extensions/configure/test_list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/extensions/configure/test_set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:35:59.339583 cdpcli-beta-0.9.91/tests/unit/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    38131 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/extensions/df/test_createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/extensions/df/test_upload_file.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/extensions/test_cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/extensions/test_df.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/extensions/test_generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/extensions/test_interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/extensions/test_logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/extensions/test_operation_extension.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/extensions/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/extensions/test_redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/extensions/test_workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/extensions/test_writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_cli_data.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_credentials.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_endpoint.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_loaders.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_protocol.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_table_formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/tests/unit/test_validate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-06-28 19:23:12.000000 cdpcli-beta-0.9.91/versioneer.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.613861 cdpcli-beta-0.9.92/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/LICENSE.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/MANIFEST.in
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-07-13 16:50:38.613861 cdpcli-beta-0.9.92/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/README.md
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.617861 cdpcli-beta-0.9.92/cdpcli/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-07-13 16:50:38.617861 cdpcli-beta-0.9.92/cdpcli/_version.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/cdprequest.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/clicommand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/clidriver.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/compat.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/config.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/configloader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/credentials.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.601861 cdpcli-beta-0.9.92/cdpcli/data/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/data/_retry.json
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      246 2023-07-13 16:50:37.000000 cdpcli-beta-0.9.92/cdpcli/data/aliases.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/audit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-07-13 16:50:37.000000 cdpcli-beta-0.9.92/cdpcli/data/audit/audit.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/data/cli.json
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/cloudprivatelinks/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8803 2023-07-13 16:50:34.000000 cdpcli-beta-0.9.92/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/compute/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    97819 2023-07-13 16:50:34.000000 cdpcli-beta-0.9.92/cdpcli/data/compute/compute.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/datacatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-07-13 16:50:37.000000 cdpcli-beta-0.9.92/cdpcli/data/datacatalog/datacatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/datahub/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   150925 2023-07-13 16:50:36.000000 cdpcli-beta-0.9.92/cdpcli/data/datahub/datahub.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/datalake/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   105668 2023-07-13 16:50:35.000000 cdpcli-beta-0.9.92/cdpcli/data/datalake/datalake.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/de/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    32532 2023-07-13 16:50:37.000000 cdpcli-beta-0.9.92/cdpcli/data/de/de.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    93690 2023-07-13 16:50:35.000000 cdpcli-beta-0.9.92/cdpcli/data/df/df.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/dfworkload/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    82316 2023-07-13 16:50:37.000000 cdpcli-beta-0.9.92/cdpcli/data/dfworkload/dfworkload.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/drscp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-07-13 16:50:35.000000 cdpcli-beta-0.9.92/cdpcli/data/drscp/drscp.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/dw/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   193989 2023-07-13 16:50:34.000000 cdpcli-beta-0.9.92/cdpcli/data/dw/dw.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/environments/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   181639 2023-07-13 16:50:33.000000 cdpcli-beta-0.9.92/cdpcli/data/environments/environments.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/iam/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   149065 2023-07-13 16:50:35.000000 cdpcli-beta-0.9.92/cdpcli/data/iam/iam.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/imagecatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    25663 2023-07-13 16:50:34.000000 cdpcli-beta-0.9.92/cdpcli/data/imagecatalog/imagecatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/ml/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    56972 2023-07-13 16:50:37.000000 cdpcli-beta-0.9.92/cdpcli/data/ml/ml.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/opdb/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    73060 2023-07-13 16:50:36.000000 cdpcli-beta-0.9.92/cdpcli/data/opdb/opdb.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        4 2023-07-13 16:50:37.000000 cdpcli-beta-0.9.92/cdpcli/data/release.txt
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/data/replicationmanager/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    54815 2023-07-13 16:50:37.000000 cdpcli-beta-0.9.92/cdpcli/data/replicationmanager/replicationmanager.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/doc/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/doc/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/doc/docstringparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/doc/restdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/doc/style.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/endpoint.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.597861 cdpcli-beta-0.9.92/cdpcli/examples/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/examples/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/examples/configure/_description.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/examples/configure/get/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/examples/configure/get/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/examples/configure/get/_examples.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.605861 cdpcli-beta-0.9.92/cdpcli/examples/configure/set/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/examples/configure/set/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/examples/configure/set/_examples.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/exceptions.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.609861 cdpcli-beta-0.9.92/cdpcli/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/commands.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.609861 cdpcli-beta-0.9.92/cdpcli/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/configure/classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/configure/configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/configure/get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/configure/list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/configure/set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.609861 cdpcli-beta-0.9.92/cdpcli/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29050 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/df/createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/df/register.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/refdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/extensions/writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/loader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/main.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/paramformfactor.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/parser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/schema.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/serialize.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/table.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/text.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/textwriter.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.609861 cdpcli-beta-0.9.92/cdpcli/thirdparty/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/thirdparty/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/thirdparty/six.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/translate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/cdpcli/validate.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.609861 cdpcli-beta-0.9.92/cdpcli_beta.egg-info/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-07-13 16:50:38.000000 cdpcli-beta-0.9.92/cdpcli_beta.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4297 2023-07-13 16:50:38.000000 cdpcli-beta-0.9.92/cdpcli_beta.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-07-13 16:50:38.000000 cdpcli-beta-0.9.92/cdpcli_beta.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-07-13 16:50:38.000000 cdpcli-beta-0.9.92/cdpcli_beta.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-07-13 16:50:38.000000 cdpcli-beta-0.9.92/cdpcli_beta.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-07-13 16:50:38.000000 cdpcli-beta-0.9.92/cdpcli_beta.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-07-13 16:50:38.617861 cdpcli-beta-0.9.92/setup.cfg
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1429 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/setup.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/setup_common.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.597861 cdpcli-beta-0.9.92/tests/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.613861 cdpcli-beta-0.9.92/tests/unit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.613861 cdpcli-beta-0.9.92/tests/unit/cdp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/cdp/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.613861 cdpcli-beta-0.9.92/tests/unit/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.613861 cdpcli-beta-0.9.92/tests/unit/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/configure/test_classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/configure/test_configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/configure/test_get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/configure/test_list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/configure/test_set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:50:38.613861 cdpcli-beta-0.9.92/tests/unit/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    38131 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/df/test_createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/df/test_upload_file.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/test_cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/test_df.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/test_generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/test_interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/test_logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/test_operation_extension.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/test_redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/test_workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/extensions/test_writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_cli_data.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_credentials.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_endpoint.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_loaders.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_protocol.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_table_formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/tests/unit/test_validate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-07-13 16:37:48.000000 cdpcli-beta-0.9.92/versioneer.py
```

### Comparing `cdpcli-beta-0.9.91/LICENSE.txt` & `cdpcli-beta-0.9.92/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt` & `cdpcli-beta-0.9.92/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/PKG-INFO` & `cdpcli-beta-0.9.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdpcli-beta
-Version: 0.9.91
+Version: 0.9.92
 Summary: Cloudera CDP Command Line Interface (BETA)
 Home-page: https://console.cdp.cloudera.com/
 Author: Cloudera, Inc.
 License: Apache License 2.0
 Description: # Cloudera CDP Command Line Interface
         
         This package provides a unified command line interface to the Cloudera Data
```

### Comparing `cdpcli-beta-0.9.91/README.md` & `cdpcli-beta-0.9.92/README.md`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/__init__.py` & `cdpcli-beta-0.9.92/cdpcli/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/argparser.py` & `cdpcli-beta-0.9.92/cdpcli/argparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/argprocess.py` & `cdpcli-beta-0.9.92/cdpcli/argprocess.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/arguments.py` & `cdpcli-beta-0.9.92/cdpcli/arguments.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/auth.py` & `cdpcli-beta-0.9.92/cdpcli/auth.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/cdprequest.py` & `cdpcli-beta-0.9.92/cdpcli/cdprequest.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/clicommand.py` & `cdpcli-beta-0.9.92/cdpcli/clicommand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/clidriver.py` & `cdpcli-beta-0.9.92/cdpcli/clidriver.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/client.py` & `cdpcli-beta-0.9.92/cdpcli/client.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/compat.py` & `cdpcli-beta-0.9.92/cdpcli/compat.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/completer.py` & `cdpcli-beta-0.9.92/cdpcli/completer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/config.py` & `cdpcli-beta-0.9.92/cdpcli/config.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/configloader.py` & `cdpcli-beta-0.9.92/cdpcli/configloader.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/credentials.py` & `cdpcli-beta-0.9.92/cdpcli/credentials.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/data/_retry.json` & `cdpcli-beta-0.9.92/cdpcli/data/_retry.json`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/data/audit/audit.yaml` & `cdpcli-beta-0.9.92/cdpcli/data/audit/audit.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: audit
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.91
+  version: 0.9.92
   title: Cloudera Audit Service
   license:
     name: Apache 2.0
   description: Cloudera CDP Auditing is a web service for interacting with the audit subsystem.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.91/cdpcli/data/cli.json` & `cdpcli-beta-0.9.92/cdpcli/data/cli.json`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml` & `cdpcli-beta-0.9.92/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: cloudprivatelinks
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: BETA
 info:
-  version: 0.9.91
+  version: 0.9.92
   title: Cloudera CloudPrivateLinks API Service
   license:
     name: Apache 2.0
   description: Provisions PrivateLink Endpoints on the cloud environments.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.91/cdpcli/data/compute/compute.yaml` & `cdpcli-beta-0.9.92/cdpcli/data/compute/compute.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: compute
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.91
+  version: 0.9.92
   title: Cloudera Compute Service
   license:
     name: Apache 2.0
   description: Defining service of compute public API service
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.91/cdpcli/data/datacatalog/datacatalog.yaml` & `cdpcli-beta-0.9.92/cdpcli/data/datacatalog/datacatalog.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: datacatalog
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.91
+  version: 0.9.92
   title: Cloudera DataCatalog Service
   license:
     name: Apache 2.0
   description: Cloudera DataCatalog Service is a web service, using this service a user can execute operations like launching profilers in DataCatalog.
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.91/cdpcli/data/datahub/datahub.yaml` & `cdpcli-beta-0.9.92/cdpcli/data/datahub/datahub.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: datahub
 x-interface-model: cdp
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.91
+  version: 0.9.92
   title: Cloudera Data hub Service
   license:
     name: Apache 2.0
   description: Cloudera data hub is a service for launching and managing workload clusters powered by Cloudera Runtime.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -1295,17 +1295,14 @@
         description: The error code.
       message:
         type: string
         description: The error message.
   ImageRequest:
     type: object
     description: The details of the image used for cluster instances.
-    required:
-      - id
-      - catalogName
     properties:
       id:
         type: string
         description: The ID of the image used for cluster instances. This is generated by the cloud provider to uniquely identify the image.
       catalogName:
         type: string
         description: The image catalog name.
```

### Comparing `cdpcli-beta-0.9.91/cdpcli/data/datalake/datalake.yaml` & `cdpcli-beta-0.9.92/cdpcli/data/datalake/datalake.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: datalake
 x-interface-model: cdp
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.91
+  version: 0.9.92
   title: Cloudera Datalake Service
   license:
     name: Apache 2.0
   description: Cloudera data lake is a service for launching and managing data lake clusters powered by Cloudera Runtime.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -2713,25 +2713,23 @@
     description: Response object to rotate autotls certificates on datalake's hosts, deprecated.
     x-deprecated: true
   RenewCertificateResponse:
     type: object
     description: Response object for renew certificate request, deprecated.
     x-deprecated: true
   ImageRequest:
-    description: The image request for the datalake. This must not be set if the runtime parameter is provided. The image ID parameter is required if this is present, but the image catalog name is optional, defaulting to 'cdp-default' if not present.
+    description: The image request for the datalake. When the 'runtime' parameter is set, only the 'os' parameter can be provided. Otherwise, you can use 'catalog name' and/or 'id' for selecting an image.
     type: object
-    required:
-      - id
     properties:
       id:
         type: string
         description: The image ID from the catalog. The corresponding image will be used for the created cluster machines.
       catalogName:
         type: string
-        description: The name of the custom image catalog to use.
+        description: The name of the custom image catalog to use, defaulting to 'cdp-default' if not present.
         default: cdp-default
   ResizeDatalakeRequest:
     type: object
     description: Datalake resize request.
     required:
       - datalakeName
       - targetSize
```

### Comparing `cdpcli-beta-0.9.91/cdpcli/data/de/de.yaml` & `cdpcli-beta-0.9.92/cdpcli/data/de/de.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: de
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.91
+  version: 0.9.92
   title: Cloudera Data Engineering
   license:
     name: Apache 2.0
   description: Create and manage Cloudera Data Engineering Services.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.91/cdpcli/data/df/df.yaml` & `cdpcli-beta-0.9.92/cdpcli/data/df/df.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: df
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.91
+  version: 0.9.92
   title: Cloudera DataFlow Service
   license:
     name: Apache 2.0
   description: Manage DataFlow Services.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.91/cdpcli/data/dfworkload/dfworkload.yaml` & `cdpcli-beta-0.9.92/cdpcli/data/dfworkload/dfworkload.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 swagger: '2.0'
 x-endpoint-name: dfworkload
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
   description: "This REST API provides remote access to the DataFlow Service.\n Endpoints that are marked as [BETA] are subject to change in future releases of the application without backwards compatibility and without a major version change."
-  version: 0.9.91
+  version: 0.9.92
   title: Cloudera DataFlow Workload Service
   license:
     name: Apache 2.0
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.91/cdpcli/data/drscp/drscp.yaml` & `cdpcli-beta-0.9.92/cdpcli/data/drscp/drscp.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: drscp
 x-products: CDP
 x-form-factors: private
 x-audit: true
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.91
+  version: 0.9.92
   title: CDP Control Plane Data Recovery Service
   license:
     name: Apache 2.0
   description: The API of Data Recovery Service for CDP Private Cloud Control Plane .
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.91/cdpcli/data/dw/dw.yaml` & `cdpcli-beta-0.9.92/cdpcli/data/dw/dw.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 swagger: '2.0'
 x-endpoint-name: dw
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.91
+  version: 0.9.92
   title: Cloudera Data Warehouse [EXPERIMENTAL]
   license:
     name: Apache 2.0
   description: Install and manage Cloudera Data Warehouse clusters.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -2152,15 +2152,15 @@
         description: Enables private SQL for the cluster deployment.
         default: false
       privateDNSZoneAKS:
         type: string
         description: Private DNS zone AKS resource ID.
       enablePrivateAks:
         type: boolean
-        description: Enable Azure Private AKS mode.
+        description: Enable Azure Private AKS mode. Note that this feature is currently unstable due to critical networking issues within the Azure Software Definition Layer (SDN). This problem prevents the deployment of necessary components and results in unpredictable behavior and instability, impacting operations such as environment activation, VW creation, modification, and start/stop operations. While we work towards a resolution with Microsoft, estimated within the next 6-9 months, we recommend utilizing alternative methods like enabling public endpoints or virtual network peering for accessing your Azure Cluster.
         default: false
   PrivateCloudActivationOptions:
     type: object
     description: Options for activating a Private Cloud environment.
     required:
       - delegationUsername
       - delegationPassword
```

### Comparing `cdpcli-beta-0.9.91/cdpcli/data/environments/environments.yaml` & `cdpcli-beta-0.9.92/cdpcli/data/environments/environments.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: environments2
 x-display-name: environments
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.91
+  version: 0.9.92
   title: Cloudera Environments Service
   license:
     name: Apache 2.0
   description: Cloudera Environments Service is a web service that manages cloud provider access.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -2427,14 +2427,19 @@
         description: When this is enabled, then Azure Postgres will be configured with Private Endpoint and a Private DNS Zone. When this is disabled, then Azure Service Endpoints will be created. The default value is disabled.
       endpointAccessGatewayScheme:
         type: string
         description: The scheme for the endpoint gateway. PUBLIC creates an external endpoint that can be accessed over the Internet. Defaults to PRIVATE which restricts the traffic to be internal to the VNet.
         enum:
           - PUBLIC
           - PRIVATE
+      endpointAccessGatewaySubnetIds:
+        type: array
+        items:
+          type: string
+        description: The subnets to use for endpoint access gateway.
       encryptionKeyUrl:
         type: string
         description: URL of the key which will be used to encrypt the Azure Managed Disks, if entitlement has been granted.
         x-no-paramfile: true
       encryptionKeyResourceGroupName:
         type: string
         description: Name of the existing Azure resource group hosting the Azure Key Vault containing customer managed key which will be used to encrypt the Azure Managed Disks. It is required only when the entitlement is granted and the resource group of the key vault is different from the resource group in which the environment is to be created. Omitting it implies that, the key vault containing the encryption key is present in the same resource group where the environment would be created.
@@ -2493,14 +2498,19 @@
         description: The FreeIPA creation request for the environment
       endpointAccessGatewayScheme:
         type: string
         description: The scheme for the endpoint gateway. PUBLIC creates an external endpoint that can be accessed over the Internet. Defaults to PRIVATE which restricts the traffic to be internal to the VPC.
         enum:
           - PUBLIC
           - PRIVATE
+      endpointAccessGatewaySubnetIds:
+        type: array
+        items:
+          type: string
+        description: The subnets to use for endpoint access gateway.
       tags:
         type: array
         description: Tags that can be attached to GCP resources. Please refer to Google documentation for the rules https://cloud.google.com/compute/docs/labeling-resources#label_format.
         items:
           $ref: '#/definitions/GcpTagRequest'
       proxyConfigName:
         type: string
@@ -4823,18 +4833,17 @@
           - HA
         description: The target FreeIPA availability type.
       operationId:
         description: UUID of the request for this operation. This ID can be used to get the status of the operation.
         type: string
   DownscaleFreeipaRequest:
     type: object
-    description: The request object for FreeIPA downscale.
+    description: The request object for FreeIPA downscale. Either targetAvailabilityType or instances
     required:
       - environmentName
-      - targetAvailabilityType
     properties:
       environmentName:
         type: string
         description: The name or CRN of the environment.
       targetAvailabilityType:
         type: string
         enum:
```

### Comparing `cdpcli-beta-0.9.91/cdpcli/data/iam/iam.yaml` & `cdpcli-beta-0.9.92/cdpcli/data/iam/iam.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: iam
 x-products: ALTUS,CDP
 x-form-factors: public,private
 x-altus-releases: PUBLIC
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.91
+  version: 0.9.92
   title: Cloudera IAM Service
   license:
     name: Apache 2.0
   description: Cloudera CDP IAM is a web service that you can use to manage users and user permissions under your CDP account.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.91/cdpcli/data/imagecatalog/imagecatalog.yaml` & `cdpcli-beta-0.9.92/cdpcli/data/imagecatalog/imagecatalog.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: imagecatalog
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.91
+  version: 0.9.92
   title: Image catalog service
   license:
     name: Apache 2.0
   description: Service for managing custom image catalogs and their associated Cloudera Runtime and FreeIPA images.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.91/cdpcli/data/ml/ml.yaml` & `cdpcli-beta-0.9.92/cdpcli/data/ml/ml.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: ml
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.91
+  version: 0.9.92
   title: Cloudera Machine Learning
   license:
     name: Apache 2.0
   description: Install and manage Cloudera Machine Learning applications.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.91/cdpcli/data/opdb/opdb.yaml` & `cdpcli-beta-0.9.92/cdpcli/data/opdb/opdb.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: opdb
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.91
+  version: 0.9.92
   title: Operational Database service
   license:
     name: Apache 2.0
   description: Interact with the Cloudera Operational Database service
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.91/cdpcli/data/replicationmanager/replicationmanager.yaml` & `cdpcli-beta-0.9.92/cdpcli/data/replicationmanager/replicationmanager.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: replicationmanager
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.91
+  version: 0.9.92
   title: Cloudera Replication Manager Service
   license:
     name: Apache 2.0
   description: Create and manage replication policies using Cloudera Replication Manager.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -392,14 +392,35 @@
           description: Describes a successful response to a valid request.
           schema:
             $ref: '#/definitions/CollectDiagnosticBundleResponse'
         default:
           description: The default response on an error.
           schema:
             $ref: '#/definitions/Error'
+  /api/v1/replicationmanager/getCommandStatus:
+    post:
+      summary: Get the status of the given CM command.
+      description: Return the current status of the given CM command.
+      operationId: getCommandStatus
+      x-mutating: false
+      parameters:
+        - name: input
+          in: body
+          required: true
+          schema:
+            $ref: '#/definitions/GetCommandStatusRequest'
+      responses:
+        200:
+          description: Describes a successful response to a valid request.
+          schema:
+            $ref: '#/definitions/GetCommandStatusResponse'
+        default:
+          description: The default response on an error.
+          schema:
+            $ref: '#/definitions/Error'
 definitions:
   Error:
     type: object
     description: An object returned on an error.
     properties:
       code:
         type: string
@@ -884,14 +905,69 @@
         type: boolean
       startTime:
         description: Start time of the diagnostic bundle collection command.
         type: string
       resultMessage:
         description: Diagnostic bundle collection command result message.
         type: string
+  GetCommandStatusRequest:
+    type: object
+    description: Get the current status of any CM command.
+    required:
+      - clusterCrn
+      - commandId
+    properties:
+      clusterCrn:
+        description: The CRN of the target cluster.
+        type: string
+      commandId:
+        description: ID of a CM command on the cluster.
+        type: string
+  GetCommandStatusResponse:
+    type: object
+    description: Response object for get command status.
+    required:
+      - commandId
+    properties:
+      commandId:
+        description: Id of the CM command.
+        format: int64
+        type: integer
+      success:
+        description: Whether the diagnostic collection is successful.
+        type: boolean
+      active:
+        description: Whether the command is still active.
+        type: boolean
+      name:
+        description: Name of the policy.
+        type: string
+      startTime:
+        description: Start time of the CM command.
+        type: string
+      endTime:
+        description: End time of the CM command.
+        type: string
+      resultDataUrl:
+        description: Some commands have result data URL for downloading the diagnostic bundle. On certain CM versions the bundle download is only available through this URL, but not with download-diagnostic-bundle operation.
+        type: string
+      resultMessage:
+        description: Result message of the command.
+        type: string
+      bundleStatus:
+        description: The current status of the command.
+        type: string
+        enum:
+          - IN_PROGRESS
+          - DOWNLOADABLE_WITH_URL
+          - DOWNLOADABLE_WITH_CLI
+          - FAILED
+      bundleStatusMessage:
+        description: Further information about the current command status.
+        type: string
   RerunPolicyRequest:
     type: object
     description: Request object for rerun policy.
     required:
       - clusterCrn
       - policyName
     properties:
```

### Comparing `cdpcli-beta-0.9.91/cdpcli/doc/docstringparser.py` & `cdpcli-beta-0.9.92/cdpcli/doc/docstringparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/doc/restdoc.py` & `cdpcli-beta-0.9.92/cdpcli/doc/restdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/doc/style.py` & `cdpcli-beta-0.9.92/cdpcli/doc/style.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/docs.py` & `cdpcli-beta-0.9.92/cdpcli/docs.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/endpoint.py` & `cdpcli-beta-0.9.92/cdpcli/endpoint.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/examples/configure/_description.rst` & `cdpcli-beta-0.9.92/cdpcli/examples/configure/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/examples/configure/get/_description.rst` & `cdpcli-beta-0.9.92/cdpcli/examples/configure/get/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/examples/configure/get/_examples.rst` & `cdpcli-beta-0.9.92/cdpcli/examples/configure/get/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/examples/configure/set/_description.rst` & `cdpcli-beta-0.9.92/cdpcli/examples/configure/set/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/examples/configure/set/_examples.rst` & `cdpcli-beta-0.9.92/cdpcli/examples/configure/set/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/exceptions.py` & `cdpcli-beta-0.9.92/cdpcli/exceptions.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/__init__.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/arguments.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/arguments.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/cliinputjson.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/cliinputjson.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/commands.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/commands.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/configure/__init__.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/configure/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/configure/classify.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/configure/classify.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/configure/configure.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/configure/configure.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/configure/get.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/configure/get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/configure/list.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/configure/list.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/configure/set.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/configure/set.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/df/__init__.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/df/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/df/createdeployment.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/df/createdeployment.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/df/register.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/df/register.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/generatecliskeleton.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/interactivelogin.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/interactivelogin.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/logout.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/logout.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/paginate.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/redirect.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/redirect.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/refdoc.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/refdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/workload.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/workload.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/extensions/writer.py` & `cdpcli-beta-0.9.92/cdpcli/extensions/writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/formatter.py` & `cdpcli-beta-0.9.92/cdpcli/formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/help.py` & `cdpcli-beta-0.9.92/cdpcli/help.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/loader.py` & `cdpcli-beta-0.9.92/cdpcli/loader.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/main.py` & `cdpcli-beta-0.9.92/cdpcli/main.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/model.py` & `cdpcli-beta-0.9.92/cdpcli/model.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/paginate.py` & `cdpcli-beta-0.9.92/cdpcli/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/paramfile.py` & `cdpcli-beta-0.9.92/cdpcli/paramfile.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/paramformfactor.py` & `cdpcli-beta-0.9.92/cdpcli/paramformfactor.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/parser.py` & `cdpcli-beta-0.9.92/cdpcli/parser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/retryhandler.py` & `cdpcli-beta-0.9.92/cdpcli/retryhandler.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/schema.py` & `cdpcli-beta-0.9.92/cdpcli/schema.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/serialize.py` & `cdpcli-beta-0.9.92/cdpcli/serialize.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/shorthand.py` & `cdpcli-beta-0.9.92/cdpcli/shorthand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/signers.py` & `cdpcli-beta-0.9.92/cdpcli/signers.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/table.py` & `cdpcli-beta-0.9.92/cdpcli/table.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/text.py` & `cdpcli-beta-0.9.92/cdpcli/text.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/textwriter.py` & `cdpcli-beta-0.9.92/cdpcli/textwriter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/thirdparty/six.py` & `cdpcli-beta-0.9.92/cdpcli/thirdparty/six.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/translate.py` & `cdpcli-beta-0.9.92/cdpcli/translate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/utils.py` & `cdpcli-beta-0.9.92/cdpcli/utils.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli/validate.py` & `cdpcli-beta-0.9.92/cdpcli/validate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/cdpcli_beta.egg-info/PKG-INFO` & `cdpcli-beta-0.9.92/cdpcli_beta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdpcli-beta
-Version: 0.9.91
+Version: 0.9.92
 Summary: Cloudera CDP Command Line Interface (BETA)
 Home-page: https://console.cdp.cloudera.com/
 Author: Cloudera, Inc.
 License: Apache License 2.0
 Description: # Cloudera CDP Command Line Interface
         
         This package provides a unified command line interface to the Cloudera Data
```

### Comparing `cdpcli-beta-0.9.91/cdpcli_beta.egg-info/SOURCES.txt` & `cdpcli-beta-0.9.92/cdpcli_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/setup.py` & `cdpcli-beta-0.9.92/setup.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/setup_common.py` & `cdpcli-beta-0.9.92/setup_common.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/__init__.py` & `cdpcli-beta-0.9.92/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/cdp/__init__.py` & `cdpcli-beta-0.9.92/tests/unit/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/extensions/__init__.py` & `cdpcli-beta-0.9.92/tests/unit/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/extensions/configure/test_classify.py` & `cdpcli-beta-0.9.92/tests/unit/extensions/configure/test_classify.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/extensions/configure/test_configure.py` & `cdpcli-beta-0.9.92/tests/unit/extensions/configure/test_configure.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/extensions/configure/test_get.py` & `cdpcli-beta-0.9.92/tests/unit/extensions/configure/test_get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/extensions/configure/test_list.py` & `cdpcli-beta-0.9.92/tests/unit/extensions/configure/test_list.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/extensions/configure/test_set.py` & `cdpcli-beta-0.9.92/tests/unit/extensions/configure/test_set.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/extensions/df/test_createdeployment.py` & `cdpcli-beta-0.9.92/tests/unit/extensions/df/test_createdeployment.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/extensions/df/test_upload_file.py` & `cdpcli-beta-0.9.92/tests/unit/extensions/df/test_upload_file.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/extensions/test_cliinputjson.py` & `cdpcli-beta-0.9.92/tests/unit/extensions/test_cliinputjson.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/extensions/test_df.py` & `cdpcli-beta-0.9.92/tests/unit/extensions/test_df.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/extensions/test_generatecliskeleton.py` & `cdpcli-beta-0.9.92/tests/unit/extensions/test_generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/extensions/test_interactivelogin.py` & `cdpcli-beta-0.9.92/tests/unit/extensions/test_interactivelogin.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/extensions/test_logout.py` & `cdpcli-beta-0.9.92/tests/unit/extensions/test_logout.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/extensions/test_operation_extension.py` & `cdpcli-beta-0.9.92/tests/unit/extensions/test_operation_extension.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/extensions/test_paginate.py` & `cdpcli-beta-0.9.92/tests/unit/extensions/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/extensions/test_redirect.py` & `cdpcli-beta-0.9.92/tests/unit/extensions/test_redirect.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/extensions/test_workload.py` & `cdpcli-beta-0.9.92/tests/unit/extensions/test_workload.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/extensions/test_writer.py` & `cdpcli-beta-0.9.92/tests/unit/extensions/test_writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_argparser.py` & `cdpcli-beta-0.9.92/tests/unit/test_argparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_argprocess.py` & `cdpcli-beta-0.9.92/tests/unit/test_argprocess.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_auth.py` & `cdpcli-beta-0.9.92/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_cli_data.py` & `cdpcli-beta-0.9.92/tests/unit/test_cli_data.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_client.py` & `cdpcli-beta-0.9.92/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_completer.py` & `cdpcli-beta-0.9.92/tests/unit/test_completer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_credentials.py` & `cdpcli-beta-0.9.92/tests/unit/test_credentials.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_docs.py` & `cdpcli-beta-0.9.92/tests/unit/test_docs.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_endpoint.py` & `cdpcli-beta-0.9.92/tests/unit/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_help.py` & `cdpcli-beta-0.9.92/tests/unit/test_help.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_loaders.py` & `cdpcli-beta-0.9.92/tests/unit/test_loaders.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_model.py` & `cdpcli-beta-0.9.92/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_paginate.py` & `cdpcli-beta-0.9.92/tests/unit/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_paramfile.py` & `cdpcli-beta-0.9.92/tests/unit/test_paramfile.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_protocol.py` & `cdpcli-beta-0.9.92/tests/unit/test_protocol.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_retryhandler.py` & `cdpcli-beta-0.9.92/tests/unit/test_retryhandler.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_shorthand.py` & `cdpcli-beta-0.9.92/tests/unit/test_shorthand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_signers.py` & `cdpcli-beta-0.9.92/tests/unit/test_signers.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_table_formatter.py` & `cdpcli-beta-0.9.92/tests/unit/test_table_formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_utils.py` & `cdpcli-beta-0.9.92/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/tests/unit/test_validate.py` & `cdpcli-beta-0.9.92/tests/unit/test_validate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.91/versioneer.py` & `cdpcli-beta-0.9.92/versioneer.py`

 * *Files identical despite different names*

