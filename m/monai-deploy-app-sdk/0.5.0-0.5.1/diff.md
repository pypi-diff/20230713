# Comparing `tmp/monai_deploy_app_sdk-0.5.0-py3-none-any.whl.zip` & `tmp/monai_deploy_app_sdk-0.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,86 +1,89 @@
-Zip file size: 157080 bytes, number of entries: 84
--rw-rw-r--  2.0 unx      815 b- defN 22-Oct-08 20:44 monai/deploy/__init__.py
--rw-rw-r--  2.0 unx      497 b- defN 22-Oct-19 04:54 monai/deploy/_version.py
--rw-rw-r--  2.0 unx     1359 b- defN 22-Aug-30 23:50 monai/deploy/exceptions.py
--rw-rw-r--  2.0 unx      665 b- defN 22-Aug-30 23:50 monai/deploy/logging.json
--rw-rw-r--  2.0 unx      771 b- defN 22-Aug-30 23:50 monai/deploy/cli/__init__.py
--rw-rw-r--  2.0 unx      666 b- defN 22-Aug-30 23:50 monai/deploy/cli/__main__.py
--rw-rw-r--  2.0 unx     2991 b- defN 22-Aug-30 23:50 monai/deploy/cli/exec_command.py
--rw-rw-r--  2.0 unx     4624 b- defN 22-Aug-30 23:50 monai/deploy/cli/main.py
--rw-rw-r--  2.0 unx     1182 b- defN 22-Aug-30 23:50 monai/deploy/core/__init__.py
--rw-rw-r--  2.0 unx     2579 b- defN 22-Aug-30 23:50 monai/deploy/core/app_context.py
--rw-rw-r--  2.0 unx    17711 b- defN 22-Aug-30 23:50 monai/deploy/core/application.py
--rw-rw-r--  2.0 unx     3094 b- defN 22-Aug-30 23:50 monai/deploy/core/env.py
--rw-rw-r--  2.0 unx     4121 b- defN 22-Aug-30 23:50 monai/deploy/core/execution_context.py
--rw-rw-r--  2.0 unx     5125 b- defN 22-Aug-30 23:50 monai/deploy/core/io_context.py
--rw-rw-r--  2.0 unx      736 b- defN 22-Aug-30 23:50 monai/deploy/core/io_type.py
--rw-rw-r--  2.0 unx    10925 b- defN 22-Aug-30 23:50 monai/deploy/core/operator.py
--rw-rw-r--  2.0 unx     2599 b- defN 22-Aug-30 23:50 monai/deploy/core/operator_info.py
--rw-rw-r--  2.0 unx     5094 b- defN 22-Aug-30 23:50 monai/deploy/core/resource.py
--rw-rw-r--  2.0 unx     2046 b- defN 22-Aug-30 23:50 monai/deploy/core/runtime_env.py
--rw-rw-r--  2.0 unx      790 b- defN 22-Aug-30 23:50 monai/deploy/core/datastores/__init__.py
--rw-rw-r--  2.0 unx     2062 b- defN 22-Aug-30 23:50 monai/deploy/core/datastores/datastore.py
--rw-rw-r--  2.0 unx     1522 b- defN 22-Aug-30 23:50 monai/deploy/core/datastores/factory.py
--rw-rw-r--  2.0 unx     1258 b- defN 22-Aug-30 23:50 monai/deploy/core/datastores/memory.py
--rw-rw-r--  2.0 unx     1068 b- defN 22-Aug-30 23:50 monai/deploy/core/domain/__init__.py
--rw-rw-r--  2.0 unx     2901 b- defN 22-Aug-30 23:50 monai/deploy/core/domain/datapath.py
--rw-rw-r--  2.0 unx     8530 b- defN 22-Aug-30 23:50 monai/deploy/core/domain/dicom_series.py
--rw-rw-r--  2.0 unx     5605 b- defN 22-Oct-17 07:27 monai/deploy/core/domain/dicom_series_selection.py
--rw-rw-r--  2.0 unx     1963 b- defN 22-Aug-30 23:50 monai/deploy/core/domain/dicom_sop_instance.py
--rw-rw-r--  2.0 unx     3611 b- defN 22-Aug-30 23:50 monai/deploy/core/domain/dicom_study.py
--rw-rw-r--  2.0 unx     1057 b- defN 22-Aug-30 23:50 monai/deploy/core/domain/domain.py
--rw-rw-r--  2.0 unx     1863 b- defN 22-Oct-19 03:22 monai/deploy/core/domain/image.py
--rw-rw-r--  2.0 unx     1005 b- defN 22-Aug-30 23:50 monai/deploy/core/executors/__init__.py
--rw-rw-r--  2.0 unx     2118 b- defN 22-Aug-30 23:50 monai/deploy/core/executors/executor.py
--rw-rw-r--  2.0 unx     1584 b- defN 22-Aug-30 23:50 monai/deploy/core/executors/factory.py
--rw-rw-r--  2.0 unx     1964 b- defN 22-Aug-30 23:50 monai/deploy/core/executors/multi_process_executor.py
--rw-rw-r--  2.0 unx     1796 b- defN 22-Aug-30 23:50 monai/deploy/core/executors/multi_threaded_executor.py
--rw-rw-r--  2.0 unx     7361 b- defN 22-Aug-30 23:50 monai/deploy/core/executors/single_process_executor.py
--rw-rw-r--  2.0 unx      770 b- defN 22-Aug-30 23:50 monai/deploy/core/graphs/__init__.py
--rw-rw-r--  2.0 unx     1528 b- defN 22-Aug-30 23:50 monai/deploy/core/graphs/factory.py
--rw-rw-r--  2.0 unx     3094 b- defN 22-Aug-30 23:50 monai/deploy/core/graphs/graph.py
--rw-rw-r--  2.0 unx     2139 b- defN 22-Aug-30 23:50 monai/deploy/core/graphs/nx_digraph.py
--rw-rw-r--  2.0 unx      950 b- defN 22-Aug-30 23:50 monai/deploy/core/models/__init__.py
--rw-rw-r--  2.0 unx     2248 b- defN 22-Aug-30 23:50 monai/deploy/core/models/factory.py
--rw-rw-r--  2.0 unx     7865 b- defN 22-Aug-30 23:50 monai/deploy/core/models/model.py
--rw-rw-r--  2.0 unx     3398 b- defN 22-Aug-30 23:50 monai/deploy/core/models/named_model.py
--rw-rw-r--  2.0 unx     4472 b- defN 22-Aug-30 23:50 monai/deploy/core/models/torch_model.py
--rw-rw-r--  2.0 unx     4650 b- defN 22-Aug-30 23:50 monai/deploy/core/models/triton_model.py
--rw-rw-r--  2.0 unx     2090 b- defN 22-Oct-19 03:22 monai/deploy/operators/__init__.py
--rw-rw-r--  2.0 unx     5606 b- defN 22-Aug-30 23:50 monai/deploy/operators/clara_viz_operator.py
--rw-rw-r--  2.0 unx    13935 b- defN 22-Aug-30 23:50 monai/deploy/operators/dicom_data_loader_operator.py
--rw-rw-r--  2.0 unx    12526 b- defN 22-Oct-19 03:22 monai/deploy/operators/dicom_encapsulated_pdf_writer_operator.py
--rw-rw-r--  2.0 unx    19847 b- defN 22-Oct-19 04:21 monai/deploy/operators/dicom_seg_writer_operator.py
--rw-rw-r--  2.0 unx    16601 b- defN 22-Oct-19 03:22 monai/deploy/operators/dicom_series_selector_operator.py
--rw-rw-r--  2.0 unx    16661 b- defN 22-Oct-17 07:27 monai/deploy/operators/dicom_series_to_volume_operator.py
--rw-rw-r--  2.0 unx    13201 b- defN 22-Oct-19 03:22 monai/deploy/operators/dicom_text_sr_writer_operator.py
--rw-rw-r--  2.0 unx    12724 b- defN 22-Oct-17 07:27 monai/deploy/operators/dicom_utils.py
--rw-rw-r--  2.0 unx     2975 b- defN 22-Aug-30 23:50 monai/deploy/operators/inference_operator.py
--rw-rw-r--  2.0 unx    36177 b- defN 22-Oct-13 23:53 monai/deploy/operators/monai_bundle_inference_operator.py
--rw-rw-r--  2.0 unx    20280 b- defN 22-Oct-13 23:53 monai/deploy/operators/monai_seg_inference_operator.py
--rw-rw-r--  2.0 unx     3179 b- defN 22-Aug-30 23:50 monai/deploy/operators/png_converter_operator.py
--rw-rw-r--  2.0 unx    22010 b- defN 22-Aug-30 23:50 monai/deploy/operators/publisher_operator.py
--rw-rw-r--  2.0 unx    17563 b- defN 22-Sep-28 22:08 monai/deploy/operators/stl_conversion_operator.py
--rw-rw-r--  2.0 unx      574 b- defN 22-Aug-30 23:50 monai/deploy/packager/__init__.py
--rw-rw-r--  2.0 unx      955 b- defN 22-Aug-30 23:50 monai/deploy/packager/constants.py
--rw-rw-r--  2.0 unx     2530 b- defN 22-Aug-30 23:50 monai/deploy/packager/package_command.py
--rw-rw-r--  2.0 unx     5239 b- defN 22-Aug-30 23:50 monai/deploy/packager/templates.py
--rw-rw-r--  2.0 unx    14360 b- defN 22-Oct-13 23:53 monai/deploy/packager/util.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Aug-30 23:50 monai/deploy/runner/__init__.py
--rw-rw-r--  2.0 unx     1759 b- defN 22-Aug-30 23:50 monai/deploy/runner/run_command.py
--rw-rw-r--  2.0 unx     6943 b- defN 22-Aug-30 23:50 monai/deploy/runner/runner.py
--rw-rw-r--  2.0 unx     2455 b- defN 22-Aug-30 23:50 monai/deploy/runner/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Aug-30 23:50 monai/deploy/utils/__init__.py
--rw-rw-r--  2.0 unx     2897 b- defN 22-Aug-30 23:50 monai/deploy/utils/argparse_types.py
--rw-rw-r--  2.0 unx     1838 b- defN 22-Aug-30 23:50 monai/deploy/utils/fileutil.py
--rw-rw-r--  2.0 unx    12624 b- defN 22-Aug-30 23:50 monai/deploy/utils/importutil.py
--rw-rw-r--  2.0 unx     4142 b- defN 22-Aug-30 23:50 monai/deploy/utils/sizeutil.py
--rw-rw-r--  2.0 unx     2597 b- defN 22-Aug-30 23:50 monai/deploy/utils/spinner.py
--rw-rw-r--  2.0 unx     4512 b- defN 22-Aug-30 23:50 monai/deploy/utils/version.py
--rw-rw-r--  2.0 unx    11357 b- defN 22-Oct-19 04:54 monai_deploy_app_sdk-0.5.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     6607 b- defN 22-Oct-19 04:54 monai_deploy_app_sdk-0.5.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Oct-19 04:54 monai_deploy_app_sdk-0.5.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       60 b- defN 22-Oct-19 04:54 monai_deploy_app_sdk-0.5.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        6 b- defN 22-Oct-19 04:54 monai_deploy_app_sdk-0.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     7919 b- defN 22-Oct-19 04:54 monai_deploy_app_sdk-0.5.0.dist-info/RECORD
-84 files, 451613 bytes uncompressed, 144288 bytes compressed:  68.1%
+Zip file size: 161456 bytes, number of entries: 87
+-rw-rw-r--  2.0 unx      815 b- defN 23-Jul-11 20:03 monai/deploy/__init__.py
+-rw-rw-r--  2.0 unx      497 b- defN 23-Jul-13 05:15 monai/deploy/_version.py
+-rw-rw-r--  2.0 unx      496 b- defN 23-Mar-21 03:53 monai/deploy/_version_local.py
+-rw-rw-r--  2.0 unx     1359 b- defN 23-Jul-11 20:03 monai/deploy/exceptions.py
+-rw-rw-r--  2.0 unx      665 b- defN 23-Jul-11 20:03 monai/deploy/logging.json
+-rw-rw-r--  2.0 unx      771 b- defN 23-Jul-11 20:03 monai/deploy/cli/__init__.py
+-rw-rw-r--  2.0 unx      666 b- defN 23-Jul-11 20:03 monai/deploy/cli/__main__.py
+-rw-rw-r--  2.0 unx     2991 b- defN 23-Jul-11 20:03 monai/deploy/cli/exec_command.py
+-rw-rw-r--  2.0 unx     4624 b- defN 23-Jul-11 20:03 monai/deploy/cli/main.py
+-rw-rw-r--  2.0 unx     1182 b- defN 23-Jul-11 20:03 monai/deploy/core/__init__.py
+-rw-rw-r--  2.0 unx     2579 b- defN 23-Jul-11 20:03 monai/deploy/core/app_context.py
+-rw-rw-r--  2.0 unx    17722 b- defN 23-Jul-12 04:01 monai/deploy/core/application.py
+-rw-rw-r--  2.0 unx     3094 b- defN 23-Jul-12 04:01 monai/deploy/core/env.py
+-rw-rw-r--  2.0 unx     4121 b- defN 23-Jul-11 20:03 monai/deploy/core/execution_context.py
+-rw-rw-r--  2.0 unx     5116 b- defN 23-Jul-12 04:01 monai/deploy/core/io_context.py
+-rw-rw-r--  2.0 unx      736 b- defN 23-Jul-11 20:03 monai/deploy/core/io_type.py
+-rw-rw-r--  2.0 unx    10925 b- defN 23-Jul-11 20:03 monai/deploy/core/operator.py
+-rw-rw-r--  2.0 unx     2599 b- defN 23-Jul-11 20:03 monai/deploy/core/operator_info.py
+-rw-rw-r--  2.0 unx     5140 b- defN 23-Jul-12 04:01 monai/deploy/core/resource.py
+-rw-rw-r--  2.0 unx     2046 b- defN 23-Jul-11 20:03 monai/deploy/core/runtime_env.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jul-11 20:03 monai/deploy/core/datastores/__init__.py
+-rw-rw-r--  2.0 unx     2062 b- defN 23-Jul-11 20:03 monai/deploy/core/datastores/datastore.py
+-rw-rw-r--  2.0 unx     1522 b- defN 23-Jul-11 20:03 monai/deploy/core/datastores/factory.py
+-rw-rw-r--  2.0 unx     1258 b- defN 23-Jul-11 20:03 monai/deploy/core/datastores/memory.py
+-rw-rw-r--  2.0 unx     1068 b- defN 23-Jul-11 20:03 monai/deploy/core/domain/__init__.py
+-rw-rw-r--  2.0 unx     2901 b- defN 23-Jul-12 04:01 monai/deploy/core/domain/datapath.py
+-rw-rw-r--  2.0 unx     8530 b- defN 23-Jul-11 20:03 monai/deploy/core/domain/dicom_series.py
+-rw-rw-r--  2.0 unx     5605 b- defN 23-Jul-11 20:03 monai/deploy/core/domain/dicom_series_selection.py
+-rw-rw-r--  2.0 unx     1963 b- defN 23-Jul-11 20:03 monai/deploy/core/domain/dicom_sop_instance.py
+-rw-rw-r--  2.0 unx     3611 b- defN 23-Jul-11 20:03 monai/deploy/core/domain/dicom_study.py
+-rw-rw-r--  2.0 unx     1057 b- defN 23-Jul-11 20:03 monai/deploy/core/domain/domain.py
+-rw-rw-r--  2.0 unx     1863 b- defN 23-Jul-11 20:03 monai/deploy/core/domain/image.py
+-rw-rw-r--  2.0 unx     1005 b- defN 23-Jul-11 20:03 monai/deploy/core/executors/__init__.py
+-rw-rw-r--  2.0 unx     2118 b- defN 23-Jul-11 20:03 monai/deploy/core/executors/executor.py
+-rw-rw-r--  2.0 unx     1584 b- defN 23-Jul-11 20:03 monai/deploy/core/executors/factory.py
+-rw-rw-r--  2.0 unx     1964 b- defN 23-Jul-11 20:03 monai/deploy/core/executors/multi_process_executor.py
+-rw-rw-r--  2.0 unx     1796 b- defN 23-Jul-11 20:03 monai/deploy/core/executors/multi_threaded_executor.py
+-rw-rw-r--  2.0 unx     7359 b- defN 23-Jul-11 20:08 monai/deploy/core/executors/single_process_executor.py
+-rw-rw-r--  2.0 unx      770 b- defN 23-Jul-11 20:03 monai/deploy/core/graphs/__init__.py
+-rw-rw-r--  2.0 unx     1528 b- defN 23-Jul-11 20:03 monai/deploy/core/graphs/factory.py
+-rw-rw-r--  2.0 unx     3094 b- defN 23-Jul-11 20:03 monai/deploy/core/graphs/graph.py
+-rw-rw-r--  2.0 unx     2137 b- defN 23-Jul-11 20:08 monai/deploy/core/graphs/nx_digraph.py
+-rw-rw-r--  2.0 unx      950 b- defN 23-Jul-11 20:03 monai/deploy/core/models/__init__.py
+-rw-rw-r--  2.0 unx     2248 b- defN 23-Jul-11 20:03 monai/deploy/core/models/factory.py
+-rw-rw-r--  2.0 unx     7865 b- defN 23-Jul-12 04:01 monai/deploy/core/models/model.py
+-rw-rw-r--  2.0 unx     3398 b- defN 23-Jul-12 04:01 monai/deploy/core/models/named_model.py
+-rw-rw-r--  2.0 unx     4472 b- defN 23-Jul-11 20:03 monai/deploy/core/models/torch_model.py
+-rw-rw-r--  2.0 unx     4650 b- defN 23-Jul-11 20:03 monai/deploy/core/models/triton_model.py
+-rw-rw-r--  2.0 unx     2164 b- defN 23-Jul-11 20:08 monai/deploy/operators/__init__.py
+-rw-rw-r--  2.0 unx     5606 b- defN 23-Jul-11 20:03 monai/deploy/operators/clara_viz_operator.py
+-rw-rw-r--  2.0 unx    13957 b- defN 23-Jul-12 04:01 monai/deploy/operators/dicom_data_loader_operator.py
+-rw-rw-r--  2.0 unx    12525 b- defN 23-Jul-11 20:08 monai/deploy/operators/dicom_encapsulated_pdf_writer_operator.py
+-rw-rw-r--  2.0 unx    20276 b- defN 23-Jul-11 20:08 monai/deploy/operators/dicom_seg_writer_operator.py
+-rw-rw-r--  2.0 unx    16599 b- defN 23-Jul-12 04:01 monai/deploy/operators/dicom_series_selector_operator.py
+-rw-rw-r--  2.0 unx    16660 b- defN 23-Jul-11 20:08 monai/deploy/operators/dicom_series_to_volume_operator.py
+-rw-rw-r--  2.0 unx    13200 b- defN 23-Jul-11 20:08 monai/deploy/operators/dicom_text_sr_writer_operator.py
+-rw-rw-r--  2.0 unx    12722 b- defN 23-Jul-11 20:08 monai/deploy/operators/dicom_utils.py
+-rw-rw-r--  2.0 unx     2975 b- defN 23-Jul-11 20:03 monai/deploy/operators/inference_operator.py
+-rw-rw-r--  2.0 unx    39476 b- defN 23-Jul-12 04:01 monai/deploy/operators/monai_bundle_inference_operator.py
+-rw-rw-r--  2.0 unx    22856 b- defN 23-Jul-11 20:08 monai/deploy/operators/monai_seg_inference_operator.py
+-rw-rw-r--  2.0 unx     1963 b- defN 23-Jul-05 23:55 monai/deploy/operators/nii_data_loader_operator.py
+-rw-rw-r--  2.0 unx     3179 b- defN 23-Jul-11 20:03 monai/deploy/operators/png_converter_operator.py
+-rw-rw-r--  2.0 unx    22010 b- defN 23-Jul-11 20:03 monai/deploy/operators/publisher_operator.py
+-rw-rw-r--  2.0 unx    17563 b- defN 23-Jul-11 20:03 monai/deploy/operators/stl_conversion_operator.py
+-rw-rw-r--  2.0 unx      574 b- defN 23-Jul-11 20:03 monai/deploy/packager/__init__.py
+-rw-rw-r--  2.0 unx      955 b- defN 23-Jul-11 20:08 monai/deploy/packager/constants.py
+-rw-rw-r--  2.0 unx     2530 b- defN 23-Jul-11 20:03 monai/deploy/packager/package_command.py
+-rw-rw-r--  2.0 unx     5318 b- defN 23-Jul-11 20:08 monai/deploy/packager/templates.py
+-rw-rw-r--  2.0 unx    14645 b- defN 23-Jul-12 04:01 monai/deploy/packager/util.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-11 20:03 monai/deploy/runner/__init__.py
+-rw-rw-r--  2.0 unx     1759 b- defN 23-Jul-11 20:03 monai/deploy/runner/run_command.py
+-rw-rw-r--  2.0 unx     7093 b- defN 23-Jul-12 04:01 monai/deploy/runner/runner.py
+-rw-rw-r--  2.0 unx     2455 b- defN 23-Jul-11 20:03 monai/deploy/runner/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-11 20:03 monai/deploy/utils/__init__.py
+-rw-rw-r--  2.0 unx     2897 b- defN 23-Jul-12 04:01 monai/deploy/utils/argparse_types.py
+-rw-rw-r--  2.0 unx     1140 b- defN 23-Apr-06 20:59 monai/deploy/utils/deviceutil.py
+-rw-rw-r--  2.0 unx     1838 b- defN 23-Jul-11 20:03 monai/deploy/utils/fileutil.py
+-rw-rw-r--  2.0 unx    13957 b- defN 23-Jul-12 04:01 monai/deploy/utils/importutil.py
+-rw-rw-r--  2.0 unx     4142 b- defN 23-Jul-12 04:01 monai/deploy/utils/sizeutil.py
+-rw-rw-r--  2.0 unx     2597 b- defN 23-Jul-11 20:03 monai/deploy/utils/spinner.py
+-rw-rw-r--  2.0 unx     4512 b- defN 23-Jul-12 04:01 monai/deploy/utils/version.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jul-13 05:15 monai_deploy_app_sdk-0.5.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     6636 b- defN 23-Jul-13 05:15 monai_deploy_app_sdk-0.5.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-13 05:15 monai_deploy_app_sdk-0.5.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       60 b- defN 23-Jul-13 05:15 monai_deploy_app_sdk-0.5.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jul-13 05:15 monai_deploy_app_sdk-0.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     8201 b- defN 23-Jul-13 05:15 monai_deploy_app_sdk-0.5.1.dist-info/RECORD
+87 files, 463807 bytes uncompressed, 148212 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: monai/deploy/__init__.py
 Comment: 
 
 Filename: monai/deploy/_version.py
 Comment: 
 
+Filename: monai/deploy/_version_local.py
+Comment: 
+
 Filename: monai/deploy/exceptions.py
 Comment: 
 
 Filename: monai/deploy/logging.json
 Comment: 
 
 Filename: monai/deploy/cli/__init__.py
@@ -171,14 +174,17 @@
 
 Filename: monai/deploy/operators/monai_bundle_inference_operator.py
 Comment: 
 
 Filename: monai/deploy/operators/monai_seg_inference_operator.py
 Comment: 
 
+Filename: monai/deploy/operators/nii_data_loader_operator.py
+Comment: 
+
 Filename: monai/deploy/operators/png_converter_operator.py
 Comment: 
 
 Filename: monai/deploy/operators/publisher_operator.py
 Comment: 
 
 Filename: monai/deploy/operators/stl_conversion_operator.py
@@ -213,14 +219,17 @@
 
 Filename: monai/deploy/utils/__init__.py
 Comment: 
 
 Filename: monai/deploy/utils/argparse_types.py
 Comment: 
 
+Filename: monai/deploy/utils/deviceutil.py
+Comment: 
+
 Filename: monai/deploy/utils/fileutil.py
 Comment: 
 
 Filename: monai/deploy/utils/importutil.py
 Comment: 
 
 Filename: monai/deploy/utils/sizeutil.py
@@ -228,26 +237,26 @@
 
 Filename: monai/deploy/utils/spinner.py
 Comment: 
 
 Filename: monai/deploy/utils/version.py
 Comment: 
 
-Filename: monai_deploy_app_sdk-0.5.0.dist-info/LICENSE
+Filename: monai_deploy_app_sdk-0.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: monai_deploy_app_sdk-0.5.0.dist-info/METADATA
+Filename: monai_deploy_app_sdk-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: monai_deploy_app_sdk-0.5.0.dist-info/WHEEL
+Filename: monai_deploy_app_sdk-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: monai_deploy_app_sdk-0.5.0.dist-info/entry_points.txt
+Filename: monai_deploy_app_sdk-0.5.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: monai_deploy_app_sdk-0.5.0.dist-info/top_level.txt
+Filename: monai_deploy_app_sdk-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: monai_deploy_app_sdk-0.5.0.dist-info/RECORD
+Filename: monai_deploy_app_sdk-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## monai/deploy/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2022-10-18T21:54:08-0700",
+ "date": "2023-07-12T22:15:04-0700",
  "dirty": false,
  "error": null,
- "full-revisionid": "95f5ec64d53fabfa9da3066644c681854befe44f",
- "version": "0.5.0"
+ "full-revisionid": "978f28c62d00f653beb895176947a631c342c69b",
+ "version": "0.5.1"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## monai/deploy/core/application.py

```diff
@@ -78,15 +78,15 @@
         # Setup app description
         if not self.name:
             self.name = self.__class__.__name__
         if not self.description:
             self.description = get_docstring(self.__class__)
         if not self.version:
             try:
-                from _version import get_versions
+                from monai.deploy._version import get_versions
 
                 self.version = get_versions()["version"]
             except ImportError:
                 self.version = "0.0.0"
 
         # Set the application path
         if path:
@@ -201,21 +201,21 @@
         destination_op.ensure_valid()
 
         op_output_labels = source_op.op_info.get_labels(IO.OUTPUT)
         op_input_labels = destination_op.op_info.get_labels(IO.INPUT)
         if not io_map:
             if len(op_output_labels) > 1:
                 raise IOMappingError(
-                    f"The source operator has more than one output port "
+                    "The source operator has more than one output port "
                     f"({', '.join(op_output_labels)}) so mapping should be specified explicitly!"
                 )
             if len(op_input_labels) > 1:
                 raise IOMappingError(
                     f"The destination operator has more than one output port ({', '.join(op_input_labels)}) "
-                    f"so mapping should be specified explicitly!"
+                    "so mapping should be specified explicitly!"
                 )
             io_map = {"": {""}}
 
         # Convert io_map's values to the set of strings.
         io_maps: Dict[str, Set[str]] = io_map  # type: ignore
         for k, v in io_map.items():
             if isinstance(v, str):
@@ -223,51 +223,51 @@
 
         # Verify that the source & destination operator have the input and output ports specified by the io_map
         output_labels = list(io_maps.keys())
 
         if len(op_output_labels) == 1 and len(output_labels) != 1:
             raise IOMappingError(
                 f"The source operator({source_op.name}) has only one port with label "
-                f"'{next(iter(op_output_labels))}' but io_map specifies {len(output_labels)} "
+                f"{next(iter(op_output_labels))!r} but io_map specifies {len(output_labels)} "
                 f"labels({', '.join(output_labels)}) to the source operator's output port"
             )
 
         for output_label in output_labels:
             if output_label not in op_output_labels:
                 if len(op_output_labels) == 1 and len(output_labels) == 1 and output_label == "":
                     # Set the default output port label.
                     io_maps[next(iter(op_output_labels))] = io_maps[output_label]
                     del io_maps[output_label]
                     break
                 raise IOMappingError(
-                    f"The source operator({source_op.name}) has no output port with label '{output_label}'. "
+                    f"The source operator({source_op.name}) has no output port with label {output_label!r}. "
                     f"It should be one of ({', '.join(op_output_labels)})."
                 )
 
         output_labels = list(io_maps.keys())  # re-evaluate output_labels
         for output_label in output_labels:
             input_labels = io_maps[output_label]
 
             if len(op_input_labels) == 1 and len(input_labels) != 1:
                 raise IOMappingError(
                     f"The destination operator({destination_op.name}) has only one port with label "
-                    f"'{next(iter(op_input_labels))}' but io_map specifies {len(input_labels)} "
+                    f"{next(iter(op_input_labels))!r} but io_map specifies {len(input_labels)} "
                     f"labels({', '.join(input_labels)}) to the destination operator's input port"
                 )
 
             for input_label in input_labels:
                 if input_label not in op_input_labels:
                     if len(op_input_labels) == 1 and len(input_labels) == 1 and input_label == "":
                         # Set the default input port label.
                         input_labels.clear()
                         input_labels.add(next(iter(op_input_labels)))
                         break
                     raise IOMappingError(
-                        f"The destination operator({destination_op.name}) has no input port with label '{input_label}'. "
-                        f"It should be one of ({', '.join(op_input_labels)})."
+                        f"The destination operator({destination_op.name}) has no input port with label {input_label!r}."
+                        f" It should be one of ({', '.join(op_input_labels)})."
                     )
 
         self._graph.add_flow(source_op, destination_op, io_maps)
 
     def get_package_info(self, model_path: Union[str, Path] = "") -> Dict:
         """Returns the package information of this application.
```

## monai/deploy/core/env.py

```diff
@@ -33,15 +33,15 @@
         """
         if type(pip_packages) is str:
             requirements_path = Path(pip_packages)
 
             if requirements_path.exists():
                 pip_packages = requirements_path.read_text().strip().splitlines()  # make it a list
             else:
-                raise FileNotFoundError(f"The '{requirements_path}' file does not exist!")
+                raise FileNotFoundError(f"The {requirements_path!r} file does not exist!")
 
         self._pip_packages = list(pip_packages or [])
 
     @property
     def pip_packages(self) -> List[str]:
         """Get the list of pip packages.
```

## monai/deploy/core/io_context.py

```diff
@@ -45,15 +45,15 @@
     def get_default_label(self, label: str = "") -> str:
         """Get a default label for IO context."""
         if label not in self._labels:
             if label == "" and len(self._labels) == 1:
                 label = next(iter(self._labels))
             else:
                 raise IOMappingError(
-                    f"'{label}' is not a valid {self._io_kind} of the operator({self._op.name}). "
+                    f"{label!r} is not a valid {self._io_kind} of the operator({self._op.name}). "
                     f"It should be one of ({', '.join(self._labels)})."
                 )
         return label
 
     def get_group_path(self, postfix: str = "") -> str:
         """Returns the path for the group.
 
@@ -78,15 +78,15 @@
 
             "/operators/{self._op.uid}/{execution_index}/{self._io_kind}/{label}"
         """
         label = self.get_default_label(label)
         key = self.get_group_path(f"{self._io_kind}/{label}")
         storage = self._storage
         if not storage.exists(key):
-            raise ItemNotExistsError(f"'{key}' does not exist.")
+            raise ItemNotExistsError(f"{key!r} does not exist.")
         return storage.get(key)
 
     def set(self, value: Any, label: str = ""):
         """Sets the data for the operator.
 
         It uses a sub path ({self._io_kind}/{label}) to set the data.
         The final group path (key) would be:
@@ -105,18 +105,18 @@
                 value.to_absolute()
 
             # Verify the type of the value is matching the type of the input/output of the operator.
             # Use 'typeguard' package because Python's built-in isinstance() does not support parameterized generic type
             # checking: https://www.python.org/dev/peps/pep-0585/#id15
             data_type = self._op_info.get_data_type(self._io_kind, label)
             try:
-                check_type("value", value, data_type)
+                check_type(value, data_type)
             except TypeError as err:
                 raise IOMappingError(
-                    f"The data type of '{label}' in the {self._io_kind} of '{self._op}' is {data_type}, but the value"
+                    f"The data type of {label!r} in the {self._io_kind} of {self._op!r} is {data_type}, but the value"
                     f" to set is the data type of {type(value)}."
                 ) from err
 
             storage.put(key, value)
 
 
 class InputContext(IOContext):
```

## monai/deploy/core/resource.py

```diff
@@ -60,23 +60,25 @@
         """Sets resource limits from the given values if each attribute is not None."""
 
         if cpu_limit is not None:
             if self._cpu is None:
                 self._cpu = cpu_limit
             else:
                 raise ItemAlreadyExistsError(
-                    f"'cpu' wouldn't be set to {cpu_limit} because it is already set to {self._cpu} by the runtime environment."
+                    f"'cpu' wouldn't be set to {cpu_limit} because it is already set to {self._cpu} by the runtime"
+                    " environment."
                 )
 
         if gpu_limit is not None:
             if self._gpu is None:
                 self._gpu = gpu_limit
             else:
                 raise ItemAlreadyExistsError(
-                    f"'gpu' wouldn't be set to {gpu_limit} because it is already set to {self._gpu} by the runtime environment."
+                    f"'gpu' wouldn't be set to {gpu_limit} because it is already set to {self._gpu} by the runtime"
+                    " environment."
                 )
 
         if type(memory_limit) == str:
             try:
                 self._memory = get_bytes(memory_limit)
             except Exception as err:
                 raise WrongValueError(
```

## monai/deploy/core/domain/datapath.py

```diff
@@ -63,14 +63,14 @@
 
     def get(self, name: Optional[str] = "") -> DataPath:
         if name not in self._paths:
             if name == "" and len(self._paths) == 1:
                 return next(iter(self._paths.values()))
             else:
                 raise IOMappingError(
-                    f"'{name}' is not a valid name. It should be one of ({', '.join(self._paths.keys())})."
+                    f"{name!r} is not a valid name. It should be one of ({', '.join(self._paths.keys())})."
                 )
         else:
             datapath = self._paths.get(name)
             if not datapath:
-                raise ItemNotExistsError(f"A DataPath instance for '{name}' does not exist.")
+                raise ItemNotExistsError(f"A DataPath instance for {name!r} does not exist.")
             return datapath
```

## monai/deploy/core/executors/single_process_executor.py

```diff
@@ -137,15 +137,15 @@
 
                         raise IOMappingError(
                             f"No IO mappings found for {op.name} -> {next_op.name} in "
                             f"{inspect.getabsfile(self.app.__class__)}"
                         )
 
                     next_op_exec_context = ExecutionContext(exec_context, next_op)
-                    for (out_label, in_labels) in io_map.items():
+                    for out_label, in_labels in io_map.items():
                         output = op_exec_context.output_context.get(out_label)
                         for in_label in in_labels:
                             next_op_exec_context.input_context.set(output, in_label)
         finally:
             # Always restore pwd even if an exception is raised (This logic can be run in an IPython environment)
             os.chdir(old_pwd)
```

## monai/deploy/core/graphs/nx_digraph.py

```diff
@@ -48,9 +48,9 @@
         return (op for op in self._graph.nodes())
 
     def gen_worklist(self) -> Generator[Optional[Operator], None, None]:
         worklist: Generator[Optional[Operator], None, None] = topological_sort(self._graph)
         return worklist
 
     def gen_next_operators(self, op: Operator) -> Generator[Optional[Operator], None, None]:
-        for (_, v) in self._graph.out_edges(op):
+        for _, v in self._graph.out_edges(op):
             yield v
```

## monai/deploy/core/models/model.py

```diff
@@ -160,15 +160,15 @@
             A model object is returned, matching the provided name if given.
         """
         if name:
             item = self._items.get(name)
             if item:
                 return item
             else:
-                raise ItemNotExistsError(f"A model with '{name}' does not exist.")
+                raise ItemNotExistsError(f"A model with {name!r} does not exist.")
         else:
             item_count = len(self._items)
             if item_count == 1:
                 return next(iter(self._items.values()))
             elif item_count > 1:
                 raise UnknownTypeError(
                     f"There are more than one model. It should be one of ({', '.join(self._items.keys())})."
```

## monai/deploy/core/models/named_model.py

```diff
@@ -79,13 +79,13 @@
         if not all((p.is_dir() for p in model_path.iterdir())):
             return False, None
 
         for model_folder in model_path.iterdir():
             # 3) Each model folder must contain only one model definition file or folder.
             if sum(1 for _ in model_folder.iterdir()) != 1:
                 logger.warning(
-                    f"Model repository '{model_folder}' contains more than one model definition file or folder "
+                    f"Model repository {model_folder!r} contains more than one model definition file or folder "
                     "so not treated as NamedModel."
                 )
                 return False, None
 
         return True, cls.model_type
```

## monai/deploy/operators/__init__.py

```diff
@@ -26,23 +26,25 @@
     ModelInfo
     MonaiBundleInferenceOperator
     MonaiSegInferenceOperator
     PNGConverterOperator
     PublisherOperator
     STLConversionOperator
     STLConverter
+    NiftiDataLoader
 """
 
 from .clara_viz_operator import ClaraVizOperator
 from .dicom_data_loader_operator import DICOMDataLoaderOperator
 from .dicom_encapsulated_pdf_writer_operator import DICOMEncapsulatedPDFWriterOperator
 from .dicom_seg_writer_operator import DICOMSegmentationWriterOperator
 from .dicom_series_selector_operator import DICOMSeriesSelectorOperator
 from .dicom_series_to_volume_operator import DICOMSeriesToVolumeOperator
 from .dicom_text_sr_writer_operator import DICOMTextSRWriterOperator
 from .dicom_utils import EquipmentInfo, ModelInfo, random_with_n_digits, save_dcm_file, write_common_modules
 from .inference_operator import InferenceOperator
 from .monai_bundle_inference_operator import BundleConfigNames, IOMapping, MonaiBundleInferenceOperator
 from .monai_seg_inference_operator import MonaiSegInferenceOperator
+from .nii_data_loader_operator import NiftiDataLoader
 from .png_converter_operator import PNGConverterOperator
 from .publisher_operator import PublisherOperator
 from .stl_conversion_operator import STLConversionOperator, STLConverter
```

## monai/deploy/operators/dicom_data_loader_operator.py

```diff
@@ -114,15 +114,14 @@
         for file in files:
             try:
                 sop_instances.append(dcmread(file))
             except InvalidDicomError as ex:
                 logging.warning(f"Ignored {file}, reason being: {ex}")
 
         for sop_instance in sop_instances:
-
             study_instance_uid = sop_instance[0x0020, 0x000D].value.name  # name is the UID as str
 
             if study_instance_uid not in study_dict:
                 study = DICOMStudy(study_instance_uid)
                 self.populate_study_attributes(study, sop_instance)
                 study_dict[study_instance_uid] = study
 
@@ -305,15 +304,16 @@
                 except KeyError:
                     pass
                 # Need to get pydicom dataset to use properties and get method of a dict.
                 ds = sop.get_native_sop_instance()
                 print(f"   'StudyInstanceUID': {ds.StudyInstanceUID if ds.StudyInstanceUID else ''}")
                 print(f"  'SeriesDescription': {ds.SeriesDescription if ds.SeriesDescription else ''}")
                 print(
-                    f"  'IssuerOfPatientID': {ds.get('IssuerOfPatientID', '').repval if ds.get('IssuerOfPatientID', '') else '' }"
+                    "  'IssuerOfPatientID':"
+                    f" {ds.get('IssuerOfPatientID', '').repval if ds.get('IssuerOfPatientID', '') else '' }"
                 )
                 try:
                     print(f"  'IssuerOfPatientID': {ds.IssuerOfPatientID if ds.IssuerOfPatientID else '' }")
                 except AttributeError:
                     print(
                         "    If the IssuerOfPatientID does not exist, ds.IssuerOfPatientID would throw AttributeError."
                     )
```

## monai/deploy/operators/dicom_encapsulated_pdf_writer_operator.py

```diff
@@ -38,15 +38,14 @@
 # The SR writer operator class
 @md.input("pdf_bytes", Bytes, IOType.IN_MEMORY)
 @md.input("pdf_file", DataPath, IOType.DISK)
 @md.input("study_selected_series_list", List[StudySelectedSeries], IOType.IN_MEMORY)
 @md.output("dicom_instance", DataPath, IOType.DISK)
 @md.env(pip_packages=["pydicom >= 1.4.2", "PyPDF2 >= 2.11.1", "monai"])
 class DICOMEncapsulatedPDFWriterOperator(Operator):
-
     DCM_EXTENSION = ".dcm"
 
     def __init__(
         self,
         copy_tags: bool,
         model_info: ModelInfo,
         equipment_info: Optional[EquipmentInfo] = None,
```

## monai/deploy/operators/dicom_seg_writer_operator.py

```diff
@@ -7,14 +7,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import datetime
 import logging
+import os
 from pathlib import Path
 from random import randint
 from typing import TYPE_CHECKING, Dict, List, Optional, Sequence, Union
 
 import numpy as np
 from typeguard import typechecked
 
@@ -168,14 +169,15 @@
     # DICOM instance file extension. Case insensitive in string comparison.
     DCM_EXTENSION = ".dcm"
 
     def __init__(
         self,
         segment_descriptions: List[SegmentDescription],
         custom_tags: Optional[Dict[str, str]] = None,
+        omit_empty_frames: bool = True,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         """Instantiates the DICOM Seg Writer instance with optional list of segment label strings.
 
         Each unique, non-zero integer value in the segmentation image represents a segment that must be
@@ -188,20 +190,23 @@
 
         Note: this interface is subject to change. It is planned that a new object will encapsulate the
         segment label information, including label value, name, description etc.
 
         Args:
             segment_descriptions: List[SegmentDescription]
                 Object encapsulating the description of each segment present in the segmentation.
-            custom_tags: OptonalDict[str, str], optional
+            custom_tags: Optional[Dict[str, str]], optional
                 Dictionary for setting custom DICOM tags using Keywords and str values only
+            omit_empty_frames: bool, optional
+                Whether to omit frames that contain no segmented pixels from the output segmentation.
         """
 
         self._seg_descs = [sd.to_segment_description(n) for n, sd in enumerate(segment_descriptions, 1)]
         self._custom_tags = custom_tags
+        self._omit_empty_frames = omit_empty_frames
 
     def compute(self, op_input: InputContext, op_output: OutputContext, context: ExecutionContext):
         """Performs computation for this operator and handles I/O.
 
         For now, only a single segmentation image object or file is supported and the selected DICOM
         series for inference is required, because the DICOM Seg IOD needs to refer to original instance.
         When there are multiple selected series in the input, the first series' containing study will
@@ -286,14 +291,15 @@
             series_number=random_with_n_digits(4),
             sop_instance_uid=seg_sop_instance_uid,
             instance_number=1,
             manufacturer="The MONAI Consortium",
             manufacturer_model_name="MONAI Deploy App SDK",
             software_versions=version_str,
             device_serial_number="0000",
+            omit_empty_frames=self._omit_empty_frames,
         )
 
         # Adding a few tags that are not in the Dataset
         # Also try to set the custom tags that are of string type
         dt_now = datetime.datetime.now()
         seg.SeriesDate = dt_now.strftime("%Y%m%d")
         seg.SeriesTime = dt_now.strftime("%H%M%S")
@@ -302,17 +308,19 @@
         )  # '2022-09-27T22:36:20.143857-07:00'
 
         if self._custom_tags:
             for k, v in self._custom_tags.items():
                 if isinstance(k, str) and isinstance(v, str):
                     try:
                         if k in seg:
-                            seg.data_element(k).value = v
+                            data_element = seg.data_element(k)
+                            if data_element:
+                                data_element.value = v
                         else:
-                            seg.update({k: v})
+                            seg.update({k: v})  # type: ignore
                     except Exception as ex:
                         # Best effort for now.
                         logging.warning(f"Tag {k} was not written, due to {ex}")
 
         seg.save_as(output_path)
 
         try:
```

## monai/deploy/operators/dicom_series_selector_operator.py

```diff
@@ -173,15 +173,15 @@
         Returns:
             list: list of StudySelectedSeries objects
         """
 
         study_selected_series_list = []
         for study in dicom_study_list:
             logging.info(f"Working on study, instance UID: {study.StudyInstanceUID}")
-            print((f"Working on study, instance UID: {study.StudyInstanceUID}"))
+            print(f"Working on study, instance UID: {study.StudyInstanceUID}")
             study_selected_series = StudySelectedSeries(study)
             for series in study.get_all_series():
                 logging.info(f"Working on series, instance UID: {str(series.SeriesInstanceUID)}")
                 print(f"Working on series, instance UID: {str(series.SeriesInstanceUID)}")
                 selected_series = SelectedSeries("", series, None)  # No selection name or Image obj.
                 study_selected_series.add_selected_series(selected_series)
             study_selected_series_list.append(study_selected_series)
@@ -209,15 +209,15 @@
             # Combine Study and current Series properties for matching
             series_attr = self._get_instance_properties(series)
             series_attr.update(study_attr)
 
             matched = True
             # Simple matching on attribute value
             for key, value_to_match in attributes.items():
-                logging.info(f"On attribute: '{key}' to match value: '{value_to_match}'")
+                logging.info(f"On attribute: {key!r} to match value: {value_to_match!r}")
                 # Ignore None
                 if not value_to_match:
                     continue
                 # Try getting the attribute value from Study and current Series prop dict
                 attr_value = series_attr.get(key, None)
                 logging.info(f"    Series attribute {key} value: {attr_value}")
```

## monai/deploy/operators/dicom_series_to_volume_operator.py

```diff
@@ -385,15 +385,14 @@
                 else:
                     prop_dict[attribute] = attr_val
 
         return prop_dict
 
 
 def test():
-
     from pathlib import Path
 
     from monai.deploy.operators.dicom_data_loader_operator import DICOMDataLoaderOperator
     from monai.deploy.operators.dicom_series_selector_operator import DICOMSeriesSelectorOperator
 
     current_file_dir = Path(__file__).parent.resolve()
     data_path = current_file_dir.joinpath("../../../examples/ai_spleen_seg_data/dcm")
```

## monai/deploy/operators/dicom_text_sr_writer_operator.py

```diff
@@ -35,15 +35,14 @@
 # The SR writer operator class
 @md.input("classification_result", Text, IOType.IN_MEMORY)
 @md.input("classification_result_file", DataPath, IOType.DISK)
 @md.input("study_selected_series_list", List[StudySelectedSeries], IOType.IN_MEMORY)
 @md.output("dicom_instance", DataPath, IOType.DISK)
 @md.env(pip_packages=["pydicom >= 1.4.2", "monai"])
 class DICOMTextSRWriterOperator(Operator):
-
     # File extension for the generated DICOM Part 10 file.
     DCM_EXTENSION = ".dcm"
 
     def __init__(
         self,
         copy_tags: bool,
         model_info: ModelInfo,
```

## monai/deploy/operators/dicom_utils.py

```diff
@@ -56,15 +56,14 @@
         - Device UID (0018,1002)
 
     Each time an AI Model is modified, for example by training, it would be appropriate to update
     the Device UID.
     """
 
     def __init__(self, creator: str = "", name: str = "", version: str = "", uid: str = ""):
-
         self.creator = creator if isinstance(creator, str) else ""
         self.name = name if isinstance(name, str) else ""
         self.version = version if isinstance(version, str) else ""
         self.uid = uid if isinstance(uid, str) else ""
 
 
 class EquipmentInfo(object):
@@ -73,15 +72,14 @@
     def __init__(
         self,
         manufacturer: str = "MONAI Deploy",
         manufacturer_model: str = "MONAI Deploy App SDK",
         series_number: str = "0000",
         software_version_number: str = "",
     ):
-
         self.manufacturer = manufacturer if isinstance(manufacturer, str) else ""
         self.manufacturer_model = manufacturer_model if isinstance(manufacturer_model, str) else ""
         self.series_number = series_number if isinstance(series_number, str) else ""
         if software_version_number:
             self.software_version_number = str(software_version_number)[0:15]
         else:
             try:
```

## monai/deploy/operators/monai_bundle_inference_operator.py

```diff
@@ -9,14 +9,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import logging
 import os
 import pickle
+import tempfile
 import time
 import zipfile
 from copy import deepcopy
 from pathlib import Path
 from threading import Lock
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
@@ -58,51 +59,118 @@
 
 
 def get_bundle_config(bundle_path, config_names):
     """
     Gets the configuration parser from the specified Torchscript bundle file path.
     """
 
-    def _read_from_archive(archive, root_name: str, relative_path: str, path_list: List[str]):
-        """A helper function for reading a file in an zip archive.
+    bundle_suffixes = (".json", ".yaml", "yml")  # The only supported file ext(s)
+    config_folder = "extra"
 
-        Tries to read with the full path of # a archive file, if error, then find the relative
-        path and then read the file.
+    def _read_from_archive(archive, root_name: str, config_name: str, do_search=True):
+        """A helper function for reading the content of a config in the zip archive.
+
+        Tries to read config content at the expected path in the archive, if error occurs,
+        search and read with alternative paths.
         """
+
         content_text = None
-        try:
-            content_text = archive.read(f"{root_name}/{relative_path}")
-        except KeyError:
-            logging.debug(f"Trying to find the metadata/config file in the bundle archive: {relative_path}.")
-            for n in path_list:
-                if relative_path in n:
-                    content_text = archive.read(n)
-                    break
-            if content_text is None:
-                raise
+        config_name = config_name.split(".")[0]  # In case ext is present
+
+        # Try directly read with constructed and expected path into the archive
+        for suffix in bundle_suffixes:
+            path = Path(root_name, config_folder, config_name).with_suffix(suffix)
+            try:
+                logging.debug(f"Trying to read config {config_name!r} content from {path}.")
+                content_text = archive.read(str(path))
+                break
+            except Exception:
+                logging.debug(f"Error reading from {path}. Will try alternative ways.")
+                continue
+
+        # Try search for the name in the name list of the archive
+        if not content_text and do_search:
+            logging.debug(f"Trying to find the file in the archive for config {config_name!r}.")
+            name_list = archive.namelist()
+            for suffix in bundle_suffixes:
+                for n in name_list:
+                    if (f"{config_name}{suffix}").casefold in n.casefold():
+                        logging.debug(f"Trying to read content of config {config_name!r} from {n}.")
+                        content_text = archive.read(n)
+                        break
+
+        if not content_text:
+            raise IOError(f"Cannot read config {config_name}{bundle_suffixes} or its content in the archive.")
 
         return content_text
 
+    def _extract_from_archive(
+        archive, root_name: str, config_names: List[str], dest_folder: Union[str, Path], do_search=True
+    ):
+        """A helper function for extract files of configs from the archive to the destination folder
+
+        Tries to extract with the full paths from the archive file, if error occurs, tries to search for
+        and read from the file(s) if do_search is true.
+        """
+
+        config_names = [cn.split(".")[0] for cn in config_names]  # In case the extension is present
+        file_list = []
+
+        # Try directly read first with path into the archive
+        for suffix in bundle_suffixes:
+            try:
+                logging.debug(f"Trying to extract {config_names} with ext {suffix}.")
+                file_list = [str(Path(root_name, config_folder, cn).with_suffix(suffix)) for cn in config_names]
+                archive.extractall(members=file_list, path=dest_folder)
+                break
+            except Exception as ex:
+                file_list = []
+                logging.debug(f"Will try file search after error on extracting {config_names} with {file_list}: {ex}")
+                continue
+
+        # If files not extracted, try search for expected files in the name list of the archive
+        if (len(file_list) < 1) and do_search:
+            logging.debug(f"Trying to find the config files in the archive for {config_names}.")
+            name_list = archive.namelist()
+            leftovers = deepcopy(config_names)  # to track any that are not found.
+            for cn in config_names:
+                for suffix in bundle_suffixes:
+                    found = False
+                    for n in name_list:
+                        if (f"{cn}{suffix}").casefold() in n.casefold():
+                            found = True
+                            archive.extract(member=n, path=dest_folder)
+                            break
+                    if found:
+                        leftovers.remove(cn)
+                        break
+
+            if len(leftovers) > 0:
+                raise IOError(f"Failed to extract content for these config(s): {leftovers}.")
+
+        return file_list
+
+    # End of helper functions
+
     if isinstance(config_names, str):
         config_names = [config_names]
 
-    name, _ = os.path.splitext(os.path.basename(bundle_path))
+    name, _ = os.path.splitext(os.path.basename(bundle_path))  # bundle file name same archive folder name
     parser = ConfigParser()
 
     # Parser to read the required metadata and extra config contents from the archive
-    with zipfile.ZipFile(bundle_path, "r") as archive:
-        name_list = archive.namelist()
-        metadata_relative_path = "extra/metadata.json"
-        metadata_text = _read_from_archive(archive, name, metadata_relative_path, name_list)
-        parser.read_meta(f=json.loads(metadata_text))
-
-        for cn in config_names:
-            config_relative_path = f"extra/{cn}.json"
-            config_text = _read_from_archive(archive, name, config_relative_path, name_list)
-            parser.read_config(f=json.loads(config_text))
+    with tempfile.TemporaryDirectory() as tmp_dir:
+        with zipfile.ZipFile(bundle_path, "r") as archive:
+            metadata_config_name = "metadata"
+            metadata_text = _read_from_archive(archive, name, metadata_config_name)
+            parser.read_meta(f=json.loads(metadata_text))
+
+            # now get the other named configs
+            file_list = _extract_from_archive(archive, name, config_names, tmp_dir)
+            parser.read_config([Path(tmp_dir, f_path) for f_path in file_list])
 
     parser.parse()
 
     return parser
 
 
 DISALLOW_LOAD_SAVE = ["LoadImage", "SaveImage"]
@@ -196,14 +264,15 @@
         self.postproc_name: str = postproc_name
         self.inferer_name: str = inferer_name
         self.config_names: List[str] = _ensure_str_list(config_names)
 
 
 DEFAULT_BundleConfigNames = BundleConfigNames()
 
+
 # The operator env decorator defines the required pip packages commonly used in the Bundles.
 # The MONAI Deploy App SDK packager currently relies on the App to consolidate all required packages in order to
 # install them in the MAP Docker image.
 # TODO: Dynamically setting the pip_packages env on init requires the bundle path be passed in. Apps using this
 #       operator may choose to pass in a accessible bundle path at development and packaging stage. Ideally,
 #       the bundle path should be passed in by the Packager, e.g. via env var, when the App is initialized.
 #       As of now, the Packager only passes in the model path after the App including all operators are init'ed.
@@ -257,15 +326,15 @@
         Args:
             input_mapping (List[IOMapping]): Define the inputs' name, type, and storage type.
             output_mapping (List[IOMapping]): Defines the outputs' name, type, and storage type.
             model_name (Optional[str], optional): Name of the model/bundle, needed in multi-model case.
                                                   Defaults to "".
             bundle_path (Optional[str], optional): For completing . Defaults to None.
             bundle_config_names (BundleConfigNames, optional): Relevant config item names in a the bundle.
-                                                               Defaults to None.
+                                                               Defaults to DEFAULT_BundleConfigNames.
         """
 
         super().__init__(*args, **kwargs)
         self._executing = False
         self._lock = Lock()
 
         self._model_name = model_name.strip() if isinstance(model_name, str) else ""
@@ -696,15 +765,14 @@
         img_meta_dict: Dict = img.metadata()
 
         if (
             not img_meta_dict
             or ("spacing" in img_meta_dict and "original_affine" in img_meta_dict)
             or "row_pixel_spacing" not in img_meta_dict
         ):
-
             return img.asnumpy(), img_meta_dict
         else:
             return self._convert_from_image_dicom_source(img)
 
     def _convert_from_image_dicom_source(self, img: Image) -> Tuple[np.ndarray, Dict]:
         """Converts the Image object to the expected numpy array with metadata dictionary.
```

## monai/deploy/operators/monai_seg_inference_operator.py

```diff
@@ -11,40 +11,49 @@
 
 from threading import Lock
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 
 from monai.deploy.utils.importutil import optional_import
+from monai.utils import StrEnum  # Will use the built-in StrEnum when SDK requires Python 3.11.
 
 MONAI_UTILS = "monai.utils"
 torch, _ = optional_import("torch", "1.5")
 np_str_obj_array_pattern, _ = optional_import("torch.utils.data._utils.collate", name="np_str_obj_array_pattern")
 Dataset, _ = optional_import("monai.data", name="Dataset")
 DataLoader, _ = optional_import("monai.data", name="DataLoader")
 ImageReader_, image_reader_ok_ = optional_import("monai.data", name="ImageReader")
 # Dynamic class is not handled so make it Any for now: https://github.com/python/mypy/issues/2477
 ImageReader: Any = ImageReader_
 if not image_reader_ok_:
     ImageReader = object  # for 'class InMemImageReader(ImageReader):' to work
 decollate_batch, _ = optional_import("monai.data", name="decollate_batch")
 sliding_window_inference, _ = optional_import("monai.inferers", name="sliding_window_inference")
+simple_inference, _ = optional_import("monai.inferers", name="SimpleInferer")
 ensure_tuple, _ = optional_import(MONAI_UTILS, name="ensure_tuple")
 MetaKeys, _ = optional_import(MONAI_UTILS, name="MetaKeys")
 SpaceKeys, _ = optional_import(MONAI_UTILS, name="SpaceKeys")
 Compose_, _ = optional_import("monai.transforms", name="Compose")
 # Dynamic class is not handled so make it Any for now: https://github.com/python/mypy/issues/2477
 Compose: Any = Compose_
 
 import monai.deploy.core as md
 from monai.deploy.core import ExecutionContext, Image, InputContext, IOType, OutputContext
 
 from .inference_operator import InferenceOperator
 
-__all__ = ["MonaiSegInferenceOperator", "InMemImageReader"]
+__all__ = ["MonaiSegInferenceOperator", "InfererType", "InMemImageReader"]
+
+
+class InfererType(StrEnum):
+    """Represents the supported types of the inferer, e.g. Simple and Sliding Window."""
+
+    SIMPLE = "simple"
+    SLIDING_WINDOW = "sliding_window"
 
 
 @md.input("image", Image, IOType.IN_MEMORY)
 @md.output("seg_image", Image, IOType.IN_MEMORY)
 @md.env(pip_packages=["monai>=1.0.0", "torch>=1.10.2", "numpy>=1.21"])
 class MonaiSegInferenceOperator(InferenceOperator):
     """This segmentation operator uses MONAI transforms and Sliding Window Inference.
@@ -57,44 +66,54 @@
     """
 
     # For testing the app directly, the model should be at the following path.
     MODEL_LOCAL_PATH = "model/model.ts"
 
     def __init__(
         self,
-        roi_size: Union[Sequence[int], int],
+        roi_size: Optional[Union[Sequence[int], int]],
         pre_transforms: Compose,
         post_transforms: Compose,
         model_name: Optional[str] = "",
-        overlap: float = 0.5,
+        overlap: float = 0.25,
+        sw_batch_size: int = 4,
+        inferer: Union[InfererType, str] = InfererType.SLIDING_WINDOW,
         *args,
         **kwargs,
     ):
         """Creates a instance of this class.
 
         Args:
-            roi_size (Union[Sequence[int], int]): The tensor size used in inference.
+            roi_size (Union[Sequence[int], int]): The window size to execute "SLIDING_WINDOW" evaluation.
+                                                  An optional input only to be passed for "SLIDING_WINDOW".
+                                                  If using a "SIMPLE" Inferer, this input is ignored.
             pre_transforms (Compose): MONAI Compose object used for pre-transforms.
             post_transforms (Compose): MONAI Compose object used for post-transforms.
             model_name (str, optional): Name of the model. Default to "" for single model app.
-            overlap (float): The overlap used in sliding window inference.
+            overlap (float): The amount of overlap between scans along each spatial dimension. Defaults to 0.25.
+                             Applicable for "SLIDING_WINDOW" only.
+            sw_batch_size(int): The batch size to run window slices. Defaults to 4.
+                           Applicable for "SLIDING_WINDOW" only.
+            inferer (InfererType): The type of inferer to use, "SIMPLE" or "SLIDING_WINDOW". Defaults to "SLIDING_WINDOW".
         """
 
         super().__init__()
         self._executing = False
         self._lock = Lock()
         self._input_dataset_key = "image"
         self._pred_dataset_key = "pred"
         self._input_image = None  # Image will come in when compute is called.
         self._reader: Any = None
         self._roi_size = ensure_tuple(roi_size)
         self._pre_transform = pre_transforms
         self._post_transforms = post_transforms
         self._model_name = model_name.strip() if isinstance(model_name, str) else ""
-        self.overlap = overlap
+        self._overlap = overlap
+        self._sw_batch_size = sw_batch_size
+        self._inferer = inferer
 
     @property
     def roi_size(self):
         """The ROI size of tensors used in prediction."""
         return self._roi_size
 
     @roi_size.setter
@@ -130,14 +149,36 @@
 
     @overlap.setter
     def overlap(self, val: float):
         if val < 0 or val > 1:
             raise ValueError("Overlap must be between 0 and 1.")
         self._overlap = val
 
+    @property
+    def sw_batch_size(self):
+        """The batch size to run window slices"""
+        return self._sw_batch_size
+
+    @sw_batch_size.setter
+    def sw_batch_size(self, val: int):
+        if not isinstance(val, int) or val < 0:
+            raise ValueError("sw_batch_size must be a positive integer.")
+        self._sw_batch_size = val
+
+    @property
+    def inferer(self) -> Union[InfererType, str]:
+        """The type of inferer to use"""
+        return self._inferer
+
+    @inferer.setter
+    def inferer(self, val: InfererType):
+        if not isinstance(val, InfererType):
+            raise ValueError(f"Value must be of the correct type {InfererType}.")
+        self._inferer = val
+
     def _convert_dicom_metadata_datatype(self, metadata: Dict):
         """Converts metadata in pydicom types to the corresponding native types.
 
         It is known that some values of the metadata are of the pydicom types, for images converted
         from DICOM series. Need to use this function to convert the types with best effort and for
         the few knowns metadata attributes, until the following issue is addressed:
             https://github.com/Project-MONAI/monai-deploy-app-sdk/issues/185
@@ -214,22 +255,30 @@
 
             dataset = Dataset(data=[{self._input_dataset_key: img_name}], transform=pre_transforms)
             dataloader = DataLoader(dataset, batch_size=1, shuffle=False, num_workers=0)
 
             with torch.no_grad():
                 for d in dataloader:
                     images = d[self._input_dataset_key].to(device)
-                    sw_batch_size = 4
-                    d[self._pred_dataset_key] = sliding_window_inference(
-                        inputs=images,
-                        roi_size=self._roi_size,
-                        sw_batch_size=sw_batch_size,
-                        overlap=self.overlap,
-                        predictor=model,
-                    )
+                    if self._inferer == InfererType.SLIDING_WINDOW:
+                        # Uses the util function to drive the sliding_window inferer
+                        d[self._pred_dataset_key] = sliding_window_inference(
+                            inputs=images,
+                            roi_size=self._roi_size,
+                            sw_batch_size=self._sw_batch_size,
+                            overlap=self._overlap,
+                            predictor=model,
+                        )
+                    elif self._inferer == InfererType.SIMPLE:
+                        # Instantiates the SimpleInferer and directly uses its __call__ function
+                        d[self._pred_dataset_key] = simple_inference()(inputs=images, network=model)
+                    else:
+                        raise ValueError(
+                            f"Unknown inferer: {self._inferer}. Available options are sliding_window or simple."
+                        )
                     d = [post_transforms(i) for i in decollate_batch(d)]
                     out_ndarray = d[0][self._pred_dataset_key].cpu().numpy()
                     # Need to squeeze out the channel dim fist
                     out_ndarray = np.squeeze(out_ndarray, 0)
                     # NOTE: The domain Image object simply contains a Arraylike obj as image as of now.
                     #       When the original DICOM series is converted by the Series to Volume operator,
                     #       using pydicom pixel_array, the 2D ndarray of each slice has index order HW, and
@@ -237,16 +286,18 @@
                     #       the image gets transposed to WHD and used as such in the inference pipeline.
                     #       So once post-transforms have completed, and the channel is squeezed out,
                     #       the resultant ndarray for the prediction image needs to be transposed back, so the
                     #       array index order is back to DHW, the same order as the in-memory input Image obj.
                     out_ndarray = out_ndarray.T.astype(np.uint8)
                     print(f"Output Seg image numpy array shaped: {out_ndarray.shape}")
                     print(f"Output Seg image pixel max value: {np.amax(out_ndarray)}")
+                    print(f"Output Seg image pixel min value: {np.amin(out_ndarray)}")
                     out_image = Image(out_ndarray, input_img_metadata)
                     op_output.set(out_image, "seg_image")
+
         finally:
             # Reset state on completing this method execution.
             with self._lock:
                 self._executing = False
 
     def pre_process(self, data: Any, *args, **kwargs) -> Union[Any, Image, Tuple[Any, ...], Dict[Any, Any]]:
         """Transforms input before being used for predicting on a model.
```

## monai/deploy/packager/constants.py

```diff
@@ -12,15 +12,15 @@
 
 class DefaultValues:
     """
     This class contains default values for various parameters.
     """
 
     DOCKER_FILE_NAME = "dockerfile"
-    BASE_IMAGE = "nvcr.io/nvidia/pytorch:21.07-py3"
+    BASE_IMAGE = "nvcr.io/nvidia/pytorch:22.08-py3"
     DOCKERFILE_TYPE = "pytorch"
     WORK_DIR = "/var/monai/"
     INPUT_DIR = "input"
     OUTPUT_DIR = "output"
     MODELS_DIR = "/opt/monai/models"
     API_VERSION = "0.1.0"
     TIMEOUT = 0
```

## monai/deploy/packager/templates.py

```diff
@@ -1,22 +1,22 @@
-# Copyright 2021 MONAI Consortium
+# Copyright 2021-2022 MONAI Consortium
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License
 
 COMMON_FOOTPRINT = """
     USER root
 
-    RUN pip install --no-cache-dir --upgrade setuptools==57.4.0 pip==21.3.1 wheel==0.37.0 numpy>=1.21
+    RUN pip install --no-cache-dir --upgrade setuptools==59.5.0 pip==22.3 wheel==0.37.1 numpy>=1.21.6
 
     RUN mkdir -p /etc/monai/ \\
      && mkdir -p /opt/monai/ \\
      && mkdir -p {working_dir} \\
      && mkdir -p {app_dir} \\
      && mkdir -p {executor_dir} \\
      && mkdir -p {full_input_path} \\
@@ -68,14 +68,15 @@
     ENV DEBIAN_FRONTEND=noninteractive
     ENV TERM=xterm-256color
     ENV MONAI_INPUTPATH={full_input_path}
     ENV MONAI_OUTPUTPATH={full_output_path}
     ENV MONAI_WORKDIR={working_dir}
     ENV MONAI_APPLICATION={app_dir}
     ENV MONAI_TIMEOUT={timeout}
+    ENV MONAI_MODELPATH={models_dir}
 
     RUN apt update \\
      && apt upgrade -y --no-install-recommends \\
      && apt install -y --no-install-recommends \\
         build-essential \\
         python3 \\
         python3-pip \\
@@ -102,14 +103,15 @@
     ENV DEBIAN_FRONTEND=noninteractive
     ENV TERM=xterm-256color
     ENV MONAI_INPUTPATH={full_input_path}
     ENV MONAI_OUTPUTPATH={full_output_path}
     ENV MONAI_WORKDIR={working_dir}
     ENV MONAI_APPLICATION={app_dir}
     ENV MONAI_TIMEOUT={timeout}
+    ENV MONAI_MODELPATH={models_dir}
 
     RUN apt update \\
      && apt upgrade -y --no-install-recommends \\
      && apt install -y --no-install-recommends \\
         curl \\
         unzip \\
      && apt autoremove -y \\
```

## monai/deploy/packager/util.py

```diff
@@ -13,14 +13,15 @@
 import logging
 import os
 import shutil
 import subprocess
 import sys
 import tempfile
 from argparse import Namespace
+from pathlib import Path
 from typing import Dict
 
 from monai.deploy.exceptions import WrongValueError
 from monai.deploy.packager.constants import DefaultValues
 from monai.deploy.packager.templates import Template
 from monai.deploy.utils.fileutil import checksum
 from monai.deploy.utils.importutil import dist_module_path, dist_requires, get_application
@@ -37,15 +38,18 @@
     template to build MAP
     Args:
         base_image (str): potential base image to build MAP Docker image
     Returns:
         str: returns string identifier of the dockerfile template to build MAP
         if valid base image provided, returns empty string otherwise
     """
-    valid_prefixes = {"nvcr.io/nvidia/cuda": "ubuntu", "nvcr.io/nvidia/pytorch": "pytorch"}
+    if "rocm" in base_image:
+        valid_prefixes = {"rocm/pytorch": "ubuntu"}
+    else:
+        valid_prefixes = {"nvcr.io/nvidia/cuda": "ubuntu", "nvcr.io/nvidia/pytorch": "pytorch"}
 
     for prefix, template in valid_prefixes.items():
         if prefix in base_image:
             return template
 
     return ""
 
@@ -85,19 +89,19 @@
     # Verify proper base image:
     dockerfile_type = ""
 
     if args.base:
         dockerfile_type = verify_base_image(args.base)
         if not dockerfile_type:
             logger.error(
-                "Provided base image '{}' is not supported \n \
-                          Please provide a Cuda or Pytorch image from https://ngc.nvidia.com/ (nvcr.io/nvidia)".format(
-                    args.base
-                )
+                "Provided base image '{}' is not supported \n                         Please provide a ROCm or Cuda"
+                " based Pytorch image from \n                         https://hub.docker.com/r/rocm/pytorch or"
+                " https://ngc.nvidia.com/ (nvcr.io/nvidia)".format(args.base)
             )
+
             sys.exit(1)
 
     processed_args["dockerfile_type"] = dockerfile_type if args.base else DefaultValues.DOCKERFILE_TYPE
 
     base_image = DefaultValues.BASE_IMAGE
     if args.base:
         base_image = args.base
@@ -173,15 +177,17 @@
         # Use local requirements.txt packages if provided, otherwise use sdk provided packages
         if local_requirements_file:
             with open(local_requirements_file, "r") as lr:
                 for line in lr:
                     requirements_file.write(line)
         else:
             requirements_file.writelines("\n".join(pip_packages))
-    map_requirements_path = "/tmp/requirements.txt"
+
+    # Parameter for the Dockerfile for copying content to internal path
+    map_requirements_path = str(Path(app_dir) / "requirements.txt")
 
     # Copy model files to temp directory (under 'model' folder)
     target_models_path = os.path.join(temp_dir, "models")
     os.makedirs(target_models_path, exist_ok=True)
     for model_entry in local_models:
         model_name = model_entry["name"]
         model_path = model_entry["path"]
@@ -225,15 +231,15 @@
     # Write out .dockerignore file
     dockerignore_file_path = os.path.join(temp_dir, ".dockerignore")
     with open(dockerignore_file_path, "w") as dockerignore_file:
         docker_ignore_template = Template.get_template(".dockerignore")
         dockerignore_file.write(docker_ignore_template)
 
     # Build dockerfile into an MAP image
-    docker_build_cmd = f'''docker build -f "{docker_file_path}" -t {tag} "{temp_dir}"'''
+    docker_build_cmd = f"""docker build -f {docker_file_path!r} -t {tag} {temp_dir!r}"""
     if sys.platform != "win32":
         docker_build_cmd += """ --build-arg MONAI_UID=$(id -u) --build-arg MONAI_GID=$(id -g)"""
     if no_cache:
         docker_build_cmd += " --no-cache"
     proc = subprocess.Popen(docker_build_cmd, stdout=subprocess.PIPE, shell=True)
 
     logger.debug("Docker image build command: %s", docker_build_cmd)
```

## monai/deploy/runner/runner.py

```diff
@@ -16,14 +16,15 @@
 import shutil
 import sys
 import tempfile
 from pathlib import Path
 from typing import Tuple
 
 from monai.deploy.runner.utils import get_requested_gpus, run_cmd, verify_image
+from monai.deploy.utils.deviceutil import has_rocm
 
 logger = logging.getLogger("app_runner")
 
 
 def fetch_map_manifest(map_name: str) -> Tuple[dict, dict, int]:
     """
     Execute MONAI Application Package and fetch application manifest.
@@ -36,15 +37,15 @@
         pkg_info: package manifest as a python dict
         returncode: command return code
     """
     logger.info("\nReading MONAI App Package manifest...")
 
     with tempfile.TemporaryDirectory() as info_dir:
         if sys.platform == "win32":
-            cmd = f'docker run --rm -a STDOUT -a STDERR -v "{info_dir}":/var/run/monai/export/config {map_name}'
+            cmd = f'docker run --rm -a STDOUT -a STDERR -v " {info_dir}":/var/run/monai/export/config {map_name}'
         else:
             cmd = f"""docker_id=$(docker create {map_name})
 docker cp $docker_id:/etc/monai/app.json "{info_dir}/app.json"
 docker cp $docker_id:/etc/monai/pkg.json "{info_dir}/pkg.json"
 docker rm -v $docker_id > /dev/null
 """
         returncode = run_cmd(cmd)
@@ -83,30 +84,31 @@
         returncode: command returncode
     """
     cmd = "docker run --rm -a STDERR"
 
     # Use nvidia-docker if GPU resources are requested
     requested_gpus = get_requested_gpus(pkg_info)
     if requested_gpus > 0:
-        cmd = "nvidia-docker run --rm -a STDERR"
+        if not has_rocm():
+            cmd = "nvidia-docker run --rm -a STDERR"
 
     if not quiet:
         cmd += " -a STDOUT"
 
     # Use POSIX path for input and output paths as local paths are mounted to those paths in the container.
     map_input = Path(app_info["input"]["path"]).as_posix()
     map_output = Path(app_info["output"]["path"]).as_posix()
     if not posixpath.isabs(map_input):
         map_input = posixpath.join(app_info["working-directory"], map_input)
 
     if not posixpath.isabs(map_output):
         map_output = posixpath.join(app_info["working-directory"], map_output)
 
-    cmd += f' -e MONAI_INPUTPATH="{map_input}"'
-    cmd += f' -e MONAI_OUTPUTPATH="{map_output}"'
+    cmd += ' -e MONAI_INPUTPATH="{}"'.format(map_input)
+    cmd += ' -e MONAI_OUTPUTPATH="{}"'.format(map_output)
     # TODO(bhatt-piyush): Handle model environment correctly (maybe solved by fixing 'monai-exec')
     cmd += " -e MONAI_MODELPATH=/opt/monai/models"
 
     map_command = app_info["command"]
     # TODO(bhatt-piyush): Fix 'monai-exec' to work correctly.
     cmd += ' -v "{}":"{}" -v "{}":"{}" --shm-size=1g --entrypoint "/bin/bash" "{}" -c "{}"'.format(
         input_path.absolute(), map_input, output_path.absolute(), map_output, map_name, map_command
@@ -156,20 +158,21 @@
         pkg_info: package manifest as a python dict
 
     Returns:
         True if all dependencies are satisfied, otherwise False.
     """
     requested_gpus = get_requested_gpus(pkg_info)
     if requested_gpus > 0:
-        # check for nvidia-docker
-        prog = "nvidia-docker"
-        logger.info('--> Verifying if "%s" is installed...\n', prog)
-        if not shutil.which(prog):
-            logger.error('ERROR: "%s" not installed, please install nvidia-docker.', prog)
-            return False
+        if not has_rocm():
+            # check for nvidia-docker
+            prog = "nvidia-docker"
+            logger.info('--> Verifying if "%s" is installed...\n', prog)
+            if not shutil.which(prog):
+                logger.error('ERROR: "%s" not installed, please install nvidia-docker.', prog)
+                return False
 
     return True
 
 
 def main(args: argparse.Namespace):
     """
     Main entry function for MONAI Application Runner.
```

## monai/deploy/utils/argparse_types.py

```diff
@@ -32,15 +32,15 @@
         If path doesn't exist, create the directory and return absolute path as a pathlib.Path object.
     """
     dir_path = Path(path).absolute()
     if dir_path.exists():
         if dir_path.is_dir():
             return dir_path
         else:
-            raise argparse.ArgumentTypeError(f"Expected directory path: '{dir_path}' is not a directory")
+            raise argparse.ArgumentTypeError(f"Expected directory path: {dir_path!r} is not a directory")
 
     # create directory
     dir_path.mkdir(parents=True)
     return dir_path
 
 
 def valid_existing_dir_path(path: str) -> Path:
@@ -54,15 +54,15 @@
         If path exists and is a directory, return absolute path as a pathlib.Path object.
 
         If path doesn't exist or it is not a directory, raises argparse.ArgumentTypeError.
     """
     dir_path = Path(path).absolute()
     if dir_path.exists() and dir_path.is_dir():
         return dir_path
-    raise argparse.ArgumentTypeError(f"No such directory: '{dir_path}'")
+    raise argparse.ArgumentTypeError(f"No such directory: {dir_path!r}")
 
 
 def valid_existing_path(path: str) -> Path:
     """Helper type checking and type converting method for ArgumentParser.add_argument
     to convert string input to pathlib.Path if the given file/folder path exists.
 
     Args:
@@ -72,8 +72,8 @@
         If path exists, return absolute path as a pathlib.Path object.
 
         If path doesn't exist, raises argparse.ArgumentTypeError.
     """
     file_path = Path(path).absolute()
     if file_path.exists():
         return file_path
-    raise argparse.ArgumentTypeError(f"No such file/folder: '{file_path}'")
+    raise argparse.ArgumentTypeError(f"No such file/folder: {file_path!r}")
```

## monai/deploy/utils/importutil.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 MONAI Consortium
+# Copyright 2021-2022 MONAI Consortium
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
@@ -110,15 +110,15 @@
 
     Returns:
         A file path of the class.
     """
 
     try:
         return Path(inspect.getfile(cls))
-    except TypeError:
+    except (TypeError, OSError):
         # If in IPython shell, use inspect.stack() to get the caller's file path
         stack = inspect.stack()
         for frame in stack:
             if frame.filename.endswith("interactiveshell.py") and frame.function == "run_code":
                 return Path("ipython")
         # If not in IPython shell, re-raise the error
         raise
@@ -151,15 +151,15 @@
 
 
 def exact_version(the_module, version_str: str = "") -> bool:
     """
     Returns True if the module's __version__ matches version_str
     """
     if not hasattr(the_module, "__version__"):
-        warnings.warn(f"{the_module} has no attribute __version__ in exact_version check.")
+        warnings.warn(f"{the_module} has no attribute __version__ in exact_version check.", stacklevel=2)
         return False
     return bool(the_module.__version__ == version_str)
 
 
 def optional_import(
     module: str,
     version: str = "",
@@ -234,15 +234,15 @@
             return the_module, True
         if not version_args and version_checker(pkg, f"{version}"):
             return the_module, True
 
     # preparing lazy error message
     msg = descriptor.format(actual_cmd)
     if version and tb is None:  # a pure version issue
-        msg += f" (requires '{module} {version}' by '{version_checker.__name__}')"
+        msg += f" (requires '{module} {version}' by {version_checker.__name__!r})"
     if exception_str:
         msg += f" ({exception_str})"
 
     class _LazyRaise:
         def __init__(self, *_args, **_kwargs):
             _default_msg = (
                 f"{msg}."
@@ -276,22 +276,53 @@
 
 def is_dist_editable(project_name: str) -> bool:
     distributions: Dict = {v.key: v for v in pkg_resources.working_set}
     dist: Any = distributions.get(project_name)
     if not hasattr(dist, "egg_info"):
         return False
     egg_info = Path(dist.egg_info)
-    if egg_info.is_dir() and egg_info.suffix == ".egg-info":
-        return True
+    if egg_info.is_dir():
+        if egg_info.suffix == ".egg-info":
+            return True
+        elif egg_info.suffix == ".dist-info":
+            if (egg_info / "direct_url.json").exists():
+                import json
+
+                # Check direct_url.json for "editable": true
+                # (https://packaging.python.org/en/latest/specifications/direct-url/)
+                with open(egg_info / "direct_url.json", "r") as f:
+                    data = json.load(f)
+                    try:
+                        if data["dir_info"]["editable"]:
+                            return True
+                    except KeyError:
+                        pass
     return False
 
 
 def dist_module_path(project_name: str) -> str:
     distributions: Dict = {v.key: v for v in pkg_resources.working_set}
     dist: Any = distributions.get(project_name)
+    if hasattr(dist, "egg_info"):
+        egg_info = Path(dist.egg_info)
+        if egg_info.is_dir() and egg_info.suffix == ".dist-info":
+            if (egg_info / "direct_url.json").exists():
+                import json
+
+                # Check direct_url.json for "url"
+                # (https://packaging.python.org/en/latest/specifications/direct-url/)
+                with open(egg_info / "direct_url.json", "r") as f:
+                    data = json.load(f)
+                    try:
+                        file_url = data["url"]
+                        if file_url.startswith("file://"):
+                            return str(file_url[7:])
+                    except KeyError:
+                        pass
+
     if hasattr(dist, "module_path"):
         return str(dist.module_path)
     return ""
 
 
 def is_module_installed(project_name: str) -> bool:
     distributions: Dict = {v.key: v for v in pkg_resources.working_set}
```

## monai/deploy/utils/sizeutil.py

```diff
@@ -62,26 +62,26 @@
             raise ValueError("Negative size not allowed.")
         return size
     if not isinstance(size, str):
         raise TypeError("Size must be a string or integer.")
 
     m = re.match(r"^\s*(?P<size>(([1-9]\d+)|\d)(\.\d+)?)\s*(?P<unit>[a-z]{1,3})?\s*$", size, re.IGNORECASE)
     if not m:
-        raise ValueError(f"Invalid size string ('{size}').")
+        raise ValueError(f"Invalid size string ({size!r}).")
 
     parsed_size = float(m.group("size"))
 
     unit_match = m.group("unit")
     if unit_match:
         parsed_unit = unit_match.lower()
     else:
         parsed_unit = "b"  # default to bytes
 
     if parsed_unit not in BYTES_UNIT:
-        raise ValueError(f"Invalid unit ('{parsed_unit}').")
+        raise ValueError(f"Invalid unit ({parsed_unit!r}).")
 
     return int(parsed_size * BYTES_UNIT[parsed_unit])
 
 
 def convert_bytes(num_bytes: int, unit: str = "Mi") -> Union[str, int]:
     """Converts a number of bytes to a string representation.
 
@@ -111,15 +111,15 @@
     if not isinstance(num_bytes, int):
         raise TypeError("Size must be an integer.")
     if num_bytes < 0:
         raise ValueError("Negative size not allowed.")
 
     unit_lowered = unit.lower()
     if unit_lowered not in BYTES_UNIT:
-        raise ValueError(f"Invalid unit ('{unit}').")
+        raise ValueError(f"Invalid unit ({unit!r}).")
 
     converted = float(num_bytes) / BYTES_UNIT[unit_lowered] * 10
 
     if unit_lowered == "b":
         return int(converted) // 10  # return as integer
 
     if int(converted) % 10 == 0:
```

## monai/deploy/utils/version.py

```diff
@@ -119,14 +119,14 @@
             build = ""
 
         semver_str = f"{release}{pre_release}{build}"
 
         if SEMVER_REGEX.match(semver_str):
             return semver_str
         else:
-            raise ValueError(f"Invalid semver string: '{semver_str}' (from '{version_str}')")
+            raise ValueError(f"Invalid semver string: {semver_str!r} (from {version_str!r})")
     else:
         raise ValueError(f"Invalid version string: {version_str}")
 
 
 if __name__ == "__main__":
     print(get_sdk_semver())
```

## Comparing `monai_deploy_app_sdk-0.5.0.dist-info/LICENSE` & `monai_deploy_app_sdk-0.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `monai_deploy_app_sdk-0.5.0.dist-info/METADATA` & `monai_deploy_app_sdk-0.5.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: monai-deploy-app-sdk
-Version: 0.5.0
+Version: 0.5.1
 Summary: A framework and associated tools to design, verify and analyze performance of MONAI apps
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
-Project-URL: Documentation, https://docs.monai.io/projects/monai-deploy-app-sdk/en/latest/
+Project-URL: Documentation, https://docs.monai.io/projects/monai-deploy-app-sdk/en/stable/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/monai-deploy-app-sdk/issues
 Project-URL: Source Code, https://github.com/Project-MONAI/monai-deploy-app-sdk
 Platform: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
-Requires-Dist: numpy (>=1.21.2)
+Requires-Dist: numpy (>=1.21.6)
 Requires-Dist: networkx (>=2.4)
 Requires-Dist: colorama (>=0.4.1)
-Requires-Dist: typeguard (>=2.12.1)
+Requires-Dist: typeguard (>=3.0.0)
 Provides-Extra: all
 Requires-Dist: cucim (~=21.06) ; extra == 'all'
 Provides-Extra: cucim
 Requires-Dist: cucim (~=21.06) ; extra == 'cucim'
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/Project-MONAI/MONAI/dev/docs/images/MONAI-logo-color.png" width="50%" alt='project-monai'>
@@ -84,32 +84,32 @@
 monai-deploy run simple_app:latest input output
 ```
 
 ### [Tutorials](https://docs.monai.io/projects/monai-deploy-app-sdk/en/latest/getting_started/tutorials/index.html)
 
 Tutorials are provided to help getting started with the App SDK, to name but a few below.
 
-#### [1) Creating a simple image processing app](https://docs.monai.io/projects/monai-deploy-app-sdk/en/latest/getting_started/tutorials/01_simple_app.html)
+#### [1) Creating a simple image processing app](https://docs.monai.io/projects/monai-deploy-app-sdk/en/latest/getting_started/tutorials/simple_app.html)
 
-#### [2) Creating MedNIST Classifier app](https://docs.monai.io/projects/monai-deploy-app-sdk/en/latest/getting_started/tutorials/02_mednist_app.html)
+#### [2) Creating MedNIST Classifier app](https://docs.monai.io/projects/monai-deploy-app-sdk/en/latest/getting_started/tutorials/mednist_app.html)
 
 YouTube Video:
 
 - [MedNIST Classification Example](https://www.youtube.com/watch?v=WwjilJFHuU4)
 
-### [3) Creating a Segmentation app](https://docs.monai.io/projects/monai-deploy-app-sdk/en/latest/getting_started/tutorials/03_segmentation_app.html)
+### [3) Creating a Segmentation app](https://docs.monai.io/projects/monai-deploy-app-sdk/en/latest/getting_started/tutorials/segmentation_app.html)
 
 YouTube Video:
 
 - [Spleen Organ Segmentation - Jupyter Notebook Tutorial](https://www.youtube.com/watch?v=cqDVxzYt9lY)
 - [Spleen Organ Segmentation - Deep Dive](https://www.youtube.com/watch?v=nivgfD4pwWE)
 
-### [4) Creating a Segmentation app](https://docs.monai.io/projects/monai-deploy-app-sdk/en/latest/getting_started/tutorials/03_segmentation_viz_app.html)
+### [4) Creating a Segmentation app including visualization with Clara Viz](https://docs.monai.io/projects/monai-deploy-app-sdk/en/latest/getting_started/tutorials/segmentation_clara-viz_app.html)
 
-### [5) Creating a Segmentation app consuming a MONAI Bundle](https://docs.monai.io/projects/monai-deploy-app-sdk/en/latest/getting_started/tutorials/06_monai_bundle_app.html)
+### [5) Creating a Segmentation app consuming a MONAI Bundle](https://docs.monai.io/projects/monai-deploy-app-sdk/en/latest/getting_started/tutorials/monai_bundle_app.html)
 
 ### [Examples](https://docs.monai.io/projects/monai-deploy-app-sdk/en/latest/getting_started/examples.html)
 
 <https://github.com/Project-MONAI/monai-deploy-app-sdk/tree/main/examples/apps> has example apps that you can see.
 
 - ai_livertumor_seg_app
 - ai_spleen_seg_app
```

## Comparing `monai_deploy_app_sdk-0.5.0.dist-info/RECORD` & `monai_deploy_app_sdk-0.5.1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,84 +1,87 @@
 monai/deploy/__init__.py,sha256=cg_n8jgCtMpjsW5DVexjVI_hvxAWINXRcFv4tXz_2Rk,815
-monai/deploy/_version.py,sha256=tuEIHuyD3fgW5j2l3wFHGOxighFTMi-kjarFIa9LLg8,497
+monai/deploy/_version.py,sha256=F-HpOWp5wj0438hQffmYTPXXiVG3j-P229c0gdQH2bA,497
+monai/deploy/_version_local.py,sha256=munT4eLvF4rCneNJmmFhb8Ynr3mTKamoUSqj8LF7rxg,496
 monai/deploy/exceptions.py,sha256=8o4Xym6WQktL2FRiei7D06Jr9zlrNu91aIHc4bWNCdw,1359
 monai/deploy/logging.json,sha256=50nU8-uOWnPkw9JHXySMscMOFdB-W0rELBRPmDfw04g,665
 monai/deploy/cli/__init__.py,sha256=Y8vDfuPHxlP_YTh_dfGI63HahoJfhndnBLeHPnlmb5c,771
 monai/deploy/cli/__main__.py,sha256=QMBo8u_RRF1OZyKnkb_F3xMOFz5ebh_gHbdij44alQM,666
 monai/deploy/cli/exec_command.py,sha256=HFjkBB15mLiFEaW7CyPCncp68F-D5rfU3IYIyGe3VPM,2991
 monai/deploy/cli/main.py,sha256=q-afRNppEfA7jbV75ldukP3hIgMyro5OK5B9vETA_jc,4624
 monai/deploy/core/__init__.py,sha256=RQ77EmGj6R6HIDkJwkvEuSHwvc096fhlGELIRzf0PYg,1182
 monai/deploy/core/app_context.py,sha256=sxZUSpMk5nSGwzuuG1A9QRZnfGNHYkZ-Dc9XRsI6uj0,2579
-monai/deploy/core/application.py,sha256=t6I7ouU7AC51xJKGSdnlTM8tkr9fo4fqo9zpabdZuHw,17711
-monai/deploy/core/env.py,sha256=LZWJWia3Wj6errFW4LF13VCluM5cQFBfOjsk9-EFhyo,3094
+monai/deploy/core/application.py,sha256=PJ2DqHalCo3a--jRO5MuYJCLhnfDbgfSHs8e6lqMHPU,17722
+monai/deploy/core/env.py,sha256=UWSvXXxTDp-VXNgT2aj4jQoyKxLume_ZWs5dy9wIdYE,3094
 monai/deploy/core/execution_context.py,sha256=lAoHHi0ZLOJTADnPe0Fs5lvMsMeHVlhnOtBlQRD4RTg,4121
-monai/deploy/core/io_context.py,sha256=W8fbxnI0S-7nrnc-A-s5BRLOu1_3WBiGert3PTJ54_g,5125
+monai/deploy/core/io_context.py,sha256=ahj9UhcFzEpHO6EywWk-EjbGeUU1gE2ss8lJ2JKh6aU,5116
 monai/deploy/core/io_type.py,sha256=3I2vsVIM4AUmOZKuMZlojctANntJLVnPI-I3FcjTL9E,736
 monai/deploy/core/operator.py,sha256=6KVnasJ7bBzy1hbn8Yn8cAG7Om2H1flj8m0Y5Pi2bWQ,10925
 monai/deploy/core/operator_info.py,sha256=RgtsnCXltCARDHqKis91eJZjfmqQ28LU_UKkHpPc9T4,2599
-monai/deploy/core/resource.py,sha256=0X_WWi-SuigdkJSA-P8RQ0oMxdGsAr9hu6P_xa6sybw,5094
+monai/deploy/core/resource.py,sha256=1Iw8IORiYyXBS4D3QBT_ttXQ60uWoBdUS17rk4-jygE,5140
 monai/deploy/core/runtime_env.py,sha256=S7LIhKeXvmM9PMJLmov8aecLfNwkhsfmWnOT2a3OUc8,2046
 monai/deploy/core/datastores/__init__.py,sha256=fbbUSdRYdKLnyppa5mCw020Mbot4mACm8S7B6G4Ilf8,790
 monai/deploy/core/datastores/datastore.py,sha256=R06esFD-adxN9oBwXXoG1Z1FZfcSJStSkEV8gyx_U5I,2062
 monai/deploy/core/datastores/factory.py,sha256=caiW28bvDDhc3lGGvdbJkraloBawmA87eZ3b83AOmn8,1522
 monai/deploy/core/datastores/memory.py,sha256=kUP508ux3y7RWnLKmWZXrzoYRJS0KisySU-5ZRusL7I,1258
 monai/deploy/core/domain/__init__.py,sha256=ZJRVP9QMKuW1YC2ZrCYiEkTdvqnb-ZlZgFqX6jFC1EM,1068
-monai/deploy/core/domain/datapath.py,sha256=OZlw9VV8htCjR2FdIFPMA3NKKCITN0FdpMNHu-J89n0,2901
+monai/deploy/core/domain/datapath.py,sha256=hZFlW01Ombj18ZdZD7lJ8q-rQg7p8c3doNYzI8UpN18,2901
 monai/deploy/core/domain/dicom_series.py,sha256=4EgYfqKmIZoi5HqPfHGbAduqq4s6TLq9kvGzJ8f62X4,8530
 monai/deploy/core/domain/dicom_series_selection.py,sha256=_bDQ8FmxdEKgYzPsGuP5H7B631DJCua60Uz7Kqr8OlI,5605
 monai/deploy/core/domain/dicom_sop_instance.py,sha256=N6SmSiOdt8iOLAONy5t_mEq26GyWxeRYdM_qZ8oqOJM,1963
 monai/deploy/core/domain/dicom_study.py,sha256=uyvqYMh_QRYgWUN3MbSd59tVuRK40L3OkVXJYoLUxVo,3611
 monai/deploy/core/domain/domain.py,sha256=ffhF1s9ZRBsdjuGvUiSqXuijwPQff-OaZxewwO5d1jc,1057
 monai/deploy/core/domain/image.py,sha256=EYEvEsBHrA6UGZGZsaNjRXtVWOgGt4UU_ZujGipAAVk,1863
 monai/deploy/core/executors/__init__.py,sha256=NNygZ6IwHqh2c7TA7Gamc6wrOIHWv8mD8UVpREDu8Jw,1005
 monai/deploy/core/executors/executor.py,sha256=OiIaYsAVYIGjUSNaEqd4Ce1BygRoxMWcd_X4j3_5rsI,2118
 monai/deploy/core/executors/factory.py,sha256=bvNKY2CJS7CUeDRcqRHMTlxjeS4oq_En_xh6I09bZzc,1584
 monai/deploy/core/executors/multi_process_executor.py,sha256=PtmiMGKOYWXknsxnwz58JGhECG-gYFjYiMtl2cn8-Dw,1964
 monai/deploy/core/executors/multi_threaded_executor.py,sha256=EkWhWR_BtFqBIWo_r7abcm8CoEvpEgrgA9-typmbpb8,1796
-monai/deploy/core/executors/single_process_executor.py,sha256=1vOXrRdlNICLRdDwDrE2dpqy5TQlC1v2B449D5b48JY,7361
+monai/deploy/core/executors/single_process_executor.py,sha256=MtwVU9e21P2TE5LTUcVZjrqOzRkXVz0zYem2ulJ4o1A,7359
 monai/deploy/core/graphs/__init__.py,sha256=SMvGkra6rHGyECZOltSCO7iC3i_6_zfIYA1Wk_BUQ_Q,770
 monai/deploy/core/graphs/factory.py,sha256=7nsx9Sc47DMTXNfL4LvxJENSS5zldWEGLw2LijnNV6Y,1528
 monai/deploy/core/graphs/graph.py,sha256=IK-LoMGSH50qgkXk3jYxg8nszYa1LTQqiBmPiojGHDI,3094
-monai/deploy/core/graphs/nx_digraph.py,sha256=yUxSj_tEb0q0nHGezn3nSn7c0J20SeiF4qMYapM99oc,2139
+monai/deploy/core/graphs/nx_digraph.py,sha256=6GcyfnPFxke1OUooywqKabk7EmsJt62MuYQe5-Ddqlg,2137
 monai/deploy/core/models/__init__.py,sha256=CEpqFDgMBE3SAcKRn3V7pGe5AWEWgphn3AKJpGLdFqE,950
 monai/deploy/core/models/factory.py,sha256=aVJUD24QzMaJAlE_y4_AYQJAzVDlPtGHLJ6GiF-LrcQ,2248
-monai/deploy/core/models/model.py,sha256=rHW6JFiBST-CTUA-Q4iaBOefrITHOFjd7JWLTv_5qIg,7865
-monai/deploy/core/models/named_model.py,sha256=aAg5SkVypBDd8XwVItJZLD-s_sJfqlnSbQM0RzwrJjc,3398
+monai/deploy/core/models/model.py,sha256=GSaA2NizeUyMRcmvyLvdTG9GamAB1E7wyk1CU7Pkkjo,7865
+monai/deploy/core/models/named_model.py,sha256=s4UkXLfni2wgc1y4xLqafuJ-MxY7Uek_8kur3hNe3QI,3398
 monai/deploy/core/models/torch_model.py,sha256=tkqSnkMOdprTcTUbfXZaNRCuOd3d_uak2xLd7Psw4gI,4472
 monai/deploy/core/models/triton_model.py,sha256=PpK9_bwJ1YidjAKsxwuJXLopEyfUWzn_iitaeKvwFCA,4650
-monai/deploy/operators/__init__.py,sha256=orD8pv9FnzBg4SlJ6RRp2_Fk-UuFYbYyqJ3McQhCv8k,2090
+monai/deploy/operators/__init__.py,sha256=wy6vFzs9WL8gKeI05noCBj235bJfaa3jx0kzLwVfJX8,2164
 monai/deploy/operators/clara_viz_operator.py,sha256=kTQDyr4wiVCAIU8zCTOg7YxW51lm8CzscHV2UXG6EKA,5606
-monai/deploy/operators/dicom_data_loader_operator.py,sha256=peNNcnDjXSSV1sZ7uF07_qjed38VmBhJSjimZBuifmE,13935
-monai/deploy/operators/dicom_encapsulated_pdf_writer_operator.py,sha256=PIT0DLzm--umnUS4XRvg1vGolLsurR__iK9BJhOzomc,12526
-monai/deploy/operators/dicom_seg_writer_operator.py,sha256=nJejYkNLhn70041ChiTNOvhBTXupb6VWGP_MTkNzSkg,19847
-monai/deploy/operators/dicom_series_selector_operator.py,sha256=CTTn5fc2yNWvt7lYA2Z0kTIrGDhFbCPE5kdCmDtHC3s,16601
-monai/deploy/operators/dicom_series_to_volume_operator.py,sha256=raKxsY8St_sSZVInTg_GAmhUuQkAiwGZLkofCHLc4sQ,16661
-monai/deploy/operators/dicom_text_sr_writer_operator.py,sha256=wBg6mifehzOcSfrMOYUGf_rYLtasvy5t7wK5_D7JOxE,13201
-monai/deploy/operators/dicom_utils.py,sha256=FZIl_-qk0RlE0zwEZf9Uija9u8b3WYDY8rM-5miBlW0,12724
+monai/deploy/operators/dicom_data_loader_operator.py,sha256=uVNIlKw_gW7uvpSMx81VXP5xznld5IBva3sKbVxiZYk,13957
+monai/deploy/operators/dicom_encapsulated_pdf_writer_operator.py,sha256=TZT9wzCvb0PX5M66r-_fjX-Ooo-YncnvBxYVUxt6UQ8,12525
+monai/deploy/operators/dicom_seg_writer_operator.py,sha256=wOfrlGtEfJJQr-7CALtddJ4bqkJSsukEO5oFjULDxKU,20276
+monai/deploy/operators/dicom_series_selector_operator.py,sha256=4O4QjtVRLNzJt-fCqrfCHk9eaCXPv521q33C3RnhmYI,16599
+monai/deploy/operators/dicom_series_to_volume_operator.py,sha256=kA9E6g2YoPEfAj_x_y_UyDQ99-SFM7wMIIPwxT6SarE,16660
+monai/deploy/operators/dicom_text_sr_writer_operator.py,sha256=kDURccW-tpAWAe4BJTDXKtyJQLQdARoFbhTrvHg69Gg,13200
+monai/deploy/operators/dicom_utils.py,sha256=gX2kQ7Ug-gYG0mMYJ_qth9m1_snvEomxaocYDC0-cvQ,12722
 monai/deploy/operators/inference_operator.py,sha256=qKrzJ_lQblvw9Cxjqnrm3yDVmYoRFDlaZPTDoMg6taY,2975
-monai/deploy/operators/monai_bundle_inference_operator.py,sha256=tnI5Ye61JT5oH21uG5IMdK9jXUDZacVlMy5OpKnUaIU,36177
-monai/deploy/operators/monai_seg_inference_operator.py,sha256=HIRK4021Z12We04jGXt_vITOV9OrjyOhob0q0P667Zo,20280
+monai/deploy/operators/monai_bundle_inference_operator.py,sha256=tffedP8wxJcB-3mENyiYrZKGCgNB4iOuA79FW34SREo,39476
+monai/deploy/operators/monai_seg_inference_operator.py,sha256=wOeFUdFSThpWw1Bjl9RvG2B9qysP0OWwEWm0l1gFQb4,22856
+monai/deploy/operators/nii_data_loader_operator.py,sha256=xwco9cXkxrDlju-WjcTa6Kw72v-al05vfnZ3QJb7qmc,1963
 monai/deploy/operators/png_converter_operator.py,sha256=JdvyuXRbUXYCfTS5lxGp9fzb7IcxCnVNbg-9TsXVawI,3179
 monai/deploy/operators/publisher_operator.py,sha256=PDDOEYTaj5noGx3n_XS9U4QK2s7wjBt1p_VByVDOzuo,22010
 monai/deploy/operators/stl_conversion_operator.py,sha256=C4cGMfEWBM_919QSH-8X-6qzx5S4J2CfHz1ycbsmzm4,17563
 monai/deploy/packager/__init__.py,sha256=x_LZN2_TJWKGRK2ctBlUGeiMeFQ3LqW6dxittEkYM4k,574
-monai/deploy/packager/constants.py,sha256=WRc6psMZUhwXINJbR41Unyzq8fPEsmdkOnUw1KKAYgs,955
+monai/deploy/packager/constants.py,sha256=APCUAfLkQOg6g7eDBsBfHI8Nq9OUeP6D6jqDHZXBZgs,955
 monai/deploy/packager/package_command.py,sha256=QYlv8D7-hmn727c1rJnqpfwvwBTy53-fwI4HgIkip9E,2530
-monai/deploy/packager/templates.py,sha256=2poHpdxbcwS1lAgu1zvafs1prFb_Yi4MZtnqzxtbCOs,5239
-monai/deploy/packager/util.py,sha256=Z7eYQAX3Bo45BJw_J67zCbZSfshQOv7KKA0m1a8D2as,14360
+monai/deploy/packager/templates.py,sha256=d0kF4Q2SlONbDUDyptAu9mFMhSnTG9sv_8hsVSaRorU,5318
+monai/deploy/packager/util.py,sha256=ZYEMT0k1bbAfKw9-ukcxgMDaFF-_9g5Jj2_vtl3UWVM,14645
 monai/deploy/runner/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 monai/deploy/runner/run_command.py,sha256=8jtujUCVtEvHNVpvBVju5VhOmU0iqzLZnLpcqdczB00,1759
-monai/deploy/runner/runner.py,sha256=SOmpHc1gUduOiRy5-9aSTeAUZON7naCo81GEq4oCuVg,6943
+monai/deploy/runner/runner.py,sha256=qLITu5Igt_YSLP1fpMcTmBlvGEb-RP6ollJnKas6vqw,7093
 monai/deploy/runner/utils.py,sha256=ZaLvjIb_3CRbDa2mRSm7YyrjhY6f-p5OBzVpE0UbjUY,2455
 monai/deploy/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-monai/deploy/utils/argparse_types.py,sha256=sesS-l08pM18iG2XpVSnV6k8oFepdZkL6plhvAomum4,2897
+monai/deploy/utils/argparse_types.py,sha256=zCg8E61qQA8IRBmX708TMFNyAiMnZBw3aoRvXeFafls,2897
+monai/deploy/utils/deviceutil.py,sha256=hXmkMaKuHxrmpoKuc4tExr7BB7zOQIqnPLncznZzkuk,1140
 monai/deploy/utils/fileutil.py,sha256=9ep1glfCrCm-h85x5j_TKVs9KwxYTWrOtr_JV4Kb3Z0,1838
-monai/deploy/utils/importutil.py,sha256=obx-8YO5ewgpqL05OpXzwwV20VZLuJf-372a6e-YDqw,12624
-monai/deploy/utils/sizeutil.py,sha256=S_hegbFply6xutZx3D9tGuKqDoMsfXzw6c6RrMAIYZk,4142
+monai/deploy/utils/importutil.py,sha256=CxvlmwiCxHOAfIvdEtodF8RGioKpZs-C7ETYIC9GGMM,13957
+monai/deploy/utils/sizeutil.py,sha256=yej-GxO3NlguVhyy8WjcZB-Ard49eubtxAi90z0v5UE,4142
 monai/deploy/utils/spinner.py,sha256=PpqAE2CfBXEw1qEWUP9woW-vw28L4Tyn5AUeWsbnXwc,2597
-monai/deploy/utils/version.py,sha256=MGXnbE6HyrEanWa5BSID_xD8CzAlO4Sxgzmsx5E13Fc,4512
-monai_deploy_app_sdk-0.5.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-monai_deploy_app_sdk-0.5.0.dist-info/METADATA,sha256=Y8w6AxHcBrDVByD_CH7D6PL_6guG0wg0k5LW6JV1mCk,6607
-monai_deploy_app_sdk-0.5.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-monai_deploy_app_sdk-0.5.0.dist-info/entry_points.txt,sha256=Tmf1rCh_1wDk_ePd1_U2W5E-o5LKyZHpj_qfe7vEytc,60
-monai_deploy_app_sdk-0.5.0.dist-info/top_level.txt,sha256=UaNwRzLGORdus41Ip446s3bBfViLkdkDsXDo34J2P44,6
-monai_deploy_app_sdk-0.5.0.dist-info/RECORD,,
+monai/deploy/utils/version.py,sha256=gnHKAX6ep91ECJOJE1EPx-WTx_BM5Zxv8kDqAPuBswg,4512
+monai_deploy_app_sdk-0.5.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+monai_deploy_app_sdk-0.5.1.dist-info/METADATA,sha256=GqOqi4SO9Egt3Ol0ySoUKltqlQHQZisgdcYV23d7vVY,6636
+monai_deploy_app_sdk-0.5.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+monai_deploy_app_sdk-0.5.1.dist-info/entry_points.txt,sha256=Tmf1rCh_1wDk_ePd1_U2W5E-o5LKyZHpj_qfe7vEytc,60
+monai_deploy_app_sdk-0.5.1.dist-info/top_level.txt,sha256=UaNwRzLGORdus41Ip446s3bBfViLkdkDsXDo34J2P44,6
+monai_deploy_app_sdk-0.5.1.dist-info/RECORD,,
```

