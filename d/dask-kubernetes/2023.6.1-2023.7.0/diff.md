# Comparing `tmp/dask-kubernetes-2023.6.1.tar.gz` & `tmp/dask-kubernetes-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-kubernetes-2023.6.1.tar", last modified: Thu Jun 29 09:24:10 2023, max compression
+gzip compressed data, was "dask-kubernetes-2023.7.0.tar", last modified: Thu Jul 13 09:24:03 2023, max compression
```

## Comparing `dask-kubernetes-2023.6.1.tar` & `dask-kubernetes-2023.7.0.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.501344 dask-kubernetes-2023.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-29 09:24:10.501344 dask-kubernetes-2023.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.505344 dask-kubernetes-2023.6.1/dask_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-29 09:24:10.505344 dask-kubernetes-2023.6.1/dask_kubernetes/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.493343 dask-kubernetes-2023.6.1/dask_kubernetes/aiopykube/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/aiopykube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/aiopykube/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/aiopykube/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/aiopykube/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/aiopykube/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.493343 dask-kubernetes-2023.6.1/dask_kubernetes/aiopykube/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/aiopykube/tests/test_pykube_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/aiopykube/tests/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.493343 dask-kubernetes-2023.6.1/dask_kubernetes/classic/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/classic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28558 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/classic/kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.497343 dask-kubernetes-2023.6.1/dask_kubernetes/classic/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/classic/tests/config-demo.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/classic/tests/fake_gcp_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    28838 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/classic/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/classic/tests/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.497343 dask-kubernetes-2023.6.1/dask_kubernetes/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.497343 dask-kubernetes-2023.6.1/dask_kubernetes/common/
--rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/common/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/common/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/common/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.497343 dask-kubernetes-2023.6.1/dask_kubernetes/common/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/common/tests/test_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/common/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.497343 dask-kubernetes-2023.6.1/dask_kubernetes/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.497343 dask-kubernetes-2023.6.1/dask_kubernetes/helm/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/helm/helmcluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.497343 dask-kubernetes-2023.6.1/dask_kubernetes/helm/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.497343 dask-kubernetes-2023.6.1/dask_kubernetes/helm/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/helm/tests/resources/values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/helm/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/kubernetes.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.497343 dask-kubernetes-2023.6.1/dask_kubernetes/operator/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.497343 dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37016 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.497343 dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.497343 dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/plugins/noop/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/plugins/noop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/plugins/noop/noop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.497343 dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.497343 dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    24649 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/tests/test_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.497343 dask-kubernetes-2023.6.1/dask_kubernetes/operator/customresources/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/customresources/daskautoscaler.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/customresources/daskautoscaler.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/customresources/daskcluster.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/customresources/daskcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/customresources/daskjob.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/customresources/daskjob.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/customresources/daskworkergroup.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/customresources/daskworkergroup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/customresources/templates.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.493343 dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.501344 dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/chartpress.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.501344 dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.501344 dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   283847 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   471240 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   140704 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.501344 dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/rolebinding.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/serviceaccount.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.501344 dask-kubernetes-2023.6.1/dask_kubernetes/operator/kubecluster/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/kubecluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/kubecluster/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    42764 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/kubecluster/kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.501344 dask-kubernetes-2023.6.1/dask_kubernetes/operator/kubecluster/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/kubecluster/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/kubecluster/tests/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:10.493343 dask-kubernetes-2023.6.1/dask_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-29 09:24:10.000000 dask-kubernetes-2023.6.1/dask_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-29 09:24:10.000000 dask-kubernetes-2023.6.1/dask_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 09:24:10.000000 dask-kubernetes-2023.6.1/dask_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-29 09:24:10.000000 dask-kubernetes-2023.6.1/dask_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 09:24:10.000000 dask-kubernetes-2023.6.1/dask_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-29 09:24:10.000000 dask-kubernetes-2023.6.1/dask_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 09:24:10.000000 dask-kubernetes-2023.6.1/dask_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-29 09:24:10.505344 dask-kubernetes-2023.6.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1032 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68747 2023-06-29 09:23:58.000000 dask-kubernetes-2023.6.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.134774 dask-kubernetes-2023.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-13 09:24:03.134774 dask-kubernetes-2023.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.134774 dask-kubernetes-2023.7.0/dask_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-13 09:24:03.134774 dask-kubernetes-2023.7.0/dask_kubernetes/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.122774 dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.122774 dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/tests/test_pykube_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/tests/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/classic/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/classic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28558 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/classic/kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/classic/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/classic/tests/config-demo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/classic/tests/fake_gcp_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28838 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/classic/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/classic/tests/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/common/
+-rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/common/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/common/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/common/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/common/tests/test_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/common/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/helm/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/helm/helmcluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/helm/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/helm/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/helm/tests/resources/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/helm/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/kubernetes.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33066 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/plugins/noop/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/plugins/noop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/plugins/noop/noop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    26316 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/test_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.130774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskautoscaler.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskautoscaler.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskcluster.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskcluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskjob.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskworkergroup.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskworkergroup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/templates.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.122774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.130774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/chartpress.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.130774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.130774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   283847 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   471240 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   140704 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.130774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/rolebinding.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/serviceaccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.130774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42764 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.134774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/tests/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.122774 dask-kubernetes-2023.7.0/dask_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-13 09:24:03.000000 dask-kubernetes-2023.7.0/dask_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-13 09:24:03.000000 dask-kubernetes-2023.7.0/dask_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:24:03.000000 dask-kubernetes-2023.7.0/dask_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-13 09:24:03.000000 dask-kubernetes-2023.7.0/dask_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:24:03.000000 dask-kubernetes-2023.7.0/dask_kubernetes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-13 09:24:03.000000 dask-kubernetes-2023.7.0/dask_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 09:24:03.000000 dask-kubernetes-2023.7.0/dask_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-13 09:24:03.134774 dask-kubernetes-2023.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1032 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68747 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/versioneer.py
```

### Comparing `dask-kubernetes-2023.6.1/LICENSE` & `dask-kubernetes-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/PKG-INFO` & `dask-kubernetes-2023.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-kubernetes
-Version: 2023.6.1
+Version: 2023.7.0
 Summary: Native Kubernetes integration for Dask
 Home-page: https://github.com/dask/dask-kubernetes
 Maintainer: Jacob Tomlinson
 License: BSD
 Keywords: dask,kubernetes,distributed
 Requires-Python: >=3.9
 License-File: LICENSE
```

### Comparing `dask-kubernetes-2023.6.1/README.rst` & `dask-kubernetes-2023.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/__init__.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/aiopykube/dask.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/dask.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/aiopykube/mixins.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/mixins.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/aiopykube/objects.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/aiopykube/query.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/query.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/aiopykube/tests/test_pykube_objects.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/tests/test_pykube_objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/aiopykube/tests/test_query.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/classic/kubecluster.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/classic/kubecluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/classic/tests/config-demo.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/classic/tests/config-demo.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/classic/tests/test_async.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/classic/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/classic/tests/test_sync.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/classic/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/cli/cli.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/cli/cli.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/common/auth.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/common/auth.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/common/networking.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/common/networking.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/common/objects.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/common/objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/common/tests/test_kind.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/common/tests/test_kind.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/common/tests/test_objects.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/common/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/common/utils.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/common/utils.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/conftest.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/conftest.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/experimental/__init__.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/helm/helmcluster.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/helm/helmcluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/helm/tests/test_helm.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/helm/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/kubernetes.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/kubernetes.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,20 @@
   port: 0
   idle-timeout: null
   deploy-mode: "remote"
   interface: null
   protocol: "tcp://"
   dashboard_address: ":8787"
 
+  # Dask Operator Controller options
+  controller:
+    worker-allocation:
+      batch-size: null
+      delay: null
+
   # Timeout to wait for the scheduler service to be up (in seconds)
   # Set it to 0 to wait indefinitely (not recommended)
   scheduler-service-wait-timeout: 30
   # Number of retries to resolve scheduler service name when running
   # from within the Kubernetes cluster.
   # Must be set to 1 or greater.
   scheduler-service-name-resolution-retries: 20
```

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/_objects.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     version = "kubernetes.dask.org/v1"
     endpoint = "daskworkergroups"
     kind = "DaskWorkerGroup"
     plural = "daskworkergroups"
     singular = "daskworkergroup"
     namespaced = True
     scalable = True
+    scalable_spec = "worker.replicas"
 
     async def pods(self) -> List[Pod]:
         return await self.api.get(
             Pod.endpoint,
             label_selector=",".join(
                 [
                     f"dask.org/cluster-name={self.spec['cluster']}",
```

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/controller.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,30 @@
 import time
 from contextlib import suppress
 from datetime import datetime
 from uuid import uuid4
 
 import aiohttp
 import kopf
+from kr8s.asyncio.objects import Pod
 import kubernetes_asyncio as kubernetes
 from importlib_metadata import entry_points
 from kubernetes_asyncio.client import ApiException
 
-from dask_kubernetes.operator._objects import DaskCluster
+from dask_kubernetes.operator._objects import (
+    DaskCluster,
+    DaskAutoscaler,
+    DaskWorkerGroup,
+    DaskJob,
+)
 from dask_kubernetes.common.auth import ClusterAuth
 from dask_kubernetes.common.networking import get_scheduler_address
 from distributed.core import rpc, clean_exception
 from distributed.protocol.pickle import dumps
+import dask.config
 
 _ANNOTATION_NAMESPACES_TO_IGNORE = (
     "kopf.zalando.org",
     "kubectl.kubernetes.io",
 )
 _LABEL_NAMESPACES_TO_IGNORE = ()
 
@@ -568,33 +575,19 @@
 
 
 worker_group_scale_locks = defaultdict(lambda: asyncio.Lock())
 
 
 @kopf.on.field("daskcluster.kubernetes.dask.org", field="spec.worker.replicas")
 async def daskcluster_default_worker_group_replica_update(
-    name, namespace, meta, spec, old, new, body, logger, **kwargs
+    name, namespace, old, new, **kwargs
 ):
-    if old is None:
-        return
-    worker_group_name = f"{name}-default"
-
-    async with kubernetes.client.api_client.ApiClient() as api_client:
-        custom_objects_api = kubernetes.client.CustomObjectsApi(api_client)
-        custom_objects_api.api_client.set_default_header(
-            "content-type", "application/merge-patch+json"
-        )
-        await custom_objects_api.patch_namespaced_custom_object_scale(
-            group="kubernetes.dask.org",
-            version="v1",
-            plural="daskworkergroups",
-            namespace=namespace,
-            name=worker_group_name,
-            body={"spec": {"replicas": new}},
-        )
+    if old is not None:
+        wg = await DaskWorkerGroup.get(f"{name}-default", namespace=namespace)
+        await wg.scale(new)
 
 
 @kopf.on.field("daskworkergroup.kubernetes.dask.org", field="spec.worker.replicas")
 async def daskworkergroup_replica_update(
     name, namespace, meta, spec, new, body, logger, **kwargs
 ):
     cluster_name = spec["cluster"]
@@ -636,16 +629,20 @@
             annotations = _get_annotations(meta)
             worker_spec = spec["worker"]
             if "metadata" in worker_spec:
                 if "annotations" in worker_spec["metadata"]:
                     annotations.update(**worker_spec["metadata"]["annotations"])
                 if "labels" in worker_spec["metadata"]:
                     labels.update(**worker_spec["metadata"]["labels"])
+
+            SIZE = dask.config.get("kubernetes.controller.worker-allocation.batch-size")
+            DELAY = dask.config.get("kubernetes.controller.worker-allocation.delay")
+            batch_size = min(workers_needed, SIZE) if SIZE else workers_needed
             if workers_needed > 0:
-                for _ in range(workers_needed):
+                for _ in range(batch_size):
                     data = build_worker_deployment_spec(
                         worker_group_name=name,
                         namespace=namespace,
                         cluster_name=cluster_name,
                         uuid=uuid4().hex[:10],
                         pod_spec=worker_spec["spec"],
                         annotations=annotations,
@@ -655,17 +652,22 @@
                     kopf.label(data, labels=cluster_labels)
                     await kubernetes.client.AppsV1Api(
                         api_client
                     ).create_namespaced_deployment(
                         namespace=namespace,
                         body=data,
                     )
-                logger.info(
-                    f"Scaled worker group {name} up to {desired_workers} workers."
-                )
+            if SIZE:
+                if workers_needed > SIZE:
+                    raise kopf.TemporaryError(
+                        "Added maximum number of workers for this batch but still need to create more workers, "
+                        f"waiting for {DELAY} seconds before continuing.",
+                        delay=DELAY,
+                    )
+            logger.info(f"Scaled worker group {name} up to {desired_workers} workers.")
             if workers_needed < 0:
                 worker_ids = await retire_workers(
                     n_workers=-workers_needed,
                     scheduler_service_name=f"{cluster_name}-scheduler",
                     worker_group_name=name,
                     namespace=namespace,
                     logger=logger,
@@ -765,243 +767,153 @@
     "pod",
     field="status.phase",
     labels={"dask.org/component": "job-runner"},
     new="Running",
 )
 async def handle_runner_status_change_running(meta, namespace, logger, **kwargs):
     logger.info("Job now in running")
-    async with kubernetes.client.api_client.ApiClient() as api_client:
-        customobjectsapi = kubernetes.client.CustomObjectsApi(api_client)
-        api_client.set_default_header("content-type", "application/merge-patch+json")
-        await customobjectsapi.patch_namespaced_custom_object_status(
-            group="kubernetes.dask.org",
-            version="v1",
-            plural="daskjobs",
-            namespace=namespace,
-            name=meta["labels"]["dask.org/cluster-name"],
-            body={
-                "status": {
-                    "jobStatus": "Running",
-                    "startTime": datetime.utcnow().strftime(KUBERNETES_DATETIME_FORMAT),
-                }
-            },
-        )
+    name = meta["labels"]["dask.org/cluster-name"]
+    job = await DaskJob.get(name, namespace=namespace)
+    await job.patch(
+        {
+            "status": {
+                "jobStatus": "Running",
+                "startTime": datetime.utcnow().strftime(KUBERNETES_DATETIME_FORMAT),
+            }
+        },
+        subresource="status",
+    )
 
 
 @kopf.on.field(
     "pod",
     field="status.phase",
     labels={"dask.org/component": "job-runner"},
     new="Succeeded",
 )
 async def handle_runner_status_change_succeeded(meta, namespace, logger, **kwargs):
     logger.info("Job succeeded, deleting Dask cluster.")
-    async with kubernetes.client.api_client.ApiClient() as api_client:
-        customobjectsapi = kubernetes.client.CustomObjectsApi(api_client)
-        await customobjectsapi.delete_namespaced_custom_object(
-            group="kubernetes.dask.org",
-            version="v1",
-            plural="daskclusters",
-            namespace=namespace,
-            name=meta["labels"]["dask.org/cluster-name"],
-        )
-        api_client.set_default_header("content-type", "application/merge-patch+json")
-        await customobjectsapi.patch_namespaced_custom_object_status(
-            group="kubernetes.dask.org",
-            version="v1",
-            plural="daskjobs",
-            namespace=namespace,
-            name=meta["labels"]["dask.org/cluster-name"],
-            body={
-                "status": {
-                    "jobStatus": "Successful",
-                    "endTime": datetime.utcnow().strftime(KUBERNETES_DATETIME_FORMAT),
-                }
-            },
-        )
+    name = meta["labels"]["dask.org/cluster-name"]
+    cluster = await DaskCluster.get(name, namespace=namespace)
+    await cluster.delete()
+    job = await DaskJob.get(name, namespace=namespace)
+    await job.patch(
+        {
+            "status": {
+                "jobStatus": "Successful",
+                "endTime": datetime.utcnow().strftime(KUBERNETES_DATETIME_FORMAT),
+            }
+        },
+        subresource="status",
+    )
 
 
 @kopf.on.field(
     "pod",
     field="status.phase",
     labels={"dask.org/component": "job-runner"},
     new="Failed",
 )
 async def handle_runner_status_change_succeeded(meta, namespace, logger, **kwargs):
     logger.info("Job failed, deleting Dask cluster.")
-    async with kubernetes.client.api_client.ApiClient() as api_client:
-        customobjectsapi = kubernetes.client.CustomObjectsApi(api_client)
-        await customobjectsapi.delete_namespaced_custom_object(
-            group="kubernetes.dask.org",
-            version="v1",
-            plural="daskclusters",
-            namespace=namespace,
-            name=meta["labels"]["dask.org/cluster-name"],
-        )
-        api_client.set_default_header("content-type", "application/merge-patch+json")
-        await customobjectsapi.patch_namespaced_custom_object_status(
-            group="kubernetes.dask.org",
-            version="v1",
-            plural="daskjobs",
-            namespace=namespace,
-            name=meta["labels"]["dask.org/cluster-name"],
-            body={
-                "status": {
-                    "jobStatus": "Failed",
-                    "endTime": datetime.utcnow().strftime(KUBERNETES_DATETIME_FORMAT),
-                }
-            },
-        )
+    name = meta["labels"]["dask.org/cluster-name"]
+    cluster = await DaskCluster.get(name, namespace=namespace)
+    await cluster.delete()
+    job = await DaskJob.get(name, namespace=namespace)
+    await job.patch(
+        {
+            "status": {
+                "jobStatus": "Failed",
+                "endTime": datetime.utcnow().strftime(KUBERNETES_DATETIME_FORMAT),
+            }
+        },
+        subresource="status",
+    )
 
 
 @kopf.on.create("daskautoscaler.kubernetes.dask.org")
-async def daskautoscaler_create(spec, name, namespace, logger, **kwargs):
+async def daskautoscaler_create(name, spec, namespace, logger, patch, **kwargs):
     """When an autoscaler is created make it a child of the associated cluster for cascade deletion."""
-    async with kubernetes.client.api_client.ApiClient() as api_client:
-        api = kubernetes.client.CustomObjectsApi(api_client)
-        cluster = await api.get_namespaced_custom_object(
-            group="kubernetes.dask.org",
-            version="v1",
-            plural="daskclusters",
-            namespace=namespace,
-            name=spec["cluster"],
-        )
-        new_spec = dict(spec)
-        kopf.adopt(new_spec, owner=cluster)
-        api.api_client.set_default_header(
-            "content-type", "application/merge-patch+json"
-        )
-        await api.patch_namespaced_custom_object(
-            group="kubernetes.dask.org",
-            version="v1",
-            plural="daskautoscalers",
-            namespace=namespace,
-            name=name,
-            body=new_spec,
-        )
-        logger.info(f"Successfully adopted by {spec['cluster']}")
+    cluster = await DaskCluster.get(spec["cluster"], namespace=namespace)
+    kopf.adopt(patch, owner=cluster.raw)
+    logger.info(f"Autoscaler {name} successfully adopted by cluster {spec['cluster']}")
 
 
 @kopf.timer("daskautoscaler.kubernetes.dask.org", interval=5.0)
 async def daskautoscaler_adapt(spec, name, namespace, logger, **kwargs):
-    async with kubernetes.client.api_client.ApiClient() as api_client:
-        coreapi = kubernetes.client.CoreV1Api(api_client)
+    try:
+        scheduler = await Pod.get(
+            label_selector={
+                "dask.org/component": "scheduler",
+                "dask.org/cluster-name": spec["cluster"],
+            },
+        )
+        if not await scheduler.ready():
+            raise ValueError()
+    except ValueError:
+        logger.info("Scheduler not ready, skipping autoscaling")
+        return
 
-        pod_ready = False
-        try:
-            pods = await coreapi.list_namespaced_pod(
-                namespace=namespace,
-                label_selector=f"dask.org/component=scheduler,dask.org/cluster-name={spec['cluster']}",
-            )
-            scheduler_pod = await coreapi.read_namespaced_pod(
-                pods.items[0].metadata.name, namespace
-            )
-            if scheduler_pod.status.phase == "Running":
-                pod_ready = True
-        except ApiException as e:
-            if e.status != 404:
-                raise e
-
-        if not pod_ready:
-            logger.info("Scheduler not ready, skipping autoscaling")
-            return
+    autoscaler = await DaskAutoscaler.get(name, namespace=namespace)
+    worker_group = await DaskWorkerGroup.get(
+        f"{spec['cluster']}-default", namespace=namespace
+    )
 
-        customobjectsapi = kubernetes.client.CustomObjectsApi(api_client)
-        customobjectsapi.api_client.set_default_header(
-            "content-type", "application/merge-patch+json"
+    current_replicas = worker_group.replicas
+    cooldown_until = float(
+        autoscaler.annotations.get(
+            DASK_AUTOSCALER_COOLDOWN_UNTIL_ANNOTATION, time.time()
         )
+    )
 
-        autoscaler_resource = await customobjectsapi.get_namespaced_custom_object(
-            group="kubernetes.dask.org",
-            version="v1",
-            plural="daskautoscalers",
-            namespace=namespace,
-            name=name,
-        )
+    # Cooldown autoscaling to prevent thrashing
+    if time.time() < cooldown_until:
+        logger.debug("Autoscaler for %s is in cooldown", spec["cluster"])
+        return
 
-        worker_group_resource = await customobjectsapi.get_namespaced_custom_object(
-            group="kubernetes.dask.org",
-            version="v1",
-            plural="daskworkergroups",
+    # Ask the scheduler for the desired number of worker
+    try:
+        desired_workers = await get_desired_workers(
+            scheduler_service_name=f"{spec['cluster']}-scheduler",
             namespace=namespace,
-            name=f"{spec['cluster']}-default",
-        )
-
-        current_replicas = int(worker_group_resource["spec"]["worker"]["replicas"])
-        cooldown_until = float(
-            autoscaler_resource.get("metadata", {})
-            .get("annotations", {})
-            .get(DASK_AUTOSCALER_COOLDOWN_UNTIL_ANNOTATION, time.time())
+            logger=logger,
         )
+    except SchedulerCommError:
+        logger.error("Unable to get desired number of workers from scheduler.")
+        return
 
-        # Cooldown autoscaling to prevent thrashing
-        if time.time() < cooldown_until:
-            logger.debug("Autoscaler for %s is in cooldown", spec["cluster"])
-            return
+    # Ensure the desired number is within the min and max
+    desired_workers = max(spec["minimum"], desired_workers)
+    desired_workers = min(spec["maximum"], desired_workers)
+
+    if current_replicas > 0:
+        max_scale_down = int(current_replicas * 0.25)
+        max_scale_down = 1 if max_scale_down == 0 else max_scale_down
+        desired_workers = max(current_replicas - max_scale_down, desired_workers)
+
+    # Update the default DaskWorkerGroup
+    if desired_workers != current_replicas:
+        await worker_group.scale(desired_workers)
 
-        # Ask the scheduler for the desired number of worker
-        try:
-            desired_workers = await get_desired_workers(
-                scheduler_service_name=f"{spec['cluster']}-scheduler",
-                namespace=namespace,
-                logger=logger,
-            )
-        except SchedulerCommError:
-            logger.error("Unable to get desired number of workers from scheduler.")
-            return
-
-        # Ensure the desired number is within the min and max
-        desired_workers = max(spec["minimum"], desired_workers)
-        desired_workers = min(spec["maximum"], desired_workers)
-
-        if current_replicas > 0:
-            max_scale_down = int(current_replicas * 0.25)
-            max_scale_down = 1 if max_scale_down == 0 else max_scale_down
-            desired_workers = max(current_replicas - max_scale_down, desired_workers)
-
-        # Update the default DaskWorkerGroup
-        if desired_workers != current_replicas:
-            await customobjectsapi.patch_namespaced_custom_object_scale(
-                group="kubernetes.dask.org",
-                version="v1",
-                plural="daskworkergroups",
-                namespace=namespace,
-                name=f"{spec['cluster']}-default",
-                body={"spec": {"replicas": desired_workers}},
-            )
+        cooldown_until = time.time() + 15
 
-            cooldown_until = time.time() + 15
-
-            await customobjectsapi.patch_namespaced_custom_object(
-                group="kubernetes.dask.org",
-                version="v1",
-                plural="daskautoscalers",
-                namespace=namespace,
-                name=name,
-                body={
-                    "metadata": {
-                        "annotations": {
-                            DASK_AUTOSCALER_COOLDOWN_UNTIL_ANNOTATION: str(
-                                cooldown_until
-                            )
-                        }
-                    }
-                },
-            )
+        await autoscaler.annotate(
+            {DASK_AUTOSCALER_COOLDOWN_UNTIL_ANNOTATION: str(cooldown_until)}
+        )
 
-            logger.info(
-                "Autoscaler updated %s worker count from %d to %d",
-                spec["cluster"],
-                current_replicas,
-                desired_workers,
-            )
-        else:
-            logger.debug(
-                "Not autoscaling %s with %d workers", spec["cluster"], current_replicas
-            )
+        logger.info(
+            "Autoscaler updated %s worker count from %d to %d",
+            spec["cluster"],
+            current_replicas,
+            desired_workers,
+        )
+    else:
+        logger.debug(
+            "Not autoscaling %s with %d workers", spec["cluster"], current_replicas
+        )
 
 
 @kopf.timer("daskcluster.kubernetes.dask.org", interval=5.0)
 async def daskcluster_autoshutdown(spec, name, namespace, logger, **kwargs):
     if spec["idleTimeout"]:
         try:
             idle_since = await check_scheduler_idle(
```

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/controller/tests/test_controller.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/test_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pathlib
 from contextlib import asynccontextmanager
 from datetime import datetime, timedelta
 
 import pytest
 import yaml
 from dask.distributed import Client
+import dask.config
 
 from kr8s.asyncio.objects import Pod, Deployment, Service
 from dask_kubernetes.operator.controller import (
     KUBERNETES_DATETIME_FORMAT,
     get_job_runner_pod_name,
 )
 from dask_kubernetes.operator._objects import DaskCluster, DaskWorkerGroup, DaskJob
@@ -401,14 +402,52 @@
                 await asyncio.sleep(0.1)
             # Wait for worker Pods to be ready
             await asyncio.gather(
                 *[pod.wait(conditions="condition=Ready", timeout=60) for pod in pods]
             )
 
 
+@pytest.mark.asyncio
+async def test_simplecluster_batched_worker_deployments(
+    k8s_cluster, kopf_runner, gen_cluster
+):
+    with kopf_runner as runner:
+        with dask.config.set(
+            {
+                "kubernetes.controller.worker-allocation.batch-size": 1,
+                "kubernetes.controller.worker-allocation.delay": 5,
+            }
+        ):
+            async with gen_cluster() as (cluster_name, ns):
+                scheduler_deployment_name = "simple-scheduler"
+                worker_pod_name = "simple-default-worker"
+                service_name = "simple-scheduler"
+                while scheduler_deployment_name not in k8s_cluster.kubectl(
+                    "get", "deployments", "-n", ns
+                ):
+                    await asyncio.sleep(0.1)
+                while service_name not in k8s_cluster.kubectl("get", "svc", "-n", ns):
+                    await asyncio.sleep(0.1)
+                while worker_pod_name not in k8s_cluster.kubectl(
+                    "get", "pods", "-n", ns
+                ):
+                    await asyncio.sleep(0.1)
+
+                with k8s_cluster.port_forward(
+                    f"service/{service_name}", 8786, "-n", ns
+                ) as port:
+                    async with Client(
+                        f"tcp://localhost:{port}", asynchronous=True
+                    ) as client:
+                        await client.wait_for_workers(2)
+                        futures = client.map(lambda x: x + 1, range(10))
+                        total = client.submit(sum, futures)
+                        assert (await total) == sum(map(lambda x: x + 1, range(10)))
+
+
 def _get_job_status(k8s_cluster, ns):
     return json.loads(
         k8s_cluster.kubectl(
             "get",
             "-n",
             ns,
             "daskjobs.kubernetes.dask.org",
```

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/customresources/daskautoscaler.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskautoscaler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/customresources/daskcluster.patch.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskcluster.patch.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/customresources/daskcluster.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskcluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/customresources/daskjob.patch.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskjob.patch.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/customresources/daskjob.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/customresources/daskworkergroup.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/customresources/templates.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/templates.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/chartpress.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/chartpress.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -28,25 +28,36 @@
         {{- toYaml .Values.podSecurityContext | nindent 8 }}
       containers:
         - name: {{ .Chart.Name }}
           securityContext:
             {{- toYaml .Values.securityContext | nindent 12 }}
           image: "{{ .Values.image.name }}:{{ .Values.image.tag }}"
           imagePullPolicy: {{ .Values.image.pullPolicy }}
+          env:
+            - name: DASK_KUBERNETES__CONTROLLER__WORKER_ALLOCATION__BATCH_SIZE
+              value:
+                {{- toYaml .Values.workerAllocation.size | nindent 16 }}
+            - name: DASK_KUBERNETES__CONTROLLER__WORKER_ALLOCATION__DELAY
+              value:
+                {{- toYaml .Values.workerAllocation.delay | nindent 16 }}
           args:
             - --liveness=http://0.0.0.0:8080/healthz
           {{- with .Values.kopfArgs }}
             {{- toYaml . | nindent 12 }}
           {{- end }}
           resources:
             {{- toYaml .Values.resources | nindent 12 }}
           livenessProbe:
             httpGet:
               path: /healthz
               port: 8080
+          volumeMounts:
+            {{- toYaml .Values.volumeMounts | nindent 12 }}
+      volumes:
+        {{- toYaml .Values.volumes | nindent 8 }}
       {{- with .Values.nodeSelector }}
       nodeSelector:
         {{- toYaml . | nindent 8 }}
       {{- end }}
       {{- with .Values.affinity }}
       affinity:
         {{- toYaml . | nindent 8 }}
```

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,18 @@
   # limits:
   #   cpu: 100m
   #   memory: 128Mi
   # requests:
   #   cpu: 100m
   #   memory: 128Mi
 
+volumes: []  # Volumes for the operator pod
+
+volumeMounts: []  # Volume mounts for the operator container
+
 nodeSelector: {}  # Node selector
 
 tolerations: []  # Tolerations
 
 affinity: {}  # Affinity
 
 kopfArgs: # Command line flags to pass to kopf on start up
@@ -81,7 +85,11 @@
       additionalLabels: {} # Additional labels to add to the PodMonitor metadata.
       interval: 15s # Interval at which metrics should be scraped.
       jobLabel: "" # The label to use to retrieve the job name from.
       podTargetLabels:  # PodTargetLabels transfers labels on the Kubernetes Pod onto the target.
         - dask.org/cluster-name
         - dask.org/workergroup-name
       metricRelabelings: [] # MetricRelabelConfigs to apply to samples before ingestion.
+
+workerAllocation:
+  size: nil
+  delay: nil
```

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/kubecluster/discovery.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/discovery.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/kubecluster/kubecluster.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/kubecluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/kubecluster/tests/conftest.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/kubecluster/tests/test_discovery.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py` & `dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes.egg-info/PKG-INFO` & `dask-kubernetes-2023.7.0/dask_kubernetes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-kubernetes
-Version: 2023.6.1
+Version: 2023.7.0
 Summary: Native Kubernetes integration for Dask
 Home-page: https://github.com/dask/dask-kubernetes
 Maintainer: Jacob Tomlinson
 License: BSD
 Keywords: dask,kubernetes,distributed
 Requires-Python: >=3.9
 License-File: LICENSE
```

### Comparing `dask-kubernetes-2023.6.1/dask_kubernetes.egg-info/SOURCES.txt` & `dask-kubernetes-2023.7.0/dask_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/setup.cfg` & `dask-kubernetes-2023.7.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -75,13 +75,14 @@
 000004a0: 790a 7461 675f 7072 6566 6978 203d 200a  y.tag_prefix = .
 000004b0: 7061 7265 6e74 6469 725f 7072 6566 6978  parentdir_prefix
 000004c0: 203d 2064 6173 6b2d 6b75 6265 726e 6574   = dask-kubernet
 000004d0: 6573 2d0a 0a5b 746f 6f6c 3a70 7974 6573  es-..[tool:pytes
 000004e0: 745d 0a61 6464 6f70 7473 203d 202d 7620  t].addopts = -v 
 000004f0: 2d2d 6b65 6570 2d63 6c75 7374 6572 202d  --keep-cluster -
 00000500: 2d64 7572 6174 696f 6e73 3d31 300a 7469  -durations=10.ti
-00000510: 6d65 6f75 7420 3d20 3330 300a 7265 7275  meout = 300.reru
-00000520: 6e73 203d 2035 0a61 7379 6e63 696f 5f6d  ns = 5.asyncio_m
-00000530: 6f64 6520 3d20 7374 7269 6374 0a0a 5b65  ode = strict..[e
-00000540: 6767 5f69 6e66 6f5d 0a74 6167 5f62 7569  gg_info].tag_bui
-00000550: 6c64 203d 200a 7461 675f 6461 7465 203d  ld = .tag_date =
-00000560: 2030 0a0a                                 0..
+00000510: 6d65 6f75 7420 3d20 3630 0a74 696d 656f  meout = 60.timeo
+00000520: 7574 5f66 756e 635f 6f6e 6c79 203d 2074  ut_func_only = t
+00000530: 7275 650a 7265 7275 6e73 203d 2033 0a61  rue.reruns = 3.a
+00000540: 7379 6e63 696f 5f6d 6f64 6520 3d20 7374  syncio_mode = st
+00000550: 7269 6374 0a0a 5b65 6767 5f69 6e66 6f5d  rict..[egg_info]
+00000560: 0a74 6167 5f62 7569 6c64 203d 200a 7461  .tag_build = .ta
+00000570: 675f 6461 7465 203d 2030 0a0a            g_date = 0..
```

### Comparing `dask-kubernetes-2023.6.1/setup.py` & `dask-kubernetes-2023.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.6.1/versioneer.py` & `dask-kubernetes-2023.7.0/versioneer.py`

 * *Files identical despite different names*

