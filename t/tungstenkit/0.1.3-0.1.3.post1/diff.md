# Comparing `tmp/tungstenkit-0.1.3.tar.gz` & `tmp/tungstenkit-0.1.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tungstenkit-0.1.3.tar", max compression
+gzip compressed data, was "tungstenkit-0.1.3.post1.tar", max compression
```

## Comparing `tungstenkit-0.1.3.tar` & `tungstenkit-0.1.3.post1.tar`

### file list

```diff
@@ -1,171 +1,171 @@
--rw-r--r--   0        0        0    11352 2023-07-13 17:08:18.581431 tungstenkit-0.1.3/LICENSE
--rw-r--r--   0        0        0     7736 2023-06-14 05:43:16.713685 tungstenkit-0.1.3/README.md
--rw-r--r--   0        0        0     2868 2023-07-13 18:00:39.580090 tungstenkit-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      424 2023-06-02 07:54:47.474527 tungstenkit-0.1.3/tungstenkit/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.3/tungstenkit/_internal/__init__.py
--rw-r--r--   0        0        0     7544 2023-07-13 18:31:33.027824 tungstenkit-0.1.3/tungstenkit/_internal/blob_store.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.3/tungstenkit/_internal/cli/__init__.py
--rw-r--r--   0        0        0     2636 2023-07-10 01:51:59.287508 tungstenkit-0.1.3/tungstenkit/_internal/cli/callbacks.py
--rw-r--r--   0        0        0     2296 2023-05-26 10:03:30.716386 tungstenkit-0.1.3/tungstenkit/_internal/cli/login_command.py
--rw-r--r--   0        0        0     1414 2023-06-05 05:27:13.011868 tungstenkit-0.1.3/tungstenkit/_internal/cli/main.py
--rw-r--r--   0        0        0    11227 2023-07-10 08:15:53.146471 tungstenkit-0.1.3/tungstenkit/_internal/cli/model_commands.py
--rw-r--r--   0        0        0      653 2023-05-05 07:02:23.664425 tungstenkit-0.1.3/tungstenkit/_internal/cli/options.py
--rw-r--r--   0        0        0     5656 2023-07-11 15:36:54.859197 tungstenkit-0.1.3/tungstenkit/_internal/configs.py
--rw-r--r--   0        0        0     2615 2023-07-13 18:15:37.115651 tungstenkit-0.1.3/tungstenkit/_internal/constants.py
--rw-r--r--   0        0        0       58 2023-05-05 07:02:23.660425 tungstenkit-0.1.3/tungstenkit/_internal/containerize/__init__.py
--rw-r--r--   0        0        0      385 2023-05-05 07:02:23.660425 tungstenkit-0.1.3/tungstenkit/_internal/containerize/base_images/__init__.py
--rw-r--r--   0        0        0      474 2023-05-12 12:06:44.057340 tungstenkit-0.1.3/tungstenkit/_internal/containerize/base_images/base_image.py
--rw-r--r--   0        0        0      574 2023-05-05 07:02:23.660425 tungstenkit-0.1.3/tungstenkit/_internal/containerize/base_images/common.py
--rw-r--r--   0        0        0      238 2023-05-05 07:02:23.660425 tungstenkit-0.1.3/tungstenkit/_internal/containerize/base_images/conda_image.py
--rw-r--r--   0        0        0     2552 2023-05-11 12:17:37.316053 tungstenkit-0.1.3/tungstenkit/_internal/containerize/base_images/cuda_image.py
--rw-r--r--   0        0        0      369 2023-05-05 07:02:23.660425 tungstenkit-0.1.3/tungstenkit/_internal/containerize/base_images/custom_image.py
--rw-r--r--   0        0        0     1622 2023-05-11 12:17:39.436044 tungstenkit-0.1.3/tungstenkit/_internal/containerize/base_images/python_image.py
--rw-r--r--   0        0        0    12994 2023-07-13 18:49:42.467782 tungstenkit-0.1.3/tungstenkit/_internal/containerize/build_context.py
--rw-r--r--   0        0        0      172 2023-05-29 05:33:04.832002 tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/__init__.py
--rw-r--r--   0        0        0     8989 2023-07-13 16:07:48.443313 tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py
--rw-r--r--   0        0        0      653 2023-07-06 06:52:05.821846 tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py
--rw-r--r--   0        0        0     1194 2023-07-13 16:07:48.443313 tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/template_args.py
--rw-r--r--   0        0        0      262 2023-07-06 06:46:41.931629 tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/templates/debian.j2
--rw-r--r--   0        0        0      757 2023-05-29 05:58:54.040070 tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2
--rw-r--r--   0        0        0      212 2023-05-16 11:28:43.619589 tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/templates/macros/cache.j2
--rw-r--r--   0        0        0      638 2023-07-06 06:33:50.121875 tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2
--rw-r--r--   0        0        0      365 2023-07-06 07:18:49.448528 tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/templates/setup_tungsten.j2
--rw-r--r--   0        0        0     1149 2023-07-10 06:59:55.446738 tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2
--rw-r--r--   0        0        0      899 2023-05-12 11:41:21.669195 tungstenkit-0.1.3/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py
--rw-r--r--   0        0        0     4387 2023-07-06 14:13:05.914071 tungstenkit-0.1.3/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py
--rw-r--r--   0        0        0     1655 2023-07-06 13:41:56.275424 tungstenkit-0.1.3/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py
--rw-r--r--   0        0        0     4410 2023-07-06 14:01:27.074963 tungstenkit-0.1.3/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py
--rw-r--r--   0        0        0     6699 2023-07-06 14:03:06.017399 tungstenkit-0.1.3/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py
--rw-r--r--   0        0        0        0 2023-05-16 13:16:00.016349 tungstenkit-0.1.3/tungstenkit/_internal/containerize/metadata/__init__.py
--rw-r--r--   0        0        0     4690 2023-07-05 07:18:21.638440 tungstenkit-0.1.3/tungstenkit/_internal/containerize/metadata/metadata_loader.py
--rw-r--r--   0        0        0     3641 2023-07-10 02:27:14.161709 tungstenkit-0.1.3/tungstenkit/_internal/containerize/model.py
--rw-r--r--   0        0        0      254 2023-05-16 12:49:36.477427 tungstenkit-0.1.3/tungstenkit/_internal/containerize/pkg_manager/__init__.py
--rw-r--r--   0        0        0      862 2023-07-06 13:52:01.692543 tungstenkit-0.1.3/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py
--rw-r--r--   0        0        0     8301 2023-07-06 14:11:58.842769 tungstenkit-0.1.3/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py
--rw-r--r--   0        0        0      916 2023-07-06 12:32:13.585865 tungstenkit-0.1.3/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py
--rw-r--r--   0        0        0       72 2023-05-17 07:08:58.956133 tungstenkit-0.1.3/tungstenkit/_internal/containers/__init__.py
--rw-r--r--   0        0        0     5101 2023-05-29 11:49:56.298526 tungstenkit-0.1.3/tungstenkit/_internal/containers/model.py
--rw-r--r--   0        0        0      132 2023-05-05 07:02:23.664425 tungstenkit-0.1.3/tungstenkit/_internal/contexts.py
--rw-r--r--   0        0        0       71 2023-06-05 05:24:44.708624 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/__init__.py
--rw-r--r--   0        0        0     6200 2023-07-10 07:59:58.496310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/404.html
--rw-r--r--   0        0        0     6231 2023-07-10 07:59:58.472310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/500.html
--rw-r--r--   0        0        0   691797 2023-07-10 07:59:58.100309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/347-963bdcebbaf02b7e.js
--rw-r--r--   0        0        0    78459 2023-07-10 07:59:58.096310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.b1049bda686b7dd5.js
--rw-r--r--   0        0        0   458866 2023-07-10 07:59:58.100309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js
--rw-r--r--   0        0        0   141052 2023-07-10 07:59:58.096310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js
--rw-r--r--   0        0        0    89842 2023-07-10 07:59:58.096310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-74c4d6b2b5c362f3.js
--rw-r--r--   0        0        0     5020 2023-07-10 07:59:58.100309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/404-1e77c517c165fca8.js
--rw-r--r--   0        0        0     5049 2023-07-10 07:59:58.100309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/500-8c3654eb5b977ca1.js
--rw-r--r--   0        0        0   130456 2023-07-10 07:59:58.100309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-0e0952e6981dcf87.js
--rw-r--r--   0        0        0      245 2023-07-10 07:59:58.100309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_error-8353112a01355ec2.js
--rw-r--r--   0        0        0    26735 2023-07-10 07:59:58.100309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-7a54d14da4b684a5.js
--rw-r--r--   0        0        0    91460 2023-07-10 07:59:58.096310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0        0        0     3853 2023-07-10 07:59:58.096310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-05b74e0eb69d9e61.js
--rw-r--r--   0        0        0      791 2023-07-10 07:59:58.096310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/css/9e15ad138d9a3a18.css
--rw-r--r--   0        0        0    43645 2023-07-10 07:59:58.100309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/css/ba142f674ff207f4.css
--rw-r--r--   0        0        0      525 2023-07-10 07:59:58.100309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/lxMPbv8KZV6yW6yn81HoY/_buildManifest.js
--rw-r--r--   0        0        0       77 2023-07-10 07:59:58.100309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/lxMPbv8KZV6yW6yn81HoY/_ssgManifest.js
--rw-r--r--   0        0        0   259838 2023-07-10 07:59:58.108310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/favicon.ico
--rw-r--r--   0        0        0     6244 2023-07-10 07:59:58.468309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/index.html
--rw-r--r--   0        0        0    61184 2023-07-10 07:59:58.108310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/logo.svg
--rw-r--r--   0        0        0    27505 2023-07-10 07:59:58.108310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png
--rw-r--r--   0        0        0    18388 2023-07-10 07:59:58.108310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png
--rw-r--r--   0        0        0     2753 2023-07-10 07:54:49.523774 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/schemas.py
--rw-r--r--   0        0        0     5175 2023-07-06 10:20:57.794967 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/server.py
--rw-r--r--   0        0        0      104 2023-06-02 07:57:24.533701 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/services/__init__.py
--rw-r--r--   0        0        0     5805 2023-06-05 05:24:44.712623 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/services/file_service.py
--rw-r--r--   0        0        0    12611 2023-07-10 07:38:59.016468 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/services/prediction_service.py
--rw-r--r--   0        0        0    11504 2023-07-06 20:48:14.411044 tungstenkit-0.1.3/tungstenkit/_internal/io.py
--rw-r--r--   0        0        0     8790 2023-07-06 20:45:16.176235 tungstenkit-0.1.3/tungstenkit/_internal/io_schema.py
--rw-r--r--   0        0        0    12599 2023-07-13 16:07:48.435312 tungstenkit-0.1.3/tungstenkit/_internal/json_store.py
--rw-r--r--   0        0        0     2955 2023-05-05 07:02:23.664425 tungstenkit-0.1.3/tungstenkit/_internal/logging.py
--rw-r--r--   0        0        0      144 2023-05-26 07:24:03.204132 tungstenkit-0.1.3/tungstenkit/_internal/model_clients/__init__.py
--rw-r--r--   0        0        0     4359 2023-05-29 11:37:12.601663 tungstenkit-0.1.3/tungstenkit/_internal/model_clients/api_client.py
--rw-r--r--   0        0        0     3960 2023-07-10 07:38:59.016468 tungstenkit-0.1.3/tungstenkit/_internal/model_clients/container_client.py
--rw-r--r--   0        0        0      745 2023-07-10 07:55:04.871827 tungstenkit-0.1.3/tungstenkit/_internal/model_clients/schemas.py
--rw-r--r--   0        0        0     7765 2023-06-07 06:18:29.909695 tungstenkit-0.1.3/tungstenkit/_internal/model_def.py
--rw-r--r--   0        0        0     5102 2023-07-06 06:51:08.438142 tungstenkit-0.1.3/tungstenkit/_internal/model_def_loader.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.680424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/__init__.py
--rw-r--r--   0        0        0       32 2023-05-05 07:02:23.680424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/__main__.py
--rw-r--r--   0        0        0     2895 2023-05-29 10:20:23.323945 tungstenkit-0.1.3/tungstenkit/_internal/model_server/cli.py
--rw-r--r--   0        0        0     3549 2023-06-08 12:11:43.077003 tungstenkit-0.1.3/tungstenkit/_internal/model_server/config.py
--rw-r--r--   0        0        0      144 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/enums.py
--rw-r--r--   0        0        0       70 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/event_buses/__init__.py
--rw-r--r--   0        0        0      772 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py
--rw-r--r--   0        0        0      125 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/event_buses/event.py
--rw-r--r--   0        0        0      337 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/event_buses/factory.py
--rw-r--r--   0        0        0      511 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/event_buses/local_event_bus.py
--rw-r--r--   0        0        0       78 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/file_uploaders/__init__.py
--rw-r--r--   0        0        0      209 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/file_uploaders/abstract_file_uploader.py
--rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/file_uploaders/azure_file_uploader.py
--rw-r--r--   0        0        0      602 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/file_uploaders/factory.py
--rw-r--r--   0        0        0      675 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py
--rw-r--r--   0        0        0     2019 2023-07-13 16:07:48.447312 tungstenkit-0.1.3/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py
--rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/file_uploaders/s3_file_uploader.py
--rw-r--r--   0        0        0     5521 2023-06-07 06:18:04.645895 tungstenkit-0.1.3/tungstenkit/_internal/model_server/http_server.py
--rw-r--r--   0        0        0      563 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/ids.py
--rw-r--r--   0        0        0      184 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/input_queues/__init__.py
--rw-r--r--   0        0        0      526 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py
--rw-r--r--   0        0        0      348 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/input_queues/factory.py
--rw-r--r--   0        0        0     3215 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/input_queues/local_input_queue.py
--rw-r--r--   0        0        0      131 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/input_queues/shared.py
--rw-r--r--   0        0        0       69 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/prediction_worker/__init__.py
--rw-r--r--   0        0        0     3785 2023-05-29 05:33:04.832002 tungstenkit-0.1.3/tungstenkit/_internal/model_server/prediction_worker/executor.py
--rw-r--r--   0        0        0    10183 2023-07-04 14:01:36.565839 tungstenkit-0.1.3/tungstenkit/_internal/model_server/prediction_worker/subproc.py
--rw-r--r--   0        0        0     9882 2023-07-10 07:38:59.016468 tungstenkit-0.1.3/tungstenkit/_internal/model_server/prediction_worker/worker.py
--rw-r--r--   0        0        0      248 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/result_caches/__init__.py
--rw-r--r--   0        0        0     1487 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py
--rw-r--r--   0        0        0      396 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/result_caches/factory.py
--rw-r--r--   0        0        0    10441 2023-07-10 07:38:59.016468 tungstenkit-0.1.3/tungstenkit/_internal/model_server/result_caches/local_result_cache.py
--rw-r--r--   0        0        0      473 2023-07-10 07:39:03.628446 tungstenkit-0.1.3/tungstenkit/_internal/model_server/result_caches/shared.py
--rw-r--r--   0        0        0     1344 2023-05-26 13:10:09.787054 tungstenkit-0.1.3/tungstenkit/_internal/model_server/schema.py
--rw-r--r--   0        0        0      503 2023-05-05 07:02:23.688424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/server_exceptions.py
--rw-r--r--   0        0        0      682 2023-07-13 16:07:48.439313 tungstenkit-0.1.3/tungstenkit/_internal/model_store.py
--rw-r--r--   0        0        0      183 2023-05-29 09:28:27.561951 tungstenkit-0.1.3/tungstenkit/_internal/pred_interface/__init__.py
--rw-r--r--   0        0        0     5210 2023-07-10 07:38:59.016468 tungstenkit-0.1.3/tungstenkit/_internal/pred_interface/abstract_interface.py
--rw-r--r--   0        0        0      652 2023-05-29 09:28:27.561951 tungstenkit-0.1.3/tungstenkit/_internal/pred_interface/api_interface.py
--rw-r--r--   0        0        0     1186 2023-05-29 11:48:55.226776 tungstenkit-0.1.3/tungstenkit/_internal/pred_interface/local_interface.py
--rw-r--r--   0        0        0      440 2023-06-02 08:59:18.116896 tungstenkit-0.1.3/tungstenkit/_internal/storables/__init__.py
--rw-r--r--   0        0        0     1272 2023-07-13 18:45:11.437138 tungstenkit-0.1.3/tungstenkit/_internal/storables/avatar_data.py
--rw-r--r--   0        0        0     3208 2023-06-07 05:33:58.896669 tungstenkit-0.1.3/tungstenkit/_internal/storables/markdown_data.py
--rw-r--r--   0        0        0     7495 2023-07-13 16:07:48.439313 tungstenkit-0.1.3/tungstenkit/_internal/storables/model_data.py
--rw-r--r--   0        0        0     1095 2023-06-02 08:48:54.116248 tungstenkit-0.1.3/tungstenkit/_internal/storables/model_io_data.py
--rw-r--r--   0        0        0     5534 2023-06-01 05:57:34.935268 tungstenkit-0.1.3/tungstenkit/_internal/storables/pred_example_data.py
--rw-r--r--   0        0        0     4414 2023-07-13 18:33:59.595617 tungstenkit-0.1.3/tungstenkit/_internal/storables/source_file_data.py
--rw-r--r--   0        0        0     9258 2023-05-24 07:42:33.408342 tungstenkit-0.1.3/tungstenkit/_internal/task.py
--rw-r--r--   0        0        0      128 2023-05-26 07:24:22.424035 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/__init__.py
--rw-r--r--   0        0        0    15616 2023-07-11 15:20:57.364515 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/api_client.py
--rw-r--r--   0        0        0    11314 2023-07-10 01:48:48.085029 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/client.py
--rw-r--r--   0        0        0      553 2023-07-10 01:39:23.366905 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/__init__.py
--rw-r--r--   0        0        0       78 2023-05-05 07:02:23.664425 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/common.py
--rw-r--r--   0        0        0       97 2023-05-05 07:02:23.664425 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/datapoint.py
--rw-r--r--   0        0        0      423 2023-05-05 07:02:23.664425 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/dataset.py
--rw-r--r--   0        0        0      139 2023-06-05 12:56:54.269846 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/files.py
--rw-r--r--   0        0        0      124 2023-05-05 07:02:23.664425 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/instance.py
--rw-r--r--   0        0        0     2149 2023-07-10 07:01:26.786401 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/model.py
--rw-r--r--   0        0        0      101 2023-05-05 07:02:23.664425 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/namespace.py
--rw-r--r--   0        0        0      736 2023-07-09 23:37:27.167610 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/project.py
--rw-r--r--   0        0        0       85 2023-05-05 07:02:23.664425 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/token.py
--rw-r--r--   0        0        0      240 2023-06-05 07:47:15.889709 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/user.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.688424 tungstenkit-0.1.3/tungstenkit/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1019 2023-06-05 05:54:41.512092 tungstenkit-0.1.3/tungstenkit/_internal/utils/avatar.py
--rw-r--r--   0        0        0     2996 2023-05-05 07:02:23.688424 tungstenkit-0.1.3/tungstenkit/_internal/utils/console.py
--rw-r--r--   0        0        0     1587 2023-05-26 08:35:24.498820 tungstenkit-0.1.3/tungstenkit/_internal/utils/context.py
--rw-r--r--   0        0        0    18819 2023-07-10 08:20:25.497586 tungstenkit-0.1.3/tungstenkit/_internal/utils/docker.py
--rw-r--r--   0        0        0     3640 2023-06-07 05:33:58.896669 tungstenkit-0.1.3/tungstenkit/_internal/utils/file.py
--rw-r--r--   0        0        0      669 2023-06-07 05:33:58.896669 tungstenkit-0.1.3/tungstenkit/_internal/utils/gpu.py
--rw-r--r--   0        0        0     5354 2023-07-10 06:15:33.654911 tungstenkit-0.1.3/tungstenkit/_internal/utils/imports.py
--rw-r--r--   0        0        0     1721 2023-05-26 05:49:57.704257 tungstenkit-0.1.3/tungstenkit/_internal/utils/json.py
--rw-r--r--   0        0        0     5004 2023-06-07 05:33:58.896669 tungstenkit-0.1.3/tungstenkit/_internal/utils/markdown.py
--rw-r--r--   0        0        0      551 2023-05-05 07:02:23.688424 tungstenkit-0.1.3/tungstenkit/_internal/utils/pydantic.py
--rw-r--r--   0        0        0     2387 2023-06-01 15:17:39.232806 tungstenkit-0.1.3/tungstenkit/_internal/utils/regex.py
--rw-r--r--   0        0        0    13290 2023-06-07 05:33:58.896669 tungstenkit-0.1.3/tungstenkit/_internal/utils/requests.py
--rw-r--r--   0        0        0     2297 2023-06-01 12:30:46.490995 tungstenkit-0.1.3/tungstenkit/_internal/utils/serialize.py
--rw-r--r--   0        0        0      724 2023-05-25 05:44:14.647421 tungstenkit-0.1.3/tungstenkit/_internal/utils/string.py
--rw-r--r--   0        0        0      969 2023-07-06 21:03:05.436744 tungstenkit-0.1.3/tungstenkit/_internal/utils/types.py
--rw-r--r--   0        0        0     3081 2023-06-07 05:33:58.896669 tungstenkit-0.1.3/tungstenkit/_internal/utils/uri.py
--rw-r--r--   0        0        0     6349 2023-07-06 14:01:18.315109 tungstenkit-0.1.3/tungstenkit/_internal/utils/version.py
--rw-r--r--   0        0        0      353 2023-05-05 07:02:23.688424 tungstenkit-0.1.3/tungstenkit/_versions.py
--rw-r--r--   0        0        0     2425 2023-07-09 23:20:04.455331 tungstenkit-0.1.3/tungstenkit/exceptions.py
--rw-r--r--   0        0        0       72 2023-05-29 09:27:58.222097 tungstenkit-0.1.3/tungstenkit/models.py
--rw-r--r--   0        0        0    10564 1970-01-01 00:00:00.000000 tungstenkit-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11352 2023-07-13 17:08:18.581431 tungstenkit-0.1.3.post1/LICENSE
+-rw-r--r--   0        0        0     7736 2023-06-14 05:43:16.713685 tungstenkit-0.1.3.post1/README.md
+-rw-r--r--   0        0        0     2874 2023-07-13 19:57:08.212540 tungstenkit-0.1.3.post1/pyproject.toml
+-rw-r--r--   0        0        0      424 2023-06-02 07:54:47.474527 tungstenkit-0.1.3.post1/tungstenkit/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.3.post1/tungstenkit/_internal/__init__.py
+-rw-r--r--   0        0        0     7544 2023-07-13 18:31:33.027824 tungstenkit-0.1.3.post1/tungstenkit/_internal/blob_store.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.3.post1/tungstenkit/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     2636 2023-07-10 01:51:59.287508 tungstenkit-0.1.3.post1/tungstenkit/_internal/cli/callbacks.py
+-rw-r--r--   0        0        0     2296 2023-05-26 10:03:30.716386 tungstenkit-0.1.3.post1/tungstenkit/_internal/cli/login_command.py
+-rw-r--r--   0        0        0     1414 2023-06-05 05:27:13.011868 tungstenkit-0.1.3.post1/tungstenkit/_internal/cli/main.py
+-rw-r--r--   0        0        0    11227 2023-07-10 08:15:53.146471 tungstenkit-0.1.3.post1/tungstenkit/_internal/cli/model_commands.py
+-rw-r--r--   0        0        0      653 2023-05-05 07:02:23.664425 tungstenkit-0.1.3.post1/tungstenkit/_internal/cli/options.py
+-rw-r--r--   0        0        0     5656 2023-07-11 15:36:54.859197 tungstenkit-0.1.3.post1/tungstenkit/_internal/configs.py
+-rw-r--r--   0        0        0     2615 2023-07-13 18:15:37.115651 tungstenkit-0.1.3.post1/tungstenkit/_internal/constants.py
+-rw-r--r--   0        0        0       58 2023-05-05 07:02:23.660425 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/__init__.py
+-rw-r--r--   0        0        0      385 2023-05-05 07:02:23.660425 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/base_images/__init__.py
+-rw-r--r--   0        0        0      474 2023-05-12 12:06:44.057340 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/base_images/base_image.py
+-rw-r--r--   0        0        0      574 2023-05-05 07:02:23.660425 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/base_images/common.py
+-rw-r--r--   0        0        0      238 2023-05-05 07:02:23.660425 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/base_images/conda_image.py
+-rw-r--r--   0        0        0     2552 2023-05-11 12:17:37.316053 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/base_images/cuda_image.py
+-rw-r--r--   0        0        0      369 2023-05-05 07:02:23.660425 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/base_images/custom_image.py
+-rw-r--r--   0        0        0     1622 2023-05-11 12:17:39.436044 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/base_images/python_image.py
+-rw-r--r--   0        0        0    12994 2023-07-13 18:49:42.467782 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/build_context.py
+-rw-r--r--   0        0        0      172 2023-05-29 05:33:04.832002 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/dockerfiles/__init__.py
+-rw-r--r--   0        0        0     8989 2023-07-13 16:07:48.443313 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py
+-rw-r--r--   0        0        0      653 2023-07-06 06:52:05.821846 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py
+-rw-r--r--   0        0        0     1194 2023-07-13 16:07:48.443313 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/dockerfiles/template_args.py
+-rw-r--r--   0        0        0      262 2023-07-06 06:46:41.931629 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/dockerfiles/templates/debian.j2
+-rw-r--r--   0        0        0      757 2023-05-29 05:58:54.040070 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2
+-rw-r--r--   0        0        0      212 2023-05-16 11:28:43.619589 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/dockerfiles/templates/macros/cache.j2
+-rw-r--r--   0        0        0      638 2023-07-06 06:33:50.121875 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2
+-rw-r--r--   0        0        0      365 2023-07-06 07:18:49.448528 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/dockerfiles/templates/setup_tungsten.j2
+-rw-r--r--   0        0        0     1149 2023-07-10 06:59:55.446738 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2
+-rw-r--r--   0        0        0      899 2023-05-12 11:41:21.669195 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py
+-rw-r--r--   0        0        0     4387 2023-07-06 14:13:05.914071 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py
+-rw-r--r--   0        0        0     1655 2023-07-06 13:41:56.275424 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py
+-rw-r--r--   0        0        0     4410 2023-07-06 14:01:27.074963 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py
+-rw-r--r--   0        0        0     6699 2023-07-06 14:03:06.017399 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py
+-rw-r--r--   0        0        0        0 2023-05-16 13:16:00.016349 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/metadata/__init__.py
+-rw-r--r--   0        0        0     4690 2023-07-05 07:18:21.638440 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/metadata/metadata_loader.py
+-rw-r--r--   0        0        0     3641 2023-07-10 02:27:14.161709 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/model.py
+-rw-r--r--   0        0        0      254 2023-05-16 12:49:36.477427 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/pkg_manager/__init__.py
+-rw-r--r--   0        0        0      862 2023-07-06 13:52:01.692543 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py
+-rw-r--r--   0        0        0     8301 2023-07-06 14:11:58.842769 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py
+-rw-r--r--   0        0        0      916 2023-07-06 12:32:13.585865 tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py
+-rw-r--r--   0        0        0       72 2023-05-17 07:08:58.956133 tungstenkit-0.1.3.post1/tungstenkit/_internal/containers/__init__.py
+-rw-r--r--   0        0        0     5101 2023-05-29 11:49:56.298526 tungstenkit-0.1.3.post1/tungstenkit/_internal/containers/model.py
+-rw-r--r--   0        0        0      132 2023-05-05 07:02:23.664425 tungstenkit-0.1.3.post1/tungstenkit/_internal/contexts.py
+-rw-r--r--   0        0        0       71 2023-06-05 05:24:44.708624 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/__init__.py
+-rw-r--r--   0        0        0     6200 2023-07-10 07:59:58.496310 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/404.html
+-rw-r--r--   0        0        0     6231 2023-07-10 07:59:58.472310 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/500.html
+-rw-r--r--   0        0        0   691797 2023-07-10 07:59:58.100309 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/347-963bdcebbaf02b7e.js
+-rw-r--r--   0        0        0    78459 2023-07-10 07:59:58.096310 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.b1049bda686b7dd5.js
+-rw-r--r--   0        0        0   458866 2023-07-10 07:59:58.100309 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js
+-rw-r--r--   0        0        0   141052 2023-07-10 07:59:58.096310 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js
+-rw-r--r--   0        0        0    89842 2023-07-10 07:59:58.096310 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-74c4d6b2b5c362f3.js
+-rw-r--r--   0        0        0     5020 2023-07-10 07:59:58.100309 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/404-1e77c517c165fca8.js
+-rw-r--r--   0        0        0     5049 2023-07-10 07:59:58.100309 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/500-8c3654eb5b977ca1.js
+-rw-r--r--   0        0        0   130456 2023-07-10 07:59:58.100309 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-0e0952e6981dcf87.js
+-rw-r--r--   0        0        0      245 2023-07-10 07:59:58.100309 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_error-8353112a01355ec2.js
+-rw-r--r--   0        0        0    26735 2023-07-10 07:59:58.100309 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-7a54d14da4b684a5.js
+-rw-r--r--   0        0        0    91460 2023-07-10 07:59:58.096310 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0        0        0     3853 2023-07-10 07:59:58.096310 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-05b74e0eb69d9e61.js
+-rw-r--r--   0        0        0      791 2023-07-10 07:59:58.096310 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/css/9e15ad138d9a3a18.css
+-rw-r--r--   0        0        0    43645 2023-07-10 07:59:58.100309 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/css/ba142f674ff207f4.css
+-rw-r--r--   0        0        0      525 2023-07-10 07:59:58.100309 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/lxMPbv8KZV6yW6yn81HoY/_buildManifest.js
+-rw-r--r--   0        0        0       77 2023-07-10 07:59:58.100309 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/lxMPbv8KZV6yW6yn81HoY/_ssgManifest.js
+-rw-r--r--   0        0        0   259838 2023-07-10 07:59:58.108310 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/favicon.ico
+-rw-r--r--   0        0        0     6244 2023-07-10 07:59:58.468309 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/index.html
+-rw-r--r--   0        0        0    61184 2023-07-10 07:59:58.108310 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/logo.svg
+-rw-r--r--   0        0        0    27505 2023-07-10 07:59:58.108310 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png
+-rw-r--r--   0        0        0    18388 2023-07-10 07:59:58.108310 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png
+-rw-r--r--   0        0        0     2753 2023-07-10 07:54:49.523774 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/schemas.py
+-rw-r--r--   0        0        0     5175 2023-07-06 10:20:57.794967 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/server.py
+-rw-r--r--   0        0        0      104 2023-06-02 07:57:24.533701 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/services/__init__.py
+-rw-r--r--   0        0        0     5805 2023-06-05 05:24:44.712623 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/services/file_service.py
+-rw-r--r--   0        0        0    12611 2023-07-10 07:38:59.016468 tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/services/prediction_service.py
+-rw-r--r--   0        0        0    11504 2023-07-06 20:48:14.411044 tungstenkit-0.1.3.post1/tungstenkit/_internal/io.py
+-rw-r--r--   0        0        0     8790 2023-07-06 20:45:16.176235 tungstenkit-0.1.3.post1/tungstenkit/_internal/io_schema.py
+-rw-r--r--   0        0        0    12599 2023-07-13 16:07:48.435312 tungstenkit-0.1.3.post1/tungstenkit/_internal/json_store.py
+-rw-r--r--   0        0        0     2955 2023-05-05 07:02:23.664425 tungstenkit-0.1.3.post1/tungstenkit/_internal/logging.py
+-rw-r--r--   0        0        0      144 2023-05-26 07:24:03.204132 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_clients/__init__.py
+-rw-r--r--   0        0        0     4359 2023-05-29 11:37:12.601663 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_clients/api_client.py
+-rw-r--r--   0        0        0     3960 2023-07-10 07:38:59.016468 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_clients/container_client.py
+-rw-r--r--   0        0        0      745 2023-07-10 07:55:04.871827 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_clients/schemas.py
+-rw-r--r--   0        0        0     7765 2023-06-07 06:18:29.909695 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_def.py
+-rw-r--r--   0        0        0     5102 2023-07-06 06:51:08.438142 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_def_loader.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.680424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-05 07:02:23.680424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/__main__.py
+-rw-r--r--   0        0        0     2895 2023-05-29 10:20:23.323945 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/cli.py
+-rw-r--r--   0        0        0     3549 2023-06-08 12:11:43.077003 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/config.py
+-rw-r--r--   0        0        0      144 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/enums.py
+-rw-r--r--   0        0        0       70 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/event_buses/__init__.py
+-rw-r--r--   0        0        0      772 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py
+-rw-r--r--   0        0        0      125 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/event_buses/event.py
+-rw-r--r--   0        0        0      337 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/event_buses/factory.py
+-rw-r--r--   0        0        0      511 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/event_buses/local_event_bus.py
+-rw-r--r--   0        0        0       78 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/file_uploaders/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/file_uploaders/abstract_file_uploader.py
+-rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/file_uploaders/azure_file_uploader.py
+-rw-r--r--   0        0        0      602 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/file_uploaders/factory.py
+-rw-r--r--   0        0        0      675 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py
+-rw-r--r--   0        0        0     2019 2023-07-13 16:07:48.447312 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py
+-rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/file_uploaders/s3_file_uploader.py
+-rw-r--r--   0        0        0     5521 2023-06-07 06:18:04.645895 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/http_server.py
+-rw-r--r--   0        0        0      563 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/ids.py
+-rw-r--r--   0        0        0      184 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/input_queues/__init__.py
+-rw-r--r--   0        0        0      526 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py
+-rw-r--r--   0        0        0      348 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/input_queues/factory.py
+-rw-r--r--   0        0        0     3215 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/input_queues/local_input_queue.py
+-rw-r--r--   0        0        0      131 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/input_queues/shared.py
+-rw-r--r--   0        0        0       69 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/prediction_worker/__init__.py
+-rw-r--r--   0        0        0     3785 2023-05-29 05:33:04.832002 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/prediction_worker/executor.py
+-rw-r--r--   0        0        0    10183 2023-07-04 14:01:36.565839 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/prediction_worker/subproc.py
+-rw-r--r--   0        0        0     9882 2023-07-10 07:38:59.016468 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/prediction_worker/worker.py
+-rw-r--r--   0        0        0      248 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/result_caches/__init__.py
+-rw-r--r--   0        0        0     1487 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py
+-rw-r--r--   0        0        0      396 2023-05-05 07:02:23.684424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/result_caches/factory.py
+-rw-r--r--   0        0        0    10441 2023-07-10 07:38:59.016468 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/result_caches/local_result_cache.py
+-rw-r--r--   0        0        0      473 2023-07-10 07:39:03.628446 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/result_caches/shared.py
+-rw-r--r--   0        0        0     1344 2023-05-26 13:10:09.787054 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/schema.py
+-rw-r--r--   0        0        0      503 2023-05-05 07:02:23.688424 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/server_exceptions.py
+-rw-r--r--   0        0        0      682 2023-07-13 16:07:48.439313 tungstenkit-0.1.3.post1/tungstenkit/_internal/model_store.py
+-rw-r--r--   0        0        0      183 2023-05-29 09:28:27.561951 tungstenkit-0.1.3.post1/tungstenkit/_internal/pred_interface/__init__.py
+-rw-r--r--   0        0        0     5210 2023-07-10 07:38:59.016468 tungstenkit-0.1.3.post1/tungstenkit/_internal/pred_interface/abstract_interface.py
+-rw-r--r--   0        0        0      652 2023-05-29 09:28:27.561951 tungstenkit-0.1.3.post1/tungstenkit/_internal/pred_interface/api_interface.py
+-rw-r--r--   0        0        0     1186 2023-05-29 11:48:55.226776 tungstenkit-0.1.3.post1/tungstenkit/_internal/pred_interface/local_interface.py
+-rw-r--r--   0        0        0      440 2023-06-02 08:59:18.116896 tungstenkit-0.1.3.post1/tungstenkit/_internal/storables/__init__.py
+-rw-r--r--   0        0        0     1272 2023-07-13 18:45:11.437138 tungstenkit-0.1.3.post1/tungstenkit/_internal/storables/avatar_data.py
+-rw-r--r--   0        0        0     3208 2023-06-07 05:33:58.896669 tungstenkit-0.1.3.post1/tungstenkit/_internal/storables/markdown_data.py
+-rw-r--r--   0        0        0     7495 2023-07-13 19:56:23.712844 tungstenkit-0.1.3.post1/tungstenkit/_internal/storables/model_data.py
+-rw-r--r--   0        0        0     1095 2023-06-02 08:48:54.116248 tungstenkit-0.1.3.post1/tungstenkit/_internal/storables/model_io_data.py
+-rw-r--r--   0        0        0     5534 2023-06-01 05:57:34.935268 tungstenkit-0.1.3.post1/tungstenkit/_internal/storables/pred_example_data.py
+-rw-r--r--   0        0        0     4414 2023-07-13 18:33:59.595617 tungstenkit-0.1.3.post1/tungstenkit/_internal/storables/source_file_data.py
+-rw-r--r--   0        0        0     9258 2023-05-24 07:42:33.408342 tungstenkit-0.1.3.post1/tungstenkit/_internal/task.py
+-rw-r--r--   0        0        0      128 2023-05-26 07:24:22.424035 tungstenkit-0.1.3.post1/tungstenkit/_internal/tungsten_clients/__init__.py
+-rw-r--r--   0        0        0    15616 2023-07-11 15:20:57.364515 tungstenkit-0.1.3.post1/tungstenkit/_internal/tungsten_clients/api_client.py
+-rw-r--r--   0        0        0    11314 2023-07-10 01:48:48.085029 tungstenkit-0.1.3.post1/tungstenkit/_internal/tungsten_clients/client.py
+-rw-r--r--   0        0        0      553 2023-07-10 01:39:23.366905 tungstenkit-0.1.3.post1/tungstenkit/_internal/tungsten_clients/schemas/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-05 07:02:23.664425 tungstenkit-0.1.3.post1/tungstenkit/_internal/tungsten_clients/schemas/common.py
+-rw-r--r--   0        0        0       97 2023-05-05 07:02:23.664425 tungstenkit-0.1.3.post1/tungstenkit/_internal/tungsten_clients/schemas/datapoint.py
+-rw-r--r--   0        0        0      423 2023-05-05 07:02:23.664425 tungstenkit-0.1.3.post1/tungstenkit/_internal/tungsten_clients/schemas/dataset.py
+-rw-r--r--   0        0        0      139 2023-06-05 12:56:54.269846 tungstenkit-0.1.3.post1/tungstenkit/_internal/tungsten_clients/schemas/files.py
+-rw-r--r--   0        0        0      124 2023-05-05 07:02:23.664425 tungstenkit-0.1.3.post1/tungstenkit/_internal/tungsten_clients/schemas/instance.py
+-rw-r--r--   0        0        0     2149 2023-07-10 07:01:26.786401 tungstenkit-0.1.3.post1/tungstenkit/_internal/tungsten_clients/schemas/model.py
+-rw-r--r--   0        0        0      101 2023-05-05 07:02:23.664425 tungstenkit-0.1.3.post1/tungstenkit/_internal/tungsten_clients/schemas/namespace.py
+-rw-r--r--   0        0        0      736 2023-07-09 23:37:27.167610 tungstenkit-0.1.3.post1/tungstenkit/_internal/tungsten_clients/schemas/project.py
+-rw-r--r--   0        0        0       85 2023-05-05 07:02:23.664425 tungstenkit-0.1.3.post1/tungstenkit/_internal/tungsten_clients/schemas/token.py
+-rw-r--r--   0        0        0      240 2023-06-05 07:47:15.889709 tungstenkit-0.1.3.post1/tungstenkit/_internal/tungsten_clients/schemas/user.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.688424 tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1019 2023-06-05 05:54:41.512092 tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/avatar.py
+-rw-r--r--   0        0        0     2996 2023-05-05 07:02:23.688424 tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/console.py
+-rw-r--r--   0        0        0     1587 2023-05-26 08:35:24.498820 tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/context.py
+-rw-r--r--   0        0        0    18789 2023-07-13 19:56:11.484928 tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/docker.py
+-rw-r--r--   0        0        0     3640 2023-06-07 05:33:58.896669 tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/file.py
+-rw-r--r--   0        0        0      669 2023-06-07 05:33:58.896669 tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/gpu.py
+-rw-r--r--   0        0        0     5354 2023-07-10 06:15:33.654911 tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/imports.py
+-rw-r--r--   0        0        0     1721 2023-05-26 05:49:57.704257 tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/json.py
+-rw-r--r--   0        0        0     5004 2023-06-07 05:33:58.896669 tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/markdown.py
+-rw-r--r--   0        0        0      551 2023-05-05 07:02:23.688424 tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/pydantic.py
+-rw-r--r--   0        0        0     2387 2023-06-01 15:17:39.232806 tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/regex.py
+-rw-r--r--   0        0        0    13290 2023-06-07 05:33:58.896669 tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/requests.py
+-rw-r--r--   0        0        0     2297 2023-06-01 12:30:46.490995 tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/serialize.py
+-rw-r--r--   0        0        0      724 2023-05-25 05:44:14.647421 tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/string.py
+-rw-r--r--   0        0        0      969 2023-07-06 21:03:05.436744 tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/types.py
+-rw-r--r--   0        0        0     3081 2023-06-07 05:33:58.896669 tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/uri.py
+-rw-r--r--   0        0        0     6349 2023-07-06 14:01:18.315109 tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/version.py
+-rw-r--r--   0        0        0      353 2023-05-05 07:02:23.688424 tungstenkit-0.1.3.post1/tungstenkit/_versions.py
+-rw-r--r--   0        0        0     2425 2023-07-09 23:20:04.455331 tungstenkit-0.1.3.post1/tungstenkit/exceptions.py
+-rw-r--r--   0        0        0       72 2023-05-29 09:27:58.222097 tungstenkit-0.1.3.post1/tungstenkit/models.py
+-rw-r--r--   0        0        0    10570 1970-01-01 00:00:00.000000 tungstenkit-0.1.3.post1/PKG-INFO
```

### Comparing `tungstenkit-0.1.3/LICENSE` & `tungstenkit-0.1.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/README.md` & `tungstenkit-0.1.3.post1/README.md`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/pyproject.toml` & `tungstenkit-0.1.3.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tungstenkit"
-version = "0.1.3"
+version = "0.1.3.post1"
 description = "ML container made simple"
 authors = ["Tungsten Contributors <foss@tungsten-ai.com>"]
 homepage = "https://github.com/tungsten-ai/tungstenkit"
 readme = ["README.md"]
 packages = [{include = "tungstenkit"}]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/blob_store.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/blob_store.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/cli/callbacks.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/cli/callbacks.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/cli/login_command.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/cli/login_command.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/cli/main.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/cli/model_commands.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/cli/model_commands.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/cli/options.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/cli/options.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/configs.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/configs.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/constants.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containerize/base_images/common.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/base_images/common.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containerize/base_images/cuda_image.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/base_images/cuda_image.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containerize/base_images/python_image.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/base_images/python_image.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containerize/build_context.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/build_context.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/template_args.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/dockerfiles/template_args.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containerize/metadata/metadata_loader.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/metadata/metadata_loader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containerize/model.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/containers/model.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/containers/model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/404.html` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/404.html`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/500.html` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/500.html`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/347-963bdcebbaf02b7e.js` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/347-963bdcebbaf02b7e.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.b1049bda686b7dd5.js` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.b1049bda686b7dd5.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-74c4d6b2b5c362f3.js` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-74c4d6b2b5c362f3.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/404-1e77c517c165fca8.js` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/404-1e77c517c165fca8.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/500-8c3654eb5b977ca1.js` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/500-8c3654eb5b977ca1.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-0e0952e6981dcf87.js` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-0e0952e6981dcf87.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-7a54d14da4b684a5.js` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-7a54d14da4b684a5.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-05b74e0eb69d9e61.js` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-05b74e0eb69d9e61.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/css/9e15ad138d9a3a18.css` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/css/9e15ad138d9a3a18.css`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/css/ba142f674ff207f4.css` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/css/ba142f674ff207f4.css`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/lxMPbv8KZV6yW6yn81HoY/_buildManifest.js` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/_next/static/lxMPbv8KZV6yW6yn81HoY/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/favicon.ico` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/index.html` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/index.html`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/logo.svg` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/logo.svg`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/schemas.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/schemas.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/server.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/server.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/services/file_service.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/services/file_service.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/services/prediction_service.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/demo_server/services/prediction_service.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/io.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/io.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/io_schema.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/io_schema.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/json_store.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/json_store.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/logging.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/logging.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_clients/api_client.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_clients/container_client.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_clients/container_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_clients/schemas.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_clients/schemas.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_def.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_def.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_def_loader.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_def_loader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_server/cli.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/cli.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_server/config.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/config.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_server/file_uploaders/factory.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/file_uploaders/factory.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_server/http_server.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/http_server.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_server/ids.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/ids.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_server/input_queues/local_input_queue.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/input_queues/local_input_queue.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_server/prediction_worker/executor.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/prediction_worker/executor.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_server/prediction_worker/subproc.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/prediction_worker/subproc.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_server/prediction_worker/worker.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/prediction_worker/worker.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_server/result_caches/local_result_cache.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/result_caches/local_result_cache.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_server/schema.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_server/schema.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/model_store.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/model_store.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/pred_interface/abstract_interface.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/pred_interface/abstract_interface.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/pred_interface/api_interface.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/pred_interface/api_interface.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/pred_interface/local_interface.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/pred_interface/local_interface.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/storables/avatar_data.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/storables/avatar_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/storables/markdown_data.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/storables/markdown_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/storables/model_data.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/storables/model_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/storables/model_io_data.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/storables/model_io_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/storables/pred_example_data.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/storables/pred_example_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/storables/source_file_data.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/storables/source_file_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/task.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/task.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/api_client.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/tungsten_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/client.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/tungsten_clients/client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/__init__.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/tungsten_clients/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/model.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/tungsten_clients/schemas/model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/project.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/tungsten_clients/schemas/project.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/utils/avatar.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/utils/console.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/console.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/utils/context.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/context.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/utils/docker.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/docker.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,16 +276,15 @@
 def remove_docker_image(
     image_name_or_id: str,
     force: bool = False,
     docker_client: t.Optional[DockerClient] = None,
 ):
     docker_client = docker_client if docker_client else get_docker_client()
     try:
-        image: Image = docker_client.images.get(image_name_or_id)
-        image.remove(force=force)
+        docker_client.api.remove_image(image_name_or_id, force=force)
     except (docker_errors.NotFound, docker_errors.APIError) as e:
         if force:
             return
         raise DockerError(str(e))
 
 
 def copy_from_image(
```

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/utils/file.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/file.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/utils/gpu.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/utils/imports.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/imports.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/utils/json.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/json.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/utils/markdown.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/markdown.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/utils/pydantic.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/utils/regex.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/regex.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/utils/requests.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/requests.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/utils/serialize.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/utils/string.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/string.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/utils/types.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/types.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/utils/uri.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/uri.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/_internal/utils/version.py` & `tungstenkit-0.1.3.post1/tungstenkit/_internal/utils/version.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/tungstenkit/exceptions.py` & `tungstenkit-0.1.3.post1/tungstenkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.3/PKG-INFO` & `tungstenkit-0.1.3.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tungstenkit
-Version: 0.1.3
+Version: 0.1.3.post1
 Summary: ML container made simple
 Home-page: https://github.com/tungsten-ai/tungstenkit
 Author: Tungsten Contributors
 Author-email: foss@tungsten-ai.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

