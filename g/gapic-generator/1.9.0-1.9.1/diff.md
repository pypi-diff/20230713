# Comparing `tmp/gapic-generator-1.9.0.tar.gz` & `tmp/gapic-generator-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gapic-generator-1.9.0.tar", last modified: Fri Mar 17 11:28:01 2023, max compression
+gzip compressed data, was "gapic-generator-1.9.1.tar", last modified: Wed Mar 22 16:41:14 2023, max compression
```

## Comparing `gapic-generator-1.9.0.tar` & `gapic-generator-1.9.1.tar`

### file list

```diff
@@ -1,755 +1,756 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.375412 gapic-generator-1.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      182 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     2285 2023-03-17 11:28:01.375412 gapic-generator-1.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     1237 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.263397 gapic-generator-1.9.0/gapic/
--rw-rw-r--   0 root         (0)     1003      575 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.263397 gapic-generator-1.9.0/gapic/cli/
--rw-rw-r--   0 root         (0)     1003      575 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/cli/__init__.py
--rw-rw-r--   0 root         (0)     1003     1632 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/cli/dump.py
--rw-rw-r--   0 root         (0)     1003     2548 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/cli/generate.py
--rw-rw-r--   0 root         (0)     1003      446 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/cli/generate_with_pandoc.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.263397 gapic-generator-1.9.0/gapic/configurable_snippetgen/
--rw-rw-r--   0 root         (0)     1003      574 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/configurable_snippetgen/__init__.py
--rw-rw-r--   0 root         (0)     1003     9620 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/configurable_snippetgen/configured_snippet.py
--rw-rw-r--   0 root         (0)     1003     2669 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/configurable_snippetgen/libcst_utils.py
--rw-rw-r--   0 root         (0)     1003    43112 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/configurable_snippetgen/snippet_config_language.proto
--rw-rw-r--   0 root         (0)     1003    27715 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/configurable_snippetgen/snippet_config_language_pb2.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.263397 gapic-generator-1.9.0/gapic/generator/
--rw-rw-r--   0 root         (0)     1003      843 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/generator/__init__.py
--rw-rw-r--   0 root         (0)     1003     1451 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/generator/formatter.py
--rw-rw-r--   0 root         (0)     1003    17499 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/generator/generator.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.267397 gapic-generator-1.9.0/gapic/samplegen/
--rw-rw-r--   0 root         (0)     1003      703 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/samplegen/__init__.py
--rw-rw-r--   0 root         (0)     1003     4513 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/samplegen/manifest.py
--rw-rw-r--   0 root         (0)     1003    48624 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/samplegen/samplegen.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.267397 gapic-generator-1.9.0/gapic/samplegen_utils/
--rw-rw-r--   0 root         (0)     1003      737 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/samplegen_utils/__init__.py
--rw-rw-r--   0 root         (0)     1003     8189 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/samplegen_utils/snippet_index.py
--rw-rw-r--   0 root         (0)     1003    10573 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/samplegen_utils/snippet_metadata.proto
--rw-rw-r--   0 root         (0)     1003    10134 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/samplegen_utils/snippet_metadata_pb2.py
--rw-rw-r--   0 root         (0)     1003     2420 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/samplegen_utils/types.py
--rw-rw-r--   0 root         (0)     1003     4761 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/samplegen_utils/utils.py
--rw-rw-r--   0 root         (0)     1003     3728 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/samplegen_utils/yaml.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.267397 gapic-generator-1.9.0/gapic/schema/
--rw-rw-r--   0 root         (0)     1003      993 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/schema/__init__.py
--rw-rw-r--   0 root         (0)     1003    52170 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/schema/api.py
--rw-rw-r--   0 root         (0)     1003     1223 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/schema/imp.py
--rw-rw-r--   0 root         (0)     1003    16394 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/schema/metadata.py
--rw-rw-r--   0 root         (0)     1003     2465 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/schema/mixins.py
--rw-rw-r--   0 root         (0)     1003     8771 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/schema/naming.py
--rw-rw-r--   0 root         (0)     1003    69198 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/schema/wrappers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.271398 gapic-generator-1.9.0/gapic/templates/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.247394 gapic-generator-1.9.0/gapic/templates/%namespace/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.271398 gapic-generator-1.9.0/gapic/templates/%namespace/%name/
--rw-rw-r--   0 root         (0)     1003     3226 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name/__init__.py.j2
--rw-rw-r--   0 root         (0)     1003      115 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name/gapic_version.py.j2
--rw-rw-r--   0 root         (0)     1003      100 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name/py.typed.j2
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.271398 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.271398 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/
--rw-rw-r--   0 root         (0)     1003     2285 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/__init__.py.j2
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.271398 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.271398 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/
--rw-rw-r--   0 root         (0)     1003      356 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/__init__.py.j2
--rw-rw-r--   0 root         (0)     1003    27851 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/_async_mixins.py.j2
--rw-rw-r--   0 root         (0)     1003    12207 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/_client_macros.j2
--rw-rw-r--   0 root         (0)     1003    27648 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/_mixins.py.j2
--rw-rw-r--   0 root         (0)     1003    30862 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/async_client.py.j2
--rw-rw-r--   0 root         (0)     1003    30675 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/client.py.j2
--rw-rw-r--   0 root         (0)     1003     6958 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/pagers.py.j2
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.275398 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/
--rw-rw-r--   0 root         (0)     1003     1232 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/__init__.py.j2
--rw-rw-r--   0 root         (0)     1003    10632 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/_mixins.py.j2
--rw-rw-r--   0 root         (0)     1003     3686 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/_rest_mixins.py.j2
--rw-rw-r--   0 root         (0)     1003    13074 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/base.py.j2
--rw-rw-r--   0 root         (0)     1003    17307 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/grpc.py.j2
--rw-rw-r--   0 root         (0)     1003    17598 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/grpc_asyncio.py.j2
--rw-rw-r--   0 root         (0)     1003    19419 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/rest.py.j2
--rw-rw-r--   0 root         (0)     1003       28 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/__init__.py.j2
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.275398 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/types/
--rw-rw-r--   0 root         (0)     1003     1227 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/types/%proto.py.j2
--rw-rw-r--   0 root         (0)     1003      646 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/types/__init__.py.j2
--rw-rw-r--   0 root         (0)     1003      639 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/types/_enum.py.j2
--rw-rw-r--   0 root         (0)     1003     4291 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/types/_message.py.j2
--rw-rw-r--   0 root         (0)     1003       37 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/gapic_metadata.json.j2
--rw-rw-r--   0 root         (0)     1003      115 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/gapic_version.py.j2
--rw-rw-r--   0 root         (0)     1003      100 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/py.typed.j2
--rw-rw-r--   0 root         (0)     1003      359 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/.coveragerc.j2
--rw-rw-r--   0 root         (0)     1003      879 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/.flake8.j2
--rw-rw-r--   0 root         (0)     1003      200 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/MANIFEST.in.j2
--rw-rw-r--   0 root         (0)     1003     1461 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/README.rst.j2
--rw-rw-r--   0 root         (0)     1003      122 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/_base.py.j2
--rw-rw-r--   0 root         (0)     1003      576 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/_license.j2
--rw-rw-r--   0 root         (0)     1003     1042 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/_pypi_packages.j2
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.275398 gapic-generator-1.9.0/gapic/templates/docs/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.275398 gapic-generator-1.9.0/gapic/templates/docs/%name_%version/
--rw-rw-r--   0 root         (0)     1003      528 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/docs/%name_%version/%service.rst.j2
--rw-rw-r--   0 root         (0)     1003      296 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/docs/%name_%version/services.rst.j2
--rw-rw-r--   0 root         (0)     1003      283 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/docs/%name_%version/types.rst.j2
--rw-rw-r--   0 root         (0)     1003    12131 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/docs/conf.py.j2
--rw-rw-r--   0 root         (0)     1003      164 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/docs/index.rst.j2
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.275398 gapic-generator-1.9.0/gapic/templates/examples/
--rw-rw-r--   0 root         (0)     1003      386 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/examples/_generated_sample_comment.j2
--rw-rw-r--   0 root         (0)     1003    12491 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/examples/feature_fragments.j2
--rw-rw-r--   0 root         (0)     1003     1926 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/examples/sample.py.j2
--rw-rw-r--   0 root         (0)     1003       54 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/mypy.ini.j2
--rw-rw-r--   0 root         (0)     1003     4502 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/noxfile.py.j2
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.275398 gapic-generator-1.9.0/gapic/templates/scripts/
--rw-rw-r--   0 root         (0)     1003     6479 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/scripts/fixup_%name_%version_keywords.py.j2
--rw-rw-r--   0 root         (0)     1003     3300 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/setup.py.j2
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.279399 gapic-generator-1.9.0/gapic/templates/testing/
--rw-rw-r--   0 root         (0)     1003      521 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/testing/_default_constraints.j2
--rw-rw-r--   0 root         (0)     1003      110 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/testing/constraints-3.10.txt.j2
--rw-rw-r--   0 root         (0)     1003      110 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/testing/constraints-3.11.txt.j2
--rw-rw-r--   0 root         (0)     1003      111 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/testing/constraints-3.12.txt.j2
--rw-rw-r--   0 root         (0)     1003      768 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/testing/constraints-3.7.txt.j2
--rw-rw-r--   0 root         (0)     1003      110 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/testing/constraints-3.8.txt.j2
--rw-rw-r--   0 root         (0)     1003      110 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/testing/constraints-3.9.txt.j2
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.279399 gapic-generator-1.9.0/gapic/templates/tests/
--rw-rw-r--   0 root         (0)     1003       29 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/tests/__init__.py.j2
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.279399 gapic-generator-1.9.0/gapic/templates/tests/unit/
--rw-rw-r--   0 root         (0)     1003       29 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/tests/unit/__init__.py.j2
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.279399 gapic-generator-1.9.0/gapic/templates/tests/unit/gapic/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.251395 gapic-generator-1.9.0/gapic/templates/tests/unit/gapic/%name_%version/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.279399 gapic-generator-1.9.0/gapic/templates/tests/unit/gapic/%name_%version/%sub/
--rw-rw-r--   0 root         (0)     1003       29 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/tests/unit/gapic/%name_%version/%sub/__init__.py.j2
--rw-rw-r--   0 root         (0)     1003    67200 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/tests/unit/gapic/%name_%version/%sub/_test_mixins.py.j2
--rw-rw-r--   0 root         (0)     1003    62369 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/tests/unit/gapic/%name_%version/%sub/test_%service.py.j2
--rw-rw-r--   0 root         (0)     1003    64283 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/tests/unit/gapic/%name_%version/%sub/test_macros.j2
--rw-rw-r--   0 root         (0)     1003       29 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/templates/tests/unit/gapic/__init__.py.j2
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.283399 gapic-generator-1.9.0/gapic/utils/
--rw-rw-r--   0 root         (0)     1003     1644 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/utils/__init__.py
--rw-rw-r--   0 root         (0)     1003     1424 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/utils/cache.py
--rw-rw-r--   0 root         (0)     1003     2172 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/utils/case.py
--rw-rw-r--   0 root         (0)     1003     1155 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/utils/checks.py
--rw-rw-r--   0 root         (0)     1003     2369 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/utils/code.py
--rw-rw-r--   0 root         (0)     1003     1035 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/utils/doc.py
--rw-rw-r--   0 root         (0)     1003     1377 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/utils/filename.py
--rw-rw-r--   0 root         (0)     1003     4546 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/utils/lines.py
--rw-rw-r--   0 root         (0)     1003     8459 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/utils/options.py
--rw-rw-r--   0 root         (0)     1003     1215 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/utils/reserved_names.py
--rw-rw-r--   0 root         (0)     1003     2655 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/utils/rst.py
--rw-rw-r--   0 root         (0)     1003     1696 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/utils/uri_conv.py
--rw-rw-r--   0 root         (0)     1003     3198 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/gapic/utils/uri_sample.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.283399 gapic-generator-1.9.0/gapic_generator.egg-info/
--rw-r--r--   0 root         (0)     1003     2285 2023-03-17 11:28:01.000000 gapic-generator-1.9.0/gapic_generator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003    43870 2023-03-17 11:28:01.000000 gapic-generator-1.9.0/gapic_generator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-17 11:28:01.000000 gapic-generator-1.9.0/gapic_generator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003      110 2023-03-17 11:28:01.000000 gapic-generator-1.9.0/gapic_generator.egg-info/entry_points.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-17 11:28:01.000000 gapic-generator-1.9.0/gapic_generator.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      239 2023-03-17 11:28:01.000000 gapic-generator-1.9.0/gapic_generator.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        6 2023-03-17 11:28:01.000000 gapic-generator-1.9.0/gapic_generator.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-03-17 11:28:01.375412 gapic-generator-1.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2740 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.259396 gapic-generator-1.9.0/tests/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.283399 gapic-generator-1.9.0/tests/cert/
--rw-rw-r--   0 root         (0)     1003     1249 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/cert/mtls.crt
--rw-rw-r--   0 root         (0)     1003     1704 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/cert/mtls.key
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.287400 gapic-generator-1.9.0/tests/fragments/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.251395 gapic-generator-1.9.0/tests/fragments/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.287400 gapic-generator-1.9.0/tests/fragments/google/api/
--rw-rw-r--   0 root         (0)     1003     1045 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/google/api/annotations.proto
--rw-rw-r--   0 root         (0)     1003     3392 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/google/api/client.proto
--rw-rw-r--   0 root         (0)     1003     3604 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/google/api/field_behavior.proto
--rw-rw-r--   0 root         (0)     1003    15140 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/google/api/http.proto
--rw-rw-r--   0 root         (0)     1003    14928 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/google/api/routing.proto
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.287400 gapic-generator-1.9.0/tests/fragments/google/cloud/
--rw-rw-r--   0 root         (0)     1003     6309 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/google/cloud/extended_operations.proto
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.287400 gapic-generator-1.9.0/tests/fragments/google/longrunning/
--rw-rw-r--   0 root         (0)     1003    10515 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/google/longrunning/operations.proto
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.287400 gapic-generator-1.9.0/tests/fragments/google/protobuf/
--rw-rw-r--   0 root         (0)     1003     5916 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/google/protobuf/any.proto
--rw-rw-r--   0 root         (0)     1003    37969 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/google/protobuf/descriptor.proto
--rw-rw-r--   0 root         (0)     1003     3778 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/google/protobuf/struct.proto
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.287400 gapic-generator-1.9.0/tests/fragments/google/rpc/
--rw-rw-r--   0 root         (0)     1003     1924 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/google/rpc/status.proto
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.287400 gapic-generator-1.9.0/tests/fragments/google/type/
--rw-rw-r--   0 root         (0)     1003     1204 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/google/type/dayofweek.proto
--rw-rw-r--   0 root         (0)     1003      677 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/import.proto
--rw-rw-r--   0 root         (0)     1003     5309 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/test_dynamic_routing.proto
--rw-rw-r--   0 root         (0)     1003     2494 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/test_enum_indexed_types.proto
--rw-rw-r--   0 root         (0)     1003     2057 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/test_enum_indexed_types_nonlocal.proto
--rw-rw-r--   0 root         (0)     1003     3245 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/test_extended_operation_forwardcompat_lro.proto
--rw-rw-r--   0 root         (0)     1003     1073 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/test_flattened_value.proto
--rw-rw-r--   0 root         (0)     1003      929 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/test_keyword_import.proto
--rw-rw-r--   0 root         (0)     1003     1334 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/test_multiple_required_fields.proto
--rw-rw-r--   0 root         (0)     1003     2399 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/test_non_primitive_body.proto
--rw-rw-r--   0 root         (0)     1003      978 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/test_optional_signature.proto
--rw-rw-r--   0 root         (0)     1003      932 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/test_recursive_messages.proto
--rw-rw-r--   0 root         (0)     1003     1206 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/test_repeated_double.proto
--rw-rw-r--   0 root         (0)     1003     1205 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/test_required_non_string.proto
--rw-rw-r--   0 root         (0)     1003     1090 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/test_reserved_field_name.proto
--rw-rw-r--   0 root         (0)     1003     2121 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/test_reserved_method_names.proto
--rw-rw-r--   0 root         (0)     1003     1174 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/fragments/test_rest_streaming.proto
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.291401 gapic-generator-1.9.0/tests/integration/
--rw-rw-r--   0 root         (0)     1003     4195 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/BUILD.bazel
--rwxrwxr-x   0 root         (0)     1003     2246 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/cloudasset_grpc_service_config.json
--rw-rw-r--   0 root         (0)     1003     1567 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/eventarc_grpc_service_config.json
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.259396 gapic-generator-1.9.0/tests/integration/goldens/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.291401 gapic-generator-1.9.0/tests/integration/goldens/asset/
--rwxrwxr-x   0 root         (0)     1003      251 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/.coveragerc
--rwxrwxr-x   0 root         (0)     1003      879 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/.flake8
--rw-rw-r--   0 root         (0)     1003      218 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/BUILD.bazel
--rwxrwxr-x   0 root         (0)     1003       87 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/MANIFEST.in
--rwxrwxr-x   0 root         (0)     1003     1444 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.291401 gapic-generator-1.9.0/tests/integration/goldens/asset/docs/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.291401 gapic-generator-1.9.0/tests/integration/goldens/asset/docs/asset_v1/
--rwxrwxr-x   0 root         (0)     1003      251 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/docs/asset_v1/asset_service.rst
--rwxrwxr-x   0 root         (0)     1003      127 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/docs/asset_v1/services.rst
--rwxrwxr-x   0 root         (0)     1003      154 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/docs/asset_v1/types.rst
--rwxrwxr-x   0 root         (0)     1003    12437 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/docs/conf.py
--rwxrwxr-x   0 root         (0)     1003      100 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/docs/index.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.251395 gapic-generator-1.9.0/tests/integration/goldens/asset/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.251395 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.291401 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset/
--rwxrwxr-x   0 root         (0)     1003     5026 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset/__init__.py
--rwxrwxr-x   0 root         (0)     1003      652 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset/gapic_version.py
--rwxrwxr-x   0 root         (0)     1003       79 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.291401 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/
--rwxrwxr-x   0 root         (0)     1003     3943 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/__init__.py
--rwxrwxr-x   0 root         (0)     1003     5144 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/gapic_metadata.json
--rwxrwxr-x   0 root         (0)     1003      652 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/gapic_version.py
--rwxrwxr-x   0 root         (0)     1003       79 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.291401 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/
--rwxrwxr-x   0 root         (0)     1003      600 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.295401 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/
--rwxrwxr-x   0 root         (0)     1003      761 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/__init__.py
--rwxrwxr-x   0 root         (0)     1003    73168 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/async_client.py
--rwxrwxr-x   0 root         (0)     1003    81928 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/client.py
--rwxrwxr-x   0 root         (0)     1003    15929 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.295401 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/
--rwxrwxr-x   0 root         (0)     1003     1390 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/__init__.py
--rwxrwxr-x   0 root         (0)     1003    13960 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/base.py
--rwxrwxr-x   0 root         (0)     1003    27703 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/grpc.py
--rwxrwxr-x   0 root         (0)     1003    28155 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/grpc_asyncio.py
--rwxrwxr-x   0 root         (0)     1003    66674 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.295401 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/types/
--rwxrwxr-x   0 root         (0)     1003     2796 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/types/__init__.py
--rwxrwxr-x   0 root         (0)     1003    71698 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/types/asset_service.py
--rwxrwxr-x   0 root         (0)     1003    44537 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/types/assets.py
--rwxrwxr-x   0 root         (0)     1003       54 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/mypy.ini
--rwxrwxr-x   0 root         (0)     1003     4811 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/noxfile.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.251395 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.299402 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/
--rwxrwxr-x   0 root         (0)     1003     1969 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_analyze_iam_policy_async.py
--rwxrwxr-x   0 root         (0)     1003     2277 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_analyze_iam_policy_longrunning_async.py
--rwxrwxr-x   0 root         (0)     1003     2256 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_analyze_iam_policy_longrunning_sync.py
--rwxrwxr-x   0 root         (0)     1003     1950 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_analyze_iam_policy_sync.py
--rwxrwxr-x   0 root         (0)     1003     1896 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_batch_get_assets_history_async.py
--rwxrwxr-x   0 root         (0)     1003     1877 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_batch_get_assets_history_sync.py
--rwxrwxr-x   0 root         (0)     1003     1935 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_create_feed_async.py
--rwxrwxr-x   0 root         (0)     1003     1916 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_create_feed_sync.py
--rwxrwxr-x   0 root         (0)     1003     1765 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_delete_feed_async.py
--rwxrwxr-x   0 root         (0)     1003     1746 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_delete_feed_sync.py
--rwxrwxr-x   0 root         (0)     1003     2061 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_export_assets_async.py
--rwxrwxr-x   0 root         (0)     1003     2040 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_export_assets_sync.py
--rwxrwxr-x   0 root         (0)     1003     1804 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_get_feed_async.py
--rwxrwxr-x   0 root         (0)     1003     1785 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_get_feed_sync.py
--rwxrwxr-x   0 root         (0)     1003     1866 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_list_assets_async.py
--rwxrwxr-x   0 root         (0)     1003     1847 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_list_assets_sync.py
--rwxrwxr-x   0 root         (0)     1003     1820 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_list_feeds_async.py
--rwxrwxr-x   0 root         (0)     1003     1801 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_list_feeds_sync.py
--rwxrwxr-x   0 root         (0)     1003     1928 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_search_all_iam_policies_async.py
--rwxrwxr-x   0 root         (0)     1003     1909 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_search_all_iam_policies_sync.py
--rwxrwxr-x   0 root         (0)     1003     1914 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_search_all_resources_async.py
--rwxrwxr-x   0 root         (0)     1003     1895 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_search_all_resources_sync.py
--rwxrwxr-x   0 root         (0)     1003     1871 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_update_feed_async.py
--rwxrwxr-x   0 root         (0)     1003     1852 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_update_feed_sync.py
--rwxrwxr-x   0 root         (0)     1003    53439 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/snippet_metadata_google.cloud.asset.v1.json
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.299402 gapic-generator-1.9.0/tests/integration/goldens/asset/scripts/
--rwxrwxr-x   0 root         (0)     1003     6786 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/scripts/fixup_asset_v1_keywords.py
--rwxrwxr-x   0 root         (0)     1003     2959 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.303402 gapic-generator-1.9.0/tests/integration/goldens/asset/testing/
--rwxrwxr-x   0 root         (0)     1003      188 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/testing/constraints-3.10.txt
--rwxrwxr-x   0 root         (0)     1003      188 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/testing/constraints-3.11.txt
--rwxrwxr-x   0 root         (0)     1003      188 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/testing/constraints-3.12.txt
--rwxrwxr-x   0 root         (0)     1003      387 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/testing/constraints-3.7.txt
--rwxrwxr-x   0 root         (0)     1003      188 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/testing/constraints-3.8.txt
--rwxrwxr-x   0 root         (0)     1003      188 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/testing/constraints-3.9.txt
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.303402 gapic-generator-1.9.0/tests/integration/goldens/asset/tests/
--rwxrwxr-x   0 root         (0)     1003      601 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.303402 gapic-generator-1.9.0/tests/integration/goldens/asset/tests/unit/
--rwxrwxr-x   0 root         (0)     1003      601 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.303402 gapic-generator-1.9.0/tests/integration/goldens/asset/tests/unit/gapic/
--rwxrwxr-x   0 root         (0)     1003      601 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.303402 gapic-generator-1.9.0/tests/integration/goldens/asset/tests/unit/gapic/asset_v1/
--rwxrwxr-x   0 root         (0)     1003      601 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/tests/unit/gapic/asset_v1/__init__.py
--rwxrwxr-x   0 root         (0)     1003   275574 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/asset/tests/unit/gapic/asset_v1/test_asset_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.303402 gapic-generator-1.9.0/tests/integration/goldens/credentials/
--rwxrwxr-x   0 root         (0)     1003      259 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/.coveragerc
--rwxrwxr-x   0 root         (0)     1003      879 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/.flake8
--rw-rw-r--   0 root         (0)     1003      218 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/BUILD.bazel
--rwxrwxr-x   0 root         (0)     1003       95 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/MANIFEST.in
--rwxrwxr-x   0 root         (0)     1003     1452 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.303402 gapic-generator-1.9.0/tests/integration/goldens/credentials/docs/
--rwxrwxr-x   0 root         (0)     1003    12479 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/docs/conf.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.303402 gapic-generator-1.9.0/tests/integration/goldens/credentials/docs/credentials_v1/
--rwxrwxr-x   0 root         (0)     1003      154 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/docs/credentials_v1/iam_credentials.rst
--rwxrwxr-x   0 root         (0)     1003      137 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/docs/credentials_v1/services.rst
--rwxrwxr-x   0 root         (0)     1003      166 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/docs/credentials_v1/types.rst
--rwxrwxr-x   0 root         (0)     1003      112 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/docs/index.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.251395 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.251395 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.307403 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials/
--rwxrwxr-x   0 root         (0)     1003     1774 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials/__init__.py
--rwxrwxr-x   0 root         (0)     1003      652 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials/gapic_version.py
--rwxrwxr-x   0 root         (0)     1003       83 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.307403 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/
--rwxrwxr-x   0 root         (0)     1003     1476 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/__init__.py
--rwxrwxr-x   0 root         (0)     1003     2112 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/gapic_metadata.json
--rwxrwxr-x   0 root         (0)     1003      652 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/gapic_version.py
--rwxrwxr-x   0 root         (0)     1003       83 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.307403 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/
--rwxrwxr-x   0 root         (0)     1003      600 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.307403 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/
--rwxrwxr-x   0 root         (0)     1003      769 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/__init__.py
--rwxrwxr-x   0 root         (0)     1003    35450 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/async_client.py
--rwxrwxr-x   0 root         (0)     1003    43639 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.307403 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/
--rwxrwxr-x   0 root         (0)     1003     1418 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/__init__.py
--rwxrwxr-x   0 root         (0)     1003     8779 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/base.py
--rwxrwxr-x   0 root         (0)     1003    15857 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/grpc.py
--rwxrwxr-x   0 root         (0)     1003    16120 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/grpc_asyncio.py
--rwxrwxr-x   0 root         (0)     1003    27405 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.307403 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/types/
--rwxrwxr-x   0 root         (0)     1003     1067 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/types/__init__.py
--rwxrwxr-x   0 root         (0)     1003     9840 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/types/common.py
--rwxrwxr-x   0 root         (0)     1003      774 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/types/iamcredentials.py
--rwxrwxr-x   0 root         (0)     1003       54 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/mypy.ini
--rwxrwxr-x   0 root         (0)     1003     4815 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/noxfile.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.255396 gapic-generator-1.9.0/tests/integration/goldens/credentials/samples/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.311403 gapic-generator-1.9.0/tests/integration/goldens/credentials/samples/generated_samples/
--rwxrwxr-x   0 root         (0)     1003     1960 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_generate_access_token_async.py
--rwxrwxr-x   0 root         (0)     1003     1941 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_generate_access_token_sync.py
--rwxrwxr-x   0 root         (0)     1003     1923 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_generate_id_token_async.py
--rwxrwxr-x   0 root         (0)     1003     1904 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_generate_id_token_sync.py
--rwxrwxr-x   0 root         (0)     1003     1877 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_sign_blob_async.py
--rwxrwxr-x   0 root         (0)     1003     1858 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_sign_blob_sync.py
--rwxrwxr-x   0 root         (0)     1003     1871 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_sign_jwt_async.py
--rwxrwxr-x   0 root         (0)     1003     1852 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_sign_jwt_sync.py
--rwxrwxr-x   0 root         (0)     1003    20248 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/samples/generated_samples/snippet_metadata_google.iam.credentials.v1.json
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.311403 gapic-generator-1.9.0/tests/integration/goldens/credentials/scripts/
--rwxrwxr-x   0 root         (0)     1003     6188 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/scripts/fixup_credentials_v1_keywords.py
--rwxrwxr-x   0 root         (0)     1003     2932 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.311403 gapic-generator-1.9.0/tests/integration/goldens/credentials/testing/
--rwxrwxr-x   0 root         (0)     1003      169 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/testing/constraints-3.10.txt
--rwxrwxr-x   0 root         (0)     1003      169 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/testing/constraints-3.11.txt
--rwxrwxr-x   0 root         (0)     1003      169 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/testing/constraints-3.12.txt
--rwxrwxr-x   0 root         (0)     1003      360 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/testing/constraints-3.7.txt
--rwxrwxr-x   0 root         (0)     1003      169 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/testing/constraints-3.8.txt
--rwxrwxr-x   0 root         (0)     1003      169 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/testing/constraints-3.9.txt
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.311403 gapic-generator-1.9.0/tests/integration/goldens/credentials/tests/
--rwxrwxr-x   0 root         (0)     1003      601 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.311403 gapic-generator-1.9.0/tests/integration/goldens/credentials/tests/unit/
--rwxrwxr-x   0 root         (0)     1003      601 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.311403 gapic-generator-1.9.0/tests/integration/goldens/credentials/tests/unit/gapic/
--rwxrwxr-x   0 root         (0)     1003      601 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.311403 gapic-generator-1.9.0/tests/integration/goldens/credentials/tests/unit/gapic/credentials_v1/
--rwxrwxr-x   0 root         (0)     1003      601 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/tests/unit/gapic/credentials_v1/__init__.py
--rwxrwxr-x   0 root         (0)     1003   127249 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/credentials/tests/unit/gapic/credentials_v1/test_iam_credentials.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.315404 gapic-generator-1.9.0/tests/integration/goldens/eventarc/
--rwxrwxr-x   0 root         (0)     1003      257 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/.coveragerc
--rwxrwxr-x   0 root         (0)     1003      879 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/.flake8
--rw-rw-r--   0 root         (0)     1003      218 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/BUILD.bazel
--rwxrwxr-x   0 root         (0)     1003       93 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/MANIFEST.in
--rwxrwxr-x   0 root         (0)     1003     1450 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.315404 gapic-generator-1.9.0/tests/integration/goldens/eventarc/docs/
--rwxrwxr-x   0 root         (0)     1003    12470 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/docs/conf.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.315404 gapic-generator-1.9.0/tests/integration/goldens/eventarc/docs/eventarc_v1/
--rwxrwxr-x   0 root         (0)     1003      239 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/docs/eventarc_v1/eventarc.rst
--rwxrwxr-x   0 root         (0)     1003      128 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/docs/eventarc_v1/services.rst
--rwxrwxr-x   0 root         (0)     1003      163 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/docs/eventarc_v1/types.rst
--rwxrwxr-x   0 root         (0)     1003      106 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/docs/index.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.255396 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.255396 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.315404 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc/
--rwxrwxr-x   0 root         (0)     1003     2094 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc/__init__.py
--rwxrwxr-x   0 root         (0)     1003      652 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc/gapic_version.py
--rwxrwxr-x   0 root         (0)     1003       82 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.315404 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/
--rwxrwxr-x   0 root         (0)     1003     1666 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/__init__.py
--rwxrwxr-x   0 root         (0)     1003     2440 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/gapic_metadata.json
--rwxrwxr-x   0 root         (0)     1003      652 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/gapic_version.py
--rwxrwxr-x   0 root         (0)     1003       82 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.315404 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/
--rwxrwxr-x   0 root         (0)     1003      600 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.319404 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/
--rwxrwxr-x   0 root         (0)     1003      745 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/__init__.py
--rwxrwxr-x   0 root         (0)     1003    34859 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/async_client.py
--rwxrwxr-x   0 root         (0)     1003    45027 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/client.py
--rwxrwxr-x   0 root         (0)     1003     5713 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.319404 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/
--rwxrwxr-x   0 root         (0)     1003     1334 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/__init__.py
--rwxrwxr-x   0 root         (0)     1003     8147 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/base.py
--rwxrwxr-x   0 root         (0)     1003    17065 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/grpc.py
--rwxrwxr-x   0 root         (0)     1003    17359 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/grpc_asyncio.py
--rwxrwxr-x   0 root         (0)     1003    32762 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.319404 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/types/
--rwxrwxr-x   0 root         (0)     1003     1218 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/types/__init__.py
--rwxrwxr-x   0 root         (0)     1003     9099 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/types/eventarc.py
--rwxrwxr-x   0 root         (0)     1003     9077 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/types/trigger.py
--rwxrwxr-x   0 root         (0)     1003       54 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/mypy.ini
--rwxrwxr-x   0 root         (0)     1003     4814 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/noxfile.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.255396 gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.319404 gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/
--rwxrwxr-x   0 root         (0)     1003     2312 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_create_trigger_async.py
--rwxrwxr-x   0 root         (0)     1003     2291 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_create_trigger_sync.py
--rwxrwxr-x   0 root         (0)     1003     1953 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_delete_trigger_async.py
--rwxrwxr-x   0 root         (0)     1003     1932 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_delete_trigger_sync.py
--rwxrwxr-x   0 root         (0)     1003     1818 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_get_trigger_async.py
--rwxrwxr-x   0 root         (0)     1003     1799 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_get_trigger_sync.py
--rwxrwxr-x   0 root         (0)     1003     1874 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_list_triggers_async.py
--rwxrwxr-x   0 root         (0)     1003     1855 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_list_triggers_sync.py
--rwxrwxr-x   0 root         (0)     1003     1926 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_update_trigger_async.py
--rwxrwxr-x   0 root         (0)     1003     1905 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_update_trigger_sync.py
--rwxrwxr-x   0 root         (0)     1003    23069 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/snippet_metadata_google.cloud.eventarc.v1.json
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.323405 gapic-generator-1.9.0/tests/integration/goldens/eventarc/scripts/
--rwxrwxr-x   0 root         (0)     1003     6269 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/scripts/fixup_eventarc_v1_keywords.py
--rwxrwxr-x   0 root         (0)     1003     2924 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.323405 gapic-generator-1.9.0/tests/integration/goldens/eventarc/testing/
--rwxrwxr-x   0 root         (0)     1003      169 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/testing/constraints-3.10.txt
--rwxrwxr-x   0 root         (0)     1003      169 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/testing/constraints-3.11.txt
--rwxrwxr-x   0 root         (0)     1003      169 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/testing/constraints-3.12.txt
--rwxrwxr-x   0 root         (0)     1003      360 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/testing/constraints-3.7.txt
--rwxrwxr-x   0 root         (0)     1003      169 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/testing/constraints-3.8.txt
--rwxrwxr-x   0 root         (0)     1003      169 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/testing/constraints-3.9.txt
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.323405 gapic-generator-1.9.0/tests/integration/goldens/eventarc/tests/
--rwxrwxr-x   0 root         (0)     1003      601 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.323405 gapic-generator-1.9.0/tests/integration/goldens/eventarc/tests/unit/
--rwxrwxr-x   0 root         (0)     1003      601 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.323405 gapic-generator-1.9.0/tests/integration/goldens/eventarc/tests/unit/gapic/
--rwxrwxr-x   0 root         (0)     1003      601 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.323405 gapic-generator-1.9.0/tests/integration/goldens/eventarc/tests/unit/gapic/eventarc_v1/
--rwxrwxr-x   0 root         (0)     1003      601 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/tests/unit/gapic/eventarc_v1/__init__.py
--rwxrwxr-x   0 root         (0)     1003   156163 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/eventarc/tests/unit/gapic/eventarc_v1/test_eventarc.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.323405 gapic-generator-1.9.0/tests/integration/goldens/logging/
--rwxrwxr-x   0 root         (0)     1003      255 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/.coveragerc
--rwxrwxr-x   0 root         (0)     1003      879 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/.flake8
--rw-rw-r--   0 root         (0)     1003      218 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/BUILD.bazel
--rwxrwxr-x   0 root         (0)     1003       91 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/MANIFEST.in
--rwxrwxr-x   0 root         (0)     1003     1448 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.323405 gapic-generator-1.9.0/tests/integration/goldens/logging/docs/
--rwxrwxr-x   0 root         (0)     1003    12459 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/docs/conf.py
--rwxrwxr-x   0 root         (0)     1003      104 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/docs/index.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.327406 gapic-generator-1.9.0/tests/integration/goldens/logging/docs/logging_v2/
--rwxrwxr-x   0 root         (0)     1003      269 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/docs/logging_v2/config_service_v2.rst
--rwxrwxr-x   0 root         (0)     1003      273 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/docs/logging_v2/logging_service_v2.rst
--rwxrwxr-x   0 root         (0)     1003      273 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/docs/logging_v2/metrics_service_v2.rst
--rwxrwxr-x   0 root         (0)     1003      181 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/docs/logging_v2/services.rst
--rwxrwxr-x   0 root         (0)     1003      160 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/docs/logging_v2/types.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.255396 gapic-generator-1.9.0/tests/integration/goldens/logging/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.255396 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.327406 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging/
--rwxrwxr-x   0 root         (0)     1003     7206 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging/__init__.py
--rwxrwxr-x   0 root         (0)     1003      652 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging/gapic_version.py
--rwxrwxr-x   0 root         (0)     1003       81 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.327406 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/
--rwxrwxr-x   0 root         (0)     1003     5492 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/__init__.py
--rwxrwxr-x   0 root         (0)     1003    13874 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/gapic_metadata.json
--rwxrwxr-x   0 root         (0)     1003      652 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/gapic_version.py
--rwxrwxr-x   0 root         (0)     1003       81 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.327406 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/
--rwxrwxr-x   0 root         (0)     1003      600 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.327406 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/
--rwxrwxr-x   0 root         (0)     1003      773 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/__init__.py
--rwxrwxr-x   0 root         (0)     1003   109303 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/async_client.py
--rwxrwxr-x   0 root         (0)     1003   120770 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/client.py
--rwxrwxr-x   0 root         (0)     1003    20534 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.331406 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/
--rwxrwxr-x   0 root         (0)     1003     1432 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/__init__.py
--rwxrwxr-x   0 root         (0)     1003    19189 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/base.py
--rwxrwxr-x   0 root         (0)     1003    38551 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/grpc.py
--rwxrwxr-x   0 root         (0)     1003    39233 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/grpc_asyncio.py
--rwxrwxr-x   0 root         (0)     1003   129808 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.331406 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/
--rwxrwxr-x   0 root         (0)     1003      777 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/__init__.py
--rwxrwxr-x   0 root         (0)     1003    43622 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/async_client.py
--rwxrwxr-x   0 root         (0)     1003    50677 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/client.py
--rwxrwxr-x   0 root         (0)     1003    16108 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.331406 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/
--rwxrwxr-x   0 root         (0)     1003     1446 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/__init__.py
--rwxrwxr-x   0 root         (0)     1003    11152 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/base.py
--rwxrwxr-x   0 root         (0)     1003    18757 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/grpc.py
--rwxrwxr-x   0 root         (0)     1003    19066 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/grpc_asyncio.py
--rwxrwxr-x   0 root         (0)     1003    32422 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.331406 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/
--rwxrwxr-x   0 root         (0)     1003      777 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/__init__.py
--rwxrwxr-x   0 root         (0)     1003    34495 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/async_client.py
--rwxrwxr-x   0 root         (0)     1003    42593 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/client.py
--rwxrwxr-x   0 root         (0)     1003     5794 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.335407 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/
--rwxrwxr-x   0 root         (0)     1003     1446 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/__init__.py
--rwxrwxr-x   0 root         (0)     1003     9857 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/base.py
--rwxrwxr-x   0 root         (0)     1003    16452 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/grpc.py
--rwxrwxr-x   0 root         (0)     1003    16739 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/grpc_asyncio.py
--rwxrwxr-x   0 root         (0)     1003    32409 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.335407 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/types/
--rwxrwxr-x   0 root         (0)     1003     3610 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/types/__init__.py
--rwxrwxr-x   0 root         (0)     1003    12763 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/types/log_entry.py
--rwxrwxr-x   0 root         (0)     1003    23104 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/types/logging.py
--rwxrwxr-x   0 root         (0)     1003    50688 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/types/logging_config.py
--rwxrwxr-x   0 root         (0)     1003    13420 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/types/logging_metrics.py
--rwxrwxr-x   0 root         (0)     1003       54 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/mypy.ini
--rwxrwxr-x   0 root         (0)     1003     4813 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/noxfile.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.259396 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.347408 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/
--rwxrwxr-x   0 root         (0)     1003     1886 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_bucket_async.py
--rwxrwxr-x   0 root         (0)     1003     1867 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_bucket_sync.py
--rwxrwxr-x   0 root         (0)     1003     2011 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_exclusion_async.py
--rwxrwxr-x   0 root         (0)     1003     1992 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_exclusion_sync.py
--rwxrwxr-x   0 root         (0)     1003     1961 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_sink_async.py
--rwxrwxr-x   0 root         (0)     1003     1942 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_sink_sync.py
--rwxrwxr-x   0 root         (0)     1003     1870 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_view_async.py
--rwxrwxr-x   0 root         (0)     1003     1851 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_view_sync.py
--rwxrwxr-x   0 root         (0)     1003     1788 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_bucket_async.py
--rwxrwxr-x   0 root         (0)     1003     1769 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_bucket_sync.py
--rwxrwxr-x   0 root         (0)     1003     1806 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_exclusion_async.py
--rwxrwxr-x   0 root         (0)     1003     1787 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_exclusion_sync.py
--rwxrwxr-x   0 root         (0)     1003     1786 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_sink_async.py
--rwxrwxr-x   0 root         (0)     1003     1767 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_sink_sync.py
--rwxrwxr-x   0 root         (0)     1003     1776 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_view_async.py
--rwxrwxr-x   0 root         (0)     1003     1757 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_view_sync.py
--rwxrwxr-x   0 root         (0)     1003     1827 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_bucket_async.py
--rwxrwxr-x   0 root         (0)     1003     1808 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_bucket_sync.py
--rwxrwxr-x   0 root         (0)     1003     1865 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_cmek_settings_async.py
--rwxrwxr-x   0 root         (0)     1003     1846 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_cmek_settings_sync.py
--rwxrwxr-x   0 root         (0)     1003     1845 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_exclusion_async.py
--rwxrwxr-x   0 root         (0)     1003     1826 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_exclusion_sync.py
--rwxrwxr-x   0 root         (0)     1003     1825 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_sink_async.py
--rwxrwxr-x   0 root         (0)     1003     1806 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_sink_sync.py
--rwxrwxr-x   0 root         (0)     1003     1815 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_view_async.py
--rwxrwxr-x   0 root         (0)     1003     1796 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_view_sync.py
--rwxrwxr-x   0 root         (0)     1003     1883 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_buckets_async.py
--rwxrwxr-x   0 root         (0)     1003     1864 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_buckets_sync.py
--rwxrwxr-x   0 root         (0)     1003     1901 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_exclusions_async.py
--rwxrwxr-x   0 root         (0)     1003     1882 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_exclusions_sync.py
--rwxrwxr-x   0 root         (0)     1003     1871 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_sinks_async.py
--rwxrwxr-x   0 root         (0)     1003     1852 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_sinks_sync.py
--rwxrwxr-x   0 root         (0)     1003     1871 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_views_async.py
--rwxrwxr-x   0 root         (0)     1003     1852 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_views_sync.py
--rwxrwxr-x   0 root         (0)     1003     1800 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_undelete_bucket_async.py
--rwxrwxr-x   0 root         (0)     1003     1781 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_undelete_bucket_sync.py
--rwxrwxr-x   0 root         (0)     1003     1845 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_bucket_async.py
--rwxrwxr-x   0 root         (0)     1003     1826 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_bucket_sync.py
--rwxrwxr-x   0 root         (0)     1003     1883 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_cmek_settings_async.py
--rwxrwxr-x   0 root         (0)     1003     1864 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_cmek_settings_sync.py
--rwxrwxr-x   0 root         (0)     1003     2007 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_exclusion_async.py
--rwxrwxr-x   0 root         (0)     1003     1988 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_exclusion_sync.py
--rwxrwxr-x   0 root         (0)     1003     1967 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_sink_async.py
--rwxrwxr-x   0 root         (0)     1003     1948 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_sink_sync.py
--rwxrwxr-x   0 root         (0)     1003     1833 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_view_async.py
--rwxrwxr-x   0 root         (0)     1003     1814 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_view_sync.py
--rwxrwxr-x   0 root         (0)     1003     1781 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_delete_log_async.py
--rwxrwxr-x   0 root         (0)     1003     1762 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_delete_log_sync.py
--rwxrwxr-x   0 root         (0)     1003     1950 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_log_entries_async.py
--rwxrwxr-x   0 root         (0)     1003     1931 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_log_entries_sync.py
--rwxrwxr-x   0 root         (0)     1003     1868 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_logs_async.py
--rwxrwxr-x   0 root         (0)     1003     1849 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_logs_sync.py
--rwxrwxr-x   0 root         (0)     1003     1985 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_monitored_resource_descriptors_async.py
--rwxrwxr-x   0 root         (0)     1003     1966 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_monitored_resource_descriptors_sync.py
--rwxrwxr-x   0 root         (0)     1003     2274 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_tail_log_entries_async.py
--rwxrwxr-x   0 root         (0)     1003     2249 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_tail_log_entries_sync.py
--rwxrwxr-x   0 root         (0)     1003     1943 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_write_log_entries_async.py
--rwxrwxr-x   0 root         (0)     1003     1924 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_write_log_entries_sync.py
--rwxrwxr-x   0 root         (0)     1003     1998 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_create_log_metric_async.py
--rwxrwxr-x   0 root         (0)     1003     1979 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_create_log_metric_sync.py
--rwxrwxr-x   0 root         (0)     1003     1825 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_delete_log_metric_async.py
--rwxrwxr-x   0 root         (0)     1003     1806 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_delete_log_metric_sync.py
--rwxrwxr-x   0 root         (0)     1003     1864 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_get_log_metric_async.py
--rwxrwxr-x   0 root         (0)     1003     1845 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_get_log_metric_sync.py
--rwxrwxr-x   0 root         (0)     1003     1906 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_list_log_metrics_async.py
--rwxrwxr-x   0 root         (0)     1003     1887 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_list_log_metrics_sync.py
--rwxrwxr-x   0 root         (0)     1003     2008 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_update_log_metric_async.py
--rwxrwxr-x   0 root         (0)     1003     1989 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_update_log_metric_sync.py
--rwxrwxr-x   0 root         (0)     1003   151672 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/snippet_metadata_google.logging.v2.json
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.347408 gapic-generator-1.9.0/tests/integration/goldens/logging/scripts/
--rwxrwxr-x   0 root         (0)     1003     7882 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/scripts/fixup_logging_v2_keywords.py
--rwxrwxr-x   0 root         (0)     1003     2920 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.347408 gapic-generator-1.9.0/tests/integration/goldens/logging/testing/
--rwxrwxr-x   0 root         (0)     1003      169 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/testing/constraints-3.10.txt
--rwxrwxr-x   0 root         (0)     1003      169 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/testing/constraints-3.11.txt
--rwxrwxr-x   0 root         (0)     1003      169 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/testing/constraints-3.12.txt
--rwxrwxr-x   0 root         (0)     1003      360 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/testing/constraints-3.7.txt
--rwxrwxr-x   0 root         (0)     1003      169 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/testing/constraints-3.8.txt
--rwxrwxr-x   0 root         (0)     1003      169 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/testing/constraints-3.9.txt
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.347408 gapic-generator-1.9.0/tests/integration/goldens/logging/tests/
--rwxrwxr-x   0 root         (0)     1003      601 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.347408 gapic-generator-1.9.0/tests/integration/goldens/logging/tests/unit/
--rwxrwxr-x   0 root         (0)     1003      601 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.347408 gapic-generator-1.9.0/tests/integration/goldens/logging/tests/unit/gapic/
--rwxrwxr-x   0 root         (0)     1003      601 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.351409 gapic-generator-1.9.0/tests/integration/goldens/logging/tests/unit/gapic/logging_v2/
--rwxrwxr-x   0 root         (0)     1003      601 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/tests/unit/gapic/logging_v2/__init__.py
--rwxrwxr-x   0 root         (0)     1003   462598 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/tests/unit/gapic/logging_v2/test_config_service_v2.py
--rwxrwxr-x   0 root         (0)     1003   158758 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/tests/unit/gapic/logging_v2/test_logging_service_v2.py
--rwxrwxr-x   0 root         (0)     1003   159800 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/logging/tests/unit/gapic/logging_v2/test_metrics_service_v2.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.351409 gapic-generator-1.9.0/tests/integration/goldens/redis/
--rwxrwxr-x   0 root         (0)     1003      251 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/.coveragerc
--rwxrwxr-x   0 root         (0)     1003      879 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/.flake8
--rw-rw-r--   0 root         (0)     1003      218 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/BUILD.bazel
--rwxrwxr-x   0 root         (0)     1003       87 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/MANIFEST.in
--rwxrwxr-x   0 root         (0)     1003     1444 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.351409 gapic-generator-1.9.0/tests/integration/goldens/redis/docs/
--rwxrwxr-x   0 root         (0)     1003    12437 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/docs/conf.py
--rwxrwxr-x   0 root         (0)     1003      100 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/docs/index.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.351409 gapic-generator-1.9.0/tests/integration/goldens/redis/docs/redis_v1/
--rwxrwxr-x   0 root         (0)     1003      243 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/docs/redis_v1/cloud_redis.rst
--rwxrwxr-x   0 root         (0)     1003      125 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/docs/redis_v1/services.rst
--rwxrwxr-x   0 root         (0)     1003      154 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/docs/redis_v1/types.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.259396 gapic-generator-1.9.0/tests/integration/goldens/redis/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.259396 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.355409 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis/
--rwxrwxr-x   0 root         (0)     1003     2656 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis/__init__.py
--rwxrwxr-x   0 root         (0)     1003      652 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis/gapic_version.py
--rwxrwxr-x   0 root         (0)     1003       79 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.355409 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/
--rwxrwxr-x   0 root         (0)     1003     2148 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/__init__.py
--rwxrwxr-x   0 root         (0)     1003     3978 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/gapic_metadata.json
--rwxrwxr-x   0 root         (0)     1003      652 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/gapic_version.py
--rwxrwxr-x   0 root         (0)     1003       79 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.355409 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/
--rwxrwxr-x   0 root         (0)     1003      600 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.355409 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/
--rwxrwxr-x   0 root         (0)     1003      753 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/__init__.py
--rwxrwxr-x   0 root         (0)     1003    59144 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/async_client.py
--rwxrwxr-x   0 root         (0)     1003    69218 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/client.py
--rwxrwxr-x   0 root         (0)     1003     5708 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.355409 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/
--rwxrwxr-x   0 root         (0)     1003     1362 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/__init__.py
--rwxrwxr-x   0 root         (0)     1003    10038 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/base.py
--rwxrwxr-x   0 root         (0)     1003    24385 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/grpc.py
--rwxrwxr-x   0 root         (0)     1003    24769 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/grpc_asyncio.py
--rwxrwxr-x   0 root         (0)     1003    54127 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.355409 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/types/
--rwxrwxr-x   0 root         (0)     1003     1512 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/types/__init__.py
--rwxrwxr-x   0 root         (0)     1003    25588 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/types/cloud_redis.py
--rwxrwxr-x   0 root         (0)     1003       54 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/mypy.ini
--rwxrwxr-x   0 root         (0)     1003     4811 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/noxfile.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.259396 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.359410 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/
--rwxrwxr-x   0 root         (0)     1003     2129 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_create_instance_async.py
--rwxrwxr-x   0 root         (0)     1003     2108 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_create_instance_sync.py
--rwxrwxr-x   0 root         (0)     1003     1919 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_delete_instance_async.py
--rwxrwxr-x   0 root         (0)     1003     1898 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_delete_instance_sync.py
--rwxrwxr-x   0 root         (0)     1003     2053 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_export_instance_async.py
--rwxrwxr-x   0 root         (0)     1003     2032 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_export_instance_sync.py
--rwxrwxr-x   0 root         (0)     1003     1931 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_failover_instance_async.py
--rwxrwxr-x   0 root         (0)     1003     1910 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_failover_instance_sync.py
--rwxrwxr-x   0 root         (0)     1003     1812 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_get_instance_async.py
--rwxrwxr-x   0 root         (0)     1003     1793 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_get_instance_sync.py
--rwxrwxr-x   0 root         (0)     1003     2043 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_import_instance_async.py
--rwxrwxr-x   0 root         (0)     1003     2022 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_import_instance_sync.py
--rwxrwxr-x   0 root         (0)     1003     1868 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_list_instances_async.py
--rwxrwxr-x   0 root         (0)     1003     1849 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_list_instances_sync.py
--rwxrwxr-x   0 root         (0)     1003     2057 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_update_instance_async.py
--rwxrwxr-x   0 root         (0)     1003     2036 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_update_instance_sync.py
--rwxrwxr-x   0 root         (0)     1003     1970 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_upgrade_instance_async.py
--rwxrwxr-x   0 root         (0)     1003     1949 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_upgrade_instance_sync.py
--rwxrwxr-x   0 root         (0)     1003    41251 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/snippet_metadata_google.cloud.redis.v1.json
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.359410 gapic-generator-1.9.0/tests/integration/goldens/redis/scripts/
--rwxrwxr-x   0 root         (0)     1003     6396 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/scripts/fixup_redis_v1_keywords.py
--rwxrwxr-x   0 root         (0)     1003     2912 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.363411 gapic-generator-1.9.0/tests/integration/goldens/redis/testing/
--rwxrwxr-x   0 root         (0)     1003      169 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/testing/constraints-3.10.txt
--rwxrwxr-x   0 root         (0)     1003      169 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/testing/constraints-3.11.txt
--rwxrwxr-x   0 root         (0)     1003      169 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/testing/constraints-3.12.txt
--rwxrwxr-x   0 root         (0)     1003      360 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/testing/constraints-3.7.txt
--rwxrwxr-x   0 root         (0)     1003      169 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/testing/constraints-3.8.txt
--rwxrwxr-x   0 root         (0)     1003      169 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/testing/constraints-3.9.txt
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.363411 gapic-generator-1.9.0/tests/integration/goldens/redis/tests/
--rwxrwxr-x   0 root         (0)     1003      601 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.363411 gapic-generator-1.9.0/tests/integration/goldens/redis/tests/unit/
--rwxrwxr-x   0 root         (0)     1003      601 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.363411 gapic-generator-1.9.0/tests/integration/goldens/redis/tests/unit/gapic/
--rwxrwxr-x   0 root         (0)     1003      601 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.363411 gapic-generator-1.9.0/tests/integration/goldens/redis/tests/unit/gapic/redis_v1/
--rwxrwxr-x   0 root         (0)     1003      601 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/tests/unit/gapic/redis_v1/__init__.py
--rwxrwxr-x   0 root         (0)     1003   232638 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/goldens/redis/tests/unit/gapic/redis_v1/test_cloud_redis.py
--rwxrwxr-x   0 root         (0)     1003      828 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/iamcredentials_grpc_service_config.json
--rwxrwxr-x   0 root         (0)     1003     3935 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/logging_grpc_service_config.json
--rwxrwxr-x   0 root         (0)     1003     1244 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/integration/redis_grpc_service_config.json
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.363411 gapic-generator-1.9.0/tests/snippetgen/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.367411 gapic-generator-1.9.0/tests/snippetgen/goldens/
--rw-rw-r--   0 root         (0)     1003     1935 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_list_resources_async.py
--rw-rw-r--   0 root         (0)     1003     1916 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_list_resources_sync.py
--rw-rw-r--   0 root         (0)     1003     2258 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_bidi_streaming_async.py
--rw-rw-r--   0 root         (0)     1003     2233 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_bidi_streaming_sync.py
--rw-rw-r--   0 root         (0)     1003     2203 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_lro_signatures_async.py
--rw-rw-r--   0 root         (0)     1003     2182 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_lro_signatures_sync.py
--rw-rw-r--   0 root         (0)     1003     2109 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_one_signature_async.py
--rw-rw-r--   0 root         (0)     1003     2090 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_one_signature_sync.py
--rw-rw-r--   0 root         (0)     1003     2160 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_server_streaming_async.py
--rw-rw-r--   0 root         (0)     1003     2135 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_server_streaming_sync.py
--rw-rw-r--   0 root         (0)     1003     1875 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_one_of_method_async.py
--rw-rw-r--   0 root         (0)     1003     1961 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_one_of_method_required_field_async.py
--rw-rw-r--   0 root         (0)     1003     1942 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_one_of_method_required_field_sync.py
--rw-rw-r--   0 root         (0)     1003     1856 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_one_of_method_sync.py
--rw-rw-r--   0 root         (0)     1003    13844 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/snippetgen/goldens/snippet_metadata_mollusca_v1.json
--rw-rw-r--   0 root         (0)     1003     4610 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/snippetgen/snippets.proto
--rw-rw-r--   0 root         (0)     1003     2818 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/snippetgen/test_snippetgen.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.367411 gapic-generator-1.9.0/tests/system/
--rw-rw-r--   0 root         (0)     1003     6811 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/system/conftest.py
--rw-rw-r--   0 root         (0)     1003     1645 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/system/test_client_context_manager.py
--rw-rw-r--   0 root         (0)     1003     3128 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/system/test_error_details.py
--rw-rw-r--   0 root         (0)     1003     1645 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/system/test_grpc_interceptor_streams.py
--rw-rw-r--   0 root         (0)     1003     1770 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/system/test_lro.py
--rw-rw-r--   0 root         (0)     1003     3047 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/system/test_pagination.py
--rw-rw-r--   0 root         (0)     1003     4090 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/system/test_resource_crud.py
--rw-rw-r--   0 root         (0)     1003     1884 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/system/test_retry.py
--rw-rw-r--   0 root         (0)     1003     7593 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/system/test_streams.py
--rw-rw-r--   0 root         (0)     1003     3317 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/system/test_unary.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.367411 gapic-generator-1.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/__init__.py
--rw-rw-r--   0 root         (0)     1003     5256 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/common_types.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.367411 gapic-generator-1.9.0/tests/unit/configurable_snippetgen/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.367411 gapic-generator-1.9.0/tests/unit/configurable_snippetgen/resources/
--rw-rw-r--   0 root         (0)     1003     1161 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/configurable_snippetgen/resources/README.md
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.367411 gapic-generator-1.9.0/tests/unit/configurable_snippetgen/resources/speech/
--rw-rw-r--   0 root         (0)     1003   213102 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/configurable_snippetgen/resources/speech/request.desc
--rw-rw-r--   0 root         (0)     1003     4695 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/configurable_snippetgen/resources/speech/speech_createCustomClass.json
--rw-rw-r--   0 root         (0)     1003     2311 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/configurable_snippetgen/resources/speech/speech_v1_generated_adaptation_create_custom_class_basic_async.py
--rw-rw-r--   0 root         (0)     1003     8717 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/configurable_snippetgen/test_configured_snippet.py
--rw-rw-r--   0 root         (0)     1003     3433 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/configurable_snippetgen/test_libcst_utils.py
--rw-rw-r--   0 root         (0)     1003     1536 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/configurable_snippetgen/test_resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.371412 gapic-generator-1.9.0/tests/unit/generator/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/generator/__init__.py
--rw-rw-r--   0 root         (0)     1003     2725 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/generator/test_formatter.py
--rw-rw-r--   0 root         (0)     1003    28198 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/generator/test_generator.py
--rw-rw-r--   0 root         (0)     1003     7938 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/generator/test_options.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.371412 gapic-generator-1.9.0/tests/unit/samplegen/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/samplegen/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.371412 gapic-generator-1.9.0/tests/unit/samplegen/golden_snippets/
--rw-rw-r--   0 root         (0)     1003     2080 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/samplegen/golden_snippets/sample_basic.py
--rw-rw-r--   0 root         (0)     1003     2097 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/samplegen/golden_snippets/sample_basic_async.py
--rw-rw-r--   0 root         (0)     1003     2080 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/samplegen/golden_snippets/sample_basic_unflattenable.py
--rw-rw-r--   0 root         (0)     1003     1992 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/samplegen/golden_snippets/sample_basic_void_method.py
--rw-rw-r--   0 root         (0)     1003    23715 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/samplegen/test_integration.py
--rw-rw-r--   0 root         (0)     1003     5328 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/samplegen/test_manifest.py
--rw-rw-r--   0 root         (0)     1003    80651 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/samplegen/test_samplegen.py
--rw-rw-r--   0 root         (0)     1003    10145 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/samplegen/test_snippet_index.py
--rw-rw-r--   0 root         (0)     1003    42147 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/samplegen/test_template.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.371412 gapic-generator-1.9.0/tests/unit/schema/
--rw-rw-r--   0 root         (0)     1003   104006 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/schema/test_api.py
--rw-rw-r--   0 root         (0)     1003     1790 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/schema/test_imp.py
--rw-rw-r--   0 root         (0)     1003     7161 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/schema/test_metadata.py
--rw-rw-r--   0 root         (0)     1003     7589 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/schema/test_naming.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.375412 gapic-generator-1.9.0/tests/unit/schema/wrappers/
--rw-rw-r--   0 root         (0)     1003     1847 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/schema/wrappers/test_enums.py
--rw-rw-r--   0 root         (0)     1003    16779 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/schema/wrappers/test_field.py
--rw-rw-r--   0 root         (0)     1003    16096 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/schema/wrappers/test_message.py
--rw-rw-r--   0 root         (0)     1003    31723 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/schema/wrappers/test_method.py
--rw-rw-r--   0 root         (0)     1003     1026 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/schema/wrappers/test_oneof.py
--rw-rw-r--   0 root         (0)     1003     1568 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/schema/wrappers/test_python.py
--rw-rw-r--   0 root         (0)     1003     5545 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/schema/wrappers/test_routing.py
--rw-rw-r--   0 root         (0)     1003    21284 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/schema/wrappers/test_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-17 11:28:01.375412 gapic-generator-1.9.0/tests/unit/utils/
--rw-rw-r--   0 root         (0)     1003      981 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/utils/test_cache.py
--rw-rw-r--   0 root         (0)     1003     1322 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/utils/test_case.py
--rw-rw-r--   0 root         (0)     1003     1406 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/utils/test_checks.py
--rw-rw-r--   0 root         (0)     1003     1212 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/utils/test_code.py
--rw-rw-r--   0 root         (0)     1003     1218 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/utils/test_filename.py
--rw-rw-r--   0 root         (0)     1003     2529 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/utils/test_lines.py
--rw-rw-r--   0 root         (0)     1003     2232 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/utils/test_rst.py
--rw-rw-r--   0 root         (0)     1003     1130 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/utils/test_uri_conv.py
--rw-rw-r--   0 root         (0)     1003     1205 2023-03-17 11:25:17.000000 gapic-generator-1.9.0/tests/unit/utils/test_uri_sample.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.253655 gapic-generator-1.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      182 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     2285 2023-03-22 16:41:14.253655 gapic-generator-1.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     1237 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.137652 gapic-generator-1.9.1/gapic/
+-rw-rw-r--   0 root         (0)     1003      575 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.137652 gapic-generator-1.9.1/gapic/cli/
+-rw-rw-r--   0 root         (0)     1003      575 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/cli/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1632 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/cli/dump.py
+-rw-rw-r--   0 root         (0)     1003     2548 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/cli/generate.py
+-rw-rw-r--   0 root         (0)     1003      446 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/cli/generate_with_pandoc.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.137652 gapic-generator-1.9.1/gapic/configurable_snippetgen/
+-rw-rw-r--   0 root         (0)     1003      574 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/configurable_snippetgen/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9620 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/configurable_snippetgen/configured_snippet.py
+-rw-rw-r--   0 root         (0)     1003     2669 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/configurable_snippetgen/libcst_utils.py
+-rw-rw-r--   0 root         (0)     1003    43112 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/configurable_snippetgen/snippet_config_language.proto
+-rw-rw-r--   0 root         (0)     1003    27715 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/configurable_snippetgen/snippet_config_language_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.141652 gapic-generator-1.9.1/gapic/generator/
+-rw-rw-r--   0 root         (0)     1003      843 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/generator/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1451 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/generator/formatter.py
+-rw-rw-r--   0 root         (0)     1003    17499 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/generator/generator.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.141652 gapic-generator-1.9.1/gapic/samplegen/
+-rw-rw-r--   0 root         (0)     1003      703 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/samplegen/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4513 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/samplegen/manifest.py
+-rw-rw-r--   0 root         (0)     1003    48624 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/samplegen/samplegen.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.141652 gapic-generator-1.9.1/gapic/samplegen_utils/
+-rw-rw-r--   0 root         (0)     1003      737 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/samplegen_utils/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8189 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/samplegen_utils/snippet_index.py
+-rw-rw-r--   0 root         (0)     1003    10573 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/samplegen_utils/snippet_metadata.proto
+-rw-rw-r--   0 root         (0)     1003    10134 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/samplegen_utils/snippet_metadata_pb2.py
+-rw-rw-r--   0 root         (0)     1003     2420 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/samplegen_utils/types.py
+-rw-rw-r--   0 root         (0)     1003     4761 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/samplegen_utils/utils.py
+-rw-rw-r--   0 root         (0)     1003     3728 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/samplegen_utils/yaml.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.141652 gapic-generator-1.9.1/gapic/schema/
+-rw-rw-r--   0 root         (0)     1003      993 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/schema/__init__.py
+-rw-rw-r--   0 root         (0)     1003    52287 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/schema/api.py
+-rw-rw-r--   0 root         (0)     1003     1223 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/schema/imp.py
+-rw-rw-r--   0 root         (0)     1003    16503 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/schema/metadata.py
+-rw-rw-r--   0 root         (0)     1003     2465 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/schema/mixins.py
+-rw-rw-r--   0 root         (0)     1003     8771 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/schema/naming.py
+-rw-rw-r--   0 root         (0)     1003    69198 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/schema/wrappers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.145652 gapic-generator-1.9.1/gapic/templates/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.121652 gapic-generator-1.9.1/gapic/templates/%namespace/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.145652 gapic-generator-1.9.1/gapic/templates/%namespace/%name/
+-rw-rw-r--   0 root         (0)     1003     3226 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name/__init__.py.j2
+-rw-rw-r--   0 root         (0)     1003      115 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name/gapic_version.py.j2
+-rw-rw-r--   0 root         (0)     1003      100 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name/py.typed.j2
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.145652 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.145652 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/
+-rw-rw-r--   0 root         (0)     1003     2285 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/__init__.py.j2
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.145652 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.149652 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/
+-rw-rw-r--   0 root         (0)     1003      356 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/__init__.py.j2
+-rw-rw-r--   0 root         (0)     1003    27851 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/_async_mixins.py.j2
+-rw-rw-r--   0 root         (0)     1003    12203 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/_client_macros.j2
+-rw-rw-r--   0 root         (0)     1003    27648 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/_mixins.py.j2
+-rw-rw-r--   0 root         (0)     1003    30858 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/async_client.py.j2
+-rw-rw-r--   0 root         (0)     1003    30675 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/client.py.j2
+-rw-rw-r--   0 root         (0)     1003     6958 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/pagers.py.j2
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.149652 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/
+-rw-rw-r--   0 root         (0)     1003     1232 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/__init__.py.j2
+-rw-rw-r--   0 root         (0)     1003    10632 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/_mixins.py.j2
+-rw-rw-r--   0 root         (0)     1003     3686 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/_rest_mixins.py.j2
+-rw-rw-r--   0 root         (0)     1003    13074 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/base.py.j2
+-rw-rw-r--   0 root         (0)     1003    17307 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/grpc.py.j2
+-rw-rw-r--   0 root         (0)     1003    17598 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/grpc_asyncio.py.j2
+-rw-rw-r--   0 root         (0)     1003    19429 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/rest.py.j2
+-rw-rw-r--   0 root         (0)     1003       28 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/__init__.py.j2
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.149652 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/types/
+-rw-rw-r--   0 root         (0)     1003     1227 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/types/%proto.py.j2
+-rw-rw-r--   0 root         (0)     1003      646 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/types/__init__.py.j2
+-rw-rw-r--   0 root         (0)     1003      639 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/types/_enum.py.j2
+-rw-rw-r--   0 root         (0)     1003     4291 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/types/_message.py.j2
+-rw-rw-r--   0 root         (0)     1003       37 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/gapic_metadata.json.j2
+-rw-rw-r--   0 root         (0)     1003      115 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/gapic_version.py.j2
+-rw-rw-r--   0 root         (0)     1003      100 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/py.typed.j2
+-rw-rw-r--   0 root         (0)     1003      359 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/.coveragerc.j2
+-rw-rw-r--   0 root         (0)     1003      879 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/.flake8.j2
+-rw-rw-r--   0 root         (0)     1003      200 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/MANIFEST.in.j2
+-rw-rw-r--   0 root         (0)     1003     1461 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/README.rst.j2
+-rw-rw-r--   0 root         (0)     1003      122 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/_base.py.j2
+-rw-rw-r--   0 root         (0)     1003      576 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/_license.j2
+-rw-rw-r--   0 root         (0)     1003     1042 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/_pypi_packages.j2
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.149652 gapic-generator-1.9.1/gapic/templates/docs/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.149652 gapic-generator-1.9.1/gapic/templates/docs/%name_%version/
+-rw-rw-r--   0 root         (0)     1003      528 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/docs/%name_%version/%service.rst.j2
+-rw-rw-r--   0 root         (0)     1003      296 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/docs/%name_%version/services.rst.j2
+-rw-rw-r--   0 root         (0)     1003      283 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/docs/%name_%version/types.rst.j2
+-rw-rw-r--   0 root         (0)     1003    12131 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/docs/conf.py.j2
+-rw-rw-r--   0 root         (0)     1003      164 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/docs/index.rst.j2
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.153653 gapic-generator-1.9.1/gapic/templates/examples/
+-rw-rw-r--   0 root         (0)     1003      386 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/examples/_generated_sample_comment.j2
+-rw-rw-r--   0 root         (0)     1003    12491 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/examples/feature_fragments.j2
+-rw-rw-r--   0 root         (0)     1003     1926 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/examples/sample.py.j2
+-rw-rw-r--   0 root         (0)     1003       54 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/mypy.ini.j2
+-rw-rw-r--   0 root         (0)     1003     4502 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/noxfile.py.j2
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.153653 gapic-generator-1.9.1/gapic/templates/scripts/
+-rw-rw-r--   0 root         (0)     1003     6479 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/scripts/fixup_%name_%version_keywords.py.j2
+-rw-rw-r--   0 root         (0)     1003     3300 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/setup.py.j2
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.153653 gapic-generator-1.9.1/gapic/templates/testing/
+-rw-rw-r--   0 root         (0)     1003      521 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/testing/_default_constraints.j2
+-rw-rw-r--   0 root         (0)     1003      110 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/testing/constraints-3.10.txt.j2
+-rw-rw-r--   0 root         (0)     1003      110 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/testing/constraints-3.11.txt.j2
+-rw-rw-r--   0 root         (0)     1003      111 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/testing/constraints-3.12.txt.j2
+-rw-rw-r--   0 root         (0)     1003      768 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/testing/constraints-3.7.txt.j2
+-rw-rw-r--   0 root         (0)     1003      110 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/testing/constraints-3.8.txt.j2
+-rw-rw-r--   0 root         (0)     1003      110 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/testing/constraints-3.9.txt.j2
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.153653 gapic-generator-1.9.1/gapic/templates/tests/
+-rw-rw-r--   0 root         (0)     1003       29 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/tests/__init__.py.j2
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.153653 gapic-generator-1.9.1/gapic/templates/tests/unit/
+-rw-rw-r--   0 root         (0)     1003       29 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/tests/unit/__init__.py.j2
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.153653 gapic-generator-1.9.1/gapic/templates/tests/unit/gapic/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.121652 gapic-generator-1.9.1/gapic/templates/tests/unit/gapic/%name_%version/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.153653 gapic-generator-1.9.1/gapic/templates/tests/unit/gapic/%name_%version/%sub/
+-rw-rw-r--   0 root         (0)     1003       29 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/tests/unit/gapic/%name_%version/%sub/__init__.py.j2
+-rw-rw-r--   0 root         (0)     1003    67200 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/tests/unit/gapic/%name_%version/%sub/_test_mixins.py.j2
+-rw-rw-r--   0 root         (0)     1003    62369 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/tests/unit/gapic/%name_%version/%sub/test_%service.py.j2
+-rw-rw-r--   0 root         (0)     1003    64283 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/tests/unit/gapic/%name_%version/%sub/test_macros.j2
+-rw-rw-r--   0 root         (0)     1003       29 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/templates/tests/unit/gapic/__init__.py.j2
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.157652 gapic-generator-1.9.1/gapic/utils/
+-rw-rw-r--   0 root         (0)     1003     1644 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/utils/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1424 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/utils/cache.py
+-rw-rw-r--   0 root         (0)     1003     2172 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/utils/case.py
+-rw-rw-r--   0 root         (0)     1003     1155 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/utils/checks.py
+-rw-rw-r--   0 root         (0)     1003     2369 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/utils/code.py
+-rw-rw-r--   0 root         (0)     1003     1035 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/utils/doc.py
+-rw-rw-r--   0 root         (0)     1003     1377 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/utils/filename.py
+-rw-rw-r--   0 root         (0)     1003     4546 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/utils/lines.py
+-rw-rw-r--   0 root         (0)     1003     8459 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/utils/options.py
+-rw-rw-r--   0 root         (0)     1003     1215 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/utils/reserved_names.py
+-rw-rw-r--   0 root         (0)     1003     2655 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/utils/rst.py
+-rw-rw-r--   0 root         (0)     1003     1696 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/utils/uri_conv.py
+-rw-rw-r--   0 root         (0)     1003     3198 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/gapic/utils/uri_sample.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.157652 gapic-generator-1.9.1/gapic_generator.egg-info/
+-rw-r--r--   0 root         (0)     1003     2285 2023-03-22 16:41:14.000000 gapic-generator-1.9.1/gapic_generator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003    43905 2023-03-22 16:41:14.000000 gapic-generator-1.9.1/gapic_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-03-22 16:41:14.000000 gapic-generator-1.9.1/gapic_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003      110 2023-03-22 16:41:14.000000 gapic-generator-1.9.1/gapic_generator.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-03-22 16:41:14.000000 gapic-generator-1.9.1/gapic_generator.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      239 2023-03-22 16:41:14.000000 gapic-generator-1.9.1/gapic_generator.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        6 2023-03-22 16:41:14.000000 gapic-generator-1.9.1/gapic_generator.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-03-22 16:41:14.253655 gapic-generator-1.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2740 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.133652 gapic-generator-1.9.1/tests/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.157652 gapic-generator-1.9.1/tests/cert/
+-rw-rw-r--   0 root         (0)     1003     1249 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/cert/mtls.crt
+-rw-rw-r--   0 root         (0)     1003     1704 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/cert/mtls.key
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.161653 gapic-generator-1.9.1/tests/fragments/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.125652 gapic-generator-1.9.1/tests/fragments/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.161653 gapic-generator-1.9.1/tests/fragments/google/api/
+-rw-rw-r--   0 root         (0)     1003     1045 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/google/api/annotations.proto
+-rw-rw-r--   0 root         (0)     1003     3392 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/google/api/client.proto
+-rw-rw-r--   0 root         (0)     1003     3604 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/google/api/field_behavior.proto
+-rw-rw-r--   0 root         (0)     1003    15140 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/google/api/http.proto
+-rw-rw-r--   0 root         (0)     1003    14928 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/google/api/routing.proto
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.161653 gapic-generator-1.9.1/tests/fragments/google/cloud/
+-rw-rw-r--   0 root         (0)     1003     6309 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/google/cloud/extended_operations.proto
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.161653 gapic-generator-1.9.1/tests/fragments/google/longrunning/
+-rw-rw-r--   0 root         (0)     1003    10515 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/google/longrunning/operations.proto
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.161653 gapic-generator-1.9.1/tests/fragments/google/protobuf/
+-rw-rw-r--   0 root         (0)     1003     5916 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/google/protobuf/any.proto
+-rw-rw-r--   0 root         (0)     1003    37969 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/google/protobuf/descriptor.proto
+-rw-rw-r--   0 root         (0)     1003     3778 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/google/protobuf/struct.proto
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.161653 gapic-generator-1.9.1/tests/fragments/google/rpc/
+-rw-rw-r--   0 root         (0)     1003     1924 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/google/rpc/status.proto
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.161653 gapic-generator-1.9.1/tests/fragments/google/type/
+-rw-rw-r--   0 root         (0)     1003     1204 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/google/type/dayofweek.proto
+-rw-rw-r--   0 root         (0)     1003      677 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/import.proto
+-rw-rw-r--   0 root         (0)     1003     5309 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/test_dynamic_routing.proto
+-rw-rw-r--   0 root         (0)     1003     2494 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/test_enum_indexed_types.proto
+-rw-rw-r--   0 root         (0)     1003     2057 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/test_enum_indexed_types_nonlocal.proto
+-rw-rw-r--   0 root         (0)     1003     3245 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/test_extended_operation_forwardcompat_lro.proto
+-rw-rw-r--   0 root         (0)     1003     1073 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/test_flattened_value.proto
+-rw-rw-r--   0 root         (0)     1003      929 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/test_keyword_import.proto
+-rw-rw-r--   0 root         (0)     1003     1334 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/test_multiple_required_fields.proto
+-rw-rw-r--   0 root         (0)     1003     2399 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/test_non_primitive_body.proto
+-rw-rw-r--   0 root         (0)     1003      978 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/test_optional_signature.proto
+-rw-rw-r--   0 root         (0)     1003      932 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/test_recursive_messages.proto
+-rw-rw-r--   0 root         (0)     1003     1206 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/test_repeated_double.proto
+-rw-rw-r--   0 root         (0)     1003     1205 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/test_required_non_string.proto
+-rw-rw-r--   0 root         (0)     1003     1090 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/test_reserved_field_name.proto
+-rw-rw-r--   0 root         (0)     1003     2121 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/test_reserved_method_names.proto
+-rw-rw-r--   0 root         (0)     1003     1174 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/fragments/test_rest_streaming.proto
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.165653 gapic-generator-1.9.1/tests/integration/
+-rw-rw-r--   0 root         (0)     1003     4482 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/BUILD.bazel
+-rwxrwxr-x   0 root         (0)     1003     2246 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/cloudasset_grpc_service_config.json
+-rw-rw-r--   0 root         (0)     1003     1567 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/eventarc_grpc_service_config.json
+-rw-rw-r--   0 root         (0)     1003      214 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/eventarc_v1.yaml
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.133652 gapic-generator-1.9.1/tests/integration/goldens/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.165653 gapic-generator-1.9.1/tests/integration/goldens/asset/
+-rwxrwxr-x   0 root         (0)     1003      251 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/.coveragerc
+-rwxrwxr-x   0 root         (0)     1003      879 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/.flake8
+-rw-rw-r--   0 root         (0)     1003      218 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/BUILD.bazel
+-rwxrwxr-x   0 root         (0)     1003       87 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/MANIFEST.in
+-rwxrwxr-x   0 root         (0)     1003     1444 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.165653 gapic-generator-1.9.1/tests/integration/goldens/asset/docs/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.165653 gapic-generator-1.9.1/tests/integration/goldens/asset/docs/asset_v1/
+-rwxrwxr-x   0 root         (0)     1003      251 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/docs/asset_v1/asset_service.rst
+-rwxrwxr-x   0 root         (0)     1003      127 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/docs/asset_v1/services.rst
+-rwxrwxr-x   0 root         (0)     1003      154 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/docs/asset_v1/types.rst
+-rwxrwxr-x   0 root         (0)     1003    12437 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/docs/conf.py
+-rwxrwxr-x   0 root         (0)     1003      100 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/docs/index.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.125652 gapic-generator-1.9.1/tests/integration/goldens/asset/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.125652 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.165653 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset/
+-rwxrwxr-x   0 root         (0)     1003     5026 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset/__init__.py
+-rwxrwxr-x   0 root         (0)     1003      652 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset/gapic_version.py
+-rwxrwxr-x   0 root         (0)     1003       79 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.169653 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/
+-rwxrwxr-x   0 root         (0)     1003     3943 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/__init__.py
+-rwxrwxr-x   0 root         (0)     1003     5144 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/gapic_metadata.json
+-rwxrwxr-x   0 root         (0)     1003      652 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/gapic_version.py
+-rwxrwxr-x   0 root         (0)     1003       79 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.169653 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/
+-rwxrwxr-x   0 root         (0)     1003      600 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.169653 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/
+-rwxrwxr-x   0 root         (0)     1003      761 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/__init__.py
+-rwxrwxr-x   0 root         (0)     1003    73168 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/async_client.py
+-rwxrwxr-x   0 root         (0)     1003    81928 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/client.py
+-rwxrwxr-x   0 root         (0)     1003    15929 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.169653 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/
+-rwxrwxr-x   0 root         (0)     1003     1390 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/__init__.py
+-rwxrwxr-x   0 root         (0)     1003    13960 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/base.py
+-rwxrwxr-x   0 root         (0)     1003    27703 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/grpc.py
+-rwxrwxr-x   0 root         (0)     1003    28155 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/grpc_asyncio.py
+-rwxrwxr-x   0 root         (0)     1003    66672 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.169653 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/types/
+-rwxrwxr-x   0 root         (0)     1003     2796 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/types/__init__.py
+-rwxrwxr-x   0 root         (0)     1003    71698 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/types/asset_service.py
+-rwxrwxr-x   0 root         (0)     1003    44537 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/types/assets.py
+-rwxrwxr-x   0 root         (0)     1003       54 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/mypy.ini
+-rwxrwxr-x   0 root         (0)     1003     4811 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/noxfile.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.125652 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.177653 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/
+-rwxrwxr-x   0 root         (0)     1003     1969 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_analyze_iam_policy_async.py
+-rwxrwxr-x   0 root         (0)     1003     2277 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_analyze_iam_policy_longrunning_async.py
+-rwxrwxr-x   0 root         (0)     1003     2256 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_analyze_iam_policy_longrunning_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1950 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_analyze_iam_policy_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1896 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_batch_get_assets_history_async.py
+-rwxrwxr-x   0 root         (0)     1003     1877 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_batch_get_assets_history_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1935 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_create_feed_async.py
+-rwxrwxr-x   0 root         (0)     1003     1916 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_create_feed_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1765 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_delete_feed_async.py
+-rwxrwxr-x   0 root         (0)     1003     1746 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_delete_feed_sync.py
+-rwxrwxr-x   0 root         (0)     1003     2061 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_export_assets_async.py
+-rwxrwxr-x   0 root         (0)     1003     2040 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_export_assets_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1804 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_get_feed_async.py
+-rwxrwxr-x   0 root         (0)     1003     1785 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_get_feed_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1866 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_list_assets_async.py
+-rwxrwxr-x   0 root         (0)     1003     1847 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_list_assets_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1820 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_list_feeds_async.py
+-rwxrwxr-x   0 root         (0)     1003     1801 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_list_feeds_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1928 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_search_all_iam_policies_async.py
+-rwxrwxr-x   0 root         (0)     1003     1909 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_search_all_iam_policies_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1914 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_search_all_resources_async.py
+-rwxrwxr-x   0 root         (0)     1003     1895 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_search_all_resources_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1871 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_update_feed_async.py
+-rwxrwxr-x   0 root         (0)     1003     1852 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_update_feed_sync.py
+-rwxrwxr-x   0 root         (0)     1003    53439 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/snippet_metadata_google.cloud.asset.v1.json
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.177653 gapic-generator-1.9.1/tests/integration/goldens/asset/scripts/
+-rwxrwxr-x   0 root         (0)     1003     6786 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/scripts/fixup_asset_v1_keywords.py
+-rwxrwxr-x   0 root         (0)     1003     2959 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.177653 gapic-generator-1.9.1/tests/integration/goldens/asset/testing/
+-rwxrwxr-x   0 root         (0)     1003      188 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/testing/constraints-3.10.txt
+-rwxrwxr-x   0 root         (0)     1003      188 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/testing/constraints-3.11.txt
+-rwxrwxr-x   0 root         (0)     1003      188 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/testing/constraints-3.12.txt
+-rwxrwxr-x   0 root         (0)     1003      387 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/testing/constraints-3.7.txt
+-rwxrwxr-x   0 root         (0)     1003      188 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/testing/constraints-3.8.txt
+-rwxrwxr-x   0 root         (0)     1003      188 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/testing/constraints-3.9.txt
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.177653 gapic-generator-1.9.1/tests/integration/goldens/asset/tests/
+-rwxrwxr-x   0 root         (0)     1003      601 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.177653 gapic-generator-1.9.1/tests/integration/goldens/asset/tests/unit/
+-rwxrwxr-x   0 root         (0)     1003      601 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.177653 gapic-generator-1.9.1/tests/integration/goldens/asset/tests/unit/gapic/
+-rwxrwxr-x   0 root         (0)     1003      601 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.177653 gapic-generator-1.9.1/tests/integration/goldens/asset/tests/unit/gapic/asset_v1/
+-rwxrwxr-x   0 root         (0)     1003      601 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/tests/unit/gapic/asset_v1/__init__.py
+-rwxrwxr-x   0 root         (0)     1003   275574 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/asset/tests/unit/gapic/asset_v1/test_asset_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.181653 gapic-generator-1.9.1/tests/integration/goldens/credentials/
+-rwxrwxr-x   0 root         (0)     1003      259 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/.coveragerc
+-rwxrwxr-x   0 root         (0)     1003      879 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/.flake8
+-rw-rw-r--   0 root         (0)     1003      218 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/BUILD.bazel
+-rwxrwxr-x   0 root         (0)     1003       95 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/MANIFEST.in
+-rwxrwxr-x   0 root         (0)     1003     1452 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.181653 gapic-generator-1.9.1/tests/integration/goldens/credentials/docs/
+-rwxrwxr-x   0 root         (0)     1003    12479 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/docs/conf.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.181653 gapic-generator-1.9.1/tests/integration/goldens/credentials/docs/credentials_v1/
+-rwxrwxr-x   0 root         (0)     1003      154 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/docs/credentials_v1/iam_credentials.rst
+-rwxrwxr-x   0 root         (0)     1003      137 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/docs/credentials_v1/services.rst
+-rwxrwxr-x   0 root         (0)     1003      166 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/docs/credentials_v1/types.rst
+-rwxrwxr-x   0 root         (0)     1003      112 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/docs/index.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.125652 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.125652 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.181653 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials/
+-rwxrwxr-x   0 root         (0)     1003     1774 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials/__init__.py
+-rwxrwxr-x   0 root         (0)     1003      652 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials/gapic_version.py
+-rwxrwxr-x   0 root         (0)     1003       83 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.181653 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/
+-rwxrwxr-x   0 root         (0)     1003     1476 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/__init__.py
+-rwxrwxr-x   0 root         (0)     1003     2112 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/gapic_metadata.json
+-rwxrwxr-x   0 root         (0)     1003      652 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/gapic_version.py
+-rwxrwxr-x   0 root         (0)     1003       83 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.181653 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/
+-rwxrwxr-x   0 root         (0)     1003      600 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.181653 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/
+-rwxrwxr-x   0 root         (0)     1003      769 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/__init__.py
+-rwxrwxr-x   0 root         (0)     1003    35450 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/async_client.py
+-rwxrwxr-x   0 root         (0)     1003    43639 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.185653 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/
+-rwxrwxr-x   0 root         (0)     1003     1418 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/__init__.py
+-rwxrwxr-x   0 root         (0)     1003     8779 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/base.py
+-rwxrwxr-x   0 root         (0)     1003    15857 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/grpc.py
+-rwxrwxr-x   0 root         (0)     1003    16120 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/grpc_asyncio.py
+-rwxrwxr-x   0 root         (0)     1003    27405 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.185653 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/types/
+-rwxrwxr-x   0 root         (0)     1003     1067 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/types/__init__.py
+-rwxrwxr-x   0 root         (0)     1003     9840 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/types/common.py
+-rwxrwxr-x   0 root         (0)     1003      774 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/types/iamcredentials.py
+-rwxrwxr-x   0 root         (0)     1003       54 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/mypy.ini
+-rwxrwxr-x   0 root         (0)     1003     4815 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/noxfile.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.129652 gapic-generator-1.9.1/tests/integration/goldens/credentials/samples/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.185653 gapic-generator-1.9.1/tests/integration/goldens/credentials/samples/generated_samples/
+-rwxrwxr-x   0 root         (0)     1003     1960 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_generate_access_token_async.py
+-rwxrwxr-x   0 root         (0)     1003     1941 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_generate_access_token_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1923 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_generate_id_token_async.py
+-rwxrwxr-x   0 root         (0)     1003     1904 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_generate_id_token_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1877 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_sign_blob_async.py
+-rwxrwxr-x   0 root         (0)     1003     1858 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_sign_blob_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1871 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_sign_jwt_async.py
+-rwxrwxr-x   0 root         (0)     1003     1852 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_sign_jwt_sync.py
+-rwxrwxr-x   0 root         (0)     1003    20248 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/samples/generated_samples/snippet_metadata_google.iam.credentials.v1.json
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.185653 gapic-generator-1.9.1/tests/integration/goldens/credentials/scripts/
+-rwxrwxr-x   0 root         (0)     1003     6188 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/scripts/fixup_credentials_v1_keywords.py
+-rwxrwxr-x   0 root         (0)     1003     2932 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.185653 gapic-generator-1.9.1/tests/integration/goldens/credentials/testing/
+-rwxrwxr-x   0 root         (0)     1003      169 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/testing/constraints-3.10.txt
+-rwxrwxr-x   0 root         (0)     1003      169 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/testing/constraints-3.11.txt
+-rwxrwxr-x   0 root         (0)     1003      169 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/testing/constraints-3.12.txt
+-rwxrwxr-x   0 root         (0)     1003      360 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/testing/constraints-3.7.txt
+-rwxrwxr-x   0 root         (0)     1003      169 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/testing/constraints-3.8.txt
+-rwxrwxr-x   0 root         (0)     1003      169 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/testing/constraints-3.9.txt
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.189653 gapic-generator-1.9.1/tests/integration/goldens/credentials/tests/
+-rwxrwxr-x   0 root         (0)     1003      601 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.189653 gapic-generator-1.9.1/tests/integration/goldens/credentials/tests/unit/
+-rwxrwxr-x   0 root         (0)     1003      601 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.189653 gapic-generator-1.9.1/tests/integration/goldens/credentials/tests/unit/gapic/
+-rwxrwxr-x   0 root         (0)     1003      601 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.189653 gapic-generator-1.9.1/tests/integration/goldens/credentials/tests/unit/gapic/credentials_v1/
+-rwxrwxr-x   0 root         (0)     1003      601 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/tests/unit/gapic/credentials_v1/__init__.py
+-rwxrwxr-x   0 root         (0)     1003   127249 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/credentials/tests/unit/gapic/credentials_v1/test_iam_credentials.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.189653 gapic-generator-1.9.1/tests/integration/goldens/eventarc/
+-rwxrwxr-x   0 root         (0)     1003      257 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/.coveragerc
+-rwxrwxr-x   0 root         (0)     1003      879 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/.flake8
+-rw-rw-r--   0 root         (0)     1003      218 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/BUILD.bazel
+-rwxrwxr-x   0 root         (0)     1003       93 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/MANIFEST.in
+-rwxrwxr-x   0 root         (0)     1003     1450 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.189653 gapic-generator-1.9.1/tests/integration/goldens/eventarc/docs/
+-rwxrwxr-x   0 root         (0)     1003    12470 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/docs/conf.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.189653 gapic-generator-1.9.1/tests/integration/goldens/eventarc/docs/eventarc_v1/
+-rwxrwxr-x   0 root         (0)     1003      239 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/docs/eventarc_v1/eventarc.rst
+-rwxrwxr-x   0 root         (0)     1003      128 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/docs/eventarc_v1/services.rst
+-rwxrwxr-x   0 root         (0)     1003      163 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/docs/eventarc_v1/types.rst
+-rwxrwxr-x   0 root         (0)     1003      106 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/docs/index.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.129652 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.129652 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.189653 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc/
+-rwxrwxr-x   0 root         (0)     1003     2094 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc/__init__.py
+-rwxrwxr-x   0 root         (0)     1003      652 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc/gapic_version.py
+-rwxrwxr-x   0 root         (0)     1003       82 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.193653 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/
+-rwxrwxr-x   0 root         (0)     1003     1666 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/__init__.py
+-rwxrwxr-x   0 root         (0)     1003     2440 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/gapic_metadata.json
+-rwxrwxr-x   0 root         (0)     1003      652 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/gapic_version.py
+-rwxrwxr-x   0 root         (0)     1003       82 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.193653 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/
+-rwxrwxr-x   0 root         (0)     1003      600 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.193653 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/
+-rwxrwxr-x   0 root         (0)     1003      745 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/__init__.py
+-rwxrwxr-x   0 root         (0)     1003    35032 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/async_client.py
+-rwxrwxr-x   0 root         (0)     1003    45203 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/client.py
+-rwxrwxr-x   0 root         (0)     1003     5713 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.193653 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/
+-rwxrwxr-x   0 root         (0)     1003     1334 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/__init__.py
+-rwxrwxr-x   0 root         (0)     1003     8320 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/base.py
+-rwxrwxr-x   0 root         (0)     1003    17238 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/grpc.py
+-rwxrwxr-x   0 root         (0)     1003    17532 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/grpc_asyncio.py
+-rwxrwxr-x   0 root         (0)     1003    32930 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.193653 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/types/
+-rwxrwxr-x   0 root         (0)     1003     1218 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/types/__init__.py
+-rwxrwxr-x   0 root         (0)     1003     9099 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/types/eventarc.py
+-rwxrwxr-x   0 root         (0)     1003     9077 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/types/trigger.py
+-rwxrwxr-x   0 root         (0)     1003       54 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/mypy.ini
+-rwxrwxr-x   0 root         (0)     1003     4814 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/noxfile.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.129652 gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.197653 gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/
+-rwxrwxr-x   0 root         (0)     1003     2312 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_create_trigger_async.py
+-rwxrwxr-x   0 root         (0)     1003     2291 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_create_trigger_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1953 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_delete_trigger_async.py
+-rwxrwxr-x   0 root         (0)     1003     1932 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_delete_trigger_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1818 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_get_trigger_async.py
+-rwxrwxr-x   0 root         (0)     1003     1799 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_get_trigger_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1874 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_list_triggers_async.py
+-rwxrwxr-x   0 root         (0)     1003     1855 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_list_triggers_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1926 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_update_trigger_async.py
+-rwxrwxr-x   0 root         (0)     1003     1905 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_update_trigger_sync.py
+-rwxrwxr-x   0 root         (0)     1003    23069 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/snippet_metadata_google.cloud.eventarc.v1.json
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.197653 gapic-generator-1.9.1/tests/integration/goldens/eventarc/scripts/
+-rwxrwxr-x   0 root         (0)     1003     6269 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/scripts/fixup_eventarc_v1_keywords.py
+-rwxrwxr-x   0 root         (0)     1003     2971 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.197653 gapic-generator-1.9.1/tests/integration/goldens/eventarc/testing/
+-rwxrwxr-x   0 root         (0)     1003      188 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/testing/constraints-3.10.txt
+-rwxrwxr-x   0 root         (0)     1003      188 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/testing/constraints-3.11.txt
+-rwxrwxr-x   0 root         (0)     1003      188 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/testing/constraints-3.12.txt
+-rwxrwxr-x   0 root         (0)     1003      387 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/testing/constraints-3.7.txt
+-rwxrwxr-x   0 root         (0)     1003      188 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/testing/constraints-3.8.txt
+-rwxrwxr-x   0 root         (0)     1003      188 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/testing/constraints-3.9.txt
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.197653 gapic-generator-1.9.1/tests/integration/goldens/eventarc/tests/
+-rwxrwxr-x   0 root         (0)     1003      601 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.197653 gapic-generator-1.9.1/tests/integration/goldens/eventarc/tests/unit/
+-rwxrwxr-x   0 root         (0)     1003      601 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.197653 gapic-generator-1.9.1/tests/integration/goldens/eventarc/tests/unit/gapic/
+-rwxrwxr-x   0 root         (0)     1003      601 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.197653 gapic-generator-1.9.1/tests/integration/goldens/eventarc/tests/unit/gapic/eventarc_v1/
+-rwxrwxr-x   0 root         (0)     1003      601 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/tests/unit/gapic/eventarc_v1/__init__.py
+-rwxrwxr-x   0 root         (0)     1003   156375 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/eventarc/tests/unit/gapic/eventarc_v1/test_eventarc.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.201654 gapic-generator-1.9.1/tests/integration/goldens/logging/
+-rwxrwxr-x   0 root         (0)     1003      255 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/.coveragerc
+-rwxrwxr-x   0 root         (0)     1003      879 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/.flake8
+-rw-rw-r--   0 root         (0)     1003      218 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/BUILD.bazel
+-rwxrwxr-x   0 root         (0)     1003       91 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/MANIFEST.in
+-rwxrwxr-x   0 root         (0)     1003     1448 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.201654 gapic-generator-1.9.1/tests/integration/goldens/logging/docs/
+-rwxrwxr-x   0 root         (0)     1003    12459 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/docs/conf.py
+-rwxrwxr-x   0 root         (0)     1003      104 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/docs/index.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.201654 gapic-generator-1.9.1/tests/integration/goldens/logging/docs/logging_v2/
+-rwxrwxr-x   0 root         (0)     1003      269 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/docs/logging_v2/config_service_v2.rst
+-rwxrwxr-x   0 root         (0)     1003      273 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/docs/logging_v2/logging_service_v2.rst
+-rwxrwxr-x   0 root         (0)     1003      273 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/docs/logging_v2/metrics_service_v2.rst
+-rwxrwxr-x   0 root         (0)     1003      181 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/docs/logging_v2/services.rst
+-rwxrwxr-x   0 root         (0)     1003      160 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/docs/logging_v2/types.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.129652 gapic-generator-1.9.1/tests/integration/goldens/logging/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.129652 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.201654 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging/
+-rwxrwxr-x   0 root         (0)     1003     7206 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging/__init__.py
+-rwxrwxr-x   0 root         (0)     1003      652 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging/gapic_version.py
+-rwxrwxr-x   0 root         (0)     1003       81 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.201654 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/
+-rwxrwxr-x   0 root         (0)     1003     5492 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/__init__.py
+-rwxrwxr-x   0 root         (0)     1003    13874 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/gapic_metadata.json
+-rwxrwxr-x   0 root         (0)     1003      652 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/gapic_version.py
+-rwxrwxr-x   0 root         (0)     1003       81 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.201654 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/
+-rwxrwxr-x   0 root         (0)     1003      600 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.205654 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/
+-rwxrwxr-x   0 root         (0)     1003      773 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/__init__.py
+-rwxrwxr-x   0 root         (0)     1003   109353 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/async_client.py
+-rwxrwxr-x   0 root         (0)     1003   120820 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/client.py
+-rwxrwxr-x   0 root         (0)     1003    20534 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.205654 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/
+-rwxrwxr-x   0 root         (0)     1003     1432 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/__init__.py
+-rwxrwxr-x   0 root         (0)     1003    19189 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/base.py
+-rwxrwxr-x   0 root         (0)     1003    38551 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/grpc.py
+-rwxrwxr-x   0 root         (0)     1003    39233 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/grpc_asyncio.py
+-rwxrwxr-x   0 root         (0)     1003   129806 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.205654 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/
+-rwxrwxr-x   0 root         (0)     1003      777 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/__init__.py
+-rwxrwxr-x   0 root         (0)     1003    43626 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/async_client.py
+-rwxrwxr-x   0 root         (0)     1003    50681 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/client.py
+-rwxrwxr-x   0 root         (0)     1003    16108 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.209654 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/
+-rwxrwxr-x   0 root         (0)     1003     1446 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/__init__.py
+-rwxrwxr-x   0 root         (0)     1003    11152 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/base.py
+-rwxrwxr-x   0 root         (0)     1003    18757 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/grpc.py
+-rwxrwxr-x   0 root         (0)     1003    19066 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/grpc_asyncio.py
+-rwxrwxr-x   0 root         (0)     1003    32421 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.209654 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/
+-rwxrwxr-x   0 root         (0)     1003      777 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/__init__.py
+-rwxrwxr-x   0 root         (0)     1003    34495 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/async_client.py
+-rwxrwxr-x   0 root         (0)     1003    42593 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/client.py
+-rwxrwxr-x   0 root         (0)     1003     5794 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.209654 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/
+-rwxrwxr-x   0 root         (0)     1003     1446 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/__init__.py
+-rwxrwxr-x   0 root         (0)     1003     9857 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/base.py
+-rwxrwxr-x   0 root         (0)     1003    16452 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/grpc.py
+-rwxrwxr-x   0 root         (0)     1003    16739 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/grpc_asyncio.py
+-rwxrwxr-x   0 root         (0)     1003    32409 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.209654 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/types/
+-rwxrwxr-x   0 root         (0)     1003     3610 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/types/__init__.py
+-rwxrwxr-x   0 root         (0)     1003    12763 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/types/log_entry.py
+-rwxrwxr-x   0 root         (0)     1003    23104 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/types/logging.py
+-rwxrwxr-x   0 root         (0)     1003    50688 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/types/logging_config.py
+-rwxrwxr-x   0 root         (0)     1003    13420 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/types/logging_metrics.py
+-rwxrwxr-x   0 root         (0)     1003       54 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/mypy.ini
+-rwxrwxr-x   0 root         (0)     1003     4813 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/noxfile.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.133652 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.225654 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/
+-rwxrwxr-x   0 root         (0)     1003     1886 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_bucket_async.py
+-rwxrwxr-x   0 root         (0)     1003     1867 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_bucket_sync.py
+-rwxrwxr-x   0 root         (0)     1003     2011 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_exclusion_async.py
+-rwxrwxr-x   0 root         (0)     1003     1992 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_exclusion_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1961 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_sink_async.py
+-rwxrwxr-x   0 root         (0)     1003     1942 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_sink_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1870 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_view_async.py
+-rwxrwxr-x   0 root         (0)     1003     1851 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_view_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1788 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_bucket_async.py
+-rwxrwxr-x   0 root         (0)     1003     1769 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_bucket_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1806 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_exclusion_async.py
+-rwxrwxr-x   0 root         (0)     1003     1787 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_exclusion_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1786 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_sink_async.py
+-rwxrwxr-x   0 root         (0)     1003     1767 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_sink_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1776 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_view_async.py
+-rwxrwxr-x   0 root         (0)     1003     1757 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_view_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1827 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_bucket_async.py
+-rwxrwxr-x   0 root         (0)     1003     1808 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_bucket_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1865 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_cmek_settings_async.py
+-rwxrwxr-x   0 root         (0)     1003     1846 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_cmek_settings_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1845 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_exclusion_async.py
+-rwxrwxr-x   0 root         (0)     1003     1826 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_exclusion_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1825 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_sink_async.py
+-rwxrwxr-x   0 root         (0)     1003     1806 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_sink_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1815 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_view_async.py
+-rwxrwxr-x   0 root         (0)     1003     1796 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_view_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1883 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_buckets_async.py
+-rwxrwxr-x   0 root         (0)     1003     1864 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_buckets_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1901 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_exclusions_async.py
+-rwxrwxr-x   0 root         (0)     1003     1882 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_exclusions_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1871 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_sinks_async.py
+-rwxrwxr-x   0 root         (0)     1003     1852 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_sinks_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1871 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_views_async.py
+-rwxrwxr-x   0 root         (0)     1003     1852 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_views_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1800 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_undelete_bucket_async.py
+-rwxrwxr-x   0 root         (0)     1003     1781 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_undelete_bucket_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1845 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_bucket_async.py
+-rwxrwxr-x   0 root         (0)     1003     1826 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_bucket_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1883 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_cmek_settings_async.py
+-rwxrwxr-x   0 root         (0)     1003     1864 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_cmek_settings_sync.py
+-rwxrwxr-x   0 root         (0)     1003     2007 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_exclusion_async.py
+-rwxrwxr-x   0 root         (0)     1003     1988 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_exclusion_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1967 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_sink_async.py
+-rwxrwxr-x   0 root         (0)     1003     1948 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_sink_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1833 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_view_async.py
+-rwxrwxr-x   0 root         (0)     1003     1814 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_view_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1781 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_delete_log_async.py
+-rwxrwxr-x   0 root         (0)     1003     1762 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_delete_log_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1950 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_log_entries_async.py
+-rwxrwxr-x   0 root         (0)     1003     1931 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_log_entries_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1868 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_logs_async.py
+-rwxrwxr-x   0 root         (0)     1003     1849 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_logs_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1985 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_monitored_resource_descriptors_async.py
+-rwxrwxr-x   0 root         (0)     1003     1966 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_monitored_resource_descriptors_sync.py
+-rwxrwxr-x   0 root         (0)     1003     2274 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_tail_log_entries_async.py
+-rwxrwxr-x   0 root         (0)     1003     2249 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_tail_log_entries_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1943 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_write_log_entries_async.py
+-rwxrwxr-x   0 root         (0)     1003     1924 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_write_log_entries_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1998 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_create_log_metric_async.py
+-rwxrwxr-x   0 root         (0)     1003     1979 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_create_log_metric_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1825 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_delete_log_metric_async.py
+-rwxrwxr-x   0 root         (0)     1003     1806 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_delete_log_metric_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1864 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_get_log_metric_async.py
+-rwxrwxr-x   0 root         (0)     1003     1845 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_get_log_metric_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1906 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_list_log_metrics_async.py
+-rwxrwxr-x   0 root         (0)     1003     1887 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_list_log_metrics_sync.py
+-rwxrwxr-x   0 root         (0)     1003     2008 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_update_log_metric_async.py
+-rwxrwxr-x   0 root         (0)     1003     1989 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_update_log_metric_sync.py
+-rwxrwxr-x   0 root         (0)     1003   151672 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/snippet_metadata_google.logging.v2.json
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.225654 gapic-generator-1.9.1/tests/integration/goldens/logging/scripts/
+-rwxrwxr-x   0 root         (0)     1003     7882 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/scripts/fixup_logging_v2_keywords.py
+-rwxrwxr-x   0 root         (0)     1003     2920 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.225654 gapic-generator-1.9.1/tests/integration/goldens/logging/testing/
+-rwxrwxr-x   0 root         (0)     1003      169 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/testing/constraints-3.10.txt
+-rwxrwxr-x   0 root         (0)     1003      169 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/testing/constraints-3.11.txt
+-rwxrwxr-x   0 root         (0)     1003      169 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/testing/constraints-3.12.txt
+-rwxrwxr-x   0 root         (0)     1003      360 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/testing/constraints-3.7.txt
+-rwxrwxr-x   0 root         (0)     1003      169 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/testing/constraints-3.8.txt
+-rwxrwxr-x   0 root         (0)     1003      169 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/testing/constraints-3.9.txt
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.225654 gapic-generator-1.9.1/tests/integration/goldens/logging/tests/
+-rwxrwxr-x   0 root         (0)     1003      601 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.225654 gapic-generator-1.9.1/tests/integration/goldens/logging/tests/unit/
+-rwxrwxr-x   0 root         (0)     1003      601 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.225654 gapic-generator-1.9.1/tests/integration/goldens/logging/tests/unit/gapic/
+-rwxrwxr-x   0 root         (0)     1003      601 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.229654 gapic-generator-1.9.1/tests/integration/goldens/logging/tests/unit/gapic/logging_v2/
+-rwxrwxr-x   0 root         (0)     1003      601 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/tests/unit/gapic/logging_v2/__init__.py
+-rwxrwxr-x   0 root         (0)     1003   462598 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/tests/unit/gapic/logging_v2/test_config_service_v2.py
+-rwxrwxr-x   0 root         (0)     1003   158758 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/tests/unit/gapic/logging_v2/test_logging_service_v2.py
+-rwxrwxr-x   0 root         (0)     1003   159800 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/logging/tests/unit/gapic/logging_v2/test_metrics_service_v2.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.229654 gapic-generator-1.9.1/tests/integration/goldens/redis/
+-rwxrwxr-x   0 root         (0)     1003      251 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/.coveragerc
+-rwxrwxr-x   0 root         (0)     1003      879 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/.flake8
+-rw-rw-r--   0 root         (0)     1003      218 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/BUILD.bazel
+-rwxrwxr-x   0 root         (0)     1003       87 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/MANIFEST.in
+-rwxrwxr-x   0 root         (0)     1003     1444 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.229654 gapic-generator-1.9.1/tests/integration/goldens/redis/docs/
+-rwxrwxr-x   0 root         (0)     1003    12437 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/docs/conf.py
+-rwxrwxr-x   0 root         (0)     1003      100 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/docs/index.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.229654 gapic-generator-1.9.1/tests/integration/goldens/redis/docs/redis_v1/
+-rwxrwxr-x   0 root         (0)     1003      243 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/docs/redis_v1/cloud_redis.rst
+-rwxrwxr-x   0 root         (0)     1003      125 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/docs/redis_v1/services.rst
+-rwxrwxr-x   0 root         (0)     1003      154 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/docs/redis_v1/types.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.133652 gapic-generator-1.9.1/tests/integration/goldens/redis/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.133652 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.233654 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis/
+-rwxrwxr-x   0 root         (0)     1003     2656 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis/__init__.py
+-rwxrwxr-x   0 root         (0)     1003      652 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis/gapic_version.py
+-rwxrwxr-x   0 root         (0)     1003       79 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.233654 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/
+-rwxrwxr-x   0 root         (0)     1003     2148 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/__init__.py
+-rwxrwxr-x   0 root         (0)     1003     3978 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/gapic_metadata.json
+-rwxrwxr-x   0 root         (0)     1003      652 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/gapic_version.py
+-rwxrwxr-x   0 root         (0)     1003       79 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.233654 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/
+-rwxrwxr-x   0 root         (0)     1003      600 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.233654 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/
+-rwxrwxr-x   0 root         (0)     1003      753 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/__init__.py
+-rwxrwxr-x   0 root         (0)     1003    59144 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/async_client.py
+-rwxrwxr-x   0 root         (0)     1003    69218 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/client.py
+-rwxrwxr-x   0 root         (0)     1003     5708 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.233654 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/
+-rwxrwxr-x   0 root         (0)     1003     1362 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/__init__.py
+-rwxrwxr-x   0 root         (0)     1003    10038 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/base.py
+-rwxrwxr-x   0 root         (0)     1003    24385 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/grpc.py
+-rwxrwxr-x   0 root         (0)     1003    24769 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/grpc_asyncio.py
+-rwxrwxr-x   0 root         (0)     1003    54118 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.233654 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/types/
+-rwxrwxr-x   0 root         (0)     1003     1512 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/types/__init__.py
+-rwxrwxr-x   0 root         (0)     1003    25588 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/types/cloud_redis.py
+-rwxrwxr-x   0 root         (0)     1003       54 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/mypy.ini
+-rwxrwxr-x   0 root         (0)     1003     4811 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/noxfile.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.133652 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.237654 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/
+-rwxrwxr-x   0 root         (0)     1003     2129 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_create_instance_async.py
+-rwxrwxr-x   0 root         (0)     1003     2108 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_create_instance_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1919 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_delete_instance_async.py
+-rwxrwxr-x   0 root         (0)     1003     1898 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_delete_instance_sync.py
+-rwxrwxr-x   0 root         (0)     1003     2053 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_export_instance_async.py
+-rwxrwxr-x   0 root         (0)     1003     2032 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_export_instance_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1931 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_failover_instance_async.py
+-rwxrwxr-x   0 root         (0)     1003     1910 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_failover_instance_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1812 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_get_instance_async.py
+-rwxrwxr-x   0 root         (0)     1003     1793 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_get_instance_sync.py
+-rwxrwxr-x   0 root         (0)     1003     2043 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_import_instance_async.py
+-rwxrwxr-x   0 root         (0)     1003     2022 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_import_instance_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1868 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_list_instances_async.py
+-rwxrwxr-x   0 root         (0)     1003     1849 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_list_instances_sync.py
+-rwxrwxr-x   0 root         (0)     1003     2057 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_update_instance_async.py
+-rwxrwxr-x   0 root         (0)     1003     2036 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_update_instance_sync.py
+-rwxrwxr-x   0 root         (0)     1003     1970 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_upgrade_instance_async.py
+-rwxrwxr-x   0 root         (0)     1003     1949 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_upgrade_instance_sync.py
+-rwxrwxr-x   0 root         (0)     1003    41251 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/snippet_metadata_google.cloud.redis.v1.json
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.237654 gapic-generator-1.9.1/tests/integration/goldens/redis/scripts/
+-rwxrwxr-x   0 root         (0)     1003     6396 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/scripts/fixup_redis_v1_keywords.py
+-rwxrwxr-x   0 root         (0)     1003     2912 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.241654 gapic-generator-1.9.1/tests/integration/goldens/redis/testing/
+-rwxrwxr-x   0 root         (0)     1003      169 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/testing/constraints-3.10.txt
+-rwxrwxr-x   0 root         (0)     1003      169 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/testing/constraints-3.11.txt
+-rwxrwxr-x   0 root         (0)     1003      169 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/testing/constraints-3.12.txt
+-rwxrwxr-x   0 root         (0)     1003      360 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/testing/constraints-3.7.txt
+-rwxrwxr-x   0 root         (0)     1003      169 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/testing/constraints-3.8.txt
+-rwxrwxr-x   0 root         (0)     1003      169 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/testing/constraints-3.9.txt
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.241654 gapic-generator-1.9.1/tests/integration/goldens/redis/tests/
+-rwxrwxr-x   0 root         (0)     1003      601 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.241654 gapic-generator-1.9.1/tests/integration/goldens/redis/tests/unit/
+-rwxrwxr-x   0 root         (0)     1003      601 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.241654 gapic-generator-1.9.1/tests/integration/goldens/redis/tests/unit/gapic/
+-rwxrwxr-x   0 root         (0)     1003      601 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.241654 gapic-generator-1.9.1/tests/integration/goldens/redis/tests/unit/gapic/redis_v1/
+-rwxrwxr-x   0 root         (0)     1003      601 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/tests/unit/gapic/redis_v1/__init__.py
+-rwxrwxr-x   0 root         (0)     1003   232638 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/goldens/redis/tests/unit/gapic/redis_v1/test_cloud_redis.py
+-rwxrwxr-x   0 root         (0)     1003      828 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/iamcredentials_grpc_service_config.json
+-rwxrwxr-x   0 root         (0)     1003     3935 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/logging_grpc_service_config.json
+-rwxrwxr-x   0 root         (0)     1003     1244 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/integration/redis_grpc_service_config.json
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.241654 gapic-generator-1.9.1/tests/snippetgen/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.245654 gapic-generator-1.9.1/tests/snippetgen/goldens/
+-rw-rw-r--   0 root         (0)     1003     1935 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_list_resources_async.py
+-rw-rw-r--   0 root         (0)     1003     1916 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_list_resources_sync.py
+-rw-rw-r--   0 root         (0)     1003     2258 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_bidi_streaming_async.py
+-rw-rw-r--   0 root         (0)     1003     2233 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_bidi_streaming_sync.py
+-rw-rw-r--   0 root         (0)     1003     2203 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_lro_signatures_async.py
+-rw-rw-r--   0 root         (0)     1003     2182 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_lro_signatures_sync.py
+-rw-rw-r--   0 root         (0)     1003     2109 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_one_signature_async.py
+-rw-rw-r--   0 root         (0)     1003     2090 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_one_signature_sync.py
+-rw-rw-r--   0 root         (0)     1003     2160 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_server_streaming_async.py
+-rw-rw-r--   0 root         (0)     1003     2135 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_server_streaming_sync.py
+-rw-rw-r--   0 root         (0)     1003     1875 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_one_of_method_async.py
+-rw-rw-r--   0 root         (0)     1003     1961 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_one_of_method_required_field_async.py
+-rw-rw-r--   0 root         (0)     1003     1942 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_one_of_method_required_field_sync.py
+-rw-rw-r--   0 root         (0)     1003     1856 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_one_of_method_sync.py
+-rw-rw-r--   0 root         (0)     1003    13844 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/snippetgen/goldens/snippet_metadata_mollusca_v1.json
+-rw-rw-r--   0 root         (0)     1003     4610 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/snippetgen/snippets.proto
+-rw-rw-r--   0 root         (0)     1003     2818 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/snippetgen/test_snippetgen.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.245654 gapic-generator-1.9.1/tests/system/
+-rw-rw-r--   0 root         (0)     1003     6811 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/system/conftest.py
+-rw-rw-r--   0 root         (0)     1003     1645 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/system/test_client_context_manager.py
+-rw-rw-r--   0 root         (0)     1003     3128 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/system/test_error_details.py
+-rw-rw-r--   0 root         (0)     1003     1645 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/system/test_grpc_interceptor_streams.py
+-rw-rw-r--   0 root         (0)     1003     1770 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/system/test_lro.py
+-rw-rw-r--   0 root         (0)     1003     3047 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/system/test_pagination.py
+-rw-rw-r--   0 root         (0)     1003     4090 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/system/test_resource_crud.py
+-rw-rw-r--   0 root         (0)     1003     1884 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/system/test_retry.py
+-rw-rw-r--   0 root         (0)     1003     7593 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/system/test_streams.py
+-rw-rw-r--   0 root         (0)     1003     3317 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/system/test_unary.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.245654 gapic-generator-1.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003        0 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5256 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/common_types.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.245654 gapic-generator-1.9.1/tests/unit/configurable_snippetgen/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.245654 gapic-generator-1.9.1/tests/unit/configurable_snippetgen/resources/
+-rw-rw-r--   0 root         (0)     1003     1161 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/configurable_snippetgen/resources/README.md
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.249655 gapic-generator-1.9.1/tests/unit/configurable_snippetgen/resources/speech/
+-rw-rw-r--   0 root         (0)     1003   213102 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/configurable_snippetgen/resources/speech/request.desc
+-rw-rw-r--   0 root         (0)     1003     4695 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/configurable_snippetgen/resources/speech/speech_createCustomClass.json
+-rw-rw-r--   0 root         (0)     1003     2311 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/configurable_snippetgen/resources/speech/speech_v1_generated_adaptation_create_custom_class_basic_async.py
+-rw-rw-r--   0 root         (0)     1003     8717 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/configurable_snippetgen/test_configured_snippet.py
+-rw-rw-r--   0 root         (0)     1003     3433 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/configurable_snippetgen/test_libcst_utils.py
+-rw-rw-r--   0 root         (0)     1003     1536 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/configurable_snippetgen/test_resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.249655 gapic-generator-1.9.1/tests/unit/generator/
+-rw-rw-r--   0 root         (0)     1003        0 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/generator/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2725 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/generator/test_formatter.py
+-rw-rw-r--   0 root         (0)     1003    28198 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/generator/test_generator.py
+-rw-rw-r--   0 root         (0)     1003     7938 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/generator/test_options.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.249655 gapic-generator-1.9.1/tests/unit/samplegen/
+-rw-rw-r--   0 root         (0)     1003        0 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/samplegen/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.249655 gapic-generator-1.9.1/tests/unit/samplegen/golden_snippets/
+-rw-rw-r--   0 root         (0)     1003     2080 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/samplegen/golden_snippets/sample_basic.py
+-rw-rw-r--   0 root         (0)     1003     2097 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/samplegen/golden_snippets/sample_basic_async.py
+-rw-rw-r--   0 root         (0)     1003     2080 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/samplegen/golden_snippets/sample_basic_unflattenable.py
+-rw-rw-r--   0 root         (0)     1003     1992 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/samplegen/golden_snippets/sample_basic_void_method.py
+-rw-rw-r--   0 root         (0)     1003    23715 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/samplegen/test_integration.py
+-rw-rw-r--   0 root         (0)     1003     5328 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/samplegen/test_manifest.py
+-rw-rw-r--   0 root         (0)     1003    80651 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/samplegen/test_samplegen.py
+-rw-rw-r--   0 root         (0)     1003    10145 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/samplegen/test_snippet_index.py
+-rw-rw-r--   0 root         (0)     1003    42147 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/samplegen/test_template.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.253655 gapic-generator-1.9.1/tests/unit/schema/
+-rw-rw-r--   0 root         (0)     1003    97787 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/schema/test_api.py
+-rw-rw-r--   0 root         (0)     1003     1790 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/schema/test_imp.py
+-rw-rw-r--   0 root         (0)     1003     8431 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/schema/test_metadata.py
+-rw-rw-r--   0 root         (0)     1003     7589 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/schema/test_naming.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.253655 gapic-generator-1.9.1/tests/unit/schema/wrappers/
+-rw-rw-r--   0 root         (0)     1003     1847 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/schema/wrappers/test_enums.py
+-rw-rw-r--   0 root         (0)     1003    16779 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/schema/wrappers/test_field.py
+-rw-rw-r--   0 root         (0)     1003    16096 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/schema/wrappers/test_message.py
+-rw-rw-r--   0 root         (0)     1003    31723 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/schema/wrappers/test_method.py
+-rw-rw-r--   0 root         (0)     1003     1026 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/schema/wrappers/test_oneof.py
+-rw-rw-r--   0 root         (0)     1003     1568 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/schema/wrappers/test_python.py
+-rw-rw-r--   0 root         (0)     1003     5545 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/schema/wrappers/test_routing.py
+-rw-rw-r--   0 root         (0)     1003    21284 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/schema/wrappers/test_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-22 16:41:14.253655 gapic-generator-1.9.1/tests/unit/utils/
+-rw-rw-r--   0 root         (0)     1003      981 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/utils/test_cache.py
+-rw-rw-r--   0 root         (0)     1003     1322 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/utils/test_case.py
+-rw-rw-r--   0 root         (0)     1003     1406 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/utils/test_checks.py
+-rw-rw-r--   0 root         (0)     1003     1212 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/utils/test_code.py
+-rw-rw-r--   0 root         (0)     1003     1218 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/utils/test_filename.py
+-rw-rw-r--   0 root         (0)     1003     2529 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/utils/test_lines.py
+-rw-rw-r--   0 root         (0)     1003     2232 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/utils/test_rst.py
+-rw-rw-r--   0 root         (0)     1003     1130 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/utils/test_uri_conv.py
+-rw-rw-r--   0 root         (0)     1003     1205 2023-03-22 16:38:27.000000 gapic-generator-1.9.1/tests/unit/utils/test_uri_sample.py
```

### Comparing `gapic-generator-1.9.0/LICENSE` & `gapic-generator-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/PKG-INFO` & `gapic-generator-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gapic-generator
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google API Client Generator for Python
 Home-page: https://github.com/googleapis/gapic-generator-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `gapic-generator-1.9.0/README.rst` & `gapic-generator-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/__init__.py` & `gapic-generator-1.9.1/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/cli/__init__.py` & `gapic-generator-1.9.1/gapic/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/cli/dump.py` & `gapic-generator-1.9.1/gapic/cli/dump.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/cli/generate.py` & `gapic-generator-1.9.1/gapic/cli/generate.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/configurable_snippetgen/__init__.py` & `gapic-generator-1.9.1/gapic/configurable_snippetgen/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/configurable_snippetgen/configured_snippet.py` & `gapic-generator-1.9.1/gapic/configurable_snippetgen/configured_snippet.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/configurable_snippetgen/libcst_utils.py` & `gapic-generator-1.9.1/gapic/configurable_snippetgen/libcst_utils.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/configurable_snippetgen/snippet_config_language.proto` & `gapic-generator-1.9.1/gapic/configurable_snippetgen/snippet_config_language.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/configurable_snippetgen/snippet_config_language_pb2.py` & `gapic-generator-1.9.1/gapic/configurable_snippetgen/snippet_config_language_pb2.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/generator/__init__.py` & `gapic-generator-1.9.1/gapic/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/generator/formatter.py` & `gapic-generator-1.9.1/gapic/generator/formatter.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/generator/generator.py` & `gapic-generator-1.9.1/gapic/generator/generator.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/samplegen/__init__.py` & `gapic-generator-1.9.1/gapic/samplegen/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/samplegen/manifest.py` & `gapic-generator-1.9.1/gapic/samplegen/manifest.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/samplegen/samplegen.py` & `gapic-generator-1.9.1/gapic/samplegen/samplegen.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/samplegen_utils/__init__.py` & `gapic-generator-1.9.1/gapic/samplegen_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/samplegen_utils/snippet_index.py` & `gapic-generator-1.9.1/gapic/samplegen_utils/snippet_index.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/samplegen_utils/snippet_metadata.proto` & `gapic-generator-1.9.1/gapic/samplegen_utils/snippet_metadata.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/samplegen_utils/snippet_metadata_pb2.py` & `gapic-generator-1.9.1/gapic/samplegen_utils/snippet_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/samplegen_utils/types.py` & `gapic-generator-1.9.1/gapic/samplegen_utils/types.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/samplegen_utils/utils.py` & `gapic-generator-1.9.1/gapic/samplegen_utils/utils.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/samplegen_utils/yaml.py` & `gapic-generator-1.9.1/gapic/samplegen_utils/yaml.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/schema/__init__.py` & `gapic-generator-1.9.1/gapic/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/schema/api.py` & `gapic-generator-1.9.1/gapic/schema/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -485,15 +485,17 @@
 
         return gm
 
     def gapic_metadata_json(self, options: Options) -> str:
         return MessageToJson(self.gapic_metadata(options), sort_keys=True)
 
     def requires_package(self, pkg: Tuple[str, ...]) -> bool:
-        return any(
+        pkg_has_iam_mixin = self.has_iam_mixin and \
+            pkg == ('google', 'iam', 'v1')
+        return pkg_has_iam_mixin or any(
             message.ident.package == pkg
             for proto in self.all_protos.values()
             for message in proto.all_messages.values()
         )
 
     def get_custom_operation_service(self, method: "wrappers.Method") -> "wrappers.Service":
         """Return the extended operation service that should be polled for progress
```

### Comparing `gapic-generator-1.9.0/gapic/schema/imp.py` & `gapic-generator-1.9.1/gapic/schema/imp.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/schema/metadata.py` & `gapic-generator-1.9.1/gapic/schema/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,27 @@
         return '.'.join(self.package + self.parent + (self.name,))
 
     @property
     def proto_package(self) -> str:
         """Return the proto package for this type."""
         return '.'.join(self.package)
 
+    def convert_to_versioned_package(self) -> Tuple[str, ...]:
+        # We need to change the import statement to use an
+        # underscore between the module and the version. For example,
+        # change google.cloud.documentai.v1 to google.cloud.documentai_v1.
+        # Check if the package name contains a version.
+        version_regex = "^v\d[^/]*$"
+        regex_match = re.match(version_regex, self.package[-1])
+        if regex_match and len(self.package) > 1:
+            versioned_module = f"{self.package[-2]}_{regex_match[0]}"
+            return self.package[:-2] + (versioned_module,)
+        else:
+            return self.package
+
     @cached_property
     def python_import(self) -> imp.Import:
         """Return the Python import for this type."""
         # If there is no naming object, then this is a special case for
         # Python types.
         #
         # FIXME: This does not attempt to do an isinstance check on PythonType
@@ -199,35 +212,19 @@
                     self.api_naming.versioned_module_name,
                 ) + self.subpackage + ('types',),
                 module=self.module,
                 alias=self.module_alias,
             )
 
         if self.is_proto_plus_type:
-            # We need to change the import statement to use an
-            # underscore between the module and the version. For example,
-            # change google.cloud.documentai.v1 to google.cloud.documentai_v1.
-            # Check if the package name contains a version.
-            version_regex = "^v\d[^/]*$"
-            regex_match = re.match(version_regex, self.package[-1])
-
-            if regex_match and len(self.package) > 1:
-                versioned_module = f"{self.package[-2]}_{regex_match[0]}"
-                return imp.Import(
-                    package=self.package[:-2] +
-                    (versioned_module, 'types'),
-                    module=self.module,
-                    alias=self.module_alias,
-                )
-            else:
-                return imp.Import(
-                    package=self.package + ('types',),
-                    module=self.module,
-                    alias=self.module_alias,
-                )
+            return imp.Import(
+                package=self.convert_to_versioned_package() + ('types',),
+                module=self.module,
+                alias=self.module_alias,
+            )
 
         # Return the standard import.
         return imp.Import(
             package=self.package,
             module=f'{self.module}_pb2',
         )
 
@@ -243,14 +240,21 @@
 
         # Check if this is a generated type
         # Use the original module name rather than the module_alias
         if self.proto_package.startswith(self.api_naming.proto_package):
             return '.'.join(self.api_naming.module_namespace + (
                 self.api_naming.versioned_module_name,
             ) + self.subpackage + ('types',) + self.parent + (self.name, ))
+        elif self.is_proto_plus_type:
+            return ".".join(
+                self.convert_to_versioned_package()
+                + ("types",)
+                + self.parent
+                + (self.name,)
+            )
 
         # Anything left is a standard _pb2 type
         return f'{self.proto_package}.{self.module}_pb2.{self.name}'
 
     @property
     def subpackage(self) -> Tuple[str, ...]:
         """Return the subpackage below the versioned module name, if any."""
```

### Comparing `gapic-generator-1.9.0/gapic/schema/mixins.py` & `gapic-generator-1.9.1/gapic/schema/mixins.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/schema/naming.py` & `gapic-generator-1.9.1/gapic/schema/naming.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/schema/wrappers.py` & `gapic-generator-1.9.1/gapic/schema/wrappers.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/%namespace/%name/__init__.py.j2` & `gapic-generator-1.9.1/gapic/templates/%namespace/%name/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/__init__.py.j2` & `gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/_async_mixins.py.j2` & `gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/_async_mixins.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/_client_macros.j2` & `gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/_client_macros.j2`

 * *Files 2% similar despite different names*

```diff
@@ -46,26 +46,26 @@
         {% endif %}
         {% endwith %}
 
         Args:
             {% if not method.client_streaming %}
             request (Union[{{ method.input.ident.sphinx }}, dict]):
                 The request object.{{ " " }}
-                {{- method.input.meta.doc|wrap(width=72, offset=36, indent=16) }}
+                {{- method.input.meta.doc|rst(width=72, indent=16, nl=False) }}
             {% for key, field in method.flattened_fields.items() %}
             {{ field.name }} ({{ field.ident.sphinx }}):
                 {{ field.meta.doc|rst(width=72, indent=16) }}
                 This corresponds to the ``{{ key }}`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             {% endfor %}
             {% else %}
             requests (Iterator[{{ method.input.ident.sphinx }}]):
                 The request object iterator.{{ " " }}
-                {{- method.input.meta.doc|wrap(width=72, offset=36, indent=16) }}
+                {{- method.input.meta.doc|rst(width=72, indent=16, nl=False) }}
             {% endif %}
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         {% if not method.void %}
```

### Comparing `gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/_mixins.py.j2` & `gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/_mixins.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/async_client.py.j2` & `gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/async_client.py.j2`

 * *Files 0% similar despite different names*

```diff
@@ -224,26 +224,26 @@
         {% endif %}
         {% endwith %}
 
         Args:
             {% if not method.client_streaming %}
             request (Optional[Union[{{ method.input.ident.sphinx }}, dict]]):
                 The request object.{{ " " }}
-                {{- method.input.meta.doc|wrap(width=72, offset=36, indent=16) }}
+                {{- method.input.meta.doc|rst(width=72, indent=16, nl=False) }}
             {% for key, field in method.flattened_fields.items() %}
             {{ field.name }} (:class:`{{ field.ident.sphinx }}`):
                 {{ field.meta.doc|rst(width=72, indent=16) }}
                 This corresponds to the ``{{ key }}`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             {% endfor %}
             {% else %}
             requests (AsyncIterator[`{{ method.input.ident.sphinx }}`]):
                 The request object AsyncIterator.{{ " " }}
-                {{- method.input.meta.doc|wrap(width=72, offset=36, indent=16) }}
+                {{- method.input.meta.doc|rst(width=72, indent=16, nl=False) }}
             {% endif %}
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         {% if not method.void %}
```

### Comparing `gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/client.py.j2` & `gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/client.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/pagers.py.j2` & `gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/pagers.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/__init__.py.j2` & `gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/_mixins.py.j2` & `gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/_mixins.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/_rest_mixins.py.j2` & `gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/_rest_mixins.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/base.py.j2` & `gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/base.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/grpc.py.j2` & `gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/grpc.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/grpc_asyncio.py.j2` & `gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/grpc_asyncio.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/rest.py.j2` & `gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/services/%service/transports/rest.py.j2`

 * *Files 0% similar despite different names*

```diff
@@ -327,15 +327,15 @@
             {{ (method.name|snake_case).replace('_',' ')|wrap(
                     width=70, offset=45, indent=8) }}
             {{- ' ' -}} method over HTTP.
 
             Args:
                 request (~.{{ method.input.ident }}):
                     The request object.{{ ' ' }}
-                    {{- method.input.meta.doc|rst(width=72, indent=16) }}
+                    {{- method.input.meta.doc|rst(width=72, indent=16, nl=False) }}
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
             {% if not method.void %}
```

### Comparing `gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/types/%proto.py.j2` & `gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/types/%proto.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/types/__init__.py.j2` & `gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/types/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/types/_enum.py.j2` & `gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/types/_enum.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/%namespace/%name_%version/%sub/types/_message.py.j2` & `gapic-generator-1.9.1/gapic/templates/%namespace/%name_%version/%sub/types/_message.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/.flake8.j2` & `gapic-generator-1.9.1/gapic/templates/.flake8.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/README.rst.j2` & `gapic-generator-1.9.1/gapic/templates/README.rst.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/_license.j2` & `gapic-generator-1.9.1/gapic/templates/_license.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/_pypi_packages.j2` & `gapic-generator-1.9.1/gapic/templates/_pypi_packages.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/docs/%name_%version/%service.rst.j2` & `gapic-generator-1.9.1/gapic/templates/docs/%name_%version/%service.rst.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/docs/conf.py.j2` & `gapic-generator-1.9.1/gapic/templates/docs/conf.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/examples/feature_fragments.j2` & `gapic-generator-1.9.1/gapic/templates/examples/feature_fragments.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/examples/sample.py.j2` & `gapic-generator-1.9.1/gapic/templates/examples/sample.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/noxfile.py.j2` & `gapic-generator-1.9.1/gapic/templates/noxfile.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/scripts/fixup_%name_%version_keywords.py.j2` & `gapic-generator-1.9.1/gapic/templates/scripts/fixup_%name_%version_keywords.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/setup.py.j2` & `gapic-generator-1.9.1/gapic/templates/setup.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/testing/_default_constraints.j2` & `gapic-generator-1.9.1/gapic/templates/testing/_default_constraints.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/testing/constraints-3.7.txt.j2` & `gapic-generator-1.9.1/gapic/templates/testing/constraints-3.7.txt.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/tests/unit/gapic/%name_%version/%sub/_test_mixins.py.j2` & `gapic-generator-1.9.1/gapic/templates/tests/unit/gapic/%name_%version/%sub/_test_mixins.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/tests/unit/gapic/%name_%version/%sub/test_%service.py.j2` & `gapic-generator-1.9.1/gapic/templates/tests/unit/gapic/%name_%version/%sub/test_%service.py.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/templates/tests/unit/gapic/%name_%version/%sub/test_macros.j2` & `gapic-generator-1.9.1/gapic/templates/tests/unit/gapic/%name_%version/%sub/test_macros.j2`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/utils/__init__.py` & `gapic-generator-1.9.1/gapic/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/utils/cache.py` & `gapic-generator-1.9.1/gapic/utils/cache.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/utils/case.py` & `gapic-generator-1.9.1/gapic/utils/case.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/utils/checks.py` & `gapic-generator-1.9.1/gapic/utils/checks.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/utils/code.py` & `gapic-generator-1.9.1/gapic/utils/code.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/utils/doc.py` & `gapic-generator-1.9.1/gapic/utils/doc.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/utils/filename.py` & `gapic-generator-1.9.1/gapic/utils/filename.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/utils/lines.py` & `gapic-generator-1.9.1/gapic/utils/lines.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/utils/options.py` & `gapic-generator-1.9.1/gapic/utils/options.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/utils/reserved_names.py` & `gapic-generator-1.9.1/gapic/utils/reserved_names.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/utils/rst.py` & `gapic-generator-1.9.1/gapic/utils/rst.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/utils/uri_conv.py` & `gapic-generator-1.9.1/gapic/utils/uri_conv.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic/utils/uri_sample.py` & `gapic-generator-1.9.1/gapic/utils/uri_sample.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/gapic_generator.egg-info/PKG-INFO` & `gapic-generator-1.9.1/gapic_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gapic-generator
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google API Client Generator for Python
 Home-page: https://github.com/googleapis/gapic-generator-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `gapic-generator-1.9.0/gapic_generator.egg-info/SOURCES.txt` & `gapic-generator-1.9.1/gapic_generator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
 tests/fragments/google/protobuf/descriptor.proto
 tests/fragments/google/protobuf/struct.proto
 tests/fragments/google/rpc/status.proto
 tests/fragments/google/type/dayofweek.proto
 tests/integration/BUILD.bazel
 tests/integration/cloudasset_grpc_service_config.json
 tests/integration/eventarc_grpc_service_config.json
+tests/integration/eventarc_v1.yaml
 tests/integration/iamcredentials_grpc_service_config.json
 tests/integration/logging_grpc_service_config.json
 tests/integration/redis_grpc_service_config.json
 tests/integration/goldens/asset/.coveragerc
 tests/integration/goldens/asset/.flake8
 tests/integration/goldens/asset/BUILD.bazel
 tests/integration/goldens/asset/MANIFEST.in
```

### Comparing `gapic-generator-1.9.0/setup.py` & `gapic-generator-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import os
 
 import setuptools
 
 name = "gapic-generator"
 description = "Google API Client Generator for Python"
 url = "https://github.com/googleapis/gapic-generator-python"
-version = "1.9.0"
+version = "1.9.1"
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     "click >= 6.7",
     "google-api-core >= 2.8.0",
     "googleapis-common-protos >= 1.55.0",
     "grpcio >= 1.24.3",
     "jinja2 >= 2.10",
```

### Comparing `gapic-generator-1.9.0/tests/cert/mtls.crt` & `gapic-generator-1.9.1/tests/cert/mtls.crt`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/cert/mtls.key` & `gapic-generator-1.9.1/tests/cert/mtls.key`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/google/api/annotations.proto` & `gapic-generator-1.9.1/tests/fragments/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/google/api/client.proto` & `gapic-generator-1.9.1/tests/fragments/google/api/client.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/google/api/field_behavior.proto` & `gapic-generator-1.9.1/tests/fragments/google/api/field_behavior.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/google/api/http.proto` & `gapic-generator-1.9.1/tests/fragments/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/google/api/routing.proto` & `gapic-generator-1.9.1/tests/fragments/google/api/routing.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/google/cloud/extended_operations.proto` & `gapic-generator-1.9.1/tests/fragments/google/cloud/extended_operations.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/google/longrunning/operations.proto` & `gapic-generator-1.9.1/tests/fragments/google/longrunning/operations.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/google/protobuf/any.proto` & `gapic-generator-1.9.1/tests/fragments/google/protobuf/any.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/google/protobuf/descriptor.proto` & `gapic-generator-1.9.1/tests/fragments/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/google/protobuf/struct.proto` & `gapic-generator-1.9.1/tests/fragments/google/protobuf/struct.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/google/rpc/status.proto` & `gapic-generator-1.9.1/tests/fragments/google/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/google/type/dayofweek.proto` & `gapic-generator-1.9.1/tests/fragments/google/type/dayofweek.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/import.proto` & `gapic-generator-1.9.1/tests/fragments/import.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/test_dynamic_routing.proto` & `gapic-generator-1.9.1/tests/fragments/test_dynamic_routing.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/test_enum_indexed_types.proto` & `gapic-generator-1.9.1/tests/fragments/test_enum_indexed_types.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/test_enum_indexed_types_nonlocal.proto` & `gapic-generator-1.9.1/tests/fragments/test_enum_indexed_types_nonlocal.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/test_extended_operation_forwardcompat_lro.proto` & `gapic-generator-1.9.1/tests/fragments/test_extended_operation_forwardcompat_lro.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/test_flattened_value.proto` & `gapic-generator-1.9.1/tests/fragments/test_flattened_value.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/test_keyword_import.proto` & `gapic-generator-1.9.1/tests/fragments/test_keyword_import.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/test_multiple_required_fields.proto` & `gapic-generator-1.9.1/tests/fragments/test_multiple_required_fields.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/test_non_primitive_body.proto` & `gapic-generator-1.9.1/tests/fragments/test_non_primitive_body.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/test_optional_signature.proto` & `gapic-generator-1.9.1/tests/fragments/test_optional_signature.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/test_recursive_messages.proto` & `gapic-generator-1.9.1/tests/fragments/test_recursive_messages.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/test_repeated_double.proto` & `gapic-generator-1.9.1/tests/fragments/test_repeated_double.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/test_required_non_string.proto` & `gapic-generator-1.9.1/tests/fragments/test_required_non_string.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/test_reserved_field_name.proto` & `gapic-generator-1.9.1/tests/fragments/test_reserved_field_name.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/test_reserved_method_names.proto` & `gapic-generator-1.9.1/tests/fragments/test_reserved_method_names.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/fragments/test_rest_streaming.proto` & `gapic-generator-1.9.1/tests/fragments/test_rest_streaming.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/BUILD.bazel` & `gapic-generator-1.9.1/tests/integration/BUILD.bazel`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,19 @@
     "py_gapic_assembly_pkg",
 )
 load(
     "@gapic_generator_python//rules_python_gapic/test:integration_test.bzl",
     "golden_update",
     "integration_test",
 )
+load(
+    "@com_github_grpc_grpc//bazel:python_rules.bzl",
+    "py_proto_library",
+)
+
 load("@rules_proto//proto:defs.bzl", "proto_library")
 
 package(default_visibility = ["//visibility:public"])
 
 ####################################################
 # Integration Test Rules
 #
@@ -77,25 +82,32 @@
     ],
     legacy_create_init = False,
     deps = [
         ":credentials_py_gapic",
     ],
 )
 
+py_proto_library(
+    name = "iam_policy_py_proto",
+    deps = ["@com_google_googleapis//google/iam/v1:iam_policy_proto"],
+)
+
 # Eventarc.
 py_gapic_library(
     name = "eventarc_py_gapic",
     srcs = ["@com_google_googleapis//google/cloud/eventarc/v1:eventarc_proto"],
     grpc_service_config = "eventarc_grpc_service_config.json",
     opt_args = [
         "python-gapic-namespace=google.cloud",
         "python-gapic-name=eventarc",
         "autogen-snippets",
     ],
+    service_yaml = "eventarc_v1.yaml",
     transport = "grpc+rest",
+    deps = [":iam_policy_py_proto"]
 )
 
 py_test(
     name = "eventarc_py_gapic_test",
     srcs = [
         "eventarc_py_gapic_pytest.py",
         "eventarc_py_gapic_test.py",
```

### Comparing `gapic-generator-1.9.0/tests/integration/cloudasset_grpc_service_config.json` & `gapic-generator-1.9.1/tests/integration/cloudasset_grpc_service_config.json`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/eventarc_grpc_service_config.json` & `gapic-generator-1.9.1/tests/integration/eventarc_grpc_service_config.json`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/.flake8` & `gapic-generator-1.9.1/tests/integration/goldens/asset/.flake8`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/README.rst` & `gapic-generator-1.9.1/tests/integration/goldens/asset/README.rst`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/docs/conf.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset/gapic_version.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset/gapic_version.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/gapic_metadata.json` & `gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/gapic_version.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/gapic_version.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/async_client.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/async_client.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/client.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/client.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/pagers.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/pagers.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/base.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/grpc.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/grpc_asyncio.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/rest.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/services/asset_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -496,15 +496,14 @@
                 ) -> asset_service.AnalyzeIamPolicyResponse:
             r"""Call the analyze iam policy method over HTTP.
 
             Args:
                 request (~.asset_service.AnalyzeIamPolicyRequest):
                     The request object. A request message for
                 [AssetService.AnalyzeIamPolicy][google.cloud.asset.v1.AssetService.AnalyzeIamPolicy].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -577,15 +576,14 @@
             r"""Call the analyze iam policy
         longrunning method over HTTP.
 
             Args:
                 request (~.asset_service.AnalyzeIamPolicyLongrunningRequest):
                     The request object. A request message for
                 [AssetService.AnalyzeIamPolicyLongrunning][google.cloud.asset.v1.AssetService.AnalyzeIamPolicyLongrunning].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
```

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/types/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/types/asset_service.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/types/asset_service.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/google/cloud/asset_v1/types/assets.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/google/cloud/asset_v1/types/assets.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/noxfile.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/noxfile.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_analyze_iam_policy_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_analyze_iam_policy_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_analyze_iam_policy_longrunning_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_analyze_iam_policy_longrunning_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_analyze_iam_policy_longrunning_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_analyze_iam_policy_longrunning_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_analyze_iam_policy_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_analyze_iam_policy_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_batch_get_assets_history_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_batch_get_assets_history_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_batch_get_assets_history_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_batch_get_assets_history_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_create_feed_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_create_feed_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_create_feed_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_create_feed_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_delete_feed_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_delete_feed_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_delete_feed_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_delete_feed_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_export_assets_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_export_assets_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_export_assets_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_export_assets_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_get_feed_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_get_feed_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_get_feed_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_get_feed_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_list_assets_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_list_assets_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_list_assets_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_list_assets_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_list_feeds_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_list_feeds_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_list_feeds_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_list_feeds_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_search_all_iam_policies_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_search_all_iam_policies_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_search_all_iam_policies_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_search_all_iam_policies_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_search_all_resources_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_search_all_resources_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_search_all_resources_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_search_all_resources_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_update_feed_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_update_feed_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_update_feed_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/cloudasset_v1_generated_asset_service_update_feed_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/samples/generated_samples/snippet_metadata_google.cloud.asset.v1.json` & `gapic-generator-1.9.1/tests/integration/goldens/asset/samples/generated_samples/snippet_metadata_google.cloud.asset.v1.json`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/scripts/fixup_asset_v1_keywords.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/scripts/fixup_asset_v1_keywords.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/setup.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/setup.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/tests/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/tests/unit/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/tests/unit/gapic/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/tests/unit/gapic/asset_v1/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/tests/unit/gapic/asset_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/asset/tests/unit/gapic/asset_v1/test_asset_service.py` & `gapic-generator-1.9.1/tests/integration/goldens/asset/tests/unit/gapic/asset_v1/test_asset_service.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/.flake8` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/.flake8`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/README.rst` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/README.rst`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/docs/conf.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials/gapic_version.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials/gapic_version.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/gapic_metadata.json` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/gapic_version.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/gapic_version.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/async_client.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/async_client.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/client.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/client.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/base.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/base.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/grpc.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/grpc_asyncio.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/rest.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/services/iam_credentials/transports/rest.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/types/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/types/common.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/types/common.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/google/iam/credentials_v1/types/iamcredentials.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/google/iam/credentials_v1/types/iamcredentials.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/noxfile.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/noxfile.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_generate_access_token_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_generate_access_token_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_generate_access_token_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_generate_access_token_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_generate_id_token_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_generate_id_token_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_generate_id_token_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_generate_id_token_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_sign_blob_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_sign_blob_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_sign_blob_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_sign_blob_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_sign_jwt_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_sign_jwt_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_sign_jwt_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/samples/generated_samples/iamcredentials_v1_generated_iam_credentials_sign_jwt_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/samples/generated_samples/snippet_metadata_google.iam.credentials.v1.json` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/samples/generated_samples/snippet_metadata_google.iam.credentials.v1.json`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/scripts/fixup_credentials_v1_keywords.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/scripts/fixup_credentials_v1_keywords.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/setup.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/setup.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/tests/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/tests/unit/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/tests/unit/gapic/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/tests/unit/gapic/credentials_v1/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/tests/unit/gapic/credentials_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/credentials/tests/unit/gapic/credentials_v1/test_iam_credentials.py` & `gapic-generator-1.9.1/tests/integration/goldens/credentials/tests/unit/gapic/credentials_v1/test_iam_credentials.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/.flake8` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/.flake8`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/README.rst` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/README.rst`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/docs/conf.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc/gapic_version.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc/gapic_version.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/gapic_metadata.json` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/gapic_version.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/gapic_version.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/async_client.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 from google.cloud.eventarc_v1.services.eventarc import pagers
 from google.cloud.eventarc_v1.types import eventarc
 from google.cloud.eventarc_v1.types import trigger
 from google.cloud.eventarc_v1.types import trigger as gce_trigger
+from google.cloud.location import locations_pb2 # type: ignore
+from google.iam.v1 import iam_policy_pb2  # type: ignore
+from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from .transports.base import EventarcTransport, DEFAULT_CLIENT_INFO
 from .transports.grpc_asyncio import EventarcGrpcAsyncIOTransport
 from .client import EventarcClient
```

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/client.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 from google.cloud.eventarc_v1.services.eventarc import pagers
 from google.cloud.eventarc_v1.types import eventarc
 from google.cloud.eventarc_v1.types import trigger
 from google.cloud.eventarc_v1.types import trigger as gce_trigger
+from google.cloud.location import locations_pb2 # type: ignore
+from google.iam.v1 import iam_policy_pb2  # type: ignore
+from google.iam.v1 import policy_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from .transports.base import EventarcTransport, DEFAULT_CLIENT_INFO
 from .transports.grpc import EventarcGrpcTransport
 from .transports.grpc_asyncio import EventarcGrpcAsyncIOTransport
 from .transports.rest import EventarcRestTransport
 
@@ -1049,13 +1052,16 @@
 
 
 
 
 
 
 
+
+
+
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(gapic_version=package_version.__version__)
 
 
 __all__ = (
     "EventarcClient",
 )
```

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/pagers.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/pagers.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/base.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 from google.api_core import retry as retries
 from google.api_core import operations_v1
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account # type: ignore
 
 from google.cloud.eventarc_v1.types import eventarc
 from google.cloud.eventarc_v1.types import trigger
+from google.cloud.location import locations_pb2 # type: ignore
+from google.iam.v1 import iam_policy_pb2  # type: ignore
+from google.iam.v1 import policy_pb2  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(gapic_version=package_version.__version__)
 
 
 class EventarcTransport(abc.ABC):
     """Abstract transport class for Eventarc."""
```

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/grpc.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc  # type: ignore
 
 from google.cloud.eventarc_v1.types import eventarc
 from google.cloud.eventarc_v1.types import trigger
+from google.cloud.location import locations_pb2 # type: ignore
+from google.iam.v1 import iam_policy_pb2  # type: ignore
+from google.iam.v1 import policy_pb2  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 from .base import EventarcTransport, DEFAULT_CLIENT_INFO
 
 
 class EventarcGrpcTransport(EventarcTransport):
     """gRPC backend transport for Eventarc.
```

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/grpc_asyncio.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 
 import grpc                        # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.cloud.eventarc_v1.types import eventarc
 from google.cloud.eventarc_v1.types import trigger
+from google.cloud.location import locations_pb2 # type: ignore
+from google.iam.v1 import iam_policy_pb2  # type: ignore
+from google.iam.v1 import policy_pb2  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 from .base import EventarcTransport, DEFAULT_CLIENT_INFO
 from .grpc import EventarcGrpcTransport
 
 
 class EventarcGrpcAsyncIOTransport(EventarcTransport):
     """gRPC AsyncIO backend transport for Eventarc.
```

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/rest.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/services/eventarc/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 from google.api_core import rest_helpers
 from google.api_core import rest_streaming
 from google.api_core import path_template
 from google.api_core import gapic_v1
 
 from google.protobuf import json_format
 from google.api_core import operations_v1
+from google.iam.v1 import iam_policy_pb2  # type: ignore
+from google.iam.v1 import policy_pb2  # type: ignore
+from google.cloud.location import locations_pb2 # type: ignore
 from requests import __version__ as requests_version
 import dataclasses
 import re
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
 import warnings
 
 try:
@@ -342,15 +345,14 @@
                 ) -> operations_pb2.Operation:
             r"""Call the create trigger method over HTTP.
 
             Args:
                 request (~.eventarc.CreateTriggerRequest):
                     The request object. The request message for the
                 CreateTrigger method.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -430,15 +432,14 @@
                 ) -> operations_pb2.Operation:
             r"""Call the delete trigger method over HTTP.
 
             Args:
                 request (~.eventarc.DeleteTriggerRequest):
                     The request object. The request message for the
                 DeleteTrigger method.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -509,15 +510,14 @@
                 ) -> trigger.Trigger:
             r"""Call the get trigger method over HTTP.
 
             Args:
                 request (~.eventarc.GetTriggerRequest):
                     The request object. The request message for the
                 GetTrigger method.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -589,15 +589,14 @@
                 ) -> eventarc.ListTriggersResponse:
             r"""Call the list triggers method over HTTP.
 
             Args:
                 request (~.eventarc.ListTriggersRequest):
                     The request object. The request message for the
                 ListTriggers method.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -669,15 +668,14 @@
                 ) -> operations_pb2.Operation:
             r"""Call the update trigger method over HTTP.
 
             Args:
                 request (~.eventarc.UpdateTriggerRequest):
                     The request object. The request message for the
                 UpdateTrigger method.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
```

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/types/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/types/eventarc.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/types/eventarc.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/types/trigger.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/google/cloud/eventarc_v1/types/trigger.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/noxfile.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/noxfile.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_create_trigger_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_create_trigger_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_create_trigger_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_create_trigger_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_delete_trigger_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_delete_trigger_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_delete_trigger_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_delete_trigger_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_get_trigger_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_get_trigger_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_get_trigger_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_get_trigger_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_list_triggers_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_list_triggers_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_list_triggers_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_list_triggers_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_update_trigger_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_update_trigger_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_update_trigger_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/eventarc_v1_generated_eventarc_update_trigger_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/samples/generated_samples/snippet_metadata_google.cloud.eventarc.v1.json` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/samples/generated_samples/snippet_metadata_google.cloud.eventarc.v1.json`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/scripts/fixup_eventarc_v1_keywords.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/scripts/fixup_eventarc_v1_keywords.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/setup.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,36 +16,36 @@
 import io
 import os
 
 import setuptools # type: ignore
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
-name = 'google-cloud-eventarc'
+name = 'google-cloud-redis'
 
 
-description = "Google Cloud Eventarc API client library"
+description = "Google Cloud Redis API client library"
 
 version = {}
-with open(os.path.join(package_root, 'google/cloud/eventarc/gapic_version.py')) as fp:
+with open(os.path.join(package_root, 'google/cloud/redis/gapic_version.py')) as fp:
     exec(fp.read(), version)
 version = version["__version__"]
 
 if version[0] == "0":
     release_status = "Development Status :: 4 - Beta"
 else:
     release_status = "Development Status :: 5 - Production/Stable"
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-eventarc"
+url = "https://github.com/googleapis/python-redis"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/tests/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/tests/unit/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/tests/unit/gapic/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/tests/unit/gapic/eventarc_v1/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/tests/unit/gapic/eventarc_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/eventarc/tests/unit/gapic/eventarc_v1/test_eventarc.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/tests/unit/gapic/eventarc_v1/test_eventarc.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 from google.cloud.eventarc_v1.services.eventarc import EventarcAsyncClient
 from google.cloud.eventarc_v1.services.eventarc import EventarcClient
 from google.cloud.eventarc_v1.services.eventarc import pagers
 from google.cloud.eventarc_v1.services.eventarc import transports
 from google.cloud.eventarc_v1.types import eventarc
 from google.cloud.eventarc_v1.types import trigger
 from google.cloud.eventarc_v1.types import trigger as gce_trigger
+from google.cloud.location import locations_pb2
+from google.iam.v1 import iam_policy_pb2  # type: ignore
+from google.iam.v1 import options_pb2  # type: ignore
+from google.iam.v1 import policy_pb2  # type: ignore
 from google.longrunning import operations_pb2
 from google.oauth2 import service_account
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import google.auth
```

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/.flake8` & `gapic-generator-1.9.1/tests/integration/goldens/logging/.flake8`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/README.rst` & `gapic-generator-1.9.1/tests/integration/goldens/logging/README.rst`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/docs/conf.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging/gapic_version.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging/gapic_version.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/gapic_metadata.json` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/gapic_version.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/gapic_version.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/async_client.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.ListBucketsRequest, dict]]):
-                The request object. The parameters to `ListBuckets`.
+                The request object. The parameters to ``ListBuckets``.
             parent (:class:`str`):
                 Required. The parent resource whose buckets are to be
                 listed:
 
                 ::
 
                     "projects/[PROJECT_ID]/locations/[LOCATION_ID]"
@@ -350,15 +350,15 @@
                 response = await client.get_bucket(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.GetBucketRequest, dict]]):
-                The request object. The parameters to `GetBucket`.
+                The request object. The parameters to ``GetBucket``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -431,15 +431,15 @@
                 response = await client.create_bucket(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.CreateBucketRequest, dict]]):
-                The request object. The parameters to `CreateBucket`.
+                The request object. The parameters to ``CreateBucket``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -519,15 +519,15 @@
                 response = await client.update_bucket(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.UpdateBucketRequest, dict]]):
-                The request object. The parameters to `UpdateBucket`.
+                The request object. The parameters to ``UpdateBucket``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -596,15 +596,15 @@
                 )
 
                 # Make the request
                 await client.delete_bucket(request=request)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.DeleteBucketRequest, dict]]):
-                The request object. The parameters to `DeleteBucket`.
+                The request object. The parameters to ``DeleteBucket``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
@@ -665,15 +665,15 @@
                 )
 
                 # Make the request
                 await client.undelete_bucket(request=request)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.UndeleteBucketRequest, dict]]):
-                The request object. The parameters to `UndeleteBucket`.
+                The request object. The parameters to ``UndeleteBucket``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
@@ -738,15 +738,15 @@
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.ListViewsRequest, dict]]):
-                The request object. The parameters to `ListViews`.
+                The request object. The parameters to ``ListViews``.
             parent (:class:`str`):
                 Required. The bucket whose views are to be listed:
 
                 ::
 
                     "projects/[PROJECT_ID]/locations/[LOCATION_ID]/buckets/[BUCKET_ID]"
 
@@ -851,15 +851,15 @@
                 response = await client.get_view(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.GetViewRequest, dict]]):
-                The request object. The parameters to `GetView`.
+                The request object. The parameters to ``GetView``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -933,15 +933,15 @@
                 response = await client.create_view(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.CreateViewRequest, dict]]):
-                The request object. The parameters to `CreateView`.
+                The request object. The parameters to ``CreateView``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -1014,15 +1014,15 @@
                 response = await client.update_view(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.UpdateViewRequest, dict]]):
-                The request object. The parameters to `UpdateView`.
+                The request object. The parameters to ``UpdateView``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -1091,15 +1091,15 @@
                 )
 
                 # Make the request
                 await client.delete_view(request=request)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.DeleteViewRequest, dict]]):
-                The request object. The parameters to `DeleteView`.
+                The request object. The parameters to ``DeleteView``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
@@ -1164,15 +1164,15 @@
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.ListSinksRequest, dict]]):
-                The request object. The parameters to `ListSinks`.
+                The request object. The parameters to ``ListSinks``.
             parent (:class:`str`):
                 Required. The parent resource whose sinks are to be
                 listed:
 
                 ::
 
                     "projects/[PROJECT_ID]"
@@ -1290,15 +1290,15 @@
                 response = await client.get_sink(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.GetSinkRequest, dict]]):
-                The request object. The parameters to `GetSink`.
+                The request object. The parameters to ``GetSink``.
             sink_name (:class:`str`):
                 Required. The resource name of the sink:
 
                 ::
 
                     "projects/[PROJECT_ID]/sinks/[SINK_ID]"
                     "organizations/[ORGANIZATION_ID]/sinks/[SINK_ID]"
@@ -1423,15 +1423,15 @@
                 response = await client.create_sink(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.CreateSinkRequest, dict]]):
-                The request object. The parameters to `CreateSink`.
+                The request object. The parameters to ``CreateSink``.
             parent (:class:`str`):
                 Required. The resource in which to create the sink:
 
                 ::
 
                     "projects/[PROJECT_ID]"
                     "organizations/[ORGANIZATION_ID]"
@@ -1560,15 +1560,15 @@
                 response = await client.update_sink(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.UpdateSinkRequest, dict]]):
-                The request object. The parameters to `UpdateSink`.
+                The request object. The parameters to ``UpdateSink``.
             sink_name (:class:`str`):
                 Required. The full resource name of the sink to update,
                 including the parent resource and the sink identifier:
 
                 ::
 
                     "projects/[PROJECT_ID]/sinks/[SINK_ID]"
@@ -1713,15 +1713,15 @@
                 )
 
                 # Make the request
                 await client.delete_sink(request=request)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.DeleteSinkRequest, dict]]):
-                The request object. The parameters to `DeleteSink`.
+                The request object. The parameters to ``DeleteSink``.
             sink_name (:class:`str`):
                 Required. The full resource name of the sink to delete,
                 including the parent resource and the sink identifier:
 
                 ::
 
                     "projects/[PROJECT_ID]/sinks/[SINK_ID]"
@@ -1822,15 +1822,15 @@
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.ListExclusionsRequest, dict]]):
-                The request object. The parameters to `ListExclusions`.
+                The request object. The parameters to ``ListExclusions``.
             parent (:class:`str`):
                 Required. The parent resource whose exclusions are to be
                 listed.
 
                 ::
 
                     "projects/[PROJECT_ID]"
@@ -1948,15 +1948,15 @@
                 response = await client.get_exclusion(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.GetExclusionRequest, dict]]):
-                The request object. The parameters to `GetExclusion`.
+                The request object. The parameters to ``GetExclusion``.
             name (:class:`str`):
                 Required. The resource name of an existing exclusion:
 
                 ::
 
                     "projects/[PROJECT_ID]/exclusions/[EXCLUSION_ID]"
                     "organizations/[ORGANIZATION_ID]/exclusions/[EXCLUSION_ID]"
@@ -2083,15 +2083,15 @@
                 response = await client.create_exclusion(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.CreateExclusionRequest, dict]]):
-                The request object. The parameters to `CreateExclusion`.
+                The request object. The parameters to ``CreateExclusion``.
             parent (:class:`str`):
                 Required. The parent resource in which to create the
                 exclusion:
 
                 ::
 
                     "projects/[PROJECT_ID]"
@@ -2220,15 +2220,15 @@
                 response = await client.update_exclusion(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.UpdateExclusionRequest, dict]]):
-                The request object. The parameters to `UpdateExclusion`.
+                The request object. The parameters to ``UpdateExclusion``.
             name (:class:`str`):
                 Required. The resource name of the exclusion to update:
 
                 ::
 
                     "projects/[PROJECT_ID]/exclusions/[EXCLUSION_ID]"
                     "organizations/[ORGANIZATION_ID]/exclusions/[EXCLUSION_ID]"
@@ -2361,15 +2361,15 @@
                 )
 
                 # Make the request
                 await client.delete_exclusion(request=request)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.DeleteExclusionRequest, dict]]):
-                The request object. The parameters to `DeleteExclusion`.
+                The request object. The parameters to ``DeleteExclusion``.
             name (:class:`str`):
                 Required. The resource name of an existing exclusion to
                 delete:
 
                 ::
 
                     "projects/[PROJECT_ID]/exclusions/[EXCLUSION_ID]"
@@ -2479,16 +2479,17 @@
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.GetCmekSettingsRequest, dict]]):
                 The request object. The parameters to
                 [GetCmekSettings][google.logging.v2.ConfigServiceV2.GetCmekSettings].
-                See [Enabling CMEK for Logs
-                Router](https://cloud.google.com/logging/docs/routing/managed-encryption)
+
+                See `Enabling CMEK for Logs
+                Router <https://cloud.google.com/logging/docs/routing/managed-encryption>`__
                 for more information.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
@@ -2587,16 +2588,17 @@
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.UpdateCmekSettingsRequest, dict]]):
                 The request object. The parameters to
                 [UpdateCmekSettings][google.logging.v2.ConfigServiceV2.UpdateCmekSettings].
-                See [Enabling CMEK for Logs
-                Router](https://cloud.google.com/logging/docs/routing/managed-encryption)
+
+                See `Enabling CMEK for Logs
+                Router <https://cloud.google.com/logging/docs/routing/managed-encryption>`__
                 for more information.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
```

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/client.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,15 +459,15 @@
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.ListBucketsRequest, dict]):
-                The request object. The parameters to `ListBuckets`.
+                The request object. The parameters to ``ListBuckets``.
             parent (str):
                 Required. The parent resource whose buckets are to be
                 listed:
 
                 ::
 
                     "projects/[PROJECT_ID]/locations/[LOCATION_ID]"
@@ -580,15 +580,15 @@
                 response = client.get_bucket(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.GetBucketRequest, dict]):
-                The request object. The parameters to `GetBucket`.
+                The request object. The parameters to ``GetBucket``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -662,15 +662,15 @@
                 response = client.create_bucket(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.CreateBucketRequest, dict]):
-                The request object. The parameters to `CreateBucket`.
+                The request object. The parameters to ``CreateBucket``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -751,15 +751,15 @@
                 response = client.update_bucket(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.UpdateBucketRequest, dict]):
-                The request object. The parameters to `UpdateBucket`.
+                The request object. The parameters to ``UpdateBucket``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -829,15 +829,15 @@
                 )
 
                 # Make the request
                 client.delete_bucket(request=request)
 
         Args:
             request (Union[google.cloud.logging_v2.types.DeleteBucketRequest, dict]):
-                The request object. The parameters to `DeleteBucket`.
+                The request object. The parameters to ``DeleteBucket``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
@@ -899,15 +899,15 @@
                 )
 
                 # Make the request
                 client.undelete_bucket(request=request)
 
         Args:
             request (Union[google.cloud.logging_v2.types.UndeleteBucketRequest, dict]):
-                The request object. The parameters to `UndeleteBucket`.
+                The request object. The parameters to ``UndeleteBucket``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
@@ -973,15 +973,15 @@
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.ListViewsRequest, dict]):
-                The request object. The parameters to `ListViews`.
+                The request object. The parameters to ``ListViews``.
             parent (str):
                 Required. The bucket whose views are to be listed:
 
                 ::
 
                     "projects/[PROJECT_ID]/locations/[LOCATION_ID]/buckets/[BUCKET_ID]"
 
@@ -1086,15 +1086,15 @@
                 response = client.get_view(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.GetViewRequest, dict]):
-                The request object. The parameters to `GetView`.
+                The request object. The parameters to ``GetView``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -1169,15 +1169,15 @@
                 response = client.create_view(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.CreateViewRequest, dict]):
-                The request object. The parameters to `CreateView`.
+                The request object. The parameters to ``CreateView``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -1251,15 +1251,15 @@
                 response = client.update_view(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.UpdateViewRequest, dict]):
-                The request object. The parameters to `UpdateView`.
+                The request object. The parameters to ``UpdateView``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
@@ -1329,15 +1329,15 @@
                 )
 
                 # Make the request
                 client.delete_view(request=request)
 
         Args:
             request (Union[google.cloud.logging_v2.types.DeleteViewRequest, dict]):
-                The request object. The parameters to `DeleteView`.
+                The request object. The parameters to ``DeleteView``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
@@ -1403,15 +1403,15 @@
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.ListSinksRequest, dict]):
-                The request object. The parameters to `ListSinks`.
+                The request object. The parameters to ``ListSinks``.
             parent (str):
                 Required. The parent resource whose sinks are to be
                 listed:
 
                 ::
 
                     "projects/[PROJECT_ID]"
@@ -1521,15 +1521,15 @@
                 response = client.get_sink(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.GetSinkRequest, dict]):
-                The request object. The parameters to `GetSink`.
+                The request object. The parameters to ``GetSink``.
             sink_name (str):
                 Required. The resource name of the sink:
 
                 ::
 
                     "projects/[PROJECT_ID]/sinks/[SINK_ID]"
                     "organizations/[ORGANIZATION_ID]/sinks/[SINK_ID]"
@@ -1646,15 +1646,15 @@
                 response = client.create_sink(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.CreateSinkRequest, dict]):
-                The request object. The parameters to `CreateSink`.
+                The request object. The parameters to ``CreateSink``.
             parent (str):
                 Required. The resource in which to create the sink:
 
                 ::
 
                     "projects/[PROJECT_ID]"
                     "organizations/[ORGANIZATION_ID]"
@@ -1783,15 +1783,15 @@
                 response = client.update_sink(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.UpdateSinkRequest, dict]):
-                The request object. The parameters to `UpdateSink`.
+                The request object. The parameters to ``UpdateSink``.
             sink_name (str):
                 Required. The full resource name of the sink to update,
                 including the parent resource and the sink identifier:
 
                 ::
 
                     "projects/[PROJECT_ID]/sinks/[SINK_ID]"
@@ -1928,15 +1928,15 @@
                 )
 
                 # Make the request
                 client.delete_sink(request=request)
 
         Args:
             request (Union[google.cloud.logging_v2.types.DeleteSinkRequest, dict]):
-                The request object. The parameters to `DeleteSink`.
+                The request object. The parameters to ``DeleteSink``.
             sink_name (str):
                 Required. The full resource name of the sink to delete,
                 including the parent resource and the sink identifier:
 
                 ::
 
                     "projects/[PROJECT_ID]/sinks/[SINK_ID]"
@@ -2029,15 +2029,15 @@
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.ListExclusionsRequest, dict]):
-                The request object. The parameters to `ListExclusions`.
+                The request object. The parameters to ``ListExclusions``.
             parent (str):
                 Required. The parent resource whose exclusions are to be
                 listed.
 
                 ::
 
                     "projects/[PROJECT_ID]"
@@ -2147,15 +2147,15 @@
                 response = client.get_exclusion(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.GetExclusionRequest, dict]):
-                The request object. The parameters to `GetExclusion`.
+                The request object. The parameters to ``GetExclusion``.
             name (str):
                 Required. The resource name of an existing exclusion:
 
                 ::
 
                     "projects/[PROJECT_ID]/exclusions/[EXCLUSION_ID]"
                     "organizations/[ORGANIZATION_ID]/exclusions/[EXCLUSION_ID]"
@@ -2274,15 +2274,15 @@
                 response = client.create_exclusion(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.CreateExclusionRequest, dict]):
-                The request object. The parameters to `CreateExclusion`.
+                The request object. The parameters to ``CreateExclusion``.
             parent (str):
                 Required. The parent resource in which to create the
                 exclusion:
 
                 ::
 
                     "projects/[PROJECT_ID]"
@@ -2411,15 +2411,15 @@
                 response = client.update_exclusion(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.UpdateExclusionRequest, dict]):
-                The request object. The parameters to `UpdateExclusion`.
+                The request object. The parameters to ``UpdateExclusion``.
             name (str):
                 Required. The resource name of the exclusion to update:
 
                 ::
 
                     "projects/[PROJECT_ID]/exclusions/[EXCLUSION_ID]"
                     "organizations/[ORGANIZATION_ID]/exclusions/[EXCLUSION_ID]"
@@ -2552,15 +2552,15 @@
                 )
 
                 # Make the request
                 client.delete_exclusion(request=request)
 
         Args:
             request (Union[google.cloud.logging_v2.types.DeleteExclusionRequest, dict]):
-                The request object. The parameters to `DeleteExclusion`.
+                The request object. The parameters to ``DeleteExclusion``.
             name (str):
                 Required. The resource name of an existing exclusion to
                 delete:
 
                 ::
 
                     "projects/[PROJECT_ID]/exclusions/[EXCLUSION_ID]"
@@ -2662,16 +2662,17 @@
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.GetCmekSettingsRequest, dict]):
                 The request object. The parameters to
                 [GetCmekSettings][google.logging.v2.ConfigServiceV2.GetCmekSettings].
-                See [Enabling CMEK for Logs
-                Router](https://cloud.google.com/logging/docs/routing/managed-encryption)
+
+                See `Enabling CMEK for Logs
+                Router <https://cloud.google.com/logging/docs/routing/managed-encryption>`__
                 for more information.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
@@ -2771,16 +2772,17 @@
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.UpdateCmekSettingsRequest, dict]):
                 The request object. The parameters to
                 [UpdateCmekSettings][google.logging.v2.ConfigServiceV2.UpdateCmekSettings].
-                See [Enabling CMEK for Logs
-                Router](https://cloud.google.com/logging/docs/routing/managed-encryption)
+
+                See `Enabling CMEK for Logs
+                Router <https://cloud.google.com/logging/docs/routing/managed-encryption>`__
                 for more information.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
```

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/pagers.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/pagers.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/base.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/base.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/grpc.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/grpc_asyncio.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/rest.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/config_service_v2/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1542,15 +1542,14 @@
                 request (~.logging_config.GetCmekSettingsRequest):
                     The request object. The parameters to
                 [GetCmekSettings][google.logging.v2.ConfigServiceV2.GetCmekSettings].
 
                 See `Enabling CMEK for Logs
                 Router <https://cloud.google.com/logging/docs/routing/managed-encryption>`__
                 for more information.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -2504,15 +2503,14 @@
                 request (~.logging_config.UpdateCmekSettingsRequest):
                     The request object. The parameters to
                 [UpdateCmekSettings][google.logging.v2.ConfigServiceV2.UpdateCmekSettings].
 
                 See `Enabling CMEK for Logs
                 Router <https://cloud.google.com/logging/docs/routing/managed-encryption>`__
                 for more information.
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
```

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/async_client.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -536,15 +536,15 @@
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
             request (Optional[Union[google.cloud.logging_v2.types.ListLogEntriesRequest, dict]]):
-                The request object. The parameters to `ListLogEntries`.
+                The request object. The parameters to ``ListLogEntries``.
             resource_names (:class:`MutableSequence[str]`):
                 Required. Names of one or more parent resources from
                 which to retrieve log entries:
 
                 ::
 
                     "projects/[PROJECT_ID]"
@@ -928,15 +928,15 @@
 
                 # Handle the response
                 async for response in stream:
                     print(response)
 
         Args:
             requests (AsyncIterator[`google.cloud.logging_v2.types.TailLogEntriesRequest`]):
-                The request object AsyncIterator. The parameters to `TailLogEntries`.
+                The request object AsyncIterator. The parameters to ``TailLogEntries``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
```

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/client.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -713,15 +713,15 @@
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.logging_v2.types.ListLogEntriesRequest, dict]):
-                The request object. The parameters to `ListLogEntries`.
+                The request object. The parameters to ``ListLogEntries``.
             resource_names (MutableSequence[str]):
                 Required. Names of one or more parent resources from
                 which to retrieve log entries:
 
                 ::
 
                     "projects/[PROJECT_ID]"
@@ -1082,15 +1082,15 @@
 
                 # Handle the response
                 for response in stream:
                     print(response)
 
         Args:
             requests (Iterator[google.cloud.logging_v2.types.TailLogEntriesRequest]):
-                The request object iterator. The parameters to `TailLogEntries`.
+                The request object iterator. The parameters to ``TailLogEntries``.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
```

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/pagers.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/pagers.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/base.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/base.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/grpc.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/grpc_asyncio.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/rest.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/logging_service_v2/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -551,15 +551,14 @@
             r"""Call the list monitored resource
         descriptors method over HTTP.
 
             Args:
                 request (~.logging.ListMonitoredResourceDescriptorsRequest):
                     The request object. The parameters to
                 ListMonitoredResourceDescriptors
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
```

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/async_client.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/async_client.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/client.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/client.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/pagers.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/pagers.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/base.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/base.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/grpc.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/grpc_asyncio.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/rest.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/services/metrics_service_v2/transports/rest.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/types/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/types/log_entry.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/types/log_entry.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/types/logging.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/types/logging.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/types/logging_config.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/types/logging_config.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/google/cloud/logging_v2/types/logging_metrics.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/google/cloud/logging_v2/types/logging_metrics.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/noxfile.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/noxfile.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_bucket_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_bucket_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_bucket_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_bucket_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_exclusion_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_exclusion_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_exclusion_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_exclusion_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_sink_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_sink_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_sink_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_sink_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_view_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_view_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_view_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_create_view_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_bucket_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_bucket_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_bucket_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_bucket_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_exclusion_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_exclusion_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_exclusion_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_exclusion_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_sink_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_sink_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_sink_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_sink_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_view_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_view_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_view_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_delete_view_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_bucket_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_bucket_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_bucket_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_bucket_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_cmek_settings_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_cmek_settings_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_cmek_settings_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_cmek_settings_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_exclusion_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_exclusion_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_exclusion_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_exclusion_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_sink_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_sink_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_sink_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_sink_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_view_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_view_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_view_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_get_view_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_buckets_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_buckets_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_buckets_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_buckets_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_exclusions_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_exclusions_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_exclusions_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_exclusions_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_sinks_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_sinks_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_sinks_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_sinks_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_views_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_views_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_views_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_list_views_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_undelete_bucket_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_undelete_bucket_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_undelete_bucket_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_undelete_bucket_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_bucket_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_bucket_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_bucket_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_bucket_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_cmek_settings_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_cmek_settings_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_cmek_settings_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_cmek_settings_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_exclusion_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_exclusion_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_exclusion_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_exclusion_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_sink_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_sink_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_sink_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_sink_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_view_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_view_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_view_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_config_service_v2_update_view_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_delete_log_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_delete_log_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_delete_log_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_delete_log_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_log_entries_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_log_entries_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_log_entries_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_log_entries_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_logs_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_logs_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_logs_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_logs_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_monitored_resource_descriptors_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_monitored_resource_descriptors_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_monitored_resource_descriptors_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_list_monitored_resource_descriptors_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_tail_log_entries_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_tail_log_entries_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_tail_log_entries_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_tail_log_entries_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_write_log_entries_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_write_log_entries_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_write_log_entries_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_logging_service_v2_write_log_entries_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_create_log_metric_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_create_log_metric_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_create_log_metric_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_create_log_metric_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_delete_log_metric_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_delete_log_metric_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_delete_log_metric_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_delete_log_metric_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_get_log_metric_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_get_log_metric_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_get_log_metric_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_get_log_metric_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_list_log_metrics_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_list_log_metrics_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_list_log_metrics_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_list_log_metrics_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_update_log_metric_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_update_log_metric_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_update_log_metric_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/logging_v2_generated_metrics_service_v2_update_log_metric_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/samples/generated_samples/snippet_metadata_google.logging.v2.json` & `gapic-generator-1.9.1/tests/integration/goldens/logging/samples/generated_samples/snippet_metadata_google.logging.v2.json`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/scripts/fixup_logging_v2_keywords.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/scripts/fixup_logging_v2_keywords.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/setup.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/setup.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/tests/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/tests/unit/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/tests/unit/gapic/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/tests/unit/gapic/logging_v2/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/tests/unit/gapic/logging_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/tests/unit/gapic/logging_v2/test_config_service_v2.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/tests/unit/gapic/logging_v2/test_config_service_v2.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/tests/unit/gapic/logging_v2/test_logging_service_v2.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/tests/unit/gapic/logging_v2/test_logging_service_v2.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/logging/tests/unit/gapic/logging_v2/test_metrics_service_v2.py` & `gapic-generator-1.9.1/tests/integration/goldens/logging/tests/unit/gapic/logging_v2/test_metrics_service_v2.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/.flake8` & `gapic-generator-1.9.1/tests/integration/goldens/redis/.flake8`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/README.rst` & `gapic-generator-1.9.1/tests/integration/goldens/redis/README.rst`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/docs/conf.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis/gapic_version.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis/gapic_version.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/gapic_metadata.json` & `gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/gapic_version.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/gapic_version.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/async_client.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/async_client.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/client.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/client.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/pagers.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/pagers.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/base.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/base.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/grpc.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/grpc_asyncio.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/rest.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/services/cloud_redis/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,15 +455,14 @@
                 ) -> operations_pb2.Operation:
             r"""Call the create instance method over HTTP.
 
             Args:
                 request (~.cloud_redis.CreateInstanceRequest):
                     The request object. Request for
                 [CreateInstance][google.cloud.redis.v1.CloudRedis.CreateInstance].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -543,15 +542,14 @@
                 ) -> operations_pb2.Operation:
             r"""Call the delete instance method over HTTP.
 
             Args:
                 request (~.cloud_redis.DeleteInstanceRequest):
                     The request object. Request for
                 [DeleteInstance][google.cloud.redis.v1.CloudRedis.DeleteInstance].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -622,15 +620,14 @@
                 ) -> operations_pb2.Operation:
             r"""Call the export instance method over HTTP.
 
             Args:
                 request (~.cloud_redis.ExportInstanceRequest):
                     The request object. Request for
                 [Export][google.cloud.redis.v1.CloudRedis.ExportInstance].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -710,15 +707,14 @@
                 ) -> operations_pb2.Operation:
             r"""Call the failover instance method over HTTP.
 
             Args:
                 request (~.cloud_redis.FailoverInstanceRequest):
                     The request object. Request for
                 [Failover][google.cloud.redis.v1.CloudRedis.FailoverInstance].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -798,15 +794,14 @@
                 ) -> cloud_redis.Instance:
             r"""Call the get instance method over HTTP.
 
             Args:
                 request (~.cloud_redis.GetInstanceRequest):
                     The request object. Request for
                 [GetInstance][google.cloud.redis.v1.CloudRedis.GetInstance].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -876,15 +871,14 @@
                 ) -> operations_pb2.Operation:
             r"""Call the import instance method over HTTP.
 
             Args:
                 request (~.cloud_redis.ImportInstanceRequest):
                     The request object. Request for
                 [Import][google.cloud.redis.v1.CloudRedis.ImportInstance].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -964,15 +958,14 @@
                 ) -> cloud_redis.ListInstancesResponse:
             r"""Call the list instances method over HTTP.
 
             Args:
                 request (~.cloud_redis.ListInstancesRequest):
                     The request object. Request for
                 [ListInstances][google.cloud.redis.v1.CloudRedis.ListInstances].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1044,15 +1037,14 @@
                 ) -> operations_pb2.Operation:
             r"""Call the update instance method over HTTP.
 
             Args:
                 request (~.cloud_redis.UpdateInstanceRequest):
                     The request object. Request for
                 [UpdateInstance][google.cloud.redis.v1.CloudRedis.UpdateInstance].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1132,15 +1124,14 @@
                 ) -> operations_pb2.Operation:
             r"""Call the upgrade instance method over HTTP.
 
             Args:
                 request (~.cloud_redis.UpgradeInstanceRequest):
                     The request object. Request for
                 [UpgradeInstance][google.cloud.redis.v1.CloudRedis.UpgradeInstance].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
```

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/types/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/google/cloud/redis_v1/types/cloud_redis.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/google/cloud/redis_v1/types/cloud_redis.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/noxfile.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/noxfile.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_create_instance_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_create_instance_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_create_instance_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_create_instance_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_delete_instance_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_delete_instance_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_delete_instance_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_delete_instance_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_export_instance_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_export_instance_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_export_instance_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_export_instance_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_failover_instance_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_failover_instance_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_failover_instance_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_failover_instance_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_get_instance_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_get_instance_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_get_instance_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_get_instance_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_import_instance_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_import_instance_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_import_instance_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_import_instance_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_list_instances_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_list_instances_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_list_instances_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_list_instances_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_update_instance_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_update_instance_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_update_instance_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_update_instance_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_upgrade_instance_async.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_upgrade_instance_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_upgrade_instance_sync.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/redis_v1_generated_cloud_redis_upgrade_instance_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/samples/generated_samples/snippet_metadata_google.cloud.redis.v1.json` & `gapic-generator-1.9.1/tests/integration/goldens/redis/samples/generated_samples/snippet_metadata_google.cloud.redis.v1.json`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/scripts/fixup_redis_v1_keywords.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/scripts/fixup_redis_v1_keywords.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/setup.py` & `gapic-generator-1.9.1/tests/integration/goldens/eventarc/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,36 +16,37 @@
 import io
 import os
 
 import setuptools # type: ignore
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
-name = 'google-cloud-redis'
+name = 'google-cloud-eventarc'
 
 
-description = "Google Cloud Redis API client library"
+description = "Google Cloud Eventarc API client library"
 
 version = {}
-with open(os.path.join(package_root, 'google/cloud/redis/gapic_version.py')) as fp:
+with open(os.path.join(package_root, 'google/cloud/eventarc/gapic_version.py')) as fp:
     exec(fp.read(), version)
 version = version["__version__"]
 
 if version[0] == "0":
     release_status = "Development Status :: 4 - Beta"
 else:
     release_status = "Development Status :: 5 - Production/Stable"
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
+    "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
-url = "https://github.com/googleapis/python-redis"
+url = "https://github.com/googleapis/python-eventarc"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/tests/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/tests/unit/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/tests/unit/gapic/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/tests/unit/gapic/redis_v1/__init__.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/tests/unit/gapic/redis_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/goldens/redis/tests/unit/gapic/redis_v1/test_cloud_redis.py` & `gapic-generator-1.9.1/tests/integration/goldens/redis/tests/unit/gapic/redis_v1/test_cloud_redis.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/iamcredentials_grpc_service_config.json` & `gapic-generator-1.9.1/tests/integration/iamcredentials_grpc_service_config.json`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/logging_grpc_service_config.json` & `gapic-generator-1.9.1/tests/integration/logging_grpc_service_config.json`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/integration/redis_grpc_service_config.json` & `gapic-generator-1.9.1/tests/integration/redis_grpc_service_config.json`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_list_resources_async.py` & `gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_list_resources_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_list_resources_sync.py` & `gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_list_resources_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_bidi_streaming_async.py` & `gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_bidi_streaming_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_bidi_streaming_sync.py` & `gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_bidi_streaming_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_lro_signatures_async.py` & `gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_lro_signatures_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_lro_signatures_sync.py` & `gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_lro_signatures_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_one_signature_async.py` & `gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_one_signature_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_one_signature_sync.py` & `gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_one_signature_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_server_streaming_async.py` & `gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_server_streaming_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_server_streaming_sync.py` & `gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_method_server_streaming_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_one_of_method_async.py` & `gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_one_of_method_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_one_of_method_required_field_async.py` & `gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_one_of_method_required_field_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_one_of_method_required_field_sync.py` & `gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_one_of_method_required_field_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/snippetgen/goldens/mollusca_v1_generated_snippets_one_of_method_sync.py` & `gapic-generator-1.9.1/tests/snippetgen/goldens/mollusca_v1_generated_snippets_one_of_method_sync.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/snippetgen/goldens/snippet_metadata_mollusca_v1.json` & `gapic-generator-1.9.1/tests/snippetgen/goldens/snippet_metadata_mollusca_v1.json`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/snippetgen/snippets.proto` & `gapic-generator-1.9.1/tests/snippetgen/snippets.proto`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/snippetgen/test_snippetgen.py` & `gapic-generator-1.9.1/tests/snippetgen/test_snippetgen.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/system/conftest.py` & `gapic-generator-1.9.1/tests/system/conftest.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/system/test_client_context_manager.py` & `gapic-generator-1.9.1/tests/system/test_client_context_manager.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/system/test_error_details.py` & `gapic-generator-1.9.1/tests/system/test_error_details.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/system/test_grpc_interceptor_streams.py` & `gapic-generator-1.9.1/tests/system/test_grpc_interceptor_streams.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/system/test_lro.py` & `gapic-generator-1.9.1/tests/system/test_lro.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/system/test_pagination.py` & `gapic-generator-1.9.1/tests/system/test_pagination.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/system/test_resource_crud.py` & `gapic-generator-1.9.1/tests/system/test_resource_crud.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/system/test_retry.py` & `gapic-generator-1.9.1/tests/system/test_retry.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/system/test_streams.py` & `gapic-generator-1.9.1/tests/system/test_streams.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/system/test_unary.py` & `gapic-generator-1.9.1/tests/system/test_unary.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/common_types.py` & `gapic-generator-1.9.1/tests/unit/common_types.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/configurable_snippetgen/resources/README.md` & `gapic-generator-1.9.1/tests/unit/configurable_snippetgen/resources/README.md`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/configurable_snippetgen/resources/speech/request.desc` & `gapic-generator-1.9.1/tests/unit/configurable_snippetgen/resources/speech/request.desc`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/configurable_snippetgen/resources/speech/speech_createCustomClass.json` & `gapic-generator-1.9.1/tests/unit/configurable_snippetgen/resources/speech/speech_createCustomClass.json`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/configurable_snippetgen/resources/speech/speech_v1_generated_adaptation_create_custom_class_basic_async.py` & `gapic-generator-1.9.1/tests/unit/configurable_snippetgen/resources/speech/speech_v1_generated_adaptation_create_custom_class_basic_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/configurable_snippetgen/test_configured_snippet.py` & `gapic-generator-1.9.1/tests/unit/configurable_snippetgen/test_configured_snippet.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/configurable_snippetgen/test_libcst_utils.py` & `gapic-generator-1.9.1/tests/unit/configurable_snippetgen/test_libcst_utils.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/configurable_snippetgen/test_resources.py` & `gapic-generator-1.9.1/tests/unit/configurable_snippetgen/test_resources.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/generator/test_formatter.py` & `gapic-generator-1.9.1/tests/unit/generator/test_formatter.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/generator/test_generator.py` & `gapic-generator-1.9.1/tests/unit/generator/test_generator.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/generator/test_options.py` & `gapic-generator-1.9.1/tests/unit/generator/test_options.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/samplegen/golden_snippets/sample_basic.py` & `gapic-generator-1.9.1/tests/unit/samplegen/golden_snippets/sample_basic.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/samplegen/golden_snippets/sample_basic_async.py` & `gapic-generator-1.9.1/tests/unit/samplegen/golden_snippets/sample_basic_async.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/samplegen/golden_snippets/sample_basic_unflattenable.py` & `gapic-generator-1.9.1/tests/unit/samplegen/golden_snippets/sample_basic_unflattenable.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/samplegen/golden_snippets/sample_basic_void_method.py` & `gapic-generator-1.9.1/tests/unit/samplegen/golden_snippets/sample_basic_void_method.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/samplegen/test_integration.py` & `gapic-generator-1.9.1/tests/unit/samplegen/test_integration.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/samplegen/test_manifest.py` & `gapic-generator-1.9.1/tests/unit/samplegen/test_manifest.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/samplegen/test_samplegen.py` & `gapic-generator-1.9.1/tests/unit/samplegen/test_samplegen.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/samplegen/test_snippet_index.py` & `gapic-generator-1.9.1/tests/unit/samplegen/test_snippet_index.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/samplegen/test_template.py` & `gapic-generator-1.9.1/tests/unit/samplegen/test_template.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/schema/test_api.py` & `gapic-generator-1.9.1/tests/unit/schema/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -730,54 +730,14 @@
         ),
         make_file_pb2(
             name="bab.v1.proto",
             package="google.bab.v1",
             messages=(make_message_pb2(name="ImportedMessageBab", fields=()),),
         ),
         make_file_pb2(
-            name="bac.v10.proto",
-            package="google.bac.v10",
-            messages=(make_message_pb2(name="ImportedMessageBac", fields=()),),
-        ),
-        make_file_pb2(
-            name="bad.v2beta.proto",
-            package="google.bad.v2beta",
-            messages=(make_message_pb2(name="ImportedMessageBad", fields=()),),
-        ),
-        make_file_pb2(
-            name="bae.v2beta20.proto",
-            package="google.bae.v2beta20",
-            messages=(make_message_pb2(name="ImportedMessageBae", fields=()),),
-        ),
-        make_file_pb2(
-            name="baf.v20beta.proto",
-            package="google.baf.v20beta",
-            messages=(make_message_pb2(name="ImportedMessageBaf", fields=()),),
-        ),
-        make_file_pb2(
-            name="bag.v20p1.proto",
-            package="google.bag.v20p1",
-            messages=(make_message_pb2(name="ImportedMessageBag", fields=()),),
-        ),
-        make_file_pb2(
-            name="bah.v20p1alpha3p5.proto",
-            package="google.bah.v20p1alpha3p5",
-            messages=(make_message_pb2(name="ImportedMessageBah", fields=()),),
-        ),
-        make_file_pb2(
-            name="bah.v20p1.bai.proto",
-            package="google.bah.v20p1.bai",
-            messages=(make_message_pb2(name="ImportedMessageBai", fields=()),),
-        ),
-        make_file_pb2(
-            name="bah.v20p1.baj.v3.proto",
-            package="google.bah.v20p1.baj.v3",
-            messages=(make_message_pb2(name="ImportedMessageBaj", fields=()),),
-        ),
-        make_file_pb2(
             name="common.proto",
             package="google.example.v1.common",
             messages=(make_message_pb2(name="Bar"),),
         ),
         make_file_pb2(
             name="foo.proto",
             package="google.example.v1",
@@ -820,94 +780,14 @@
                                 make_field_pb2(
                                     name="imported_message_bab",
                                     number=1,
                                     type_name=".google.bab.v1.ImportedMessageBab",
                                 ),
                             ),
                         ),
-                        make_message_pb2(
-                            name="Bac",
-                            fields=(
-                                make_field_pb2(
-                                    name="imported_message_bac",
-                                    number=1,
-                                    type_name=".google.bac.v10.ImportedMessageBac",
-                                ),
-                            ),
-                        ),
-                        make_message_pb2(
-                            name="Bad",
-                            fields=(
-                                make_field_pb2(
-                                    name="imported_message_bad",
-                                    number=1,
-                                    type_name=".google.bad.v2beta.ImportedMessageBad",
-                                ),
-                            ),
-                        ),
-                        make_message_pb2(
-                            name="Bae",
-                            fields=(
-                                make_field_pb2(
-                                    name="imported_message_bae",
-                                    number=1,
-                                    type_name=".google.bae.v2beta20.ImportedMessageBae",
-                                ),
-                            ),
-                        ),
-                        make_message_pb2(
-                            name="Baf",
-                            fields=(
-                                make_field_pb2(
-                                    name="imported_message_baf",
-                                    number=1,
-                                    type_name=".google.baf.v20beta.ImportedMessageBaf",
-                                ),
-                            ),
-                        ),
-                        make_message_pb2(
-                            name="Bag",
-                            fields=(
-                                make_field_pb2(
-                                    name="imported_message_bag",
-                                    number=1,
-                                    type_name=".google.bag.v20p1.ImportedMessageBag",
-                                ),
-                            ),
-                        ),
-                        make_message_pb2(
-                            name="Bah",
-                            fields=(
-                                make_field_pb2(
-                                    name="imported_message_bah",
-                                    number=1,
-                                    type_name=".google.bah.v20p1alpha3p5.ImportedMessageBah",
-                                ),
-                            ),
-                        ),
-                        make_message_pb2(
-                            name="Bai",
-                            fields=(
-                                make_field_pb2(
-                                    name="imported_message_bai",
-                                    number=1,
-                                    type_name=".google.bah.v20p1.bai.ImportedMessageBai",
-                                ),
-                            ),
-                        ),
-                        make_message_pb2(
-                            name="Baj",
-                            fields=(
-                                make_field_pb2(
-                                    name="imported_message_baj",
-                                    number=1,
-                                    type_name=".google.bah.v20p1.baj.v3.ImportedMessageBaj",
-                                ),
-                            ),
-                        ),
                     ),
                 ),
                 make_message_pb2(
                     name="GetFooResponse",
                     fields=(
                         make_field_pb2(
                             name="foo",
@@ -933,86 +813,55 @@
     )
 
     api_schema = api.API.build(fd, package="google.example.v1")
 
     assert api_schema.protos["foo.proto"].python_modules == (
         imp.Import(package=("google", "baa"), module="baa_pb2"),
         imp.Import(package=("google", "bab", "v1"), module="bab_v1_pb2"),
-        imp.Import(package=("google", "bac", "v10"), module="bac_v10_pb2"),
-        imp.Import(package=("google", "bad", "v2beta"),
-                   module="bad_v2beta_pb2"),
-        imp.Import(package=("google", "bae", "v2beta20"),
-                   module="bae_v2beta20_pb2"),
-        imp.Import(package=("google", "baf", "v20beta"),
-                   module="baf_v20beta_pb2"),
-        imp.Import(package=("google", "bag", "v20p1"), module="bag_v20p1_pb2"),
-        imp.Import(
-            package=("google", "bah", "v20p1", "bai"),
-            module="bah_v20p1_bai_pb2"
-        ),
-        imp.Import(
-            package=("google", "bah", "v20p1", "baj", "v3"),
-            module="bah_v20p1_baj_v3_pb2",
-        ),
-        imp.Import(
-            package=("google", "bah", "v20p1alpha3p5"), module="bah_v20p1alpha3p5_pb2"
-        ),
         imp.Import(package=("google", "dep"), module="dep_pb2"),
     )
+    assert (
+        api_schema.protos["foo.proto"]
+        .all_messages["google.example.v1.GetFooRequest.Bab"]
+        .fields["imported_message_bab"]
+        .ident.sphinx
+        == "google.bab.v1.bab_v1_pb2.ImportedMessageBab"
+    )
 
     # Ensure that we can change the import statements to cater for a
     # dependency that uses proto-plus types.
     # For example,
     # `from google.bar import bar_pb2` becomes `from google.bar.types import bar``
     # `from google.baz.v2 import baz_pb2` becomes `from google.baz_v2.types improt baz_v2`
     api_schema = api.API.build(
         fd,
         package="google.example.v1",
         opts=Options(
             proto_plus_deps="+".join(
                 (
                     "google.baa",
                     "google.bab.v1",
-                    "google.bac.v10",
-                    "google.bad.v2beta",
-                    "google.bae.v2beta20",
-                    "google.baf.v20beta",
-                    "google.bag.v20p1",
-                    "google.bah.v20p1alpha3p5",
-                    "google.bah.v20p1.bai",
-                    "google.bah.v20p1.baj.v3",
                 )
             )
         ),
     )
     assert api_schema.protos["foo.proto"].python_modules == (
         imp.Import(package=("google", "baa", "types"), module="baa"),
         imp.Import(package=("google", "bab_v1", "types"), module="bab_v1"),
-        imp.Import(package=("google", "bac_v10", "types"), module="bac_v10"),
-        imp.Import(package=("google", "bad_v2beta", "types"),
-                   module="bad_v2beta"),
-        imp.Import(package=("google", "bae_v2beta20", "types"),
-                   module="bae_v2beta20"),
-        imp.Import(package=("google", "baf_v20beta", "types"),
-                   module="baf_v20beta"),
-        imp.Import(package=("google", "bag_v20p1", "types"),
-                   module="bag_v20p1"),
-        imp.Import(
-            package=("google", "bah", "v20p1", "bai", "types"), module="bah_v20p1_bai"
-        ),
-        imp.Import(
-            package=("google", "bah", "v20p1", "baj_v3", "types"),
-            module="bah_v20p1_baj_v3",
-        ),
-        imp.Import(
-            package=("google", "bah_v20p1alpha3p5", "types"), module="bah_v20p1alpha3p5"
-        ),
         imp.Import(package=("google", "dep"), module="dep_pb2"),
     )
 
+    assert (
+        api_schema.protos["foo.proto"]
+        .all_messages["google.example.v1.GetFooRequest.Bab"]
+        .fields["imported_message_bab"]
+        .ident.sphinx
+        == "google.bab_v1.types.ImportedMessageBab"
+    )
+
 
 def test_services():
     L = descriptor_pb2.SourceCodeInfo.Location
 
     # Make a silly helper method to not repeat some of the structure.
     def _n(method_name: str):
         return {
@@ -2729,7 +2578,27 @@
     m4.options.Extensions[annotations_pb2.http].post = r4['post']
     m4.options.Extensions[annotations_pb2.http].body = r4['body']
 
     api_schema = api.API.build(fd, 'google.example.v1', opts=opts)
     assert api_schema.mixin_api_methods == {
         'CancelOperation': m1, 'DeleteOperation': m2, 'WaitOperation': m3,
         'GetOperation': m4}
+
+
+def test_has_iam_mixin():
+    # Check that has_iam_mixin() property of API returns True when the
+    # service YAML contains `google.iam.v1.IAMPolicy`.
+    fd = (
+        make_file_pb2(
+            name='example.proto',
+            package='google.example.v1',
+            messages=(make_message_pb2(name='ExampleRequest', fields=()),),
+        ),)
+    opts = Options(service_yaml_config={
+        'apis': [
+            {
+                'name': 'google.iam.v1.IAMPolicy'
+            }
+        ],
+    })
+    api_schema = api.API.build(fd, 'google.example.v1', opts=opts)
+    assert api_schema.has_iam_mixin
```

### Comparing `gapic-generator-1.9.0/tests/unit/schema/test_imp.py` & `gapic-generator-1.9.1/tests/unit/schema/test_imp.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/schema/test_metadata.py` & `gapic-generator-1.9.1/tests/unit/schema/test_metadata.py`

 * *Files 26% similar despite different names*

```diff
@@ -62,14 +62,46 @@
 
 def test_address_proto():
     addr = metadata.Address(package=('foo', 'bar'), module='baz', name='Bacon')
     assert addr.proto == 'foo.bar.Bacon'
     assert addr.proto_package == 'foo.bar'
 
 
+def test_proto_package_version_parsing():
+    addr = metadata.Address(package=("baa"))
+    assert addr.convert_to_versioned_package() == ("baa")
+
+    addr = metadata.Address(package=("bab", "v1"))
+    assert addr.convert_to_versioned_package() == ("bab_v1",)
+
+    addr = metadata.Address(package=("bac", "v10"))
+    assert addr.convert_to_versioned_package() == ("bac_v10",)
+
+    addr = metadata.Address(package=("bad", "v2beta"))
+    assert addr.convert_to_versioned_package() == ("bad_v2beta",)
+
+    addr = metadata.Address(package=("bae", "v2beta20"))
+    assert addr.convert_to_versioned_package() == ("bae_v2beta20",)
+
+    addr = metadata.Address(package=("baf", "v20beta"))
+    assert addr.convert_to_versioned_package() == ("baf_v20beta",)
+
+    addr = metadata.Address(package=("bag", "v20p1"))
+    assert addr.convert_to_versioned_package() == ("bag_v20p1",)
+
+    addr = metadata.Address(package=("bah", "v20p1alpha3p5"))
+    assert addr.convert_to_versioned_package() == ("bah_v20p1alpha3p5",)
+
+    addr = metadata.Address(package=("bai", "v20p1"))
+    assert addr.convert_to_versioned_package() == ("bai_v20p1",)
+
+    addr = metadata.Address(package=("bah", "v20p1", "baj", "v3"))
+    assert addr.convert_to_versioned_package() == ("bah", "v20p1", "baj_v3")
+
+
 def test_address_child_no_parent():
     addr = metadata.Address(package=('foo', 'bar'), module='baz')
     child = addr.child('Bacon', path=(4, 0))
     assert child.name == 'Bacon'
     assert child.parent == ()
     assert child.module_path == (4, 0)
```

### Comparing `gapic-generator-1.9.0/tests/unit/schema/test_naming.py` & `gapic-generator-1.9.1/tests/unit/schema/test_naming.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/schema/wrappers/test_enums.py` & `gapic-generator-1.9.1/tests/unit/schema/wrappers/test_enums.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/schema/wrappers/test_field.py` & `gapic-generator-1.9.1/tests/unit/schema/wrappers/test_field.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/schema/wrappers/test_message.py` & `gapic-generator-1.9.1/tests/unit/schema/wrappers/test_message.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/schema/wrappers/test_method.py` & `gapic-generator-1.9.1/tests/unit/schema/wrappers/test_method.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/schema/wrappers/test_oneof.py` & `gapic-generator-1.9.1/tests/unit/schema/wrappers/test_oneof.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/schema/wrappers/test_python.py` & `gapic-generator-1.9.1/tests/unit/schema/wrappers/test_python.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/schema/wrappers/test_routing.py` & `gapic-generator-1.9.1/tests/unit/schema/wrappers/test_routing.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/schema/wrappers/test_service.py` & `gapic-generator-1.9.1/tests/unit/schema/wrappers/test_service.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/utils/test_cache.py` & `gapic-generator-1.9.1/tests/unit/utils/test_cache.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/utils/test_case.py` & `gapic-generator-1.9.1/tests/unit/utils/test_case.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/utils/test_checks.py` & `gapic-generator-1.9.1/tests/unit/utils/test_checks.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/utils/test_code.py` & `gapic-generator-1.9.1/tests/unit/utils/test_code.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/utils/test_filename.py` & `gapic-generator-1.9.1/tests/unit/utils/test_filename.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/utils/test_lines.py` & `gapic-generator-1.9.1/tests/unit/utils/test_lines.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/utils/test_rst.py` & `gapic-generator-1.9.1/tests/unit/utils/test_rst.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/utils/test_uri_conv.py` & `gapic-generator-1.9.1/tests/unit/utils/test_uri_conv.py`

 * *Files identical despite different names*

### Comparing `gapic-generator-1.9.0/tests/unit/utils/test_uri_sample.py` & `gapic-generator-1.9.1/tests/unit/utils/test_uri_sample.py`

 * *Files identical despite different names*

