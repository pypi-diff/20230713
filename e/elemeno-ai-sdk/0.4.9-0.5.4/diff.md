# Comparing `tmp/elemeno_ai_sdk-0.4.9-py2.py3-none-any.whl.zip` & `tmp/elemeno_ai_sdk-0.5.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,72 +1,68 @@
-Zip file size: 63181 bytes, number of entries: 70
--rw-r--r--  2.0 unx      235 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/__init__.py
--rw-r--r--  2.0 unx      375 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/__main__.py
--rw-r--r--  2.0 unx      935 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/cli.py
--rw-r--r--  2.0 unx     1143 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/config.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/cos/__init__.py
--rw-r--r--  2.0 unx      680 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/cos/base_cos.py
--rw-r--r--  2.0 unx     2279 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/cos/minio.py
--rw-r--r--  2.0 unx     3421 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/cos/s3.py
--rw-r--r--  2.0 unx       32 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/cos/file_utils/__init__.py
--rw-r--r--  2.0 unx    10897 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/cos/file_utils/elastic_to_cos copy.py
--rw-r--r--  2.0 unx     5426 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/cos/file_utils/elastic_to_cos.py
--rw-r--r--  2.0 unx     3408 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/cos/file_utils/elastic_to_cos_dask.py
--rw-r--r--  2.0 unx     1456 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/cos/file_utils/zip_utils.py
--rw-r--r--  2.0 unx       33 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/cos/types/__init__.py
--rw-r--r--  2.0 unx     1424 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/cos/types/cos_object.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/deps/__init__.py
--rw-r--r--  2.0 unx      672 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/deps/git_helper.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/feastproxy/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/feastproxy/feastproxy.py
--rw-r--r--  2.0 unx     2083 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/registry.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/conversion/__init__.py
--rw-r--r--  2.0 unx     1245 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/conversion/converter.py
--rw-r--r--  2.0 unx     1072 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/conversion/converter_abc.py
--rw-r--r--  2.0 unx     1150 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/conversion/sklearn.py
--rw-r--r--  2.0 unx     1271 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/conversion/tensorflow.py
--rw-r--r--  2.0 unx     1425 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/conversion/tflite.py
--rw-r--r--  2.0 unx      940 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/conversion/torch.py
--rw-r--r--  2.0 unx     1072 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/conversion/.ipynb_checkpoints/converter_abc-checkpoint.py
--rw-r--r--  2.0 unx      919 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/conversion/.ipynb_checkpoints/tensorflow-checkpoint.py
--rw-r--r--  2.0 unx      996 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/conversion/.ipynb_checkpoints/tflite-checkpoint.py
--rw-r--r--  2.0 unx      755 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/conversion/.ipynb_checkpoints/torch-checkpoint.py
--rw-r--r--  2.0 unx      245 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/__init__.py
--rw-r--r--  2.0 unx    19542 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/feature_store.py
--rw-r--r--  2.0 unx     6447 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/feature_table.py
--rw-r--r--  2.0 unx      551 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/materialize.py
--rw-r--r--  2.0 unx     3886 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/query.py
--rw-r--r--  2.0 unx     5496 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/types.py
--rw-r--r--  2.0 unx      292 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/ingest/__init_.py
--rw-r--r--  2.0 unx      157 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/ingest/sink/__init__.py
--rw-r--r--  2.0 unx     1997 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/ingest/sink/base_ingestion.py
--rw-r--r--  2.0 unx     5494 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/ingest/sink/bigquery_ingestion.py
--rw-r--r--  2.0 unx      298 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/ingest/sink/file_ingestion.py
--rw-r--r--  2.0 unx     1922 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/ingest/sink/ingestion_sink_builder.py
--rw-r--r--  2.0 unx     5838 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/ingest/sink/minio_ingestion.py
--rw-r--r--  2.0 unx    10380 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/ingest/sink/redshift_ingestion.py
--rw-r--r--  2.0 unx      515 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/ingest/sink/redshift_test_ingestion.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/ingest/source/__init__.py
--rw-r--r--  2.0 unx      528 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/ingest/source/base_source.py
--rw-r--r--  2.0 unx     1854 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/ingest/source/bigquery.py
--rw-r--r--  2.0 unx     6260 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/ingest/source/elastic.py
--rw-r--r--  2.0 unx     1385 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/ingest/source/gcs.py
--rw-r--r--  2.0 unx     4483 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/ingest/source/ingestion_source_builder.py
--rw-r--r--  2.0 unx     2836 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/ingest/source/redshift.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/transform/__init__.py
--rw-r--r--  2.0 unx      901 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/transform/dsl/base_ops.py
--rw-r--r--  2.0 unx       40 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/transform/dsl/functions/__init__.py
--rw-r--r--  2.0 unx     2107 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/features/transform/dsl/functions/change_shape.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/inference/__init__.py
--rw-r--r--  2.0 unx     1424 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/inference/client.py
--rw-r--r--  2.0 unx      457 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/inference/inference_response.py
--rw-r--r--  2.0 unx     1819 b- defN 23-Mar-03 20:14 elemeno_ai_sdk/ml/inference/input_space.py
--rw-r--r--  2.0 unx       66 b- defN 23-Mar-03 20:15 elemeno_ai_sdk-0.4.9.dist-info/AUTHORS.rst
--rw-r--r--  2.0 unx      592 b- defN 23-Mar-03 20:15 elemeno_ai_sdk-0.4.9.dist-info/LICENSE
--rw-r--r--  2.0 unx    15965 b- defN 23-Mar-03 20:15 elemeno_ai_sdk-0.4.9.dist-info/LICENSE-3RDPARTY.txt
--rw-r--r--  2.0 unx     3156 b- defN 23-Mar-03 20:15 elemeno_ai_sdk-0.4.9.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Mar-03 20:15 elemeno_ai_sdk-0.4.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Mar-03 20:14 elemeno_ai_sdk-0.4.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 23-Mar-03 20:14 elemeno_ai_sdk-0.4.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     7018 b- defN 23-Mar-03 20:15 elemeno_ai_sdk-0.4.9.dist-info/RECORD
-70 files, 159473 bytes uncompressed, 51565 bytes compressed:  67.7%
+Zip file size: 63670 bytes, number of entries: 66
+-rw-r--r--  2.0 unx      235 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/__init__.py
+-rw-r--r--  2.0 unx      375 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/__main__.py
+-rw-r--r--  2.0 unx      935 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/cli.py
+-rw-r--r--  2.0 unx     2406 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/config.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/cos/__init__.py
+-rw-r--r--  2.0 unx      680 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/cos/base_cos.py
+-rw-r--r--  2.0 unx     2404 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/cos/minio.py
+-rw-r--r--  2.0 unx     3421 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/cos/s3.py
+-rw-r--r--  2.0 unx       32 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/cos/file_utils/__init__.py
+-rw-r--r--  2.0 unx    10897 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/cos/file_utils/elastic_to_cos copy.py
+-rw-r--r--  2.0 unx     5426 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/cos/file_utils/elastic_to_cos.py
+-rw-r--r--  2.0 unx     3408 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/cos/file_utils/elastic_to_cos_dask.py
+-rw-r--r--  2.0 unx     1456 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/cos/file_utils/zip_utils.py
+-rw-r--r--  2.0 unx       33 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/cos/types/__init__.py
+-rw-r--r--  2.0 unx     1424 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/cos/types/cos_object.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/deps/__init__.py
+-rw-r--r--  2.0 unx      672 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/deps/git_helper.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/feastproxy/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/feastproxy/feastproxy.py
+-rw-r--r--  2.0 unx     2083 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/registry.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/conversion/__init__.py
+-rw-r--r--  2.0 unx     1245 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/conversion/converter.py
+-rw-r--r--  2.0 unx     1072 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/conversion/converter_abc.py
+-rw-r--r--  2.0 unx     1150 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/conversion/sklearn.py
+-rw-r--r--  2.0 unx     1271 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/conversion/tensorflow.py
+-rw-r--r--  2.0 unx     1425 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/conversion/tflite.py
+-rw-r--r--  2.0 unx      940 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/conversion/torch.py
+-rw-r--r--  2.0 unx      245 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/__init__.py
+-rw-r--r--  2.0 unx    27287 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/feature_store.py
+-rw-r--r--  2.0 unx     6550 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/feature_table.py
+-rw-r--r--  2.0 unx     3886 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/query.py
+-rw-r--r--  2.0 unx     5496 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/types.py
+-rw-r--r--  2.0 unx      292 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/utils.py
+-rw-r--r--  2.0 unx     2340 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/config/repo_config.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/ingest/__init_.py
+-rw-r--r--  2.0 unx      210 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/ingest/sink/__init__.py
+-rw-r--r--  2.0 unx     2318 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/ingest/sink/base_ingestion.py
+-rw-r--r--  2.0 unx     6908 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/ingest/sink/bigquery_ingestion.py
+-rw-r--r--  2.0 unx      577 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/ingest/sink/file_ingestion.py
+-rw-r--r--  2.0 unx     1922 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/ingest/sink/ingestion_sink_builder.py
+-rw-r--r--  2.0 unx     9050 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/ingest/sink/minio_ingestion.py
+-rw-r--r--  2.0 unx    10046 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/ingest/sink/redshift_ingestion.py
+-rw-r--r--  2.0 unx      571 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/ingest/sink/redshift_test_ingestion.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/ingest/source/__init__.py
+-rw-r--r--  2.0 unx      535 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/ingest/source/base_source.py
+-rw-r--r--  2.0 unx     1854 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/ingest/source/bigquery.py
+-rw-r--r--  2.0 unx     6280 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/ingest/source/elastic.py
+-rw-r--r--  2.0 unx     1385 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/ingest/source/gcs.py
+-rw-r--r--  2.0 unx     4965 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/ingest/source/ingestion_source_builder.py
+-rw-r--r--  2.0 unx     3594 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/ingest/source/redshift.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/transform/__init__.py
+-rw-r--r--  2.0 unx      901 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/transform/dsl/base_ops.py
+-rw-r--r--  2.0 unx       40 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/transform/dsl/functions/__init__.py
+-rw-r--r--  2.0 unx     2107 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/features/transform/dsl/functions/change_shape.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/inference/__init__.py
+-rw-r--r--  2.0 unx     1424 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/inference/client.py
+-rw-r--r--  2.0 unx      457 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/inference/inference_response.py
+-rw-r--r--  2.0 unx     1819 b- defN 23-Jul-12 23:15 elemeno_ai_sdk/ml/inference/input_space.py
+-rw-r--r--  2.0 unx       66 b- defN 23-Jul-12 23:16 elemeno_ai_sdk-0.5.4.dist-info/AUTHORS.rst
+-rw-r--r--  2.0 unx      592 b- defN 23-Jul-12 23:16 elemeno_ai_sdk-0.5.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    15965 b- defN 23-Jul-12 23:16 elemeno_ai_sdk-0.5.4.dist-info/LICENSE-3RDPARTY.txt
+-rw-r--r--  2.0 unx     3116 b- defN 23-Jul-12 23:16 elemeno_ai_sdk-0.5.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-12 23:16 elemeno_ai_sdk-0.5.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Jul-12 23:15 elemeno_ai_sdk-0.5.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-Jul-12 23:15 elemeno_ai_sdk-0.5.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     6519 b- defN 23-Jul-12 23:16 elemeno_ai_sdk-0.5.4.dist-info/RECORD
+66 files, 172485 bytes uncompressed, 52908 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -75,47 +75,35 @@
 
 Filename: elemeno_ai_sdk/ml/conversion/tflite.py
 Comment: 
 
 Filename: elemeno_ai_sdk/ml/conversion/torch.py
 Comment: 
 
-Filename: elemeno_ai_sdk/ml/conversion/.ipynb_checkpoints/converter_abc-checkpoint.py
-Comment: 
-
-Filename: elemeno_ai_sdk/ml/conversion/.ipynb_checkpoints/tensorflow-checkpoint.py
-Comment: 
-
-Filename: elemeno_ai_sdk/ml/conversion/.ipynb_checkpoints/tflite-checkpoint.py
-Comment: 
-
-Filename: elemeno_ai_sdk/ml/conversion/.ipynb_checkpoints/torch-checkpoint.py
-Comment: 
-
 Filename: elemeno_ai_sdk/ml/features/__init__.py
 Comment: 
 
 Filename: elemeno_ai_sdk/ml/features/feature_store.py
 Comment: 
 
 Filename: elemeno_ai_sdk/ml/features/feature_table.py
 Comment: 
 
-Filename: elemeno_ai_sdk/ml/features/materialize.py
-Comment: 
-
 Filename: elemeno_ai_sdk/ml/features/query.py
 Comment: 
 
 Filename: elemeno_ai_sdk/ml/features/types.py
 Comment: 
 
 Filename: elemeno_ai_sdk/ml/features/utils.py
 Comment: 
 
+Filename: elemeno_ai_sdk/ml/features/config/repo_config.py
+Comment: 
+
 Filename: elemeno_ai_sdk/ml/features/ingest/__init_.py
 Comment: 
 
 Filename: elemeno_ai_sdk/ml/features/ingest/sink/__init__.py
 Comment: 
 
 Filename: elemeno_ai_sdk/ml/features/ingest/sink/base_ingestion.py
@@ -180,32 +168,32 @@
 
 Filename: elemeno_ai_sdk/ml/inference/inference_response.py
 Comment: 
 
 Filename: elemeno_ai_sdk/ml/inference/input_space.py
 Comment: 
 
-Filename: elemeno_ai_sdk-0.4.9.dist-info/AUTHORS.rst
+Filename: elemeno_ai_sdk-0.5.4.dist-info/AUTHORS.rst
 Comment: 
 
-Filename: elemeno_ai_sdk-0.4.9.dist-info/LICENSE
+Filename: elemeno_ai_sdk-0.5.4.dist-info/LICENSE
 Comment: 
 
-Filename: elemeno_ai_sdk-0.4.9.dist-info/LICENSE-3RDPARTY.txt
+Filename: elemeno_ai_sdk-0.5.4.dist-info/LICENSE-3RDPARTY.txt
 Comment: 
 
-Filename: elemeno_ai_sdk-0.4.9.dist-info/METADATA
+Filename: elemeno_ai_sdk-0.5.4.dist-info/METADATA
 Comment: 
 
-Filename: elemeno_ai_sdk-0.4.9.dist-info/WHEEL
+Filename: elemeno_ai_sdk-0.5.4.dist-info/WHEEL
 Comment: 
 
-Filename: elemeno_ai_sdk-0.4.9.dist-info/entry_points.txt
+Filename: elemeno_ai_sdk-0.5.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: elemeno_ai_sdk-0.4.9.dist-info/top_level.txt
+Filename: elemeno_ai_sdk-0.5.4.dist-info/top_level.txt
 Comment: 
 
-Filename: elemeno_ai_sdk-0.4.9.dist-info/RECORD
+Filename: elemeno_ai_sdk-0.5.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## elemeno_ai_sdk/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.4.9'
+__version__ = '0.5.4'
 
 import logging
 import os
 
 __name__ = 'elemeno_ai_sdk'
 
 LOGLEVEL = os.environ.get('LOGLEVEL', 'WARNING').upper()
```

## elemeno_ai_sdk/config.py

```diff
@@ -1,35 +1,72 @@
 import logging
 import os
 from omegaconf import OmegaConf
+import json
+import requests
+from typing import Mapping, Iterable
 
 class Configs:
-    """ Loads the configuration from the elemeno.yaml file. This class looks for the file in the current directory,
+    """
+    Loads the configuration from the elemeno.yaml file. This class looks for the file in the current directory,
     unless specified with the environment variable ELEMENO_CFG_FILE.
 
     To be able to use environment variables within elemeno.yaml, you need to follow omegaconf specifications. For example:
     ```
     feature_store:
       feast_config_path: ${oc.env:FEAST_CONFIG_PATH}
     ```
     """
     _instance = None
-    _props = None
+    _props = OmegaConf.create()
 
     def __init__(self):
         raise RuntimeError("Call instance() instead")
 
     @classmethod
+    def parse(cls, configdict):
+        if cls._props:
+            cls._props = OmegaConf.merge(cls._props, OmegaConf.create(configdict))
+        else:
+            cls._props = OmegaConf.create(configdict)
+        cls._instance = cls.__new__(cls)
+        return cls._instance.props
+
+    @classmethod
     def instance(cls, force_reload=False):
         cfg_path = os.getenv('ELEMENO_CFG_FILE', 'elemeno.yaml')
         try:
+            # check if cfg_path exists
+            if not os.path.exists(cfg_path):
+                logging.warning("Couldn't find a config file at %s, will continue without loading it", cfg_path)
+                props = OmegaConf.create()
+                return props
             if cls._instance is None or force_reload:
                 cls._instance = cls.__new__(cls)
                 cls._props = OmegaConf.load(cfg_path)
             return cls._instance.props
-        except:
-            logging.warning("Couldn't find a config file at %s, will continue without loading it", cfg_path)
-            return None
+        except Exception as e:
+            logging.error("Unexpected error when instantiating the config object", e)
+            props = OmegaConf.create()
+            return props
 
     @property
     def props(self):
         return self._props
+    
+
+    def auth_fs(self):
+       JWT_TOKEN_PATH = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'jwt_token')
+       SAAS_ADRESS = 'https://c3po-stg.elemeno.ai/'
+       
+       with open(JWT_TOKEN_PATH) as f:
+        JWT_TOKEN =  json.load(f)
+    
+       headers = {'x-token: Bearer {}'.format(JWT_TOKEN)}
+
+       response = requests.get(SAAS_ADRESS + 'user/settings/sdk/authentication', headers=headers)
+       #globals().update(response)  
+
+       return json.loads(response)
+    
+    def parse_jwt_token(self, jwt_token: Mapping[str, Iterable[str]]):
+        pass
```

## elemeno_ai_sdk/cos/minio.py

```diff
@@ -23,14 +23,17 @@
       self.client = Minio(
           host,
           access_key=access_key,
           secret_key=secret_key,
           secure=use_ssl
       )
     
+    def bucket_exists(self, bucket_name: str) -> bool:
+       return self.client.bucket_exists(bucket_name=bucket_name)
+    
     def list_dir(self, bucket_name: str, prefix: str = "") -> list:
         found = self.client.bucket_exists(bucket_name)
         if not found:
             raise ValueError("The specified bucket doesn't exist")
         for eo in self.client.list_objects(bucket_name, prefix=prefix):
           yield self.to_cos_object(eo)
```

## elemeno_ai_sdk/ml/features/feature_store.py

```diff
@@ -1,442 +1,672 @@
-
-
-from datetime import datetime
 import json
-from typing import Optional, Dict, List, Any, Union
-import pandas as pd
+from datetime import datetime
+from typing import Any
+from typing import Callable
+from typing import Dict
+from typing import List
+from typing import Optional
+from typing import Union
+
 import feast
+import pandas as pd
 from feast.infra.offline_stores.offline_store import RetrievalJob
-from elemeno_ai_sdk.ml.features.feature_table import FeatureTable
-from elemeno_ai_sdk.config import Configs
+
 from elemeno_ai_sdk import logger
+from elemeno_ai_sdk.config import Configs
+from elemeno_ai_sdk.ml.features.config.repo_config import create_repo_config
+from elemeno_ai_sdk.ml.features.feature_table import FeatureTable
 from elemeno_ai_sdk.ml.features.ingest.sink.file_ingestion import FileIngestion
-from elemeno_ai_sdk.ml.features.ingest.sink.ingestion_sink_builder \
-   import FileIngestionSinkType, IngestionSinkBuilder, IngestionSinkType
+from elemeno_ai_sdk.ml.features.ingest.sink.file_ingestion import MediaColumn
+from elemeno_ai_sdk.ml.features.ingest.sink.ingestion_sink_builder import (
+    FileIngestionSinkType,
+)
+from elemeno_ai_sdk.ml.features.ingest.sink.ingestion_sink_builder import (
+    IngestionSinkBuilder,
+)
+from elemeno_ai_sdk.ml.features.ingest.sink.ingestion_sink_builder import (
+    IngestionSinkType,
+)
 from elemeno_ai_sdk.ml.features.ingest.sink.minio_ingestion import MinioIngestion
-from elemeno_ai_sdk.ml.features.ingest.source.ingestion_source_builder \
-  import IngestionSourceBuilder, IngestionSourceType
 from elemeno_ai_sdk.ml.features.ingest.source.base_source import ReadResponse
+from elemeno_ai_sdk.ml.features.ingest.source.ingestion_source_builder import (
+    IngestionSourceBuilder,
+)
+from elemeno_ai_sdk.ml.features.ingest.source.ingestion_source_builder import (
+    IngestionSourceType,
+)
 
-class FeatureStore:
 
-  def __init__(self, 
-    sink_type: Optional[IngestionSinkType] = None,
-    file_sink_type: Optional[FileIngestionSinkType] = None,
-    source_type: Optional[IngestionSourceType] = None, **kwargs) -> None:
-    """ 
-    A FeatureStore is the starting point for working with Elemeno feature store via SDK.
-    
-    Use this class in conjunction with the FeatureTable class to create, read, update, and delete features.
-    """
-    self._elm_config = Configs.instance()
-    self._fs = feast.FeatureStore(repo_path=self._elm_config.feature_store.feast_config_path, )
-    if not sink_type:
-      logger.info("No sink type provided, read-only mode will be used")
-    else:
-      self._sink_type = sink_type
-      if sink_type == IngestionSinkType.BIGQUERY:
-        self._sink = IngestionSinkBuilder().build_bigquery(self._fs)
-      elif sink_type == IngestionSinkType.REDSHIFT:
-        redshift_params = self._elm_config.feature_store.sink.params
-        self._sink = IngestionSinkBuilder().build_redshift(self._fs, self._get_connection_string(redshift_params))
-      elif sink_type == IngestionSinkType._REDSHIFT_UNIT_TESTS:
-        redshift_params = self._elm_config.feature_store.sink.params
-        self._sink = IngestionSinkBuilder()._build_redshift_unit_tests(self._fs, self._get_connection_string(redshift_params))
-      else:
-        raise Exception("Unsupported sink type %s", sink_type)
-    if not source_type:
-      logger.info("No source type provided, read-only mode will be used")
-    else:
-      if source_type == IngestionSourceType.BIGQUERY:
-        self._source = IngestionSourceBuilder().build_big_query()
-      elif source_type == IngestionSourceType.ELASTIC:
-        self._source = IngestionSourceBuilder().build_elastic()
-      elif source_type == IngestionSourceType.REDSHIFT:
-        self._source = IngestionSourceBuilder().build_redshift()
-      elif source_type == IngestionSourceType.GCS:
-        self._source = IngestionSourceBuilder().build_gcs()
-      else:
-        raise Exception("Unsupported source type %s", source_type)
-    self._file_sink_type = file_sink_type
-    if not file_sink_type:
-      logger.info("File sink type not specified, will not download files when there are binary columns")
-    else:
-      if not self._elm_config.dask.uri:
-        logger.warn("Dask URI not specified, will not download files")
-      else:
-        print("Creating instance of MinioIngestionDask")
-        self. _file_sink = MinioIngestion(self._elm_config.dask.uri)
-    self.config = self._fs.config
-    # memory holds a reference for the result of the last data handling method
-    self._memory = None
-
-  def read_from_query(self, query: str) -> pd.DataFrame:
-    return super().read_from_query(self._source, query)
-
-  def _get_connection_string(self, redshift_params):
-    if self._sink_type == IngestionSinkType._REDSHIFT_UNIT_TESTS:
-      return "sqlite:///test.db"
-    user = redshift_params.user
-    password = redshift_params.password
-    host = redshift_params.host
-    port = redshift_params.port 
-    database = redshift_params.database 
-    return f"postgresql://{user}:{password}@{host}:{port}/{database}"
-
-  @property
-  def fs(self) -> feast.FeatureStore:
-    return self._fs
-
-  def ingest_response(self, feature_table: FeatureTable, 
-      to_ingest: ReadResponse, renames: Optional[Dict[str, str]] = None,
-      all_columns: Optional[List[str]] = None) -> None:
-    """ 
-    Ingest the given dataframe into the given feature table.
-    
-    This method allows you to rename the columns of the dataframe before ingesting.
-    
-    You can also filter the columns to be ingested.
-    
-    It is required that your dataframe have the timestamp columns (event_timestamp and created_timestamp) with the correct types (pd.DateTime).
-
-    args:
-    
-    - feature_table: FeatureTable object
-    - to_ingest: A ReadResponse instance (since base_source.py ReadResponse)
-    - renames: A dictionary of column names to be renamed.
-    - all_columns: A list of columns to be ingested. If None, all columns will be ingested.
-    """
-    feature_table.table_schema
-    if self._has_medias(feature_table):
-      self._ingest_files(to_ingest)
-    self.ingest(feature_table, to_ingest.dataframe, renames, all_columns)
-
-  def _media_columns(self, feature_table):
-    media_columns = []
-    for k, p in feature_table.original_schema.items():
-      if p['type'] == 'binary_upload' or p['type'] == 'binary_download':
-        media_columns.append(k)
-    return media_columns
-  
-  def _has_medias(self, feature_table):
-    mcols = self._media_columns(feature_table)
-    return len(mcols) > 0
-
-
-  def staging_ingest(self, to_ingest: pd.DataFrame, name: str) -> None:
-    """ 
-    Ingest the given dataframe into a staging are in the feature store batch persistence
-
-    The ingest data will not be a feature table yet, instead it will be available as 
-    a simple structure in the persistence, and can be later turned into a feature table
-    using the staging_to_feature_table method.
-
-    args:
-    
-    - to_ingest: A dataframe to be ingested
-    - name: The name of the staging area
-    """
-    self._sink.staging_ingest(to_ingest, name)
-
-  def ingest(self, feature_table: FeatureTable, 
-      to_ingest: pd.DataFrame, renames: Optional[Dict[str, str]] = None,
-      all_columns: Optional[List[str]] = None) -> None:
-    """ 
-    Ingest the given dataframe into the given feature table.
-    
-    This method allows you to rename the columns of the dataframe before ingesting.
-    
-    You can also filter the columns to be ingested.
-    
-    It is required that your dataframe have the timestamp columns (event_timestamp and created_timestamp) with the correct types (pd.DateTime).
-
-    args:
-    
-    - feature_table: FeatureTable object
-    - to_ingest: A pandas dataframe to be ingested
-    - renames: A dictionary of column names to be renamed
-    - all_columns: A list of columns to be ingested. If None, all columns will be ingested
-    """
-    media_cols = self._media_columns(feature_table)
-    if len(media_cols) > 0:
-      self._ingest_files_from_df(to_ingest, media_cols)
-    self._sink.ingest(to_ingest, feature_table, renames, all_columns)
-    
-  def _ingest_files_from_df(self, to_ingest: pd.DataFrame, media_cols: List[str]):
-    if self._file_sink_type is None:
-      raise ValueError("File sink type not specified, cannot ingest files")  
-    self._file_sink.io_batch_ingest(to_ingest, media_cols)
-
-  def _ingest_files(self, to_ingest: ReadResponse):
-    if self._file_sink_type is None:
-      raise ValueError("File sink type not specified, cannot ingest files")  
-    medias = json.loads(to_ingest.prepared_medias)
-    print("len of to_ingest.prepared_medias", len(medias))
-    self._file_sink.io_batch_ingest(medias)
-  
-  def ingest_from_query_same_source(self, ft: FeatureTable, query: str):
-    """ 
-    Ingest data from a query. Used when the source and the sink are the same.
-    
-    It's important to notice that your query must return the timestamp columns (event_timestamp and created_timestamp) with the correct timestamp types of the source of choice.
-    
-    The query will be executed against the source of data you defined, so make sure query contains a compatible SQL statement.
-
-    args:
-    
-    - ft: The FeatureTable object
-    - query: A SQL query to ingest data from.
-    """
-    self._sink.ingest_from_query(query, ft)
-
-  def read_and_ingest_from_query(self, ft: 'FeatureTable', query: str, 
-      binary_cols: List[str], ignore_when_empty: Optional[List[str]] = None, **kwargs):
-    """
-    Ingest data from a query. Used when the source and the sink are different.
-    
-    It's important to notice that your query must return the timestamp columns (event_timestamp and created_timestamp) with the correct timestamp types of the source of choice.
-    
-    The query will be executed against the source of data you defined, so make sure query contains a compatible SQL statement.
-
-    args:
-    
-    - ft: The FeatureTable object
-    - query: A SQL query to ingest data from.
-    - binary_cols: A list of columns that are binary and will be downloaded to cloud object storage.
-    - ignore_when_empty: A list of columns that will be ignored when the result is empty.
-    """
-    if not 'index' in kwargs:
-      raise("index must be provided")
-    
-    read_response = self._source.read(query=query, binary_columns=binary_cols, dest_folder_col="id", media_id_col="id", **kwargs)
-    # make sure only the featuretable columns are ingested
-    cols = [e.name for e in ft.entities]
-    cols.extend([f.name for f in ft.features])
-    cols.extend([ft.created_col, ft.evt_col])
-    if ignore_when_empty != None:
-      read_response.dataframe = read_response.dataframe.dropna(subset=ignore_when_empty)
-    self.ingest_response(ft, read_response, all_columns=cols)
-
-  def read_and_ingest_from_query_after(self, ft: 'FeatureTable', query: str, after: str, binary_cols: Optional[List[str]] = None,
-      ignore_when_empty: Optional[List[str]] = None, **kwargs):
-    """
-    Ingest data from a query after a specific timestamp. Used when the source and the sink are different.
-
-    It's important to notice that your query must return the timestamp columns (event_timestamp and created_timestamp) with the correct timestamp types of the source of choice.
-    
-    The query will be executed against the source of data you defined, so make sure query contains a compatible SQL statement.
-
-    args:
-    - ft: The FeatureTable object
-    - query: A SQL query to ingest data from.
-    - after: A timestamp after which the query will be executed. Use the same date format of the source.
-    - binary_cols: A list of binary columns containing references to files to be downloaded to our cloud object storage.
-    """
-    if not 'index' in kwargs:
-      raise("index must be provided")
-    read_response = self._source.read_after(query=query, timestamp_str=after, binary_columns=binary_cols, media_id_col="id", dest_folder_col="id", **kwargs)
-    # make sure only the featuretable columns are ingested
-    cols = [e.name for e in ft.entities]
-    cols.extend([f.name for f in ft.features])
-    cols.extend([ft.created_col, ft.evt_col])
-    if ignore_when_empty != None:
-      read_response.dataframe = read_response.dataframe.dropna(subset=ignore_when_empty)
-    self.ingest_response(ft, read_response, all_columns=cols)
-
-  def read_all(self) -> pd.DataFrame:
-    """
-    Read all data from the source.
-    """
-    return self._source.read()
-
-  def get_historical_features(self, entity_source: pd.DataFrame, feature_refs: List[str]) -> RetrievalJob:
-    """ Get historical features from the feature store.
-    This method allows you to retrieve historical features from the feature store.
-    
-    You must specify a dataframe with the entity_id and entity_type columns.
-    
-    You must specify a list of feature_refs to retrieve. feature_refs are the name of the features.
-
-    args:
-    
-    - entity_source: A dataframe with the entity_id and entity_type columns.
-    - feature_refs: A list of feature_refs to retrieve.
-
-    returns:
-    
-    - A RetrievalJob object.
-    """
-    return self._fs.get_historical_features(entity_source, feature_refs)
-
-  def get_online_features(self, entities: List[Dict[str, Any]],
-        requested_features: Optional[List[str]]=None) \
-        -> feast.online_response.OnlineResponse:
-    """ 
-    Get online features from the feature store.
-    This method allows you to retrieve online features from the feature store.
-    
-    You must specify a list of entities to retrieve.
-    
-    You may specify a list of features to retrieve. If None, all features will be retrieved.
-
-    args:
-    
-    - entities: A list of entities to retrieve.
-    - requested_features: Optional list of features to retrieve. If None, all features will be retrieved.
-    
-    returns:
-    
-    - An OnlineResponse object.
-    """
-    if self._fs.config.online_store is None:
-      raise ValueError("Online store is not configure, make sure to configure the property online_store in the config yaml")
-    return self._fs.get_online_features(features=requested_features, entity_rows=entities)
-  
-  def get_training_features(self, feature_table: FeatureTable,
+class FeatureStore:
+    def __init__(
+        self,
+        sink_type: Optional[IngestionSinkType] = None,
+        file_sink_type: Optional[FileIngestionSinkType] = None,
+        source_type: Optional[IngestionSourceType] = None,
+        config: Optional[Dict] = None,
+        **kwargs,
+    ) -> None:
+        """
+        A FeatureStore is the starting point for working with Elemeno feature store via SDK.
+
+        Use this class in conjunction with the FeatureTable class to create, read, update, and delete features.
+        """
+
+        self._elm_config = Configs.instance()
+        if config is not None:
+            logger.debug("Using provided config via code")
+            self._elm_config = Configs.parse(config)
+
+        if self._elm_config.is_empty():
+            raise Exception(
+                "Missing elemeno.yaml file. Make sure it's in the current directory or in the ELEMENO_CFG_FILE environment variable."
+            )
+
+        repo_config = create_repo_config(self._elm_config)
+        self._fs = feast.FeatureStore(
+            repo_config=repo_config,
+        )
+
+        self._source_type = source_type
+        self._sink_type = sink_type
+        self._file_sink = file_sink_type
+
+        if not sink_type:
+            logger.info("No sink type provided, read-only mode will be used")
+        else:
+            self._sink_type = sink_type
+            if sink_type == IngestionSinkType.BIGQUERY:
+                self._sink = IngestionSinkBuilder().build_bigquery(self._fs)
+            elif sink_type == IngestionSinkType.REDSHIFT:
+                redshift_params = self._elm_config.feature_store.sink.params
+                self._sink = IngestionSinkBuilder().build_redshift(
+                    self._fs, self._get_connection_string(redshift_params)
+                )
+            elif sink_type == IngestionSinkType._REDSHIFT_UNIT_TESTS:
+                redshift_params = self._elm_config.feature_store.sink.params
+                self._sink = IngestionSinkBuilder()._build_redshift_unit_tests(
+                    self._fs, self._get_connection_string(redshift_params)
+                )
+            else:
+                raise Exception("Unsupported sink type %s", sink_type)
+        if not source_type:
+            logger.info("No source type provided, read-only mode will be used")
+        else:
+            if source_type == IngestionSourceType.BIGQUERY:
+                self._source = IngestionSourceBuilder().build_big_query()
+            elif source_type == IngestionSourceType.ELASTIC:
+                self._source = IngestionSourceBuilder().build_elastic()
+            elif source_type == IngestionSourceType.REDSHIFT:
+                self._source = IngestionSourceBuilder().build_redshift()
+            elif source_type == IngestionSourceType.GCS:
+                self._source = IngestionSourceBuilder().build_gcs()
+            else:
+                raise Exception("Unsupported source type %s", source_type)
+        self._file_sink_type = file_sink_type
+        if not file_sink_type:
+            logger.info(
+                "File sink type not specified, will not download files when there are binary columns"
+            )
+        else:
+            self._file_sink = MinioIngestion()
+        self.config = self._fs.config
+        # memory holds a reference for the result of the last data handling method
+        self._memory = None
+
+    def read_from_query(self, query: str) -> pd.DataFrame:
+        return super().read_from_query(self._source, query)
+
+    def _get_connection_string(self, redshift_params):
+        if self._sink_type == IngestionSinkType._REDSHIFT_UNIT_TESTS:
+            return "sqlite:///test.db?mode=rwc"
+        user = redshift_params.user
+        password = redshift_params.password
+        host = redshift_params.host
+        port = redshift_params.port
+        database = redshift_params.database
+        return f"postgresql://{user}:{password}@{host}:{port}/{database}"
+
+    @property
+    def fs(self) -> feast.FeatureStore:
+        return self._fs
+
+    def ingest_response(
+        self,
+        feature_table: FeatureTable,
+        to_ingest: ReadResponse,
+        renames: Optional[Dict[str, str]] = None,
+        all_columns: Optional[List[str]] = None,
+    ) -> None:
+        """
+        Ingest the given dataframe into the given feature table.
+
+        This method allows you to rename the columns of the dataframe before ingesting.
+
+        You can also filter the columns to be ingested.
+
+        It is required that your dataframe have the timestamp columns (event_timestamp and created_timestamp) with the correct types (pd.DateTime).
+
+        args:
+
+        - feature_table: FeatureTable object
+        - to_ingest: A ReadResponse instance (since base_source.py ReadResponse)
+        - renames: A dictionary of column names to be renamed.
+        - all_columns: A list of columns to be ingested. If None, all columns will be ingested.
+        """
+        if self._has_medias(feature_table):
+            self._ingest_files(to_ingest)
+        self.ingest(feature_table, to_ingest.dataframe, renames, all_columns)
+
+    def _media_columns(self, feature_table):
+        media_columns = []
+        if not feature_table.original_schema:
+            logger.debug("No original schema, assuming no media columns")
+            return media_columns
+        for k, p in feature_table.original_schema["properties"].items():
+            if p["type"] == "binary_upload" or p["type"] == "binary_download":
+                m = MediaColumn(k, p["type"] == "binary_upload")
+                media_columns.append(m)
+        return media_columns
+
+    def _has_medias(self, feature_table):
+        mcols = self._media_columns(feature_table)
+        return len(mcols) > 0
+
+    def staging_ingest(self, to_ingest: pd.DataFrame, name: str) -> None:
+        """
+        Ingest the given dataframe into a staging are in the feature store batch persistence
+
+        The ingest data will not be a feature table yet, instead it will be available as
+        a simple structure in the persistence, and can be later turned into a feature table
+        using the staging_to_feature_table method.
+
+        args:
+
+        - to_ingest: A dataframe to be ingested
+        - name: The name of the staging area
+        """
+        self._sink.staging_ingest(to_ingest, name)
+
+    def ingest(
+        self,
+        feature_table: FeatureTable,
+        to_ingest: pd.DataFrame,
+        renames: Optional[Dict[str, str]] = None,
+        all_columns: Optional[List[str]] = None,
+    ) -> None:
+        """
+        Ingest the given dataframe into the given feature table.
+
+        This method allows you to rename the columns of the dataframe before ingesting.
+
+        You can also filter the columns to be ingested.
+
+        It is required that your dataframe have the timestamp columns (event_timestamp and created_timestamp) with the correct types (pd.DateTime).
+
+        args:
+
+        - feature_table: FeatureTable object
+        - to_ingest: A pandas dataframe to be ingested
+        - renames: A dictionary of column names to be renamed
+        - all_columns: A list of columns to be ingested. If None, all columns will be ingested
+        """
+        media_cols = self._media_columns(feature_table)
+        if len(media_cols) > 0:
+            self._ingest_files_from_df(feature_table.name, to_ingest, media_cols)
+        self._sink.ingest(to_ingest, feature_table, renames, all_columns)
+
+    def _ingest_files_from_df(
+        self, feature_table_name: str, to_ingest: pd.DataFrame, media_cols: List[str]
+    ):
+        if self._file_sink_type is None:
+            raise ValueError("File sink type not specified, cannot ingest files")
+        self._file_sink.io_batch_ingest_from_df(
+            feature_table_name, to_ingest, media_cols
+        )
+
+    def _ingest_files(self, to_ingest: ReadResponse):
+        if self._file_sink_type is None:
+            raise ValueError("File sink type not specified, cannot ingest files")
+        medias = json.loads(to_ingest.prepared_medias)
+        print("len of to_ingest.prepared_medias", len(medias))
+        self._file_sink.io_batch_ingest(medias)
+
+    def ingest_from_query_same_source(self, ft: FeatureTable, query: str):
+        """
+        Ingest data from a query. Used when the source and the sink are the same.
+
+        It's important to notice that your query must return the timestamp columns (event_timestamp and created_timestamp) with the correct timestamp types of the source of choice.
+
+        The query will be executed against the source of data you defined, so make sure query contains a compatible SQL statement.
+
+        args:
+
+        - ft: The FeatureTable object
+        - query: A SQL query to ingest data from.
+        """
+        self._sink.ingest_from_query(query, ft)
+
+    def read_and_ingest_from_query(
+        self,
+        ft: "FeatureTable",
+        query: str,
+        binary_cols: List[str],
+        ignore_when_empty: Optional[List[str]] = None,
+        **kwargs,
+    ):
+        """
+        Ingest data from a query. Used when the source and the sink are different.
+
+        It's important to notice that your query must return the timestamp columns (event_timestamp and created_timestamp) with the correct timestamp types of the source of choice.
+
+        The query will be executed against the source of data you defined, so make sure query contains a compatible SQL statement.
+
+        args:
+
+        - ft: The FeatureTable object
+        - query: A SQL query to ingest data from.
+        - binary_cols: A list of columns that are binary and will be downloaded to cloud object storage.
+        - ignore_when_empty: A list of columns that will be ignored when the result is empty.
+        """
+        read_response = self._source.read(
+            base_query=query,
+            binary_columns=binary_cols,
+            dest_folder_col="id",
+            media_id_col="id",
+            **kwargs,
+        )
+        # make sure only the featuretable columns are ingested
+        cols = [e.name for e in ft.entities]
+        cols.extend([f.name for f in ft.features])
+        cols.extend([ft.created_col, ft.evt_col])
+        if ignore_when_empty != None:
+            read_response.dataframe = read_response.dataframe.dropna(
+                subset=ignore_when_empty
+            )
+        self.ingest_response(ft, read_response, all_columns=cols)
+
+    def read_transform_and_ingest(
+        self,
+        ft: "FeatureTable",
+        query: str,
+        transformations: List[Callable[[pd.DataFrame], pd.DataFrame]],
+        binary_cols: Optional[List[str]] = None,
+        ignore_when_empty: Optional[List[str]] = None,
+        **kwargs,
+    ):
+        """
+        Ingest data from a query after applying a pipeline of transformations. Used when the source and the sink are different.
+
+        It's important to notice that your query must return the timestamp columns (event_timestamp and created_timestamp) with the correct timestamp types of the source of choice.
+
+        The query will be executed against the source of data you defined, so make sure query contains a compatible SQL statement.
+        args:
+
+        - ft: The FeatureTable object
+        - query: A SQL query to ingest data from.
+        - binary_cols: A list of columns that are binary and will be downloaded to cloud object storage.
+        - transformations: A list of transformation functions to be applied on the dataframe
+        - ignore_when_empty: A list of columns that will be ignored when the result is empty.
+        """
+        read_response = self._source.read(
+            base_query=query,
+            binary_columns=binary_cols,
+            dest_folder_col="id",
+            media_id_col="id",
+            **kwargs,
+        )
+        # make sure only the featuretable columns are ingested
+        cols = [e.name for e in ft.entities]
+        cols.extend([f.name for f in ft.features])
+        cols.extend([ft.created_col, ft.evt_col])
+        if ignore_when_empty != None:
+            read_response.dataframe = read_response.dataframe.dropna(
+                subset=ignore_when_empty
+            )
+
+        # Apply transformations
+        for transform in transformations:
+            read_response.dataframe = transform(read_response.dataframe)
+
+        self.ingest_response(ft, read_response, all_columns=cols)
+
+    def transform_and_ingest(
+        self,
+        ft: "FeatureTable",
+        response: pd.DataFrame,
+        transformations: List[Callable[[pd.DataFrame], pd.DataFrame]],
+        all_columns: Optional[List[str]] = None,
+        binary_cols: Optional[List[str]] = None,
+        ignore_when_empty: Optional[List[str]] = None,
+        **kwargs,
+    ):
+        """
+        Ingest data from a query after applying a pipeline of transformations. Used when the source and the sink are different.
+
+        It's important to notice that your query must return the timestamp columns (event_timestamp and created_timestamp) with the correct timestamp types of the source of choice.
+
+        The query will be executed against the source of data you defined, so make sure query contains a compatible SQL statement.
+        args:
+
+        - ft: The FeatureTable object
+        - binary_cols: A list of columns that are binary and will be downloaded to cloud object storage.
+        - transformations: A list of transformation functions to be applied on the dataframe
+        - ignore_when_empty: A list of columns that will be ignored when the result is empty.
+        """
+        cols = [e.name for e in ft.entities]
+        cols.extend([f.name for f in ft.features])
+        cols.extend([ft.created_col, ft.evt_col])
+        if ignore_when_empty != None:
+            response = response.dropna(subset=ignore_when_empty)
+
+        # Apply transformations
+        for transform in transformations:
+            response = transform(response)
+
+        self.ingest(ft, response, all_columns=cols)
+
+    def read_and_ingest_from_query_after(
+        self,
+        ft: "FeatureTable",
+        query: str,
+        after: str,
+        binary_cols: Optional[List[str]] = None,
+        ignore_when_empty: Optional[List[str]] = None,
+        **kwargs,
+    ):
+        """
+        Ingest data from a query after a specific timestamp. Used when the source and the sink are different.
+
+        It's important to notice that your query must return the timestamp columns (event_timestamp and created_timestamp) with the correct timestamp types of the source of choice.
+
+        The query will be executed against the source of data you defined, so make sure query contains a compatible SQL statement.
+
+        args:
+        - ft: The FeatureTable object
+        - query: A SQL query to ingest data from.
+        - after: A timestamp after which the query will be executed. Use the same date format of the source.
+        - binary_cols: A list of binary columns containing references to files to be downloaded to our cloud object storage.
+        """
+        read_response = self._source.read_after(
+            base_query=query,
+            timestamp_str=after,
+            binary_columns=binary_cols,
+            media_id_col="id",
+            dest_folder_col="id",
+            **kwargs,
+        )
+        # make sure only the featuretable columns are ingested
+        cols = [e.name for e in ft.entities]
+        cols.extend([f.name for f in ft.features])
+        cols.extend([ft.created_col, ft.evt_col])
+        if ignore_when_empty != None:
+            read_response.dataframe = read_response.dataframe.dropna(
+                subset=ignore_when_empty
+            )
+        self.ingest_response(ft, read_response, all_columns=cols)
+
+    def read_all(self) -> pd.DataFrame:
+        """
+        Read all data from the source.
+        """
+        return self._source.read()
+
+    def get_historical_features(
+        self, entity_source: pd.DataFrame, feature_refs: List[str]
+    ) -> RetrievalJob:
+        """Get historical features from the feature store.
+        This method allows you to retrieve historical features from the feature store.
+
+        You must specify a dataframe with the entity_id and entity_type columns.
+
+        You must specify a list of feature_refs to retrieve. feature_refs are the name of the features.
+
+        args:
+
+        - entity_source: A dataframe with the entity_id and entity_type columns.
+        - feature_refs: A list of feature_refs to retrieve.
+
+        returns:
+
+        - A RetrievalJob object.
+        """
+        return self._fs.get_historical_features(entity_source, feature_refs)
+
+    def materialize_incremental(
+        self,
+        feature_table: FeatureTable,
+        end_ts: str = datetime.now().replace(microsecond=0).isoformat(),
+    ):
+        """
+        Materialize the offline data to the online table incrementaly.
+
+        args:
+          feature_table (FeatureTable): The feature table to materialize.
+          end_ts (str, optional): The end timestamp to materialize. Defaults to datetime.now().replace(microsecond=0).isoformat().
+
+        """
+        self._fs.materialize_incremental([feature_table.get_view()], end_ts)
+
+    def get_online_features(
+        self,
+        entities: List[Dict[str, Any]],
+        requested_features: Optional[List[str]] = None,
+    ) -> feast.online_response.OnlineResponse:
+        """
+        Get online features from the feature store.
+        This method allows you to retrieve online features from the feature store.
+
+        You must specify a list of entities to retrieve.
+
+        You may specify a list of features to retrieve. If None, all features will be retrieved.
+
+        args:
+
+        - entities: A list of entities to retrieve.
+        - requested_features: Optional list of features to retrieve. If None, all features will be retrieved.
+
+        returns:
+
+        - An OnlineResponse object.
+        """
+        if self._fs.config.online_store is None:
+            raise ValueError(
+                "Online store is not configure, make sure to configure the property online_store in the config yaml"
+            )
+        return self._fs.get_online_features(
+            features=requested_features, entity_rows=entities
+        )
+
+    def get_training_features(
+        self,
+        feature_table: FeatureTable,
         features_selected: List[str] = None,
         date_from: Optional[datetime] = None,
         date_to: Optional[datetime] = None,
         limit: Optional[int] = None,
         only_most_recent: Optional[bool] = True,
         diff_table: Optional[str] = None,
         diff_join_key: Optional[str] = None,
         join_key: Optional[str] = None,
         diff_where: Optional[Dict] = None,
-        timestamp_column: Optional[str] = "created_timestamp") -> pd.DataFrame:
-    """ 
-    Get the training features for the given feature view.
-    
-    args:
-    
-    - feature_table: Feature view name
-    - features_selected: A list of features to be selected. If None, all features will be selected.
-    - date_from: The start date of the training period. If None, the start date of the feature table will be used.
-    - date_to: The end date of the training period. If None, the end date of the feature table will be used.
-    - only_most_recent: If True, only the most recent features will be selected. If False, all features will be selected.
-    - diff_table: If not None, the features will be compared with the features in the diff_table. The diff_table should have a column with the same name of the features table in order to compare. This is useful for when you want to filter, at query time, features from the result.
-    - diff_join_key: The join key to be used to compare the features.
-    - diff_where: A dictionary with the where clause to be used to compare the features.
-    - timestamp_column: The timestamp column to be used to filter the features. Valid values are "created_timestamp" and "event_timestamp". Default is "created_timestamp".
-    
-    returns:
-    
-    A dataframe with the training features.
-    """
-    table_name = feature_table.name
-    if features_selected is None:
-      columns = "*"
-    else:
-      columns = ",".join(map(lambda x: f"\"{table_name}\".{x}", features_selected))
-    join = ""
-    if diff_table and diff_join_key:
-      left_join_key = join_key if join_key else diff_join_key
-      join = f"LEFT JOIN \"{diff_table}\" ON \"{table_name}\".{left_join_key} = \"{diff_table}\".{diff_join_key}"
-      if diff_where:
-        for k,v in diff_where.items():
-          join += f" AND \"{diff_table}\".{k} = '{v}'"
-    where = ""
-    if timestamp_column != "created_timestamp" and timestamp_column != "event_timestamp":
-      raise ValueError(f"Invalid timestamp_column: {timestamp_column}. Valid values are 'created_timestamp' and 'event_timestamp'")
-    if date_from:
-      where += f"WHERE \"{table_name}\".{timestamp_column} >= '{date_from.isoformat()}'"
-    if date_to:
-      if where != "":
-        where += f" AND \"{table_name}\".{timestamp_column} <= '{date_to.isoformat()}'"
-      else:
-        where += f"WHERE \"{table_name}\".{timestamp_column} <= '{date_to.isoformat()}'"
-    if diff_table and where != "":
-      where += f" AND \"{diff_table}\".{diff_join_key} is null"
-    elif diff_table:
-      where += f"WHERE \"{diff_table}\".{diff_join_key} is null"
-    if limit:
-      where += f" LIMIT {limit}"
-    query = f"SELECT {columns} FROM \"{table_name}\" {join} {where} ORDER BY \"{table_name}\".{timestamp_column} ASC"
-    df = self._sink.read_table(query)
-    if only_most_recent:
-      return df.sort_values(by="created_timestamp", ascending=False) \
-        .groupby(by=[e.name for e in feature_table.entities]) \
-        .tail(1)
-    else:
-      return df
-
-
-  def ingest_schema(self, feature_table: FeatureTable, schema_file_path: str) -> None:
-    """
-    Ingest the schema of the feature table into the feature store. Useful when you're creating a new feature table.
-
-    args:
-    
-    - feature_table: FeatureTable object
-    - schema_file_path: Twhe local path to the schema file.
-
-    The is the first step to create a feature table via SDK, you will need to manually create a json schema file to your table.
-    The schema file syntax uses an extension of JSONSchema. It's basically a JSONSchema file with some additional fields and properties.
-    The additional fields are necessary in order to identify which of the columns are keys and how the timestamps will be identified.
-
-    Example of a feature table schema file:
-
-    >>> schema_example = {
-      "type": "object",
-      "properties": {
-        "userId": {
-          "isKey": "true",
-          "type": "string"
-        },
-        "address": {
-          "type": "object"
-        },
-        "medianSpent": {
-          "type": "number"
+        download_binaries: Optional[bool] = False,
+        timestamp_column: Optional[str] = "created_timestamp",
+    ) -> pd.DataFrame:
+        """
+        Get the training features for the given feature view.
+
+        args:
+
+        - feature_table: Feature view name
+        - features_selected: A list of features to be selected. If None, all features will be selected.
+        - date_from: The start date of the training period. If None, the start date of the feature table will be used.
+        - date_to: The end date of the training period. If None, the end date of the feature table will be used.
+        - only_most_recent: If True, only the most recent features will be selected. If False, all features will be selected.
+        - diff_table: If not None, the features will be compared with the features in the diff_table. The diff_table should have a column with the same name of the features table in order to compare. This is useful for when you want to filter, at query time, features from the result.
+        - diff_join_key: The join key to be used to compare the features.
+        - diff_where: A dictionary with the where clause to be used to compare the features.
+        - timestamp_column: The timestamp column to be used to filter the features. Valid values are "created_timestamp" and "event_timestamp". Default is "created_timestamp".
+
+        returns:
+
+        A dataframe with the training features.
+        """
+        table_name = feature_table.name
+        if features_selected is None:
+            columns = "*"
+        else:
+            columns = ",".join(map(lambda x: f'"{table_name}".{x}', features_selected))
+        join = ""
+        if diff_table and diff_join_key:
+            left_join_key = join_key if join_key else diff_join_key
+            join = f'LEFT JOIN "{diff_table}" ON "{table_name}".{left_join_key} = "{diff_table}".{diff_join_key}'
+            if diff_where:
+                for k, v in diff_where.items():
+                    join += f" AND \"{diff_table}\".{k} = '{v}'"
+        where = ""
+        if (
+            timestamp_column != "created_timestamp"
+            and timestamp_column != "event_timestamp"
+        ):
+            raise ValueError(
+                f"Invalid timestamp_column: {timestamp_column}. Valid values are 'created_timestamp' and 'event_timestamp'"
+            )
+        if date_from:
+            where += f"WHERE \"{table_name}\".{timestamp_column} >= '{date_from.isoformat()}'"
+        if date_to:
+            if where != "":
+                where += f" AND \"{table_name}\".{timestamp_column} <= '{date_to.isoformat()}'"
+            else:
+                where += f"WHERE \"{table_name}\".{timestamp_column} <= '{date_to.isoformat()}'"
+        if diff_table and where != "":
+            where += f' AND "{diff_table}".{diff_join_key} is null'
+        elif diff_table:
+            where += f'WHERE "{diff_table}".{diff_join_key} is null'
+        if limit:
+            where += f" LIMIT {limit}"
+        query = f'SELECT {columns} FROM "{table_name}" {join} {where} ORDER BY "{table_name}".{timestamp_column} ASC'
+        df = self._sink.read_table(query)
+
+        if download_binaries and self._has_medias(feature_table=feature_table):
+            self._file_sink.io_batch_digest(
+                feature_table.name, df, self._media_columns(feature_table)
+            )
+
+        if only_most_recent:
+            return (
+                df.sort_values(by="created_timestamp", ascending=False)
+                .groupby(by=[e.name for e in feature_table.entities])
+                .tail(1)
+            )
+        else:
+            return df
+
+    def ingest_schema(self, feature_table: FeatureTable, schema_file_path: str) -> None:
+        """
+        Ingest the schema of the feature table into the feature store. Useful when you're creating a new feature table.
+
+        args:
+
+        - feature_table: FeatureTable object
+        - schema_file_path: Twhe local path to the schema file.
+
+        The is the first step to create a feature table via SDK, you will need to manually create a json schema file to your table.
+        The schema file syntax uses an extension of JSONSchema. It's basically a JSONSchema file with some additional fields and properties.
+        The additional fields are necessary in order to identify which of the columns are keys and how the timestamps will be identified.
+
+        Example of a feature table schema file:
+
+        >>> schema_example = {
+          "type": "object",
+          "properties": {
+            "userId": {
+              "isKey": "true",
+              "type": "string"
+            },
+            "address": {
+              "type": "object"
+            },
+            "medianSpent": {
+              "type": "number"
+            }
+            "age": {
+              "type": "integer"
+            },
+            "created_timestamp": {
+              "examples": [
+                "1970-01-01T00:00:00+00:00"
+              ],
+              "format": "date-time",
+              "type": "string"
+            },
+            "event_timestamp": {
+              "examples": [
+                "1970-01-01T00:00:00+00:00"
+              ],
+              "format": "date-time",
+              "type": "string"
+            }
+          }
         }
-        "age": {
-          "type": "integer"
-        },
-        "created_timestamp": {
-          "examples": [
-            "1970-01-01T00:00:00+00:00"
-          ],
-          "format": "date-time",
-          "type": "string"
-        },
-        "event_timestamp": {
-          "examples": [
-            "1970-01-01T00:00:00+00:00"
-          ],
-          "format": "date-time",
-          "type": "string"
-        }
-      }
-    }
-    """
-    self._sink.ingest_schema(feature_table, schema_file_path)
-    # call get_view to force an apply of the schema
-    feature_table.get_view()
-
-  def get_sink_last_ts(self, feature_table: 'FeatureTable', date_from: Optional[datetime] = None, where: Optional[Dict[str, Any]] = None) -> Any:
-    """
-    Get the last row of the feature table.
-    This is particularly useful when ingesting or reading data,
-    the result of this method could be piped into the date_from
-    of your method to read data from a source.
-
-    args:
-    
-    - feature_table: FeatureTable object
-    - date_from: The start date of the training period. If None, the start date of the feature table will be used.
-
-    returns:
-
-    - A timestamp of the same type used in the event_timestamp column
-    """
-    row = self._sink.get_last_row(feature_table, date_from=date_from, where=where)
-    if row is None or row.empty:
-      return None
-    # rename column if the db returned in the format bellow, otherwise no-op
-    row = row.rename(columns={f"{feature_table.evt_col}": "max"})
-    return row["max"][0]
-
-  def apply(self, objects: Union[feast.Entity, feast.FeatureView, feast.OnDemandFeatureView, feast.FeatureService,
-    List[Union[feast.FeatureView, feast.OnDemandFeatureView, feast.Entity, feast.FeatureService]]],
-        objects_to_delete: List[Union[feast.FeatureView, feast.OnDemandFeatureView, feast.Entity, feast.FeatureService, None]] = None,
-        partial: bool = True):
-    self._fs.apply(objects=objects, objects_to_delete=objects_to_delete, partial=partial)
+        """
+        self._sink.ingest_schema(feature_table, schema_file_path)
+        # call get_view to force an apply of the schema
+        feature_table.get_view()
+
+    def get_sink_last_ts(
+        self,
+        feature_table: "FeatureTable",
+        date_from: Optional[datetime] = None,
+        where: Optional[Dict[str, Any]] = None,
+    ) -> Any:
+        """
+        Get the last row of the feature table.
+        This is particularly useful when ingesting or reading data,
+        the result of this method could be piped into the date_from
+        of your method to read data from a source.
+
+        args:
+
+        - feature_table: FeatureTable object
+        - date_from: The start date of the training period. If None, the start date of the feature table will be used.
+
+        returns:
+
+        - A timestamp of the same type used in the event_timestamp column
+        """
+        row = self._sink.get_last_row(feature_table, date_from=date_from, where=where)
+        if row is None or row.empty:
+            return None
+        # rename column if the db returned in the format bellow, otherwise no-op
+        row = row.rename(columns={f"{feature_table.evt_col}": "max"})
+        return row["max"][0]
+
+    def apply(
+        self,
+        objects: Union[
+            feast.Entity,
+            feast.FeatureView,
+            feast.OnDemandFeatureView,
+            feast.FeatureService,
+            List[
+                Union[
+                    feast.FeatureView,
+                    feast.OnDemandFeatureView,
+                    feast.Entity,
+                    feast.FeatureService,
+                ]
+            ],
+        ],
+        objects_to_delete: List[
+            Union[
+                feast.FeatureView,
+                feast.OnDemandFeatureView,
+                feast.Entity,
+                feast.FeatureService,
+                None,
+            ]
+        ] = None,
+        partial: bool = True,
+    ):
+        self._fs.apply(
+            objects=objects, objects_to_delete=objects_to_delete, partial=partial
+        )
```

## elemeno_ai_sdk/ml/features/feature_table.py

```diff
@@ -1,14 +1,15 @@
 import typing
 from google.protobuf.duration_pb2 import Duration
 import pandas as pd
 import datetime
 import feast
 from elemeno_ai_sdk import logger, config
 from feast.data_format import JsonFormat
+import feast.types
 from elemeno_ai_sdk.ml.features.types import FeatureType
 
 class FeatureTable:
   """ A FeatureTable is the object that is used to define feature tables on Elemeno feature store.
 
   If you're looking to create a new feature table or read data look at ingest_schema of the class FeatureStore.
   """
@@ -25,15 +26,15 @@
     self._features = [] if features is None else features
     self._feast_elm = feature_store
     self._duration = ttl_duration_weeks
     self._online = online
     self.is_streaming = is_streaming
     self._evt_col = event_column
     self._created_col = created_column
-    self._original_schema = []
+    self._original_schema = None
     self._table_schema = []
     self._elm_config = config.Configs.instance()
 
 
   @property
   def entities(self) -> typing.List[feast.Entity]:
     return self._entities
@@ -47,15 +48,15 @@
     return self._created_col
   
   @property
   def table_schema(self) -> typing.List[typing.Dict]:
     return self._table_schema
   
   @property
-  def original_schema(self) -> typing.List[typing.Dict]:
+  def original_schema(self) -> typing.Dict[str, typing.Any]:
     return self._original_schema
 
   @entities.setter
   def entities(self, value):
     self._entities = value
 
 
@@ -182,15 +183,15 @@
       event_timestamp_column=self.evt_col,
       created_timestamp_column=self.created_col
     )
 
     fv = feast.FeatureView(
       name = self.name,
       entities=self._entities,
-      features=self._features,
+      schema=[feast.Field(name=f.name, dtype=feast.types.from_value_type(f.dtype)) for f in self._features],
       online=self._online,
       source=ft_source,
       tags={}
     )
     self._feast_elm.apply(objects=self.entities)
     self._feast_elm.apply(objects=fv)
```

## elemeno_ai_sdk/ml/features/ingest/sink/__init__.py

```diff
@@ -1,3 +1,4 @@
 from .ingestion_sink_builder import IngestionSinkBuilder
 from .bigquery_ingestion import BigQueryIngestion
 from .redshift_ingestion import RedshiftIngestion
+from .ingestion_sink_builder import IngestionSinkType
```

## elemeno_ai_sdk/ml/features/ingest/sink/base_ingestion.py

```diff
@@ -19,17 +19,23 @@
       expected_columns: Optional[List[str]] = None, **kwargs) -> None:
     if ft.created_col not in to_ingest.columns:
       logger.warn("Could not find created_timestamp column in dataframe. Adding it now with default value.")
       to_ingest[ft.created_col] = pd.to_datetime('now', utc=True)
     if ft.evt_col not in to_ingest.columns:
       logger.warn("Could not find event_timestamp column in dataframe. Adding it now with default value.")
       to_ingest[ft.evt_col] = pd.to_datetime('now', utc=True)
+    if renames is not None:
+      to_ingest = to_ingest.rename(columns=renames)
+    if expected_columns is None or len(expected_columns) == 0:
+      logger.warning("No expected columns provided. Will ingest all columns.")
+      expected_columns = to_ingest.columns.to_list()
+    to_ingest = to_ingest.filter(expected_columns, axis=1)
 
   @abc.abstractmethod
-  def create_table(self, to_ingest: pd.DataFrame, ft_name: str, engine: Any, **kwargs) -> None:
+  def create_table(self, to_ingest: pd.DataFrame, ft_name: str, **kwargs) -> None:
     pass
 
   @abc.abstractmethod
   def staging_ingest(self, to_ingest: pd.DataFrame, name: str) -> None:
     pass
   
   @abc.abstractmethod
```

## elemeno_ai_sdk/ml/features/ingest/sink/bigquery_ingestion.py

```diff
@@ -1,14 +1,15 @@
 from datetime import datetime
 import json
 import typing
 import feast
 
 import pandas as pd
 from google.cloud import bigquery
+from google.cloud.exceptions import Conflict
 from elemeno_ai_sdk import logger
 from elemeno_ai_sdk.ml.features.feature_table import FeatureTable
 from elemeno_ai_sdk.ml.features.types import FeatureType
 from elemeno_ai_sdk.ml.features.ingest.sink.base_ingestion import Ingestion
 from elemeno_ai_sdk.ml.features.utils import create_insert_into
 
 class BigQueryIngestion(Ingestion):
@@ -95,11 +96,57 @@
       location = self._fs.config.offline_store.location
       dataframe.to_gbq(destination_table=f"{dataset}.{feature_table.name}",
           project_id=project_id, if_exists="append", location=location)
 
   def get_last_row(self, feature_table: 'FeatureTable', date_from: typing.Optional[datetime] = None, where: typing.Optional[typing.Dict[str, typing.Any]] = None) -> pd.DataFrame:
     raise(NotImplementedError("This method is not implemented yet."))
 
-def create_table(self, to_ingest: pd.DataFrame, ft_name: str, engine: typing.Any):
-  #TODO: implement
-  raise NotImplementedError("BigQueryIngestion.create_table is not implemented.")
+  def create_table(self, to_ingest: pd.DataFrame, table_name: str, project_id: str, dataset_id: str) -> pd.DataFrame:
+    """
+    Creates a table in BigQuery if it does not exist.
+
+    args:
+    
+    - to_ingest: DataFrame to ingest
+    - table_name: name of table to be created
+    - project_id: GCP project ID
+    - dataset_id: ID of the dataset in BigQuery
+
+    return:
+    
+    - DataFrame with columns in the same order as the FeatureTable
+    """
+    to_ingest = to_ingest.convert_dtypes()
+
+    date_cols = ["created_timestamp", "create_timestamp", "event_timestamp", "created_date", "record_date", "updated_date"]
+    
+    columns = {}
+    for col, dtype in to_ingest.dtypes.items():
+        if col == 'media' or 'media' in col.split('_'):
+            columns[f'{col}_status'] = 'BOOLEAN'
+            to_ingest[f'{col}_status'] = False
+        if col in date_cols:
+            columns[col] = "STRING"
+        else:
+            columns[col] = dtype.name
+
+    # create BigQuery client
+    bqclient = bigquery.Client(project=project_id)
+
+    # create dataset if it doesn't exist
+    dataset_ref = bqclient.dataset(dataset_id)
+    dataset = bigquery.Dataset(dataset_ref)
+    try:
+        bqclient.create_dataset(dataset)
+    except Conflict:
+        pass
+
+    # create table if it doesn't exist
+    table_ref = dataset_ref.table(table_name)
+    table = bigquery.Table(table_ref, schema=[bigquery.SchemaField(col, columns[col]) for col in columns])
+    try:
+        bqclient.create_table(table)
+    except Conflict:
+        pass
+
+    return to_ingest
```

## elemeno_ai_sdk/ml/features/ingest/sink/file_ingestion.py

```diff
@@ -4,13 +4,22 @@
 
 import pandas as pd
 
 
 class FileIngestion(abc.ABC):
 
   @abc.abstractmethod
-  def io_batch_ingest_from_df(self, to_ingest: pd.DataFrame, media_columns: List[str]):
+  def io_batch_ingest_from_df(self, to_ingest: pd.DataFrame, media_columns: List['MediaColumn']):
     pass
 
   @abc.abstractmethod
   def io_batch_ingest(self, to_ingest: List[Dict]):
-    pass
+    pass
+
+  @abc.abstractmethod
+  def io_batch_digest(self, feature_table_name: str, to_digest: pd.DataFrame, media_columns: List['MediaColumn']):
+    pass
+class MediaColumn:
+
+  def __init__(self, name: str, is_upload: bool):
+    self.name = name
+    self.is_upload = is_upload
```

## elemeno_ai_sdk/ml/features/ingest/sink/minio_ingestion.py

```diff
@@ -1,111 +1,193 @@
 
 import io
+import os
 import pandas as pd
 from typing import Dict, List, Optional
 from elemeno_ai_sdk.cos.minio import MinioClient
 from elemeno_ai_sdk.config import logging
 from multiprocessing import Pool, cpu_count
 from functools import partial
+from minio import S3Error
 import requests
 from elemeno_ai_sdk.config import Configs
-from elemeno_ai_sdk.ml.features.ingest.sink.file_ingestion import FileIngestion
+from elemeno_ai_sdk.ml.features.ingest.sink.file_ingestion import FileIngestion, MediaColumn
 
 class IngestionParams:
 
-  def __init__(self, minio_host: str, minio_user: str, minio_pass: str, minio_ssl: bool, 
-    media_path_col: str, to_ingest: Dict, dest_folder: Optional[str], 
+  def __init__(self, media_path_col: str, to_ingest: Dict, dest_folder: Optional[str], 
     dest_folder_col: Optional[str] = None, media_name_col: Optional[str] = None,
     minio_bucket: str = "elemeno-cos"):
 
-    self.minio_host = minio_host
-    self.minio_user = minio_user
-    self.minio_pass = minio_pass
-    self.minio_ssl = minio_ssl
     self.media_path_col = media_path_col
     self.dest_folder = dest_folder
     self.dest_folder_col = dest_folder_col
     self.media_name_col = media_name_col
     self.minio_bucket = minio_bucket
     self.to_ingest = to_ingest
+
+class DigestionParams:
+
+  def __init__(self, media_path_col: str, to_digest: Dict, remote_folder: Optional[str], 
+    remote_folder_col: Optional[str] = None, media_name_col: Optional[str] = None,
+    minio_bucket: str = "elemeno-cos"):
+
+    self.media_path_col = media_path_col
+    self.remote_folder = remote_folder
+    self.remote_folder_col = remote_folder_col
+    self.media_name_col = media_name_col
+    self.minio_bucket = minio_bucket
+    self.to_digest = to_digest
+
+def minio_client():
+  config = Configs.instance()
+  client = MinioClient(host=config.cos.host,
+    access_key=config.cos.key_id,
+    secret_key=config.cos.secret,
+    use_ssl=config.cos.use_ssl,)
+  return client
 class MinioIngestion(FileIngestion):
 
-  def io_batch_ingest_from_df(self, feature_table_name: str, to_ingest: pd.DataFrame, media_columns: List[str]):
-    config = Configs.instance()
-    local_path_cols = filter(lambda x: "http" not in x and "https" not in x, media_columns)
-    remote_path_cols = filter(lambda x: "http" in x or "https" in x, media_columns)
+  def __init__(self):
+    self.config = Configs.instance()
+    pass
+
+  def io_batch_ingest_from_df(self, feature_table_name: str, to_ingest: pd.DataFrame, media_columns: List[MediaColumn]):
+    local_path_cols = filter(lambda x: x if "http" not in x.name and "https" not in x.name else None, media_columns)
+    remote_path_cols = filter(lambda x: x if "http" in x.name or "https" in x.name else None, media_columns)
     df_dict = to_ingest.to_dict('records')
     for col in local_path_cols:
-      logging.info("Uploading {} files from media column {}".format(len(df_dict), col))
-      dest_folder_name = f"{feature_table_name}_{col}"
-      pool = Pool(cpu_count())
-      raw = map(lambda x: IngestionParams(config.cos.host, config.cos.key_id, config.cos.secret, config.cos.use_ssl,
-        media_path_col=col, to_ingest=x, dest_folder=dest_folder_name, minio_bucket=config.cos.bucket), df_dict)
-      upload_func = partial(self.upload_file_to_remote)
-      pool.map(upload_func, raw)
-      pool.close()
-      pool.join()
+      if col and col.is_upload:
+        logging.info("Uploading {} files from media column {}".format(len(df_dict), col.name))
+        dest_folder_name = f"{feature_table_name}_{col.name}"
+        pool = Pool(cpu_count())
+        raw = map(lambda x: IngestionParams(media_path_col=col.name, to_ingest=x, dest_folder=dest_folder_name, minio_bucket=self.config.cos.bucket), df_dict)
+        upload_func = partial(self.upload_file_to_remote)
+        pool.map(upload_func, raw)
+        pool.close()
+        pool.join()
     
     for col in remote_path_cols:
-      logging.info("Downloading {} files from media column {} to the remote persistence".format(len(df_dict), col))
-      pool = Pool(cpu_count())
-      raw = map(lambda x: IngestionParams(config.cos.host, config.cos.key_id, config.cos.secret, config.cos.use_ssl,
-        media_path_col=col, to_ingest=x, dest_folder=dest_folder_name, minio_bucket=config.cos.bucket), df_dict)
-      pool = Pool(cpu_count())
-      download_func = partial(self.download_file_to_remote)
-      pool.map(download_func, raw)
-      pool.close()
-      pool.join()
+      if col and not col.is_upload:
+        logging.info("Downloading {} files from media column {} to the remote persistence".format(len(df_dict), col))
+        pool = Pool(cpu_count())
+        raw = map(lambda x: IngestionParams(media_path_col=col.name, to_ingest=x, dest_folder=dest_folder_name, minio_bucket=self.config.cos.bucket), df_dict)
+        pool = Pool(cpu_count())
+        download_func = partial(self.download_file_to_remote)
+        pool.map(download_func, raw)
+        pool.close()
+        pool.join()
     logging.info("Finished processing binary files ingestion")
     return None
 
   def io_batch_ingest(self, to_ingest: List[Dict]):
-    config = Configs.instance()
+    config = self.config
     print("prepare map")
-    raw = map(lambda x: IngestionParams(config.cos.host, 
-          config.cos.key_id, config.cos.secret, config.cos.use_ssl,
-          config.feature_store.source.params.binary.media_id_col, config.feature_store.source.params.binary.media_url_col,
+    raw = map(lambda x: IngestionParams(config.feature_store.source.params.binary.media_id_col, config.feature_store.source.params.binary.media_url_col,
           config.feature_store.source.params.binary.dest_folder_col,
           to_ingest=x), to_ingest)
     pool = Pool(cpu_count())
     download_func = partial(self.download_file_to_remote)
     print("start map for downloading files")
     pool.map(download_func, raw)
     pool.close()
     pool.join()
     return None
+  
+  def _remove_duplicates(self, df_dict, media_columns):
+    """
+    Remove duplicated rows from a list of dictionaries based on the values of
+    the specified media columns.
+    
+    Parameters:
+    - df_dict: a list of dictionaries representing a DataFrame
+    - media_columns: a list of column names to use as the criteria for detecting duplicates
+    
+    Returns:
+    A list of dictionaries with duplicated rows removed based on the specified media columns.
+    """
+    unique_rows = []
+    seen_media = set()
+    for row in df_dict:
+        media = tuple(row[col.name] for col in media_columns)
+        if media not in seen_media:
+            unique_rows.append(row)
+            seen_media.add(media)
+    return unique_rows
+  
+  def io_batch_digest(self, feature_table_name: str, to_digest: pd.DataFrame, media_columns: List['MediaColumn']):
+    # guarantee unique values on medias
+    df_dict = to_digest.to_dict('records')
+    # remove duplicated records from the dict
+    self._remove_duplicates(df_dict, media_columns)
+    for col in media_columns:
+      logging.info("Downloading {} files from media column {}".format(len(to_digest), col.name))
+      remote_folder_name = f"{feature_table_name}_{col.name}"
+      pool = Pool(cpu_count())
+      raw = map(lambda x: DigestionParams(media_path_col=col.name, to_digest=x, remote_folder=remote_folder_name, minio_bucket=self.config.cos.bucket), df_dict)
+      download_func = partial(self.download_file_from_remote)
+      pool.map(download_func, raw)
+      pool.close()
+      pool.join()
+    logging.info("Finished processing binary files digestion")
+    return None
+
+
+  def download_file_from_remote(self, p: 'DigestionParams'):
+    client = minio_client()
+    logging.info("Processing {}".format(type(p)))
+    
+    to_digest = p.to_digest
+    file_path = to_digest[p.media_path_col]
+    file_path = os.path.normpath(file_path)
+    folder_remote = to_digest[p.remote_folder_col] if p.remote_folder_col else p.remote_folder
+    # remove ./ from the file name when it's present
+    folder_remote = os.path.normpath(folder_remote)
+    bucket = p.minio_bucket
+
+    # check if bucket exists on minio
+    if not client.bucket_exists(bucket):
+      raise ValueError("The specified bucket does not exists")
+
+    try:
+      local_folder = ".binaries"
+      if not os.path.exists(local_folder):
+        os.makedirs(local_folder)
+      local_file_path = os.path.join(local_folder, folder_remote, file_path)
+
+      client.get_object(bucket, f"{folder_remote}/{file_path}", local_file_path)
+      logging.debug("Downloaded file {} from bucket {} and folder {}".format(file_path, bucket, folder_remote))
+    except (Exception, S3Error) as e:
+      logging.error("Error downloading file {} from bucket {} and folder {}. Error: {}".format(file_path, bucket, folder_remote, e))
+    return None
 
   def upload_file_to_remote(self, p: 'IngestionParams'):
+    client = minio_client()
     logging.info("Processing {}".format(type(p)))
-    client = MinioClient(host=p.minio_host,
-      access_key=p.minio_user,
-      secret_key=p.minio_pass,
-      use_ssl=p.minio_ssl)
 
     to_ingest = p.to_ingest
     file_path = to_ingest[p.media_path_col]
-    folder_remote = to_ingest[p.dest_folder_col] if p.dest_folder_col else to_ingest[p.dest_folder_col]
+    file_path = os.path.normpath(file_path)
+    folder_remote = to_ingest[p.dest_folder_col] if p.dest_folder_col else p.dest_folder
+    folder_remote = os.path.normpath(folder_remote)
     bucket = p.minio_bucket
     
     try:
       with open(file_path, 'rb') as file_data:
-        client.put_object(bucket, f"{folder_remote}/{file_path}", io.BytesIO(file_data))
+        file_contents = file_data.read()
+        client.put_object(bucket, f"{folder_remote}/{file_path}", io.BytesIO(file_contents))
         logging.debug("Uploaded file {} to bucket {} and folder {}".format(file_path, bucket, folder_remote))
     except Exception as e:
       logging.error(f"error uploading file {file_path} to folder: {folder_remote}")
       logging.error(e)
     pass
 
   def download_file_to_remote(self, p: 'IngestionParams'):
     try:
       logging.error("Processing {}".format(type(p)))
-      client = MinioClient(host=p.minio_host,
-        access_key=p.minio_user,
-        secret_key=p.minio_pass,
-        use_ssl=p.minio_ssl)
       
       headers = {"user-agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/100.0.4896.127 Safari/537.36"}
       to_ingest = p.to_ingest
       media_id = to_ingest[p.media_id_col]
       media_url = to_ingest[p.media_url_col].replace("\\", "")
       folder_id = to_ingest[p.dest_folder_col]
       position = to_ingest['position']
@@ -115,15 +197,15 @@
       content_type = r.headers['content-type']
       logging.error("Will check image")
       if content_type.startswith('image'):
           logging.error("Image found")
           st = io.BytesIO(r.content)
           media_extension = media_url.split('.')[-1]
           try:
-              client.put_object('elemeno-cos', f"binary_data_parallel/{folder_id}/{position}_{media_id}.{media_extension}", st)
+              self.client.put_object('elemeno-cos', f"binary_data_parallel/{folder_id}/{position}_{media_id}.{media_extension}", st)
               logging.error("uploaded path: " + f"binary_data_parallel/{folder_id}/{position}_{media_id}.{media_extension}")
           except Exception as e:
               logging.error("error uploading file to folder: " + folder_id)
               logging.error(e)
       else:
         logging.error(f'{media_id}: {media_url}')
         logging.error("Not an image")
```

## elemeno_ai_sdk/ml/features/ingest/sink/redshift_ingestion.py

```diff
@@ -90,20 +90,14 @@
     
     - to_ingest: DataFrame to ingest
     - ft: FeatureTable to ingest to
     - renames: Optional dictionary of column names to rename
     - expected_columns: Optional list of columns to check for
     """
     super().ingest(to_ingest, ft, renames, expected_columns)
-    if renames is not None:
-      to_ingest = to_ingest.rename(columns=renames)
-    if expected_columns is None or len(expected_columns) == 0:
-      logger.warning("No expected columns provided. Will ingest all columns.")
-      expected_columns = to_ingest.columns.to_list()
-    to_ingest = to_ingest.filter(expected_columns, axis=1)
     conn = self._conn
     try:
       logger.info("Within RedshiftIngestion.ingest, about to create table {}".format(ft.name))
       # create table if not exists
       to_ingest = self.create_table(to_ingest, ft.name, conn)
       # ingest data
       max_rows_per_insert = 5000
```

## elemeno_ai_sdk/ml/features/ingest/sink/redshift_test_ingestion.py

```diff
@@ -1,17 +1,19 @@
 
 from elemeno_ai_sdk.ml.features.ingest.sink.redshift_ingestion import RedshiftIngestion
+from elemeno_ai_sdk.ml.features.feature_table import FeatureTable
+import typing
 
 
 class RedshiftTestIngestion(RedshiftIngestion):
-    def __init__(self, fs, connection_string: str):
-      super().__init__(fs, connection_string=connection_string)
-      self.rs_types = {
-        "object": "BLOB",
-        "string[python]": "TEXT",
-        "string": "TEXT",
-        "Int64": "INTEGER",
-        "Int32": "INTEGER",
-        "Float64": "REAL",
-        "bool": "INTEGER",
-        "datetime64[ns]": "TEXT"
-      }
+  def __init__(self, fs, connection_string: str):
+    super().__init__(fs, connection_string=connection_string)
+    self.rs_types = {
+      "object": "BLOB",
+      "string[python]": "TEXT",
+      "string": "TEXT",
+      "Int64": "INTEGER",
+      "Int32": "INTEGER",
+      "Float64": "REAL",
+      "bool": "INTEGER",
+      "datetime64[ns]": "TEXT"
+    }
```

## elemeno_ai_sdk/ml/features/ingest/source/base_source.py

```diff
@@ -1,14 +1,14 @@
 import abc
 from typing import Dict, List, Optional
 import pandas as pd
 
 
 class ReadResponse:
-  def __init__(self, dataframe: pd.DataFrame, prepared_medias: Optional[str]):
+  def __init__(self, dataframe: pd.DataFrame, prepared_medias: Optional[str] = None):
     self.dataframe = dataframe
     self.prepared_medias = prepared_medias
 class BaseSource(abc.ABC):
 
   def __init__(self, **kwargs):
     self.source_type = type(self).__name__
```

## elemeno_ai_sdk/ml/features/ingest/source/elastic.py

```diff
@@ -9,22 +9,22 @@
 class ElasticIngestionSource(BaseSource):
 
   def __init__(self, host: str, username: str, password: str):
     super().__init__()
     self._es = Elasticsearch(hosts=[host],
             http_auth=(username, password))
   
-  def read(self, index: str = "", query: str = "", max_per_page: int = 1000, max_pages: Optional[int] = None, 
+  def read(self, index: str = "", base_query: str = "", max_per_page: int = 1000, max_pages: Optional[int] = None, 
     binary_columns: Optional[List[str]] = None, media_id_col: Optional[str] = None, dest_folder_col: Optional[str] = None) -> ReadResponse:
     """ Reads data from elastic.
 
     args:
     
     - index: The index to read from.
-    - query: The query to use.
+    - base_query: The query to use.
     - max_per_page: The maximum number of records to read per page.
     - binary_columns: A list of columns containing links to binary files (jpeg, pdf, etc) that will be downloaded by a Sink.
     - media_id_col: The column containing the media id.
     - dest_folder_col: The column containing the destination folder.
   
     return:
     
@@ -78,24 +78,24 @@
     return ReadResponse(dataframe=df, prepared_medias=json.dumps(binary_prepared))
 
   def _add_to_prepard_medias(self, binary_columns: List[str], media_id_col: str, dest_folder_col: str, res: Dict, prepared_medias: List = []):
     if binary_columns is not None:
       for bin_col in binary_columns:
         prepared_medias.extend(self.prepare_medias(res['hits']['hits'], bin_col, media_id_col, dest_folder_col))
 
-  def read_after(self, timestamp_str: str, index: str = "", query: str = "", max_per_page: int = 1000, 
+  def read_after(self, timestamp_str: str, index: str = "", base_query: str = "", max_per_page: int = 1000, 
     binary_columns: Optional[List[str]] = None, media_id_col: Optional[str] = None, dest_folder_col: Optional[str] = None) -> ReadResponse:
     """ Read data after a given timestamp. 
     When using this function you can't specify a range filter in the query.
 
     args:
     
     - timestamp_str: A string representing a timestamp. It should have the same format used in the source elastic.
     - index: The index to read from.
-    - query: The query to use.
+    - base_query: The query to use.
     - max_per_page: The maximum number of records to read per page.
     - binary_columns: A list of columns containing links to binary files (jpeg, pdf, etc) that will be downloaded by a Sink.
     - media_id_col: The column containing the media id.
     - dest_folder_col: The column containing the destination folder.
     
     return:
```

## elemeno_ai_sdk/ml/features/ingest/source/ingestion_source_builder.py

```diff
@@ -76,38 +76,45 @@
     """
     if project_id is None:
       project_id = self._config.feature_store.source.params.project_id
     self.type = IngestionSourceType.BIGQUERY
     return BigQueryIngestionSource(gcp_project_id=project_id, base_query=base_query)
 
   def build_redshift(self, cluster_name: Optional[str]=None, host: Optional[str]=None,
-    port: Optional[int]=None, user: Optional[str]=None, password: Optional[str]=None, database: Optional[str]=None, base_query: Optional[str]=None) -> RedshiftIngestionSource:
+    port: Optional[int]=None, user: Optional[str]=None, password: Optional[str]=None, database: Optional[str]=None, base_query: Optional[str]=None,
+    iam_role: Optional[str]=None) -> RedshiftIngestionSource:
     """ Builds a Redshift ingestion source instance.
     
     args:
     
     - cluster_name: The name of the Redshift cluster. When specified we will use IAM authentication.
     - host: The host of the Redshift instance. Not used when cluster_name is specified.
     - port: The port of the Redshift instance. Not used when cluster_name is specified.
     - user: The username of the Redshift instance. Not used when cluster_name is specified.
     - password: The password of the Redshift instance. Not used when cluster_name is specified.
     - database: The name of the Redshift database.
     - base_query: The base query to be used to query the Redshift.
+    - iam_role: The IAM role to be used to query the Redshift. Not used when cluster_name is not specified.
     
     return:
     
     - A Redshift ingestion source instance.
     """
     if cluster_name is None:
       cluster_name = self._config.feature_store.source.params.cluster_name
     if database is None:
       database = self._config.feature_store.source.params.database
     if host is None:
       host = self._config.feature_store.source.params.host
     if port is None:
       port = self._config.feature_store.source.params.port
     if user is None:
-      user = self._config.feature_store.source.params.user
+      if hasattr(self._config.feature_store.source.params, "user"):
+        user = self._config.feature_store.source.params.user
     if password is None:
-      password = self._config.feature_store.source.params.password
+      if hasattr(self._config.feature_store.source.params, "password"):
+        password = self._config.feature_store.source.params.password
+    if iam_role is None:
+      if hasattr(self._config.feature_store.source.params, "iam_role"):
+        iam_role = self._config.feature_store.source.params.iam_role
     self.type = IngestionSourceType.REDSHIFT
-    return RedshiftIngestionSource(cluster_name=cluster_name, database=database, base_query=base_query)
+    return RedshiftIngestionSource(cluster_name=cluster_name, user=user, database=database, base_query=base_query, iam_role=iam_role)
```

## elemeno_ai_sdk/ml/features/ingest/source/redshift.py

```diff
@@ -1,73 +1,92 @@
 from typing import Optional
 import pandas as pd
 
 import redshift_connector
 
-from elemeno_ai_sdk.ml.features.ingest.source.base_source import BaseSource
+from elemeno_ai_sdk.ml.features.ingest.source.base_source import BaseSource, ReadResponse
 
 MAX_LINES_TO_IMPORT = 10000
 
 
 # TODO Add sql metadata validation
 class RedshiftIngestionSource(BaseSource):
 
     def __init__(self, database: str, cluster_name: Optional[str]=None, base_query: Optional[str]=None,
-      host: Optional[str]=None, port: Optional[int]=None, user: Optional[str]=None, password: Optional[str]=None):
+      host: Optional[str]=None, port: Optional[int]=None, user: Optional[str]=None, password: Optional[str]=None,
+      iam_role: Optional[str]=None):
       """ Initializes a Redshift ingestion source.
       
       args:
 
       - database: The name of the database.
       - cluster_name: The name of the cluster. Used when IAM authentication.
       - base_query: The base query to be used to query the Redshift.
       - host: The host of the Redshift instance.
       - port: The port of the Redshift instance.
       - user: The username of the Redshift instance.
       - password: The password of the Redshift instance.
+      - iam_role: The IAM role to be used to query the Redshift.
 
       """
-      if cluster_name is not None and (host is not None or port is not None or user is not None or password is not None):
-        raise ValueError("When specifying cluster name you cannot specify host, port, user or password")
+      # if cluster_name is not None and (host is not None or port is not None or user is not None or password is not None):
+      #   raise ValueError("When specifying cluster name you cannot specify host, port, user or password")
       self.host = host
       self.port = port
       self.user = user
       self.password = password
       self.cluster_name = cluster_name
       self.base_query = base_query
       self.database = database
+      self.iam_role = iam_role
 
-    def read(self, base_query: Optional[str]=None, **kwargs) -> pd.DataFrame:
+    def read(self, base_query: Optional[str]=None, **kwargs) -> ReadResponse:
       """ Reads data from the Redshift source.
 
       args:
 
       - base_query: The base query to be used to query the Redshift.
 
       return:
 
       - A dataframe containing the data.
       """
       if base_query is not None:
         self.base_query = base_query
-      with redshift_connector.connect(
-          iam=True,
-          database=self.database,
-          db_user='awsuser',
-          password='',
-          user='',
-          cluster_identifier=self.cluster_name,
-          profile='default'
-      ) as conn:
-        with conn.cursor() as cursor:
-          conn.autocommit = True
-          cursor.execute(" {} ".format(self.base_query))
-          return cursor.fetch_dataframe()
+      if self.iam_role is not None:
+        with redshift_connector.connect(
+            iam=True,
+            database=self.database,
+            db_user=self.user,
+            password='',
+            user='',
+            cluster_identifier=self.cluster_name,
+            profile='default',
+            preferred_role=self.iam_role,
+        ) as conn:
+          with conn.cursor() as cursor:
+            conn.autocommit = True
+            cursor.execute(self.base_query)
+            return ReadResponse(dataframe=cursor.fetch_dataframe())
+      else:
+        with redshift_connector.connect(
+            iam=False,
+            database=self.database,
+            db_user=self.user,
+            password=self.password,
+            user=self.user,
+            cluster_identifier=self.cluster_name,
+            profile='default',
+        ) as conn:
+          with conn.cursor() as cursor:
+            conn.autocommit = True
+            cursor.execute(self.base_query)
+            return ReadResponse(dataframe=cursor.fetch_dataframe())
 
-    def read_after(self, timestamp_str: str, base_query: Optional[str] = None, **kwargs) -> pd.DataFrame:
+    def read_after(self, timestamp_str: str, base_query: Optional[str] = None, **kwargs) -> ReadResponse:
       """ Reads data from the Redshift source after a certain timestamp.
 
       args:
 
       - timestamp_str: The timestamp after which to read data.
       - base_query: The base query to be used to query the Redshift.
```

## Comparing `elemeno_ai_sdk-0.4.9.dist-info/LICENSE` & `elemeno_ai_sdk-0.5.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `elemeno_ai_sdk-0.4.9.dist-info/LICENSE-3RDPARTY.txt` & `elemeno_ai_sdk-0.5.4.dist-info/LICENSE-3RDPARTY.txt`

 * *Files identical despite different names*

## Comparing `elemeno_ai_sdk-0.4.9.dist-info/METADATA` & `elemeno_ai_sdk-0.5.4.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elemeno-ai-sdk
-Version: 0.4.9
+Version: 0.5.4
 Summary: A set of glue code and utilities to make using elemeno AI platform a smooth experience
 Home-page: https://gitlab.com/elemeno-ai/python-elemeno-ai-sdk
 Author: Lucas Bonatto Miguel
 Author-email: developer@elemeno.ai
 License: Apache-2.0
 Project-URL: Issue Tracker, https://gitlab.com/elemeno-ai/python-elemeno-ai-sdk/issues
 Keywords: artificial intelligence,ai,machine learning,ml,sdk,elemeno,mlops
@@ -22,35 +22,34 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
-Requires-Dist: feast[aws,gcp,redis] (==0.26.0)
+Requires-Dist: feast[aws,gcp,redis] (==0.31.0)
 Requires-Dist: GitPython (==3.1.26)
-Requires-Dist: google-auth-oauthlib (==0.4.6)
 Requires-Dist: Jinja2 (==3.0.3)
 Requires-Dist: mlflow (==1.26.1)
 Requires-Dist: numpy (>=1.22)
-Requires-Dist: omegaconf (==2.1.0)
-Requires-Dist: onnx (==1.10.2)
+Requires-Dist: omegaconf (>=2.1.0)
 Requires-Dist: pandas (>=1.2.4)
 Requires-Dist: pandas-gbq (==0.15.0)
-Requires-Dist: protobuf (<5,>3)
-Requires-Dist: setuptools (==53.0.0)
+Requires-Dist: setuptools (>=59.5.0)
 Requires-Dist: sphinx-rtd-theme (==1.0.0)
 Requires-Dist: tf2onnx (==1.9.3)
+Requires-Dist: onnxruntime (>=1.8.1)
 Requires-Dist: elasticsearch[async] (==8.1.3)
-Requires-Dist: redshift-connector (==2.0.904)
-Requires-Dist: sqlalchemy-redshift (==0.8.9)
+Requires-Dist: redshift-connector (==2.0.911)
+Requires-Dist: sqlalchemy-redshift (==0.8.14)
 Requires-Dist: typer (==0.6.1)
 Requires-Dist: psycopg2-binary (==2.9.4)
 Requires-Dist: pyspark (==3.3.0)
 Requires-Dist: asyncio (==3.4.3)
+Requires-Dist: minio (>=7.1.3)
 
 ========
 Overview
 ========
 
 A set of glue code and utilities to make using elemeno AI platform a smooth experience
```

## Comparing `elemeno_ai_sdk-0.4.9.dist-info/RECORD` & `elemeno_ai_sdk-0.5.4.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-elemeno_ai_sdk/__init__.py,sha256=VWMeMu8UQHfA9s5GkncjqBruLbTvYrVWlr-hiGuuxEg,235
+elemeno_ai_sdk/__init__.py,sha256=tneVjSi5aGZhlDaN1rGJWQE6sczqLsBSw1P-qH0jxpM,235
 elemeno_ai_sdk/__main__.py,sha256=yt95v6S5o46xfSPSFPe7-vsmQg-ChV-5ChINupX_e9I,375
 elemeno_ai_sdk/cli.py,sha256=Wf2sLpT8PWylBeyxQ-Wz6d6Ri4j6bBt8x2NxUe3nTKM,935
-elemeno_ai_sdk/config.py,sha256=XurrulDd_8JY_Jdt0pQmFgHvNC923T8vaMZ3erCR-G4,1143
+elemeno_ai_sdk/config.py,sha256=Cg1nwE7r-L857YxruK0VxAuOlx9nBKdXWB3uXV9ZTPE,2406
 elemeno_ai_sdk/cos/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 elemeno_ai_sdk/cos/base_cos.py,sha256=0VYeRPCVUdo94KxQE9Ayc09vm0YG4_dZof_6XGVyfXE,680
-elemeno_ai_sdk/cos/minio.py,sha256=2lCNw1bL1_I9z2GCRUUdqombinACEKU21aYj_h2skLE,2279
+elemeno_ai_sdk/cos/minio.py,sha256=Usdea0yB1-J-F1-LcjmXlvIOok3TnU0HziTjUqbFmAc,2404
 elemeno_ai_sdk/cos/s3.py,sha256=n4eR1_wCr-tuoNbMug9MYAZ1MMhDstY-MaVwUvchabM,3421
 elemeno_ai_sdk/cos/file_utils/__init__.py,sha256=HLIRYTDkAABLYzYupLEQDPL9MXRdiUHeRqzVijcjzeM,32
 elemeno_ai_sdk/cos/file_utils/elastic_to_cos copy.py,sha256=HwgsVkLoJ4oa-96QgDYERMRuv7TslHOFe7uZNu5TBZ8,10897
 elemeno_ai_sdk/cos/file_utils/elastic_to_cos.py,sha256=c43Nn4N3IiNcC61JhnjgA3Y-tV1kzqFjZCpVH9zXDQs,5426
 elemeno_ai_sdk/cos/file_utils/elastic_to_cos_dask.py,sha256=AmmP0F_pXUQwKRK-j45b1ZdBYROdqOBDpuOIYwI-hH0,3408
 elemeno_ai_sdk/cos/file_utils/zip_utils.py,sha256=s6XZz2Fi3gnd0YI2N7u0L14ZW0qX9azDgepk3AzbT74,1456
 elemeno_ai_sdk/cos/types/__init__.py,sha256=F7WNj5gXv-j0KSxPO75sem1GKrNGIVhvr78-it2tELA,33
@@ -21,50 +21,46 @@
 elemeno_ai_sdk/ml/conversion/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 elemeno_ai_sdk/ml/conversion/converter.py,sha256=PP0krZnkzzu3vBQS718FqC2K4CyNCpZeV6sGBsFRPCo,1245
 elemeno_ai_sdk/ml/conversion/converter_abc.py,sha256=gLCkeB6YDpcQqpcVHV1vCiHiXA_jJMMhLMecgd7BfV0,1072
 elemeno_ai_sdk/ml/conversion/sklearn.py,sha256=RPypjj0qCyMKH7ppRIxe6ZkkTMZhBMf0rbIyR6Uue8o,1150
 elemeno_ai_sdk/ml/conversion/tensorflow.py,sha256=P7wYGoVvAWYeC28SjkZM2ImPl-_J-cVEuf_mamkSMSc,1271
 elemeno_ai_sdk/ml/conversion/tflite.py,sha256=IQNF4rk2rO7jR-dWXqec8Iit1LHsU8bUlwCcvKZ8BxM,1425
 elemeno_ai_sdk/ml/conversion/torch.py,sha256=rpbBlWtb33VMv-wjVjsoMWxd3EDPw0-VsCdjr-fZK_4,940
-elemeno_ai_sdk/ml/conversion/.ipynb_checkpoints/converter_abc-checkpoint.py,sha256=gLCkeB6YDpcQqpcVHV1vCiHiXA_jJMMhLMecgd7BfV0,1072
-elemeno_ai_sdk/ml/conversion/.ipynb_checkpoints/tensorflow-checkpoint.py,sha256=qopSm6qfVE_EkElUIaauCxkW_m4iM0o3gSRJTVQ_EWc,919
-elemeno_ai_sdk/ml/conversion/.ipynb_checkpoints/tflite-checkpoint.py,sha256=cjNmh7XSQ4HYm_u4yWm3GLNk0qIjq_-pOTYdk5gpKMc,996
-elemeno_ai_sdk/ml/conversion/.ipynb_checkpoints/torch-checkpoint.py,sha256=WhU1QQXpFj3HHWamHk8H1S0JrXjs-bU0Nf1suOt3lI4,755
 elemeno_ai_sdk/ml/features/__init__.py,sha256=xTCm_hc8vlwsOHdthSBnoeSrnEW55eXPx00xQfXE-40,245
-elemeno_ai_sdk/ml/features/feature_store.py,sha256=GMa4_AVHxcdCtxUrBFsE76qS0t8iDB8T5neQqV1MqDI,19542
-elemeno_ai_sdk/ml/features/feature_table.py,sha256=8zTNyQYuEogHfQLHea9cXtGM4euNU6CiVMtMBUBfvLk,6447
-elemeno_ai_sdk/ml/features/materialize.py,sha256=Dc3r4QxMOqx3Ha2bHVFJizViAA-jpPI4psxsG3UWx70,551
+elemeno_ai_sdk/ml/features/feature_store.py,sha256=w-V0CNJS75QC5bUcY8NBg6vzqEuTxqjxU1Ekay6r4eo,27287
+elemeno_ai_sdk/ml/features/feature_table.py,sha256=KE96qHS0z0saY0U8yYI8ddjM7CC6oqWbSN9pP_UxOw8,6550
 elemeno_ai_sdk/ml/features/query.py,sha256=mWBzVFXqM4d4EYkYGfLpNyb_VvPv6kutCboljtN2ZrI,3886
 elemeno_ai_sdk/ml/features/types.py,sha256=weHBDUrEHY6mHy1Bxx62DKjYm43IeOiSAujKBvgK6yg,5496
 elemeno_ai_sdk/ml/features/utils.py,sha256=PTAKtvTFtNnfyr0EKL3UJ38ovSkaf2oyVQiPHR4upLs,292
+elemeno_ai_sdk/ml/features/config/repo_config.py,sha256=NXbLsK58PCPPiVw_bAdn5LngpEiKN8xvedNAb_xAJbM,2340
 elemeno_ai_sdk/ml/features/ingest/__init_.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-elemeno_ai_sdk/ml/features/ingest/sink/__init__.py,sha256=Y4lxBZLaCjGAQxaCNozNrQOW1hF-fClRpUXgRwdt9EM,157
-elemeno_ai_sdk/ml/features/ingest/sink/base_ingestion.py,sha256=7e9KgOk1UbQw-gIH3LjMobUXZaSvsmKolc8x1B9raNA,1997
-elemeno_ai_sdk/ml/features/ingest/sink/bigquery_ingestion.py,sha256=q2WZ7KpKYRS-lH2ZKXDd6BGuzcfB6TkuI7CZSO2zOsE,5494
-elemeno_ai_sdk/ml/features/ingest/sink/file_ingestion.py,sha256=0iv__CrJHPaOQSPxDOlbsKKqoKHoQ_TM_Jhp2bumdKQ,298
+elemeno_ai_sdk/ml/features/ingest/sink/__init__.py,sha256=aZarrt04grEE3FNZw7BT4myrxs6xchMR3da9l7N_nfI,210
+elemeno_ai_sdk/ml/features/ingest/sink/base_ingestion.py,sha256=xBe4OEmGM1M86NLAcUuqjhyunoDB5uDcPlZGkpxzAng,2318
+elemeno_ai_sdk/ml/features/ingest/sink/bigquery_ingestion.py,sha256=hFV-XGxeXRA7GHcLPsAX8KxG5933ds18N3eOv_0Gja4,6908
+elemeno_ai_sdk/ml/features/ingest/sink/file_ingestion.py,sha256=TTy0CPB0wbh7sEbcHXRajJFmqiwdmVoDW9DjYlcr9wY,577
 elemeno_ai_sdk/ml/features/ingest/sink/ingestion_sink_builder.py,sha256=2WhEbZ6Gn6Z12zq9YfoP6VWAiiSL2w3GkmOKNHpt6fI,1922
-elemeno_ai_sdk/ml/features/ingest/sink/minio_ingestion.py,sha256=0NZwcmqRoeT6Pq25GsfaUyr95yYs6HPzh6FN7A3zX3s,5838
-elemeno_ai_sdk/ml/features/ingest/sink/redshift_ingestion.py,sha256=Wo4WifVC-XqYNmiMDOyiqfkcglWrOzjFSh-ypXF0aU4,10380
-elemeno_ai_sdk/ml/features/ingest/sink/redshift_test_ingestion.py,sha256=mkjUvfK9PxzawelBaVrN7Sg-yPhQ8CgVUeRRIibrwhQ,515
+elemeno_ai_sdk/ml/features/ingest/sink/minio_ingestion.py,sha256=JSOfBvZJqTmqToUZWAP5nVCocNL46t92geI1e0twm9I,9050
+elemeno_ai_sdk/ml/features/ingest/sink/redshift_ingestion.py,sha256=McbW8FOXFjieWdSromwtuAi7vKJQyN2jSSEIc2AlF10,10046
+elemeno_ai_sdk/ml/features/ingest/sink/redshift_test_ingestion.py,sha256=kYbQl4-Y5HC2x9mKrKcM9vL0haX288aCkTPRvNg3_GE,571
 elemeno_ai_sdk/ml/features/ingest/source/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-elemeno_ai_sdk/ml/features/ingest/source/base_source.py,sha256=XdRAqxjHJp5NbS_PjvOWsRNNyYFh5Z9NbgUQpIOFtu0,528
+elemeno_ai_sdk/ml/features/ingest/source/base_source.py,sha256=rnp73IQhOYXeUlndVUtXRdKCJ7MbymfvBKnkvTmf_TE,535
 elemeno_ai_sdk/ml/features/ingest/source/bigquery.py,sha256=Rnc5m3YjKPZW0JUSHCnJtPFSf6iDCcUhdI_TOSkYkhM,1854
-elemeno_ai_sdk/ml/features/ingest/source/elastic.py,sha256=RFQoow3DcVOM9s_j8uuadKGXruWT72eJrzq_WYHRlpI,6260
+elemeno_ai_sdk/ml/features/ingest/source/elastic.py,sha256=W0HME1ftDwv9O6b5vOT6_AFE-TRr-u_rT9dxZB8S2LY,6280
 elemeno_ai_sdk/ml/features/ingest/source/gcs.py,sha256=k8sZWE7iARrkUEk97AdX9gmFz8znFhgjYw9AXOxuxFw,1385
-elemeno_ai_sdk/ml/features/ingest/source/ingestion_source_builder.py,sha256=l5SHp3DHoGi32_Unf6QSB6g4lqwBOialCzr5iThxkOw,4483
-elemeno_ai_sdk/ml/features/ingest/source/redshift.py,sha256=_fK0vKX1MvwhQqj9BvrRsmWPRsfAhbqT_WUPyUbPHBU,2836
+elemeno_ai_sdk/ml/features/ingest/source/ingestion_source_builder.py,sha256=ASgCJpWbgM7unPX7o8qCDrm9ZO4fmzhpIL_WHotY4gQ,4965
+elemeno_ai_sdk/ml/features/ingest/source/redshift.py,sha256=xc22R2lr_wDRJ9PYc1llJBpEBdkCmm_dZ1J9x653NNQ,3594
 elemeno_ai_sdk/ml/features/transform/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 elemeno_ai_sdk/ml/features/transform/dsl/base_ops.py,sha256=rr1rnbtIVwKsPTNLiIk6a8-bvvlVmsmSEw8066OMDjM,901
 elemeno_ai_sdk/ml/features/transform/dsl/functions/__init__.py,sha256=zhJ5qjunoVxG7iwu4Wo28snictQHiYGaQ_D3EVwXopE,40
 elemeno_ai_sdk/ml/features/transform/dsl/functions/change_shape.py,sha256=VbXCCA2mwTHWshYecaeumOoUxMkq_ya4u3_X18XyT8I,2107
 elemeno_ai_sdk/ml/inference/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 elemeno_ai_sdk/ml/inference/client.py,sha256=ZNDZ3swpxKSmxOGfZOkWgrKMUkX7YnbTe3B37omi9S4,1424
 elemeno_ai_sdk/ml/inference/inference_response.py,sha256=rLIdfkTSWK-Zgr78rpVB1Cxrt31VF5jxh2ePIi_LQqU,457
 elemeno_ai_sdk/ml/inference/input_space.py,sha256=ddgTFxVG8S7UtwE85spvzYZmZekRzWXQf0VEBvgiP2A,1819
-elemeno_ai_sdk-0.4.9.dist-info/AUTHORS.rst,sha256=F4ZoKcTVHGREVA68Zxz8kXkQKMHkm-psRPOX15aEfTs,66
-elemeno_ai_sdk-0.4.9.dist-info/LICENSE,sha256=T3q_vT9bSF7O8zKxgQJkaqHfegAG9AMYQ2USuMd6kKw,592
-elemeno_ai_sdk-0.4.9.dist-info/LICENSE-3RDPARTY.txt,sha256=MXgzdAQL8HCYjE4UyFDtb7goq-4y6d6Hxu5x753NRns,15965
-elemeno_ai_sdk-0.4.9.dist-info/METADATA,sha256=iBd9F-zfsEZGvDmvzR4A5EWpkEBjsTgzXZtBGlfy9bQ,3156
-elemeno_ai_sdk-0.4.9.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-elemeno_ai_sdk-0.4.9.dist-info/entry_points.txt,sha256=MxLJDKUD5b4cVYFBMFH0Urs8zDxznly_99y2C40uXc0,53
-elemeno_ai_sdk-0.4.9.dist-info/top_level.txt,sha256=xq4olxjXm95p4Y71rv-7qTYMyA9XXuZfFHestuoZovo,15
-elemeno_ai_sdk-0.4.9.dist-info/RECORD,,
+elemeno_ai_sdk-0.5.4.dist-info/AUTHORS.rst,sha256=F4ZoKcTVHGREVA68Zxz8kXkQKMHkm-psRPOX15aEfTs,66
+elemeno_ai_sdk-0.5.4.dist-info/LICENSE,sha256=T3q_vT9bSF7O8zKxgQJkaqHfegAG9AMYQ2USuMd6kKw,592
+elemeno_ai_sdk-0.5.4.dist-info/LICENSE-3RDPARTY.txt,sha256=MXgzdAQL8HCYjE4UyFDtb7goq-4y6d6Hxu5x753NRns,15965
+elemeno_ai_sdk-0.5.4.dist-info/METADATA,sha256=rH4fSnWQ4X1M4jDz_tuNILBPiDS-qeH9UHoy03mx8ow,3116
+elemeno_ai_sdk-0.5.4.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+elemeno_ai_sdk-0.5.4.dist-info/entry_points.txt,sha256=MxLJDKUD5b4cVYFBMFH0Urs8zDxznly_99y2C40uXc0,53
+elemeno_ai_sdk-0.5.4.dist-info/top_level.txt,sha256=xq4olxjXm95p4Y71rv-7qTYMyA9XXuZfFHestuoZovo,15
+elemeno_ai_sdk-0.5.4.dist-info/RECORD,,
```

