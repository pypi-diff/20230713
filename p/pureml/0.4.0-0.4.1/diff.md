# Comparing `tmp/pureml-0.4.0.tar.gz` & `tmp/pureml-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pureml-0.4.0.tar", max compression
+gzip compressed data, was "pureml-0.4.1.tar", max compression
```

## Comparing `pureml-0.4.0.tar` & `pureml-0.4.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0     6690 2023-05-21 10:58:34.529091 pureml-0.4.0/README.md
--rw-r--r--   0        0        0      735 2023-07-13 09:52:21.777305 pureml-0.4.0/pureml/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/cli/__init__.py
--rw-r--r--   0        0        0     9766 2023-07-10 21:08:37.716024 pureml-0.4.0/pureml/cli/auth.py
--rw-r--r--   0        0        0     2285 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/cli/helpers.py
--rw-r--r--   0        0        0     3255 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/cli/main.py
--rw-r--r--   0        0        0     3365 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/cli/orgs.py
--rw-r--r--   0        0        0      451 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/cli/public.pem
--rw-r--r--   0        0        0     1697 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/cli/puremlconfig.py
--rw-r--r--   0        0        0     7182 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/cli/secrets.py
--rw-r--r--   0        0        0     2754 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/components/__init__.py
--rw-r--r--   0        0        0     1829 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/components/auth.py
--rw-r--r--   0        0        0    15074 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/components/dataset.py
--rw-r--r--   0        0        0       88 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/components/log/__init__.py
--rw-r--r--   0        0        0     6866 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/components/log/arrays.py
--rw-r--r--   0        0        0     6634 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/components/log/artifacts.py
--rw-r--r--   0        0        0     6708 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/components/log/audio.py
--rw-r--r--   0        0        0     9603 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/components/log/figure.py
--rw-r--r--   0        0        0     6679 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/components/log/image.py
--rw-r--r--   0        0        0     2041 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/components/log/log.py
--rw-r--r--   0        0        0     5929 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/components/log/metrics.py
--rw-r--r--   0        0        0     5925 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/components/log/params.py
--rw-r--r--   0        0        0     6166 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/components/log/pip_requirement.py
--rw-r--r--   0        0        0     6181 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/components/log/predict.py
--rw-r--r--   0        0        0     6049 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/components/log/resources.py
--rw-r--r--   0        0        0     6776 2023-05-21 10:58:34.529091 pureml-0.4.0/pureml/components/log/tabular.py
--rw-r--r--   0        0        0     6168 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/components/log/video.py
--rw-r--r--   0        0        0    13508 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/components/model.py
--rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/config/__init__.py
--rw-r--r--   0        0        0     3753 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/config/parser.py
--rw-r--r--   0        0        0      123 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/decorators/__init__.py
--rw-r--r--   0        0        0     2219 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/decorators/dataset.py
--rw-r--r--   0        0        0      856 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/decorators/load_data.py
--rw-r--r--   0        0        0     2720 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/decorators/model.py
--rw-r--r--   0        0        0      607 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/decorators/pip_requirements.py
--rw-r--r--   0        0        0      838 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/decorators/predict.py
--rw-r--r--   0        0        0      895 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/decorators/transformer.py
--rw-r--r--   0        0        0       73 2023-07-10 21:08:37.716024 pureml-0.4.0/pureml/evaluate/__init__.py
--rw-r--r--   0        0        0     1489 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/evaluate/classification.py
--rw-r--r--   0        0        0     5574 2023-07-13 09:52:21.777305 pureml-0.4.0/pureml/evaluate/eval.py
--rw-r--r--   0        0        0     2150 2023-07-10 21:08:37.716024 pureml-0.4.0/pureml/evaluate/eval_old.py
--rw-r--r--   0        0        0     1665 2023-06-14 19:32:31.884622 pureml-0.4.0/pureml/evaluate/grade.py
--rw-r--r--   0        0        0      227 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/evaluate/metrics/__init__.py
--rw-r--r--   0        0        0      633 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/evaluate/metrics/accuracy.py
--rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/evaluate/metrics/base.py
--rw-r--r--   0        0        0      673 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/evaluate/metrics/confusion_matrix.py
--rw-r--r--   0        0        0      699 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/evaluate/metrics/f1.py
--rw-r--r--   0        0        0      629 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/evaluate/metrics/mae.py
--rw-r--r--   0        0        0      686 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/evaluate/metrics/mse.py
--rw-r--r--   0        0        0      802 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/evaluate/metrics/precision.py
--rw-r--r--   0        0        0      787 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/evaluate/metrics/recall.py
--rw-r--r--   0        0        0     1225 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/evaluate/metrics/roc_auc.py
--rw-r--r--   0        0        0      654 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/evaluate/regression.py
--rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/lineage/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/lineage/data/__init__.py
--rw-r--r--   0        0        0     2852 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/lineage/data/create_lineage.py
--rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/package/__init__.py
--rw-r--r--   0        0        0     6446 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/package/docker.py
--rw-r--r--   0        0        0     6192 2023-07-10 21:08:37.728025 pureml-0.4.0/pureml/package/fastapi.py
--rw-r--r--   0        0        0      876 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/packaging/__init__.py
--rw-r--r--   0        0        0      496 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/packaging/errors.py
--rw-r--r--   0        0        0     2245 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/packaging/model_framework.py
--rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/packaging/model_packaging/__init__.py
--rw-r--r--   0        0        0      973 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/packaging/model_packaging/catboost.py
--rw-r--r--   0        0        0     1103 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/packaging/model_packaging/custom.py
--rw-r--r--   0        0        0      965 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/packaging/model_packaging/keras.py
--rw-r--r--   0        0        0      976 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/packaging/model_packaging/lightgbm.py
--rw-r--r--   0        0        0     1075 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/packaging/model_packaging/pytorch.py
--rw-r--r--   0        0        0     1146 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/packaging/model_packaging/pytorch_tabnet.py
--rw-r--r--   0        0        0     2163 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/packaging/model_packaging/sklearn.py
--rw-r--r--   0        0        0     1028 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/packaging/model_packaging/tensorflow.py
--rw-r--r--   0        0        0     1021 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/packaging/model_packaging/xgboost.py
--rw-r--r--   0        0        0     4006 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/packaging/packaging.py
--rw-r--r--   0        0        0     1381 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/packaging/packaging_utils.py
--rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/predictor/__init__.py
--rw-r--r--   0        0        0      778 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/predictor/predictor.py
--rw-r--r--   0        0        0      439 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/schema/__init__.py
--rw-r--r--   0        0        0     2675 2023-07-10 21:08:37.728025 pureml-0.4.0/pureml/schema/backend.py
--rw-r--r--   0        0        0      350 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/schema/config.py
--rw-r--r--   0        0        0      330 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/schema/dataset.py
--rw-r--r--   0        0        0      140 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/schema/env.py
--rw-r--r--   0        0        0      474 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/schema/log.py
--rw-r--r--   0        0        0      396 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/schema/model.py
--rw-r--r--   0        0        0     1007 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/schema/packaging.py
--rw-r--r--   0        0        0     2528 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/schema/paths.py
--rw-r--r--   0        0        0     1222 2023-07-10 21:08:37.728025 pureml-0.4.0/pureml/schema/predict.py
--rw-r--r--   0        0        0      308 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/schema/request.py
--rw-r--r--   0        0        0      385 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/schema/singleton.py
--rw-r--r--   0        0        0      243 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/schema/storage.py
--rw-r--r--   0        0        0      177 2023-05-21 10:58:34.533091 pureml-0.4.0/pureml/schema/types.py
--rw-r--r--   0        0        0       66 2023-05-21 10:58:34.537091 pureml-0.4.0/pureml/settings/__init__.py
--rw-r--r--   0        0        0      278 2023-05-21 10:58:34.537091 pureml-0.4.0/pureml/settings/backend.py
--rw-r--r--   0        0        0      376 2023-05-21 10:58:34.537091 pureml-0.4.0/pureml/settings/storage.py
--rw-r--r--   0        0        0        0 2023-05-21 10:58:34.537091 pureml-0.4.0/pureml/utils/__init__.py
--rw-r--r--   0        0        0     1751 2023-05-21 10:58:34.537091 pureml-0.4.0/pureml/utils/config.py
--rw-r--r--   0        0        0     2234 2023-05-21 10:58:34.537091 pureml-0.4.0/pureml/utils/constants.py
--rw-r--r--   0        0        0     1044 2023-05-21 10:58:34.537091 pureml-0.4.0/pureml/utils/env.py
--rw-r--r--   0        0        0     2942 2023-05-21 10:58:34.537091 pureml-0.4.0/pureml/utils/hash.py
--rw-r--r--   0        0        0      522 2023-05-21 10:58:34.537091 pureml-0.4.0/pureml/utils/log_utils.py
--rw-r--r--   0        0        0     1985 2023-05-21 10:58:34.537091 pureml-0.4.0/pureml/utils/package.py
--rw-r--r--   0        0        0    14445 2023-05-21 10:58:34.537091 pureml-0.4.0/pureml/utils/pipeline.py
--rw-r--r--   0        0        0     2868 2023-05-21 10:58:34.537091 pureml-0.4.0/pureml/utils/predict.py
--rw-r--r--   0        0        0      816 2023-05-21 10:58:34.537091 pureml-0.4.0/pureml/utils/readme.py
--rw-r--r--   0        0        0     1643 2023-05-21 10:58:34.537091 pureml-0.4.0/pureml/utils/resources.py
--rw-r--r--   0        0        0      137 2023-05-21 10:58:34.537091 pureml-0.4.0/pureml/utils/source_code.py
--rw-r--r--   0        0        0        0 2023-05-21 10:58:34.537091 pureml-0.4.0/pureml/utils/types.py
--rw-r--r--   0        0        0      698 2023-05-21 10:58:34.537091 pureml-0.4.0/pureml/utils/version_utils.py
--rw-r--r--   0        0        0     1954 2023-07-13 09:52:21.777305 pureml-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     8659 1970-01-01 00:00:00.000000 pureml-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     6690 2023-05-21 10:58:34.529091 pureml-0.4.1/README.md
+-rw-r--r--   0        0        0      735 2023-07-13 10:44:46.013588 pureml-0.4.1/pureml/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/cli/__init__.py
+-rw-r--r--   0        0        0     9766 2023-07-10 21:08:37.716024 pureml-0.4.1/pureml/cli/auth.py
+-rw-r--r--   0        0        0     2285 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/cli/helpers.py
+-rw-r--r--   0        0        0     3255 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/cli/main.py
+-rw-r--r--   0        0        0     3365 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/cli/orgs.py
+-rw-r--r--   0        0        0      451 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/cli/public.pem
+-rw-r--r--   0        0        0     1697 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/cli/puremlconfig.py
+-rw-r--r--   0        0        0     7182 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/cli/secrets.py
+-rw-r--r--   0        0        0     2754 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/components/__init__.py
+-rw-r--r--   0        0        0     1829 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/components/auth.py
+-rw-r--r--   0        0        0    15074 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/components/dataset.py
+-rw-r--r--   0        0        0       88 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/components/log/__init__.py
+-rw-r--r--   0        0        0     6866 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/components/log/arrays.py
+-rw-r--r--   0        0        0     6634 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/components/log/artifacts.py
+-rw-r--r--   0        0        0     6708 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/components/log/audio.py
+-rw-r--r--   0        0        0     9603 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/components/log/figure.py
+-rw-r--r--   0        0        0     6679 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/components/log/image.py
+-rw-r--r--   0        0        0     2041 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/components/log/log.py
+-rw-r--r--   0        0        0     5929 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/components/log/metrics.py
+-rw-r--r--   0        0        0     5925 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/components/log/params.py
+-rw-r--r--   0        0        0     6166 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/components/log/pip_requirement.py
+-rw-r--r--   0        0        0     6181 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/components/log/predict.py
+-rw-r--r--   0        0        0     6049 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/components/log/resources.py
+-rw-r--r--   0        0        0     6776 2023-05-21 10:58:34.529091 pureml-0.4.1/pureml/components/log/tabular.py
+-rw-r--r--   0        0        0     6168 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/components/log/video.py
+-rw-r--r--   0        0        0    13508 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/components/model.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/config/__init__.py
+-rw-r--r--   0        0        0     3753 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/config/parser.py
+-rw-r--r--   0        0        0      123 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/decorators/__init__.py
+-rw-r--r--   0        0        0     2219 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/decorators/dataset.py
+-rw-r--r--   0        0        0      856 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/decorators/load_data.py
+-rw-r--r--   0        0        0     2720 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/decorators/model.py
+-rw-r--r--   0        0        0      607 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/decorators/pip_requirements.py
+-rw-r--r--   0        0        0      838 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/decorators/predict.py
+-rw-r--r--   0        0        0      895 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/decorators/transformer.py
+-rw-r--r--   0        0        0       73 2023-07-10 21:08:37.716024 pureml-0.4.1/pureml/evaluate/__init__.py
+-rw-r--r--   0        0        0     1489 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/evaluate/classification.py
+-rw-r--r--   0        0        0     5577 2023-07-13 10:44:50.920731 pureml-0.4.1/pureml/evaluate/eval.py
+-rw-r--r--   0        0        0     2150 2023-07-10 21:08:37.716024 pureml-0.4.1/pureml/evaluate/eval_old.py
+-rw-r--r--   0        0        0     1665 2023-06-14 19:32:31.884622 pureml-0.4.1/pureml/evaluate/grade.py
+-rw-r--r--   0        0        0      227 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/evaluate/metrics/__init__.py
+-rw-r--r--   0        0        0      633 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/evaluate/metrics/accuracy.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/evaluate/metrics/base.py
+-rw-r--r--   0        0        0      673 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/evaluate/metrics/confusion_matrix.py
+-rw-r--r--   0        0        0      699 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/evaluate/metrics/f1.py
+-rw-r--r--   0        0        0      629 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/evaluate/metrics/mae.py
+-rw-r--r--   0        0        0      686 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/evaluate/metrics/mse.py
+-rw-r--r--   0        0        0      802 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/evaluate/metrics/precision.py
+-rw-r--r--   0        0        0      787 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/evaluate/metrics/recall.py
+-rw-r--r--   0        0        0     1225 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/evaluate/metrics/roc_auc.py
+-rw-r--r--   0        0        0      654 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/evaluate/regression.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/lineage/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/lineage/data/__init__.py
+-rw-r--r--   0        0        0     2852 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/lineage/data/create_lineage.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/package/__init__.py
+-rw-r--r--   0        0        0     6446 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/package/docker.py
+-rw-r--r--   0        0        0     6192 2023-07-10 21:08:37.728025 pureml-0.4.1/pureml/package/fastapi.py
+-rw-r--r--   0        0        0      876 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/packaging/__init__.py
+-rw-r--r--   0        0        0      496 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/packaging/errors.py
+-rw-r--r--   0        0        0     2245 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/packaging/model_framework.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/packaging/model_packaging/__init__.py
+-rw-r--r--   0        0        0      973 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/packaging/model_packaging/catboost.py
+-rw-r--r--   0        0        0     1103 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/packaging/model_packaging/custom.py
+-rw-r--r--   0        0        0      965 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/packaging/model_packaging/keras.py
+-rw-r--r--   0        0        0      976 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/packaging/model_packaging/lightgbm.py
+-rw-r--r--   0        0        0     1075 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/packaging/model_packaging/pytorch.py
+-rw-r--r--   0        0        0     1146 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/packaging/model_packaging/pytorch_tabnet.py
+-rw-r--r--   0        0        0     2163 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/packaging/model_packaging/sklearn.py
+-rw-r--r--   0        0        0     1028 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/packaging/model_packaging/tensorflow.py
+-rw-r--r--   0        0        0     1021 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/packaging/model_packaging/xgboost.py
+-rw-r--r--   0        0        0     4006 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/packaging/packaging.py
+-rw-r--r--   0        0        0     1381 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/packaging/packaging_utils.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/predictor/__init__.py
+-rw-r--r--   0        0        0      778 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/predictor/predictor.py
+-rw-r--r--   0        0        0      439 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/schema/__init__.py
+-rw-r--r--   0        0        0     2675 2023-07-10 21:08:37.728025 pureml-0.4.1/pureml/schema/backend.py
+-rw-r--r--   0        0        0      350 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/schema/config.py
+-rw-r--r--   0        0        0      330 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/schema/dataset.py
+-rw-r--r--   0        0        0      140 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/schema/env.py
+-rw-r--r--   0        0        0      474 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/schema/log.py
+-rw-r--r--   0        0        0      396 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/schema/model.py
+-rw-r--r--   0        0        0     1007 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/schema/packaging.py
+-rw-r--r--   0        0        0     2528 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/schema/paths.py
+-rw-r--r--   0        0        0     1222 2023-07-10 21:08:37.728025 pureml-0.4.1/pureml/schema/predict.py
+-rw-r--r--   0        0        0      308 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/schema/request.py
+-rw-r--r--   0        0        0      385 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/schema/singleton.py
+-rw-r--r--   0        0        0      243 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/schema/storage.py
+-rw-r--r--   0        0        0      177 2023-05-21 10:58:34.533091 pureml-0.4.1/pureml/schema/types.py
+-rw-r--r--   0        0        0       66 2023-05-21 10:58:34.537091 pureml-0.4.1/pureml/settings/__init__.py
+-rw-r--r--   0        0        0      278 2023-05-21 10:58:34.537091 pureml-0.4.1/pureml/settings/backend.py
+-rw-r--r--   0        0        0      376 2023-05-21 10:58:34.537091 pureml-0.4.1/pureml/settings/storage.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:58:34.537091 pureml-0.4.1/pureml/utils/__init__.py
+-rw-r--r--   0        0        0     1751 2023-05-21 10:58:34.537091 pureml-0.4.1/pureml/utils/config.py
+-rw-r--r--   0        0        0     2234 2023-05-21 10:58:34.537091 pureml-0.4.1/pureml/utils/constants.py
+-rw-r--r--   0        0        0     1044 2023-05-21 10:58:34.537091 pureml-0.4.1/pureml/utils/env.py
+-rw-r--r--   0        0        0     2942 2023-05-21 10:58:34.537091 pureml-0.4.1/pureml/utils/hash.py
+-rw-r--r--   0        0        0      522 2023-05-21 10:58:34.537091 pureml-0.4.1/pureml/utils/log_utils.py
+-rw-r--r--   0        0        0     1985 2023-05-21 10:58:34.537091 pureml-0.4.1/pureml/utils/package.py
+-rw-r--r--   0        0        0    14445 2023-05-21 10:58:34.537091 pureml-0.4.1/pureml/utils/pipeline.py
+-rw-r--r--   0        0        0     2868 2023-05-21 10:58:34.537091 pureml-0.4.1/pureml/utils/predict.py
+-rw-r--r--   0        0        0      816 2023-05-21 10:58:34.537091 pureml-0.4.1/pureml/utils/readme.py
+-rw-r--r--   0        0        0     1643 2023-05-21 10:58:34.537091 pureml-0.4.1/pureml/utils/resources.py
+-rw-r--r--   0        0        0      137 2023-05-21 10:58:34.537091 pureml-0.4.1/pureml/utils/source_code.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:58:34.537091 pureml-0.4.1/pureml/utils/types.py
+-rw-r--r--   0        0        0      698 2023-05-21 10:58:34.537091 pureml-0.4.1/pureml/utils/version_utils.py
+-rw-r--r--   0        0        0     1954 2023-07-13 10:44:34.131598 pureml-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     8659 1970-01-01 00:00:00.000000 pureml-0.4.1/PKG-INFO
```

### Comparing `pureml-0.4.0/README.md` & `pureml-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/__init__.py` & `pureml-0.4.1/pureml/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 
 from .package import docker, fastapi
 
 from .schema import Input, Output
 from .predictor.predictor import BasePredictor
 
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
```

### Comparing `pureml-0.4.0/pureml/cli/auth.py` & `pureml-0.4.1/pureml/cli/auth.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/cli/helpers.py` & `pureml-0.4.1/pureml/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/cli/main.py` & `pureml-0.4.1/pureml/cli/main.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/cli/orgs.py` & `pureml-0.4.1/pureml/cli/orgs.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/cli/puremlconfig.py` & `pureml-0.4.1/pureml/cli/puremlconfig.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/cli/secrets.py` & `pureml-0.4.1/pureml/cli/secrets.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/components/__init__.py` & `pureml-0.4.1/pureml/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/components/auth.py` & `pureml-0.4.1/pureml/components/auth.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/components/dataset.py` & `pureml-0.4.1/pureml/components/dataset.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/components/log/arrays.py` & `pureml-0.4.1/pureml/components/log/arrays.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/components/log/artifacts.py` & `pureml-0.4.1/pureml/components/log/artifacts.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/components/log/audio.py` & `pureml-0.4.1/pureml/components/log/audio.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/components/log/figure.py` & `pureml-0.4.1/pureml/components/log/figure.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/components/log/image.py` & `pureml-0.4.1/pureml/components/log/image.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/components/log/log.py` & `pureml-0.4.1/pureml/components/log/log.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/components/log/metrics.py` & `pureml-0.4.1/pureml/components/log/metrics.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/components/log/params.py` & `pureml-0.4.1/pureml/components/log/params.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/components/log/pip_requirement.py` & `pureml-0.4.1/pureml/components/log/pip_requirement.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/components/log/predict.py` & `pureml-0.4.1/pureml/components/log/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/components/log/resources.py` & `pureml-0.4.1/pureml/components/log/resources.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/components/log/tabular.py` & `pureml-0.4.1/pureml/components/log/tabular.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/components/log/video.py` & `pureml-0.4.1/pureml/components/log/video.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/components/model.py` & `pureml-0.4.1/pureml/components/model.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/config/parser.py` & `pureml-0.4.1/pureml/config/parser.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/decorators/dataset.py` & `pureml-0.4.1/pureml/decorators/dataset.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/decorators/load_data.py` & `pureml-0.4.1/pureml/decorators/load_data.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/decorators/model.py` & `pureml-0.4.1/pureml/decorators/model.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/decorators/pip_requirements.py` & `pureml-0.4.1/pureml/decorators/pip_requirements.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/decorators/predict.py` & `pureml-0.4.1/pureml/decorators/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/decorators/transformer.py` & `pureml-0.4.1/pureml/decorators/transformer.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/evaluate/classification.py` & `pureml-0.4.1/pureml/evaluate/classification.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/evaluate/eval.py` & `pureml-0.4.1/pureml/evaluate/eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,16 +131,16 @@
         task_type=None, label_dataset=label_dataset, label_model=label_model
     )
 
     evaluator.load()
 
     y_pred = evaluator.get_y_pred()
     y_true = evaluator.get_y_true()
-    sensitive_features = evaluator.get_sensitive_features
-    #sensitive_features=None
+    sensitive_features = evaluator.get_sensitive_features()
+    # sensitive_features=None
 
 
     values = eval_fn(y_true=y_true,y_pred=y_pred,sensitive_features=sensitive_features,
                      evaluators = task_type,y_pred_scores=None,path_to_config=path_to_config,as_pdf=True,pdf_file_name=pdf_file_name)
     print()
     evaluator.post(values)
```

### Comparing `pureml-0.4.0/pureml/evaluate/eval_old.py` & `pureml-0.4.1/pureml/evaluate/eval_old.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/evaluate/grade.py` & `pureml-0.4.1/pureml/evaluate/grade.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/evaluate/metrics/accuracy.py` & `pureml-0.4.1/pureml/evaluate/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/evaluate/metrics/confusion_matrix.py` & `pureml-0.4.1/pureml/evaluate/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/evaluate/metrics/f1.py` & `pureml-0.4.1/pureml/evaluate/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/evaluate/metrics/mae.py` & `pureml-0.4.1/pureml/evaluate/metrics/mae.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/evaluate/metrics/mse.py` & `pureml-0.4.1/pureml/evaluate/metrics/mse.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/evaluate/metrics/precision.py` & `pureml-0.4.1/pureml/evaluate/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/evaluate/metrics/recall.py` & `pureml-0.4.1/pureml/evaluate/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/evaluate/metrics/roc_auc.py` & `pureml-0.4.1/pureml/evaluate/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/evaluate/regression.py` & `pureml-0.4.1/pureml/evaluate/regression.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/lineage/data/create_lineage.py` & `pureml-0.4.1/pureml/lineage/data/create_lineage.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/package/docker.py` & `pureml-0.4.1/pureml/package/docker.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/package/fastapi.py` & `pureml-0.4.1/pureml/package/fastapi.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/packaging/__init__.py` & `pureml-0.4.1/pureml/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/packaging/model_framework.py` & `pureml-0.4.1/pureml/packaging/model_framework.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/packaging/model_packaging/catboost.py` & `pureml-0.4.1/pureml/packaging/model_packaging/catboost.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/packaging/model_packaging/custom.py` & `pureml-0.4.1/pureml/packaging/model_packaging/custom.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/packaging/model_packaging/keras.py` & `pureml-0.4.1/pureml/packaging/model_packaging/keras.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/packaging/model_packaging/lightgbm.py` & `pureml-0.4.1/pureml/packaging/model_packaging/lightgbm.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/packaging/model_packaging/pytorch.py` & `pureml-0.4.1/pureml/packaging/model_packaging/pytorch.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/packaging/model_packaging/pytorch_tabnet.py` & `pureml-0.4.1/pureml/packaging/model_packaging/pytorch_tabnet.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/packaging/model_packaging/sklearn.py` & `pureml-0.4.1/pureml/packaging/model_packaging/sklearn.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/packaging/model_packaging/tensorflow.py` & `pureml-0.4.1/pureml/packaging/model_packaging/tensorflow.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/packaging/model_packaging/xgboost.py` & `pureml-0.4.1/pureml/packaging/model_packaging/xgboost.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/packaging/packaging.py` & `pureml-0.4.1/pureml/packaging/packaging.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/packaging/packaging_utils.py` & `pureml-0.4.1/pureml/packaging/packaging_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/predictor/predictor.py` & `pureml-0.4.1/pureml/predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/schema/backend.py` & `pureml-0.4.1/pureml/schema/backend.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/schema/packaging.py` & `pureml-0.4.1/pureml/schema/packaging.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/schema/paths.py` & `pureml-0.4.1/pureml/schema/paths.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/schema/predict.py` & `pureml-0.4.1/pureml/schema/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/utils/config.py` & `pureml-0.4.1/pureml/utils/config.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/utils/constants.py` & `pureml-0.4.1/pureml/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/utils/env.py` & `pureml-0.4.1/pureml/utils/env.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/utils/hash.py` & `pureml-0.4.1/pureml/utils/hash.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/utils/log_utils.py` & `pureml-0.4.1/pureml/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/utils/package.py` & `pureml-0.4.1/pureml/utils/package.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/utils/pipeline.py` & `pureml-0.4.1/pureml/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/utils/predict.py` & `pureml-0.4.1/pureml/utils/predict.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/utils/readme.py` & `pureml-0.4.1/pureml/utils/readme.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/utils/resources.py` & `pureml-0.4.1/pureml/utils/resources.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pureml/utils/version_utils.py` & `pureml-0.4.1/pureml/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `pureml-0.4.0/pyproject.toml` & `pureml-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pureml"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 license = "Apache-2.0"
 authors = ["vamsidhar muthireddy <vamsi.muthireddy@gmail.com>"]
 readme = "README.md"
 homepage = "https://pureml.com/"
 repository = "https://github.com/engageml-github/Pure"
 documentation = "https://docs.pureml.com"
```

### Comparing `pureml-0.4.0/PKG-INFO` & `pureml-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pureml
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Home-page: https://pureml.com/
 License: Apache-2.0
 Keywords: pureml,model-store,machine-learning,python,model-registry,collabortion
 Author: vamsidhar muthireddy
 Author-email: vamsi.muthireddy@gmail.com
 Requires-Python: >=3.8,<4.0
```

