# Comparing `tmp/tmlt_analytics-0.7.2.tar.gz` & `tmp/tmlt_analytics-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmlt_analytics-0.7.2.tar", max compression
+gzip compressed data, was "tmlt_analytics-0.7.3.tar", max compression
```

## Comparing `tmlt_analytics-0.7.2.tar` & `tmlt_analytics-0.7.3.tar`

### file list

```diff
@@ -1,170 +1,170 @@
--rw-r--r--   0        0        0    18237 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/CHANGELOG.rst
--rw-r--r--   0        0        0    11358 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/LICENSE
--rw-r--r--   0        0        0    20138 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/LICENSE.docs
--rw-r--r--   0        0        0      121 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/NOTICE
--rw-r--r--   0        0        0     2593 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/README.md
--rw-r--r--   0        0        0      951 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/_static/css/custom.css
--rw-r--r--   0        0        0    12470 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/_static/favicon.ico
--rw-r--r--   0        0        0     1001 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/_static/js/version-banner.js
--rw-r--r--   0        0        0    30903 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/_static/logo.png
--rw-r--r--   0        0        0       50 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/_templates/build-info.html
--rw-r--r--   0        0        0      408 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/_templates/layout.html
--rw-r--r--   0        0        0       23 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/_templates/package-name.html
--rw-r--r--   0        0        0     6786 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/conf.py
--rw-r--r--   0        0        0     1599 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/bigquery/bigquery-setup.rst
--rw-r--r--   0        0        0     3005 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/bigquery/docker-image.rst
--rw-r--r--   0        0        0     1225 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/bigquery/index.rst
--rw-r--r--   0        0        0     6280 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/bigquery/inputs-outputs.rst
--rw-r--r--   0        0        0     5760 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/bigquery/parameters.rst
--rw-r--r--   0        0        0     4733 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/bigquery/running-the-program.rst
--rw-r--r--   0        0        0     1706 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/bigquery/setup.rst
--rw-r--r--   0        0        0     6911 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/databricks.rst
--rw-r--r--   0        0        0      328 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/index.rst
--rw-r--r--   0        0        0     4783 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/installation.rst
--rw-r--r--   0        0        0     2735 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/howto-guides/troubleshooting.rst
--rw-r--r--   0        0        0   118378 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/images/api_diagram.svg
--rw-r--r--   0        0        0    85925 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/images/chart_age_at_joining.png
--rw-r--r--   0        0        0    27267 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/images/chart_attacker_certainty.png
--rw-r--r--   0        0        0    41645 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/images/chart_average_age_by_edu.png
--rw-r--r--   0        0        0    34101 2023-06-15 12:45:45.149361 tmlt_analytics-0.7.2/doc/images/chart_books_by_unique_members.png
--rw-r--r--   0        0        0   104926 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_counts_age_gender.png
--rw-r--r--   0        0        0    34006 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_counts_different_eps.png
--rw-r--r--   0        0        0    25097 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_counts_edu+sex.png
--rw-r--r--   0        0        0    13993 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_counts_education.png
--rw-r--r--   0        0        0    41034 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_error_vs_partition_age_edu.png
--rw-r--r--   0        0        0    59042 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_favorite_genres.png
--rw-r--r--   0        0        0    14310 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_filters_education.png
--rw-r--r--   0        0        0    30330 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_genres_by_age.png
--rw-r--r--   0        0        0    14782 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_quantiles_education.png
--rw-r--r--   0        0        0    20853 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_senior_counts_1.png
--rw-r--r--   0        0        0    21067 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_senior_counts_2.png
--rw-r--r--   0        0        0    29335 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_teen_edu_counts.png
--rw-r--r--   0        0        0    20226 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/chart_younger_age_counts.png
--rw-r--r--   0        0        0    29155 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/clamping_bounds_averages.png
--rw-r--r--   0        0        0     9416 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/clamping_bounds_schema.png
--rw-r--r--   0        0        0    18639 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/flat_map_row_example.svg
--rw-r--r--   0        0        0    23590 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/flow_chart_truncation.svg
--rw-r--r--   0        0        0    14685 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/histogram_books_borrowed.png
--rw-r--r--   0        0        0     1844 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/index_api.svg
--rw-r--r--   0        0        0      609 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/index_howto_guides.svg
--rw-r--r--   0        0        0     1196 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/index_more.svg
--rw-r--r--   0        0        0      604 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/index_topic_guides.svg
--rw-r--r--   0        0        0     1371 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/index_tutorials.svg
--rw-r--r--   0        0        0    23369 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/intuitive_noise_visualization.png
--rw-r--r--   0        0        0    30903 2023-06-15 12:45:45.153361 tmlt_analytics-0.7.2/doc/images/logo.png
--rw-r--r--   0        0        0    85314 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/images/mock_checkout_logs.svg
--rw-r--r--   0        0        0    59239 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/images/private_join_example.svg
--rw-r--r--   0        0        0    35838 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/images/private_join_tables.svg
--rw-r--r--   0        0        0    32227 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/images/public_join_example_zips.svg
--rw-r--r--   0        0        0     5602 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/index.rst
--rw-r--r--   0        0        0      662 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/intersphinx_mapping.json
--rw-r--r--   0        0        0     3169 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/privacy-policy.rst
--rw-r--r--   0        0        0     2024 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/templates/python/class.rst
--rw-r--r--   0        0        0     3440 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/templates/python/module.rst
--rw-r--r--   0        0        0      396 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/topic-guides/index.rst
--rw-r--r--   0        0        0    11697 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/topic-guides/nulls-nans-infinities.rst
--rw-r--r--   0        0        0     8608 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/topic-guides/privacy-budgets.rst
--rw-r--r--   0        0        0     6595 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/topic-guides/privacy-promise.rst
--rw-r--r--   0        0        0     7726 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/topic-guides/spark.rst
--rw-r--r--   0        0        0    12513 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/topic-guides/understanding-sensitivity.rst
--rw-r--r--   0        0        0     8462 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/topic-guides/working-with-sessions.rst
--rw-r--r--   0        0        0     9124 2023-06-15 12:45:45.157361 tmlt_analytics-0.7.2/doc/tutorials/clamping-bounds.rst
--rw-r--r--   0        0        0     7246 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/doc/tutorials/first-steps.rst
--rw-r--r--   0        0        0    18802 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/doc/tutorials/groupby-queries.rst
--rw-r--r--   0        0        0      430 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/doc/tutorials/index.rst
--rw-r--r--   0        0        0    12394 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/doc/tutorials/more-with-privacy-ids.rst
--rw-r--r--   0        0        0     8452 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/doc/tutorials/privacy-budget-basics.rst
--rw-r--r--   0        0        0    15179 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/doc/tutorials/privacy-id-basics.rst
--rw-r--r--   0        0        0    16252 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/doc/tutorials/simple-transformations.rst
--rw-r--r--   0        0        0     4789 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/examples/interactive_evaluation.ipynb
--rw-r--r--   0        0        0     5459 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/examples/private_join.ipynb
--rw-r--r--   0        0        0     6570 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/examples/zcdp_puredp_switching.ipynb
--rw-r--r--   0        0        0     4646 2023-06-15 12:46:22.353936 tmlt_analytics-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      108 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/__init__.py
--rw-r--r--   0        0        0     6965 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/conftest.py
--rw-r--r--   0        0        0      115 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/__init__.py
--rw-r--r--   0        0        0      108 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/__init__.py
--rw-r--r--   0        0        0     5642 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/conftest.py
--rw-r--r--   0        0        0      151 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/ids/__init__.py
--rw-r--r--   0        0        0    15227 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/ids/test_constraint_propagation.py
--rw-r--r--   0        0        0     6531 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/ids/test_count_distinct_optimization.py
--rw-r--r--   0        0        0     9106 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/ids/test_id_col_operations.py
--rw-r--r--   0        0        0    22181 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/ids/test_l0_linf_truncation.py
--rw-r--r--   0        0        0    14256 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/ids/test_l1_truncation.py
--rw-r--r--   0        0        0     3965 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/ids/test_partition.py
--rw-r--r--   0        0        0      143 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/mixed/__init__.py
--rw-r--r--   0        0        0     5087 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/mixed/test_mixed_session.py
--rw-r--r--   0        0        0      152 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/rows/__init__.py
--rw-r--r--   0        0        0    26463 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/rows/conftest.py
--rw-r--r--   0        0        0    42789 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/rows/test_add_max_rows.py
--rw-r--r--   0        0        0     6122 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/rows/test_add_max_rows_in_max_groups.py
--rw-r--r--   0        0        0    13702 2023-06-15 12:45:45.161361 tmlt_analytics-0.7.2/test/system/session/rows/test_add_max_rows_infs_nulls.py
--rw-r--r--   0        0        0    11017 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/system/session/rows/test_invalid.py
--rw-r--r--   0        0        0     4465 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/system/session/test_budgets.py
--rw-r--r--   0        0        0     2212 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/system/session/test_invalid_constraints.py
--rw-r--r--   0        0        0      108 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/__init__.py
--rw-r--r--   0        0        0      298 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/query_expr_compiler/__init__.py
--rw-r--r--   0        0        0    76707 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/query_expr_compiler/test_measurement_visitor.py
--rw-r--r--   0        0        0    54860 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/query_expr_compiler/test_output_schema_visitor.py
--rw-r--r--   0        0        0      107 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/query_expr_compiler/transformation_visitor/__init__.py
--rw-r--r--   0        0        0    17843 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/query_expr_compiler/transformation_visitor/conftest.py
--rw-r--r--   0        0        0    24152 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py
--rw-r--r--   0        0        0    36839 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py
--rw-r--r--   0        0        0     7610 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py
--rw-r--r--   0        0        0    15631 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_binning_spec.py
--rw-r--r--   0        0        0     2301 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_catalog.py
--rw-r--r--   0        0        0      657 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_cleanup.py
--rw-r--r--   0        0        0     5285 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_constraints.py
--rw-r--r--   0        0        0    21123 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_keyset.py
--rw-r--r--   0        0        0    14053 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_neighboring_relations.py
--rw-r--r--   0        0        0     3401 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_noise_info.py
--rw-r--r--   0        0        0     5865 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_privacy_budget.py
--rw-r--r--   0        0        0     5480 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_privacy_budget_rounding_helper.py
--rw-r--r--   0        0        0     3011 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_protected_change.py
--rw-r--r--   0        0        0    40576 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_query_builder.py
--rw-r--r--   0        0        0    63726 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_query_expr_compiler.py
--rw-r--r--   0        0        0    16787 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_query_expression.py
--rw-r--r--   0        0        0     4874 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_query_expression_visitor.py
--rw-r--r--   0        0        0     2172 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_schema.py
--rw-r--r--   0        0        0    13538 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_schema_conversion.py
--rw-r--r--   0        0        0    87562 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_session.py
--rw-r--r--   0        0        0     1604 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_table_identifiers.py
--rw-r--r--   0        0        0     5372 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_transformation_utils.py
--rw-r--r--   0        0        0      747 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_truncation_strategy.py
--rw-r--r--   0        0        0      518 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test/unit/test_utils.py
--rw-r--r--   0        0        0       37 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/test_requirements.txt
--rw-r--r--   0        0        0      222 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/tmlt/analytics/__init__.py
--rw-r--r--   0        0        0     3666 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/tmlt/analytics/_catalog.py
--rw-r--r--   0        0        0     3555 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/tmlt/analytics/_coerce_spark_schema.py
--rw-r--r--   0        0        0    16162 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/tmlt/analytics/_neighboring_relation.py
--rw-r--r--   0        0        0     7164 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/tmlt/analytics/_neighboring_relation_visitor.py
--rw-r--r--   0        0        0     5683 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/tmlt/analytics/_noise_info.py
--rw-r--r--   0        0        0     4021 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/tmlt/analytics/_privacy_budget_rounding_helper.py
--rw-r--r--   0        0        0      184 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/__init__.py
--rw-r--r--   0        0        0    10044 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/_compiler.py
--rw-r--r--   0        0        0     7694 2023-06-15 12:45:45.165361 tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py
--rw-r--r--   0        0        0    42627 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py
--rw-r--r--   0        0        0    46889 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py
--rw-r--r--   0        0        0    60357 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py
--rw-r--r--   0        0        0    12795 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/_schema.py
--rw-r--r--   0        0        0     1250 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/_table_identifier.py
--rw-r--r--   0        0        0     3980 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/_table_reference.py
--rw-r--r--   0        0        0    10148 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/_transformation_utils.py
--rw-r--r--   0        0        0      420 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/_type_checking.py
--rw-r--r--   0        0        0    11871 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/binning_spec.py
--rw-r--r--   0        0        0      306 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/cleanup.py
--rw-r--r--   0        0        0      458 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/constraints/__init__.py
--rw-r--r--   0        0        0     1101 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/constraints/_base.py
--rw-r--r--   0        0        0      735 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/constraints/_simplify.py
--rw-r--r--   0        0        0    12758 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/constraints/_truncation.py
--rw-r--r--   0        0        0    11850 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/keyset.py
--rw-r--r--   0        0        0    10546 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/privacy_budget.py
--rw-r--r--   0        0        0     5482 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/protected_change.py
--rw-r--r--   0        0        0        0 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/py.typed
--rw-r--r--   0        0        0   129668 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/query_builder.py
--rw-r--r--   0        0        0    41076 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/query_expr.py
--rw-r--r--   0        0        0    80902 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/session.py
--rw-r--r--   0        0        0     3965 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/truncation_strategy.py
--rw-r--r--   0        0        0     5397 2023-06-15 12:45:45.169361 tmlt_analytics-0.7.2/tmlt/analytics/utils.py
--rw-r--r--   0        0        0     3529 1970-01-01 00:00:00.000000 tmlt_analytics-0.7.2/setup.py
--rw-r--r--   0        0        0     3908 1970-01-01 00:00:00.000000 tmlt_analytics-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    18334 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/CHANGELOG.rst
+-rw-r--r--   0        0        0    11358 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/LICENSE
+-rw-r--r--   0        0        0    20138 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/LICENSE.docs
+-rw-r--r--   0        0        0      121 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/NOTICE
+-rw-r--r--   0        0        0     2593 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/README.md
+-rw-r--r--   0        0        0      951 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/_static/css/custom.css
+-rw-r--r--   0        0        0    12470 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/_static/favicon.ico
+-rw-r--r--   0        0        0     1001 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/_static/js/version-banner.js
+-rw-r--r--   0        0        0    30903 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/_static/logo.png
+-rw-r--r--   0        0        0       50 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/_templates/build-info.html
+-rw-r--r--   0        0        0      408 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/_templates/layout.html
+-rw-r--r--   0        0        0       23 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/_templates/package-name.html
+-rw-r--r--   0        0        0     6786 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/conf.py
+-rw-r--r--   0        0        0     1599 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/howto-guides/bigquery/bigquery-setup.rst
+-rw-r--r--   0        0        0     3005 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/howto-guides/bigquery/docker-image.rst
+-rw-r--r--   0        0        0     1225 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/howto-guides/bigquery/index.rst
+-rw-r--r--   0        0        0     6280 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/howto-guides/bigquery/inputs-outputs.rst
+-rw-r--r--   0        0        0     5761 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/howto-guides/bigquery/parameters.rst
+-rw-r--r--   0        0        0     4733 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/howto-guides/bigquery/running-the-program.rst
+-rw-r--r--   0        0        0     1706 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/howto-guides/bigquery/setup.rst
+-rw-r--r--   0        0        0     6911 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/howto-guides/databricks.rst
+-rw-r--r--   0        0        0      328 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/howto-guides/index.rst
+-rw-r--r--   0        0        0     4783 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/howto-guides/installation.rst
+-rw-r--r--   0        0        0     2735 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/howto-guides/troubleshooting.rst
+-rw-r--r--   0        0        0   118378 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/images/api_diagram.svg
+-rw-r--r--   0        0        0    85925 2023-07-13 18:20:34.738807 tmlt_analytics-0.7.3/doc/images/chart_age_at_joining.png
+-rw-r--r--   0        0        0    27267 2023-07-13 18:20:34.742807 tmlt_analytics-0.7.3/doc/images/chart_attacker_certainty.png
+-rw-r--r--   0        0        0    41645 2023-07-13 18:20:34.742807 tmlt_analytics-0.7.3/doc/images/chart_average_age_by_edu.png
+-rw-r--r--   0        0        0    34101 2023-07-13 18:20:34.742807 tmlt_analytics-0.7.3/doc/images/chart_books_by_unique_members.png
+-rw-r--r--   0        0        0   104926 2023-07-13 18:20:34.742807 tmlt_analytics-0.7.3/doc/images/chart_counts_age_gender.png
+-rw-r--r--   0        0        0    34006 2023-07-13 18:20:34.742807 tmlt_analytics-0.7.3/doc/images/chart_counts_different_eps.png
+-rw-r--r--   0        0        0    25097 2023-07-13 18:20:34.742807 tmlt_analytics-0.7.3/doc/images/chart_counts_edu+sex.png
+-rw-r--r--   0        0        0    13993 2023-07-13 18:20:34.742807 tmlt_analytics-0.7.3/doc/images/chart_counts_education.png
+-rw-r--r--   0        0        0    41034 2023-07-13 18:20:34.742807 tmlt_analytics-0.7.3/doc/images/chart_error_vs_partition_age_edu.png
+-rw-r--r--   0        0        0    59042 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/chart_favorite_genres.png
+-rw-r--r--   0        0        0    14310 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/chart_filters_education.png
+-rw-r--r--   0        0        0    30330 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/chart_genres_by_age.png
+-rw-r--r--   0        0        0    14782 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/chart_quantiles_education.png
+-rw-r--r--   0        0        0    20853 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/chart_senior_counts_1.png
+-rw-r--r--   0        0        0    21067 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/chart_senior_counts_2.png
+-rw-r--r--   0        0        0    29335 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/chart_teen_edu_counts.png
+-rw-r--r--   0        0        0    20226 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/chart_younger_age_counts.png
+-rw-r--r--   0        0        0    29155 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/clamping_bounds_averages.png
+-rw-r--r--   0        0        0     9416 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/clamping_bounds_schema.png
+-rw-r--r--   0        0        0    18639 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/flat_map_row_example.svg
+-rw-r--r--   0        0        0    23590 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/flow_chart_truncation.svg
+-rw-r--r--   0        0        0    14685 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/histogram_books_borrowed.png
+-rw-r--r--   0        0        0     1844 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/index_api.svg
+-rw-r--r--   0        0        0      609 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/index_howto_guides.svg
+-rw-r--r--   0        0        0     1196 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/index_more.svg
+-rw-r--r--   0        0        0      604 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/index_topic_guides.svg
+-rw-r--r--   0        0        0     1371 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/index_tutorials.svg
+-rw-r--r--   0        0        0    23369 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/intuitive_noise_visualization.png
+-rw-r--r--   0        0        0    30903 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/logo.png
+-rw-r--r--   0        0        0    85314 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/mock_checkout_logs.svg
+-rw-r--r--   0        0        0    59239 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/private_join_example.svg
+-rw-r--r--   0        0        0    35838 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/private_join_tables.svg
+-rw-r--r--   0        0        0    32227 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/images/public_join_example_zips.svg
+-rw-r--r--   0        0        0     5510 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/index.rst
+-rw-r--r--   0        0        0      662 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/intersphinx_mapping.json
+-rw-r--r--   0        0        0     3169 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/privacy-policy.rst
+-rw-r--r--   0        0        0     2024 2023-07-13 18:20:34.750807 tmlt_analytics-0.7.3/doc/templates/python/class.rst
+-rw-r--r--   0        0        0     3440 2023-07-13 18:20:34.754807 tmlt_analytics-0.7.3/doc/templates/python/module.rst
+-rw-r--r--   0        0        0      396 2023-07-13 18:20:34.754807 tmlt_analytics-0.7.3/doc/topic-guides/index.rst
+-rw-r--r--   0        0        0    11697 2023-07-13 18:20:34.754807 tmlt_analytics-0.7.3/doc/topic-guides/nulls-nans-infinities.rst
+-rw-r--r--   0        0        0     8608 2023-07-13 18:20:34.754807 tmlt_analytics-0.7.3/doc/topic-guides/privacy-budgets.rst
+-rw-r--r--   0        0        0     6595 2023-07-13 18:20:34.754807 tmlt_analytics-0.7.3/doc/topic-guides/privacy-promise.rst
+-rw-r--r--   0        0        0     7726 2023-07-13 18:20:34.754807 tmlt_analytics-0.7.3/doc/topic-guides/spark.rst
+-rw-r--r--   0        0        0    12513 2023-07-13 18:20:34.754807 tmlt_analytics-0.7.3/doc/topic-guides/understanding-sensitivity.rst
+-rw-r--r--   0        0        0     8462 2023-07-13 18:20:34.754807 tmlt_analytics-0.7.3/doc/topic-guides/working-with-sessions.rst
+-rw-r--r--   0        0        0     9124 2023-07-13 18:20:34.754807 tmlt_analytics-0.7.3/doc/tutorials/clamping-bounds.rst
+-rw-r--r--   0        0        0     7246 2023-07-13 18:20:34.754807 tmlt_analytics-0.7.3/doc/tutorials/first-steps.rst
+-rw-r--r--   0        0        0    18802 2023-07-13 18:20:34.754807 tmlt_analytics-0.7.3/doc/tutorials/groupby-queries.rst
+-rw-r--r--   0        0        0      430 2023-07-13 18:20:34.754807 tmlt_analytics-0.7.3/doc/tutorials/index.rst
+-rw-r--r--   0        0        0    12394 2023-07-13 18:20:34.754807 tmlt_analytics-0.7.3/doc/tutorials/more-with-privacy-ids.rst
+-rw-r--r--   0        0        0     8452 2023-07-13 18:20:34.754807 tmlt_analytics-0.7.3/doc/tutorials/privacy-budget-basics.rst
+-rw-r--r--   0        0        0    15179 2023-07-13 18:20:34.754807 tmlt_analytics-0.7.3/doc/tutorials/privacy-id-basics.rst
+-rw-r--r--   0        0        0    16252 2023-07-13 18:20:34.754807 tmlt_analytics-0.7.3/doc/tutorials/simple-transformations.rst
+-rw-r--r--   0        0        0     4789 2023-07-13 18:20:34.754807 tmlt_analytics-0.7.3/examples/interactive_evaluation.ipynb
+-rw-r--r--   0        0        0     5459 2023-07-13 18:20:34.754807 tmlt_analytics-0.7.3/examples/private_join.ipynb
+-rw-r--r--   0        0        0     6570 2023-07-13 18:20:34.754807 tmlt_analytics-0.7.3/examples/zcdp_puredp_switching.ipynb
+-rw-r--r--   0        0        0     4689 2023-07-13 18:21:16.786646 tmlt_analytics-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/__init__.py
+-rw-r--r--   0        0        0     7451 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/conftest.py
+-rw-r--r--   0        0        0      115 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/system/__init__.py
+-rw-r--r--   0        0        0      108 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/system/session/__init__.py
+-rw-r--r--   0        0        0     5642 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/system/session/conftest.py
+-rw-r--r--   0        0        0      151 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/system/session/ids/__init__.py
+-rw-r--r--   0        0        0    15227 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/system/session/ids/test_constraint_propagation.py
+-rw-r--r--   0        0        0     6531 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/system/session/ids/test_count_distinct_optimization.py
+-rw-r--r--   0        0        0     9106 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/system/session/ids/test_id_col_operations.py
+-rw-r--r--   0        0        0    22181 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/system/session/ids/test_l0_linf_truncation.py
+-rw-r--r--   0        0        0    14256 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/system/session/ids/test_l1_truncation.py
+-rw-r--r--   0        0        0     3965 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/system/session/ids/test_partition.py
+-rw-r--r--   0        0        0      143 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/system/session/mixed/__init__.py
+-rw-r--r--   0        0        0     5087 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/system/session/mixed/test_mixed_session.py
+-rw-r--r--   0        0        0      152 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/system/session/rows/__init__.py
+-rw-r--r--   0        0        0    26463 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/system/session/rows/conftest.py
+-rw-r--r--   0        0        0    42789 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/system/session/rows/test_add_max_rows.py
+-rw-r--r--   0        0        0     6122 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/system/session/rows/test_add_max_rows_in_max_groups.py
+-rw-r--r--   0        0        0    18921 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/system/session/rows/test_add_max_rows_infs_nulls.py
+-rw-r--r--   0        0        0    11017 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/system/session/rows/test_invalid.py
+-rw-r--r--   0        0        0     4465 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/system/session/test_budgets.py
+-rw-r--r--   0        0        0     2212 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/system/session/test_invalid_constraints.py
+-rw-r--r--   0        0        0      108 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/__init__.py
+-rw-r--r--   0        0        0      298 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/query_expr_compiler/__init__.py
+-rw-r--r--   0        0        0    76707 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/query_expr_compiler/test_measurement_visitor.py
+-rw-r--r--   0        0        0    60117 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/query_expr_compiler/test_output_schema_visitor.py
+-rw-r--r--   0        0        0      107 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/query_expr_compiler/transformation_visitor/__init__.py
+-rw-r--r--   0        0        0    17843 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/query_expr_compiler/transformation_visitor/conftest.py
+-rw-r--r--   0        0        0    24152 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py
+-rw-r--r--   0        0        0    36839 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py
+-rw-r--r--   0        0        0     7610 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py
+-rw-r--r--   0        0        0    15631 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/test_binning_spec.py
+-rw-r--r--   0        0        0     2301 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/test_catalog.py
+-rw-r--r--   0        0        0      657 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/test_cleanup.py
+-rw-r--r--   0        0        0     5285 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/test_constraints.py
+-rw-r--r--   0        0        0    21123 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/test_keyset.py
+-rw-r--r--   0        0        0    14053 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/test_neighboring_relations.py
+-rw-r--r--   0        0        0     3401 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/test_noise_info.py
+-rw-r--r--   0        0        0     5865 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/test_privacy_budget.py
+-rw-r--r--   0        0        0     5480 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/test_privacy_budget_rounding_helper.py
+-rw-r--r--   0        0        0     3011 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/test_protected_change.py
+-rw-r--r--   0        0        0    40576 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/test_query_builder.py
+-rw-r--r--   0        0        0    63726 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/test_query_expr_compiler.py
+-rw-r--r--   0        0        0    16787 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/test_query_expression.py
+-rw-r--r--   0        0        0     4874 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/test_query_expression_visitor.py
+-rw-r--r--   0        0        0     2172 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/test_schema.py
+-rw-r--r--   0        0        0    13538 2023-07-13 18:20:34.762807 tmlt_analytics-0.7.3/test/unit/test_schema_conversion.py
+-rw-r--r--   0        0        0    89952 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/test/unit/test_session.py
+-rw-r--r--   0        0        0     1604 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/test/unit/test_table_identifiers.py
+-rw-r--r--   0        0        0     5372 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/test/unit/test_transformation_utils.py
+-rw-r--r--   0        0        0      747 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/test/unit/test_truncation_strategy.py
+-rw-r--r--   0        0        0      518 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/test/unit/test_utils.py
+-rw-r--r--   0        0        0       18 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/test_requirements.txt
+-rw-r--r--   0        0        0      222 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/__init__.py
+-rw-r--r--   0        0        0     3666 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/_catalog.py
+-rw-r--r--   0        0        0     3555 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/_coerce_spark_schema.py
+-rw-r--r--   0        0        0    16162 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/_neighboring_relation.py
+-rw-r--r--   0        0        0     7164 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/_neighboring_relation_visitor.py
+-rw-r--r--   0        0        0     5683 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/_noise_info.py
+-rw-r--r--   0        0        0     4021 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/_privacy_budget_rounding_helper.py
+-rw-r--r--   0        0        0      184 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/_query_expr_compiler/__init__.py
+-rw-r--r--   0        0        0    10044 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/_query_expr_compiler/_compiler.py
+-rw-r--r--   0        0        0     7694 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py
+-rw-r--r--   0        0        0    42627 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py
+-rw-r--r--   0        0        0    47115 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py
+-rw-r--r--   0        0        0    60222 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py
+-rw-r--r--   0        0        0    12795 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/_schema.py
+-rw-r--r--   0        0        0     1250 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/_table_identifier.py
+-rw-r--r--   0        0        0     3980 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/_table_reference.py
+-rw-r--r--   0        0        0    10148 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/_transformation_utils.py
+-rw-r--r--   0        0        0      420 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/_type_checking.py
+-rw-r--r--   0        0        0    12087 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/binning_spec.py
+-rw-r--r--   0        0        0      306 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/cleanup.py
+-rw-r--r--   0        0        0      458 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/constraints/__init__.py
+-rw-r--r--   0        0        0     1101 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/constraints/_base.py
+-rw-r--r--   0        0        0      735 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/constraints/_simplify.py
+-rw-r--r--   0        0        0    12758 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/constraints/_truncation.py
+-rw-r--r--   0        0        0    11850 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/keyset.py
+-rw-r--r--   0        0        0    10546 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/privacy_budget.py
+-rw-r--r--   0        0        0     5482 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/protected_change.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:20:34.770807 tmlt_analytics-0.7.3/tmlt/analytics/py.typed
+-rw-r--r--   0        0        0   129752 2023-07-13 18:20:34.778807 tmlt_analytics-0.7.3/tmlt/analytics/query_builder.py
+-rw-r--r--   0        0        0    41076 2023-07-13 18:20:34.778807 tmlt_analytics-0.7.3/tmlt/analytics/query_expr.py
+-rw-r--r--   0        0        0    81600 2023-07-13 18:20:34.778807 tmlt_analytics-0.7.3/tmlt/analytics/session.py
+-rw-r--r--   0        0        0     3965 2023-07-13 18:20:34.778807 tmlt_analytics-0.7.3/tmlt/analytics/truncation_strategy.py
+-rw-r--r--   0        0        0     5397 2023-07-13 18:20:34.778807 tmlt_analytics-0.7.3/tmlt/analytics/utils.py
+-rw-r--r--   0        0        0     3529 1970-01-01 00:00:00.000000 tmlt_analytics-0.7.3/setup.py
+-rw-r--r--   0        0        0     3908 1970-01-01 00:00:00.000000 tmlt_analytics-0.7.3/PKG-INFO
```

### Comparing `tmlt_analytics-0.7.2/CHANGELOG.rst` & `tmlt_analytics-0.7.3/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 .. _analytics-changelog:
 
 Changelog
 =========
 
+0.7.3 - 2023-07-13
+------------------
+
+Fixed
+~~~~~
+- Fixed a crash in public and private joins.
+
 0.7.2 - 2023-06-15
 ------------------
 
 This release adds support for running Tumult Analytics on Python 3.10.
 It also enables adding continuous Gaussian noise to query results, and addresses a number of bugs and API inconsistencies.
 
 Added
```

### Comparing `tmlt_analytics-0.7.2/LICENSE` & `tmlt_analytics-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/LICENSE.docs` & `tmlt_analytics-0.7.3/LICENSE.docs`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/README.md` & `tmlt_analytics-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/_static/css/custom.css` & `tmlt_analytics-0.7.3/doc/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/_static/favicon.ico` & `tmlt_analytics-0.7.3/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/_static/js/version-banner.js` & `tmlt_analytics-0.7.3/doc/_static/js/version-banner.js`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/_static/logo.png` & `tmlt_analytics-0.7.3/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/conf.py` & `tmlt_analytics-0.7.3/doc/conf.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/howto-guides/bigquery/bigquery-setup.rst` & `tmlt_analytics-0.7.3/doc/howto-guides/bigquery/bigquery-setup.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/howto-guides/bigquery/docker-image.rst` & `tmlt_analytics-0.7.3/doc/howto-guides/bigquery/docker-image.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/howto-guides/bigquery/index.rst` & `tmlt_analytics-0.7.3/doc/howto-guides/bigquery/index.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/howto-guides/bigquery/inputs-outputs.rst` & `tmlt_analytics-0.7.3/doc/howto-guides/bigquery/inputs-outputs.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/howto-guides/bigquery/parameters.rst` & `tmlt_analytics-0.7.3/doc/howto-guides/bigquery/parameters.rst`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         "tumult-labs.analytics_tutorial.library_members",
         "tumult-labs.analytics_tutorial.member_counts"
     )
 
 .. note:: Replace the bucket, input, and output with the values
     specific to your project.
 
-Now, recall our Tufts Analytics program defined :ref:`earlier<bigquery inputs and outputs>`.
+Now, recall our Tumult Analytics program defined :ref:`earlier<bigquery inputs and outputs>`.
 
 .. code-block:: python
 
     import json
     import os
 
     from pyspark.sql import SparkSession
```

### Comparing `tmlt_analytics-0.7.2/doc/howto-guides/bigquery/running-the-program.rst` & `tmlt_analytics-0.7.3/doc/howto-guides/bigquery/running-the-program.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/howto-guides/bigquery/setup.rst` & `tmlt_analytics-0.7.3/doc/howto-guides/bigquery/setup.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/howto-guides/databricks.rst` & `tmlt_analytics-0.7.3/doc/howto-guides/databricks.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/howto-guides/installation.rst` & `tmlt_analytics-0.7.3/doc/howto-guides/installation.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/howto-guides/troubleshooting.rst` & `tmlt_analytics-0.7.3/doc/howto-guides/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/api_diagram.svg` & `tmlt_analytics-0.7.3/doc/images/api_diagram.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/chart_age_at_joining.png` & `tmlt_analytics-0.7.3/doc/images/chart_age_at_joining.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/chart_attacker_certainty.png` & `tmlt_analytics-0.7.3/doc/images/chart_attacker_certainty.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/chart_average_age_by_edu.png` & `tmlt_analytics-0.7.3/doc/images/chart_average_age_by_edu.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/chart_books_by_unique_members.png` & `tmlt_analytics-0.7.3/doc/images/chart_books_by_unique_members.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/chart_counts_age_gender.png` & `tmlt_analytics-0.7.3/doc/images/chart_counts_age_gender.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/chart_counts_different_eps.png` & `tmlt_analytics-0.7.3/doc/images/chart_counts_different_eps.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/chart_counts_edu+sex.png` & `tmlt_analytics-0.7.3/doc/images/chart_counts_edu+sex.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/chart_counts_education.png` & `tmlt_analytics-0.7.3/doc/images/chart_counts_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/chart_error_vs_partition_age_edu.png` & `tmlt_analytics-0.7.3/doc/images/chart_error_vs_partition_age_edu.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/chart_favorite_genres.png` & `tmlt_analytics-0.7.3/doc/images/chart_favorite_genres.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/chart_filters_education.png` & `tmlt_analytics-0.7.3/doc/images/chart_filters_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/chart_genres_by_age.png` & `tmlt_analytics-0.7.3/doc/images/chart_genres_by_age.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/chart_quantiles_education.png` & `tmlt_analytics-0.7.3/doc/images/chart_quantiles_education.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/chart_senior_counts_1.png` & `tmlt_analytics-0.7.3/doc/images/chart_senior_counts_1.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/chart_senior_counts_2.png` & `tmlt_analytics-0.7.3/doc/images/chart_senior_counts_2.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/chart_teen_edu_counts.png` & `tmlt_analytics-0.7.3/doc/images/chart_teen_edu_counts.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/chart_younger_age_counts.png` & `tmlt_analytics-0.7.3/doc/images/chart_younger_age_counts.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/clamping_bounds_averages.png` & `tmlt_analytics-0.7.3/doc/images/clamping_bounds_averages.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/clamping_bounds_schema.png` & `tmlt_analytics-0.7.3/doc/images/clamping_bounds_schema.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/flat_map_row_example.svg` & `tmlt_analytics-0.7.3/doc/images/flat_map_row_example.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/flow_chart_truncation.svg` & `tmlt_analytics-0.7.3/doc/images/flow_chart_truncation.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/histogram_books_borrowed.png` & `tmlt_analytics-0.7.3/doc/images/histogram_books_borrowed.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/index_api.svg` & `tmlt_analytics-0.7.3/doc/images/index_api.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/index_howto_guides.svg` & `tmlt_analytics-0.7.3/doc/images/index_howto_guides.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/index_more.svg` & `tmlt_analytics-0.7.3/doc/images/index_more.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/index_topic_guides.svg` & `tmlt_analytics-0.7.3/doc/images/index_topic_guides.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/index_tutorials.svg` & `tmlt_analytics-0.7.3/doc/images/index_tutorials.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/intuitive_noise_visualization.png` & `tmlt_analytics-0.7.3/doc/images/intuitive_noise_visualization.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/logo.png` & `tmlt_analytics-0.7.3/doc/images/logo.png`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/mock_checkout_logs.svg` & `tmlt_analytics-0.7.3/doc/images/mock_checkout_logs.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/private_join_example.svg` & `tmlt_analytics-0.7.3/doc/images/private_join_example.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/private_join_tables.svg` & `tmlt_analytics-0.7.3/doc/images/private_join_tables.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/images/public_join_example_zips.svg` & `tmlt_analytics-0.7.3/doc/images/public_join_example_zips.svg`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/index.rst` & `tmlt_analytics-0.7.3/doc/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,14 @@
   experts, and runs in production at institutions like the U.S. Census Bureau.
 - … *scalable*: it runs on `Spark <http://spark.apache.org>`__, so it can scale
   to very large datasets.
 
 For new users, `this Colab notebook <https://colab.research.google.com/drive/18J_UrHAKJf52RMRxi4OOpk59dV9tvKxO#offline=true&sandboxMode=true>`__ demonstrates basic features of the library without requiring a local installation.
 To explore further or work on larger datasets, a good starting point is the :ref:`installation instructions <installation instructions>`.
 
-A good starting point is the :ref:`installation instructions <installation instructions>`.
-
 The Tumult Analytics documentation introduces all of the concepts necessary to get started producing differentially private results.
 Users who wish to learn more about the fundamentals of differential privacy can consult
 `this blog post series <https://desfontain.es/privacy/friendly-intro-to-differential-privacy.html>`__
 or `this longer introduction <https://privacytools.seas.harvard.edu/files/privacytools/files/pedagogical-document-dp_0.pdf>`__.
 
 .. panels::
    :card: + intro-card text-center
```

### Comparing `tmlt_analytics-0.7.2/doc/intersphinx_mapping.json` & `tmlt_analytics-0.7.3/doc/intersphinx_mapping.json`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/privacy-policy.rst` & `tmlt_analytics-0.7.3/doc/privacy-policy.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/templates/python/class.rst` & `tmlt_analytics-0.7.3/doc/templates/python/class.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/templates/python/module.rst` & `tmlt_analytics-0.7.3/doc/templates/python/module.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/topic-guides/nulls-nans-infinities.rst` & `tmlt_analytics-0.7.3/doc/topic-guides/nulls-nans-infinities.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/topic-guides/privacy-budgets.rst` & `tmlt_analytics-0.7.3/doc/topic-guides/privacy-budgets.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/topic-guides/privacy-promise.rst` & `tmlt_analytics-0.7.3/doc/topic-guides/privacy-promise.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/topic-guides/spark.rst` & `tmlt_analytics-0.7.3/doc/topic-guides/spark.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/topic-guides/understanding-sensitivity.rst` & `tmlt_analytics-0.7.3/doc/topic-guides/understanding-sensitivity.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/topic-guides/working-with-sessions.rst` & `tmlt_analytics-0.7.3/doc/topic-guides/working-with-sessions.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/tutorials/clamping-bounds.rst` & `tmlt_analytics-0.7.3/doc/tutorials/clamping-bounds.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/tutorials/first-steps.rst` & `tmlt_analytics-0.7.3/doc/tutorials/first-steps.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/tutorials/groupby-queries.rst` & `tmlt_analytics-0.7.3/doc/tutorials/groupby-queries.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/tutorials/more-with-privacy-ids.rst` & `tmlt_analytics-0.7.3/doc/tutorials/more-with-privacy-ids.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/tutorials/privacy-budget-basics.rst` & `tmlt_analytics-0.7.3/doc/tutorials/privacy-budget-basics.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/tutorials/privacy-id-basics.rst` & `tmlt_analytics-0.7.3/doc/tutorials/privacy-id-basics.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/doc/tutorials/simple-transformations.rst` & `tmlt_analytics-0.7.3/doc/tutorials/simple-transformations.rst`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/examples/interactive_evaluation.ipynb` & `tmlt_analytics-0.7.3/examples/interactive_evaluation.ipynb`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/examples/private_join.ipynb` & `tmlt_analytics-0.7.3/examples/private_join.ipynb`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/examples/zcdp_puredp_switching.ipynb` & `tmlt_analytics-0.7.3/examples/zcdp_puredp_switching.ipynb`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/pyproject.toml` & `tmlt_analytics-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 readme = "README.md"
 authors = []
 license = "Apache-2.0"
 homepage = "https://www.tmlt.dev/"
 repository = "https://gitlab.com/tumult-labs/analytics"
 documentation = "https://docs.tmlt.dev/analytics/latest"
 # The version field is required in this file format, even though it's ignored because of poetry-dynamic-versioning.
-version = "0.7.2"
+version = "0.7.3"
 
 classifiers = [
    "Development Status :: 4 - Beta",
    "Intended Audience :: Developers",
    "Intended Audience :: Education",
    "Intended Audience :: Science/Research",
    "Natural Language :: English",
@@ -91,14 +91,17 @@
 requires = ["poetry-core>=1.3.2", "poetry-dynamic-versioning"]
 
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "semver"
 pattern = "^(?P<base>\\d+\\.\\d+\\.\\d+)(-(?P<stage>[a-zA-Z]+)\\.(?P<revision>\\d+))?"
 
+[tool.black]
+force-exclude = "noxfile.py"
+
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 line_length = 88
```

### Comparing `tmlt_analytics-0.7.2/test/conftest.py` & `tmlt_analytics-0.7.3/test/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -162,7 +162,29 @@
     transformation.return_value = return_value
     transformation.stability_function.return_value = stability_function_return_value
     transformation.stability_relation.return_value = stability_relation_return_value
     transformation.__or__ = Transformation.__or__
     if not stability_function_implemented:
         transformation.stability_function.side_effect = NotImplementedError("TEST")
     return transformation
+
+
+def params(d):
+    """Allows parameterizing tests with dictionaries.
+
+    Examples:
+    @params(
+        {
+            "test_case_1": {
+                "arg1": value1,
+                "arg2": value2,
+            },
+        }
+    )
+    test_func(...)
+    """
+    argnames = sorted({k for v in d.values() for k in v.keys()})
+    return pytest.mark.parametrize(
+        argnames=argnames,
+        argvalues=[[v.get(k) for k in argnames] for v in d.values()],
+        ids=d.keys(),
+    )
```

### Comparing `tmlt_analytics-0.7.2/test/system/session/conftest.py` & `tmlt_analytics-0.7.3/test/system/session/conftest.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/system/session/ids/test_constraint_propagation.py` & `tmlt_analytics-0.7.3/test/system/session/ids/test_constraint_propagation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/system/session/ids/test_count_distinct_optimization.py` & `tmlt_analytics-0.7.3/test/system/session/ids/test_count_distinct_optimization.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/system/session/ids/test_id_col_operations.py` & `tmlt_analytics-0.7.3/test/system/session/ids/test_id_col_operations.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/system/session/ids/test_l0_linf_truncation.py` & `tmlt_analytics-0.7.3/test/system/session/ids/test_l0_linf_truncation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/system/session/ids/test_l1_truncation.py` & `tmlt_analytics-0.7.3/test/system/session/ids/test_l1_truncation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/system/session/ids/test_partition.py` & `tmlt_analytics-0.7.3/test/system/session/ids/test_partition.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/system/session/mixed/test_mixed_session.py` & `tmlt_analytics-0.7.3/test/system/session/mixed/test_mixed_session.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/system/session/rows/conftest.py` & `tmlt_analytics-0.7.3/test/system/session/rows/conftest.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/system/session/rows/test_add_max_rows.py` & `tmlt_analytics-0.7.3/test/system/session/rows/test_add_max_rows.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/system/session/rows/test_add_max_rows_in_max_groups.py` & `tmlt_analytics-0.7.3/test/system/session/rows/test_add_max_rows_in_max_groups.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/system/session/rows/test_invalid.py` & `tmlt_analytics-0.7.3/test/system/session/rows/test_invalid.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/system/session/test_budgets.py` & `tmlt_analytics-0.7.3/test/system/session/test_budgets.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/system/session/test_invalid_constraints.py` & `tmlt_analytics-0.7.3/test/system/session/test_invalid_constraints.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/query_expr_compiler/test_measurement_visitor.py` & `tmlt_analytics-0.7.3/test/unit/query_expr_compiler/test_measurement_visitor.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/query_expr_compiler/test_output_schema_visitor.py` & `tmlt_analytics-0.7.3/test/unit/query_expr_compiler/test_output_schema_visitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,16 @@
     Rename,
     ReplaceInfinity,
     ReplaceNullAndNan,
     Select,
 )
 from tmlt.analytics.truncation_strategy import TruncationStrategy
 
+from ...conftest import params
+
 # Convenience lambda functions to create dataframes for KeySets
 GET_PUBLIC = lambda: SparkSession.builder.getOrCreate().createDataFrame(
     [],
     schema=StructType(
         [StructField("A", LongType(), False), StructField("A+B", LongType(), False)]
     ),
 )
@@ -1013,14 +1015,138 @@
     def test_visit_join_public(
         self, query: JoinPublic, expected_schema: Schema
     ) -> None:
         """Test visit_join_public."""
         schema = self.visitor.visit_join_public(query)
         assert schema == expected_schema
 
+    # pylint: disable=no-self-use
+    @params(
+        {
+            "all_allow_null": {
+                "left_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=True)}
+                ),
+                "right_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=True)}
+                ),
+                "expected_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=True)}
+                ),
+            },
+            "no_nulls_null": {
+                "left_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=False)}
+                ),
+                "right_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=False)}
+                ),
+                "expected_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=False)}
+                ),
+            },
+            "public_only_null": {
+                "left_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=False)}
+                ),
+                "right_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=True)}
+                ),
+                "expected_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=False)}
+                ),
+            },
+            "private_only_null": {
+                "left_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=True)}
+                ),
+                "right_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=False)}
+                ),
+                "expected_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=False)}
+                ),
+            },
+        }
+    )
+    def test_visit_join_private_nulls(self, left_schema, right_schema, expected_schema):
+        """Test that OutputSchemaVisitor correctly propagates nulls through a join."""
+        catalog = Catalog()
+        catalog.add_private_table("left", left_schema)
+        catalog.add_private_table("right", right_schema)
+        visitor = OutputSchemaVisitor(catalog)
+        query = JoinPrivate(
+            child=PrivateSource("left"),
+            right_operand_expr=PrivateSource("right"),
+            truncation_strategy_left=TruncationStrategy.DropExcess(1),
+            truncation_strategy_right=TruncationStrategy.DropExcess(1),
+        )
+        result_schema = visitor.visit_join_private(query)
+        assert result_schema == expected_schema
+
+    @params(
+        {
+            "all_allow_null": {
+                "private_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=True)}
+                ),
+                "public_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=True)}
+                ),
+                "expected_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=True)}
+                ),
+            },
+            "no_nulls_null": {
+                "private_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=False)}
+                ),
+                "public_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=False)}
+                ),
+                "expected_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=False)}
+                ),
+            },
+            "public_only_null": {
+                "private_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=False)}
+                ),
+                "public_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=True)}
+                ),
+                "expected_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=False)}
+                ),
+            },
+            "private_only_null": {
+                "private_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=True)}
+                ),
+                "public_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=False)}
+                ),
+                "expected_schema": Schema(
+                    {"A": ColumnDescriptor(ColumnType.VARCHAR, allow_null=False)}
+                ),
+            },
+        }
+    )
+    def test_visit_join_public_nulls(
+        self, private_schema, public_schema, expected_schema
+    ):
+        """Test that OutputSchemaVisitor correctly propagates nulls through a join."""
+        catalog = Catalog()
+        catalog.add_private_table("private", private_schema)
+        catalog.add_public_table("public", public_schema)
+        visitor = OutputSchemaVisitor(catalog)
+        query = JoinPublic(child=PrivateSource("private"), public_table="public")
+        result_schema = visitor.visit_join_public(query)
+        assert result_schema == expected_schema
+
     @pytest.mark.parametrize(
         "query,expected_schema",
         [
             (
                 ReplaceNullAndNan(child=PrivateSource("private"), replace_with={}),
                 Schema(
                     {
```

### Comparing `tmlt_analytics-0.7.2/test/unit/query_expr_compiler/transformation_visitor/conftest.py` & `tmlt_analytics-0.7.3/test/unit/query_expr_compiler/transformation_visitor/conftest.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py` & `tmlt_analytics-0.7.3/test/unit/query_expr_compiler/transformation_visitor/test_add_keys.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py` & `tmlt_analytics-0.7.3/test/unit/query_expr_compiler/transformation_visitor/test_add_rows.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py` & `tmlt_analytics-0.7.3/test/unit/query_expr_compiler/transformation_visitor/test_constraints.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/test_binning_spec.py` & `tmlt_analytics-0.7.3/test/unit/test_binning_spec.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/test_catalog.py` & `tmlt_analytics-0.7.3/test/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/test_cleanup.py` & `tmlt_analytics-0.7.3/test/unit/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/test_constraints.py` & `tmlt_analytics-0.7.3/test/unit/test_constraints.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/test_keyset.py` & `tmlt_analytics-0.7.3/test/unit/test_keyset.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/test_neighboring_relations.py` & `tmlt_analytics-0.7.3/test/unit/test_neighboring_relations.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/test_noise_info.py` & `tmlt_analytics-0.7.3/test/unit/test_noise_info.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/test_privacy_budget.py` & `tmlt_analytics-0.7.3/test/unit/test_privacy_budget.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/test_privacy_budget_rounding_helper.py` & `tmlt_analytics-0.7.3/test/unit/test_privacy_budget_rounding_helper.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/test_protected_change.py` & `tmlt_analytics-0.7.3/test/unit/test_protected_change.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/test_query_builder.py` & `tmlt_analytics-0.7.3/test/unit/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/test_query_expr_compiler.py` & `tmlt_analytics-0.7.3/test/unit/test_query_expr_compiler.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/test_query_expression.py` & `tmlt_analytics-0.7.3/test/unit/test_query_expression.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/test_query_expression_visitor.py` & `tmlt_analytics-0.7.3/test/unit/test_query_expression_visitor.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/test_schema.py` & `tmlt_analytics-0.7.3/test/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/test_schema_conversion.py` & `tmlt_analytics-0.7.3/test/unit/test_schema_conversion.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/test_session.py` & `tmlt_analytics-0.7.3/test/unit/test_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,27 +71,28 @@
 from tmlt.analytics._table_reference import TableReference
 from tmlt.analytics.constraints import (
     Constraint,
     MaxGroupsPerID,
     MaxRowsPerGroupPerID,
     MaxRowsPerID,
 )
+from tmlt.analytics.keyset import KeySet
 from tmlt.analytics.privacy_budget import (
     ApproxDPBudget,
     PrivacyBudget,
     PureDPBudget,
     RhoZCDPBudget,
 )
 from tmlt.analytics.protected_change import (
     AddMaxRows,
     AddMaxRowsInMaxGroups,
     AddOneRow,
     AddRowsWithID,
 )
-from tmlt.analytics.query_builder import QueryBuilder
+from tmlt.analytics.query_builder import GroupedQueryBuilder, QueryBuilder
 from tmlt.analytics.query_expr import PrivateSource, QueryExpr
 from tmlt.analytics.session import Session
 
 from ..conftest import assert_frame_equal_with_sort, create_mock_transformation
 
 
 def _privacy_budget_to_exact_number(
@@ -1237,31 +1238,50 @@
                 + expected_output
             )
             session.describe("private")
             # pylint: enable=line-too-long
             mock_print.assert_called_with(expected)
 
     @pytest.mark.parametrize(
-        "query,expected_output",
+        "query,constraint_output,group_output",
         [
             (
                 QueryBuilder("private").enforce(MaxRowsPerID(5)),
                 "\t\t- MaxRowsPerID(max=5)",
+                "",
             ),
             (
                 QueryBuilder("private")
                 .enforce(MaxGroupsPerID("X", 5))
                 .enforce(MaxRowsPerGroupPerID("B", 1)),
                 "\t\t- MaxGroupsPerID(grouping_column='X', max=5)\n\t\t"
                 "- MaxRowsPerGroupPerID(grouping_column='B', max=1)",
+                "",
+            ),
+            (
+                QueryBuilder("private")
+                .enforce(MaxRowsPerID(5))
+                .groupby(KeySet.from_dict({})),
+                "\t\t- MaxRowsPerID(max=5)",
+                "",
+            ),
+            (
+                QueryBuilder("private")
+                .enforce(MaxRowsPerID(5))
+                .groupby(KeySet.from_dict({"A": ["0", "1"]})),
+                "\t\t- MaxRowsPerID(max=5)",
+                "\nGrouped on columns 'A' (2 groups)",
             ),
         ],
     )
     def test_describe_query_with_constraints(
-        self, query: QueryBuilder, expected_output: str
+        self,
+        query: Union[QueryBuilder, GroupedQueryBuilder],
+        constraint_output: str,
+        group_output: str,
     ):
         """Test :func:`_describe` with a query with constraints."""
         with patch("builtins.print") as mock_print, patch(
             "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
         ) as mock_accountant:
             self._setup_accountant_with_id(
                 mock_accountant, privacy_budget=ExactNumber(10)
@@ -1270,20 +1290,69 @@
             session = Session(accountant=mock_accountant, public_sources={})
             expected = (
                 """Columns:
 \t- 'A'  VARCHAR, ID column (in ID space identifier_A)
 \t- 'B'  INTEGER
 \t- 'X'  INTEGER
 \tConstraints:\n"""
-                + expected_output
+                + constraint_output
+                + group_output
             )
             session.describe(query)
             # pylint: enable=line-too-long
             mock_print.assert_called_with(expected)
 
+    @pytest.mark.parametrize(
+        "query,expected_output",
+        [
+            pytest.param(
+                QueryBuilder("private").groupby(KeySet.from_dict({})),
+                """Columns:
+\t- 'A'  VARCHAR
+\t- 'B'  INTEGER
+\t- 'X'  INTEGER""",
+                id="query_builder_groupby_empty",
+            ),
+            pytest.param(
+                QueryBuilder("private").groupby(KeySet.from_dict({"A": ["0", "1"]})),
+                """Columns:
+\t- 'A'  VARCHAR
+\t- 'B'  INTEGER
+\t- 'X'  INTEGER
+Grouped on columns 'A' (2 groups)""",
+                id="query_builder_groupby_1_col",
+            ),
+            pytest.param(
+                QueryBuilder("private").groupby(
+                    KeySet.from_dict({"A": ["0", "1"], "B": [0, 1]})
+                ),
+                """Columns:
+\t- 'A'  VARCHAR
+\t- 'B'  INTEGER
+\t- 'X'  INTEGER
+Grouped on columns 'A', 'B' (4 groups)""",
+                id="query_builder_groupby_multi_col",
+            ),
+        ],
+    )
+    def test_describe_grouped_query(
+        self, query: GroupedQueryBuilder, expected_output: str
+    ):
+        """Test :func:`_describe` with a QueryExpr, QueryBuilder, or table name."""
+        with patch("builtins.print") as mock_print, patch(
+            "tmlt.core.measurements.interactive_measurements.PrivacyAccountant"
+        ) as mock_accountant:
+            self._setup_accountant(mock_accountant, privacy_budget=ExactNumber(10))
+            mock_accountant.state = PrivacyAccountantState.ACTIVE
+
+            session = Session(accountant=mock_accountant, public_sources={})
+
+            session.describe(query)
+            mock_print.assert_called_with(expected_output)
+
     def test_supported_spark_types(self, spark):
         """Session works with supported Spark data types."""
         alltypes_sdf = spark.createDataFrame(
             pd.DataFrame(
                 [[1.2, 3.4, 17, 42, "blah"]], columns=["A", "B", "C", "D", "E"]
             ),
             schema=StructType(
```

### Comparing `tmlt_analytics-0.7.2/test/unit/test_table_identifiers.py` & `tmlt_analytics-0.7.3/test/unit/test_table_identifiers.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/test_transformation_utils.py` & `tmlt_analytics-0.7.3/test/unit/test_transformation_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/test_truncation_strategy.py` & `tmlt_analytics-0.7.3/test/unit/test_truncation_strategy.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/test/unit/test_utils.py` & `tmlt_analytics-0.7.3/test/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/_catalog.py` & `tmlt_analytics-0.7.3/tmlt/analytics/_catalog.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/_coerce_spark_schema.py` & `tmlt_analytics-0.7.3/tmlt/analytics/_coerce_spark_schema.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/_neighboring_relation.py` & `tmlt_analytics-0.7.3/tmlt/analytics/_neighboring_relation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/_neighboring_relation_visitor.py` & `tmlt_analytics-0.7.3/tmlt/analytics/_neighboring_relation_visitor.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/_noise_info.py` & `tmlt_analytics-0.7.3/tmlt/analytics/_noise_info.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/_privacy_budget_rounding_helper.py` & `tmlt_analytics-0.7.3/tmlt/analytics/_privacy_budget_rounding_helper.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/_compiler.py` & `tmlt_analytics-0.7.3/tmlt/analytics/_query_expr_compiler/_compiler.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py` & `tmlt_analytics-0.7.3/tmlt/analytics/_query_expr_compiler/_constraint_propagation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py` & `tmlt_analytics-0.7.3/tmlt/analytics/_query_expr_compiler/_measurement_visitor.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py` & `tmlt_analytics-0.7.3/tmlt/analytics/_query_expr_compiler/_output_schema_visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,16 +97,22 @@
         if left_schema[column].column_type != right_schema[column].column_type:
             raise ValueError(
                 "Join columns must have identical types on both tables, "
                 f"but column '{column}' does not: {left_schema[column]} and "
                 f"{right_schema[column]} are incompatible"
             )
 
+    join_column_schemas = {column: left_schema[column] for column in join_columns}
+    for column in join_column_schemas:
+        join_column_schemas[column].allow_null = (
+            left_schema[column].allow_null and right_schema[column].allow_null
+        )
+
     output_schema = {
-        **{column: left_schema[column] for column in join_columns},
+        **join_column_schemas,
         **{
             column + ("_left" if column in common_columns else ""): left_schema[column]
             for column in left_schema
             if column not in join_columns
         },
         **{
             column
```

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py` & `tmlt_analytics-0.7.3/tmlt/analytics/_query_expr_compiler/_transformation_visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -856,18 +856,14 @@
                     f"There is no public source with the identifier {expr.public_table}"
                 ) from e
         else:
             public_df = expr.public_table
 
         public_df_schema = Schema(spark_schema_to_analytics_columns(public_df.schema))
 
-        join_null_cols = any(
-            col_desc.allow_null for col_desc in public_df_schema.values()
-        )
-
         def gen_transformation_dictmetric(parent_domain, parent_metric, target):
             input_domain = lookup_domain(child_transformation.output_domain, child_ref)
             input_metric = lookup_metric(child_transformation.output_metric, child_ref)
             if not isinstance(input_domain, SparkDataFrameDomain):
                 raise AssertionError(
                     "Unrecognized input domain. This is probably a bug; "
                     "please let us know about it so we can fix it!"
@@ -887,15 +883,15 @@
                     input_domain=SparkDataFrameDomain(input_domain.schema),
                     public_df=public_df,
                     public_df_domain=SparkDataFrameDomain(
                         analytics_to_spark_columns_descriptor(public_df_schema)
                     ),
                     join_cols=expr.join_columns if expr.join_columns else None,
                     metric=input_metric,
-                    join_on_nulls=join_null_cols,
+                    join_on_nulls=True,
                 ),
                 lambda *args: None,
             )
 
         def gen_transformation_ark(parent_domain, parent_metric, target):
             return PublicJoinValueTransformation(
                 parent_domain,
@@ -903,15 +899,15 @@
                 child_ref.identifier,
                 target,
                 public_df,
                 SparkDataFrameDomain(
                     analytics_to_spark_columns_descriptor(public_df_schema)
                 ),
                 expr.join_columns,
-                join_on_nulls=join_null_cols,
+                join_on_nulls=True,
             )
 
         child_domain = lookup_domain(child_transformation.output_domain, child_ref)
         if not isinstance(child_domain, SparkDataFrameDomain):
             raise AssertionError(
                 "Unrecognized input domain. This is probably a bug; "
                 "please let us know about it so we can fix it!"
```

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/_schema.py` & `tmlt_analytics-0.7.3/tmlt/analytics/_schema.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/_table_identifier.py` & `tmlt_analytics-0.7.3/tmlt/analytics/_table_identifier.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/_table_reference.py` & `tmlt_analytics-0.7.3/tmlt/analytics/_table_reference.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/_transformation_utils.py` & `tmlt_analytics-0.7.3/tmlt/analytics/_transformation_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/binning_spec.py` & `tmlt_analytics-0.7.3/tmlt/analytics/binning_spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,14 +122,18 @@
     All :data:`supported data types <tmlt.analytics.session.SUPPORTED_SPARK_TYPES>`
     can be binned using a BinningSpec.
 
     Values outside the range of the provided bins and ``None`` types are all
     mapped to ``None`` (``null`` in Spark), as are NaN values by default. Bin
     names are generated based on the bin edges, but custom names can be provided.
 
+    By default, the right edge of each bin is included in that bin: using edges
+    `[0, 5, 10]` will lead to bins `[0, 5]` and `(5, 10]`. To include the
+    left edge instead, set the ``right`` parameter to False.
+
     Examples:
         >>> spec = BinningSpec([0,5,10])
         >>> spec.bins()
         ['[0, 5]', '(5, 10]']
         >>> spec(0)
         '[0, 5]'
         >>> spec(5)
```

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/constraints/_base.py` & `tmlt_analytics-0.7.3/tmlt/analytics/constraints/_base.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/constraints/_simplify.py` & `tmlt_analytics-0.7.3/tmlt/analytics/constraints/_simplify.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/constraints/_truncation.py` & `tmlt_analytics-0.7.3/tmlt/analytics/constraints/_truncation.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/keyset.py` & `tmlt_analytics-0.7.3/tmlt/analytics/keyset.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/privacy_budget.py` & `tmlt_analytics-0.7.3/tmlt/analytics/privacy_budget.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/protected_change.py` & `tmlt_analytics-0.7.3/tmlt/analytics/protected_change.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/query_builder.py` & `tmlt_analytics-0.7.3/tmlt/analytics/query_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,16 @@
     def join_public(
         self,
         public_table: Union[DataFrame, str],
         join_columns: Optional[Sequence[str]] = None,
     ) -> "QueryBuilder":
         """Updates the current query to join with a dataframe or public source.
 
+        This operation is an inner join.
+
         This operation performs a natural join between two tables. This means
         that the resulting table will contain all columns unique to each input
         table, along with one copy of each common column. In most cases, the
         columns have the same names they did in the input tables.
 
         By default, the input tables are joined on all common columns (i.e.,
         columns whose names and data types match). However if ``join_columns``
@@ -277,14 +279,16 @@
     ) -> "QueryBuilder":
         # pylint: disable=protected-access
         """Updates the current query to join with another :class:`QueryBuilder`.
 
         The current query can also join with a named private table (represented
         as a string).
 
+        This operation is an inner join.
+
         This operation is a natural join, with the same behavior and requirements as
         :func:`join_public`.
 
         For operations on tables with a
         :class:`~tmlt.analytics.protected_change.ProtectedChange` that protects
         adding or removing rows (e.g.
         :class:`~tmlt.analytics.protected_change.AddMaxRows`), there is a key
```

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/query_expr.py` & `tmlt_analytics-0.7.3/tmlt/analytics/query_expr.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/session.py` & `tmlt_analytics-0.7.3/tmlt/analytics/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 from tmlt.analytics.protected_change import (
     AddMaxRows,
     AddMaxRowsInMaxGroups,
     AddOneRow,
     AddRowsWithID,
     ProtectedChange,
 )
-from tmlt.analytics.query_builder import ColumnType, QueryBuilder
+from tmlt.analytics.query_builder import ColumnType, GroupedQueryBuilder, QueryBuilder
 from tmlt.analytics.query_expr import QueryExpr
 
 __all__ = ["Session", "SUPPORTED_SPARK_TYPES", "TYPE_COERCION_MAP"]
 
 
 class _PrivateSourceTuple(NamedTuple):
     """Named tuple of private Dataframe, domain and protected change."""
@@ -743,15 +743,16 @@
                 "Session accountant's input metric has an incorrect type. This is "
                 "probably a bug; please let us know about it so we can "
                 "fix it!"
             )
         return self._accountant.input_metric
 
     def describe(
-        self, obj: Optional[Union[QueryExpr, QueryBuilder, str]] = None
+        self,
+        obj: Optional[Union[QueryExpr, QueryBuilder, GroupedQueryBuilder, str]] = None,
     ) -> None:
         """Describe a Session, table, or query.
 
         If ``obj`` is not specified, ``session.describe()`` will describe the
         Session and all of the tables it contains.
 
         If ``obj`` is a :class:`~tmlt.analytics.query_builder.QueryBuilder` or
@@ -804,25 +805,25 @@
                 - 'X'  INTEGER
 
         Args:
             obj: The table or query to be described, or None to describe the
                 whole Session.
         """
         if obj is None:
-            self._describe_self()
-        elif isinstance(obj, QueryExpr):
-            self._describe_query(obj)
+            print(self._describe_self())
+        elif isinstance(obj, (QueryExpr, GroupedQueryBuilder)):
+            print(self._describe_query_obj(obj))
         elif isinstance(obj, QueryBuilder):
-            self._describe_query(obj.query_expr)
+            print(self._describe_query_obj(obj.query_expr))
         elif isinstance(obj, str):
-            self._describe_query(QueryBuilder(obj).query_expr)
+            print(self._describe_query_obj(QueryBuilder(obj).query_expr))
         else:
             assert_never(obj)
 
-    def _describe_self(self) -> None:
+    def _describe_self(self) -> str:
         """Describe the current state of this session."""
         out = []
         state = self._accountant.state
         if state == PrivacyAccountantState.ACTIVE:
             # Don't add anything to output if the session is active
             pass
         elif state == PrivacyAccountantState.RETIRED:
@@ -886,43 +887,56 @@
                     + "\n".join(private_table_descs)
                 )
             if len(public_table_descs) != 0:
                 out.append(
                     "The following public tables are available:\n"
                     + "\n".join(public_table_descs)
                 )
-        print("\n".join(out))
+        return "\n".join(out)
 
-    def _describe_query(self, query_expr: QueryExpr):
-        """Describe the output schema of a query and the constraints on it."""
-        schema = self._compiler.query_schema(query_expr, self._catalog)
+    def _describe_query_obj(
+        self, query_obj: Union[QueryExpr, GroupedQueryBuilder]
+    ) -> str:
+        """Build a description of a query object."""
+        if isinstance(query_obj, GroupedQueryBuilder):
+            expr = query_obj._query_expr  # pylint: disable=protected-access
+        else:
+            expr = query_obj
+        schema = self._compiler.query_schema(expr, self._catalog)
         schema_desc = _describe_schema(schema)
         constraints: Optional[List[Constraint]] = None
         try:
             constraints = self._compiler.build_transformation(
-                query=query_expr,
+                query=expr,
                 input_domain=self._input_domain,
                 input_metric=self._input_metric,
                 public_sources=self._public_sources,
                 catalog=self._catalog,
                 table_constraints=self._table_constraints,
             )[2]
         except NotImplementedError:
             # If the query results in a measurement, this will happen.
             # There are no constraints on measurements, so we can just
             # pass the schema description through.
             pass
         description = "\n".join(schema_desc)
-        if not constraints:
-            print(description)
-        else:
+        if constraints:
             description += "\n\tConstraints:\n"
             constraints_strs = [f"\t\t- {e}" for e in constraints]
             description += "\n".join(constraints_strs)
-            print(description)
+        if isinstance(query_obj, GroupedQueryBuilder):
+            ks_df = (
+                query_obj._groupby_keys.dataframe()  # pylint: disable=protected-access
+            )
+            if len(ks_df.columns) > 0:
+                description += "\nGrouped on columns "
+                col_strs = [f"'{col}'" for col in ks_df.columns]
+                description += ", ".join(col_strs)
+                description += f" ({ks_df.count()} groups)"
+        return description
 
     @typechecked
     def get_schema(self, source_id: str) -> Schema:
         """Returns the schema for any data source.
 
         This includes information on whether the columns are nullable.
```

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/truncation_strategy.py` & `tmlt_analytics-0.7.3/tmlt/analytics/truncation_strategy.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/tmlt/analytics/utils.py` & `tmlt_analytics-0.7.3/tmlt/analytics/utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_analytics-0.7.2/setup.py` & `tmlt_analytics-0.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'sympy>=1.8,<1.10',
  'tmlt.core>=0.10.1,<0.11.0',
  'typeguard>=2.12.1,<2.13.0',
  'typing-extensions>=3.10.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'tmlt-analytics',
-    'version': '0.7.2',
+    'version': '0.7.3',
     'description': "Tumult's differential privacy analytics API",
     'long_description': "# Tumult Analytics\n\nTumult Analytics is a library that allows users to execute differentially private operations on\ndata without having to worry about the privacy implementation, which is handled\nautomatically by the API. It is built atop the [Tumult Core library](https://gitlab.com/tumult-labs/core).\n\n## Installation\n\nSee the [installation instructions in the documentation](https://docs.tmlt.dev/analytics/latest/installation.html#prerequisites)\nfor information about setting up prerequisites such as Spark.\n\nOnce the prerequisites are installed, you can install Tumult Analytics using [pip](https://pypi.org/project/pip).\n\n```bash\npip install tmlt.analytics\n```\n\n## Documentation\n\nThe full documentation is located at https://docs.tmlt.dev/analytics/latest/.\n\n## Support\n\nIf you have any questions/concerns, please [create an issue](https://gitlab.com/tumult-labs/analytics/-/issues) or reach out to us on [Slack](https://tmltdev.slack.com/join/shared_invite/zt-1bky0mh9v-vOB8azKAVoxmzJDUdWd5Wg#).\n\n## Contributing\n\nWe are not yet accepting external contributions, but please let us know if you are interested in contributing [via Slack](https://tmltdev.slack.com/join/shared_invite/zt-1bky0mh9v-vOB8azKAVoxmzJDUdWd5Wg#).\n\nSee [CONTRIBUTING.md](CONTRIBUTING.md) for information about installing our development dependencies and running tests.\n\n## Citing Tumult Analytics\n\nIf you use Tumult Analytics for a scientific publication, we would appreciate citations to the published software or/and its whitepaper. Both citations can be found below; for the software citation, please replace the version with the version you are using.\n\n```\n@software{tumultanalyticssoftware,\n    author = {Tumult Labs},\n    title = {Tumult {{Analytics}}},\n    month = dec,\n    year = 2022,\n    version = {latest},\n    url = {https://tmlt.dev}\n}\n```\n\n```\n@article{tumultanalyticswhitepaper,\n  title={Tumult {{Analytics}}: a robust, easy-to-use, scalable, and expressive framework for differential privacy},\n  author={Berghel, Skye and Bohannon, Philip and Desfontaines, Damien and Estes, Charles and Haney, Sam and Hartman, Luke and Hay, Michael and Machanavajjhala, Ashwin and Magerlein, Tom and Miklau, Gerome and Pai, Amritha and Sexton, William and Shrestha, Ruchit},\n  journal={arXiv preprint arXiv:2212.04133},\n  month = dec,\n  year={2022}\n}\n```\n\n## License\n\nCopyright Tumult Labs 2023\n\nTumult Analytics' source code is licensed under the Apache License, version 2.0 (Apache-2.0).\nTumult Analytics' documentation is licensed under\nCreative Commons Attribution-ShareAlike 4.0 International (CC-BY-SA-4.0).\n",
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.tmlt.dev/',
```

### Comparing `tmlt_analytics-0.7.2/PKG-INFO` & `tmlt_analytics-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmlt-analytics
-Version: 0.7.2
+Version: 0.7.3
 Summary: Tumult's differential privacy analytics API
 Home-page: https://www.tmlt.dev/
 License: Apache-2.0
 Requires-Python: >=3.7.1,<3.11.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

