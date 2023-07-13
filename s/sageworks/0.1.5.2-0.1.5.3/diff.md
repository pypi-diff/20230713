# Comparing `tmp/sageworks-0.1.5.2.tar.gz` & `tmp/sageworks-0.1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sageworks-0.1.5.2.tar", last modified: Mon May 15 23:21:53 2023, max compression
+gzip compressed data, was "sageworks-0.1.5.3.tar", last modified: Thu Jul 13 16:19:19 2023, max compression
```

## Comparing `sageworks-0.1.5.2.tar` & `sageworks-0.1.5.3.tar`

### file list

```diff
@@ -1,273 +1,311 @@
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.679161 sageworks-0.1.5.2/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.624478 sageworks-0.1.5.2/.github/
--rw-r--r--   0 briford    (501) staff       (20)      499 2023-04-03 17:04:32.000000 sageworks-0.1.5.2/.github/dependabot.yml
--rw-r--r--   0 briford    (501) staff       (20)     1899 2023-03-25 19:33:37.000000 sageworks-0.1.5.2/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)      281 2023-03-28 23:51:00.000000 sageworks-0.1.5.2/CONTRIBUTING.md
--rw-r--r--   0 briford    (501) staff       (20)     1080 2023-02-17 22:10:33.000000 sageworks-0.1.5.2/LICENSE
--rw-r--r--   0 briford    (501) staff       (20)     1426 2023-04-30 02:31:13.000000 sageworks-0.1.5.2/Makefile
--rw-r--r--   0 briford    (501) staff       (20)     5964 2023-05-15 23:21:53.679250 sageworks-0.1.5.2/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)     5231 2023-05-06 21:24:25.000000 sageworks-0.1.5.2/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)      463 2023-04-03 17:04:32.000000 sageworks-0.1.5.2/SECURITY.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.618717 sageworks-0.1.5.2/applications/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.624690 sageworks-0.1.5.2/applications/aws_dashboard/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.625161 sageworks-0.1.5.2/applications/aws_dashboard/assets/
--rw-r--r--   0 briford    (501) staff       (20)    12412 2023-05-15 21:52:25.000000 sageworks-0.1.5.2/applications/aws_dashboard/assets/custom.css
--rw-r--r--   0 briford    (501) staff       (20)      318 2023-03-21 14:30:06.000000 sageworks-0.1.5.2/applications/aws_dashboard/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)     1081 2023-05-15 22:35:52.000000 sageworks-0.1.5.2/applications/aws_dashboard/aws_dashboard.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.626316 sageworks-0.1.5.2/applications/aws_dashboard/pages/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.627601 sageworks-0.1.5.2/applications/aws_dashboard/pages/callbacks/
--rw-r--r--   0 briford    (501) staff       (20)     4725 2023-05-15 22:23:21.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)      928 2023-05-10 17:06:02.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     4748 2023-05-15 22:23:21.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     1777 2023-05-14 18:41:54.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/callbacks/main_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     4757 2023-05-10 17:06:02.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/callbacks/models_callbacks.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.628087 sageworks-0.1.5.2/applications/aws_dashboard/pages/data/
--rw-r--r--   0 briford    (501) staff       (20)     1867 2023-04-08 01:44:28.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/data/toy_data.csv
--rw-r--r--   0 briford    (501) staff       (20)      597 2023-04-05 23:27:13.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/data/toy_scores.json
--rw-r--r--   0 briford    (501) staff       (20)     2545 2023-05-15 23:15:00.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/data_sources.py
--rw-r--r--   0 briford    (501) staff       (20)     1425 2023-05-10 17:06:02.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)     2576 2023-05-15 23:15:00.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/feature_sets.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.629306 sageworks-0.1.5.2/applications/aws_dashboard/pages/layout/
--rw-r--r--   0 briford    (501) staff       (20)     2696 2023-05-15 01:07:25.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/layout/data_sources_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1143 2023-04-09 22:27:31.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/layout/endpoints_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2707 2023-05-15 22:17:03.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/layout/feature_sets_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1584 2023-04-07 15:53:06.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/layout/main_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2436 2023-05-09 15:15:28.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/layout/models_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2115 2023-05-11 20:29:48.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/main.py
--rw-r--r--   0 briford    (501) staff       (20)     2547 2023-05-10 17:06:02.000000 sageworks-0.1.5.2/applications/aws_dashboard/pages/models.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.630101 sageworks-0.1.5.2/applications/hello_world/
--rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.5.2/applications/hello_world/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2152 2023-05-10 22:36:25.000000 sageworks-0.1.5.2/applications/hello_world/hello_world.py
--rw-r--r--   0 briford    (501) staff       (20)     1060 2023-04-02 18:05:33.000000 sageworks-0.1.5.2/applications/hello_world/layout.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.630776 sageworks-0.1.5.2/applications/model_viewer/
--rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.5.2/applications/model_viewer/callbacks.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.631297 sageworks-0.1.5.2/applications/model_viewer/data/
--rw-r--r--   0 briford    (501) staff       (20)     1849 2023-03-12 02:23:08.000000 sageworks-0.1.5.2/applications/model_viewer/data/toy_data.csv
--rw-r--r--   0 briford    (501) staff       (20)      597 2023-03-12 02:23:08.000000 sageworks-0.1.5.2/applications/model_viewer/data/toy_scores.json
--rw-r--r--   0 briford    (501) staff       (20)     3069 2023-04-02 18:05:33.000000 sageworks-0.1.5.2/applications/model_viewer/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2525 2023-05-09 15:17:31.000000 sageworks-0.1.5.2/applications/model_viewer/model_viewer.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.632048 sageworks-0.1.5.2/applications/web_admin/
--rw-r--r--   0 briford    (501) staff       (20)      213 2023-04-02 18:05:33.000000 sageworks-0.1.5.2/applications/web_admin/flask_test.py
--rw-r--r--   0 briford    (501) staff       (20)      201 2023-03-03 22:18:34.000000 sageworks-0.1.5.2/applications/web_admin/hello-world-http-test.ini
--rw-r--r--   0 briford    (501) staff       (20)      235 2023-03-03 22:19:17.000000 sageworks-0.1.5.2/applications/web_admin/hello-world.ini
--rw-r--r--   0 briford    (501) staff       (20)      399 2023-03-03 22:20:51.000000 sageworks-0.1.5.2/applications/web_admin/hello-world.service
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.632249 sageworks-0.1.5.2/applications/web_admin/nginx_conf/
--rw-r--r--   0 briford    (501) staff       (20)      486 2023-03-03 22:17:39.000000 sageworks-0.1.5.2/applications/web_admin/nginx_conf/nginx.conf
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.632641 sageworks-0.1.5.2/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     3315 2023-05-05 02:30:09.000000 sageworks-0.1.5.2/aws_setup/aws_account_check.py
--rw-r--r--   0 briford    (501) staff       (20)     4013 2023-05-05 02:30:09.000000 sageworks-0.1.5.2/aws_setup/build_ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.634264 sageworks-0.1.5.2/aws_setup/sageworks_cdk/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-04-20 17:45:20.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1028 2023-04-30 02:31:15.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1291 2023-04-30 16:18:03.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/app.py
--rw-r--r--   0 briford    (501) staff       (20)     1998 2023-04-20 17:45:20.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-04-20 17:45:20.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       70 2023-04-30 17:09:37.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-04-20 17:45:20.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.634508 sageworks-0.1.5.2/aws_setup/sageworks_cdk/stacks/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/stacks/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2304 2023-05-05 02:30:09.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/stacks/sageworks_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.634640 sageworks-0.1.5.2/aws_setup/sageworks_cdk/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.634801 sageworks-0.1.5.2/aws_setup/sageworks_cdk/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      720 2023-04-30 02:31:15.000000 sageworks-0.1.5.2/aws_setup/sageworks_cdk/tests/unit/test_sageworks_sandbox_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.634953 sageworks-0.1.5.2/config/
--rw-r--r--   0 briford    (501) staff       (20)      147 2023-04-30 02:43:00.000000 sageworks-0.1.5.2/config/sageworks_config.ini
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.636236 sageworks-0.1.5.2/data/
--rw-r--r--   0 briford    (501) staff       (20)   196156 2023-03-26 18:42:12.000000 sageworks-0.1.5.2/data/abalone.csv
--rw-r--r--   0 briford    (501) staff       (20)      829 2023-05-02 22:39:27.000000 sageworks-0.1.5.2/data/test_data.csv
--rw-r--r--   0 briford    (501) staff       (20)     2270 2023-04-19 19:55:29.000000 sageworks-0.1.5.2/data/test_data.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.637115 sageworks-0.1.5.2/docs/
--rw-r--r--   0 briford    (501) staff       (20)     1770 2023-05-09 15:36:49.000000 sageworks-0.1.5.2/docs/admin_notes.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.643240 sageworks-0.1.5.2/docs/images/
--rw-r--r--   0 briford    (501) staff       (20)   605827 2022-12-06 17:43:49.000000 sageworks-0.1.5.2/docs/images/big_spider.png
--rw-r--r--   0 briford    (501) staff       (20)    32320 2023-01-15 22:00:05.000000 sageworks-0.1.5.2/docs/images/graph_representation.png
--rw-r--r--   0 briford    (501) staff       (20)    15549 2023-03-06 20:35:02.000000 sageworks-0.1.5.2/docs/images/powered_aws_dark_blue.png
--rw-r--r--   0 briford    (501) staff       (20)    10003 2023-03-06 20:33:32.000000 sageworks-0.1.5.2/docs/images/powered_aws_transparent.png
--rw-r--r--   0 briford    (501) staff       (20)     6435 2023-03-06 20:31:13.000000 sageworks-0.1.5.2/docs/images/powered_aws_white.png
--rw-r--r--   0 briford    (501) staff       (20)    21174 2023-03-06 20:40:25.000000 sageworks-0.1.5.2/docs/images/powered_aws_with_tm_grey.png
--rw-r--r--   0 briford    (501) staff       (20)    51137 2023-01-15 21:19:16.000000 sageworks-0.1.5.2/docs/images/sageworks.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-03-10 19:48:12.000000 sageworks-0.1.5.2/docs/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)    30017 2023-01-15 21:23:57.000000 sageworks-0.1.5.2/docs/images/scp.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-01-12 16:00:43.000000 sageworks-0.1.5.2/docs/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)   381209 2022-12-06 17:43:49.000000 sageworks-0.1.5.2/docs/images/small_spider.png
--rw-r--r--   0 briford    (501) staff       (20)      667 2023-03-15 14:00:32.000000 sageworks-0.1.5.2/docs/sageworks_classes_concepts.md
--rw-r--r--   0 briford    (501) staff       (20)     1873 2023-03-13 14:45:22.000000 sageworks-0.1.5.2/docs/scp_consulting.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.644056 sageworks-0.1.5.2/examples/
--rw-r--r--   0 briford    (501) staff       (20)     1240 2023-04-02 18:05:33.000000 sageworks-0.1.5.2/examples/data_to_data_example.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.644403 sageworks-0.1.5.2/notebooks/
--rw-r--r--   0 briford    (501) staff       (20)   236926 2023-05-06 21:30:24.000000 sageworks-0.1.5.2/notebooks/ML_Pipeline_with_SageWorks.ipynb
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.649126 sageworks-0.1.5.2/notebooks/images/
--rw-r--r--   0 briford    (501) staff       (20)   142099 2023-04-14 22:52:23.000000 sageworks-0.1.5.2/notebooks/images/athena_query_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   191022 2023-04-14 22:50:14.000000 sageworks-0.1.5.2/notebooks/images/aws_dashboard_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   222686 2023-04-14 23:47:56.000000 sageworks-0.1.5.2/notebooks/images/dashboard_aqsol_features.png
--rw-r--r--   0 briford    (501) staff       (20)   171441 2023-04-15 00:30:02.000000 sageworks-0.1.5.2/notebooks/images/model_screenshot.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-04-15 16:18:02.000000 sageworks-0.1.5.2/notebooks/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-04-15 16:17:49.000000 sageworks-0.1.5.2/notebooks/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)      211 2023-05-02 03:06:50.000000 sageworks-0.1.5.2/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.653194 sageworks-0.1.5.2/scripts/
--rw-r--r--   0 briford    (501) staff       (20)     1373 2023-04-09 21:27:30.000000 sageworks-0.1.5.2/scripts/data_source_tags.py
--rw-r--r--   0 briford    (501) staff       (20)     1717 2023-05-05 02:30:09.000000 sageworks-0.1.5.2/scripts/generate_jsonl_data.py
--rw-r--r--   0 briford    (501) staff       (20)     1306 2023-04-09 21:27:30.000000 sageworks-0.1.5.2/scripts/list_data_sources.py
--rw-r--r--   0 briford    (501) staff       (20)      527 2023-05-15 23:21:53.679561 sageworks-0.1.5.2/setup.cfg
--rw-r--r--   0 briford    (501) staff       (20)     1787 2023-05-15 23:21:38.000000 sageworks-0.1.5.2/setup.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.619652 sageworks-0.1.5.2/src/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.653481 sageworks-0.1.5.2/src/sageworks/
--rw-r--r--   0 briford    (501) staff       (20)      853 2023-04-22 21:03:48.000000 sageworks-0.1.5.2/src/sageworks/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.654302 sageworks-0.1.5.2/src/sageworks/algorithms/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/algorithms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.619894 sageworks-0.1.5.2/src/sageworks/algorithms/graph/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.654389 sageworks-0.1.5.2/src/sageworks/algorithms/graph/heavy/
--rw-r--r--   0 briford    (501) staff       (20)       96 2023-03-05 20:00:31.000000 sageworks-0.1.5.2/src/sageworks/algorithms/graph/heavy/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.654625 sageworks-0.1.5.2/src/sageworks/algorithms/graph/light/
--rw-r--r--   0 briford    (501) staff       (20)      122 2023-03-05 19:59:59.000000 sageworks-0.1.5.2/src/sageworks/algorithms/graph/light/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.620061 sageworks-0.1.5.2/src/sageworks/algorithms/table/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.654845 sageworks-0.1.5.2/src/sageworks/algorithms/table/heavy/
--rw-r--r--   0 briford    (501) staff       (20)      169 2023-03-05 20:04:10.000000 sageworks-0.1.5.2/src/sageworks/algorithms/table/heavy/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.655931 sageworks-0.1.5.2/src/sageworks/algorithms/table/light/
--rw-r--r--   0 briford    (501) staff       (20)       95 2023-03-05 20:05:08.000000 sageworks-0.1.5.2/src/sageworks/algorithms/table/light/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     1751 2023-04-05 21:18:09.000000 sageworks-0.1.5.2/src/sageworks/algorithms/table/light/data_source_eda.py
--rw-r--r--   0 briford    (501) staff       (20)     9476 2023-04-09 21:27:30.000000 sageworks-0.1.5.2/src/sageworks/algorithms/table/light/feature_spider.py
--rw-r--r--   0 briford    (501) staff       (20)     4186 2023-04-09 21:27:30.000000 sageworks-0.1.5.2/src/sageworks/algorithms/table/light/row_tagger.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.656622 sageworks-0.1.5.2/src/sageworks/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      639 2023-03-05 21:06:58.000000 sageworks-0.1.5.2/src/sageworks/artifacts/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-01 03:28:03.000000 sageworks-0.1.5.2/src/sageworks/artifacts/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     5706 2023-05-14 17:23:33.000000 sageworks-0.1.5.2/src/sageworks/artifacts/artifact.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.657570 sageworks-0.1.5.2/src/sageworks/artifacts/data_sources/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/artifacts/data_sources/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    15504 2023-05-15 19:02:40.000000 sageworks-0.1.5.2/src/sageworks/artifacts/data_sources/athena_source.py
--rw-r--r--   0 briford    (501) staff       (20)     3129 2023-05-14 17:27:17.000000 sageworks-0.1.5.2/src/sageworks/artifacts/data_sources/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2891 2023-05-14 15:23:51.000000 sageworks-0.1.5.2/src/sageworks/artifacts/data_sources/data_source_abstract.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.657913 sageworks-0.1.5.2/src/sageworks/artifacts/endpoints/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/artifacts/endpoints/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     9792 2023-05-14 17:29:06.000000 sageworks-0.1.5.2/src/sageworks/artifacts/endpoints/endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.658365 sageworks-0.1.5.2/src/sageworks/artifacts/feature_sets/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/artifacts/feature_sets/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    13915 2023-05-15 23:16:08.000000 sageworks-0.1.5.2/src/sageworks/artifacts/feature_sets/feature_set.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.658573 sageworks-0.1.5.2/src/sageworks/artifacts/models/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/artifacts/models/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     4419 2023-05-14 17:29:06.000000 sageworks-0.1.5.2/src/sageworks/artifacts/models/model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.659284 sageworks-0.1.5.2/src/sageworks/aws_service_broker/
--rw-r--r--   0 briford    (501) staff       (20)     7633 2023-05-04 14:48:56.000000 sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_account_clamp.py
--rw-r--r--   0 briford    (501) staff       (20)     9590 2023-05-12 17:33:32.000000 sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_broker.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.661256 sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-14 19:44:44.000000 sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2501 2023-05-11 17:16:49.000000 sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
--rw-r--r--   0 briford    (501) staff       (20)     6066 2023-05-11 17:16:49.000000 sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)     3325 2023-05-11 18:41:08.000000 sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)     5772 2023-05-12 17:34:32.000000 sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)     4297 2023-05-11 18:40:16.000000 sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     2949 2023-05-10 23:23:46.000000 sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.661936 sageworks-0.1.5.2/src/sageworks/transforms/
--rw-r--r--   0 briford    (501) staff       (20)     1432 2023-03-17 17:39:22.000000 sageworks-0.1.5.2/src/sageworks/transforms/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/transforms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.620674 sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.662307 sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/heavy/
--rw-r--r--   0 briford    (501) staff       (20)     7367 2023-05-05 02:30:09.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.663122 sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/light/
--rw-r--r--   0 briford    (501) staff       (20)     2997 2023-04-14 22:16:23.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2483 2023-04-19 22:41:04.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/light/json_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     4155 2023-04-30 02:50:10.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.663428 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.663517 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.663598 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:15:48.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.663779 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:16:45.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.664404 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2231 2023-05-12 22:12:48.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/light/clean_data.py
--rw-r--r--   0 briford    (501) staff       (20)     2298 2023-05-12 21:29:54.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/light/data_to_data_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.664784 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.664998 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/heavy/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     5817 2023-05-12 17:46:07.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/heavy/data_to_features_heavy.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.665283 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:14.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.665568 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:14.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.666195 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2538 2023-05-12 17:52:28.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/light/data_to_features_light.py
--rw-r--r--   0 briford    (501) staff       (20)     2974 2023-05-12 17:46:07.000000 sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.666440 sageworks-0.1.5.2/src/sageworks/transforms/features_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 18:06:15.000000 sageworks-0.1.5.2/src/sageworks/transforms/features_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.621544 sageworks-0.1.5.2/src/sageworks/transforms/features_to_features/heavy/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.666535 sageworks-0.1.5.2/src/sageworks/transforms/features_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:46.000000 sageworks-0.1.5.2/src/sageworks/transforms/features_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.666783 sageworks-0.1.5.2/src/sageworks/transforms/features_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:46.000000 sageworks-0.1.5.2/src/sageworks/transforms/features_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.667089 sageworks-0.1.5.2/src/sageworks/transforms/features_to_model/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/transforms/features_to_model/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7840 2023-05-12 17:53:53.000000 sageworks-0.1.5.2/src/sageworks/transforms/features_to_model/features_to_model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.667683 sageworks-0.1.5.2/src/sageworks/transforms/features_to_model/light_model_harness/
--rw-r--r--   0 briford    (501) staff       (20)        8 2023-03-25 02:07:31.000000 sageworks-0.1.5.2/src/sageworks/transforms/features_to_model/light_model_harness/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)     5179 2023-04-18 16:01:35.000000 sageworks-0.1.5.2/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.668037 sageworks-0.1.5.2/src/sageworks/transforms/model_to_endpoint/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.2/src/sageworks/transforms/model_to_endpoint/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2800 2023-05-12 17:54:23.000000 sageworks-0.1.5.2/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.669273 sageworks-0.1.5.2/src/sageworks/transforms/pandas_transforms/
--rw-r--r--   0 briford    (501) staff       (20)     2745 2023-04-13 18:18:49.000000 sageworks-0.1.5.2/src/sageworks/transforms/pandas_transforms/data_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     3144 2023-04-13 18:18:49.000000 sageworks-0.1.5.2/src/sageworks/transforms/pandas_transforms/features_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     7003 2023-05-12 21:36:54.000000 sageworks-0.1.5.2/src/sageworks/transforms/pandas_transforms/pandas_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)    10872 2023-05-12 17:52:28.000000 sageworks-0.1.5.2/src/sageworks/transforms/pandas_transforms/pandas_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     7517 2023-05-12 23:56:39.000000 sageworks-0.1.5.2/src/sageworks/transforms/pandas_transforms/pandas_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     6705 2023-05-14 17:33:24.000000 sageworks-0.1.5.2/src/sageworks/transforms/transform.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.671659 sageworks-0.1.5.2/src/sageworks/utils/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 02:34:19.000000 sageworks-0.1.5.2/src/sageworks/utils/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3962 2023-04-30 02:31:13.000000 sageworks-0.1.5.2/src/sageworks/utils/cache.py
--rw-r--r--   0 briford    (501) staff       (20)     5113 2023-04-09 21:27:30.000000 sageworks-0.1.5.2/src/sageworks/utils/df_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     2417 2023-05-14 17:23:33.000000 sageworks-0.1.5.2/src/sageworks/utils/iso_8601.py
--rw-r--r--   0 briford    (501) staff       (20)     6532 2023-05-05 02:30:09.000000 sageworks-0.1.5.2/src/sageworks/utils/redis_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     3618 2023-04-17 19:53:54.000000 sageworks-0.1.5.2/src/sageworks/utils/sageworks_config.py
--rw-r--r--   0 briford    (501) staff       (20)     3558 2023-04-12 15:59:21.000000 sageworks-0.1.5.2/src/sageworks/utils/sageworks_event_bridge.py
--rw-r--r--   0 briford    (501) staff       (20)      531 2023-04-02 18:05:33.000000 sageworks-0.1.5.2/src/sageworks/utils/sageworks_logging.py
--rw-r--r--   0 briford    (501) staff       (20)     2209 2023-04-02 19:53:47.000000 sageworks-0.1.5.2/src/sageworks/utils/sageworks_sqs.py
--rw-r--r--   0 briford    (501) staff       (20)     1469 2023-05-15 01:49:43.000000 sageworks-0.1.5.2/src/sageworks/utils/type_abbrev.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.672993 sageworks-0.1.5.2/src/sageworks/views/
--rw-r--r--   0 briford    (501) staff       (20)    11812 2023-05-12 17:36:11.000000 sageworks-0.1.5.2/src/sageworks/views/artifacts_text_view.py
--rw-r--r--   0 briford    (501) staff       (20)     3063 2023-05-12 17:33:32.000000 sageworks-0.1.5.2/src/sageworks/views/artifacts_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     4307 2023-05-15 19:34:45.000000 sageworks-0.1.5.2/src/sageworks/views/data_source_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     4307 2023-05-15 22:08:31.000000 sageworks-0.1.5.2/src/sageworks/views/feature_set_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     1296 2023-04-19 17:02:05.000000 sageworks-0.1.5.2/src/sageworks/views/view.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.676103 sageworks-0.1.5.2/src/sageworks/web_components/
--rw-r--r--   0 briford    (501) staff       (20)     1304 2023-05-05 02:30:09.000000 sageworks-0.1.5.2/src/sageworks/web_components/box_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     1661 2023-04-08 01:37:21.000000 sageworks-0.1.5.2/src/sageworks/web_components/confusion_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     2316 2023-05-15 19:38:51.000000 sageworks-0.1.5.2/src/sageworks/web_components/data_source_details.py
--rw-r--r--   0 briford    (501) staff       (20)     1247 2023-04-09 21:27:30.000000 sageworks-0.1.5.2/src/sageworks/web_components/feature_details.py
--rw-r--r--   0 briford    (501) staff       (20)      815 2023-04-02 19:53:47.000000 sageworks-0.1.5.2/src/sageworks/web_components/feature_importance.py
--rw-r--r--   0 briford    (501) staff       (20)     2316 2023-05-15 22:17:03.000000 sageworks-0.1.5.2/src/sageworks/web_components/feature_set_details.py
--rw-r--r--   0 briford    (501) staff       (20)     1182 2023-04-07 23:04:10.000000 sageworks-0.1.5.2/src/sageworks/web_components/histogram.py
--rw-r--r--   0 briford    (501) staff       (20)      837 2023-04-09 21:27:30.000000 sageworks-0.1.5.2/src/sageworks/web_components/line_chart.py
--rw-r--r--   0 briford    (501) staff       (20)     1507 2023-04-09 21:30:08.000000 sageworks-0.1.5.2/src/sageworks/web_components/model_data.py
--rw-r--r--   0 briford    (501) staff       (20)     1703 2023-04-02 19:53:47.000000 sageworks-0.1.5.2/src/sageworks/web_components/model_details.py
--rw-r--r--   0 briford    (501) staff       (20)     1551 2023-04-09 21:27:30.000000 sageworks-0.1.5.2/src/sageworks/web_components/scatter_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     2227 2023-05-11 20:41:25.000000 sageworks-0.1.5.2/src/sageworks/web_components/table.py
--rw-r--r--   0 briford    (501) staff       (20)     2134 2023-05-15 22:23:21.000000 sageworks-0.1.5.2/src/sageworks/web_components/violin_plot.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.654194 sageworks-0.1.5.2/src/sageworks.egg-info/
--rw-r--r--   0 briford    (501) staff       (20)     5964 2023-05-15 23:21:53.000000 sageworks-0.1.5.2/src/sageworks.egg-info/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)     8884 2023-05-15 23:21:53.000000 sageworks-0.1.5.2/src/sageworks.egg-info/SOURCES.txt
--rw-r--r--   0 briford    (501) staff       (20)        1 2023-05-15 23:21:53.000000 sageworks-0.1.5.2/src/sageworks.egg-info/dependency_links.txt
--rw-r--r--   0 briford    (501) staff       (20)      134 2023-05-15 23:21:53.000000 sageworks-0.1.5.2/src/sageworks.egg-info/requires.txt
--rw-r--r--   0 briford    (501) staff       (20)       10 2023-05-15 23:21:53.000000 sageworks-0.1.5.2/src/sageworks.egg-info/top_level.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.676340 sageworks-0.1.5.2/tests/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.677521 sageworks-0.1.5.2/tests/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)     1250 2023-05-14 17:27:17.000000 sageworks-0.1.5.2/tests/artifacts/data_source_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1483 2023-04-11 20:37:15.000000 sageworks-0.1.5.2/tests/artifacts/endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1155 2023-05-14 17:27:17.000000 sageworks-0.1.5.2/tests/artifacts/feature_set_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      799 2023-04-02 18:05:33.000000 sageworks-0.1.5.2/tests/artifacts/model_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.677959 sageworks-0.1.5.2/tests/aws_account/
--rw-r--r--   0 briford    (501) staff       (20)     1105 2023-05-05 02:37:56.000000 sageworks-0.1.5.2/tests/aws_account/aws_account_clamp_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      642 2023-05-05 02:38:20.000000 sageworks-0.1.5.2/tests/aws_account/aws_service_broker_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     3341 2023-04-19 17:23:07.000000 sageworks-0.1.5.2/tests/create_sageworks_objs_for_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-15 23:21:53.678897 sageworks-0.1.5.2/tests/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      554 2023-05-12 17:46:18.000000 sageworks-0.1.5.2/tests/transforms/data_to_data_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      682 2023-05-12 18:00:39.000000 sageworks-0.1.5.2/tests/transforms/data_to_features_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      655 2023-05-12 18:01:20.000000 sageworks-0.1.5.2/tests/transforms/features_to_model_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      642 2023-05-12 17:46:18.000000 sageworks-0.1.5.2/tests/transforms/model_to_endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      628 2023-05-12 17:46:18.000000 sageworks-0.1.5.2/tests/transforms/pandas_to_data_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      729 2023-05-05 02:35:30.000000 sageworks-0.1.5.2/tox.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.656698 sageworks-0.1.5.3/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.602721 sageworks-0.1.5.3/.github/
+-rw-r--r--   0 briford    (501) staff       (20)      499 2023-04-03 17:04:32.000000 sageworks-0.1.5.3/.github/dependabot.yml
+-rw-r--r--   0 briford    (501) staff       (20)     1899 2023-03-25 19:33:37.000000 sageworks-0.1.5.3/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)      281 2023-03-28 23:51:00.000000 sageworks-0.1.5.3/CONTRIBUTING.md
+-rw-r--r--   0 briford    (501) staff       (20)     1080 2023-02-17 22:10:33.000000 sageworks-0.1.5.3/LICENSE
+-rw-r--r--   0 briford    (501) staff       (20)     1426 2023-04-30 02:31:13.000000 sageworks-0.1.5.3/Makefile
+-rw-r--r--   0 briford    (501) staff       (20)     6160 2023-07-13 16:19:19.656801 sageworks-0.1.5.3/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)     5427 2023-05-21 20:47:12.000000 sageworks-0.1.5.3/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)      463 2023-04-03 17:04:32.000000 sageworks-0.1.5.3/SECURITY.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.597409 sageworks-0.1.5.3/applications/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.604012 sageworks-0.1.5.3/applications/anomaly_inspector/
+-rw-r--r--   0 briford    (501) staff       (20)      181 2023-06-22 22:41:36.000000 sageworks-0.1.5.3/applications/anomaly_inspector/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)      360 2023-06-22 22:41:36.000000 sageworks-0.1.5.3/applications/anomaly_inspector/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     3251 2023-06-24 15:03:34.000000 sageworks-0.1.5.3/applications/anomaly_inspector/app.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.604309 sageworks-0.1.5.3/applications/anomaly_inspector/assets/
+-rw-r--r--   0 briford    (501) staff       (20)    12807 2023-06-22 22:41:36.000000 sageworks-0.1.5.3/applications/anomaly_inspector/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)      318 2023-06-22 22:41:36.000000 sageworks-0.1.5.3/applications/anomaly_inspector/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)     5857 2023-06-25 23:40:53.000000 sageworks-0.1.5.3/applications/anomaly_inspector/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     3686 2023-06-25 23:40:53.000000 sageworks-0.1.5.3/applications/anomaly_inspector/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)       94 2023-06-22 22:41:36.000000 sageworks-0.1.5.3/applications/anomaly_inspector/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.605276 sageworks-0.1.5.3/applications/aws_dashboard/
+-rw-r--r--   0 briford    (501) staff       (20)      181 2023-05-30 18:33:37.000000 sageworks-0.1.5.3/applications/aws_dashboard/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)      338 2023-06-19 00:15:57.000000 sageworks-0.1.5.3/applications/aws_dashboard/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1080 2023-06-26 22:31:00.000000 sageworks-0.1.5.3/applications/aws_dashboard/app.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.606019 sageworks-0.1.5.3/applications/aws_dashboard/assets/
+-rw-r--r--   0 briford    (501) staff       (20)    12861 2023-06-26 20:21:02.000000 sageworks-0.1.5.3/applications/aws_dashboard/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)      318 2023-03-21 14:30:06.000000 sageworks-0.1.5.3/applications/aws_dashboard/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)      732 2023-06-14 20:43:24.000000 sageworks-0.1.5.3/applications/aws_dashboard/assets/trash.png
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.597061 sageworks-0.1.5.3/applications/aws_dashboard/pages/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.606488 sageworks-0.1.5.3/applications/aws_dashboard/pages/data/
+-rw-r--r--   0 briford    (501) staff       (20)     1867 2023-06-19 00:14:28.000000 sageworks-0.1.5.3/applications/aws_dashboard/pages/data/toy_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)      597 2023-06-19 00:14:28.000000 sageworks-0.1.5.3/applications/aws_dashboard/pages/data/toy_scores.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.607209 sageworks-0.1.5.3/applications/aws_dashboard/pages/data_sources/
+-rw-r--r--   0 briford    (501) staff       (20)     5078 2023-06-25 23:40:53.000000 sageworks-0.1.5.3/applications/aws_dashboard/pages/data_sources/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2801 2023-06-25 23:40:53.000000 sageworks-0.1.5.3/applications/aws_dashboard/pages/data_sources/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2859 2023-06-24 15:03:34.000000 sageworks-0.1.5.3/applications/aws_dashboard/pages/data_sources/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.607717 sageworks-0.1.5.3/applications/aws_dashboard/pages/endpoints/
+-rw-r--r--   0 briford    (501) staff       (20)      928 2023-06-25 23:40:53.000000 sageworks-0.1.5.3/applications/aws_dashboard/pages/endpoints/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     1186 2023-06-19 00:14:28.000000 sageworks-0.1.5.3/applications/aws_dashboard/pages/endpoints/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1416 2023-06-19 00:14:28.000000 sageworks-0.1.5.3/applications/aws_dashboard/pages/endpoints/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.608258 sageworks-0.1.5.3/applications/aws_dashboard/pages/feature_sets/
+-rw-r--r--   0 briford    (501) staff       (20)     5056 2023-06-26 22:32:00.000000 sageworks-0.1.5.3/applications/aws_dashboard/pages/feature_sets/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2812 2023-06-25 23:40:53.000000 sageworks-0.1.5.3/applications/aws_dashboard/pages/feature_sets/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2749 2023-06-26 22:20:48.000000 sageworks-0.1.5.3/applications/aws_dashboard/pages/feature_sets/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.608953 sageworks-0.1.5.3/applications/aws_dashboard/pages/main/
+-rw-r--r--   0 briford    (501) staff       (20)     9768 2023-06-26 20:11:48.000000 sageworks-0.1.5.3/applications/aws_dashboard/pages/main/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2539 2023-06-24 15:03:34.000000 sageworks-0.1.5.3/applications/aws_dashboard/pages/main/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2652 2023-06-26 20:11:48.000000 sageworks-0.1.5.3/applications/aws_dashboard/pages/main/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.609640 sageworks-0.1.5.3/applications/aws_dashboard/pages/models/
+-rw-r--r--   0 briford    (501) staff       (20)     4836 2023-06-25 23:40:53.000000 sageworks-0.1.5.3/applications/aws_dashboard/pages/models/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2554 2023-06-14 20:43:24.000000 sageworks-0.1.5.3/applications/aws_dashboard/pages/models/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2478 2023-06-25 23:40:53.000000 sageworks-0.1.5.3/applications/aws_dashboard/pages/models/page.py
+-rw-r--r--   0 briford    (501) staff       (20)       94 2023-05-30 18:33:37.000000 sageworks-0.1.5.3/applications/aws_dashboard/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.610299 sageworks-0.1.5.3/applications/hello_world/
+-rw-r--r--   0 briford    (501) staff       (20)     3875 2023-05-31 16:41:45.000000 sageworks-0.1.5.3/applications/hello_world/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2152 2023-05-10 22:36:25.000000 sageworks-0.1.5.3/applications/hello_world/hello_world.py
+-rw-r--r--   0 briford    (501) staff       (20)     1060 2023-04-02 18:05:33.000000 sageworks-0.1.5.3/applications/hello_world/layout.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.610932 sageworks-0.1.5.3/applications/model_viewer/
+-rw-r--r--   0 briford    (501) staff       (20)     3875 2023-05-31 16:41:45.000000 sageworks-0.1.5.3/applications/model_viewer/callbacks.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.611346 sageworks-0.1.5.3/applications/model_viewer/data/
+-rw-r--r--   0 briford    (501) staff       (20)     1849 2023-03-12 02:23:08.000000 sageworks-0.1.5.3/applications/model_viewer/data/toy_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)      597 2023-03-12 02:23:08.000000 sageworks-0.1.5.3/applications/model_viewer/data/toy_scores.json
+-rw-r--r--   0 briford    (501) staff       (20)     3069 2023-04-02 18:05:33.000000 sageworks-0.1.5.3/applications/model_viewer/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2562 2023-06-25 23:40:53.000000 sageworks-0.1.5.3/applications/model_viewer/model_viewer.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.612588 sageworks-0.1.5.3/applications/outlier_inspector/
+-rw-r--r--   0 briford    (501) staff       (20)      181 2023-06-20 17:01:42.000000 sageworks-0.1.5.3/applications/outlier_inspector/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)      360 2023-06-20 18:15:46.000000 sageworks-0.1.5.3/applications/outlier_inspector/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     3386 2023-06-27 17:36:09.000000 sageworks-0.1.5.3/applications/outlier_inspector/app.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.613058 sageworks-0.1.5.3/applications/outlier_inspector/assets/
+-rw-r--r--   0 briford    (501) staff       (20)    12861 2023-06-26 18:18:41.000000 sageworks-0.1.5.3/applications/outlier_inspector/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)      318 2023-06-20 17:01:42.000000 sageworks-0.1.5.3/applications/outlier_inspector/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)     5726 2023-06-25 23:40:53.000000 sageworks-0.1.5.3/applications/outlier_inspector/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     3687 2023-06-25 23:40:53.000000 sageworks-0.1.5.3/applications/outlier_inspector/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)       94 2023-06-20 17:01:42.000000 sageworks-0.1.5.3/applications/outlier_inspector/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.613874 sageworks-0.1.5.3/applications/web_admin/
+-rw-r--r--   0 briford    (501) staff       (20)      213 2023-04-02 18:05:33.000000 sageworks-0.1.5.3/applications/web_admin/flask_test.py
+-rw-r--r--   0 briford    (501) staff       (20)      201 2023-03-03 22:18:34.000000 sageworks-0.1.5.3/applications/web_admin/hello-world-http-test.ini
+-rw-r--r--   0 briford    (501) staff       (20)      235 2023-03-03 22:19:17.000000 sageworks-0.1.5.3/applications/web_admin/hello-world.ini
+-rw-r--r--   0 briford    (501) staff       (20)      399 2023-03-03 22:20:51.000000 sageworks-0.1.5.3/applications/web_admin/hello-world.service
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.614107 sageworks-0.1.5.3/applications/web_admin/nginx_conf/
+-rw-r--r--   0 briford    (501) staff       (20)      486 2023-03-03 22:17:39.000000 sageworks-0.1.5.3/applications/web_admin/nginx_conf/nginx.conf
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.614769 sageworks-0.1.5.3/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     3315 2023-05-05 02:30:09.000000 sageworks-0.1.5.3/aws_setup/aws_account_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     1399 2023-05-23 20:50:24.000000 sageworks-0.1.5.3/aws_setup/aws_identity_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     4338 2023-05-23 16:47:14.000000 sageworks-0.1.5.3/aws_setup/build_ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.616202 sageworks-0.1.5.3/aws_setup/sageworks_cdk/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-04-20 17:45:20.000000 sageworks-0.1.5.3/aws_setup/sageworks_cdk/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1028 2023-04-30 02:31:15.000000 sageworks-0.1.5.3/aws_setup/sageworks_cdk/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1291 2023-04-30 16:18:03.000000 sageworks-0.1.5.3/aws_setup/sageworks_cdk/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     1998 2023-04-20 17:45:20.000000 sageworks-0.1.5.3/aws_setup/sageworks_cdk/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-04-20 17:45:20.000000 sageworks-0.1.5.3/aws_setup/sageworks_cdk/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       70 2023-04-30 17:09:37.000000 sageworks-0.1.5.3/aws_setup/sageworks_cdk/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-04-20 17:45:20.000000 sageworks-0.1.5.3/aws_setup/sageworks_cdk/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.616442 sageworks-0.1.5.3/aws_setup/sageworks_cdk/stacks/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.3/aws_setup/sageworks_cdk/stacks/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2304 2023-05-05 02:30:09.000000 sageworks-0.1.5.3/aws_setup/sageworks_cdk/stacks/sageworks_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.616618 sageworks-0.1.5.3/aws_setup/sageworks_cdk/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.3/aws_setup/sageworks_cdk/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.616790 sageworks-0.1.5.3/aws_setup/sageworks_cdk/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.3/aws_setup/sageworks_cdk/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      720 2023-04-30 02:31:15.000000 sageworks-0.1.5.3/aws_setup/sageworks_cdk/tests/unit/test_sageworks_sandbox_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.616987 sageworks-0.1.5.3/config/
+-rw-r--r--   0 briford    (501) staff       (20)      147 2023-04-30 02:43:00.000000 sageworks-0.1.5.3/config/sageworks_config.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.618035 sageworks-0.1.5.3/data/
+-rw-r--r--   0 briford    (501) staff       (20)   196156 2023-03-26 18:42:12.000000 sageworks-0.1.5.3/data/abalone.csv
+-rw-r--r--   0 briford    (501) staff       (20)     1515 2023-06-23 23:19:28.000000 sageworks-0.1.5.3/data/test_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)     2270 2023-04-19 19:55:29.000000 sageworks-0.1.5.3/data/test_data.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.618657 sageworks-0.1.5.3/docs/
+-rw-r--r--   0 briford    (501) staff       (20)     1770 2023-05-09 15:36:49.000000 sageworks-0.1.5.3/docs/admin_notes.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.623823 sageworks-0.1.5.3/docs/images/
+-rw-r--r--   0 briford    (501) staff       (20)   605827 2022-12-06 17:43:49.000000 sageworks-0.1.5.3/docs/images/big_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)    32320 2023-01-15 22:00:05.000000 sageworks-0.1.5.3/docs/images/graph_representation.png
+-rw-r--r--   0 briford    (501) staff       (20)    15549 2023-03-06 20:35:02.000000 sageworks-0.1.5.3/docs/images/powered_aws_dark_blue.png
+-rw-r--r--   0 briford    (501) staff       (20)    10003 2023-03-06 20:33:32.000000 sageworks-0.1.5.3/docs/images/powered_aws_transparent.png
+-rw-r--r--   0 briford    (501) staff       (20)     6435 2023-03-06 20:31:13.000000 sageworks-0.1.5.3/docs/images/powered_aws_white.png
+-rw-r--r--   0 briford    (501) staff       (20)    21174 2023-03-06 20:40:25.000000 sageworks-0.1.5.3/docs/images/powered_aws_with_tm_grey.png
+-rw-r--r--   0 briford    (501) staff       (20)    51137 2023-01-15 21:19:16.000000 sageworks-0.1.5.3/docs/images/sageworks.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-03-10 19:48:12.000000 sageworks-0.1.5.3/docs/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)    30017 2023-01-15 21:23:57.000000 sageworks-0.1.5.3/docs/images/scp.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-01-12 16:00:43.000000 sageworks-0.1.5.3/docs/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)   381209 2022-12-06 17:43:49.000000 sageworks-0.1.5.3/docs/images/small_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)      667 2023-03-15 14:00:32.000000 sageworks-0.1.5.3/docs/sageworks_classes_concepts.md
+-rw-r--r--   0 briford    (501) staff       (20)     1873 2023-03-13 14:45:22.000000 sageworks-0.1.5.3/docs/scp_consulting.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.624621 sageworks-0.1.5.3/examples/
+-rw-r--r--   0 briford    (501) staff       (20)     1240 2023-04-02 18:05:33.000000 sageworks-0.1.5.3/examples/data_to_data_example.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.624874 sageworks-0.1.5.3/notebooks/
+-rw-r--r--   0 briford    (501) staff       (20)   236926 2023-05-06 21:30:24.000000 sageworks-0.1.5.3/notebooks/ML_Pipeline_with_SageWorks.ipynb
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.629285 sageworks-0.1.5.3/notebooks/images/
+-rw-r--r--   0 briford    (501) staff       (20)   142099 2023-04-14 22:52:23.000000 sageworks-0.1.5.3/notebooks/images/athena_query_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   191022 2023-04-14 22:50:14.000000 sageworks-0.1.5.3/notebooks/images/aws_dashboard_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   222686 2023-04-14 23:47:56.000000 sageworks-0.1.5.3/notebooks/images/dashboard_aqsol_features.png
+-rw-r--r--   0 briford    (501) staff       (20)   171441 2023-04-15 00:30:02.000000 sageworks-0.1.5.3/notebooks/images/model_screenshot.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-04-15 16:18:02.000000 sageworks-0.1.5.3/notebooks/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-04-15 16:17:49.000000 sageworks-0.1.5.3/notebooks/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)      224 2023-05-24 23:05:26.000000 sageworks-0.1.5.3/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.633643 sageworks-0.1.5.3/scripts/
+-rw-r--r--   0 briford    (501) staff       (20)     1373 2023-04-09 21:27:30.000000 sageworks-0.1.5.3/scripts/data_source_tags.py
+-rw-r--r--   0 briford    (501) staff       (20)      998 2023-06-25 23:40:53.000000 sageworks-0.1.5.3/scripts/dns_data_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     1717 2023-06-25 23:40:53.000000 sageworks-0.1.5.3/scripts/generate_jsonl_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     1306 2023-04-09 21:27:30.000000 sageworks-0.1.5.3/scripts/list_data_sources.py
+-rw-r--r--   0 briford    (501) staff       (20)      527 2023-07-13 16:19:19.657139 sageworks-0.1.5.3/setup.cfg
+-rw-r--r--   0 briford    (501) staff       (20)     1836 2023-07-13 16:18:50.000000 sageworks-0.1.5.3/setup.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.598423 sageworks-0.1.5.3/src/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.633877 sageworks-0.1.5.3/src/sageworks/
+-rw-r--r--   0 briford    (501) staff       (20)      853 2023-04-22 21:03:48.000000 sageworks-0.1.5.3/src/sageworks/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.634828 sageworks-0.1.5.3/src/sageworks/algorithms/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.3/src/sageworks/algorithms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.598631 sageworks-0.1.5.3/src/sageworks/algorithms/graph/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.634927 sageworks-0.1.5.3/src/sageworks/algorithms/graph/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)       96 2023-03-05 20:00:31.000000 sageworks-0.1.5.3/src/sageworks/algorithms/graph/heavy/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.635169 sageworks-0.1.5.3/src/sageworks/algorithms/graph/light/
+-rw-r--r--   0 briford    (501) staff       (20)      122 2023-03-05 19:59:59.000000 sageworks-0.1.5.3/src/sageworks/algorithms/graph/light/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.598788 sageworks-0.1.5.3/src/sageworks/algorithms/table/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.635402 sageworks-0.1.5.3/src/sageworks/algorithms/table/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)      169 2023-03-05 20:04:10.000000 sageworks-0.1.5.3/src/sageworks/algorithms/table/heavy/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.636363 sageworks-0.1.5.3/src/sageworks/algorithms/table/light/
+-rw-r--r--   0 briford    (501) staff       (20)       95 2023-03-05 20:05:08.000000 sageworks-0.1.5.3/src/sageworks/algorithms/table/light/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     1751 2023-04-05 21:18:09.000000 sageworks-0.1.5.3/src/sageworks/algorithms/table/light/data_source_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)     9476 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/algorithms/table/light/feature_spider.py
+-rw-r--r--   0 briford    (501) staff       (20)     4186 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/algorithms/table/light/row_tagger.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.636944 sageworks-0.1.5.3/src/sageworks/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      639 2023-03-05 21:06:58.000000 sageworks-0.1.5.3/src/sageworks/artifacts/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-01 03:28:03.000000 sageworks-0.1.5.3/src/sageworks/artifacts/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     6294 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/artifacts/artifact.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.638057 sageworks-0.1.5.3/src/sageworks/artifacts/data_sources/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.3/src/sageworks/artifacts/data_sources/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    24977 2023-07-13 14:20:01.000000 sageworks-0.1.5.3/src/sageworks/artifacts/data_sources/athena_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     3381 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/artifacts/data_sources/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     3509 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/artifacts/data_sources/data_source_abstract.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.638431 sageworks-0.1.5.3/src/sageworks/artifacts/endpoints/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.3/src/sageworks/artifacts/endpoints/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     9808 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/artifacts/endpoints/endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.638857 sageworks-0.1.5.3/src/sageworks/artifacts/feature_sets/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.3/src/sageworks/artifacts/feature_sets/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    16069 2023-06-26 21:12:04.000000 sageworks-0.1.5.3/src/sageworks/artifacts/feature_sets/feature_set.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.639212 sageworks-0.1.5.3/src/sageworks/artifacts/models/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.3/src/sageworks/artifacts/models/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     4423 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/artifacts/models/model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.639749 sageworks-0.1.5.3/src/sageworks/aws_service_broker/
+-rw-r--r--   0 briford    (501) staff       (20)     7997 2023-06-26 17:40:01.000000 sageworks-0.1.5.3/src/sageworks/aws_service_broker/aws_account_clamp.py
+-rw-r--r--   0 briford    (501) staff       (20)     9818 2023-07-03 15:14:53.000000 sageworks-0.1.5.3/src/sageworks/aws_service_broker/aws_service_broker.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.641340 sageworks-0.1.5.3/src/sageworks/aws_service_broker/aws_service_connectors/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-14 19:44:44.000000 sageworks-0.1.5.3/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2237 2023-05-28 16:44:16.000000 sageworks-0.1.5.3/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
+-rw-r--r--   0 briford    (501) staff       (20)     3919 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)     3007 2023-05-28 16:41:24.000000 sageworks-0.1.5.3/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)     5440 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)     3726 2023-06-24 15:03:34.000000 sageworks-0.1.5.3/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py
+-rw-r--r--   0 briford    (501) staff       (20)     3820 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     3715 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.641545 sageworks-0.1.5.3/src/sageworks/cli/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-05-24 23:05:26.000000 sageworks-0.1.5.3/src/sageworks/cli/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2226 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/cli/cli.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.641978 sageworks-0.1.5.3/src/sageworks/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)     1432 2023-03-17 17:39:22.000000 sageworks-0.1.5.3/src/sageworks/transforms/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.3/src/sageworks/transforms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.599477 sageworks-0.1.5.3/src/sageworks/transforms/data_loaders/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.642221 sageworks-0.1.5.3/src/sageworks/transforms/data_loaders/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)     8493 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.642732 sageworks-0.1.5.3/src/sageworks/transforms/data_loaders/light/
+-rw-r--r--   0 briford    (501) staff       (20)     2997 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2483 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/transforms/data_loaders/light/json_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     4155 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.642970 sageworks-0.1.5.3/src/sageworks/transforms/data_to_data/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.3/src/sageworks/transforms/data_to_data/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.643056 sageworks-0.1.5.3/src/sageworks/transforms/data_to_data/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.3/src/sageworks/transforms/data_to_data/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.643141 sageworks-0.1.5.3/src/sageworks/transforms/data_to_data/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:15:48.000000 sageworks-0.1.5.3/src/sageworks/transforms/data_to_data/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.643348 sageworks-0.1.5.3/src/sageworks/transforms/data_to_data/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:16:45.000000 sageworks-0.1.5.3/src/sageworks/transforms/data_to_data/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.643793 sageworks-0.1.5.3/src/sageworks/transforms/data_to_data/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.3/src/sageworks/transforms/data_to_data/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2231 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/transforms/data_to_data/light/clean_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     2298 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/transforms/data_to_data/light/data_to_data_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.643927 sageworks-0.1.5.3/src/sageworks/transforms/data_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.3/src/sageworks/transforms/data_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.644015 sageworks-0.1.5.3/src/sageworks/transforms/data_to_features/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.3/src/sageworks/transforms/data_to_features/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.644116 sageworks-0.1.5.3/src/sageworks/transforms/data_to_features/heavy/chunk/
+-rw-r--r--   0 briford    (501) staff       (20)     3941 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.644243 sageworks-0.1.5.3/src/sageworks/transforms/data_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:14.000000 sageworks-0.1.5.3/src/sageworks/transforms/data_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.644476 sageworks-0.1.5.3/src/sageworks/transforms/data_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:14.000000 sageworks-0.1.5.3/src/sageworks/transforms/data_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.644727 sageworks-0.1.5.3/src/sageworks/transforms/data_to_features/heavy/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     6644 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.645196 sageworks-0.1.5.3/src/sageworks/transforms/data_to_features/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.3/src/sageworks/transforms/data_to_features/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3307 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/transforms/data_to_features/light/data_to_features_light.py
+-rw-r--r--   0 briford    (501) staff       (20)     2974 2023-05-12 17:46:07.000000 sageworks-0.1.5.3/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.645421 sageworks-0.1.5.3/src/sageworks/transforms/features_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 18:06:15.000000 sageworks-0.1.5.3/src/sageworks/transforms/features_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.600395 sageworks-0.1.5.3/src/sageworks/transforms/features_to_features/heavy/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.645527 sageworks-0.1.5.3/src/sageworks/transforms/features_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:46.000000 sageworks-0.1.5.3/src/sageworks/transforms/features_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.645778 sageworks-0.1.5.3/src/sageworks/transforms/features_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:46.000000 sageworks-0.1.5.3/src/sageworks/transforms/features_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.646047 sageworks-0.1.5.3/src/sageworks/transforms/features_to_model/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.3/src/sageworks/transforms/features_to_model/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7713 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/transforms/features_to_model/features_to_model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.646546 sageworks-0.1.5.3/src/sageworks/transforms/features_to_model/light_model_harness/
+-rw-r--r--   0 briford    (501) staff       (20)        8 2023-03-25 02:07:31.000000 sageworks-0.1.5.3/src/sageworks/transforms/features_to_model/light_model_harness/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)     5179 2023-04-18 16:01:35.000000 sageworks-0.1.5.3/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.646903 sageworks-0.1.5.3/src/sageworks/transforms/model_to_endpoint/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.3/src/sageworks/transforms/model_to_endpoint/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2760 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.647983 sageworks-0.1.5.3/src/sageworks/transforms/pandas_transforms/
+-rw-r--r--   0 briford    (501) staff       (20)     2745 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/transforms/pandas_transforms/data_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     3144 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/transforms/pandas_transforms/features_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     7003 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/transforms/pandas_transforms/pandas_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)    14106 2023-06-26 21:12:04.000000 sageworks-0.1.5.3/src/sageworks/transforms/pandas_transforms/pandas_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     3913 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/transforms/pandas_transforms/pandas_to_features_chunked.py
+-rw-r--r--   0 briford    (501) staff       (20)    10506 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/transforms/pandas_transforms/pandas_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     6715 2023-06-26 21:13:00.000000 sageworks-0.1.5.3/src/sageworks/transforms/transform.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.650006 sageworks-0.1.5.3/src/sageworks/utils/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 02:34:19.000000 sageworks-0.1.5.3/src/sageworks/utils/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3962 2023-04-30 02:31:13.000000 sageworks-0.1.5.3/src/sageworks/utils/cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     5113 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/utils/df_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     2417 2023-05-14 17:23:33.000000 sageworks-0.1.5.3/src/sageworks/utils/iso_8601.py
+-rw-r--r--   0 briford    (501) staff       (20)     6615 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/utils/redis_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     3618 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/utils/sageworks_config.py
+-rw-r--r--   0 briford    (501) staff       (20)     3558 2023-04-12 15:59:21.000000 sageworks-0.1.5.3/src/sageworks/utils/sageworks_event_bridge.py
+-rw-r--r--   0 briford    (501) staff       (20)      529 2023-05-23 21:37:21.000000 sageworks-0.1.5.3/src/sageworks/utils/sageworks_logging.py
+-rw-r--r--   0 briford    (501) staff       (20)     2209 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/utils/sageworks_sqs.py
+-rw-r--r--   0 briford    (501) staff       (20)     1469 2023-05-15 01:49:43.000000 sageworks-0.1.5.3/src/sageworks/utils/type_abbrev.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.651348 sageworks-0.1.5.3/src/sageworks/views/
+-rw-r--r--   0 briford    (501) staff       (20)    15068 2023-07-03 15:00:27.000000 sageworks-0.1.5.3/src/sageworks/views/artifacts_text_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     5041 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/views/artifacts_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     4633 2023-06-26 21:05:35.000000 sageworks-0.1.5.3/src/sageworks/views/data_source_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     4996 2023-06-26 21:09:32.000000 sageworks-0.1.5.3/src/sageworks/views/feature_set_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     2008 2023-05-23 20:04:12.000000 sageworks-0.1.5.3/src/sageworks/views/model_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     1296 2023-04-19 17:02:05.000000 sageworks-0.1.5.3/src/sageworks/views/view.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.653962 sageworks-0.1.5.3/src/sageworks/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)      837 2023-06-26 17:57:01.000000 sageworks-0.1.5.3/src/sageworks/web_components/color_maps.py
+-rw-r--r--   0 briford    (501) staff       (20)     1661 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/web_components/confusion_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     2469 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/web_components/data_and_feature_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     4039 2023-06-27 18:25:38.000000 sageworks-0.1.5.3/src/sageworks/web_components/distribution_plots.py
+-rw-r--r--   0 briford    (501) staff       (20)     1182 2023-04-07 23:04:10.000000 sageworks-0.1.5.3/src/sageworks/web_components/histogram.py
+-rw-r--r--   0 briford    (501) staff       (20)      837 2023-04-09 21:27:30.000000 sageworks-0.1.5.3/src/sageworks/web_components/line_chart.py
+-rw-r--r--   0 briford    (501) staff       (20)     1247 2023-04-09 21:27:30.000000 sageworks-0.1.5.3/src/sageworks/web_components/mock_feature_details.py
+-rw-r--r--   0 briford    (501) staff       (20)      815 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/web_components/mock_feature_importance.py
+-rw-r--r--   0 briford    (501) staff       (20)     1507 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/web_components/mock_model_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     1703 2023-06-25 23:40:21.000000 sageworks-0.1.5.3/src/sageworks/web_components/mock_model_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2300 2023-06-26 19:16:17.000000 sageworks-0.1.5.3/src/sageworks/web_components/scatter_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     4858 2023-06-27 20:10:00.000000 sageworks-0.1.5.3/src/sageworks/web_components/table.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.634725 sageworks-0.1.5.3/src/sageworks.egg-info/
+-rw-r--r--   0 briford    (501) staff       (20)     6160 2023-07-13 16:19:19.000000 sageworks-0.1.5.3/src/sageworks.egg-info/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)    10096 2023-07-13 16:19:19.000000 sageworks-0.1.5.3/src/sageworks.egg-info/SOURCES.txt
+-rw-r--r--   0 briford    (501) staff       (20)        1 2023-07-13 16:19:19.000000 sageworks-0.1.5.3/src/sageworks.egg-info/dependency_links.txt
+-rw-r--r--   0 briford    (501) staff       (20)       52 2023-07-13 16:19:19.000000 sageworks-0.1.5.3/src/sageworks.egg-info/entry_points.txt
+-rw-r--r--   0 briford    (501) staff       (20)      213 2023-07-13 16:19:19.000000 sageworks-0.1.5.3/src/sageworks.egg-info/requires.txt
+-rw-r--r--   0 briford    (501) staff       (20)       10 2023-07-13 16:19:19.000000 sageworks-0.1.5.3/src/sageworks.egg-info/top_level.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.654202 sageworks-0.1.5.3/tests/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.655050 sageworks-0.1.5.3/tests/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)     1258 2023-05-29 15:53:07.000000 sageworks-0.1.5.3/tests/artifacts/data_source_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1483 2023-04-11 20:37:15.000000 sageworks-0.1.5.3/tests/artifacts/endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1163 2023-05-29 15:53:07.000000 sageworks-0.1.5.3/tests/artifacts/feature_set_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      799 2023-04-02 18:05:33.000000 sageworks-0.1.5.3/tests/artifacts/model_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.655489 sageworks-0.1.5.3/tests/aws_account/
+-rw-r--r--   0 briford    (501) staff       (20)     1105 2023-05-05 02:37:56.000000 sageworks-0.1.5.3/tests/aws_account/aws_account_clamp_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      642 2023-05-05 02:38:20.000000 sageworks-0.1.5.3/tests/aws_account/aws_service_broker_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     3341 2023-04-19 17:23:07.000000 sageworks-0.1.5.3/tests/create_sageworks_objs_for_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-07-13 16:19:19.656489 sageworks-0.1.5.3/tests/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      554 2023-05-12 17:46:18.000000 sageworks-0.1.5.3/tests/transforms/data_to_data_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      682 2023-05-20 23:13:06.000000 sageworks-0.1.5.3/tests/transforms/data_to_features_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      655 2023-05-12 18:01:20.000000 sageworks-0.1.5.3/tests/transforms/features_to_model_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      642 2023-05-12 17:46:18.000000 sageworks-0.1.5.3/tests/transforms/model_to_endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      628 2023-05-12 17:46:18.000000 sageworks-0.1.5.3/tests/transforms/pandas_to_data_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      729 2023-05-05 02:35:30.000000 sageworks-0.1.5.3/tox.ini
```

### Comparing `sageworks-0.1.5.2/.gitignore` & `sageworks-0.1.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/LICENSE` & `sageworks-0.1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/Makefile` & `sageworks-0.1.5.3/Makefile`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/PKG-INFO` & `sageworks-0.1.5.3/Readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,23 @@
-Metadata-Version: 2.1
-Name: sageworks
-Version: 0.1.5.2
-Summary: SageWorks: A Python WorkBench for creating and deploying SageMaker Models
-Home-page: https://github.com/SuperCowPowers/sageworks
-Author: SuperCowPowers LLC
-Author-email: support@supercowpowers.com
-License: MIT
-Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <img align="left" src="docs/images/scp.png" width="180">
 
 # SageWorks<sup><i>TM</i></sup>
 
+<p align="center">
 <img height="360" align="left" src="https://user-images.githubusercontent.com/4806709/236641571-fc38899a-8b92-4b7c-80a0-cc9d39b92e4a.png">
 <img height="360" aligh="right" src="https://user-images.githubusercontent.com/4806709/236641581-51777977-bca4-4af3-8bec-fb1758c964b8.png">
+</p>
 
 #### SageWorks: The scientist's workbench powered by AWS® for scalability, flexibility, and security.
 
 SageWorks is a medium granularity framework that manages and aggregates AWS® Services into classes and concepts. When you use SageWorks you think about **DataSources**, **FeatureSets**, **Models**, and **Endpoints**. Underneath the hood those classes handle all the details around updating and managing a **complex set of AWS Services**. All the power and none of the pain so that your team can **Do Science Faster!**
 
-<img src="docs/images/sageworks_concepts.png">
+<p align="center">
+<img width="800" src="docs/images/sageworks_concepts.png">
+</p>
 
 ### Full SageWorks OverView
 [SageWorks Architected FrameWork](https://docs.google.com/presentation/d/1ZiSy4ulEx5gfNQS76yRv8vgkehJ9gXRJ1PulutLKzis/edit?usp=sharing)
 
 
 ## Why SageWorks?
 
@@ -42,23 +28,27 @@
 - SageWorks provides **visibility** and **transparency** into AWS SageMaker® Pipelines
     - What S3 data sources are getting pulled?
     - What Features Store/Group is the Model Using?
     - What's the ***Provenance*** of a Model in Model Registry?
     - What SageMaker Endpoints are associated with this model?
 
 
-**Single pane of glass** visibility into the AWS Services that underpin the SageWorks Classes. We can see that SageWorks automatically tags and tracks the inputs of all artifacts providing 'data provenance' for all steps in the AWS modeling pipeline.
+### Single Pane of Glass
+Visibility into the AWS Services that underpin the SageWorks Classes. We can see that SageWorks automatically tags and tracks the inputs of all artifacts providing 'data provenance' for all steps in the AWS modeling pipeline.
 
-<img width="1000" alt="Screenshot 2023-03-31 at 2 16 36 PM" src="https://user-images.githubusercontent.com/4806709/229222245-59e342c1-7254-47de-a453-268448643143.png">
+<p align="center">
+<img width="800" alt="Top Dashboard" src="https://github.com/SuperCowPowers/sageworks/assets/4806709/c4a7f054-e640-407c-9e5c-f9d3ea1bd717.png">
+</p>
 
 <i><b> Clearly illustrated:</b> SageWorks provides intuitive and transparent visibility into the full pipeline of your AWS Sagemaker Deployments.</i>
 
 
 ## Getting Started
 - [SageWorks Overview](https://docs.google.com/presentation/d/1ZiSy4ulEx5gfNQS76yRv8vgkehJ9gXRJ1PulutLKzis/edit?usp=sharing) Slides that cover and illustrate the SageWorks Modeling Pipeline.
+- [SageWorks Docs/Wiki](https://github.com/SuperCowPowers/sageworks/wiki) Our general documentation for getting started with SageWorks.
 - [SageWorks AWS Onboarding](https://github.com/SuperCowPowers/sageworks/wiki/Onboarding-SageWorks-to-AWS) Deploy the SageWorks Stack to your AWS Account. 
 - [Notebook: Start to Finish AWS ML Pipeline](https://nbviewer.org/github/SuperCowPowers/sageworks/blob/main/notebooks/ML_Pipeline_with_SageWorks.ipynb) Building an AWS® ML Pipeline from start to finish.
 - [Video: Coding with SageWorks](https://drive.google.com/file/d/1iO7IuQtTYdx4BtQjxv9lI1aVJ2ZcAo43/view?usp=sharing) Informal coding + chatting while building a full ML pipeline.
 - Join our [Discord](https://discord.gg/WHAJuz8sw8) for questions and advice on using SageWorks within your organization.
 
 ### SageWorks Zen
 - The AWS SageMaker® set of services is vast and **complex**.
```

### Comparing `sageworks-0.1.5.2/Readme.md` & `sageworks-0.1.5.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,41 @@
+Metadata-Version: 2.1
+Name: sageworks
+Version: 0.1.5.3
+Summary: SageWorks: A Python WorkBench for creating and deploying SageMaker Models
+Home-page: https://github.com/SuperCowPowers/sageworks
+Author: SuperCowPowers LLC
+Author-email: support@supercowpowers.com
+License: MIT
+Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <img align="left" src="docs/images/scp.png" width="180">
 
 # SageWorks<sup><i>TM</i></sup>
 
+<p align="center">
 <img height="360" align="left" src="https://user-images.githubusercontent.com/4806709/236641571-fc38899a-8b92-4b7c-80a0-cc9d39b92e4a.png">
 <img height="360" aligh="right" src="https://user-images.githubusercontent.com/4806709/236641581-51777977-bca4-4af3-8bec-fb1758c964b8.png">
+</p>
 
 #### SageWorks: The scientist's workbench powered by AWS® for scalability, flexibility, and security.
 
 SageWorks is a medium granularity framework that manages and aggregates AWS® Services into classes and concepts. When you use SageWorks you think about **DataSources**, **FeatureSets**, **Models**, and **Endpoints**. Underneath the hood those classes handle all the details around updating and managing a **complex set of AWS Services**. All the power and none of the pain so that your team can **Do Science Faster!**
 
-<img src="docs/images/sageworks_concepts.png">
+<p align="center">
+<img width="800" src="docs/images/sageworks_concepts.png">
+</p>
 
 ### Full SageWorks OverView
 [SageWorks Architected FrameWork](https://docs.google.com/presentation/d/1ZiSy4ulEx5gfNQS76yRv8vgkehJ9gXRJ1PulutLKzis/edit?usp=sharing)
 
 
 ## Why SageWorks?
 
@@ -24,23 +46,27 @@
 - SageWorks provides **visibility** and **transparency** into AWS SageMaker® Pipelines
     - What S3 data sources are getting pulled?
     - What Features Store/Group is the Model Using?
     - What's the ***Provenance*** of a Model in Model Registry?
     - What SageMaker Endpoints are associated with this model?
 
 
-**Single pane of glass** visibility into the AWS Services that underpin the SageWorks Classes. We can see that SageWorks automatically tags and tracks the inputs of all artifacts providing 'data provenance' for all steps in the AWS modeling pipeline.
+### Single Pane of Glass
+Visibility into the AWS Services that underpin the SageWorks Classes. We can see that SageWorks automatically tags and tracks the inputs of all artifacts providing 'data provenance' for all steps in the AWS modeling pipeline.
 
-<img width="1000" alt="Screenshot 2023-03-31 at 2 16 36 PM" src="https://user-images.githubusercontent.com/4806709/229222245-59e342c1-7254-47de-a453-268448643143.png">
+<p align="center">
+<img width="800" alt="Top Dashboard" src="https://github.com/SuperCowPowers/sageworks/assets/4806709/c4a7f054-e640-407c-9e5c-f9d3ea1bd717.png">
+</p>
 
 <i><b> Clearly illustrated:</b> SageWorks provides intuitive and transparent visibility into the full pipeline of your AWS Sagemaker Deployments.</i>
 
 
 ## Getting Started
 - [SageWorks Overview](https://docs.google.com/presentation/d/1ZiSy4ulEx5gfNQS76yRv8vgkehJ9gXRJ1PulutLKzis/edit?usp=sharing) Slides that cover and illustrate the SageWorks Modeling Pipeline.
+- [SageWorks Docs/Wiki](https://github.com/SuperCowPowers/sageworks/wiki) Our general documentation for getting started with SageWorks.
 - [SageWorks AWS Onboarding](https://github.com/SuperCowPowers/sageworks/wiki/Onboarding-SageWorks-to-AWS) Deploy the SageWorks Stack to your AWS Account. 
 - [Notebook: Start to Finish AWS ML Pipeline](https://nbviewer.org/github/SuperCowPowers/sageworks/blob/main/notebooks/ML_Pipeline_with_SageWorks.ipynb) Building an AWS® ML Pipeline from start to finish.
 - [Video: Coding with SageWorks](https://drive.google.com/file/d/1iO7IuQtTYdx4BtQjxv9lI1aVJ2ZcAo43/view?usp=sharing) Informal coding + chatting while building a full ML pipeline.
 - Join our [Discord](https://discord.gg/WHAJuz8sw8) for questions and advice on using SageWorks within your organization.
 
 ### SageWorks Zen
 - The AWS SageMaker® set of services is vast and **complex**.
```

### Comparing `sageworks-0.1.5.2/applications/aws_dashboard/assets/custom.css` & `sageworks-0.1.5.3/applications/aws_dashboard/assets/custom.css`

 * *Files 11% similar despite different names*

```diff
@@ -37,141 +37,284 @@
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 .container {
   position: relative;
   width: 100%;
   max-width: 960px;
   margin: 0 auto;
   padding: 0 20px;
-  box-sizing: border-box; }
+  box-sizing: border-box;
+}
+
 .column,
 .columns {
   width: 100%;
   float: left;
-  box-sizing: border-box; }
+  box-sizing: border-box;
+}
 
 /* For devices larger than 400px */
 @media (min-width: 400px) {
   .container {
     width: 85%;
-    padding: 0; }
+    padding: 0;
+  }
 }
 
 /* For devices larger than 550px */
 @media (min-width: 550px) {
   .container {
-    width: 80%; }
+    width: 80%;
+  }
+
   .column,
   .columns {
-    margin-left: 4%; }
+    margin-left: 4%;
+  }
+
   .column:first-child,
   .columns:first-child {
-    margin-left: 0; }
+    margin-left: 0;
+  }
 
   .one.column,
-  .one.columns                    { width: 4.66666666667%; }
-  .two.columns                    { width: 13.3333333333%; }
-  .three.columns                  { width: 22%;            }
-  .four.columns                   { width: 30.6666666667%; }
-  .five.columns                   { width: 39.3333333333%; }
-  .six.columns                    { width: 48%;            }
-  .seven.columns                  { width: 56.6666666667%; }
-  .eight.columns                  { width: 65.3333333333%; }
-  .nine.columns                   { width: 74.0%;          }
-  .ten.columns                    { width: 82.6666666667%; }
-  .eleven.columns                 { width: 91.3333333333%; }
-  .twelve.columns                 { width: 100%; margin-left: 0; }
-
-  .one-third.column               { width: 30.6666666667%; }
-  .two-thirds.column              { width: 65.3333333333%; }
-
-  .one-half.column                { width: 48%; }
+  .one.columns {
+    width: 4.66666666667%;
+  }
+
+  .two.columns {
+    width: 13.3333333333%;
+  }
+
+  .three.columns {
+    width: 22%;
+  }
+
+  .four.columns {
+    width: 30.6666666667%;
+  }
+
+  .five.columns {
+    width: 39.3333333333%;
+  }
+
+  .six.columns {
+    width: 48%;
+  }
+
+  .seven.columns {
+    width: 56.6666666667%;
+  }
+
+  .eight.columns {
+    width: 65.3333333333%;
+  }
+
+  .nine.columns {
+    width: 74.0%;
+  }
+
+  .ten.columns {
+    width: 82.6666666667%;
+  }
+
+  .eleven.columns {
+    width: 91.3333333333%;
+  }
+
+  .twelve.columns {
+    width: 100%;
+    margin-left: 0;
+  }
+
+  .one-third.column {
+    width: 30.6666666667%;
+  }
+
+  .two-thirds.column {
+    width: 65.3333333333%;
+  }
+
+  .one-half.column {
+    width: 48%;
+  }
 
   /* Offsets */
   .offset-by-one.column,
-  .offset-by-one.columns          { margin-left: 8.66666666667%; }
+  .offset-by-one.columns {
+    margin-left: 8.66666666667%;
+  }
+
   .offset-by-two.column,
-  .offset-by-two.columns          { margin-left: 17.3333333333%; }
+  .offset-by-two.columns {
+    margin-left: 17.3333333333%;
+  }
+
   .offset-by-three.column,
-  .offset-by-three.columns        { margin-left: 26%;            }
+  .offset-by-three.columns {
+    margin-left: 26%;
+  }
+
   .offset-by-four.column,
-  .offset-by-four.columns         { margin-left: 34.6666666667%; }
+  .offset-by-four.columns {
+    margin-left: 34.6666666667%;
+  }
+
   .offset-by-five.column,
-  .offset-by-five.columns         { margin-left: 43.3333333333%; }
+  .offset-by-five.columns {
+    margin-left: 43.3333333333%;
+  }
+
   .offset-by-six.column,
-  .offset-by-six.columns          { margin-left: 52%;            }
+  .offset-by-six.columns {
+    margin-left: 52%;
+  }
+
   .offset-by-seven.column,
-  .offset-by-seven.columns        { margin-left: 60.6666666667%; }
+  .offset-by-seven.columns {
+    margin-left: 60.6666666667%;
+  }
+
   .offset-by-eight.column,
-  .offset-by-eight.columns        { margin-left: 69.3333333333%; }
+  .offset-by-eight.columns {
+    margin-left: 69.3333333333%;
+  }
+
   .offset-by-nine.column,
-  .offset-by-nine.columns         { margin-left: 78.0%;          }
+  .offset-by-nine.columns {
+    margin-left: 78.0%;
+  }
+
   .offset-by-ten.column,
-  .offset-by-ten.columns          { margin-left: 86.6666666667%; }
+  .offset-by-ten.columns {
+    margin-left: 86.6666666667%;
+  }
+
   .offset-by-eleven.column,
-  .offset-by-eleven.columns       { margin-left: 95.3333333333%; }
+  .offset-by-eleven.columns {
+    margin-left: 95.3333333333%;
+  }
 
   .offset-by-one-third.column,
-  .offset-by-one-third.columns    { margin-left: 34.6666666667%; }
+  .offset-by-one-third.columns {
+    margin-left: 34.6666666667%;
+  }
+
   .offset-by-two-thirds.column,
-  .offset-by-two-thirds.columns   { margin-left: 69.3333333333%; }
+  .offset-by-two-thirds.columns {
+    margin-left: 69.3333333333%;
+  }
 
   .offset-by-one-half.column,
-  .offset-by-one-half.columns     { margin-left: 52%; }
+  .offset-by-one-half.columns {
+    margin-left: 52%;
+  }
 
 }
 
 
 /* Base Styles
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 /* NOTE
 html is set to 62.5% so that all the REM measurements throughout Skeleton
 are based on 10px sizing. So basically 1.5rem = 15px :) */
 html {
   font-size: 62.5%;
   background: #222222;
 }
-  
+
 body {
-  font-size: 1.5em; /* currently ems cause chrome bug misinterpreting rems on body element */
+  font-size: 1.5em;
+  /* currently ems cause chrome bug misinterpreting rems on body element */
   line-height: 1.6;
   font-weight: 400;
   font-family: "Open Sans", "HelveticaNeue", "Helvetica Neue", Helvetica, Arial, sans-serif;
-  color: rgb(200, 200, 200); }
+  color: rgb(200, 200, 200);
+}
 
 
 /* Typography
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
-h1, h2, h3, h4, h5, h6 {
+h1,
+h2,
+h3,
+h4,
+h5,
+h6 {
   margin-top: 0;
   margin-bottom: 0;
-  font-weight: 300; }
-h1 { font-size: 4.0rem; line-height: 1.2;  letter-spacing: -.1rem;
-  margin-bottom: 0rem; color: rgb(200, 200, 200);}
-h2 { font-size: 3.3rem; line-height: 1.25; letter-spacing: -.1rem;
-  margin-bottom: 0rem; margin-top: 1.8rem; color: rgb(200, 200, 200);}
-h3 { font-size: 2.7rem; line-height: 1.3;  letter-spacing: -.1rem;
-  margin-bottom: 0rem; margin-top: 1.5rem; color: rgb(200, 200, 200);}
-h4 { font-size: 2.6rem; line-height: 1.35; letter-spacing: -.08rem;
-  margin-bottom: 0rem; margin-top: 1.2rem; color: rgb(200, 200, 200);}
-h5 { font-size: 2.2rem; line-height: 1.5;  letter-spacing: -.05rem;
-  margin-bottom: 0rem; margin-top: 0.6rem; color: rgb(200, 200, 200);}
-h6 { font-size: 2.0rem; line-height: 1.6;  letter-spacing: 0;
-  margin-bottom: 0.75rem; margin-top: 0.75rem; color: rgb(200, 200, 200);}
+  font-weight: 300;
+}
+
+h1 {
+  font-size: 4.0rem;
+  line-height: 1.2;
+  letter-spacing: -.1rem;
+  margin-bottom: 0rem;
+  color: rgb(200, 200, 200);
+}
+
+h2 {
+  font-size: 3.3rem;
+  line-height: 1.25;
+  letter-spacing: -.1rem;
+  margin-bottom: 0rem;
+  margin-top: 1.8rem;
+  color: rgb(200, 200, 200);
+}
+
+h3 {
+  font-size: 2.7rem;
+  line-height: 1.3;
+  letter-spacing: -.1rem;
+  margin-bottom: 0rem;
+  margin-top: 1.5rem;
+  color: rgb(200, 200, 200);
+}
+
+h4 {
+  font-size: 2.6rem;
+  line-height: 1.35;
+  letter-spacing: -.08rem;
+  margin-bottom: 0rem;
+  margin-top: 1.2rem;
+  color: rgb(200, 200, 200);
+}
+
+h5 {
+  font-size: 2.2rem;
+  line-height: 1.5;
+  letter-spacing: -.05rem;
+  margin-bottom: 0rem;
+  margin-top: 0.6rem;
+  color: rgb(200, 200, 200);
+}
+
+h6 {
+  font-size: 2.0rem;
+  line-height: 1.6;
+  letter-spacing: 0;
+  margin-bottom: 0.75rem;
+  margin-top: 0.75rem;
+  color: rgb(200, 200, 200);
+}
 
 p {
-  margin-top: 0; }
+  margin-top: 0;
+}
 
 
 /* Links
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
-a:hover, a:visited, a:link, a:active
-{
-    text-decoration: none;
-    cursor: pointer;
-    color: rgb(160, 180, 255);
+a:hover,
+a:visited,
+a:link,
+a:active {
+  text-decoration: none;
+  cursor: pointer;
+  color: rgb(160, 180, 255);
 }
 
 
 /* Blockquotes
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 blockquote {
   border-left: 4px lightgrey solid;
@@ -204,209 +347,270 @@
   text-transform: uppercase;
   text-decoration: none;
   white-space: nowrap;
   background-color: transparent;
   border-radius: 4px;
   border: 1px solid #bbb;
   cursor: pointer;
-  box-sizing: border-box; }
+  box-sizing: border-box;
+}
+
 .button:hover,
 button:hover,
 input[type="submit"]:hover,
 input[type="reset"]:hover,
 input[type="button"]:hover,
 .button:focus,
 button:focus,
 input[type="submit"]:focus,
 input[type="reset"]:focus,
 input[type="button"]:focus {
   color: #333;
   border-color: #888;
-  outline: 0; }
+  outline: 0;
+}
+
 .button.button-primary,
 button.button-primary,
 input[type="submit"].button-primary,
 input[type="reset"].button-primary,
 input[type="button"].button-primary {
   color: #FFF;
   background-color: #33C3F0;
-  border-color: #33C3F0; }
+  border-color: #33C3F0;
+}
+
 .button.button-primary:hover,
 button.button-primary:hover,
 input[type="submit"].button-primary:hover,
 input[type="reset"].button-primary:hover,
 input[type="button"].button-primary:hover,
 .button.button-primary:focus,
 button.button-primary:focus,
 input[type="submit"].button-primary:focus,
 input[type="reset"].button-primary:focus,
 input[type="button"].button-primary:focus {
   color: #FFF;
   background-color: #1EAEDB;
-  border-color: #1EAEDB; }
+  border-color: #1EAEDB;
+}
 
 
 /* Forms
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 input[type="email"],
 input[type="number"],
 input[type="search"],
 input[type="text"],
 input[type="tel"],
 input[type="url"],
 input[type="password"],
 textarea,
 select {
   height: 38px;
-  padding: 6px 10px; /* The 6px vertically centers text on FF, ignored by Webkit */
+  padding: 6px 10px;
+  /* The 6px vertically centers text on FF, ignored by Webkit */
   background-color: #fff;
   border: 1px solid #D1D1D1;
   border-radius: 4px;
   box-shadow: none;
-  box-sizing: border-box; 
+  box-sizing: border-box;
   font-family: inherit;
-  font-size: inherit; /*https://stackoverflow.com/questions/6080413/why-doesnt-input-inherit-the-font-from-body*/}
+  font-size: inherit;
+  /*https://stackoverflow.com/questions/6080413/why-doesnt-input-inherit-the-font-from-body*/
+}
+
 /* Removes awkward default styles on some inputs for iOS */
 input[type="email"],
 input[type="number"],
 input[type="search"],
 input[type="text"],
 input[type="tel"],
 input[type="url"],
 input[type="password"],
 textarea {
   -webkit-appearance: none;
-     -moz-appearance: none;
-          appearance: none; }
+  -moz-appearance: none;
+  appearance: none;
+}
+
 textarea {
   min-height: 65px;
   padding-top: 6px;
-  padding-bottom: 6px; }
+  padding-bottom: 6px;
+}
+
 input[type="email"]:focus,
 input[type="number"]:focus,
 input[type="search"]:focus,
 input[type="text"]:focus,
 input[type="tel"]:focus,
 input[type="url"]:focus,
 input[type="password"]:focus,
 textarea:focus,
 select:focus {
   border: 1px solid #33C3F0;
-  outline: 0; }
+  outline: 0;
+}
+
 label,
 legend {
   display: block;
-  margin-bottom: 0px; }
+  margin-bottom: 0px;
+}
+
 fieldset {
   padding: 0;
-  border-width: 0; }
+  border-width: 0;
+}
+
 input[type="checkbox"],
 input[type="radio"] {
-  display: inline; }
-label > .label-body {
+  display: inline;
+}
+
+label>.label-body {
   display: inline-block;
   margin-left: .5rem;
-  font-weight: normal; }
+  font-weight: normal;
+}
 
 
 /* Lists
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 ul {
-  list-style: circle inside; }
+  list-style: circle inside;
+}
+
 ol {
-  list-style: decimal inside; }
-ol, ul {
+  list-style: decimal inside;
+}
+
+ol,
+ul {
   padding-left: 30;
-  margin-top: 0; }
+  margin-top: 0;
+}
+
 ul ul,
 ul ol,
 ol ol,
 ol ul {
   margin: 1.5rem 0 1.5rem 3rem;
-  font-size: 100%; }
+  font-size: 100%;
+}
+
 li {
-  margin: -2px; }
+  margin: -2px;
+}
 
 
 /* Tables
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 table {
   border: 4px solid #222222;
   border-collapse: collapse;
 }
+
+tr:hover {
+  background-color: #444444 !important;
+}
+
 tr {
-  border: 1px solid #666666;
+  border: 1px solid #444444;
 }
+
 th:not(.CalendarDay),
 td:not(.CalendarDay) {
   padding: 12px 15px;
   text-align: left;
-  border-bottom: 1px solid #E1E1E1; }
+  border-bottom: 1px solid #E1E1E1;
+}
+
 th:first-child:not(.CalendarDay),
 td:first-child:not(.CalendarDay) {
-  padding-left: 0; }
+  padding-left: 0;
+}
+
 th:last-child:not(.CalendarDay),
 td:last-child:not(.CalendarDay) {
-  padding-right: 0; }
+  padding-right: 0;
+}
 
 
 /* Spacing
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 button,
 .button {
-  margin-bottom: 0rem; }
+  margin-bottom: 0rem;
+}
+
 input,
 textarea,
 select,
 fieldset {
-  margin-bottom: 0rem; }
+  margin-bottom: 0rem;
+}
+
 pre,
 dl,
 figure,
 table,
 form {
-  margin-bottom: 0rem; }
+  margin-bottom: 0rem;
+}
+
 p,
 ul,
 ol {
-  margin-bottom: 0.75rem; }
+  margin-bottom: 0.75rem;
+}
 
 /* Utilities
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 .u-full-width {
   width: 100%;
-  box-sizing: border-box; }
+  box-sizing: border-box;
+}
+
 .u-max-full-width {
   max-width: 100%;
-  box-sizing: border-box; }
+  box-sizing: border-box;
+}
+
 .u-pull-right {
-  float: right; }
+  float: right;
+}
+
 .u-pull-left {
-  float: left; }
+  float: left;
+}
 
 
 /* Misc
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 hr {
   margin-top: 3rem;
   margin-bottom: 3.5rem;
   border-width: 0;
-  border-top: 1px solid #E1E1E1; }
+  border-top: 1px solid #E1E1E1;
+}
 
 
 /* Clearing
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 
 /* Self Clearing Goodness */
 .container:after,
 .row:after,
 .u-cf {
   content: "";
   display: table;
-  clear: both; }
+  clear: both;
+}
 
 
 /* Media Queries
 –––––––––––––––––––––––––––––––––––––––––––––––––– */
 /*
 Note: The best way to structure the use of media queries is to create the queries
 near the relevant code. For example, if you wanted to change the styles for buttons
@@ -425,7 +629,35 @@
 @media (min-width: 750px) {}
 
 /* Larger than desktop */
 @media (min-width: 1000px) {}
 
 /* Larger than Desktop HD */
 @media (min-width: 1200px) {}
+
+/* Tooltip with column type */
+.dash-tooltip .dash-table-tooltip {
+  position: relative;
+  background-color: #555 !important;
+  color: #fff in !important;
+  max-width: fit-content !important;
+  min-width: fit-content !important;
+  padding: 2px 10px;
+  border-radius: 4px;
+}
+
+/* Visual effect for the trash can */
+#trash-icon {
+  display: block;
+  margin: auto;
+  width: 15px;
+  height: 20px;
+  transition: transform 0.3s;
+}
+
+#trash-icon:hover {
+  transform: scale(1.2);
+}
+
+#trash-icon:active {
+  transform: scale(0.9);
+}
```

### Comparing `sageworks-0.1.5.2/applications/aws_dashboard/aws_dashboard.py` & `sageworks-0.1.5.3/applications/aws_dashboard/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Note: The 'app' and 'server' objects need to be at the top level since NGINX/uWSGI needs to
 #       import this file and use the server object as an ^entry-point^ into the Dash Application Code
 
 # Create our Dash Application
 # app = Dash(title='SageWorks: Artifacts', external_stylesheets=[dbc.themes.BOOTSTRAP], use_pages=True)
 # app = Dash(title="SageWorks: Artifacts", use_pages=True)
 app = Dash(
-    title="SageWorks: Artifacts",
+    title="SageWorks Dashboard",
     external_stylesheets=[dbc.themes.DARKLY],
     use_pages=True,
 )
 server = app.server
 
 # For Multi-Page Applications, we need to create a 'page container' to hold all the pages
 app.layout = dash.page_container
```

### Comparing `sageworks-0.1.5.2/applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py` & `sageworks-0.1.5.3/applications/aws_dashboard/pages/data_sources/callbacks.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 from datetime import datetime
 import dash
 from dash import Dash
 from dash.dependencies import Input, Output
 
 # SageWorks Imports
 from sageworks.views.data_source_web_view import DataSourceWebView
-from sageworks.web_components import data_source_details, violin_plot
+from sageworks.web_components import data_and_feature_details, distribution_plots
 
 
 def refresh_data_timer(app: Dash):
     @app.callback(
         Output("last-updated-data-sources", "children"),
         Input("data-sources-updater", "n_intervals"),
     )
     def time_updated(_n):
         return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
 
 
 def update_data_sources_table(app: Dash, data_source_broker: DataSourceWebView):
-    @app.callback(Output("data_sources_table", "data"), Input("data-sources-updater", "n_intervals"))
+    @app.callback(
+        Output("data_sources_table", "data"),
+        Input("data-sources-updater", "n_intervals"),
+    )
     def data_sources_update(_n):
         """Return the table data as a dictionary"""
         data_source_broker.refresh()
         data_source_rows = data_source_broker.data_sources_summary()
         data_source_rows["id"] = data_source_rows.index
         return data_source_rows.to_dict("records")
 
@@ -47,24 +50,27 @@
         ]
         return row_style
 
 
 # Updates the data source details when a row is selected in the summary
 def update_data_source_details(app: Dash, data_source_web_view: DataSourceWebView):
     @app.callback(
-        [Output("data_details_header", "children"), Output("data_source_details", "children")],
+        [
+            Output("data_details_header", "children"),
+            Output("data_source_details", "children"),
+        ],
         Input("data_sources_table", "derived_viewport_selected_row_ids"),
     )
     def generate_new_markdown(selected_rows):
         print(f"Selected Rows: {selected_rows}")
         if not selected_rows or selected_rows[0] is None:
             return dash.no_update
         print("Calling DataSource Details...")
         data_details = data_source_web_view.data_source_details(selected_rows[0])
-        data_details_markdown = data_source_details.create_markdown(data_details)
+        data_details_markdown = data_and_feature_details.create_markdown(data_details)
 
         # Name of the data source for the Header
         data_source_name = data_source_web_view.data_source_name(selected_rows[0])
         header = f"Details: {data_source_name}"
 
         # Return the details/markdown for these data details
         return [header, data_details_markdown]
@@ -108,8 +114,18 @@
     )
     def generate_new_violin_plot(selected_rows):
         print(f"Selected Rows: {selected_rows}")
         if not selected_rows or selected_rows[0] is None:
             return dash.no_update
         print("Calling DataSource Sample Rows Refresh...")
         smart_sample_rows = data_source_web_view.data_source_smart_sample(selected_rows[0])
-        return violin_plot.create_figure(smart_sample_rows)
+        return distribution_plots.create_figure(
+            smart_sample_rows,
+            plot_type="violin",
+            figure_args={
+                "box_visible": True,
+                "meanline_visible": True,
+                "showlegend": False,
+                "points": "all",
+            },
+            max_plots=48,
+        )
```

### Comparing `sageworks-0.1.5.2/applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py` & `sageworks-0.1.5.3/applications/aws_dashboard/pages/endpoints/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py` & `sageworks-0.1.5.3/applications/aws_dashboard/pages/feature_sets/callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-"""FeatureSets Callbacks: Callback within the FeatureSets Web User Interface"""
+"""Callbacks for the FeatureSets Subpage Web User Interface"""
 from datetime import datetime
 import dash
 from dash import Dash
 from dash.dependencies import Input, Output
 
 # SageWorks Imports
 from sageworks.views.feature_set_web_view import FeatureSetWebView
-from sageworks.web_components import feature_set_details, violin_plot
+from sageworks.web_components import data_and_feature_details, distribution_plots, table
 
 
 def refresh_data_timer(app: Dash):
     @app.callback(
         Output("last-updated-feature-sets", "children"),
         Input("feature-sets-updater", "n_intervals"),
     )
     def time_updated(_n):
         return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
 
 
 def update_feature_sets_table(app: Dash, feature_set_broker: FeatureSetWebView):
-    @app.callback(Output("feature_sets_table", "data"), Input("feature-sets-updater", "n_intervals"))
+    @app.callback(
+        Output("feature_sets_table", "data"),
+        Input("feature-sets-updater", "n_intervals"),
+    )
     def feature_sets_update(_n):
-        """Return the table data as a dictionary"""
+        """Return the table data for the FeatureSets Table"""
         feature_set_broker.refresh()
         feature_set_rows = feature_set_broker.feature_sets_summary()
         feature_set_rows["id"] = feature_set_rows.index
         return feature_set_rows.to_dict("records")
 
 
 # Highlights the selected row in the table
@@ -47,24 +50,27 @@
         ]
         return row_style
 
 
 # Updates the data source details when a row is selected in the summary
 def update_feature_set_details(app: Dash, feature_set_web_view: FeatureSetWebView):
     @app.callback(
-        [Output("feature_details_header", "children"), Output("feature_set_details", "children")],
+        [
+            Output("feature_details_header", "children"),
+            Output("feature_set_details", "children"),
+        ],
         Input("feature_sets_table", "derived_viewport_selected_row_ids"),
     )
     def generate_new_markdown(selected_rows):
         print(f"Selected Rows: {selected_rows}")
         if not selected_rows or selected_rows[0] is None:
             return dash.no_update
         print("Calling FeatureSet Details...")
         feature_details = feature_set_web_view.feature_set_details(selected_rows[0])
-        feature_details_markdown = feature_set_details.create_markdown(feature_details)
+        feature_details_markdown = data_and_feature_details.create_markdown(feature_details)
 
         # Name of the data source for the Header
         feature_set_name = feature_set_web_view.feature_set_name(selected_rows[0])
         header = f"Details: {feature_set_name}"
 
         # Return the details/markdown for these data details
         return [header, feature_details_markdown]
@@ -88,15 +94,15 @@
         sample_rows = feature_set_web_view.feature_set_sample(selected_rows[0])
 
         # Name of the data source
         feature_set_name = feature_set_web_view.feature_set_name(selected_rows[0])
         header = f"Sampled Rows: {feature_set_name}"
 
         # The columns need to be in a special format for the DataTable
-        column_setup = [{"name": c, "id": c, "presentation": "input"} for c in sample_rows.columns]
+        column_setup = table.column_setup(sample_rows)
 
         # Return the columns and the data
         return [header, column_setup, sample_rows.to_dict("records")]
 
 
 def update_violin_plots(app: Dash, feature_set_web_view: FeatureSetWebView):
     """Updates the Violin Plots when a new data source is selected"""
@@ -108,8 +114,18 @@
     )
     def generate_new_violin_plot(selected_rows):
         print(f"Selected Rows: {selected_rows}")
         if not selected_rows or selected_rows[0] is None:
             return dash.no_update
         print("Calling FeatureSet Sample Rows Refresh...")
         smart_sample_rows = feature_set_web_view.feature_set_smart_sample(selected_rows[0])
-        return violin_plot.create_figure(smart_sample_rows)
+        return distribution_plots.create_figure(
+            smart_sample_rows,
+            plot_type="violin",
+            figure_args={
+                "box_visible": True,
+                "meanline_visible": True,
+                "showlegend": False,
+                "points": "all",
+            },
+            max_plots=48,
+        )
```

### Comparing `sageworks-0.1.5.2/applications/aws_dashboard/pages/callbacks/models_callbacks.py` & `sageworks-0.1.5.3/applications/aws_dashboard/pages/models/callbacks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,61 @@
-"""Callbacks/Connections in the Web User Interface"""
+"""Callbacks for the Model Subpage Web User Interface"""
 import dash
 from dash import Dash
 from dash.dependencies import Input, Output
 from datetime import datetime
 
 # SageWorks Imports
-from sageworks.web_components.model_data import ModelData
+from sageworks.web_components.mock_model_data import ModelData
 from sageworks.web_components import (
-    feature_importance,
+    mock_feature_importance,
     confusion_matrix,
-    model_details,
-    feature_details,
+    mock_model_details,
+    mock_feature_details,
 )
-from sageworks.views.artifacts_web_view import ArtifactsWebView
+from sageworks.views.model_web_view import ModelWebView
 
 
-def update_last_updated(app: Dash):
+def refresh_data_timer(app: Dash):
     @app.callback(
         Output("last-updated-models", "children"),
         Input("models-updater", "n_intervals"),
     )
-    def time_updated(n):
+    def time_updated(_n):
         return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
 
 
-def update_models_table(app: Dash, sageworks_artifacts: ArtifactsWebView):
+def update_models_table(app: Dash, model_broker: ModelWebView):
     @app.callback(Output("models_table", "data"), Input("models-updater", "n_intervals"))
-    def data_sources_update(n):
-        print("Calling Models Refresh...")
-        sageworks_artifacts.refresh()
-        models = sageworks_artifacts.models_summary()
-        return models.to_dict("records")
+    def feature_sets_update(_n):
+        """Return the table data as a dictionary"""
+        model_broker.refresh()
+        model_rows = model_broker.models_summary()
+        model_rows["id"] = model_rows.index
+        return model_rows.to_dict("records")
 
 
 # Highlights the selected row in the table
 def table_row_select(app: Dash, table_name: str):
     @app.callback(
         Output(table_name, "style_data_conditional"),
         Input(table_name, "derived_viewport_selected_row_ids"),
     )
     def style_selected_rows(selected_rows):
         print(f"Selected Rows: {selected_rows}")
         if not selected_rows or selected_rows[0] is None:
             return dash.no_update
-        foo = [
+        row_style = [
             {
                 "if": {"filter_query": "{{id}} ={}".format(i)},
                 "backgroundColor": "rgb(80, 80, 80)",
             }
             for i in selected_rows
         ]
-        return foo
+        return row_style
 
 
 # Updates the feature importance and confusion matrix figures when a model is selected
 def update_figures(app: Dash, model_data: ModelData):
     @app.callback(
         [Output("feature_importance", "figure"), Output("confusion_matrix", "figure")],
         Input("models_table", "derived_viewport_selected_row_ids"),
@@ -67,15 +68,15 @@
             selected_rows = [0]
 
         # Grab the data for this row
         model_row_index = selected_rows[0]
 
         # Generate a figure for the feature importance component
         feature_info = model_data.get_model_feature_importance(model_row_index)
-        feature_figure = feature_importance.create_figure(feature_info)
+        feature_figure = mock_feature_importance.create_figure(feature_info)
 
         # Generate a figure for the confusion matrix component
         c_matrix = model_data.get_model_confusion_matrix(model_row_index)
         matrix_figure = confusion_matrix.create_figure(c_matrix)
 
         # Now return both of the new figures
         return [feature_figure, matrix_figure]
@@ -95,15 +96,15 @@
             selected_rows = [0]
 
         # Grab the data for this row
         model_row_index = selected_rows[0]
 
         # Generate new Details (Markdown) for the selected model
         model_info = model_data.get_model_details(model_row_index)
-        model_markdown = model_details.create_markdown(model_info)
+        model_markdown = mock_model_details.create_markdown(model_info)
 
         # Return the details/markdown for this model
         return model_markdown
 
 
 # Updates the feature details when a model row is selected
 def update_feature_details(app: Dash, model_data: ModelData):
@@ -119,11 +120,11 @@
             selected_rows = [0]
 
         # Grab the data for this row
         model_row_index = selected_rows[0]
 
         # Generate new Details (Markdown) for the features for this model
         feature_info = model_data.get_model_feature_importance(model_row_index)
-        feature_markdown = feature_details.create_markdown(feature_info)
+        feature_markdown = mock_feature_details.create_markdown(feature_info)
 
         # Return the details/markdown for these features
         return feature_markdown
```

### Comparing `sageworks-0.1.5.2/applications/aws_dashboard/pages/data/toy_data.csv` & `sageworks-0.1.5.3/applications/aws_dashboard/pages/data/toy_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/applications/aws_dashboard/pages/data/toy_scores.json` & `sageworks-0.1.5.3/applications/aws_dashboard/pages/data/toy_scores.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/applications/aws_dashboard/pages/endpoints.py` & `sageworks-0.1.5.3/applications/aws_dashboard/pages/endpoints/page.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,18 +4,22 @@
 
 # SageWorks Imports
 from sageworks.web_components import line_chart
 from sageworks.views.artifacts_web_view import ArtifactsWebView
 from sageworks.web_components import table
 
 # Local Imports
-from pages.layout.endpoints_layout import endpoints_layout
-import pages.callbacks.endpoints_callbacks as callbacks
+from .layout import endpoints_layout
+from . import callbacks
 
-register_page(__name__, path="/endpoints")
+register_page(
+    __name__,
+    path="/endpoints",
+    name="SageWorks - Endpoints",
+)
 
 
 # Okay feels a bit weird but Dash pages just have a bunch of top level code (no classes/methods)
 
 # Grab a view that gives us a summary of all the artifacts currently in SageWorks
 sageworks_artifacts = ArtifactsWebView()
 endpoints_summary = sageworks_artifacts.endpoints_summary()
@@ -30,18 +34,18 @@
 )
 
 # Create a fake scatter plot
 endpoint_traffic = line_chart.create()
 
 # Create our components
 components = {
-    "endpoints_details": endpoints_table,
+    "endpoints_table": endpoints_table,
     "endpoint_traffic": endpoint_traffic,
 }
 
+# Set up our layout (Dash looks for a var called layout)
+layout = endpoints_layout(**components)
+
 # Setup our callbacks/connections
 app = dash.get_app()
 callbacks.update_last_updated(app)
 callbacks.update_endpoints_table(app, sageworks_artifacts)
-
-# Set up our layout (Dash looks for a var called layout)
-layout = endpoints_layout(components)
```

### Comparing `sageworks-0.1.5.2/applications/aws_dashboard/pages/feature_sets.py` & `sageworks-0.1.5.3/applications/aws_dashboard/pages/feature_sets/page.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """DataSources:  A SageWorks Web Interface to view, interact, and manage Data Sources"""
 from dash import register_page
 import dash
 from dash_bootstrap_templates import load_figure_template
 
 # SageWorks Imports
-from sageworks.web_components import violin_plot, table, feature_set_details
+from sageworks.web_components import table, data_and_feature_details, distribution_plots
 from sageworks.views.feature_set_web_view import FeatureSetWebView
 
 # Local Imports
-from pages.layout.feature_sets_layout import feature_sets_layout
-import pages.callbacks.feature_sets_callbacks as callbacks
+from .layout import feature_sets_layout
+from . import callbacks
 
-register_page(__name__, path="/feature_sets", name="Feature Sets")
 
+register_page(__name__, path="/feature_sets", name="SageWorks - Feature Sets")
 
 # Okay feels a bit weird but Dash pages just have a bunch of top level code (no classes/methods)
 
 # Put the components into 'dark' mode
 load_figure_template("darkly")
 
-# Grab a view that gives us a summary of the DataSources in SageWorks
+# Grab a view that gives us a summary of the FeatureSets in SageWorks
 feature_set_broker = FeatureSetWebView()
 feature_set_rows = feature_set_broker.feature_sets_summary()
 
 # Create a table to display the data sources
 feature_sets_table = table.create(
     "feature_sets_table",
     feature_set_rows,
@@ -39,38 +39,49 @@
     sample_rows,
     header_color="rgb(60, 60, 100)",
     max_height="200px",
 )
 
 # Data Source Details
 details = feature_set_broker.feature_set_details(0)
-data_details = feature_set_details.create("feature_set_details", details)
+data_details = data_and_feature_details.create("feature_set_details", details)
 
 # Create a box plot of all the numeric columns in the sample rows
 smart_sample_rows = feature_set_broker.feature_set_smart_sample(0)
-violin = violin_plot.create("feature_set_violin_plot", smart_sample_rows)
+violin = distribution_plots.create(
+    "feature_set_violin_plot",
+    smart_sample_rows,
+    plot_type="violin",
+    figure_args={
+        "box_visible": True,
+        "meanline_visible": True,
+        "showlegend": False,
+        "points": "all",
+    },
+    max_plots=48,
+)
 
 # Create our components
 components = {
     "feature_sets_table": feature_sets_table,
-    "feature_set_details": data_details,
     "feature_set_sample_rows": feature_set_sample_rows,
+    "feature_set_details": data_details,
     "violin_plot": violin,
 }
 
+# Set up our layout (Dash looks for a var called layout)
+layout = feature_sets_layout(**components)
+
 # Setup our callbacks/connections
 app = dash.get_app()
 
 # Refresh our data timer
 callbacks.refresh_data_timer(app)
 
 # Periodic update to the data sources summary table
 callbacks.update_feature_sets_table(app, feature_set_broker)
 
 # Callbacks for when a data source is selected
 callbacks.table_row_select(app, "feature_sets_table")
 callbacks.update_feature_set_details(app, feature_set_broker)
 callbacks.update_feature_set_sample_rows(app, feature_set_broker)
 callbacks.update_violin_plots(app, feature_set_broker)
-
-# Set up our layout (Dash looks for a var called layout)
-layout = feature_sets_layout(components)
```

### Comparing `sageworks-0.1.5.2/applications/aws_dashboard/pages/layout/data_sources_layout.py` & `sageworks-0.1.5.3/applications/aws_dashboard/pages/data_sources/layout.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 """DataSources Layout: Layout for the DataSources page in the Artifact Viewer"""
-from dash import html, dcc
+from dash import html, dcc, dash_table
 import dash_bootstrap_components as dbc
 
 
-def data_sources_layout(components: dict) -> html.Div:
+def data_sources_layout(
+    data_sources_table: dash_table.DataTable,
+    data_source_details: dcc.Markdown,
+    data_source_sample_rows: dash_table.DataTable,
+    violin_plot: dcc.Graph,
+) -> html.Div:
     # Just put all the tables in as Rows for Now (do something fancy later)
     layout = html.Div(
         children=[
             dbc.Row(
                 [
                     html.H2("SageWorks: DataSources (Alpha)"),
                     html.Div(
@@ -19,48 +24,48 @@
                             "padding": "0px 0px 0px 160px",
                         },
                     ),
                     dbc.Row(style={"padding": "30px 0px 0px 0px"}),
                 ]
             ),
             # List out all the Data Sources
-            dbc.Row(components["data_sources_table"]),
+            dbc.Row(data_sources_table),
             # Data Source Details, Sample Rows, and Violin Plots
             # Row [ Sample Rows ]
             # Row [ Column 1                      Column 2 ]
             #       (Row(Data Source Details))    Row(Violin Plots)
             #
             dbc.Row(
                 html.H3("Sampled Rows", id="sample_rows_header"),
                 style={"padding": "30px 0px 10px 0px"},
             ),
             dbc.Row(
-                components["data_source_sample_rows"],
+                data_source_sample_rows,
                 style={"padding": "0px 0px 30px 0px"},
             ),
             dbc.Row(
                 [
                     # Column 1: Data Source Details
                     dbc.Col(
                         [
                             dbc.Row(
                                 html.H3("Details", id="data_details_header"),
                                 style={"padding": "0px 0px 10px 0px"},
                             ),
                             dbc.Row(
-                                components["data_source_details"],
+                                data_source_details,
                                 style={"padding": "0px 0px 30px 0px"},
                             ),
                         ],
                         width=4,
                     ),
                     # Column 2: Sample Rows and Violin Plots
                     dbc.Col(
                         [
-                            dbc.Row(components["violin_plot"]),
+                            dbc.Row(violin_plot),
                         ],
                         width=8,
                     ),
                     # Just the auto updater
                     dcc.Interval(id="data-sources-updater", interval=5000, n_intervals=0),
                 ]
             ),
```

### Comparing `sageworks-0.1.5.2/applications/aws_dashboard/pages/layout/endpoints_layout.py` & `sageworks-0.1.5.3/applications/aws_dashboard/pages/endpoints/layout.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Endpoints Layout: Layout for the Endpoints page in the Artifact Viewer"""
-from dash import html, dcc
+from dash import html, dcc, dash_table
 import dash_bootstrap_components as dbc
 
 
-def endpoints_layout(components: dict) -> html.Div:
+def endpoints_layout(
+    endpoints_table: dash_table.DataTable,
+    endpoint_traffic: dcc.Graph,
+) -> html.Div:
     # Just put all the tables in as Rows for Now (do something fancy later)
     layout = html.Div(
         children=[
             dbc.Row(
                 [
                     html.H2("SageWorks: Endpoints (Alpha)"),
                     html.Div(
@@ -18,14 +21,14 @@
                             "fontSize": 15,
                             "padding": "0px 0px 0px 160px",
                         },
                     ),
                     dbc.Row(style={"padding": "30px 0px 0px 0px"}),
                 ]
             ),
-            dbc.Row(components["endpoints_details"]),
-            dbc.Row(components["endpoint_traffic"]),
+            dbc.Row(endpoints_table),
+            dbc.Row(endpoint_traffic),
             dcc.Interval(id="endpoints-updater", interval=5000, n_intervals=0),
         ],
         style={"margin": "30px"},
     )
     return layout
```

### Comparing `sageworks-0.1.5.2/applications/aws_dashboard/pages/layout/feature_sets_layout.py` & `sageworks-0.1.5.3/applications/aws_dashboard/pages/feature_sets/layout.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 """FeatureSets Layout: Layout for the FeatureSets page in the Artifact Viewer"""
-from dash import html, dcc
+from dash import html, dcc, dash_table
 import dash_bootstrap_components as dbc
 
 
-def feature_sets_layout(components: dict) -> html.Div:
+def feature_sets_layout(
+    feature_sets_table: dash_table.DataTable,
+    feature_set_sample_rows: dash_table.DataTable,
+    feature_set_details: dcc.Markdown,
+    violin_plot: dcc.Graph,
+) -> html.Div:
     # Just put all the tables in as Rows for Now (do something fancy later)
     layout = html.Div(
         children=[
             dbc.Row(
                 [
                     html.H2("SageWorks: FeatureSets (Alpha)"),
                     html.Div(
@@ -19,48 +24,48 @@
                             "padding": "0px 0px 0px 160px",
                         },
                     ),
                     dbc.Row(style={"padding": "30px 0px 0px 0px"}),
                 ]
             ),
             # List out all the Data Sources
-            dbc.Row(components["feature_sets_table"]),
+            dbc.Row(feature_sets_table),
             # Data Source Details, Sample Rows, and Violin Plots
             # Row [ Sample Rows ]
             # Row [ Column 1                      Column 2 ]
             #       (Row(Data Source Details))    Row(Violin Plots)
             #
             dbc.Row(
                 html.H3("Sampled Rows", id="feature_sample_rows_header"),
                 style={"padding": "30px 0px 10px 0px"},
             ),
             dbc.Row(
-                components["feature_set_sample_rows"],
+                feature_set_sample_rows,
                 style={"padding": "0px 0px 30px 0px"},
             ),
             dbc.Row(
                 [
                     # Column 1: Data Source Details
                     dbc.Col(
                         [
                             dbc.Row(
                                 html.H3("Details", id="feature_details_header"),
                                 style={"padding": "0px 0px 10px 0px"},
                             ),
                             dbc.Row(
-                                components["feature_set_details"],
+                                feature_set_details,
                                 style={"padding": "0px 0px 30px 0px"},
                             ),
                         ],
                         width=4,
                     ),
                     # Column 2: Sample Rows and Violin Plots
                     dbc.Col(
                         [
-                            dbc.Row(components["violin_plot"]),
+                            dbc.Row(violin_plot),
                         ],
                         width=8,
                     ),
                     # Just the auto updater
                     dcc.Interval(id="feature-sets-updater", interval=5000, n_intervals=0),
                 ]
             ),
```

### Comparing `sageworks-0.1.5.2/applications/aws_dashboard/pages/layout/models_layout.py` & `sageworks-0.1.5.3/applications/aws_dashboard/pages/models/layout.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 """Layout for the models page"""
-from dash import dcc, html
+from dash import dcc, html, dash_table
 import dash_bootstrap_components as dbc
 
 
-def models_layout(components: dict) -> html.Div:
+def models_layout(
+    models_table: dash_table.DataTable,
+    model_details: dcc.Markdown,
+    confusion_matrix: dcc.Graph,
+    scatter_plot: dcc.Graph,
+    feature_importance: dcc.Graph,
+    feature_details: dcc.Markdown,
+) -> html.Div:
     layout = html.Div(
         children=[
             dbc.Row(html.H2("SageWorks: Models (Alpha)")),
             html.Div(
                 "Last Updated: ",
                 id="last-updated-models",
                 style={
@@ -18,42 +25,42 @@
             ),
             dbc.Row(style={"padding": "30px 0px 0px 0px"}),
             dbc.Row(
                 [
                     # Model Table and Model Details
                     dbc.Col(
                         [
-                            dbc.Row(components["models_table"]),
+                            dbc.Row(models_table),
                             dbc.Row(
                                 html.H3("Model Details"),
                                 style={"padding": "50px 0px 0px 20px"},
                             ),
                             dbc.Row(
                                 [
-                                    dbc.Col(components["model_details"]),
-                                    dbc.Col(components["confusion_matrix"]),
+                                    dbc.Col(model_details),
+                                    dbc.Col(confusion_matrix),
                                 ]
                             ),
-                            dbc.Row(components["scatter_plot"]),
+                            dbc.Row(scatter_plot),
                         ],
                         width=8,
                     ),
                     # Feature Importance and Details
                     dbc.Col(
                         [
                             dbc.Row(html.H3("Feature Importance")),
-                            dbc.Row(components["feature_importance"]),
+                            dbc.Row(feature_importance),
                             dbc.Row(
                                 html.H3(
                                     "Feature Details",
                                     style={"padding": "20px 0px 0px 20px"},
                                 )
                             ),
                             dbc.Row(
-                                components["feature_details"],
+                                feature_details,
                                 style={"padding": "0px 0px 0px 20px"},
                             ),
                         ],
                         width=4,
                     ),
                 ]
             ),
```

### Comparing `sageworks-0.1.5.2/applications/aws_dashboard/pages/main.py` & `sageworks-0.1.5.3/applications/aws_dashboard/pages/main/page.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,67 +3,84 @@
 import dash
 
 # SageWorks Imports
 from sageworks.views.artifacts_web_view import ArtifactsWebView
 from sageworks.web_components import table
 
 # Local Imports
-from pages.layout.main_layout import main_layout
-import pages.callbacks.main_callbacks as callbacks
+from .layout import main_layout
+from . import callbacks
 
-register_page(__name__, path="/")
+register_page(
+    __name__,
+    path="/",
+    name="SageWorks",
+)
 
 
 # Okay feels a bit weird but Dash pages just have a bunch of top level code (no classes/methods)
 
 # Grab a view that gives us a summary of all the artifacts currently in SageWorks
 web_artifacts_summary = ArtifactsWebView()
 sageworks_artifacts = web_artifacts_summary.view_data()
 
+for df in sageworks_artifacts:
+    if df != "INCOMING_DATA" and df != "GLUE_JOBS":
+        sageworks_artifacts[df]["del"] = "<img src='../assets/trash.png' id='trash-icon'>"
+
 # Grab the Artifact Information DataFrame for each AWS Service and pass it to the table creation
 tables = dict()
 tables["INCOMING_DATA"] = table.create(
-    "INCOMING_DATA",
-    sageworks_artifacts["INCOMING_DATA"],
+    table_id="INCOMING_DATA",
+    df=sageworks_artifacts["INCOMING_DATA"],
+    header_color="rgb(60, 60, 100)",
+    markdown_columns=["Name"],
+)
+tables["GLUE_JOBS"] = table.create(
+    table_id="GLUE_JOBS",
+    df=sageworks_artifacts["GLUE_JOBS"],
     header_color="rgb(60, 60, 100)",
+    markdown_columns=["Name"],
 )
 tables["DATA_SOURCES"] = table.create(
-    "DATA_SOURCES",
-    sageworks_artifacts["DATA_SOURCES"],
+    table_id="DATA_SOURCES",
+    df=sageworks_artifacts["DATA_SOURCES"],
     header_color="rgb(100, 60, 60)",
-    markdown_columns=["Name"],
+    markdown_columns=["Name", "del"],
 )
 tables["FEATURE_SETS"] = table.create(
-    "FEATURE_SETS",
-    sageworks_artifacts["FEATURE_SETS"],
+    table_id="FEATURE_SETS",
+    df=sageworks_artifacts["FEATURE_SETS"],
     header_color="rgb(100, 100, 60)",
-    markdown_columns=["Feature Group"],
+    markdown_columns=["Feature Group", "del"],
 )
 tables["MODELS"] = table.create(
-    "MODELS",
-    sageworks_artifacts["MODELS"],
+    table_id="MODELS",
+    df=sageworks_artifacts["MODELS"],
     header_color="rgb(60, 100, 60)",
-    markdown_columns=["Model Group"],
+    markdown_columns=["Model Group", "del"],
 )
 tables["ENDPOINTS"] = table.create(
-    "ENDPOINTS",
-    sageworks_artifacts["ENDPOINTS"],
+    table_id="ENDPOINTS",
+    df=sageworks_artifacts["ENDPOINTS"],
     header_color="rgb(100, 60, 100)",
-    markdown_columns=["Name"],
+    markdown_columns=["Name", "del"],
 )
 
 # Create our components
 components = {
     "incoming_data": tables["INCOMING_DATA"],
+    "glue_jobs": tables["GLUE_JOBS"],
     "data_sources": tables["DATA_SOURCES"],
     "feature_sets": tables["FEATURE_SETS"],
     "models": tables["MODELS"],
     "endpoints": tables["ENDPOINTS"],
 }
 
+# Set up our layout (Dash looks for a var called layout)
+layout = main_layout(**components)
+
 # Setup our callbacks/connections
 app = dash.get_app()
 callbacks.update_last_updated(app, web_artifacts_summary)
 callbacks.update_artifact_tables(app)
-
-# Set up our layout (Dash looks for a var called layout)
-layout = main_layout(components)
+callbacks.remove_artifact_callbacks(app)
```

### Comparing `sageworks-0.1.5.2/applications/aws_dashboard/pages/models.py` & `sageworks-0.1.5.3/applications/aws_dashboard/pages/models/page.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,78 @@
-import os
+from pathlib import Path
 from dash import register_page
 import dash
 from dash_bootstrap_templates import load_figure_template
 
 
 # SageWorks Imports
 
 from sageworks.web_components import confusion_matrix, table, scatter_plot
 from sageworks.web_components import (
-    feature_importance,
-    model_data,
-    model_details,
-    feature_details,
+    mock_feature_importance,
+    mock_model_data,
+    mock_model_details,
+    mock_feature_details,
 )
-from sageworks.views.artifacts_web_view import ArtifactsWebView
+from sageworks.views.model_web_view import ModelWebView
 
 # Local Imports
-from pages.layout.models_layout import models_layout
-import pages.callbacks.models_callbacks as callbacks
+from .layout import models_layout
+from . import callbacks
 
-register_page(__name__, path="/models")
+register_page(
+    __name__,
+    path="/models",
+    name="SageWorks - Models",
+)
 
 # Okay feels a bit weird but Dash pages just have a bunch of top level code (no classes/methods)
 
 # Put the components into 'dark' mode
 load_figure_template("darkly")
 
-# Grab a view that gives us a summary of all the artifacts currently in SageWorks
-web_artifacts_summary = ArtifactsWebView()
-models_summary = web_artifacts_summary.models_summary(concise=True)
+# Grab a view that gives us a summary of the FeatureSets in SageWorks
+model_broker = ModelWebView()
+models_rows = model_broker.models_summary()
 
 # Read in our fake model data
-data_path = os.path.join(os.path.dirname(__file__), "data/toy_data.csv")
-fake_model_info = model_data.ModelData(data_path)
+data_path = str(Path(__file__).resolve().parent.parent / "data/toy_data.csv")
+fake_model_info = mock_model_data.ModelData(data_path)
 
 # Create a table to display the models
 models_table = table.create(
     "models_table",
-    models_summary,
+    models_rows,
     header_color="rgb(60, 100, 60)",
     row_select="single",
     markdown_columns=["Model Group"],
 )
 
 # Create all the other components on this page
 model_df = fake_model_info.get_model_df()
-details = model_details.create(fake_model_info.get_model_details(0))
+details = mock_model_details.create(fake_model_info.get_model_details(0))
 c_matrix = confusion_matrix.create(fake_model_info.get_model_confusion_matrix(0))
-scatter = scatter_plot.create(model_df, variant=3)
-my_feature_importance = feature_importance.create(fake_model_info.get_model_feature_importance(0))
-my_feature_details = feature_details.create(fake_model_info.get_model_feature_importance(0))
+scatter = scatter_plot.create("model performance", model_df)
+my_feature_importance = mock_feature_importance.create(fake_model_info.get_model_feature_importance(0))
+my_feature_details = mock_feature_details.create(fake_model_info.get_model_feature_importance(0))
 components = {
     "models_table": models_table,
     "model_details": details,
     "confusion_matrix": c_matrix,
     "scatter_plot": scatter,
     "feature_importance": my_feature_importance,
     "feature_details": my_feature_details,
 }
 
+# Set up our layout (Dash looks for a var called layout)
+layout = models_layout(**components)
+
 # Setup our callbacks/connections
 app = dash.get_app()
-callbacks.update_last_updated(app)
-# FIXME: Updating the table somehow breaks the row selection callback
-# callbacks.update_models_table(app, models_summary)
+callbacks.refresh_data_timer(app)
+callbacks.update_models_table(app, model_broker)
 
 # Callback for the model table
 callbacks.table_row_select(app, "models_table")
 callbacks.update_figures(app, fake_model_info)
 callbacks.update_model_details(app, fake_model_info)
 callbacks.update_feature_details(app, fake_model_info)
-
-# Set up our layout (Dash looks for a var called layout)
-layout = models_layout(components)
```

### Comparing `sageworks-0.1.5.2/applications/hello_world/callbacks.py` & `sageworks-0.1.5.3/applications/hello_world/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Callbacks/Connections in the Web User Interface"""
 import dash
 from dash import Dash
 from dash.dependencies import Input, Output
 
 # SageWorks Imports
-from sageworks.web_components.model_data import ModelData
+from sageworks.web_components.mock_model_data import ModelData
 from sageworks.web_components import (
     feature_importance,
     confusion_matrix,
     model_details,
     feature_details,
 )
```

### Comparing `sageworks-0.1.5.2/applications/hello_world/hello_world.py` & `sageworks-0.1.5.3/applications/hello_world/hello_world.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/applications/hello_world/layout.py` & `sageworks-0.1.5.3/applications/hello_world/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/applications/model_viewer/callbacks.py` & `sageworks-0.1.5.3/applications/model_viewer/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Callbacks/Connections in the Web User Interface"""
 import dash
 from dash import Dash
 from dash.dependencies import Input, Output
 
 # SageWorks Imports
-from sageworks.web_components.model_data import ModelData
+from sageworks.web_components.mock_model_data import ModelData
 from sageworks.web_components import (
     feature_importance,
     confusion_matrix,
     model_details,
     feature_details,
 )
```

### Comparing `sageworks-0.1.5.2/applications/model_viewer/data/toy_data.csv` & `sageworks-0.1.5.3/applications/model_viewer/data/toy_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/applications/model_viewer/data/toy_scores.json` & `sageworks-0.1.5.3/applications/model_viewer/data/toy_scores.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/applications/model_viewer/layout.py` & `sageworks-0.1.5.3/applications/model_viewer/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/applications/model_viewer/model_viewer.py` & `sageworks-0.1.5.3/applications/model_viewer/model_viewer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os
+from pathlib import Path
 from dash import Dash
 import dash_bootstrap_components as dbc
 
 
 # SageWorks Imports
 from sageworks.web_components import confusion_matrix, table, scatter_plot
 from sageworks.web_components import (
@@ -27,28 +27,28 @@
 
 
 def setup_model_details_view():
     # Set Default Template for figures
     # load_figure_template('darkly')
 
     # Read in our model data
-    data_path = os.path.join(os.path.dirname(__file__), "data/toy_data.csv")
+    data_path = str(Path(__file__).resolve().parent.parent / "data/toy_data.csv")
     model_info = model_data.ModelData(data_path)
 
     # Create our components
     model_df = model_info.get_model_df()
     model_table = table.create(
         "model_table",
         model_df,
         show_columns=["model_name", "date_created", "f_scores"],
         row_select="single",
     )
     details = model_details.create(model_info.get_model_details(0))
     c_matrix = confusion_matrix.create(model_info.get_model_confusion_matrix(0))
-    scatter = scatter_plot.create(model_df)
+    scatter = scatter_plot.create("model_scatter", model_df)
     my_feature_importance = feature_importance.create(model_info.get_model_feature_importance(0))
     my_feature_details = feature_details.create(model_info.get_model_feature_importance(0))
     components = {
         "model_table": model_table,
         "model_details": details,
         "confusion_matrix": c_matrix,
         "scatter_plot": scatter,
```

### Comparing `sageworks-0.1.5.2/aws_setup/aws_account_check.py` & `sageworks-0.1.5.3/aws_setup/aws_account_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/aws_setup/build_ml_pipeline.py` & `sageworks-0.1.5.3/aws_setup/build_ml_pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,34 +61,41 @@
     if not DataSource("abalone_data").check():
         my_loader = CSVToDataSource(abalone_data_path, "abalone_data")
         my_loader.set_output_tags("abalone:public")
         my_loader.transform()
         print("Waiting for the abalone_data to be created...")
         time.sleep(10)
 
+    # Give user a warning about how long the rest of the script will take
+    print("\n******************************************************************************")
+    print("Note: The rest of this script takes about 20 minutes (AWS finalize/wait times)")
+    print("******************************************************************************\n")
+    time.sleep(5)
+
     # Create the test_feature_set FeatureSet
     if not FeatureSet("test_feature_set").check():
         data_to_features = DataToFeaturesLight("test_data", "test_feature_set")
         data_to_features.set_output_tags(["test", "small"])
         data_to_features.transform(id_column="id", event_time_column="date")
 
     # Create the abalone_feature_set FeatureSet
     if not FeatureSet("abalone_feature_set").check():
         data_to_features = DataToFeaturesLight("abalone_data", "abalone_feature_set")
         data_to_features.set_output_tags(["abalone", "public"])
         data_to_features.transform()
-        print("AWS takes a LONG time to populate their Feature Store/Groups. Run this script again in 10 minutes...")
-        sys.exit(0)
 
     # Create the abalone_regression Model
     if not Model("abalone-regression").check():
         features_to_model = FeaturesToModel("abalone_feature_set", "abalone-regression")
         features_to_model.set_output_tags(["abalone", "regression"])
         features_to_model.transform(target="class_number_of_rings", description="Abalone Regression Model")
+
+    # Wait for the Model to be created
+    while not Model("abalone-regression").check():
         print("Waiting for the Model to be created...")
-        time.sleep(30)
+        time.sleep(5)
 
     # Create the abalone_regression Endpoint
     if not Endpoint("abalone-regression-end").check():
         model_to_endpoint = ModelToEndpoint("abalone-regression", "abalone-regression-end")
         model_to_endpoint.set_output_tags(["abalone", "regression"])
         model_to_endpoint.transform()
```

### Comparing `sageworks-0.1.5.2/aws_setup/sageworks_cdk/README.md` & `sageworks-0.1.5.3/aws_setup/sageworks_cdk/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/aws_setup/sageworks_cdk/app.py` & `sageworks-0.1.5.3/aws_setup/sageworks_cdk/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/aws_setup/sageworks_cdk/cdk.json` & `sageworks-0.1.5.3/aws_setup/sageworks_cdk/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/aws_setup/sageworks_cdk/stacks/sageworks_stack.py` & `sageworks-0.1.5.3/aws_setup/sageworks_cdk/stacks/sageworks_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/aws_setup/sageworks_cdk/tests/unit/test_sageworks_sandbox_stack.py` & `sageworks-0.1.5.3/aws_setup/sageworks_cdk/tests/unit/test_sageworks_sandbox_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/data/abalone.csv` & `sageworks-0.1.5.3/data/abalone.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/data/test_data.json` & `sageworks-0.1.5.3/data/test_data.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/docs/admin_notes.md` & `sageworks-0.1.5.3/docs/admin_notes.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/docs/images/big_spider.png` & `sageworks-0.1.5.3/docs/images/big_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/docs/images/graph_representation.png` & `sageworks-0.1.5.3/docs/images/graph_representation.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/docs/images/powered_aws_dark_blue.png` & `sageworks-0.1.5.3/docs/images/powered_aws_dark_blue.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/docs/images/powered_aws_transparent.png` & `sageworks-0.1.5.3/docs/images/powered_aws_transparent.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/docs/images/powered_aws_white.png` & `sageworks-0.1.5.3/docs/images/powered_aws_white.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/docs/images/powered_aws_with_tm_grey.png` & `sageworks-0.1.5.3/docs/images/powered_aws_with_tm_grey.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/docs/images/sageworks.png` & `sageworks-0.1.5.3/docs/images/sageworks.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/docs/images/sageworks_concepts.png` & `sageworks-0.1.5.3/docs/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/docs/images/scp.png` & `sageworks-0.1.5.3/docs/images/scp.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/docs/images/scp_labs.png` & `sageworks-0.1.5.3/docs/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/docs/images/small_spider.png` & `sageworks-0.1.5.3/docs/images/small_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/docs/sageworks_classes_concepts.md` & `sageworks-0.1.5.3/docs/sageworks_classes_concepts.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/docs/scp_consulting.md` & `sageworks-0.1.5.3/docs/scp_consulting.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/examples/data_to_data_example.py` & `sageworks-0.1.5.3/examples/data_to_data_example.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/notebooks/ML_Pipeline_with_SageWorks.ipynb` & `sageworks-0.1.5.3/notebooks/ML_Pipeline_with_SageWorks.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/notebooks/images/athena_query_aqsol.png` & `sageworks-0.1.5.3/notebooks/images/athena_query_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/notebooks/images/aws_dashboard_aqsol.png` & `sageworks-0.1.5.3/notebooks/images/aws_dashboard_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/notebooks/images/dashboard_aqsol_features.png` & `sageworks-0.1.5.3/notebooks/images/dashboard_aqsol_features.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/notebooks/images/model_screenshot.png` & `sageworks-0.1.5.3/notebooks/images/model_screenshot.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/notebooks/images/sageworks_concepts.png` & `sageworks-0.1.5.3/notebooks/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/notebooks/images/scp_labs.png` & `sageworks-0.1.5.3/notebooks/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/scripts/data_source_tags.py` & `sageworks-0.1.5.3/scripts/data_source_tags.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/scripts/generate_jsonl_data.py` & `sageworks-0.1.5.3/scripts/generate_jsonl_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/scripts/list_data_sources.py` & `sageworks-0.1.5.3/scripts/list_data_sources.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/setup.cfg` & `sageworks-0.1.5.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/setup.py` & `sageworks-0.1.5.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 #!/usr/bin/env python
 """Setup.py for SageWorks: Sagemaker Workbench"""
 
 import os
 import glob
-
 from setuptools import setup, find_packages
 
 readme = open("Readme.md").read()
 
+# Requirements
+path = os.path.abspath(os.path.dirname(__file__))
+with open(os.path.join(path, "requirements.txt")) as f:
+    install_requires = f.read().strip().split("\n")
+
 
 # Data and Example Files
 def get_files(dir_name):
     """Simple directory walker"""
     return [(os.path.join(".", d), [os.path.join(d, f) for f in files]) for d, _, files in os.walk(dir_name)]
 
 
 setup(
     name="sageworks",
     # use_scm_version=True,
-    version="0.1.5.2",
+    version="0.1.5.3",
     description="SageWorks: A Python WorkBench for creating and deploying SageMaker Models",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="SuperCowPowers LLC",
     author_email="support@supercowpowers.com",
     url="https://github.com/SuperCowPowers/sageworks",
     packages=find_packages("src"),
     package_dir={"": "src"},
     py_modules=[os.path.splitext(os.path.basename(path))[0] for path in glob.glob("src/*.py")],
     include_package_data=True,
     data_files=get_files("data") + get_files("examples"),
-    install_requires=[
-        "boto3",
-        "awswrangler >= 3.0.0",
-        "sagemaker >= 2.143",
-        "pandas",
-        "scikit-learn",
-        "redis",
-        "dash",
-        "dash-bootstrap-components",
-        "dash-bootstrap-templates",
-        "termcolor",
-    ],
+    install_requires=install_requires,
     license="MIT",
     keywords="SageMaker, Machine Learning, AWS, Python, Utilities",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
     setup_requires=["setuptools_scm", "setuptools"],
+    entry_points={
+        "console_scripts": [
+            "sageworks = sageworks.cli.cli:cli",
+        ],
+    },
 )
```

### Comparing `sageworks-0.1.5.2/src/sageworks/__init__.py` & `sageworks-0.1.5.3/src/sageworks/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/algorithms/table/light/data_source_eda.py` & `sageworks-0.1.5.3/src/sageworks/algorithms/table/light/data_source_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/algorithms/table/light/feature_spider.py` & `sageworks-0.1.5.3/src/sageworks/algorithms/table/light/feature_spider.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/algorithms/table/light/row_tagger.py` & `sageworks-0.1.5.3/src/sageworks/algorithms/table/light/row_tagger.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/artifacts/Readme.md` & `sageworks-0.1.5.3/src/sageworks/artifacts/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/artifacts/artifact.py` & `sageworks-0.1.5.3/src/sageworks/artifacts/artifact.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     log = logging.getLogger(__name__)
 
     # Set up our Boto3 and SageMaker Session and SageMaker Client
     aws_account_clamp = AWSAccountClamp()
     boto_session = aws_account_clamp.boto_session()
     sm_session = aws_account_clamp.sagemaker_session(boto_session)
     sm_client = aws_account_clamp.sagemaker_client(boto_session)
-    aws_region = aws_account_clamp.region()
+    aws_region = aws_account_clamp.region
 
     # AWSServiceBroker pulls and collects metadata from a bunch of AWS Services
     aws_broker = AWSServiceBroker()
 
     # Grab our SageWorksConfig for S3 Buckets and other SageWorks specific settings
     sageworks_config = SageWorksConfig()
     data_catalog_db = "sageworks"
@@ -76,15 +76,15 @@
 
     @abstractmethod
     def aws_url(self):
         """AWS console/web interface for this artifact"""
         pass
 
     @abstractmethod
-    def all_meta(self) -> dict:
+    def aws_meta(self) -> dict:
         """Get the full AWS metadata for this artifact"""
         pass
 
     @abstractmethod
     def delete(self):
         """Delete this artifact including all related AWS objects"""
         pass
@@ -115,32 +115,49 @@
 
     def sageworks_tags(self) -> list:
         """Get the tags for this artifact"""
         combined_tags = self.sageworks_meta().get("sageworks_tags", "")
         tags = combined_tags.split(":")
         return tags
 
+    def get_input(self) -> str:
+        """Get the input data for this artifact"""
+        return self.sageworks_meta().get("sageworks_input", "unknown")
+
+    def get_status(self) -> str:
+        """Get the status for this artifact"""
+        return self.sageworks_meta().get("sageworks_status", "unknown")
+
+    def set_status(self, status: str):
+        """Set the status for this artifact
+        Args:
+            status (str): Status to set for this artifact
+        """
+        current_meta = self.sageworks_meta()
+        current_meta["sageworks_status"] = status
+        self.upsert_sageworks_meta(current_meta)
+
     def summary(self) -> dict:
         """This is generic summary information for all Artifacts. If you
         want to get more detailed information, call the details() method
         which is implemented by the specific Artifact class"""
         return {
             "uuid": self.uuid,
             "aws_arn": self.arn(),
-            "aws_url": self.aws_url(),
             "size": self.size(),
             "created": self.created(),
             "modified": self.modified(),
+            "input": self.get_input(),
             "sageworks_tags": self.sageworks_tags(),
         }
 
     @staticmethod
     def _aws_tags_to_dict(aws_tags) -> dict:
         """Internal: AWS Tags are in an odd format, so convert to regular dictionary"""
-        return {item["Key"]: item["Value"] for item in aws_tags if "sageworks" in item["Key"]}
+        return {item["Key"]: item["Value"] for item in aws_tags}
 
     @staticmethod
     def _dict_to_aws_tags(meta_data: dict) -> list:
         """Internal: AWS Tags are in an odd format, so we need to dictionary
         Args:
             meta_data (dict): Dictionary of metadata to convert to AWS Tags
         """
```

### Comparing `sageworks-0.1.5.2/src/sageworks/artifacts/data_sources/athena_source.py` & `sageworks-0.1.5.3/src/sageworks/artifacts/feature_sets/feature_set.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,384 +1,391 @@
-"""AthenaSource: SageWorks Data Source accessible through Athena"""
+"""FeatureSet: SageWorks Feature Set accessible through Athena"""
+import time
+from datetime import datetime, timezone
+
+import botocore.exceptions
 import pandas as pd
 import awswrangler as wr
-from datetime import datetime
-import json
+import numpy as np
+
+from sagemaker.feature_store.feature_group import FeatureGroup
+from sagemaker.feature_store.feature_store import FeatureStore
 
 # SageWorks Imports
-from sageworks.artifacts.data_sources.data_source_abstract import DataSourceAbstract
+from sageworks.artifacts.artifact import Artifact
+from sageworks.artifacts.data_sources.data_source import DataSource
+from sageworks.artifacts.data_sources.athena_source import AthenaSource
 from sageworks.aws_service_broker.aws_service_broker import ServiceCategory
 from sageworks.utils.iso_8601 import convert_all_to_iso8601
 
 
-class AthenaSource(DataSourceAbstract):
-    """AthenaSource: SageWorks Data Source accessible through Athena
+class FeatureSet(Artifact):
+    """FeatureSet: SageWorks Feature Set accessible through Athena
 
     Common Usage:
-        my_data = AthenaSource(data_uuid, database="sageworks")
-        my_data.summary()
-        my_data.details()
-        df = my_data.query(f"select * from {data_uuid} limit 5")
+        my_features = FeatureSet(feature_uuid)
+        my_features.summary()
+        my_features.details()
     """
 
-    def __init__(self, data_uuid, database="sageworks"):
-        """AthenaSource Initialization
+    def __init__(self, feature_uuid, force_refresh: bool = False):
+        """FeatureSet Initialization
 
         Args:
-            data_uuid (str): Name of Athena Table
-            database (str): Athena Database Name
+            feature_uuid (str): Name of Feature Set in SageWorks Metadata.
+            force_refresh (bool, optional): Force a refresh of the metadata. Defaults to False.
         """
-
         # Call superclass init
-        super().__init__(data_uuid)
+        super().__init__(feature_uuid)
+
+        # Grab an AWS Metadata Broker object and pull information for Feature Sets
+        self.feature_set_name = feature_uuid
+
+        # Refresh our feature and data source metadata
+        self.feature_meta = self._refresh_broker(force_refresh)
 
-        self.data_catalog_db = database
-        self.table_name = data_uuid
+        # Sanity check and then set up our FeatureSet attributes
+        if self.feature_meta is None:
+            self.log.info(f"Could not find feature set {self.feature_set_name} within current visibility scope")
+            self.data_source = None
+            return
+        else:
+            self.record_id = self.feature_meta["RecordIdentifierFeatureName"]
+            self.event_time = self.feature_meta["EventTimeFeatureName"]
+
+            # Pull Athena and S3 Storage information from metadata
+            self.athena_database = self.feature_meta["sageworks_meta"].get("athena_database")
+            self.athena_table = self.feature_meta["sageworks_meta"].get("athena_table")
+            self.s3_storage = self.feature_meta["sageworks_meta"].get("s3_storage")
+
+            # Create our internal DataSource (hardcoded to Athena for now)
+            self.data_source = AthenaSource(self.athena_table, self.athena_database, force_refresh=force_refresh)
 
-        # Refresh our internal catalog metadata
-        self.catalog_table_meta = None
-        self.refresh()
+        # Spin up our Feature Store
+        self.feature_store = FeatureStore(self.sm_session)
 
         # All done
-        print(f"AthenaSource Initialized: {self.data_catalog_db}.{self.table_name}")
+        self.log.info(f"FeatureSet Initialized: {self.feature_set_name}")
 
-    def refresh(self, force_fresh: bool = False):
-        """Refresh our internal catalog metadata
+    def _refresh_broker(self, force_refresh: bool = False):
+        """Internal: Refresh our internal AWS Feature Store metadata
         Args:
-            force_fresh (bool): Force a refresh of the metadata
+            force_refresh (bool, optional): Force a refresh of the metadata. Defaults to False.
         """
-        _catalog_meta = self.aws_broker.get_metadata(ServiceCategory.DATA_CATALOG, force_fresh=force_fresh)
-        self.catalog_table_meta = _catalog_meta[self.data_catalog_db].get(self.table_name)
+        _catalog_meta = self.aws_broker.get_metadata(ServiceCategory.FEATURE_STORE, force_refresh=force_refresh)
+        return _catalog_meta.get(self.feature_set_name)
 
     def check(self) -> bool:
-        """Validation Checks for this Data Source"""
-
-        # We're we able to pull AWS Metadata for this table_name?"""
-        if self.catalog_table_meta is None:
-            self.log.info(f"AthenaSource.check() {self.table_name} not found in SageWorks Metadata...")
+        """Does the feature_set_name exist in the AWS Metadata?"""
+        if self.feature_meta is None:
+            self.log.info(f"FeatureSet.check() {self.feature_set_name} not found in AWS Metadata!")
             return False
+        else:  # Also check our Data Source
+            if not self.data_source.check():
+                self.log.critical(f"Data Source check failed for {self.feature_set_name}")
+                self.log.critical("Delete this Feature Set and recreate it to fix this issue")
+                return False
+        # AOK
         return True
 
-    def deep_check(self) -> bool:
-        """These are more comprehensive checks for this Data Source (may take a LONG TIME)"""
-
-        # Can we run an Athena Test Query
-        try:
-            self.athena_test_query()
-            return True
-        except Exception as exc:
-            self.log.critical(f"Athena Test Query Failed: {exc}")
-            return False
+    def aws_meta(self) -> dict:
+        """Get ALL the AWS metadata for this artifact"""
+        return self.feature_meta
 
     def arn(self) -> str:
         """AWS ARN (Amazon Resource Name) for this artifact"""
-        # Grab our SageWorks Role Manager, get our AWS account id, and region for ARN creation
-        account_id = self.aws_account_clamp.account_id()
-        region = self.aws_account_clamp.region()
-        arn = f"arn:aws:glue:{region}:{account_id}:table/{self.data_catalog_db}/{self.table_name}"
-        return arn
-
-    def sageworks_meta(self):
-        """Get the SageWorks specific metadata for this Artifact"""
-        params = self.all_meta().get("Parameters", {})
-        return {key: value for key, value in params.items() if "sageworks" in key}
-
-    def upsert_sageworks_meta(self, new_meta: dict):
-        """Add SageWorks specific metadata to this Artifact
-        Args:
-            new_meta (dict): Dictionary of new metadata to add
-        """
-        # Grab our existing metadata
-        meta = self.sageworks_meta()
-
-        # Make sure the new data has keys that are valid
-        for key in new_meta.keys():
-            if not key.startswith("sageworks_"):
-                new_meta[f"sageworks_{key}"] = new_meta.pop(key)
-
-        # Now convert any non-string values to JSON strings
-        for key, value in new_meta.items():
-            if not isinstance(value, str):
-                new_meta[key] = json.dumps(value)
-
-        # Update our existing metadata with the new metadata
-        meta.update(new_meta)
-
-        # Store our updated metadata
-        wr.catalog.upsert_table_parameters(
-            parameters=meta,
-            database=self.data_catalog_db,
-            table=self.table_name,
-            boto3_session=self.boto_session,
-        )
+        return self.feature_meta["FeatureGroupArn"]
 
     def size(self) -> float:
-        """Return the size of this data in MegaBytes"""
-        size_in_bytes = sum(wr.s3.size_objects(self.s3_storage_location(), boto3_session=self.boto_session).values())
-        size_in_mb = size_in_bytes / 1_000_000
-        return size_in_mb
-
-    def all_meta(self) -> dict:
-        """Get the FULL AWS metadata for this artifact"""
-        return self.catalog_table_meta
-
-    def aws_url(self):
-        """The AWS URL for looking at/querying this data source"""
-        return f"https://{self.aws_region}.console.aws.amazon.com/athena/home"
+        """Return the size of the internal DataSource in MegaBytes"""
+        return self.data_source.size()
 
-    def created(self) -> datetime:
-        """Return the datetime when this artifact was created"""
-        return self.catalog_table_meta["CreateTime"]
+    def column_names(self) -> list[str]:
+        """Return the column names of the Feature Set"""
+        return list(self.column_details().keys())
 
-    def modified(self) -> datetime:
-        """Return the datetime when this artifact was last modified"""
-        return self.catalog_table_meta["UpdateTime"]
+    def column_types(self) -> list[str]:
+        """Return the column types of the Feature Set"""
+        return list(self.column_details().values())
 
-    def num_rows(self) -> int:
-        """Return the number of rows for this Data Source"""
-        count_df = self.query(f'select count(*) AS count from "{self.data_catalog_db}"."{self.table_name}"')
-        return count_df["count"][0]
+    def column_details(self) -> dict:
+        """Return the column details of the Feature Set"""
+        return {item["FeatureName"]: item["FeatureType"] for item in self.feature_meta["FeatureDefinitions"]}
 
     def num_columns(self) -> int:
-        """Return the number of columns for this Data Source"""
+        """Return the number of columns of the Feature Set"""
         return len(self.column_names())
 
-    def column_names(self) -> list[str]:
-        """Return the column names for this Athena Table"""
-        return [item["Name"] for item in self.catalog_table_meta["StorageDescriptor"]["Columns"]]
-
-    def column_types(self) -> list[str]:
-        """Return the column types of the internal AthenaSource"""
-        return [item["Type"] for item in self.catalog_table_meta["StorageDescriptor"]["Columns"]]
+    def num_rows(self) -> int:
+        """Return the number of rows of the internal DataSource"""
+        return self.data_source.num_rows()
 
     def query(self, query: str) -> pd.DataFrame:
-        """Query the AthenaSource"""
-        df = wr.athena.read_sql_query(sql=query, database=self.data_catalog_db, boto3_session=self.boto_session)
-        scanned_bytes = df.query_metadata["Statistics"]["DataScannedInBytes"]
-        self.log.info(f"Athena Query successful (scanned bytes: {scanned_bytes})")
-        return df
-
-    def s3_storage_location(self) -> str:
-        """Get the S3 Storage Location for this Data Source"""
-        return self.catalog_table_meta["StorageDescriptor"]["Location"]
-
-    def athena_test_query(self):
-        """Validate that Athena Queries are working"""
-        query = f"select count(*) as count from {self.table_name}"
-        df = wr.athena.read_sql_query(sql=query, database=self.data_catalog_db, boto3_session=self.boto_session)
-        scanned_bytes = df.query_metadata["Statistics"]["DataScannedInBytes"]
-        self.log.info(f"Athena TEST Query successful (scanned bytes: {scanned_bytes})")
+        """Query the internal DataSource"""
+        return self.data_source.query(query)
 
-    def sample_df(self, recompute: bool = False) -> pd.DataFrame:
-        """Pull a sample of rows from the DataSource
-        Args:
-            recompute(bool): Recompute the sample (default: False)
-        Returns:
-            pd.DataFrame: A sample DataFrame from this DataSource
-        """
-
-        # First check if we have already computed the quartiles
-        if self.sageworks_meta().get("sageworks_sample_rows") and not recompute:
-            return pd.read_json(self.sageworks_meta()["sageworks_sample_rows"], orient="records", lines=True)
-
-        # Note: Hardcoded to 100 rows so that metadata storage is consistent
-        sample_rows = 100
-        num_rows = self.num_rows()
-        if num_rows > sample_rows:
-            # Bernoulli Sampling has reasonable variance so we're going to +1 the
-            # sample percentage and then simply clamp it to 100 rows
-            percentage = round(sample_rows * 100.0 / num_rows) + 1
-            self.log.warning(f"DataSource has {num_rows} rows.. sampling down to {sample_rows}...")
-            query = f"SELECT * FROM {self.table_name} TABLESAMPLE BERNOULLI({percentage})"
-        else:
-            query = f"SELECT * FROM {self.table_name}"
-        sample_df = self.query(query).head(sample_rows)
+    def aws_url(self):
+        """The AWS URL for looking at/querying the underlying data source"""
+        return self.data_source.details().get("aws_url", "unknown")
 
-        # Store the sample_df in our SageWorks metadata
-        rows_json = sample_df.to_json(orient="records", lines=True)
-        self.upsert_sageworks_meta({"sageworks_sample_rows": rows_json})
+    def created(self) -> datetime:
+        """Return the datetime when this artifact was created"""
+        return self.feature_meta["CreationTime"]
 
-        # Return the sample_df
-        return sample_df
+    def modified(self) -> datetime:
+        """Return the datetime when this artifact was last modified"""
+        # Note: We can't currently figure out how to this from AWS Metadata
+        return self.feature_meta["CreationTime"]
 
-    def quartiles(self, recompute: bool = False) -> dict[dict]:
-        """Compute Quartiles for all the numeric columns in a DataSource
-        Args:
-            recompute(bool): Recompute the quartiles (default: False)
-        Returns:
-            dict(dict): A dictionary of quartiles for each column in the form
-                 {'col1': {'min': 0, 'q1': 1, 'median': 2, 'q3': 3, 'max': 4},
-                  'col2': ...}
+    def get_data_source(self) -> DataSource:
+        """Return the underlying DataSource object"""
+        return self.data_source
+
+    def get_feature_store(self) -> FeatureStore:
+        """Return the underlying AWS FeatureStore object. This can be useful for more advanced usage
+        with create_dataset() such as Joins and time ranges and a host of other options
+        See: https://docs.aws.amazon.com/sagemaker/latest/dg/feature-store-create-a-dataset.html
         """
+        return self.feature_store
 
-        # First check if we have already computed the quartiles
-        if self.sageworks_meta().get("sageworks_quartiles") and not recompute:
-            return json.loads(self.sageworks_meta()["sageworks_quartiles"])
-
-        # For every column in the table that is numeric, get the quartiles
-        self.log.info("Computing Quartiles for all numeric columns (this may take a while)...")
-        quartile_data = []
-        for column, data_type in zip(self.column_names(), self.column_types()):
-            print(column, data_type)
-            if data_type in ["bigint", "double", "int", "smallint", "tinyint"]:
-                query = (
-                    f'SELECT MIN("{column}") AS min, '
-                    f'approx_percentile("{column}", 0.25) AS q1, '
-                    f'approx_percentile("{column}", 0.5) AS median, '
-                    f'approx_percentile("{column}", 0.75) AS q3, '
-                    f'MAX("{column}") AS max FROM {self.table_name}'
-                )
-                result_df = self.query(query)
-                result_df["column_name"] = column
-                quartile_data.append(result_df)
-        quartile_dict = pd.concat(quartile_data).set_index("column_name").to_dict(orient="index")
-
-        # Push the quartile data into our DataSource Metadata
-        self.upsert_sageworks_meta({"sageworks_quartiles": quartile_dict})
-
-        # Return the quartile data
-        return quartile_dict
-
-    def value_counts(self, recompute: bool = False) -> dict[dict]:
-        """Compute 'value_counts' for all the string columns in a DataSource
+    def create_s3_training_data(self, training_split=80, test_split=20, val_split=0) -> str:
+        """Create some Training Data (S3 CSV) from a Feature Set using standard options. If you want
+        additional options/features use the get_feature_store() method and see AWS docs for all
+        the details: https://docs.aws.amazon.com/sagemaker/latest/dg/feature-store-create-a-dataset.html
         Args:
-            recompute(bool): Recompute the value counts (default: False)
+            training_split (int): Percentage of data that goes into the TRAINING set
+            test_split (int): Percentage of data that goes into the TEST set
+            val_split (int): Percentage of data that goes into the VALIDATION set (default=0)
         Returns:
-            dict(dict): A dictionary of value counts for each column in the form
-                 {'col1': {'value_1': X, 'value_2': Y, 'value_3': Z,...},
-                  'col2': ...}
+            str: The full path/file for the CSV file created by Feature Store create_dataset()
         """
 
-        # First check if we have already computed the quartiles
-        if self.sageworks_meta().get("sageworks_value_counts") and not recompute:
-            return json.loads(self.sageworks_meta()["sageworks_value_counts"])
-
-        # For every column in the table that is numeric, get the quartiles
-        self.log.info("Computing 'value_counts' for all string columns...")
-        value_count_dict = dict()
-        for column, data_type in zip(self.column_names(), self.column_types()):
-            print(column, data_type)
-            if data_type in ["string"]:
-                query = (
-                    f'SELECT "{column}", count(*) as count '
-                    f"FROM {self.table_name} "
-                    f'GROUP BY "{column}" ORDER BY count DESC limit 10'
-                )
-                # Convert int64 to int so that we can serialize to JSON
-                result_df = self.query(query)
-                result_df["count"] = result_df["count"].astype(int)
-
-                # Convert the result_df into a dictionary
-                value_count_dict[column] = dict(zip(result_df[column], result_df["count"]))
-
-        # Push the value_count data into our DataSource Metadata
-        self.upsert_sageworks_meta({"sageworks_value_counts": value_count_dict})
-
-        # Return the value_count data
-        return value_count_dict
+        # Set up the S3 Query results path
+        date_time = datetime.now(timezone.utc).strftime("%Y-%m-%d_%H:%M:%S")
+        s3_output_path = self.feature_sets_s3_path + f"/{self.feature_set_name}/datasets/all_{date_time}"
+
+        # Get the snapshot query
+        query = self.snapshot_query()
+
+        # Make the query
+        athena_query = FeatureGroup(name=self.feature_set_name, sagemaker_session=self.sm_session).athena_query()
+        athena_query.run(query, output_location=s3_output_path)
+        self.log.info("Waiting for Athena Query...")
+        athena_query.wait()
+        query_execution = athena_query.get_query_execution()
+
+        # Get the full path to the S3 files with the results
+        full_s3_path = s3_output_path + f"/{query_execution['QueryExecution']['QueryExecutionId']}.csv"
+        return full_s3_path
+
+    def snapshot_query(self):
+        """An Athena query to get the latest snapshot of features"""
+        # Remove FeatureGroup metadata columns that might have gotten added
+        columns = self.column_names()
+        filter_columns = ["write_time", "api_invocation_time", "is_deleted"]
+        columns = ", ".join(['"' + x + '"' for x in columns if x not in filter_columns])
+
+        query = (
+            f"SELECT {columns} "
+            f"    FROM (SELECT *, row_number() OVER (PARTITION BY {self.record_id} "
+            f"        ORDER BY {self.event_time} desc, api_invocation_time DESC, write_time DESC) AS row_num "
+            f'        FROM "{self.athena_table}") '
+            "    WHERE row_num = 1 and  NOT is_deleted;"
+        )
+        return query
 
     def details(self, recompute: bool = False) -> dict[dict]:
-        """Additional Details about this AthenaSource Artifact
+        """Additional Details about this FeatureSet Artifact
         Args:
             recompute(bool): Recompute the details (default: False)
         Returns:
-            dict(dict): A dictionary of details about this AthenaSource
+            dict(dict): A dictionary of details about this FeatureSet
         """
-
         # First check if we have already computed the details
-        if self.sageworks_meta().get("sageworks_details") and not recompute:
-            return json.loads(self.sageworks_meta()["sageworks_details"])
+        if self.sageworks_meta().get("details_computed") and not recompute:
+            # Get the SageWorks Metadata
+            meta = self.sageworks_meta()
+
+            # Hack for AWS URL
+            meta["aws_url"] = meta["aws_url"].replace("__question__", "?").replace("__pound__", "#")
+            return meta
+
+        # Create a dictionary of details
+        details = dict()
+        details["details_computed"] = True
+
+        # Number of Columns
+        details["num_columns"] = self.num_columns()
+
+        # Number of Rows
+        details["num_rows"] = self.num_rows()
+
+        # Additional Details
+        details["sageworks_status"] = self.get_status()
+        details["sageworks_input"] = self.get_input()
+        details["sageworks_tags"] = ":".join(self.sageworks_tags())
+
+        # Underlying Storage Details
+        details["storage_type"] = "athena"  # TODO: Add RDS support
+        details["storage_uuid"] = self.data_source.uuid
 
-        details = super().details()
-        details["s3_storage_location"] = self.s3_storage_location()
+        # SageMaker Tags have a bunch of constraints so we need to do some replacements
+        details["aws_url"] = self.aws_url().replace("?", "__question__").replace("#", "__pound__")
 
         # Convert any datetime fields to ISO-8601 strings
         details = convert_all_to_iso8601(details)
 
         # Push the details data into our DataSource Metadata
-        self.upsert_sageworks_meta({"sageworks_details": details})
+        self.upsert_sageworks_meta(details)
 
         # Return the details data
         return details
 
     def delete(self):
-        """Delete the AWS Data Catalog Table and S3 Storage Objects"""
+        """Delete the Feature Set: Feature Group, Catalog Table, and S3 Storage Objects"""
 
-        # Make sure the Feature Group exists
-        if not self.check():
-            self.log.warning(f"Trying to delete a AthenaSource that doesn't exist: {self.table_name}")
-
-        # Delete Data Catalog Table
-        self.log.info(f"Deleting DataCatalog Table: {self.data_catalog_db}.{self.table_name}...")
-        wr.catalog.delete_table_if_exists(self.data_catalog_db, self.table_name, boto3_session=self.boto_session)
-
-        # Delete S3 Storage Objects
-        self.log.info(f"Deleting S3 Storage Object: {self.s3_storage_location()}...")
-        wr.s3.delete_objects(self.s3_storage_location(), boto3_session=self.boto_session)
+        # Delete the Feature Group and ensure that it gets deleted
+        remove_fg = FeatureGroup(name=self.feature_set_name, sagemaker_session=self.sm_session)
+        remove_fg.delete()
+        self.ensure_feature_group_deleted(remove_fg)
+
+        # Delete our underlying DataSource (Data Catalog Table and S3 Storage Objects)
+        self.data_source.delete()
+
+        # Feature Sets can often have a lot of cruft so delete the entire bucket/prefix
+        s3_delete_path = self.feature_sets_s3_path + f"/{self.feature_set_name}"
+        self.log.info(f"Deleting S3 Storage Objects {s3_delete_path}")
+        wr.s3.delete_objects(s3_delete_path, boto3_session=self.boto_session)
+
+    def ensure_feature_group_deleted(self, feature_group):
+        status = "Deleting"
+        while status == "Deleting":
+            self.log.info("FeatureSet being Deleted...")
+            try:
+                status = feature_group.describe().get("FeatureGroupStatus")
+            except botocore.exceptions.ClientError as error:
+                # If the exception is a ResourceNotFound, this is fine, otherwise raise all other exceptions
+                if error.response["Error"]["Code"] == "ResourceNotFound":
+                    break
+                else:
+                    raise error
+            time.sleep(1)
+        self.log.info(f"FeatureSet {feature_group.name} successfully deleted")
 
+    def quartiles(self, recompute: bool = False) -> dict:
+        """Get the quartiles for the numeric columns of the underlying DataSource
+        Args:
+            recompute (bool): Recompute the quartiles (default=False)
+        Returns:
+            dict: A dictionary of quartiles for the numeric columns
+        """
+        return self.data_source.quartiles(recompute)
 
-if __name__ == "__main__":
-    """Exercise the AthenaSource Class"""
-    from pprint import pprint
+    def sample_df(self, recompute: bool = False) -> pd.DataFrame:
+        """Get a sample of the data from the underlying DataSource
+        Args:
+            recompute (bool): Recompute the sample (default=False)
+        Returns:
+            pd.DataFrame: A sample of the data from the underlying DataSource
+        """
+        return self.data_source.sample_df(recompute)
+
+    def outliers(self, scale: float = 1.7, recompute: bool = False) -> pd.DataFrame:
+        """Compute outliers for all the numeric columns in a DataSource
+        Args:
+            scale(float): The scale to use for the IQR (default: 1.7)
+            recompute(bool): Recompute the outliers (default: False)
+        Returns:
+            pd.DataFrame: A DataFrame of outliers from this DataSource
+        Notes:
+            Uses the IQR * 1.7 (~= 3 Sigma) method to compute outliers
+            The scale parameter can be adjusted to change the IQR multiplier
+        """
+        return self.data_source.outliers(scale, recompute)
+
+    def anomalies(self) -> pd.DataFrame:
+        """Get a set of anomalous data from the underlying DataSource
+        Returns:
+            pd.DataFrame: A dataframe of anomalies from the underlying DataSource
+        """
 
-    # Retrieve a Data Source
-    my_data = AthenaSource("test_data")
+        # FIXME: Mock this for now
+        anom_df = self.sample_df().copy()
+        anom_df["anomaly_score"] = np.random.rand(anom_df.shape[0])
+        anom_df["cluster"] = np.random.randint(0, 10, anom_df.shape[0])
+        anom_df["x"] = np.random.rand(anom_df.shape[0])
+        anom_df["y"] = np.random.rand(anom_df.shape[0])
+        return anom_df
 
-    # Verify that the Athena Data Source exists
-    assert my_data.check()
+    def value_counts(self, recompute: bool = False) -> dict:
+        """Get the quartiles for the string columns of the underlying DataSource
+        Args:
+            recompute (bool): Recompute the value counts (default=False)
+        Returns:
+            dict: A dictionary of value counts for the string columns
+        """
+        return self.data_source.value_counts(recompute)
 
-    # What's my SageWorks UUID
-    print(f"UUID: {my_data.uuid}")
 
-    # What's my AWS ARN and URL
-    print(f"AWS ARN: {my_data.arn()}")
-    print(f"AWS URL: {my_data.aws_url()}")
+if __name__ == "__main__":
+    """Exercise for FeatureSet Class"""
+    from pprint import pprint
 
-    # Get the S3 Storage for this Data Source
-    print(f"S3 Storage: {my_data.s3_storage_location()}")
+    # Setup Pandas output options
+    pd.set_option("display.max_colwidth", 50)
+    pd.set_option("display.max_columns", 15)
+    pd.set_option("display.width", 1000)
 
-    # What's the size of the data?
-    print(f"Size of Data (MB): {my_data.size()}")
+    # Grab a FeatureSet object and pull some information from it
+    my_features = FeatureSet("abalone_feature_set")
 
-    # When was it created and last modified?
-    print(f"Created: {my_data.created()}")
-    print(f"Modified: {my_data.modified()}")
+    # Call the various methods
+    # What's my AWS ARN and URL
+    print(f"AWS ARN: {my_features.arn()}")
+    print(f"AWS URL: {my_features.aws_url()}")
 
-    # Column Names and Types
-    print(f"Column Names: {my_data.column_names()}")
-    print(f"Column Types: {my_data.column_types()}")
+    # Let's do a check/validation of the feature set
+    print(f"Feature Set Check: {my_features.check()}")
 
-    # Get Tags associated with this Artifact
-    print(f"Tags: {my_data.sageworks_tags()}")
+    # How many rows and columns?
+    num_rows = my_features.num_rows()
+    num_columns = my_features.num_columns()
+    print(f"Rows: {num_rows} Columns: {num_columns}")
+
+    # What are the column names?
+    columns = my_features.column_names()
+    print(columns)
+
+    # Get the metadata and tags associated with this feature set
+    print(f"SageWorks Meta: {my_features.sageworks_meta()}")
+    print(f"SageWorks Tags: {my_features.sageworks_tags()}")
+
+    # Get a summary for this Feature Set
+    print("\nSummary:")
+    pprint(my_features.summary())
+
+    # Get the details for this Feature Set
+    print("\nDetails:")
+    pprint(my_features.details(recompute=True))
+
+    # Now do deep dive on storage
+    storage = my_features.get_data_source()
+    print("\nStorage Details:")
+    pprint(storage.details())
 
     # Get a sample of the data
-    df = my_data.sample_df()
+    df = my_features.sample_df()
     print(f"Sample Data: {df.shape}")
     print(df)
 
-    # Get the SageWorks Metadata for this Data Source
-    meta = my_data.sageworks_meta()
-    print("\nSageWorks Meta")
-    pprint(meta)
-
-    # Get details for this Data Source
-    my_details = my_data.details(recompute=True)
-    print("\nDetails")
-    pprint(my_details)
-
-    # Get quartiles for numeric columns
-    quartile_info = my_data.quartiles(recompute=True)
-    print("\nQuartiles")
+    # Get quartiles for all the columns
+    quartile_info = my_features.quartiles()
+    print("Quartiles")
     pprint(quartile_info)
 
-    # Get value_counts for string columns
-    value_count_info = my_data.value_counts(recompute=True)
-    print("\nValue Counts")
-    pprint(value_count_info)
-
-    # Get ALL Metadata associated with this Artifact
-    print("\n\nALL Meta")
-    pprint(my_data.all_meta())
-
-    # Now delete the AWS artifacts associated with this DataSource
-    # print('Deleting SageWorks Data Source...')
-    # my_data.delete()
+    # Get outliers for all the columns
+    anom_df = my_features.outliers()
+    print(anom_df)
+
+    # Now delete the AWS artifacts associated with this Feature Set
+    # print('Deleting SageWorks Feature Set...')
+    # my_features.delete()
```

### Comparing `sageworks-0.1.5.2/src/sageworks/artifacts/data_sources/data_source.py` & `sageworks-0.1.5.3/src/sageworks/artifacts/data_sources/data_source.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,27 +23,28 @@
         sample_df(): Returns a SAMPLED pd.DataFrame from this DataSource
         summary(): Returns a summary of this DataSource
         details(): Returns additional details about this DataSource
         quartiles(): Returns the quartiles for each numeric column in this DataSource
         value_counts(): Returns the value counts for each string column in this DataSource
         sageworks_meta(): Returns the SageWorks Metadata for this DataSource
         sageworks_tags(): Returns the SageWorks Tags for this DataSource
-        all_meta(): Returns ALL AWS Metadata for this DataSource
+        aws_meta(): Returns ALL AWS Metadata for this DataSource
     """
 
-    def __new__(cls, uuid, data_source_type: str = "athena"):
+    def __new__(cls, uuid, force_refresh: bool = False, data_source_type: str = "athena"):
         """DataSource: A Factory for DataSources (Athena, RDS, etc)
         Args:
             uuid: The UUID of the DataSource
+            force_refresh(bool): Force a refresh of the DataSource (default: False)
             data_source_type: The type of DataSource (athena, rds, etc)
         Returns:
             object: A concrete DataSource class (AthenaSource, RDSSource)
         """
         if data_source_type == "athena":
-            return AthenaSource(uuid)
+            return AthenaSource(uuid, force_refresh=force_refresh)
         else:
             raise NotImplementedError(f"DataSource type {data_source_type} not implemented")
 
 
 if __name__ == "__main__":
     """Exercise the DataSource Factory Class"""
     from pprint import pprint
@@ -74,13 +75,16 @@
     # Column Names and Types
     print(f"Column Names: {my_data.column_names()}")
     print(f"Column Types: {my_data.column_types()}")
 
     # Get Tags associated with this Artifact
     print(f"Tags: {my_data.sageworks_tags()}")
 
-    # Get ALL Metadata associated with this Artifact
+    # Get ALL the AWS Metadata associated with this Artifact
     print("\n\nALL Meta")
-    pprint(my_data.all_meta())
+    pprint(my_data.aws_meta())
 
     # Get a SAMPLE of the data
     print(f"Sample Data: {my_data.sample_df()}")
+
+    # Force a refresh of the DataSource
+    my_data = DataSource("abalone_data", force_refresh=True)
```

### Comparing `sageworks-0.1.5.2/src/sageworks/artifacts/data_sources/data_source_abstract.py` & `sageworks-0.1.5.3/src/sageworks/artifacts/data_sources/data_source_abstract.py`

 * *Files 24% similar despite different names*

```diff
@@ -60,14 +60,29 @@
         Returns:
             dict(dict): A dictionary of quartiles for each column in the form
                  {'col1': {'min': 0, 'q1': 1, 'median': 2, 'q3': 3, 'max': 4},
                   'col2': ...}
         """
         pass
 
+    @abstractmethod
+    def outliers(self, scale: float = 1.7, recompute: bool = False) -> pd.DataFrame:
+        """Return a DataFrame of outliers from this DataSource
+        Args:
+            scale(float): The scale to use for the IQR (default: 1.7)
+            recompute(bool): Recompute the outliers (default: False)
+        Returns:
+            pd.DataFrame: A DataFrame of outliers from this DataSource
+        Notes:
+            Uses the IQR * 1.7 (~= 3 Sigma) method to compute outliers
+            The scale parameter can be adjusted to change the IQR multiplier
+        """
+        pass
+
+    @abstractmethod
     def value_counts(self, recompute: bool = False) -> dict[dict]:
         """Compute 'value_counts' for all the string columns in a DataSource
         Args:
             recompute(bool): Recompute the value counts (default: False)
         Returns:
             dict(dict): A dictionary of value counts for each column in the form
                  {'col1': {'value_1': X, 'value_2': Y, 'value_3': Z,...},
```

### Comparing `sageworks-0.1.5.2/src/sageworks/artifacts/endpoints/endpoint.py` & `sageworks-0.1.5.3/src/sageworks/artifacts/endpoints/endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,16 +156,16 @@
             error_df[column] = df[column].values
         return error_df
 
     def size(self) -> float:
         """Return the size of this data in MegaBytes"""
         return 0.0
 
-    def all_meta(self) -> dict:
-        """Get ALL the metadata for this artifact"""
+    def aws_meta(self) -> dict:
+        """Get ALL the AWS metadata for this artifact"""
         return self.endpoint_meta
 
     def arn(self) -> str:
         """AWS ARN (Amazon Resource Name) for this artifact"""
         return self.endpoint_meta["EndpointArn"]
 
     def aws_url(self):
@@ -210,18 +210,20 @@
             self.sm_client.delete_endpoint_config(EndpointConfigName=self.endpoint_name)
         except botocore.exceptions.ClientError:
             self.log.info(f"Endpoint Config {self.endpoint_name} doesn't exist...")
 
 
 if __name__ == "__main__":
     """Exercise the Endpoint Class"""
-    from sageworks.transforms.pandas_transforms.features_to_pandas import FeaturesToPandas
+    from sageworks.transforms.pandas_transforms.features_to_pandas import (
+        FeaturesToPandas,
+    )
 
     # Grab an Endpoint object and pull some information from it
-    my_endpoint = Endpoint("abalone-regression-endpoint")
+    my_endpoint = Endpoint("abalone-regression-end")
 
     # Call the various methods
 
     # Let's do a check/validation of the Endpoint
     assert my_endpoint.check()
 
     # Creation/Modification Times
```

### Comparing `sageworks-0.1.5.2/src/sageworks/artifacts/models/model.py` & `sageworks-0.1.5.3/src/sageworks/artifacts/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
             return False
         return True
 
     def size(self) -> float:
         """Return the size of this data in MegaBytes"""
         return 0.0
 
-    def all_meta(self) -> dict:
-        """Get ALL the metadata for this artifact"""
+    def aws_meta(self) -> dict:
+        """Get ALL the AWS metadata for this artifact"""
         return self.latest_model
 
     def arn(self) -> str:
         """AWS ARN (Amazon Resource Name) for the Model Package Group"""
         return self.group_arn()
 
     def group_arn(self) -> str:
```

### Comparing `sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_account_clamp.py` & `sageworks-0.1.5.3/src/sageworks/aws_service_broker/aws_account_clamp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 """AWSAccountClamp provides logic/functionality over a set of AWS IAM Services"""
 import sys
 import boto3
-from botocore.exceptions import ClientError, UnauthorizedSSOTokenError, TokenRetrievalError
+from botocore.exceptions import (
+    ClientError,
+    UnauthorizedSSOTokenError,
+    TokenRetrievalError,
+)
 from botocore.credentials import RefreshableCredentials
 from botocore.session import get_session
 from sagemaker.session import Session as SageSession
 from datetime import timedelta
 import logging
 
 # SageWorks Imports
@@ -22,27 +26,39 @@
         self.log = logging.getLogger(__file__)
 
         # Grab the AWS Role Name from the SageWorks Config
         config = SageWorksConfig()
         role_name = config.get_config_value("SAGEWORKS_AWS", "SAGEWORKS_ROLE_NAME")
         self.role_name = role_name
 
+        # Quick check on SSO Token
+        try:
+            boto3.client("sts").get_caller_identity()
+        except (ClientError, UnauthorizedSSOTokenError, TokenRetrievalError):
+            self.log.critical("AWS Identity Check Failure: Check AWS_PROFILE and/or Renew SSO Token...")
+            sys.exit(1)
+
+        # Let's fill in some of the AWS Session details
+        self.sageworks_bucket_name = config.get_config_value("SAGEWORKS_AWS", "S3_BUCKET_NAME")
+        self.account_id = boto3.client("sts").get_caller_identity()["Account"]
+        self.region = boto3.session.Session().region_name
+
         # The default AWS Assume Role TTL is 1 hour, so we'll set our TTL to 50 minutes
         self.session_time_delta = timedelta(minutes=50)
 
     def check_aws_identity(self) -> bool:
         """Check the AWS Identity currently active"""
         # Check AWS Identity Token
         sts = boto3.client("sts")
         try:
             identity = sts.get_caller_identity()
             self.log.info("AWS Account Info:")
             self.log.info(f"Account: {identity['Account']}")
             self.log.info(f"ARN: {identity['Arn']}")
-            self.log.info(f"Region: {self.region()}")
+            self.log.info(f"Region: {self.region}")
             return True
         except (ClientError, UnauthorizedSSOTokenError) as exc:
             self.log.critical("AWS Identity Check Failure: Check AWS_PROFILE and/or Renew SSO Token...")
             self.log.critical(exc)
             sys.exit(1)  # FIXME: Longer term we probably want to raise exc and have caller catch it
 
     def check_app_config(self, boto_session: boto3.Session) -> bool:
@@ -138,23 +154,14 @@
         return SageSession(boto_session=session)
 
     def sagemaker_client(self, session: boto3.Session = None):
         """Create a sageworks SageMaker client (using our boto3 refreshable session)"""
         session = session or self.boto_session()
         return session.client("sagemaker")
 
-    @staticmethod
-    def account_id():
-        """Get the AWS AccountID"""
-        return boto3.client("sts").get_caller_identity()["Account"]
-
-    def region(self):
-        """Get the AWS AccountID"""
-        return self.boto_session().region_name
-
 
 if __name__ == "__main__":
     """Exercise the AWS Account Clamp Class"""
 
     # Create the class
     aws_account_clamp = AWSAccountClamp()
```

### Comparing `sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_broker.py` & `sageworks-0.1.5.3/src/sageworks/aws_service_broker/aws_service_broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,30 +5,36 @@
 import logging
 from threading import Thread
 
 # SageWorks Imports
 from sageworks.utils.cache import Cache
 from sageworks.utils.redis_cache import RedisCache
 from sageworks.aws_service_broker.aws_service_connectors.s3_bucket import S3Bucket
+from sageworks.aws_service_broker.aws_service_connectors.glue_jobs import GlueJobs
 from sageworks.aws_service_broker.aws_service_connectors.data_catalog import DataCatalog
-from sageworks.aws_service_broker.aws_service_connectors.feature_store import FeatureStore
-from sageworks.aws_service_broker.aws_service_connectors.model_registry import ModelRegistry
+from sageworks.aws_service_broker.aws_service_connectors.feature_store import (
+    FeatureStore,
+)
+from sageworks.aws_service_broker.aws_service_connectors.model_registry import (
+    ModelRegistry,
+)
 from sageworks.aws_service_broker.aws_service_connectors.endpoints import Endpoints
 from sageworks.utils.sageworks_config import SageWorksConfig
 from sageworks.utils.sageworks_logging import logging_setup
 
 # Setup Logging
 logging_setup()
 
 
 # Enumerated types for SageWorks Meta Requests
 class ServiceCategory(Enum):
     """Enumerated Types for SageWorks Meta Requests"""
 
     INCOMING_DATA_S3 = auto()
+    GLUE_JOBS = auto()
     DATA_SOURCES_S3 = auto()
     FEATURE_SETS_S3 = auto()
     DATA_CATALOG = auto()
     FEATURE_STORE = auto()
     MODELS = auto()
     ENDPOINTS = auto()
 
@@ -70,14 +76,15 @@
         # - models = Model Registry
         # - endpoints = Sagemaker Endpoints, Model Monitors
 
         # Pull in AWS Service Connectors
         cls.incoming_data_s3 = S3Bucket(cls.incoming_data_bucket)
         cls.data_sources_s3 = S3Bucket(cls.data_sources_bucket)
         cls.feature_sets_s3 = S3Bucket(cls.feature_sets_bucket)
+        cls.glue_jobs = GlueJobs()
         cls.data_catalog = DataCatalog(database_scope)
         cls.feature_store = FeatureStore()
         cls.model_registry = ModelRegistry()
         cls.endpoints = Endpoints()
 
         # Cache for Metadata
         if RedisCache().check():
@@ -89,14 +96,15 @@
             cls.fresh_cache = Cache(expire=10)
             cls.open_threads = []
 
         # This connection map sets up the connector objects for each category of metadata
         # Note: Even though this seems confusing, it makes other code WAY simpler
         cls.connection_map = {
             ServiceCategory.INCOMING_DATA_S3: cls.incoming_data_s3,
+            ServiceCategory.GLUE_JOBS: cls.glue_jobs,
             ServiceCategory.DATA_SOURCES_S3: cls.data_sources_s3,
             ServiceCategory.FEATURE_SETS_S3: cls.feature_sets_s3,
             ServiceCategory.DATA_CATALOG: cls.data_catalog,
             ServiceCategory.FEATURE_STORE: cls.feature_store,
             ServiceCategory.MODELS: cls.model_registry,
             ServiceCategory.ENDPOINTS: cls.endpoints,
         }
@@ -106,65 +114,65 @@
         """Refresh the Metadata for the given Category
 
         Args:
             category (ServiceCategory): The Category of metadata to Pull
         """
         # Refresh the connection for the given category and pull new data
         cls.connection_map[category].refresh()
-        cls.meta_cache.set(category, cls.connection_map[category].metadata())
+        cls.meta_cache.set(category, cls.connection_map[category].aws_meta())
         cls.fresh_cache.set(category, True)
 
     @classmethod
-    def get_metadata(cls, category: ServiceCategory, force_fresh=False) -> dict:
+    def get_metadata(cls, category: ServiceCategory, force_refresh=False) -> dict:
         """Pull Metadata for the given Service Category
 
         Args:
             category (ServiceCategory): The Service Category to pull metadata from
-            force_fresh (bool, optional): Force a refresh of the metadata. Defaults to False.
+            force_refresh (bool, optional): Force a refresh of the metadata. Defaults to False.
 
         Returns:
             dict: The Metadata for the Requested Service Category
         """
         # Logic:
         # - NO metadata in the cache, we need to BLOCK and get it
         # - Metadata is in the cache but is stale, launch a thread to refresh, return stale data
         # - Metadata is in the cache and is fresh, so we just return it
 
         # Do we have this AWS data already in the cache?
         meta_data = cls.meta_cache.get(category)
 
         # If we don't have the AWS data in the cache, we need to BLOCK and get it
-        if meta_data is None or force_fresh:
+        if meta_data is None or force_refresh:
             cls.log.info(f"Blocking: Getting metadata for {category}...")
             cls.refresh_aws_data(category)
             return cls.meta_cache.get(category)
 
         # Is the AWS data stale?
         if cls.fresh_cache.get(category) is None:
             cls.log.info(f"Async: Metadata for {category} is stale, launching refresh thread...")
             cls.fresh_cache.set(category, True)
             thread = Thread(target=cls.refresh_aws_data, args=(category,))
             cls.open_threads.append(thread)
             thread.start()
             return cls.meta_cache.get(category)
 
         # If the metadata is fresh, just return it
-        cls.log.info(f"Metadata for {category} is fresh!")
+        cls.log.debug(f"Metadata for {category} is fresh!")
         return cls.meta_cache.get(category)
 
     @classmethod
-    def get_all_metadata(cls, force_fresh=False) -> dict:
+    def get_all_metadata(cls, force_refresh=False) -> dict:
         """Pull the metadata for ALL the Service Categories
         Args:
-            force_fresh (bool, optional): Force a refresh of the metadata. Defaults to False.
+            force_refresh (bool, optional): Force a refresh of the metadata. Defaults to False.
         Returns:
             dict: The Metadata for ALL the Service Categories
         """
         cls.log.warning("Getting ALL AWS Metadata: You should call get_metadata() with specific categories")
-        return {_category: cls.get_metadata(_category, force_fresh) for _category in ServiceCategory}
+        return {_category: cls.get_metadata(_category, force_refresh) for _category in ServiceCategory}
 
     @classmethod
     def wait_for_refreshes(cls) -> None:
         """Wait for any open threads to finish"""
         for thread in cls.open_threads:
             thread.join()
 
@@ -213,15 +221,15 @@
 
     # Get the Metadata for ALL the categories
     # NOTE: There should be NO Refreshes in the logs
     pprint(aws_broker.get_all_metadata())
 
     # Get the Metadata for ALL the categories
     # NOTE: This should force a refresh of the metadata
-    # pprint(aws_broker.get_all_metadata(force_fresh=True))
+    # pprint(aws_broker.get_all_metadata(force_refresh=True))
 
     # Get S3 object sizes
     incoming_data_size = aws_broker.get_s3_object_sizes(ServiceCategory.INCOMING_DATA_S3)
     print(f"Incoming Data Size: {incoming_data_size} Bytes")
 
     data_sources_size = aws_broker.get_s3_object_sizes(ServiceCategory.DATA_SOURCES_S3)
     print(f"Data Sources Size: {data_sources_size} Bytes")
```

### Comparing `sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/connector.py` & `sageworks-0.1.5.3/src/sageworks/aws_service_broker/aws_service_connectors/connector.py`

 * *Files 23% similar despite different names*

```diff
@@ -41,31 +41,25 @@
         """Refresh data/metadata associated with this service"""
         # We could do something here to refresh the AWS Session or whatever
 
         # Call the subclass Refresh method
         return self.refresh_impl()
 
     @abstractmethod
-    def metadata(self) -> dict:
-        """Return all the metadata for this AWS Service"""
+    def aws_meta(self) -> dict:
+        """Return ALL the AWS metadata for this AWS Service"""
         pass
 
     @staticmethod
     def _aws_tags_to_dict(aws_tags) -> dict:
         """Internal: AWS Tags are in an odd format, so convert to regular dictionary"""
-        return {item["Key"]: item["Value"] for item in aws_tags if "sageworks" in item["Key"]}
+        return {item["Key"]: item["Value"] for item in aws_tags}
 
-    def sageworks_meta(self, arn: str) -> dict:
-        """Get the SageWorks specific metadata for this Artifact/ARN
-        Note: This functionality will work for Feature Store, Models, and Endpoints
-              but not for Data Catalogs. The Data Catalog class has its own methods
+    def sageworks_meta_via_arn(self, arn: str) -> dict:
+        """Helper: Get the SageWorks specific metadata for this ARN
+        Note: This functionality is a helper or Feature Store, Models, and Endpoints.
+              The Data Catalog and Glue Jobs class have their own methods/logic
         """
         self.log.info(f"Retrieving SageWorks Metadata for Artifact: {arn}...")
         aws_tags = self.sm_session.list_tags(arn)
         meta = self._aws_tags_to_dict(aws_tags)
         return meta
-
-    def sageworks_tags(self, arn: str) -> list:
-        """Get the SageWorks tags for this Artifact/ARN"""
-        combined_tags = self.sageworks_meta(arn).get("sageworks_tags", "")
-        tags = combined_tags.split(":")
-        return tags
```

### Comparing `sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py` & `sageworks-0.1.5.3/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,18 +32,18 @@
         _end_names = [_endpoint["EndpointName"] for _endpoint in _endpoints]
 
         # Get the details for Endpoints and convert to a data structure with direct lookup
         self.endpoint_data = {name: self._retrieve_details(name) for name in _end_names}
 
         # Additional details under the sageworks_meta section for each Model Group
         for _end_name, end_info in self.endpoint_data.items():
-            sageworks_meta = self.sageworks_meta(end_info["EndpointArn"])
+            sageworks_meta = self.sageworks_meta_via_arn(end_info["EndpointArn"])
             end_info["sageworks_meta"] = sageworks_meta
 
-    def metadata(self) -> dict:
+    def aws_meta(self) -> dict:
         """Get the full AWS metadata about endpoints"""
         return self.endpoint_data
 
     def endpoint_names(self) -> list:
         """Get all the endpoint names in AWS"""
         return list(self.endpoint_data.keys())
 
@@ -79,16 +79,7 @@
     print("Endpoints:")
     for end_name in my_endpoints.endpoint_names():
         print(f"\t{end_name}")
 
     # Get the details for a specific Endpoint
     endpoint_info = my_endpoints.endpoint_details(end_name)
     pprint(endpoint_info)
-
-    # Get the tags for this Endpoint
-    my_arn = endpoint_info["EndpointArn"]
-    my_tags = my_endpoints.sageworks_tags(my_arn)
-    print(f"Tags: {my_tags}")
-
-    # Get the SageWorks Metadata for this Endpoint
-    my_sageworks_meta = my_endpoints.sageworks_meta(my_arn)
-    print(f"SageWorks Metadata: {my_sageworks_meta}")
```

### Comparing `sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py` & `sageworks-0.1.5.3/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,39 +33,39 @@
 
         # Get the details for each Feature Group and convert to a data structure with direct lookup
         self.feature_data = {name: self._feature_group_details(name) for name in _fg_names}
 
         # Additional details under the sageworks_meta section for each Feature Group
         for fg_name in _fg_names:
             arn = self.feature_data[fg_name]["FeatureGroupArn"]
-            sageworks_meta = self.sageworks_meta(arn)
+            sageworks_meta = self.sageworks_meta_via_arn(arn)
             add_data = {
                 "athena_database": self.athena_database_name(fg_name),
                 "athena_table": self.athena_table_name(fg_name),
                 "s3_storage": self.s3_storage(fg_name),
             }
             sageworks_meta.update(add_data)
             self.feature_data[fg_name]["sageworks_meta"] = sageworks_meta
 
-    def metadata(self) -> dict:
-        """Get all the table information in this database"""
+    def aws_meta(self) -> dict:
+        """Return ALL the AWS metadata for this AWS Feature Store"""
         return self.feature_data
 
     def feature_group_names(self) -> list:
-        """Get all the feature group names in this database"""
+        """Get all the feature group names"""
         return list(self.feature_data.keys())
 
     def feature_group_details(self, feature_group_name: str) -> dict:
         """Get the details for a specific feature group"""
         return self.feature_data.get(feature_group_name)
 
     def athena_database_name(self, feature_group_name: str) -> str:
         """Get the Athena Database Name for a specific feature group"""
         try:
-            return self.feature_data[feature_group_name]["OfflineStoreConfig"]["DataCatalogConfig"]["Database"]
+            return self.feature_data[feature_group_name]["OfflineStoreConfig"]["DataCatalogConfig"]["Database"].lower()
         except KeyError:
             return "-"
 
     def athena_table_name(self, feature_group_name: str) -> str:
         """Get the Athena Table Name for a specific feature group"""
         try:
             return self.feature_data[feature_group_name]["OfflineStoreConfig"]["DataCatalogConfig"]["TableName"]
@@ -133,16 +133,7 @@
     my_database = feature_store.athena_database_name(my_group)
 
     # Get the Athena Table Name for this Feature Group
     my_table = feature_store.athena_table_name(my_group)
 
     # Get the Athena Query for this Feature Group
     my_query = feature_store.snapshot_query(my_group)
-
-    # Get the tags for this Feature Group
-    my_arn = group_info["FeatureGroupArn"]
-    my_tags = feature_store.sageworks_tags(my_arn)
-    print(f"Tags: {my_tags}")
-
-    # Get the SageWorks Metadata for this Feature Group
-    my_sageworks_meta = feature_store.sageworks_meta(my_arn)
-    print(f"SageWorks Metadata: {my_sageworks_meta}")
```

### Comparing `sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py` & `sageworks-0.1.5.3/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,35 +36,31 @@
         self.model_package_group_arn = _model_groups[0]["ModelPackageGroupArn"] if _model_groups else None
 
         # Get the details for each Model Group and convert to a data structure with direct lookup
         self.model_data = {name: self._model_group_details(name) for name in _mg_names}
 
         # Additional details under the sageworks_meta section for each Model Group
         for mg_name in _mg_names:
-            sageworks_meta = self.sageworks_meta(self.model_package_group_arn)
+            sageworks_meta = self.sageworks_meta_via_arn(self.model_package_group_arn)
             # Model groups have a list of models
             for model_info in self.model_data[mg_name]:
                 model_info["sageworks_meta"] = sageworks_meta
 
-    def metadata(self) -> dict:
-        """Get all the table information in this database"""
+    def aws_meta(self) -> dict:
+        """Return ALL the AWS metadata for the AWS Model Registry"""
         return self.model_data
 
     def model_group_names(self) -> list:
         """Get all the feature group names in this database"""
         return list(self.model_data.keys())
 
     def model_group_details(self, model_group_name: str) -> dict:
         """Get the details for a specific feature group"""
         return self.model_data.get(model_group_name)
 
-    def s3_storage(self, model_group_name: str) -> str:
-        """Get the S3 Location for a specific feature group"""
-        return "TBD Later"
-
     def _model_group_details(self, model_group_name: str) -> dict:
         """Internal: Do not call this method directly, use model_group_details() instead"""
 
         # Grab the Model Group details from the AWS Model Registry
         details = self.sm_client.list_model_packages(ModelPackageGroupName=model_group_name)["ModelPackageSummaryList"]
         for detail in details:
             model_arn = detail["ModelPackageArn"]
@@ -94,16 +90,7 @@
     for my_group_name in model_registry.model_group_names():
         print(f"\t{my_group_name}")
 
     # Get the details for a specific Model Group
     my_group = "abalone-regression"
     group_info = model_registry.model_group_details(my_group)
     pprint(group_info)
-
-    # Get the tags for this Model Group
-    my_arn = model_registry.model_package_group_arn
-    my_tags = model_registry.sageworks_tags(my_arn)
-    print(f"Tags: {my_tags}")
-
-    # Get the SageWorks Metadata for this Model Group
-    my_sageworks_meta = model_registry.sageworks_meta(my_arn)
-    print(f"SageWorks Metadata: {my_sageworks_meta}")
```

### Comparing `sageworks-0.1.5.2/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py` & `sageworks-0.1.5.3/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """S3Bucket: Class to retrieve object/file information from an AWS S3 Bucket"""
 import awswrangler as wr
+from botocore.exceptions import ClientError
 
 
 # SageWorks Imports
 from sageworks.aws_service_broker.aws_service_connectors.connector import Connector
 
 
 # Class to retrieve object/file information from an AWS S3 Bucket
@@ -27,19 +28,28 @@
             self.log.critical(f"Could not connect to AWS S3 {self.bucket}: {e}")
             return False
 
     def refresh_impl(self):
         """Load/reload the files in the bucket"""
         # Grab all the files in this bucket
         self.log.info(f"Reading S3 Bucket: {self.bucket}...")
-        _aws_file_info = wr.s3.describe_objects(self.bucket, boto3_session=self.boto_session)
+        try:
+            _aws_file_info = wr.s3.describe_objects(self.bucket, boto3_session=self.boto_session)
+        except ClientError as error:
+            # If the exception is a ResourceNotFound, this is fine, otherwise raise all other exceptions
+            if error.response["Error"]["Code"] in ["ResourceNotFound", "NoSuchBucket"]:
+                self.log.warning(f"Describing objects in {self.bucket} gave ResourceNotFound")
+                return {}
+            else:
+                self.log.warning(f"Describing objects in {self.bucket} gave {error.response['Error']['Code']}")
+                return {}
         self.s3_bucket_data = {full_path: info for full_path, info in _aws_file_info.items()}
 
-    def metadata(self) -> dict:
-        """Get all the metadata for the files in this bucket"""
+    def aws_meta(self) -> dict:
+        """Return ALL the AWS metadata for the AWS S3 Service"""
         return self.s3_bucket_data
 
     def file_names(self) -> list:
         """Get all the file names in this bucket"""
         return list(self.s3_bucket_data.keys())
 
     def bucket_size(self) -> list:
@@ -74,9 +84,15 @@
     for file_name in s3_bucket.file_names():
         print(f"\t{file_name}")
 
     # Get the size of all the objects in this bucket
     print(f"Bucket Size: {s3_bucket.bucket_size()}")
 
     # Get additional info for a specific file
-    my_file_info = s3_bucket.file_info("abalone.csv")
+    my_file_info = s3_bucket.file_info(file_name)
     pprint(my_file_info)
+
+    # Test the functionality for a bucket that doesn't exist
+    not_exist_bucket = "s3://non_existent_bucket"
+    s3_bucket = S3Bucket(not_exist_bucket)
+    s3_bucket.check()
+    s3_bucket.refresh()
```

### Comparing `sageworks-0.1.5.2/src/sageworks/transforms/Readme.md` & `sageworks-0.1.5.3/src/sageworks/transforms/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py` & `sageworks-0.1.5.3/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 # Import all the AWS Glue Python Libraries
 from awsglue.utils import getResolvedOptions
 from awsglue.context import GlueContext
 from awsglue.job import Job
 from pyspark.context import SparkContext
 from awsglue.dynamicframe import DynamicFrame
-from awsglue.transforms import ApplyMapping
+from awsglue.transforms import Relationalize
+from pyspark.sql.functions import col, to_timestamp
 
 
 class S3HeavyToDataSource:
     def __init__(self, glue_context: GlueContext, input_uuid: str, output_uuid: str):
         """S3HeavyToDataSource: Class to move HEAVY S3 Files into a SageWorks DataSource
         Args:
             glue_context: GlueContext, AWS Glue Specific wrapper around SparkContext
@@ -22,47 +23,66 @@
         """
         self.log = glue_context.get_logger()
 
         # FIXME: Pull these from Parameter Store or Config
         self.input_uuid = input_uuid
         self.output_uuid = output_uuid
         self.output_meta = {"sageworks_input": self.input_uuid}
-        sageworks_bucket = "s3://scp-sageworks-artifacts"
+        sageworks_bucket = "s3://sandbox-sageworks-artifacts"
         self.data_source_s3_path = sageworks_bucket + "/data-sources"
 
         # Our Spark Context
         self.glue_context = glue_context
 
-    @staticmethod
-    def column_type_conversion(input_dyf: DynamicFrame) -> DynamicFrame:
-        """Convert the column types from the input data (Spark) to the output data (Athena/Parquet)"""
-        # Define the mapping from Spark data types to Athena data types
-        type_mapping = {"struct": "string", "choice": "long"}
-
-        # Get the column names and types from the input data
-        column_names_types = [(col.name, col.dataType.typeName()) for col in input_dyf.schema().fields]
-        input_dyf.printSchema()
-
-        # Define the mapping from input column names/types (Spark) to output
-        # column names and types that are compatible with Athena/Parquet.
-        mapping = []
-        for name, col_type in column_names_types:
-            output_type = type_mapping.get(col_type, col_type)
-            if col_type == "timestamp":
-                # Apply to_timestamp transformation for timestamp columns
-                output_type = f"to_timestamp({name})"
-            mapping.append((name, col_type, name, output_type))
-        print(mapping)
+    def column_conversions(self, dyf: DynamicFrame, time_columns: list = []) -> DynamicFrame:
+        """Convert columns in the DynamicFrame to the correct data types
+        Args:
+            dyf (DynamicFrame): The DynamicFrame to convert
+            time_columns (list): A list of column names to convert to timestamp
+        Returns:
+            DynamicFrame: The converted DynamicFrame
+        """
 
-        # Apply the mapping and convert data types
-        output_dyf = ApplyMapping.apply(frame=input_dyf, mappings=mapping, transformation_ctx="applymapping")
-        output_dyf.printSchema()
+        # Convert the timestamp columns to timestamp types
+        spark_df = dyf.toDF()
+        for column in time_columns:
+            spark_df = spark_df.withColumn(column, to_timestamp(col(column)))
+
+        # Convert the Spark DataFrame back to a Glue DynamicFrame
+        output_dyf = DynamicFrame.fromDF(spark_df, self.glue_context, "output_dyf")
+
+        # Now resolve any 'choice' columns
+        specs = [(field.name, "cast:long") for field in dyf.schema().fields if field.dataType.typeName() == "choice"]
+        print(specs)
+        if specs:
+            output_dyf = output_dyf.resolveChoice(specs=specs)
         return output_dyf
 
-    def transform(self, input_type: str = "json", overwrite: bool = True):
+    @staticmethod
+    def remove_periods_from_column_names(dyf: DynamicFrame) -> DynamicFrame:
+        """Remove periods from column names in the DynamicFrame
+        Args:
+            dyf (DynamicFrame): The DynamicFrame to convert
+        Returns:
+            DynamicFrame: The converted DynamicFrame
+        """
+        # Extract the column names from the schema
+        old_column_names = [field.name for field in dyf.schema().fields]
+
+        # Create a new list of renamed column names
+        new_column_names = [name.replace(".", "_") for name in old_column_names]
+        print(old_column_names)
+        print(new_column_names)
+
+        # Create a new DynamicFrame with renamed columns
+        for c_old, c_new in zip(old_column_names, new_column_names):
+            dyf = dyf.rename_field(f"`{c_old}`", c_new)
+        return dyf
+
+    def transform(self, input_type: str = "json", timestamp_columns: list = None):
         """Convert the CSV or JSON data into Parquet Format in the SageWorks S3 Bucket, and
         store the information about the data to the AWS Data Catalog sageworks database"""
 
         # Add some tags here
         tags = ["heavy"]
 
         # Create the Output Parquet file S3 Storage Path
@@ -79,74 +99,87 @@
             },
             format=input_type,
             # format_options={'jsonPath': 'auto'}, Look into this later
         )
         self.log.info("Incoming DataFrame...")
         input_dyf.show(5)
 
+        # Create a Dynamic Frame Collection (dfc)
+        dfc = Relationalize.apply(input_dyf, name="root")
+
+        # Aggregate the collection into a single dynamic frame
+        all_data = dfc.select("root")
+
+        print("Before Column Conversions")
+        all_data.printSchema()
+
+        # Relationalize will put periods in the column names. This will cause
+        # problems later when we try to create a FeatureSet from this DataSource
+        output_dyf = self.remove_periods_from_column_names(all_data)
+
         # Convert the columns types from Spark types to Athena/Parquet types
-        output_dyf = self.column_type_conversion(input_dyf)
+        output_dyf = self.column_conversions(output_dyf, timestamp_columns)
+
+        print("After Column Conversions")
+        output_dyf.printSchema()
 
         # Write Parquet files to S3
         self.log.info(f"Writing Parquet files to {s3_storage_path}...")
         self.glue_context.purge_s3_path(s3_storage_path, {"retentionPeriod": 0})
         self.glue_context.write_dynamic_frame.from_options(
             frame=output_dyf,
             connection_type="s3",
             connection_options={
                 "path": s3_storage_path
                 # "partitionKeys": ["year", "month", "day"],
             },
-            format="parquet",
+            format="orc",
         )
 
         # Set up our SageWorks metadata (description, tags, etc)
         description = f"SageWorks data source: {self.output_uuid}"
         sageworks_meta = {"sageworks_tags": ":".join(tags)}
         for key, value in self.output_meta.items():
             sageworks_meta[key] = value
 
         # Create a new table in the AWS Data Catalog
         self.log.info(f"Creating Data Catalog Table: {self.output_uuid}...")
 
         # Converting the Spark Types to Athena Types
         def to_athena_type(col):
-            athena_type_map = {"long": "bigint", "struct": "string"}
+            athena_type_map = {"long": "bigint"}
             spark_type = col.dataType.typeName()
             return athena_type_map.get(spark_type, spark_type)
 
         column_name_types = [{"Name": col.name, "Type": to_athena_type(col)} for col in output_dyf.schema().fields]
         table_input = {
             "Name": self.output_uuid,
             "Description": description,
             "Parameters": sageworks_meta,
             "TableType": "EXTERNAL_TABLE",
             "StorageDescriptor": {
                 "Columns": column_name_types,
                 "Location": s3_storage_path,
                 "InputFormat": "org.apache.hadoop.mapred.TextInputFormat",
-                "OutputFormat": "org.apache.hadoop.hive.ql.io.HiveIgnoreKeyTextOutputFormat",
                 "Compressed": True,
-                "NumberOfBuckets": -1,
                 "SerdeInfo": {
-                    "SerializationLibrary": "org.apache.hadoop.hive.ql.io.parquet.serde.ParquetHiveSerDe",
-                    "Parameters": {"serialization.format": "1"},
+                    # "SerializationLibrary": "org.apache.hadoop.hive.ql.io.parquet.serde.ParquetHiveSerDe",
+                    "SerializationLibrary": "org.apache.hadoop.hive.ql.io.orc.OrcSerde",
                 },
             },
         }
 
         # Delete the Data Catalog Table if it already exists
-        if overwrite:
-            glue_client = boto3.client("glue")
-            try:
-                glue_client.delete_table(DatabaseName="sageworks", Name=self.output_uuid)
-                self.log.info(f"Deleting Data Catalog Table: {self.output_uuid}...")
-            except ClientError as e:
-                if e.response["Error"]["Code"] != "EntityNotFoundException":
-                    raise e
+        glue_client = boto3.client("glue")
+        try:
+            glue_client.delete_table(DatabaseName="sageworks", Name=self.output_uuid)
+            self.log.info(f"Deleting Data Catalog Table: {self.output_uuid}...")
+        except ClientError as e:
+            if e.response["Error"]["Code"] != "EntityNotFoundException":
+                raise e
 
         self.log.info(f"Creating Data Catalog Table: {self.output_uuid}...")
         glue_client.create_table(DatabaseName="sageworks", TableInput=table_input)
 
         # All done!
         self.log.info(f"{self.input_uuid} --> {self.output_uuid} complete!")
 
@@ -161,16 +194,16 @@
     # These are all AWS Glue Job specific
     sc = SparkContext()
     glueContext = GlueContext(sc)
     job = Job(glueContext)
     job.init(args["JOB_NAME"], args)
 
     # Test the Heavy Data Loader
-    input_path = "s3://scp-sageworks-artifacts/incoming-data/dns/"
+    input_path = "s3://sandbox-sageworks-artifacts/incoming-data/dns/"
     data_output_uuid = "heavy_dns"
     my_loader = S3HeavyToDataSource(glueContext, input_path, data_output_uuid)
 
     # Store this data as a SageWorks DataSource
-    my_loader.transform()
+    my_loader.transform(timestamp_columns=["timestamp"])
 
     # Commit the Glue Job
     job.commit()
```

### Comparing `sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py` & `sageworks-0.1.5.3/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/light/json_to_data_source.py` & `sageworks-0.1.5.3/src/sageworks/transforms/data_loaders/light/json_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py` & `sageworks-0.1.5.3/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/light/clean_data.py` & `sageworks-0.1.5.3/src/sageworks/transforms/data_to_data/light/clean_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/transforms/data_to_data/light/data_to_data_light.py` & `sageworks-0.1.5.3/src/sageworks/transforms/data_to_data/light/data_to_data_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/heavy/data_to_features_heavy.py` & `sageworks-0.1.5.3/src/sageworks/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """DataToFeaturesHeavy: Class to Transform a DataSource into a FeatureSet (Athena/FeatureStore)"""
-import pandas as pd
 import time
 import botocore
+import pandas as pd
 from sagemaker.feature_store.feature_group import FeatureGroup
 import awswrangler as wr
 from sagemaker.feature_store.inputs import DataCatalogConfig
 
 # Local imports
 from sageworks.transforms.transform import Transform
 from sageworks.artifacts.data_sources.data_source import DataSource
@@ -13,57 +13,55 @@
 
 
 class DataToFeaturesHeavy(Transform):
     """DataToFeaturesHeavy: Class to Transform a DataSource into a FeatureSet (Athena/FeatureStore)
 
     Common Usage:
         to_features = DataToFeaturesHeavy(output_uuid)
-        to_features.set_output_tags(["abalone", "heavy", "whatever"])
-        to_features.set_input(df, id_column="id"/None, event_time_column="date"/None)
-        to_features.transform()
+        to_features.set_output_tags(["heavy", "whatever"])
+        to_features.transform(query, id_column, event_time_column=None)
     """
 
     def __init__(self, input_uuid: str, output_uuid: str):
         """DataToFeaturesHeavy Initialization"""
 
         # Call superclass init
         super().__init__(input_uuid, output_uuid)
 
         # Set up all my instance attributes
         self.id_column = None
         self.event_time_column = None
         self.input_data_source = DataSource(input_uuid)
-        self.input_sample_df = self.input_data_source.sample_df()
         self.output_database = "sagemaker_featurestore"
 
     @staticmethod
-    def convert_nullable_types(df: pd.DataFrame) -> pd.DataFrame:
-        """Convert the new Pandas 'nullable types' since AWS SageMaker code doesn't currently support them
-        See: https://github.com/aws/sagemaker-python-sdk/pull/3740"""
-        for column in list(df.select_dtypes(include=[pd.Int32Dtype]).columns):
-            df[column] = df[column].astype("int32")
+    def convert_column_types(df: pd.DataFrame) -> pd.DataFrame:
+        """Convert the types of the DataFrame to the correct types for the Feature Store"""
+        datetime_type = ["datetime", "datetime64", "datetime64[ns]", "datetimetz"]
+        for column in df.select_dtypes(include=datetime_type).columns:
+            df[column] = df[column].astype("string")
         for column in list(df.select_dtypes(include=[pd.Int64Dtype]).columns):
             df[column] = df[column].astype("int64")
         for column in list(df.select_dtypes(include=[pd.Float64Dtype]).columns):
             df[column] = df[column].astype("float64")
         return df
 
-    def transform_impl(self, query, id_column: str, event_time_column: str = None, delete_existing: bool = True):
+    def transform_impl(self, query, id_column: str, event_time_column: str = None):
         """Convert the Data Source into a Feature Set, also storing the information
         about the data to the AWS Data Catalog sageworks database and create S3 Objects"""
 
         # Do we want to delete the existing FeatureSet?
-        if delete_existing:
-            try:
-                delete_fs = FeatureSet(self.output_uuid)
-                if delete_fs.check():
-                    delete_fs.delete()
-            except botocore.exceptions.ClientError as exc:
-                self.log.info(f"FeatureSet {self.output_uuid} doesn't exist...")
-                self.log.info(exc)
+        try:
+            delete_fs = FeatureSet(self.output_uuid)
+            if delete_fs.check():
+                delete_fs.delete()
+                time.sleep(5)
+        except botocore.exceptions.ClientError as exc:
+            self.log.info(f"FeatureSet {self.output_uuid} doesn't exist...")
+            self.log.info(exc)
 
         # Set the ID and Event Time Columns
         self.id_column = id_column
         self.event_time_column = event_time_column
 
         # Create the Output Parquet file S3 Storage Path for this Feature Set
         s3_storage_path = f"{self.feature_sets_s3_path}"
@@ -78,28 +76,37 @@
             s3_output=s3_storage_path,
             write_compression="snappy",
             boto3_session=self.boto_session,
             wait=True,
         )
         self.log.info(f"FeatureSet Data Created: {info}")
 
-        # Convert Int32, Int64 and Float64 types (see: https://github.com/aws/sagemaker-python-sdk/pull/3740)
-        self.input_sample_df = self.convert_nullable_types(self.input_sample_df)
+        # Now we're going to use the Athena Query to create a sample DataFrame
+        sample_df = self.input_data_source.query(query + " LIMIT 1000")
+
+        # We need to convert some of our column types to the correct types
+        # Feature Store only supports these data types:
+        # - Integral
+        # - Fractional
+        # - String (timestamp/datetime types need to be converted to string)
+        sample_df = self.convert_column_types(sample_df)
 
         # Create a Feature Group and load our Feature Definitions
         self.log.info(f"Creating FeatureGroup: {self.output_uuid}")
         my_feature_group = FeatureGroup(name=self.output_uuid, sagemaker_session=self.sm_session)
-        my_feature_group.load_feature_definitions(data_frame=self.input_sample_df)
+        my_feature_group.load_feature_definitions(data_frame=sample_df)
 
         # Get the metadata/tags to push into AWS
         aws_tags = self.get_aws_tags()
 
         # Data Catalog Config
         my_config = DataCatalogConfig(
-            table_name=self.output_uuid, catalog="AwsDataCatalog", database=self.output_database
+            table_name=self.output_uuid,
+            catalog="AwsDataCatalog",
+            database=self.output_database,
         )
 
         # Write out the DataFrame to Parquet/FeatureSet/Athena
         my_feature_group.create(
             s3_uri=s3_storage_path,
             record_identifier_name=self.id_column,
             event_time_feature_name=self.event_time_column,
@@ -109,25 +116,49 @@
             data_catalog_config=my_config,
             disable_glue_table_creation=True,
         )
 
         # Ensure/wait for the feature group to be created
         self.ensure_feature_group_created(my_feature_group)
 
+        # Create the FeatureSet Object
+        self.log.info(f"Creating FeatureSet Object: {self.output_uuid}")
+        my_feature_set = FeatureSet(self.output_uuid, force_refresh=True)
+
+        # Compute Details, Quartiles, and SampleDF from the Feature Group
+        my_feature_set.details()
+        my_feature_set.data_source.details()
+        my_feature_set.quartiles()
+        my_feature_set.sample_df()
+        my_feature_set.set_status("ready")
+        self.log.info("FeatureSet Object Created")
+
     def ensure_feature_group_created(self, feature_group):
         status = feature_group.describe().get("FeatureGroupStatus")
         while status == "Creating":
             self.log.info("FeatureSet being Created...")
             time.sleep(5)
             status = feature_group.describe().get("FeatureGroupStatus")
         self.log.info(f"FeatureSet {feature_group.name} successfully created")
+        time.sleep(5)
 
 
 if __name__ == "__main__":
     """Exercise the DataToFeaturesHeavy Class"""
 
     # Create my DF to Feature Set Transform
-    data_to_features_heavy = DataToFeaturesHeavy("heavy_data_test", "heavy_data_test_features")
+    data_to_features_heavy = DataToFeaturesHeavy("heavy_dns", "dns_features_1")
     data_to_features_heavy.set_output_tags(["test", "heavy"])
 
     # Store this dataframe as a SageWorks Feature Set
-    data_to_features_heavy.transform(query="SELECT * FROM heavy_data_test", id_column="id", event_time_column="date")
+    fields = [
+        "timestamp",
+        "flow_id",
+        "in_iface",
+        "proto",
+        "dns_type",
+        "dns_rrtype",
+        "dns_flags",
+        "dns_rcode",
+    ]
+    query = f"SELECT {', '.join(fields)} FROM heavy_dns"
+    data_to_features_heavy.transform(query=query, id_column="flow_id", event_time_column="timestamp")
```

### Comparing `sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/light/data_to_features_light.py` & `sageworks-0.1.5.3/src/sageworks/transforms/pandas_transforms/features_to_pandas.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,85 @@
-"""DataToFeaturesLight: Base Class for Light DataSource to FeatureSet using Pandas"""
+"""FeaturesToPandas: Class to transform a FeatureSet into a Pandas DataFrame"""
+import pandas as pd
 
 # Local imports
 from sageworks.transforms.transform import Transform, TransformInput, TransformOutput
-from sageworks.transforms.pandas_transforms.data_to_pandas import DataToPandas
-from sageworks.transforms.pandas_transforms.pandas_to_features import PandasToFeatures
+from sageworks.artifacts.feature_sets.feature_set import FeatureSet
 
 
-class DataToFeaturesLight(Transform):
-    """DataToFeaturesLight: Base Class for Light DataSource to FeatureSet using Pandas
+class FeaturesToPandas(Transform):
+    """FeaturesToPandas: Class to transform a FeatureSet into a Pandas DataFrame
 
     Common Usage:
-        to_features = DataToFeaturesLight(data_uuid, feature_uuid)
-        to_features.set_output_tags(["abalone", "public", "whatever"])
-        to_features.transform(id_column="id"/None, event_time_column="date"/None)
+        feature_to_df = FeaturesToPandas(feature_set_uuid)
+        feature_to_df.transform(max_rows=<optional max rows to sample>)
+        my_df = feature_to_df.get_output()
     """
 
-    def __init__(self, data_uuid: str, feature_uuid: str):
-        """DataToFeaturesLight Initialization"""
+    def __init__(self, feature_set_name: str):
+        """FeaturesToPandas Initialization"""
 
         # Call superclass init
-        super().__init__(data_uuid, feature_uuid)
+        super().__init__(input_uuid=feature_set_name, output_uuid="DataFrame")
 
         # Set up all my instance attributes
-        self.input_type = TransformInput.DATA_SOURCE
-        self.output_type = TransformOutput.FEATURE_SET
-        self.input_df = None
+        self.input_type = TransformInput.FEATURE_SET
+        self.output_type = TransformOutput.PANDAS_DF
         self.output_df = None
+        self.transform_run = False
 
-    def pre_transform(self, **kwargs):
-        """Pull the input DataSource into our Input Pandas DataFrame"""
+    def transform_impl(self, max_rows=100000):
+        """Convert the FeatureSet into a Pandas DataFrame"""
 
-        # Grab the Input (Data Source)
-        self.input_df = DataToPandas(self.input_uuid).get_output()  # Shorthand for transform, get_output
-
-    def transform_impl(self, **kwargs):
-        """Base Class is simply an identity transform"""
-        self.output_df = self.input_df
-
-    def post_transform(self, id_column=None, event_time_column=None):
-        """At this point the output DataFrame should be populated, so publish it as a Feature Set"""
-        # Now publish to the output location
-        output_features = PandasToFeatures(self.output_uuid)
-        output_features.set_input(self.output_df, id_column=id_column, event_time_column=event_time_column)
-        output_features.set_output_tags(self.output_tags)
-        output_features.add_output_meta(self.output_meta)
-        output_features.transform()
+        # Grab the Input (Feature Set)
+        input_data = FeatureSet(self.input_uuid)
+        if not input_data.check():
+            self.log.critical(f"Feature Set Check on {self.input_uuid} failed!")
+            return
+
+        # Grab the table for this Feature Set
+        table = input_data.athena_table
+
+        # Get the list of columns (and subtract metadata columns that might get added)
+        columns = input_data.column_names()
+        filter_columns = ["write_time", "api_invocation_time", "is_deleted"]
+        columns = ", ".join([x for x in columns if x not in filter_columns])
+
+        # Get the number of rows in the Feature Set
+        num_rows = input_data.num_rows()
+
+        # If the data source has more rows than max_rows, do a sample query
+        if num_rows > max_rows:
+            percentage = round(max_rows * 100.0 / num_rows)
+            self.log.warning(f"DataSource has {num_rows} rows.. sampling down to {max_rows}...")
+            query = f'SELECT {columns} FROM "{table}" TABLESAMPLE BERNOULLI({percentage})'
+        else:
+            query = f'SELECT {columns} FROM "{table}"'
+
+        # Mark the transform as complete and set the output DataFrame
+        self.transform_run = True
+        self.output_df = input_data.query(query)
+
+    def get_output(self) -> pd.DataFrame:
+        """Get the DataFrame Output from this Transform"""
+        if not self.transform_run:
+            self.transform()
+        return self.output_df
 
 
 if __name__ == "__main__":
-    """Exercise the DataToFeaturesLight Class"""
+    """Exercise the FeaturesToPandas Class"""
 
-    # Create the class with inputs and outputs and invoke the transform
-    input_uuid = "abalone_data"
-    output_uuid = "abalone_feature_set"
-    data_to_features = DataToFeaturesLight(input_uuid, output_uuid)
-    data_to_features.set_output_tags(["abalone", "public"])
-    # data_to_features.transform(id_column="id", event_time_column="date")
-    data_to_features.transform(id_column="id")
+    # Setup Pandas output options
+    pd.set_option("display.max_colwidth", 15)
+    pd.set_option("display.max_columns", 15)
+    pd.set_option("display.width", 1000)
+
+    # Create the FeatureSet to DF Transform
+    feature_to_df = FeaturesToPandas("test-feature-set")
+
+    # Transform the DataSource into a Pandas DataFrame (with max_rows = 1000)
+    feature_to_df.transform(max_rows=1000)
+
+    # Grab the output and show it
+    my_df = feature_to_df.get_output()
+    print(my_df)
```

### Comparing `sageworks-0.1.5.2/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py` & `sageworks-0.1.5.3/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/transforms/features_to_model/features_to_model.py` & `sageworks-0.1.5.3/src/sageworks/transforms/features_to_model/features_to_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,23 +61,22 @@
         xgb_script = xgb_script.replace("{{model_type}}", model_type)
 
         # Now write out the generated model script and return the name
         with open(output_path, "w") as fp:
             fp.write(xgb_script)
         return script_name
 
-    def transform_impl(self, target, description, feature_list=None, model_type="regression", delete_existing=True):
+    def transform_impl(self, target, description, feature_list=None, model_type="regression"):
         """Generic Features to Model: Note you should create a new class and inherit from
         this one to include specific logic for your Feature Set/Model
         Args:
             target (str): Column name of the target variable
             description (str): Description of the model
             feature_list (list[str]): A list of columns for the features
             model_type (str): regression or classification
-            delete_existing (bool): Delete the existing model if it exists
         """
         # Set our model description
         self.model_description = description
 
         # Get our Feature Set and create an S3 CSV Training dataset
         feature_set = FeatureSet(self.input_uuid)
         s3_training_path = feature_set.create_s3_training_data()
@@ -126,22 +125,22 @@
 
         # Train the estimator
         self.estimator.fit({"train": s3_training_path})
 
         # Now delete the training data
         self.log.info(f"Deleting training data {s3_training_path}...")
         wr.s3.delete_objects(
-            [s3_training_path, s3_training_path.replace(".csv", ".csv.metadata")], boto3_session=self.boto_session
+            [s3_training_path, s3_training_path.replace(".csv", ".csv.metadata")],
+            boto3_session=self.boto_session,
         )
 
-        # Do they want to delete any existing models?
-        if delete_existing:
-            self.log.info("Trying to delete existing model...")
-            delete_model = Model(self.output_uuid)
-            delete_model.delete()
+        # Delete the existing model (if it exists)
+        self.log.info("Trying to delete existing model...")
+        delete_model = Model(self.output_uuid)
+        delete_model.delete()
 
         # Create Model and officially Register
         self.log.info(f"Creating new model {self.output_uuid}...")
         self.create_and_register_model()
 
         # Now add our SageWorks meta data
```

### Comparing `sageworks-0.1.5.2/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template` & `sageworks-0.1.5.3/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py` & `sageworks-0.1.5.3/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,26 +24,25 @@
         # Call superclass init
         super().__init__(model_uuid, endpoint_uuid)
 
         # Set up all my instance attributes
         self.input_type = TransformInput.MODEL
         self.output_type = TransformOutput.ENDPOINT
 
-    def transform_impl(self, delete_existing: bool = True):
+    def transform_impl(self):
         """Compute a Feature Set based on RDKit Descriptors"""
 
         # Get the Model Package ARN for our input model
         model_package_arn = Model(self.input_uuid).model_arn()
 
         # Create a Model Package
         model_package = ModelPackage(role=self.sageworks_role_arn, model_package_arn=model_package_arn)
 
-        # Check for delete
-        if delete_existing:
-            self.delete_endpoint()
+        # Delete endpoint (if it already exists)
+        self.delete_endpoint()
 
         # Get the metadata/tags to push into AWS
         aws_tags = self.get_aws_tags()
 
         # Deploy an Endpoint
         model_package.deploy(
             initial_instance_count=1,
```

### Comparing `sageworks-0.1.5.2/src/sageworks/transforms/pandas_transforms/data_to_pandas.py` & `sageworks-0.1.5.3/src/sageworks/transforms/pandas_transforms/data_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/transforms/pandas_transforms/pandas_to_data.py` & `sageworks-0.1.5.3/src/sageworks/transforms/pandas_transforms/pandas_to_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/transforms/pandas_transforms/pandas_utils.py` & `sageworks-0.1.5.3/src/sageworks/transforms/pandas_transforms/pandas_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -139,17 +139,75 @@
 
     output_df = input_df[numeric_df.apply(lambda x: np.abs(x - x.mean()) / x.std() < sigma).all(axis=1)]
     if input_df.shape[0] != output_df.shape[0]:
         log.info(f"Dropped {input_df.shape[0] - output_df.shape[0]} outlier rows")
     return output_df
 
 
+def displayable_df(input_df: pd.DataFrame) -> pd.DataFrame:
+    """Create a displayable dataframe from FeatureSet data
+    Args:
+        input_df (pd.DataFrame): Input DataFrame
+    Returns:
+        pd.DataFrame: DataFrame with displayable columns
+    """
+    exclude_columns = ["write_time", "api_invocation_time", "is_deleted", "training"]
+    df = input_df[input_df.columns.difference(exclude_columns)].copy()
+    dummy_cols = get_dummy_cols(df)
+
+    # Okay, so this is a bit of a hack, but we need to replace all but the last underscore
+    # run the from_dummies method, then change the column names back to the original
+    """
+    new_column_names = []
+    for col in dummy_cols:
+        count = col.count("_") - 1
+        new_column_names.append(col.replace("_", "-", count))
+    df.rename(columns=dict(zip(dummy_cols, new_column_names)), inplace=True)
+    un_dummy = pd.from_dummies(df[new_column_names], sep="_")
+    un_dummy.columns = un_dummy.columns.str.replace("-", "_")
+    return pd.concat([df.drop(new_column_names, axis=1), un_dummy], axis=1)
+    """
+    un_dummy = undummify(df[dummy_cols])
+    return pd.concat([df.drop(dummy_cols, axis=1), un_dummy], axis=1)
+
+
+def undummify(df, prefix_sep="_"):
+    cols2collapse = {prefix_sep.join(item.split(prefix_sep)[:-1]): (prefix_sep in item) for item in df.columns}
+    series_list = []
+    for col, needs_to_collapse in cols2collapse.items():
+        if needs_to_collapse:
+            undummified = df.filter(like=col).idxmax(axis=1).apply(lambda x: x.split(prefix_sep)[-1]).rename(col)
+            series_list.append(undummified)
+        else:
+            series_list.append(df[col])
+    undummified_df = pd.concat(series_list, axis=1)
+    return undummified_df
+
+
+def get_dummy_cols(df: pd.DataFrame) -> list:
+    """Determines a list of dummy columns for the given DataFrame
+    Args:
+        df (pd.DataFrame): Input DataFrame
+    Returns:
+        list: List of dummy columns
+    """
+    dum_cols = list(df.select_dtypes(include=["int", "bool"]).columns)
+    underscore_cols = [col for col in df.columns if "_" in col and col in dum_cols]
+    dummy_cols = []
+    for col in underscore_cols:
+        # Just columns with 0 and 1
+        if set(df[col].unique()).issubset([0, 1]):
+            dummy_cols.append(col)
+    return dummy_cols
+
+
 if __name__ == "__main__":
     """Exercise the Pandas Utility Methods"""
     from datetime import datetime
+    from sageworks.artifacts.feature_sets.feature_set import FeatureSet
 
     # Setup Pandas output options
     pd.set_option("display.max_colwidth", 35)
     pd.set_option("display.max_columns", 15)
     pd.set_option("display.width", 1000)
 
     # Create some fake data
@@ -249,7 +307,25 @@
 
     # Drop Outliers
     norm_df = drop_outliers_iqr(clean_df)
     log.info(norm_df)
 
     norm_df = drop_outliers_sdev(clean_df)
     log.info(norm_df)
+
+    # Create a FeatureSet and compute it's displayable dataframe
+    fs = FeatureSet("test_feature_set")
+    df = fs.sample_df()
+    print(df.head())
+    display_df = displayable_df(df)
+    print(display_df.head(10))
+
+    # Try with a column that has a '_' in it
+    df.rename(columns={"name": "first_name"}, inplace=True)
+    display_df = displayable_df(df)
+    print(display_df.head(10))
+
+    # TEMP: Try is with our DNS data
+    fs = FeatureSet("dns_features_2")
+    dns_df = fs.query("SELECT * from dns_features_2_1686239028 limit 100")
+    display_df = displayable_df(dns_df)
+    print(display_df.head(10))
```

### Comparing `sageworks-0.1.5.2/src/sageworks/transforms/transform.py` & `sageworks-0.1.5.3/src/sageworks/transforms/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,31 +90,31 @@
 
         # For DataSource and FeatureSet we'll compute sample rows, quartiles, and value counts
         if self.output_type == TransformOutput.DATA_SOURCE:
             self.log.info("Computing Details, Sample Rows, and Quartiles...")
             while not DataSource(self.output_uuid).check():
                 self.log.info("Waiting for DataSource to be created...")
                 sleep(1)
-            ds = DataSource(self.output_uuid)
-            ds.refresh(force_fresh=True)
+            ds = DataSource(self.output_uuid, force_refresh=True)
             ds.details()
             ds.sample_df()
             ds.quartiles()
+            ds.outliers()
             ds.value_counts()
 
         elif self.output_type == TransformOutput.FEATURE_SET:
             self.log.info("Computing Details, Sample Rows, and Quartiles...")
             while not FeatureSet(self.output_uuid).check():
                 self.log.info("Waiting for FeatureSet to be created...")
                 sleep(1)
-            fs = FeatureSet(self.output_uuid)
-            fs.refresh(force_fresh=True)
+            fs = FeatureSet(self.output_uuid, force_refresh=True)
             fs.details()
             fs.sample_df()
             fs.quartiles()
+            fs.outliers()
             fs.value_counts()
 
     def set_output_tags(self, tags: list | str):
         """Set the tags that will be associated with the output object
         Args:
             tags (list | str): The list of tags or a ':' separated string of tags"""
         if isinstance(tags, list):
```

### Comparing `sageworks-0.1.5.2/src/sageworks/utils/cache.py` & `sageworks-0.1.5.3/src/sageworks/utils/cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/utils/df_to_endpoint.py` & `sageworks-0.1.5.3/src/sageworks/utils/df_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/utils/iso_8601.py` & `sageworks-0.1.5.3/src/sageworks/utils/iso_8601.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/utils/redis_cache.py` & `sageworks-0.1.5.3/src/sageworks/utils/redis_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,22 @@
     redis_db = None
     try:
         # Create a temporary connection to test the connection
         _redis_db = redis.Redis(host, port=port, password=password, socket_timeout=1)
         _redis_db.ping()
 
         # Now create the actual connection
-        redis_db = redis.Redis(host, port=port, password=password, charset="utf-8", decode_responses=True, db=0)
+        redis_db = redis.Redis(
+            host,
+            port=port,
+            password=password,
+            charset="utf-8",
+            decode_responses=True,
+            db=0,
+        )
         log.info(f"Redis connection success: {host}:{port}...")
     except (redis.exceptions.ConnectionError, redis.exceptions.TimeoutError):
         msg = f"Could not connect to Redis Database: {host}:{port}..."
         log.warning(msg)
 
     @classmethod
     def check(cls):
```

### Comparing `sageworks-0.1.5.2/src/sageworks/utils/sageworks_config.py` & `sageworks-0.1.5.3/src/sageworks/utils/sageworks_config.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/utils/sageworks_event_bridge.py` & `sageworks-0.1.5.3/src/sageworks/utils/sageworks_event_bridge.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/utils/sageworks_logging.py` & `sageworks-0.1.5.3/src/sageworks/utils/sageworks_logging.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,9 +9,9 @@
         stream=os.sys.stdout,
         level=os.environ.get("LOGLEVEL", "INFO"),
         format="%(asctime)s (%(filename)s:%(lineno)d) %(levelname)s %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
     )
 
     # Make boto be more quiet
-    logging.getLogger("boto3").setLevel(logging.CRITICAL)
-    logging.getLogger("botocore").setLevel(logging.CRITICAL)
+    logging.getLogger("boto3").setLevel(logging.WARNING)
+    logging.getLogger("botocore").setLevel(logging.WARNING)
```

### Comparing `sageworks-0.1.5.2/src/sageworks/utils/sageworks_sqs.py` & `sageworks-0.1.5.3/src/sageworks/utils/sageworks_sqs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/utils/type_abbrev.py` & `sageworks-0.1.5.3/src/sageworks/utils/type_abbrev.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/views/artifacts_text_view.py` & `sageworks-0.1.5.3/src/sageworks/views/artifacts_text_view.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """ArtifactsTextView pulls All the metadata from the AWS Service Broker and organizes/summarizes it"""
-import sys
-import argparse
+import json
 import pandas as pd
 from termcolor import colored
 
 # SageWorks Imports
 from sageworks.views.view import View
 from sageworks.aws_service_broker.aws_service_broker import ServiceCategory
 
@@ -14,119 +13,166 @@
         """ArtifactsTextView pulls All the metadata from the AWS Service Broker and organizes/summarizes it"""
         # Call SuperClass Initialization
         super().__init__()
 
         # Get AWS Service information for ALL the categories (data_source, feature_set, endpoints, etc)
         self.aws_artifact_data = self.aws_broker.get_all_metadata()
 
-        # Get AWS Account Region
-        self.aws_region = self.aws_account_clamp.region()
-
         # Setup Pandas output options
         pd.set_option("display.max_colwidth", 50)
         pd.set_option("display.max_columns", 15)
         pd.set_option("display.width", 1000)
 
     def check(self) -> bool:
         """Can we connect to this view/service?"""
         return True  # I'm great, thx for asking
 
-    def refresh(self):
+    def refresh(self, force_refresh: bool = False) -> None:
         """Refresh data/metadata associated with this view"""
-        self.aws_artifact_data = self.aws_broker.get_all_metadata()
+        self.aws_artifact_data = self.aws_broker.get_all_metadata(force_refresh=force_refresh)
 
     def view_data(self) -> dict:
         """Get all the data that's useful for this view
 
         Returns:
             dict: Dictionary of Pandas Dataframes, e.g. {'INCOMING_DATA_S3': pd.DataFrame, ...}
         """
 
         # We're filling in Summary Data for all the AWS Services
         summary_data = {
             "INCOMING_DATA": self.incoming_data_summary(),
+            "GLUE_JOBS": self.glue_jobs_summary(),
             "DATA_SOURCES": self.data_sources_summary(),
             "FEATURE_SETS": self.feature_sets_summary(),
             "MODELS": self.models_summary(),
             "ENDPOINTS": self.endpoints_summary(),
         }
         return summary_data
 
     @staticmethod
     def header_text(header_text: str) -> str:
         """Colorize text for the terminal"""
         color_map = {
             "INCOMING_DATA": "cyan",
+            "GLUE_JOBS": "cyan",
             "DATA_SOURCES": "red",
             "FEATURE_SETS": "yellow",
             "MODELS": "green",
             "ENDPOINTS": "magenta",
         }
         header = f"\n{'='*111}\n{header_text}\n{'='*111}"
         return colored(header, color_map[header_text])
 
     def summary(self) -> None:
         """Give a summary of all the Artifact data to stdout"""
         for name, df in self.view_data().items():
             print(self.header_text(name))
             if df.empty:
-                print("\tNo ArtifactsTextView Found")
+                print("\tNo Artifacts Found")
             else:
+                # Remove any columns that start with _
+                df = df.loc[:, ~df.columns.str.startswith("_")]
                 print(df.to_string(index=False))
 
     def incoming_data_summary(self) -> pd.DataFrame:
         """Get summary data about data in the incoming-data S3 Bucket"""
         data = self.aws_artifact_data[ServiceCategory.INCOMING_DATA_S3]
         data_summary = []
         for name, info in data.items():
-            # Get the size of the S3 Storage Object(s)
+            # Get the name and the size of the S3 Storage Object(s)
+            name = "/".join(name.split("/")[-2:]).replace("incoming-data/", "")
+            info["Name"] = name
             size = info.get("ContentLength") / 1_000_000
             summary = {
-                "Name": "/".join(name.split("/")[-2:]).replace("incoming-data/", ""),
+                "Name": name,
                 "Size(MB)": f"{size:.2f}",
                 "Modified": self.datetime_string(info.get("LastModified", "-")),
                 "ContentType": str(info.get("ContentType", "-")),
                 "ServerSideEncryption": info.get("ServerSideEncryption", "-"),
-                "Tags": str(
-                    info.get("tags", "-"),
-                ),
+                "Tags": str(info.get("tags", "-")),
+                "_aws_url": self.aws_url(info, "S3"),  # Hidden Column
             }
             data_summary.append(summary)
 
         # Make sure we have data else return just the column names
         if data_summary:
             return pd.DataFrame(data_summary)
         else:
-            columns = ["Name", "Size(MB)", "Modified", "ContentType", "ServerSideEncryption", "Tags"]
+            columns = [
+                "Name",
+                "Size(MB)",
+                "Modified",
+                "ContentType",
+                "ServerSideEncryption",
+                "Tags",
+                "_aws_url",
+            ]
+            return pd.DataFrame(columns=columns)
+
+    def glue_jobs_summary(self) -> pd.DataFrame:
+        """Get summary data about AWS Glue Jobs"""
+        glue_meta = self.aws_artifact_data[ServiceCategory.GLUE_JOBS]
+        glue_summary = []
+
+        # Get the information about each Glue Job
+        for name, info in glue_meta.items():  # Just the sageworks database
+            summary = {
+                "Name": info["Name"],
+                "GlueVersion": info["GlueVersion"],
+                "Workers": info["NumberOfWorkers"],
+                "WorkerType": info["WorkerType"],
+                "Modified": self.datetime_string(info.get("LastModifiedOn")),
+                "LastRun": self.datetime_string(info["sageworks_meta"]["last_run"]),
+                "Status": info["sageworks_meta"]["status"],
+                "_aws_url": self.aws_url(info, "GlueJob"),  # Hidden Column
+            }
+            glue_summary.append(summary)
+
+        # Make sure we have data else return just the column names
+        if glue_summary:
+            return pd.DataFrame(glue_summary)
+        else:
+            columns = [
+                "Name",
+                "GlueVersion",
+                "Workers",
+                "WorkerType",
+                "Modified",
+                "LastRun",
+                "Status",
+                "_aws_url",
+            ]
             return pd.DataFrame(columns=columns)
 
     def data_sources_summary(self) -> pd.DataFrame:
         """Get summary data about the SageWorks DataSources"""
         data_catalog = self.aws_artifact_data[ServiceCategory.DATA_CATALOG]
         data_summary = []
 
         # Get the SageWorks DataSources
         if "sageworks" in data_catalog:
             for name, info in data_catalog["sageworks"].items():  # Just the sageworks database
                 # Get the size of the S3 Storage Object(s)
                 size = self.aws_broker.get_s3_object_sizes(
-                    ServiceCategory.DATA_SOURCES_S3, info["StorageDescriptor"]["Location"]
+                    ServiceCategory.DATA_SOURCES_S3,
+                    info["StorageDescriptor"]["Location"],
                 )
                 size = f"{size/1_000_000:.2f}"
                 summary = {
                     "Name": name,
                     "Ver": info.get("VersionId", "-"),
                     "Size(MB)": size,
                     "Modified": self.datetime_string(info.get("UpdateTime")),
                     "Num Columns": self.num_columns(info),
                     "DataLake": info.get("IsRegisteredWithLakeFormation", "-"),
                     "Tags": info.get("Parameters", {}).get("sageworks_tags", "-"),
                     "Input": str(
                         info.get("Parameters", {}).get("sageworks_input", "-"),
                     ),
+                    "_aws_url": self.aws_url(info, "DataSource"),  # Hidden Column
                 }
                 data_summary.append(summary)
 
         # Make sure we have data else return just the column names
         if data_summary:
             return pd.DataFrame(data_summary)
         else:
@@ -135,39 +181,43 @@
                 "Ver",
                 "Size(MB)",
                 "Modified",
                 "Num Columns",
                 "DataLake",
                 "Tags",
                 "Input",
+                "_aws_url",
             ]
             return pd.DataFrame(columns=columns)
 
     def feature_sets_summary(self) -> pd.DataFrame:
         """Get summary data about the SageWorks FeatureSets"""
         data = self.aws_artifact_data[ServiceCategory.FEATURE_STORE]
         data_summary = []
         for feature_group, group_info in data.items():
             # Get the SageWorks metadata for this Feature Group
             sageworks_meta = group_info.get("sageworks_meta", {})
 
             # Get the size of the S3 Storage Object(s)
             size = self.aws_broker.get_s3_object_sizes(
-                ServiceCategory.FEATURE_SETS_S3, group_info["OfflineStoreConfig"]["S3StorageConfig"]["S3Uri"]
+                ServiceCategory.FEATURE_SETS_S3,
+                group_info["OfflineStoreConfig"]["S3StorageConfig"]["S3Uri"],
             )
             size = f"{size / 1_000_000:.2f}"
+            cat_config = group_info["OfflineStoreConfig"].get("DataCatalogConfig", {})
             summary = {
                 "Feature Group": group_info["FeatureGroupName"],
                 "Size(MB)": size,
-                "Catalog DB": group_info["OfflineStoreConfig"].get("DataCatalogConfig", {}).get("Database", "-"),
-                "Athena Table": group_info["OfflineStoreConfig"].get("DataCatalogConfig", {}).get("TableName", "-"),
+                "Catalog DB": cat_config.get("Database", "-").lower(),
+                "Athena Table": cat_config.get("TableName", "-"),
                 "Online": str(group_info.get("OnlineStoreConfig", {}).get("EnableOnlineStore", "False")),
                 "Created": self.datetime_string(group_info.get("CreationTime")),
                 "Tags": sageworks_meta.get("sageworks_tags", "-"),
                 "Input": sageworks_meta.get("sageworks_input", "-"),
+                "_aws_url": self.aws_url(group_info, "FeatureSet"),  # Hidden Column
             }
             data_summary.append(summary)
 
         # Make sure we have data else return just the column names
         if data_summary:
             return pd.DataFrame(data_summary)
         else:
@@ -176,14 +226,15 @@
                 "Size(MB)",
                 "Catalog DB",
                 "Athena Table",
                 "Online",
                 "Created",
                 "Tags",
                 "Input",
+                "_aws_url",
             ]
             return pd.DataFrame(columns=columns)
 
     def models_summary(self) -> pd.DataFrame:
         """Get summary data about the SageWorks Models"""
         data = self.aws_artifact_data[ServiceCategory.MODELS]
         model_summary = []
@@ -272,26 +323,46 @@
     def datetime_string(datetime_obj):
         """Helper: Convert DateTime Object into a nice string"""
         if datetime_obj is None:
             return "-"
         # Date + Hour Minute
         return datetime_obj.strftime("%Y-%m-%d %H:%M")
 
+    def aws_url(self, artifact_info, artifact_type):
+        """Helper: Try to extract the AWS URL from the Artifact Info Object"""
+        if artifact_type == "S3":
+            # Construct the AWS URL for the S3 Bucket
+            name = artifact_info["Name"]
+            region = self.aws_account_clamp.region
+            s3_prefix = f"incoming-data/{name}"
+            bucket_name = self.aws_account_clamp.sageworks_bucket_name
+            base_url = "https://s3.console.aws.amazon.com/s3/object"
+            return f"{base_url}/{bucket_name}?region={region}&prefix={s3_prefix}"
+        elif artifact_type == "GlueJob":
+            # Construct the AWS URL for the Glue Job
+            region = self.aws_account_clamp.region
+            job_name = artifact_info["Name"]
+            base_url = f"https://{region}.console.aws.amazon.com/gluestudio/home"
+            return f"{base_url}?region={region}#/editor/job/{job_name}/details"
+        elif artifact_type == "DataSource":
+            details = artifact_info.get("Parameters", {}).get("sageworks_details", "{}")
+            return json.loads(details).get("aws_url", "unknown")
+        elif artifact_type == "FeatureSet":
+            aws_url = artifact_info.get("sageworks_meta", {}).get("aws_url", "unknown")
+            # Hack for constraints on the SageMaker Feature Group Tags
+            return aws_url.replace("__question__", "?").replace("__pound__", "#")
+
 
 if __name__ == "__main__":
-    # Collect args from the command line
-    parser = argparse.ArgumentParser()
-    args, commands = parser.parse_known_args()
-
-    # Check for unknown args
-    if commands:
-        print("Unrecognized args: %s" % commands)
-        sys.exit(1)
+    import time
 
     # Create the class and get the AWS Model Registry details
     artifacts = ArtifactsTextView()
 
     # Pull the data for all Artifacts in the AWS Account
     artifacts.view_data()
 
     # Give a text summary of all the Artifacts in the AWS Account
     artifacts.summary()
+
+    # Give any broker threads time to finish
+    time.sleep(1)
```

### Comparing `sageworks-0.1.5.2/src/sageworks/views/data_source_web_view.py` & `sageworks-0.1.5.3/src/sageworks/views/data_source_web_view.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,61 +16,71 @@
         self.data_sources_df = self.data_sources_summary()
 
     def refresh(self):
         """Refresh the data from the AWS Service Broker"""
         super().refresh()
         self.data_sources_df = self.data_sources_summary()
 
-    def view_data(self) -> dict:
+    def view_data(self) -> pd.DataFrame:
         """Get all the data that's useful for this view
 
         Returns:
-            dict: Dictionary of Pandas Dataframes, e.g. {'DATA_SOURCES': pd.DataFrame, ...}
+            pd.DataFrame: DataFrame of the DataSources View Data
         """
-        return {"DATA_SOURCES": self.data_sources_df}  # Just the DataSources Summary Dataframe
+        return self.data_sources_df
 
     def data_source_sample(self, data_source_index: int) -> pd.DataFrame:
         """Get a sample dataframe for the given DataSource Index"""
         data_uuid = self.data_source_name(data_source_index)
         if data_uuid is not None:
             ds = DataSource(data_uuid)
-            sample_rows = ds.sample_df()
+            return ds.sample_df()
         else:
-            sample_rows = pd.DataFrame()
-        return sample_rows
+            return pd.DataFrame()
+
+    def data_source_outliers(self, data_source_index: int) -> pd.DataFrame:
+        """Get a dataframe of outliers for the given DataSource Index"""
+        data_uuid = self.data_source_name(data_source_index)
+        if data_uuid is not None:
+            ds = DataSource(data_uuid)
+            return ds.outliers()
+        else:
+            return pd.DataFrame()
 
     def data_source_quartiles(self, data_source_index: int) -> (dict, None):
         """Get all columns quartiles for the given DataSource Index"""
         data_uuid = self.data_source_name(data_source_index)
         if data_uuid is not None:
-            quartiles_data = DataSource(data_uuid).quartiles()
-            return quartiles_data
+            return DataSource(data_uuid).quartiles()
         else:
             return None
 
     def data_source_smart_sample(self, data_source_index: int) -> pd.DataFrame:
         """Get a SMART sample dataframe for the given DataSource Index
         Note:
-            SMART here means a sample data + quartiles for each column"""
+            SMART here means a sample data + quartiles + outliers for each column"""
         # Sample DataFrame
         sample_rows = self.data_source_sample(data_source_index)
 
+        # Outliers DataFrame
+        outlier_rows = self.data_source_outliers(data_source_index)
+
         # Quartiles Data
         quartiles_data = self.data_source_quartiles(data_source_index)
         if quartiles_data is None:
             return sample_rows
 
         # Convert the Quartiles Data into a DataFrame
         quartiles_dict_list = dict()
         for col_name, quartiles in quartiles_data.items():
             quartiles_dict_list[col_name] = quartiles.values()
         quartiles_df = pd.DataFrame(quartiles_dict_list)
 
         # Combine the sample rows with the quartiles data
-        return pd.concat([sample_rows, quartiles_df]).reset_index(drop=True)
+        return pd.concat([sample_rows, outlier_rows, quartiles_df]).reset_index(drop=True).drop_duplicates()
 
     def data_source_details(self, data_source_index: int) -> (dict, None):
         """Get all of the details for the given DataSource Index"""
         data_uuid = self.data_source_name(data_source_index)
         if data_uuid is not None:
             ds = DataSource(data_uuid)
             details_data = ds.details()
@@ -93,15 +103,15 @@
     from pprint import pprint
 
     # Create the class and get the AWS DataSource details
     data_view = DataSourceWebView()
 
     # List the DataSources
     print("DataSourcesSummary:")
-    summary = data_view.view_data()["DATA_SOURCES"]
+    summary = data_view.view_data()
     print(summary.head())
 
     # Get the details for the first DataSource
     print("\nDataSourceDetails:")
     details = data_view.data_source_details(0)
     pprint(details)
```

### Comparing `sageworks-0.1.5.2/src/sageworks/views/feature_set_web_view.py` & `sageworks-0.1.5.3/src/sageworks/views/feature_set_web_view.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,69 +16,83 @@
         self.feature_sets_df = self.feature_sets_summary()
 
     def refresh(self):
         """Refresh the data from the AWS Service Broker"""
         super().refresh()
         self.feature_sets_df = self.feature_sets_summary()
 
-    def view_data(self) -> dict:
+    def view_data(self) -> pd.DataFrame:
         """Get all the data that's useful for this view
 
         Returns:
-            dict: Dictionary of Pandas Dataframes, e.g. {'DATA_SOURCES': pd.DataFrame, ...}
+            pd.DataFrame: DataFrame of the FeatureSets View Data
         """
-        return {"DATA_SOURCES": self.feature_sets_df}  # Just the FeatureSets Summary Dataframe
+        return self.feature_sets_df
 
     def feature_set_sample(self, feature_set_index: int) -> pd.DataFrame:
         """Get a sample dataframe for the given FeatureSet Index"""
-        data_uuid = self.feature_set_name(feature_set_index)
-        if data_uuid is not None:
-            ds = FeatureSet(data_uuid)
-            sample_rows = ds.sample_df()
+        uuid = self.feature_set_name(feature_set_index)
+        fs = FeatureSet(uuid)
+        if fs.check() and fs.get_status() == "ready":
+            return fs.sample_df()
+        else:
+            status = fs.get_status() if fs.check() else "not found"
+            return pd.DataFrame({"uuid": [uuid], "status": [f"{status}"]})
+
+    def feature_set_outliers(self, feature_set_index: int) -> pd.DataFrame:
+        """Get a dataframe of outliers for the given FeatureSet Index"""
+        uuid = self.feature_set_name(feature_set_index)
+        fs = FeatureSet(uuid)
+        if fs.check() and fs.get_status() == "ready":
+            return fs.outliers()
         else:
-            sample_rows = pd.DataFrame()
-        return sample_rows
+            status = fs.get_status() if fs.check() else "not found"
+            return pd.DataFrame({"uuid": [uuid], "status": [f"{status}"]})
 
     def feature_set_quartiles(self, feature_set_index: int) -> (dict, None):
         """Get all columns quartiles for the given FeatureSet Index"""
         data_uuid = self.feature_set_name(feature_set_index)
-        if data_uuid is not None:
-            quartiles_data = FeatureSet(data_uuid).quartiles()
-            return quartiles_data
+        uuid = self.feature_set_name(feature_set_index)
+        fs = FeatureSet(uuid)
+        if fs.check() and fs.get_status() == "ready":
+            return FeatureSet(data_uuid).quartiles()
         else:
             return None
 
     def feature_set_smart_sample(self, feature_set_index: int) -> pd.DataFrame:
         """Get a SMART sample dataframe for the given FeatureSet Index
         Note:
-            SMART here means a sample data + quartiles for each column"""
+            SMART here means a sample data + outliers + quartiles for each column"""
         # Sample DataFrame
         sample_rows = self.feature_set_sample(feature_set_index)
 
+        # Outliers DataFrame
+        outlier_rows = self.feature_set_outliers(feature_set_index)
+
         # Quartiles Data
         quartiles_data = self.feature_set_quartiles(feature_set_index)
         if quartiles_data is None:
             return sample_rows
 
         # Convert the Quartiles Data into a DataFrame
         quartiles_dict_list = dict()
         for col_name, quartiles in quartiles_data.items():
             quartiles_dict_list[col_name] = quartiles.values()
         quartiles_df = pd.DataFrame(quartiles_dict_list)
 
         # Combine the sample rows with the quartiles data
-        return pd.concat([sample_rows, quartiles_df]).reset_index(drop=True)
+        return pd.concat([sample_rows, outlier_rows, quartiles_df]).reset_index(drop=True).drop_duplicates()
 
     def feature_set_details(self, feature_set_index: int) -> (dict, None):
-        """Get all of the details for the given FeatureSet Index"""
-        data_uuid = self.feature_set_name(feature_set_index)
-        if data_uuid is not None:
-            ds = FeatureSet(data_uuid)
-            details_data = ds.details()
-            details_data["value_counts"] = ds.value_counts()
+        """Get all the details for the given FeatureSet Index"""
+        uuid = self.feature_set_name(feature_set_index)
+        fs = FeatureSet(uuid)
+        if fs.check() and fs.get_status() == "ready":
+            details_data = fs.data_source.details()
+            details_data["value_counts"] = fs.value_counts()
             return details_data
         else:
             return None
 
     def feature_set_name(self, feature_set_index: int) -> (str, None):
         """Helper method for getting the data source name for the given FeatureSet Index"""
         if not self.feature_sets_df.empty and feature_set_index < len(self.feature_sets_df):
@@ -89,24 +103,24 @@
 
 
 if __name__ == "__main__":
     # Exercising the FeatureSetWebView
     from pprint import pprint
 
     # Create the class and get the AWS FeatureSet details
-    data_view = FeatureSetWebView()
+    feature_view = FeatureSetWebView()
 
     # List the FeatureSets
     print("FeatureSetsSummary:")
-    summary = data_view.view_data()["DATA_SOURCES"]
+    summary = feature_view.view_data()
     print(summary.head())
 
     # Get the details for the first FeatureSet
     print("\nFeatureSetDetails:")
-    details = data_view.feature_set_details(0)
+    details = feature_view.feature_set_details(0)
     pprint(details)
 
     # Get a sample dataframe for the given FeatureSets
     print("\nSampleDataFrame:")
-    sample_df = data_view.feature_set_smart_sample(0)
+    sample_df = feature_view.feature_set_smart_sample(0)
     print(sample_df.shape)
     print(sample_df.head())
```

### Comparing `sageworks-0.1.5.2/src/sageworks/views/view.py` & `sageworks-0.1.5.3/src/sageworks/views/view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/web_components/confusion_matrix.py` & `sageworks-0.1.5.3/src/sageworks/web_components/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/web_components/data_source_details.py` & `sageworks-0.1.5.3/src/sageworks/web_components/data_and_feature_details.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """A Component for details/information about DataSources"""
 from dash import dcc
 
 
-def create_markdown(data_source_details: dict) -> str:
-    """Create the Markdown for the details/information about the DataSource
+def create_markdown(artifact_details: dict) -> str:
+    """Create the Markdown for the details/information about the DataSource or the FeatureSet
     Args:
-        data_source_details (dict): A dictionary of information about the data source
+        artifact_details (dict): A dictionary of information about the artifact
     Returns:
         str: A Markdown string
     """
 
     markdown_template = """
     **Rows:** <<num_rows>>  **Columns:** <<num_columns>>
     <br>**Created/Modified:** <<created>> / <<modified>>
@@ -24,40 +24,48 @@
         <summary><b><<column_name>></b></summary>
         <ul>
         <<bullet_list>>
         </ul>
     </details>
     """
 
+    # Sanity Check for empty data
+    if not artifact_details:
+        return "No data source details found"
+
     # Loop through all the details and replace in the template
-    for key, value in data_source_details.items():
+    for key, value in artifact_details.items():
         # Hack for dates
         if ".000Z" in str(value):
             value = value.replace(".000Z", "").replace("T", " ")
         markdown_template = markdown_template.replace(f"<<{key}>>", str(value))
 
     # Loop through the column details and create collapsible sections
     details_markdown = ""
-    for column_name, value_counts in data_source_details["value_counts"].items():
+    for column_name, value_counts in artifact_details["value_counts"].items():
         bullet_list = ""
         for value, count in value_counts.items():
             bullet_list += f"<li>{value}: {count}</li>"
         details_markdown += details_template.replace("<<column_name>>", column_name).replace(
             "<<bullet_list>>", bullet_list
         )
 
     # Now actually replace the column details in the markdown
     markdown_template = markdown_template.replace("<<column_details_markdown>>", details_markdown)
     return markdown_template
 
 
-def create(component_id: str, data_source_details: dict) -> dcc.Markdown:
-    """Create a Markdown Component details/information about the DataSource
+def create(component_id: str, artifact_details: dict) -> dcc.Markdown:
+    """Create a Markdown Component details/information about the DataSource or the FeatureSet
     Args:
         component_id (str): The ID of the UI component
-        data_source_details (dict): A dictionary of column information
+        artifact_details (dict): A dictionary of column information
     Returns:
         dcc.Markdown: A Dash Markdown Component
     """
 
     # Generate a figure and wrap it in a Dash Graph Component
-    return dcc.Markdown(id=component_id, children=create_markdown(data_source_details), dangerously_allow_html=True)
+    return dcc.Markdown(
+        id=component_id,
+        children=create_markdown(artifact_details),
+        dangerously_allow_html=True,
+    )
```

### Comparing `sageworks-0.1.5.2/src/sageworks/web_components/feature_details.py` & `sageworks-0.1.5.3/src/sageworks/web_components/mock_feature_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/web_components/feature_importance.py` & `sageworks-0.1.5.3/src/sageworks/web_components/mock_feature_importance.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/web_components/histogram.py` & `sageworks-0.1.5.3/src/sageworks/web_components/histogram.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/web_components/line_chart.py` & `sageworks-0.1.5.3/src/sageworks/web_components/line_chart.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/web_components/model_data.py` & `sageworks-0.1.5.3/src/sageworks/web_components/mock_model_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks/web_components/model_details.py` & `sageworks-0.1.5.3/src/sageworks/web_components/mock_model_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/src/sageworks.egg-info/PKG-INFO` & `sageworks-0.1.5.3/src/sageworks.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.1.5.2
+Version: 0.1.5.3
 Summary: SageWorks: A Python WorkBench for creating and deploying SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 3 - Alpha
@@ -16,22 +16,26 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img align="left" src="docs/images/scp.png" width="180">
 
 # SageWorks<sup><i>TM</i></sup>
 
+<p align="center">
 <img height="360" align="left" src="https://user-images.githubusercontent.com/4806709/236641571-fc38899a-8b92-4b7c-80a0-cc9d39b92e4a.png">
 <img height="360" aligh="right" src="https://user-images.githubusercontent.com/4806709/236641581-51777977-bca4-4af3-8bec-fb1758c964b8.png">
+</p>
 
 #### SageWorks: The scientist's workbench powered by AWS® for scalability, flexibility, and security.
 
 SageWorks is a medium granularity framework that manages and aggregates AWS® Services into classes and concepts. When you use SageWorks you think about **DataSources**, **FeatureSets**, **Models**, and **Endpoints**. Underneath the hood those classes handle all the details around updating and managing a **complex set of AWS Services**. All the power and none of the pain so that your team can **Do Science Faster!**
 
-<img src="docs/images/sageworks_concepts.png">
+<p align="center">
+<img width="800" src="docs/images/sageworks_concepts.png">
+</p>
 
 ### Full SageWorks OverView
 [SageWorks Architected FrameWork](https://docs.google.com/presentation/d/1ZiSy4ulEx5gfNQS76yRv8vgkehJ9gXRJ1PulutLKzis/edit?usp=sharing)
 
 
 ## Why SageWorks?
 
@@ -42,23 +46,27 @@
 - SageWorks provides **visibility** and **transparency** into AWS SageMaker® Pipelines
     - What S3 data sources are getting pulled?
     - What Features Store/Group is the Model Using?
     - What's the ***Provenance*** of a Model in Model Registry?
     - What SageMaker Endpoints are associated with this model?
 
 
-**Single pane of glass** visibility into the AWS Services that underpin the SageWorks Classes. We can see that SageWorks automatically tags and tracks the inputs of all artifacts providing 'data provenance' for all steps in the AWS modeling pipeline.
+### Single Pane of Glass
+Visibility into the AWS Services that underpin the SageWorks Classes. We can see that SageWorks automatically tags and tracks the inputs of all artifacts providing 'data provenance' for all steps in the AWS modeling pipeline.
 
-<img width="1000" alt="Screenshot 2023-03-31 at 2 16 36 PM" src="https://user-images.githubusercontent.com/4806709/229222245-59e342c1-7254-47de-a453-268448643143.png">
+<p align="center">
+<img width="800" alt="Top Dashboard" src="https://github.com/SuperCowPowers/sageworks/assets/4806709/c4a7f054-e640-407c-9e5c-f9d3ea1bd717.png">
+</p>
 
 <i><b> Clearly illustrated:</b> SageWorks provides intuitive and transparent visibility into the full pipeline of your AWS Sagemaker Deployments.</i>
 
 
 ## Getting Started
 - [SageWorks Overview](https://docs.google.com/presentation/d/1ZiSy4ulEx5gfNQS76yRv8vgkehJ9gXRJ1PulutLKzis/edit?usp=sharing) Slides that cover and illustrate the SageWorks Modeling Pipeline.
+- [SageWorks Docs/Wiki](https://github.com/SuperCowPowers/sageworks/wiki) Our general documentation for getting started with SageWorks.
 - [SageWorks AWS Onboarding](https://github.com/SuperCowPowers/sageworks/wiki/Onboarding-SageWorks-to-AWS) Deploy the SageWorks Stack to your AWS Account. 
 - [Notebook: Start to Finish AWS ML Pipeline](https://nbviewer.org/github/SuperCowPowers/sageworks/blob/main/notebooks/ML_Pipeline_with_SageWorks.ipynb) Building an AWS® ML Pipeline from start to finish.
 - [Video: Coding with SageWorks](https://drive.google.com/file/d/1iO7IuQtTYdx4BtQjxv9lI1aVJ2ZcAo43/view?usp=sharing) Informal coding + chatting while building a full ML pipeline.
 - Join our [Discord](https://discord.gg/WHAJuz8sw8) for questions and advice on using SageWorks within your organization.
 
 ### SageWorks Zen
 - The AWS SageMaker® set of services is vast and **complex**.
```

### Comparing `sageworks-0.1.5.2/src/sageworks.egg-info/SOURCES.txt` & `sageworks-0.1.5.3/src/sageworks.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,48 +5,69 @@
 Readme.md
 SECURITY.md
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 .github/dependabot.yml
-applications/aws_dashboard/aws_dashboard.py
+applications/anomaly_inspector/Dockerfile
+applications/anomaly_inspector/README.md
+applications/anomaly_inspector/app.py
+applications/anomaly_inspector/callbacks.py
+applications/anomaly_inspector/layout.py
+applications/anomaly_inspector/requirements.txt
+applications/anomaly_inspector/assets/custom.css
+applications/anomaly_inspector/assets/favicon.ico
+applications/aws_dashboard/Dockerfile
+applications/aws_dashboard/README.md
+applications/aws_dashboard/app.py
+applications/aws_dashboard/requirements.txt
 applications/aws_dashboard/assets/custom.css
 applications/aws_dashboard/assets/favicon.ico
-applications/aws_dashboard/pages/data_sources.py
-applications/aws_dashboard/pages/endpoints.py
-applications/aws_dashboard/pages/feature_sets.py
-applications/aws_dashboard/pages/main.py
-applications/aws_dashboard/pages/models.py
-applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py
-applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py
-applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py
-applications/aws_dashboard/pages/callbacks/main_callbacks.py
-applications/aws_dashboard/pages/callbacks/models_callbacks.py
+applications/aws_dashboard/assets/trash.png
 applications/aws_dashboard/pages/data/toy_data.csv
 applications/aws_dashboard/pages/data/toy_scores.json
-applications/aws_dashboard/pages/layout/data_sources_layout.py
-applications/aws_dashboard/pages/layout/endpoints_layout.py
-applications/aws_dashboard/pages/layout/feature_sets_layout.py
-applications/aws_dashboard/pages/layout/main_layout.py
-applications/aws_dashboard/pages/layout/models_layout.py
+applications/aws_dashboard/pages/data_sources/callbacks.py
+applications/aws_dashboard/pages/data_sources/layout.py
+applications/aws_dashboard/pages/data_sources/page.py
+applications/aws_dashboard/pages/endpoints/callbacks.py
+applications/aws_dashboard/pages/endpoints/layout.py
+applications/aws_dashboard/pages/endpoints/page.py
+applications/aws_dashboard/pages/feature_sets/callbacks.py
+applications/aws_dashboard/pages/feature_sets/layout.py
+applications/aws_dashboard/pages/feature_sets/page.py
+applications/aws_dashboard/pages/main/callbacks.py
+applications/aws_dashboard/pages/main/layout.py
+applications/aws_dashboard/pages/main/page.py
+applications/aws_dashboard/pages/models/callbacks.py
+applications/aws_dashboard/pages/models/layout.py
+applications/aws_dashboard/pages/models/page.py
 applications/hello_world/callbacks.py
 applications/hello_world/hello_world.py
 applications/hello_world/layout.py
 applications/model_viewer/callbacks.py
 applications/model_viewer/layout.py
 applications/model_viewer/model_viewer.py
 applications/model_viewer/data/toy_data.csv
 applications/model_viewer/data/toy_scores.json
+applications/outlier_inspector/Dockerfile
+applications/outlier_inspector/README.md
+applications/outlier_inspector/app.py
+applications/outlier_inspector/callbacks.py
+applications/outlier_inspector/layout.py
+applications/outlier_inspector/requirements.txt
+applications/outlier_inspector/assets/custom.css
+applications/outlier_inspector/assets/favicon.ico
 applications/web_admin/flask_test.py
 applications/web_admin/hello-world-http-test.ini
 applications/web_admin/hello-world.ini
 applications/web_admin/hello-world.service
 applications/web_admin/nginx_conf/nginx.conf
 aws_setup/aws_account_check.py
+aws_setup/aws_identity_check.py
 aws_setup/build_ml_pipeline.py
 aws_setup/sageworks_cdk/.gitignore
 aws_setup/sageworks_cdk/README.md
 aws_setup/sageworks_cdk/app.py
 aws_setup/sageworks_cdk/cdk.json
 aws_setup/sageworks_cdk/requirements-dev.txt
 aws_setup/sageworks_cdk/requirements.txt
@@ -79,20 +100,22 @@
 notebooks/images/athena_query_aqsol.png
 notebooks/images/aws_dashboard_aqsol.png
 notebooks/images/dashboard_aqsol_features.png
 notebooks/images/model_screenshot.png
 notebooks/images/sageworks_concepts.png
 notebooks/images/scp_labs.png
 scripts/data_source_tags.py
+scripts/dns_data_to_features.py
 scripts/generate_jsonl_data.py
 scripts/list_data_sources.py
 src/sageworks/__init__.py
 src/sageworks.egg-info/PKG-INFO
 src/sageworks.egg-info/SOURCES.txt
 src/sageworks.egg-info/dependency_links.txt
+src/sageworks.egg-info/entry_points.txt
 src/sageworks.egg-info/requires.txt
 src/sageworks.egg-info/top_level.txt
 src/sageworks/algorithms/__init__.py
 src/sageworks/algorithms/graph/heavy/Readme.md
 src/sageworks/algorithms/graph/light/Readme.md
 src/sageworks/algorithms/table/heavy/Readme.md
 src/sageworks/algorithms/table/light/Readme.md
@@ -115,16 +138,19 @@
 src/sageworks/aws_service_broker/aws_account_clamp.py
 src/sageworks/aws_service_broker/aws_service_broker.py
 src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
 src/sageworks/aws_service_broker/aws_service_connectors/connector.py
 src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
 src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
 src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
+src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py
 src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
 src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
+src/sageworks/cli/__init__.py
+src/sageworks/cli/cli.py
 src/sageworks/transforms/Readme.md
 src/sageworks/transforms/__init__.py
 src/sageworks/transforms/transform.py
 src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
 src/sageworks/transforms/data_loaders/light/csv_to_data_source.py
 src/sageworks/transforms/data_loaders/light/json_to_data_source.py
 src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py
@@ -133,17 +159,18 @@
 src/sageworks/transforms/data_to_data/heavy/emr/Readme.md
 src/sageworks/transforms/data_to_data/heavy/glue/Readme.md
 src/sageworks/transforms/data_to_data/light/__init__.py
 src/sageworks/transforms/data_to_data/light/clean_data.py
 src/sageworks/transforms/data_to_data/light/data_to_data_light.py
 src/sageworks/transforms/data_to_features/__init__.py
 src/sageworks/transforms/data_to_features/heavy/__init__.py
-src/sageworks/transforms/data_to_features/heavy/data_to_features_heavy.py
+src/sageworks/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py
 src/sageworks/transforms/data_to_features/heavy/emr/Readme.md
 src/sageworks/transforms/data_to_features/heavy/glue/Readme.md
+src/sageworks/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py
 src/sageworks/transforms/data_to_features/light/__init__.py
 src/sageworks/transforms/data_to_features/light/data_to_features_light.py
 src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py
 src/sageworks/transforms/features_to_features/__init__.py
 src/sageworks/transforms/features_to_features/heavy/emr/Readme.md
 src/sageworks/transforms/features_to_features/heavy/glue/Readme.md
 src/sageworks/transforms/features_to_model/__init__.py
@@ -152,14 +179,15 @@
 src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template
 src/sageworks/transforms/model_to_endpoint/__init__.py
 src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py
 src/sageworks/transforms/pandas_transforms/data_to_pandas.py
 src/sageworks/transforms/pandas_transforms/features_to_pandas.py
 src/sageworks/transforms/pandas_transforms/pandas_to_data.py
 src/sageworks/transforms/pandas_transforms/pandas_to_features.py
+src/sageworks/transforms/pandas_transforms/pandas_to_features_chunked.py
 src/sageworks/transforms/pandas_transforms/pandas_utils.py
 src/sageworks/utils/__init__.py
 src/sageworks/utils/cache.py
 src/sageworks/utils/df_to_endpoint.py
 src/sageworks/utils/iso_8601.py
 src/sageworks/utils/redis_cache.py
 src/sageworks/utils/sageworks_config.py
@@ -167,28 +195,28 @@
 src/sageworks/utils/sageworks_logging.py
 src/sageworks/utils/sageworks_sqs.py
 src/sageworks/utils/type_abbrev.py
 src/sageworks/views/artifacts_text_view.py
 src/sageworks/views/artifacts_web_view.py
 src/sageworks/views/data_source_web_view.py
 src/sageworks/views/feature_set_web_view.py
+src/sageworks/views/model_web_view.py
 src/sageworks/views/view.py
-src/sageworks/web_components/box_plot.py
+src/sageworks/web_components/color_maps.py
 src/sageworks/web_components/confusion_matrix.py
-src/sageworks/web_components/data_source_details.py
-src/sageworks/web_components/feature_details.py
-src/sageworks/web_components/feature_importance.py
-src/sageworks/web_components/feature_set_details.py
+src/sageworks/web_components/data_and_feature_details.py
+src/sageworks/web_components/distribution_plots.py
 src/sageworks/web_components/histogram.py
 src/sageworks/web_components/line_chart.py
-src/sageworks/web_components/model_data.py
-src/sageworks/web_components/model_details.py
+src/sageworks/web_components/mock_feature_details.py
+src/sageworks/web_components/mock_feature_importance.py
+src/sageworks/web_components/mock_model_data.py
+src/sageworks/web_components/mock_model_details.py
 src/sageworks/web_components/scatter_plot.py
 src/sageworks/web_components/table.py
-src/sageworks/web_components/violin_plot.py
 tests/create_sageworks_objs_for_tests.py
 tests/artifacts/data_source_tests.py
 tests/artifacts/endpoint_tests.py
 tests/artifacts/feature_set_tests.py
 tests/artifacts/model_tests.py
 tests/aws_account/aws_account_clamp_tests.py
 tests/aws_account/aws_service_broker_tests.py
```

### Comparing `sageworks-0.1.5.2/tests/artifacts/data_source_tests.py` & `sageworks-0.1.5.3/tests/artifacts/data_source_tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     # When was it created and last modified?
     print(f"Created: {my_data.created()}")
     print(f"Modified: {my_data.modified()}")
 
     # Get Tags associated with this Artifact
     print(f"Tags: {my_data.sageworks_tags()}")
 
-    # Get ALL Metadata associated with this Artifact
+    # Get ALL the AWS Metadata associated with this Artifact
     print("\n\nALL Meta")
-    pprint(my_data.all_meta())
+    pprint(my_data.aws_meta())
 
     # Now delete the AWS artifacts associated with this DataSource
     # print('Deleting SageWorks Data Source...')
     # my_data.delete()
 
 
 if __name__ == "__main__":
```

### Comparing `sageworks-0.1.5.2/tests/artifacts/endpoint_tests.py` & `sageworks-0.1.5.3/tests/artifacts/endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/tests/artifacts/feature_set_tests.py` & `sageworks-0.1.5.3/tests/artifacts/feature_set_tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,17 +24,17 @@
     # What are the column names?
     columns = my_features.column_names()
     print(columns)
 
     # Get Tags associated with this Feature Set
     print(f"Tags: {my_features.sageworks_tags()}")
 
-    # Get ALL Metadata associated with this Feature Set
+    # Get ALL the AWS Metadata associated with this Feature Set
     print("\n\nALL Meta")
-    pprint(my_features.all_meta())
+    pprint(my_features.aws_meta())
 
     # Now delete the AWS artifacts associated with this Feature Set
     # print('Deleting SageWorks Feature Set...')
     # my_features.delete()
 
 
 if __name__ == "__main__":
```

### Comparing `sageworks-0.1.5.2/tests/artifacts/model_tests.py` & `sageworks-0.1.5.3/tests/artifacts/model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/tests/aws_account/aws_account_clamp_tests.py` & `sageworks-0.1.5.3/tests/aws_account/aws_account_clamp_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/tests/aws_account/aws_service_broker_tests.py` & `sageworks-0.1.5.3/tests/aws_account/aws_service_broker_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/tests/create_sageworks_objs_for_tests.py` & `sageworks-0.1.5.3/tests/create_sageworks_objs_for_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/tests/transforms/data_to_data_tests.py` & `sageworks-0.1.5.3/tests/transforms/data_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/tests/transforms/data_to_features_tests.py` & `sageworks-0.1.5.3/tests/transforms/data_to_features_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/tests/transforms/features_to_model_tests.py` & `sageworks-0.1.5.3/tests/transforms/features_to_model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/tests/transforms/model_to_endpoint_tests.py` & `sageworks-0.1.5.3/tests/transforms/model_to_endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/tests/transforms/pandas_to_data_tests.py` & `sageworks-0.1.5.3/tests/transforms/pandas_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.2/tox.ini` & `sageworks-0.1.5.3/tox.ini`

 * *Files identical despite different names*

