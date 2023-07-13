# Comparing `tmp/dask-kubernetes-2023.7.0.tar.gz` & `tmp/dask-kubernetes-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-kubernetes-2023.7.0.tar", last modified: Thu Jul 13 09:24:03 2023, max compression
+gzip compressed data, was "dask-kubernetes-2023.7.1.tar", last modified: Thu Jul 13 16:04:15 2023, max compression
```

## Comparing `dask-kubernetes-2023.7.0.tar` & `dask-kubernetes-2023.7.1.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.134774 dask-kubernetes-2023.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-13 09:24:03.134774 dask-kubernetes-2023.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.134774 dask-kubernetes-2023.7.0/dask_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-13 09:24:03.134774 dask-kubernetes-2023.7.0/dask_kubernetes/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.122774 dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.122774 dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/tests/test_pykube_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/tests/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/classic/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/classic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28558 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/classic/kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/classic/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/classic/tests/config-demo.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/classic/tests/fake_gcp_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    28838 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/classic/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/classic/tests/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/common/
--rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/common/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/common/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/common/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/common/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/common/tests/test_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/common/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/helm/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/helm/helmcluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/helm/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/helm/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/helm/tests/resources/values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/helm/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/kubernetes.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33066 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/plugins/noop/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/plugins/noop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/plugins/noop/noop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.126774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    26316 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/test_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.130774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskautoscaler.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskautoscaler.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskcluster.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskjob.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskjob.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskworkergroup.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskworkergroup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/templates.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.122774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.130774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/chartpress.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.130774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.130774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   283847 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   471240 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   140704 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.130774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/rolebinding.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/serviceaccount.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.130774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    42764 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.134774 dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/tests/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:24:03.122774 dask-kubernetes-2023.7.0/dask_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-13 09:24:03.000000 dask-kubernetes-2023.7.0/dask_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-13 09:24:03.000000 dask-kubernetes-2023.7.0/dask_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:24:03.000000 dask-kubernetes-2023.7.0/dask_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-13 09:24:03.000000 dask-kubernetes-2023.7.0/dask_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:24:03.000000 dask-kubernetes-2023.7.0/dask_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-13 09:24:03.000000 dask-kubernetes-2023.7.0/dask_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 09:24:03.000000 dask-kubernetes-2023.7.0/dask_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-13 09:24:03.134774 dask-kubernetes-2023.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1032 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68747 2023-07-13 09:23:56.000000 dask-kubernetes-2023.7.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.247977 dask-kubernetes-2023.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-13 16:04:15.247977 dask-kubernetes-2023.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.247977 dask-kubernetes-2023.7.1/dask_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-13 16:04:15.247977 dask-kubernetes-2023.7.1/dask_kubernetes/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.239977 dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.239977 dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/tests/test_pykube_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/tests/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.239977 dask-kubernetes-2023.7.1/dask_kubernetes/classic/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/classic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28558 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/classic/kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.239977 dask-kubernetes-2023.7.1/dask_kubernetes/classic/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/classic/tests/config-demo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/classic/tests/fake_gcp_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28838 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/classic/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/classic/tests/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.239977 dask-kubernetes-2023.7.1/dask_kubernetes/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.239977 dask-kubernetes-2023.7.1/dask_kubernetes/common/
+-rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/common/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/common/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/common/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.239977 dask-kubernetes-2023.7.1/dask_kubernetes/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/common/tests/test_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/common/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.239977 dask-kubernetes-2023.7.1/dask_kubernetes/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/helm/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/helm/helmcluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/helm/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/helm/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/helm/tests/resources/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/helm/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/kubernetes.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33038 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/plugins/noop/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/plugins/noop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/plugins/noop/noop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    26316 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/test_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskautoscaler.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskautoscaler.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskcluster.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskcluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskjob.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskworkergroup.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskworkergroup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/templates.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.235977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/chartpress.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   283847 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   471240 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   140704 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.247977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/rolebinding.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/serviceaccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.247977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42764 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.247977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/tests/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.239977 dask-kubernetes-2023.7.1/dask_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-13 16:04:15.000000 dask-kubernetes-2023.7.1/dask_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-13 16:04:15.000000 dask-kubernetes-2023.7.1/dask_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:04:15.000000 dask-kubernetes-2023.7.1/dask_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-13 16:04:15.000000 dask-kubernetes-2023.7.1/dask_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:04:15.000000 dask-kubernetes-2023.7.1/dask_kubernetes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-13 16:04:15.000000 dask-kubernetes-2023.7.1/dask_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 16:04:15.000000 dask-kubernetes-2023.7.1/dask_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-13 16:04:15.247977 dask-kubernetes-2023.7.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1032 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68747 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/versioneer.py
```

### Comparing `dask-kubernetes-2023.7.0/LICENSE` & `dask-kubernetes-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/PKG-INFO` & `dask-kubernetes-2023.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-kubernetes
-Version: 2023.7.0
+Version: 2023.7.1
 Summary: Native Kubernetes integration for Dask
 Home-page: https://github.com/dask/dask-kubernetes
 Maintainer: Jacob Tomlinson
 License: BSD
 Keywords: dask,kubernetes,distributed
 Requires-Python: >=3.9
 License-File: LICENSE
```

### Comparing `dask-kubernetes-2023.7.0/README.rst` & `dask-kubernetes-2023.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/__init__.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/dask.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/dask.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/mixins.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/mixins.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/objects.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/query.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/query.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/tests/test_pykube_objects.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/tests/test_pykube_objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/aiopykube/tests/test_query.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/classic/kubecluster.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/classic/kubecluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/classic/tests/config-demo.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/classic/tests/config-demo.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/classic/tests/test_async.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/classic/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/classic/tests/test_sync.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/classic/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/cli/cli.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/cli/cli.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/common/auth.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/common/auth.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/common/networking.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/common/networking.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/common/objects.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/common/objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/common/tests/test_kind.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/common/tests/test_kind.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/common/tests/test_objects.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/common/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/common/utils.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/common/utils.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/conftest.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/conftest.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/experimental/__init__.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/helm/helmcluster.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/helm/helmcluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/helm/tests/test_helm.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/helm/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/kubernetes.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/kubernetes.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/_objects.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,49 +81,49 @@
     scalable_spec = "worker.replicas"
 
     async def pods(self) -> List[Pod]:
         return await self.api.get(
             Pod.endpoint,
             label_selector=",".join(
                 [
-                    f"dask.org/cluster-name={self.spec['cluster']}",
+                    f"dask.org/cluster-name={self.spec.cluster}",
                     "dask.org/component=worker",
                     f"dask.org/workergroup-name={self.name}",
                 ]
             ),
             namespace=self.namespace,
         )
 
     async def deployments(self) -> List[Deployment]:
         return await self.api.get(
             Deployment.endpoint,
             label_selector=",".join(
                 [
-                    f"dask.org/cluster-name={self.spec['cluster']}",
+                    f"dask.org/cluster-name={self.spec.cluster}",
                     "dask.org/component=worker",
                     f"dask.org/workergroup-name={self.name}",
                 ]
             ),
             namespace=self.namespace,
         )
 
     async def cluster(self) -> DaskCluster:
-        return await DaskCluster.get(self.spec["cluster"], namespace=self.namespace)
+        return await DaskCluster.get(self.spec.cluster, namespace=self.namespace)
 
 
 class DaskAutoscaler(APIObject):
     version = "kubernetes.dask.org/v1"
     endpoint = "daskautoscalers"
     kind = "DaskAutoscaler"
     plural = "daskautoscalers"
     singular = "daskautoscaler"
     namespaced = True
 
     async def cluster(self) -> DaskCluster:
-        return await DaskCluster.get(self.spec["cluster"], namespace=self.namespace)
+        return await DaskCluster.get(self.spec.cluster, namespace=self.namespace)
 
 
 class DaskJob(APIObject):
     version = "kubernetes.dask.org/v1"
     endpoint = "daskjobs"
     kind = "DaskJob"
     plural = "daskjobs"
```

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/controller.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -827,19 +827,20 @@
             }
         },
         subresource="status",
     )
 
 
 @kopf.on.create("daskautoscaler.kubernetes.dask.org")
-async def daskautoscaler_create(name, spec, namespace, logger, patch, **kwargs):
+async def daskautoscaler_create(body, logger, **_):
     """When an autoscaler is created make it a child of the associated cluster for cascade deletion."""
-    cluster = await DaskCluster.get(spec["cluster"], namespace=namespace)
-    kopf.adopt(patch, owner=cluster.raw)
-    logger.info(f"Autoscaler {name} successfully adopted by cluster {spec['cluster']}")
+    autoscaler = await DaskAutoscaler(body)
+    cluster = await autoscaler.cluster()
+    await cluster.adopt(autoscaler)
+    logger.info(f"Autoscaler {autoscaler.name} adopted by cluster {cluster.name}")
 
 
 @kopf.timer("daskautoscaler.kubernetes.dask.org", interval=5.0)
 async def daskautoscaler_adapt(spec, name, namespace, logger, **kwargs):
     try:
         scheduler = await Pod.get(
             label_selector={
```

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/controller/tests/test_controller.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskautoscaler.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskautoscaler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskcluster.patch.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskcluster.patch.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskcluster.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskcluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskjob.patch.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskjob.patch.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskjob.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/daskworkergroup.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/customresources/templates.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/templates.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/chartpress.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/chartpress.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -87,9 +87,9 @@
       jobLabel: "" # The label to use to retrieve the job name from.
       podTargetLabels:  # PodTargetLabels transfers labels on the Kubernetes Pod onto the target.
         - dask.org/cluster-name
         - dask.org/workergroup-name
       metricRelabelings: [] # MetricRelabelConfigs to apply to samples before ingestion.
 
 workerAllocation:
-  size: nil
-  delay: nil
+  size: null
+  delay: null
```

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/discovery.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/discovery.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/kubecluster.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/kubecluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/tests/conftest.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/tests/test_discovery.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py` & `dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes.egg-info/PKG-INFO` & `dask-kubernetes-2023.7.1/dask_kubernetes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-kubernetes
-Version: 2023.7.0
+Version: 2023.7.1
 Summary: Native Kubernetes integration for Dask
 Home-page: https://github.com/dask/dask-kubernetes
 Maintainer: Jacob Tomlinson
 License: BSD
 Keywords: dask,kubernetes,distributed
 Requires-Python: >=3.9
 License-File: LICENSE
```

### Comparing `dask-kubernetes-2023.7.0/dask_kubernetes.egg-info/SOURCES.txt` & `dask-kubernetes-2023.7.1/dask_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/setup.cfg` & `dask-kubernetes-2023.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/setup.py` & `dask-kubernetes-2023.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.0/versioneer.py` & `dask-kubernetes-2023.7.1/versioneer.py`

 * *Files identical despite different names*

