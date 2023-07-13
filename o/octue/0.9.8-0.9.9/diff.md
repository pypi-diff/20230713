# Comparing `tmp/octue-0.9.8.tar.gz` & `tmp/octue-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octue-0.9.8.tar", last modified: Tue Feb  1 12:42:27 2022, max compression
+gzip compressed data, was "octue-0.9.9.tar", last modified: Tue Feb  1 15:51:46 2022, max compression
```

## Comparing `octue-0.9.8.tar` & `octue-0.9.9.tar`

### file list

```diff
@@ -1,228 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.713121 octue-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-02-01 12:42:21.000000 octue-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-02-01 12:42:21.000000 octue-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7170 2022-02-01 12:42:27.713121 octue-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6384 2022-02-01 12:42:21.000000 octue-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.693120 octue-0.9.8/octue/
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-02-01 12:42:21.000000 octue-0.9.8/octue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11130 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.697120 octue-0.9.8/octue/cloud/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2992 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.697120 octue-0.9.8/octue/cloud/deployment/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/deployment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.697120 octue-0.9.8/octue/cloud/deployment/google/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/deployment/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3606 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/deployment/google/answer_pub_sub_question.py
--rw-r--r--   0 runner    (1001) docker     (121)    14266 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/deployment/google/base_deployer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.697120 octue-0.9.8/octue/cloud/deployment/google/cloud_run/
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/deployment/google/cloud_run/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/deployment/google/cloud_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10687 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/deployment/google/cloud_run/deployer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1653 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/deployment/google/cloud_run/flask_app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.697120 octue-0.9.8/octue/cloud/deployment/google/dataflow/
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/deployment/google/dataflow/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/deployment/google/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8190 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/deployment/google/dataflow/deployer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4029 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/deployment/google/dataflow/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)     2857 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/emulators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.697120 octue-0.9.8/octue/cloud/pub_sub/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/pub_sub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/pub_sub/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     9458 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/pub_sub/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)    17874 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/pub_sub/service.py
--rw-r--r--   0 runner    (1001) docker     (121)     5755 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/pub_sub/subscription.py
--rw-r--r--   0 runner    (1001) docker     (121)     3001 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/pub_sub/topic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.697120 octue-0.9.8/octue/cloud/storage/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14448 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/storage/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2359 2022-02-01 12:42:21.000000 octue-0.9.8/octue/cloud/storage/path.py
--rw-r--r--   0 runner    (1001) docker     (121)      875 2022-02-01 12:42:21.000000 octue-0.9.8/octue/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.697120 octue-0.9.8/octue/essentials/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/octue/essentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-02-01 12:42:21.000000 octue-0.9.8/octue/essentials/monitor_messages.py
--rw-r--r--   0 runner    (1001) docker     (121)     3828 2022-02-01 12:42:21.000000 octue-0.9.8/octue/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6119 2022-02-01 12:42:21.000000 octue-0.9.8/octue/log_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.697120 octue-0.9.8/octue/mixins/
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-02-01 12:42:21.000000 octue-0.9.8/octue/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-02-01 12:42:21.000000 octue-0.9.8/octue/mixins/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      569 2022-02-01 12:42:21.000000 octue-0.9.8/octue/mixins/cool_nameable.py
--rw-r--r--   0 runner    (1001) docker     (121)     9513 2022-02-01 12:42:21.000000 octue-0.9.8/octue/mixins/filterable.py
--rw-r--r--   0 runner    (1001) docker     (121)     3551 2022-02-01 12:42:21.000000 octue-0.9.8/octue/mixins/hashable.py
--rw-r--r--   0 runner    (1001) docker     (121)     2263 2022-02-01 12:42:21.000000 octue-0.9.8/octue/mixins/identifiable.py
--rw-r--r--   0 runner    (1001) docker     (121)      721 2022-02-01 12:42:21.000000 octue-0.9.8/octue/mixins/labelable.py
--rw-r--r--   0 runner    (1001) docker     (121)     3372 2022-02-01 12:42:21.000000 octue-0.9.8/octue/mixins/pathable.py
--rw-r--r--   0 runner    (1001) docker     (121)     4116 2022-02-01 12:42:21.000000 octue-0.9.8/octue/mixins/serialisable.py
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-02-01 12:42:21.000000 octue-0.9.8/octue/mixins/taggable.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.701121 octue-0.9.8/octue/resources/
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-02-01 12:42:21.000000 octue-0.9.8/octue/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7263 2022-02-01 12:42:21.000000 octue-0.9.8/octue/resources/analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     2759 2022-02-01 12:42:21.000000 octue-0.9.8/octue/resources/child.py
--rw-r--r--   0 runner    (1001) docker     (121)    27985 2022-02-01 12:42:21.000000 octue-0.9.8/octue/resources/datafile.py
--rw-r--r--   0 runner    (1001) docker     (121)    11080 2022-02-01 12:42:21.000000 octue-0.9.8/octue/resources/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     8779 2022-02-01 12:42:21.000000 octue-0.9.8/octue/resources/filter_containers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3673 2022-02-01 12:42:21.000000 octue-0.9.8/octue/resources/label.py
--rw-r--r--   0 runner    (1001) docker     (121)     8628 2022-02-01 12:42:21.000000 octue-0.9.8/octue/resources/manifest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2138 2022-02-01 12:42:21.000000 octue-0.9.8/octue/resources/service_backends.py
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-02-01 12:42:21.000000 octue-0.9.8/octue/resources/tag.py
--rw-r--r--   0 runner    (1001) docker     (121)    15597 2022-02-01 12:42:21.000000 octue-0.9.8/octue/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.701121 octue-0.9.8/octue/templates/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.693120 octue-0.9.8/octue/templates/template-child-services/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.701121 octue-0.9.8/octue/templates/template-child-services/elevation_service/
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-child-services/elevation_service/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-child-services/elevation_service/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.693120 octue-0.9.8/octue/templates/template-child-services/elevation_service/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.701121 octue-0.9.8/octue/templates/template-child-services/elevation_service/data/configuration/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-child-services/elevation_service/data/configuration/values.json
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-child-services/elevation_service/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-child-services/elevation_service/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1757 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-child-services/elevation_service/twine.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.701121 octue-0.9.8/octue/templates/template-child-services/parent_service/
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-child-services/parent_service/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2507 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-child-services/parent_service/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.693120 octue-0.9.8/octue/templates/template-child-services/parent_service/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.701121 octue-0.9.8/octue/templates/template-child-services/parent_service/data/configuration/
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-child-services/parent_service/data/configuration/children.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.701121 octue-0.9.8/octue/templates/template-child-services/parent_service/data/input/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-child-services/parent_service/data/input/values.json
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-child-services/parent_service/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-child-services/parent_service/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1345 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-child-services/parent_service/twine.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.701121 octue-0.9.8/octue/templates/template-child-services/wind_speed_service/
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-child-services/wind_speed_service/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-child-services/wind_speed_service/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.693120 octue-0.9.8/octue/templates/template-child-services/wind_speed_service/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.701121 octue-0.9.8/octue/templates/template-child-services/wind_speed_service/data/configuration/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-child-services/wind_speed_service/data/configuration/values.json
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-child-services/wind_speed_service/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-child-services/wind_speed_service/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1755 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-child-services/wind_speed_service/twine.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.701121 octue-0.9.8/octue/templates/template-python-fractal/
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-python-fractal/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2971 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-python-fractal/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.693120 octue-0.9.8/octue/templates/template-python-fractal/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.705121 octue-0.9.8/octue/templates/template-python-fractal/data/configuration/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-python-fractal/data/configuration/configuration_values.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.705121 octue-0.9.8/octue/templates/template-python-fractal/fractal/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-python-fractal/fractal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3793 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-python-fractal/fractal/fractal.py
--rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-python-fractal/fractal/mandelbrot.py
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-python-fractal/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-python-fractal/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1870 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-python-fractal/twine.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.705121 octue-0.9.8/octue/templates/template-using-manifests/
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-using-manifests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     5480 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-using-manifests/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.705121 octue-0.9.8/octue/templates/template-using-manifests/cleaner/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-using-manifests/cleaner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-using-manifests/cleaner/clean.py
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-using-manifests/cleaner/read_csv_files.py
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-using-manifests/cleaner/read_dat_file.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.693120 octue-0.9.8/octue/templates/template-using-manifests/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.705121 octue-0.9.8/octue/templates/template-using-manifests/data/configuration/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-using-manifests/data/configuration/values.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.705121 octue-0.9.8/octue/templates/template-using-manifests/data/input/
--rw-r--r--   0 runner    (1001) docker     (121)     1582 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-using-manifests/data/input/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.693120 octue-0.9.8/octue/templates/template-using-manifests/data/input/raw_met_mast_data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.705121 octue-0.9.8/octue/templates/template-using-manifests/data/input/raw_met_mast_data/08DEC/
--rw-r--r--   0 runner    (1001) docker     (121)     4444 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-using-manifests/data/input/raw_met_mast_data/08DEC/High Res Meteorological Mast Data - 8 Dec_1.csv
--rw-r--r--   0 runner    (1001) docker     (121)     4472 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-using-manifests/data/input/raw_met_mast_data/08DEC/High Res Meteorological Mast Data - 8 Dec_2.csv
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-using-manifests/data/input/raw_met_mast_data/08DEC/meta - 8 Dec.dat
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-using-manifests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-using-manifests/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      791 2022-02-01 12:42:21.000000 octue-0.9.8/octue/templates/template-using-manifests/twine.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.705121 octue-0.9.8/octue/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-02-01 12:42:21.000000 octue-0.9.8/octue/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      936 2022-02-01 12:42:21.000000 octue-0.9.8/octue/utils/decoders.py
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-02-01 12:42:21.000000 octue-0.9.8/octue/utils/encoders.py
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-02-01 12:42:21.000000 octue-0.9.8/octue/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      761 2022-02-01 12:42:21.000000 octue-0.9.8/octue/utils/folders.py
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-02-01 12:42:21.000000 octue-0.9.8/octue/utils/gen_uuid.py
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-02-01 12:42:21.000000 octue-0.9.8/octue/utils/isfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-02-01 12:42:21.000000 octue-0.9.8/octue/utils/isfolder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1558 2022-02-01 12:42:21.000000 octue-0.9.8/octue/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)     1472 2022-02-01 12:42:21.000000 octue-0.9.8/octue/utils/persistence.py
--rw-r--r--   0 runner    (1001) docker     (121)     1699 2022-02-01 12:42:21.000000 octue-0.9.8/octue/utils/processes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.697120 octue-0.9.8/octue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7170 2022-02-01 12:42:27.000000 octue-0.9.8/octue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7209 2022-02-01 12:42:27.000000 octue-0.9.8/octue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-01 12:42:27.000000 octue-0.9.8/octue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-02-01 12:42:27.000000 octue-0.9.8/octue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-01 12:42:27.000000 octue-0.9.8/octue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-02-01 12:42:27.000000 octue-0.9.8/octue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-01 12:42:27.000000 octue-0.9.8/octue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-02-01 12:42:27.713121 octue-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-02-01 12:42:21.000000 octue-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.693120 octue-0.9.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.705121 octue-0.9.8/tests/cloud/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.705121 octue-0.9.8/tests/cloud/deployment/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/deployment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.705121 octue-0.9.8/tests/cloud/deployment/google/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/deployment/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.709121 octue-0.9.8/tests/cloud/deployment/google/cloud_run/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/deployment/google/cloud_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12414 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/deployment/google/cloud_run/test_cloud_run_deployer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1692 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/deployment/google/cloud_run/test_cloud_run_deployment.py
--rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/deployment/google/cloud_run/test_flask_app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.709121 octue-0.9.8/tests/cloud/deployment/google/dataflow/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/deployment/google/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14004 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/deployment/google/dataflow/test_dataflow_deployer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/deployment/google/dataflow/test_dataflow_deployment.py
--rw-r--r--   0 runner    (1001) docker     (121)     4853 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/deployment/google/test_answer_pub_sub_question.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.709121 octue-0.9.8/tests/cloud/pub_sub/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/pub_sub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10040 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/pub_sub/mocks.py
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/pub_sub/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     9206 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/pub_sub/test_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)    34908 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/pub_sub/test_service.py
--rw-r--r--   0 runner    (1001) docker     (121)     3727 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/pub_sub/test_subscription.py
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/pub_sub/test_topic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.709121 octue-0.9.8/tests/cloud/storage/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13028 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/storage/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     6535 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/storage/test_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     2118 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-02-01 12:42:21.000000 octue-0.9.8/tests/cloud/test_emulators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.709121 octue-0.9.8/tests/essentials/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/tests/essentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      842 2022-02-01 12:42:21.000000 octue-0.9.8/tests/essentials/test_monitor_messages.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.709121 octue-0.9.8/tests/mixins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/tests/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-02-01 12:42:21.000000 octue-0.9.8/tests/mixins/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2089 2022-02-01 12:42:21.000000 octue-0.9.8/tests/mixins/test_cool_nameable.py
--rw-r--r--   0 runner    (1001) docker     (121)    18609 2022-02-01 12:42:21.000000 octue-0.9.8/tests/mixins/test_filterable.py
--rw-r--r--   0 runner    (1001) docker     (121)     3319 2022-02-01 12:42:21.000000 octue-0.9.8/tests/mixins/test_hashable.py
--rw-r--r--   0 runner    (1001) docker     (121)     2819 2022-02-01 12:42:21.000000 octue-0.9.8/tests/mixins/test_identifiable.py
--rw-r--r--   0 runner    (1001) docker     (121)     3013 2022-02-01 12:42:21.000000 octue-0.9.8/tests/mixins/test_labellable.py
--rw-r--r--   0 runner    (1001) docker     (121)     4988 2022-02-01 12:42:21.000000 octue-0.9.8/tests/mixins/test_pathable.py
--rw-r--r--   0 runner    (1001) docker     (121)     3089 2022-02-01 12:42:21.000000 octue-0.9.8/tests/mixins/test_serialisable.py
--rw-r--r--   0 runner    (1001) docker     (121)     2993 2022-02-01 12:42:21.000000 octue-0.9.8/tests/mixins/test_taggable.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.709121 octue-0.9.8/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (121)      569 2022-02-01 12:42:21.000000 octue-0.9.8/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-02-01 12:42:21.000000 octue-0.9.8/tests/resources/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-02-01 12:42:21.000000 octue-0.9.8/tests/resources/test_child.py
--rw-r--r--   0 runner    (1001) docker     (121)    37057 2022-02-01 12:42:21.000000 octue-0.9.8/tests/resources/test_datafile.py
--rw-r--r--   0 runner    (1001) docker     (121)    25283 2022-02-01 12:42:21.000000 octue-0.9.8/tests/resources/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)    15308 2022-02-01 12:42:21.000000 octue-0.9.8/tests/resources/test_filter_containers.py
--rw-r--r--   0 runner    (1001) docker     (121)     8433 2022-02-01 12:42:21.000000 octue-0.9.8/tests/resources/test_label.py
--rw-r--r--   0 runner    (1001) docker     (121)     8341 2022-02-01 12:42:21.000000 octue-0.9.8/tests/resources/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (121)      898 2022-02-01 12:42:21.000000 octue-0.9.8/tests/resources/test_service_backends.py
--rw-r--r--   0 runner    (1001) docker     (121)     2144 2022-02-01 12:42:21.000000 octue-0.9.8/tests/resources/test_tag.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.713121 octue-0.9.8/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/tests/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6852 2022-02-01 12:42:21.000000 octue-0.9.8/tests/templates/test_template_apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.713121 octue-0.9.8/tests/test_app_modules/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/tests/test_app_modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.713121 octue-0.9.8/tests/test_app_modules/app_class/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/tests/test_app_modules/app_class/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-02-01 12:42:21.000000 octue-0.9.8/tests/test_app_modules/app_class/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.713121 octue-0.9.8/tests/test_app_modules/app_module/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/tests/test_app_modules/app_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-02-01 12:42:21.000000 octue-0.9.8/tests/test_app_modules/app_module/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:27.713121 octue-0.9.8/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 12:42:21.000000 octue-0.9.8/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2022-02-01 12:42:21.000000 octue-0.9.8/tests/utils/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (121)     5627 2022-02-01 12:42:21.000000 octue-0.9.8/tests/utils/test_persistence.py
--rw-r--r--   0 runner    (1001) docker     (121)     2520 2022-02-01 12:42:21.000000 octue-0.9.8/tests/utils/test_processes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.919317 octue-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-02-01 15:51:43.000000 octue-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-02-01 15:51:43.000000 octue-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     7170 2022-02-01 15:51:46.919317 octue-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6384 2022-02-01 15:51:43.000000 octue-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.903316 octue-0.9.9/octue/
+-rw-r--r--   0 runner    (1001) docker     (121)      859 2022-02-01 15:51:44.000000 octue-0.9.9/octue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11130 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.903316 octue-0.9.9/octue/cloud/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2992 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.903316 octue-0.9.9/octue/cloud/deployment/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/deployment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.903316 octue-0.9.9/octue/cloud/deployment/google/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/deployment/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3606 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/deployment/google/answer_pub_sub_question.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14266 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/deployment/google/base_deployer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.903316 octue-0.9.9/octue/cloud/deployment/google/cloud_run/
+-rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/deployment/google/cloud_run/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/deployment/google/cloud_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10687 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/deployment/google/cloud_run/deployer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1653 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/deployment/google/cloud_run/flask_app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.903316 octue-0.9.9/octue/cloud/deployment/google/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (121)      519 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/deployment/google/dataflow/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/deployment/google/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8190 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/deployment/google/dataflow/deployer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4142 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/deployment/google/dataflow/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2857 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/emulators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.907316 octue-0.9.9/octue/cloud/pub_sub/
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/pub_sub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/pub_sub/logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9458 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/pub_sub/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17874 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/pub_sub/service.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5755 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/pub_sub/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3001 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/pub_sub/topic.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.907316 octue-0.9.9/octue/cloud/storage/
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14448 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/storage/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2359 2022-02-01 15:51:44.000000 octue-0.9.9/octue/cloud/storage/path.py
+-rw-r--r--   0 runner    (1001) docker     (121)      875 2022-02-01 15:51:44.000000 octue-0.9.9/octue/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.907316 octue-0.9.9/octue/essentials/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/octue/essentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-02-01 15:51:44.000000 octue-0.9.9/octue/essentials/monitor_messages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3828 2022-02-01 15:51:44.000000 octue-0.9.9/octue/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6119 2022-02-01 15:51:44.000000 octue-0.9.9/octue/log_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.907316 octue-0.9.9/octue/mixins/
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2022-02-01 15:51:44.000000 octue-0.9.9/octue/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      781 2022-02-01 15:51:44.000000 octue-0.9.9/octue/mixins/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      569 2022-02-01 15:51:44.000000 octue-0.9.9/octue/mixins/cool_nameable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9513 2022-02-01 15:51:44.000000 octue-0.9.9/octue/mixins/filterable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3551 2022-02-01 15:51:44.000000 octue-0.9.9/octue/mixins/hashable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2263 2022-02-01 15:51:44.000000 octue-0.9.9/octue/mixins/identifiable.py
+-rw-r--r--   0 runner    (1001) docker     (121)      721 2022-02-01 15:51:44.000000 octue-0.9.9/octue/mixins/labelable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3372 2022-02-01 15:51:44.000000 octue-0.9.9/octue/mixins/pathable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4116 2022-02-01 15:51:44.000000 octue-0.9.9/octue/mixins/serialisable.py
+-rw-r--r--   0 runner    (1001) docker     (121)      718 2022-02-01 15:51:44.000000 octue-0.9.9/octue/mixins/taggable.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.907316 octue-0.9.9/octue/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2022-02-01 15:51:44.000000 octue-0.9.9/octue/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7263 2022-02-01 15:51:44.000000 octue-0.9.9/octue/resources/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2759 2022-02-01 15:51:44.000000 octue-0.9.9/octue/resources/child.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27985 2022-02-01 15:51:44.000000 octue-0.9.9/octue/resources/datafile.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11080 2022-02-01 15:51:44.000000 octue-0.9.9/octue/resources/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8779 2022-02-01 15:51:44.000000 octue-0.9.9/octue/resources/filter_containers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3673 2022-02-01 15:51:44.000000 octue-0.9.9/octue/resources/label.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8628 2022-02-01 15:51:44.000000 octue-0.9.9/octue/resources/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2138 2022-02-01 15:51:44.000000 octue-0.9.9/octue/resources/service_backends.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-02-01 15:51:44.000000 octue-0.9.9/octue/resources/tag.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15597 2022-02-01 15:51:44.000000 octue-0.9.9/octue/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.907316 octue-0.9.9/octue/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.899316 octue-0.9.9/octue/templates/template-child-services/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.907316 octue-0.9.9/octue/templates/template-child-services/elevation_service/
+-rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-child-services/elevation_service/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      315 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-child-services/elevation_service/app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.899316 octue-0.9.9/octue/templates/template-child-services/elevation_service/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.907316 octue-0.9.9/octue/templates/template-child-services/elevation_service/data/configuration/
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-child-services/elevation_service/data/configuration/values.json
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-child-services/elevation_service/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-child-services/elevation_service/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1757 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-child-services/elevation_service/twine.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.907316 octue-0.9.9/octue/templates/template-child-services/parent_service/
+-rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-child-services/parent_service/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     2507 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-child-services/parent_service/app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.899316 octue-0.9.9/octue/templates/template-child-services/parent_service/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.907316 octue-0.9.9/octue/templates/template-child-services/parent_service/data/configuration/
+-rw-r--r--   0 runner    (1001) docker     (121)      580 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-child-services/parent_service/data/configuration/children.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.907316 octue-0.9.9/octue/templates/template-child-services/parent_service/data/input/
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-child-services/parent_service/data/input/values.json
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-child-services/parent_service/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-child-services/parent_service/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1345 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-child-services/parent_service/twine.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.911316 octue-0.9.9/octue/templates/template-child-services/wind_speed_service/
+-rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-child-services/wind_speed_service/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      339 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-child-services/wind_speed_service/app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.903316 octue-0.9.9/octue/templates/template-child-services/wind_speed_service/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.911316 octue-0.9.9/octue/templates/template-child-services/wind_speed_service/data/configuration/
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-child-services/wind_speed_service/data/configuration/values.json
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-child-services/wind_speed_service/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-child-services/wind_speed_service/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1755 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-child-services/wind_speed_service/twine.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.911316 octue-0.9.9/octue/templates/template-python-fractal/
+-rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-python-fractal/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     2971 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-python-fractal/app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.903316 octue-0.9.9/octue/templates/template-python-fractal/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.911316 octue-0.9.9/octue/templates/template-python-fractal/data/configuration/
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-python-fractal/data/configuration/configuration_values.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.911316 octue-0.9.9/octue/templates/template-python-fractal/fractal/
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-python-fractal/fractal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3793 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-python-fractal/fractal/fractal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-python-fractal/fractal/mandelbrot.py
+-rw-r--r--   0 runner    (1001) docker     (121)      817 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-python-fractal/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-python-fractal/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1870 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-python-fractal/twine.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.911316 octue-0.9.9/octue/templates/template-using-manifests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-using-manifests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     5480 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-using-manifests/app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.911316 octue-0.9.9/octue/templates/template-using-manifests/cleaner/
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-using-manifests/cleaner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-using-manifests/cleaner/clean.py
+-rw-r--r--   0 runner    (1001) docker     (121)      874 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-using-manifests/cleaner/read_csv_files.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-using-manifests/cleaner/read_dat_file.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.903316 octue-0.9.9/octue/templates/template-using-manifests/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.911316 octue-0.9.9/octue/templates/template-using-manifests/data/configuration/
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-using-manifests/data/configuration/values.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.911316 octue-0.9.9/octue/templates/template-using-manifests/data/input/
+-rw-r--r--   0 runner    (1001) docker     (121)     1582 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-using-manifests/data/input/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.903316 octue-0.9.9/octue/templates/template-using-manifests/data/input/raw_met_mast_data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.911316 octue-0.9.9/octue/templates/template-using-manifests/data/input/raw_met_mast_data/08DEC/
+-rw-r--r--   0 runner    (1001) docker     (121)     4444 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-using-manifests/data/input/raw_met_mast_data/08DEC/High Res Meteorological Mast Data - 8 Dec_1.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     4472 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-using-manifests/data/input/raw_met_mast_data/08DEC/High Res Meteorological Mast Data - 8 Dec_2.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      874 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-using-manifests/data/input/raw_met_mast_data/08DEC/meta - 8 Dec.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-using-manifests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      410 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-using-manifests/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      791 2022-02-01 15:51:44.000000 octue-0.9.9/octue/templates/template-using-manifests/twine.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.911316 octue-0.9.9/octue/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-02-01 15:51:44.000000 octue-0.9.9/octue/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      936 2022-02-01 15:51:44.000000 octue-0.9.9/octue/utils/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-02-01 15:51:44.000000 octue-0.9.9/octue/utils/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (121)      835 2022-02-01 15:51:44.000000 octue-0.9.9/octue/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      761 2022-02-01 15:51:44.000000 octue-0.9.9/octue/utils/folders.py
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2022-02-01 15:51:44.000000 octue-0.9.9/octue/utils/gen_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (121)      627 2022-02-01 15:51:44.000000 octue-0.9.9/octue/utils/isfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)      659 2022-02-01 15:51:44.000000 octue-0.9.9/octue/utils/isfolder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1558 2022-02-01 15:51:44.000000 octue-0.9.9/octue/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1472 2022-02-01 15:51:44.000000 octue-0.9.9/octue/utils/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1699 2022-02-01 15:51:44.000000 octue-0.9.9/octue/utils/processes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.903316 octue-0.9.9/octue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7170 2022-02-01 15:51:46.000000 octue-0.9.9/octue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7209 2022-02-01 15:51:46.000000 octue-0.9.9/octue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-01 15:51:46.000000 octue-0.9.9/octue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-02-01 15:51:46.000000 octue-0.9.9/octue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-01 15:51:46.000000 octue-0.9.9/octue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2022-02-01 15:51:46.000000 octue-0.9.9/octue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-01 15:51:46.000000 octue-0.9.9/octue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      724 2022-02-01 15:51:46.919317 octue-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-02-01 15:51:44.000000 octue-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.903316 octue-0.9.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.911316 octue-0.9.9/tests/cloud/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.911316 octue-0.9.9/tests/cloud/deployment/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/deployment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.911316 octue-0.9.9/tests/cloud/deployment/google/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/deployment/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.915316 octue-0.9.9/tests/cloud/deployment/google/cloud_run/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/deployment/google/cloud_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14123 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/deployment/google/cloud_run/test_cloud_run_deployer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1692 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/deployment/google/cloud_run/test_cloud_run_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/deployment/google/cloud_run/test_flask_app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.915316 octue-0.9.9/tests/cloud/deployment/google/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/deployment/google/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15428 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/deployment/google/dataflow/test_dataflow_deployer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/deployment/google/dataflow/test_dataflow_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4853 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/deployment/google/test_answer_pub_sub_question.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.915316 octue-0.9.9/tests/cloud/pub_sub/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/pub_sub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10040 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/pub_sub/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/pub_sub/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9206 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/pub_sub/test_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34908 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/pub_sub/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3727 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/pub_sub/test_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/pub_sub/test_topic.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.915316 octue-0.9.9/tests/cloud/storage/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13028 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/storage/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6535 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/storage/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2118 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-02-01 15:51:44.000000 octue-0.9.9/tests/cloud/test_emulators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.915316 octue-0.9.9/tests/essentials/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/tests/essentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      842 2022-02-01 15:51:44.000000 octue-0.9.9/tests/essentials/test_monitor_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.915316 octue-0.9.9/tests/mixins/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/tests/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      572 2022-02-01 15:51:44.000000 octue-0.9.9/tests/mixins/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2089 2022-02-01 15:51:44.000000 octue-0.9.9/tests/mixins/test_cool_nameable.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18609 2022-02-01 15:51:44.000000 octue-0.9.9/tests/mixins/test_filterable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3319 2022-02-01 15:51:44.000000 octue-0.9.9/tests/mixins/test_hashable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2819 2022-02-01 15:51:44.000000 octue-0.9.9/tests/mixins/test_identifiable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3013 2022-02-01 15:51:44.000000 octue-0.9.9/tests/mixins/test_labellable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4988 2022-02-01 15:51:44.000000 octue-0.9.9/tests/mixins/test_pathable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3089 2022-02-01 15:51:44.000000 octue-0.9.9/tests/mixins/test_serialisable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2993 2022-02-01 15:51:44.000000 octue-0.9.9/tests/mixins/test_taggable.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.915316 octue-0.9.9/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)      569 2022-02-01 15:51:44.000000 octue-0.9.9/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-02-01 15:51:44.000000 octue-0.9.9/tests/resources/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-02-01 15:51:44.000000 octue-0.9.9/tests/resources/test_child.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37057 2022-02-01 15:51:44.000000 octue-0.9.9/tests/resources/test_datafile.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25283 2022-02-01 15:51:44.000000 octue-0.9.9/tests/resources/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15308 2022-02-01 15:51:44.000000 octue-0.9.9/tests/resources/test_filter_containers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8433 2022-02-01 15:51:44.000000 octue-0.9.9/tests/resources/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8341 2022-02-01 15:51:44.000000 octue-0.9.9/tests/resources/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      898 2022-02-01 15:51:44.000000 octue-0.9.9/tests/resources/test_service_backends.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2144 2022-02-01 15:51:44.000000 octue-0.9.9/tests/resources/test_tag.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.915316 octue-0.9.9/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/tests/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6852 2022-02-01 15:51:44.000000 octue-0.9.9/tests/templates/test_template_apps.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.915316 octue-0.9.9/tests/test_app_modules/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/tests/test_app_modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.915316 octue-0.9.9/tests/test_app_modules/app_class/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/tests/test_app_modules/app_class/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-02-01 15:51:44.000000 octue-0.9.9/tests/test_app_modules/app_class/app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.915316 octue-0.9.9/tests/test_app_modules/app_module/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/tests/test_app_modules/app_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      305 2022-02-01 15:51:44.000000 octue-0.9.9/tests/test_app_modules/app_module/app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:46.915316 octue-0.9.9/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 15:51:44.000000 octue-0.9.9/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1287 2022-02-01 15:51:44.000000 octue-0.9.9/tests/utils/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5627 2022-02-01 15:51:44.000000 octue-0.9.9/tests/utils/test_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2520 2022-02-01 15:51:44.000000 octue-0.9.9/tests/utils/test_processes.py
```

### Comparing `octue-0.9.8/LICENSE` & `octue-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/PKG-INFO` & `octue-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octue
-Version: 0.9.8
+Version: 0.9.9
 Summary: A package providing template applications for data services, and a python SDK to the Octue API
 Home-page: https://www.github.com/octue/octue-sdk-python
 Author: Thomas Clark (github: thclark)
 Author-email: support@octue.com
 License: MIT
 Keywords: digital,twins,twined,data,services,science,api,apps,ml
 Platform: UNKNOWN
```

### Comparing `octue-0.9.8/README.md` & `octue-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/__init__.py` & `octue-0.9.9/octue/__init__.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/cli.py` & `octue-0.9.9/octue/cli.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/cloud/credentials.py` & `octue-0.9.9/octue/cloud/credentials.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/cloud/deployment/google/answer_pub_sub_question.py` & `octue-0.9.9/octue/cloud/deployment/google/answer_pub_sub_question.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/cloud/deployment/google/base_deployer.py` & `octue-0.9.9/octue/cloud/deployment/google/base_deployer.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/cloud/deployment/google/cloud_run/Dockerfile` & `octue-0.9.9/octue/cloud/deployment/google/cloud_run/Dockerfile`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/cloud/deployment/google/cloud_run/deployer.py` & `octue-0.9.9/octue/cloud/deployment/google/cloud_run/deployer.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/cloud/deployment/google/cloud_run/flask_app.py` & `octue-0.9.9/octue/cloud/deployment/google/cloud_run/flask_app.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/cloud/deployment/google/dataflow/Dockerfile` & `octue-0.9.9/octue/cloud/deployment/google/dataflow/Dockerfile`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/cloud/deployment/google/dataflow/deployer.py` & `octue-0.9.9/octue/cloud/deployment/google/dataflow/deployer.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/cloud/deployment/google/dataflow/pipeline.py` & `octue-0.9.9/octue/cloud/deployment/google/dataflow/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,24 +56,26 @@
         "project": project_name,
         "region": region,
         "temp_location": temporary_files_location,
         "job_name": service_name,
         "sdk_container_image": image_uri,
         "setup_file": os.path.abspath(setup_file_path),
         "update": update,
-        "dataflow_service_options": ["enable_prime"],
         "streaming": True,
         **(extra_options or {}),
     }
 
     if service_account_email:
         pipeline_options["service_account_email"] = service_account_email
 
     if worker_machine_type:
         pipeline_options["worker_machine_type"] = worker_machine_type
+    else:
+        # Dataflow Prime can only be used if a worker machine type is not specified.
+        pipeline_options["dataflow_service_options"] = ["enable_prime"]
 
     if maximum_instances:
         pipeline_options["max_num_workers"] = maximum_instances
 
     pipeline_options = PipelineOptions.from_dictionary(pipeline_options)
     pipeline = apache_beam.Pipeline(options=pipeline_options)
```

### Comparing `octue-0.9.8/octue/cloud/emulators.py` & `octue-0.9.9/octue/cloud/emulators.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/cloud/pub_sub/logging.py` & `octue-0.9.9/octue/cloud/pub_sub/logging.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/cloud/pub_sub/message_handler.py` & `octue-0.9.9/octue/cloud/pub_sub/message_handler.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/cloud/pub_sub/service.py` & `octue-0.9.9/octue/cloud/pub_sub/service.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/cloud/pub_sub/subscription.py` & `octue-0.9.9/octue/cloud/pub_sub/subscription.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/cloud/pub_sub/topic.py` & `octue-0.9.9/octue/cloud/pub_sub/topic.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/cloud/storage/client.py` & `octue-0.9.9/octue/cloud/storage/client.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/cloud/storage/path.py` & `octue-0.9.9/octue/cloud/storage/path.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/definitions.py` & `octue-0.9.9/octue/definitions.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/essentials/monitor_messages.py` & `octue-0.9.9/octue/essentials/monitor_messages.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/exceptions.py` & `octue-0.9.9/octue/exceptions.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/log_handlers.py` & `octue-0.9.9/octue/log_handlers.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/mixins/base.py` & `octue-0.9.9/octue/mixins/base.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/mixins/cool_nameable.py` & `octue-0.9.9/octue/mixins/cool_nameable.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/mixins/filterable.py` & `octue-0.9.9/octue/mixins/filterable.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/mixins/hashable.py` & `octue-0.9.9/octue/mixins/hashable.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/mixins/identifiable.py` & `octue-0.9.9/octue/mixins/identifiable.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/mixins/labelable.py` & `octue-0.9.9/octue/mixins/labelable.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/mixins/pathable.py` & `octue-0.9.9/octue/mixins/pathable.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/mixins/serialisable.py` & `octue-0.9.9/octue/mixins/serialisable.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/mixins/taggable.py` & `octue-0.9.9/octue/mixins/taggable.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/resources/analysis.py` & `octue-0.9.9/octue/resources/analysis.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/resources/child.py` & `octue-0.9.9/octue/resources/child.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/resources/datafile.py` & `octue-0.9.9/octue/resources/datafile.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/resources/dataset.py` & `octue-0.9.9/octue/resources/dataset.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/resources/filter_containers.py` & `octue-0.9.9/octue/resources/filter_containers.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/resources/label.py` & `octue-0.9.9/octue/resources/label.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/resources/manifest.py` & `octue-0.9.9/octue/resources/manifest.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/resources/service_backends.py` & `octue-0.9.9/octue/resources/service_backends.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/resources/tag.py` & `octue-0.9.9/octue/resources/tag.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/runner.py` & `octue-0.9.9/octue/runner.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-child-services/elevation_service/.gitignore` & `octue-0.9.9/octue/templates/template-child-services/elevation_service/.gitignore`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-child-services/elevation_service/twine.json` & `octue-0.9.9/octue/templates/template-child-services/elevation_service/twine.json`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-child-services/parent_service/.gitignore` & `octue-0.9.9/octue/templates/template-child-services/parent_service/.gitignore`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-child-services/parent_service/app.py` & `octue-0.9.9/octue/templates/template-child-services/parent_service/app.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-child-services/parent_service/data/configuration/children.json` & `octue-0.9.9/octue/templates/template-child-services/parent_service/data/configuration/children.json`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-child-services/parent_service/twine.json` & `octue-0.9.9/octue/templates/template-child-services/parent_service/twine.json`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-child-services/wind_speed_service/.gitignore` & `octue-0.9.9/octue/templates/template-child-services/wind_speed_service/.gitignore`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-child-services/wind_speed_service/twine.json` & `octue-0.9.9/octue/templates/template-child-services/wind_speed_service/twine.json`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-python-fractal/.gitignore` & `octue-0.9.9/octue/templates/template-python-fractal/.gitignore`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-python-fractal/app.py` & `octue-0.9.9/octue/templates/template-python-fractal/app.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-python-fractal/fractal/fractal.py` & `octue-0.9.9/octue/templates/template-python-fractal/fractal/fractal.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-python-fractal/fractal/mandelbrot.py` & `octue-0.9.9/octue/templates/template-python-fractal/fractal/mandelbrot.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-python-fractal/requirements.txt` & `octue-0.9.9/octue/templates/template-python-fractal/requirements.txt`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-python-fractal/twine.json` & `octue-0.9.9/octue/templates/template-python-fractal/twine.json`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-using-manifests/.gitignore` & `octue-0.9.9/octue/templates/template-using-manifests/.gitignore`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-using-manifests/app.py` & `octue-0.9.9/octue/templates/template-using-manifests/app.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-using-manifests/cleaner/clean.py` & `octue-0.9.9/octue/templates/template-using-manifests/cleaner/clean.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-using-manifests/cleaner/read_csv_files.py` & `octue-0.9.9/octue/templates/template-using-manifests/cleaner/read_csv_files.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-using-manifests/cleaner/read_dat_file.py` & `octue-0.9.9/octue/templates/template-using-manifests/cleaner/read_dat_file.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-using-manifests/data/input/manifest.json` & `octue-0.9.9/octue/templates/template-using-manifests/data/input/manifest.json`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-using-manifests/data/input/raw_met_mast_data/08DEC/High Res Meteorological Mast Data - 8 Dec_1.csv` & `octue-0.9.9/octue/templates/template-using-manifests/data/input/raw_met_mast_data/08DEC/High Res Meteorological Mast Data - 8 Dec_1.csv`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-using-manifests/data/input/raw_met_mast_data/08DEC/High Res Meteorological Mast Data - 8 Dec_2.csv` & `octue-0.9.9/octue/templates/template-using-manifests/data/input/raw_met_mast_data/08DEC/High Res Meteorological Mast Data - 8 Dec_2.csv`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-using-manifests/data/input/raw_met_mast_data/08DEC/meta - 8 Dec.dat` & `octue-0.9.9/octue/templates/template-using-manifests/data/input/raw_met_mast_data/08DEC/meta - 8 Dec.dat`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-using-manifests/requirements.txt` & `octue-0.9.9/octue/templates/template-using-manifests/requirements.txt`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/templates/template-using-manifests/twine.json` & `octue-0.9.9/octue/templates/template-using-manifests/twine.json`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/utils/decoders.py` & `octue-0.9.9/octue/utils/decoders.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/utils/encoders.py` & `octue-0.9.9/octue/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/utils/exceptions.py` & `octue-0.9.9/octue/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/utils/folders.py` & `octue-0.9.9/octue/utils/folders.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/utils/isfile.py` & `octue-0.9.9/octue/utils/isfile.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/utils/isfolder.py` & `octue-0.9.9/octue/utils/isfolder.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/utils/objects.py` & `octue-0.9.9/octue/utils/objects.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/utils/persistence.py` & `octue-0.9.9/octue/utils/persistence.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue/utils/processes.py` & `octue-0.9.9/octue/utils/processes.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/octue.egg-info/PKG-INFO` & `octue-0.9.9/octue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octue
-Version: 0.9.8
+Version: 0.9.9
 Summary: A package providing template applications for data services, and a python SDK to the Octue API
 Home-page: https://www.github.com/octue/octue-sdk-python
 Author: Thomas Clark (github: thclark)
 Author-email: support@octue.com
 License: MIT
 Keywords: digital,twins,twined,data,services,science,api,apps,ml
 Platform: UNKNOWN
```

### Comparing `octue-0.9.8/octue.egg-info/SOURCES.txt` & `octue-0.9.9/octue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/setup.cfg` & `octue-0.9.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/setup.py` & `octue-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     readme_text = f.read()
 
 with open("LICENSE") as f:
     license_text = f.read()
 
 setup(
     name="octue",
-    version="0.9.8",
+    version="0.9.9",
     py_modules=["cli"],
     install_requires=[
         "apache-beam[gcp]==2.35.0",
         "click>=7.1.2",
         "coolname>=1.1.0",
         "Flask>=1.1",
         "google-cloud-pubsub==1.7.0",
```

### Comparing `octue-0.9.8/tests/cloud/deployment/google/cloud_run/test_cloud_run_deployer.py` & `octue-0.9.9/tests/cloud/deployment/google/cloud_run/test_cloud_run_deployer.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,35 +3,31 @@
 from unittest.mock import Mock, patch
 
 from octue.cloud.deployment.google.cloud_run.deployer import DEFAULT_CLOUD_RUN_DOCKERFILE_URL, CloudRunDeployer
 from octue.exceptions import DeploymentError
 from tests.base import BaseTestCase
 
 
-octue_configuration = {
+OCTUE_CONFIGURATION = {
     "services": [
         {
             "name": "test-service",
             "repository_name": "test-repository",
             "repository_owner": "octue",
             "project_name": "test-project",
             "region": "europe-west2",
             "branch_pattern": "my-branch",
         }
     ]
 }
 
-service = octue_configuration["services"][0]
-
-
+SERVICE = OCTUE_CONFIGURATION["services"][0]
 GET_SUBSCRIPTIONS_METHOD_PATH = "octue.cloud.deployment.google.cloud_run.deployer.Topic.get_subscriptions"
-
 SERVICE_ID = "octue.services.0df08f9f-30ad-4db3-8029-ea584b4290b7"
-
-EXPECTED_IMAGE_NAME = f"eu.gcr.io/{service['project_name']}/{service['repository_name']}/{service['name']}:$SHORT_SHA"
+EXPECTED_IMAGE_NAME = f"eu.gcr.io/{SERVICE['project_name']}/{SERVICE['repository_name']}/{SERVICE['name']}:$SHORT_SHA"
 
 EXPECTED_CLOUD_BUILD_CONFIGURATION = {
     "steps": [
         {
             "id": "Get default Octue Dockerfile",
             "name": "alpine:latest",
             "args": ["wget", DEFAULT_CLOUD_RUN_DOCKERFILE_URL],
@@ -57,89 +53,125 @@
             "args": [
                 "run",
                 "services",
                 "update",
                 "test-service",
                 "--platform=managed",
                 f"--image={EXPECTED_IMAGE_NAME}",
-                f"--region={service['region']}",
+                f"--region={SERVICE['region']}",
                 "--memory=128Mi",
                 "--cpu=1",
-                f"--set-env-vars=SERVICE_ID={SERVICE_ID},SERVICE_NAME={service['name']}",
+                f"--set-env-vars=SERVICE_ID={SERVICE_ID},SERVICE_NAME={SERVICE['name']}",
                 "--timeout=3600",
                 "--concurrency=10",
                 "--min-instances=0",
                 "--max-instances=10",
                 "--ingress=internal",
             ],
         },
     ],
     "images": [EXPECTED_IMAGE_NAME],
 }
 
 EXPECTED_BUILD_TRIGGER_CREATION_COMMAND = [
     "gcloud",
-    f"--project={service['project_name']}",
+    f"--project={SERVICE['project_name']}",
     "beta",
     "builds",
     "triggers",
     "create",
     "github",
-    f"--name={service['name']}",
-    f"--repo-name={service['repository_name']}",
-    f"--repo-owner={service['repository_owner']}",
-    f"--description=Build the {service['name']!r} service and deploy it to Cloud Run.",
-    f"--branch-pattern={service['branch_pattern']}",
+    f"--name={SERVICE['name']}",
+    f"--repo-name={SERVICE['repository_name']}",
+    f"--repo-owner={SERVICE['repository_owner']}",
+    f"--description=Build the {SERVICE['name']!r} service and deploy it to Cloud Run.",
+    f"--branch-pattern={SERVICE['branch_pattern']}",
 ]
 
 
 class TestCloudRunDeployer(BaseTestCase):
     def test_generate_cloud_build_configuration(self):
         """Test that a correct Google Cloud Build configuration is generated from the given `octue.yaml` file."""
         with tempfile.TemporaryDirectory() as temporary_directory:
-            octue_configuration_path = self._create_octue_configuration_file(octue_configuration, temporary_directory)
+            octue_configuration_path = self._create_octue_configuration_file(OCTUE_CONFIGURATION, temporary_directory)
             deployer = CloudRunDeployer(octue_configuration_path, service_id=SERVICE_ID)
             deployer._generate_cloud_build_configuration()
 
         self.assertEqual(deployer.generated_cloud_build_configuration, EXPECTED_CLOUD_BUILD_CONFIGURATION)
 
     def test_generate_cloud_build_configuration_with_custom_dockerfile(self):
         """Test that a correct Google Cloud Build configuration is generated from the given `octue.yaml` file when a
         dockerfile path is given.
         """
-        try:
-            service["dockerfile_path"] = "path/to/Dockerfile"
+        octue_configuration_with_custom_dockerfile = copy.deepcopy(OCTUE_CONFIGURATION)
+        octue_configuration_with_custom_dockerfile["services"][0]["dockerfile_path"] = "path/to/Dockerfile"
+
+        with tempfile.TemporaryDirectory() as temporary_directory:
+            octue_configuration_path = self._create_octue_configuration_file(
+                octue_configuration_with_custom_dockerfile,
+                temporary_directory,
+            )
+
+            deployer = CloudRunDeployer(octue_configuration_path, service_id=SERVICE_ID)
+            deployer._generate_cloud_build_configuration()
+
+        # Expect the extra "Get default Octue Dockerfile" step to be absent and the given Dockerfile path to be
+        # provided in the first step.
+        expected_cloud_build_configuration = copy.deepcopy(EXPECTED_CLOUD_BUILD_CONFIGURATION)
+        expected_cloud_build_configuration["steps"] = expected_cloud_build_configuration["steps"][1:]
+
+        expected_cloud_build_configuration["steps"][0]["args"][1] = (
+            f"docker build '-t' '{EXPECTED_IMAGE_NAME}' . '-f' "
+            f"{octue_configuration_with_custom_dockerfile['services'][0]['dockerfile_path']}"
+        )
+
+        self.assertEqual(deployer.generated_cloud_build_configuration, expected_cloud_build_configuration)
+
+    def test_generate_cloud_build_configuration_with_build_secrets(self):
+        """Test generating a Cloud Build configuration with build secrets."""
+        secret_name = "MY_BIG_SECRET"
+
+        octue_configuration_with_build_secrets = copy.deepcopy(OCTUE_CONFIGURATION)
+        service = octue_configuration_with_build_secrets["services"][0]
+        service["secrets"] = {"build": [secret_name]}
+
+        with tempfile.TemporaryDirectory() as temporary_directory:
+            octue_configuration_path = self._create_octue_configuration_file(
+                octue_configuration_with_build_secrets,
+                temporary_directory,
+            )
+
+            deployer = CloudRunDeployer(octue_configuration_path, service_id=SERVICE_ID)
+            deployer._generate_cloud_build_configuration()
+
+        expected_cloud_build_configuration = copy.deepcopy(EXPECTED_CLOUD_BUILD_CONFIGURATION)
+
+        expected_cloud_build_configuration["availableSecrets"] = {
+            "secretManager": [
+                {
+                    "versionName": f'projects/{service["project_name"]}/secrets/{secret_name}/versions/latest',
+                    "env": secret_name,
+                }
+            ]
+        }
 
-            with tempfile.TemporaryDirectory() as temporary_directory:
-                octue_configuration_path = self._create_octue_configuration_file(
-                    octue_configuration, temporary_directory
-                )
-                deployer = CloudRunDeployer(octue_configuration_path, service_id=SERVICE_ID)
-                deployer._generate_cloud_build_configuration()
-
-            # Expect the extra "Get default Octue Dockerfile" step to be absent and the given Dockerfile path to be
-            # provided in the first step.
-            expected_cloud_build_configuration = copy.deepcopy(EXPECTED_CLOUD_BUILD_CONFIGURATION)
-            expected_cloud_build_configuration["steps"] = expected_cloud_build_configuration["steps"][1:]
-
-            expected_cloud_build_configuration["steps"][0]["args"][
-                1
-            ] = f"docker build '-t' '{EXPECTED_IMAGE_NAME}' . '-f' {service['dockerfile_path']}"
+        expected_cloud_build_configuration["steps"][1]["args"][
+            1
+        ] = f"docker build '-t' {EXPECTED_IMAGE_NAME!r} --build-arg={secret_name}=$${secret_name} . '-f' Dockerfile"
 
-            self.assertEqual(deployer.generated_cloud_build_configuration, expected_cloud_build_configuration)
+        expected_cloud_build_configuration["steps"][1]["secretEnv"] = [secret_name]
 
-        finally:
-            del service["dockerfile_path"]
+        self.assertEqual(deployer.generated_cloud_build_configuration, expected_cloud_build_configuration)
 
     def test_deploy(self):
         """Test that the build trigger creation, build and deployment, and Eventarc run trigger creation are requested
         correctly.
         """
         with tempfile.TemporaryDirectory() as temporary_directory:
-            octue_configuration_path = self._create_octue_configuration_file(octue_configuration, temporary_directory)
+            octue_configuration_path = self._create_octue_configuration_file(OCTUE_CONFIGURATION, temporary_directory)
             deployer = CloudRunDeployer(octue_configuration_path, service_id=SERVICE_ID)
 
             with patch("subprocess.run", return_value=Mock(returncode=0)) as mock_run:
                 with patch("octue.cloud.deployment.google.cloud_run.deployer.Topic.create"):
                     with patch(GET_SUBSCRIPTIONS_METHOD_PATH, return_value=["test-service"]):
                         with patch("octue.cloud.deployment.google.cloud_run.deployer.Subscription"):
                             with patch("octue.cloud.deployment.google.cloud_run.deployer.Service"):
@@ -163,78 +195,78 @@
             )
 
             # Test the build trigger run request.
             self.assertEqual(
                 mock_run.call_args_list[1].args[0],
                 [
                     "gcloud",
-                    f"--project={service['project_name']}",
+                    f"--project={SERVICE['project_name']}",
                     "--format=json",
                     "beta",
                     "builds",
                     "triggers",
                     "run",
-                    service["name"],
+                    SERVICE["name"],
                     "--branch=my-branch",
                 ],
             )
 
             # Test waiting for the build trigger run to complete.
             self.assertEqual(
                 mock_run.call_args_list[2].args[0],
                 [
                     "gcloud",
-                    f'--project={service["project_name"]}',
+                    f'--project={SERVICE["project_name"]}',
                     "--format=json",
                     "builds",
                     "describe",
                     mock_build_id,
                 ],
             )
 
             # Test setting the Cloud Run service to accept unauthenticated requests.
             self.assertEqual(
                 mock_run.call_args_list[3].args[0],
                 [
                     "gcloud",
-                    f'--project={service["project_name"]}',
+                    f'--project={SERVICE["project_name"]}',
                     "run",
                     "services",
                     "add-iam-policy-binding",
-                    service["name"],
-                    f'--region={service["region"]}',
+                    SERVICE["name"],
+                    f'--region={SERVICE["region"]}',
                     "--member=allUsers",
                     "--role=roles/run.invoker",
                 ],
             )
 
             # Test the Eventarc run trigger creation request.
             self.assertEqual(
                 mock_run.call_args_list[4].args[0],
                 [
                     "gcloud",
-                    f'--project={service["project_name"]}',
+                    f'--project={SERVICE["project_name"]}',
                     "beta",
                     "eventarc",
                     "triggers",
                     "create",
-                    f'{service["name"]}-trigger',
+                    f'{SERVICE["name"]}-trigger',
                     "--matching-criteria=type=google.cloud.pubsub.topic.v1.messagePublished",
-                    f"--destination-run-service={service['name']}",
-                    f"--location={service['region']}",
+                    f"--destination-run-service={SERVICE['name']}",
+                    f"--location={SERVICE['region']}",
                     f"--transport-topic={SERVICE_ID}",
                 ],
             )
 
     def test_create_build_trigger_with_update(self):
         """Test that creating a build trigger for a service when one already exists and the deployer is in `update`
         mode results in the existing trigger being deleted and recreated.
         """
         with tempfile.TemporaryDirectory() as temporary_directory:
-            octue_configuration_path = self._create_octue_configuration_file(octue_configuration, temporary_directory)
+            octue_configuration_path = self._create_octue_configuration_file(OCTUE_CONFIGURATION, temporary_directory)
             deployer = CloudRunDeployer(octue_configuration_path)
             deployer._generate_cloud_build_configuration()
 
             temporary_file = tempfile.NamedTemporaryFile(delete=False)
 
             with patch("tempfile.NamedTemporaryFile", return_value=temporary_file):
                 with patch(
@@ -254,33 +286,33 @@
         self.assertEqual(mock_run_command.call_args_list[0].args[0], expected_build_trigger_creation_command)
 
         # Test that trigger deletion is requested.
         self.assertEqual(
             mock_run_command.call_args_list[1].args[0],
             [
                 "gcloud",
-                f"--project={service['project_name']}",
+                f"--project={SERVICE['project_name']}",
                 "beta",
                 "builds",
                 "triggers",
                 "delete",
-                service["name"],
+                SERVICE["name"],
             ],
         )
 
         # Test the build trigger creation request is retried.
         self.assertEqual(mock_run_command.call_args_list[2].args[0], expected_build_trigger_creation_command)
 
     def test_create_eventarc_run_trigger_with_update(self):
         """Test that creating an Eventarc run trigger for a service when one already exists and the deployer is in
         `update` mode results in the Eventarc subscription update being skipped and an "already exists" message being
         printed.
         """
         with tempfile.TemporaryDirectory() as temporary_directory:
-            octue_configuration_path = self._create_octue_configuration_file(octue_configuration, temporary_directory)
+            octue_configuration_path = self._create_octue_configuration_file(OCTUE_CONFIGURATION, temporary_directory)
             deployer = CloudRunDeployer(octue_configuration_path)
 
             with patch("octue.cloud.deployment.google.cloud_run.deployer.Topic.create"):
                 with patch(
                     "octue.cloud.deployment.google.cloud_run.deployer.CloudRunDeployer._run_command",
                     side_effect=DeploymentError("already exists"),
                 ):
```

### Comparing `octue-0.9.8/tests/cloud/deployment/google/cloud_run/test_cloud_run_deployment.py` & `octue-0.9.9/tests/cloud/deployment/google/cloud_run/test_cloud_run_deployment.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/cloud/deployment/google/cloud_run/test_flask_app.py` & `octue-0.9.9/tests/cloud/deployment/google/cloud_run/test_flask_app.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/cloud/deployment/google/dataflow/test_dataflow_deployer.py` & `octue-0.9.9/tests/cloud/deployment/google/dataflow/test_dataflow_deployer.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     OCTUE_SDK_PYTHON_IMAGE_URI,
     DataflowDeployer,
 )
 from octue.exceptions import DeploymentError
 from tests.base import BaseTestCase
 
 
-octue_configuration = {
+OCTUE_CONFIGURATION = {
     "services": [
         {
             "name": "test-service",
             "repository_name": "test-repository",
             "repository_owner": "octue",
             "project_name": "test-project",
             "region": "europe-west2",
@@ -27,24 +27,24 @@
             "service_account_email": "account@domain.com",
             "maximum_instances": 30,
             "machine_type": "e2-standard-2",
         }
     ]
 }
 
-service = octue_configuration["services"][0]
+SERVICE = OCTUE_CONFIGURATION["services"][0]
 
-octue_configuration_with_cloud_build_path = {
-    "services": [{**copy.copy(service), "cloud_build_configuration_path": "cloudbuild.yaml"}]
+OCTUE_CONFIGURATION_WITH_CLOUD_BUILD_PATH = {
+    "services": [{**copy.copy(SERVICE), "cloud_build_configuration_path": "cloudbuild.yaml"}]
 }
 
 SERVICE_ID = "octue.services.0df08f9f-30ad-4db3-8029-ea584b4290b7"
 
 EXPECTED_IMAGE_NAME = (
-    f"eu.gcr.io/{service['project_name']}/{service['repository_name']}/" f"{service['name']}:$SHORT_SHA"
+    f"eu.gcr.io/{SERVICE['project_name']}/{SERVICE['repository_name']}/" f"{SERVICE['name']}:$SHORT_SHA"
 )
 
 EXPECTED_CLOUD_BUILD_CONFIGURATION = {
     "steps": [
         {
             "id": "Get default Octue Dockerfile",
             "name": "alpine:latest",
@@ -54,15 +54,15 @@
             "id": "Build image",
             "name": "gcr.io/cloud-builders/docker",
             "entrypoint": "bash",
             "args": [
                 "-c",
                 (
                     f"docker build '-t' {EXPECTED_IMAGE_NAME!r} --build-arg=SERVICE_ID={SERVICE_ID} "
-                    f"--build-arg=SERVICE_NAME={service['name']} . '-f' Dockerfile"
+                    f"--build-arg=SERVICE_NAME={SERVICE['name']} . '-f' Dockerfile"
                 ),
             ],
         },
         {
             "id": "Push image",
             "name": "gcr.io/cloud-builders/docker",
             "args": ["push", EXPECTED_IMAGE_NAME],
@@ -82,42 +82,42 @@
         },
     ],
     "images": [EXPECTED_IMAGE_NAME],
 }
 
 EXPECTED_BUILD_TRIGGER_CREATION_COMMAND = [
     "gcloud",
-    f"--project={service['project_name']}",
+    f"--project={SERVICE['project_name']}",
     "beta",
     "builds",
     "triggers",
     "create",
     "github",
-    f"--name={service['name']}",
-    f"--repo-name={service['repository_name']}",
-    f"--repo-owner={service['repository_owner']}",
-    f"--description=Build the {service['name']!r} service and deploy it to Dataflow.",
-    f"--branch-pattern={service['branch_pattern']}",
+    f"--name={SERVICE['name']}",
+    f"--repo-name={SERVICE['repository_name']}",
+    f"--repo-owner={SERVICE['repository_owner']}",
+    f"--description=Build the {SERVICE['name']!r} service and deploy it to Dataflow.",
+    f"--branch-pattern={SERVICE['branch_pattern']}",
 ]
 
 
 class TestDataflowDeployer(BaseTestCase):
     def test_generate_cloud_build_configuration(self):
         """Test that a correct Google Cloud Build configuration is generated from the given `octue.yaml` file."""
         with tempfile.TemporaryDirectory() as temporary_directory:
-            octue_configuration_path = self._create_octue_configuration_file(octue_configuration, temporary_directory)
+            octue_configuration_path = self._create_octue_configuration_file(OCTUE_CONFIGURATION, temporary_directory)
             deployer = DataflowDeployer(octue_configuration_path, service_id=SERVICE_ID)
 
         deployer._generate_cloud_build_configuration()
         self.assertEqual(deployer.generated_cloud_build_configuration, EXPECTED_CLOUD_BUILD_CONFIGURATION)
 
     def test_deploy(self):
         """Test that the build trigger creation and run are requested correctly."""
         with tempfile.TemporaryDirectory() as temporary_directory:
-            octue_configuration_path = self._create_octue_configuration_file(octue_configuration, temporary_directory)
+            octue_configuration_path = self._create_octue_configuration_file(OCTUE_CONFIGURATION, temporary_directory)
             deployer = DataflowDeployer(octue_configuration_path, service_id=SERVICE_ID)
 
             with patch("subprocess.run", return_value=Mock(returncode=0)) as mock_run:
                 mock_build_id = "my-build-id"
 
                 with patch(
                     "json.loads",
@@ -138,43 +138,43 @@
             )
 
             # Test the build trigger run request.
             self.assertEqual(
                 mock_run.call_args_list[1].args[0],
                 [
                     "gcloud",
-                    f"--project={service['project_name']}",
+                    f"--project={SERVICE['project_name']}",
                     "--format=json",
                     "beta",
                     "builds",
                     "triggers",
                     "run",
-                    service["name"],
+                    SERVICE["name"],
                     "--branch=my-branch",
                 ],
             )
 
             # Test waiting for the build trigger run to complete.
             self.assertEqual(
                 mock_run.call_args_list[2].args[0],
                 [
                     "gcloud",
-                    f'--project={service["project_name"]}',
+                    f'--project={SERVICE["project_name"]}',
                     "--format=json",
                     "builds",
                     "describe",
                     mock_build_id,
                 ],
             )
 
     def test_deploy_with_cloud_build_file_provided(self):
         """Test deploying to Dataflow with a `cloudbuild.yaml` path provided in the `octue.yaml` file"""
         with tempfile.TemporaryDirectory() as temporary_directory:
             octue_configuration_path = self._create_octue_configuration_file(
-                octue_configuration_with_cloud_build_path,
+                OCTUE_CONFIGURATION_WITH_CLOUD_BUILD_PATH,
                 temporary_directory,
             )
 
             deployer = DataflowDeployer(octue_configuration_path, service_id=SERVICE_ID, image_uri_template="blah")
 
             with patch("subprocess.run", return_value=Mock(returncode=0)) as mock_run:
                 mock_build_id = "my-build-id"
@@ -190,101 +190,104 @@
                         deployer.deploy()
 
             # Test the build trigger creation request.
             self.assertEqual(
                 mock_run.call_args_list[0].args[0],
                 EXPECTED_BUILD_TRIGGER_CREATION_COMMAND
                 + [
-                    f"--build-config={octue_configuration_with_cloud_build_path['services'][0]['cloud_build_configuration_path']}"
+                    f"--build-config={OCTUE_CONFIGURATION_WITH_CLOUD_BUILD_PATH['services'][0]['cloud_build_configuration_path']}"
                 ],
             )
 
             # Test the build trigger run request.
             self.assertEqual(
                 mock_run.call_args_list[1].args[0],
                 [
                     "gcloud",
-                    f"--project={octue_configuration_with_cloud_build_path['services'][0]['project_name']}",
+                    f"--project={OCTUE_CONFIGURATION_WITH_CLOUD_BUILD_PATH['services'][0]['project_name']}",
                     "--format=json",
                     "beta",
                     "builds",
                     "triggers",
                     "run",
-                    octue_configuration_with_cloud_build_path["services"][0]["name"],
+                    OCTUE_CONFIGURATION_WITH_CLOUD_BUILD_PATH["services"][0]["name"],
                     "--branch=my-branch",
                 ],
             )
 
             # Test waiting for the build trigger run to complete.
             self.assertEqual(
                 mock_run.call_args_list[2].args[0],
                 [
                     "gcloud",
-                    f'--project={service["project_name"]}',
+                    f'--project={SERVICE["project_name"]}',
                     "--format=json",
                     "builds",
                     "describe",
                     mock_build_id,
                 ],
             )
 
     def test_create_streaming_dataflow_job(self):
         """Test creating a streaming dataflow job directly."""
         with tempfile.TemporaryDirectory() as temporary_directory:
-            octue_configuration_path = self._create_octue_configuration_file(octue_configuration, temporary_directory)
+            octue_configuration_path = self._create_octue_configuration_file(OCTUE_CONFIGURATION, temporary_directory)
             deployer = DataflowDeployer(octue_configuration_path, service_id=SERVICE_ID)
 
             with patch(
                 "octue.cloud.deployment.google.dataflow.pipeline.Topic",
                 return_value=Mock(path="projects/my-project/topics/my-topic"),
             ):
-                with patch("octue.cloud.deployment.google.dataflow.pipeline.DataflowRunner") as mock_runner:
+                with patch("octue.cloud.deployment.google.dataflow.pipeline.DataflowRunner.run_pipeline") as mock_run:
                     deployer.create_streaming_dataflow_job(image_uri="my-image-uri")
 
-            options = mock_runner.mock_calls[1].kwargs["options"].get_all_options()
+            options = mock_run.call_args.kwargs["options"].get_all_options()
             self.assertFalse(options["update"])
             self.assertTrue(options["streaming"])
-            self.assertEqual(options["project"], service["project_name"])
-            self.assertEqual(options["job_name"], service["name"])
+            self.assertEqual(options["project"], SERVICE["project_name"])
+            self.assertEqual(options["job_name"], SERVICE["name"])
             self.assertEqual(options["temp_location"], DEFAULT_DATAFLOW_TEMPORARY_FILES_LOCATION)
-            self.assertEqual(options["region"], service["region"])
-            self.assertEqual(options["dataflow_service_options"], ["enable_prime"])
+            self.assertEqual(options["region"], SERVICE["region"])
             self.assertEqual(options["sdk_container_image"], "my-image-uri")
             self.assertEqual(options["setup_file"], DEFAULT_SETUP_FILE_PATH)
 
+            # Check that "enable_prime" isn't in the Dataflow service options (it should be disabled if a machine type
+            # is specified in the octue configuration file).
+            self.assertIsNone(options["dataflow_service_options"])
+
     def test_updating_streaming_dataflow_job(self):
         """Test updating an existing streaming dataflow job."""
         with tempfile.TemporaryDirectory() as temporary_directory:
-            octue_configuration_path = self._create_octue_configuration_file(octue_configuration, temporary_directory)
+            octue_configuration_path = self._create_octue_configuration_file(OCTUE_CONFIGURATION, temporary_directory)
             deployer = DataflowDeployer(octue_configuration_path, service_id=SERVICE_ID)
 
             with patch(
                 "octue.cloud.deployment.google.dataflow.pipeline.Topic",
                 return_value=Mock(path="projects/my-project/topics/my-topic"),
             ):
-                with patch("octue.cloud.deployment.google.dataflow.pipeline.DataflowRunner") as mock_runner:
+                with patch("octue.cloud.deployment.google.dataflow.pipeline.DataflowRunner.run_pipeline") as mock_run:
                     deployer.create_streaming_dataflow_job(image_uri="my-image-uri", update=True)
 
-            options = mock_runner.mock_calls[1].kwargs["options"].get_all_options()
+            options = mock_run.call_args.kwargs["options"].get_all_options()
             self.assertTrue(options["update"])
             self.assertTrue(options["streaming"])
-            self.assertEqual(options["project"], service["project_name"])
-            self.assertEqual(options["job_name"], service["name"])
+            self.assertIsNone(options["dataflow_service_options"])
+            self.assertEqual(options["project"], SERVICE["project_name"])
+            self.assertEqual(options["job_name"], SERVICE["name"])
             self.assertEqual(options["temp_location"], DEFAULT_DATAFLOW_TEMPORARY_FILES_LOCATION)
-            self.assertEqual(options["region"], service["region"])
-            self.assertEqual(options["dataflow_service_options"], ["enable_prime"])
+            self.assertEqual(options["region"], SERVICE["region"])
             self.assertEqual(options["sdk_container_image"], "my-image-uri")
             self.assertEqual(options["setup_file"], DEFAULT_SETUP_FILE_PATH)
 
     def test_create_streaming_dataflow_job_when_job_does_not_already_exist(self):
         """Test that attempting to deploy an update to a Dataflow job when a job with the name of service does not
         already exist results in the job deployment being retried with `update` set to `False`.
         """
         with tempfile.TemporaryDirectory() as temporary_directory:
-            octue_configuration_path = self._create_octue_configuration_file(octue_configuration, temporary_directory)
+            octue_configuration_path = self._create_octue_configuration_file(OCTUE_CONFIGURATION, temporary_directory)
             deployer = DataflowDeployer(octue_configuration_path, service_id=SERVICE_ID)
 
             with patch(
                 "octue.cloud.deployment.google.dataflow.pipeline.Topic",
                 return_value=Mock(path="projects/my-project/topics/my-topic"),
             ):
                 with patch(
@@ -300,20 +303,45 @@
             # Check that the second attempt was to create the service.
             second_attempt_options = mock_runner.mock_calls[1].kwargs["options"].get_all_options()
             self.assertFalse(second_attempt_options["update"])
 
     def test_deployment_error_raised_if_dataflow_job_already_exists(self):
         """Test that a deployment error is raised if a Dataflow job already exists with the same name as the service."""
         with tempfile.TemporaryDirectory() as temporary_directory:
-            octue_configuration_path = self._create_octue_configuration_file(octue_configuration, temporary_directory)
+            octue_configuration_path = self._create_octue_configuration_file(OCTUE_CONFIGURATION, temporary_directory)
             deployer = DataflowDeployer(octue_configuration_path, service_id=SERVICE_ID)
 
             with patch(
                 "octue.cloud.deployment.google.dataflow.pipeline.Topic",
                 return_value=Mock(path="projects/my-project/topics/my-topic"),
             ):
                 with patch(
                     "octue.cloud.deployment.google.dataflow.pipeline.DataflowRunner.run_pipeline",
                     side_effect=DataflowJobAlreadyExistsError(),
                 ):
                     with self.assertRaises(DeploymentError):
                         deployer.create_streaming_dataflow_job(image_uri="my-image-uri", update=True)
+
+    def test_dataflow_prime_enabled_if_machine_type_not_specified(self):
+        """Test that Dataflow Prime is enabled if the machine type is not specified in the octue configuration."""
+        with tempfile.TemporaryDirectory() as temporary_directory:
+            octue_configuration_with_no_machine_type = copy.deepcopy(OCTUE_CONFIGURATION)
+            del octue_configuration_with_no_machine_type["services"][0]["machine_type"]
+
+            octue_configuration_path = self._create_octue_configuration_file(
+                octue_configuration_with_no_machine_type,
+                temporary_directory,
+            )
+
+            deployer = DataflowDeployer(octue_configuration_path, service_id=SERVICE_ID)
+
+            with patch(
+                "octue.cloud.deployment.google.dataflow.pipeline.Topic",
+                return_value=Mock(path="projects/my-project/topics/my-topic"),
+            ):
+                with patch("octue.cloud.deployment.google.dataflow.pipeline.DataflowRunner.run_pipeline") as mock_run:
+                    deployer.create_streaming_dataflow_job(image_uri="my-image-uri")
+
+        self.assertEqual(
+            mock_run.call_args.kwargs["options"].get_all_options()["dataflow_service_options"],
+            ["enable_prime"],
+        )
```

### Comparing `octue-0.9.8/tests/cloud/deployment/google/dataflow/test_dataflow_deployment.py` & `octue-0.9.9/tests/cloud/deployment/google/dataflow/test_dataflow_deployment.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/cloud/deployment/google/test_answer_pub_sub_question.py` & `octue-0.9.9/tests/cloud/deployment/google/test_answer_pub_sub_question.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/cloud/pub_sub/mocks.py` & `octue-0.9.9/tests/cloud/pub_sub/mocks.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/cloud/pub_sub/test_logging.py` & `octue-0.9.9/tests/cloud/pub_sub/test_logging.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/cloud/pub_sub/test_message_handler.py` & `octue-0.9.9/tests/cloud/pub_sub/test_message_handler.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/cloud/pub_sub/test_service.py` & `octue-0.9.9/tests/cloud/pub_sub/test_service.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/cloud/pub_sub/test_subscription.py` & `octue-0.9.9/tests/cloud/pub_sub/test_subscription.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/cloud/pub_sub/test_topic.py` & `octue-0.9.9/tests/cloud/pub_sub/test_topic.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/cloud/storage/test_client.py` & `octue-0.9.9/tests/cloud/storage/test_client.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/cloud/storage/test_path.py` & `octue-0.9.9/tests/cloud/storage/test_path.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/cloud/test_credentials.py` & `octue-0.9.9/tests/cloud/test_credentials.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/cloud/test_emulators.py` & `octue-0.9.9/tests/cloud/test_emulators.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/essentials/test_monitor_messages.py` & `octue-0.9.9/tests/essentials/test_monitor_messages.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/mixins/test_base.py` & `octue-0.9.9/tests/mixins/test_base.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/mixins/test_cool_nameable.py` & `octue-0.9.9/tests/mixins/test_cool_nameable.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/mixins/test_filterable.py` & `octue-0.9.9/tests/mixins/test_filterable.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/mixins/test_hashable.py` & `octue-0.9.9/tests/mixins/test_hashable.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/mixins/test_identifiable.py` & `octue-0.9.9/tests/mixins/test_identifiable.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/mixins/test_labellable.py` & `octue-0.9.9/tests/mixins/test_labellable.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/mixins/test_pathable.py` & `octue-0.9.9/tests/mixins/test_pathable.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/mixins/test_serialisable.py` & `octue-0.9.9/tests/mixins/test_serialisable.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/mixins/test_taggable.py` & `octue-0.9.9/tests/mixins/test_taggable.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/resources/__init__.py` & `octue-0.9.9/tests/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/resources/test_analysis.py` & `octue-0.9.9/tests/resources/test_analysis.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/resources/test_child.py` & `octue-0.9.9/tests/resources/test_child.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/resources/test_datafile.py` & `octue-0.9.9/tests/resources/test_datafile.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/resources/test_dataset.py` & `octue-0.9.9/tests/resources/test_dataset.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/resources/test_filter_containers.py` & `octue-0.9.9/tests/resources/test_filter_containers.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/resources/test_label.py` & `octue-0.9.9/tests/resources/test_label.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/resources/test_manifest.py` & `octue-0.9.9/tests/resources/test_manifest.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/resources/test_service_backends.py` & `octue-0.9.9/tests/resources/test_service_backends.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/resources/test_tag.py` & `octue-0.9.9/tests/resources/test_tag.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/templates/test_template_apps.py` & `octue-0.9.9/tests/templates/test_template_apps.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/utils/test_objects.py` & `octue-0.9.9/tests/utils/test_objects.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/utils/test_persistence.py` & `octue-0.9.9/tests/utils/test_persistence.py`

 * *Files identical despite different names*

### Comparing `octue-0.9.8/tests/utils/test_processes.py` & `octue-0.9.9/tests/utils/test_processes.py`

 * *Files identical despite different names*

