# Comparing `tmp/tungstenkit-0.1.2.post8.tar.gz` & `tmp/tungstenkit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tungstenkit-0.1.2.post8.tar", max compression
+gzip compressed data, was "tungstenkit-0.1.3.tar", max compression
```

## Comparing `tungstenkit-0.1.2.post8.tar` & `tungstenkit-0.1.3.tar`

### file list

```diff
@@ -1,171 +1,171 @@
--rw-r--r--   0        0        0    11346 2023-05-30 17:30:59.381479 tungstenkit-0.1.2.post8/LICENSE
--rw-r--r--   0        0        0     7736 2023-06-14 05:43:16.713685 tungstenkit-0.1.2.post8/README.md
--rw-r--r--   0        0        0     2869 2023-07-12 13:31:44.565865 tungstenkit-0.1.2.post8/pyproject.toml
--rw-r--r--   0        0        0      424 2023-06-02 07:54:47.474527 tungstenkit-0.1.2.post8/tungstenkit/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post8/tungstenkit/_internal/__init__.py
--rw-r--r--   0        0        0     7499 2023-06-01 05:57:34.935268 tungstenkit-0.1.2.post8/tungstenkit/_internal/blob_store.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post8/tungstenkit/_internal/cli/__init__.py
--rw-r--r--   0        0        0     2636 2023-07-10 01:51:59.287508 tungstenkit-0.1.2.post8/tungstenkit/_internal/cli/callbacks.py
--rw-r--r--   0        0        0     2296 2023-05-26 10:03:30.716386 tungstenkit-0.1.2.post8/tungstenkit/_internal/cli/login_command.py
--rw-r--r--   0        0        0     1414 2023-06-05 05:27:13.011868 tungstenkit-0.1.2.post8/tungstenkit/_internal/cli/main.py
--rw-r--r--   0        0        0    11227 2023-07-10 08:15:53.146471 tungstenkit-0.1.2.post8/tungstenkit/_internal/cli/model_commands.py
--rw-r--r--   0        0        0      653 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post8/tungstenkit/_internal/cli/options.py
--rw-r--r--   0        0        0     5656 2023-07-11 15:36:54.859197 tungstenkit-0.1.2.post8/tungstenkit/_internal/configs.py
--rw-r--r--   0        0        0     2471 2023-07-10 07:04:01.709772 tungstenkit-0.1.2.post8/tungstenkit/_internal/constants.py
--rw-r--r--   0        0        0       58 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/__init__.py
--rw-r--r--   0        0        0      385 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/base_images/__init__.py
--rw-r--r--   0        0        0      474 2023-05-12 12:06:44.057340 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/base_images/base_image.py
--rw-r--r--   0        0        0      574 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/base_images/common.py
--rw-r--r--   0        0        0      238 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/base_images/conda_image.py
--rw-r--r--   0        0        0     2552 2023-05-11 12:17:37.316053 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/base_images/cuda_image.py
--rw-r--r--   0        0        0      369 2023-05-05 07:02:23.660425 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/base_images/custom_image.py
--rw-r--r--   0        0        0     1622 2023-05-11 12:17:39.436044 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/base_images/python_image.py
--rw-r--r--   0        0        0    13013 2023-07-10 07:02:50.614069 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/build_context.py
--rw-r--r--   0        0        0      172 2023-05-29 05:33:04.832002 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/dockerfiles/__init__.py
--rw-r--r--   0        0        0     8989 2023-07-11 15:36:22.315306 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py
--rw-r--r--   0        0        0      653 2023-07-06 06:52:05.821846 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py
--rw-r--r--   0        0        0     1194 2023-07-11 15:39:12.682710 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/dockerfiles/template_args.py
--rw-r--r--   0        0        0      262 2023-07-06 06:46:41.931629 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/dockerfiles/templates/debian.j2
--rw-r--r--   0        0        0      757 2023-05-29 05:58:54.040070 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2
--rw-r--r--   0        0        0      212 2023-05-16 11:28:43.619589 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/dockerfiles/templates/macros/cache.j2
--rw-r--r--   0        0        0      638 2023-07-06 06:33:50.121875 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2
--rw-r--r--   0        0        0      365 2023-07-06 07:18:49.448528 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/dockerfiles/templates/setup_tungsten.j2
--rw-r--r--   0        0        0     1149 2023-07-10 06:59:55.446738 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2
--rw-r--r--   0        0        0      899 2023-05-12 11:41:21.669195 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py
--rw-r--r--   0        0        0     4387 2023-07-06 14:13:05.914071 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py
--rw-r--r--   0        0        0     1655 2023-07-06 13:41:56.275424 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py
--rw-r--r--   0        0        0     4410 2023-07-06 14:01:27.074963 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py
--rw-r--r--   0        0        0     6699 2023-07-06 14:03:06.017399 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py
--rw-r--r--   0        0        0        0 2023-05-16 13:16:00.016349 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/metadata/__init__.py
--rw-r--r--   0        0        0     4690 2023-07-05 07:18:21.638440 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/metadata/metadata_loader.py
--rw-r--r--   0        0        0     3641 2023-07-10 02:27:14.161709 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/model.py
--rw-r--r--   0        0        0      254 2023-05-16 12:49:36.477427 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/pkg_manager/__init__.py
--rw-r--r--   0        0        0      862 2023-07-06 13:52:01.692543 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py
--rw-r--r--   0        0        0     8301 2023-07-06 14:11:58.842769 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py
--rw-r--r--   0        0        0      916 2023-07-06 12:32:13.585865 tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py
--rw-r--r--   0        0        0       72 2023-05-17 07:08:58.956133 tungstenkit-0.1.2.post8/tungstenkit/_internal/containers/__init__.py
--rw-r--r--   0        0        0     5101 2023-05-29 11:49:56.298526 tungstenkit-0.1.2.post8/tungstenkit/_internal/containers/model.py
--rw-r--r--   0        0        0      132 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post8/tungstenkit/_internal/contexts.py
--rw-r--r--   0        0        0       71 2023-06-05 05:24:44.708624 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/__init__.py
--rw-r--r--   0        0        0     6200 2023-07-10 07:59:58.496310 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/404.html
--rw-r--r--   0        0        0     6231 2023-07-10 07:59:58.472310 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/500.html
--rw-r--r--   0        0        0   691797 2023-07-10 07:59:58.100309 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/347-963bdcebbaf02b7e.js
--rw-r--r--   0        0        0    78459 2023-07-10 07:59:58.096310 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.b1049bda686b7dd5.js
--rw-r--r--   0        0        0   458866 2023-07-10 07:59:58.100309 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js
--rw-r--r--   0        0        0   141052 2023-07-10 07:59:58.096310 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js
--rw-r--r--   0        0        0    89842 2023-07-10 07:59:58.096310 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-74c4d6b2b5c362f3.js
--rw-r--r--   0        0        0     5020 2023-07-10 07:59:58.100309 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/404-1e77c517c165fca8.js
--rw-r--r--   0        0        0     5049 2023-07-10 07:59:58.100309 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/500-8c3654eb5b977ca1.js
--rw-r--r--   0        0        0   130456 2023-07-10 07:59:58.100309 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-0e0952e6981dcf87.js
--rw-r--r--   0        0        0      245 2023-07-10 07:59:58.100309 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_error-8353112a01355ec2.js
--rw-r--r--   0        0        0    26735 2023-07-10 07:59:58.100309 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-7a54d14da4b684a5.js
--rw-r--r--   0        0        0    91460 2023-07-10 07:59:58.096310 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0        0        0     3853 2023-07-10 07:59:58.096310 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-05b74e0eb69d9e61.js
--rw-r--r--   0        0        0      791 2023-07-10 07:59:58.096310 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/css/9e15ad138d9a3a18.css
--rw-r--r--   0        0        0    43645 2023-07-10 07:59:58.100309 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/css/ba142f674ff207f4.css
--rw-r--r--   0        0        0      525 2023-07-10 07:59:58.100309 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/lxMPbv8KZV6yW6yn81HoY/_buildManifest.js
--rw-r--r--   0        0        0       77 2023-07-10 07:59:58.100309 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/lxMPbv8KZV6yW6yn81HoY/_ssgManifest.js
--rw-r--r--   0        0        0   259838 2023-07-10 07:59:58.108310 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/favicon.ico
--rw-r--r--   0        0        0     6244 2023-07-10 07:59:58.468309 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/index.html
--rw-r--r--   0        0        0    61184 2023-07-10 07:59:58.108310 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/logo.svg
--rw-r--r--   0        0        0    27505 2023-07-10 07:59:58.108310 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png
--rw-r--r--   0        0        0    18388 2023-07-10 07:59:58.108310 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png
--rw-r--r--   0        0        0     2753 2023-07-10 07:54:49.523774 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/schemas.py
--rw-r--r--   0        0        0     5175 2023-07-06 10:20:57.794967 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/server.py
--rw-r--r--   0        0        0      104 2023-06-02 07:57:24.533701 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/services/__init__.py
--rw-r--r--   0        0        0     5805 2023-06-05 05:24:44.712623 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/services/file_service.py
--rw-r--r--   0        0        0    12611 2023-07-10 07:38:59.016468 tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/services/prediction_service.py
--rw-r--r--   0        0        0    11504 2023-07-06 20:48:14.411044 tungstenkit-0.1.2.post8/tungstenkit/_internal/io.py
--rw-r--r--   0        0        0     8790 2023-07-06 20:45:16.176235 tungstenkit-0.1.2.post8/tungstenkit/_internal/io_schema.py
--rw-r--r--   0        0        0    11809 2023-07-10 01:23:36.875478 tungstenkit-0.1.2.post8/tungstenkit/_internal/json_store.py
--rw-r--r--   0        0        0     2955 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post8/tungstenkit/_internal/logging.py
--rw-r--r--   0        0        0      144 2023-05-26 07:24:03.204132 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_clients/__init__.py
--rw-r--r--   0        0        0     4359 2023-05-29 11:37:12.601663 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_clients/api_client.py
--rw-r--r--   0        0        0     3960 2023-07-10 07:38:59.016468 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_clients/container_client.py
--rw-r--r--   0        0        0      745 2023-07-10 07:55:04.871827 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_clients/schemas.py
--rw-r--r--   0        0        0     7765 2023-06-07 06:18:29.909695 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_def.py
--rw-r--r--   0        0        0     5102 2023-07-06 06:51:08.438142 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_def_loader.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.680424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/__init__.py
--rw-r--r--   0        0        0       32 2023-05-05 07:02:23.680424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/__main__.py
--rw-r--r--   0        0        0     2895 2023-05-29 10:20:23.323945 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/cli.py
--rw-r--r--   0        0        0     3549 2023-06-08 12:11:43.077003 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/config.py
--rw-r--r--   0        0        0      144 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/enums.py
--rw-r--r--   0        0        0       70 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/event_buses/__init__.py
--rw-r--r--   0        0        0      772 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py
--rw-r--r--   0        0        0      125 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/event_buses/event.py
--rw-r--r--   0        0        0      337 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/event_buses/factory.py
--rw-r--r--   0        0        0      511 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/event_buses/local_event_bus.py
--rw-r--r--   0        0        0       78 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/file_uploaders/__init__.py
--rw-r--r--   0        0        0      209 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/file_uploaders/abstract_file_uploader.py
--rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/file_uploaders/azure_file_uploader.py
--rw-r--r--   0        0        0      602 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/file_uploaders/factory.py
--rw-r--r--   0        0        0      675 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py
--rw-r--r--   0        0        0     2019 2023-07-12 13:23:55.022491 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py
--rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/file_uploaders/s3_file_uploader.py
--rw-r--r--   0        0        0     5521 2023-06-07 06:18:04.645895 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/http_server.py
--rw-r--r--   0        0        0      563 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/ids.py
--rw-r--r--   0        0        0      184 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/input_queues/__init__.py
--rw-r--r--   0        0        0      526 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py
--rw-r--r--   0        0        0      348 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/input_queues/factory.py
--rw-r--r--   0        0        0     3215 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/input_queues/local_input_queue.py
--rw-r--r--   0        0        0      131 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/input_queues/shared.py
--rw-r--r--   0        0        0       69 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/prediction_worker/__init__.py
--rw-r--r--   0        0        0     3785 2023-05-29 05:33:04.832002 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/prediction_worker/executor.py
--rw-r--r--   0        0        0    10183 2023-07-04 14:01:36.565839 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/prediction_worker/subproc.py
--rw-r--r--   0        0        0     9882 2023-07-10 07:38:59.016468 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/prediction_worker/worker.py
--rw-r--r--   0        0        0      248 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/result_caches/__init__.py
--rw-r--r--   0        0        0     1487 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py
--rw-r--r--   0        0        0      396 2023-05-05 07:02:23.684424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/result_caches/factory.py
--rw-r--r--   0        0        0    10441 2023-07-10 07:38:59.016468 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/result_caches/local_result_cache.py
--rw-r--r--   0        0        0      473 2023-07-10 07:39:03.628446 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/result_caches/shared.py
--rw-r--r--   0        0        0     1344 2023-05-26 13:10:09.787054 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/schema.py
--rw-r--r--   0        0        0      503 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/server_exceptions.py
--rw-r--r--   0        0        0      692 2023-07-10 00:18:51.354537 tungstenkit-0.1.2.post8/tungstenkit/_internal/model_store.py
--rw-r--r--   0        0        0      183 2023-05-29 09:28:27.561951 tungstenkit-0.1.2.post8/tungstenkit/_internal/pred_interface/__init__.py
--rw-r--r--   0        0        0     5210 2023-07-10 07:38:59.016468 tungstenkit-0.1.2.post8/tungstenkit/_internal/pred_interface/abstract_interface.py
--rw-r--r--   0        0        0      652 2023-05-29 09:28:27.561951 tungstenkit-0.1.2.post8/tungstenkit/_internal/pred_interface/api_interface.py
--rw-r--r--   0        0        0     1186 2023-05-29 11:48:55.226776 tungstenkit-0.1.2.post8/tungstenkit/_internal/pred_interface/local_interface.py
--rw-r--r--   0        0        0      440 2023-06-02 08:59:18.116896 tungstenkit-0.1.2.post8/tungstenkit/_internal/storables/__init__.py
--rw-r--r--   0        0        0     1283 2023-06-08 12:35:31.307729 tungstenkit-0.1.2.post8/tungstenkit/_internal/storables/avatar_data.py
--rw-r--r--   0        0        0     3208 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post8/tungstenkit/_internal/storables/markdown_data.py
--rw-r--r--   0        0        0     7677 2023-06-07 06:16:15.430768 tungstenkit-0.1.2.post8/tungstenkit/_internal/storables/model_data.py
--rw-r--r--   0        0        0     1095 2023-06-02 08:48:54.116248 tungstenkit-0.1.2.post8/tungstenkit/_internal/storables/model_io_data.py
--rw-r--r--   0        0        0     5534 2023-06-01 05:57:34.935268 tungstenkit-0.1.2.post8/tungstenkit/_internal/storables/pred_example_data.py
--rw-r--r--   0        0        0     4307 2023-06-07 07:01:15.173276 tungstenkit-0.1.2.post8/tungstenkit/_internal/storables/source_file_data.py
--rw-r--r--   0        0        0     9258 2023-05-24 07:42:33.408342 tungstenkit-0.1.2.post8/tungstenkit/_internal/task.py
--rw-r--r--   0        0        0      128 2023-05-26 07:24:22.424035 tungstenkit-0.1.2.post8/tungstenkit/_internal/tungsten_clients/__init__.py
--rw-r--r--   0        0        0    15616 2023-07-11 15:20:57.364515 tungstenkit-0.1.2.post8/tungstenkit/_internal/tungsten_clients/api_client.py
--rw-r--r--   0        0        0    11314 2023-07-10 01:48:48.085029 tungstenkit-0.1.2.post8/tungstenkit/_internal/tungsten_clients/client.py
--rw-r--r--   0        0        0      553 2023-07-10 01:39:23.366905 tungstenkit-0.1.2.post8/tungstenkit/_internal/tungsten_clients/schemas/__init__.py
--rw-r--r--   0        0        0       78 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post8/tungstenkit/_internal/tungsten_clients/schemas/common.py
--rw-r--r--   0        0        0       97 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post8/tungstenkit/_internal/tungsten_clients/schemas/datapoint.py
--rw-r--r--   0        0        0      423 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post8/tungstenkit/_internal/tungsten_clients/schemas/dataset.py
--rw-r--r--   0        0        0      139 2023-06-05 12:56:54.269846 tungstenkit-0.1.2.post8/tungstenkit/_internal/tungsten_clients/schemas/files.py
--rw-r--r--   0        0        0      124 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post8/tungstenkit/_internal/tungsten_clients/schemas/instance.py
--rw-r--r--   0        0        0     2149 2023-07-10 07:01:26.786401 tungstenkit-0.1.2.post8/tungstenkit/_internal/tungsten_clients/schemas/model.py
--rw-r--r--   0        0        0      101 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post8/tungstenkit/_internal/tungsten_clients/schemas/namespace.py
--rw-r--r--   0        0        0      736 2023-07-09 23:37:27.167610 tungstenkit-0.1.2.post8/tungstenkit/_internal/tungsten_clients/schemas/project.py
--rw-r--r--   0        0        0       85 2023-05-05 07:02:23.664425 tungstenkit-0.1.2.post8/tungstenkit/_internal/tungsten_clients/schemas/token.py
--rw-r--r--   0        0        0      240 2023-06-05 07:47:15.889709 tungstenkit-0.1.2.post8/tungstenkit/_internal/tungsten_clients/schemas/user.py
--rw-r--r--   0        0        0        0 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1019 2023-06-05 05:54:41.512092 tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/avatar.py
--rw-r--r--   0        0        0     2996 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/console.py
--rw-r--r--   0        0        0     1587 2023-05-26 08:35:24.498820 tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/context.py
--rw-r--r--   0        0        0    18819 2023-07-10 08:20:25.497586 tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/docker.py
--rw-r--r--   0        0        0     3640 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/file.py
--rw-r--r--   0        0        0      669 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/gpu.py
--rw-r--r--   0        0        0     5354 2023-07-10 06:15:33.654911 tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/imports.py
--rw-r--r--   0        0        0     1721 2023-05-26 05:49:57.704257 tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/json.py
--rw-r--r--   0        0        0     5004 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/markdown.py
--rw-r--r--   0        0        0      551 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/pydantic.py
--rw-r--r--   0        0        0     2387 2023-06-01 15:17:39.232806 tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/regex.py
--rw-r--r--   0        0        0    13290 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/requests.py
--rw-r--r--   0        0        0     2297 2023-06-01 12:30:46.490995 tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/serialize.py
--rw-r--r--   0        0        0      724 2023-05-25 05:44:14.647421 tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/string.py
--rw-r--r--   0        0        0      969 2023-07-06 21:03:05.436744 tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/types.py
--rw-r--r--   0        0        0     3081 2023-06-07 05:33:58.896669 tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/uri.py
--rw-r--r--   0        0        0     6349 2023-07-06 14:01:18.315109 tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/version.py
--rw-r--r--   0        0        0      353 2023-05-05 07:02:23.688424 tungstenkit-0.1.2.post8/tungstenkit/_versions.py
--rw-r--r--   0        0        0     2425 2023-07-09 23:20:04.455331 tungstenkit-0.1.2.post8/tungstenkit/exceptions.py
--rw-r--r--   0        0        0       72 2023-05-29 09:27:58.222097 tungstenkit-0.1.2.post8/tungstenkit/models.py
--rw-r--r--   0        0        0    10565 1970-01-01 00:00:00.000000 tungstenkit-0.1.2.post8/PKG-INFO
+-rw-r--r--   0        0        0    11352 2023-07-13 17:08:18.581431 tungstenkit-0.1.3/LICENSE
+-rw-r--r--   0        0        0     7736 2023-06-14 05:43:16.713685 tungstenkit-0.1.3/README.md
+-rw-r--r--   0        0        0     2868 2023-07-13 18:00:39.580090 tungstenkit-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      424 2023-06-02 07:54:47.474527 tungstenkit-0.1.3/tungstenkit/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.3/tungstenkit/_internal/__init__.py
+-rw-r--r--   0        0        0     7544 2023-07-13 18:31:33.027824 tungstenkit-0.1.3/tungstenkit/_internal/blob_store.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.660425 tungstenkit-0.1.3/tungstenkit/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     2636 2023-07-10 01:51:59.287508 tungstenkit-0.1.3/tungstenkit/_internal/cli/callbacks.py
+-rw-r--r--   0        0        0     2296 2023-05-26 10:03:30.716386 tungstenkit-0.1.3/tungstenkit/_internal/cli/login_command.py
+-rw-r--r--   0        0        0     1414 2023-06-05 05:27:13.011868 tungstenkit-0.1.3/tungstenkit/_internal/cli/main.py
+-rw-r--r--   0        0        0    11227 2023-07-10 08:15:53.146471 tungstenkit-0.1.3/tungstenkit/_internal/cli/model_commands.py
+-rw-r--r--   0        0        0      653 2023-05-05 07:02:23.664425 tungstenkit-0.1.3/tungstenkit/_internal/cli/options.py
+-rw-r--r--   0        0        0     5656 2023-07-11 15:36:54.859197 tungstenkit-0.1.3/tungstenkit/_internal/configs.py
+-rw-r--r--   0        0        0     2615 2023-07-13 18:15:37.115651 tungstenkit-0.1.3/tungstenkit/_internal/constants.py
+-rw-r--r--   0        0        0       58 2023-05-05 07:02:23.660425 tungstenkit-0.1.3/tungstenkit/_internal/containerize/__init__.py
+-rw-r--r--   0        0        0      385 2023-05-05 07:02:23.660425 tungstenkit-0.1.3/tungstenkit/_internal/containerize/base_images/__init__.py
+-rw-r--r--   0        0        0      474 2023-05-12 12:06:44.057340 tungstenkit-0.1.3/tungstenkit/_internal/containerize/base_images/base_image.py
+-rw-r--r--   0        0        0      574 2023-05-05 07:02:23.660425 tungstenkit-0.1.3/tungstenkit/_internal/containerize/base_images/common.py
+-rw-r--r--   0        0        0      238 2023-05-05 07:02:23.660425 tungstenkit-0.1.3/tungstenkit/_internal/containerize/base_images/conda_image.py
+-rw-r--r--   0        0        0     2552 2023-05-11 12:17:37.316053 tungstenkit-0.1.3/tungstenkit/_internal/containerize/base_images/cuda_image.py
+-rw-r--r--   0        0        0      369 2023-05-05 07:02:23.660425 tungstenkit-0.1.3/tungstenkit/_internal/containerize/base_images/custom_image.py
+-rw-r--r--   0        0        0     1622 2023-05-11 12:17:39.436044 tungstenkit-0.1.3/tungstenkit/_internal/containerize/base_images/python_image.py
+-rw-r--r--   0        0        0    12994 2023-07-13 18:49:42.467782 tungstenkit-0.1.3/tungstenkit/_internal/containerize/build_context.py
+-rw-r--r--   0        0        0      172 2023-05-29 05:33:04.832002 tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/__init__.py
+-rw-r--r--   0        0        0     8989 2023-07-13 16:07:48.443313 tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py
+-rw-r--r--   0        0        0      653 2023-07-06 06:52:05.821846 tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py
+-rw-r--r--   0        0        0     1194 2023-07-13 16:07:48.443313 tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/template_args.py
+-rw-r--r--   0        0        0      262 2023-07-06 06:46:41.931629 tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/templates/debian.j2
+-rw-r--r--   0        0        0      757 2023-05-29 05:58:54.040070 tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2
+-rw-r--r--   0        0        0      212 2023-05-16 11:28:43.619589 tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/templates/macros/cache.j2
+-rw-r--r--   0        0        0      638 2023-07-06 06:33:50.121875 tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2
+-rw-r--r--   0        0        0      365 2023-07-06 07:18:49.448528 tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/templates/setup_tungsten.j2
+-rw-r--r--   0        0        0     1149 2023-07-10 06:59:55.446738 tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2
+-rw-r--r--   0        0        0      899 2023-05-12 11:41:21.669195 tungstenkit-0.1.3/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py
+-rw-r--r--   0        0        0     4387 2023-07-06 14:13:05.914071 tungstenkit-0.1.3/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py
+-rw-r--r--   0        0        0     1655 2023-07-06 13:41:56.275424 tungstenkit-0.1.3/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py
+-rw-r--r--   0        0        0     4410 2023-07-06 14:01:27.074963 tungstenkit-0.1.3/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py
+-rw-r--r--   0        0        0     6699 2023-07-06 14:03:06.017399 tungstenkit-0.1.3/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py
+-rw-r--r--   0        0        0        0 2023-05-16 13:16:00.016349 tungstenkit-0.1.3/tungstenkit/_internal/containerize/metadata/__init__.py
+-rw-r--r--   0        0        0     4690 2023-07-05 07:18:21.638440 tungstenkit-0.1.3/tungstenkit/_internal/containerize/metadata/metadata_loader.py
+-rw-r--r--   0        0        0     3641 2023-07-10 02:27:14.161709 tungstenkit-0.1.3/tungstenkit/_internal/containerize/model.py
+-rw-r--r--   0        0        0      254 2023-05-16 12:49:36.477427 tungstenkit-0.1.3/tungstenkit/_internal/containerize/pkg_manager/__init__.py
+-rw-r--r--   0        0        0      862 2023-07-06 13:52:01.692543 tungstenkit-0.1.3/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py
+-rw-r--r--   0        0        0     8301 2023-07-06 14:11:58.842769 tungstenkit-0.1.3/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py
+-rw-r--r--   0        0        0      916 2023-07-06 12:32:13.585865 tungstenkit-0.1.3/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py
+-rw-r--r--   0        0        0       72 2023-05-17 07:08:58.956133 tungstenkit-0.1.3/tungstenkit/_internal/containers/__init__.py
+-rw-r--r--   0        0        0     5101 2023-05-29 11:49:56.298526 tungstenkit-0.1.3/tungstenkit/_internal/containers/model.py
+-rw-r--r--   0        0        0      132 2023-05-05 07:02:23.664425 tungstenkit-0.1.3/tungstenkit/_internal/contexts.py
+-rw-r--r--   0        0        0       71 2023-06-05 05:24:44.708624 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/__init__.py
+-rw-r--r--   0        0        0     6200 2023-07-10 07:59:58.496310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/404.html
+-rw-r--r--   0        0        0     6231 2023-07-10 07:59:58.472310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/500.html
+-rw-r--r--   0        0        0   691797 2023-07-10 07:59:58.100309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/347-963bdcebbaf02b7e.js
+-rw-r--r--   0        0        0    78459 2023-07-10 07:59:58.096310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.b1049bda686b7dd5.js
+-rw-r--r--   0        0        0   458866 2023-07-10 07:59:58.100309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js
+-rw-r--r--   0        0        0   141052 2023-07-10 07:59:58.096310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js
+-rw-r--r--   0        0        0    89842 2023-07-10 07:59:58.096310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-74c4d6b2b5c362f3.js
+-rw-r--r--   0        0        0     5020 2023-07-10 07:59:58.100309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/404-1e77c517c165fca8.js
+-rw-r--r--   0        0        0     5049 2023-07-10 07:59:58.100309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/500-8c3654eb5b977ca1.js
+-rw-r--r--   0        0        0   130456 2023-07-10 07:59:58.100309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-0e0952e6981dcf87.js
+-rw-r--r--   0        0        0      245 2023-07-10 07:59:58.100309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_error-8353112a01355ec2.js
+-rw-r--r--   0        0        0    26735 2023-07-10 07:59:58.100309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-7a54d14da4b684a5.js
+-rw-r--r--   0        0        0    91460 2023-07-10 07:59:58.096310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0        0        0     3853 2023-07-10 07:59:58.096310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-05b74e0eb69d9e61.js
+-rw-r--r--   0        0        0      791 2023-07-10 07:59:58.096310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/css/9e15ad138d9a3a18.css
+-rw-r--r--   0        0        0    43645 2023-07-10 07:59:58.100309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/css/ba142f674ff207f4.css
+-rw-r--r--   0        0        0      525 2023-07-10 07:59:58.100309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/lxMPbv8KZV6yW6yn81HoY/_buildManifest.js
+-rw-r--r--   0        0        0       77 2023-07-10 07:59:58.100309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/lxMPbv8KZV6yW6yn81HoY/_ssgManifest.js
+-rw-r--r--   0        0        0   259838 2023-07-10 07:59:58.108310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/favicon.ico
+-rw-r--r--   0        0        0     6244 2023-07-10 07:59:58.468309 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/index.html
+-rw-r--r--   0        0        0    61184 2023-07-10 07:59:58.108310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/logo.svg
+-rw-r--r--   0        0        0    27505 2023-07-10 07:59:58.108310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png
+-rw-r--r--   0        0        0    18388 2023-07-10 07:59:58.108310 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png
+-rw-r--r--   0        0        0     2753 2023-07-10 07:54:49.523774 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/schemas.py
+-rw-r--r--   0        0        0     5175 2023-07-06 10:20:57.794967 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/server.py
+-rw-r--r--   0        0        0      104 2023-06-02 07:57:24.533701 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/services/__init__.py
+-rw-r--r--   0        0        0     5805 2023-06-05 05:24:44.712623 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/services/file_service.py
+-rw-r--r--   0        0        0    12611 2023-07-10 07:38:59.016468 tungstenkit-0.1.3/tungstenkit/_internal/demo_server/services/prediction_service.py
+-rw-r--r--   0        0        0    11504 2023-07-06 20:48:14.411044 tungstenkit-0.1.3/tungstenkit/_internal/io.py
+-rw-r--r--   0        0        0     8790 2023-07-06 20:45:16.176235 tungstenkit-0.1.3/tungstenkit/_internal/io_schema.py
+-rw-r--r--   0        0        0    12599 2023-07-13 16:07:48.435312 tungstenkit-0.1.3/tungstenkit/_internal/json_store.py
+-rw-r--r--   0        0        0     2955 2023-05-05 07:02:23.664425 tungstenkit-0.1.3/tungstenkit/_internal/logging.py
+-rw-r--r--   0        0        0      144 2023-05-26 07:24:03.204132 tungstenkit-0.1.3/tungstenkit/_internal/model_clients/__init__.py
+-rw-r--r--   0        0        0     4359 2023-05-29 11:37:12.601663 tungstenkit-0.1.3/tungstenkit/_internal/model_clients/api_client.py
+-rw-r--r--   0        0        0     3960 2023-07-10 07:38:59.016468 tungstenkit-0.1.3/tungstenkit/_internal/model_clients/container_client.py
+-rw-r--r--   0        0        0      745 2023-07-10 07:55:04.871827 tungstenkit-0.1.3/tungstenkit/_internal/model_clients/schemas.py
+-rw-r--r--   0        0        0     7765 2023-06-07 06:18:29.909695 tungstenkit-0.1.3/tungstenkit/_internal/model_def.py
+-rw-r--r--   0        0        0     5102 2023-07-06 06:51:08.438142 tungstenkit-0.1.3/tungstenkit/_internal/model_def_loader.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.680424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-05 07:02:23.680424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/__main__.py
+-rw-r--r--   0        0        0     2895 2023-05-29 10:20:23.323945 tungstenkit-0.1.3/tungstenkit/_internal/model_server/cli.py
+-rw-r--r--   0        0        0     3549 2023-06-08 12:11:43.077003 tungstenkit-0.1.3/tungstenkit/_internal/model_server/config.py
+-rw-r--r--   0        0        0      144 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/enums.py
+-rw-r--r--   0        0        0       70 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/event_buses/__init__.py
+-rw-r--r--   0        0        0      772 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py
+-rw-r--r--   0        0        0      125 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/event_buses/event.py
+-rw-r--r--   0        0        0      337 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/event_buses/factory.py
+-rw-r--r--   0        0        0      511 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/event_buses/local_event_bus.py
+-rw-r--r--   0        0        0       78 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/file_uploaders/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/file_uploaders/abstract_file_uploader.py
+-rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/file_uploaders/azure_file_uploader.py
+-rw-r--r--   0        0        0      602 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/file_uploaders/factory.py
+-rw-r--r--   0        0        0      675 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py
+-rw-r--r--   0        0        0     2019 2023-07-13 16:07:48.447312 tungstenkit-0.1.3/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py
+-rw-r--r--   0        0        0        7 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/file_uploaders/s3_file_uploader.py
+-rw-r--r--   0        0        0     5521 2023-06-07 06:18:04.645895 tungstenkit-0.1.3/tungstenkit/_internal/model_server/http_server.py
+-rw-r--r--   0        0        0      563 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/ids.py
+-rw-r--r--   0        0        0      184 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/input_queues/__init__.py
+-rw-r--r--   0        0        0      526 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py
+-rw-r--r--   0        0        0      348 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/input_queues/factory.py
+-rw-r--r--   0        0        0     3215 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/input_queues/local_input_queue.py
+-rw-r--r--   0        0        0      131 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/input_queues/shared.py
+-rw-r--r--   0        0        0       69 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/prediction_worker/__init__.py
+-rw-r--r--   0        0        0     3785 2023-05-29 05:33:04.832002 tungstenkit-0.1.3/tungstenkit/_internal/model_server/prediction_worker/executor.py
+-rw-r--r--   0        0        0    10183 2023-07-04 14:01:36.565839 tungstenkit-0.1.3/tungstenkit/_internal/model_server/prediction_worker/subproc.py
+-rw-r--r--   0        0        0     9882 2023-07-10 07:38:59.016468 tungstenkit-0.1.3/tungstenkit/_internal/model_server/prediction_worker/worker.py
+-rw-r--r--   0        0        0      248 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/result_caches/__init__.py
+-rw-r--r--   0        0        0     1487 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py
+-rw-r--r--   0        0        0      396 2023-05-05 07:02:23.684424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/result_caches/factory.py
+-rw-r--r--   0        0        0    10441 2023-07-10 07:38:59.016468 tungstenkit-0.1.3/tungstenkit/_internal/model_server/result_caches/local_result_cache.py
+-rw-r--r--   0        0        0      473 2023-07-10 07:39:03.628446 tungstenkit-0.1.3/tungstenkit/_internal/model_server/result_caches/shared.py
+-rw-r--r--   0        0        0     1344 2023-05-26 13:10:09.787054 tungstenkit-0.1.3/tungstenkit/_internal/model_server/schema.py
+-rw-r--r--   0        0        0      503 2023-05-05 07:02:23.688424 tungstenkit-0.1.3/tungstenkit/_internal/model_server/server_exceptions.py
+-rw-r--r--   0        0        0      682 2023-07-13 16:07:48.439313 tungstenkit-0.1.3/tungstenkit/_internal/model_store.py
+-rw-r--r--   0        0        0      183 2023-05-29 09:28:27.561951 tungstenkit-0.1.3/tungstenkit/_internal/pred_interface/__init__.py
+-rw-r--r--   0        0        0     5210 2023-07-10 07:38:59.016468 tungstenkit-0.1.3/tungstenkit/_internal/pred_interface/abstract_interface.py
+-rw-r--r--   0        0        0      652 2023-05-29 09:28:27.561951 tungstenkit-0.1.3/tungstenkit/_internal/pred_interface/api_interface.py
+-rw-r--r--   0        0        0     1186 2023-05-29 11:48:55.226776 tungstenkit-0.1.3/tungstenkit/_internal/pred_interface/local_interface.py
+-rw-r--r--   0        0        0      440 2023-06-02 08:59:18.116896 tungstenkit-0.1.3/tungstenkit/_internal/storables/__init__.py
+-rw-r--r--   0        0        0     1272 2023-07-13 18:45:11.437138 tungstenkit-0.1.3/tungstenkit/_internal/storables/avatar_data.py
+-rw-r--r--   0        0        0     3208 2023-06-07 05:33:58.896669 tungstenkit-0.1.3/tungstenkit/_internal/storables/markdown_data.py
+-rw-r--r--   0        0        0     7495 2023-07-13 16:07:48.439313 tungstenkit-0.1.3/tungstenkit/_internal/storables/model_data.py
+-rw-r--r--   0        0        0     1095 2023-06-02 08:48:54.116248 tungstenkit-0.1.3/tungstenkit/_internal/storables/model_io_data.py
+-rw-r--r--   0        0        0     5534 2023-06-01 05:57:34.935268 tungstenkit-0.1.3/tungstenkit/_internal/storables/pred_example_data.py
+-rw-r--r--   0        0        0     4414 2023-07-13 18:33:59.595617 tungstenkit-0.1.3/tungstenkit/_internal/storables/source_file_data.py
+-rw-r--r--   0        0        0     9258 2023-05-24 07:42:33.408342 tungstenkit-0.1.3/tungstenkit/_internal/task.py
+-rw-r--r--   0        0        0      128 2023-05-26 07:24:22.424035 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/__init__.py
+-rw-r--r--   0        0        0    15616 2023-07-11 15:20:57.364515 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/api_client.py
+-rw-r--r--   0        0        0    11314 2023-07-10 01:48:48.085029 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/client.py
+-rw-r--r--   0        0        0      553 2023-07-10 01:39:23.366905 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-05 07:02:23.664425 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/common.py
+-rw-r--r--   0        0        0       97 2023-05-05 07:02:23.664425 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/datapoint.py
+-rw-r--r--   0        0        0      423 2023-05-05 07:02:23.664425 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/dataset.py
+-rw-r--r--   0        0        0      139 2023-06-05 12:56:54.269846 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/files.py
+-rw-r--r--   0        0        0      124 2023-05-05 07:02:23.664425 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/instance.py
+-rw-r--r--   0        0        0     2149 2023-07-10 07:01:26.786401 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/model.py
+-rw-r--r--   0        0        0      101 2023-05-05 07:02:23.664425 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/namespace.py
+-rw-r--r--   0        0        0      736 2023-07-09 23:37:27.167610 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/project.py
+-rw-r--r--   0        0        0       85 2023-05-05 07:02:23.664425 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/token.py
+-rw-r--r--   0        0        0      240 2023-06-05 07:47:15.889709 tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/user.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:02:23.688424 tungstenkit-0.1.3/tungstenkit/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1019 2023-06-05 05:54:41.512092 tungstenkit-0.1.3/tungstenkit/_internal/utils/avatar.py
+-rw-r--r--   0        0        0     2996 2023-05-05 07:02:23.688424 tungstenkit-0.1.3/tungstenkit/_internal/utils/console.py
+-rw-r--r--   0        0        0     1587 2023-05-26 08:35:24.498820 tungstenkit-0.1.3/tungstenkit/_internal/utils/context.py
+-rw-r--r--   0        0        0    18819 2023-07-10 08:20:25.497586 tungstenkit-0.1.3/tungstenkit/_internal/utils/docker.py
+-rw-r--r--   0        0        0     3640 2023-06-07 05:33:58.896669 tungstenkit-0.1.3/tungstenkit/_internal/utils/file.py
+-rw-r--r--   0        0        0      669 2023-06-07 05:33:58.896669 tungstenkit-0.1.3/tungstenkit/_internal/utils/gpu.py
+-rw-r--r--   0        0        0     5354 2023-07-10 06:15:33.654911 tungstenkit-0.1.3/tungstenkit/_internal/utils/imports.py
+-rw-r--r--   0        0        0     1721 2023-05-26 05:49:57.704257 tungstenkit-0.1.3/tungstenkit/_internal/utils/json.py
+-rw-r--r--   0        0        0     5004 2023-06-07 05:33:58.896669 tungstenkit-0.1.3/tungstenkit/_internal/utils/markdown.py
+-rw-r--r--   0        0        0      551 2023-05-05 07:02:23.688424 tungstenkit-0.1.3/tungstenkit/_internal/utils/pydantic.py
+-rw-r--r--   0        0        0     2387 2023-06-01 15:17:39.232806 tungstenkit-0.1.3/tungstenkit/_internal/utils/regex.py
+-rw-r--r--   0        0        0    13290 2023-06-07 05:33:58.896669 tungstenkit-0.1.3/tungstenkit/_internal/utils/requests.py
+-rw-r--r--   0        0        0     2297 2023-06-01 12:30:46.490995 tungstenkit-0.1.3/tungstenkit/_internal/utils/serialize.py
+-rw-r--r--   0        0        0      724 2023-05-25 05:44:14.647421 tungstenkit-0.1.3/tungstenkit/_internal/utils/string.py
+-rw-r--r--   0        0        0      969 2023-07-06 21:03:05.436744 tungstenkit-0.1.3/tungstenkit/_internal/utils/types.py
+-rw-r--r--   0        0        0     3081 2023-06-07 05:33:58.896669 tungstenkit-0.1.3/tungstenkit/_internal/utils/uri.py
+-rw-r--r--   0        0        0     6349 2023-07-06 14:01:18.315109 tungstenkit-0.1.3/tungstenkit/_internal/utils/version.py
+-rw-r--r--   0        0        0      353 2023-05-05 07:02:23.688424 tungstenkit-0.1.3/tungstenkit/_versions.py
+-rw-r--r--   0        0        0     2425 2023-07-09 23:20:04.455331 tungstenkit-0.1.3/tungstenkit/exceptions.py
+-rw-r--r--   0        0        0       72 2023-05-29 09:27:58.222097 tungstenkit-0.1.3/tungstenkit/models.py
+-rw-r--r--   0        0        0    10564 1970-01-01 00:00:00.000000 tungstenkit-0.1.3/PKG-INFO
```

### Comparing `tungstenkit-0.1.2.post8/LICENSE` & `tungstenkit-0.1.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2023 Tungsten AI Inc.
+   Copyright 2023 Tungsten Contributors.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `tungstenkit-0.1.2.post8/README.md` & `tungstenkit-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/pyproject.toml` & `tungstenkit-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tungstenkit"
-version = "0.1.2.post8"
+version = "0.1.3"
 description = "ML container made simple"
 authors = ["Tungsten Contributors <foss@tungsten-ai.com>"]
 homepage = "https://github.com/tungsten-ai/tungstenkit"
 readme = ["README.md"]
 packages = [{include = "tungstenkit"}]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -65,16 +65,16 @@
 fasteners = "^0.18"
 furl = "^2.1.3"
 requests-toolbelt = "^0.10.1"
 binaryornot = "^0.4.4"
 python-multipart = "^0.0.6"
 urllib3 = "^1.26"
 dill = "^0.3.6"
-appdirs = "^1.4.4"
 pynvml = "^11.5.0"
+platformdirs = "^3.8.1"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.1"
 black = "^22.3.0"
 isort = "^4.3.21"
 autoflake = "^1.3.1"
 flake8 = "^3.7.9"
```

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/blob_store.py` & `tungstenkit-0.1.3/tungstenkit/_internal/blob_store.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,21 +14,28 @@
 
 from tungstenkit._internal.constants import DATA_DIR, LOCK_DIR
 from tungstenkit._internal.utils.file import list_dirs, list_files
 
 BlobStorableType = t.TypeVar("BlobStorableType", bound="BlobStorable")
 BlobContainerType = t.TypeVar("BlobContainerType")
 FileBlobCreatePolicy: TypeAlias = Literal["copy", "rename"]
+
+BLOBS_DATA_DIR = DATA_DIR / "blobs" / "data"
+BLOBS_LOCK_PATH = LOCK_DIR / "blobs.lock"
 BUF_SIZE_FOR_HASHING = 1048576  # 1MB
 
 
 @attrs.frozen(kw_only=True, order=True)
 class Blob:
     digest: str
-    file_path: Path = attrs.field(eq=False, order=False)
+    file_name: str
+
+    @property
+    def file_path(self):
+        return _build_blob_dir_path(self.digest) / self.file_name
 
     def remove(self):
         shutil.rmtree(self.file_path.parent)
 
 
 class BlobStorable(abc.ABC, t.Generic[BlobContainerType]):
     @abc.abstractmethod
@@ -40,36 +47,30 @@
     @classmethod
     @abc.abstractmethod
     def load_blobs(cls: t.Type[BlobStorableType], data: BlobContainerType) -> BlobStorableType:
         pass
 
 
 class BlobStore:
-    _base_dir: t.ClassVar[Path] = DATA_DIR / "blobs"
-    _lock_path: t.ClassVar[Path] = LOCK_DIR / "blobs.lock"
-
-    __data_dir: Path
-
     def __init__(self) -> None:
-        self.__data_dir = self._base_dir / "data"
-        self.__data_dir.mkdir(parents=True, exist_ok=True)
-        self._lock = InterProcessReaderWriterLock(path=self._lock_path)
+        BLOBS_DATA_DIR.mkdir(parents=True, exist_ok=True)
+        self._lock = InterProcessReaderWriterLock(path=BLOBS_LOCK_PATH)
 
     def list_digests(self) -> t.List[str]:
-        return [d.name for base_dir in list_dirs(self.__data_dir) for d in list_dirs(base_dir)]
+        return [d.name for base_dir in list_dirs(BLOBS_DATA_DIR) for d in list_dirs(base_dir)]
 
     def get_by_digest(self, digest: str) -> Blob:
-        blob_dir = self._build_blob_dir_path(digest)
+        blob_dir = _build_blob_dir_path(digest)
         if not blob_dir.exists():
             raise KeyError(f"Blob not found: {digest}")
 
-        return Blob(digest=digest, file_path=list_files(blob_dir)[0])
+        return Blob(digest=digest, file_name=list_files(blob_dir)[0].name)
 
     def check_if_contained(self, digest: str) -> bool:
-        return self._build_blob_dir_path(digest).exists()
+        return _build_blob_dir_path(digest).exists()
 
     def add_multiple_by_writing(self, *args: t.Union[Path, t.Tuple[bytes, str]]) -> t.List[Blob]:
         """
         Add blobs to the blob cache
 
         :param args: a sequence of paths and named bytes.
             Each element of list can be either a ``pathlib.Path`` object or
@@ -103,24 +104,24 @@
         try:
             with ThreadPoolExecutor(max_workers=min(8, len(args))) as executor:
                 for idx, digest in executor.map(_hash, range(len(args)), args):
                     idx_to_digest_mapping[idx] = digest
 
                 list_blob_dir, list_file_name, list_path_or_bytes = [], [], []
                 for digest, (file_name, path_or_bytes) in to_be_added.items():
-                    list_blob_dir.append(self._build_blob_dir_path(digest))
+                    list_blob_dir.append(_build_blob_dir_path(digest))
                     list_file_name.append(file_name)
                     list_path_or_bytes.append(path_or_bytes)
                 for _ in executor.map(
                     _write_blob, list_blob_dir, list_file_name, list_path_or_bytes
                 ):
                     pass
         except BaseException as e:
             for digest in to_be_added.keys():
-                d = self._build_blob_dir_path(digest)
+                d = _build_blob_dir_path(digest)
                 if d.exists():
                     shutil.rmtree(d)
 
             raise e
 
         return [
             self.get_by_digest(idx_to_digest_mapping[idx]) for idx in sorted(idx_to_digest_mapping)
@@ -130,18 +131,18 @@
         return self.add_multiple_by_writing(path_or_named_bytes)[0]
 
     def add_by_renaming(self, path: Path) -> Blob:
         path = path.resolve()
         digest = _hash_file(path)
         if self.check_if_contained(digest):
             return self.get_by_digest(digest)
-        blob_dir = self._build_blob_dir_path(digest)
+        blob_dir = _build_blob_dir_path(digest)
         blob_dir.mkdir(parents=True)
         os.replace(path.resolve(), blob_dir / path.name)
-        return Blob(digest=digest, file_path=path)
+        return Blob(digest=digest, file_name=path.name)
 
     def delete_unused(self, used: t.Set[Blob]) -> None:
         with self._lock.write_lock():
             self._sanitize()
             digests = self.list_digests()
             to_be_removed = []
             for digest in digests:
@@ -160,24 +161,24 @@
         try:
             self._lock.acquire_read_lock()
             yield
         finally:
             self._lock.release_read_lock()
 
     def _build_blob_dir_path(self, digest: str) -> Path:
-        return self.__data_dir / digest[:2] / digest
+        return BLOBS_DATA_DIR / digest[:2] / digest
 
     def _sanitize(self) -> None:
         """
         Remove blobs whose directory is corrupted.
         """
         digests = self.list_digests()
         to_be_removed = []
         for digest in digests:
-            directory = self._build_blob_dir_path(digest)
+            directory = _build_blob_dir_path(digest)
             if len(list_files(directory)) == 0:
                 to_be_removed.append(str(directory))
         if to_be_removed:
             with ThreadPoolExecutor(max_workers=8) as executor:
                 executor.map(shutil.rmtree, to_be_removed)
 
 
@@ -209,7 +210,11 @@
             tmp_file_path.write_bytes(path_or_bytes)
         else:
             shutil.copyfile(path_or_bytes.resolve(), tmp_file_path)
         os.replace(tmp_file_path, blob_file_path)
     except BaseException as e:
         shutil.rmtree(str(blob_dir))
         raise e
+
+
+def _build_blob_dir_path(digest: str) -> Path:
+    return BLOBS_DATA_DIR / digest[:2] / digest
```

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/cli/callbacks.py` & `tungstenkit-0.1.3/tungstenkit/_internal/cli/callbacks.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/cli/login_command.py` & `tungstenkit-0.1.3/tungstenkit/_internal/cli/login_command.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/cli/main.py` & `tungstenkit-0.1.3/tungstenkit/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/cli/model_commands.py` & `tungstenkit-0.1.3/tungstenkit/_internal/cli/model_commands.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/cli/options.py` & `tungstenkit-0.1.3/tungstenkit/_internal/cli/options.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/configs.py` & `tungstenkit-0.1.3/tungstenkit/_internal/configs.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/constants.py` & `tungstenkit-0.1.3/tungstenkit/_internal/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import re
 import tempfile
 from pathlib import Path, PurePosixPath
 
-from appdirs import AppDirs
 from packaging.version import Version
+from platformdirs import user_config_path, user_data_path
 
-appdirs = AppDirs(appname="tungstenkit", appauthor="tungsten")
+import tungstenkit
 
 
 def default_model_repo() -> str:
     wd_name = (
         re.sub(r"[^A-Za-z0-9_-]+", "", Path(os.getcwd()).resolve().parts[-1])
         .lower()
         .replace("_", "-")
@@ -31,21 +31,31 @@
    ██║   ╚██████╔╝██║ ╚████║╚██████╔╝███████║   ██║   ███████╗██║ ╚████║
    ╚═╝    ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝ ╚══════╝   ╚═╝   ╚══════╝╚═╝  ╚═══╝
                                                                         
 
 """
 
 DEFAULT_MODEL_MODULE = "tungsten_model"
-DEFAULT_TUNGSTEN_SERVER_URL = "https://api.tungsten-ai.com"
+DEFAULT_TUNGSTEN_SERVER_URL = "https://api.tungsten.run"
+DEFAULT_GPU_MEM_GB = 16
 
-DATA_DIR = Path(os.getenv("TUNGSTEN_DATA_DIR", Path(appdirs.user_data_dir)))
+DATA_DIR = Path(
+    os.getenv(
+        "TUNGSTEN_HOME", Path(user_data_path(tungstenkit.__name__, appauthor=False, roaming=True))
+    )
+)
 DATA_DIR = DATA_DIR.resolve()
 DATA_DIR.mkdir(parents=True, exist_ok=True)
 
-CONFIG_DIR = Path(os.getenv("TUNGSTEN_CONFIG_DIR", Path(appdirs.user_config_dir)))
+CONFIG_DIR = Path(
+    os.getenv(
+        "TUNGSTEN_CONFIG_DIR",
+        Path(user_config_path(tungstenkit.__name__, appauthor=False, roaming=True)),
+    )
+)
 CONFIG_DIR = CONFIG_DIR.resolve()
 CONFIG_DIR.mkdir(parents=True, exist_ok=True)
 
 LOCK_DIR = Path(tempfile.gettempdir()) / "tungsten" / "locks"
 LOCK_DIR.mkdir(parents=True, exist_ok=True)
 
 TUNGSTEN_DIR_IN_CONTAINER = PurePosixPath("/etc/tungsten")
```

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/base_images/common.py` & `tungstenkit-0.1.3/tungstenkit/_internal/containerize/base_images/common.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/base_images/cuda_image.py` & `tungstenkit-0.1.3/tungstenkit/_internal/containerize/base_images/cuda_image.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/base_images/python_image.py` & `tungstenkit-0.1.3/tungstenkit/_internal/containerize/base_images/python_image.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/build_context.py` & `tungstenkit-0.1.3/tungstenkit/_internal/containerize/build_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from uuid import uuid4
 
 import attrs
 from filelock import FileLock
 from pathspec import PathSpec
 from rich.progress import Progress, TextColumn
 
-import tungstenkit
 from tungstenkit import exceptions
 from tungstenkit._internal import storables
 from tungstenkit._internal.configs import BuildConfig
 from tungstenkit._internal.constants import TUNGSTEN_DIR_IN_CONTAINER
 from tungstenkit._internal.logging import log_debug, log_info, log_warning
 from tungstenkit._internal.utils.context import hide_traceback
 from tungstenkit._internal.utils.file import (
```

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py` & `tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/base_dockerfile.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py` & `tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/model_dockerfile.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/dockerfiles/template_args.py` & `tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/template_args.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2` & `tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/templates/install_python.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2` & `tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/templates/setup_base_image.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2` & `tungstenkit-0.1.3/tungstenkit/_internal/containerize/dockerfiles/templates/setup_user.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py` & `tungstenkit-0.1.3/tungstenkit/_internal/containerize/gpu_pkg_collections/__init__.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py` & `tungstenkit-0.1.3/tungstenkit/_internal/containerize/gpu_pkg_collections/base_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py` & `tungstenkit-0.1.3/tungstenkit/_internal/containerize/gpu_pkg_collections/common.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py` & `tungstenkit-0.1.3/tungstenkit/_internal/containerize/gpu_pkg_collections/tf_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py` & `tungstenkit-0.1.3/tungstenkit/_internal/containerize/gpu_pkg_collections/torch_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/metadata/metadata_loader.py` & `tungstenkit-0.1.3/tungstenkit/_internal/containerize/metadata/metadata_loader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/model.py` & `tungstenkit-0.1.3/tungstenkit/_internal/containerize/model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py` & `tungstenkit-0.1.3/tungstenkit/_internal/containerize/pkg_manager/pip_requirement.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py` & `tungstenkit-0.1.3/tungstenkit/_internal/containerize/pkg_manager/pkg_manager.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py` & `tungstenkit-0.1.3/tungstenkit/_internal/containerize/pkg_manager/requirements_txt.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/containers/model.py` & `tungstenkit-0.1.3/tungstenkit/_internal/containers/model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/404.html` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/404.html`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/500.html` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/500.html`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/347-963bdcebbaf02b7e.js` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/347-963bdcebbaf02b7e.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.b1049bda686b7dd5.js` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/925e0f50.b1049bda686b7dd5.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/d6e1aeb5-ab9bd27fd3f7ec69.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/framework-2c79e2a64abdb08b.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-74c4d6b2b5c362f3.js` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/main-74c4d6b2b5c362f3.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/404-1e77c517c165fca8.js` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/404-1e77c517c165fca8.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/500-8c3654eb5b977ca1.js` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/500-8c3654eb5b977ca1.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-0e0952e6981dcf87.js` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/_app-0e0952e6981dcf87.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-7a54d14da4b684a5.js` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/pages/index-7a54d14da4b684a5.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-05b74e0eb69d9e61.js` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/chunks/webpack-05b74e0eb69d9e61.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/css/9e15ad138d9a3a18.css` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/css/9e15ad138d9a3a18.css`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/css/ba142f674ff207f4.css` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/css/ba142f674ff207f4.css`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/_next/static/lxMPbv8KZV6yW6yn81HoY/_buildManifest.js` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/_next/static/lxMPbv8KZV6yW6yn81HoY/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/favicon.ico` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/index.html` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/index.html`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/logo.svg` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/logo.svg`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/tungstenWithoutText.png`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/frontend/tungsten_greyed_out_logo.png`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/schemas.py` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/schemas.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/server.py` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/server.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/services/file_service.py` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/services/file_service.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/demo_server/services/prediction_service.py` & `tungstenkit-0.1.3/tungstenkit/_internal/demo_server/services/prediction_service.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/io.py` & `tungstenkit-0.1.3/tungstenkit/_internal/io.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/io_schema.py` & `tungstenkit-0.1.3/tungstenkit/_internal/io_schema.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/json_store.py` & `tungstenkit-0.1.3/tungstenkit/_internal/json_store.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,26 +8,29 @@
 import cattrs
 from filelock import FileLock
 
 from tungstenkit import exceptions
 from tungstenkit._internal.blob_store import Blob, BlobStorable, BlobStore, FileBlobCreatePolicy
 from tungstenkit._internal.constants import DATA_DIR, LOCK_DIR
 from tungstenkit._internal.logging import log_debug
+from tungstenkit._internal.utils.docker import parse_docker_image_name
 from tungstenkit._internal.utils.file import write_safely
 from tungstenkit._internal.utils.serialize import convert_attrs_to_json, load_attrs_from_json
 from tungstenkit._internal.utils.string import camel_to_snake
 from tungstenkit._internal.utils.types import get_superclass_type_args
 
 StorableType = t.TypeVar("StorableType", bound="JSONStorable")
 ItemType = t.TypeVar("ItemType", bound="JSONItem")
 CollectionType = t.TypeVar("CollectionType", bound="_JSONCollection")
 
+DEFAULT_TAG = "latest"
+
 
 class JSONStorable(BlobStorable[ItemType]):
-    _store: "JSONCollection[ItemType]"
+    _store: "JSONStore[ItemType]"
 
     def save(self, file_blob_create_policy: FileBlobCreatePolicy = "copy") -> ItemType:
         blob_store = BlobStore()
         with blob_store.prevent_deletion():
             data = self.save_blobs(blob_store, file_blob_create_policy)
             store = self._get_store()
             store.add(data)
@@ -38,76 +41,70 @@
         data = cls._get_store().get(name)
         return cls.load_blobs(data)
 
     @staticmethod
     def generate_id() -> str:
         return uuid4().hex
 
+    @staticmethod
+    def parse_name(name: str) -> t.Tuple[str, t.Optional[str]]:
+        return parse_docker_image_name(name)
+
     @classmethod
-    def _get_store(cls: t.Type[StorableType]) -> "JSONCollection[ItemType]":
+    def _get_store(cls: t.Type[StorableType]) -> "JSONStore[ItemType]":
         if not hasattr(cls, "_store"):
             args = get_superclass_type_args(cls, JSONStorable)
             if len(args) == 0:
                 raise RuntimeError("Type argument is not set")
             data_cls: t.Type[ItemType] = args[0]
-            cls._store = JSONCollection[data_cls](data_cls)  # type: ignore
+            cls._store = JSONStore[data_cls](data_cls)  # type: ignore
         return cls._store
 
 
 class JSONItem(abc.ABC):
     @property
     @abc.abstractmethod
     def id(self) -> str:
         pass
 
     @property
     @abc.abstractmethod
-    def hash(self) -> str:
-        pass
-
-    @property
-    @abc.abstractmethod
     def repo_name(self) -> str:
         pass
 
     @property
     @abc.abstractmethod
     def tag(self) -> str:
         pass
 
     @property
-    @abc.abstractmethod
-    def blobs(self) -> t.Set[Blob]:
-        pass
-
-    @property
     def name(self) -> str:
         return self.repo_name + ":" + self.tag
 
     @property
     @abc.abstractmethod
-    def created_at(self) -> datetime:
+    def blobs(self) -> t.Set[Blob]:
         pass
 
+    @property
     @abc.abstractmethod
-    def cleanup(self):
+    def created_at(self) -> datetime:
         pass
 
-    @staticmethod
     @abc.abstractmethod
-    def parse_name(name: str) -> t.Tuple[str, str]:
+    def cleanup(self):
         pass
 
     @classmethod
     def get_typename(cls) -> str:
         return camel_to_snake(cls.__name__)
 
 
 # TODO encapsulate JSONCollection
-class JSONCollection(t.Generic[ItemType]):
+class JSONStore(t.Generic[ItemType]):
     _item_type: t.Type[ItemType]
     _collection_type: "t.Type[_JSONCollection[ItemType]]"
 
     def __init__(self, item_type: t.Type[ItemType]):
         self._item_type = item_type
         self._collection_type = _JSONCollection[item_type]  # type: ignore
         self.base_dir.mkdir(parents=True, exist_ok=True)
@@ -126,73 +123,94 @@
     def collection_path(self) -> Path:
         return self.base_dir / "collection.json"
 
     def add(self, item: ItemType):
         """Add to the colleciton and prune dangling items"""
         with self._filelock:
             col = self._collection_type.load(self._item_type, self.collection_path)
-            col.add(item)
+            col.add_item(item)
             self._gc(col)
             col.save(self.collection_path)
 
-    # def get_latest_tag(self, repo: str):
+    def tag(self, src_name: str, dest_name: str) -> str:
+        src_repo, _src_tag = JSONStorable.parse_name(src_name)
+        src_tag = _src_tag if _src_tag else DEFAULT_TAG
+
+        dest_repo, _dest_tag = JSONStorable.parse_name(dest_name)
+        dest_tag = _dest_tag if _dest_tag else src_tag
 
-    def tag(self, src_name: str, dest_name: str):
-        src_repo, src_tag = self._item_type.parse_name(src_name)
-        dest_repo, dest_tag = self._item_type.parse_name(dest_name)
         with self._filelock:
             col = self._collection_type.load(self._item_type, self.collection_path)
-            src = col.get_by_tag(src_repo, src_tag)
+            src = col.get_item_by_tag(src_repo, src_tag)
             if src is None:
-                self._raise_not_found_by_name(src_name)
-            col.tag(dest_repo, dest_tag, src.id)  # type: ignore
+                raise exceptions.NotFound(self._build_not_found_err_msg(src_name))
+            col.tag_item(dest_repo, dest_tag, src.id)
             col.save(self.collection_path)
 
+        return dest_repo + ":" + dest_tag
+
     def update(self, item: ItemType) -> None:
         with self._filelock:
             col = self._collection_type.load(self._item_type, self.collection_path)
-            orig = col.get_by_id(item.id)
+            orig = col.get_item_by_id(item.id)
             if orig is None:
-                self._raise_not_found_by_id(item.id)
-            col.update(item)
+                raise exceptions.NotFound(self._build_not_found_err_msg(item.name))
+            col.update_item(item)
             col.save(self.collection_path)
 
     def get(self, name: str) -> ItemType:
-        repo, tag = self._item_type.parse_name(name)
+        repo, _tag = JSONStorable.parse_name(name)
+
         with self._filelock:
             col = self._collection_type.load(self._item_type, self.collection_path)
 
-        item = col.get_by_tag(repo, tag)
+        if not col.check_repo_exsistence(repo):
+            raise exceptions.NotFound(self._build_not_found_err_msg(name))
+
+        if _tag is None:
+            if col.check_tag_exsistence_in_repo(repo, DEFAULT_TAG):
+                tag = DEFAULT_TAG
+            else:
+                _tag = col.get_latest_tag_in_repo(repo_name=name)
+                if _tag is None:
+                    raise exceptions.NotFound(self._build_not_found_err_msg(name))
+                else:
+                    tag = _tag
+        else:
+            tag = _tag
+
+        item = col.get_item_by_tag(repo, tag)
         if item is None:
-            self._raise_not_found_by_name(repo + ":" + tag)
+            self._build_not_found_err_msg(name)
         attrs_kwargs = {k: v for k, v in attrs.asdict(item, recurse=False).items() if k != "tag"}
         return self._item_type(tag=tag, **attrs_kwargs)  # type: ignore
 
     # TODO Take fields argument
     def list(self) -> t.List[ItemType]:
         ret: t.List[ItemType] = []
         with self._filelock:
             col = self._collection_type.load(self._item_type, self.collection_path)
 
-        items = col.list()
+        items = col.list_items()
         for _, tag, item in items:
             attrs_kwargs = {
                 k: v for k, v in attrs.asdict(item, recurse=False).items() if k != "tag"
             }
             ret.append(self._item_type(tag=tag, **attrs_kwargs))  # type: ignore
 
         return ret
 
     def delete(self, name: str):
-        repo, tag = self._item_type.parse_name(name)
+        repo, _tag = JSONStorable.parse_name(name)
+        tag = _tag if _tag else DEFAULT_TAG
 
         with self._filelock:
             col = self._collection_type.load(self._item_type, self.collection_path)
             if tag not in col.repositories[repo]:
-                self._raise_not_found_by_name(name)
+                raise exceptions.NotFound(self._build_not_found_err_msg(name))
 
             del col.repositories[repo][tag]
             if len(col.repositories[repo]) == 0:
                 del col.repositories[repo]
 
             self._gc(col)
             self._delete_unused_blobs()
@@ -212,78 +230,83 @@
         col: "_JSONCollection[ItemType]",
     ):
         removed_id_and_data = col.prune()
         if len(removed_id_and_data) == 0:
             return
 
         for _, item in removed_id_and_data:
-            if not col.check_hash_exsistence(item.hash):
-                item.cleanup()
+            item.cleanup()
 
     def _delete_unused_blobs(self):
         self._blob_store.delete_unused(self._collect_blobs())
 
     def _collect_blobs(self) -> t.Set[Blob]:
         blobs: t.Set[Blob] = set()
         for m in self.list():
             blobs = blobs.union(m.blobs)
         return blobs
 
-    def _raise_not_found_by_name(self, name: str):
-        raise exceptions.NotFound(f"{self._item_type.get_typename()} '{name}'")
-
-    def _raise_not_found_by_id(self, id: str):
-        raise exceptions.NotFound(f"{self._item_type.get_typename()} id '{id}'")
+    def _build_not_found_err_msg(self, name: str):
+        return f"{self._item_type.get_typename()} '{name}'"
 
 
 @attrs.frozen
 class _JSONCollection(t.Generic[ItemType]):
     repositories: t.Dict[str, t.Dict[str, str]] = attrs.field(factory=dict)
     items: t.Dict[str, ItemType] = attrs.field(factory=dict)
 
-    def tag(self, repo_name: str, tag: str, id: str):
+    def tag_item(self, repo_name: str, tag: str, id: str):
         if repo_name not in self.repositories.keys():
             self.repositories[repo_name] = dict()
         self.repositories[repo_name][tag] = id
         return id
 
-    def add(
+    def add_item(
         self,
         item: ItemType,
     ):
         if item.repo_name not in self.repositories.keys():
             self.repositories[item.repo_name] = dict()
         self.items[item.id] = item
-        self.tag(item.repo_name, item.tag, item.id)
+        self.tag_item(item.repo_name, item.tag, item.id)
 
-    def update(self, item: ItemType):
+    def update_item(self, item: ItemType):
         orig = self.items[item.id]
         assert orig.id == item.id
         self.items[item.id] = item
 
-    def get_by_tag(self, repo_name: str, tag: str) -> t.Optional[ItemType]:
+    def get_item_by_tag(self, repo_name: str, tag: str) -> t.Optional[ItemType]:
         if repo_name not in self.repositories or tag not in self.repositories[repo_name]:
             return None
         item = self.items[self.repositories[repo_name][tag]]
         return item
 
-    def get_by_id(self, id: str) -> t.Optional[ItemType]:
+    def get_item_by_id(self, id: str) -> t.Optional[ItemType]:
         if id not in self.items:
             return None
         return self.items[id]
 
-    def list(self) -> t.List[t.Tuple[str, str, ItemType]]:
+    def get_latest_tag_in_repo(self, repo_name: str) -> t.Optional[str]:
+        if len(self.repositories[repo_name]) == 0:
+            return None
+        return sorted(
+            self.repositories[repo_name].keys(),
+            key=lambda key: self.items[self.repositories[repo_name][key]].created_at,
+            reverse=True,
+        )[0]
+
+    def list_items(self) -> t.List[t.Tuple[str, str, ItemType]]:
         ret: t.List[t.Tuple[str, str, ItemType]] = []
         for repo_name in self.repositories.keys():
             for tag, id in self.repositories[repo_name].items():
                 item = self.items[id]
                 ret.append((repo_name, tag, item))
         return sorted(ret, key=lambda val: (val[0], datetime.utcnow() - val[2].created_at))
 
-    def list_in_repo(self, repo_name: str) -> t.List[t.Tuple[str, ItemType]]:
+    def list_items_in_repo(self, repo_name: str) -> t.List[t.Tuple[str, ItemType]]:
         ret: t.List[t.Tuple[str, ItemType]] = []
         for tag, id in self.repositories[repo_name].items():
             item = self.items[id]
             ret.append((tag, item))
         return sorted(ret, key=lambda val: val[1].created_at, reverse=True)
 
     def prune(
@@ -299,31 +322,24 @@
             is_removed = not self.check_item_exsistence(id)
             if is_removed:
                 deleted.append((id, self.items[id]))
                 del self.items[id]
 
         return deleted
 
-    def check_item_exsistence(self, id: str) -> bool:
-        for repo_name in self.repositories.keys():
-            if id in self.repositories[repo_name].values():
-                return True
-        return False
+    def check_tag_exsistence_in_repo(self, repo_name: str, tag: str) -> bool:
+        return repo_name in self.repositories and tag in self.repositories[repo_name]
 
-    def check_hash_exsistence(self, hash_val: str) -> bool:
-        for repo_name in self.repositories.keys():
-            for id in self.repositories[repo_name].values():
-                data = self.items[id]
-                if data.hash == hash_val:
-                    return True
-        return False
-
-    def cleanup(self, removed: ItemType):
-        if not self.check_hash_exsistence(removed.hash):
-            removed.cleanup()
+    def check_repo_exsistence(self, repo_name: str) -> bool:
+        return repo_name in self.repositories
+
+    def check_item_exsistence(self, id: str) -> bool:
+        return any(
+            id in self.repositories[repo_name].values() for repo_name in self.repositories.keys()
+        )
 
     def save(self, path: Path):
         log_debug(f"Save JSON collection to '{path}'")
         serialized = convert_attrs_to_json(self)
         write_safely(path, serialized)
 
     @classmethod
```

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/logging.py` & `tungstenkit-0.1.3/tungstenkit/_internal/logging.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_clients/api_client.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_clients/container_client.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_clients/container_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_clients/schemas.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_clients/schemas.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_def.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_def.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_def_loader.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_def_loader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/cli.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_server/cli.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/config.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_server/config.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_server/event_buses/abstract_event_bus.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/file_uploaders/factory.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_server/file_uploaders/factory.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_server/file_uploaders/in_memory_file_uploader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_server/file_uploaders/local_fs_file_uploader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/http_server.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_server/http_server.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/ids.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_server/ids.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_server/input_queues/abstract_input_queue.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/input_queues/local_input_queue.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_server/input_queues/local_input_queue.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/prediction_worker/executor.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_server/prediction_worker/executor.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/prediction_worker/subproc.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_server/prediction_worker/subproc.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/prediction_worker/worker.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_server/prediction_worker/worker.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_server/result_caches/abstract_result_cache.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/result_caches/local_result_cache.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_server/result_caches/local_result_cache.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_server/schema.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_server/schema.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/model_store.py` & `tungstenkit-0.1.3/tungstenkit/_internal/model_store.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing as t
 
-from tungstenkit._internal.json_store import JSONCollection
+from tungstenkit._internal.json_store import JSONStore
 from tungstenkit._internal.storables.model_data import ModelData, StoredModelData
 
-_store = JSONCollection[StoredModelData](StoredModelData)
+_store = JSONStore[StoredModelData](StoredModelData)
 
 
 def add(model: ModelData) -> None:
     stored = model.save()
     _store.add(stored)
```

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/pred_interface/abstract_interface.py` & `tungstenkit-0.1.3/tungstenkit/_internal/pred_interface/abstract_interface.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/pred_interface/api_interface.py` & `tungstenkit-0.1.3/tungstenkit/_internal/pred_interface/api_interface.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/pred_interface/local_interface.py` & `tungstenkit-0.1.3/tungstenkit/_internal/pred_interface/local_interface.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/storables/avatar_data.py` & `tungstenkit-0.1.3/tungstenkit/_internal/storables/avatar_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     def save_blobs(
         self,
         blob_store: BlobStore,
         file_blob_create_policy: FileBlobCreatePolicy = "copy",
     ) -> StoredAvatar:
         filename = "avatar" + self.extension
-        blob = blob_store.add_by_writing((self.bytes_, "avatar" + filename))
+        blob = blob_store.add_by_writing((self.bytes_, filename))
         return StoredAvatar(blob=blob)
 
     @classmethod
     def load_blobs(cls, data: StoredAvatar) -> "AvatarData":
         return AvatarData(
             bytes_=data.blob.file_path.read_bytes(),
             extension=data.extension,
```

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/storables/markdown_data.py` & `tungstenkit-0.1.3/tungstenkit/_internal/storables/markdown_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/storables/model_data.py` & `tungstenkit-0.1.3/tungstenkit/_internal/storables/model_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import typing as t
 from datetime import datetime
 
 import attrs
 
+from tungstenkit import exceptions
 from tungstenkit._internal.blob_store import Blob, BlobStore, FileBlobCreatePolicy
+from tungstenkit._internal.constants import DEFAULT_GPU_MEM_GB
 from tungstenkit._internal.json_store import JSONItem, JSONStorable
-from tungstenkit._internal.utils.docker import get_docker_client, parse_docker_image_name
+from tungstenkit._internal.utils.docker import (
+    get_docker_client,
+    parse_docker_image_name,
+    remove_docker_image,
+)
 from tungstenkit._internal.utils.serialize import load_attrs_from_json
 
 from .avatar_data import AvatarData, StoredAvatar
 from .markdown_data import MarkdownData, StoredMarkdown
 from .model_io_data import ModelIOData, StoredModelIOData
 from .source_file_data import (
     SerializedSourceFileCollection,
@@ -59,43 +65,41 @@
                     batch_size = int(val)
         if labels:
             for label_name, label_value in labels.items():
                 if label_name == "device":
                     device = label_value
                 elif label_name == "gpu_mem_gb":
                     gpu_mem_gb = int(label_value)
+                    if device == "gpu" and gpu_mem_gb == 0:
+                        gpu_mem_gb = DEFAULT_GPU_MEM_GB
 
         return _ModelDataInImage(
             module_name=module_name,
             class_name=class_name,
             docker_image_id=docker_image_id,
             batch_size=batch_size,
             device=device,
             gpu_mem_gb=gpu_mem_gb,
         )
 
 
 @attrs.frozen(kw_only=True)
-class StoredModelData(_ModelDataInImage, JSONItem):
+class StoredModelData(JSONItem):
     id: str
     repo_name: str
     tag: str
 
     io: StoredModelIOData
     avatar: StoredAvatar
     readme: t.Optional[StoredMarkdown] = None
     source_files: t.Optional[SerializedSourceFileCollection] = None
 
     created_at: datetime = attrs.field(factory=datetime.utcnow)
 
     @property
-    def hash(self) -> str:
-        return self.docker_image_id
-
-    @property
     def blobs(self) -> t.Set[Blob]:
         blob_set: t.Set[Blob] = set()
 
         blob_set.add(self.io.blob)
 
         blob_set.add(self.avatar.blob)
 
@@ -111,16 +115,15 @@
             for f in source_files.files:
                 if f.blob is not None:
                     blob_set.add(f.blob)
 
         return blob_set
 
     def cleanup(self):
-        docker_client = get_docker_client(timeout=None)
-        docker_client.images.remove(image=self.docker_image_id, force=True)
+        remove_docker_image(self.name)
 
     @staticmethod
     def parse_name(name: str) -> t.Tuple[str, str]:
         repo, tag = parse_docker_image_name(name)
         if tag:
             return repo, tag
         return repo, "latest"
@@ -210,24 +213,18 @@
         if self._created_at:
             extra_kwargs["created_at"] = self._created_at
 
         return StoredModelData(
             id=self.id,
             repo_name=self.repo_name,
             tag=self.tag,
-            readme=stored_readme,
             io=stored_schema,
             avatar=stored_avatar,
+            readme=stored_readme,
             source_files=stored_source_files,
-            module_name=self.module_name,
-            class_name=self.class_name,
-            docker_image_id=self.docker_image_id,
-            batch_size=self.batch_size,
-            device=self.device,
-            gpu_mem_gb=self.gpu_mem_gb,
             **extra_kwargs,
         )
 
     @classmethod
     def load_blobs(cls, data: StoredModelData) -> "ModelData":
         return ModelData(
             name=data.name,
```

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/storables/model_io_data.py` & `tungstenkit-0.1.3/tungstenkit/_internal/storables/model_io_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/storables/pred_example_data.py` & `tungstenkit-0.1.3/tungstenkit/_internal/storables/pred_example_data.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/storables/source_file_data.py` & `tungstenkit-0.1.3/tungstenkit/_internal/storables/source_file_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,19 @@
             (convert_attrs_to_json(stored).encode("utf-8"), "source_files.json")
         )
 
         return SerializedSourceFileCollection(blob=serialized)
 
     @classmethod
     def load_blobs(cls, data: SerializedSourceFileCollection) -> "SourceFileCollection":
-        stored_col = load_attrs_from_json(StoredSourceFileCollection, data.blob.file_path)
+        try:
+            stored_col = load_attrs_from_json(StoredSourceFileCollection, data.blob.file_path)
+        except Exception as e:
+            print(data.blob.file_path)
+            raise e
         col = cls()
         for stored_src_file in stored_col.files:
             abs_path_in_host_fs = (
                 None if stored_src_file.blob is None else stored_src_file.blob.file_path
             )
             col.add(
                 SourceFile(
```

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/task.py` & `tungstenkit-0.1.3/tungstenkit/_internal/task.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/tungsten_clients/api_client.py` & `tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/tungsten_clients/client.py` & `tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/tungsten_clients/schemas/__init__.py` & `tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/tungsten_clients/schemas/model.py` & `tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/tungsten_clients/schemas/project.py` & `tungstenkit-0.1.3/tungstenkit/_internal/tungsten_clients/schemas/project.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/avatar.py` & `tungstenkit-0.1.3/tungstenkit/_internal/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/console.py` & `tungstenkit-0.1.3/tungstenkit/_internal/utils/console.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/context.py` & `tungstenkit-0.1.3/tungstenkit/_internal/utils/context.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/docker.py` & `tungstenkit-0.1.3/tungstenkit/_internal/utils/docker.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/file.py` & `tungstenkit-0.1.3/tungstenkit/_internal/utils/file.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/gpu.py` & `tungstenkit-0.1.3/tungstenkit/_internal/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/imports.py` & `tungstenkit-0.1.3/tungstenkit/_internal/utils/imports.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/json.py` & `tungstenkit-0.1.3/tungstenkit/_internal/utils/json.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/markdown.py` & `tungstenkit-0.1.3/tungstenkit/_internal/utils/markdown.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/pydantic.py` & `tungstenkit-0.1.3/tungstenkit/_internal/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/regex.py` & `tungstenkit-0.1.3/tungstenkit/_internal/utils/regex.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/requests.py` & `tungstenkit-0.1.3/tungstenkit/_internal/utils/requests.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/serialize.py` & `tungstenkit-0.1.3/tungstenkit/_internal/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/string.py` & `tungstenkit-0.1.3/tungstenkit/_internal/utils/string.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/types.py` & `tungstenkit-0.1.3/tungstenkit/_internal/utils/types.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/uri.py` & `tungstenkit-0.1.3/tungstenkit/_internal/utils/uri.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/_internal/utils/version.py` & `tungstenkit-0.1.3/tungstenkit/_internal/utils/version.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/tungstenkit/exceptions.py` & `tungstenkit-0.1.3/tungstenkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.1.2.post8/PKG-INFO` & `tungstenkit-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tungstenkit
-Version: 0.1.2.post8
+Version: 0.1.3
 Summary: ML container made simple
 Home-page: https://github.com/tungsten-ai/tungstenkit
 Author: Tungsten Contributors
 Author-email: foss@tungsten-ai.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -30,15 +30,14 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Typing :: Typed
-Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: attrs (>=22.1.0,<23.0.0)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: binaryornot (>=0.4.4,<0.5.0)
 Requires-Dist: cattrs (>=22.1.0,<23.0.0)
 Requires-Dist: dill (>=0.3.6,<0.4.0)
 Requires-Dist: docker (>=6.0.1,<7.0.0)
 Requires-Dist: fastapi (>=0.88.0,<1.0.0)
@@ -47,14 +46,15 @@
 Requires-Dist: furl (>=2.1.3,<3.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: loguru (>=0.6.0,<1.0.0)
 Requires-Dist: markdown (>=3.4.1,<4.0.0)
 Requires-Dist: markdownify (>=0.11.6,<0.12.0)
 Requires-Dist: pathspec (>=0.10.2,<0.11.0)
 Requires-Dist: pillow (>=5.2.0)
+Requires-Dist: platformdirs (>=3.8.1,<4.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pynvml (>=11.5.0,<12.0.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: pyyaml (>=5.4,<6.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: requests-toolbelt (>=0.10.1,<0.11.0)
 Requires-Dist: rich (>=13.3.1,<14.0.0)
```

