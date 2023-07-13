# Comparing `tmp/troubadix-23.7.0.tar.gz` & `tmp/troubadix-23.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troubadix-23.7.0.tar", max compression
+gzip compressed data, was "troubadix-23.7.1.tar", max compression
```

## Comparing `troubadix-23.7.0.tar` & `troubadix-23.7.1.tar`

### file list

```diff
@@ -1,195 +1,195 @@
--rw-r--r--   0        0        0    35149 2023-07-10 08:28:45.946539 troubadix-23.7.0/LICENSE
--rw-r--r--   0        0        0     2730 2023-07-10 08:28:45.946539 troubadix-23.7.0/README.md
--rw-r--r--   0        0        0     2516 2023-07-10 08:28:45.946539 troubadix-23.7.0/pyproject.toml
--rw-r--r--   0        0        0      716 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/__init__.py
--rw-r--r--   0        0        0      716 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/helper/__init__.py
--rw-r--r--   0        0        0     8416 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/helper/test_linguistic_exception_handler.py
--rw-r--r--   0        0        0     1940 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/helper/test_patterns.py
--rw-r--r--   0        0        0     2396 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/__init__.py
--rw-r--r--   0        0        0     1012 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/fail.nasl
--rw-r--r--   0        0        0     1291 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/fail2.nasl
--rw-r--r--   0        0        0     2100 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test.nasl
--rw-r--r--   0        0        0     2450 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_badwords.py
--rw-r--r--   0        0        0     5109 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_copyright_text.py
--rw-r--r--   0        0        0     6961 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_copyright_year.py
--rw-r--r--   0        0        0     5004 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_creation_date.py
--rw-r--r--   0        0        0     5881 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_cve_format.py
--rw-r--r--   0        0        0     4914 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_cvss_format.py
--rw-r--r--   0        0        0     8970 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_dependencies.py
--rw-r--r--   0        0        0     5808 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_dependency_category_order.py
--rw-r--r--   0        0        0     5589 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_deprecated_dependency.py
--rw-r--r--   0        0        0     4545 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_deprecated_functions.py
--rw-r--r--   0        0        0     2394 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_double_end_points.py
--rw-r--r--   0        0        0     3504 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_duplicate_oid.py
--rw-r--r--   0        0        0     4686 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_duplicated_script_tags.py
--rw-r--r--   0        0        0     3906 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_encoding.py
--rw-r--r--   0        0        0     1982 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/fail_bad_new_line.nasl
--rw-r--r--   0        0        0      246 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/fail_badwords.nasl
--rw-r--r--   0        0        0     1979 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/fail_name_and_copyright_newline.nasl
--rw-r--r--   0        0        0     1965 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/fail_name_newline.nasl
--rwxr-xr-x   0        0        0     1012 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/fail_permissions.nasl
--rw-r--r--   0        0        0      150 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/fail_spelling.nasl
--rw-r--r--   0        0        0     2213 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/fail.nasl
--rw-r--r--   0        0        0      246 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/fail_badwords.nasl
--rw-r--r--   0        0        0     1990 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl
--rw-r--r--   0        0        0     1987 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl
--rw-r--r--   0        0        0     2134 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl
--rw-r--r--   0        0        0     1023 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/runner/fail.nasl
--rw-r--r--   0        0        0     1302 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl
--rw-r--r--   0        0        0     2122 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/runner/test.nasl
--rw-r--r--   0        0        0     2119 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl
--rw-r--r--   0        0        0     1023 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/test.inc
--rw-r--r--   0        0        0     2122 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/test.nasl
--rw-r--r--   0        0        0     2976 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/nasl/warning.nasl
--rw-r--r--   0        0        0     1012 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/ok_permissions.nasl
--rw-r--r--   0        0        0     2100 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_files/test_oid.nasl
--rw-r--r--   0        0        0     4548 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_forking_nasl_functions.py
--rw-r--r--   0        0        0     2271 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_get_kb_on_services.py
--rw-r--r--   0        0        0     9438 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_grammar.py
--rw-r--r--   0        0        0     6936 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_http_links_in_tags.py
--rw-r--r--   0        0        0     4730 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_illegal_characters.py
--rw-r--r--   0        0        0     5965 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_log_messages.py
--rw-r--r--   0        0        0     6174 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_malformed_dependencies.py
--rw-r--r--   0        0        0    21051 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_misplaced_compare_in_if.py
--rw-r--r--   0        0        0     3585 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_missing_desc_exit.py
--rw-r--r--   0        0        0     3101 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_missing_tag_solution.py
--rw-r--r--   0        0        0     4688 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_newlines.py
--rw-r--r--   0        0        0    40813 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_overlong_script_tags.py
--rw-r--r--   0        0        0     4294 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_prod_svc_detect_in_vulnvt.py
--rw-r--r--   0        0        0     4594 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_qod.py
--rw-r--r--   0        0        0     5844 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_reporting_consistency.py
--rw-r--r--   0        0        0     3371 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_add_preference_type.py
--rw-r--r--   0        0        0     2353 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_calls_empty_values.py
--rw-r--r--   0        0        0     2799 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_calls_recommended.py
--rw-r--r--   0        0        0     2650 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_category.py
--rw-r--r--   0        0        0     3469 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_copyright.py
--rw-r--r--   0        0        0     3877 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_family.py
--rw-r--r--   0        0        0     3079 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_tag_form.py
--rw-r--r--   0        0        0     6010 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_tag_whitespaces.py
--rw-r--r--   0        0        0     3313 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_tags_mandatory.py
--rw-r--r--   0        0        0     4858 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_version_and_last_modification_tags.py
--rw-r--r--   0        0        0     3016 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_xref_form.py
--rw-r--r--   0        0        0     2189 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_script_xref_url.py
--rw-r--r--   0        0        0     6599 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_security_messages.py
--rw-r--r--   0        0        0     3021 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_set_get_kb_calls.py
--rw-r--r--   0        0        0     7260 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_solution_text.py
--rw-r--r--   0        0        0     3306 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_solution_type.py
--rw-r--r--   0        0        0     2827 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_spelling.py
--rw-r--r--   0        0        0     1813 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_tabs.py
--rw-r--r--   0        0        0     6297 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_todo_tbd.py
--rw-r--r--   0        0        0     2398 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_trailing_spaces_tabs.py
--rw-r--r--   0        0        0     3868 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_using_display.py
--rw-r--r--   0        0        0    24134 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_valid_oid.py
--rw-r--r--   0        0        0     4154 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_valid_script_tag_names.py
--rw-r--r--   0        0        0     1947 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_vt_file_permissions.py
--rw-r--r--   0        0        0     5189 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/plugins/test_vt_placement.py
--rw-r--r--   0        0        0      716 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/__init__.py
--rw-r--r--   0        0        0      716 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/changed_packages/__init__.py
--rw-r--r--   0        0        0      716 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/__init__.py
--rw-r--r--   0        0        0     3075 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py
--rw-r--r--   0        0        0     2620 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/test_added_release.py
--rw-r--r--   0        0        0     1792 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py
--rw-r--r--   0        0        0     3258 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/test_changed_update.py
--rw-r--r--   0        0        0     3584 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py
--rw-r--r--   0        0        0     3780 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/changed_packages/test_changed_packages.py
--rw-r--r--   0        0        0     2427 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/changed_packages/test_package.py
--rw-r--r--   0        0        0     2977 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/test_changed_cves.py
--rw-r--r--   0        0        0     2952 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/test_changed_oid.py
--rw-r--r--   0        0        0     3962 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/test_last_modification.py
--rw-r--r--   0        0        0     7347 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/test_no_solution.py
--rw-r--r--   0        0        0     6293 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/standalone_plugins/test_version_updated.py
--rw-r--r--   0        0        0     4768 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/test_argparser.py
--rw-r--r--   0        0        0     3947 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/test_helper.py
--rw-r--r--   0        0        0     3671 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/test_naslinter.py
--rw-r--r--   0        0        0     3399 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/test_reporter.py
--rw-r--r--   0        0        0     2517 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/test_results.py
--rw-r--r--   0        0        0    17972 2023-07-10 08:28:45.950539 troubadix-23.7.0/tests/test_runner.py
--rw-r--r--   0        0        0      716 2023-07-10 08:28:45.950539 troubadix-23.7.0/troubadix/__init__.py
--rw-r--r--   0        0        0      103 2023-07-10 08:28:45.950539 troubadix-23.7.0/troubadix/__version__.py
--rw-r--r--   0        0        0     6999 2023-07-10 08:28:45.950539 troubadix-23.7.0/troubadix/argparser.py
--rw-r--r--   0        0        0      338 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/codespell/codespell.additions
--rw-r--r--   0        0        0   125216 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/codespell/codespell.exclude
--rw-r--r--   0        0        0      756 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/codespell/codespell.ignore
--rw-r--r--   0        0        0     1061 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/helper/__init__.py
--rw-r--r--   0        0        0     3105 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/helper/helper.py
--rw-r--r--   0        0        0     6811 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/helper/linguistic_exception_handler.py
--rw-r--r--   0        0        0     9370 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/helper/patterns.py
--rw-r--r--   0        0        0     3508 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugin.py
--rw-r--r--   0        0        0     7013 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/__init__.py
--rw-r--r--   0        0        0     4507 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/badwords.py
--rw-r--r--   0        0        0     3583 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/copyright_text.py
--rw-r--r--   0        0        0     3334 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/copyright_year.py
--rw-r--r--   0        0        0     3357 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/creation_date.py
--rw-r--r--   0        0        0     3400 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/cve_format.py
--rw-r--r--   0        0        0     2309 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/cvss_format.py
--rw-r--r--   0        0        0     4456 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/dependencies.py
--rw-r--r--   0        0        0     7316 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/dependency_category_order.py
--rw-r--r--   0        0        0     4137 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/deprecated_dependency.py
--rw-r--r--   0        0        0     2568 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/deprecated_functions.py
--rw-r--r--   0        0        0     2509 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/double_end_points.py
--rw-r--r--   0        0        0     2652 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/duplicate_oid.py
--rw-r--r--   0        0        0     3179 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/duplicated_script_tags.py
--rw-r--r--   0        0        0     2090 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/encoding.py
--rw-r--r--   0        0        0     6014 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/forking_nasl_functions.py
--rw-r--r--   0        0        0     3401 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/get_kb_on_services.py
--rw-r--r--   0        0        0     8566 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/grammar.py
--rw-r--r--   0        0        0     7157 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/http_links_in_tags.py
--rw-r--r--   0        0        0     4406 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/illegal_characters.py
--rw-r--r--   0        0        0     2960 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/log_messages.py
--rw-r--r--   0        0        0     3000 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/malformed_dependencies.py
--rw-r--r--   0        0        0     5330 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/misplaced_compare_in_if.py
--rw-r--r--   0        0        0     2411 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/missing_desc_exit.py
--rw-r--r--   0        0        0     2828 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/missing_tag_solution.py
--rw-r--r--   0        0        0     2788 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/newlines.py
--rw-r--r--   0        0        0     2373 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/overlong_script_tags.py
--rw-r--r--   0        0        0     4584 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/prod_svc_detect_in_vulnvt.py
--rw-r--r--   0        0        0     3790 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/qod.py
--rw-r--r--   0        0        0     4081 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/reporting_consistency.py
--rw-r--r--   0        0        0     3193 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_add_preference_type.py
--rw-r--r--   0        0        0     2512 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_calls_empty_values.py
--rw-r--r--   0        0        0     3137 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_calls_recommended.py
--rw-r--r--   0        0        0     2184 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_category.py
--rw-r--r--   0        0        0     2310 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_copyright.py
--rw-r--r--   0        0        0     4023 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_family.py
--rw-r--r--   0        0        0     1773 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_tag_form.py
--rw-r--r--   0        0        0     2172 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_tag_whitespaces.py
--rw-r--r--   0        0        0     2630 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_tags_mandatory.py
--rw-r--r--   0        0        0     7026 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_version_and_last_modification_tags.py
--rw-r--r--   0        0        0     1848 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_xref_form.py
--rw-r--r--   0        0        0     2875 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/script_xref_url.py
--rw-r--r--   0        0        0     4708 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/security_messages.py
--rw-r--r--   0        0        0     3415 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/set_get_kb_calls.py
--rw-r--r--   0        0        0     5852 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/solution_text.py
--rw-r--r--   0        0        0     2602 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/solution_type.py
--rw-r--r--   0        0        0     9557 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/spelling.py
--rw-r--r--   0        0        0     1319 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/tabs.py
--rw-r--r--   0        0        0     1733 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/todo_tbd.py
--rw-r--r--   0        0        0     2049 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/trailing_spaces_tabs.py
--rw-r--r--   0        0        0     4046 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/using_display.py
--rw-r--r--   0        0        0    16627 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/valid_oid.py
--rw-r--r--   0        0        0     3447 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/valid_script_tag_names.py
--rw-r--r--   0        0        0     3285 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/variable_assigned_in_if.py
--rw-r--r--   0        0        0     1521 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/vt_file_permissions.py
--rw-r--r--   0        0        0     2800 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/plugins/vt_placement.py
--rw-r--r--   0        0        0     9176 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/reporter.py
--rw-r--r--   0        0        0     2632 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/results.py
--rw-r--r--   0        0        0     5172 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/runner.py
--rw-r--r--   0        0        0       22 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/standalone_plugins/__init__.py
--rw-r--r--   0        0        0     4145 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/standalone_plugins/allowed_rev_diff.py
--rw-r--r--   0        0        0     2921 2023-07-10 08:28:45.954539 troubadix-23.7.0/troubadix/standalone_plugins/changed_cves.py
--rw-r--r--   0        0        0     4074 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/changed_oid.py
--rw-r--r--   0        0        0     5742 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/changed_packages.py
--rw-r--r--   0        0        0      923 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/__init__.py
--rw-r--r--   0        0        0     1797 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py
--rw-r--r--   0        0        0     1486 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/added_release.py
--rw-r--r--   0        0        0     1124 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py
--rw-r--r--   0        0        0     1952 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/changed_update.py
--rw-r--r--   0        0        0     1632 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py
--rw-r--r--   0        0        0     1278 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/marker.py
--rw-r--r--   0        0        0     2743 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/package.py
--rw-r--r--   0        0        0     1028 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/common.py
--rw-r--r--   0        0        0     4616 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/last_modification.py
--rw-r--r--   0        0        0     8463 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/no_solution.py
--rw-r--r--   0        0        0     4263 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/standalone_plugins/version_updated.py
--rw-r--r--   0        0        0     6045 2023-07-10 08:28:45.958539 troubadix-23.7.0/troubadix/troubadix.py
--rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 troubadix-23.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-13 14:53:02.430204 troubadix-23.7.1/LICENSE
+-rw-r--r--   0        0        0     2730 2023-07-13 14:53:02.430204 troubadix-23.7.1/README.md
+-rw-r--r--   0        0        0     2516 2023-07-13 14:53:02.434203 troubadix-23.7.1/pyproject.toml
+-rw-r--r--   0        0        0      716 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/__init__.py
+-rw-r--r--   0        0        0      716 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/helper/__init__.py
+-rw-r--r--   0        0        0     8416 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/helper/test_linguistic_exception_handler.py
+-rw-r--r--   0        0        0     1940 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/helper/test_patterns.py
+-rw-r--r--   0        0        0     2396 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/__init__.py
+-rw-r--r--   0        0        0     1012 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/fail.nasl
+-rw-r--r--   0        0        0     1291 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/fail2.nasl
+-rw-r--r--   0        0        0     2100 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test.nasl
+-rw-r--r--   0        0        0     2450 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_badwords.py
+-rw-r--r--   0        0        0     5109 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_copyright_text.py
+-rw-r--r--   0        0        0     6961 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_copyright_year.py
+-rw-r--r--   0        0        0     5004 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_creation_date.py
+-rw-r--r--   0        0        0     5881 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_cve_format.py
+-rw-r--r--   0        0        0     4914 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_cvss_format.py
+-rw-r--r--   0        0        0     8970 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_dependencies.py
+-rw-r--r--   0        0        0     5808 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_dependency_category_order.py
+-rw-r--r--   0        0        0     5589 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_deprecated_dependency.py
+-rw-r--r--   0        0        0     4545 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_deprecated_functions.py
+-rw-r--r--   0        0        0     2394 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_double_end_points.py
+-rw-r--r--   0        0        0     3504 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_duplicate_oid.py
+-rw-r--r--   0        0        0     4686 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_duplicated_script_tags.py
+-rw-r--r--   0        0        0     3906 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_encoding.py
+-rw-r--r--   0        0        0     1982 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_files/fail_bad_new_line.nasl
+-rw-r--r--   0        0        0      246 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_files/fail_badwords.nasl
+-rw-r--r--   0        0        0     1979 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_files/fail_name_and_copyright_newline.nasl
+-rw-r--r--   0        0        0     1965 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_files/fail_name_newline.nasl
+-rwxr-xr-x   0        0        0     1012 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_files/fail_permissions.nasl
+-rw-r--r--   0        0        0      150 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_files/fail_spelling.nasl
+-rw-r--r--   0        0        0     2213 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/fail.nasl
+-rw-r--r--   0        0        0      246 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/fail_badwords.nasl
+-rw-r--r--   0        0        0     1990 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl
+-rw-r--r--   0        0        0     1987 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl
+-rw-r--r--   0        0        0     2134 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl
+-rw-r--r--   0        0        0     1023 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/runner/fail.nasl
+-rw-r--r--   0        0        0     1302 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl
+-rw-r--r--   0        0        0     2122 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/runner/test.nasl
+-rw-r--r--   0        0        0     2119 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl
+-rw-r--r--   0        0        0     1023 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/test.inc
+-rw-r--r--   0        0        0     2122 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/test.nasl
+-rw-r--r--   0        0        0     2976 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_files/nasl/warning.nasl
+-rw-r--r--   0        0        0     1012 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_files/ok_permissions.nasl
+-rw-r--r--   0        0        0     2100 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_files/test_oid.nasl
+-rw-r--r--   0        0        0     4548 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_forking_nasl_functions.py
+-rw-r--r--   0        0        0     2271 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_get_kb_on_services.py
+-rw-r--r--   0        0        0     9438 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_grammar.py
+-rw-r--r--   0        0        0     6936 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_http_links_in_tags.py
+-rw-r--r--   0        0        0     4730 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_illegal_characters.py
+-rw-r--r--   0        0        0     5965 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_log_messages.py
+-rw-r--r--   0        0        0     6174 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_malformed_dependencies.py
+-rw-r--r--   0        0        0    21051 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_misplaced_compare_in_if.py
+-rw-r--r--   0        0        0     3585 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_missing_desc_exit.py
+-rw-r--r--   0        0        0     3101 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_missing_tag_solution.py
+-rw-r--r--   0        0        0     4688 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_newlines.py
+-rw-r--r--   0        0        0    40813 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_overlong_script_tags.py
+-rw-r--r--   0        0        0     4294 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_prod_svc_detect_in_vulnvt.py
+-rw-r--r--   0        0        0     4594 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_qod.py
+-rw-r--r--   0        0        0     5844 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_reporting_consistency.py
+-rw-r--r--   0        0        0     3371 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_script_add_preference_type.py
+-rw-r--r--   0        0        0     2353 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_script_calls_empty_values.py
+-rw-r--r--   0        0        0     2799 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_script_calls_recommended.py
+-rw-r--r--   0        0        0     2650 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_script_category.py
+-rw-r--r--   0        0        0     3469 2023-07-13 14:53:02.434203 troubadix-23.7.1/tests/plugins/test_script_copyright.py
+-rw-r--r--   0        0        0     3877 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/plugins/test_script_family.py
+-rw-r--r--   0        0        0     3079 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/plugins/test_script_tag_form.py
+-rw-r--r--   0        0        0     6010 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/plugins/test_script_tag_whitespaces.py
+-rw-r--r--   0        0        0     3313 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/plugins/test_script_tags_mandatory.py
+-rw-r--r--   0        0        0     4858 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/plugins/test_script_version_and_last_modification_tags.py
+-rw-r--r--   0        0        0     3016 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/plugins/test_script_xref_form.py
+-rw-r--r--   0        0        0     2189 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/plugins/test_script_xref_url.py
+-rw-r--r--   0        0        0     6599 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/plugins/test_security_messages.py
+-rw-r--r--   0        0        0     3021 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/plugins/test_set_get_kb_calls.py
+-rw-r--r--   0        0        0     7260 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/plugins/test_solution_text.py
+-rw-r--r--   0        0        0     3306 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/plugins/test_solution_type.py
+-rw-r--r--   0        0        0     2827 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/plugins/test_spelling.py
+-rw-r--r--   0        0        0     1813 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/plugins/test_tabs.py
+-rw-r--r--   0        0        0     6297 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/plugins/test_todo_tbd.py
+-rw-r--r--   0        0        0     2398 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/plugins/test_trailing_spaces_tabs.py
+-rw-r--r--   0        0        0     3868 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/plugins/test_using_display.py
+-rw-r--r--   0        0        0    24134 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/plugins/test_valid_oid.py
+-rw-r--r--   0        0        0     4154 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/plugins/test_valid_script_tag_names.py
+-rw-r--r--   0        0        0     1947 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/plugins/test_vt_file_permissions.py
+-rw-r--r--   0        0        0     5189 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/plugins/test_vt_placement.py
+-rw-r--r--   0        0        0      716 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/standalone_plugins/__init__.py
+-rw-r--r--   0        0        0      716 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/standalone_plugins/changed_packages/__init__.py
+-rw-r--r--   0        0        0      716 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/standalone_plugins/changed_packages/markers/__init__.py
+-rw-r--r--   0        0        0     3075 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py
+-rw-r--r--   0        0        0     2620 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/standalone_plugins/changed_packages/markers/test_added_release.py
+-rw-r--r--   0        0        0     1792 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py
+-rw-r--r--   0        0        0     3258 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/standalone_plugins/changed_packages/markers/test_changed_update.py
+-rw-r--r--   0        0        0     3584 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py
+-rw-r--r--   0        0        0     3780 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/standalone_plugins/changed_packages/test_changed_packages.py
+-rw-r--r--   0        0        0     2427 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/standalone_plugins/changed_packages/test_package.py
+-rw-r--r--   0        0        0     2977 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/standalone_plugins/test_changed_cves.py
+-rw-r--r--   0        0        0     2952 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/standalone_plugins/test_changed_oid.py
+-rw-r--r--   0        0        0     3962 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/standalone_plugins/test_last_modification.py
+-rw-r--r--   0        0        0     7347 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/standalone_plugins/test_no_solution.py
+-rw-r--r--   0        0        0     6293 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/standalone_plugins/test_version_updated.py
+-rw-r--r--   0        0        0     4768 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/test_argparser.py
+-rw-r--r--   0        0        0     3947 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/test_helper.py
+-rw-r--r--   0        0        0     3671 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/test_naslinter.py
+-rw-r--r--   0        0        0     3399 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/test_reporter.py
+-rw-r--r--   0        0        0     2517 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/test_results.py
+-rw-r--r--   0        0        0    17972 2023-07-13 14:53:02.438204 troubadix-23.7.1/tests/test_runner.py
+-rw-r--r--   0        0        0      716 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/__init__.py
+-rw-r--r--   0        0        0      103 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/__version__.py
+-rw-r--r--   0        0        0     6999 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/argparser.py
+-rw-r--r--   0        0        0      338 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/codespell/codespell.additions
+-rw-r--r--   0        0        0   125981 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/codespell/codespell.exclude
+-rw-r--r--   0        0        0      756 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/codespell/codespell.ignore
+-rw-r--r--   0        0        0     1061 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/helper/__init__.py
+-rw-r--r--   0        0        0     3105 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/helper/helper.py
+-rw-r--r--   0        0        0     6811 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/helper/linguistic_exception_handler.py
+-rw-r--r--   0        0        0     9370 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/helper/patterns.py
+-rw-r--r--   0        0        0     3508 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/plugin.py
+-rw-r--r--   0        0        0     7013 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/plugins/__init__.py
+-rw-r--r--   0        0        0     4507 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/plugins/badwords.py
+-rw-r--r--   0        0        0     3583 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/plugins/copyright_text.py
+-rw-r--r--   0        0        0     3334 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/plugins/copyright_year.py
+-rw-r--r--   0        0        0     3357 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/plugins/creation_date.py
+-rw-r--r--   0        0        0     3400 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/plugins/cve_format.py
+-rw-r--r--   0        0        0     2309 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/plugins/cvss_format.py
+-rw-r--r--   0        0        0     4456 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/plugins/dependencies.py
+-rw-r--r--   0        0        0     7316 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/plugins/dependency_category_order.py
+-rw-r--r--   0        0        0     4137 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/plugins/deprecated_dependency.py
+-rw-r--r--   0        0        0     2568 2023-07-13 14:53:02.438204 troubadix-23.7.1/troubadix/plugins/deprecated_functions.py
+-rw-r--r--   0        0        0     2509 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/double_end_points.py
+-rw-r--r--   0        0        0     2652 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/duplicate_oid.py
+-rw-r--r--   0        0        0     3179 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/duplicated_script_tags.py
+-rw-r--r--   0        0        0     2090 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/encoding.py
+-rw-r--r--   0        0        0     6014 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/forking_nasl_functions.py
+-rw-r--r--   0        0        0     3401 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/get_kb_on_services.py
+-rw-r--r--   0        0        0     8566 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/grammar.py
+-rw-r--r--   0        0        0     7157 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/http_links_in_tags.py
+-rw-r--r--   0        0        0     4406 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/illegal_characters.py
+-rw-r--r--   0        0        0     2960 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/log_messages.py
+-rw-r--r--   0        0        0     3000 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/malformed_dependencies.py
+-rw-r--r--   0        0        0     5330 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/misplaced_compare_in_if.py
+-rw-r--r--   0        0        0     2411 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/missing_desc_exit.py
+-rw-r--r--   0        0        0     2828 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/missing_tag_solution.py
+-rw-r--r--   0        0        0     2788 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/newlines.py
+-rw-r--r--   0        0        0     2373 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/overlong_script_tags.py
+-rw-r--r--   0        0        0     4584 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/prod_svc_detect_in_vulnvt.py
+-rw-r--r--   0        0        0     3816 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/qod.py
+-rw-r--r--   0        0        0     4081 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/reporting_consistency.py
+-rw-r--r--   0        0        0     3193 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/script_add_preference_type.py
+-rw-r--r--   0        0        0     2512 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/script_calls_empty_values.py
+-rw-r--r--   0        0        0     3137 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/script_calls_recommended.py
+-rw-r--r--   0        0        0     2184 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/script_category.py
+-rw-r--r--   0        0        0     2310 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/script_copyright.py
+-rw-r--r--   0        0        0     4023 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/script_family.py
+-rw-r--r--   0        0        0     1773 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/script_tag_form.py
+-rw-r--r--   0        0        0     2172 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/script_tag_whitespaces.py
+-rw-r--r--   0        0        0     2630 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/script_tags_mandatory.py
+-rw-r--r--   0        0        0     7026 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/script_version_and_last_modification_tags.py
+-rw-r--r--   0        0        0     1848 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/script_xref_form.py
+-rw-r--r--   0        0        0     2875 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/script_xref_url.py
+-rw-r--r--   0        0        0     4708 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/security_messages.py
+-rw-r--r--   0        0        0     3415 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/set_get_kb_calls.py
+-rw-r--r--   0        0        0     5852 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/solution_text.py
+-rw-r--r--   0        0        0     2602 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/solution_type.py
+-rw-r--r--   0        0        0     9557 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/spelling.py
+-rw-r--r--   0        0        0     1319 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/tabs.py
+-rw-r--r--   0        0        0     1733 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/todo_tbd.py
+-rw-r--r--   0        0        0     2049 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/trailing_spaces_tabs.py
+-rw-r--r--   0        0        0     4046 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/using_display.py
+-rw-r--r--   0        0        0    16627 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/valid_oid.py
+-rw-r--r--   0        0        0     3447 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/valid_script_tag_names.py
+-rw-r--r--   0        0        0     3285 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/variable_assigned_in_if.py
+-rw-r--r--   0        0        0     1521 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/vt_file_permissions.py
+-rw-r--r--   0        0        0     2800 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/plugins/vt_placement.py
+-rw-r--r--   0        0        0     9176 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/reporter.py
+-rw-r--r--   0        0        0     2632 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/results.py
+-rw-r--r--   0        0        0     5172 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/runner.py
+-rw-r--r--   0        0        0       22 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/standalone_plugins/__init__.py
+-rw-r--r--   0        0        0     4145 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/standalone_plugins/allowed_rev_diff.py
+-rw-r--r--   0        0        0     2921 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/standalone_plugins/changed_cves.py
+-rw-r--r--   0        0        0     4074 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/standalone_plugins/changed_oid.py
+-rw-r--r--   0        0        0     5742 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/standalone_plugins/changed_packages/changed_packages.py
+-rw-r--r--   0        0        0      923 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/standalone_plugins/changed_packages/marker/__init__.py
+-rw-r--r--   0        0        0     1797 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py
+-rw-r--r--   0        0        0     1486 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/standalone_plugins/changed_packages/marker/added_release.py
+-rw-r--r--   0        0        0     1124 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py
+-rw-r--r--   0        0        0     1952 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/standalone_plugins/changed_packages/marker/changed_update.py
+-rw-r--r--   0        0        0     1632 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py
+-rw-r--r--   0        0        0     1278 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/standalone_plugins/changed_packages/marker/marker.py
+-rw-r--r--   0        0        0     2743 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/standalone_plugins/changed_packages/package.py
+-rw-r--r--   0        0        0     1028 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/standalone_plugins/common.py
+-rw-r--r--   0        0        0     4616 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/standalone_plugins/last_modification.py
+-rw-r--r--   0        0        0     8463 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/standalone_plugins/no_solution.py
+-rw-r--r--   0        0        0     4263 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/standalone_plugins/version_updated.py
+-rw-r--r--   0        0        0     6045 2023-07-13 14:53:02.442204 troubadix-23.7.1/troubadix/troubadix.py
+-rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 troubadix-23.7.1/PKG-INFO
```

### Comparing `troubadix-23.7.0/LICENSE` & `troubadix-23.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/README.md` & `troubadix-23.7.1/README.md`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/pyproject.toml` & `troubadix-23.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troubadix"
-version = "23.7.0"
+version = "23.7.1"
 description = "A linting and QA check tool for NASL files"
 authors = ["Greenbone <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/greenbone/troubadix"
 homepage = "https://github.com/greenbone/troubadix"
```

### Comparing `troubadix-23.7.0/tests/__init__.py` & `troubadix-23.7.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/helper/__init__.py` & `troubadix-23.7.1/tests/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/helper/test_linguistic_exception_handler.py` & `troubadix-23.7.1/tests/helper/test_linguistic_exception_handler.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/helper/test_patterns.py` & `troubadix-23.7.1/tests/helper/test_patterns.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/__init__.py` & `troubadix-23.7.1/tests/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/fail.nasl` & `troubadix-23.7.1/tests/plugins/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/fail2.nasl` & `troubadix-23.7.1/tests/plugins/fail2.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test.nasl` & `troubadix-23.7.1/tests/plugins/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_badwords.py` & `troubadix-23.7.1/tests/plugins/test_badwords.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_copyright_text.py` & `troubadix-23.7.1/tests/plugins/test_copyright_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_copyright_year.py` & `troubadix-23.7.1/tests/plugins/test_copyright_year.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_creation_date.py` & `troubadix-23.7.1/tests/plugins/test_creation_date.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_cve_format.py` & `troubadix-23.7.1/tests/plugins/test_cve_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_cvss_format.py` & `troubadix-23.7.1/tests/plugins/test_cvss_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_dependencies.py` & `troubadix-23.7.1/tests/plugins/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_dependency_category_order.py` & `troubadix-23.7.1/tests/plugins/test_dependency_category_order.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_deprecated_dependency.py` & `troubadix-23.7.1/tests/plugins/test_deprecated_dependency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_deprecated_functions.py` & `troubadix-23.7.1/tests/plugins/test_deprecated_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_double_end_points.py` & `troubadix-23.7.1/tests/plugins/test_double_end_points.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_duplicate_oid.py` & `troubadix-23.7.1/tests/plugins/test_duplicate_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_duplicated_script_tags.py` & `troubadix-23.7.1/tests/plugins/test_duplicated_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_encoding.py` & `troubadix-23.7.1/tests/plugins/test_encoding.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_files/fail_bad_new_line.nasl` & `troubadix-23.7.1/tests/plugins/test_files/fail_bad_new_line.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_files/fail_name_and_copyright_newline.nasl` & `troubadix-23.7.1/tests/plugins/test_files/fail_name_and_copyright_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_files/fail_name_newline.nasl` & `troubadix-23.7.1/tests/plugins/test_files/fail_name_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_files/fail_permissions.nasl` & `troubadix-23.7.1/tests/plugins/test_files/fail_permissions.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/fail.nasl` & `troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl` & `troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl` & `troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl` & `troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/runner/fail.nasl` & `troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/runner/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl` & `troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/runner/test.nasl` & `troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/runner/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl` & `troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/test.inc` & `troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/test.inc`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_files/nasl/21.04/test.nasl` & `troubadix-23.7.1/tests/plugins/test_files/nasl/21.04/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_files/nasl/warning.nasl` & `troubadix-23.7.1/tests/plugins/test_files/nasl/warning.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_files/ok_permissions.nasl` & `troubadix-23.7.1/tests/plugins/test_files/ok_permissions.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_files/test_oid.nasl` & `troubadix-23.7.1/tests/plugins/test_files/test_oid.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_forking_nasl_functions.py` & `troubadix-23.7.1/tests/plugins/test_forking_nasl_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_get_kb_on_services.py` & `troubadix-23.7.1/tests/plugins/test_get_kb_on_services.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_grammar.py` & `troubadix-23.7.1/tests/plugins/test_grammar.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_http_links_in_tags.py` & `troubadix-23.7.1/tests/plugins/test_http_links_in_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_illegal_characters.py` & `troubadix-23.7.1/tests/plugins/test_illegal_characters.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_log_messages.py` & `troubadix-23.7.1/tests/plugins/test_log_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_malformed_dependencies.py` & `troubadix-23.7.1/tests/plugins/test_malformed_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_misplaced_compare_in_if.py` & `troubadix-23.7.1/tests/plugins/test_misplaced_compare_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_missing_desc_exit.py` & `troubadix-23.7.1/tests/plugins/test_missing_desc_exit.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_missing_tag_solution.py` & `troubadix-23.7.1/tests/plugins/test_missing_tag_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_newlines.py` & `troubadix-23.7.1/tests/plugins/test_newlines.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_overlong_script_tags.py` & `troubadix-23.7.1/tests/plugins/test_overlong_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_prod_svc_detect_in_vulnvt.py` & `troubadix-23.7.1/tests/plugins/test_prod_svc_detect_in_vulnvt.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_qod.py` & `troubadix-23.7.1/tests/plugins/test_qod.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_reporting_consistency.py` & `troubadix-23.7.1/tests/plugins/test_reporting_consistency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_script_add_preference_type.py` & `troubadix-23.7.1/tests/plugins/test_script_add_preference_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_script_calls_empty_values.py` & `troubadix-23.7.1/tests/plugins/test_script_calls_empty_values.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_script_calls_recommended.py` & `troubadix-23.7.1/tests/plugins/test_script_calls_recommended.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_script_category.py` & `troubadix-23.7.1/tests/plugins/test_script_category.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_script_copyright.py` & `troubadix-23.7.1/tests/plugins/test_script_copyright.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_script_family.py` & `troubadix-23.7.1/tests/plugins/test_script_family.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_script_tag_form.py` & `troubadix-23.7.1/tests/plugins/test_script_tag_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_script_tag_whitespaces.py` & `troubadix-23.7.1/tests/plugins/test_script_tag_whitespaces.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_script_tags_mandatory.py` & `troubadix-23.7.1/tests/plugins/test_script_tags_mandatory.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_script_version_and_last_modification_tags.py` & `troubadix-23.7.1/tests/plugins/test_script_version_and_last_modification_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_script_xref_form.py` & `troubadix-23.7.1/tests/plugins/test_script_xref_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_script_xref_url.py` & `troubadix-23.7.1/tests/plugins/test_script_xref_url.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_security_messages.py` & `troubadix-23.7.1/tests/plugins/test_security_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_set_get_kb_calls.py` & `troubadix-23.7.1/tests/plugins/test_set_get_kb_calls.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_solution_text.py` & `troubadix-23.7.1/tests/plugins/test_solution_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_solution_type.py` & `troubadix-23.7.1/tests/plugins/test_solution_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_spelling.py` & `troubadix-23.7.1/tests/plugins/test_spelling.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_tabs.py` & `troubadix-23.7.1/tests/plugins/test_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_todo_tbd.py` & `troubadix-23.7.1/tests/plugins/test_todo_tbd.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_trailing_spaces_tabs.py` & `troubadix-23.7.1/tests/plugins/test_trailing_spaces_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_using_display.py` & `troubadix-23.7.1/tests/plugins/test_using_display.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_valid_oid.py` & `troubadix-23.7.1/tests/plugins/test_valid_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_valid_script_tag_names.py` & `troubadix-23.7.1/tests/plugins/test_valid_script_tag_names.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_vt_file_permissions.py` & `troubadix-23.7.1/tests/plugins/test_vt_file_permissions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/plugins/test_vt_placement.py` & `troubadix-23.7.1/tests/plugins/test_vt_placement.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/standalone_plugins/__init__.py` & `troubadix-23.7.1/tests/standalone_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/standalone_plugins/changed_packages/__init__.py` & `troubadix-23.7.1/tests/standalone_plugins/changed_packages/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/__init__.py` & `troubadix-23.7.1/tests/standalone_plugins/changed_packages/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py` & `troubadix-23.7.1/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/test_added_release.py` & `troubadix-23.7.1/tests/standalone_plugins/changed_packages/markers/test_added_release.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py` & `troubadix-23.7.1/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/test_changed_update.py` & `troubadix-23.7.1/tests/standalone_plugins/changed_packages/markers/test_changed_update.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py` & `troubadix-23.7.1/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/standalone_plugins/changed_packages/test_changed_packages.py` & `troubadix-23.7.1/tests/standalone_plugins/changed_packages/test_changed_packages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/standalone_plugins/changed_packages/test_package.py` & `troubadix-23.7.1/tests/standalone_plugins/changed_packages/test_package.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/standalone_plugins/test_changed_cves.py` & `troubadix-23.7.1/tests/standalone_plugins/test_changed_cves.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/standalone_plugins/test_changed_oid.py` & `troubadix-23.7.1/tests/standalone_plugins/test_changed_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/standalone_plugins/test_last_modification.py` & `troubadix-23.7.1/tests/standalone_plugins/test_last_modification.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/standalone_plugins/test_no_solution.py` & `troubadix-23.7.1/tests/standalone_plugins/test_no_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/standalone_plugins/test_version_updated.py` & `troubadix-23.7.1/tests/standalone_plugins/test_version_updated.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/test_argparser.py` & `troubadix-23.7.1/tests/test_argparser.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/test_helper.py` & `troubadix-23.7.1/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/test_naslinter.py` & `troubadix-23.7.1/tests/test_naslinter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/test_reporter.py` & `troubadix-23.7.1/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/test_results.py` & `troubadix-23.7.1/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/tests/test_runner.py` & `troubadix-23.7.1/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/__init__.py` & `troubadix-23.7.1/troubadix/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/argparser.py` & `troubadix-23.7.1/troubadix/argparser.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/codespell/codespell.exclude` & `troubadix-23.7.1/troubadix/codespell/codespell.exclude`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,15 @@
         check_matches = re.finditer('[^\r\n]*[#]+[ ]*([Tt]hunderbird|[Ss]ea[Mm]onkey|[Hh]ot[Ff]ix|[Ff]irefox|[Pp]ower[Pp]oint( Viewer)?)[ ]*[Cc]heck[^\r\n]*\n', text)
 China_Internet_Network_Information_Center_EV_Certificates_Ro ot:2.4.72.159.0.1.crt (server auth)
 China_Internet_Network_Information_Center_EV_Certificates_Ro ot:2.4.72.159.0.1.crt server auth
 Christian Loos discovered an information disclosure flaw which may reveal RSS feeds URLs, and thus ticket data.
 Christian Loos discovered a remote denial of service vulnerability, exploitable via the email gateway and affecting any installation which accepts mail from untrusted sources. Depending on RT's logging configuration, a remote attacker can take advantage of this flaw to cause CPU and excessive disk usage.
 chunks in CAF audio files. If a user or automated system were tricked into
   Cisco ACI Multi-Site Orchestrator (MSO) to send a specific API request to a managed Cisco APIC or
+# Cisco Network Analysis Module (NAM)
 # Cisco TelePresence TC and TE Software Multiple Security Vulnerabilities
 Claus Jorgensen reported that a text input box can be pre-filled with a filename and then turned into a file-upload control, allowing a malicious website to steal any local file whose name they can guess. [MFSA-2006-23]
 Claus Wahlers reported that random images from GPU memory
   Clemens Huebner and Kevin Stange discovered that Pidgin incorrectly handled
                clen +
   clen = "567";
   clen = data_len( data:_ciphers );
@@ -337,14 +338,15 @@
   family_id = 'oval:org.mitre.oval:obj:99';
   family_xml = '\t\t<family_item xmlns="http://oval.mitre.org/XMLSchema/oval-sys' +
 (FATE#312793, bnc#782369). The userland utilities were published seperately to support this feature.
 (FATE#313309) The ipset userland utility will be published seperately to support this feature.
 (FATE#314441). A seperate hyper-v package will be published to support this feature.
   feature for Cisco Nexus 9000 Series Fabric Switches in Application Centric Infrastructure (ACI)
   feature is available to ensure that nobody can gain remote access to the modem (via the WAN/DSL interface).
+  feature of Cisco Nexus 9000 Series Fabric Switches in ACI mode could allow an unauthenticated,
 # Fedora Update for tre FEDORA-2016-0a952a3bc0
 # Fedora Update for tre FEDORA-2016-0ff6c3d84b
 # Fedora Update for tre FEDORA-2016-cd09eab674
 files. If a user were tricked into opening a specially-crafted CAF file, a
   files to potentially execute code and it is tracked by the Mitre CVE
   file_xml = '\t\t<file_item' + status + ' xmlns="http://oval.mitre.org/XMLSchema/' +
 Fixed a bug where Podman could not run containers usin... [Please see the references for more information on the vulnerabilities]");
@@ -782,14 +784,15 @@
   script_name("Cisco Nexus 9000 Series ACI Mode Switch Software Link Layer Discovery Protocol Buffer Overflow Vulnerability (cisco-sa-20190731-nxos-bo)");
   script_name("Cisco Nexus 9000 Series Fabric Switches ACI Mode Arbitrary File Read Vulnerability (cisco-sa-naci-afr-UtjfO2D7)");
   script_name("Cisco Nexus 9000 Series Fabric Switches ACI Mode Border Leaf Endpoint Learning Vulnerability (cisco-sa-20190828-nexus-aci-dos)");
   script_name("Cisco Nexus 9000 Series Fabric Switches ACI Mode Fabric Infrastructure VLAN Unauthorized Access Vulnerability (cisco-sa-20190703-n9kaci-bypass)");
   script_name("Cisco Nexus 9000 Series Fabric Switches ACI Mode Multi-Pod and Multi-Site TCP DoS Vulnerability (cisco-sa-n9kaci-tcp-dos-YXukt6gM)");
   script_name("Cisco Nexus 9000 Series Fabric Switches ACI Mode Privilege Escalation Vulnerability (cisco-sa-naci-mdvul-vrKVgNU)");
   script_name("Cisco Nexus 9000 Series Fabric Switches ACI Mode Queue Wedge DoS Vulnerability (cisco-sa-n9kaci-queue-wedge-cLDDEfKF)");
+  script_name("Cisco Nexus 9000 Series Fabric Switches ACI Multi-Site CloudSec Encryption Information Disclosure Vulnerability (cisco-sa-aci-cloudsec-enc-Vs5Wn2sX)");
   script_name("Cisco Nexus 9000 Series Fabric Switches in ACI Mode Link Layer Discovery Protocol Memory Leak Denial of Service Vulnerability (cisco-sa-aci-lldp-dos-ySCNZOpX)");
   script_name("Cisco RV340, RV340W, RV345, and RV345P Dual WAN Gigabit VPN Routers Authenticated Remote Code Execution Vulnerabilities (cisco-sa-sb-rv34x-rce-8bfG2h6b)");
   script_name("Cisco RV340, RV340W, RV345, and RV345P Dual WAN Gigabit VPN Routers Local Privilege Escalation Vulnerability (cisco-sa-rv-34x-privesc-GLN8ZAQE)");
   script_name("Cisco RV340, RV340W, RV345, and RV345P Dual WAN Gigabit VPN Routers SSL Denial of Service Vulnerability");
   script_name("Cisco RV340, RV340W, RV345, and RV345P Dual WAN Gigabit VPN Routers SSL Remote Code Execution and Denial of Service Vulnerability");
   script_name("Cisco RV340, RV340W, RV345, and RV345P Dual WAN Gigabit VPN Routers Web Management Vulnerabilities (cisco-sa-rv340-cmdinj-rcedos-pY8J3qfy)");
   script_name("Cisco TelePresence TC and TE Software Multiple Security Vulnerabilities");
@@ -920,14 +923,15 @@
   script_tag(name:"insight", value:"When UPnP services and WAN http administrative access are enabled,
   script_tag(name:"solution", value:"All FreeS/WAN 1.9x users should upgrade to the latest stable version:
   script_tag(name:"solution", value:"Ask the vendor for an update. Ensure remote WAN management is disabled on the affected devices.
   script_tag(name:"solution", value:"Please take the time to visit cve.mitre.org and check the
   script_tag(name:"solution", value:"Since LSAT is not actively maintained anymore, this package has been
   script_tag(name:"solution", value:"Upgrade to Apple Mac OS X Big Sur version
   script_tag(name:"summary", value:"A security vulnerability in Avenger's News System (ANS) allows
+  script_tag(name:"summary", value:"A vulnerability in the Cisco ACI Multi-Site CloudSec encryption
   script_tag(name:"summary", value:"A vulnerability in the IPv6 neighbor discovery (ND) handling of Cisco IOS XE Software on
   script_tag(name:"summary", value:"A vulnerability in the Network Access Manager (NAM) module of
   script_tag(name:"summary", value:"Cisco TelePresence TC and TE Software are prone to multiple
   script_tag(name:"summary", value:"Juraj Somorovsky, Robert Merget and Nimrod Aviram discovered a padding
   script_tag(name:"summary", value:"Listet alle erfuellten Tests der 'AKIF Orientierungshilfe Windows 10 Ueberpruefung' auf.");
   script_tag(name:"summary", value:"Listet alle Fehler der 'AKIF Orientierungshilfe Windows 10 Uberpruefung' auf.");
   script_tag(name:"summary", value:"Listet alle nicht erfuellten Tests der 'AKIF Orientierungshilfe Windows 10 Ueberpruefung' auf.");
@@ -1088,14 +1092,15 @@
 - SUNRPC: Fix READ_PLUS crasher (Chuck Lever)
 supply input to this crate, they could have caused a denial of service in the
   supporting the Apache JServ Protocol (AJP) accessible from a public WAN (Internet) / public LAN.");
  support was already present, but it was not enforcable).");
 support was enhanced and fixed, support for HDA sound on Acer Aspire
 # Swarmpit Web UI Public WAN (Internet) Accessible
   Switches for Application Centric Infrastructure (ACI) could allow an unauthenticated, adjacent
+  Switches in ACI mode that are running releases 14.0 and later if they are part of a Multi-Site
 Switches in Application-Centric Infrastructure (ACI) Mode could allow an unauthenticated, remote attacker to cause
 syntax. As a consequence, removing an ACI failed with a syntax error.
   system_root_id = 'oval:org.mitre.oval:obj:219';
 systems with HDA sound needing MSI support were added to the quirks
 	tags. Also removed references to cve.mitre.org. This
 take priviliges into account for the connecting user,
       "TANQ PRODUTO" >< res || "TANK PRODUKT" >< res || "REC 90" >< res ||
@@ -1201,14 +1206,15 @@
  * Tolerating bad MIME headers in ANS.1 parser.
   to or through a WAN interface of an affected device.");
 to the buildd network are needed (to provide the new Rust-based toolchain
   to the router from the WAN IP address.");
  to use of unitialized use of memory (bsc#1133037).
   TP3106, USG9500, VP9660, ViewPoint 8660, ViewPoint 9030, eCNS210_TD and eSpace U1981.");
  transfered in cleartext (bsc#1158440).");
+  transit between sites on current ACI Spine Switches hardware.");
 - Transport of TE related metrics over OSPF, IS-IS.
 triggerD = raw_string(0x06,0x00,0x07,0x00,0x20,0x00,0x00,0x00,0x0e,0x00,0x32,
 Tuomas Haanpaa and Matti Kamunen from Synopsys Ltd discovered that the NFSv2 and NFSv3 server implementations are vulnerable to an out-of-bounds memory access issue while processing arbitrarily long arguments sent by NFSv2/NFSv3 PRC clients, leading to a denial of service.
 two intermediate CAs which could be used to generate rogue end-entity
 udev: Downgrade message when settting inotify watch up fails.
  unconstrained interal data buffering (bsc#1145575).
  unconstrained interal data buffering (bsc#1146097).
@@ -1265,14 +1271,15 @@
   vers = ssh_get_bin_version(full_prog_name:file, version_argv:"--version", ver_pattern:"Kerberos 5 [Rr]elease ([0-9.]+)", sock:sock);
  + vfs_recycle: Prevent flooding the log if we're called on non-existant
     vgx_file_id = 'oval:org.mitre.oval:obj:308';
     vgx_file_variable_id = 'oval:org.mitre.oval:var:209';
 via crafted description chunks in a CAF audio file, leading to a
   vulnerability by flooding an adjacent IOS XE device with specific ND messages.");
   vulnerability by sending crafted IPv6 Neighbor Discovery (ND) packets to an affected device for
+  vulnerability that is described in this advisory. Customers who are using the Cisco ACI Multi-Site
 vuln_url = "/olt/Login.do/../../olt/UploadFileUpload.do";
 # WAN Emulator Remote Command Execution Vulnerabilities
        && '">WAN IP<' >< res && '">LAN IP<' >< res ) {
     # WAN Miniport (IPv6)|5|(null)|(null)
 Wan-Teh Chang as the original reporters of CVE-2013-5607.
   web-based interface for Cisco Small Business RV320 and RV325 Dual Gigabit WAN VPN Routers could
   webcontent/aas/aas_store.jsp.");
@@ -1302,14 +1309,15 @@
   which ultimately allows for overwriting Structured Exception Handler (SEH) addresses and the
   Wide Area Network (WAN) Settings and 'addURLFilter', 'addHostFilter'
 will execute user defined network requests to both WAN and LAN clients. A remote unauthenticated attacker can use
     win32k_file_id = 'oval:org.mitre.oval:obj:570';
     win32k_file_variable_id = 'oval:org.mitre.oval:var:200';
     winsrv_file_id = 'oval:org.mitre.oval:obj:1382';
     winsrv_file_variable_id = 'oval:org.mitre.oval:var:200';
+  with an on-path position between the ACI sites could exploit this vulnerability by intercepting
   withheld from the requestor.");
 With this update, the ACI check is stopped when the ACI is going to be
 "/wls-wsat/CoordinatorPortType11", "weblogic\.wsee\.wstx\.wsat\.v1[01]\.endpoint\.CoordinatorPort",
 "/wls-wsat/CoordinatorPortType", "weblogic\.wsee\.wstx\.wsat\.v1[01]\.endpoint\.CoordinatorPort",
 "/wls-wsat/ParticipantPortType11", "weblogic\.wsee\.wstx\.wsat\.v1[01]\.endpoint\.ParticipantPort",
 "/wls-wsat/ParticipantPortType", "weblogic\.wsee\.wstx\.wsat\.v1[01]\.endpoint\.ParticipantPort",
 "/wls-wsat/RegistrationPortTypeRPC11", "weblogic\.wsee\.wstx\.wsc\.v1[01]\.endpoint\.RegistrationPort");
```

### Comparing `troubadix-23.7.0/troubadix/codespell/codespell.ignore` & `troubadix-23.7.1/troubadix/codespell/codespell.ignore`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/helper/__init__.py` & `troubadix-23.7.1/troubadix/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/helper/helper.py` & `troubadix-23.7.1/troubadix/helper/helper.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/helper/linguistic_exception_handler.py` & `troubadix-23.7.1/troubadix/helper/linguistic_exception_handler.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/helper/patterns.py` & `troubadix-23.7.1/troubadix/helper/patterns.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugin.py` & `troubadix-23.7.1/troubadix/plugin.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/__init__.py` & `troubadix-23.7.1/troubadix/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/badwords.py` & `troubadix-23.7.1/troubadix/plugins/badwords.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/copyright_text.py` & `troubadix-23.7.1/troubadix/plugins/copyright_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/copyright_year.py` & `troubadix-23.7.1/troubadix/plugins/copyright_year.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/creation_date.py` & `troubadix-23.7.1/troubadix/plugins/creation_date.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/cve_format.py` & `troubadix-23.7.1/troubadix/plugins/cve_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/cvss_format.py` & `troubadix-23.7.1/troubadix/plugins/cvss_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/dependencies.py` & `troubadix-23.7.1/troubadix/plugins/dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/dependency_category_order.py` & `troubadix-23.7.1/troubadix/plugins/dependency_category_order.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/deprecated_dependency.py` & `troubadix-23.7.1/troubadix/plugins/deprecated_dependency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/deprecated_functions.py` & `troubadix-23.7.1/troubadix/plugins/deprecated_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/double_end_points.py` & `troubadix-23.7.1/troubadix/plugins/double_end_points.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/duplicate_oid.py` & `troubadix-23.7.1/troubadix/plugins/duplicate_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/duplicated_script_tags.py` & `troubadix-23.7.1/troubadix/plugins/duplicated_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/encoding.py` & `troubadix-23.7.1/troubadix/plugins/encoding.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/forking_nasl_functions.py` & `troubadix-23.7.1/troubadix/plugins/forking_nasl_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/get_kb_on_services.py` & `troubadix-23.7.1/troubadix/plugins/get_kb_on_services.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/grammar.py` & `troubadix-23.7.1/troubadix/plugins/grammar.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/http_links_in_tags.py` & `troubadix-23.7.1/troubadix/plugins/http_links_in_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/illegal_characters.py` & `troubadix-23.7.1/troubadix/plugins/illegal_characters.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/log_messages.py` & `troubadix-23.7.1/troubadix/plugins/log_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/malformed_dependencies.py` & `troubadix-23.7.1/troubadix/plugins/malformed_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/misplaced_compare_in_if.py` & `troubadix-23.7.1/troubadix/plugins/misplaced_compare_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/missing_desc_exit.py` & `troubadix-23.7.1/troubadix/plugins/missing_desc_exit.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/missing_tag_solution.py` & `troubadix-23.7.1/troubadix/plugins/missing_tag_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/newlines.py` & `troubadix-23.7.1/troubadix/plugins/newlines.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/overlong_script_tags.py` & `troubadix-23.7.1/troubadix/plugins/overlong_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/prod_svc_detect_in_vulnvt.py` & `troubadix-23.7.1/troubadix/plugins/prod_svc_detect_in_vulnvt.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/qod.py` & `troubadix-23.7.1/troubadix/plugins/qod.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     "remote_banner",
     "executable_version",
     "remote_analysis",
     "remote_probe",
     "remote_banner_unreliable",
     "executable_version_unreliable",
     "general_note",
+    "package_unreliable",
 ]
 
 
 class CheckQod(FilePlugin):
     name = "check_qod"
 
     def run(self) -> Iterator[LinterResult]:
```

### Comparing `troubadix-23.7.0/troubadix/plugins/reporting_consistency.py` & `troubadix-23.7.1/troubadix/plugins/reporting_consistency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/script_add_preference_type.py` & `troubadix-23.7.1/troubadix/plugins/script_add_preference_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/script_calls_empty_values.py` & `troubadix-23.7.1/troubadix/plugins/script_calls_empty_values.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/script_calls_recommended.py` & `troubadix-23.7.1/troubadix/plugins/script_calls_recommended.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/script_category.py` & `troubadix-23.7.1/troubadix/plugins/script_category.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/script_copyright.py` & `troubadix-23.7.1/troubadix/plugins/script_copyright.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/script_family.py` & `troubadix-23.7.1/troubadix/plugins/script_family.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/script_tag_form.py` & `troubadix-23.7.1/troubadix/plugins/script_tag_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/script_tag_whitespaces.py` & `troubadix-23.7.1/troubadix/plugins/script_tag_whitespaces.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/script_tags_mandatory.py` & `troubadix-23.7.1/troubadix/plugins/script_tags_mandatory.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/script_version_and_last_modification_tags.py` & `troubadix-23.7.1/troubadix/plugins/script_version_and_last_modification_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/script_xref_form.py` & `troubadix-23.7.1/troubadix/plugins/script_xref_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/script_xref_url.py` & `troubadix-23.7.1/troubadix/plugins/script_xref_url.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/security_messages.py` & `troubadix-23.7.1/troubadix/plugins/security_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/set_get_kb_calls.py` & `troubadix-23.7.1/troubadix/plugins/set_get_kb_calls.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/solution_text.py` & `troubadix-23.7.1/troubadix/plugins/solution_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/solution_type.py` & `troubadix-23.7.1/troubadix/plugins/solution_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/spelling.py` & `troubadix-23.7.1/troubadix/plugins/spelling.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/tabs.py` & `troubadix-23.7.1/troubadix/plugins/tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/todo_tbd.py` & `troubadix-23.7.1/troubadix/plugins/todo_tbd.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/trailing_spaces_tabs.py` & `troubadix-23.7.1/troubadix/plugins/trailing_spaces_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/using_display.py` & `troubadix-23.7.1/troubadix/plugins/using_display.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/valid_oid.py` & `troubadix-23.7.1/troubadix/plugins/valid_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/valid_script_tag_names.py` & `troubadix-23.7.1/troubadix/plugins/valid_script_tag_names.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/variable_assigned_in_if.py` & `troubadix-23.7.1/troubadix/plugins/variable_assigned_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/vt_file_permissions.py` & `troubadix-23.7.1/troubadix/plugins/vt_file_permissions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/plugins/vt_placement.py` & `troubadix-23.7.1/troubadix/plugins/vt_placement.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/reporter.py` & `troubadix-23.7.1/troubadix/reporter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/results.py` & `troubadix-23.7.1/troubadix/results.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/runner.py` & `troubadix-23.7.1/troubadix/runner.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/standalone_plugins/allowed_rev_diff.py` & `troubadix-23.7.1/troubadix/standalone_plugins/allowed_rev_diff.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/standalone_plugins/changed_cves.py` & `troubadix-23.7.1/troubadix/standalone_plugins/changed_cves.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/standalone_plugins/changed_oid.py` & `troubadix-23.7.1/troubadix/standalone_plugins/changed_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/changed_packages.py` & `troubadix-23.7.1/troubadix/standalone_plugins/changed_packages/changed_packages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/__init__.py` & `troubadix-23.7.1/troubadix/standalone_plugins/changed_packages/marker/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py` & `troubadix-23.7.1/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/added_release.py` & `troubadix-23.7.1/troubadix/standalone_plugins/changed_packages/marker/added_release.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py` & `troubadix-23.7.1/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/changed_update.py` & `troubadix-23.7.1/troubadix/standalone_plugins/changed_packages/marker/changed_update.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py` & `troubadix-23.7.1/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/marker/marker.py` & `troubadix-23.7.1/troubadix/standalone_plugins/changed_packages/marker/marker.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/standalone_plugins/changed_packages/package.py` & `troubadix-23.7.1/troubadix/standalone_plugins/changed_packages/package.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/standalone_plugins/common.py` & `troubadix-23.7.1/troubadix/standalone_plugins/common.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/standalone_plugins/last_modification.py` & `troubadix-23.7.1/troubadix/standalone_plugins/last_modification.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/standalone_plugins/no_solution.py` & `troubadix-23.7.1/troubadix/standalone_plugins/no_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/standalone_plugins/version_updated.py` & `troubadix-23.7.1/troubadix/standalone_plugins/version_updated.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/troubadix/troubadix.py` & `troubadix-23.7.1/troubadix/troubadix.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.7.0/PKG-INFO` & `troubadix-23.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troubadix
-Version: 23.7.0
+Version: 23.7.1
 Summary: A linting and QA check tool for NASL files
 Home-page: https://github.com/greenbone/troubadix
 License: GPL-3.0-or-later
 Author: Greenbone
 Author-email: info@greenbone.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

