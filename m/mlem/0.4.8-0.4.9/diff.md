# Comparing `tmp/mlem-0.4.8.tar.gz` & `tmp/mlem-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlem-0.4.8.tar", last modified: Tue Mar 14 10:24:10 2023, max compression
+gzip compressed data, was "mlem-0.4.9.tar", last modified: Thu Mar 23 11:55:40 2023, max compression
```

## Comparing `mlem-0.4.8.tar` & `mlem-0.4.9.tar`

### file list

```diff
@@ -1,311 +1,311 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.856607 mlem-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-14 10:23:52.000000 mlem-0.4.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.816605 mlem-0.4.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-14 10:23:52.000000 mlem-0.4.8/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-14 10:23:52.000000 mlem-0.4.8/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.816605 mlem-0.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-03-14 10:23:52.000000 mlem-0.4.8/.github/workflows/check-test-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-03-14 10:23:52.000000 mlem-0.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-03-14 10:23:52.000000 mlem-0.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20778 2023-03-14 10:23:52.000000 mlem-0.4.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-03-14 10:23:52.000000 mlem-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-14 10:23:52.000000 mlem-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-03-14 10:24:10.856607 mlem-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-03-14 10:23:52.000000 mlem-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.816605 mlem-0.4.8/mlem/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-14 10:24:10.000000 mlem-0.4.8/mlem/_mlem_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.816605 mlem-0.4.8/mlem/api/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15979 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/api/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/api/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.820606 mlem-0.4.8/mlem/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/cli/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/cli/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/cli/checkenv.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/cli/clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/cli/declare.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/cli/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/cli/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/cli/import_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/cli/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/cli/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/cli/link.py
--rw-r--r--   0 runner    (1001) docker     (123)    19353 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/cli/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/cli/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    20208 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.824606 mlem-0.4.8/mlem/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/bitbucketfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/callable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/catboost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.828606 mlem-0.4.8/mlem/contrib/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21000 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/docker/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15539 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/docker/context.py
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/docker/copy.j2
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/docker/dockerfile.j2
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/docker/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/docker/install_req.j2
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/docker/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/dvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.828606 mlem-0.4.8/mlem/contrib/flyio/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/flyio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/flyio/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/flyio/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/gitlabfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.828606 mlem-0.4.8/mlem/contrib/heroku/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/heroku/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/heroku/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/heroku/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/heroku/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/heroku/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/heroku/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.828606 mlem-0.4.8/mlem/contrib/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/kubernetes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/kubernetes/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/kubernetes/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/kubernetes/resources.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/kubernetes/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/kubernetes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9573 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)    24506 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/pil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.828606 mlem-0.4.8/mlem/contrib/pip/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/pip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/pip/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/pip/setup.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/pip/source.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.832606 mlem-0.4.8/mlem/contrib/sagemaker/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/sagemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/sagemaker/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/sagemaker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/sagemaker/copy.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/sagemaker/env_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/sagemaker/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/sagemaker/mlem_sagemaker.tf
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/sagemaker/post_copy.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/sagemaker/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/sagemaker/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/sklearn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.832606 mlem-0.4.8/mlem/contrib/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/streamlit/_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/streamlit/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/streamlit/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/venv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/contrib/xgboost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.836606 mlem-0.4.8/mlem/core/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)    14457 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    33605 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/core/data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/core/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/core/import_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/core/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/core/meta_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    45469 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/core/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    19386 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/core/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.836606 mlem-0.4.8/mlem/polydantic/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/polydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/polydantic/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/polydantic/lazy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.836606 mlem-0.4.8/mlem/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/runtime/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    10600 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/runtime/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.836606 mlem-0.4.8/mlem/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/utils/backport.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/utils/entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/utils/fslock.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/utils/importing.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/utils/mlem.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    21799 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/utils/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/utils/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-14 10:23:52.000000 mlem-0.4.8/mlem/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.816605 mlem-0.4.8/mlem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-03-14 10:24:10.000000 mlem-0.4.8/mlem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-03-14 10:24:10.000000 mlem-0.4.8/mlem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 10:24:10.000000 mlem-0.4.8/mlem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-03-14 10:24:10.000000 mlem-0.4.8/mlem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 10:24:10.000000 mlem-0.4.8/mlem.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-03-14 10:24:10.000000 mlem-0.4.8/mlem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-14 10:24:10.000000 mlem-0.4.8/mlem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-14 10:23:52.000000 mlem-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-14 10:23:52.000000 mlem-0.4.8/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-14 10:24:10.856607 mlem-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-03-14 10:23:52.000000 mlem-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.836606 mlem-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.840607 mlem-0.4.8/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/api/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/api/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/api/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.840607 mlem-0.4.8/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/cli/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/cli/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/cli/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/cli/test_checkenv.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/cli/test_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/cli/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    16295 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/cli/test_declare.py
--rw-r--r--   0 runner    (1001) docker     (123)    16476 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/cli/test_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/cli/test_import_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/cli/test_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/cli/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/cli/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/cli/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/cli/test_serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/cli/test_stderr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/cli/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.844607 mlem-0.4.8/tests/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.844607 mlem-0.4.8/tests/contrib/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/resources/im.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.844607 mlem-0.4.8/tests/contrib/resources/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/resources/pandas/.mlem.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_bitbucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_callable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_catboost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.848607 mlem-0.4.8/tests/contrib/test_docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_docker/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.848607 mlem-0.4.8/tests/contrib/test_docker/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_docker/resources/dockerfile.j2
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_docker/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_docker/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_docker/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_docker/test_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_docker/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_heroku.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.848607 mlem-0.4.8/tests/contrib/test_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_kubernetes/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_kubernetes/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_kubernetes/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_kubernetes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_venv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/contrib/test_xgboost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.848607 mlem-0.4.8/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.852607 mlem-0.4.8/tests/core/custom_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/custom_requirements/model_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.852607 mlem-0.4.8/tests/core/custom_requirements/pack_1/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/custom_requirements/pack_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/custom_requirements/pack_1/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/custom_requirements/pack_1/model_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.852607 mlem-0.4.8/tests/core/custom_requirements/pack_2/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/custom_requirements/pack_2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.852607 mlem-0.4.8/tests/core/custom_requirements/pkg/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/custom_requirements/pkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/custom_requirements/pkg/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.852607 mlem-0.4.8/tests/core/custom_requirements/pkg/subpkg/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/custom_requirements/pkg/subpkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/custom_requirements/pkg/subpkg/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/custom_requirements/pkg/subpkg/testfile.json
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/custom_requirements/pkg_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/custom_requirements/proxy_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/custom_requirements/proxy_pkg_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/custom_requirements/shell_reqs.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/custom_requirements/test_remote_custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/custom_requirements/test_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/custom_requirements/test_shell_reqs.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/custom_requirements/unused_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/custom_requirements/use_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/custom_requirements/use_model_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.852607 mlem-0.4.8/tests/core/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/resources/emoji_model_inside.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/resources/emoji_model_outside.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/resources/emoji_model_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/resources/file.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/resources/server.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/test_data_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    19790 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/test_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/test_meta_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/test_model_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/core/test_requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.852607 mlem-0.4.8/tests/polydantic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/polydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/polydantic/test_lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/polydantic/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/polydantic/test_serde.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.812605 mlem-0.4.8/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.852607 mlem-0.4.8/tests/resources/empty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/resources/empty/.mlem.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.852607 mlem-0.4.8/tests/resources/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/resources/storage/.mlem.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.856607 mlem-0.4.8/tests/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/runtime/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/runtime/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/runtime/test_model_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/test_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/test_telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:24:10.856607 mlem-0.4.8/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/utils/module_tools_mock_req.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/utils/test_entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/utils/test_fslock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/utils/test_module_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/utils/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/utils/test_root.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-14 10:23:52.000000 mlem-0.4.8/tests/utils/test_save.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-14 10:23:52.000000 mlem-0.4.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.544458 mlem-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-23 11:55:26.000000 mlem-0.4.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.524458 mlem-0.4.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-23 11:55:26.000000 mlem-0.4.9/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-23 11:55:26.000000 mlem-0.4.9/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.524458 mlem-0.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-03-23 11:55:26.000000 mlem-0.4.9/.github/workflows/check-test-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-03-23 11:55:26.000000 mlem-0.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-03-23 11:55:26.000000 mlem-0.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20778 2023-03-23 11:55:26.000000 mlem-0.4.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-03-23 11:55:26.000000 mlem-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-23 11:55:26.000000 mlem-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-03-23 11:55:40.544458 mlem-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-03-23 11:55:26.000000 mlem-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.524458 mlem-0.4.9/mlem/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-23 11:55:39.000000 mlem-0.4.9/mlem/_mlem_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.524458 mlem-0.4.9/mlem/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15979 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/api/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/api/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.528458 mlem-0.4.9/mlem/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/cli/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/cli/checkenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/cli/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/cli/declare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/cli/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/cli/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/cli/import_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/cli/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/cli/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19353 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/cli/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/cli/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20208 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.528458 mlem-0.4.9/mlem/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/bitbucketfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/callable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/catboost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.528458 mlem-0.4.9/mlem/contrib/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21100 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/docker/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16040 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/docker/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/docker/copy.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/docker/dockerfile.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/docker/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/docker/install_req.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/docker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.532458 mlem-0.4.9/mlem/contrib/flyio/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/flyio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/flyio/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/flyio/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/gitlabfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.532458 mlem-0.4.9/mlem/contrib/heroku/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/heroku/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/heroku/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/heroku/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/heroku/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/heroku/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/heroku/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.532458 mlem-0.4.9/mlem/contrib/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/kubernetes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/kubernetes/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/kubernetes/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/kubernetes/resources.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/kubernetes/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/kubernetes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9573 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24506 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/pil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.532458 mlem-0.4.9/mlem/contrib/pip/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/pip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/pip/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/pip/setup.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/pip/source.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.532458 mlem-0.4.9/mlem/contrib/sagemaker/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/sagemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/sagemaker/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/sagemaker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/sagemaker/copy.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/sagemaker/env_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/sagemaker/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/sagemaker/mlem_sagemaker.tf
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/sagemaker/post_copy.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/sagemaker/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/sagemaker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/sklearn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.532458 mlem-0.4.9/mlem/contrib/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/streamlit/_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/streamlit/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/streamlit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/contrib/xgboost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.532458 mlem-0.4.9/mlem/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14457 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33605 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/core/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/core/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/core/import_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/core/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/core/meta_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45590 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/core/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20780 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/core/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.532458 mlem-0.4.9/mlem/polydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/polydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/polydantic/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/polydantic/lazy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.536458 mlem-0.4.9/mlem/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/runtime/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10600 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/runtime/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.536458 mlem-0.4.9/mlem/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/utils/backport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/utils/entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/utils/fslock.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/utils/importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/utils/mlem.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    21774 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/utils/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/utils/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-23 11:55:26.000000 mlem-0.4.9/mlem/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.524458 mlem-0.4.9/mlem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-03-23 11:55:40.000000 mlem-0.4.9/mlem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-03-23 11:55:40.000000 mlem-0.4.9/mlem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 11:55:40.000000 mlem-0.4.9/mlem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-03-23 11:55:40.000000 mlem-0.4.9/mlem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 11:55:40.000000 mlem-0.4.9/mlem.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-03-23 11:55:40.000000 mlem-0.4.9/mlem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-23 11:55:40.000000 mlem-0.4.9/mlem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-23 11:55:26.000000 mlem-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-23 11:55:26.000000 mlem-0.4.9/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-23 11:55:40.544458 mlem-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-03-23 11:55:26.000000 mlem-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.536458 mlem-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.536458 mlem-0.4.9/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/api/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/api/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/api/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.536458 mlem-0.4.9/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/cli/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/cli/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/cli/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/cli/test_checkenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/cli/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/cli/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16295 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/cli/test_declare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16476 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/cli/test_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/cli/test_import_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/cli/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/cli/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/cli/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/cli/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/cli/test_serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/cli/test_stderr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/cli/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.540458 mlem-0.4.9/tests/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.540458 mlem-0.4.9/tests/contrib/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/resources/im.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.540458 mlem-0.4.9/tests/contrib/resources/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/resources/pandas/.mlem.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_bitbucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_callable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_catboost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.540458 mlem-0.4.9/tests/contrib/test_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_docker/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.540458 mlem-0.4.9/tests/contrib/test_docker/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_docker/resources/dockerfile.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_docker/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_docker/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_docker/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_docker/test_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_docker/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_heroku.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.540458 mlem-0.4.9/tests/contrib/test_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_kubernetes/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_kubernetes/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_kubernetes/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_kubernetes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/contrib/test_xgboost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.540458 mlem-0.4.9/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.540458 mlem-0.4.9/tests/core/custom_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/custom_requirements/model_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.544458 mlem-0.4.9/tests/core/custom_requirements/pack_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/custom_requirements/pack_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/custom_requirements/pack_1/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/custom_requirements/pack_1/model_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.544458 mlem-0.4.9/tests/core/custom_requirements/pack_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/custom_requirements/pack_2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.544458 mlem-0.4.9/tests/core/custom_requirements/pkg/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/custom_requirements/pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/custom_requirements/pkg/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.544458 mlem-0.4.9/tests/core/custom_requirements/pkg/subpkg/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/custom_requirements/pkg/subpkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/custom_requirements/pkg/subpkg/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/custom_requirements/pkg/subpkg/testfile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/custom_requirements/pkg_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/custom_requirements/proxy_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/custom_requirements/proxy_pkg_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/custom_requirements/shell_reqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/custom_requirements/test_remote_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/custom_requirements/test_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/custom_requirements/test_shell_reqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/custom_requirements/unused_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/custom_requirements/use_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/custom_requirements/use_model_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.544458 mlem-0.4.9/tests/core/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/resources/emoji_model_inside.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/resources/emoji_model_outside.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/resources/emoji_model_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/resources/file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/resources/server.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/test_data_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19790 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/test_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/test_meta_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/test_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/core/test_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.544458 mlem-0.4.9/tests/polydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/polydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/polydantic/test_lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/polydantic/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/polydantic/test_serde.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.524458 mlem-0.4.9/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.544458 mlem-0.4.9/tests/resources/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/resources/empty/.mlem.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.544458 mlem-0.4.9/tests/resources/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/resources/storage/.mlem.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.544458 mlem-0.4.9/tests/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/runtime/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/runtime/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/runtime/test_model_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/test_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/test_telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:40.544458 mlem-0.4.9/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/utils/module_tools_mock_req.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/utils/test_entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/utils/test_fslock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/utils/test_module_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/utils/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/utils/test_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-23 11:55:26.000000 mlem-0.4.9/tests/utils/test_save.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-23 11:55:26.000000 mlem-0.4.9/tox.ini
```

### Comparing `mlem-0.4.8/.github/workflows/check-test-release.yml` & `mlem-0.4.9/.github/workflows/check-test-release.yml`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/.gitignore` & `mlem-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/.pre-commit-config.yaml` & `mlem-0.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/.pylintrc` & `mlem-0.4.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/LICENSE` & `mlem-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/PKG-INFO` & `mlem-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlem
-Version: 0.4.8
+Version: 0.4.9
 Summary: Version and deploy your models following GitOps principles
 Home-page: https://mlem.ai
 Download-URL: https://github.com/iterative/mlem
 Author: Mikhail Sveshnikov
 Author-email: mike0sv@iterative.ai
 Maintainer: Iterative
 Maintainer-email: support@mlem.ai
@@ -260,17 +260,14 @@
 ```
 
 ## Contributing
 
 Contributions are welcome! Please see our [Contributing Guide](https://mlem.ai/doc/contributing/core)
 for more details.
 
-Check out the [MLEM weekly board](https://github.com/orgs/iterative/projects/322/views/4)
-to learn about what we do, and about the exciting new functionality that is going to be added soon.
-
 Thanks to all our contributors!
 
 ## Copyright
 
 This project is distributed under the Apache license version 2.0 (see the LICENSE file in the project root).
 
 By submitting a pull request to this project, you agree to license your contribution under the Apache license version 2.0 to this project.
```

### Comparing `mlem-0.4.8/README.md` & `mlem-0.4.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -198,17 +198,14 @@
 ```
 
 ## Contributing
 
 Contributions are welcome! Please see our [Contributing Guide](https://mlem.ai/doc/contributing/core)
 for more details.
 
-Check out the [MLEM weekly board](https://github.com/orgs/iterative/projects/322/views/4)
-to learn about what we do, and about the exciting new functionality that is going to be added soon.
-
 Thanks to all our contributors!
 
 ## Copyright
 
 This project is distributed under the Apache license version 2.0 (see the LICENSE file in the project root).
 
 By submitting a pull request to this project, you agree to license your contribution under the Apache license version 2.0 to this project.
```

### Comparing `mlem-0.4.8/mlem/api/commands.py` & `mlem-0.4.9/mlem/api/commands.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/api/migrations.py` & `mlem-0.4.9/mlem/api/migrations.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/api/utils.py` & `mlem-0.4.9/mlem/api/utils.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/cli/__init__.py` & `mlem-0.4.9/mlem/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/cli/apply.py` & `mlem-0.4.9/mlem/cli/apply.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/cli/build.py` & `mlem-0.4.9/mlem/cli/build.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/cli/checkenv.py` & `mlem-0.4.9/mlem/cli/checkenv.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/cli/clone.py` & `mlem-0.4.9/mlem/cli/clone.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/cli/config.py` & `mlem-0.4.9/mlem/cli/config.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/cli/declare.py` & `mlem-0.4.9/mlem/cli/declare.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/cli/deployment.py` & `mlem-0.4.9/mlem/cli/deployment.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 from mlem.core.objects import (
     DeployState,
     DeployStatus,
     MlemDeployment,
     MlemModel,
 )
 from mlem.telemetry import pass_telemetry_params
-from mlem.ui import echo, no_echo, set_echo
+from mlem.ui import EMOJI_STOP, echo, no_echo, set_echo
 
 logger = logging.getLogger(__name__)
 
 deployment = Typer(
     name="deployment",
     help="A set of commands to set up and manage deployments",
     cls=mlem_group("runtime", aliases=["deploy"]),
@@ -112,14 +112,17 @@
             ..., help="Where to save the object (.mlem file)"
         ),
         model: str = make_not_required(option_model),
         model_project: Optional[str] = option_model_project,
         model_rev: Optional[str] = option_model_rev,
         project: Optional[str] = option_project,
         file_conf: List[str] = option_file_conf("deployment"),
+        force: bool = Option(
+            False, is_flag=True, help="Force re-create if parameters changed"
+        ),
         **__kwargs__,
     ):
         from mlem.api.commands import deploy
 
         if model is None:
             raise click.MissingParameter(
                 param=get_click_param(
@@ -135,17 +138,26 @@
             str_conf=None,
             file_conf=file_conf,
             **__kwargs__,
         )
         try:
             meta = load_meta(path, project=project, force_type=MlemDeployment)
             if meta != _meta:
-                raise DeploymentError(
-                    f"Different deployment meta already exists at {meta.loc}. Please use `mlem deployment run --load <path> ...`"
-                )
+                if not meta.is_state_empty:
+                    if not force:
+                        raise DeploymentError(
+                            f"Different deployment meta already exists at {meta.loc}. Please use `mlem deployment run --load <path> ...`"
+                        )
+                    echo(
+                        EMOJI_STOP
+                        + "Removing old deployment since parameters changed"
+                    )
+                    meta.remove()
+                with wrap_build_error(type_name, MlemDeployment):
+                    meta = _meta.dump(path, project=project)
         except MlemObjectNotFound:
             with wrap_build_error(type_name, MlemDeployment):
                 meta = _meta.dump(path, project=project)
         mlem_model = load_meta(
             model,
             project=model_project,
             rev=model_rev,
```

### Comparing `mlem-0.4.8/mlem/cli/dev.py` & `mlem-0.4.9/mlem/cli/dev.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/cli/import_object.py` & `mlem-0.4.9/mlem/cli/import_object.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/cli/info.py` & `mlem-0.4.9/mlem/cli/info.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/cli/link.py` & `mlem-0.4.9/mlem/cli/link.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/cli/main.py` & `mlem-0.4.9/mlem/cli/main.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/cli/migrate.py` & `mlem-0.4.9/mlem/cli/migrate.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/cli/serve.py` & `mlem-0.4.9/mlem/cli/serve.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/cli/types.py` & `mlem-0.4.9/mlem/cli/types.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/cli/utils.py` & `mlem-0.4.9/mlem/cli/utils.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/config.py` & `mlem-0.4.9/mlem/config.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/bitbucketfs.py` & `mlem-0.4.9/mlem/contrib/bitbucketfs.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/callable.py` & `mlem-0.4.9/mlem/contrib/callable.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/catboost.py` & `mlem-0.4.9/mlem/contrib/catboost.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/docker/base.py` & `mlem-0.4.9/mlem/contrib/docker/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,19 @@
 import docker
 import requests
 from docker import errors
 from docker.errors import NotFound
 from pydantic import BaseModel
 
 from mlem.config import LOCAL_CONFIG, project_config
-from mlem.contrib.docker.context import DockerBuildArgs, DockerModelDirectory
+from mlem.contrib.docker.context import (
+    DockerBuildArgs,
+    DockerModelDirectory,
+    get_build_args,
+)
 from mlem.contrib.docker.utils import (
     build_image_with_logs,
     container_is_running,
     container_logs,
     container_status,
     create_docker_client,
     image_exists_at_dockerhub,
@@ -588,14 +592,15 @@
             try:
                 image, _ = build_image_with_logs(
                     client,
                     path=context_dir,
                     tag=tag,
                     rm=True,
                     platform=self.args.platform,
+                    buildargs=get_build_args(self.args.build_arg),
                 )
                 docker_image = DockerImage(**self.image.dict())
                 docker_image.image_id = image.id
                 echo(EMOJI_OK + f"Built docker image {tag}")
 
                 if self.push:
                     docker_image.registry.push(client, tag)
```

### Comparing `mlem-0.4.8/mlem/contrib/docker/context.py` & `mlem-0.4.9/mlem/contrib/docker/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -240,14 +240,16 @@
     """command to clean after package installation"""
     prebuild_hook: Optional[Callable[[str], Any]] = None
     """callable to call before build, accepts python version. Used for pre-building server images"""
     mlem_whl: Optional[str] = None
     """a path to mlem .whl file. If it is empty, mlem will be installed from pip"""
     platform: Optional[str] = None
     """platform to build docker for, see docs.docker.com/desktop/multi-arch/"""
+    build_arg: List[str] = []
+    """args to use at build time https://docs.docker.com/engine/reference/commandline/build/#build-arg"""
 
     def get_base_image(self):
         if self.base_image is None:
             return f"python:{self.python_version}-slim"
         if isinstance(self.base_image, str):
             return self.base_image
         if not callable(self.base_image):
@@ -266,14 +268,25 @@
                 self.templates_dir += other.templates_dir
             else:
                 value = getattr(other, field)
                 if value is not None:
                     setattr(self, field, value)
 
 
+def get_build_args(build_arg) -> Dict[str, Optional[str]]:
+    args = {}
+    for arg in build_arg:
+        if "=" in arg:
+            key, value = arg.split("=", 1)
+            args[key] = os.getenv(arg) or value
+        else:
+            args[arg] = os.getenv(arg)
+    return args
+
+
 class DockerModelDirectory(BaseModel):
     model: MlemModel
     server: Server
     docker_args: "DockerBuildArgs"
     debug: bool
     path: str
     model_name: str = "model"
@@ -366,15 +379,17 @@
         with open(
             os.path.join(self.path, "Dockerfile"), "w", encoding="utf8"
         ) as df:
             unix_packages = requirements.of_type(UnixPackageRequirement)
             dockerfile = DockerfileGenerator(
                 **self.docker_args.dict()
             ).generate(
-                env=env, packages=[p.package_name for p in unix_packages or []]
+                env=env,
+                arg=get_build_args(self.docker_args.build_arg),
+                packages=[p.package_name for p in unix_packages or []],
             )
             df.write(dockerfile)
 
     def write_configs(self):
         with self.fs.open(
             posixpath.join(self.path, SERVER), "w", encoding="utf8"
         ) as f:
```

### Comparing `mlem-0.4.8/mlem/contrib/docker/helpers.py` & `mlem-0.4.9/mlem/contrib/docker/helpers.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/docker/utils.py` & `mlem-0.4.9/mlem/contrib/docker/utils.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/dvc.py` & `mlem-0.4.9/mlem/contrib/dvc.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/fastapi.py` & `mlem-0.4.9/mlem/contrib/fastapi.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/flyio/meta.py` & `mlem-0.4.9/mlem/contrib/flyio/meta.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/flyio/utils.py` & `mlem-0.4.9/mlem/contrib/flyio/utils.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/git.py` & `mlem-0.4.9/mlem/contrib/git.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/github.py` & `mlem-0.4.9/mlem/contrib/github.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/gitlabfs.py` & `mlem-0.4.9/mlem/contrib/gitlabfs.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/heroku/build.py` & `mlem-0.4.9/mlem/contrib/heroku/build.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/heroku/meta.py` & `mlem-0.4.9/mlem/contrib/heroku/meta.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/heroku/server.py` & `mlem-0.4.9/mlem/contrib/heroku/server.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/heroku/utils.py` & `mlem-0.4.9/mlem/contrib/heroku/utils.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/kubernetes/base.py` & `mlem-0.4.9/mlem/contrib/kubernetes/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,14 +74,16 @@
     """Docker registry"""
     daemon: Optional[DockerDaemon] = DockerDaemon(host="")
     """Docker daemon"""
     kube_config_file_path: Optional[str] = None
     """Path for kube config file of the cluster"""
     templates_dir: List[str] = []
     """List of dirs where templates reside"""
+    build_arg: List[str] = []
+    """Args to use at build time https://docs.docker.com/engine/reference/commandline/build/#build-arg"""
 
     def load_kube_config(self):
         config.load_kube_config(
             config_file=self.kube_config_file_path
             or os.getenv("KUBECONFIG", default="~/.kube/config")
         )
 
@@ -130,14 +132,15 @@
                 image_name = self.get_image_name()
                 state.image = build_k8s_docker(
                     meta=model,
                     image_name=image_name,
                     registry=self.get_registry(),
                     daemon=self.daemon,
                     server=self.get_server(),
+                    build_arg=self.build_arg,
                 )
                 state.update_model(model)
                 redeploy = True
 
             if (
                 state.deployment_name is None or redeploy
             ) and state.image is not None:
```

### Comparing `mlem-0.4.8/mlem/contrib/kubernetes/build.py` & `mlem-0.4.9/mlem/contrib/kubernetes/build.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import List, Optional
 
 from mlem.core.objects import MlemModel
 from mlem.runtime.server import Server
 from mlem.ui import EMOJI_BUILD, echo, set_offset
 
 from ..docker.base import DockerDaemon, DockerRegistry
 from ..docker.helpers import build_model_image
@@ -12,20 +12,22 @@
     meta: MlemModel,
     image_name: str,
     registry: Optional[DockerRegistry],
     daemon: Optional[DockerDaemon],
     server: Server,
     platform: Optional[str] = "linux/amd64",
     # runners usually do not support arm64 images built on Mac M1 devices
+    build_arg: Optional[List[str]] = None,
 ):
     echo(EMOJI_BUILD + f"Creating docker image {image_name}")
     with set_offset(2):
         return build_model_image(
             meta,
             image_name,
             server,
             daemon=daemon,
             registry=registry,
             tag=meta.meta_hash(),
             force_overwrite=True,
             platform=platform,
+            build_arg=build_arg or [],
         )
```

### Comparing `mlem-0.4.8/mlem/contrib/kubernetes/context.py` & `mlem-0.4.9/mlem/contrib/kubernetes/context.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/kubernetes/resources.yaml.j2` & `mlem-0.4.9/mlem/contrib/kubernetes/resources.yaml.j2`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/kubernetes/service.py` & `mlem-0.4.9/mlem/contrib/kubernetes/service.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/kubernetes/utils.py` & `mlem-0.4.9/mlem/contrib/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/lightgbm.py` & `mlem-0.4.9/mlem/contrib/lightgbm.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/numpy.py` & `mlem-0.4.9/mlem/contrib/numpy.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/onnx.py` & `mlem-0.4.9/mlem/contrib/onnx.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/pandas.py` & `mlem-0.4.9/mlem/contrib/pandas.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/pil.py` & `mlem-0.4.9/mlem/contrib/pil.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/pip/base.py` & `mlem-0.4.9/mlem/contrib/pip/base.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/pip/setup.py.j2` & `mlem-0.4.9/mlem/contrib/pip/setup.py.j2`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/rabbitmq.py` & `mlem-0.4.9/mlem/contrib/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/requirements.py` & `mlem-0.4.9/mlem/contrib/requirements.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/sagemaker/build.py` & `mlem-0.4.9/mlem/contrib/sagemaker/build.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/sagemaker/env_setup.py` & `mlem-0.4.9/mlem/contrib/sagemaker/env_setup.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/sagemaker/meta.py` & `mlem-0.4.9/mlem/contrib/sagemaker/meta.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/sagemaker/mlem_sagemaker.tf` & `mlem-0.4.9/mlem/contrib/sagemaker/mlem_sagemaker.tf`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/sagemaker/runtime.py` & `mlem-0.4.9/mlem/contrib/sagemaker/runtime.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/sagemaker/utils.py` & `mlem-0.4.9/mlem/contrib/sagemaker/utils.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/scipy.py` & `mlem-0.4.9/mlem/contrib/scipy.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/sklearn.py` & `mlem-0.4.9/mlem/contrib/sklearn.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 ModelType implementations for any sklearn-compatible classes as well as `Pipeline`
 """
 from typing import Any, ClassVar, Dict, List, Optional, Union
 
 import sklearn
 from sklearn.base import ClassifierMixin, RegressorMixin
-from sklearn.feature_extraction.text import TransformerMixin
+from sklearn.feature_extraction.text import TransformerMixin, _VectorizerMixin
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing._encoders import _BaseEncoder
 
 from mlem.constants import TRANSFORM_METHOD_NAME
 from mlem.core.hooks import IsInstanceHookMixin
 from mlem.core.model import (
     ModelHook,
@@ -137,15 +137,15 @@
 
 
 class SklearnTransformer(SklearnModel):
     """
     Model Type implementation for sklearn transformers
     """
 
-    valid_types: ClassVar = (TransformerMixin, _BaseEncoder)
+    valid_types: ClassVar = (TransformerMixin, _BaseEncoder, _VectorizerMixin)
     type: ClassVar = "sklearn_transformer"
 
     @classmethod
     def process(
         cls,
         obj: Any,
         sample_data: Optional[Any] = None,
@@ -155,15 +155,15 @@
         methods_sample_data = methods_sample_data or {}
         sample_data = methods_sample_data.get(
             TRANSFORM_METHOD_NAME, sample_data
         )
         methods = {
             TRANSFORM_METHOD_NAME: Signature.from_method(
                 obj.transform,
+                sample_data,
                 auto_infer=sample_data is not None,
-                X=sample_data,
             ),
         }
 
         return SklearnTransformer(io=SimplePickleIO(), methods=methods).bind(
             obj
         )
```

### Comparing `mlem-0.4.8/mlem/contrib/streamlit/_template.py` & `mlem-0.4.9/mlem/contrib/streamlit/_template.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/streamlit/server.py` & `mlem-0.4.9/mlem/contrib/streamlit/server.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/streamlit/utils.py` & `mlem-0.4.9/mlem/contrib/streamlit/utils.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/tensorflow.py` & `mlem-0.4.9/mlem/contrib/tensorflow.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/torch.py` & `mlem-0.4.9/mlem/contrib/torch.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/torchvision.py` & `mlem-0.4.9/mlem/contrib/torchvision.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/venv.py` & `mlem-0.4.9/mlem/contrib/venv.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/contrib/xgboost.py` & `mlem-0.4.9/mlem/contrib/xgboost.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/core/artifacts.py` & `mlem-0.4.9/mlem/core/artifacts.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/core/base.py` & `mlem-0.4.9/mlem/core/base.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/core/data_type.py` & `mlem-0.4.9/mlem/core/data_type.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/core/errors.py` & `mlem-0.4.9/mlem/core/errors.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/core/hooks.py` & `mlem-0.4.9/mlem/core/hooks.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/core/import_objects.py` & `mlem-0.4.9/mlem/core/import_objects.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/core/meta_io.py` & `mlem-0.4.9/mlem/core/meta_io.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/core/metadata.py` & `mlem-0.4.9/mlem/core/metadata.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/core/model.py` & `mlem-0.4.9/mlem/core/model.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/core/objects.py` & `mlem-0.4.9/mlem/core/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1273,14 +1273,18 @@
         return self.state_manager
 
     def get_state(self) -> ST:
         return self._state_manager.get_state(
             self, self.state_type
         ) or self.state_type(declaration=self)
 
+    @property
+    def is_state_empty(self):
+        return self._state_manager.get_state(self, self.state_type) is None
+
     def lock_state(self):
         return self._state_manager.lock_state(self)
 
     def update_state(self, state: ST):
         self._state_manager.update_state(self, state)
 
     def purge_state(self):
```

### Comparing `mlem-0.4.8/mlem/core/requirements.py` & `mlem-0.4.9/mlem/core/requirements.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     Optional,
     Sequence,
     Type,
     TypeVar,
     Union,
 )
 
+from importlib_metadata import Distribution, PackageNotFoundError
 from pydantic import BaseModel, root_validator
 
 from mlem.core.base import MlemABC
 
 # I dont know how to do this better
 from mlem.core.errors import HookNotFound, WrongRequirementsError
 from mlem.core.hooks import Analyzer, Hook
@@ -82,14 +83,20 @@
     """Name of python module"""
     version: Optional[str] = None
     """Version of python package"""
     package_name: Optional[str] = None
     """Pip package name for this module, if it is different from module name"""
     extra_index: Optional[str] = None
     """Extra index to use for this package"""
+    source_url: Optional[str] = None
+    """URL to download package from"""
+    vcs: Optional[str] = None
+    """Version control system"""
+    vcs_commit: Optional[str] = None
+    """Commit hash to checkout from VCS"""
 
     @root_validator
     def set_package_name(cls, values):  # pylint: disable=no-self-argument
         package_name = values.get("package_name")
         if not package_name:
             from mlem.utils.module import get_package_name
 
@@ -108,14 +115,16 @@
 
     def get_repr(self):
         """
         pip installable representation of this module
         """
         if self.version is not None:
             return f"{self.package}=={self.version}"
+        if self.vcs_commit is not None:
+            return f"{self.vcs}+{self.source_url}@{self.vcs_commit}"
         return self.package
 
     @classmethod
     def materialize(cls, reqs, target: str):
         reqs = [r.get_repr() for r in reqs]
         requirement_string = "\n".join(reqs)
         with open(os.path.join(target), "w", encoding="utf8") as fp:
@@ -130,18 +139,45 @@
 
         :param mod: module object
         :param package_name: PIP package name if it is not equal to module name
         :return: :class:`InstallableRequirement`
         """
         from mlem.utils.module import get_module_version
 
+        # similar package resolution exists in mlem/contrib/docker/context.py
+        source_url = None
+        vcs = None
+        rev = None
+
+        try:
+            pkg_info = json.loads(
+                Distribution.from_name(mod.__name__).read_text(
+                    "direct_url.json"
+                )
+            )
+        except (PackageNotFoundError, json.JSONDecodeError, TypeError):
+            pass
+        else:
+            if "url" in pkg_info:
+                source_url = pkg_info["url"]
+                # installed from local source:
+                if source_url.startswith("file://"):
+                    return CustomRequirement.from_module(mod)  # type: ignore
+                # installed from git branch (probably):
+                if "vcs_info" in pkg_info:
+                    rev = pkg_info["vcs_info"]["commit_id"]
+                    vcs = pkg_info["vcs_info"]["vcs"]
+
         return InstallableRequirement(
             module=mod.__name__,
-            version=get_module_version(mod),
+            version=None if rev else get_module_version(mod),
             package_name=package_name,
+            source_url=source_url,
+            vcs_commit=rev,
+            vcs=vcs,
         )
 
     @classmethod
     def from_str(cls, name):
         """
         Factory method for creating :class:`InstallableRequirement` from string
```

### Comparing `mlem-0.4.8/mlem/ext.py` & `mlem-0.4.9/mlem/ext.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/log.py` & `mlem-0.4.9/mlem/log.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/polydantic/core.py` & `mlem-0.4.9/mlem/polydantic/core.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/polydantic/lazy.py` & `mlem-0.4.9/mlem/polydantic/lazy.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/runtime/client.py` & `mlem-0.4.9/mlem/runtime/client.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/runtime/interface.py` & `mlem-0.4.9/mlem/runtime/interface.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/runtime/server.py` & `mlem-0.4.9/mlem/runtime/server.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/telemetry.py` & `mlem-0.4.9/mlem/telemetry.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/ui.py` & `mlem-0.4.9/mlem/ui.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/utils/backport.py` & `mlem-0.4.9/mlem/utils/backport.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/utils/entrypoints.py` & `mlem-0.4.9/mlem/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/utils/fslock.py` & `mlem-0.4.9/mlem/utils/fslock.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/utils/importing.py` & `mlem-0.4.9/mlem/utils/importing.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/utils/mlem.isort.cfg` & `mlem-0.4.9/mlem/utils/mlem.isort.cfg`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/utils/module.py` & `mlem-0.4.9/mlem/utils/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,15 +327,15 @@
     :param validate_pypi: if `True` (default is `False`) perform representation validation in PyPi repository
     :return: representation as :class:`.InstallableRequirement`
     """
     mod_version = get_module_version(mod)
     if validate_pypi:
         mod_name = get_package_name(mod)
         check_pypi_module(mod_name, mod_version, raise_on_error=True)
-    return InstallableRequirement(module=mod.__name__, version=mod_version)
+    return InstallableRequirement.from_module(mod)
 
 
 def get_local_module_reqs(mod) -> List[ModuleType]:
     """Parses module AST to find all import statements"""
     try:
         tree = ast.parse(inspect.getsource(mod))
     except (OSError, TypeError):
```

### Comparing `mlem-0.4.8/mlem/utils/root.py` & `mlem-0.4.9/mlem/utils/root.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem/utils/templates.py` & `mlem-0.4.9/mlem/utils/templates.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem.egg-info/PKG-INFO` & `mlem-0.4.9/mlem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlem
-Version: 0.4.8
+Version: 0.4.9
 Summary: Version and deploy your models following GitOps principles
 Home-page: https://mlem.ai
 Download-URL: https://github.com/iterative/mlem
 Author: Mikhail Sveshnikov
 Author-email: mike0sv@iterative.ai
 Maintainer: Iterative
 Maintainer-email: support@mlem.ai
@@ -260,17 +260,14 @@
 ```
 
 ## Contributing
 
 Contributions are welcome! Please see our [Contributing Guide](https://mlem.ai/doc/contributing/core)
 for more details.
 
-Check out the [MLEM weekly board](https://github.com/orgs/iterative/projects/322/views/4)
-to learn about what we do, and about the exciting new functionality that is going to be added soon.
-
 Thanks to all our contributors!
 
 ## Copyright
 
 This project is distributed under the Apache license version 2.0 (see the LICENSE file in the project root).
 
 By submitting a pull request to this project, you agree to license your contribution under the Apache license version 2.0 to this project.
```

### Comparing `mlem-0.4.8/mlem.egg-info/SOURCES.txt` & `mlem-0.4.9/mlem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem.egg-info/entry_points.txt` & `mlem-0.4.9/mlem.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/mlem.egg-info/requires.txt` & `mlem-0.4.9/mlem.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/setup.cfg` & `mlem-0.4.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/setup.py` & `mlem-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/api/test_commands.py` & `mlem-0.4.9/tests/api/test_commands.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/api/test_migrations.py` & `mlem-0.4.9/tests/api/test_migrations.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/api/test_utils.py` & `mlem-0.4.9/tests/api/test_utils.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/cli/conftest.py` & `mlem-0.4.9/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/cli/test_apply.py` & `mlem-0.4.9/tests/cli/test_apply.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/cli/test_build.py` & `mlem-0.4.9/tests/cli/test_build.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/cli/test_checkenv.py` & `mlem-0.4.9/tests/cli/test_checkenv.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/cli/test_config.py` & `mlem-0.4.9/tests/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/cli/test_declare.py` & `mlem-0.4.9/tests/cli/test_declare.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/cli/test_deployment.py` & `mlem-0.4.9/tests/cli/test_deployment.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/cli/test_import_path.py` & `mlem-0.4.9/tests/cli/test_import_path.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/cli/test_info.py` & `mlem-0.4.9/tests/cli/test_info.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/cli/test_link.py` & `mlem-0.4.9/tests/cli/test_link.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/cli/test_main.py` & `mlem-0.4.9/tests/cli/test_main.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/cli/test_serve.py` & `mlem-0.4.9/tests/cli/test_serve.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/cli/test_stderr.py` & `mlem-0.4.9/tests/cli/test_stderr.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/cli/test_types.py` & `mlem-0.4.9/tests/cli/test_types.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/conftest.py` & `mlem-0.4.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/conftest.py` & `mlem-0.4.9/tests/contrib/conftest.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_bitbucket.py` & `mlem-0.4.9/tests/contrib/test_bitbucket.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_callable.py` & `mlem-0.4.9/tests/contrib/test_callable.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_catboost.py` & `mlem-0.4.9/tests/contrib/test_catboost.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_docker/conftest.py` & `mlem-0.4.9/tests/contrib/test_docker/conftest.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_docker/test_base.py` & `mlem-0.4.9/tests/contrib/test_docker/test_base.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_docker/test_context.py` & `mlem-0.4.9/tests/contrib/test_docker/test_context.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 REGISTRY_PORT = 5000
 
 
 def test_dockerfile_generator_custom_python_version():
     dockerfile = _cut_empty_lines(
         f"""FROM python:AAAA-slim
 WORKDIR /app
+# install Git in case something in requirements.txt will be installed from Git repo
+RUN apt-get update && apt-get -y upgrade && apt-get install --no-install-recommends -y git && apt-get clean && rm -rf /var/lib/apt/lists/*
 COPY requirements.txt .
 RUN pip install -r requirements.txt && pip cache purge
 COPY mlem_requirements.txt .
 RUN pip install -r mlem_requirements.txt && pip cache purge
 COPY {MLEM_LOCAL_WHL} .
 RUN pip install {MLEM_LOCAL_WHL} && (pip cache purge || true)
 COPY . ./
@@ -36,14 +38,16 @@
     assert _generate_dockerfile(**kwargs) == dockerfile
 
 
 def test_dockerfile_generator_unix_packages():
     dockerfile = _cut_empty_lines(
         f"""FROM python:3.6-slim
 WORKDIR /app
+# install Git in case something in requirements.txt will be installed from Git repo
+RUN kek git lol
 RUN kek aaa bbb lol
 COPY requirements.txt .
 RUN pip install -r requirements.txt && pip cache purge
 RUN pip install mlem=={mlem.__version__} && pip cache purge
 COPY . ./
 CMD sh run.sh
 """
@@ -68,14 +72,16 @@
 
 
 def test_dockerfile_generator_super_custom():
     dockerfile = _cut_empty_lines(
         f"""FROM my-python:3.6
 WORKDIR /app
 RUN echo "pre_install"
+# install Git in case something in requirements.txt will be installed from Git repo
+RUN apt-get update && apt-get -y upgrade && apt-get install --no-install-recommends -y git && apt-get clean && rm -rf /var/lib/apt/lists/*
 COPY requirements.txt .
 RUN pip install -r requirements.txt && pip cache purge
 RUN pip install mlem=={mlem.__version__} && pip cache purge
 RUN echo "post_install"
 COPY . ./
 RUN echo "post_copy"
 CMD echo "cmd" && sh run.sh
@@ -105,22 +111,26 @@
 
 
 def test_use_wheel_installation(tmpdir):
     distr = tmpdir.mkdir("distr").join("somewhatwheel.txt")
     distr.write("wheel goes brrr")
     with use_mlem_source("whl"):
         os.environ["MLEM_DOCKER_WHEEL_PATH"] = str(os.path.basename(distr))
-        dockerfile = DockerfileGenerator().generate(env={}, packages=[])
+        dockerfile = DockerfileGenerator().generate(
+            env={}, packages=[], arg={}
+        )
         assert f"RUN pip install {MLEM_LOCAL_WHL}" in dockerfile
 
 
 def _generate_dockerfile(unix_packages=None, **kwargs):
     return _cut_empty_lines(
         DockerfileGenerator(**kwargs).generate(
-            env={}, packages=[p.package_name for p in unix_packages or []]
+            env={},
+            packages=[p.package_name for p in unix_packages or []],
+            arg={},
         )
     )
 
 
 @docker_test
 def test_docker_registry_io():
     registry = DockerIORegistry()
```

### Comparing `mlem-0.4.8/tests/contrib/test_docker/test_deploy.py` & `mlem-0.4.9/tests/contrib/test_docker/test_deploy.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_docker/test_pack.py` & `mlem-0.4.9/tests/contrib/test_docker/test_pack.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_docker/test_utils.py` & `mlem-0.4.9/tests/contrib/test_docker/test_utils.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_fastapi.py` & `mlem-0.4.9/tests/contrib/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_github.py` & `mlem-0.4.9/tests/contrib/test_github.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_gitlab.py` & `mlem-0.4.9/tests/contrib/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_heroku.py` & `mlem-0.4.9/tests/contrib/test_heroku.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_kubernetes/conftest.py` & `mlem-0.4.9/tests/contrib/test_kubernetes/conftest.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_kubernetes/test_base.py` & `mlem-0.4.9/tests/contrib/test_kubernetes/test_base.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_kubernetes/test_context.py` & `mlem-0.4.9/tests/contrib/test_kubernetes/test_context.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_kubernetes/utils.py` & `mlem-0.4.9/tests/contrib/test_kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_lightgbm.py` & `mlem-0.4.9/tests/contrib/test_lightgbm.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_numpy.py` & `mlem-0.4.9/tests/contrib/test_numpy.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_onnx.py` & `mlem-0.4.9/tests/contrib/test_onnx.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_pandas.py` & `mlem-0.4.9/tests/contrib/test_pandas.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_pil.py` & `mlem-0.4.9/tests/contrib/test_pil.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_pip.py` & `mlem-0.4.9/tests/contrib/test_pip.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_rabbitmq.py` & `mlem-0.4.9/tests/contrib/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_requirements.py` & `mlem-0.4.9/tests/contrib/test_requirements.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_scipy.py` & `mlem-0.4.9/tests/contrib/test_scipy.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_sklearn.py` & `mlem-0.4.9/tests/contrib/test_sklearn.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import posixpath
 
 import lightgbm as lgb
 import numpy as np
 import pytest
-from sklearn.feature_extraction.text import TfidfTransformer
+from sklearn.feature_extraction.text import CountVectorizer, TfidfTransformer
 from sklearn.linear_model import LinearRegression, LogisticRegression
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import OneHotEncoder, StandardScaler
 from sklearn.svm import SVC
 
 from mlem.api import apply, load_meta, save
 from mlem.constants import PREDICT_METHOD_NAME, TRANSFORM_METHOD_NAME
@@ -19,14 +19,22 @@
 from mlem.core.model import Argument, ModelAnalyzer
 from mlem.core.objects import MlemModel
 from mlem.core.requirements import UnixPackageRequirement
 from tests.conftest import long
 
 
 @pytest.fixture
+def text_inp_data():
+    return [
+        "This is the first document.",
+        "This document is the second document.",
+    ]
+
+
+@pytest.fixture
 def inp_data():
     return [[1, 2, 3], [3, 2, 1]]
 
 
 @pytest.fixture
 def out_data():
     return [1, 2]
@@ -43,14 +51,21 @@
 def regressor(inp_data, out_data):
     lr = LinearRegression()
     lr.fit(inp_data, out_data)
     return lr
 
 
 @pytest.fixture
+def count_vectorizer(text_inp_data):
+    vectorizer = CountVectorizer()
+    vectorizer.fit(text_inp_data)
+    return vectorizer
+
+
+@pytest.fixture
 def transformer(inp_data):
     tf_idf = TfidfTransformer()
     tf_idf.fit(inp_data)
     return tf_idf
 
 
 @pytest.fixture
@@ -90,41 +105,58 @@
     signature = model_type.methods[PREDICT_METHOD_NAME]
     assert signature.name == PREDICT_METHOD_NAME
     assert signature.args[0] == Argument(name="X", type_=data_type)
     assert signature.returns == returns
 
 
 @pytest.mark.parametrize(
-    "transformer_fixture", ["transformer", "onehotencoder"]
+    "transformer_fixture", ["transformer", "onehotencoder", "count_vectorizer"]
 )
-def test_hook_transformer(transformer_fixture, inp_data, request):
+def test_hook_transformer(
+    transformer_fixture, inp_data, text_inp_data, request
+):
     transformer = request.getfixturevalue(transformer_fixture)
-    data_type = DataAnalyzer.analyze(inp_data)
-    model_type = ModelAnalyzer.analyze(transformer, sample_data=inp_data)
+    if transformer_fixture == "count_vectorizer":
+        input_data = text_inp_data
+        argname = "raw_documents"
+    else:
+        input_data = inp_data
+        argname = "X"
+    data_type = DataAnalyzer.analyze(input_data)
+    model_type = ModelAnalyzer.analyze(transformer, sample_data=input_data)
     assert isinstance(model_type, SklearnTransformer)
     assert TRANSFORM_METHOD_NAME in model_type.methods
     signature = model_type.methods[TRANSFORM_METHOD_NAME]
     cols = len(transformer.get_feature_names_out())
-    rows = len(inp_data)
-    returns = ScipySparseMatrix(dtype="float64", shape=(rows, cols))
+    rows = len(input_data)
+    if transformer_fixture == "count_vectorizer":
+        returns = ScipySparseMatrix(dtype="int64", shape=(rows, cols))
+    else:
+        returns = ScipySparseMatrix(dtype="float64", shape=(rows, cols))
     assert signature.name == TRANSFORM_METHOD_NAME
-    assert signature.args[0] == Argument(name="X", type_=data_type)
+    assert signature.args[0] == Argument(name=argname, type_=data_type)
     assert signature.returns == returns
 
 
 @pytest.mark.parametrize(
-    "transformer_fixture", ["transformer", "onehotencoder"]
+    "transformer_fixture", ["transformer", "onehotencoder", "count_vectorizer"]
 )
-def test_model_type__transform(transformer_fixture, inp_data, request):
+def test_model_type__transform(
+    transformer_fixture, inp_data, text_inp_data, request
+):
     transformer = request.getfixturevalue(transformer_fixture)
-    model_type = ModelAnalyzer.analyze(transformer, sample_data=inp_data)
+    if transformer_fixture == "count_vectorizer":
+        input_data = text_inp_data
+    else:
+        input_data = inp_data
+    model_type = ModelAnalyzer.analyze(transformer, sample_data=input_data)
 
     np.testing.assert_array_almost_equal(
-        transformer.transform(inp_data).todense(),
-        model_type.call_method("transform", inp_data).todense(),
+        transformer.transform(input_data).todense(),
+        model_type.call_method("transform", input_data).todense(),
     )
 
 
 @pytest.mark.parametrize(
     "transformer_fixture", ["transformer", "onehotencoder"]
 )
 def test_preprocess_transformer(
```

### Comparing `mlem-0.4.8/tests/contrib/test_streamlit.py` & `mlem-0.4.9/tests/contrib/test_streamlit.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_tensorflow.py` & `mlem-0.4.9/tests/contrib/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_torch.py` & `mlem-0.4.9/tests/contrib/test_torch.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_venv.py` & `mlem-0.4.9/tests/contrib/test_venv.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/contrib/test_xgboost.py` & `mlem-0.4.9/tests/contrib/test_xgboost.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/core/custom_requirements/pack_1/model_type.py` & `mlem-0.4.9/tests/core/custom_requirements/pack_1/model_type.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/core/custom_requirements/test_requirements.py` & `mlem-0.4.9/tests/core/custom_requirements/test_requirements.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/core/custom_requirements/test_shell_reqs.py` & `mlem-0.4.9/tests/core/custom_requirements/test_shell_reqs.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/core/test_artifacts.py` & `mlem-0.4.9/tests/core/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/core/test_base.py` & `mlem-0.4.9/tests/core/test_base.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/core/test_data_io.py` & `mlem-0.4.9/tests/core/test_data_io.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/core/test_data_type.py` & `mlem-0.4.9/tests/core/test_data_type.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/core/test_meta_io.py` & `mlem-0.4.9/tests/core/test_meta_io.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/core/test_metadata.py` & `mlem-0.4.9/tests/core/test_metadata.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/core/test_model_type.py` & `mlem-0.4.9/tests/core/test_model_type.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/core/test_objects.py` & `mlem-0.4.9/tests/core/test_objects.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/core/test_requirements.py` & `mlem-0.4.9/tests/core/test_requirements.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/polydantic/test_lazy.py` & `mlem-0.4.9/tests/polydantic/test_lazy.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/polydantic/test_multi.py` & `mlem-0.4.9/tests/polydantic/test_multi.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/polydantic/test_serde.py` & `mlem-0.4.9/tests/polydantic/test_serde.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/runtime/test_client.py` & `mlem-0.4.9/tests/runtime/test_client.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/runtime/test_interface.py` & `mlem-0.4.9/tests/runtime/test_interface.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/runtime/test_model_interface.py` & `mlem-0.4.9/tests/runtime/test_model_interface.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/test_config.py` & `mlem-0.4.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/test_ext.py` & `mlem-0.4.9/tests/test_ext.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/test_setup.py` & `mlem-0.4.9/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/utils/test_entrypoints.py` & `mlem-0.4.9/tests/utils/test_entrypoints.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/utils/test_fslock.py` & `mlem-0.4.9/tests/utils/test_fslock.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/utils/test_module_tools.py` & `mlem-0.4.9/tests/utils/test_module_tools.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/utils/test_path.py` & `mlem-0.4.9/tests/utils/test_path.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/utils/test_root.py` & `mlem-0.4.9/tests/utils/test_root.py`

 * *Files identical despite different names*

### Comparing `mlem-0.4.8/tests/utils/test_save.ipynb` & `mlem-0.4.9/tests/utils/test_save.ipynb`

 * *Files identical despite different names*

