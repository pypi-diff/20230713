# Comparing `tmp/sam-3.1.8.tar.gz` & `tmp/sam-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sam-3.1.8.tar", last modified: Thu Mar 16 13:52:52 2023, max compression
+gzip compressed data, was "sam-3.1.9.tar", last modified: Wed Apr  5 14:16:46 2023, max compression
```

## Comparing `sam-3.1.8.tar` & `sam-3.1.9.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.795521 sam-3.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-16 13:52:38.000000 sam-3.1.8/.config.example
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-16 13:52:38.000000 sam-3.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-16 13:52:38.000000 sam-3.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-03-16 13:52:52.795521 sam-3.1.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3658 2023-03-16 13:52:38.000000 sam-3.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.763521 sam-3.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:38.000000 sam-3.1.8/docs/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-16 13:52:38.000000 sam-3.1.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-16 13:52:38.000000 sam-3.1.8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.767521 sam-3.1.8/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/data_sources.rst
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/datasets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/exploration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/feature_engineering.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.771520 sam-3.1.8/docs/source/general_documents/
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/anomaly_detection.md
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/data_exploration.md
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/data_storage.md
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/feature_extraction.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.775521 sam-3.1.8/docs/source/general_documents/images/
--rw-r--r--   0 runner    (1001) docker     (123)    38042 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/images/autocorrelation.png
--rw-r--r--   0 runner    (1001) docker     (123)   249426 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/images/automatic_rolling_figure.png
--rw-r--r--   0 runner    (1001) docker     (123)    56687 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/images/automatic_rolling_importances.png
--rw-r--r--   0 runner    (1001) docker     (123)    48401 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/images/cv_holdout.png
--rw-r--r--   0 runner    (1001) docker     (123)    40691 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/images/cv_sliding_window.png
--rw-r--r--   0 runner    (1001) docker     (123)    99791 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/images/extreme_values_example_testset.png
--rw-r--r--   0 runner    (1001) docker     (123)    78370 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/images/extreme_values_example_trainset.png
--rw-r--r--   0 runner    (1001) docker     (123)    27274 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/images/flatline_removal_example.png
--rw-r--r--   0 runner    (1001) docker     (123)    14608 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/images/incident_heatmap.png
--rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/images/precision_recall_curve.png
--rw-r--r--   0 runner    (1001) docker     (123)    26400 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/images/quantile_importances_barplot.png
--rw-r--r--   0 runner    (1001) docker     (123)    12880 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/images/quantile_importances_barplot_sum.png
--rw-r--r--   0 runner    (1001) docker     (123)   140444 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/images/quantile_plot.png
--rw-r--r--   0 runner    (1001) docker     (123)    21435 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/images/synthetic_temperature.png
--rw-r--r--   0 runner    (1001) docker     (123)   168587 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/images/technical_overview.png
--rw-r--r--   0 runner    (1001) docker     (123)    15770 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/images/threshold_curve.png
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/production_platform.md
--rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/project_approach.md
--rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/tsfresh.md
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents/weather_features.md
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/general_documents.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.775521 sam-3.1.8/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)    80811 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/metrics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/models.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/preprocessing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/validation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-03-16 13:52:38.000000 sam-3.1.8/docs/source/visualization.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.775521 sam-3.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 13:52:38.000000 sam-3.1.8/examples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    18864 2023-03-16 13:52:38.000000 sam-3.1.8/examples/feature_engineering.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   193745 2023-03-16 13:52:38.000000 sam-3.1.8/examples/lasso.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   212630 2023-03-16 13:52:38.000000 sam-3.1.8/examples/mlp.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-03-16 13:52:38.000000 sam-3.1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.775521 sam-3.1.8/sam/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-16 13:52:38.000000 sam-3.1.8/sam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.779521 sam-3.1.8/sam/data_sources/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-16 13:52:38.000000 sam-3.1.8/sam/data_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-03-16 13:52:38.000000 sam-3.1.8/sam/data_sources/mongo_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-03-16 13:52:38.000000 sam-3.1.8/sam/data_sources/synthetic_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.779521 sam-3.1.8/sam/data_sources/weather/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-16 13:52:38.000000 sam-3.1.8/sam/data_sources/weather/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-03-16 13:52:38.000000 sam-3.1.8/sam/data_sources/weather/knmi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-03-16 13:52:38.000000 sam-3.1.8/sam/data_sources/weather/openweathermap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-03-16 13:52:38.000000 sam-3.1.8/sam/data_sources/weather/regenradar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-16 13:52:38.000000 sam-3.1.8/sam/data_sources/weather/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.779521 sam-3.1.8/sam/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-16 13:52:38.000000 sam-3.1.8/sam/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.779521 sam-3.1.8/sam/datasets/data/
--rw-r--r--   0 runner    (1001) docker     (123)    37618 2023-03-16 13:52:38.000000 sam-3.1.8/sam/datasets/data/rainbow_beach.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1530202 2023-03-16 13:52:38.000000 sam-3.1.8/sam/datasets/data/sewage_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-16 13:52:38.000000 sam-3.1.8/sam/datasets/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.783521 sam-3.1.8/sam/exploration/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-16 13:52:38.000000 sam-3.1.8/sam/exploration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15465 2023-03-16 13:52:38.000000 sam-3.1.8/sam/exploration/find_incidents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-03-16 13:52:38.000000 sam-3.1.8/sam/exploration/lag_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-03-16 13:52:38.000000 sam-3.1.8/sam/exploration/top_correlation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.783521 sam-3.1.8/sam/feature_engineering/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-16 13:52:38.000000 sam-3.1.8/sam/feature_engineering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21092 2023-03-16 13:52:38.000000 sam-3.1.8/sam/feature_engineering/automatic_rolling_engineering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-03-16 13:52:38.000000 sam-3.1.8/sam/feature_engineering/base_feature_engineering.py
--rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-03-16 13:52:38.000000 sam-3.1.8/sam/feature_engineering/decompose_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-03-16 13:52:38.000000 sam-3.1.8/sam/feature_engineering/lag_range.py
--rw-r--r--   0 runner    (1001) docker     (123)    23163 2023-03-16 13:52:38.000000 sam-3.1.8/sam/feature_engineering/rolling_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-03-16 13:52:38.000000 sam-3.1.8/sam/feature_engineering/simple_feature_engineering.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-03-16 13:52:38.000000 sam-3.1.8/sam/feature_engineering/weather_spei.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.787521 sam-3.1.8/sam/logging_functions/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-16 13:52:38.000000 sam-3.1.8/sam/logging_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-03-16 13:52:38.000000 sam-3.1.8/sam/logging_functions/dataframe_characteristics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-03-16 13:52:38.000000 sam-3.1.8/sam/logging_functions/new_columns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.787521 sam-3.1.8/sam/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-16 13:52:38.000000 sam-3.1.8/sam/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-03-16 13:52:38.000000 sam-3.1.8/sam/metrics/custom_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-03-16 13:52:38.000000 sam-3.1.8/sam/metrics/incident_recall.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-03-16 13:52:38.000000 sam-3.1.8/sam/metrics/keras_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-03-16 13:52:38.000000 sam-3.1.8/sam/metrics/mase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-03-16 13:52:38.000000 sam-3.1.8/sam/metrics/quantile_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-03-16 13:52:38.000000 sam-3.1.8/sam/metrics/r2_calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-03-16 13:52:38.000000 sam-3.1.8/sam/metrics/tilted_loss_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.791521 sam-3.1.8/sam/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-03-16 13:52:38.000000 sam-3.1.8/sam/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27735 2023-03-16 13:52:38.000000 sam-3.1.8/sam/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-03-16 13:52:38.000000 sam-3.1.8/sam/models/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-03-16 13:52:38.000000 sam-3.1.8/sam/models/constant_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    17186 2023-03-16 13:52:38.000000 sam-3.1.8/sam/models/keras_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-03-16 13:52:38.000000 sam-3.1.8/sam/models/lasso_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-03-16 13:52:38.000000 sam-3.1.8/sam/models/linear_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    26914 2023-03-16 13:52:38.000000 sam-3.1.8/sam/models/mlp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-03-16 13:52:38.000000 sam-3.1.8/sam/models/sam_shap_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-16 13:52:38.000000 sam-3.1.8/sam/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.791521 sam-3.1.8/sam/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-03-16 13:52:38.000000 sam-3.1.8/sam/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-03-16 13:52:38.000000 sam-3.1.8/sam/preprocessing/clip_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-03-16 13:52:38.000000 sam-3.1.8/sam/preprocessing/correct_extremes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-03-16 13:52:38.000000 sam-3.1.8/sam/preprocessing/data_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-03-16 13:52:38.000000 sam-3.1.8/sam/preprocessing/differencing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-03-16 13:52:38.000000 sam-3.1.8/sam/preprocessing/normalize_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-03-16 13:52:38.000000 sam-3.1.8/sam/preprocessing/rnn_reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-03-16 13:52:38.000000 sam-3.1.8/sam/preprocessing/sam_reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-03-16 13:52:38.000000 sam-3.1.8/sam/preprocessing/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-16 13:52:38.000000 sam-3.1.8/sam/preprocessing/train_test_split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.791521 sam-3.1.8/sam/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-16 13:52:38.000000 sam-3.1.8/sam/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-03-16 13:52:38.000000 sam-3.1.8/sam/utils/dataframe_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-03-16 13:52:38.000000 sam-3.1.8/sam/utils/sklearnhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-03-16 13:52:38.000000 sam-3.1.8/sam/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.795521 sam-3.1.8/sam/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-16 13:52:38.000000 sam-3.1.8/sam/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-03-16 13:52:38.000000 sam-3.1.8/sam/validation/base_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-03-16 13:52:38.000000 sam-3.1.8/sam/validation/flatline_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-03-16 13:52:38.000000 sam-3.1.8/sam/validation/mad_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-03-16 13:52:38.000000 sam-3.1.8/sam/validation/outside_range_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-03-16 13:52:38.000000 sam-3.1.8/sam/validation/setup_validation_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.795521 sam-3.1.8/sam/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-16 13:52:38.000000 sam-3.1.8/sam/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-03-16 13:52:38.000000 sam-3.1.8/sam/visualization/diagnostic_flatline_removal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-03-16 13:52:38.000000 sam-3.1.8/sam/visualization/extreme_removal_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-03-16 13:52:38.000000 sam-3.1.8/sam/visualization/incident_heatmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    11878 2023-03-16 13:52:38.000000 sam-3.1.8/sam/visualization/performance_evaluation_fixed_predict_ahead.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-03-16 13:52:38.000000 sam-3.1.8/sam/visualization/plot_feature_importances.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-03-16 13:52:38.000000 sam-3.1.8/sam/visualization/precision_recall.py
--rw-r--r--   0 runner    (1001) docker     (123)    15102 2023-03-16 13:52:38.000000 sam-3.1.8/sam/visualization/quantile_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-03-16 13:52:38.000000 sam-3.1.8/sam/visualization/rolling_correlations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-03-16 13:52:38.000000 sam-3.1.8/sam/visualization/threshold_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:52:52.779521 sam-3.1.8/sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-03-16 13:52:52.000000 sam-3.1.8/sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-03-16 13:52:52.000000 sam-3.1.8/sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 13:52:52.000000 sam-3.1.8/sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-16 13:52:52.000000 sam-3.1.8/sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-16 13:52:52.000000 sam-3.1.8/sam.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-16 13:52:52.795521 sam-3.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.657226 sam-3.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-05 14:16:30.000000 sam-3.1.9/.config.example
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-05 14:16:30.000000 sam-3.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-05 14:16:30.000000 sam-3.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-05 14:16:46.657226 sam-3.1.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3658 2023-04-05 14:16:30.000000 sam-3.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.633226 sam-3.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:30.000000 sam-3.1.9/docs/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-05 14:16:30.000000 sam-3.1.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-05 14:16:30.000000 sam-3.1.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.637226 sam-3.1.9/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/data_sources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/datasets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/exploration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/feature_engineering.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.637226 sam-3.1.9/docs/source/general_documents/
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/anomaly_detection.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/data_exploration.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/data_storage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/feature_extraction.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.641226 sam-3.1.9/docs/source/general_documents/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    38042 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/images/autocorrelation.png
+-rw-r--r--   0 runner    (1001) docker     (123)   249426 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/images/automatic_rolling_figure.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56687 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/images/automatic_rolling_importances.png
+-rw-r--r--   0 runner    (1001) docker     (123)    48401 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/images/cv_holdout.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40691 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/images/cv_sliding_window.png
+-rw-r--r--   0 runner    (1001) docker     (123)    99791 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/images/extreme_values_example_testset.png
+-rw-r--r--   0 runner    (1001) docker     (123)    78370 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/images/extreme_values_example_trainset.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27274 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/images/flatline_removal_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14608 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/images/incident_heatmap.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/images/precision_recall_curve.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26400 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/images/quantile_importances_barplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12880 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/images/quantile_importances_barplot_sum.png
+-rw-r--r--   0 runner    (1001) docker     (123)   140444 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/images/quantile_plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21435 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/images/synthetic_temperature.png
+-rw-r--r--   0 runner    (1001) docker     (123)   168587 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/images/technical_overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15770 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/images/threshold_curve.png
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/production_platform.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/project_approach.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/tsfresh.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents/weather_features.md
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/general_documents.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.641226 sam-3.1.9/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    80811 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/metrics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/preprocessing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/validation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-05 14:16:30.000000 sam-3.1.9/docs/source/visualization.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.641226 sam-3.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-05 14:16:30.000000 sam-3.1.9/examples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    18864 2023-04-05 14:16:30.000000 sam-3.1.9/examples/feature_engineering.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   193745 2023-04-05 14:16:30.000000 sam-3.1.9/examples/lasso.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   212630 2023-04-05 14:16:30.000000 sam-3.1.9/examples/mlp.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-05 14:16:30.000000 sam-3.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.641226 sam-3.1.9/sam/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-05 14:16:30.000000 sam-3.1.9/sam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.645226 sam-3.1.9/sam/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-05 14:16:30.000000 sam-3.1.9/sam/data_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-05 14:16:30.000000 sam-3.1.9/sam/data_sources/mongo_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-04-05 14:16:30.000000 sam-3.1.9/sam/data_sources/synthetic_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.645226 sam-3.1.9/sam/data_sources/weather/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-05 14:16:30.000000 sam-3.1.9/sam/data_sources/weather/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-04-05 14:16:30.000000 sam-3.1.9/sam/data_sources/weather/knmi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-05 14:16:30.000000 sam-3.1.9/sam/data_sources/weather/openweathermap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-05 14:16:30.000000 sam-3.1.9/sam/data_sources/weather/regenradar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-05 14:16:30.000000 sam-3.1.9/sam/data_sources/weather/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.645226 sam-3.1.9/sam/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-05 14:16:30.000000 sam-3.1.9/sam/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.645226 sam-3.1.9/sam/datasets/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    37618 2023-04-05 14:16:30.000000 sam-3.1.9/sam/datasets/data/rainbow_beach.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1530202 2023-04-05 14:16:30.000000 sam-3.1.9/sam/datasets/data/sewage_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-05 14:16:30.000000 sam-3.1.9/sam/datasets/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.649226 sam-3.1.9/sam/exploration/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-05 14:16:30.000000 sam-3.1.9/sam/exploration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15465 2023-04-05 14:16:30.000000 sam-3.1.9/sam/exploration/find_incidents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-05 14:16:30.000000 sam-3.1.9/sam/exploration/lag_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-04-05 14:16:30.000000 sam-3.1.9/sam/exploration/top_correlation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.649226 sam-3.1.9/sam/feature_engineering/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-05 14:16:30.000000 sam-3.1.9/sam/feature_engineering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21092 2023-04-05 14:16:30.000000 sam-3.1.9/sam/feature_engineering/automatic_rolling_engineering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-05 14:16:30.000000 sam-3.1.9/sam/feature_engineering/base_feature_engineering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-04-05 14:16:30.000000 sam-3.1.9/sam/feature_engineering/decompose_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-05 14:16:30.000000 sam-3.1.9/sam/feature_engineering/lag_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23163 2023-04-05 14:16:30.000000 sam-3.1.9/sam/feature_engineering/rolling_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-04-05 14:16:30.000000 sam-3.1.9/sam/feature_engineering/simple_feature_engineering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-04-05 14:16:30.000000 sam-3.1.9/sam/feature_engineering/weather_spei.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.649226 sam-3.1.9/sam/logging_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-05 14:16:30.000000 sam-3.1.9/sam/logging_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-05 14:16:30.000000 sam-3.1.9/sam/logging_functions/dataframe_characteristics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-05 14:16:30.000000 sam-3.1.9/sam/logging_functions/new_columns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.649226 sam-3.1.9/sam/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-05 14:16:30.000000 sam-3.1.9/sam/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-05 14:16:30.000000 sam-3.1.9/sam/metrics/custom_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-04-05 14:16:30.000000 sam-3.1.9/sam/metrics/incident_recall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-05 14:16:30.000000 sam-3.1.9/sam/metrics/keras_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-05 14:16:30.000000 sam-3.1.9/sam/metrics/mase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-05 14:16:30.000000 sam-3.1.9/sam/metrics/quantile_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-04-05 14:16:30.000000 sam-3.1.9/sam/metrics/r2_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-04-05 14:16:30.000000 sam-3.1.9/sam/metrics/tilted_loss_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.653226 sam-3.1.9/sam/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-05 14:16:30.000000 sam-3.1.9/sam/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27735 2023-04-05 14:16:30.000000 sam-3.1.9/sam/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-04-05 14:16:30.000000 sam-3.1.9/sam/models/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-04-05 14:16:30.000000 sam-3.1.9/sam/models/constant_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17186 2023-04-05 14:16:30.000000 sam-3.1.9/sam/models/keras_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-04-05 14:16:30.000000 sam-3.1.9/sam/models/lasso_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-05 14:16:30.000000 sam-3.1.9/sam/models/linear_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26914 2023-04-05 14:16:30.000000 sam-3.1.9/sam/models/mlp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-05 14:16:30.000000 sam-3.1.9/sam/models/sam_shap_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-05 14:16:30.000000 sam-3.1.9/sam/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.653226 sam-3.1.9/sam/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-05 14:16:30.000000 sam-3.1.9/sam/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-05 14:16:30.000000 sam-3.1.9/sam/preprocessing/clip_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-04-05 14:16:30.000000 sam-3.1.9/sam/preprocessing/correct_extremes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-05 14:16:30.000000 sam-3.1.9/sam/preprocessing/data_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-05 14:16:30.000000 sam-3.1.9/sam/preprocessing/differencing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-04-05 14:16:30.000000 sam-3.1.9/sam/preprocessing/normalize_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-04-05 14:16:30.000000 sam-3.1.9/sam/preprocessing/rnn_reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-04-05 14:16:30.000000 sam-3.1.9/sam/preprocessing/sam_reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-04-05 14:16:30.000000 sam-3.1.9/sam/preprocessing/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-05 14:16:30.000000 sam-3.1.9/sam/preprocessing/train_test_split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.653226 sam-3.1.9/sam/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-05 14:16:30.000000 sam-3.1.9/sam/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-04-05 14:16:30.000000 sam-3.1.9/sam/utils/dataframe_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-04-05 14:16:30.000000 sam-3.1.9/sam/utils/sklearnhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-05 14:16:30.000000 sam-3.1.9/sam/utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.657226 sam-3.1.9/sam/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-05 14:16:30.000000 sam-3.1.9/sam/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-05 14:16:30.000000 sam-3.1.9/sam/validation/base_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-05 14:16:30.000000 sam-3.1.9/sam/validation/flatline_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-05 14:16:30.000000 sam-3.1.9/sam/validation/mad_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-05 14:16:30.000000 sam-3.1.9/sam/validation/outside_range_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-05 14:16:30.000000 sam-3.1.9/sam/validation/setup_validation_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.657226 sam-3.1.9/sam/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-05 14:16:30.000000 sam-3.1.9/sam/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-05 14:16:30.000000 sam-3.1.9/sam/visualization/diagnostic_flatline_removal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-05 14:16:30.000000 sam-3.1.9/sam/visualization/extreme_removal_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-05 14:16:30.000000 sam-3.1.9/sam/visualization/incident_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11878 2023-04-05 14:16:30.000000 sam-3.1.9/sam/visualization/performance_evaluation_fixed_predict_ahead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-04-05 14:16:30.000000 sam-3.1.9/sam/visualization/plot_feature_importances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-05 14:16:30.000000 sam-3.1.9/sam/visualization/precision_recall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15102 2023-04-05 14:16:30.000000 sam-3.1.9/sam/visualization/quantile_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-05 14:16:30.000000 sam-3.1.9/sam/visualization/rolling_correlations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-05 14:16:30.000000 sam-3.1.9/sam/visualization/threshold_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:46.645226 sam-3.1.9/sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-05 14:16:46.000000 sam-3.1.9/sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-05 14:16:46.000000 sam-3.1.9/sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:16:46.000000 sam-3.1.9/sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-05 14:16:46.000000 sam-3.1.9/sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-05 14:16:46.000000 sam-3.1.9/sam.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-05 14:16:46.657226 sam-3.1.9/setup.cfg
```

### Comparing `sam-3.1.8/LICENSE` & `sam-3.1.9/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Royal HaskoningDHV
+Copyright (c) 2023 Royal HaskoningDHV
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `sam-3.1.8/PKG-INFO` & `sam-3.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sam
-Version: 3.1.8
+Version: 3.1.9
 Summary: Time series anomaly detection and forecasting
 Author-email: Royal HaskoningDHV <ruben.peters@rhdhv.com>
 License: MIT
 Project-URL: homepage, https://github.com/RoyalHaskoningDHV/sam
 Project-URL: issues, https://github.com/RoyalHaskoningDHV/sam/issues
 Project-URL: discussions, https://github.com/RoyalHaskoningDHV/sam/discussions
 Project-URL: documentation, https://sam-rhdhv.readthedocs.io/en/latest/
@@ -37,15 +37,15 @@
 
 SAM (Smart Asset Management) is a Python package for *timeseries analysis*, *anomaly detection* and *forecasting*.
 
 The documentation is available on [ReadTheDocs](https://sam-rhdhv.readthedocs.io/en/latest/).
 
 Author: [Royal HaskoningDHV](https://global.royalhaskoningdhv.com/)
 
-Email: [ruben.peters@rhdhv.com](mailto:ruben.peters@rhdhv.com)
+Email: [ruud.kassing@rhdhv.com](mailto:ruud.kassing@rhdhv.com)
 
 ## Getting started
 
 ### Installation
 
 The easiest way to install is package is using pip:
 ```
```

### Comparing `sam-3.1.8/README.md` & `sam-3.1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 SAM (Smart Asset Management) is a Python package for *timeseries analysis*, *anomaly detection* and *forecasting*.
 
 The documentation is available on [ReadTheDocs](https://sam-rhdhv.readthedocs.io/en/latest/).
 
 Author: [Royal HaskoningDHV](https://global.royalhaskoningdhv.com/)
 
-Email: [ruben.peters@rhdhv.com](mailto:ruben.peters@rhdhv.com)
+Email: [ruud.kassing@rhdhv.com](mailto:ruud.kassing@rhdhv.com)
 
 ## Getting started
 
 ### Installation
 
 The easiest way to install is package is using pip:
 ```
```

### Comparing `sam-3.1.8/docs/Makefile` & `sam-3.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/make.bat` & `sam-3.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/conf.py` & `sam-3.1.9/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 root_folder = Path(__file__).parents[2]
 
 
 # -- Project information -----------------------------------------------------
 
 project = "sam"
-copyright = "2018-2022, Royal HaskoningDHV"
+copyright = "2018-2023, Royal HaskoningDHV"
 author = "Royal HaskoningDHV"
 
 
 config = toml.load(root_folder / "pyproject.toml")
 
 # The short X.Y version
 version = config["project"]["version"]
```

### Comparing `sam-3.1.8/docs/source/data.rst` & `sam-3.1.9/docs/source/data.rst`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/data_sources.rst` & `sam-3.1.9/docs/source/data_sources.rst`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/examples.rst` & `sam-3.1.9/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/exploration.rst` & `sam-3.1.9/docs/source/exploration.rst`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/feature_engineering.rst` & `sam-3.1.9/docs/source/feature_engineering.rst`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/anomaly_detection.md` & `sam-3.1.9/docs/source/general_documents/anomaly_detection.md`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/data_exploration.md` & `sam-3.1.9/docs/source/general_documents/data_exploration.md`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/data_storage.md` & `sam-3.1.9/docs/source/general_documents/data_storage.md`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/feature_extraction.md` & `sam-3.1.9/docs/source/general_documents/feature_extraction.md`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/images/autocorrelation.png` & `sam-3.1.9/docs/source/general_documents/images/autocorrelation.png`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/images/automatic_rolling_figure.png` & `sam-3.1.9/docs/source/general_documents/images/automatic_rolling_figure.png`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/images/automatic_rolling_importances.png` & `sam-3.1.9/docs/source/general_documents/images/automatic_rolling_importances.png`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/images/cv_holdout.png` & `sam-3.1.9/docs/source/general_documents/images/cv_holdout.png`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/images/cv_sliding_window.png` & `sam-3.1.9/docs/source/general_documents/images/cv_sliding_window.png`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/images/extreme_values_example_testset.png` & `sam-3.1.9/docs/source/general_documents/images/extreme_values_example_testset.png`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/images/extreme_values_example_trainset.png` & `sam-3.1.9/docs/source/general_documents/images/extreme_values_example_trainset.png`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/images/flatline_removal_example.png` & `sam-3.1.9/docs/source/general_documents/images/flatline_removal_example.png`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/images/incident_heatmap.png` & `sam-3.1.9/docs/source/general_documents/images/incident_heatmap.png`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/images/precision_recall_curve.png` & `sam-3.1.9/docs/source/general_documents/images/precision_recall_curve.png`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/images/quantile_importances_barplot.png` & `sam-3.1.9/docs/source/general_documents/images/quantile_importances_barplot.png`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/images/quantile_importances_barplot_sum.png` & `sam-3.1.9/docs/source/general_documents/images/quantile_importances_barplot_sum.png`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/images/quantile_plot.png` & `sam-3.1.9/docs/source/general_documents/images/quantile_plot.png`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/images/synthetic_temperature.png` & `sam-3.1.9/docs/source/general_documents/images/synthetic_temperature.png`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/images/technical_overview.png` & `sam-3.1.9/docs/source/general_documents/images/technical_overview.png`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/images/threshold_curve.png` & `sam-3.1.9/docs/source/general_documents/images/threshold_curve.png`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/project_approach.md` & `sam-3.1.9/docs/source/general_documents/project_approach.md`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/tsfresh.md` & `sam-3.1.9/docs/source/general_documents/tsfresh.md`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/general_documents/weather_features.md` & `sam-3.1.9/docs/source/general_documents/weather_features.md`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/images/logo.png` & `sam-3.1.9/docs/source/images/logo.png`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/index.rst` & `sam-3.1.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/intro.rst` & `sam-3.1.9/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/metrics.rst` & `sam-3.1.9/docs/source/metrics.rst`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/models.rst` & `sam-3.1.9/docs/source/models.rst`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/preprocessing.rst` & `sam-3.1.9/docs/source/preprocessing.rst`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/validation.rst` & `sam-3.1.9/docs/source/validation.rst`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/docs/source/visualization.rst` & `sam-3.1.9/docs/source/visualization.rst`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/examples/feature_engineering.ipynb` & `sam-3.1.9/examples/feature_engineering.ipynb`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/examples/lasso.ipynb` & `sam-3.1.9/examples/lasso.ipynb`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/examples/mlp.ipynb` & `sam-3.1.9/examples/mlp.ipynb`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/pyproject.toml` & `sam-3.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "sam.utils",
     "sam.validation",
     "sam.visualization"
 ]
 
 [project]
 name = "sam"
-version = "3.1.8"
+version = "3.1.9"
 description = "Time series anomaly detection and forecasting"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [{name = "Royal HaskoningDHV", email = "ruben.peters@rhdhv.com"}]
 keywords = ["python", "data-science", "time-series", "forecasting", "anomaly-detection", "asset-management"]
 classifiers = [
```

### Comparing `sam-3.1.8/sam/__init__.py` & `sam-3.1.9/sam/__init__.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/data_sources/mongo_wrapper.py` & `sam-3.1.9/sam/data_sources/mongo_wrapper.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/data_sources/synthetic_data.py` & `sam-3.1.9/sam/data_sources/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/data_sources/weather/knmi.py` & `sam-3.1.9/sam/data_sources/weather/knmi.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/data_sources/weather/openweathermap.py` & `sam-3.1.9/sam/data_sources/weather/openweathermap.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/data_sources/weather/regenradar.py` & `sam-3.1.9/sam/data_sources/weather/regenradar.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/data_sources/weather/utils.py` & `sam-3.1.9/sam/data_sources/weather/utils.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/datasets/data/rainbow_beach.csv` & `sam-3.1.9/sam/datasets/data/rainbow_beach.csv`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/datasets/data/sewage_data.csv` & `sam-3.1.9/sam/datasets/data/sewage_data.csv`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/datasets/datasets.py` & `sam-3.1.9/sam/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/exploration/find_incidents.py` & `sam-3.1.9/sam/exploration/find_incidents.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/exploration/lag_correlation.py` & `sam-3.1.9/sam/exploration/lag_correlation.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/exploration/top_correlation.py` & `sam-3.1.9/sam/exploration/top_correlation.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/feature_engineering/__init__.py` & `sam-3.1.9/sam/feature_engineering/__init__.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/feature_engineering/automatic_rolling_engineering.py` & `sam-3.1.9/sam/feature_engineering/automatic_rolling_engineering.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/feature_engineering/base_feature_engineering.py` & `sam-3.1.9/sam/feature_engineering/base_feature_engineering.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/feature_engineering/decompose_datetime.py` & `sam-3.1.9/sam/feature_engineering/decompose_datetime.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/feature_engineering/lag_range.py` & `sam-3.1.9/sam/feature_engineering/lag_range.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/feature_engineering/rolling_features.py` & `sam-3.1.9/sam/feature_engineering/rolling_features.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/feature_engineering/simple_feature_engineering.py` & `sam-3.1.9/sam/feature_engineering/simple_feature_engineering.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/feature_engineering/weather_spei.py` & `sam-3.1.9/sam/feature_engineering/weather_spei.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/logging_functions/dataframe_characteristics.py` & `sam-3.1.9/sam/logging_functions/dataframe_characteristics.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/logging_functions/new_columns.py` & `sam-3.1.9/sam/logging_functions/new_columns.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/metrics/__init__.py` & `sam-3.1.9/sam/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/metrics/custom_callbacks.py` & `sam-3.1.9/sam/metrics/custom_callbacks.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/metrics/incident_recall.py` & `sam-3.1.9/sam/metrics/incident_recall.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/metrics/keras_metrics.py` & `sam-3.1.9/sam/metrics/keras_metrics.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/metrics/mase.py` & `sam-3.1.9/sam/metrics/mase.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/metrics/quantile_evaluation.py` & `sam-3.1.9/sam/metrics/quantile_evaluation.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/metrics/r2_calculation.py` & `sam-3.1.9/sam/metrics/r2_calculation.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/metrics/tilted_loss_metrics.py` & `sam-3.1.9/sam/metrics/tilted_loss_metrics.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/models/__init__.py` & `sam-3.1.9/sam/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/models/base_model.py` & `sam-3.1.9/sam/models/base_model.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/models/benchmark.py` & `sam-3.1.9/sam/models/benchmark.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/models/constant_model.py` & `sam-3.1.9/sam/models/constant_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,15 +232,18 @@
         validation_data: tuple(pd.DataFrame, pd.Series) (X_val, y_val respectively)
             Data used for validation step
 
         Returns
         -------
         Always returns None, since there is no history object of the fit procedure
         """
-        X_transformed, y_transformed, _, _ = self.preprocess_fit(X, y, validation_data)
+        # preprocess_fit (inherited from BaseTimeseriesRegressor) disallows nan values in X.
+        # ConstantTimeseriesRegressor may accept nan values so fillna(0) is used to (by)pass that
+        # check without affecting the model because X is only used for its shape.
+        X_transformed, y_transformed, _, _ = self.preprocess_fit(X.fillna(0), y, validation_data)
         self.model_ = self.get_untrained_model()
         self.model_.fit(X_transformed, y_transformed)
         return None
 
     def predict(
         self, X: pd.DataFrame, y: pd.Series = None, return_data: bool = False, **predict_kwargs
     ) -> Union[pd.DataFrame, Tuple[pd.DataFrame, pd.DataFrame]]:
```

### Comparing `sam-3.1.8/sam/models/keras_templates.py` & `sam-3.1.9/sam/models/keras_templates.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/models/lasso_model.py` & `sam-3.1.9/sam/models/lasso_model.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/models/linear_model.py` & `sam-3.1.9/sam/models/linear_model.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/models/mlp_model.py` & `sam-3.1.9/sam/models/mlp_model.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/models/sam_shap_explainer.py` & `sam-3.1.9/sam/models/sam_shap_explainer.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/models/utils.py` & `sam-3.1.9/sam/models/utils.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/preprocessing/__init__.py` & `sam-3.1.9/sam/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/preprocessing/clip_transformer.py` & `sam-3.1.9/sam/preprocessing/clip_transformer.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/preprocessing/correct_extremes.py` & `sam-3.1.9/sam/preprocessing/correct_extremes.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/preprocessing/data_scaling.py` & `sam-3.1.9/sam/preprocessing/data_scaling.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/preprocessing/differencing.py` & `sam-3.1.9/sam/preprocessing/differencing.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/preprocessing/normalize_timestamps.py` & `sam-3.1.9/sam/preprocessing/normalize_timestamps.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/preprocessing/rnn_reshape.py` & `sam-3.1.9/sam/preprocessing/rnn_reshape.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/preprocessing/sam_reshape.py` & `sam-3.1.9/sam/preprocessing/sam_reshape.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/preprocessing/time.py` & `sam-3.1.9/sam/preprocessing/time.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/preprocessing/train_test_split.py` & `sam-3.1.9/sam/preprocessing/train_test_split.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/utils/__init__.py` & `sam-3.1.9/sam/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/utils/dataframe_functions.py` & `sam-3.1.9/sam/utils/dataframe_functions.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/utils/sklearnhelpers.py` & `sam-3.1.9/sam/utils/sklearnhelpers.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/validation/base_validator.py` & `sam-3.1.9/sam/validation/base_validator.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/validation/flatline_validator.py` & `sam-3.1.9/sam/validation/flatline_validator.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/validation/mad_validator.py` & `sam-3.1.9/sam/validation/mad_validator.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/validation/outside_range_validator.py` & `sam-3.1.9/sam/validation/outside_range_validator.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/validation/setup_validation_pipeline.py` & `sam-3.1.9/sam/validation/setup_validation_pipeline.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/visualization/__init__.py` & `sam-3.1.9/sam/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/visualization/diagnostic_flatline_removal.py` & `sam-3.1.9/sam/visualization/diagnostic_flatline_removal.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/visualization/extreme_removal_plot.py` & `sam-3.1.9/sam/visualization/extreme_removal_plot.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/visualization/incident_heatmap.py` & `sam-3.1.9/sam/visualization/incident_heatmap.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/visualization/performance_evaluation_fixed_predict_ahead.py` & `sam-3.1.9/sam/visualization/performance_evaluation_fixed_predict_ahead.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/visualization/plot_feature_importances.py` & `sam-3.1.9/sam/visualization/plot_feature_importances.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/visualization/precision_recall.py` & `sam-3.1.9/sam/visualization/precision_recall.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/visualization/quantile_plot.py` & `sam-3.1.9/sam/visualization/quantile_plot.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/visualization/rolling_correlations.py` & `sam-3.1.9/sam/visualization/rolling_correlations.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam/visualization/threshold_plot.py` & `sam-3.1.9/sam/visualization/threshold_plot.py`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam.egg-info/PKG-INFO` & `sam-3.1.9/sam.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sam
-Version: 3.1.8
+Version: 3.1.9
 Summary: Time series anomaly detection and forecasting
 Author-email: Royal HaskoningDHV <ruben.peters@rhdhv.com>
 License: MIT
 Project-URL: homepage, https://github.com/RoyalHaskoningDHV/sam
 Project-URL: issues, https://github.com/RoyalHaskoningDHV/sam/issues
 Project-URL: discussions, https://github.com/RoyalHaskoningDHV/sam/discussions
 Project-URL: documentation, https://sam-rhdhv.readthedocs.io/en/latest/
@@ -37,15 +37,15 @@
 
 SAM (Smart Asset Management) is a Python package for *timeseries analysis*, *anomaly detection* and *forecasting*.
 
 The documentation is available on [ReadTheDocs](https://sam-rhdhv.readthedocs.io/en/latest/).
 
 Author: [Royal HaskoningDHV](https://global.royalhaskoningdhv.com/)
 
-Email: [ruben.peters@rhdhv.com](mailto:ruben.peters@rhdhv.com)
+Email: [ruud.kassing@rhdhv.com](mailto:ruud.kassing@rhdhv.com)
 
 ## Getting started
 
 ### Installation
 
 The easiest way to install is package is using pip:
 ```
```

### Comparing `sam-3.1.8/sam.egg-info/SOURCES.txt` & `sam-3.1.9/sam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sam-3.1.8/sam.egg-info/requires.txt` & `sam-3.1.9/sam.egg-info/requires.txt`

 * *Files identical despite different names*

