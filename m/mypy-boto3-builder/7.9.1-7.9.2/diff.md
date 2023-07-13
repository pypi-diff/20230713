# Comparing `tmp/mypy-boto3-builder-7.9.1.tar.gz` & `tmp/mypy-boto3-builder-7.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-builder-7.9.1.tar", max compression
+gzip compressed data, was "mypy-boto3-builder-7.9.2.tar", max compression
```

## Comparing `mypy-boto3-builder-7.9.1.tar` & `mypy-boto3-builder-7.9.2.tar`

### file list

```diff
@@ -1,323 +1,323 @@
--rw-r--r--   0        0        0     1071 2022-07-15 12:40:11.318768 mypy-boto3-builder-7.9.1/LICENSE
--rw-r--r--   0        0        0     7345 2022-07-15 12:40:11.318768 mypy-boto3-builder-7.9.1/README.md
--rw-r--r--   0        0        0       34 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/__init__.py
--rw-r--r--   0        0        0      116 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/__main__.py
--rw-r--r--   0        0        0     3744 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/cli_parser.py
--rw-r--r--   0        0        0     2431 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/constants.py
--rw-r--r--   0        0        0       33 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/enums/__init__.py
--rw-r--r--   0        0        0      719 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/enums/service_module_name.py
--rw-r--r--   0        0        0       35 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/generators/__init__.py
--rw-r--r--   0        0        0     3479 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/generators/aioboto3_generator.py
--rw-r--r--   0        0        0     3474 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/generators/aiobotocore_generator.py
--rw-r--r--   0        0        0     7621 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/generators/base_generator.py
--rw-r--r--   0        0        0     4848 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/generators/boto3_generator.py
--rw-r--r--   0        0        0       40 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/import_helpers/__init__.py
--rw-r--r--   0        0        0     4842 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/import_helpers/import_record.py
--rw-r--r--   0        0        0     3182 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/import_helpers/import_string.py
--rw-r--r--   0        0        0     1359 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/import_helpers/internal_import_record.py
--rw-r--r--   0        0        0     1006 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/jinja_manager.py
--rw-r--r--   0        0        0      882 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/logger.py
--rw-r--r--   0        0        0     6128 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/main.py
--rw-r--r--   0        0        0     4035 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/package_data.py
--rw-r--r--   0        0        0       49 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/__init__.py
--rw-r--r--   0        0        0     4035 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/aiobotocore_stubs_package.py
--rw-r--r--   0        0        0     6695 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/boto3_stubs_package.py
--rw-r--r--   0        0        0     3036 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/client.py
--rw-r--r--   0        0        0       35 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/docstring_parser/__init__.py
--rw-r--r--   0        0        0     3445 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/docstring_parser/argspec_parser.py
--rw-r--r--   0        0        0    12810 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/docstring_parser/docstring_parser.py
--rw-r--r--   0        0        0     4979 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/docstring_parser/syntax_grammar.py
--rw-r--r--   0        0        0     3804 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/docstring_parser/type_doc_grammar.py
--rw-r--r--   0        0        0     2051 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/docstring_parser/type_doc_line.py
--rw-r--r--   0        0        0     8300 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/docstring_parser/type_value.py
--rw-r--r--   0        0        0     2717 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/fake_service_package.py
--rw-r--r--   0        0        0     2756 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/helpers.py
--rw-r--r--   0        0        0      969 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/master_package.py
--rw-r--r--   0        0        0     1563 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/parse_attributes.py
--rw-r--r--   0        0        0     4264 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/parse_collections.py
--rw-r--r--   0        0        0      753 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/parse_identifiers.py
--rw-r--r--   0        0        0     1272 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/parse_references.py
--rw-r--r--   0        0        0     3213 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/parse_resource.py
--rw-r--r--   0        0        0     3630 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/service_package.py
--rw-r--r--   0        0        0     5760 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/service_resource.py
--rw-r--r--   0        0        0    29972 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/shape_parser.py
--rw-r--r--   0        0        0     5329 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/types_aioboto3_package.py
--rw-r--r--   0        0        0       75 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/postprocessors/__init__.py
--rw-r--r--   0        0        0     6084 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/postprocessors/aiobotocore.py
--rw-r--r--   0        0        0     9230 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/postprocessors/base.py
--rw-r--r--   0        0        0      334 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/postprocessors/botocore.py
--rw-r--r--   0        0        0        0 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/py.typed
--rw-r--r--   0        0        0     5125 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/service_name.py
--rw-r--r--   0        0        0       40 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/__init__.py
--rw-r--r--   0        0        0     3801 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/aiobotocore_stubs_package.py
--rw-r--r--   0        0        0     2048 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/argument.py
--rw-r--r--   0        0        0     1284 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/attribute.py
--rw-r--r--   0        0        0     5097 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/boto3_stubs_package.py
--rw-r--r--   0        0        0      354 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/botocore_stubs_package.py
--rw-r--r--   0        0        0     3610 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/class_record.py
--rw-r--r--   0        0        0     4436 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/client.py
--rw-r--r--   0        0        0     1696 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/collection.py
--rw-r--r--   0        0        0     4005 2022-07-15 12:40:11.326768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/function.py
--rw-r--r--   0        0        0     1238 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/master_package.py
--rw-r--r--   0        0        0      479 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/method.py
--rw-r--r--   0        0        0     2491 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/package.py
--rw-r--r--   0        0        0     2008 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/paginator.py
--rw-r--r--   0        0        0     1495 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/resource.py
--rw-r--r--   0        0        0    13580 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/service_package.py
--rw-r--r--   0        0        0     5729 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/service_resource.py
--rw-r--r--   0        0        0     2903 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/types_aioboto3_package.py
--rw-r--r--   0        0        0     1853 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/waiter.py
--rw-r--r--   0        0        0       33 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/__init__.py
--rw-r--r--   0        0        0      184 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/__init__.pyi
--rw-r--r--   0        0        0        0 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/dynamodb/__init__.pyi
--rw-r--r--   0        0        0     1241 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/dynamodb/table.pyi
--rw-r--r--   0        0        0        0 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/experimental/__init__.pyi
--rw-r--r--   0        0        0      636 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/experimental/async_chalice.pyi
--rw-r--r--   0        0        0        0 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/resources/__init__.pyi
--rw-r--r--   0        0        0     1085 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/resources/action.pyi
--rw-r--r--   0        0        0      476 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/resources/base.pyi
--rw-r--r--   0        0        0     1372 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/resources/collection.pyi
--rw-r--r--   0        0        0      585 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/resources/factory.pyi
--rw-r--r--   0        0        0      580 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/resources/response.pyi
--rw-r--r--   0        0        0        0 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/s3/__init__.pyi
--rw-r--r--   0        0        0     3860 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/s3/cse.pyi
--rw-r--r--   0        0        0     1961 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/s3/inject.pyi
--rw-r--r--   0        0        0     3156 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/session.pyi
--rw-r--r--   0        0        0       17 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/__init__.pyi
--rw-r--r--   0        0        0       96 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/args.pyi
--rw-r--r--   0        0        0     1155 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/client.pyi
--rw-r--r--   0        0        0      300 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/config.pyi
--rw-r--r--   0        0        0     5565 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/credentials.pyi
--rw-r--r--   0        0        0      466 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/discovery.pyi
--rw-r--r--   0        0        0     1390 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/endpoint.pyi
--rw-r--r--   0        0        0      404 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/eventstream.pyi
--rw-r--r--   0        0        0      595 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/handlers.pyi
--rw-r--r--   0        0        0      261 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/hooks.pyi
--rw-r--r--   0        0        0      797 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/httpsession.pyi
--rw-r--r--   0        0        0      711 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/paginate.pyi
--rw-r--r--   0        0        0      735 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/parsers.pyi
--rw-r--r--   0        0        0     1219 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/response.pyi
--rw-r--r--   0        0        0     2512 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/session.pyi
--rw-r--r--   0        0        0     2171 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/signers.pyi
--rw-r--r--   0        0        0     1792 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/utils.pyi
--rw-r--r--   0        0        0      570 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/waiter.pyi
--rw-r--r--   0        0        0     1701 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/__init__.pyi
--rw-r--r--   0        0        0      151 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/compat.pyi
--rw-r--r--   0        0        0       99 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/docs/__init__.pyi
--rw-r--r--   0        0        0      934 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/docs/utils.pyi
--rw-r--r--   0        0        0        0 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/dynamodb/__init__.pyi
--rw-r--r--   0        0        0     4582 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/dynamodb/conditions.pyi
--rw-r--r--   0        0        0      994 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/dynamodb/table.pyi
--rw-r--r--   0        0        0     1705 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/dynamodb/transform.pyi
--rw-r--r--   0        0        0     1332 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/dynamodb/types.pyi
--rw-r--r--   0        0        0        0 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/ec2/__init__.pyi
--rw-r--r--   0        0        0      361 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/ec2/createtags.pyi
--rw-r--r--   0        0        0      204 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/ec2/deletetags.pyi
--rw-r--r--   0        0        0     1253 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/exceptions.pyi
--rw-r--r--   0        0        0        0 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/resources/__init__.pyi
--rw-r--r--   0        0        0     1535 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/resources/action.pyi
--rw-r--r--   0        0        0     1094 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/resources/base.pyi
--rw-r--r--   0        0        0     1922 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/resources/collection.pyi
--rw-r--r--   0        0        0      496 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/resources/factory.pyi
--rw-r--r--   0        0        0     3607 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/resources/model.pyi
--rw-r--r--   0        0        0      565 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/resources/params.pyi
--rw-r--r--   0        0        0     1607 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/resources/response.pyi
--rw-r--r--   0        0        0        0 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/s3/__init__.pyi
--rw-r--r--   0        0        0     2251 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/s3/transfer.pyi
--rw-r--r--   0        0        0     2917 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/session.pyi
--rw-r--r--   0        0        0      779 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/utils.pyi
--rw-r--r--   0        0        0      580 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/__init__.pyi
--rw-r--r--   0        0        0     2170 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/args.pyi
--rw-r--r--   0        0        0     4202 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/auth.pyi
--rw-r--r--   0        0        0     3676 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/awsrequest.pyi
--rw-r--r--   0        0        0     5548 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/client.pyi
--rw-r--r--   0        0        0     2277 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/compat.pyi
--rw-r--r--   0        0        0     2279 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/config.pyi
--rw-r--r--   0        0        0      274 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/configloader.pyi
--rw-r--r--   0        0        0     3479 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/configprovider.pyi
--rw-r--r--   0        0        0    10847 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/credentials.pyi
--rw-r--r--   0        0        0        0 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/crt/__init__.pyi
--rw-r--r--   0        0        0     2077 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/crt/auth.pyi
--rw-r--r--   0        0        0     2173 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/discovery.pyi
--rw-r--r--   0        0        0     2184 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/endpoint.pyi
--rw-r--r--   0        0        0      708 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/errorfactory.pyi
--rw-r--r--   0        0        0     2905 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/eventstream.pyi
--rw-r--r--   0        0        0    20633 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/exceptions.pyi
--rw-r--r--   0        0        0     6183 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/handlers.pyi
--rw-r--r--   0        0        0      521 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/history.pyi
--rw-r--r--   0        0        0     2792 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/hooks.pyi
--rw-r--r--   0        0        0     1947 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/httpsession.pyi
--rw-r--r--   0        0        0     1862 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/loaders.pyi
--rw-r--r--   0        0        0     5461 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/model.pyi
--rw-r--r--   0        0        0     2309 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/monitoring.pyi
--rw-r--r--   0        0        0     1697 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/paginate.pyi
--rw-r--r--   0        0        0     2097 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/parsers.pyi
--rw-r--r--   0        0        0     1522 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/regions.pyi
--rw-r--r--   0        0        0     1070 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/response.pyi
--rw-r--r--   0        0        0        0 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/retries/__init__.pyi
--rw-r--r--   0        0        0      805 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/retries/adaptive.pyi
--rw-r--r--   0        0        0      185 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/retries/base.pyi
--rw-r--r--   0        0        0      652 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/retries/bucket.pyi
--rw-r--r--   0        0        0      348 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/retries/quota.pyi
--rw-r--r--   0        0        0      318 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/retries/special.pyi
--rw-r--r--   0        0        0     3707 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/retries/standard.pyi
--rw-r--r--   0        0        0      485 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/retries/throttling.pyi
--rw-r--r--   0        0        0     2462 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/retryhandler.pyi
--rw-r--r--   0        0        0     1721 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/serialize.pyi
--rw-r--r--   0        0        0     7151 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/session.pyi
--rw-r--r--   0        0        0     3503 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/signers.pyi
--rw-r--r--   0        0        0     1789 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/stub.pyi
--rw-r--r--   0        0        0      310 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/translate.pyi
--rw-r--r--   0        0        0    10478 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/utils.pyi
--rw-r--r--   0        0        0     1163 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/validate.pyi
--rw-r--r--   0        0        0     1538 2022-07-15 12:40:11.330768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/waiter.pyi
--rw-r--r--   0        0        0     5585 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aioboto3_service_docs/README.md.jinja2
--rw-r--r--   0        0        0     2901 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aioboto3_service_docs/client.md.jinja2
--rw-r--r--   0        0        0      581 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aioboto3_service_docs/literals.md.jinja2
--rw-r--r--   0        0        0     1552 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aioboto3_service_docs/paginators.md.jinja2
--rw-r--r--   0        0        0     4662 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aioboto3_service_docs/service_resource.md.jinja2
--rw-r--r--   0        0        0     1446 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aioboto3_service_docs/type_defs.md.jinja2
--rw-r--r--   0        0        0     9931 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aioboto3_service_docs/usage.md.jinja2
--rw-r--r--   0        0        0     1207 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aioboto3_service_docs/waiters.md.jinja2
--rw-r--r--   0        0        0     1666 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore-stubs/README.md.jinja2
--rw-r--r--   0        0        0      752 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore-stubs/aiobotocore-stubs/__main__.py.jinja2
--rw-r--r--   0        0        0        0 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore-stubs/aiobotocore-stubs/py.typed.jinja2
--rw-r--r--   0        0        0     1693 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore-stubs/aiobotocore-stubs/session.pyi.jinja2
--rw-r--r--   0        0        0       75 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore-stubs/aiobotocore-stubs/version.py.jinja2
--rw-r--r--   0        0        0     2787 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore-stubs/setup.py.jinja2
--rw-r--r--   0        0        0     7570 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/README.md.jinja2
--rw-r--r--   0        0        0     1444 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/service/__init__.pyi.jinja2
--rw-r--r--   0        0        0      913 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/service/__main__.py.jinja2
--rw-r--r--   0        0        0     1192 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/service/client.pyi.jinja2
--rw-r--r--   0        0        0      836 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/service/literals.pyi.jinja2
--rw-r--r--   0        0        0     1687 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/service/paginator.pyi.jinja2
--rw-r--r--   0        0        0        0 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/service/py.typed.jinja2
--rw-r--r--   0        0        0     2197 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/service/service_resource.pyi.jinja2
--rw-r--r--   0        0        0      824 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/service/type_defs.pyi.jinja2
--rw-r--r--   0        0        0       75 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/service/version.py.jinja2
--rw-r--r--   0        0        0     1399 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/service/waiter.pyi.jinja2
--rw-r--r--   0        0        0     1969 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/setup.py.jinja2
--rw-r--r--   0        0        0     5621 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service_docs/README.md.jinja2
--rw-r--r--   0        0        0     2958 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service_docs/client.md.jinja2
--rw-r--r--   0        0        0      581 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service_docs/literals.md.jinja2
--rw-r--r--   0        0        0     1549 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service_docs/paginators.md.jinja2
--rw-r--r--   0        0        0     4559 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service_docs/service_resource.md.jinja2
--rw-r--r--   0        0        0     1446 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service_docs/type_defs.md.jinja2
--rw-r--r--   0        0        0     5055 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service_docs/usage.md.jinja2
--rw-r--r--   0        0        0     1221 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service_docs/waiters.md.jinja2
--rw-r--r--   0        0        0     1004 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_stubs_docs/README.md.jinja2
--rw-r--r--   0        0        0     3164 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3-stubs/README.md.jinja2
--rw-r--r--   0        0        0      902 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3-stubs/boto3-stubs/__init__.pyi.jinja2
--rw-r--r--   0        0        0      746 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3-stubs/boto3-stubs/__main__.py.jinja2
--rw-r--r--   0        0        0        0 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3-stubs/boto3-stubs/py.typed.jinja2
--rw-r--r--   0        0        0     1847 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3-stubs/boto3-stubs/session.pyi.jinja2
--rw-r--r--   0        0        0       75 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3-stubs/boto3-stubs/version.py.jinja2
--rw-r--r--   0        0        0     2758 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3-stubs/setup.py.jinja2
--rw-r--r--   0        0        0     7108 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/README.md.jinja2
--rw-r--r--   0        0        0     1676 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/service/__init__.pyi.jinja2
--rw-r--r--   0        0        0      913 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/service/__main__.py.jinja2
--rw-r--r--   0        0        0     1149 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/service/client.pyi.jinja2
--rw-r--r--   0        0        0      836 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/service/literals.pyi.jinja2
--rw-r--r--   0        0        0     1646 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/service/paginator.pyi.jinja2
--rw-r--r--   0        0        0        0 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/service/py.typed.jinja2
--rw-r--r--   0        0        0     2155 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/service/service_resource.pyi.jinja2
--rw-r--r--   0        0        0      824 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/service/type_defs.pyi.jinja2
--rw-r--r--   0        0        0       75 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/service/version.py.jinja2
--rw-r--r--   0        0        0     1352 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/service/waiter.pyi.jinja2
--rw-r--r--   0        0        0     1969 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/setup.py.jinja2
--rw-r--r--   0        0        0     6244 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service_docs/README.md.jinja2
--rw-r--r--   0        0        0     2969 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service_docs/client.md.jinja2
--rw-r--r--   0        0        0      580 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service_docs/literals.md.jinja2
--rw-r--r--   0        0        0     1789 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service_docs/paginators.md.jinja2
--rw-r--r--   0        0        0     4645 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service_docs/service_resource.md.jinja2
--rw-r--r--   0        0        0     1446 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service_docs/type_defs.md.jinja2
--rw-r--r--   0        0        0     8151 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service_docs/usage.md.jinja2
--rw-r--r--   0        0        0     1203 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service_docs/waiters.md.jinja2
--rw-r--r--   0        0        0     1044 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_stubs_docs/README.md.jinja2
--rw-r--r--   0        0        0     1580 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/botocore-stubs/README.md.jinja2
--rw-r--r--   0        0        0      749 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/botocore-stubs/botocore-stubs/__main__.py.jinja2
--rw-r--r--   0        0        0        0 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/botocore-stubs/botocore-stubs/py.typed.jinja2
--rw-r--r--   0        0        0       75 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/botocore-stubs/botocore-stubs/version.py.jinja2
--rw-r--r--   0        0        0     1899 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/botocore-stubs/setup.py.jinja2
--rw-r--r--   0        0        0      393 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/argument.py.jinja2
--rw-r--r--   0        0        0      347 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/arguments_list.md.jinja2
--rw-r--r--   0        0        0      573 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/arguments_list_code.md.jinja2
--rw-r--r--   0        0        0      816 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/class.py.jinja2
--rw-r--r--   0        0        0     2667 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/footer.md.jinja2
--rw-r--r--   0        0        0      998 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/function.py.jinja2
--rw-r--r--   0        0        0      253 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/header_note.md.jinja2
--rw-r--r--   0        0        0     1924 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/how_to_install.md.jinja2
--rw-r--r--   0        0        0     1733 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/how_to_install_service.md.jinja2
--rw-r--r--   0        0        0      925 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/import_groups.py.jinja2
--rw-r--r--   0        0        0      554 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/import_record.py.jinja2
--rw-r--r--   0        0        0      395 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/import_record_fallback.py.jinja2
--rw-r--r--   0        0        0      341 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/import_record_safe.py.jinja2
--rw-r--r--   0        0        0       85 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/literal.py.jinja2
--rw-r--r--   0        0        0      810 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/method.md.jinja2
--rw-r--r--   0        0        0       85 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/method.py.jinja2
--rw-r--r--   0        0        0     1296 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/method_code.md.jinja2
--rw-r--r--   0        0        0     1257 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/module.py.jinja2
--rw-r--r--   0        0        0     1147 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/submodules.md.jinja2
--rw-r--r--   0        0        0     1737 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/type_annotation.md.jinja2
--rw-r--r--   0        0        0      769 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/type_annotation_code.md.jinja2
--rw-r--r--   0        0        0      687 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/type_hint.md.jinja2
--rw-r--r--   0        0        0     1439 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/typed_dict.py.jinja2
--rw-r--r--   0        0        0      229 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/typed_dict_new.py.jinja2
--rw-r--r--   0        0        0     3355 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/usage.md.jinja2
--rw-r--r--   0        0        0     1628 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/master/README.md.jinja2
--rw-r--r--   0        0        0        0 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/master/mypy_boto3/__init__.py.jinja2
--rw-r--r--   0        0        0       49 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/master/mypy_boto3/__main__.py.jinja2
--rw-r--r--   0        0        0       85 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/master/mypy_boto3/boto3_init.py.jinja2
--rw-r--r--   0        0        0      798 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/master/mypy_boto3/boto3_init_stub.py.jinja2
--rw-r--r--   0        0        0       81 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/master/mypy_boto3/boto3_session.py.jinja2
--rw-r--r--   0        0        0     1135 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/master/mypy_boto3/boto3_session_stub.py.jinja2
--rw-r--r--   0        0        0    14106 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/master/mypy_boto3/main.py.jinja2
--rw-r--r--   0        0        0        0 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/master/mypy_boto3/py.typed.jinja2
--rw-r--r--   0        0        0     1731 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/master/mypy_boto3/submodules.py.jinja2
--rw-r--r--   0        0        0       75 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/master/mypy_boto3/version.py.jinja2
--rw-r--r--   0        0        0     1943 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/master/setup.py.jinja2
--rw-r--r--   0        0        0     1640 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/types-aioboto3/README.md.jinja2
--rw-r--r--   0        0        0      746 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/types-aioboto3/aioboto3-stubs/__main__.py.jinja2
--rw-r--r--   0        0        0        0 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/types-aioboto3/aioboto3-stubs/py.typed.jinja2
--rw-r--r--   0        0        0     2123 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/types-aioboto3/aioboto3-stubs/session.pyi.jinja2
--rw-r--r--   0        0        0       75 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/types-aioboto3/aioboto3-stubs/version.py.jinja2
--rw-r--r--   0        0        0     2551 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/types-aioboto3/setup.py.jinja2
--rw-r--r--   0        0        0      967 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/types_aioboto3_docs/README.md.jinja2
--rw-r--r--   0        0        0      116 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/__init__.py
--rw-r--r--   0        0        0     1721 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/external_import.py
--rw-r--r--   0        0        0     2544 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/fake_annotation.py
--rw-r--r--   0        0        0     2857 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/internal_import.py
--rw-r--r--   0        0        0      712 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/remove_argument.py
--rw-r--r--   0        0        0     2356 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/type.py
--rw-r--r--   0        0        0     3564 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/type_annotation.py
--rw-r--r--   0        0        0     1668 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/type_class.py
--rw-r--r--   0        0        0     1213 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/type_constant.py
--rw-r--r--   0        0        0     3882 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/type_literal.py
--rw-r--r--   0        0        0     2550 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/type_subscript.py
--rw-r--r--   0        0        0    10655 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/type_typed_dict.py
--rw-r--r--   0        0        0       71 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_maps/__init__.py
--rw-r--r--   0        0        0    24857 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_maps/docstring_type_map.py
--rw-r--r--   0        0        0      748 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_maps/literal_type_map.py
--rw-r--r--   0        0        0     1395 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_maps/method_argument_map.py
--rw-r--r--   0        0        0     7152 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_maps/method_type_map.py
--rw-r--r--   0        0        0     4442 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_maps/shape_type_map.py
--rw-r--r--   0        0        0      508 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_maps/syntax_type_map.py
--rw-r--r--   0        0        0     1693 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_maps/typed_dicts.py
--rw-r--r--   0        0        0       46 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/utils/__init__.py
--rw-r--r--   0        0        0     1788 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/utils/boto3_utils.py
--rw-r--r--   0        0        0     1195 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/utils/botocore_changelog.py
--rw-r--r--   0        0        0     2706 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/utils/markdown.py
--rw-r--r--   0        0        0     1279 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/utils/nice_path.py
--rw-r--r--   0        0        0     1473 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/utils/pypi_manager.py
--rw-r--r--   0        0        0     4221 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/utils/strings.py
--rw-r--r--   0        0        0     3800 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/utils/typed_dict_sorter.py
--rw-r--r--   0        0        0     1630 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/utils/version.py
--rw-r--r--   0        0        0       54 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/writers/__init__.py
--rw-r--r--   0        0        0     3742 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/writers/aioboto3_processors.py
--rw-r--r--   0        0        0     4133 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/writers/aiobotocore_processors.py
--rw-r--r--   0        0        0    14520 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/writers/package_writer.py
--rw-r--r--   0        0        0     6272 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/writers/processors.py
--rw-r--r--   0        0        0     4303 2022-07-15 12:40:11.334768 mypy-boto3-builder-7.9.1/mypy_boto3_builder/writers/utils.py
--rw-r--r--   0        0        0     3542 2022-07-15 12:41:06.626359 mypy-boto3-builder-7.9.1/pyproject.toml
--rw-r--r--   0        0        0    10944 2022-07-15 12:41:09.750903 mypy-boto3-builder-7.9.1/setup.py
--rw-r--r--   0        0        0     8828 2022-07-15 12:41:09.751513 mypy-boto3-builder-7.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-07-17 00:31:39.126608 mypy-boto3-builder-7.9.2/LICENSE
+-rw-r--r--   0        0        0     7345 2022-07-17 00:31:39.126608 mypy-boto3-builder-7.9.2/README.md
+-rw-r--r--   0        0        0       34 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/__init__.py
+-rw-r--r--   0        0        0      116 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/__main__.py
+-rw-r--r--   0        0        0     3744 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/cli_parser.py
+-rw-r--r--   0        0        0     2431 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/constants.py
+-rw-r--r--   0        0        0       33 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/enums/__init__.py
+-rw-r--r--   0        0        0      719 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/enums/service_module_name.py
+-rw-r--r--   0        0        0       35 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/generators/__init__.py
+-rw-r--r--   0        0        0     3479 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/generators/aioboto3_generator.py
+-rw-r--r--   0        0        0     3474 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/generators/aiobotocore_generator.py
+-rw-r--r--   0        0        0     7621 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/generators/base_generator.py
+-rw-r--r--   0        0        0     4848 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/generators/boto3_generator.py
+-rw-r--r--   0        0        0       40 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/import_helpers/__init__.py
+-rw-r--r--   0        0        0     4842 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/import_helpers/import_record.py
+-rw-r--r--   0        0        0     3182 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/import_helpers/import_string.py
+-rw-r--r--   0        0        0     1359 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/import_helpers/internal_import_record.py
+-rw-r--r--   0        0        0     1006 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/jinja_manager.py
+-rw-r--r--   0        0        0      882 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/logger.py
+-rw-r--r--   0        0        0     6128 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/main.py
+-rw-r--r--   0        0        0     4035 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/package_data.py
+-rw-r--r--   0        0        0       49 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/__init__.py
+-rw-r--r--   0        0        0     4035 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/aiobotocore_stubs_package.py
+-rw-r--r--   0        0        0     6695 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/boto3_stubs_package.py
+-rw-r--r--   0        0        0     3036 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/client.py
+-rw-r--r--   0        0        0       35 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/docstring_parser/__init__.py
+-rw-r--r--   0        0        0     3445 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/docstring_parser/argspec_parser.py
+-rw-r--r--   0        0        0    12810 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/docstring_parser/docstring_parser.py
+-rw-r--r--   0        0        0     4979 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/docstring_parser/syntax_grammar.py
+-rw-r--r--   0        0        0     3804 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/docstring_parser/type_doc_grammar.py
+-rw-r--r--   0        0        0     2051 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/docstring_parser/type_doc_line.py
+-rw-r--r--   0        0        0     8300 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/docstring_parser/type_value.py
+-rw-r--r--   0        0        0     2717 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/fake_service_package.py
+-rw-r--r--   0        0        0     2756 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/helpers.py
+-rw-r--r--   0        0        0      969 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/master_package.py
+-rw-r--r--   0        0        0     1563 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/parse_attributes.py
+-rw-r--r--   0        0        0     4264 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/parse_collections.py
+-rw-r--r--   0        0        0      753 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/parse_identifiers.py
+-rw-r--r--   0        0        0     1272 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/parse_references.py
+-rw-r--r--   0        0        0     3213 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/parse_resource.py
+-rw-r--r--   0        0        0     3630 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/service_package.py
+-rw-r--r--   0        0        0     5760 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/service_resource.py
+-rw-r--r--   0        0        0    29972 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/shape_parser.py
+-rw-r--r--   0        0        0     5329 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/types_aioboto3_package.py
+-rw-r--r--   0        0        0       75 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/postprocessors/__init__.py
+-rw-r--r--   0        0        0     6084 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/postprocessors/aiobotocore.py
+-rw-r--r--   0        0        0     9230 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/postprocessors/base.py
+-rw-r--r--   0        0        0      334 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/postprocessors/botocore.py
+-rw-r--r--   0        0        0        0 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/py.typed
+-rw-r--r--   0        0        0     5125 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/service_name.py
+-rw-r--r--   0        0        0       40 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/__init__.py
+-rw-r--r--   0        0        0     3801 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/aiobotocore_stubs_package.py
+-rw-r--r--   0        0        0     2048 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/argument.py
+-rw-r--r--   0        0        0     1284 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/attribute.py
+-rw-r--r--   0        0        0     5097 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/boto3_stubs_package.py
+-rw-r--r--   0        0        0      354 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/botocore_stubs_package.py
+-rw-r--r--   0        0        0     3610 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/class_record.py
+-rw-r--r--   0        0        0     4436 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/client.py
+-rw-r--r--   0        0        0     1696 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/collection.py
+-rw-r--r--   0        0        0     4005 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/function.py
+-rw-r--r--   0        0        0     1238 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/master_package.py
+-rw-r--r--   0        0        0      479 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/method.py
+-rw-r--r--   0        0        0     2491 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/package.py
+-rw-r--r--   0        0        0     2008 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/paginator.py
+-rw-r--r--   0        0        0     1495 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/resource.py
+-rw-r--r--   0        0        0    13580 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/service_package.py
+-rw-r--r--   0        0        0     5729 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/service_resource.py
+-rw-r--r--   0        0        0     2903 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/types_aioboto3_package.py
+-rw-r--r--   0        0        0     1853 2022-07-17 00:31:39.138608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/waiter.py
+-rw-r--r--   0        0        0       33 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/__init__.py
+-rw-r--r--   0        0        0      184 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/__init__.pyi
+-rw-r--r--   0        0        0        0 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/dynamodb/__init__.pyi
+-rw-r--r--   0        0        0     1252 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/dynamodb/table.pyi
+-rw-r--r--   0        0        0        0 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/experimental/__init__.pyi
+-rw-r--r--   0        0        0      636 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/experimental/async_chalice.pyi
+-rw-r--r--   0        0        0        0 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/resources/__init__.pyi
+-rw-r--r--   0        0        0     1118 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/resources/action.pyi
+-rw-r--r--   0        0        0      476 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/resources/base.pyi
+-rw-r--r--   0        0        0     1383 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/resources/collection.pyi
+-rw-r--r--   0        0        0      596 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/resources/factory.pyi
+-rw-r--r--   0        0        0      602 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/resources/response.pyi
+-rw-r--r--   0        0        0        0 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/s3/__init__.pyi
+-rw-r--r--   0        0        0     3860 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/s3/cse.pyi
+-rw-r--r--   0        0        0     1961 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/s3/inject.pyi
+-rw-r--r--   0        0        0     3167 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/session.pyi
+-rw-r--r--   0        0        0       17 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/__init__.pyi
+-rw-r--r--   0        0        0       96 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/args.pyi
+-rw-r--r--   0        0        0     1177 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/client.pyi
+-rw-r--r--   0        0        0      300 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/config.pyi
+-rw-r--r--   0        0        0     5759 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/credentials.pyi
+-rw-r--r--   0        0        0      477 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/discovery.pyi
+-rw-r--r--   0        0        0     1401 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/endpoint.pyi
+-rw-r--r--   0        0        0      404 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/eventstream.pyi
+-rw-r--r--   0        0        0      595 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/handlers.pyi
+-rw-r--r--   0        0        0      261 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/hooks.pyi
+-rw-r--r--   0        0        0      797 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/httpsession.pyi
+-rw-r--r--   0        0        0      722 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/paginate.pyi
+-rw-r--r--   0        0        0      735 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/parsers.pyi
+-rw-r--r--   0        0        0     1219 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/response.pyi
+-rw-r--r--   0        0        0     2556 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/session.pyi
+-rw-r--r--   0        0        0     2182 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/signers.pyi
+-rw-r--r--   0        0        0     1803 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/utils.pyi
+-rw-r--r--   0        0        0      581 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/waiter.pyi
+-rw-r--r--   0        0        0     1701 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/__init__.pyi
+-rw-r--r--   0        0        0      151 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/compat.pyi
+-rw-r--r--   0        0        0       99 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/docs/__init__.pyi
+-rw-r--r--   0        0        0      934 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/docs/utils.pyi
+-rw-r--r--   0        0        0        0 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/dynamodb/__init__.pyi
+-rw-r--r--   0        0        0     4582 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/dynamodb/conditions.pyi
+-rw-r--r--   0        0        0      994 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/dynamodb/table.pyi
+-rw-r--r--   0        0        0     1705 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/dynamodb/transform.pyi
+-rw-r--r--   0        0        0     1332 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/dynamodb/types.pyi
+-rw-r--r--   0        0        0        0 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/ec2/__init__.pyi
+-rw-r--r--   0        0        0      361 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/ec2/createtags.pyi
+-rw-r--r--   0        0        0      204 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/ec2/deletetags.pyi
+-rw-r--r--   0        0        0     1253 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/exceptions.pyi
+-rw-r--r--   0        0        0        0 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/resources/__init__.pyi
+-rw-r--r--   0        0        0     1546 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/resources/action.pyi
+-rw-r--r--   0        0        0     1094 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/resources/base.pyi
+-rw-r--r--   0        0        0     1922 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/resources/collection.pyi
+-rw-r--r--   0        0        0      496 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/resources/factory.pyi
+-rw-r--r--   0        0        0     3607 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/resources/model.pyi
+-rw-r--r--   0        0        0      565 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/resources/params.pyi
+-rw-r--r--   0        0        0     1607 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/resources/response.pyi
+-rw-r--r--   0        0        0        0 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/s3/__init__.pyi
+-rw-r--r--   0        0        0     2190 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/s3/transfer.pyi
+-rw-r--r--   0        0        0     2917 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/session.pyi
+-rw-r--r--   0        0        0      779 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/utils.pyi
+-rw-r--r--   0        0        0      580 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/__init__.pyi
+-rw-r--r--   0        0        0     2170 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/args.pyi
+-rw-r--r--   0        0        0     4202 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/auth.pyi
+-rw-r--r--   0        0        0     3676 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/awsrequest.pyi
+-rw-r--r--   0        0        0     5548 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/client.pyi
+-rw-r--r--   0        0        0     2277 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/compat.pyi
+-rw-r--r--   0        0        0     2279 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/config.pyi
+-rw-r--r--   0        0        0      274 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/configloader.pyi
+-rw-r--r--   0        0        0     3479 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/configprovider.pyi
+-rw-r--r--   0        0        0    10847 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/credentials.pyi
+-rw-r--r--   0        0        0        0 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/crt/__init__.pyi
+-rw-r--r--   0        0        0     2077 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/crt/auth.pyi
+-rw-r--r--   0        0        0     2173 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/discovery.pyi
+-rw-r--r--   0        0        0     2184 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/endpoint.pyi
+-rw-r--r--   0        0        0      708 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/errorfactory.pyi
+-rw-r--r--   0        0        0     2905 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/eventstream.pyi
+-rw-r--r--   0        0        0    20633 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/exceptions.pyi
+-rw-r--r--   0        0        0     6183 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/handlers.pyi
+-rw-r--r--   0        0        0      521 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/history.pyi
+-rw-r--r--   0        0        0     2792 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/hooks.pyi
+-rw-r--r--   0        0        0     1947 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/httpsession.pyi
+-rw-r--r--   0        0        0     1862 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/loaders.pyi
+-rw-r--r--   0        0        0     5461 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/model.pyi
+-rw-r--r--   0        0        0     2309 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/monitoring.pyi
+-rw-r--r--   0        0        0     1697 2022-07-17 00:31:39.142608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/paginate.pyi
+-rw-r--r--   0        0        0     2097 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/parsers.pyi
+-rw-r--r--   0        0        0     1533 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/regions.pyi
+-rw-r--r--   0        0        0     1081 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/response.pyi
+-rw-r--r--   0        0        0        0 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/retries/__init__.pyi
+-rw-r--r--   0        0        0      805 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/retries/adaptive.pyi
+-rw-r--r--   0        0        0      185 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/retries/base.pyi
+-rw-r--r--   0        0        0      652 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/retries/bucket.pyi
+-rw-r--r--   0        0        0      348 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/retries/quota.pyi
+-rw-r--r--   0        0        0      318 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/retries/special.pyi
+-rw-r--r--   0        0        0     3707 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/retries/standard.pyi
+-rw-r--r--   0        0        0      485 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/retries/throttling.pyi
+-rw-r--r--   0        0        0     2473 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/retryhandler.pyi
+-rw-r--r--   0        0        0     1721 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/serialize.pyi
+-rw-r--r--   0        0        0     7151 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/session.pyi
+-rw-r--r--   0        0        0     3503 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/signers.pyi
+-rw-r--r--   0        0        0     1789 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/stub.pyi
+-rw-r--r--   0        0        0      310 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/translate.pyi
+-rw-r--r--   0        0        0    10478 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/utils.pyi
+-rw-r--r--   0        0        0     1163 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/validate.pyi
+-rw-r--r--   0        0        0     1538 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/waiter.pyi
+-rw-r--r--   0        0        0     5585 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aioboto3_service_docs/README.md.jinja2
+-rw-r--r--   0        0        0     2901 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aioboto3_service_docs/client.md.jinja2
+-rw-r--r--   0        0        0      581 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aioboto3_service_docs/literals.md.jinja2
+-rw-r--r--   0        0        0     1552 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aioboto3_service_docs/paginators.md.jinja2
+-rw-r--r--   0        0        0     4662 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aioboto3_service_docs/service_resource.md.jinja2
+-rw-r--r--   0        0        0     1446 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aioboto3_service_docs/type_defs.md.jinja2
+-rw-r--r--   0        0        0     9931 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aioboto3_service_docs/usage.md.jinja2
+-rw-r--r--   0        0        0     1207 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aioboto3_service_docs/waiters.md.jinja2
+-rw-r--r--   0        0        0     1666 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore-stubs/README.md.jinja2
+-rw-r--r--   0        0        0      752 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore-stubs/aiobotocore-stubs/__main__.py.jinja2
+-rw-r--r--   0        0        0        0 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore-stubs/aiobotocore-stubs/py.typed.jinja2
+-rw-r--r--   0        0        0     1693 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore-stubs/aiobotocore-stubs/session.pyi.jinja2
+-rw-r--r--   0        0        0       75 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore-stubs/aiobotocore-stubs/version.py.jinja2
+-rw-r--r--   0        0        0     2787 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore-stubs/setup.py.jinja2
+-rw-r--r--   0        0        0     7570 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/README.md.jinja2
+-rw-r--r--   0        0        0     1444 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/service/__init__.pyi.jinja2
+-rw-r--r--   0        0        0      913 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/service/__main__.py.jinja2
+-rw-r--r--   0        0        0     1192 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/service/client.pyi.jinja2
+-rw-r--r--   0        0        0      836 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/service/literals.pyi.jinja2
+-rw-r--r--   0        0        0     1687 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/service/paginator.pyi.jinja2
+-rw-r--r--   0        0        0        0 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/service/py.typed.jinja2
+-rw-r--r--   0        0        0     2197 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/service/service_resource.pyi.jinja2
+-rw-r--r--   0        0        0      824 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/service/type_defs.pyi.jinja2
+-rw-r--r--   0        0        0       75 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/service/version.py.jinja2
+-rw-r--r--   0        0        0     1399 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/service/waiter.pyi.jinja2
+-rw-r--r--   0        0        0     1969 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/setup.py.jinja2
+-rw-r--r--   0        0        0     5621 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service_docs/README.md.jinja2
+-rw-r--r--   0        0        0     2958 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service_docs/client.md.jinja2
+-rw-r--r--   0        0        0      581 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service_docs/literals.md.jinja2
+-rw-r--r--   0        0        0     1549 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service_docs/paginators.md.jinja2
+-rw-r--r--   0        0        0     4559 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service_docs/service_resource.md.jinja2
+-rw-r--r--   0        0        0     1446 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service_docs/type_defs.md.jinja2
+-rw-r--r--   0        0        0     5055 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service_docs/usage.md.jinja2
+-rw-r--r--   0        0        0     1221 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service_docs/waiters.md.jinja2
+-rw-r--r--   0        0        0     1004 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_stubs_docs/README.md.jinja2
+-rw-r--r--   0        0        0     3164 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3-stubs/README.md.jinja2
+-rw-r--r--   0        0        0      902 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3-stubs/boto3-stubs/__init__.pyi.jinja2
+-rw-r--r--   0        0        0      746 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3-stubs/boto3-stubs/__main__.py.jinja2
+-rw-r--r--   0        0        0        0 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3-stubs/boto3-stubs/py.typed.jinja2
+-rw-r--r--   0        0        0     1847 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3-stubs/boto3-stubs/session.pyi.jinja2
+-rw-r--r--   0        0        0       75 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3-stubs/boto3-stubs/version.py.jinja2
+-rw-r--r--   0        0        0     2758 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3-stubs/setup.py.jinja2
+-rw-r--r--   0        0        0     7108 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/README.md.jinja2
+-rw-r--r--   0        0        0     1676 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/service/__init__.pyi.jinja2
+-rw-r--r--   0        0        0      913 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/service/__main__.py.jinja2
+-rw-r--r--   0        0        0     1149 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/service/client.pyi.jinja2
+-rw-r--r--   0        0        0      836 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/service/literals.pyi.jinja2
+-rw-r--r--   0        0        0     1646 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/service/paginator.pyi.jinja2
+-rw-r--r--   0        0        0        0 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/service/py.typed.jinja2
+-rw-r--r--   0        0        0     2155 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/service/service_resource.pyi.jinja2
+-rw-r--r--   0        0        0      824 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/service/type_defs.pyi.jinja2
+-rw-r--r--   0        0        0       75 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/service/version.py.jinja2
+-rw-r--r--   0        0        0     1352 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/service/waiter.pyi.jinja2
+-rw-r--r--   0        0        0     1969 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/setup.py.jinja2
+-rw-r--r--   0        0        0     6244 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service_docs/README.md.jinja2
+-rw-r--r--   0        0        0     2969 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service_docs/client.md.jinja2
+-rw-r--r--   0        0        0      580 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service_docs/literals.md.jinja2
+-rw-r--r--   0        0        0     1789 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service_docs/paginators.md.jinja2
+-rw-r--r--   0        0        0     4645 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service_docs/service_resource.md.jinja2
+-rw-r--r--   0        0        0     1446 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service_docs/type_defs.md.jinja2
+-rw-r--r--   0        0        0     8151 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service_docs/usage.md.jinja2
+-rw-r--r--   0        0        0     1203 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service_docs/waiters.md.jinja2
+-rw-r--r--   0        0        0     1044 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_stubs_docs/README.md.jinja2
+-rw-r--r--   0        0        0     1580 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/botocore-stubs/README.md.jinja2
+-rw-r--r--   0        0        0      749 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/botocore-stubs/botocore-stubs/__main__.py.jinja2
+-rw-r--r--   0        0        0        0 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/botocore-stubs/botocore-stubs/py.typed.jinja2
+-rw-r--r--   0        0        0       75 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/botocore-stubs/botocore-stubs/version.py.jinja2
+-rw-r--r--   0        0        0     1899 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/botocore-stubs/setup.py.jinja2
+-rw-r--r--   0        0        0      393 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/argument.py.jinja2
+-rw-r--r--   0        0        0      347 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/arguments_list.md.jinja2
+-rw-r--r--   0        0        0      573 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/arguments_list_code.md.jinja2
+-rw-r--r--   0        0        0      816 2022-07-17 00:31:39.146608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/class.py.jinja2
+-rw-r--r--   0        0        0     2667 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/footer.md.jinja2
+-rw-r--r--   0        0        0      998 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/function.py.jinja2
+-rw-r--r--   0        0        0      253 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/header_note.md.jinja2
+-rw-r--r--   0        0        0     1924 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/how_to_install.md.jinja2
+-rw-r--r--   0        0        0     1733 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/how_to_install_service.md.jinja2
+-rw-r--r--   0        0        0      925 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/import_groups.py.jinja2
+-rw-r--r--   0        0        0      554 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/import_record.py.jinja2
+-rw-r--r--   0        0        0      395 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/import_record_fallback.py.jinja2
+-rw-r--r--   0        0        0      341 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/import_record_safe.py.jinja2
+-rw-r--r--   0        0        0       85 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/literal.py.jinja2
+-rw-r--r--   0        0        0      810 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/method.md.jinja2
+-rw-r--r--   0        0        0       85 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/method.py.jinja2
+-rw-r--r--   0        0        0     1296 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/method_code.md.jinja2
+-rw-r--r--   0        0        0     1257 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/module.py.jinja2
+-rw-r--r--   0        0        0     1147 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/submodules.md.jinja2
+-rw-r--r--   0        0        0     1737 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/type_annotation.md.jinja2
+-rw-r--r--   0        0        0      769 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/type_annotation_code.md.jinja2
+-rw-r--r--   0        0        0      687 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/type_hint.md.jinja2
+-rw-r--r--   0        0        0     1439 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/typed_dict.py.jinja2
+-rw-r--r--   0        0        0      229 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/typed_dict_new.py.jinja2
+-rw-r--r--   0        0        0     3355 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/usage.md.jinja2
+-rw-r--r--   0        0        0     1628 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/master/README.md.jinja2
+-rw-r--r--   0        0        0        0 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/master/mypy_boto3/__init__.py.jinja2
+-rw-r--r--   0        0        0       49 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/master/mypy_boto3/__main__.py.jinja2
+-rw-r--r--   0        0        0       85 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/master/mypy_boto3/boto3_init.py.jinja2
+-rw-r--r--   0        0        0      798 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/master/mypy_boto3/boto3_init_stub.py.jinja2
+-rw-r--r--   0        0        0       81 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/master/mypy_boto3/boto3_session.py.jinja2
+-rw-r--r--   0        0        0     1135 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/master/mypy_boto3/boto3_session_stub.py.jinja2
+-rw-r--r--   0        0        0    14106 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/master/mypy_boto3/main.py.jinja2
+-rw-r--r--   0        0        0        0 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/master/mypy_boto3/py.typed.jinja2
+-rw-r--r--   0        0        0     1731 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/master/mypy_boto3/submodules.py.jinja2
+-rw-r--r--   0        0        0       75 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/master/mypy_boto3/version.py.jinja2
+-rw-r--r--   0        0        0     1943 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/master/setup.py.jinja2
+-rw-r--r--   0        0        0     1640 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/types-aioboto3/README.md.jinja2
+-rw-r--r--   0        0        0      746 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/types-aioboto3/aioboto3-stubs/__main__.py.jinja2
+-rw-r--r--   0        0        0        0 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/types-aioboto3/aioboto3-stubs/py.typed.jinja2
+-rw-r--r--   0        0        0     2123 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/types-aioboto3/aioboto3-stubs/session.pyi.jinja2
+-rw-r--r--   0        0        0       75 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/types-aioboto3/aioboto3-stubs/version.py.jinja2
+-rw-r--r--   0        0        0     2551 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/types-aioboto3/setup.py.jinja2
+-rw-r--r--   0        0        0      967 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/types_aioboto3_docs/README.md.jinja2
+-rw-r--r--   0        0        0      116 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/__init__.py
+-rw-r--r--   0        0        0     1721 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/external_import.py
+-rw-r--r--   0        0        0     2544 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/fake_annotation.py
+-rw-r--r--   0        0        0     2857 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/internal_import.py
+-rw-r--r--   0        0        0      712 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/remove_argument.py
+-rw-r--r--   0        0        0     2356 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/type.py
+-rw-r--r--   0        0        0     3564 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/type_annotation.py
+-rw-r--r--   0        0        0     1668 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/type_class.py
+-rw-r--r--   0        0        0     1213 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/type_constant.py
+-rw-r--r--   0        0        0     3882 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/type_literal.py
+-rw-r--r--   0        0        0     2550 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/type_subscript.py
+-rw-r--r--   0        0        0    10655 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/type_typed_dict.py
+-rw-r--r--   0        0        0       71 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_maps/__init__.py
+-rw-r--r--   0        0        0    24857 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_maps/docstring_type_map.py
+-rw-r--r--   0        0        0      748 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_maps/literal_type_map.py
+-rw-r--r--   0        0        0     1395 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_maps/method_argument_map.py
+-rw-r--r--   0        0        0     7152 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_maps/method_type_map.py
+-rw-r--r--   0        0        0     4442 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_maps/shape_type_map.py
+-rw-r--r--   0        0        0      508 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_maps/syntax_type_map.py
+-rw-r--r--   0        0        0     1693 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_maps/typed_dicts.py
+-rw-r--r--   0        0        0       46 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/utils/__init__.py
+-rw-r--r--   0        0        0     1788 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/utils/boto3_utils.py
+-rw-r--r--   0        0        0     1195 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/utils/botocore_changelog.py
+-rw-r--r--   0        0        0     2706 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/utils/markdown.py
+-rw-r--r--   0        0        0     1279 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/utils/nice_path.py
+-rw-r--r--   0        0        0     1473 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/utils/pypi_manager.py
+-rw-r--r--   0        0        0     4221 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/utils/strings.py
+-rw-r--r--   0        0        0     3800 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/utils/typed_dict_sorter.py
+-rw-r--r--   0        0        0     1630 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/utils/version.py
+-rw-r--r--   0        0        0       54 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/writers/__init__.py
+-rw-r--r--   0        0        0     3742 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/writers/aioboto3_processors.py
+-rw-r--r--   0        0        0     4133 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/writers/aiobotocore_processors.py
+-rw-r--r--   0        0        0    14520 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/writers/package_writer.py
+-rw-r--r--   0        0        0     6272 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/writers/processors.py
+-rw-r--r--   0        0        0     4303 2022-07-17 00:31:39.150608 mypy-boto3-builder-7.9.2/mypy_boto3_builder/writers/utils.py
+-rw-r--r--   0        0        0     3542 2022-07-17 00:32:33.014356 mypy-boto3-builder-7.9.2/pyproject.toml
+-rw-r--r--   0        0        0    10944 2022-07-17 00:32:39.019730 mypy-boto3-builder-7.9.2/setup.py
+-rw-r--r--   0        0        0     8828 2022-07-17 00:32:39.020870 mypy-boto3-builder-7.9.2/PKG-INFO
```

### Comparing `mypy-boto3-builder-7.9.1/LICENSE` & `mypy-boto3-builder-7.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/README.md` & `mypy-boto3-builder-7.9.2/README.md`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/cli_parser.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/cli_parser.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/constants.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/constants.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/enums/service_module_name.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/enums/service_module_name.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/generators/aioboto3_generator.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/generators/aioboto3_generator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/generators/aiobotocore_generator.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/generators/aiobotocore_generator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/generators/base_generator.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/generators/base_generator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/generators/boto3_generator.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/generators/boto3_generator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/import_helpers/import_record.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/import_helpers/import_record.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/import_helpers/import_string.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/import_helpers/import_string.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/import_helpers/internal_import_record.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/import_helpers/internal_import_record.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/jinja_manager.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/jinja_manager.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/logger.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/logger.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/main.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/main.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/package_data.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/package_data.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/aiobotocore_stubs_package.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/aiobotocore_stubs_package.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/boto3_stubs_package.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/boto3_stubs_package.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/client.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/docstring_parser/argspec_parser.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/docstring_parser/argspec_parser.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/docstring_parser/docstring_parser.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/docstring_parser/docstring_parser.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/docstring_parser/syntax_grammar.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/docstring_parser/syntax_grammar.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/docstring_parser/type_doc_grammar.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/docstring_parser/type_doc_grammar.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/docstring_parser/type_doc_line.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/docstring_parser/type_doc_line.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/docstring_parser/type_value.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/docstring_parser/type_value.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/fake_service_package.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/fake_service_package.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/helpers.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/helpers.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/master_package.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/master_package.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/parse_attributes.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/parse_attributes.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/parse_collections.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/parse_collections.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/parse_identifiers.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/parse_identifiers.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/parse_references.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/parse_references.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/parse_resource.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/parse_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/service_package.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/service_package.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/service_resource.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/shape_parser.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/shape_parser.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/parsers/types_aioboto3_package.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/parsers/types_aioboto3_package.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/postprocessors/aiobotocore.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/postprocessors/aiobotocore.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/postprocessors/base.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/postprocessors/base.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/service_name.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/service_name.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/aiobotocore_stubs_package.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/aiobotocore_stubs_package.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/argument.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/argument.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/attribute.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/attribute.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/boto3_stubs_package.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/boto3_stubs_package.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/class_record.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/class_record.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/client.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/collection.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/collection.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/function.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/function.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/master_package.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/master_package.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/package.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/package.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/paginator.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/resource.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/service_package.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/service_package.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/service_resource.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/types_aioboto3_package.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/types_aioboto3_package.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/structures/waiter.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/structures/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/dynamodb/table.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/dynamodb/table.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 _R = TypeVar("_R")
 
 def register_table_methods(base_classes: List[Any], **kwargs: Any) -> None: ...
 
 class CustomTableResource(TableResource):
     # FIXME: Signature of "batch_writer" incompatible with supertype "TableResource"
-    def batch_writer(  # type: ignore
+    def batch_writer(  # type: ignore [override]
         self,
         overwrite_by_pkeys: Optional[List[str]] = ...,
         flush_amount: int = ...,
         on_exit_loop_sleep: int = ...,
     ) -> "BatchWriter": ...
 
 class BatchWriter:
```

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/experimental/async_chalice.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/experimental/async_chalice.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/resources/action.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/resources/action.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 class AIOServiceAction(ServiceAction):
     def __init__(
         self,
         action_model: Action,
         factory: Optional[ResourceFactory] = ...,
         service_context: Optional[ServiceContext] = ...,
     ) -> None: ...
-    async def __call__(  # type: ignore
+    async def __call__(  # type: ignore [override]
         self, parent: ServiceResource, *args: Any, **kwargs: Any
     ) -> Union[ServiceResource, List[ServiceResource], Dict[str, Any]]: ...
 
 class AioBatchAction(ServiceAction):
-    async def __call__(  # type: ignore
+    async def __call__(  # type: ignore [override]
         self, parent: ServiceResource, *args: Any, **kwargs: Any
     ) -> List[Dict[str, Any]]: ...
 
 class AIOWaiterAction(WaiterAction):
-    async def __call__(  # type: ignore
+    async def __call__(  # type: ignore [override]
         self, parent: ServiceResource, *args: Any, **kwargs: Any
     ) -> None: ...
```

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/resources/collection.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/resources/collection.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     Converted the __iter__
     """
 
     async def __anext__(self) -> Iterator[Any]: ...
     def __aiter__(self) -> Iterator[Any]: ...
     def __iter__(self) -> Iterator[Any]: ...
-    async def pages(self) -> Iterator[List[Any]]: ...  # type: ignore
+    async def pages(self) -> Iterator[List[Any]]: ...  # type: ignore [override]
 
 class AIOCollectionManager(CollectionManager):
     def __init__(
         self,
         collection_model: Collection,
         parent: ServiceResource,
         factory: ResourceFactory,
```

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/resources/factory.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/resources/factory.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 from boto3.utils import ServiceContext
 from botocore.hooks import BaseEventHooks
 
 logger: logging.Logger
 
 class AIOBoto3ResourceFactory(ResourceFactory):
     def __init__(self, emitter: BaseEventHooks) -> None: ...
-    async def load_from_definition(  # type: ignore
+    async def load_from_definition(  # type: ignore [override]
         self,
         resource_name: str,
         single_resource_json_definition: Any,
         service_context: ServiceContext,
     ) -> AIOBoto3ServiceResource: ...
```

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/resources/response.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/resources/response.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Union
 
 from boto3.resources.base import ServiceResource
 from boto3.resources.response import RawHandler, ResourceHandler
 
 class AIOResourceHandler(ResourceHandler):
-    async def __call__(  # type: ignore
+    async def __call__(  # type: ignore [override]
         self, parent: ServiceResource, params: Dict[str, Any], response: Dict[str, Any]
     ) -> Union[ServiceResource, List[ServiceResource]]: ...
 
 class AIORawHandler(RawHandler):
-    async def __call__(  # type: ignore
+    async def __call__(  # type: ignore [override]
         self, parent: ServiceResource, params: Dict[str, Any], response: Dict[str, Any]
     ) -> Dict[str, Any]: ...
```

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/s3/cse.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/s3/cse.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/s3/inject.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/s3/inject.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aioboto3/session.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aioboto3/session.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self,
         service_name: str,
         partition_name: str = "aws",
         allow_non_regional: bool = False,
     ) -> List[str]: ...
     def get_credentials(self) -> Credentials: ...
     def _register_default_handlers(self) -> None: ...
-    def client(  # type: ignore
+    def client(  # type: ignore [override]
         self,
         service_name: str,
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
         verify: Union[str, bool, None] = ...,
         endpoint_url: Optional[str] = ...,
```

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/client.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/client.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from botocore.history import HistoryRecorder
 
 history_recorder: HistoryRecorder
 
 _R = TypeVar("_R")
 
 class AioClientCreator(ClientCreator):
-    async def create_client(  # type: ignore
+    async def create_client(  # type: ignore [override]
         self,
         service_name: str,
         region_name: str,
         is_secure: bool = ...,
         endpoint_url: Optional[str] = ...,
         verify: Optional[Union[str, bool]] = ...,
         credentials: Optional[Any] = ...,
@@ -25,8 +25,8 @@
     ) -> AioBaseClient: ...
 
 class AioBaseClient(BaseClient):
     def get_paginator(self, operation_name: str) -> AioPaginator: ...
     def get_waiter(self, waiter_name: str) -> AIOWaiter: ...
     async def __aenter__(self: _R) -> _R: ...
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any: ...
-    async def close(self) -> None: ...  # type: ignore
+    async def close(self) -> None: ...  # type: ignore [override]
```

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/credentials.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/credentials.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -24,63 +24,65 @@
     ProcessProvider,
     ProfileProviderBuilder,
     RefreshableCredentials,
     SharedCredentialProvider,
     SSOProvider,
 )
 
+from mypy_boto3_builder.stubs_static.botocore.credentials import ReadOnlyCredentials
+
 logger: logging.Logger
 
 def create_credential_resolver(
-    session: AioSession,  # type: ignore
+    session: AioSession,
     cache: Optional[Any] = ...,
     region_name: Optional[str] = ...,
 ) -> AioCredentialResolver: ...
 
 class AioProfileProviderBuilder(ProfileProviderBuilder): ...
 
 async def get_credentials(
-    session: AioSession,  # type: ignore
+    session: AioSession,
 ) -> AioCredentials: ...
 def create_assume_role_refresher(
-    client: AioBaseClient,  # type: ignore
+    client: AioBaseClient,
     params: Any,
 ) -> Any: ...
 def create_aio_mfa_serial_refresher(actual_refresh: Any) -> Any: ...
 
 _R = TypeVar("_R")
 
 class AioCredentials(Credentials):
-    async def get_frozen_credentials(self) -> AioRefreshableCredentials: ...  # type: ignore
+    async def get_frozen_credentials(self) -> ReadOnlyCredentials: ...  # type: ignore [override]
     @classmethod
     def from_credentials(cls: Type[_R], obj: Optional[Credentials]) -> _R: ...
 
 _AioRefreshableCredentials = TypeVar(
     "_AioRefreshableCredentials", bound="AioRefreshableCredentials"
 )
 
 class AioRefreshableCredentials(RefreshableCredentials):
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...
     @classmethod
     def from_refreshable_credentials(
         cls: Type[_R], obj: Optional[RefreshableCredentials]
     ) -> _R: ...
-    @property  # type: ignore
-    def access_key(self) -> str: ...  # type: ignore
+    @property  # type: ignore [override]
+    def access_key(self) -> str: ...  # type: ignore [override]
     @access_key.setter
     def access_key(self, value: str) -> None: ...
-    @property  # type: ignore
-    def secret_key(self) -> str: ...  # type: ignore
+    @property  # type: ignore [override]
+    def secret_key(self) -> str: ...  # type: ignore [override]
     @secret_key.setter
     def secret_key(self, value: str) -> None: ...
-    @property  # type: ignore
-    def token(self) -> str: ...  # type: ignore
+    @property  # type: ignore [override]
+    def token(self) -> str: ...  # type: ignore [override]
     @token.setter
     def token(self, value: str) -> None: ...
-    async def get_frozen_credentials(self) -> RefreshableCredentials: ...  # type: ignore
+    async def get_frozen_credentials(self) -> ReadOnlyCredentials: ...  # type: ignore [override]
 
 class AioDeferredRefreshableCredentials(AioRefreshableCredentials):
     method: Any
     def __init__(self, refresh_using: Any, method: Any, time_fetcher: Any = ...) -> None: ...
     def refresh_needed(self, refresh_in: Optional[Any] = ...) -> bool: ...
 
 class AioCachedCredentialFetcher(CachedCredentialFetcher):
@@ -120,31 +122,31 @@
 class AioSharedCredentialProvider(SharedCredentialProvider):
     async def load(self) -> AioCredentials: ...
 
 class AioConfigProvider(ConfigProvider):
     async def load(self) -> AioCredentials: ...
 
 class AioBotoProvider(BotoProvider):
-    async def load(self) -> AioCredentials: ...  # type: ignore
+    async def load(self) -> AioCredentials: ...  # type: ignore [override]
 
 class AioAssumeRoleProvider(AssumeRoleProvider):
-    async def load(self) -> AioDeferredRefreshableCredentials: ...  # type: ignore
+    async def load(self) -> AioDeferredRefreshableCredentials: ...  # type: ignore [override]
 
 class AioAssumeRoleWithWebIdentityProvider(AssumeRoleWithWebIdentityProvider):
-    async def load(self) -> AioDeferredRefreshableCredentials: ...  # type: ignore
+    async def load(self) -> AioDeferredRefreshableCredentials: ...  # type: ignore [override]
 
 class AioCanonicalNameCredentialSourcer(CanonicalNameCredentialSourcer):
-    async def source_credentials(self, source_name: str) -> Any: ...  # type: ignore
+    async def source_credentials(self, source_name: str) -> Any: ...  # type: ignore [override]
 
 class AioContainerProvider(ContainerProvider):
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...
-    async def load(self) -> AioRefreshableCredentials: ...  # type: ignore
+    async def load(self) -> AioRefreshableCredentials: ...  # type: ignore [override]
 
 class AioCredentialResolver(CredentialResolver):
-    async def load_credentials(self) -> Any: ...  # type: ignore
+    async def load_credentials(self) -> Any: ...  # type: ignore [override]
 
 class AioSSOCredentialFetcher(AioCachedCredentialFetcher):
     def __init__(
         self,
         start_url: str,
         sso_region: str,
         role_name: str,
@@ -152,8 +154,8 @@
         client_creator: Any,
         token_loader: Optional[Any] = ...,
         cache: Optional[Any] = ...,
         expiry_window_seconds: Optional[Any] = ...,
     ) -> None: ...
 
 class AioSSOProvider(SSOProvider):
-    async def load(self) -> AioDeferredRefreshableCredentials: ...  # type: ignore
+    async def load(self) -> AioDeferredRefreshableCredentials: ...  # type: ignore [override]
```

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/endpoint.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/endpoint.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class AioEndpoint(Endpoint):
     async def create_request(
         self, params: Any, operation_model: Optional[Any] = ...
     ) -> Request: ...
 
 class AioEndpointCreator(EndpointCreator):
-    def create_endpoint(  # type: ignore
+    def create_endpoint(  # type: ignore [override]
         self,
         service_model: ServiceModel,
         region_name: str,
         endpoint_url: str,
         verify: Optional[Any] = ...,
         response_parser_factory: Optional[Any] = ...,
         timeout: int = ...,
```

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/handlers.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/handlers.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/httpsession.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/httpsession.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/paginate.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/paginate.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 class AioPageIterator(PageIterator):
     def __aiter__(self) -> Any: ...
     resume_token: Any
     async def __anext__(self) -> Iterator[Any]: ...
     def result_key_iters(self) -> Any: ...
     async def build_full_result(self) -> Any: ...
-    async def search(self, expression: str) -> Iterator[Any]: ...  # type: ignore
+    async def search(self, expression: str) -> Iterator[Any]: ...  # type: ignore [override]
 
 class AioPaginator(Paginator):
     PAGE_ITERATOR_CLS: Type[AioPageIterator]
 
 class ResultKeyIterator:
     result_key: str
     def __init__(self, pages_iterator: PageIterator, result_key: str) -> None: ...
```

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/parsers.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/parsers.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/response.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/response.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/session.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/session.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -27,35 +27,35 @@
     def register(
         self,
         event_name: str,
         handler: Any,
         unique_id: Optional[Any] = ...,
         unique_id_uses_count: bool = ...,
     ) -> None: ...
-    def create_client(  # type: ignore
+    def create_client(  # type: ignore [override]
         self,
         service_name: str,
         region_name: Optional[str] = ...,
         use_ssl: Optional[bool] = ...,
         endpoint_url: Optional[str] = ...,
         verify: Union[str, bool, None] = ...,
         aws_access_key_id: Optional[str] = ...,
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         api_version: Optional[str] = ...,
         config: Optional[Config] = ...,
     ) -> AioBaseClient: ...
-    async def get_credentials(self) -> AioCredentials: ...  # type: ignore
+    async def get_credentials(self) -> AioCredentials: ...  # type: ignore [override]
     def set_credentials(
         self, access_key: str, secret_key: str, token: Optional[Any] = ...
     ) -> None: ...
-    async def get_service_model(  # type: ignore
+    async def get_service_model(  # type: ignore [override]
         self, service_name: str, api_version: Optional[Any] = ...
     ) -> ServiceModel: ...
     async def get_service_data(
         self, service_name: str, api_version: Optional[Any] = ...
     ) -> Any: ...
-    async def get_available_regions(  # type: ignore
+    async def get_available_regions(  # type: ignore [override]
         self, service_name: str, partition_name: str = ..., allow_non_regional: bool = ...
     ) -> List[str]: ...
 
 def get_session(env_vars: Optional[Any] = ...) -> AioSession: ...
```

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/signers.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/signers.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from botocore.signers import RequestSigner, S3PostPresigner
 from requests.models import Request
 
 class AioRequestSigner(RequestSigner):
     async def handler(
         self, operation_name: Optional[Any] = ..., request: Optional[Any] = ..., **kwargs: Any
     ) -> None: ...
-    async def sign(  # type: ignore
+    async def sign(  # type: ignore [override]
         self,
         operation_name: str,
         request: Request,
         region_name: Optional[Any] = ...,
         signing_type: str = ...,
         expires_in: Optional[Any] = ...,
         signing_name: Optional[Any] = ...,
```

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/utils.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/utils.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 class AioInstanceMetadataFetcher(AioIMDSFetcher, InstanceMetadataFetcher):
     async def retrieve_iam_role_credentials(self) -> Dict[str, Any]: ...
 
 class AioIMDSRegionProvider(IMDSRegionProvider):
     async def provide(self) -> str: ...
 
 class AioInstanceMetadataRegionFetcher(AioIMDSFetcher, InstanceMetadataRegionFetcher):
-    async def retrieve_region(self) -> Optional[str]: ...  # type: ignore
+    async def retrieve_region(self) -> Optional[str]: ...  # type: ignore [override]
 
 class AioS3RegionRedirector(S3RegionRedirector):
     async def redirect_from_error(
         self, request_dict: Dict[str, Any], response: Response, operation: Any, **kwargs: Any
     ) -> Optional[int]: ...
     async def get_bucket_region(self, bucket: str, response: Response) -> str: ...
```

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/aiobotocore/waiter.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/aiobotocore/waiter.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 from botocore.waiter import Waiter
 from botocore.waiter import WaiterModel as WaiterModel
 
 class NormalizedOperationMethod(_NormalizedOperationMethod):
     async def __call__(self, **kwargs: Any) -> Any: ...
 
 class AIOWaiter(Waiter):
-    async def wait(self, **kwargs: Any) -> None: ...  # type: ignore
+    async def wait(self, **kwargs: Any) -> None: ...  # type: ignore [override]
 
 def create_waiter_with_client(
     waiter_name: str, waiter_model: WaiterModel, client: BaseClient
 ) -> AIOWaiter: ...
```

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/__init__.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/docs/utils.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/docs/utils.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/dynamodb/conditions.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/dynamodb/conditions.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/dynamodb/table.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/dynamodb/table.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/dynamodb/transform.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/dynamodb/transform.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/dynamodb/types.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/dynamodb/types.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/exceptions.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/resources/action.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/resources/action.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         service_context: Optional[ServiceContext] = ...,
     ) -> None: ...
     def __call__(
         self, parent: ServiceResource, *args: Any, **kwargs: Any
     ) -> Union[ServiceResource, List[ServiceResource], Dict[str, Any]]: ...
 
 class BatchAction(ServiceAction):
-    def __call__(  # type: ignore
+    def __call__(  # type: ignore [override]
         self, parent: ResourceCollection, *args: Any, **kwargs: Any
     ) -> List[Dict[str, Any]]: ...
 
 class WaiterAction:
     def __init__(self, waiter_model: Waiter, waiter_resource_name: str) -> None: ...
     def __call__(self, parent: ServiceResource, *args: Any, **kwargs: Any) -> None: ...
```

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/resources/base.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/resources/base.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/resources/collection.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/resources/collection.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/resources/model.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/resources/model.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/resources/params.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/resources/params.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/resources/response.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/resources/response.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/s3/transfer.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/s3/transfer.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from typing import Any, Callable, Dict, List, Mapping, Optional, TypeVar
 
 from botocore.client import BaseClient
 from botocore.config import Config
-from s3transfer.futures import TransferFuture
 from s3transfer.manager import TransferConfig as S3TransferConfig
 from s3transfer.manager import TransferManager
 from s3transfer.subscribers import BaseSubscriber
 from s3transfer.utils import OSUtils
 
 _R = TypeVar("_R")
 
 KB: int
 MB: int
 
 def create_transfer_manager(
     client: BaseClient,
-    config: Config,
-    osutil: Optional[OSUtils] = ...,  # type: ignore
+    config: TransferConfig,
+    osutil: Optional[OSUtils] = ...,
 ) -> TransferManager: ...
 
 class TransferConfig(S3TransferConfig):
     ALIAS: Dict[str, str]
 
     def __init__(
         self,
@@ -39,16 +38,16 @@
 class S3Transfer:
     ALLOWED_DOWNLOAD_ARGS: List[str]
     ALLOWED_UPLOAD_ARGS: List[str]
     def __init__(
         self,
         client: Optional[BaseClient] = ...,
         config: Optional[Config] = ...,
-        osutil: Optional[OSUtils] = ...,  # type: ignore
-        manager: Optional[TransferManager] = ...,  # type: ignore
+        osutil: Optional[OSUtils] = ...,
+        manager: Optional[TransferManager] = ...,
     ) -> None: ...
     def upload_file(
         self,
         filename: str,
         bucket: str,
         key: str,
         callback: Optional[Callable[[int], Any]] = ...,
@@ -64,8 +63,10 @@
     ) -> None: ...
     def __enter__(self: _R) -> _R: ...
     def __exit__(self, *args: Any) -> None: ...
 
 class ProgressCallbackInvoker(BaseSubscriber):
     def __init__(self, callback: Callable[[int], Any]) -> None: ...
     # FIXME: signature incompatible with BaseSubscriber
-    def on_progress(self, bytes_transferred: int, **kwargs: Any) -> None: ...  # type: ignore
+    def on_progress(  # type: ignore [override]
+        self, bytes_transferred: int, **kwargs: Any
+    ) -> None: ...
```

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/session.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/session.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/boto3/utils.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/boto3/utils.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/__init__.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/args.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/args.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/auth.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/auth.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/awsrequest.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/awsrequest.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/client.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/compat.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/compat.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/config.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/config.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/configprovider.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/configprovider.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/credentials.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/credentials.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/crt/auth.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/crt/auth.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/discovery.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/discovery.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/endpoint.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/endpoint.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/errorfactory.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/errorfactory.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/eventstream.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/eventstream.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/exceptions.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/handlers.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/handlers.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/history.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/history.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/hooks.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/hooks.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/httpsession.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/httpsession.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/loaders.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/loaders.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/model.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/model.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/monitoring.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/monitoring.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/paginate.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/paginate.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/parsers.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/parsers.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/regions.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/regions.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         partition_name: str = ...,
         allow_non_regional: bool = ...,
         endpoint_variant_tags: Any = ...,
     ) -> List[str]: ...
     def get_partition_dns_suffix(
         self, partition_name: str, endpoint_variant_tags: Any = ...
     ) -> str: ...
-    def construct_endpoint(  # type: ignore
+    def construct_endpoint(  # type: ignore [override]
         self,
         service_name: str,
         region_name: Optional[str] = ...,
         partition_name: Optional[str] = ...,
         use_dualstack_endpoint: bool = ...,
         use_fips_endpoint: bool = ...,
     ) -> Optional[Dict[str, Any]]: ...
```

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/response.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/response.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class StreamingBody(IOBase):
     def __init__(self, raw_stream: IO[bytes], content_length: int) -> None: ...
     def set_socket_timeout(self, timeout: float) -> None: ...
     def readable(self) -> bool: ...
     def read(self, amt: Optional[int] = ...) -> bytes: ...
     # FIXME: Signature of "readlines" incompatible with supertype "IOBase"
-    def readlines(self) -> List[bytes]: ...  # type: ignore
+    def readlines(self) -> List[bytes]: ...  # type: ignore [override]
     def __iter__(self) -> Iterator[bytes]: ...
     def iter_lines(self, chunk_size: int = ..., keepends: bool = ...) -> Iterator[bytes]: ...
     def iter_chunks(self, chunk_size: int = ...) -> Iterator[bytes]: ...
     def tell(self) -> int: ...
     def close(self) -> None: ...
     def next(self) -> bytes: ...
```

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/retries/adaptive.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/retries/adaptive.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/retries/bucket.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/retries/bucket.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/retries/standard.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/retries/standard.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/retryhandler.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/retryhandler.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     def __init__(
         self,
         checker: BaseChecker,
         max_attempts: int,
         retryable_exceptions: Optional[Iterable[Type[Exception]]] = ...,
     ) -> None: ...
     # FIXME: Signature of "__call__" incompatible with supertype "BaseChecker"
-    def __call__(  # type: ignore
+    def __call__(  # type: ignore [override]
         self,
         attempt_number: int,
         response: Mapping[str, Any],
         caught_exception: Exception,
         retries_context: Any,
     ) -> bool: ...
```

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/serialize.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/serialize.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/session.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/session.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/signers.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/signers.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/stub.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/stub.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/utils.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/utils.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/validate.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/validate.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/stubs_static/botocore/waiter.pyi` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/stubs_static/botocore/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aioboto3_service_docs/README.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aioboto3_service_docs/README.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aioboto3_service_docs/client.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aioboto3_service_docs/client.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aioboto3_service_docs/literals.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aioboto3_service_docs/literals.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aioboto3_service_docs/paginators.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aioboto3_service_docs/paginators.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aioboto3_service_docs/service_resource.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aioboto3_service_docs/service_resource.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aioboto3_service_docs/type_defs.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aioboto3_service_docs/type_defs.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aioboto3_service_docs/usage.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aioboto3_service_docs/usage.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aioboto3_service_docs/waiters.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aioboto3_service_docs/waiters.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore-stubs/README.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore-stubs/README.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore-stubs/aiobotocore-stubs/__main__.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore-stubs/aiobotocore-stubs/__main__.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore-stubs/aiobotocore-stubs/session.pyi.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore-stubs/aiobotocore-stubs/session.pyi.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore-stubs/setup.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore-stubs/setup.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/README.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/README.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/service/__init__.pyi.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/service/__init__.pyi.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/service/__main__.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/service/__main__.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/service/client.pyi.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/service/client.pyi.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/service/literals.pyi.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/service/literals.pyi.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/service/paginator.pyi.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/service/paginator.pyi.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/service/service_resource.pyi.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/service/service_resource.pyi.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/service/type_defs.pyi.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/service/type_defs.pyi.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/service/waiter.pyi.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/service/waiter.pyi.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service/setup.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service/setup.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service_docs/README.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service_docs/README.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service_docs/client.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service_docs/client.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service_docs/literals.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service_docs/literals.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service_docs/paginators.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service_docs/paginators.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service_docs/service_resource.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service_docs/service_resource.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service_docs/type_defs.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service_docs/type_defs.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service_docs/usage.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service_docs/usage.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_service_docs/waiters.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_service_docs/waiters.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/aiobotocore_stubs_docs/README.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/aiobotocore_stubs_docs/README.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3-stubs/README.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3-stubs/README.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3-stubs/boto3-stubs/__init__.pyi.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3-stubs/boto3-stubs/__init__.pyi.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3-stubs/boto3-stubs/__main__.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3-stubs/boto3-stubs/__main__.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3-stubs/boto3-stubs/session.pyi.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3-stubs/boto3-stubs/session.pyi.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3-stubs/setup.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3-stubs/setup.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/README.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/README.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/service/__init__.pyi.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/service/__init__.pyi.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/service/__main__.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/service/__main__.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/service/client.pyi.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/service/client.pyi.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/service/literals.pyi.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/service/literals.pyi.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/service/paginator.pyi.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/service/paginator.pyi.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/service/service_resource.pyi.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/service/service_resource.pyi.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/service/type_defs.pyi.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/service/type_defs.pyi.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/service/waiter.pyi.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/service/waiter.pyi.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service/setup.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service/setup.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service_docs/README.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service_docs/README.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service_docs/client.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service_docs/client.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service_docs/literals.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service_docs/literals.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service_docs/paginators.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service_docs/paginators.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service_docs/service_resource.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service_docs/service_resource.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service_docs/type_defs.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service_docs/type_defs.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service_docs/usage.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service_docs/usage.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_service_docs/waiters.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_service_docs/waiters.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/boto3_stubs_docs/README.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/boto3_stubs_docs/README.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/botocore-stubs/README.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/botocore-stubs/README.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/botocore-stubs/botocore-stubs/__main__.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/botocore-stubs/botocore-stubs/__main__.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/botocore-stubs/setup.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/botocore-stubs/setup.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/arguments_list_code.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/arguments_list_code.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/class.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/class.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/footer.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/footer.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/function.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/function.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/how_to_install.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/how_to_install.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/how_to_install_service.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/how_to_install_service.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/import_groups.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/import_groups.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/import_record.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/import_record.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/method.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/method.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/method_code.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/method_code.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/module.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/module.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/submodules.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/submodules.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/type_annotation.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/type_annotation.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/type_annotation_code.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/type_annotation_code.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/type_hint.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/type_hint.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/typed_dict.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/typed_dict.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/common/usage.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/common/usage.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/master/README.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/master/README.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/master/mypy_boto3/boto3_init_stub.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/master/mypy_boto3/boto3_init_stub.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/master/mypy_boto3/boto3_session_stub.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/master/mypy_boto3/boto3_session_stub.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/master/mypy_boto3/main.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/master/mypy_boto3/main.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/master/mypy_boto3/submodules.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/master/mypy_boto3/submodules.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/master/setup.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/master/setup.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/types-aioboto3/README.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/types-aioboto3/README.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/types-aioboto3/aioboto3-stubs/__main__.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/types-aioboto3/aioboto3-stubs/__main__.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/types-aioboto3/aioboto3-stubs/session.pyi.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/types-aioboto3/aioboto3-stubs/session.pyi.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/types-aioboto3/setup.py.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/types-aioboto3/setup.py.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/templates/types_aioboto3_docs/README.md.jinja2` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/templates/types_aioboto3_docs/README.md.jinja2`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/external_import.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/external_import.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/fake_annotation.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/fake_annotation.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/internal_import.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/internal_import.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/remove_argument.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/remove_argument.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/type.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/type.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/type_annotation.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/type_annotation.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/type_class.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/type_class.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/type_constant.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/type_constant.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/type_literal.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/type_literal.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/type_subscript.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/type_subscript.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_annotations/type_typed_dict.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_annotations/type_typed_dict.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_maps/docstring_type_map.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_maps/docstring_type_map.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_maps/literal_type_map.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_maps/literal_type_map.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_maps/method_argument_map.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_maps/method_argument_map.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_maps/method_type_map.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_maps/method_type_map.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_maps/shape_type_map.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_maps/shape_type_map.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/type_maps/typed_dicts.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/type_maps/typed_dicts.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/utils/boto3_utils.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/utils/boto3_utils.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/utils/botocore_changelog.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/utils/botocore_changelog.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/utils/markdown.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/utils/markdown.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/utils/nice_path.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/utils/nice_path.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/utils/pypi_manager.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/utils/pypi_manager.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/utils/strings.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/utils/strings.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/utils/typed_dict_sorter.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/utils/typed_dict_sorter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/utils/version.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/utils/version.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/writers/aioboto3_processors.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/writers/aioboto3_processors.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/writers/aiobotocore_processors.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/writers/aiobotocore_processors.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/writers/package_writer.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/writers/package_writer.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/writers/processors.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/writers/processors.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/mypy_boto3_builder/writers/utils.py` & `mypy-boto3-builder-7.9.2/mypy_boto3_builder/writers/utils.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-builder-7.9.1/pyproject.toml` & `mypy-boto3-builder-7.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "mypy_boto3_builder",
     "tests",
 ]
 src_paths = []
 
 [tool.poetry]
 name = "mypy-boto3-builder"
-version = "7.9.1"
+version = "7.9.2"
 description = "Builder for boto3-stubs and types-aiobotocore"
 authors = ["Vlad Emelianov <vlad.emelianov.nz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://youtype.github.io/mypy_boto3_builder/"
 repository = "https://github.com/youtype/mypy_boto3_builder"
 documentation = "https://youtype.github.io/mypy_boto3_builder/"
```

### Comparing `mypy-boto3-builder-7.9.1/setup.py` & `mypy-boto3-builder-7.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
  'requests']
 
 entry_points = \
 {'console_scripts': ['mypy_boto3_builder = mypy_boto3_builder.main:main']}
 
 setup_kwargs = {
     'name': 'mypy-boto3-builder',
-    'version': '7.9.1',
+    'version': '7.9.2',
     'description': 'Builder for boto3-stubs and types-aiobotocore',
     'long_description': "# mypy_boto3_builder\n\n[![Open in Visual Studio Code](https://open.vscode.dev/badges/open-in-vscode.svg)](https://open.vscode.dev/youtype/mypy_boto3_builder)\n\n[![PyPI - mypy-boto3-builder](https://img.shields.io/pypi/v/mypy-boto3-builder.svg?color=blue&label=mypy-boto3-builder)](https://pypi.org/project/mypy-boto3-builder)\n[![PyPI - boto3-stubs](https://img.shields.io/pypi/v/boto3-stubs.svg?color=blue&label=boto3-stubs)](https://pypi.org/project/boto3-stubs)\n[![PyPI - boto3](https://img.shields.io/pypi/v/boto3.svg?color=blue&label=boto3)](https://pypi.org/project/boto3)\n\n[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue&label=boto3-stubs%20docs)](https://youtype.github.io/boto3_stubs_docs/)\n[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue&label=Builder%20docs)](https://mypy-boto3-builder.readthedocs.io/)\n\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs.svg?color=blue)](https://pypi.org/project/boto3-stubs)\n[![PyPI - Downloads](https://img.shields.io/pypi/dm/boto3-stubs?color=blue)](https://pypistats.org/packages/boto3-stubs)\n\n![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)\n\nType annotations builder for [boto3-stubs](https://pypi.org/project/boto3-stubs/) project. Compatible with\n[VSCode](https://code.visualstudio.com/),\n[PyCharm](https://www.jetbrains.com/pycharm/),\n[Emacs](https://www.gnu.org/software/emacs/),\n[Sublime Text](https://www.sublimetext.com/),\n[mypy](https://github.com/python/mypy),\n[pyright](https://github.com/microsoft/pyright)\nand other tools.\n\nSee how it helps to find and fix potential bugs:\n\n![boto3-stubs demo](https://raw.githubusercontent.com/youtype/mypy_boto3_builder/main/demo.gif)\n\nDo you want more? Check the [documentation](https://youtype.github.io/boto3_stubs_docs/) and use `boto3` like a pro!\n\n- [mypy_boto3_builder](#mypy_boto3_builder)\n  - [Using built libraries](#using-built-libraries)\n    - [boto3](#boto3)\n    - [aiobotocore](#aiobotocore)\n    - [aioboto3](#aioboto3)\n  - [How to build type annotations](#how-to-build-type-annotations)\n    - [Locally](#locally)\n    - [With Docker image](#with-docker-image)\n  - [Development](#development)\n  - [Versioning](#versioning)\n  - [Latest changes](#latest-changes)\n  - [Thank you](#thank-you)\n    - [Toolset](#toolset)\n    - [Contributors](#contributors)\n\n## Using built libraries\n\n### boto3\n\nCheck [boto3-stubs](https://pypi.org/project/boto3-stubs/) project for installation\nand usage instructions.\n\nIf you use VSCode, add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)\nextension to your VSCode and run `AWS boto3: Quick Start` command.\n\nIf not, just install `boto3-stubs` with `pip`:\n\n```bash\npython -m pip install 'boto3-stubs[essential]'\n\n# Lite version does not provide session.client/resource overloads\n# it is more RAM-friendly, but requires explicit type annotations\npython -m pip install 'boto3-stubs-lite[essential]'\n\n# do not forget to install mypy or pyright\n```\n\nThat's it! You should already have code completion and type checking in your IDE.\n\n### aiobotocore\n\nCheck [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) project for installation\nand usage instructions.\n\nOr just install `types-aiobotocore` with `pip`:\n\n```bash\npython -m pip install 'types-aiobotocore[essential]'\n\n# Lite version does not provide session.create_client overloads\n# it is more RAM-friendly, but requires explicit type annotations\npython -m pip install 'types-aiobotocore-lite[essential]'\n\n# do not forget to install mypy or pyright\n```\n\nReady to go! Enjoy code completion and type checking in your `aiobotocore` project.\n\n### aioboto3\n\nCheck [types-aioboto3](https://pypi.org/project/types-aioboto3/) project for installation\nand usage instructions.\n\nOr just install `types-aioboto3` with `pip`:\n\n```bash\npython -m pip install 'types-aioboto3[essential]'\n\n# Lite version does not provide session.client/resource overloads\n# it is more RAM-friendly, but requires explicit type annotations\npython -m pip install 'types-aioboto3-lite[essential]'\n\n# do not forget to install mypy or pyright\n```\n\nWhoa! All `aioboto3` methods and attributes are now type-annotated and even code completion works.\n\n## How to build type annotations\n\n### Locally\n\n```bash\n# Install preferred version of `boto3`\npython -m pip install boto3==1.16.25 botocore==1.19.25\n\n# Install `mypy-boto3-builder`\npython -m pip install mypy-boto3-builder\n\n# Build all packages in mypy_boto3_output directory\npython -m mypy_boto3_builder mypy_boto3_output\n\n# Or specify required services explicitly\npython -m mypy_boto3_builder mypy_boto3_output -s ec2 s3\n\n# Install custom `boto3-stubs` packages\ncd mypy_boto3_output\npython -m pip install -e ./mypy_boto3_ec2_package\npython -m pip install -e ./mypy_boto3_s3_package\npython -m pip install -e ./boto3_stubs_package\n```\n\n### With Docker image\n\n- Install [Docker](https://docs.docker.com/install/)\n- Pull latest `mypy_boto3_builder` version and tag it\n\n```bash\ndocker pull docker.pkg.github.com/youtype/mypy_boto3_builder/mypy_boto3_builder_stable:latest\ndocker tag docker.pkg.github.com/youtype/mypy_boto3_builder/mypy_boto3_builder_stable:latest mypy_boto3_builder\n```\n\n- Generate stubs in `output` directory\n\n```bash\nmkdir output\n\n# generate stubs for all services\ndocker run -v `pwd`/output:/output -ti mypy_boto3_builder_stable\n\n# generate stubs for s3 service\ndocker run -v `pwd`/output:/output -ti mypy_boto3_builder_stable -s s3\n\n# generate stubs for a specific boto3 version\ndocker run -e BOTO3_VERSION=1.16.25 BOTOCORE_VERSION=1.19.25 -v `pwd`/output:/output -ti mypy_boto3_builder_stable\n```\n\n- Install packages from `output` directory as described above\n\n## Development\n\n- Install Python 3.10+, ideally with [pyenv](https://github.com/pyenv/pyenv)\n- Install [poetry](https://python-poetry.org/): `pip install poetry`\n- Install dependencies: `poetry install`\n- Use scripts for repo to check if everything works: `./scripts/build.sh`\n- Run manual pre-commit: `./scripts/before_commit.sh`\n\n## Versioning\n\n`mypy_boto3_builder` version is not related to `boto3` version and follows\n[PEP 440](https://www.python.org/dev/peps/pep-0440/).\n\n## Latest changes\n\nFull changelog can be found in [Releases](https://github.com/youtype/mypy_boto3_builder/releases).\n\n## Thank you\n\n### Toolset\n\n- [black](https://github.com/psf/black) developers for an awesome formatting tool\n- [Timothy Edmund Crosley](https://github.com/timothycrosley) for\n  [isort](https://github.com/PyCQA/isort) and how flexible it is\n- [mypy](https://github.com/python/mypy) developers for doing all dirty work for us\n- [pyright](https://github.com/microsoft/pyright) team for the new era of typed Python\n\n### Contributors\n\n- [Allie Fitter](https://github.com/alliefitter), author of original\n  [boto3-type-annotations](https://pypi.org/project/boto3-type-annotations/)\n- [jbpratt](https://github.com/jbpratt)\n- [Chris Hollinworth](https://github.com/chrishollinworth)\n- [Yoan Blanc](https://github.com/greut)\n- [Kostya Leschenko](https://github.com/kleschenko)\n- [pyto86](https://github.com/pyto86pri)\n- [Ashton Honnecke](https://github.com/ahonnecke)\n- [Mike Carey](https://github.com/mike-carey)\n- [Ole-Martin Bratteng](https://github.com/omBratteng)\n- [Nikhil Benesch](https://github.com/benesch)\n",
     'author': 'Vlad Emelianov',
     'author_email': 'vlad.emelianov.nz@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://youtype.github.io/mypy_boto3_builder/',
```

### Comparing `mypy-boto3-builder-7.9.1/PKG-INFO` & `mypy-boto3-builder-7.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-builder
-Version: 7.9.1
+Version: 7.9.2
 Summary: Builder for boto3-stubs and types-aiobotocore
 Home-page: https://youtype.github.io/mypy_boto3_builder/
 License: MIT
 Keywords: boto3,type-annotations,pyright,mypy,boto3-stubs
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 Requires-Python: >=3.10,<4.0
```

