# Comparing `tmp/pureml_evaluate-0.0.2.tar.gz` & `tmp/pureml_evaluate-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pureml_evaluate-0.0.2.tar", max compression
+gzip compressed data, was "pureml_evaluate-0.0.3.tar", max compression
```

## Comparing `pureml_evaluate-0.0.2.tar` & `pureml_evaluate-0.0.3.tar`

### file list

```diff
@@ -1,281 +1,282 @@
--rw-r--r--   0        0        0        0 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.2/README.md
--rw-r--r--   0        0        0       19 2023-07-10 21:08:37.688024 pureml_evaluate-0.0.2/pureml_evaluate/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/__init__.py
--rw-r--r--   0        0        0      510 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/data_metric_base.py
--rw-r--r--   0        0        0        0 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/__init__.py
--rw-r--r--   0        0        0       60 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/check.py
--rw-r--r--   0        0        0      717 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/class_imbalance.py
--rw-r--r--   0        0        0     1338 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/column_info.py
--rw-r--r--   0        0        0      998 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/conflicting_labels.py
--rw-r--r--   0        0        0      855 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/data_duplicates.py
--rw-r--r--   0        0        0      440 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/feature_feature_correlation.py
--rw-r--r--   0        0        0     2184 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/feature_label_correlation.py
--rw-r--r--   0        0        0     1599 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/identifier_label_correlation.py
--rw-r--r--   0        0        0      711 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/is_single_value.py
--rw-r--r--   0        0        0     1024 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/mixed_data_types.py
--rw-r--r--   0        0        0     1228 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/mixed_nulls.py
--rw-r--r--   0        0        0     1849 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/outlier_sample_detection.py
--rw-r--r--   0        0        0      677 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/percent_of_nulls.py
--rw-r--r--   0        0        0     1203 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/special_character.py
--rw-r--r--   0        0        0     1899 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/string_length_outOfBounds.py
--rw-r--r--   0        0        0     1877 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/string_mismatch.py
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.409891 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/__init__.py
--rw-r--r--   0        0        0     3122 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/config.json
--rw-r--r--   0        0        0     4756 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/evaluator.py
--rw-r--r--   0        0        0     2013 2023-07-10 21:06:51.437892 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/grade.py
--rw-r--r--   0        0        0    18803 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/graphs_generator.py
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.437892 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/model/fairness/__init__.py
--rw-r--r--   0        0        0     6119 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/model/fairness/fairness.py
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.437892 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/model/performance/__init__.py
--rw-r--r--   0        0        0     3184 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/model/performance/classification.py
--rw-r--r--   0        0        0     2412 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/model/performance/regression.py
--rw-r--r--   0        0        0     7488 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/evaluators/risk_evaluator.py
--rw-r--r--   0        0        0       89 2023-07-10 21:06:51.453892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/__init__.py
--rw-r--r--   0        0        0      361 2023-07-10 21:06:51.453892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/metric_base.py
--rw-r--r--   0        0        0        0 2023-06-04 16:57:58.850890 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/accuracy/README.md
--rw-r--r--   0        0        0      778 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/accuracy/accuracy.py
--rw-r--r--   0        0        0       14 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/accuracy/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.453892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/additive_chi2_kernel/README.md
--rw-r--r--   0        0        0      596 2023-07-10 21:06:51.453892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/additive_chi2_kernel/additive_chi2_kernel.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/additive_chi2_kernel/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/adjusted_mutual_info_score/README.md
--rw-r--r--   0        0        0      673 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/adjusted_mutual_info_score/adjusted_mutual_info_score.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/adjusted_mutual_info_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/adjusted_rand_score/README.md
--rw-r--r--   0        0        0      573 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/adjusted_rand_score/adjusted_rand_score.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/adjusted_rand_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/auc/README.md
--rw-r--r--   0        0        0      582 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/auc/auc.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/auc/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/average_precision_score/README.md
--rw-r--r--   0        0        0     1160 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/average_precision_score/average_precision_score.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/average_precision_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/balanced_accuracy_score/README.md
--rw-r--r--   0        0        0      655 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/balanced_accuracy_score/balanced_accuracy_score.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/balanced_accuracy_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/brier_score_loss/README.md
--rw-r--r--   0        0        0     1052 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/brier_score_loss/brier_score_loss.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/brier_score_loss/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/calinski_harabasz_score/README.md
--rw-r--r--   0        0        0      546 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/calinski_harabasz_score/calinski_harabasz_score.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/calinski_harabasz_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/chi2_kernel/README.md
--rw-r--r--   0        0        0      580 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/chi2_kernel/chi2_kernel.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/chi2_kernel/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/class_likelihood_ratios/README.md
--rw-r--r--   0        0        0      637 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/class_likelihood_ratios/class_likelihood_ratios.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/class_likelihood_ratios/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cohen_kappa_score/README.md
--rw-r--r--   0        0        0      644 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cohen_kappa_score/cohen_kappa_score.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cohen_kappa_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/completeness_score/README.md
--rw-r--r--   0        0        0      567 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/completeness_score/completeness_score.py
--rw-r--r--   0        0        0       15 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/completeness_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/confusion_matrix/README.md
--rw-r--r--   0        0        0      814 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/confusion_matrix/confusion_matrix.py
--rw-r--r--   0        0        0       14 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/confusion_matrix/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/contingency_matrix/README.md
--rw-r--r--   0        0        0      634 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/contingency_matrix/contingency_matrix.py
--rw-r--r--   0        0        0       19 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/contingency_matrix/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cosine_distances/README.md
--rw-r--r--   0        0        0      558 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cosine_distances/cosine_distances.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cosine_distances/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cosine_similarity/README.md
--rw-r--r--   0        0        0      630 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cosine_similarity/cosine_similarity.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cosine_similarity/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/coverage_error/README.md
--rw-r--r--   0        0        0      578 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/coverage_error/coverage_error.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/coverage_error/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_absolute_error_score/README.md
--rw-r--r--   0        0        0      686 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_absolute_error_score/d2_absolute_error_score.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_absolute_error_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_pinball_score/README.md
--rw-r--r--   0        0        0      683 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_pinball_score/d2_pinball_score.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_pinball_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_tweedie_score/README.md
--rw-r--r--   0        0        0      681 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_tweedie_score/d2_tweedie_score.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_tweedie_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/davies_bouldin_score/README.md
--rw-r--r--   0        0        0      551 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/davies_bouldin_score/davies_bouldin_score.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/davies_bouldin_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/dcg_score/README.md
--rw-r--r--   0        0        0     1053 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/dcg_score/dcg_score.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/dcg_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/det_curve/README.md
--rw-r--r--   0        0        0     1010 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/det_curve/det_curve.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/det_curve/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/euclidean_distances/README.md
--rw-r--r--   0        0        0      631 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/euclidean_distances/euclidean_distances.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/euclidean_distances/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/explained_variance_score/README.md
--rw-r--r--   0        0        0      690 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/explained_variance_score/explained_variance_score.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/explained_variance_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/f1_score/README.md
--rw-r--r--   0        0        0      985 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/f1_score/f1_score.py
--rw-r--r--   0        0        0       14 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/f1_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/fbeta_score/README.md
--rw-r--r--   0        0        0      717 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/fbeta_score/fbeta_score.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/fbeta_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/fowlkes_mallows_score/README.md
--rw-r--r--   0        0        0      582 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/fowlkes_mallows_score/fowlkes_mallows_score.py
--rw-r--r--   0        0        0       13 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/fowlkes_mallows_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/hamming_loss/README.md
--rw-r--r--   0        0        0      631 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/hamming_loss/hamming_loss.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/hamming_loss/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/haversine_distances/README.md
--rw-r--r--   0        0        0      507 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/haversine_distances/haversine_distances.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/haversine_distances/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/hinge_loss/README.md
--rw-r--r--   0        0        0     1098 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/hinge_loss/hinge_loss.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/hinge_loss/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/homogeneity_completeness_v_measure/README.md
--rw-r--r--   0        0        0      798 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/homogeneity_completeness_v_measure/homogeneity_completeness_v_measure.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/homogeneity_completeness_v_measure/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/homogeneity_score/README.md
--rw-r--r--   0        0        0      547 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/homogeneity_score/homogeneity_score.py
--rw-r--r--   0        0        0       13 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/homogeneity_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/jaccard_score/README.md
--rw-r--r--   0        0        0      715 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/jaccard_score/jaccard_score.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/jaccard_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/label_ranking_average_precision_score/README.md
--rw-r--r--   0        0        0      669 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/label_ranking_average_precision_score/label_ranking_average_precision_score.py
--rw-r--r--   0        0        0       15 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/label_ranking_average_precision_score/requirementx.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/label_ranking_loss/README.md
--rw-r--r--   0        0        0      598 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/label_ranking_loss/label_ranking_loss.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/label_ranking_loss/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/laplacian_kernel/README.md
--rw-r--r--   0        0        0      528 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/laplacian_kernel/laplacian_kernel.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/laplacian_kernel/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/linear_kernel/README.md
--rw-r--r--   0        0        0      519 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/linear_kernel/linear_kernel.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/linear_kernel/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/log_loss/README.md
--rw-r--r--   0        0        0     1395 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/log_loss/log_loss.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/log_loss/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/manhattan_distances/README.md
--rw-r--r--   0        0        0      506 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/manhattan_distances/manhattan_distances.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/manhattan_distances/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/matthews_corrcoef/README.md
--rw-r--r--   0        0        0      652 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/matthews_corrcoef/matthews_corrcoef.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/matthews_corrcoef/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/max_error/README.md
--rw-r--r--   0        0        0      552 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/max_error/max_error.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/max_error/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_absolute_error/README.md
--rw-r--r--   0        0        0      712 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_absolute_error/mean_absolute_error.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_absolute_error/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_absolute_percentage_error/README.md
--rw-r--r--   0        0        0      761 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_absolute_percentage_error/mean_absolute_percentage_error.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_absolute_percentage_error/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_gamma_deviance/README.md
--rw-r--r--   0        0        0      674 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_gamma_deviance/mean_gamma_deviance.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_gamma_deviance/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_pinball_loss/README.md
--rw-r--r--   0        0        0      680 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_pinball_loss/mean_pinball_loss.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_pinball_loss/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_poisson_deviance/README.md
--rw-r--r--   0        0        0      691 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_poisson_deviance/mean_poisson_deviance.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_poisson_deviance/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_squared_error/README.md
--rw-r--r--   0        0        0      765 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_squared_error/mean_squared_error.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_squared_error/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_squared_log_error/README.md
--rw-r--r--   0        0        0      760 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_squared_log_error/mean_squared_log_error.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_squared_log_error/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_tweedie_deviance/README.md
--rw-r--r--   0        0        0      697 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_tweedie_deviance/mean_tweedie_deviance.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_tweedie_deviance/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/median_absolute_error/README.md
--rw-r--r--   0        0        0      755 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/median_absolute_error/median_absolute_error.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/median_absolute_error/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/multilabel_confusion_matrix/README.md
--rw-r--r--   0        0        0      724 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/multilabel_confusion_matrix/multilabel_confusion_matrix.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/multilabel_confusion_matrix/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mutual_info_score/README.md
--rw-r--r--   0        0        0      676 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mutual_info_score/mutual_info_score.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mutual_info_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/nan_euclidean_distances/README.md
--rw-r--r--   0        0        0      647 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/nan_euclidean_distances/nan_euclidean_distances.py
--rw-r--r--   0        0        0       19 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/nan_euclidean_distances/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/ndcg_score/README.md
--rw-r--r--   0        0        0     1068 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/ndcg_score/ndcg_score.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/ndcg_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/normalized_mutual_info_score/README.md
--rw-r--r--   0        0        0      648 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/normalized_mutual_info_score/normalized_mutual_info_score.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/normalized_mutual_info_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pair_confusion_matrix/README.md
--rw-r--r--   0        0        0      549 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pair_confusion_matrix/pair_confusion_matrix.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pair_confusion_matrix/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_cosine_distances/README.md
--rw-r--r--   0        0        0      518 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_cosine_distances/paired_cosine_distances.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_cosine_distances/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_distances/README.md
--rw-r--r--   0        0        0      525 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_distances/paired_distances.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_distances/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_euclidean_distances/README.md
--rw-r--r--   0        0        0      525 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_euclidean_distances/paired_euclidean_distances.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_euclidean_distances/requirements.txt
--rw-r--r--   0        0        0      529 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_manhattan_distances/paired_manhattan_distances.py
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances/README.md
--rw-r--r--   0        0        0      602 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances/pairwise_distances.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_argmin/README.md
--rw-r--r--   0        0        0      608 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_argmin/pairwise_distances_argmin.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_argmin/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_argmin_min/README.md
--rw-r--r--   0        0        0      714 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_argmin_min/pairwise_distances_argmin_min.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_argmin_min/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_chunked/README.md
--rw-r--r--   0        0        0      668 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_chunked/pairwise_distances_chunked.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_chunked/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_kernels/README.md
--rw-r--r--   0        0        0      591 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_kernels/pairwise_kernels.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_kernels/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/polynomial_kernel/README.md
--rw-r--r--   0        0        0      571 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/polynomial_kernel/polynomial_kernel.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/polynomial_kernel/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/precision/README.md
--rw-r--r--   0        0        0     1095 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/precision/precision.py
--rw-r--r--   0        0        0       14 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/precision/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/precision_recall_curve/README.md
--rw-r--r--   0        0        0     1292 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/precision_recall_curve/precision_recall_curve.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/precision_recall_curve/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/r2_score/README.md
--rw-r--r--   0        0        0      687 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/r2_score/r2_score.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/r2_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/rand_score/README.md
--rw-r--r--   0        0        0      511 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/rand_score/rand_score.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/rand_score/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/rbf_kernel/README.md
--rw-r--r--   0        0        0      493 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/rbf_kernel/rbf_kernel.py
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/rbf_kernel/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/recall/README.md
--rw-r--r--   0        0        0     1062 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/recall/recall.py
--rw-r--r--   0        0        0       14 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/recall/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/roc_auc/README.md
--rw-r--r--   0        0        0       14 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/roc_auc/requirements.txt
--rw-r--r--   0        0        0     2568 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/roc_auc/roc_auc.py
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/roc_curve/README.md
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/roc_curve/requirements.txt
--rw-r--r--   0        0        0     1207 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/roc_curve/roc_curve.py
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/sigmoid_kernel/README.md
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/sigmoid_kernel/requirements.txt
--rw-r--r--   0        0        0      522 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/sigmoid_kernel/sigmoid_kernel.py
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/silhouette_samples/README.md
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/silhouette_samples/requirements.txt
--rw-r--r--   0        0        0      521 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/silhouette_samples/silhouette_samples.py
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/silhouette_score/README.md
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/silhouette_score/requirements.txt
--rw-r--r--   0        0        0      619 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/silhouette_score/silhouette_score.py
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/top_k_accuracy_score/README.md
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/top_k_accuracy_score/requirements.txt
--rw-r--r--   0        0        0     1357 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/top_k_accuracy_score/top_k_accuracy_score.py
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/v_measure_score/README.md
--rw-r--r--   0        0        0       13 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/v_measure_score/requirements.txt
--rw-r--r--   0        0        0      550 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/v_measure_score/v_measure_score.py
--rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/zero_one_loss/README.md
--rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/zero_one_loss/requirements.txt
--rw-r--r--   0        0        0      682 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/zero_one_loss/zero_one_loss.py
--rw-r--r--   0        0        0      922 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 pureml_evaluate-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.3/README.md
+-rw-r--r--   0        0        0       19 2023-07-13 09:45:51.195534 pureml_evaluate-0.0.3/pureml_evaluate/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/__init__.py
+-rw-r--r--   0        0        0      510 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/data_metric_base.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/__init__.py
+-rw-r--r--   0        0        0       60 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/check.py
+-rw-r--r--   0        0        0      717 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/class_imbalance.py
+-rw-r--r--   0        0        0     1338 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/column_info.py
+-rw-r--r--   0        0        0      998 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/conflicting_labels.py
+-rw-r--r--   0        0        0      855 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/data_duplicates.py
+-rw-r--r--   0        0        0      440 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/feature_feature_correlation.py
+-rw-r--r--   0        0        0     2184 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/feature_label_correlation.py
+-rw-r--r--   0        0        0     1599 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/identifier_label_correlation.py
+-rw-r--r--   0        0        0      711 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/is_single_value.py
+-rw-r--r--   0        0        0     1024 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/mixed_data_types.py
+-rw-r--r--   0        0        0     1228 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/mixed_nulls.py
+-rw-r--r--   0        0        0     1849 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/outlier_sample_detection.py
+-rw-r--r--   0        0        0      677 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/percent_of_nulls.py
+-rw-r--r--   0        0        0     1203 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/special_character.py
+-rw-r--r--   0        0        0     1899 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/string_length_outOfBounds.py
+-rw-r--r--   0        0        0     1877 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/string_mismatch.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.409891 pureml_evaluate-0.0.3/pureml_evaluate/evaluators/__init__.py
+-rw-r--r--   0        0        0     3122 2023-07-10 21:08:37.696024 pureml_evaluate-0.0.3/pureml_evaluate/evaluators/config.json
+-rw-r--r--   0        0        0    26692 2023-07-13 09:45:51.195534 pureml_evaluate-0.0.3/pureml_evaluate/evaluators/description.json
+-rw-r--r--   0        0        0     5036 2023-07-13 09:45:51.195534 pureml_evaluate-0.0.3/pureml_evaluate/evaluators/evaluator.py
+-rw-r--r--   0        0        0     2013 2023-07-10 21:06:51.437892 pureml_evaluate-0.0.3/pureml_evaluate/evaluators/grade.py
+-rw-r--r--   0        0        0    20267 2023-07-13 09:45:51.199534 pureml_evaluate-0.0.3/pureml_evaluate/evaluators/graphs_generator.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.437892 pureml_evaluate-0.0.3/pureml_evaluate/evaluators/model/fairness/__init__.py
+-rw-r--r--   0        0        0     6119 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/evaluators/model/fairness/fairness.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.437892 pureml_evaluate-0.0.3/pureml_evaluate/evaluators/model/performance/__init__.py
+-rw-r--r--   0        0        0     3184 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/evaluators/model/performance/classification.py
+-rw-r--r--   0        0        0     2412 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/evaluators/model/performance/regression.py
+-rw-r--r--   0        0        0     7847 2023-07-13 09:45:51.199534 pureml_evaluate-0.0.3/pureml_evaluate/evaluators/risk_evaluator.py
+-rw-r--r--   0        0        0       89 2023-07-10 21:06:51.453892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/__init__.py
+-rw-r--r--   0        0        0      361 2023-07-10 21:06:51.453892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/metric_base.py
+-rw-r--r--   0        0        0        0 2023-06-04 16:57:58.850890 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/accuracy/README.md
+-rw-r--r--   0        0        0      778 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/accuracy/accuracy.py
+-rw-r--r--   0        0        0       14 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/accuracy/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.453892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/additive_chi2_kernel/README.md
+-rw-r--r--   0        0        0      596 2023-07-10 21:06:51.453892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/additive_chi2_kernel/additive_chi2_kernel.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/additive_chi2_kernel/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/adjusted_mutual_info_score/README.md
+-rw-r--r--   0        0        0      673 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/adjusted_mutual_info_score/adjusted_mutual_info_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/adjusted_mutual_info_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/adjusted_rand_score/README.md
+-rw-r--r--   0        0        0      573 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/adjusted_rand_score/adjusted_rand_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/adjusted_rand_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/auc/README.md
+-rw-r--r--   0        0        0      582 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/auc/auc.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/auc/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/average_precision_score/README.md
+-rw-r--r--   0        0        0     1160 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/average_precision_score/average_precision_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/average_precision_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/balanced_accuracy_score/README.md
+-rw-r--r--   0        0        0      655 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/balanced_accuracy_score/balanced_accuracy_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.457892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/balanced_accuracy_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/brier_score_loss/README.md
+-rw-r--r--   0        0        0     1052 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/brier_score_loss/brier_score_loss.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/brier_score_loss/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/calinski_harabasz_score/README.md
+-rw-r--r--   0        0        0      546 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/calinski_harabasz_score/calinski_harabasz_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/calinski_harabasz_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/chi2_kernel/README.md
+-rw-r--r--   0        0        0      580 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/chi2_kernel/chi2_kernel.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/chi2_kernel/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/class_likelihood_ratios/README.md
+-rw-r--r--   0        0        0      637 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/class_likelihood_ratios/class_likelihood_ratios.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/class_likelihood_ratios/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/cohen_kappa_score/README.md
+-rw-r--r--   0        0        0      644 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/cohen_kappa_score/cohen_kappa_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/cohen_kappa_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/completeness_score/README.md
+-rw-r--r--   0        0        0      567 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/completeness_score/completeness_score.py
+-rw-r--r--   0        0        0       15 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/completeness_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/confusion_matrix/README.md
+-rw-r--r--   0        0        0      814 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/confusion_matrix/confusion_matrix.py
+-rw-r--r--   0        0        0       14 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/confusion_matrix/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/contingency_matrix/README.md
+-rw-r--r--   0        0        0      634 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/contingency_matrix/contingency_matrix.py
+-rw-r--r--   0        0        0       19 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/contingency_matrix/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/cosine_distances/README.md
+-rw-r--r--   0        0        0      558 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/cosine_distances/cosine_distances.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/cosine_distances/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/cosine_similarity/README.md
+-rw-r--r--   0        0        0      630 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/cosine_similarity/cosine_similarity.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/cosine_similarity/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/coverage_error/README.md
+-rw-r--r--   0        0        0      578 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/coverage_error/coverage_error.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/coverage_error/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/d2_absolute_error_score/README.md
+-rw-r--r--   0        0        0      686 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/d2_absolute_error_score/d2_absolute_error_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/d2_absolute_error_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/d2_pinball_score/README.md
+-rw-r--r--   0        0        0      683 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/d2_pinball_score/d2_pinball_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/d2_pinball_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/d2_tweedie_score/README.md
+-rw-r--r--   0        0        0      681 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/d2_tweedie_score/d2_tweedie_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/d2_tweedie_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/davies_bouldin_score/README.md
+-rw-r--r--   0        0        0      551 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/davies_bouldin_score/davies_bouldin_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/davies_bouldin_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/dcg_score/README.md
+-rw-r--r--   0        0        0     1053 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/dcg_score/dcg_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/dcg_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/det_curve/README.md
+-rw-r--r--   0        0        0     1010 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/det_curve/det_curve.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/det_curve/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/euclidean_distances/README.md
+-rw-r--r--   0        0        0      631 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/euclidean_distances/euclidean_distances.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/euclidean_distances/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/explained_variance_score/README.md
+-rw-r--r--   0        0        0      690 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/explained_variance_score/explained_variance_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/explained_variance_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-26 18:12:27.012737 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/f1_score/README.md
+-rw-r--r--   0        0        0      985 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/f1_score/f1_score.py
+-rw-r--r--   0        0        0       14 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/f1_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/fbeta_score/README.md
+-rw-r--r--   0        0        0      717 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/fbeta_score/fbeta_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/fbeta_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/fowlkes_mallows_score/README.md
+-rw-r--r--   0        0        0      582 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/fowlkes_mallows_score/fowlkes_mallows_score.py
+-rw-r--r--   0        0        0       13 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/fowlkes_mallows_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/hamming_loss/README.md
+-rw-r--r--   0        0        0      631 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/hamming_loss/hamming_loss.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/hamming_loss/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/haversine_distances/README.md
+-rw-r--r--   0        0        0      507 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/haversine_distances/haversine_distances.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/haversine_distances/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/hinge_loss/README.md
+-rw-r--r--   0        0        0     1098 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/hinge_loss/hinge_loss.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/hinge_loss/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/homogeneity_completeness_v_measure/README.md
+-rw-r--r--   0        0        0      798 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/homogeneity_completeness_v_measure/homogeneity_completeness_v_measure.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/homogeneity_completeness_v_measure/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/homogeneity_score/README.md
+-rw-r--r--   0        0        0      547 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/homogeneity_score/homogeneity_score.py
+-rw-r--r--   0        0        0       13 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/homogeneity_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/jaccard_score/README.md
+-rw-r--r--   0        0        0      715 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/jaccard_score/jaccard_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/jaccard_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/label_ranking_average_precision_score/README.md
+-rw-r--r--   0        0        0      669 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/label_ranking_average_precision_score/label_ranking_average_precision_score.py
+-rw-r--r--   0        0        0       15 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/label_ranking_average_precision_score/requirementx.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/label_ranking_loss/README.md
+-rw-r--r--   0        0        0      598 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/label_ranking_loss/label_ranking_loss.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/label_ranking_loss/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/laplacian_kernel/README.md
+-rw-r--r--   0        0        0      528 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/laplacian_kernel/laplacian_kernel.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/laplacian_kernel/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/linear_kernel/README.md
+-rw-r--r--   0        0        0      519 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/linear_kernel/linear_kernel.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/linear_kernel/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.461892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/log_loss/README.md
+-rw-r--r--   0        0        0     1395 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/log_loss/log_loss.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/log_loss/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/manhattan_distances/README.md
+-rw-r--r--   0        0        0      506 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/manhattan_distances/manhattan_distances.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/manhattan_distances/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/matthews_corrcoef/README.md
+-rw-r--r--   0        0        0      652 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/matthews_corrcoef/matthews_corrcoef.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/matthews_corrcoef/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/max_error/README.md
+-rw-r--r--   0        0        0      552 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/max_error/max_error.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/max_error/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_absolute_error/README.md
+-rw-r--r--   0        0        0      712 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_absolute_error/mean_absolute_error.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_absolute_error/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_absolute_percentage_error/README.md
+-rw-r--r--   0        0        0      761 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_absolute_percentage_error/mean_absolute_percentage_error.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_absolute_percentage_error/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_gamma_deviance/README.md
+-rw-r--r--   0        0        0      674 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_gamma_deviance/mean_gamma_deviance.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_gamma_deviance/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_pinball_loss/README.md
+-rw-r--r--   0        0        0      680 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_pinball_loss/mean_pinball_loss.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_pinball_loss/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_poisson_deviance/README.md
+-rw-r--r--   0        0        0      691 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_poisson_deviance/mean_poisson_deviance.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_poisson_deviance/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_squared_error/README.md
+-rw-r--r--   0        0        0      765 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_squared_error/mean_squared_error.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_squared_error/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_squared_log_error/README.md
+-rw-r--r--   0        0        0      760 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_squared_log_error/mean_squared_log_error.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_squared_log_error/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_tweedie_deviance/README.md
+-rw-r--r--   0        0        0      697 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_tweedie_deviance/mean_tweedie_deviance.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_tweedie_deviance/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/median_absolute_error/README.md
+-rw-r--r--   0        0        0      755 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/median_absolute_error/median_absolute_error.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/median_absolute_error/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/multilabel_confusion_matrix/README.md
+-rw-r--r--   0        0        0      724 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/multilabel_confusion_matrix/multilabel_confusion_matrix.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/multilabel_confusion_matrix/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mutual_info_score/README.md
+-rw-r--r--   0        0        0      676 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mutual_info_score/mutual_info_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mutual_info_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/nan_euclidean_distances/README.md
+-rw-r--r--   0        0        0      647 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/nan_euclidean_distances/nan_euclidean_distances.py
+-rw-r--r--   0        0        0       19 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/nan_euclidean_distances/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/ndcg_score/README.md
+-rw-r--r--   0        0        0     1068 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/ndcg_score/ndcg_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/ndcg_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/normalized_mutual_info_score/README.md
+-rw-r--r--   0        0        0      648 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/normalized_mutual_info_score/normalized_mutual_info_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/normalized_mutual_info_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pair_confusion_matrix/README.md
+-rw-r--r--   0        0        0      549 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pair_confusion_matrix/pair_confusion_matrix.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pair_confusion_matrix/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/paired_cosine_distances/README.md
+-rw-r--r--   0        0        0      518 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/paired_cosine_distances/paired_cosine_distances.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/paired_cosine_distances/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/paired_distances/README.md
+-rw-r--r--   0        0        0      525 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/paired_distances/paired_distances.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/paired_distances/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/paired_euclidean_distances/README.md
+-rw-r--r--   0        0        0      525 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/paired_euclidean_distances/paired_euclidean_distances.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/paired_euclidean_distances/requirements.txt
+-rw-r--r--   0        0        0      529 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/paired_manhattan_distances/paired_manhattan_distances.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pairwise_distances/README.md
+-rw-r--r--   0        0        0      602 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pairwise_distances/pairwise_distances.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pairwise_distances/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pairwise_distances_argmin/README.md
+-rw-r--r--   0        0        0      608 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pairwise_distances_argmin/pairwise_distances_argmin.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pairwise_distances_argmin/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pairwise_distances_argmin_min/README.md
+-rw-r--r--   0        0        0      714 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pairwise_distances_argmin_min/pairwise_distances_argmin_min.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pairwise_distances_argmin_min/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pairwise_distances_chunked/README.md
+-rw-r--r--   0        0        0      668 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pairwise_distances_chunked/pairwise_distances_chunked.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pairwise_distances_chunked/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pairwise_kernels/README.md
+-rw-r--r--   0        0        0      591 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pairwise_kernels/pairwise_kernels.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pairwise_kernels/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/polynomial_kernel/README.md
+-rw-r--r--   0        0        0      571 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/polynomial_kernel/polynomial_kernel.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/polynomial_kernel/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/precision/README.md
+-rw-r--r--   0        0        0     1095 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/precision/precision.py
+-rw-r--r--   0        0        0       14 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/precision/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/precision_recall_curve/README.md
+-rw-r--r--   0        0        0     1292 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/precision_recall_curve/precision_recall_curve.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/precision_recall_curve/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.465892 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/r2_score/README.md
+-rw-r--r--   0        0        0      687 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/r2_score/r2_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/r2_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/rand_score/README.md
+-rw-r--r--   0        0        0      511 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/rand_score/rand_score.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/rand_score/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/rbf_kernel/README.md
+-rw-r--r--   0        0        0      493 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/rbf_kernel/rbf_kernel.py
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/rbf_kernel/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/recall/README.md
+-rw-r--r--   0        0        0     1062 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/recall/recall.py
+-rw-r--r--   0        0        0       14 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/recall/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/roc_auc/README.md
+-rw-r--r--   0        0        0       14 2023-05-26 18:12:27.016737 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/roc_auc/requirements.txt
+-rw-r--r--   0        0        0     2568 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/roc_auc/roc_auc.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/roc_curve/README.md
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/roc_curve/requirements.txt
+-rw-r--r--   0        0        0     1207 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/roc_curve/roc_curve.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/sigmoid_kernel/README.md
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/sigmoid_kernel/requirements.txt
+-rw-r--r--   0        0        0      522 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/sigmoid_kernel/sigmoid_kernel.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/silhouette_samples/README.md
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/silhouette_samples/requirements.txt
+-rw-r--r--   0        0        0      521 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/silhouette_samples/silhouette_samples.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/silhouette_score/README.md
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/silhouette_score/requirements.txt
+-rw-r--r--   0        0        0      619 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/silhouette_score/silhouette_score.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/top_k_accuracy_score/README.md
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/top_k_accuracy_score/requirements.txt
+-rw-r--r--   0        0        0     1357 2023-07-10 21:08:37.700024 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/top_k_accuracy_score/top_k_accuracy_score.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/v_measure_score/README.md
+-rw-r--r--   0        0        0       13 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/v_measure_score/requirements.txt
+-rw-r--r--   0        0        0      550 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/v_measure_score/v_measure_score.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/zero_one_loss/README.md
+-rw-r--r--   0        0        0       14 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/zero_one_loss/requirements.txt
+-rw-r--r--   0        0        0      682 2023-07-10 21:06:51.469893 pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/zero_one_loss/zero_one_loss.py
+-rw-r--r--   0        0        0      922 2023-07-13 09:45:51.199534 pureml_evaluate-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 pureml_evaluate-0.0.3/PKG-INFO
```

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/class_imbalance.py` & `pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/class_imbalance.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/column_info.py` & `pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/column_info.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/conflicting_labels.py` & `pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/conflicting_labels.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/data_duplicates.py` & `pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/data_duplicates.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/feature_label_correlation.py` & `pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/feature_label_correlation.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/identifier_label_correlation.py` & `pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/identifier_label_correlation.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/is_single_value.py` & `pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/is_single_value.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/mixed_data_types.py` & `pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/mixed_data_types.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/mixed_nulls.py` & `pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/mixed_nulls.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/outlier_sample_detection.py` & `pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/outlier_sample_detection.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/percent_of_nulls.py` & `pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/percent_of_nulls.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/special_character.py` & `pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/special_character.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/string_length_outOfBounds.py` & `pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/string_length_outOfBounds.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/data_metrics/tabular/string_mismatch.py` & `pureml_evaluate-0.0.3/pureml_evaluate/data_metrics/tabular/string_mismatch.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/evaluators/config.json` & `pureml_evaluate-0.0.3/pureml_evaluate/evaluators/config.json`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/evaluators/evaluator.py` & `pureml_evaluate-0.0.3/pureml_evaluate/evaluators/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,29 +85,34 @@
                 values_subsets_all[key] = values_all
         return values_subsets_all
 
     def give_subsets(self):
         subsets = []
         unique_values = np.unique(self.sensitive_features)
 
+        #print(f"Unique values: {unique_values}")
         for value in unique_values:
+            #print(f"values: {value}")
             ind = np.where(self.sensitive_features == value)
 
+            #print(f"Ind: {ind}")
             sub_dict = {
                 "key": value,
                 "y_true": self.y_true[ind],
                 "y_pred": self.y_pred[ind],
                 "sensitive_features": self.sensitive_features[ind],
             }
 
+            #print(f"sub_dict: {sub_dict}")
             if self.y_pred_scores is not None:
                 sub_dict.update({"y_pred_scores": self.y_pred_scores[ind]})
             else:
                 sub_dict.update({"y_pred_scores": self.y_pred_scores})
 
+            #print("Sub dict passed")
             subsets.append(sub_dict)
 
         return subsets
 
 
 def eval(y_true, y_pred, sensitive_features, evaluators, y_pred_scores=None,threshold = 80,path_to_config=None,as_html=False,as_pdf=False,pdf_file_name='metrics_graph.pdf'):
     evaluator = Evaluator(
@@ -115,14 +120,17 @@
     )
 
     evaluator.load()
 
     values_all = evaluator.evaluate()
     values_subset_all = evaluator.evaluate_subsets()
 
+    if pdf_file_name is None:
+        pdf_file_name = 'metrics_graph.pdf'
+
     if path_to_config is None:
         path_to_config = pkg_resources.resource_filename(__name__, 'config.json')
     else:
         path_to_config = path_to_config
     riskevaluate = RiskEvaluator(values_all,values_subset_all,path_to_config=path_to_config)
     riskevaluate.compute_status()
```

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/evaluators/grade.py` & `pureml_evaluate-0.0.3/pureml_evaluate/evaluators/grade.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/evaluators/graphs_generator.py` & `pureml_evaluate-0.0.3/pureml_evaluate/evaluators/graphs_generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from sklearn import metrics
 import numpy as np
 import plotly.graph_objects as go
 import plotly.io as pio
 import numpy as np
 import plotly.express as px
 import pandas as pd
+import json
+import pkg_resources
+
 
 class CustomStyle(ParagraphStyle):
     def __init__(self, name, **kwargs):
         super().__init__(name, **kwargs)
         self.fontName = 'Arial'
         self.fontSize = 6
         self.textColor = 'blue'
@@ -31,55 +34,66 @@
             performance_metrics = values_all['performance']
             keys_in_subset_all = list(values_subset_all.keys())
 
             style_sheet = ParagraphStyle(name=CustomStyle)
             for metric_name, metric_values in performance_metrics.items():
                 fig = go.Figure()
                 if metric_name == 'confusion_matrix':
-                    generate_confusion_matrix_for_pdf(fig=fig,metric_values=metric_values,elements=elements,keys_in_subset_all=keys_in_subset_all,values_subset_all=values_subset_all,metric_name=metric_name)
+                    generate_confusion_matrix_for_pdf(fig=fig,metric_values=metric_values,
+                                                      elements=elements,keys_in_subset_all=keys_in_subset_all,
+                                                      values_subset_all=values_subset_all,metric_name=metric_name)
 
                 else:
                     data_for_description = {'Complete Data' : metric_values}
-                    generate_graphs_for_performance(fig,data_for_description,metric_values,keys_in_subset_all,values_subset_all,metric_name)
+                    generate_graphs_for_performance(fig,data_for_description,metric_values,keys_in_subset_all,
+                                                    values_subset_all,metric_name,elements=elements)
 
                     # Save the Plotly figure as an image in memory
                     image_data = fig.to_image(format='png')
 
                     # Create an Image object from the image data
                     img = Image(io.BytesIO(image_data))
 
                     # Set the image dimensions and add it to the elements list
                     img.drawHeight = 400
                     img.drawWidth = 600
                     elements.append(img)
                     
-                    description_paragraph = to_generate_description(metric_name=metric_name, data_for_description=data_for_description,style_sheet=style_sheet)
+                    description_paragraph = to_generate_description(metric_name=metric_name,
+                                                                     data_for_description=data_for_description,
+                                                                     style_sheet=style_sheet)
                 
                     elements.extend((description_paragraph, Spacer(1, 12)))
                     
+
         # Generate fairness graphs if data is available
         if 'fairness' in values_all and values_subset_all is not None:
             fairness_metrics = values_all['fairness']
             keys_in_subset_all = list(values_subset_all.keys())
             style_sheet = ParagraphStyle(name=CustomStyle)
             for metric_name, metric_values in fairness_metrics.items():
                 fig = go.Figure()
-                data_for_description = {}
-                fig,data_for_description= generate_fairness_graphs(fig=fig,metric_values=metric_values,keys_in_subset_all=keys_in_subset_all,values_subset_all=values_subset_all,metric_name=metric_name,data_for_description=data_for_description)
+                data_for_description = {'Complete Data' : metric_values}
+                generate_fairness_graphs(fig=fig,metric_values=metric_values,
+                                                                   keys_in_subset_all=keys_in_subset_all,
+                                                                   values_subset_all=values_subset_all,metric_name=metric_name,
+                                                                   data_for_description=data_for_description)
                     # Save the Plotly figure as an image in memory
                 image_data = fig.to_image(format='png')
 
                     # Create an Image object from the image data
                 img = Image(io.BytesIO(image_data))
 
                     # Set the image dimensions and add it to the elements list
                 img.drawHeight = 400
                 img.drawWidth = 600
                 elements.append(img)
-                description_paragraph = to_generate_description(metric_name=metric_name, data_for_description=data_for_description,style_sheet=style_sheet)
+                description_paragraph = to_generate_description(metric_name=metric_name,
+                                                                data_for_description=data_for_description,
+                                                                style_sheet=style_sheet)
                 
                 elements.extend((description_paragraph, Spacer(1, 12)))
                 
         # Build the PDF document with the elements
         doc.build(elements)
 
         if values_subset_all is None:
@@ -94,25 +108,31 @@
             keys_in_subset_all = list(values_subset_all.keys())
 
             # Generate performance graphs
             for metric_name, metric_values in performance_metrics.items():
                 fig = go.Figure()
 
                 if metric_name == 'confusion_matrix':
-                    generate_confusion_matrix_for_html(fig=fig,metric_values=metric_values,keys_in_subset_all=keys_in_subset_all,values_subset_all=values_subset_all,metric_name=metric_name)
+                    generate_confusion_matrix_for_html(fig=fig,metric_values=metric_values,
+                                                       keys_in_subset_all=keys_in_subset_all,
+                                                       values_subset_all=values_subset_all,metric_name=metric_name)
                 else:
-
-                    generate_graph_for_performance_for_html(fig=fig,metric_values=metric_values,keys_in_subset_all=keys_in_subset_all,values_subset_all=values_subset_all,metric_name=metric_name)
+                    generate_graph_for_performance_for_html(fig=fig,metric_values=metric_values,
+                                                            keys_in_subset_all=keys_in_subset_all,
+                                                            values_subset_all=values_subset_all,
+                                                            metric_name=metric_name)
 
         # Generate fairness graphs
         if 'fairness' in values_all and values_subset_all != None:
             fig = go.Figure()
             fairness_metrics = values_all['fairness']
             for metric_name, metric_values in fairness_metrics.items():
-                generate_graphs_for_fairness_for_html(fig=fig,metric_values=metric_values,keys_in_subset_all=keys_in_subset_all,values_subset_all=values_subset_all,metric_name=metric_name)
+                generate_graphs_for_fairness_for_html(fig=fig,metric_values=metric_values,
+                                                      keys_in_subset_all=keys_in_subset_all,
+                                                      values_subset_all=values_subset_all,metric_name=metric_name)
 
         if values_subset_all is None:
             fig = go.Figure()
             generate_only_for_values_all_for_html(values_all=values_all)
 
 
 def generate_confusion_matrix_for_pdf(fig,metric_values,elements,keys_in_subset_all,values_subset_all,metric_name):
@@ -154,43 +174,68 @@
 
 def to_generate_description(data_for_description,metric_name,style_sheet):
     description = " "
     data_str = " "
     for key, value in data_for_description.items():
         data_str += f"{key}: {value},\n "
     description += f" The values for each category are: {data_str[:-2]}\n"
-    keyname = format_keyname(metric_name=metric_name)    
-    description += f"The above graph shows realtion for the {keyname} metric."
+    
+    
     return Paragraph(description)
     
 def generate_fairness_graphs(fig,metric_values,keys_in_subset_all,values_subset_all,metric_name,data_for_description):
-        #data = pd.DataFrame(columns = ['xlabel','value','status'])
-        #color_map = {
-        #    'Pass': '#52BD94',
-        #    'Fail': '#D14343'
-        #}
-        color = '#52BD94' if metric_values['status'] == 'Pass' else '#D14343'
-
+        color =  get_color(metric_values['severity'])
         fig.add_trace(go.Bar(x=['Complete'], y=[metric_values['value']], name='All',marker = dict(color = color)))
-        #data = data.append({'xlabel':'Complete','value':metric_values['value'],'status':metric_values['status']},ignore_index=True)
-        data_for_description = {'Complete Data' : metric_values}
+        #data_for_description = {'Complete Data' : metric_values['value']}
         for subset_key in keys_in_subset_all:
                 subset_values = values_subset_all[subset_key]['fairness'][metric_name]
-                color = '#52BD94' if subset_values['status'] == 'Pass' else '#D14343'
-                data_for_description[subset_key] = subset_values
-                #data = data.append({'xlabel':subset_key,'value':subset_values['value'],'status':subset_values['status']},ignore_index=True)
-                fig.add_trace(go.Bar(x=[subset_key], y=[subset_values['value']], name=subset_key.capitalize(),marker = dict(color = color)))
-
-        #fig = px.bar(data, x="xlabel", y="value", color="status", barmode="group",color_discrete_map=color_map)
+                color = get_color(subset_values['severity'])
+                data_for_description[subset_key.capitalize()] = subset_values 
+                fig.add_trace(go.Bar(x=[subset_key], y=[subset_values['value']], marker = dict(color = color)))
         keyname = format_keyname(metric_name)
         fig.update_layout(title=f'Fairness - {keyname}', xaxis_title='Category', yaxis_title='Value',showlegend=False)
-        return fig,data_for_description
-        
+        # return fig,data_for_description
+
+def generate_graphs_for_performance(fig,data_for_description,metric_values,keys_in_subset_all,values_subset_all,metric_name,elements):
+    color = get_color(metric_values['severity'])
+    metric_values = metric_values['value']
+    fig.add_trace(go.Bar(x=['Complete Data'], y=[metric_values],marker = dict(color = color)))
+    for subset_key in keys_in_subset_all:
+        subset_values = values_subset_all[subset_key]['performance'][metric_name]
+        data_for_description[subset_key.capitalize()] = subset_values
+        # data = get_description(type_of_metric='performance',metric_name=metric_name)
+        # if data != None:
+        #     description = data['description']
+        #     whyitmatters = data['why it matters']
+        #     configuration = data['configuration']
+        #     data_for_description['description'] = description
+        #     data_for_description['why it matters'] = whyitmatters
+        #     data_for_description['configuration'] = configuration
+        color = get_color(subset_values['severity'])
+        fig.add_trace(go.Bar(x=[subset_key], y=[subset_values['value']],marker=dict(color=color)))
 
 
+    keyname = format_keyname(metric_name=metric_name)
+    fig.update_layout(title=f'Performance - {keyname}', xaxis_title='Category', yaxis_title='Value',showlegend=False)
+
+
+# def get_description(type_of_metric,metric_name):
+#     file_name  = pkg_resources.resource_filename(__name__, 'description.json')
+#     with open(f'{file_name}','r') as f:
+#         data = json.load(f)
+        
+#     if type_of_metric in data and metric_name in data[type_of_metric]:
+#         return {
+#              'description' : data[type_of_metric][metric_name]['description'],
+#              'why it matters' : data[type_of_metric][metric_name]['why it matters'],
+#              'configuration' : data[type_of_metric][metric_name]['configuration']
+#         }
+#     else:
+#         return None
+
 def generate_confusion_matrix_for_html(fig,metric_values,keys_in_subset_all,values_subset_all,metric_name):
         fig.add_trace(go.Heatmap(z=np.array(metric_values)))
 
         # Set layout properties
         fig.update_layout(
             title='Confusion Matrix',
             xaxis=dict(title='Predicted'),
@@ -211,41 +256,27 @@
     
             )
 
             # Save the figure as an HTML file       
             pio.write_html(fig, file=f'confusion_matrix_{subset_key}.html')
 
 
-def generate_graphs_for_performance(fig,data_for_description,metric_values,keys_in_subset_all,values_subset_all,metric_name):
-    color = '#52BD94' if metric_values['status'] == 'Pass' else  '#D14343'
-    metric_values = metric_values['value']
-    name = 'Pass' if color == '#52BD94' else 'Fail'
-    fig.add_trace(go.Bar(x=['Complete Data'], y=[metric_values], name=name,marker = dict(color = color)))
-    for subset_key in keys_in_subset_all:
-        subset_values = values_subset_all[subset_key]['performance'][metric_name]
-        data_for_description[subset_key.capitalize()] = subset_values
-        color = '#52BD94' if subset_values['status'] == 'Pass' else  '#D14343'
-        name = 'Pass' if color == '#52BD94' else 'Fail'
-        fig.add_trace(go.Bar(x=[subset_key], y=[subset_values['value']], name=name,marker=dict(color=color)))
-
-    keyname = format_keyname(metric_name=metric_name)
-    fig.update_layout(title=f'Performance - {keyname}', xaxis_title='Category', yaxis_title='Value',showlegend=False)
 
 
 
 def format_keyname(metric_name):
     metricname = metric_name.split('_')
     return (
         metricname[0].capitalize()
         if len(metricname) == 1
         else ' '.join(word.capitalize() for word in metricname))
     
 
 def generate_graph_for_performance_for_html(fig,metric_values,keys_in_subset_all,values_subset_all,metric_name):
-        color = '#52BD94' if metric_values['status'] == 'Pass' else  '#D14343'
+        color = get_color(metric_values['severity'])
         metric_values = metric_values['value']
         print(f"From Complete Data: {metric_values}")
         fig.add_trace(go.Bar(x=['Complete'], y=[metric_values], name='All',marker = dict(color = color)))
 
         # Add subset values
         for subset_key in keys_in_subset_all:
             subset_values = values_subset_all[subset_key]['performance'][metric_name]
@@ -283,14 +314,15 @@
             xaxis=dict(title='Category'),
             yaxis=dict(title='Value'),
             showlegend=False
         )
         # Save the figure as an HTML file
         pio.write_html(fig, file=f'fairness_{metric_name}.html')
 
+
 def generate_only_for_values_all(values_all,elements):
             style_sheet = getSampleStyleSheet()
             if 'performance' in values_all:
                 performance_metrics = values_all['performance']
                 for metric_name, metric_values in performance_metrics.items():   
                     fig = go.Figure()
                     data_for_description = {'Complete Data' : metric_values}
@@ -298,15 +330,15 @@
                         fig = go.Figure(data=go.Heatmap(
                                         z=np.array(metric_values),
                                         x=['True', 'False'],
                                         y=['Positive', 'Negative'],
                                         colorscale='Viridis'))
                         fig.update_layout(title='Confusion Matrix for Complete Data', xaxis_title='Predicted', yaxis_title='Actual',showlegend=False) 
                     else:
-                        color = '#52BD94' if metric_values['status'] == 'Pass' else  '#D14343'
+                        color = get_color(metric_values['severity'])
                         fig.add_trace(go.Bar(x=['Complete Data'], y=[metric_values['value']], name='All',marker=dict(color=color)))
                         keyname = format_keyname(metric_name)
                         fig.update_layout(title=f"{keyname}", xaxis_title='Data', yaxis_title='value',showlegend=False)
                     image_data = fig.to_image(format='png')
                     img = Image(io.BytesIO(image_data))
                     img.drawHeight = 400
                     img.drawWidth = 600
@@ -314,15 +346,15 @@
                     description_paragraph = to_generate_description(metric_name=metric_name, data_for_description=data_for_description,style_sheet=style_sheet)
                     elements.extend((description_paragraph, Spacer(1, 12)))
                 
             if 'fairness' in values_all:
                 fairness_metrics = values_all['fairness']
                 for metric_name, metric_values in fairness_metrics.items():
                     fig = go.Figure()
-                    color = '#52BD94' if metric_values['status'] == 'Pass' else '#D14343'
+                    color = get_color(metric_values['severity'])
                     metric_values = metric_values['value']
                     data_for_description = {'Complete Data' : metric_values}
                     keyname = format_keyname(metric_name)
                     fig.add_trace(go.Bar(x=['Complete Data'], y=[metric_values], name='All'))
                     fig.update_layout(title=f"{keyname}", xaxis_title='Data', yaxis_title='value',showlegend=False)
                     image_data = fig.to_image(format='png')
                     img = Image(io.BytesIO(image_data))
@@ -341,15 +373,16 @@
                 fig = go.Figure(data=go.Heatmap(
                                 z=np.array(metric_values),
                                 x=['True', 'False'],
                                 y=['Positive', 'Negative'],
                                 colorscale='Viridis'))
                 fig.update_layout(title='Confusion Matrix for Complete Data', xaxis_title='Predicted', yaxis_title='Actual',showlegend=False) 
             else:
-                color = '#52BD94' if metric_values['status'] == 'Pass' else  '#D14343'
+                #color = get_color(metric_values['severity'])
+                color = get_color(metric_values['severity'])
                 fig.add_trace(go.Bar(x=['Complete Data'], y=[metric_values['value']], name='All',marker=dict(color=color)))
                 keyname = format_keyname(metric_name)
                 fig.update_layout(title=f"{keyname}", xaxis_title='Data', yaxis_title='value',showlegend=False)
             # Save the figure as an HTML file
             pio.write_html(fig, file=f'performance_{metric_name}.html')
     
     if 'fairness' in values_all:
@@ -358,8 +391,19 @@
                 fig = go.Figure()
                 keyname = format_keyname(metric_name)
                 color = '#52BD94' if metric_values['status'] == 'Pass' else '#D14343'
                 fig.add_trace(go.Bar(x=['Complete Data'], y=[metric_values['value']], name='All',marker=dict(color=color)))
                 fig.update_layout(title=f"{keyname}", xaxis_title='Data', yaxis_title='value',showlegend=False)
                 # Save the figure as an HTML file
                 pio.write_html(fig, file=f'fairness_{metric_name}.html')
-          
+          
+
+# Function to get color
+def get_color(severity):
+    if severity == 'high':
+        return "#D14343"
+    elif severity == 'moderate':
+        return "#FFB020"
+    elif severity == 'pass':
+        return "#52BD94"
+    else:
+         return "#3366FF"
```

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/evaluators/model/fairness/fairness.py` & `pureml_evaluate-0.0.3/pureml_evaluate/evaluators/model/fairness/fairness.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/evaluators/model/performance/classification.py` & `pureml_evaluate-0.0.3/pureml_evaluate/evaluators/model/performance/classification.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/evaluators/model/performance/regression.py` & `pureml_evaluate-0.0.3/pureml_evaluate/evaluators/model/performance/regression.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/evaluators/risk_evaluator.py` & `pureml_evaluate-0.0.3/pureml_evaluate/evaluators/risk_evaluator.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,23 +31,23 @@
                     print('Set the threshold to default = 0.7')
                     threshold_precent = 0.7
                 except Exception as e:
                     print(f'Exception: {e} occured while reading config.json')
                     print('Set the threshold to default = 0.7')
                     threshold_precent = 0.7
 
-                status = get_status(original_value=data_from_values_all,threshold_precent=threshold_precent)
-                self.values_all['fairness'][metric_name]['status'] = status
+                severity = get_severity(original_value=data_from_values_all,threshold_precent=threshold_precent)
+                self.values_all['fairness'][metric_name]['severity'] = severity
 
                 for subset_key in keys_in_subset:
                     data_from_subset = self.values_subset_all[subset_key]['fairness'][metric_name]['value']
                     
 
-                    status = get_status(original_value=data_from_subset,threshold_precent=threshold_precent)
-                    self.values_subset_all[subset_key]['fairness'][metric_name]['status'] = status                    
+                    severity = get_severity(original_value=data_from_subset,threshold_precent=threshold_precent)
+                    self.values_subset_all[subset_key]['fairness'][metric_name]['severity'] = severity                    
                     # risk = risk_calculate(threshold_precent=threshold_precent,threshold=self.threshold)
                     # self.values_subset_all[subset_key]['fairness'][metric_name].append(risk)
         elif 'fairness' in self.values_all:
             fairness_keys = self.values_all['fairness']
 
             with open(f'{self.path_to_config}','r') as config_file:
                     config_file = json.load(config_file)
@@ -63,16 +63,16 @@
                     print('Set the threshold to default = 0.7')
                     threshold_precent = 0.7
                 except Exception as e:
                     print(f'Exception: {e} occured while reading config.json')
                     print('Set the threshold to default = 0.7')
                     threshold_precent = 0.7
 
-                status = get_status(original_value=data_from_values_all,threshold_precent=threshold_precent)
-                self.values_all['fairness'][metric_name]['status'] = status
+                severity = get_severity(original_value=data_from_values_all,threshold_precent=threshold_precent)
+                self.values_all['fairness'][metric_name]['severity'] = severity
 
 
         compute_performance_analysis(self.values_all,self.values_subset_all,self.path_to_config)
         
                     
 
 def risk_calculate(threshold_precent,threshold):
@@ -81,16 +81,24 @@
     elif threshold_precent <= threshold:
         return 'Moderate'
     elif threshold_precent <= threshold+0.4:
         return  'No Risk'
     else:
         return 'Low'
 
-def get_status(original_value,threshold_precent):
-    return 'pass' if original_value >= threshold_precent and original_value <= threshold_precent*1.5 else 'fail' 
+def get_severity(original_value,threshold_precent):
+    #return 'pass' if original_value >= threshold_precent and original_value <= threshold_precent*1.5 else 'fail' 
+    if original_value >= threshold_precent and original_value <= threshold_precent*1.5:
+        return "pass"
+    elif original_value <= threshold_precent/2:
+        return  "high"
+    elif threshold_precent/2 < original_value < threshold_precent:
+        return   "moderate"
+    else:
+        return  "low"
 
     #Say Threshold is 80 then 80 to 120 is pass and others as fail
     
 def compute_performance_analysis(values_all,values_subset_all,path_to_config):
         if 'performance' in values_all and values_subset_all != None:
             performance_keys = values_all['performance']
             keys_in_subset = list(values_subset_all.keys())
@@ -112,23 +120,23 @@
                     print('Set the threshold to default = 0.7')
                     threshold_precent = 0.7
                 except Exception as e:
                     print(f'Exception: {e} occured while reading config.json')
                     print('Set the threshold to default = 0.7')
                     threshold_precent = 0.7
                     
-                status = get_status(original_value=data_from_values_all,threshold_precent=threshold_precent)
-                values_all['performance'][metric_name]['status'] = status
+                severity = get_severity(original_value=data_from_values_all,threshold_precent=threshold_precent)
+                values_all['performance'][metric_name]['severity'] = severity
 
                 for subset_key in keys_in_subset:
                     data_from_subset = values_subset_all[subset_key]['performance'][metric_name]['value']
 
 
-                    status = get_status(original_value=data_from_subset,threshold_precent=threshold_precent)
-                    values_subset_all[subset_key]['performance'][metric_name]['status'] = status
+                    severity = get_severity(original_value=data_from_subset,threshold_precent=threshold_precent)
+                    values_subset_all[subset_key]['performance'][metric_name]['severity'] = severity
 
         elif 'performance' in values_all:
             performance_keys = values_all['performance']
             
             for metric_name,metric_values in performance_keys.items():
                 
                 if metric_name == 'confusion_matrix':
@@ -146,10 +154,10 @@
                     print('Set the threshold to default = 0.7')
                     threshold_precent = 0.7
                 except Exception as e:
                     print(f'Exception: {e} occured while reading config.json')
                     print('Set the threshold to default = 0.7')
                     threshold_precent = 0.7
                     
-                status = get_status(original_value=data_from_values_all,threshold_precent=threshold_precent)
-                values_all['performance'][metric_name]['status'] = status
+                severity = get_severity(original_value=data_from_values_all,threshold_precent=threshold_precent)
+                values_all['performance'][metric_name]['severity'] = severity
```

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/accuracy/accuracy.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/accuracy/accuracy.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/additive_chi2_kernel/additive_chi2_kernel.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/additive_chi2_kernel/additive_chi2_kernel.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/adjusted_mutual_info_score/adjusted_mutual_info_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/adjusted_mutual_info_score/adjusted_mutual_info_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/adjusted_rand_score/adjusted_rand_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/adjusted_rand_score/adjusted_rand_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/auc/auc.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/auc/auc.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/average_precision_score/average_precision_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/average_precision_score/average_precision_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/balanced_accuracy_score/balanced_accuracy_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/balanced_accuracy_score/balanced_accuracy_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/brier_score_loss/brier_score_loss.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/brier_score_loss/brier_score_loss.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/calinski_harabasz_score/calinski_harabasz_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/calinski_harabasz_score/calinski_harabasz_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/chi2_kernel/chi2_kernel.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/chi2_kernel/chi2_kernel.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/class_likelihood_ratios/class_likelihood_ratios.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/class_likelihood_ratios/class_likelihood_ratios.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cohen_kappa_score/cohen_kappa_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/cohen_kappa_score/cohen_kappa_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/completeness_score/completeness_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/completeness_score/completeness_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/confusion_matrix/confusion_matrix.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/confusion_matrix/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/contingency_matrix/contingency_matrix.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/contingency_matrix/contingency_matrix.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cosine_distances/cosine_distances.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/cosine_distances/cosine_distances.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/cosine_similarity/cosine_similarity.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/cosine_similarity/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/coverage_error/coverage_error.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/coverage_error/coverage_error.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_absolute_error_score/d2_absolute_error_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/d2_absolute_error_score/d2_absolute_error_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_pinball_score/d2_pinball_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/d2_pinball_score/d2_pinball_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/d2_tweedie_score/d2_tweedie_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/d2_tweedie_score/d2_tweedie_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/davies_bouldin_score/davies_bouldin_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/davies_bouldin_score/davies_bouldin_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/dcg_score/dcg_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/dcg_score/dcg_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/det_curve/det_curve.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/det_curve/det_curve.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/euclidean_distances/euclidean_distances.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/euclidean_distances/euclidean_distances.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/explained_variance_score/explained_variance_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/explained_variance_score/explained_variance_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/f1_score/f1_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/f1_score/f1_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/fbeta_score/fbeta_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/fbeta_score/fbeta_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/fowlkes_mallows_score/fowlkes_mallows_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/fowlkes_mallows_score/fowlkes_mallows_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/hamming_loss/hamming_loss.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/hamming_loss/hamming_loss.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/hinge_loss/hinge_loss.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/hinge_loss/hinge_loss.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/homogeneity_completeness_v_measure/homogeneity_completeness_v_measure.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/homogeneity_completeness_v_measure/homogeneity_completeness_v_measure.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/homogeneity_score/homogeneity_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/homogeneity_score/homogeneity_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/jaccard_score/jaccard_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/jaccard_score/jaccard_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/label_ranking_average_precision_score/label_ranking_average_precision_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/label_ranking_average_precision_score/label_ranking_average_precision_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/label_ranking_loss/label_ranking_loss.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/label_ranking_loss/label_ranking_loss.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/laplacian_kernel/laplacian_kernel.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/laplacian_kernel/laplacian_kernel.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/linear_kernel/linear_kernel.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/linear_kernel/linear_kernel.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/log_loss/log_loss.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/log_loss/log_loss.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/matthews_corrcoef/matthews_corrcoef.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/matthews_corrcoef/matthews_corrcoef.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/max_error/max_error.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/max_error/max_error.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_absolute_error/mean_absolute_error.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_absolute_error/mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_absolute_percentage_error/mean_absolute_percentage_error.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_absolute_percentage_error/mean_absolute_percentage_error.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_gamma_deviance/mean_gamma_deviance.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_gamma_deviance/mean_gamma_deviance.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_pinball_loss/mean_pinball_loss.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_pinball_loss/mean_pinball_loss.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_poisson_deviance/mean_poisson_deviance.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_poisson_deviance/mean_poisson_deviance.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_squared_error/mean_squared_error.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_squared_error/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_squared_log_error/mean_squared_log_error.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_squared_log_error/mean_squared_log_error.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mean_tweedie_deviance/mean_tweedie_deviance.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mean_tweedie_deviance/mean_tweedie_deviance.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/median_absolute_error/median_absolute_error.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/median_absolute_error/median_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/multilabel_confusion_matrix/multilabel_confusion_matrix.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/multilabel_confusion_matrix/multilabel_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/mutual_info_score/mutual_info_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/mutual_info_score/mutual_info_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/nan_euclidean_distances/nan_euclidean_distances.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/nan_euclidean_distances/nan_euclidean_distances.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/ndcg_score/ndcg_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/ndcg_score/ndcg_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/normalized_mutual_info_score/normalized_mutual_info_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/normalized_mutual_info_score/normalized_mutual_info_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pair_confusion_matrix/pair_confusion_matrix.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pair_confusion_matrix/pair_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_cosine_distances/paired_cosine_distances.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/paired_cosine_distances/paired_cosine_distances.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_distances/paired_distances.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/paired_distances/paired_distances.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_euclidean_distances/paired_euclidean_distances.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/paired_euclidean_distances/paired_euclidean_distances.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/paired_manhattan_distances/paired_manhattan_distances.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/paired_manhattan_distances/paired_manhattan_distances.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances/pairwise_distances.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pairwise_distances/pairwise_distances.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_argmin/pairwise_distances_argmin.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pairwise_distances_argmin/pairwise_distances_argmin.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_argmin_min/pairwise_distances_argmin_min.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pairwise_distances_argmin_min/pairwise_distances_argmin_min.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_distances_chunked/pairwise_distances_chunked.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pairwise_distances_chunked/pairwise_distances_chunked.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/pairwise_kernels/pairwise_kernels.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/pairwise_kernels/pairwise_kernels.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/polynomial_kernel/polynomial_kernel.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/polynomial_kernel/polynomial_kernel.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/precision/precision.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/precision/precision.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/precision_recall_curve/precision_recall_curve.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/precision_recall_curve/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/r2_score/r2_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/r2_score/r2_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/recall/recall.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/recall/recall.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/roc_auc/roc_auc.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/roc_auc/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/roc_curve/roc_curve.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/roc_curve/roc_curve.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/sigmoid_kernel/sigmoid_kernel.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/sigmoid_kernel/sigmoid_kernel.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/silhouette_samples/silhouette_samples.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/silhouette_samples/silhouette_samples.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/silhouette_score/silhouette_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/silhouette_score/silhouette_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/top_k_accuracy_score/top_k_accuracy_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/top_k_accuracy_score/top_k_accuracy_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/v_measure_score/v_measure_score.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/v_measure_score/v_measure_score.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pureml_evaluate/metrics/model/zero_one_loss/zero_one_loss.py` & `pureml_evaluate-0.0.3/pureml_evaluate/metrics/model/zero_one_loss/zero_one_loss.py`

 * *Files identical despite different names*

### Comparing `pureml_evaluate-0.0.2/pyproject.toml` & `pureml_evaluate-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pureml-evaluate"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["vamsidhar muthireddy <vamsi.muthireddy@gmail.com>"]
 readme = "README.md"
 
 packages = [{include = "pureml_evaluate"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pureml_evaluate-0.0.2/PKG-INFO` & `pureml_evaluate-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pureml-evaluate
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: vamsidhar muthireddy
 Author-email: vamsi.muthireddy@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

