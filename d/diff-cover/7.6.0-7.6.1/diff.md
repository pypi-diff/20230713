# Comparing `tmp/diff_cover-7.6.0.tar.gz` & `tmp/diff_cover-7.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diff_cover-7.6.0.tar", max compression
+gzip compressed data, was "diff_cover-7.6.1.tar", max compression
```

## Comparing `diff_cover-7.6.0.tar` & `diff_cover-7.6.1.tar`

### file list

```diff
@@ -1,134 +1,134 @@
--rw-r--r--   0        0        0    10174 2017-05-19 00:17:21.000000 diff_cover-7.6.0/LICENSE
--rw-r--r--   0        0        0    15616 2022-12-01 03:45:40.558740 diff_cover-7.6.0/README.rst
--rw-r--r--   0        0        0      417 2021-09-26 16:27:40.443898 diff_cover-7.6.0/diff_cover/__init__.py
--rw-r--r--   0        0        0     1942 2021-08-08 15:19:39.212215 diff_cover-7.6.0/diff_cover/command_runner.py
--rw-r--r--   0        0        0     2295 2023-01-19 03:05:26.077089 diff_cover-7.6.0/diff_cover/config_parser.py
--rw-r--r--   0        0        0     8996 2022-11-26 17:05:10.600305 diff_cover-7.6.0/diff_cover/diff_cover_tool.py
--rw-r--r--   0        0        0    11548 2023-06-11 02:20:00.909670 diff_cover-7.6.0/diff_cover/diff_quality_tool.py
--rw-r--r--   0        0        0    16726 2023-02-22 03:33:58.153476 diff_cover-7.6.0/diff_cover/diff_reporter.py
--rw-r--r--   0        0        0     3839 2022-09-19 23:15:04.810244 diff_cover-7.6.0/diff_cover/git_diff.py
--rw-r--r--   0        0        0     2036 2021-08-08 15:19:39.215258 diff_cover-7.6.0/diff_cover/git_path.py
--rw-r--r--   0        0        0      123 2020-08-23 18:59:26.239083 diff_cover-7.6.0/diff_cover/hook.py
--rw-r--r--   0        0        0      240 2019-12-12 03:52:05.646145 diff_cover-7.6.0/diff_cover/hookspecs.py
--rw-r--r--   0        0        0    14313 2023-02-22 03:33:58.153877 diff_cover-7.6.0/diff_cover/report_generator.py
--rw-r--r--   0        0        0    14118 2023-02-22 03:33:58.154379 diff_cover-7.6.0/diff_cover/snippets.py
--rw-r--r--   0        0        0      742 2021-12-02 23:59:08.058183 diff_cover-7.6.0/diff_cover/templates/console_coverage_report.txt
--rw-r--r--   0        0        0      787 2021-12-02 23:59:08.058957 diff_cover-7.6.0/diff_cover/templates/console_quality_report.txt
--rw-r--r--   0        0        0      174 2017-05-19 00:17:21.000000 diff_cover-7.6.0/diff_cover/templates/external_style.css
--rw-r--r--   0        0        0     1632 2021-12-02 23:59:08.059733 diff_cover-7.6.0/diff_cover/templates/html_coverage_report.html
--rw-r--r--   0        0        0     1880 2021-12-02 23:59:08.060501 diff_cover-7.6.0/diff_cover/templates/html_quality_report.html
--rw-r--r--   0        0        0      759 2021-12-02 23:59:08.061340 diff_cover-7.6.0/diff_cover/templates/markdown_coverage_report.md
--rw-r--r--   0        0        0      754 2021-12-02 23:59:08.062196 diff_cover-7.6.0/diff_cover/templates/markdown_quality_report.md
--rw-r--r--   0        0        0      371 2022-09-19 20:41:39.667279 diff_cover-7.6.0/diff_cover/templates/snippet_content.html
--rw-r--r--   0        0        0      229 2021-01-07 23:07:15.564857 diff_cover-7.6.0/diff_cover/templates/snippet_content.md
--rw-r--r--   0        0        0      204 2021-06-24 22:42:57.362317 diff_cover-7.6.0/diff_cover/templates/snippet_content.txt
--rw-r--r--   0        0        0      419 2017-05-19 00:17:21.000000 diff_cover-7.6.0/diff_cover/templates/snippet_style.html
--rw-r--r--   0        0        0      687 2021-08-15 21:41:36.275474 diff_cover-7.6.0/diff_cover/util.py
--rw-r--r--   0        0        0        0 2017-05-19 00:17:21.000000 diff_cover-7.6.0/diff_cover/violationsreporters/__init__.py
--rw-r--r--   0        0        0     8455 2022-12-01 03:45:40.562311 diff_cover-7.6.0/diff_cover/violationsreporters/base.py
--rw-r--r--   0        0        0     5838 2021-08-08 15:19:39.218323 diff_cover-7.6.0/diff_cover/violationsreporters/java_violations_reporter.py
--rw-r--r--   0        0        0    25987 2023-06-11 02:20:00.910269 diff_cover-7.6.0/diff_cover/violationsreporters/violations_reporter.py
--rw-r--r--   0        0        0     3464 2023-06-11 02:22:00.247199 diff_cover-7.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-08-08 15:19:39.221357 diff_cover-7.6.0/tests/__init__.py
--rw-r--r--   0        0        0      220 2021-08-08 15:19:39.221894 diff_cover-7.6.0/tests/fixtures/add_console_report.txt
--rw-r--r--   0        0        0     5234 2021-08-08 15:19:39.222148 diff_cover-7.6.0/tests/fixtures/add_html_report.html
--rw-r--r--   0        0        0      192 2021-08-08 15:19:39.222360 diff_cover-7.6.0/tests/fixtures/changed_console_report.txt
--rw-r--r--   0        0        0     4372 2021-08-08 15:19:39.222596 diff_cover-7.6.0/tests/fixtures/changed_html_report.html
--rw-r--r--   0        0        0      855 2021-08-08 15:19:39.222760 diff_cover-7.6.0/tests/fixtures/coverage.xml
--rw-r--r--   0        0        0      855 2021-08-08 15:19:39.222949 diff_cover-7.6.0/tests/fixtures/coverage1.xml
--rw-r--r--   0        0        0      855 2021-08-08 15:19:39.223212 diff_cover-7.6.0/tests/fixtures/coverage2.xml
--rw-r--r--   0        0        0      159 2021-08-08 15:19:39.223520 diff_cover-7.6.0/tests/fixtures/delete_console_report.txt
--rw-r--r--   0        0        0     3946 2021-08-08 15:19:39.223759 diff_cover-7.6.0/tests/fixtures/delete_html_report.html
--rw-r--r--   0        0        0     2664 2021-08-08 15:19:39.223983 diff_cover-7.6.0/tests/fixtures/dotnet_coverage.xml
--rw-r--r--   0        0        0      219 2021-08-08 15:19:39.224181 diff_cover-7.6.0/tests/fixtures/dotnet_coverage_console_report.txt
--rw-r--r--   0        0        0        0 2021-08-08 15:19:39.224254 diff_cover-7.6.0/tests/fixtures/empty.txt
--rw-r--r--   0        0        0      235 2021-08-08 15:19:39.224454 diff_cover-7.6.0/tests/fixtures/empty_pycodestyle_violations.txt
--rw-r--r--   0        0        0      913 2021-08-08 15:19:39.224664 diff_cover-7.6.0/tests/fixtures/external_css_html_report.html
--rw-r--r--   0        0        0     3400 2021-08-08 15:19:39.224918 diff_cover-7.6.0/tests/fixtures/external_style.css
--rw-r--r--   0        0        0      216 2021-08-08 15:19:39.225122 diff_cover-7.6.0/tests/fixtures/git_diff_add.txt
--rw-r--r--   0        0        0      216 2021-08-08 15:19:39.225264 diff_cover-7.6.0/tests/fixtures/git_diff_changed.txt
--rw-r--r--   0        0        0      560 2021-08-08 15:19:39.225411 diff_cover-7.6.0/tests/fixtures/git_diff_code_dupe.txt
--rw-r--r--   0        0        0      220 2021-08-08 15:19:39.225552 diff_cover-7.6.0/tests/fixtures/git_diff_delete.txt
--rw-r--r--   0        0        0      365 2021-08-08 15:19:39.225673 diff_cover-7.6.0/tests/fixtures/git_diff_dotnet.txt
--rw-r--r--   0        0        0      216 2021-08-08 15:19:39.225804 diff_cover-7.6.0/tests/fixtures/git_diff_external_css.txt
--rw-r--r--   0        0        0      259 2021-08-08 15:19:39.225925 diff_cover-7.6.0/tests/fixtures/git_diff_lua.txt
--rw-r--r--   0        0        0      216 2021-08-08 15:19:39.226049 diff_cover-7.6.0/tests/fixtures/git_diff_moved.txt
--rw-r--r--   0        0        0      216 2021-08-08 15:19:39.226184 diff_cover-7.6.0/tests/fixtures/git_diff_mult.txt
--rw-r--r--   0        0        0      228 2021-08-08 15:19:39.226318 diff_cover-7.6.0/tests/fixtures/git_diff_subdir.txt
--rw-r--r--   0        0        0      310 2021-08-08 15:19:39.226438 diff_cover-7.6.0/tests/fixtures/git_diff_unicode.txt
--rw-r--r--   0        0        0      543 2021-08-08 15:19:39.226578 diff_cover-7.6.0/tests/fixtures/git_diff_violations.txt
--rw-r--r--   0        0        0      266 2021-08-08 15:19:39.226708 diff_cover-7.6.0/tests/fixtures/git_diff_violations_two_files.txt
--rw-r--r--   0        0        0       33 2021-08-08 15:19:39.226827 diff_cover-7.6.0/tests/fixtures/hello.py
--rw-r--r--   0        0        0       33 2021-08-08 15:19:39.226940 diff_cover-7.6.0/tests/fixtures/hi.py
--rw-r--r--   0        0        0     1237 2021-08-08 15:19:39.227779 diff_cover-7.6.0/tests/fixtures/html_report.html
--rw-r--r--   0        0        0      677 2021-08-08 15:19:39.228378 diff_cover-7.6.0/tests/fixtures/html_report_empty.html
--rw-r--r--   0        0        0     1652 2021-08-08 15:19:39.228799 diff_cover-7.6.0/tests/fixtures/html_report_one_snippet.html
--rw-r--r--   0        0        0     1756 2021-08-08 15:19:39.229214 diff_cover-7.6.0/tests/fixtures/html_report_two_snippets.html
--rw-r--r--   0        0        0      232 2022-11-29 01:11:45.360884 diff_cover-7.6.0/tests/fixtures/lcov.info
--rw-r--r--   0        0        0      214 2021-08-08 15:19:39.229434 diff_cover-7.6.0/tests/fixtures/lua_console_report.txt
--rw-r--r--   0        0        0     1641 2021-08-08 15:19:39.229574 diff_cover-7.6.0/tests/fixtures/luacoverage.xml
--rw-r--r--   0        0        0      357 2021-08-08 15:19:39.229962 diff_cover-7.6.0/tests/fixtures/markdown_report_one_snippet.md
--rw-r--r--   0        0        0      469 2021-08-08 15:19:39.230396 diff_cover-7.6.0/tests/fixtures/markdown_report_two_snippets.md
--rw-r--r--   0        0        0      220 2021-08-08 15:19:39.230593 diff_cover-7.6.0/tests/fixtures/moved_console_report.txt
--rw-r--r--   0        0        0      855 2021-08-08 15:19:39.230720 diff_cover-7.6.0/tests/fixtures/moved_coverage.xml
--rw-r--r--   0        0        0     5234 2021-08-08 15:19:39.230926 diff_cover-7.6.0/tests/fixtures/moved_html_report.html
--rw-r--r--   0        0        0      218 2021-08-08 15:19:39.231105 diff_cover-7.6.0/tests/fixtures/mult_inputs_console_report.txt
--rw-r--r--   0        0        0     5207 2021-08-08 15:19:39.231318 diff_cover-7.6.0/tests/fixtures/mult_inputs_html_report.html
--rw-r--r--   0        0        0      262 2021-08-08 15:19:39.231442 diff_cover-7.6.0/tests/fixtures/pycodestyle_report.txt
--rw-r--r--   0        0        0     7135 2021-08-08 15:19:39.231628 diff_cover-7.6.0/tests/fixtures/pycodestyle_violations_report.html
--rw-r--r--   0        0        0      435 2021-08-08 15:19:39.231807 diff_cover-7.6.0/tests/fixtures/pycodestyle_violations_report.txt
--rw-r--r--   0        0        0     4434 2023-01-19 03:05:26.079637 diff_cover-7.6.0/tests/fixtures/pycodestyle_violations_report_external_css.html
--rw-r--r--   0        0        0      309 2021-08-08 15:19:39.232177 diff_cover-7.6.0/tests/fixtures/pyflakes_two_files.txt
--rw-r--r--   0        0        0     5810 2021-08-08 15:19:39.232398 diff_cover-7.6.0/tests/fixtures/pyflakes_violations_report.html
--rw-r--r--   0        0        0      314 2021-08-08 15:19:39.232563 diff_cover-7.6.0/tests/fixtures/pyflakes_violations_report.txt
--rw-r--r--   0        0        0     3172 2021-08-08 15:19:39.232685 diff_cover-7.6.0/tests/fixtures/pylint_dupe.txt
--rw-r--r--   0        0        0      284 2021-08-08 15:19:39.232844 diff_cover-7.6.0/tests/fixtures/pylint_dupe_violations_report.txt
--rw-r--r--   0        0        0     2884 2021-08-08 15:19:39.232987 diff_cover-7.6.0/tests/fixtures/pylint_report.txt
--rw-r--r--   0        0        0      516 2021-08-08 15:19:39.233163 diff_cover-7.6.0/tests/fixtures/pylint_violations_console_report.txt
--rw-r--r--   0        0        0     7583 2021-08-08 15:19:39.233354 diff_cover-7.6.0/tests/fixtures/pylint_violations_report.html
--rw-r--r--   0        0        0      418 2021-08-08 15:19:39.233516 diff_cover-7.6.0/tests/fixtures/pylint_violations_report.txt
--rw-r--r--   0        0        0        0 2021-08-08 15:19:39.233622 diff_cover-7.6.0/tests/fixtures/pylintrc
--rw-r--r--   0        0        0      379 2021-08-08 15:19:39.233815 diff_cover-7.6.0/tests/fixtures/show_uncovered_lines_console.txt
--rw-r--r--   0        0        0      355 2022-03-24 22:12:10.791587 diff_cover-7.6.0/tests/fixtures/snippet.css
--rw-r--r--   0        0        0      106 2021-08-08 15:19:39.234050 diff_cover-7.6.0/tests/fixtures/snippet_8859.py
--rw-r--r--   0        0        0     1410 2022-06-22 22:00:37.550883 diff_cover-7.6.0/tests/fixtures/snippet_arabic_output.html
--rw-r--r--   0        0        0      864 2022-06-22 22:00:37.551403 diff_cover-7.6.0/tests/fixtures/snippet_default.html
--rw-r--r--   0        0        0      814 2022-06-22 22:00:37.552129 diff_cover-7.6.0/tests/fixtures/snippet_invalid_violations.html
--rw-r--r--   0        0        0     4525 2022-06-22 22:00:37.553034 diff_cover-7.6.0/tests/fixtures/snippet_list.html
--rw-r--r--   0        0        0      275 2021-08-08 15:19:39.235011 diff_cover-7.6.0/tests/fixtures/snippet_list.md
--rw-r--r--   0        0        0      105 2021-08-08 15:19:39.235120 diff_cover-7.6.0/tests/fixtures/snippet_list2.md
--rw-r--r--   0        0        0      126 2021-08-08 15:19:39.235342 diff_cover-7.6.0/tests/fixtures/snippet_list3.md
--rw-r--r--   0        0        0      840 2022-06-22 22:00:37.553515 diff_cover-7.6.0/tests/fixtures/snippet_no_filename_ext.html
--rw-r--r--   0        0        0      791 2021-08-08 15:19:39.235897 diff_cover-7.6.0/tests/fixtures/snippet_src.py
--rw-r--r--   0        0        0       83 2021-08-08 15:19:39.236037 diff_cover-7.6.0/tests/fixtures/snippet_src2.cpp
--rw-r--r--   0        0        0      264 2021-08-08 15:19:39.236153 diff_cover-7.6.0/tests/fixtures/snippet_src3.cpp
--rw-r--r--   0        0        0      279 2022-06-22 22:00:37.553975 diff_cover-7.6.0/tests/fixtures/snippet_unicode.html
--rw-r--r--   0        0        0      888 2021-08-08 15:19:39.236587 diff_cover-7.6.0/tests/fixtures/snippet_unicode.py
--rw-r--r--   0        0        0     4749 2022-06-22 22:00:37.554460 diff_cover-7.6.0/tests/fixtures/snippet_unicode_html_output.html
--rw-r--r--   0        0        0      224 2021-08-08 15:19:39.236943 diff_cover-7.6.0/tests/fixtures/subdir_coverage_console_report.txt
--rw-r--r--   0        0        0     5282 2021-08-08 15:19:39.237141 diff_cover-7.6.0/tests/fixtures/subdir_coverage_html_report.html
--rw-r--r--   0        0        0       71 2021-08-08 15:19:39.237253 diff_cover-7.6.0/tests/fixtures/test_src.txt
--rw-r--r--   0        0        0      228 2021-08-08 15:19:39.237414 diff_cover-7.6.0/tests/fixtures/unicode_console_report.txt
--rw-r--r--   0        0        0      871 2021-08-08 15:19:39.237525 diff_cover-7.6.0/tests/fixtures/unicode_coverage.xml
--rw-r--r--   0        0        0     5400 2021-08-08 15:19:39.237754 diff_cover-7.6.0/tests/fixtures/unicode_html_report.html
--rw-r--r--   0        0        0      141 2021-08-08 15:19:39.237891 diff_cover-7.6.0/tests/fixtures/unicode_test_src.txt
--rw-r--r--   0        0        0      302 2021-08-08 15:19:39.238003 diff_cover-7.6.0/tests/fixtures/violations_test_file.py
--rw-r--r--   0        0        0     5801 2023-02-22 03:33:58.156711 diff_cover-7.6.0/tests/helpers.py
--rw-r--r--   0        0        0     3055 2021-08-08 15:19:39.238551 diff_cover-7.6.0/tests/snippet_list_unicode.html
--rw-r--r--   0        0        0     1575 2021-08-08 15:19:39.239555 diff_cover-7.6.0/tests/test_clover_violations_reporter/test.xml
--rw-r--r--   0        0        0      690 2021-08-08 15:19:39.239020 diff_cover-7.6.0/tests/test_clover_violations_reporter.py
--rw-r--r--   0        0        0     3066 2021-08-11 21:27:44.232023 diff_cover-7.6.0/tests/test_config_parser.py
--rw-r--r--   0        0        0     1018 2022-11-26 17:05:10.602987 diff_cover-7.6.0/tests/test_diff_cover_main.py
--rw-r--r--   0        0        0     2360 2022-11-26 17:05:10.603356 diff_cover-7.6.0/tests/test_diff_cover_tool.py
--rw-r--r--   0        0        0     4099 2021-08-08 15:19:39.240891 diff_cover-7.6.0/tests/test_diff_quality_main.py
--rw-r--r--   0        0        0    20454 2023-02-22 03:33:58.157276 diff_cover-7.6.0/tests/test_diff_reporter.py
--rw-r--r--   0        0        0     5243 2021-08-08 15:19:39.241828 diff_cover-7.6.0/tests/test_git_diff.py
--rw-r--r--   0        0        0     2703 2021-08-08 15:19:39.242459 diff_cover-7.6.0/tests/test_git_path.py
--rw-r--r--   0        0        0    21071 2023-02-22 03:33:58.157937 diff_cover-7.6.0/tests/test_integration.py
--rw-r--r--   0        0        0    22017 2023-02-22 03:33:58.158989 diff_cover-7.6.0/tests/test_java_violations_reporter.py
--rw-r--r--   0        0        0    18248 2023-02-22 03:33:58.159591 diff_cover-7.6.0/tests/test_report_generator.py
--rw-r--r--   0        0        0     8462 2021-08-08 15:19:39.244711 diff_cover-7.6.0/tests/test_snippets.py
--rw-r--r--   0        0        0      356 2021-08-15 21:41:36.276562 diff_cover-7.6.0/tests/test_util.py
--rw-r--r--   0        0        0    65687 2023-06-11 02:20:00.912629 diff_cover-7.6.0/tests/test_violations_reporter.py
--rw-r--r--   0        0        0    17229 1970-01-01 00:00:00.000000 diff_cover-7.6.0/setup.py
--rw-r--r--   0        0        0    17308 1970-01-01 00:00:00.000000 diff_cover-7.6.0/PKG-INFO
+-rw-r--r--   0        0        0    10174 2017-05-19 00:17:21.000000 diff_cover-7.6.1/LICENSE
+-rw-r--r--   0        0        0    15616 2022-12-01 03:45:40.558740 diff_cover-7.6.1/README.rst
+-rw-r--r--   0        0        0      417 2021-09-26 16:27:40.443898 diff_cover-7.6.1/diff_cover/__init__.py
+-rw-r--r--   0        0        0     1942 2021-08-08 15:19:39.212215 diff_cover-7.6.1/diff_cover/command_runner.py
+-rw-r--r--   0        0        0     2295 2023-01-19 03:05:26.077089 diff_cover-7.6.1/diff_cover/config_parser.py
+-rw-r--r--   0        0        0     8996 2022-11-26 17:05:10.600305 diff_cover-7.6.1/diff_cover/diff_cover_tool.py
+-rw-r--r--   0        0        0    11548 2023-06-11 02:20:00.909670 diff_cover-7.6.1/diff_cover/diff_quality_tool.py
+-rw-r--r--   0        0        0    16726 2023-02-22 03:33:58.153476 diff_cover-7.6.1/diff_cover/diff_reporter.py
+-rw-r--r--   0        0        0     3839 2022-09-19 23:15:04.810244 diff_cover-7.6.1/diff_cover/git_diff.py
+-rw-r--r--   0        0        0     2036 2021-08-08 15:19:39.215258 diff_cover-7.6.1/diff_cover/git_path.py
+-rw-r--r--   0        0        0      123 2020-08-23 18:59:26.239083 diff_cover-7.6.1/diff_cover/hook.py
+-rw-r--r--   0        0        0      240 2019-12-12 03:52:05.646145 diff_cover-7.6.1/diff_cover/hookspecs.py
+-rw-r--r--   0        0        0    14313 2023-02-22 03:33:58.153877 diff_cover-7.6.1/diff_cover/report_generator.py
+-rw-r--r--   0        0        0    14118 2023-02-22 03:33:58.154379 diff_cover-7.6.1/diff_cover/snippets.py
+-rw-r--r--   0        0        0      742 2021-12-02 23:59:08.058183 diff_cover-7.6.1/diff_cover/templates/console_coverage_report.txt
+-rw-r--r--   0        0        0      787 2021-12-02 23:59:08.058957 diff_cover-7.6.1/diff_cover/templates/console_quality_report.txt
+-rw-r--r--   0        0        0      174 2017-05-19 00:17:21.000000 diff_cover-7.6.1/diff_cover/templates/external_style.css
+-rw-r--r--   0        0        0     1632 2021-12-02 23:59:08.059733 diff_cover-7.6.1/diff_cover/templates/html_coverage_report.html
+-rw-r--r--   0        0        0     1880 2021-12-02 23:59:08.060501 diff_cover-7.6.1/diff_cover/templates/html_quality_report.html
+-rw-r--r--   0        0        0      759 2021-12-02 23:59:08.061340 diff_cover-7.6.1/diff_cover/templates/markdown_coverage_report.md
+-rw-r--r--   0        0        0      754 2021-12-02 23:59:08.062196 diff_cover-7.6.1/diff_cover/templates/markdown_quality_report.md
+-rw-r--r--   0        0        0      371 2022-09-19 20:41:39.667279 diff_cover-7.6.1/diff_cover/templates/snippet_content.html
+-rw-r--r--   0        0        0      229 2021-01-07 23:07:15.564857 diff_cover-7.6.1/diff_cover/templates/snippet_content.md
+-rw-r--r--   0        0        0      204 2021-06-24 22:42:57.362317 diff_cover-7.6.1/diff_cover/templates/snippet_content.txt
+-rw-r--r--   0        0        0      419 2017-05-19 00:17:21.000000 diff_cover-7.6.1/diff_cover/templates/snippet_style.html
+-rw-r--r--   0        0        0      687 2021-08-15 21:41:36.275474 diff_cover-7.6.1/diff_cover/util.py
+-rw-r--r--   0        0        0        0 2017-05-19 00:17:21.000000 diff_cover-7.6.1/diff_cover/violationsreporters/__init__.py
+-rw-r--r--   0        0        0     8455 2022-12-01 03:45:40.562311 diff_cover-7.6.1/diff_cover/violationsreporters/base.py
+-rw-r--r--   0        0        0     5838 2021-08-08 15:19:39.218323 diff_cover-7.6.1/diff_cover/violationsreporters/java_violations_reporter.py
+-rw-r--r--   0        0        0    25987 2023-06-11 02:20:00.910269 diff_cover-7.6.1/diff_cover/violationsreporters/violations_reporter.py
+-rw-r--r--   0        0        0     3464 2023-07-13 02:36:57.829460 diff_cover-7.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-08-08 15:19:39.221357 diff_cover-7.6.1/tests/__init__.py
+-rw-r--r--   0        0        0      220 2021-08-08 15:19:39.221894 diff_cover-7.6.1/tests/fixtures/add_console_report.txt
+-rw-r--r--   0        0        0     5234 2021-08-08 15:19:39.222148 diff_cover-7.6.1/tests/fixtures/add_html_report.html
+-rw-r--r--   0        0        0      192 2021-08-08 15:19:39.222360 diff_cover-7.6.1/tests/fixtures/changed_console_report.txt
+-rw-r--r--   0        0        0     4372 2021-08-08 15:19:39.222596 diff_cover-7.6.1/tests/fixtures/changed_html_report.html
+-rw-r--r--   0        0        0      855 2021-08-08 15:19:39.222760 diff_cover-7.6.1/tests/fixtures/coverage.xml
+-rw-r--r--   0        0        0      855 2021-08-08 15:19:39.222949 diff_cover-7.6.1/tests/fixtures/coverage1.xml
+-rw-r--r--   0        0        0      855 2021-08-08 15:19:39.223212 diff_cover-7.6.1/tests/fixtures/coverage2.xml
+-rw-r--r--   0        0        0      159 2021-08-08 15:19:39.223520 diff_cover-7.6.1/tests/fixtures/delete_console_report.txt
+-rw-r--r--   0        0        0     3946 2021-08-08 15:19:39.223759 diff_cover-7.6.1/tests/fixtures/delete_html_report.html
+-rw-r--r--   0        0        0     2664 2021-08-08 15:19:39.223983 diff_cover-7.6.1/tests/fixtures/dotnet_coverage.xml
+-rw-r--r--   0        0        0      219 2021-08-08 15:19:39.224181 diff_cover-7.6.1/tests/fixtures/dotnet_coverage_console_report.txt
+-rw-r--r--   0        0        0        0 2021-08-08 15:19:39.224254 diff_cover-7.6.1/tests/fixtures/empty.txt
+-rw-r--r--   0        0        0      235 2021-08-08 15:19:39.224454 diff_cover-7.6.1/tests/fixtures/empty_pycodestyle_violations.txt
+-rw-r--r--   0        0        0      913 2021-08-08 15:19:39.224664 diff_cover-7.6.1/tests/fixtures/external_css_html_report.html
+-rw-r--r--   0        0        0     3400 2021-08-08 15:19:39.224918 diff_cover-7.6.1/tests/fixtures/external_style.css
+-rw-r--r--   0        0        0      216 2021-08-08 15:19:39.225122 diff_cover-7.6.1/tests/fixtures/git_diff_add.txt
+-rw-r--r--   0        0        0      216 2021-08-08 15:19:39.225264 diff_cover-7.6.1/tests/fixtures/git_diff_changed.txt
+-rw-r--r--   0        0        0      560 2021-08-08 15:19:39.225411 diff_cover-7.6.1/tests/fixtures/git_diff_code_dupe.txt
+-rw-r--r--   0        0        0      220 2021-08-08 15:19:39.225552 diff_cover-7.6.1/tests/fixtures/git_diff_delete.txt
+-rw-r--r--   0        0        0      365 2021-08-08 15:19:39.225673 diff_cover-7.6.1/tests/fixtures/git_diff_dotnet.txt
+-rw-r--r--   0        0        0      216 2021-08-08 15:19:39.225804 diff_cover-7.6.1/tests/fixtures/git_diff_external_css.txt
+-rw-r--r--   0        0        0      259 2021-08-08 15:19:39.225925 diff_cover-7.6.1/tests/fixtures/git_diff_lua.txt
+-rw-r--r--   0        0        0      216 2021-08-08 15:19:39.226049 diff_cover-7.6.1/tests/fixtures/git_diff_moved.txt
+-rw-r--r--   0        0        0      216 2021-08-08 15:19:39.226184 diff_cover-7.6.1/tests/fixtures/git_diff_mult.txt
+-rw-r--r--   0        0        0      228 2021-08-08 15:19:39.226318 diff_cover-7.6.1/tests/fixtures/git_diff_subdir.txt
+-rw-r--r--   0        0        0      310 2021-08-08 15:19:39.226438 diff_cover-7.6.1/tests/fixtures/git_diff_unicode.txt
+-rw-r--r--   0        0        0      543 2021-08-08 15:19:39.226578 diff_cover-7.6.1/tests/fixtures/git_diff_violations.txt
+-rw-r--r--   0        0        0      266 2021-08-08 15:19:39.226708 diff_cover-7.6.1/tests/fixtures/git_diff_violations_two_files.txt
+-rw-r--r--   0        0        0       33 2021-08-08 15:19:39.226827 diff_cover-7.6.1/tests/fixtures/hello.py
+-rw-r--r--   0        0        0       33 2021-08-08 15:19:39.226940 diff_cover-7.6.1/tests/fixtures/hi.py
+-rw-r--r--   0        0        0     1237 2021-08-08 15:19:39.227779 diff_cover-7.6.1/tests/fixtures/html_report.html
+-rw-r--r--   0        0        0      677 2021-08-08 15:19:39.228378 diff_cover-7.6.1/tests/fixtures/html_report_empty.html
+-rw-r--r--   0        0        0     1652 2021-08-08 15:19:39.228799 diff_cover-7.6.1/tests/fixtures/html_report_one_snippet.html
+-rw-r--r--   0        0        0     1756 2021-08-08 15:19:39.229214 diff_cover-7.6.1/tests/fixtures/html_report_two_snippets.html
+-rw-r--r--   0        0        0      232 2022-11-29 01:11:45.360884 diff_cover-7.6.1/tests/fixtures/lcov.info
+-rw-r--r--   0        0        0      214 2021-08-08 15:19:39.229434 diff_cover-7.6.1/tests/fixtures/lua_console_report.txt
+-rw-r--r--   0        0        0     1641 2021-08-08 15:19:39.229574 diff_cover-7.6.1/tests/fixtures/luacoverage.xml
+-rw-r--r--   0        0        0      357 2021-08-08 15:19:39.229962 diff_cover-7.6.1/tests/fixtures/markdown_report_one_snippet.md
+-rw-r--r--   0        0        0      469 2021-08-08 15:19:39.230396 diff_cover-7.6.1/tests/fixtures/markdown_report_two_snippets.md
+-rw-r--r--   0        0        0      220 2021-08-08 15:19:39.230593 diff_cover-7.6.1/tests/fixtures/moved_console_report.txt
+-rw-r--r--   0        0        0      855 2021-08-08 15:19:39.230720 diff_cover-7.6.1/tests/fixtures/moved_coverage.xml
+-rw-r--r--   0        0        0     5234 2021-08-08 15:19:39.230926 diff_cover-7.6.1/tests/fixtures/moved_html_report.html
+-rw-r--r--   0        0        0      218 2021-08-08 15:19:39.231105 diff_cover-7.6.1/tests/fixtures/mult_inputs_console_report.txt
+-rw-r--r--   0        0        0     5207 2021-08-08 15:19:39.231318 diff_cover-7.6.1/tests/fixtures/mult_inputs_html_report.html
+-rw-r--r--   0        0        0      262 2021-08-08 15:19:39.231442 diff_cover-7.6.1/tests/fixtures/pycodestyle_report.txt
+-rw-r--r--   0        0        0     7135 2021-08-08 15:19:39.231628 diff_cover-7.6.1/tests/fixtures/pycodestyle_violations_report.html
+-rw-r--r--   0        0        0      435 2021-08-08 15:19:39.231807 diff_cover-7.6.1/tests/fixtures/pycodestyle_violations_report.txt
+-rw-r--r--   0        0        0     4434 2023-01-19 03:05:26.079637 diff_cover-7.6.1/tests/fixtures/pycodestyle_violations_report_external_css.html
+-rw-r--r--   0        0        0      309 2021-08-08 15:19:39.232177 diff_cover-7.6.1/tests/fixtures/pyflakes_two_files.txt
+-rw-r--r--   0        0        0     5810 2021-08-08 15:19:39.232398 diff_cover-7.6.1/tests/fixtures/pyflakes_violations_report.html
+-rw-r--r--   0        0        0      314 2021-08-08 15:19:39.232563 diff_cover-7.6.1/tests/fixtures/pyflakes_violations_report.txt
+-rw-r--r--   0        0        0     3172 2021-08-08 15:19:39.232685 diff_cover-7.6.1/tests/fixtures/pylint_dupe.txt
+-rw-r--r--   0        0        0      284 2021-08-08 15:19:39.232844 diff_cover-7.6.1/tests/fixtures/pylint_dupe_violations_report.txt
+-rw-r--r--   0        0        0     2884 2021-08-08 15:19:39.232987 diff_cover-7.6.1/tests/fixtures/pylint_report.txt
+-rw-r--r--   0        0        0      516 2021-08-08 15:19:39.233163 diff_cover-7.6.1/tests/fixtures/pylint_violations_console_report.txt
+-rw-r--r--   0        0        0     7583 2021-08-08 15:19:39.233354 diff_cover-7.6.1/tests/fixtures/pylint_violations_report.html
+-rw-r--r--   0        0        0      418 2021-08-08 15:19:39.233516 diff_cover-7.6.1/tests/fixtures/pylint_violations_report.txt
+-rw-r--r--   0        0        0        0 2021-08-08 15:19:39.233622 diff_cover-7.6.1/tests/fixtures/pylintrc
+-rw-r--r--   0        0        0      379 2021-08-08 15:19:39.233815 diff_cover-7.6.1/tests/fixtures/show_uncovered_lines_console.txt
+-rw-r--r--   0        0        0      355 2022-03-24 22:12:10.791587 diff_cover-7.6.1/tests/fixtures/snippet.css
+-rw-r--r--   0        0        0      106 2021-08-08 15:19:39.234050 diff_cover-7.6.1/tests/fixtures/snippet_8859.py
+-rw-r--r--   0        0        0     1410 2022-06-22 22:00:37.550883 diff_cover-7.6.1/tests/fixtures/snippet_arabic_output.html
+-rw-r--r--   0        0        0      864 2022-06-22 22:00:37.551403 diff_cover-7.6.1/tests/fixtures/snippet_default.html
+-rw-r--r--   0        0        0      814 2022-06-22 22:00:37.552129 diff_cover-7.6.1/tests/fixtures/snippet_invalid_violations.html
+-rw-r--r--   0        0        0     4525 2022-06-22 22:00:37.553034 diff_cover-7.6.1/tests/fixtures/snippet_list.html
+-rw-r--r--   0        0        0      275 2021-08-08 15:19:39.235011 diff_cover-7.6.1/tests/fixtures/snippet_list.md
+-rw-r--r--   0        0        0      105 2021-08-08 15:19:39.235120 diff_cover-7.6.1/tests/fixtures/snippet_list2.md
+-rw-r--r--   0        0        0      126 2021-08-08 15:19:39.235342 diff_cover-7.6.1/tests/fixtures/snippet_list3.md
+-rw-r--r--   0        0        0      840 2022-06-22 22:00:37.553515 diff_cover-7.6.1/tests/fixtures/snippet_no_filename_ext.html
+-rw-r--r--   0        0        0      791 2021-08-08 15:19:39.235897 diff_cover-7.6.1/tests/fixtures/snippet_src.py
+-rw-r--r--   0        0        0       83 2021-08-08 15:19:39.236037 diff_cover-7.6.1/tests/fixtures/snippet_src2.cpp
+-rw-r--r--   0        0        0      264 2021-08-08 15:19:39.236153 diff_cover-7.6.1/tests/fixtures/snippet_src3.cpp
+-rw-r--r--   0        0        0      279 2022-06-22 22:00:37.553975 diff_cover-7.6.1/tests/fixtures/snippet_unicode.html
+-rw-r--r--   0        0        0      888 2021-08-08 15:19:39.236587 diff_cover-7.6.1/tests/fixtures/snippet_unicode.py
+-rw-r--r--   0        0        0     4749 2022-06-22 22:00:37.554460 diff_cover-7.6.1/tests/fixtures/snippet_unicode_html_output.html
+-rw-r--r--   0        0        0      224 2021-08-08 15:19:39.236943 diff_cover-7.6.1/tests/fixtures/subdir_coverage_console_report.txt
+-rw-r--r--   0        0        0     5282 2021-08-08 15:19:39.237141 diff_cover-7.6.1/tests/fixtures/subdir_coverage_html_report.html
+-rw-r--r--   0        0        0       71 2021-08-08 15:19:39.237253 diff_cover-7.6.1/tests/fixtures/test_src.txt
+-rw-r--r--   0        0        0      228 2021-08-08 15:19:39.237414 diff_cover-7.6.1/tests/fixtures/unicode_console_report.txt
+-rw-r--r--   0        0        0      871 2021-08-08 15:19:39.237525 diff_cover-7.6.1/tests/fixtures/unicode_coverage.xml
+-rw-r--r--   0        0        0     5400 2021-08-08 15:19:39.237754 diff_cover-7.6.1/tests/fixtures/unicode_html_report.html
+-rw-r--r--   0        0        0      141 2021-08-08 15:19:39.237891 diff_cover-7.6.1/tests/fixtures/unicode_test_src.txt
+-rw-r--r--   0        0        0      302 2021-08-08 15:19:39.238003 diff_cover-7.6.1/tests/fixtures/violations_test_file.py
+-rw-r--r--   0        0        0     5801 2023-02-22 03:33:58.156711 diff_cover-7.6.1/tests/helpers.py
+-rw-r--r--   0        0        0     3055 2021-08-08 15:19:39.238551 diff_cover-7.6.1/tests/snippet_list_unicode.html
+-rw-r--r--   0        0        0     1575 2021-08-08 15:19:39.239555 diff_cover-7.6.1/tests/test_clover_violations_reporter/test.xml
+-rw-r--r--   0        0        0      690 2021-08-08 15:19:39.239020 diff_cover-7.6.1/tests/test_clover_violations_reporter.py
+-rw-r--r--   0        0        0     3066 2021-08-11 21:27:44.232023 diff_cover-7.6.1/tests/test_config_parser.py
+-rw-r--r--   0        0        0     1018 2022-11-26 17:05:10.602987 diff_cover-7.6.1/tests/test_diff_cover_main.py
+-rw-r--r--   0        0        0     2360 2022-11-26 17:05:10.603356 diff_cover-7.6.1/tests/test_diff_cover_tool.py
+-rw-r--r--   0        0        0     4099 2021-08-08 15:19:39.240891 diff_cover-7.6.1/tests/test_diff_quality_main.py
+-rw-r--r--   0        0        0    20454 2023-02-22 03:33:58.157276 diff_cover-7.6.1/tests/test_diff_reporter.py
+-rw-r--r--   0        0        0     5243 2021-08-08 15:19:39.241828 diff_cover-7.6.1/tests/test_git_diff.py
+-rw-r--r--   0        0        0     2703 2021-08-08 15:19:39.242459 diff_cover-7.6.1/tests/test_git_path.py
+-rw-r--r--   0        0        0    21071 2023-02-22 03:33:58.157937 diff_cover-7.6.1/tests/test_integration.py
+-rw-r--r--   0        0        0    22017 2023-02-22 03:33:58.158989 diff_cover-7.6.1/tests/test_java_violations_reporter.py
+-rw-r--r--   0        0        0    18248 2023-02-22 03:33:58.159591 diff_cover-7.6.1/tests/test_report_generator.py
+-rw-r--r--   0        0        0     8462 2021-08-08 15:19:39.244711 diff_cover-7.6.1/tests/test_snippets.py
+-rw-r--r--   0        0        0      356 2021-08-15 21:41:36.276562 diff_cover-7.6.1/tests/test_util.py
+-rw-r--r--   0        0        0    65687 2023-06-11 02:20:00.912629 diff_cover-7.6.1/tests/test_violations_reporter.py
+-rw-r--r--   0        0        0    17229 1970-01-01 00:00:00.000000 diff_cover-7.6.1/setup.py
+-rw-r--r--   0        0        0    17259 1970-01-01 00:00:00.000000 diff_cover-7.6.1/PKG-INFO
```

### Comparing `diff_cover-7.6.0/LICENSE` & `diff_cover-7.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/README.rst` & `diff_cover-7.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/diff_cover/command_runner.py` & `diff_cover-7.6.1/diff_cover/command_runner.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/diff_cover/config_parser.py` & `diff_cover-7.6.1/diff_cover/config_parser.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/diff_cover/diff_cover_tool.py` & `diff_cover-7.6.1/diff_cover/diff_cover_tool.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/diff_cover/diff_quality_tool.py` & `diff_cover-7.6.1/diff_cover/diff_quality_tool.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/diff_cover/diff_reporter.py` & `diff_cover-7.6.1/diff_cover/diff_reporter.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/diff_cover/git_diff.py` & `diff_cover-7.6.1/diff_cover/git_diff.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/diff_cover/git_path.py` & `diff_cover-7.6.1/diff_cover/git_path.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/diff_cover/report_generator.py` & `diff_cover-7.6.1/diff_cover/report_generator.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/diff_cover/snippets.py` & `diff_cover-7.6.1/diff_cover/snippets.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/diff_cover/templates/console_coverage_report.txt` & `diff_cover-7.6.1/diff_cover/templates/console_coverage_report.txt`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/diff_cover/templates/console_quality_report.txt` & `diff_cover-7.6.1/diff_cover/templates/console_quality_report.txt`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/diff_cover/templates/html_coverage_report.html` & `diff_cover-7.6.1/diff_cover/templates/html_coverage_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/diff_cover/templates/html_quality_report.html` & `diff_cover-7.6.1/diff_cover/templates/html_quality_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/diff_cover/templates/markdown_coverage_report.md` & `diff_cover-7.6.1/diff_cover/templates/markdown_coverage_report.md`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/diff_cover/templates/markdown_quality_report.md` & `diff_cover-7.6.1/diff_cover/templates/markdown_quality_report.md`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/diff_cover/util.py` & `diff_cover-7.6.1/diff_cover/util.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/diff_cover/violationsreporters/base.py` & `diff_cover-7.6.1/diff_cover/violationsreporters/base.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/diff_cover/violationsreporters/java_violations_reporter.py` & `diff_cover-7.6.1/diff_cover/violationsreporters/java_violations_reporter.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/diff_cover/violationsreporters/violations_reporter.py` & `diff_cover-7.6.1/diff_cover/violationsreporters/violations_reporter.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/pyproject.toml` & `diff_cover-7.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "diff_cover"
-version = "7.6.0"
+version = "7.6.1"
 description = "Run coverage and linting reports on diffs"
 authors = ["See Contributors"]
 homepage = "https://github.com/Bachmann1234/diff-cover"
 repository = "https://github.com/Bachmann1234/diff-cover"
-license = "Apache 2.0"
+license = "Apache-2.0"
 readme = "README.rst"
 classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
@@ -47,15 +47,15 @@
 chardet = ">=3.0.0"
 tomli = {version = ">=1.2.1", optional = true}
 setuptools = { version = ">=17.0.0", python = "<3.8" }
 
 [tool.poetry.dev-dependencies]
 pytest-cov = "^4.1.0"
 pytest-datadir = "^1.4.1"
-pytest-mock = "^3.10.0"
+pytest-mock = "^3.11.1"
 pycodestyle = ">=2.9.1"
 flake8 = "^5.0.4"
 pyflakes = "^2.5.0"
 pylint = "^2.17.4"
 pylint-pytest = "^1.1.2"
 pydocstyle = "^6.1.1"
 black = "^23.3.0"
```

### Comparing `diff_cover-7.6.0/tests/fixtures/add_html_report.html` & `diff_cover-7.6.1/tests/fixtures/add_html_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/changed_html_report.html` & `diff_cover-7.6.1/tests/fixtures/changed_html_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/coverage.xml` & `diff_cover-7.6.1/tests/fixtures/coverage.xml`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/coverage1.xml` & `diff_cover-7.6.1/tests/fixtures/coverage1.xml`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/coverage2.xml` & `diff_cover-7.6.1/tests/fixtures/coverage2.xml`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/delete_html_report.html` & `diff_cover-7.6.1/tests/fixtures/delete_html_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/dotnet_coverage.xml` & `diff_cover-7.6.1/tests/fixtures/dotnet_coverage.xml`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/external_css_html_report.html` & `diff_cover-7.6.1/tests/fixtures/external_css_html_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/external_style.css` & `diff_cover-7.6.1/tests/fixtures/external_style.css`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/git_diff_code_dupe.txt` & `diff_cover-7.6.1/tests/fixtures/git_diff_code_dupe.txt`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/git_diff_violations.txt` & `diff_cover-7.6.1/tests/fixtures/git_diff_violations.txt`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/html_report.html` & `diff_cover-7.6.1/tests/fixtures/html_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/html_report_empty.html` & `diff_cover-7.6.1/tests/fixtures/html_report_empty.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/html_report_one_snippet.html` & `diff_cover-7.6.1/tests/fixtures/html_report_one_snippet.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/html_report_two_snippets.html` & `diff_cover-7.6.1/tests/fixtures/html_report_two_snippets.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/luacoverage.xml` & `diff_cover-7.6.1/tests/fixtures/luacoverage.xml`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/moved_coverage.xml` & `diff_cover-7.6.1/tests/fixtures/moved_coverage.xml`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/moved_html_report.html` & `diff_cover-7.6.1/tests/fixtures/moved_html_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/mult_inputs_html_report.html` & `diff_cover-7.6.1/tests/fixtures/mult_inputs_html_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/pycodestyle_violations_report.html` & `diff_cover-7.6.1/tests/fixtures/pycodestyle_violations_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/pycodestyle_violations_report_external_css.html` & `diff_cover-7.6.1/tests/fixtures/pycodestyle_violations_report_external_css.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/pyflakes_violations_report.html` & `diff_cover-7.6.1/tests/fixtures/pyflakes_violations_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/pylint_dupe.txt` & `diff_cover-7.6.1/tests/fixtures/pylint_dupe.txt`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/pylint_report.txt` & `diff_cover-7.6.1/tests/fixtures/pylint_report.txt`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/pylint_violations_console_report.txt` & `diff_cover-7.6.1/tests/fixtures/pylint_violations_console_report.txt`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/pylint_violations_report.html` & `diff_cover-7.6.1/tests/fixtures/pylint_violations_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/snippet_arabic_output.html` & `diff_cover-7.6.1/tests/fixtures/snippet_arabic_output.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/snippet_default.html` & `diff_cover-7.6.1/tests/fixtures/snippet_default.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/snippet_invalid_violations.html` & `diff_cover-7.6.1/tests/fixtures/snippet_invalid_violations.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/snippet_list.html` & `diff_cover-7.6.1/tests/fixtures/snippet_list.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/snippet_no_filename_ext.html` & `diff_cover-7.6.1/tests/fixtures/snippet_no_filename_ext.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/snippet_src.py` & `diff_cover-7.6.1/tests/fixtures/snippet_src.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/snippet_unicode.py` & `diff_cover-7.6.1/tests/fixtures/snippet_unicode.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/snippet_unicode_html_output.html` & `diff_cover-7.6.1/tests/fixtures/snippet_unicode_html_output.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/subdir_coverage_html_report.html` & `diff_cover-7.6.1/tests/fixtures/subdir_coverage_html_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/unicode_coverage.xml` & `diff_cover-7.6.1/tests/fixtures/unicode_coverage.xml`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/fixtures/unicode_html_report.html` & `diff_cover-7.6.1/tests/fixtures/unicode_html_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/helpers.py` & `diff_cover-7.6.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/snippet_list_unicode.html` & `diff_cover-7.6.1/tests/snippet_list_unicode.html`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/test_clover_violations_reporter/test.xml` & `diff_cover-7.6.1/tests/test_clover_violations_reporter/test.xml`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/test_clover_violations_reporter.py` & `diff_cover-7.6.1/tests/test_clover_violations_reporter.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/test_config_parser.py` & `diff_cover-7.6.1/tests/test_config_parser.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/test_diff_cover_main.py` & `diff_cover-7.6.1/tests/test_diff_cover_main.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/test_diff_cover_tool.py` & `diff_cover-7.6.1/tests/test_diff_cover_tool.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/test_diff_quality_main.py` & `diff_cover-7.6.1/tests/test_diff_quality_main.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/test_diff_reporter.py` & `diff_cover-7.6.1/tests/test_diff_reporter.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/test_git_diff.py` & `diff_cover-7.6.1/tests/test_git_diff.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/test_git_path.py` & `diff_cover-7.6.1/tests/test_git_path.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/test_integration.py` & `diff_cover-7.6.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/test_java_violations_reporter.py` & `diff_cover-7.6.1/tests/test_java_violations_reporter.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/test_report_generator.py` & `diff_cover-7.6.1/tests/test_report_generator.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/test_snippets.py` & `diff_cover-7.6.1/tests/test_snippets.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/tests/test_violations_reporter.py` & `diff_cover-7.6.1/tests/test_violations_reporter.py`

 * *Files identical despite different names*

### Comparing `diff_cover-7.6.0/setup.py` & `diff_cover-7.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 entry_points = \
 {'console_scripts': ['diff-cover = diff_cover.diff_cover_tool:main',
                      'diff-quality = diff_cover.diff_quality_tool:main']}
 
 setup_kwargs = {
     'name': 'diff-cover',
-    'version': '7.6.0',
+    'version': '7.6.1',
     'description': 'Run coverage and linting reports on diffs',
     'long_description': 'diff-cover |pypi-version| |conda-version| |build-status|\n========================================================================================\n\nAutomatically find diff lines that need test coverage.\nAlso finds diff lines that have violations (according to tools such\nas pycodestyle, pyflakes, flake8, or pylint).\nThis is used as a code quality metric during code reviews.\n\nOverview\n--------\n\nDiff coverage is the percentage of new or modified\nlines that are covered by tests.  This provides a clear\nand achievable standard for code review: If you touch a line\nof code, that line should be covered.  Code coverage\nis *every* developer\'s responsibility!\n\nThe ``diff-cover`` command line tool compares an XML coverage report\nwith the output of ``git diff``.  It then reports coverage information\nfor lines in the diff.\n\nCurrently, ``diff-cover`` requires that:\n\n- You are using ``git`` for version control.\n- Your test runner generates coverage reports in Cobertura, Clover\n  or JaCoCo XML format, or LCov format.\n\nSupported XML or LCov coverage reports can be generated with many coverage tools,\nincluding:\n\n- Cobertura__ (Java)\n- Clover__ (Java)\n- JaCoCo__ (Java)\n- coverage.py__ (Python)\n- JSCover__ (JavaScript)\n- lcov__ (C/C++)\n\n__ http://cobertura.sourceforge.net/\n__ http://openclover.org/\n__ https://www.jacoco.org/\n__ http://nedbatchelder.com/code/coverage/\n__ http://tntim96.github.io/JSCover/\n__ https://ltp.sourceforge.net/coverage/lcov.php\n\n\n``diff-cover`` is designed to be extended.  If you are interested\nin adding support for other version control systems or coverage\nreport formats, see below for information on how to contribute!\n\n\nInstallation\n------------\n\nTo install the latest release:\n\n.. code:: bash\n\n    pip install diff_cover\n\n\nTo install the development version:\n\n.. code:: bash\n\n    git clone https://github.com/Bachmann1234/diff-cover.git\n    cd diff-cover\n    poetry install\n    poetry shell\n\n\nGetting Started\n---------------\n\n1. Set the current working directory to a ``git`` repository.\n\n2. Run your test suite under coverage and generate a [Cobertura, Clover or JaCoCo] XML report.\n   For example, using `pytest-cov`__:\n\n.. code:: bash\n\n    pytest --cov --cov-report=xml\n\n__ https://pypi.org/project/pytest-cov\n\nThis will create a ``coverage.xml`` file in the current working directory.\n\n**NOTE**: If you are using a different coverage generator, you will\nneed to use different commands to generate the coverage XML report.\n\n\n3. Run ``diff-cover``:\n\n.. code:: bash\n\n    diff-cover coverage.xml\n\nThis will compare the current ``git`` branch to ``origin/main`` and print\nthe diff coverage report to the console.\n\nYou can also generate an HTML, JSON or Markdown version of the report:\n\n.. code:: bash\n\n    diff-cover coverage.xml --html-report report.html\n    diff-cover coverage.xml --json-report report.json\n    diff-cover coverage.xml --markdown-report report.md\n\nMultiple XML Coverage Reports\n-------------------------------\n\nIn the case that one has multiple xml reports form multiple test suites, you\ncan get a combined coverage report (a line is counted  as covered if it is\ncovered in ANY of the xml reports) by running ``diff-cover`` with multiple\ncoverage reports as arguments. You may specify any arbitrary number of coverage\nreports:\n\n.. code:: bash\n\n    diff-cover coverage1.xml coverage2.xml\n\nQuality Coverage\n-----------------\nYou can use diff-cover to see quality reports on the diff as well by running\n``diff-quality``.\n\n.. code :: bash\n\n    diff-quality --violations=<tool>\n\nWhere ``tool`` is the quality checker to use. Currently ``pycodestyle``, ``pyflakes``,\n``flake8``, ``pylint``, ``checkstyle``, ``checkstylexml`` are supported, but more\ncheckers can (and should!) be supported. See the section "Adding `diff-quality``\nSupport for a New Quality Checker".\n\nNOTE: There\'s no way to run ``findbugs`` from ``diff-quality`` as it operating\nover the generated java bytecode and should be integrated into the build\nframework.\n\nLike ``diff-cover``, HTML, JSON or Markdown reports can be generated with\n\n.. code:: bash\n\n    diff-quality --violations=<tool> --html-report report.html\n    diff-quality --violations=<tool> --json-report report.json\n    diff-quality --violations=<tool> --markdown-report report.md\n\nIf you have already generated a report using ``pycodestyle``, ``pyflakes``, ``flake8``,\n``pylint``, ``checkstyle``, ``checkstylexml``, or ``findbugs`` you can pass the report\nto ``diff-quality``.  This is more efficient than letting ``diff-quality`` re-run\n``pycodestyle``, ``pyflakes``, ``flake8``, ``pylint``, ``checkstyle``, or ``checkstylexml``.\n\n.. code:: bash\n\n    # For pylint < 1.0\n    pylint -f parseable > pylint_report.txt\n\n    # For pylint >= 1.0\n    pylint --msg-template="{path}:{line}: [{msg_id}({symbol}), {obj}] {msg}" > pylint_report.txt\n\n    # Use the generated pylint report when running diff-quality\n    diff-quality --violations=pylint pylint_report.txt\n\n    # Use a generated pycodestyle report when running diff-quality.\n    pycodestyle > pycodestyle_report.txt\n    diff-quality --violations=pycodestyle pycodestyle_report.txt\n\nNote that you must use the ``-f parseable`` option to generate\nthe ``pylint`` report for pylint versions less than 1.0 and the\n``--msg-template`` option for versions >= 1.0.\n\n``diff-quality`` will also accept multiple ``pycodestyle``, ``pyflakes``, ``flake8``,\nor ``pylint`` reports:\n\n.. code:: bash\n\n    diff-quality --violations=pylint report_1.txt report_2.txt\n\nIf you need to pass in additional options you can with the ``options`` flag\n\n.. code:: bash\n\n    diff-quality --violations=pycodestyle --options="--exclude=\'*/migrations*\' --statistics" pycodestyle_report.txt\n\nCompare Branch\n--------------\n\nBy default, ``diff-cover`` compares the current branch to ``origin/main``.  To specify a different compare branch:\n\n.. code:: bash\n\n    diff-cover coverage.xml --compare-branch=origin/release\n\nFail Under\n----------\n\nTo have ``diff-cover`` and ``diff-quality`` return a non zero status code if the report quality/coverage percentage is\nbelow a certain threshold specify the fail-under parameter\n\n.. code:: bash\n\n    diff-cover coverage.xml --fail-under=80\n    diff-quality --violations=pycodestyle --fail-under=80\n\nThe above will return a non zero status if the coverage or quality score was below 80%.\n\nExclude/Include paths\n---------------------\n\nExplicit exclusion of paths is possible for both ``diff-cover`` and ``diff-quality``, while inclusion is\nonly supported for ``diff-quality`` (since 5.1.0).\n\nThe exclude option works with ``fnmatch``, include with ``glob``. Both options can consume multiple values.\nInclude options should be wrapped in double quotes to prevent shell globbing. Also they should be relative to\nthe current git directory.\n\n.. code:: bash\n\n    diff-cover coverage.xml --exclude setup.py\n    diff-quality --violations=pycodestyle --exclude setup.py\n\n    diff-quality --violations=pycodestyle --include project/foo/**\n\nThe following is executed for every changed file:\n\n#. check if any include pattern was specified\n#. if yes, check if the changed file is part of at least one include pattern\n#. check if the file is part of any exclude pattern\n\nIgnore/Include based on file status in git\n------------------------------------------\nBoth ``diff-cover`` and ``diff-quality`` allow users to ignore and include files based on the git\nstatus: staged, unstaged, untracked:\n\n* ``--ignore-staged``: ignore all staged files (by default include them)\n* ``--ignore-unstaged``: ignore all unstaged files (by default include them)\n* ``--include-untracked``: include all untracked files (by default ignore them)\n\nQuiet mode\n----------\nBoth ``diff-cover`` and ``diff-quality`` support a quiet mode which is disable by default.\nIt can be enabled by using the ``-q``/``--quiet`` flag:\n\n.. code:: bash\n\n    diff-cover coverage.xml -q\n    diff-quality --violations=pycodestyle -q\n\nIf enabled, the tool will only print errors and failures but no information or warning messages.\n\nConfiguration files\n-------------------\nBoth tools allow users to specify the options in a configuration file with `--config-file`/`-c`:\n\n.. code:: bash\n\n    diff-cover coverage.xml --config-file myconfig.toml\n    diff-quality --violations=pycodestyle --config-file myconfig.toml\n\nCurrently, only TOML files are supported.\nPlease note, that only non-mandatory options are supported.\nIf an option is specified in the configuration file and over the command line, the value of the\ncommand line is used.\n\nTOML configuration\n~~~~~~~~~~~~~~~~~~\n\nThe parser will only react to configuration files ending with `.toml`.\nTo use it, install `diff-cover` with the extra requirement `toml`.\n\nThe option names are the same as on the command line, but all dashes should be underscores.\nIf an option can be specified multiple times, the configuration value should be specified as a list.\n\n.. code:: toml\n\n    [tool.diff_cover]\n    compare_branch = "origin/feature"\n    quiet = true\n\n    [tool.diff_quality]\n    compare_branch = "origin/feature"\n    ignore_staged = true\n\n\nTroubleshooting\n----------------------\n\n**Issue**: ``diff-cover`` always reports: "No lines with coverage information in this diff."\n\n**Solution**: ``diff-cover`` matches source files in the coverage XML report with\nsource files in the ``git diff``.  For this reason, it\'s important\nthat the relative paths to the files match.  If you are using `coverage.py`__\nto generate the coverage XML report, then make sure you run\n``diff-cover`` from the same working directory.\n\n__ http://nedbatchelder.com/code/coverage/\n\n**Issue**: ``GitDiffTool._execute()`` raises the error:\n\n.. code:: bash\n\n    fatal: ambiguous argument \'origin/main...HEAD\': unknown revision or path not in the working tree.\n\nThis is known to occur when running ``diff-cover`` in `Travis CI`__\n\n__ http://travis-ci.org\n\n**Solution**: Fetch the remote main branch before running ``diff-cover``:\n\n.. code:: bash\n\n    git fetch origin master:refs/remotes/origin/main\n\n**Issue**: ``diff-quality`` reports "diff_cover.violations_reporter.QualityReporterError:\nNo config file found, using default configuration"\n\n**Solution**: Your project needs a `pylintrc` file.\nProvide this file (it can be empty) and ``diff-quality`` should run without issue.\n\n**Issue**: ``diff-quality`` reports "Quality tool not installed"\n\n**Solution**: ``diff-quality`` assumes you have the tool you wish to run against your diff installed.\nIf you do not have it then install it with your favorite package manager.\n\n**Issue**: ``diff-quality`` reports no quality issues\n\n**Solution**: You might use a pattern like ``diff-quality --violations foo *.py``. The last argument\nis not used to specify the files but for the quality tool report. Remove it to resolve the issue\n\nLicense\n-------\n\nThe code in this repository is licensed under the Apache 2.0 license.\nPlease see ``LICENSE.txt`` for details.\n\n\nHow to Contribute\n-----------------\n\nContributions are very welcome. The easiest way is to fork this repo, and then\nmake a pull request from your fork.\n\nNOTE: ``diff-quality`` supports a plugin model, so new tools can be integrated\nwithout requiring changes to this repo. See the section "Adding `diff-quality``\nSupport for a New Quality Checker".\n\nSetting Up For Development\n~~~~~~~~~~~~~~~~~~~~~~~~~~\n\nThis project is managed with `poetry` this can be installed with `pip`\npoetry manages a python virtual environment and organizes dependencies. It also\npackages this project.\n\n.. code:: bash\n\n    pip install poetry\n\n.. code:: bash\n\n    poetry install\n\nI would also suggest running this command after. This will make it so git blame ignores the commit\nthat formatted the entire codebase.\n\n.. code:: bash\n\n    git config blame.ignoreRevsFile .git-blame-ignore-revs\n\n\nAdding `diff-quality`` Support for a New Quality Checker\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\nAdding support for a new quality checker is simple. ``diff-quality`` supports\nplugins using the popular Python\n`pluggy package <https://pluggy.readthedocs.io/en/latest/>`_.\n\nIf the quality checker is already implemented as a Python package, great! If not,\n`create a Python package <https://packaging.python.org/tutorials/packaging-projects/>`_\nto host the plugin implementation.\n\nIn the Python package\'s ``setup.py`` file, define an entry point for the plugin,\ne.g.\n\n.. code:: python\n\n    setup(\n        ...\n        entry_points={\n            \'diff_cover\': [\n                \'sqlfluff = sqlfluff.diff_quality_plugin\'\n            ],\n        },\n        ...\n    )\n\nNotes:\n\n* The dictionary key for the entry point must be named ``diff_cover``\n* The value must be in the format ``TOOL_NAME = YOUR_PACKAGE.PLUGIN_MODULE``\n\nWhen your package is installed, ``diff-quality`` uses this information to\nlook up the tool package and module based on the tool name provided to the\n``--violations`` option of the ``diff-quality`` command, e.g.:\n\n.. code:: bash\n\n    $ diff-quality --violations sqlfluff\n\nThe plugin implementation will look something like the example below. This is\na simplified example based on a working plugin implementation.\n\n.. code:: python\n\n    from diff_cover.hook import hookimpl as diff_cover_hookimpl\n    from diff_cover.violationsreporters.base import BaseViolationReporter, Violation\n\n    class SQLFluffViolationReporter(BaseViolationReporter):\n        supported_extensions = [\'sql\']\n\n        def __init__(self):\n            super(SQLFluffViolationReporter, self).__init__(\'sqlfluff\')\n\n        def violations(self, src_path):\n            return [\n                Violation(violation.line_number, violation.description)\n                for violation in get_linter().get_violations(src_path)\n            ]\n\n        def measured_lines(self, src_path):\n            return None\n\n        @staticmethod\n        def installed():\n            return True\n\n\n    @diff_cover_hookimpl\n    def diff_cover_report_quality():\n        return SQLFluffViolationReporter()\n\nImportant notes:\n\n* ``diff-quality`` is looking for a plugin function:\n\n  * Located in your package\'s module that was listed in the ``setup.py`` entry point.\n  * Marked with the ``@diff_cover_hookimpl`` decorator\n  * Named ``diff_cover_report_quality``. (This distinguishes it from any other\n    plugin types ``diff_cover`` may support.)\n* The function should return an object with the following properties and methods:\n\n  * ``supported_extensions`` property with a list of supported file extensions\n  * ``violations()`` function that returns a list of ``Violation`` objects for\n    the specified ``src_path``. For more details on this function and other\n    possible reporting-related methods, see the ``BaseViolationReporter`` class\n    `here <https://github.com/Bachmann1234/diff_cover/blob/main/diff_cover/violationsreporters/base.py>`_.\n\nSpecial Thanks\n-------------------------\n\nShout out to the original author of diff-cover `Will Daly\n<https://github.com/wedaly>`_ and the original author of diff-quality `Sarina Canelake\n<https://github.com/sarina>`_.\n\nOriginally created with the support of `edX\n<https://github.com/edx>`_.\n\n\n.. |pypi-version| image:: https://img.shields.io/pypi/v/diff-cover.svg\n    :target: https://pypi.org/project/diff-cover\n    :alt: PyPI version\n.. |conda-version| image:: https://img.shields.io/conda/vn/conda-forge/diff-cover.svg\n    :target: https://anaconda.org/conda-forge/diff-cover\n    :alt: Conda version\n.. |build-status| image:: https://github.com/bachmann1234/diff_cover/actions/workflows/verify.yaml/badge.svg?branch=main\n    :target: https://github.com/Bachmann1234/diff_cover/actions/workflows/verify.yaml\n    :alt: Build Status\n',
     'author': 'See Contributors',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Bachmann1234/diff-cover',
```

### Comparing `diff_cover-7.6.0/PKG-INFO` & `diff_cover-7.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: diff-cover
-Version: 7.6.0
+Version: 7.6.1
 Summary: Run coverage and linting reports on diffs
 Home-page: https://github.com/Bachmann1234/diff-cover
-License: Apache 2.0
+License: Apache-2.0
 Author: See Contributors
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

