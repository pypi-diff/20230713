# Comparing `tmp/target-miso-0.9.4rc1.tar.gz` & `tmp/target-miso-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/target-miso/target-miso/dist/tmpvkl08yot/target-miso-0.9.4rc1.tar", last modified: Fri Aug  5 04:20:32 2022, max compression
+gzip compressed data, was "/home/runner/work/target-miso/target-miso/dist/.tmp-fu3lojy6/target-miso-0.9.5.tar", last modified: Thu Jul 13 15:04:45 2023, max compression
```

## Comparing `target-miso-0.9.4rc1.tar` & `target-miso-0.9.5.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 04:20:32.000000 target-miso-0.9.4rc1/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-08-05 04:20:18.000000 target-miso-0.9.4rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-05 04:20:18.000000 target-miso-0.9.4rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4295 2022-08-05 04:20:32.000000 target-miso-0.9.4rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3791 2022-08-05 04:20:18.000000 target-miso-0.9.4rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-05 04:20:24.000000 target-miso-0.9.4rc1/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-08-05 04:20:18.000000 target-miso-0.9.4rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      783 2022-08-05 04:20:32.000000 target-miso-0.9.4rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-08-05 04:20:18.000000 target-miso-0.9.4rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 04:20:32.000000 target-miso-0.9.4rc1/target_miso/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-05 04:20:18.000000 target-miso-0.9.4rc1/target_miso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1818 2022-08-05 04:20:18.000000 target-miso-0.9.4rc1/target_miso/extensions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4458 2022-08-05 04:20:18.000000 target-miso-0.9.4rc1/target_miso/miso.py
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-08-05 04:20:18.000000 target-miso-0.9.4rc1/target_miso/py_extensions.py
--rw-r--r--   0 runner    (1001) docker     (121)     9845 2022-08-05 04:20:18.000000 target-miso-0.9.4rc1/target_miso/target.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 04:20:32.000000 target-miso-0.9.4rc1/target_miso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4295 2022-08-05 04:20:32.000000 target-miso-0.9.4rc1/target_miso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-08-05 04:20:32.000000 target-miso-0.9.4rc1/target_miso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-05 04:20:32.000000 target-miso-0.9.4rc1/target_miso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-08-05 04:20:32.000000 target-miso-0.9.4rc1/target_miso.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-05 04:20:32.000000 target-miso-0.9.4rc1/target_miso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-05 04:20:32.000000 target-miso-0.9.4rc1/target_miso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:04:45.000000 target-miso-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-13 15:04:30.000000 target-miso-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 15:04:30.000000 target-miso-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-13 15:04:45.000000 target-miso-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-13 15:04:30.000000 target-miso-0.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 15:04:39.000000 target-miso-0.9.5/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 15:04:30.000000 target-miso-0.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-13 15:04:45.000000 target-miso-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 15:04:30.000000 target-miso-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:04:45.000000 target-miso-0.9.5/target_miso/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 15:04:30.000000 target-miso-0.9.5/target_miso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-13 15:04:30.000000 target-miso-0.9.5/target_miso/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-13 15:04:30.000000 target-miso-0.9.5/target_miso/miso.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-13 15:04:30.000000 target-miso-0.9.5/target_miso/py_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-13 15:04:30.000000 target-miso-0.9.5/target_miso/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:04:45.000000 target-miso-0.9.5/target_miso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-13 15:04:45.000000 target-miso-0.9.5/target_miso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-13 15:04:45.000000 target-miso-0.9.5/target_miso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:04:45.000000 target-miso-0.9.5/target_miso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-13 15:04:45.000000 target-miso-0.9.5/target_miso.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-13 15:04:45.000000 target-miso-0.9.5/target_miso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 15:04:45.000000 target-miso-0.9.5/target_miso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:04:45.000000 target-miso-0.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-13 15:04:30.000000 target-miso-0.9.5/tests/test_miso_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-13 15:04:30.000000 target-miso-0.9.5/tests/test_persist_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-13 15:04:30.000000 target-miso-0.9.5/tests/test_transform.py
```

### Comparing `target-miso-0.9.4rc1/LICENSE` & `target-miso-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `target-miso-0.9.4rc1/PKG-INFO` & `target-miso-0.9.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-miso
-Version: 0.9.4rc1
+Version: 0.9.5
 Summary: A Singer target for writing data to Miso API
 Home-page: https://github.com/MisoAI/target-miso
 Author: Hash Lin
 Author-email: hashlin@askmiso.com
 License: MIT
 Keywords: singer,singer.io,target,ETL,ELT,MisoAI,Miso,Meltano
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -46,20 +46,21 @@
 Make sure to run `meltano install` to install the dependency.
 
 ## Configuration
 
 The config object accepts the following properties:
 
 | name | required | default | explanation |
-| --- | --- | --- |
+| --- | --- | --- | --- |
 | api_server | no | https://api.askmiso.com | The Miso API server host. |
 | api_key | yes | | Your Miso API key. |
 | template_folder | yes | | Where you keep the template files. The path is relative to Meltano project directory. |
 | use_async | no | False | Whether to send request in asynchronous mode. |
 | dry_run | no | False | Whether to send request in dry-run mode. |
+| write_record_limit | no | 100 | The maximum number of records to be written. |
 
 ## Replication methods
 
 Currently, this target supports `FULL_TABLE` and `INCREMENTAL` replication methods. `LOG_BASED` is not yet supported.
 
 ## Template
```

#### html2text {}

```diff
@@ -1,52 +1,54 @@
-Metadata-Version: 2.1 Name: target-miso Version: 0.9.4rc1 Summary: A Singer
-target for writing data to Miso API Home-page: https://github.com/MisoAI/
-target-miso Author: Hash Lin Author-email: hashlin@askmiso.com License: MIT
-Keywords: singer,singer.io,target,ETL,ELT,MisoAI,Miso,Meltano Classifier:
-Programming Language :: Python :: 3 :: Only Classifier: License :: OSI Approved
-:: MIT License Classifier: Operating System :: OS Independent Description-
-Content-Type: text/markdown License-File: LICENSE # target-miso This package is
-a [Singer](https://singer.io) target that sends data to Miso's [Data API]
-(https://api.askmiso.com). Being a singer target, you can integrate it into
-your data pipeline using your favorite DataOps framework, for instance,
-[Meltano](https://meltano.com/).
+Metadata-Version: 2.1 Name: target-miso Version: 0.9.5 Summary: A Singer target
+for writing data to Miso API Home-page: https://github.com/MisoAI/target-miso
+Author: Hash Lin Author-email: hashlin@askmiso.com License: MIT Keywords:
+singer,singer.io,target,ETL,ELT,MisoAI,Miso,Meltano Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Description-Content-
+Type: text/markdown License-File: LICENSE # target-miso This package is a
+[Singer](https://singer.io) target that sends data to Miso's [Data API](https:/
+/api.askmiso.com). Being a singer target, you can integrate it into your data
+pipeline using your favorite DataOps framework, for instance, [Meltano](https:/
+/meltano.com/).
 [PyPI] [PyPI - Python Version: 3] [PyPI_-_License:_MIT]
 # Use with Meltano Follow the steps below to setup `target-miso` in your
 Meltano project. Or see the most essential project example [here](https://
 github.com/MisoAI/target-miso/tree/main/examples/csv). ## Setup Setup
 `meltano.yml` like this: ```yml # ... plugins: # ... loaders: - name: target-
 miso namespace: target_miso pip_url: target-miso executable: target-miso
 config: template_folder: template api_key: your_miso_api_key ``` Make sure to
 run `meltano install` to install the dependency. ## Configuration The config
 object accepts the following properties: | name | required | default |
-explanation | | --- | --- | --- | | api_server | no | https://api.askmiso.com |
-The Miso API server host. | | api_key | yes | | Your Miso API key. | |
-template_folder | yes | | Where you keep the template files. The path is
-relative to Meltano project directory. | | use_async | no | False | Whether to
-send request in asynchronous mode. | | dry_run | no | False | Whether to send
-request in dry-run mode. | ## Replication methods Currently, this target
-supports `FULL_TABLE` and `INCREMENTAL` replication methods. `LOG_BASED` is not
-yet supported. ## Template To specify how records are transformed into payloads
-of Miso API, for each stream from the tap, put a corresponding [jinja2](https:/
-/jinja.palletsprojects.com/en/3.1.x/) template file in your template folder.
-For example, given a stream `product`, put a template file `product.jinja` like
-this: ```nunjucks { "product_id": "{{ data.uuid }}", "created_at": "{
-{ data.created_at | datetime_format }}", "title": "{{ data.title }}",
-"description": "{{ data.description }}", "categories": "{{ data.category |
-convert_categories }}", "custom_attributes": { "vender": "{{ data.vender if
-data.vender }}" } } ``` ### Rules on output data types Miso takes 3 kinds of
-data records: `user`, `product`, and `interaction`. A record is classified into
-one of these type by the following rules: * If the payload contains the `type`
-field, it is an interaction record. * If the payload contains the `user_id`
-field, it is a user record. * If the payload contains the `product_id` field,
-it is a product record. ### Built-in filters Target Miso comes with a few
-built-in filters that can be used in template expressions: ####
-`datetime_format` Takes a string in any format compatible with [dateparser]
-(https://dateparser.readthedocs.io/en/latest/) and output in ISO format, which
-is desired by Miso API. #### `list_of_str` Wrap a string to a singleton list of
-string. For example, `"apple"` to `["apple"]`. #### `convert_categories` Wrap a
-string to a singleton double-layered list of string. For example, `"apple"` to
-`[["apple"]]`. #### `remove_symbol` 1. Convert an int to string. 1. Strip off
-some special characters from input string, including: `"`, `\`, `\\N`, `â`,
-`\r\n`, `\n`, `\r`. #### `split` Split a string into a list by comma. ####
-`fix_url` Encode (as URL component) the path component of a URL string. ####
-`jsonify` Serialize an obj to a JSON string. ---- Copyright © 2021 Miso Corp.
+explanation | | --- | --- | --- | --- | | api_server | no | https://
+api.askmiso.com | The Miso API server host. | | api_key | yes | | Your Miso API
+key. | | template_folder | yes | | Where you keep the template files. The path
+is relative to Meltano project directory. | | use_async | no | False | Whether
+to send request in asynchronous mode. | | dry_run | no | False | Whether to
+send request in dry-run mode. | | write_record_limit | no | 100 | The maximum
+number of records to be written. | ## Replication methods Currently, this
+target supports `FULL_TABLE` and `INCREMENTAL` replication methods. `LOG_BASED`
+is not yet supported. ## Template To specify how records are transformed into
+payloads of Miso API, for each stream from the tap, put a corresponding
+[jinja2](https://jinja.palletsprojects.com/en/3.1.x/) template file in your
+template folder. For example, given a stream `product`, put a template file
+`product.jinja` like this: ```nunjucks { "product_id": "{{ data.uuid }}",
+"created_at": "{{ data.created_at | datetime_format }}", "title": "{
+{ data.title }}", "description": "{{ data.description }}", "categories": "{
+{ data.category | convert_categories }}", "custom_attributes": { "vender": "{
+{ data.vender if data.vender }}" } } ``` ### Rules on output data types Miso
+takes 3 kinds of data records: `user`, `product`, and `interaction`. A record
+is classified into one of these type by the following rules: * If the payload
+contains the `type` field, it is an interaction record. * If the payload
+contains the `user_id` field, it is a user record. * If the payload contains
+the `product_id` field, it is a product record. ### Built-in filters Target
+Miso comes with a few built-in filters that can be used in template
+expressions: #### `datetime_format` Takes a string in any format compatible
+with [dateparser](https://dateparser.readthedocs.io/en/latest/) and output in
+ISO format, which is desired by Miso API. #### `list_of_str` Wrap a string to a
+singleton list of string. For example, `"apple"` to `["apple"]`. ####
+`convert_categories` Wrap a string to a singleton double-layered list of
+string. For example, `"apple"` to `[["apple"]]`. #### `remove_symbol` 1.
+Convert an int to string. 1. Strip off some special characters from input
+string, including: `"`, `\`, `\\N`, `â`, `\r\n`, `\n`, `\r`. #### `split`
+Split a string into a list by comma. #### `fix_url` Encode (as URL component)
+the path component of a URL string. #### `jsonify` Serialize an obj to a JSON
+string. ---- Copyright © 2021 Miso Corp.
```

### Comparing `target-miso-0.9.4rc1/README.md` & `target-miso-0.9.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -31,20 +31,21 @@
 Make sure to run `meltano install` to install the dependency.
 
 ## Configuration
 
 The config object accepts the following properties:
 
 | name | required | default | explanation |
-| --- | --- | --- |
+| --- | --- | --- | --- |
 | api_server | no | https://api.askmiso.com | The Miso API server host. |
 | api_key | yes | | Your Miso API key. |
 | template_folder | yes | | Where you keep the template files. The path is relative to Meltano project directory. |
 | use_async | no | False | Whether to send request in asynchronous mode. |
 | dry_run | no | False | Whether to send request in dry-run mode. |
+| write_record_limit | no | 100 | The maximum number of records to be written. |
 
 ## Replication methods
 
 Currently, this target supports `FULL_TABLE` and `INCREMENTAL` replication methods. `LOG_BASED` is not yet supported.
 
 ## Template
```

#### html2text {}

```diff
@@ -7,39 +7,41 @@
 Meltano project. Or see the most essential project example [here](https://
 github.com/MisoAI/target-miso/tree/main/examples/csv). ## Setup Setup
 `meltano.yml` like this: ```yml # ... plugins: # ... loaders: - name: target-
 miso namespace: target_miso pip_url: target-miso executable: target-miso
 config: template_folder: template api_key: your_miso_api_key ``` Make sure to
 run `meltano install` to install the dependency. ## Configuration The config
 object accepts the following properties: | name | required | default |
-explanation | | --- | --- | --- | | api_server | no | https://api.askmiso.com |
-The Miso API server host. | | api_key | yes | | Your Miso API key. | |
-template_folder | yes | | Where you keep the template files. The path is
-relative to Meltano project directory. | | use_async | no | False | Whether to
-send request in asynchronous mode. | | dry_run | no | False | Whether to send
-request in dry-run mode. | ## Replication methods Currently, this target
-supports `FULL_TABLE` and `INCREMENTAL` replication methods. `LOG_BASED` is not
-yet supported. ## Template To specify how records are transformed into payloads
-of Miso API, for each stream from the tap, put a corresponding [jinja2](https:/
-/jinja.palletsprojects.com/en/3.1.x/) template file in your template folder.
-For example, given a stream `product`, put a template file `product.jinja` like
-this: ```nunjucks { "product_id": "{{ data.uuid }}", "created_at": "{
-{ data.created_at | datetime_format }}", "title": "{{ data.title }}",
-"description": "{{ data.description }}", "categories": "{{ data.category |
-convert_categories }}", "custom_attributes": { "vender": "{{ data.vender if
-data.vender }}" } } ``` ### Rules on output data types Miso takes 3 kinds of
-data records: `user`, `product`, and `interaction`. A record is classified into
-one of these type by the following rules: * If the payload contains the `type`
-field, it is an interaction record. * If the payload contains the `user_id`
-field, it is a user record. * If the payload contains the `product_id` field,
-it is a product record. ### Built-in filters Target Miso comes with a few
-built-in filters that can be used in template expressions: ####
-`datetime_format` Takes a string in any format compatible with [dateparser]
-(https://dateparser.readthedocs.io/en/latest/) and output in ISO format, which
-is desired by Miso API. #### `list_of_str` Wrap a string to a singleton list of
-string. For example, `"apple"` to `["apple"]`. #### `convert_categories` Wrap a
-string to a singleton double-layered list of string. For example, `"apple"` to
-`[["apple"]]`. #### `remove_symbol` 1. Convert an int to string. 1. Strip off
-some special characters from input string, including: `"`, `\`, `\\N`, `â`,
-`\r\n`, `\n`, `\r`. #### `split` Split a string into a list by comma. ####
-`fix_url` Encode (as URL component) the path component of a URL string. ####
-`jsonify` Serialize an obj to a JSON string. ---- Copyright © 2021 Miso Corp.
+explanation | | --- | --- | --- | --- | | api_server | no | https://
+api.askmiso.com | The Miso API server host. | | api_key | yes | | Your Miso API
+key. | | template_folder | yes | | Where you keep the template files. The path
+is relative to Meltano project directory. | | use_async | no | False | Whether
+to send request in asynchronous mode. | | dry_run | no | False | Whether to
+send request in dry-run mode. | | write_record_limit | no | 100 | The maximum
+number of records to be written. | ## Replication methods Currently, this
+target supports `FULL_TABLE` and `INCREMENTAL` replication methods. `LOG_BASED`
+is not yet supported. ## Template To specify how records are transformed into
+payloads of Miso API, for each stream from the tap, put a corresponding
+[jinja2](https://jinja.palletsprojects.com/en/3.1.x/) template file in your
+template folder. For example, given a stream `product`, put a template file
+`product.jinja` like this: ```nunjucks { "product_id": "{{ data.uuid }}",
+"created_at": "{{ data.created_at | datetime_format }}", "title": "{
+{ data.title }}", "description": "{{ data.description }}", "categories": "{
+{ data.category | convert_categories }}", "custom_attributes": { "vender": "{
+{ data.vender if data.vender }}" } } ``` ### Rules on output data types Miso
+takes 3 kinds of data records: `user`, `product`, and `interaction`. A record
+is classified into one of these type by the following rules: * If the payload
+contains the `type` field, it is an interaction record. * If the payload
+contains the `user_id` field, it is a user record. * If the payload contains
+the `product_id` field, it is a product record. ### Built-in filters Target
+Miso comes with a few built-in filters that can be used in template
+expressions: #### `datetime_format` Takes a string in any format compatible
+with [dateparser](https://dateparser.readthedocs.io/en/latest/) and output in
+ISO format, which is desired by Miso API. #### `list_of_str` Wrap a string to a
+singleton list of string. For example, `"apple"` to `["apple"]`. ####
+`convert_categories` Wrap a string to a singleton double-layered list of
+string. For example, `"apple"` to `[["apple"]]`. #### `remove_symbol` 1.
+Convert an int to string. 1. Strip off some special characters from input
+string, including: `"`, `\`, `\\N`, `â`, `\r\n`, `\n`, `\r`. #### `split`
+Split a string into a list by comma. #### `fix_url` Encode (as URL component)
+the path component of a URL string. #### `jsonify` Serialize an obj to a JSON
+string. ---- Copyright © 2021 Miso Corp.
```

### Comparing `target-miso-0.9.4rc1/setup.cfg` & `target-miso-0.9.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `target-miso-0.9.4rc1/target_miso/extensions.py` & `target-miso-0.9.5/target_miso/extensions.py`

 * *Files identical despite different names*

### Comparing `target-miso-0.9.4rc1/target_miso/miso.py` & `target-miso-0.9.5/target_miso/miso.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         raise ValueError(f'This record is not product, user, nor interaction: {record}')
     return data_type
 
 def find_erroneous_record(res_text):
     return sorted(set([int(x) for x in re.findall('data\.(\d+)\.', res_text)]))
 
 class MisoWriter:
-    def __init__(self, api_server: str, api_key: str, use_async: bool, dry_run: bool):
+    def __init__(self, api_server: str, api_key: str, use_async: bool, dry_run: bool, write_record_limit: int = 100):
         self.type_to_buffer = {'products': [], 'interactions': [], 'users': []}
 
         retry_strategy = Retry(
             total=3,
             status_forcelist=[401, 429, 500, 502, 503, 504, 403],
             allowed_methods=["HEAD", "GET", "OPTIONS", "POST"],
             backoff_factor=1,
@@ -39,14 +39,15 @@
         adapter = HTTPAdapter(max_retries=retry_strategy)
         self.session: requests.Session = requests.Session()
         self.session.mount("https://", adapter)
         self.api_server = api_server
         self.api_key = api_key
         self.use_async = use_async
         self.dry_run = dry_run
+        self.write_record_limit = write_record_limit
 
     def _send_request(self, data: List[Dict], data_type: str):
         logger.info("try to send %s requests to %s-data-api, async:%s.",
                     len(data), data_type, self.use_async)
         try:
             response = self.session.post(
                 '{}/v1/{}?api_key={}{}{}'.format(self.api_server, data_type, self.api_key,
@@ -95,15 +96,15 @@
         ret.raise_for_status()
 
     def write_record(self, record: Dict):
         """ Write record to Miso """
         data_type = check_miso_data_type(record)
         buffer = self.type_to_buffer[data_type]
         buffer.append(record)
-        limit = 1000 if data_type == 'interactions' else 200
+        limit = 1000 if data_type == 'interactions' else self.write_record_limit
         if len(buffer) >= limit:
             self._send_request(buffer, data_type)
             buffer.clear()
 
     def flush(self):
         for data_type in list(self.type_to_buffer):
             buf = self.type_to_buffer[data_type]
```

### Comparing `target-miso-0.9.4rc1/target_miso/py_extensions.py` & `target-miso-0.9.5/target_miso/py_extensions.py`

 * *Files identical despite different names*

### Comparing `target-miso-0.9.4rc1/target_miso/target.py` & `target-miso-0.9.5/target_miso/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,16 +187,17 @@
     params = singer.utils.parse_args({'template_folder', 'api_key'})
 
     # load Miso API parameters
     api_server = params.config.get('api_server') or 'https://api.askmiso.com'
     api_key = params.config['api_key']
     use_async = is_truthy(params.config.get('use_async'))
     dry_run = is_truthy(params.config.get('dry_run'))
+    write_record_limit = int(params.config.get('write_record_limit', 100))
 
-    miso_client = MisoWriter(api_server, api_key, use_async, dry_run)
+    miso_client = MisoWriter(api_server, api_key, use_async, dry_run, write_record_limit)
     extra_config = {
         'insert_only': is_truthy(params.config.get('insert_only'))
     }
 
     if 'sentry_dsn' in params.config:
         sentry_sdk.init(dsn=params.config['sentry_dsn'])
         if 'sentry_source' in params.config:
```

### Comparing `target-miso-0.9.4rc1/target_miso.egg-info/PKG-INFO` & `target-miso-0.9.5/target_miso.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-miso
-Version: 0.9.4rc1
+Version: 0.9.5
 Summary: A Singer target for writing data to Miso API
 Home-page: https://github.com/MisoAI/target-miso
 Author: Hash Lin
 Author-email: hashlin@askmiso.com
 License: MIT
 Keywords: singer,singer.io,target,ETL,ELT,MisoAI,Miso,Meltano
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -46,20 +46,21 @@
 Make sure to run `meltano install` to install the dependency.
 
 ## Configuration
 
 The config object accepts the following properties:
 
 | name | required | default | explanation |
-| --- | --- | --- |
+| --- | --- | --- | --- |
 | api_server | no | https://api.askmiso.com | The Miso API server host. |
 | api_key | yes | | Your Miso API key. |
 | template_folder | yes | | Where you keep the template files. The path is relative to Meltano project directory. |
 | use_async | no | False | Whether to send request in asynchronous mode. |
 | dry_run | no | False | Whether to send request in dry-run mode. |
+| write_record_limit | no | 100 | The maximum number of records to be written. |
 
 ## Replication methods
 
 Currently, this target supports `FULL_TABLE` and `INCREMENTAL` replication methods. `LOG_BASED` is not yet supported.
 
 ## Template
```

#### html2text {}

```diff
@@ -1,52 +1,54 @@
-Metadata-Version: 2.1 Name: target-miso Version: 0.9.4rc1 Summary: A Singer
-target for writing data to Miso API Home-page: https://github.com/MisoAI/
-target-miso Author: Hash Lin Author-email: hashlin@askmiso.com License: MIT
-Keywords: singer,singer.io,target,ETL,ELT,MisoAI,Miso,Meltano Classifier:
-Programming Language :: Python :: 3 :: Only Classifier: License :: OSI Approved
-:: MIT License Classifier: Operating System :: OS Independent Description-
-Content-Type: text/markdown License-File: LICENSE # target-miso This package is
-a [Singer](https://singer.io) target that sends data to Miso's [Data API]
-(https://api.askmiso.com). Being a singer target, you can integrate it into
-your data pipeline using your favorite DataOps framework, for instance,
-[Meltano](https://meltano.com/).
+Metadata-Version: 2.1 Name: target-miso Version: 0.9.5 Summary: A Singer target
+for writing data to Miso API Home-page: https://github.com/MisoAI/target-miso
+Author: Hash Lin Author-email: hashlin@askmiso.com License: MIT Keywords:
+singer,singer.io,target,ETL,ELT,MisoAI,Miso,Meltano Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Description-Content-
+Type: text/markdown License-File: LICENSE # target-miso This package is a
+[Singer](https://singer.io) target that sends data to Miso's [Data API](https:/
+/api.askmiso.com). Being a singer target, you can integrate it into your data
+pipeline using your favorite DataOps framework, for instance, [Meltano](https:/
+/meltano.com/).
 [PyPI] [PyPI - Python Version: 3] [PyPI_-_License:_MIT]
 # Use with Meltano Follow the steps below to setup `target-miso` in your
 Meltano project. Or see the most essential project example [here](https://
 github.com/MisoAI/target-miso/tree/main/examples/csv). ## Setup Setup
 `meltano.yml` like this: ```yml # ... plugins: # ... loaders: - name: target-
 miso namespace: target_miso pip_url: target-miso executable: target-miso
 config: template_folder: template api_key: your_miso_api_key ``` Make sure to
 run `meltano install` to install the dependency. ## Configuration The config
 object accepts the following properties: | name | required | default |
-explanation | | --- | --- | --- | | api_server | no | https://api.askmiso.com |
-The Miso API server host. | | api_key | yes | | Your Miso API key. | |
-template_folder | yes | | Where you keep the template files. The path is
-relative to Meltano project directory. | | use_async | no | False | Whether to
-send request in asynchronous mode. | | dry_run | no | False | Whether to send
-request in dry-run mode. | ## Replication methods Currently, this target
-supports `FULL_TABLE` and `INCREMENTAL` replication methods. `LOG_BASED` is not
-yet supported. ## Template To specify how records are transformed into payloads
-of Miso API, for each stream from the tap, put a corresponding [jinja2](https:/
-/jinja.palletsprojects.com/en/3.1.x/) template file in your template folder.
-For example, given a stream `product`, put a template file `product.jinja` like
-this: ```nunjucks { "product_id": "{{ data.uuid }}", "created_at": "{
-{ data.created_at | datetime_format }}", "title": "{{ data.title }}",
-"description": "{{ data.description }}", "categories": "{{ data.category |
-convert_categories }}", "custom_attributes": { "vender": "{{ data.vender if
-data.vender }}" } } ``` ### Rules on output data types Miso takes 3 kinds of
-data records: `user`, `product`, and `interaction`. A record is classified into
-one of these type by the following rules: * If the payload contains the `type`
-field, it is an interaction record. * If the payload contains the `user_id`
-field, it is a user record. * If the payload contains the `product_id` field,
-it is a product record. ### Built-in filters Target Miso comes with a few
-built-in filters that can be used in template expressions: ####
-`datetime_format` Takes a string in any format compatible with [dateparser]
-(https://dateparser.readthedocs.io/en/latest/) and output in ISO format, which
-is desired by Miso API. #### `list_of_str` Wrap a string to a singleton list of
-string. For example, `"apple"` to `["apple"]`. #### `convert_categories` Wrap a
-string to a singleton double-layered list of string. For example, `"apple"` to
-`[["apple"]]`. #### `remove_symbol` 1. Convert an int to string. 1. Strip off
-some special characters from input string, including: `"`, `\`, `\\N`, `â`,
-`\r\n`, `\n`, `\r`. #### `split` Split a string into a list by comma. ####
-`fix_url` Encode (as URL component) the path component of a URL string. ####
-`jsonify` Serialize an obj to a JSON string. ---- Copyright © 2021 Miso Corp.
+explanation | | --- | --- | --- | --- | | api_server | no | https://
+api.askmiso.com | The Miso API server host. | | api_key | yes | | Your Miso API
+key. | | template_folder | yes | | Where you keep the template files. The path
+is relative to Meltano project directory. | | use_async | no | False | Whether
+to send request in asynchronous mode. | | dry_run | no | False | Whether to
+send request in dry-run mode. | | write_record_limit | no | 100 | The maximum
+number of records to be written. | ## Replication methods Currently, this
+target supports `FULL_TABLE` and `INCREMENTAL` replication methods. `LOG_BASED`
+is not yet supported. ## Template To specify how records are transformed into
+payloads of Miso API, for each stream from the tap, put a corresponding
+[jinja2](https://jinja.palletsprojects.com/en/3.1.x/) template file in your
+template folder. For example, given a stream `product`, put a template file
+`product.jinja` like this: ```nunjucks { "product_id": "{{ data.uuid }}",
+"created_at": "{{ data.created_at | datetime_format }}", "title": "{
+{ data.title }}", "description": "{{ data.description }}", "categories": "{
+{ data.category | convert_categories }}", "custom_attributes": { "vender": "{
+{ data.vender if data.vender }}" } } ``` ### Rules on output data types Miso
+takes 3 kinds of data records: `user`, `product`, and `interaction`. A record
+is classified into one of these type by the following rules: * If the payload
+contains the `type` field, it is an interaction record. * If the payload
+contains the `user_id` field, it is a user record. * If the payload contains
+the `product_id` field, it is a product record. ### Built-in filters Target
+Miso comes with a few built-in filters that can be used in template
+expressions: #### `datetime_format` Takes a string in any format compatible
+with [dateparser](https://dateparser.readthedocs.io/en/latest/) and output in
+ISO format, which is desired by Miso API. #### `list_of_str` Wrap a string to a
+singleton list of string. For example, `"apple"` to `["apple"]`. ####
+`convert_categories` Wrap a string to a singleton double-layered list of
+string. For example, `"apple"` to `[["apple"]]`. #### `remove_symbol` 1.
+Convert an int to string. 1. Strip off some special characters from input
+string, including: `"`, `\`, `\\N`, `â`, `\r\n`, `\n`, `\r`. #### `split`
+Split a string into a list by comma. #### `fix_url` Encode (as URL component)
+the path component of a URL string. #### `jsonify` Serialize an obj to a JSON
+string. ---- Copyright © 2021 Miso Corp.
```

