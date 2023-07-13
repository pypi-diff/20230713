# Comparing `tmp/aiges-0.8.8.tar.gz` & `tmp/aiges-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiges-0.8.8.tar", max compression
+gzip compressed data, was "aiges-0.8.9.tar", max compression
```

## Comparing `aiges-0.8.8.tar` & `aiges-0.8.9.tar`

### file list

```diff
@@ -1,86 +1,87 @@
--rw-r--r--   0        0        0    11357 2022-06-15 00:31:44.495583 aiges-0.8.8/LICENSE
--rw-r--r--   0        0        0     1151 2022-06-15 00:40:08.182732 aiges-0.8.8/aiges/__init__.py
--rw-r--r--   0        0        0     3323 2022-11-29 02:08:42.314189 aiges-0.8.8/aiges/__main__.py
--rw-r--r--   0        0        0       90 2022-11-03 05:58:54.792324 aiges-0.8.8/aiges/aiges_inner/README.md
--rw-r--r--   0        0        0     1151 2022-06-15 00:40:08.182000 aiges-0.8.8/aiges/aiges_inner/__init__.py
--rw-r--r--   0        0        0     1425 2023-03-01 08:16:07.297594 aiges-0.8.8/aiges/aiges_inner/ai.proto
--rw-r--r--   0        0        0      515 2023-03-02 01:51:31.299117 aiges-0.8.8/aiges/aiges_inner/ai_service.proto
--rw-r--r--   0        0        0     1636 2023-03-06 05:26:58.951209 aiges-0.8.8/aiges/aiges_inner/aiges_inner.proto
--rw-r--r--   0        0        0     5595 2023-03-29 05:44:31.505166 aiges-0.8.8/aiges/aiges_inner/aiges_inner_pb2.py
--rw-r--r--   0        0        0    14516 2023-03-29 05:44:31.505312 aiges-0.8.8/aiges/aiges_inner/aiges_inner_pb2_grpc.py
--rw-r--r--   0        0        0      842 2022-07-19 10:49:24.538000 aiges-0.8.8/aiges/aiges_inner/grpc_stdio.proto
--rw-r--r--   0        0        0     1900 2023-03-02 02:55:58.441931 aiges-0.8.8/aiges/aiges_inner/grpc_stdio_pb2.py
--rw-r--r--   0        0        0     3094 2023-03-02 02:55:58.438281 aiges-0.8.8/aiges/aiges_inner/grpc_stdio_pb2_grpc.py
--rw-r--r--   0        0        0     4062 2022-07-04 13:48:54.771921 aiges-0.8.8/aiges/backup/demo.json
--rw-r--r--   0        0        0     4021 2022-07-20 10:15:28.790530 aiges-0.8.8/aiges/backup/wrapper_mmocr.py
--rw-r--r--   0        0        0     1498 2022-07-20 08:18:27.238393 aiges-0.8.8/aiges/backup/wrapper_old.py
--rw-r--r--   0        0        0     1677 2022-06-15 01:48:05.297840 aiges-0.8.8/aiges/call_wrapper.py
--rw-r--r--   0        0        0     1818 2023-03-03 05:50:18.918527 aiges-0.8.8/aiges/callback.py
--rw-r--r--   0        0        0       25 2022-11-13 12:50:20.760280 aiges-0.8.8/aiges/client/Readme.md
--rw-r--r--   0        0        0     1151 2022-11-13 12:50:20.757419 aiges-0.8.8/aiges/client/__init__.py
--rw-r--r--   0        0        0     6183 2022-11-13 13:12:50.827386 aiges-0.8.8/aiges/client/client.py
--rw-r--r--   0        0        0     1900 2022-11-13 12:53:41.847174 aiges-0.8.8/aiges/client/utils/aipass_client.py
--rw-r--r--   0        0        0      204 2022-10-26 01:33:06.000000 aiges-0.8.8/aiges/client/utils/exception.py
--rw-r--r--   0        0        0     2177 2022-11-13 12:54:07.467933 aiges-0.8.8/aiges/client/utils/ne_utils.py
--rw-r--r--   0        0        0     3012 2023-03-28 12:34:18.852264 aiges-0.8.8/aiges/client.py
--rw-r--r--   0        0        0     1171 2022-07-26 15:18:10.588415 aiges-0.8.8/aiges/cmd/__init__.py
--rw-r--r--   0        0        0      265 2022-07-27 01:23:00.929292 aiges-0.8.8/aiges/cmd/config.py
--rw-r--r--   0        0        0     4725 2022-08-02 06:46:09.425970 aiges-0.8.8/aiges/cmd/create.py
--rw-r--r--   0        0        0     2669 2022-11-27 13:31:02.965147 aiges-0.8.8/aiges/cmd/package.py
--rw-r--r--   0        0        0     1384 2022-09-08 07:23:58.817883 aiges-0.8.8/aiges/cmd/root.py
--rw-r--r--   0        0        0     1151 2022-11-13 12:50:20.757000 aiges-0.8.8/aiges/concurrent/__init__.py
--rw-r--r--   0        0        0     2053 2023-03-02 13:37:44.323424 aiges-0.8.8/aiges/concurrent/fixpool.py
--rw-r--r--   0        0        0     1192 2023-03-02 11:01:06.565315 aiges-0.8.8/aiges/concurrent/pool.py
--rw-r--r--   0        0        0     2546 2022-09-08 02:50:41.715880 aiges-0.8.8/aiges/core/aiges_methods.py
--rw-r--r--   0        0        0     4420 2022-09-08 02:50:41.716028 aiges-0.8.8/aiges/core/metadata.py
--rw-r--r--   0        0        0     7850 2022-09-08 02:50:41.716166 aiges-0.8.8/aiges/core/rest.py
--rw-r--r--   0        0        0     1712 2023-02-22 12:53:05.041479 aiges-0.8.8/aiges/core/types.py
--rw-r--r--   0        0        0     3591 2023-03-02 14:20:03.189120 aiges-0.8.8/aiges/dto.py
--rw-r--r--   0        0        0       74 2022-11-04 12:47:04.911294 aiges-0.8.8/aiges/errors.py
--rw-r--r--   0        0        0     6519 2022-09-15 14:35:15.468000 aiges-0.8.8/aiges/examples/once/mmocr/wrapper.py
--rw-r--r--   0        0        0     8509 2023-03-17 02:56:21.629589 aiges-0.8.8/aiges/examples/stream/mmocr/wrapper.py
--rw-r--r--   0        0        0     8495 2022-11-26 13:54:42.871294 aiges-0.8.8/aiges/examples/stream/mock/wrapper.py
--rw-r--r--   0        0        0        0 2023-01-11 07:09:05.778269 aiges-0.8.8/aiges/gradio_util/__init__.py
--rw-r--r--   0        0        0     5268 2023-01-15 06:17:51.753946 aiges-0.8.8/aiges/gradio_util/component.py
--rw-r--r--   0        0        0    18055 2023-03-06 08:07:12.977008 aiges-0.8.8/aiges/out.json
--rw-r--r--   0        0        0     3821 2023-03-03 13:56:34.295654 aiges-0.8.8/aiges/protocol/struct.py
--rw-r--r--   0        0        0     1112 2023-03-03 12:43:35.632226 aiges-0.8.8/aiges/protocol/xsf.proto
--rw-r--r--   0        0        0     3667 2023-03-29 05:44:31.691747 aiges-0.8.8/aiges/protocol/xsf_pb2.py
--rw-r--r--   0        0        0     4096 2023-03-29 05:44:31.692360 aiges-0.8.8/aiges/protocol/xsf_pb2.pyi
--rw-r--r--   0        0        0     4721 2023-03-29 05:44:31.692431 aiges-0.8.8/aiges/protocol/xsf_pb2_grpc.py
--rw-r--r--   0        0        0     1724 2023-03-03 12:52:58.574856 aiges-0.8.8/aiges/protocol/xsfcli.py
--rw-r--r--   0        0        0     8814 2023-03-05 12:27:52.615723 aiges-0.8.8/aiges/schema/aischema.py
--rw-r--r--   0        0        0     3024 2023-03-06 04:56:39.663627 aiges-0.8.8/aiges/schema/types.py
--rw-r--r--   0        0        0     2675 2022-11-24 13:44:21.247745 aiges-0.8.8/aiges/schema/utils/schemaUtils.py
--rw-r--r--   0        0        0    36316 2023-03-06 05:06:13.483085 aiges-0.8.8/aiges/sdk.py
--rw-r--r--   0        0        0    12024 2023-03-29 05:44:19.749268 aiges-0.8.8/aiges/serve.py
--rw-r--r--   0        0        0     5315 2023-03-02 02:55:58.445779 aiges-0.8.8/aiges/server.py
--rw-r--r--   0        0        0     2284 2023-03-02 02:55:58.444481 aiges-0.8.8/aiges/server2.py
--rw-r--r--   0        0        0     9179 2023-03-02 10:03:56.694610 aiges-0.8.8/aiges/stream.py
--rw-r--r--   0        0        0     2770 2022-11-22 13:07:59.849019 aiges-0.8.8/aiges/test_data/flask_restx_test.py
--rw-r--r--   0        0        0      152 2022-11-22 11:15:30.684483 aiges-0.8.8/aiges/test_data/ok.json
--rw-r--r--   0        0        0      128 2022-11-22 11:15:44.926581 aiges-0.8.8/aiges/test_data/origin.json
--rw-r--r--   0        0        0     1830 2023-01-14 12:45:07.922832 aiges-0.8.8/aiges/test_data/pydantic_test.py
--rw-r--r--   0        0        0    95827 2022-06-15 02:02:56.681000 aiges-0.8.8/aiges/test_data/test.png
--rw-r--r--   0        0        0     8007 2022-11-22 03:30:28.575847 aiges-0.8.8/aiges/test_data/testschma.json
--rw-r--r--   0        0        0      638 2022-08-03 03:49:47.166058 aiges-0.8.8/aiges/tpls/Dockerfile.j2
--rw-r--r--   0        0        0      222 2022-07-27 01:24:01.656775 aiges-0.8.8/aiges/tpls/Readme.md.j2
--rw-r--r--   0        0        0       44 2022-08-02 06:06:33.201783 aiges-0.8.8/aiges/tpls/requirements.txt.j2
--rw-r--r--   0        0        0     5560 2022-08-02 05:56:25.900297 aiges-0.8.8/aiges/tpls/wrapper.py.j2
--rw-r--r--   0        0        0     2663 2022-09-08 02:50:41.716535 aiges-0.8.8/aiges/utils/flask_utils.py
--rw-r--r--   0        0        0     2405 2023-03-06 05:22:22.762218 aiges-0.8.8/aiges/utils/log.py
--rw-r--r--   0        0        0     2866 2023-03-03 05:37:52.319734 aiges-0.8.8/aiges/worker.py
--rw-r--r--   0        0        0     6919 2023-02-15 11:03:22.137967 aiges-0.8.8/aiges/wrapper.py
--rw-r--r--   0        0        0     8190 2022-10-18 01:30:42.234865 aiges-0.8.8/aiges/wrapper_test.py
--rw-r--r--   0        0        0     1151 2023-03-04 14:20:01.721640 aiges-0.8.8/aiges/ws/__init__.py
--rw-r--r--   0        0        0     8245 2023-03-26 14:02:43.945140 aiges-0.8.8/aiges/ws/app.py
--rw-r--r--   0        0        0     5298 2023-03-12 01:18:24.866183 aiges-0.8.8/aiges/ws/app2.py
--rw-r--r--   0        0        0      691 2023-03-16 11:21:23.346073 aiges-0.8.8/aiges/ws/sample.json
--rw-r--r--   0        0        0     1151 2023-03-10 23:55:58.923188 aiges-0.8.8/aiges/ws/tests/__init__.py
--rw-r--r--   0        0        0     1500 2023-03-10 23:55:58.920245 aiges-0.8.8/aiges/ws/tests/test_button.py
--rw-r--r--   0        0        0     3604 2023-03-14 06:51:47.178908 aiges-0.8.8/aiges/ws/ws_client.py
--rw-r--r--   0        0        0     3620 2023-03-12 01:25:08.225870 aiges-0.8.8/aiges/ws/ws_client_test.py
--rw-r--r--   0        0        0      226 2023-03-12 02:37:58.465934 aiges-0.8.8/aiges/ws/ws_client_test2.py
--rw-r--r--   0        0        0      592 2023-03-29 05:44:26.649198 aiges-0.8.8/pyproject.toml
--rw-r--r--   0        0        0     1188 2023-03-29 05:44:32.649262 aiges-0.8.8/setup.py
--rw-r--r--   0        0        0      908 2023-03-29 05:44:32.649497 aiges-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-06-15 00:31:44.495583 aiges-0.8.9/LICENSE
+-rw-r--r--   0        0        0     1151 2022-06-15 00:40:08.182732 aiges-0.8.9/aiges/__init__.py
+-rw-r--r--   0        0        0     3323 2022-11-29 02:08:42.314189 aiges-0.8.9/aiges/__main__.py
+-rw-r--r--   0        0        0       90 2022-11-03 05:58:54.792324 aiges-0.8.9/aiges/aiges_inner/README.md
+-rw-r--r--   0        0        0     1151 2022-06-15 00:40:08.182000 aiges-0.8.9/aiges/aiges_inner/__init__.py
+-rw-r--r--   0        0        0     1425 2023-03-01 08:16:07.297594 aiges-0.8.9/aiges/aiges_inner/ai.proto
+-rw-r--r--   0        0        0      515 2023-03-02 01:51:31.299117 aiges-0.8.9/aiges/aiges_inner/ai_service.proto
+-rw-r--r--   0        0        0     1636 2023-03-06 05:26:58.951209 aiges-0.8.9/aiges/aiges_inner/aiges_inner.proto
+-rw-r--r--   0        0        0     5595 2023-05-22 05:51:45.395102 aiges-0.8.9/aiges/aiges_inner/aiges_inner_pb2.py
+-rw-r--r--   0        0        0    14516 2023-05-22 05:51:45.395595 aiges-0.8.9/aiges/aiges_inner/aiges_inner_pb2_grpc.py
+-rw-r--r--   0        0        0      842 2022-07-19 10:49:24.538000 aiges-0.8.9/aiges/aiges_inner/grpc_stdio.proto
+-rw-r--r--   0        0        0     1900 2023-03-02 02:55:58.441931 aiges-0.8.9/aiges/aiges_inner/grpc_stdio_pb2.py
+-rw-r--r--   0        0        0     3094 2023-03-02 02:55:58.438281 aiges-0.8.9/aiges/aiges_inner/grpc_stdio_pb2_grpc.py
+-rw-r--r--   0        0        0     4062 2022-07-04 13:48:54.771921 aiges-0.8.9/aiges/backup/demo.json
+-rw-r--r--   0        0        0     4021 2022-07-20 10:15:28.790530 aiges-0.8.9/aiges/backup/wrapper_mmocr.py
+-rw-r--r--   0        0        0     1498 2022-07-20 08:18:27.238393 aiges-0.8.9/aiges/backup/wrapper_old.py
+-rw-r--r--   0        0        0     1677 2022-06-15 01:48:05.297840 aiges-0.8.9/aiges/call_wrapper.py
+-rw-r--r--   0        0        0     1818 2023-03-03 05:50:18.918527 aiges-0.8.9/aiges/callback.py
+-rw-r--r--   0        0        0       25 2022-11-13 12:50:20.760280 aiges-0.8.9/aiges/client/Readme.md
+-rw-r--r--   0        0        0     1151 2022-11-13 12:50:20.757419 aiges-0.8.9/aiges/client/__init__.py
+-rw-r--r--   0        0        0     6183 2022-11-13 13:12:50.827386 aiges-0.8.9/aiges/client/client.py
+-rw-r--r--   0        0        0     1900 2022-11-13 12:53:41.847174 aiges-0.8.9/aiges/client/utils/aipass_client.py
+-rw-r--r--   0        0        0      204 2022-10-26 01:33:06.000000 aiges-0.8.9/aiges/client/utils/exception.py
+-rw-r--r--   0        0        0     2177 2022-11-13 12:54:07.467933 aiges-0.8.9/aiges/client/utils/ne_utils.py
+-rw-r--r--   0        0        0     3012 2023-03-28 12:34:18.852264 aiges-0.8.9/aiges/client.py
+-rw-r--r--   0        0        0     1171 2022-07-26 15:18:10.588415 aiges-0.8.9/aiges/cmd/__init__.py
+-rw-r--r--   0        0        0      265 2022-07-27 01:23:00.929292 aiges-0.8.9/aiges/cmd/config.py
+-rw-r--r--   0        0        0     4725 2022-08-02 06:46:09.425970 aiges-0.8.9/aiges/cmd/create.py
+-rw-r--r--   0        0        0     2669 2022-11-27 13:31:02.965147 aiges-0.8.9/aiges/cmd/package.py
+-rw-r--r--   0        0        0     1384 2022-09-08 07:23:58.817883 aiges-0.8.9/aiges/cmd/root.py
+-rw-r--r--   0        0        0     1151 2022-11-13 12:50:20.757000 aiges-0.8.9/aiges/concurrent/__init__.py
+-rw-r--r--   0        0        0     2053 2023-03-02 13:37:44.323424 aiges-0.8.9/aiges/concurrent/fixpool.py
+-rw-r--r--   0        0        0     1192 2023-03-02 11:01:06.565315 aiges-0.8.9/aiges/concurrent/pool.py
+-rw-r--r--   0        0        0     2546 2022-09-08 02:50:41.715880 aiges-0.8.9/aiges/core/aiges_methods.py
+-rw-r--r--   0        0        0     4420 2022-09-08 02:50:41.716028 aiges-0.8.9/aiges/core/metadata.py
+-rw-r--r--   0        0        0     7850 2022-09-08 02:50:41.716166 aiges-0.8.9/aiges/core/rest.py
+-rw-r--r--   0        0        0     1712 2023-02-22 12:53:05.041479 aiges-0.8.9/aiges/core/types.py
+-rw-r--r--   0        0        0     3591 2023-03-02 14:20:03.189120 aiges-0.8.9/aiges/dto.py
+-rw-r--r--   0        0        0       74 2022-11-04 12:47:04.911294 aiges-0.8.9/aiges/errors.py
+-rw-r--r--   0        0        0     6519 2022-09-15 14:35:15.468000 aiges-0.8.9/aiges/examples/once/mmocr/wrapper.py
+-rw-r--r--   0        0        0     8509 2023-03-17 02:56:21.629589 aiges-0.8.9/aiges/examples/stream/mmocr/wrapper.py
+-rw-r--r--   0        0        0     8515 2023-05-22 05:09:23.695790 aiges-0.8.9/aiges/examples/stream/mock/wrapper.py
+-rw-r--r--   0        0        0        0 2023-01-11 07:09:05.778269 aiges-0.8.9/aiges/gradio_util/__init__.py
+-rw-r--r--   0        0        0     5268 2023-01-15 06:17:51.753946 aiges-0.8.9/aiges/gradio_util/component.py
+-rw-r--r--   0        0        0    18055 2023-03-06 08:07:12.977008 aiges-0.8.9/aiges/out.json
+-rw-r--r--   0        0        0     3821 2023-03-03 13:56:34.295654 aiges-0.8.9/aiges/protocol/struct.py
+-rw-r--r--   0        0        0     1112 2023-03-03 12:43:35.632226 aiges-0.8.9/aiges/protocol/xsf.proto
+-rw-r--r--   0        0        0     3667 2023-05-22 05:51:45.567944 aiges-0.8.9/aiges/protocol/xsf_pb2.py
+-rw-r--r--   0        0        0     4096 2023-05-22 05:51:45.568245 aiges-0.8.9/aiges/protocol/xsf_pb2.pyi
+-rw-r--r--   0        0        0     4721 2023-05-22 05:51:45.568329 aiges-0.8.9/aiges/protocol/xsf_pb2_grpc.py
+-rw-r--r--   0        0        0     1724 2023-03-03 12:52:58.574856 aiges-0.8.9/aiges/protocol/xsfcli.py
+-rw-r--r--   0        0        0     8814 2023-03-05 12:27:52.615723 aiges-0.8.9/aiges/schema/aischema.py
+-rw-r--r--   0        0        0     3024 2023-03-06 04:56:39.663627 aiges-0.8.9/aiges/schema/types.py
+-rw-r--r--   0        0        0     2675 2022-11-24 13:44:21.247745 aiges-0.8.9/aiges/schema/utils/schemaUtils.py
+-rw-r--r--   0        0        0    36333 2023-05-22 05:08:34.838116 aiges-0.8.9/aiges/sdk.py
+-rw-r--r--   0        0        0    12024 2023-03-29 05:44:19.749268 aiges-0.8.9/aiges/serve.py
+-rw-r--r--   0        0        0    12023 2023-04-03 02:19:43.769109 aiges-0.8.9/aiges/serve_new.py
+-rw-r--r--   0        0        0     5315 2023-03-02 02:55:58.445779 aiges-0.8.9/aiges/server.py
+-rw-r--r--   0        0        0     2284 2023-03-02 02:55:58.444481 aiges-0.8.9/aiges/server2.py
+-rw-r--r--   0        0        0     9179 2023-03-02 10:03:56.694610 aiges-0.8.9/aiges/stream.py
+-rw-r--r--   0        0        0     2770 2022-11-22 13:07:59.849019 aiges-0.8.9/aiges/test_data/flask_restx_test.py
+-rw-r--r--   0        0        0      152 2022-11-22 11:15:30.684483 aiges-0.8.9/aiges/test_data/ok.json
+-rw-r--r--   0        0        0      128 2022-11-22 11:15:44.926581 aiges-0.8.9/aiges/test_data/origin.json
+-rw-r--r--   0        0        0     1830 2023-01-14 12:45:07.922832 aiges-0.8.9/aiges/test_data/pydantic_test.py
+-rw-r--r--   0        0        0    95827 2022-06-15 02:02:56.681000 aiges-0.8.9/aiges/test_data/test.png
+-rw-r--r--   0        0        0     8007 2022-11-22 03:30:28.575847 aiges-0.8.9/aiges/test_data/testschma.json
+-rw-r--r--   0        0        0      638 2022-08-03 03:49:47.166058 aiges-0.8.9/aiges/tpls/Dockerfile.j2
+-rw-r--r--   0        0        0      222 2022-07-27 01:24:01.656775 aiges-0.8.9/aiges/tpls/Readme.md.j2
+-rw-r--r--   0        0        0       44 2022-08-02 06:06:33.201783 aiges-0.8.9/aiges/tpls/requirements.txt.j2
+-rw-r--r--   0        0        0     5560 2022-08-02 05:56:25.900297 aiges-0.8.9/aiges/tpls/wrapper.py.j2
+-rw-r--r--   0        0        0     2663 2022-09-08 02:50:41.716535 aiges-0.8.9/aiges/utils/flask_utils.py
+-rw-r--r--   0        0        0     2405 2023-03-06 05:22:22.762218 aiges-0.8.9/aiges/utils/log.py
+-rw-r--r--   0        0        0     2866 2023-03-03 05:37:52.319734 aiges-0.8.9/aiges/worker.py
+-rw-r--r--   0        0        0     6919 2023-02-15 11:03:22.137967 aiges-0.8.9/aiges/wrapper.py
+-rw-r--r--   0        0        0     8190 2022-10-18 01:30:42.234865 aiges-0.8.9/aiges/wrapper_test.py
+-rw-r--r--   0        0        0     1151 2023-03-04 14:20:01.721640 aiges-0.8.9/aiges/ws/__init__.py
+-rw-r--r--   0        0        0     8245 2023-03-26 14:02:43.945140 aiges-0.8.9/aiges/ws/app.py
+-rw-r--r--   0        0        0     5298 2023-03-12 01:18:24.866183 aiges-0.8.9/aiges/ws/app2.py
+-rw-r--r--   0        0        0      691 2023-03-16 11:21:23.346073 aiges-0.8.9/aiges/ws/sample.json
+-rw-r--r--   0        0        0     1151 2023-03-10 23:55:58.923188 aiges-0.8.9/aiges/ws/tests/__init__.py
+-rw-r--r--   0        0        0     1500 2023-03-10 23:55:58.920245 aiges-0.8.9/aiges/ws/tests/test_button.py
+-rw-r--r--   0        0        0     3604 2023-03-14 06:51:47.178908 aiges-0.8.9/aiges/ws/ws_client.py
+-rw-r--r--   0        0        0     3620 2023-03-12 01:25:08.225870 aiges-0.8.9/aiges/ws/ws_client_test.py
+-rw-r--r--   0        0        0      226 2023-03-12 02:37:58.465934 aiges-0.8.9/aiges/ws/ws_client_test2.py
+-rw-r--r--   0        0        0      592 2023-05-22 05:51:42.200242 aiges-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0     1188 2023-05-22 05:51:46.508257 aiges-0.8.9/setup.py
+-rw-r--r--   0        0        0      908 2023-05-22 05:51:46.508478 aiges-0.8.9/PKG-INFO
```

### Comparing `aiges-0.8.8/LICENSE` & `aiges-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/__init__.py` & `aiges-0.8.9/aiges/__init__.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/__main__.py` & `aiges-0.8.9/aiges/__main__.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/aiges_inner/__init__.py` & `aiges-0.8.9/aiges/aiges_inner/__init__.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/aiges_inner/ai.proto` & `aiges-0.8.9/aiges/aiges_inner/ai.proto`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/aiges_inner/ai_service.proto` & `aiges-0.8.9/aiges/aiges_inner/ai_service.proto`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/aiges_inner/aiges_inner.proto` & `aiges-0.8.9/aiges/aiges_inner/aiges_inner.proto`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/aiges_inner/aiges_inner_pb2.py` & `aiges-0.8.9/aiges/aiges_inner/aiges_inner_pb2.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/aiges_inner/aiges_inner_pb2_grpc.py` & `aiges-0.8.9/aiges/aiges_inner/aiges_inner_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/aiges_inner/grpc_stdio.proto` & `aiges-0.8.9/aiges/aiges_inner/grpc_stdio.proto`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/aiges_inner/grpc_stdio_pb2.py` & `aiges-0.8.9/aiges/aiges_inner/grpc_stdio_pb2.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/aiges_inner/grpc_stdio_pb2_grpc.py` & `aiges-0.8.9/aiges/aiges_inner/grpc_stdio_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/backup/demo.json` & `aiges-0.8.9/aiges/backup/demo.json`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/backup/wrapper_mmocr.py` & `aiges-0.8.9/aiges/backup/wrapper_mmocr.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/backup/wrapper_old.py` & `aiges-0.8.9/aiges/backup/wrapper_old.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/call_wrapper.py` & `aiges-0.8.9/aiges/call_wrapper.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/callback.py` & `aiges-0.8.9/aiges/callback.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/client/__init__.py` & `aiges-0.8.9/aiges/client/__init__.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/client/client.py` & `aiges-0.8.9/aiges/client/client.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/client/utils/aipass_client.py` & `aiges-0.8.9/aiges/client/utils/aipass_client.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/client/utils/ne_utils.py` & `aiges-0.8.9/aiges/client/utils/ne_utils.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/client.py` & `aiges-0.8.9/aiges/client.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/cmd/__init__.py` & `aiges-0.8.9/aiges/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/cmd/create.py` & `aiges-0.8.9/aiges/cmd/create.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/cmd/package.py` & `aiges-0.8.9/aiges/cmd/package.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/cmd/root.py` & `aiges-0.8.9/aiges/cmd/root.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/concurrent/__init__.py` & `aiges-0.8.9/aiges/concurrent/__init__.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/concurrent/fixpool.py` & `aiges-0.8.9/aiges/concurrent/fixpool.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/concurrent/pool.py` & `aiges-0.8.9/aiges/concurrent/pool.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/core/aiges_methods.py` & `aiges-0.8.9/aiges/core/aiges_methods.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/core/metadata.py` & `aiges-0.8.9/aiges/core/metadata.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/core/rest.py` & `aiges-0.8.9/aiges/core/rest.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/core/types.py` & `aiges-0.8.9/aiges/core/types.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/dto.py` & `aiges-0.8.9/aiges/dto.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/examples/once/mmocr/wrapper.py` & `aiges-0.8.9/aiges/examples/once/mmocr/wrapper.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/examples/stream/mmocr/wrapper.py` & `aiges-0.8.9/aiges/examples/stream/mmocr/wrapper.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/examples/stream/mock/wrapper.py` & `aiges-0.8.9/aiges/examples/stream/mock/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         Wrapper.session_total = config.get("common.lic", 10)
 
         # 流式的话，可以在init_handle_pool中 初始化引擎，以下基于线程的流式仅仅是提供示例
         self.session.init_wrapper_config(config)
         self.session.init_handle_pool("thread", 10, MyReqDataThread)
         return 0
 
-    def wrapperOnceExec(cls, params: {}, reqData: DataListCls) -> Response:
+    def wrapperOnceExec(cls, params: {}, reqData: DataListCls, usrTag: str = '') -> Response:
         """
         非会话模式计算接口,对应oneShot请求,可能存在并发调用
         @param params 功能参数
         @param  reqData     请求数据实体字段 DataListCls,可通过 aiges.dto.DataListCls查看
         @return
             响应必须返回 Response类，非Response类将会引起未知错误
         """
@@ -262,15 +262,15 @@
         d = open("/home/mmocr/resources/mmocr-logo.png", "rb").read()
         # d = b"ccccccc"
         l.len = len(d)
         l.data = d
         r.list = [l]
         self.session_thread.callback_fn(r, self.session_thread.sid)
         if l.status == DataEnd:
-            self.session_thread.reset() #最后一帧数据后 释放会话
+            self.session_thread.reset()  # 最后一帧数据后 释放会话
         # self.out_q.put(r)
 
 
 if __name__ == '__main__':
     m = Wrapper()
     # m.schema()
     m.run()
```

### Comparing `aiges-0.8.8/aiges/gradio_util/component.py` & `aiges-0.8.9/aiges/gradio_util/component.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/out.json` & `aiges-0.8.9/aiges/out.json`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/protocol/struct.py` & `aiges-0.8.9/aiges/protocol/struct.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/protocol/xsf.proto` & `aiges-0.8.9/aiges/protocol/xsf.proto`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/protocol/xsf_pb2.py` & `aiges-0.8.9/aiges/protocol/xsf_pb2.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/protocol/xsf_pb2.pyi` & `aiges-0.8.9/aiges/protocol/xsf_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/protocol/xsf_pb2_grpc.py` & `aiges-0.8.9/aiges/protocol/xsf_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/protocol/xsfcli.py` & `aiges-0.8.9/aiges/protocol/xsfcli.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/schema/aischema.py` & `aiges-0.8.9/aiges/schema/aischema.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/schema/types.py` & `aiges-0.8.9/aiges/schema/types.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/schema/utils/schemaUtils.py` & `aiges-0.8.9/aiges/schema/utils/schemaUtils.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/sdk.py` & `aiges-0.8.9/aiges/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -668,14 +668,15 @@
         for param in params:
             if param.required:
                 required_params.append(param.key)
             params_fields.update(param._schema())
             self.params_test_values.update()
             self.params_test_values[param.key] = param.test_value
         return params_fields, required_params
+
     def _parse_params_v2(self, serviceId, accepets_payloads):
         params = self.__mappings__.get('params', [])
         a_dict = {}
         _dict = {}
         for param in params:
             if isinstance(param, StringParamField):
                 if param.required:
@@ -695,16 +696,14 @@
 
             # if param.required:
             #     # todo param required should do here
             #     _dict[param.key] = param.test_value
             # else:
             #     _dict[param.key] = param.test_value
 
-
-
         # 这里是处理 accept parameters expect
         for k, v in accepets_payloads.items():
             _dict[k] = v
 
         TmpModel = create_model("TempModel", __base__=BaseModel, **_dict)
         a_dict[serviceId] = TmpModel()
 
@@ -937,15 +936,15 @@
     @param psrCnt 需要使用的个性化资源个数
 
     @return 接口错误码
         reqDat
         ret:错误码。无错误码时返回0
     '''
 
-    def wrapperOnceExec(cls, params: {}, reqData: DataListCls) -> Response:
+    def wrapperOnceExec(cls, params: {}, reqData: DataListCls, usrTag: str = "") -> Response:
         raise NotImplementedError(
             "Please Inplement Wrapper Class Method: wrapperOnceExec(cls, usrTag: str, params: {}, reqData: [], respData: [], psrIds: [], psrCnt: int) ")
 
     def wrapperOnceExecAsync(cls, params: {}, reqData: DataListCls, sid: str) -> Response:
         raise NotImplementedError(
             "Please Inplement Wrapper Class Method: wrapperOnceExec(cls, usrTag: str, params: {}, reqData: [], respData: [], psrIds: [], psrCnt: int) ")
```

### Comparing `aiges-0.8.8/aiges/serve.py` & `aiges-0.8.9/aiges/serve.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/server.py` & `aiges-0.8.9/aiges/server.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/server2.py` & `aiges-0.8.9/aiges/server2.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/stream.py` & `aiges-0.8.9/aiges/stream.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/test_data/flask_restx_test.py` & `aiges-0.8.9/aiges/test_data/flask_restx_test.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/test_data/pydantic_test.py` & `aiges-0.8.9/aiges/test_data/pydantic_test.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/test_data/test.png` & `aiges-0.8.9/aiges/test_data/test.png`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/test_data/testschma.json` & `aiges-0.8.9/aiges/test_data/testschma.json`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/tpls/Dockerfile.j2` & `aiges-0.8.9/aiges/tpls/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/tpls/wrapper.py.j2` & `aiges-0.8.9/aiges/tpls/wrapper.py.j2`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/utils/flask_utils.py` & `aiges-0.8.9/aiges/utils/flask_utils.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/utils/log.py` & `aiges-0.8.9/aiges/utils/log.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/worker.py` & `aiges-0.8.9/aiges/worker.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/wrapper.py` & `aiges-0.8.9/aiges/wrapper.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/wrapper_test.py` & `aiges-0.8.9/aiges/wrapper_test.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/ws/__init__.py` & `aiges-0.8.9/aiges/ws/__init__.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/ws/app.py` & `aiges-0.8.9/aiges/ws/app.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/ws/app2.py` & `aiges-0.8.9/aiges/ws/app2.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/ws/sample.json` & `aiges-0.8.9/aiges/ws/sample.json`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/ws/tests/__init__.py` & `aiges-0.8.9/aiges/ws/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/ws/tests/test_button.py` & `aiges-0.8.9/aiges/ws/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/ws/ws_client.py` & `aiges-0.8.9/aiges/ws/ws_client.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/aiges/ws/ws_client_test.py` & `aiges-0.8.9/aiges/ws/ws_client_test.py`

 * *Files identical despite different names*

### Comparing `aiges-0.8.8/pyproject.toml` & `aiges-0.8.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiges"
-version = "0.8.8"
+version = "0.8.9"
 description = "A module for test aiges's python wrapper.py"
 authors = ["maybaby <ybyang7@iflytek.com>"]
 license = "Apache License Version 2.0"
 [tool.poetry.dependencies]
 python = ">=3.6"
 jinja2 = ">=2.0"
 protobuf = ">=3.19"
```

### Comparing `aiges-0.8.8/setup.py` & `aiges-0.8.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
  'jsonref>=1.0.0',
  'plumbum>=1.7.0',
  'protobuf>=3.19',
  'pydantic>=1.8']
 
 setup_kwargs = {
     'name': 'aiges',
-    'version': '0.8.8',
+    'version': '0.8.9',
     'description': "A module for test aiges's python wrapper.py",
     'long_description': None,
     'author': 'maybaby',
     'author_email': 'ybyang7@iflytek.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `aiges-0.8.8/PKG-INFO` & `aiges-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiges
-Version: 0.8.8
+Version: 0.8.9
 Summary: A module for test aiges's python wrapper.py
 License: Apache License Version 2.0
 Author: maybaby
 Author-email: ybyang7@iflytek.com
 Requires-Python: >=3.6
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

