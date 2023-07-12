# Comparing `tmp/jupyterlab_pachyderm-2.7.0a4.tar.gz` & `tmp/jupyterlab_pachyderm-2.7.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_pachyderm-2.7.0a4.tar", last modified: Fri Jun 23 16:36:19 2023, max compression
+gzip compressed data, was "jupyterlab_pachyderm-2.7.0a5.tar", last modified: Wed Jul 12 20:56:47 2023, max compression
```

## Comparing `jupyterlab_pachyderm-2.7.0a4.tar` & `jupyterlab_pachyderm-2.7.0a5.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.369360 jupyterlab_pachyderm-2.7.0a4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11107 2023-06-23 16:36:19.369360 jupyterlab_pachyderm-2.7.0a4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10130 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/babel.config.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/install.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jest.config.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.345360 jupyterlab_pachyderm-2.7.0a4/jupyter-config/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.349360 jupyterlab_pachyderm-2.7.0a4/jupyter-config/nb-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyter-config/nb-config/jupyterlab_pachyderm.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.349360 jupyterlab_pachyderm-2.7.0a4/jupyter-config/server-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyter-config/server-config/jupyterlab_pachyderm.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.353360 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/dev_server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      649 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/env.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/filemanager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13073 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/handlers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.353360 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4412 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.345360 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/schemas/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.353360 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-06-23 16:36:06.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-06-23 16:36:06.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-06-23 16:36:06.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4270 2023-06-23 16:36:06.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-06-23 16:36:06.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.357360 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    70514 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)   401782 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   102166 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16896 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   161100 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/829.e9784d0c17729cab49a8.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8300 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/remoteEntry.70a21b765fbc6385e2db.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-06-23 16:36:06.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/style.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8183 2023-06-23 16:36:17.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/third-party-licenses.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/log.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11122 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/mount_server_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/pachyderm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9596 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/pps_client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.357360 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.357360 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/tests/data/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19829 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/tests/test_handlers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17560 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/tests/test_integrations.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.353360 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11107 2023-06-23 16:36:19.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4690 2023-06-23 16:36:19.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-23 16:36:19.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-23 16:35:49.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-06-23 16:36:19.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-06-23 16:36:19.000000 jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4270 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/pyproject.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.357360 jupyterlab_pachyderm-2.7.0a4/schema/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/schema/examples.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/schema/help.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/schema/mount.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/schema/telemetry.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2023-06-23 16:36:19.369360 jupyterlab_pachyderm-2.7.0a4/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2260 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.357360 jupyterlab_pachyderm-2.7.0a4/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/global.d.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/handler.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.345360 jupyterlab_pachyderm-2.7.0a4/src/plugins/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/examples/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/examples/__test__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/examples/__test__/examples.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/examples/examples.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/examples/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/help/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/help/__tests__/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/help/__tests__/__snapshots__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1937 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/help/__tests__/help.test.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/help/help.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/help/help.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/help/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6919 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/__tests__/mount.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.345360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8530 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Config/Config.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Config/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12024 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Config/__tests__/Config.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Config/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Config/hooks/useConfig.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Datum/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4675 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Datum/Datum.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Datum/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7511 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Datum/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6182 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Datum/hooks/useDatum.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/FullPageError/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1012 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/FullPageError/FullPageError.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.361360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/FullPageError/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6365 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/Pipeline.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/Splash.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3528 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4308 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/SortableList/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3730 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/SortableList/ListMount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5159 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/SortableList/ListUnmount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3498 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/SortableList/SortableList.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/SortableList/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15391 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2984 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/customFileBrowser.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1488 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8702 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/mount.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22029 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/mount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2993 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/mountDrive.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4382 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/pollMounts.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2763 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/types.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/plugins/telemetry/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/plugins/telemetry/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/telemetry/__tests__/telemetry.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/telemetry/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/plugins/telemetry/telemetry.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/setupTests.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/utils/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.345360 jupyterlab_pachyderm-2.7.0a4/src/utils/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/utils/components/Circle/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/components/Circle/Circle.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/components/Circle/circle.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/utils/components/LoadingDots/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/components/LoadingDots/LoadingDots.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/components/LoadingDots/loadingDots.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.365360 jupyterlab_pachyderm-2.7.0a4/src/utils/components/Svgs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26381 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/components/Svgs/GenericError.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    74288 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/components/Svgs/KubernetesElephant.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16523 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/components/Svgs/PachydermLogo.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/components/Svgs/StatusWarning.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/components/Svgs/index.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.369360 jupyterlab_pachyderm-2.7.0a4/src/utils/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/hooks/usePreviousValue.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/hooks/useSort.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      675 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/icons.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/src/utils/testUtils.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.369360 jupyterlab_pachyderm-2.7.0a4/style/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/style/base.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.369360 jupyterlab_pachyderm-2.7.0a4/style/components/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1524 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/style/components/button.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/style/components/input.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 16:36:19.369360 jupyterlab_pachyderm-2.7.0a4/style/icons/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/style/icons/file.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/style/icons/info.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/style/icons/mount-logo.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/style/icons/repo.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/style/index.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/style/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-06-23 16:33:48.000000 jupyterlab_pachyderm-2.7.0a4/tsconfig.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.160294 jupyterlab_pachyderm-2.7.0a5/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11107 2023-07-12 20:56:47.160294 jupyterlab_pachyderm-2.7.0a5/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10130 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/babel.config.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/install.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jest.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.136294 jupyterlab_pachyderm-2.7.0a5/jupyter-config/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.140294 jupyterlab_pachyderm-2.7.0a5/jupyter-config/nb-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyter-config/nb-config/jupyterlab_pachyderm.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.140294 jupyterlab_pachyderm-2.7.0a5/jupyter-config/server-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyter-config/server-config/jupyterlab_pachyderm.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.144294 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/dev_server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      649 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/env.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/filemanager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13073 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/handlers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.144294 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4412 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.136294 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/schemas/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.144294 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-07-12 20:56:33.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-07-12 20:56:33.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-07-12 20:56:33.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4270 2023-07-12 20:56:33.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-07-12 20:56:33.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.148294 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    70514 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   401782 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   102166 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16896 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   161098 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/829.7feefb314c4865d398d2.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8296 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/remoteEntry.b44c82c4e0aece4113cd.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-07-12 20:56:33.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/style.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8183 2023-07-12 20:56:45.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/third-party-licenses.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/log.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11122 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/mount_server_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/pachyderm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9596 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/pps_client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.148294 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.148294 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/tests/data/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19829 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/tests/test_handlers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17560 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/tests/test_integrations.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.144294 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11107 2023-07-12 20:56:47.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4690 2023-07-12 20:56:47.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-12 20:56:47.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-12 20:56:16.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-07-12 20:56:47.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-07-12 20:56:47.000000 jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4270 2023-07-12 20:54:18.000000 jupyterlab_pachyderm-2.7.0a5/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/pyproject.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.148294 jupyterlab_pachyderm-2.7.0a5/schema/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/schema/examples.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/schema/help.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/schema/mount.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/schema/telemetry.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2023-07-12 20:56:47.160294 jupyterlab_pachyderm-2.7.0a5/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2260 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.148294 jupyterlab_pachyderm-2.7.0a5/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/global.d.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/handler.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.140294 jupyterlab_pachyderm-2.7.0a5/src/plugins/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/examples/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/examples/__test__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/examples/__test__/examples.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/examples/examples.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/examples/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/help/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/help/__tests__/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/help/__tests__/__snapshots__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1937 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/help/__tests__/help.test.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/help/help.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/help/help.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/help/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6919 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/__tests__/mount.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.140294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8530 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Config/Config.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Config/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12024 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Config/__tests__/Config.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Config/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Config/hooks/useConfig.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Datum/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4675 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Datum/Datum.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Datum/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7511 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Datum/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6182 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Datum/hooks/useDatum.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/FullPageError/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1012 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/FullPageError/FullPageError.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/FullPageError/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6365 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/Pipeline.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/Splash.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.152294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3528 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4308 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/SortableList/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3730 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/SortableList/ListMount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5159 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/SortableList/ListUnmount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3498 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/SortableList/SortableList.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/SortableList/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15391 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2984 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/customFileBrowser.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1488 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8702 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/mount.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22029 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/mount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2993 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/mountDrive.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4382 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/pollMounts.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2763 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/types.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/src/plugins/telemetry/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/src/plugins/telemetry/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/telemetry/__tests__/telemetry.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/telemetry/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/plugins/telemetry/telemetry.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/setupTests.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/src/utils/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.140294 jupyterlab_pachyderm-2.7.0a5/src/utils/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/src/utils/components/Circle/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/components/Circle/Circle.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/components/Circle/circle.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/src/utils/components/LoadingDots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/components/LoadingDots/LoadingDots.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/components/LoadingDots/loadingDots.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/src/utils/components/Svgs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26381 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/components/Svgs/GenericError.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74288 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/components/Svgs/KubernetesElephant.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16523 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/components/Svgs/PachydermLogo.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/components/Svgs/StatusWarning.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/components/Svgs/index.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/src/utils/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/hooks/usePreviousValue.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/hooks/useSort.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      675 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/icons.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/src/utils/testUtils.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.156294 jupyterlab_pachyderm-2.7.0a5/style/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/style/base.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.160294 jupyterlab_pachyderm-2.7.0a5/style/components/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1524 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/style/components/button.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/style/components/input.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 20:56:47.160294 jupyterlab_pachyderm-2.7.0a5/style/icons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/style/icons/file.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/style/icons/info.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/style/icons/mount-logo.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/style/icons/repo.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/style/index.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/style/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-07-12 20:54:17.000000 jupyterlab_pachyderm-2.7.0a5/tsconfig.json
```

### Comparing `jupyterlab_pachyderm-2.7.0a4/LICENSE` & `jupyterlab_pachyderm-2.7.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/MANIFEST.in` & `jupyterlab_pachyderm-2.7.0a5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/PKG-INFO` & `jupyterlab_pachyderm-2.7.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_pachyderm
-Version: 2.7.0a4
+Version: 2.7.0a5
 Summary: A JupyterLab extension.
 Home-page: https://github.com/pachyderm/jupyterlab-pachyderm
 Author: 
 Author-email: 
 License: BSD-3-Clause
 Keywords: jupyter,jupyterlab,jupyterlab-extension
 Platform: Linux
```

### Comparing `jupyterlab_pachyderm-2.7.0a4/README.md` & `jupyterlab_pachyderm-2.7.0a5/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/__init__.py` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/_version.py` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/_version.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/env.py` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/env.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/handlers.py` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/package.json` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222223%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'2.7.0-alpha.5'"}*

```diff
@@ -66,19 +66,14 @@
             "before-build-npm": [
                 "python -m pip install jupyterlab~=3.1",
                 "npm"
             ]
         }
     },
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.70a21b765fbc6385e2db.js",
-            "style": "./style"
-        },
         "disabledExtensions": [
             "jupyterlab-pachyderm:examples"
         ],
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_pachyderm"
@@ -133,9 +128,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.7.0-alpha.4"
+    "version": "2.7.0-alpha.5"
 }
```

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig` & `jupyterlab_pachyderm-2.7.0a5/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'2.7.0-alpha.5'"}*

```diff
@@ -128,9 +128,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.7.0-alpha.4"
+    "version": "2.7.0-alpha.5"
 }
```

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/829.e9784d0c17729cab49a8.js` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/829.7feefb314c4865d398d2.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -20,18 +20,18 @@
                 i = {
                     id: "jupyterlab-pachyderm:telemetry",
                     autoStart: !0,
                     activate: e => {
                         (0, l.load)("20C6D2xFLRmyFTqtvYDEgNfwcRG", "https://pachyderm-dataplane.rudderstack.com"), window.document.onclick !== s && window.document.addEventListener("click", s)
                     }
                 };
-            var c = a(6308),
+            var c = a(8535),
                 o = a(6271),
                 m = a.n(o),
-                d = a(9764);
+                d = a(6303);
             const u = e => o.createElement("svg", Object.assign({
                 xmlns: "http://www.w3.org/2000/svg",
                 xmlnsXlink: "http://www.w3.org/1999/xlink",
                 viewBox: "0 0 100 170"
             }, e), o.createElement("defs", null, o.createElement("linearGradient", {
                 id: "pachydermLogo_svg__b",
                 x1: "90.51%",
@@ -301,18 +301,18 @@
                             command: h.openDocs
                         }, {
                             command: h.contactSupport
                         }], 20))
                     })(e, t)
                 }
             };
-            var f = a(579),
-                E = a(3058),
-                _ = a(1872),
-                g = a(8667);
+            var f = a(9071),
+                E = a(344),
+                _ = a(5139),
+                g = a(1745);
             const v = new g.LabIcon({
                     name: "jupyterlab-pachyderm:file",
                     svgstr: '<svg  viewBox="0 0 21 31" width="21px" height="31px" xmlns="http://www.w3.org/2000/svg">\n  <path d="M.85.001C.365.055-.003.491 0 1.008v28.19c0 .556.425 1.007.95 1.007h18.98c.524 0 .949-.45.949-1.007V6.608a1.04 1.04 0 00-.277-.713l-5.299-5.6a.923.923 0 00-.662-.294H.949a.895.895 0 00-.099 0zm1.048 2.014h11.705v4.698c0 .556.425 1.007.949 1.007h4.429v20.472H1.898V2.015zm13.603 1.332l2.234 2.36h-2.234v-2.36zM4.646 12.083a.949.949 0 00-.797.549c-.154.32-.135.704.05 1.007a.935.935 0 00.846.457h6.327a.94.94 0 00.833-.499 1.06 1.06 0 000-1.015.94.94 0 00-.833-.5H4.745a.895.895 0 00-.099 0zm0 4.698a.949.949 0 00-.797.549c-.154.32-.135.705.05 1.007a.935.935 0 00.846.458h11.389a.94.94 0 00.833-.5 1.06 1.06 0 000-1.015.94.94 0 00-.833-.499H4.745a.895.895 0 00-.099 0zm0 4.699a.949.949 0 00-.797.548c-.154.321-.135.705.05 1.007a.935.935 0 00.846.458h11.389a.94.94 0 00.833-.5 1.06 1.06 0 000-1.014.94.94 0 00-.833-.5H4.745a.895.895 0 00-.099 0z" fill="#582F6B" fill-rule="nonzero"/>\n</svg>\n'
                 }),
                 k = new g.LabIcon({
                     name: "jupyterlab-pachyderm:mount-logo",
                     svgstr: '<?xml version="1.0" encoding="UTF-8"?>\n<svg width="20px" height="20px" viewBox="0 0 20 20" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">\n    <defs>\n        <path d="M14,13 L14,17.041 L10,19 L6,17.041 L6,13 L10,14.8365 L14,13 Z M10,10 L14,12.0852339 L10,14 L6,12.0852339 L10,10 Z M10.9899912,1 L10.9899912,5.72256 L12.5999411,4.16117749 L14,5.51882251 L10.7000295,8.71882251 C10.3617408,9.04686292 9.83953975,9.08786797 9.455273,8.84183766 L9.37515866,8.78472348 L9.29997054,8.71882251 L6,5.51882251 L7.40005893,4.16117749 L9.01000884,5.72256 L9.01000884,1 L10.9899912,1 Z" id="path-1"></path>\n    </defs>\n    <g id="Icons" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">\n        <g id="Icon/notebook-mount/black">\n            <rect id="Bounding-Box"  class="jp-icon3" fill-opacity="0" fill="#FFFFFF" x="0" y="0" width="20" height="20"></rect>\n            <mask id="mask-2" fill="white">\n                <use xlink:href="#path-1"></use>\n            </mask>\n            <use id="Combined-Shape" fill="#926AA1" fill-rule="nonzero" xlink:href="#path-1"></use>\n            <g class="jp-icon3" id="Group" mask="url(#mask-2)" fill="#0F1012">\n                <g id="Color">\n                    <rect x="0" y="0" width="20" height="20"></rect>\n                </g>\n            </g>\n        </g>\n    </g>\n</svg>'
@@ -386,19 +386,19 @@
                                 command: e.command,
                                 category: "Pachyderm Examples",
                                 rank: e.rank
                             }))
                         })))(a, e, t))))
                     })))(e, t)
                 };
-            var C = a(6175),
-                M = a(9263),
-                S = a(680),
-                z = a(4085),
-                L = a(6779),
+            var C = a(7638),
+                M = a(931),
+                S = a(122),
+                z = a(8299),
+                L = a(127),
                 N = a(1840),
                 B = a(8832),
                 O = a(3114);
 
             function D(e = "", t = "GET", a = null, n = "pachyderm/v2") {
                 return r = this, l = void 0, i = function*() {
                     const r = _.ServerConnection.makeSettings(),
```

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/remoteEntry.70a21b765fbc6385e2db.js` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/remoteEntry.b44c82c4e0aece4113cd.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -49,22 +49,22 @@
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         67: "9d3e2934cfe0e102619e",
         371: "8ac933b7fbb0f688b6f4",
         486: "003d1d2cc9cc6927471e",
         676: "95f9b834e9f9b133c00b",
         747: "b62f963856036a13fba1",
-        829: "e9784d0c17729cab49a8"
+        829: "7feefb314c4865d398d2"
     } [e] + ".js?v=" + {
         67: "9d3e2934cfe0e102619e",
         371: "8ac933b7fbb0f688b6f4",
         486: "003d1d2cc9cc6927471e",
         676: "95f9b834e9f9b133c00b",
         747: "b62f963856036a13fba1",
-        829: "e9784d0c17729cab49a8"
+        829: "7feefb314c4865d398d2"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -116,15 +116,15 @@
                         (!u || !u.loaded && (!a != !u.eager ? a : l > u.from)) && (n[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     i = [];
-                return "default" === t && (u("jupyterlab-pachyderm", "2.7.0-alpha.4", (() => Promise.all([j.e(371), j.e(829)]).then((() => () => j(7363))))), u("lodash", "4.17.21", (() => j.e(486).then((() => () => j(6486))))), u("rudder-sdk-js", "1.2.5", (() => j.e(67).then((() => () => j(3067))))), u("yaml", "0", (() => j.e(676).then((() => () => j(5676)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("jupyterlab-pachyderm", "2.7.0-alpha.5", (() => Promise.all([j.e(371), j.e(829)]).then((() => () => j(7363))))), u("lodash", "4.17.21", (() => j.e(486).then((() => () => j(6486))))), u("rudder-sdk-js", "1.2.5", (() => j.e(67).then((() => () => j(3067))))), u("yaml", "0", (() => j.e(676).then((() => () => j(5676)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -221,36 +221,36 @@
     }, s = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, a, n) {
         var o = j.I(r);
         return o && o.then ? o.then(e.bind(e, r, j.S[r], t, a, n)) : e(r, j.S[r], t, a, n)
     })(((e, r, t, a) => (l(e, t), d(r, 0, t, a)))), h = p(((e, r, t, a, n) => {
         var o = r && j.o(r, t) && f(r, t, a);
         return o ? s(o) : n()
     })), b = {}, v = {
-        579: () => c("default", "@jupyterlab/launcher", [1, 3, 6, 4]),
-        680: () => c("default", "@jupyterlab/filebrowser", [1, 3, 6, 4]),
+        122: () => c("default", "@jupyterlab/filebrowser", [1, 3, 6, 5]),
+        127: () => c("default", "@jupyterlab/notebook", [1, 3, 6, 5]),
+        344: () => c("default", "@jupyterlab/coreutils", [1, 5, 6, 5]),
         930: () => h("default", "yaml", [1, 2, 1, 1], (() => j.e(676).then((() => () => j(5676))))),
+        931: () => c("default", "@jupyterlab/docmanager", [1, 3, 6, 5]),
         1526: () => c("default", "@lumino/coreutils", [1, 1, 11, 0]),
+        1745: () => c("default", "@jupyterlab/ui-components", [1, 3, 6, 5]),
         1840: () => c("default", "@lumino/signaling", [1, 1, 10, 0]),
-        1872: () => c("default", "@jupyterlab/services", [1, 6, 6, 4]),
-        3058: () => c("default", "@jupyterlab/coreutils", [1, 5, 6, 4]),
-        4085: () => c("default", "@jupyterlab/settingregistry", [1, 3, 6, 4]),
         4234: () => h("default", "rudder-sdk-js", [1, 1, 2, 1], (() => j.e(67).then((() => () => j(3067))))),
         4439: () => h("default", "lodash", [1, 4, 17, 21], (() => j.e(486).then((() => () => j(6486))))),
+        5139: () => c("default", "@jupyterlab/services", [1, 6, 6, 5]),
         6057: () => c("default", "@lumino/commands", [1, 1, 19, 0]),
-        6175: () => c("default", "@jupyterlab/application", [1, 3, 6, 4]),
         6271: () => c("default", "react", [1, 17, 0, 1]),
-        6308: () => c("default", "@jupyterlab/mainmenu", [1, 3, 6, 4]),
-        6779: () => c("default", "@jupyterlab/notebook", [1, 3, 6, 4]),
-        8667: () => c("default", "@jupyterlab/ui-components", [1, 3, 6, 4]),
+        6303: () => c("default", "@jupyterlab/apputils", [1, 3, 6, 5]),
+        7638: () => c("default", "@jupyterlab/application", [1, 3, 6, 5]),
+        8299: () => c("default", "@jupyterlab/settingregistry", [1, 3, 6, 5]),
+        8535: () => c("default", "@jupyterlab/mainmenu", [1, 3, 6, 5]),
         8832: () => c("default", "@lumino/widgets", [1, 1, 37, 2]),
         8918: () => c("default", "@lumino/algorithm", [1, 1, 9, 0]),
-        9263: () => c("default", "@jupyterlab/docmanager", [1, 3, 6, 4]),
-        9764: () => c("default", "@jupyterlab/apputils", [1, 3, 6, 4])
+        9071: () => c("default", "@jupyterlab/launcher", [1, 3, 6, 5])
     }, m = {
-        829: [579, 680, 930, 1526, 1840, 1872, 3058, 4085, 4234, 4439, 6057, 6175, 6271, 6308, 6779, 8667, 8832, 8918, 9263, 9764]
+        829: [122, 127, 344, 930, 931, 1526, 1745, 1840, 4234, 4439, 5139, 6057, 6271, 6303, 7638, 8299, 8535, 8832, 8918, 9071]
     }, j.f.consumes = (e, r) => {
         j.o(m, e) && m[e].forEach((e => {
             if (j.o(b, e)) return r.push(b[e]);
             var t = r => {
                     b[e] = 0, j.m[e] = t => {
                         delete j.c[e], t.exports = r()
                     }
```

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/labextension/static/third-party-licenses.json` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/mount_server_client.py` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/mount_server_client.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/pachyderm.py` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/pachyderm.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/pps_client.py` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/pps_client.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/tests/test_handlers.py` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm/tests/test_integrations.py` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm.egg-info/PKG-INFO` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-pachyderm
-Version: 2.7.0a4
+Version: 2.7.0a5
 Summary: A JupyterLab extension.
 Home-page: https://github.com/pachyderm/jupyterlab-pachyderm
 Author: 
 Author-email: 
 License: BSD-3-Clause
 Keywords: jupyter,jupyterlab,jupyterlab-extension
 Platform: Linux
```

### Comparing `jupyterlab_pachyderm-2.7.0a4/jupyterlab_pachyderm.egg-info/SOURCES.txt` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
 jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
 jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
 jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
 jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
 jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
 jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
-jupyterlab_pachyderm/labextension/static/829.e9784d0c17729cab49a8.js
-jupyterlab_pachyderm/labextension/static/remoteEntry.70a21b765fbc6385e2db.js
+jupyterlab_pachyderm/labextension/static/829.7feefb314c4865d398d2.js
+jupyterlab_pachyderm/labextension/static/remoteEntry.b44c82c4e0aece4113cd.js
 jupyterlab_pachyderm/labextension/static/style.js
 jupyterlab_pachyderm/labextension/static/third-party-licenses.json
 jupyterlab_pachyderm/tests/__init__.py
 jupyterlab_pachyderm/tests/test_handlers.py
 jupyterlab_pachyderm/tests/test_integrations.py
 jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
 jupyterlab_pachyderm/tests/data/requirements.txt
```

### Comparing `jupyterlab_pachyderm-2.7.0a4/package.json` & `jupyterlab_pachyderm-2.7.0a5/jupyterlab_pachyderm/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222223%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.b44c82c4e0aece4113cd.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'2.7.0-alpha.5'"}*

```diff
@@ -66,14 +66,19 @@
             "before-build-npm": [
                 "python -m pip install jupyterlab~=3.1",
                 "npm"
             ]
         }
     },
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.b44c82c4e0aece4113cd.js",
+            "style": "./style"
+        },
         "disabledExtensions": [
             "jupyterlab-pachyderm:examples"
         ],
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_pachyderm"
@@ -128,9 +133,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.7.0-alpha.4"
+    "version": "2.7.0-alpha.5"
 }
```

### Comparing `jupyterlab_pachyderm-2.7.0a4/pyproject.toml` & `jupyterlab_pachyderm-2.7.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/setup.cfg` & `jupyterlab_pachyderm-2.7.0a5/setup.cfg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/setup.py` & `jupyterlab_pachyderm-2.7.0a5/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/handler.ts` & `jupyterlab_pachyderm-2.7.0a5/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/examples/__test__/examples.test.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/examples/__test__/examples.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/examples/examples.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/examples/examples.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/help/__tests__/help.test.ts` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/help/__tests__/help.test.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/help/help.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/help/help.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/__tests__/mount.test.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/__tests__/mount.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Config/Config.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Config/Config.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Config/__tests__/Config.test.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Config/__tests__/Config.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Config/hooks/useConfig.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Config/hooks/useConfig.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Datum/Datum.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Datum/Datum.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Datum/hooks/useDatum.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Datum/hooks/useDatum.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/FullPageError/FullPageError.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/FullPageError/FullPageError.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/Pipeline.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/Pipeline.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/Splash.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/Splash.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/SortableList/ListMount.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/SortableList/ListMount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/SortableList/ListUnmount.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/SortableList/ListUnmount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/SortableList/SortableList.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/SortableList/SortableList.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/customFileBrowser.ts` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/customFileBrowser.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/index.ts` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/mount.css` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/mount.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/mount.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/mount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/mountDrive.ts` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/mountDrive.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/pollMounts.ts` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/pollMounts.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/mount/types.ts` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/mount/types.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/telemetry/__tests__/telemetry.test.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/telemetry/__tests__/telemetry.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/plugins/telemetry/telemetry.ts` & `jupyterlab_pachyderm-2.7.0a5/src/plugins/telemetry/telemetry.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/utils/components/Circle/Circle.tsx` & `jupyterlab_pachyderm-2.7.0a5/src/utils/components/Circle/Circle.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/utils/components/LoadingDots/loadingDots.css` & `jupyterlab_pachyderm-2.7.0a5/src/utils/components/LoadingDots/loadingDots.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/utils/components/Svgs/GenericError.js` & `jupyterlab_pachyderm-2.7.0a5/src/utils/components/Svgs/GenericError.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/utils/components/Svgs/KubernetesElephant.js` & `jupyterlab_pachyderm-2.7.0a5/src/utils/components/Svgs/KubernetesElephant.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/utils/components/Svgs/PachydermLogo.js` & `jupyterlab_pachyderm-2.7.0a5/src/utils/components/Svgs/PachydermLogo.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/utils/components/Svgs/StatusWarning.js` & `jupyterlab_pachyderm-2.7.0a5/src/utils/components/Svgs/StatusWarning.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/utils/hooks/useSort.ts` & `jupyterlab_pachyderm-2.7.0a5/src/utils/hooks/useSort.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/src/utils/icons.ts` & `jupyterlab_pachyderm-2.7.0a5/src/utils/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/style/base.css` & `jupyterlab_pachyderm-2.7.0a5/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/style/components/button.css` & `jupyterlab_pachyderm-2.7.0a5/style/components/button.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/style/icons/file.svg` & `jupyterlab_pachyderm-2.7.0a5/style/icons/file.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/style/icons/info.svg` & `jupyterlab_pachyderm-2.7.0a5/style/icons/info.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/style/icons/mount-logo.svg` & `jupyterlab_pachyderm-2.7.0a5/style/icons/mount-logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.7.0a4/style/icons/repo.svg` & `jupyterlab_pachyderm-2.7.0a5/style/icons/repo.svg`

 * *Files identical despite different names*

