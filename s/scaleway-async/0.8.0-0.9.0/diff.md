# Comparing `tmp/scaleway_async-0.8.0.tar.gz` & `tmp/scaleway_async-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaleway_async-0.8.0.tar", max compression
+gzip compressed data, was "scaleway_async-0.9.0.tar", max compression
```

## Comparing `scaleway_async-0.8.0.tar` & `scaleway_async-0.9.0.tar`

### file list

```diff
@@ -1,144 +1,149 @@
--rw-r--r--   0        0        0       30 2023-02-23 14:16:52.919687 scaleway_async-0.8.0/README.md
--rw-r--r--   0        0        0     1124 2023-02-23 14:17:22.311674 scaleway_async-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      913 2023-02-23 14:16:52.919687 scaleway_async-0.8.0/scaleway_async/__init__.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.919687 scaleway_async-0.8.0/scaleway_async/account/__init__.py
--rw-r--r--   0        0        0      382 2023-02-23 14:16:52.919687 scaleway_async-0.8.0/scaleway_async/account/v2/__init__.py
--rw-r--r--   0        0        0     6911 2023-02-23 14:16:52.919687 scaleway_async-0.8.0/scaleway_async/account/v2/api.py
--rw-r--r--   0        0        0     2093 2023-02-23 14:16:52.919687 scaleway_async-0.8.0/scaleway_async/account/v2/marshalling.py
--rw-r--r--   0        0        0     2625 2023-02-23 14:16:52.919687 scaleway_async-0.8.0/scaleway_async/account/v2/types.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.919687 scaleway_async-0.8.0/scaleway_async/applesilicon/__init__.py
--rw-r--r--   0        0        0      968 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/applesilicon/v1alpha1/__init__.py
--rw-r--r--   0        0        0    17002 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/applesilicon/v1alpha1/api.py
--rw-r--r--   0        0        0      497 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/applesilicon/v1alpha1/content.py
--rw-r--r--   0        0        0     5992 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/applesilicon/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     7236 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/applesilicon/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/baremetal/__init__.py
--rw-r--r--   0        0        0     3212 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/baremetal/v1/__init__.py
--rw-r--r--   0        0        0    51541 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/baremetal/v1/api.py
--rw-r--r--   0        0        0     1066 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/baremetal/v1/content.py
--rw-r--r--   0        0        0    23204 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/baremetal/v1/marshalling.py
--rw-r--r--   0        0        0    27688 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/baremetal/v1/types.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/cockpit/__init__.py
--rw-r--r--   0        0        0     1132 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/cockpit/v1beta1/__init__.py
--rw-r--r--   0        0        0    20173 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/cockpit/v1beta1/api.py
--rw-r--r--   0        0        0      419 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/cockpit/v1beta1/content.py
--rw-r--r--   0        0        0    10976 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/cockpit/v1beta1/marshalling.py
--rw-r--r--   0        0        0     5378 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/cockpit/v1beta1/types.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/container/__init__.py
--rw-r--r--   0        0        0     2364 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/container/v1beta1/__init__.py
--rw-r--r--   0        0        0    49036 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/container/v1beta1/api.py
--rw-r--r--   0        0        0     1345 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/container/v1beta1/content.py
--rw-r--r--   0        0        0    14231 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/container/v1beta1/marshalling.py
--rw-r--r--   0        0        0    15235 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/container/v1beta1/types.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/domain/__init__.py
--rw-r--r--   0        0        0     8352 2023-02-23 14:16:52.923687 scaleway_async-0.8.0/scaleway_async/domain/v2beta1/__init__.py
--rw-r--r--   0        0        0    83638 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/domain/v2beta1/api.py
--rw-r--r--   0        0        0     1955 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/domain/v2beta1/content.py
--rw-r--r--   0        0        0    69133 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/domain/v2beta1/marshalling.py
--rw-r--r--   0        0        0    40060 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/domain/v2beta1/types.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/flexibleip/__init__.py
--rw-r--r--   0        0        0      978 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/flexibleip/v1alpha1/__init__.py
--rw-r--r--   0        0        0    18507 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/flexibleip/v1alpha1/api.py
--rw-r--r--   0        0        0      651 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/flexibleip/v1alpha1/content.py
--rw-r--r--   0        0        0     5916 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/flexibleip/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     8562 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/flexibleip/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/function/__init__.py
--rw-r--r--   0        0        0     3852 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/function/v1beta1/__init__.py
--rw-r--r--   0        0        0    59692 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/function/v1beta1/api.py
--rw-r--r--   0        0        0     1579 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/function/v1beta1/content.py
--rw-r--r--   0        0        0    22515 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/function/v1beta1/marshalling.py
--rw-r--r--   0        0        0    22030 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/function/v1beta1/types.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/iam/__init__.py
--rw-r--r--   0        0        0     1958 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/iam/v1alpha1/__init__.py
--rw-r--r--   0        0        0    54113 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/iam/v1alpha1/api.py
--rw-r--r--   0        0        0    18078 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/iam/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    25779 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/iam/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/instance/__init__.py
--rw-r--r--   0        0        0     7904 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/instance/v1/__init__.py
--rw-r--r--   0        0        0   124439 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/instance/v1/api.py
--rw-r--r--   0        0        0     2059 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/instance/v1/content.py
--rw-r--r--   0        0        0    77638 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/instance/v1/marshalling.py
--rw-r--r--   0        0        0    53721 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/instance/v1/types.py
--rw-r--r--   0        0        0     9591 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/instance/v1/types_private.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/iot/__init__.py
--rw-r--r--   0        0        0     3456 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/iot/v1/__init__.py
--rw-r--r--   0        0        0    57153 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/iot/v1/api.py
--rw-r--r--   0        0        0      364 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/iot/v1/content.py
--rw-r--r--   0        0        0    25767 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/iot/v1/marshalling.py
--rw-r--r--   0        0        0    31600 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/iot/v1/types.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/k8s/__init__.py
--rw-r--r--   0        0        0     3066 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/k8s/v1/__init__.py
--rw-r--r--   0        0        0    50917 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/k8s/v1/api.py
--rw-r--r--   0        0        0      937 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/k8s/v1/content.py
--rw-r--r--   0        0        0    24665 2023-02-23 14:16:52.927687 scaleway_async-0.8.0/scaleway_async/k8s/v1/marshalling.py
--rw-r--r--   0        0        0    42707 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/k8s/v1/types.py
--rw-r--r--   0        0        0      544 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/k8s/v1/types_private.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/lb/__init__.py
--rw-r--r--   0        0        0     5060 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/lb/v1/__init__.py
--rw-r--r--   0        0        0   200388 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/lb/v1/api.py
--rw-r--r--   0        0        0     1111 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/lb/v1/content.py
--rw-r--r--   0        0        0    57347 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/lb/v1/marshalling.py
--rw-r--r--   0        0        0    90093 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/lb/v1/types.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/marketplace/__init__.py
--rw-r--r--   0        0        0      636 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/marketplace/v1/__init__.py
--rw-r--r--   0        0        0     4142 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/marketplace/v1/api.py
--rw-r--r--   0        0        0     5060 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/marketplace/v1/marshalling.py
--rw-r--r--   0        0        0     3082 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/marketplace/v1/types.py
--rw-r--r--   0        0        0      892 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/marketplace/v2/__init__.py
--rw-r--r--   0        0        0    12138 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/marketplace/v2/api.py
--rw-r--r--   0        0        0     5014 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/marketplace/v2/marshalling.py
--rw-r--r--   0        0        0     4980 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/marketplace/v2/types.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/mnq/__init__.py
--rw-r--r--   0        0        0     1008 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/mnq/v1alpha1/__init__.py
--rw-r--r--   0        0        0    16288 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/mnq/v1alpha1/api.py
--rw-r--r--   0        0        0     7563 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/mnq/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     8725 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/mnq/v1alpha1/types.py
--rw-r--r--   0        0        0        0 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/py.typed
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/rdb/__init__.py
--rw-r--r--   0        0        0     5652 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/rdb/v1/__init__.py
--rw-r--r--   0        0        0   101537 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/rdb/v1/api.py
--rw-r--r--   0        0        0     1923 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/rdb/v1/content.py
--rw-r--r--   0        0        0    40541 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/rdb/v1/marshalling.py
--rw-r--r--   0        0        0    48977 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/rdb/v1/types.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/redis/__init__.py
--rw-r--r--   0        0        0     1934 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/redis/v1/__init__.py
--rw-r--r--   0        0        0    38169 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/redis/v1/api.py
--rw-r--r--   0        0        0      489 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/redis/v1/content.py
--rw-r--r--   0        0        0    16095 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/redis/v1/marshalling.py
--rw-r--r--   0        0        0    18601 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/redis/v1/types.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/registry/__init__.py
--rw-r--r--   0        0        0     1190 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/registry/v1/__init__.py
--rw-r--r--   0        0        0    25059 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/registry/v1/api.py
--rw-r--r--   0        0        0      713 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/registry/v1/content.py
--rw-r--r--   0        0        0     6029 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/registry/v1/marshalling.py
--rw-r--r--   0        0        0    10933 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/registry/v1/types.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/secret/__init__.py
--rw-r--r--   0        0        0      720 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/secret/v1alpha1/__init__.py
--rw-r--r--   0        0        0    20858 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/secret/v1alpha1/api.py
--rw-r--r--   0        0        0     4727 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/secret/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     8269 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/secret/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/tem/__init__.py
--rw-r--r--   0        0        0     1098 2023-02-23 14:16:52.931687 scaleway_async-0.8.0/scaleway_async/tem/v1alpha1/__init__.py
--rw-r--r--   0        0        0    20587 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/tem/v1alpha1/api.py
--rw-r--r--   0        0        0      551 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/tem/v1alpha1/content.py
--rw-r--r--   0        0        0     8098 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/tem/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    10633 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/tem/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/test/__init__.py
--rw-r--r--   0        0        0      598 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/test/v1/__init__.py
--rw-r--r--   0        0        0    11879 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/test/v1/api.py
--rw-r--r--   0        0        0      350 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/test/v1/content.py
--rw-r--r--   0        0        0     4376 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/test/v1/marshalling.py
--rw-r--r--   0        0        0     3298 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/test/v1/types.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/vpc/__init__.py
--rw-r--r--   0        0        0      416 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/vpc/v1/__init__.py
--rw-r--r--   0        0        0    10077 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/vpc/v1/api.py
--rw-r--r--   0        0        0     2448 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/vpc/v1/marshalling.py
--rw-r--r--   0        0        0     3981 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/vpc/v1/types.py
--rw-r--r--   0        0        0      127 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/vpcgw/__init__.py
--rw-r--r--   0        0        0     2168 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/vpcgw/v1/__init__.py
--rw-r--r--   0        0        0    67947 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/vpcgw/v1/api.py
--rw-r--r--   0        0        0      757 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/vpcgw/v1/content.py
--rw-r--r--   0        0        0    19589 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/vpcgw/v1/marshalling.py
--rw-r--r--   0        0        0    32965 2023-02-23 14:16:52.935687 scaleway_async-0.8.0/scaleway_async/vpcgw/v1/types.py
--rw-r--r--   0        0        0     2009 1970-01-01 00:00:00.000000 scaleway_async-0.8.0/setup.py
--rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 scaleway_async-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-03-08 16:40:37.480112 scaleway_async-0.9.0/README.md
+-rw-r--r--   0        0        0     1124 2023-03-08 16:40:57.464228 scaleway_async-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      913 2023-03-08 16:40:37.480112 scaleway_async-0.9.0/scaleway_async/__init__.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.480112 scaleway_async-0.9.0/scaleway_async/account/__init__.py
+-rw-r--r--   0        0        0      382 2023-03-08 16:40:37.480112 scaleway_async-0.9.0/scaleway_async/account/v2/__init__.py
+-rw-r--r--   0        0        0     6931 2023-03-08 16:40:37.480112 scaleway_async-0.9.0/scaleway_async/account/v2/api.py
+-rw-r--r--   0        0        0     2093 2023-03-08 16:40:37.480112 scaleway_async-0.9.0/scaleway_async/account/v2/marshalling.py
+-rw-r--r--   0        0        0     2649 2023-03-08 16:40:37.480112 scaleway_async-0.9.0/scaleway_async/account/v2/types.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.480112 scaleway_async-0.9.0/scaleway_async/applesilicon/__init__.py
+-rw-r--r--   0        0        0      968 2023-03-08 16:40:37.480112 scaleway_async-0.9.0/scaleway_async/applesilicon/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    17002 2023-03-08 16:40:37.480112 scaleway_async-0.9.0/scaleway_async/applesilicon/v1alpha1/api.py
+-rw-r--r--   0        0        0      497 2023-03-08 16:40:37.480112 scaleway_async-0.9.0/scaleway_async/applesilicon/v1alpha1/content.py
+-rw-r--r--   0        0        0     5992 2023-03-08 16:40:37.480112 scaleway_async-0.9.0/scaleway_async/applesilicon/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     7236 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/applesilicon/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/baremetal/__init__.py
+-rw-r--r--   0        0        0     3212 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/baremetal/v1/__init__.py
+-rw-r--r--   0        0        0    51541 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/baremetal/v1/api.py
+-rw-r--r--   0        0        0     1066 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/baremetal/v1/content.py
+-rw-r--r--   0        0        0    23419 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/baremetal/v1/marshalling.py
+-rw-r--r--   0        0        0    27948 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/baremetal/v1/types.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/cockpit/__init__.py
+-rw-r--r--   0        0        0     1132 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/cockpit/v1beta1/__init__.py
+-rw-r--r--   0        0        0    20461 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/cockpit/v1beta1/api.py
+-rw-r--r--   0        0        0      419 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/cockpit/v1beta1/content.py
+-rw-r--r--   0        0        0    10976 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/cockpit/v1beta1/marshalling.py
+-rw-r--r--   0        0        0     5403 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/cockpit/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/container/__init__.py
+-rw-r--r--   0        0        0     2364 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/container/v1beta1/__init__.py
+-rw-r--r--   0        0        0    49036 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/container/v1beta1/api.py
+-rw-r--r--   0        0        0     1345 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/container/v1beta1/content.py
+-rw-r--r--   0        0        0    14231 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/container/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    15235 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/container/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/domain/__init__.py
+-rw-r--r--   0        0        0     8352 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/domain/v2beta1/__init__.py
+-rw-r--r--   0        0        0    83638 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/domain/v2beta1/api.py
+-rw-r--r--   0        0        0     1955 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/domain/v2beta1/content.py
+-rw-r--r--   0        0        0    69133 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/domain/v2beta1/marshalling.py
+-rw-r--r--   0        0        0    40060 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/domain/v2beta1/types.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/flexibleip/__init__.py
+-rw-r--r--   0        0        0      978 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/flexibleip/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    18507 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/flexibleip/v1alpha1/api.py
+-rw-r--r--   0        0        0      651 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/flexibleip/v1alpha1/content.py
+-rw-r--r--   0        0        0     5916 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/flexibleip/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     8562 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/flexibleip/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/function/__init__.py
+-rw-r--r--   0        0        0     3852 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/function/v1beta1/__init__.py
+-rw-r--r--   0        0        0    59692 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/function/v1beta1/api.py
+-rw-r--r--   0        0        0     1579 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/function/v1beta1/content.py
+-rw-r--r--   0        0        0    23167 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/function/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    22306 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/function/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/iam/__init__.py
+-rw-r--r--   0        0        0     2300 2023-03-08 16:40:37.484112 scaleway_async-0.9.0/scaleway_async/iam/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    61207 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/iam/v1alpha1/api.py
+-rw-r--r--   0        0        0    20377 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/iam/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    29047 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/iam/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/instance/__init__.py
+-rw-r--r--   0        0        0     7904 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/instance/v1/__init__.py
+-rw-r--r--   0        0        0   124439 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/instance/v1/api.py
+-rw-r--r--   0        0        0     2059 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/instance/v1/content.py
+-rw-r--r--   0        0        0    77638 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/instance/v1/marshalling.py
+-rw-r--r--   0        0        0    53721 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/instance/v1/types.py
+-rw-r--r--   0        0        0     9591 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/instance/v1/types_private.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/iot/__init__.py
+-rw-r--r--   0        0        0     3456 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/iot/v1/__init__.py
+-rw-r--r--   0        0        0    57153 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/iot/v1/api.py
+-rw-r--r--   0        0        0      364 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/iot/v1/content.py
+-rw-r--r--   0        0        0    25767 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/iot/v1/marshalling.py
+-rw-r--r--   0        0        0    31600 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/iot/v1/types.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/k8s/__init__.py
+-rw-r--r--   0        0        0     3066 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/k8s/v1/__init__.py
+-rw-r--r--   0        0        0    50917 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/k8s/v1/api.py
+-rw-r--r--   0        0        0      937 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/k8s/v1/content.py
+-rw-r--r--   0        0        0    24665 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/k8s/v1/marshalling.py
+-rw-r--r--   0        0        0    42707 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/k8s/v1/types.py
+-rw-r--r--   0        0        0      544 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/k8s/v1/types_private.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/lb/__init__.py
+-rw-r--r--   0        0        0     5060 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/lb/v1/__init__.py
+-rw-r--r--   0        0        0   201004 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/lb/v1/api.py
+-rw-r--r--   0        0        0     1111 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/lb/v1/content.py
+-rw-r--r--   0        0        0    58137 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/lb/v1/marshalling.py
+-rw-r--r--   0        0        0    90813 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/lb/v1/types.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/marketplace/__init__.py
+-rw-r--r--   0        0        0      636 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/marketplace/v1/__init__.py
+-rw-r--r--   0        0        0     4142 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/marketplace/v1/api.py
+-rw-r--r--   0        0        0     5060 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/marketplace/v1/marshalling.py
+-rw-r--r--   0        0        0     3082 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/marketplace/v1/types.py
+-rw-r--r--   0        0        0      892 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/marketplace/v2/__init__.py
+-rw-r--r--   0        0        0    12138 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/marketplace/v2/api.py
+-rw-r--r--   0        0        0     5014 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/marketplace/v2/marshalling.py
+-rw-r--r--   0        0        0     4980 2023-03-08 16:40:37.488112 scaleway_async-0.9.0/scaleway_async/marketplace/v2/types.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/mnq/__init__.py
+-rw-r--r--   0        0        0     1008 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/mnq/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    16288 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/mnq/v1alpha1/api.py
+-rw-r--r--   0        0        0     7563 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/mnq/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     8725 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/mnq/v1alpha1/types.py
+-rw-r--r--   0        0        0        0 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/py.typed
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/rdb/__init__.py
+-rw-r--r--   0        0        0     5874 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/rdb/v1/__init__.py
+-rw-r--r--   0        0        0   103268 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/rdb/v1/api.py
+-rw-r--r--   0        0        0     1923 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/rdb/v1/content.py
+-rw-r--r--   0        0        0    41536 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/rdb/v1/marshalling.py
+-rw-r--r--   0        0        0    50927 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/rdb/v1/types.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/redis/__init__.py
+-rw-r--r--   0        0        0     1934 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/redis/v1/__init__.py
+-rw-r--r--   0        0        0    38169 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/redis/v1/api.py
+-rw-r--r--   0        0        0      489 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/redis/v1/content.py
+-rw-r--r--   0        0        0    16095 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/redis/v1/marshalling.py
+-rw-r--r--   0        0        0    18601 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/redis/v1/types.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/registry/__init__.py
+-rw-r--r--   0        0        0     1190 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/registry/v1/__init__.py
+-rw-r--r--   0        0        0    25059 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/registry/v1/api.py
+-rw-r--r--   0        0        0      713 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/registry/v1/content.py
+-rw-r--r--   0        0        0     6029 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/registry/v1/marshalling.py
+-rw-r--r--   0        0        0    10933 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/registry/v1/types.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/secret/__init__.py
+-rw-r--r--   0        0        0      720 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/secret/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    27369 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/secret/v1alpha1/api.py
+-rw-r--r--   0        0        0     4727 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/secret/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     9711 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/secret/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/tem/__init__.py
+-rw-r--r--   0        0        0     1098 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/tem/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    20587 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/tem/v1alpha1/api.py
+-rw-r--r--   0        0        0      551 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/tem/v1alpha1/content.py
+-rw-r--r--   0        0        0     8098 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/tem/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    10633 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/tem/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/test/__init__.py
+-rw-r--r--   0        0        0      598 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/test/v1/__init__.py
+-rw-r--r--   0        0        0    11879 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/test/v1/api.py
+-rw-r--r--   0        0        0      350 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/test/v1/content.py
+-rw-r--r--   0        0        0     4376 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/test/v1/marshalling.py
+-rw-r--r--   0        0        0     3298 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/test/v1/types.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/vpc/__init__.py
+-rw-r--r--   0        0        0      416 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/vpc/v1/__init__.py
+-rw-r--r--   0        0        0    10109 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/vpc/v1/api.py
+-rw-r--r--   0        0        0     2448 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/vpc/v1/marshalling.py
+-rw-r--r--   0        0        0     4014 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/vpc/v1/types.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/vpcgw/__init__.py
+-rw-r--r--   0        0        0     2168 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/vpcgw/v1/__init__.py
+-rw-r--r--   0        0        0    68382 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/vpcgw/v1/api.py
+-rw-r--r--   0        0        0      757 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/vpcgw/v1/content.py
+-rw-r--r--   0        0        0    19645 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/vpcgw/v1/marshalling.py
+-rw-r--r--   0        0        0    33321 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/vpcgw/v1/types.py
+-rw-r--r--   0        0        0      127 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/webhosting/__init__.py
+-rw-r--r--   0        0        0     1316 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/webhosting/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    14508 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/webhosting/v1alpha1/api.py
+-rw-r--r--   0        0        0      393 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/webhosting/v1alpha1/content.py
+-rw-r--r--   0        0        0     7639 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/webhosting/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     8918 2023-03-08 16:40:37.492112 scaleway_async-0.9.0/scaleway_async/webhosting/v1alpha1/types.py
+-rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 scaleway_async-0.9.0/PKG-INFO
```

### Comparing `scaleway_async-0.8.0/pyproject.toml` & `scaleway_async-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scaleway-async"
-version = "0.8.0"
+version = "0.9.0"
 description = "Scaleway SDK for Python"
 authors = ["Scaleway <opensource@scaleway.com>"]
 license = "BSD"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
```

### Comparing `scaleway_async-0.8.0/scaleway_async/__init__.py` & `scaleway_async-0.9.0/scaleway_async/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/account/v2/api.py` & `scaleway_async-0.9.0/scaleway_async/account/v2/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -35,17 +35,17 @@
         *,
         name: str,
         organization_id: Optional[str] = None,
         description: Optional[str] = None,
     ) -> Project:
         """
         Create project
-        :param name: The name of the project
-        :param organization_id: The organization ID of the project
-        :param description: The description of the project
+        :param name: The name of the project.
+        :param organization_id: The organization ID of the project.
+        :param description: The description of the project.
         :return: :class:`Project <Project>`
 
         Usage:
         ::
 
             result = await api.create_project(name="example")
         """
@@ -74,20 +74,20 @@
         page: Optional[int] = None,
         page_size: Optional[int] = None,
         order_by: ListProjectsRequestOrderBy = ListProjectsRequestOrderBy.CREATED_AT_ASC,
         project_ids: Optional[List[str]] = None,
     ) -> ListProjectsResponse:
         """
         List projects
-        :param organization_id: The organization ID of the project
-        :param name: The name of the project
-        :param page: The page number for the returned projects
-        :param page_size: The maximum number of project per page
-        :param order_by: The sort order of the returned projects
-        :param project_ids: Filter out by a list of project ID
+        :param organization_id: The organization ID of the project.
+        :param name: The name of the project.
+        :param page: The page number for the returned projects.
+        :param page_size: The maximum number of project per page.
+        :param order_by: The sort order of the returned projects.
+        :param project_ids: Filter out by a list of project ID.
         :return: :class:`ListProjectsResponse <ListProjectsResponse>`
 
         Usage:
         ::
 
             result = await api.list_projects()
         """
@@ -117,20 +117,20 @@
         page: Optional[int] = None,
         page_size: Optional[int] = None,
         order_by: Optional[ListProjectsRequestOrderBy] = None,
         project_ids: Optional[List[str]] = None,
     ) -> List[Project]:
         """
         List projects
-        :param organization_id: The organization ID of the project
-        :param name: The name of the project
-        :param page: The page number for the returned projects
-        :param page_size: The maximum number of project per page
-        :param order_by: The sort order of the returned projects
-        :param project_ids: Filter out by a list of project ID
+        :param organization_id: The organization ID of the project.
+        :param name: The name of the project.
+        :param page: The page number for the returned projects.
+        :param page_size: The maximum number of project per page.
+        :param order_by: The sort order of the returned projects.
+        :param project_ids: Filter out by a list of project ID.
         :return: :class:`List[ListProjectsResponse] <List[ListProjectsResponse]>`
 
         Usage:
         ::
 
             result = await api.list_projects_all()
         """
@@ -152,15 +152,15 @@
     async def get_project(
         self,
         *,
         project_id: Optional[str] = None,
     ) -> Project:
         """
         Get project
-        :param project_id: The project ID of the project
+        :param project_id: The project ID of the project.
         :return: :class:`Project <Project>`
 
         Usage:
         ::
 
             result = await api.get_project()
         """
@@ -180,15 +180,15 @@
     async def delete_project(
         self,
         *,
         project_id: Optional[str] = None,
     ) -> Optional[None]:
         """
         Delete project
-        :param project_id: The project ID of the project
+        :param project_id: The project ID of the project.
 
         Usage:
         ::
 
             result = await api.delete_project()
         """
 
@@ -209,17 +209,17 @@
         *,
         project_id: Optional[str] = None,
         name: Optional[str] = None,
         description: Optional[str] = None,
     ) -> Project:
         """
         Update project
-        :param project_id: The project ID of the project
-        :param name: The name of the project
-        :param description: The description of the project
+        :param project_id: The project ID of the project.
+        :param name: The name of the project.
+        :param description: The description of the project.
         :return: :class:`Project <Project>`
 
         Usage:
         ::
 
             result = await api.update_project()
         """
```

### Comparing `scaleway_async-0.8.0/scaleway_async/account/v2/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/account/v2/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/account/v2/types.py` & `scaleway_async-0.9.0/scaleway_async/account/v2/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,141 +17,141 @@
     def __str__(self) -> str:
         return str(self.value)
 
 
 @dataclass
 class ListProjectsResponse:
     """
-    List projects response
+    List projects response.
     """
 
     total_count: int
     """
-    The total number of projects
+    The total number of projects.
     """
 
     projects: List[Project]
     """
-    The paginated returned projects
+    The paginated returned projects.
     """
 
 
 @dataclass
 class Project:
     """
-    Project
+    Project.
     """
 
     id: str
     """
-    The ID of the project
+    The ID of the project.
     """
 
     name: str
     """
-    The name of the project
+    The name of the project.
     """
 
     organization_id: str
     """
-    The organization ID of the project
+    The organization ID of the project.
     """
 
     created_at: Optional[datetime]
     """
-    The creation date of the project
+    The creation date of the project.
     """
 
     updated_at: Optional[datetime]
     """
-    The update date of the project
+    The update date of the project.
     """
 
     description: str
     """
-    The description of the project
+    The description of the project.
     """
 
 
 @dataclass
 class CreateProjectRequest:
     name: str
     """
-    The name of the project
+    The name of the project.
     """
 
     organization_id: Optional[str]
     """
-    The organization ID of the project
+    The organization ID of the project.
     """
 
     description: Optional[str]
     """
-    The description of the project
+    The description of the project.
     """
 
 
 @dataclass
 class ListProjectsRequest:
     organization_id: Optional[str]
     """
-    The organization ID of the project
+    The organization ID of the project.
     """
 
     name: Optional[str]
     """
-    The name of the project
+    The name of the project.
     """
 
     page: Optional[int]
     """
-    The page number for the returned projects
+    The page number for the returned projects.
     """
 
     page_size: Optional[int]
     """
-    The maximum number of project per page
+    The maximum number of project per page.
     """
 
     order_by: Optional[ListProjectsRequestOrderBy]
     """
-    The sort order of the returned projects
+    The sort order of the returned projects.
     """
 
     project_ids: Optional[List[str]]
     """
-    Filter out by a list of project ID
+    Filter out by a list of project ID.
     """
 
 
 @dataclass
 class GetProjectRequest:
     project_id: Optional[str]
     """
-    The project ID of the project
+    The project ID of the project.
     """
 
 
 @dataclass
 class DeleteProjectRequest:
     project_id: Optional[str]
     """
-    The project ID of the project
+    The project ID of the project.
     """
 
 
 @dataclass
 class UpdateProjectRequest:
     project_id: Optional[str]
     """
-    The project ID of the project
+    The project ID of the project.
     """
 
     name: Optional[str]
     """
-    The name of the project
+    The name of the project.
     """
 
     description: Optional[str]
     """
-    The description of the project
+    The description of the project.
     """
```

### Comparing `scaleway_async-0.8.0/scaleway_async/applesilicon/v1alpha1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/applesilicon/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/applesilicon/v1alpha1/api.py` & `scaleway_async-0.9.0/scaleway_async/applesilicon/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/applesilicon/v1alpha1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/applesilicon/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/applesilicon/v1alpha1/types.py` & `scaleway_async-0.9.0/scaleway_async/applesilicon/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/baremetal/v1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/baremetal/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/baremetal/v1/api.py` & `scaleway_async-0.9.0/scaleway_async/baremetal/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/baremetal/v1/content.py` & `scaleway_async-0.9.0/scaleway_async/baremetal/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/baremetal/v1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/baremetal/v1/marshalling.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,28 +412,37 @@
 
     field = data.get("price_per_hour")
     args["price_per_hour"] = unmarshal_Money(field) if field is not None else None
 
     field = data.get("price_per_month")
     args["price_per_month"] = unmarshal_Money(field) if field is not None else None
 
+    field = data.get("private_bandwidth")
+    args["private_bandwidth"] = field
+
     field = data.get("quota_name")
     args["quota_name"] = field
 
     field = data.get("raid_controllers")
     args["raid_controllers"] = [
         unmarshal_RaidController(v) for v in data["raid_controllers"]
     ]
 
+    field = data.get("shared_bandwidth")
+    args["shared_bandwidth"] = field
+
     field = data.get("stock")
     args["stock"] = field
 
     field = data.get("subscription_period")
     args["subscription_period"] = field
 
+    field = data.get("tags")
+    args["tags"] = field
+
     return Offer(**args)
 
 
 def unmarshal_Option(data: Any) -> Option:
     if type(data) is not dict:
         raise TypeError(
             f"Unmarshalling the type 'Option' failed as data isn't a dictionary."
```

### Comparing `scaleway_async-0.8.0/scaleway_async/baremetal/v1/types.py` & `scaleway_async-0.9.0/scaleway_async/baremetal/v1/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -555,15 +555,15 @@
     stock: OfferStock
     """
     Stock level
     """
 
     bandwidth: int
     """
-    Bandwidth available in bits/s with the offer
+    Public Bandwidth available in bits/s with the offer
     """
 
     commercial_range: str
     """
     Commercial range of the offer
     """
 
@@ -633,14 +633,29 @@
     """
 
     options: List[OfferOptionOffer]
     """
     Options available on offer
     """
 
+    private_bandwidth: int
+    """
+    Private bandwidth available in bits/s with the offer
+    """
+
+    shared_bandwidth: bool
+    """
+    The offer is shared or not
+    """
+
+    tags: List[str]
+    """
+    Array of tags attached to the offer
+    """
+
 
 @dataclass
 class OfferOptionOffer:
     """
     Offer. option offer
     """
```

### Comparing `scaleway_async-0.8.0/scaleway_async/cockpit/v1beta1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/cockpit/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/cockpit/v1beta1/api.py` & `scaleway_async-0.9.0/scaleway_async/cockpit/v1beta1/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,17 @@
 
     async def activate_cockpit(
         self,
         *,
         project_id: Optional[str] = None,
     ) -> Cockpit:
         """
+        Activate a cockpit associated with the given project ID.
+        :param project_id:
+        :return: :class:`Cockpit <Cockpit>`
 
         Usage:
         ::
 
             result = await api.activate_cockpit()
         """
 
@@ -156,14 +159,17 @@
 
     async def deactivate_cockpit(
         self,
         *,
         project_id: Optional[str] = None,
     ) -> Cockpit:
         """
+        Deactivate a cockpit associated with the given project ID.
+        :param project_id:
+        :return: :class:`Cockpit <Cockpit>`
 
         Usage:
         ::
 
             result = await api.deactivate_cockpit()
         """
 
@@ -183,15 +189,15 @@
 
     async def reset_cockpit_grafana(
         self,
         *,
         project_id: Optional[str] = None,
     ) -> Cockpit:
         """
-        Reset the Grafana your cockpit associated with the given project ID.
+        Reset the Grafana of your cockpit associated with the given project ID.
         :param project_id:
         :return: :class:`Cockpit <Cockpit>`
 
         Usage:
         ::
 
             result = await api.reset_cockpit_grafana()
@@ -215,15 +221,15 @@
         self,
         *,
         name: str,
         project_id: Optional[str] = None,
         scopes: Optional[TokenScopes] = None,
     ) -> Token:
         """
-        Create token associated with the given project ID.
+        Create a token associated with the given project ID.
         :param project_id:
         :param name:
         :param scopes:
         :return: :class:`Token <Token>`
 
         Usage:
         ::
@@ -372,16 +378,16 @@
         self,
         *,
         project_id: Optional[str] = None,
         contact_point: Optional[ContactPoint] = None,
     ) -> ContactPoint:
         """
         Create an alert contact point for the default receiver.
-        :param project_id: Project ID
-        :param contact_point: Contact point to create
+        :param project_id: Project ID.
+        :param contact_point: Contact point to create.
         :return: :class:`ContactPoint <ContactPoint>`
 
         Usage:
         ::
 
             result = await api.create_contact_point()
         """
@@ -406,17 +412,17 @@
         *,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
         project_id: Optional[str] = None,
     ) -> ListContactPointsResponse:
         """
         List alert contact points associated with the given cockpit ID.
-        :param page: Page number
-        :param page_size: Page size
-        :param project_id: Project ID
+        :param page: Page number.
+        :param page_size: Page size.
+        :param project_id: Project ID.
         :return: :class:`ListContactPointsResponse <ListContactPointsResponse>`
 
         Usage:
         ::
 
             result = await api.list_contact_points()
         """
@@ -439,17 +445,17 @@
         *,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
         project_id: Optional[str] = None,
     ) -> List[ContactPoint]:
         """
         List alert contact points associated with the given cockpit ID.
-        :param page: Page number
-        :param page_size: Page size
-        :param project_id: Project ID
+        :param page: Page number.
+        :param page_size: Page size.
+        :param project_id: Project ID.
         :return: :class:`List[ListContactPointsResponse] <List[ListContactPointsResponse]>`
 
         Usage:
         ::
 
             result = await api.list_contact_points_all()
         """
@@ -470,15 +476,15 @@
         *,
         project_id: Optional[str] = None,
         contact_point: Optional[ContactPoint] = None,
     ) -> Optional[None]:
         """
         Delete an alert contact point for the default receiver.
         :param project_id:
-        :param contact_point: Contact point to delete
+        :param contact_point: Contact point to delete.
 
         Usage:
         ::
 
             result = await api.delete_contact_point()
         """
```

### Comparing `scaleway_async-0.8.0/scaleway_async/cockpit/v1beta1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/cockpit/v1beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/cockpit/v1beta1/types.py` & `scaleway_async-0.9.0/scaleway_async/cockpit/v1beta1/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,67 +46,67 @@
     def __str__(self) -> str:
         return str(self.value)
 
 
 @dataclass
 class Cockpit:
     """
-    Cockpit
+    Cockpit.
     """
 
     project_id: str
     """
-    Project ID
+    Project ID.
     """
 
     created_at: Optional[datetime]
     """
-    Created at
+    Created at.
     """
 
     updated_at: Optional[datetime]
     """
-    Updated at
+    Updated at.
     """
 
     endpoints: Optional[CockpitEndpoints]
     """
-    Endpoints
+    Endpoints.
     """
 
     status: CockpitStatus
     """
-    Status
+    Status.
     """
 
     managed_alerts_enabled: bool
     """
-    Managed alerts enabled
+    Managed alerts enabled.
     """
 
 
 @dataclass
 class CockpitEndpoints:
     """
-    Cockpit. endpoints
+    Cockpit. endpoints.
     """
 
     metrics_url: str
 
     logs_url: str
 
     alertmanager_url: str
 
     grafana_url: str
 
 
 @dataclass
 class ContactPoint:
     """
-    Alert contact point
+    Alert contact point.
     """
 
     email: Optional[ContactPointEmail]
     """
     Alert contact point configuration.
     
     One-of ('configuration'): at most one of 'email' could be set.
@@ -117,79 +117,79 @@
 class ContactPointEmail:
     to: str
 
 
 @dataclass
 class GrafanaUser:
     """
-    Grafana user
+    Grafana user.
     """
 
     id: int
 
     login: str
 
     role: GrafanaUserRole
 
     password: Optional[str]
 
 
 @dataclass
 class ListContactPointsResponse:
     """
-    List contact points response
+    List contact points response.
     """
 
     total_count: int
     """
-    Total count of contact points
+    Total count of contact points.
     """
 
     contact_points: List[ContactPoint]
     """
-    Contact points array
+    Contact points array.
     """
 
     has_additional_receivers: bool
     """
-    Has receivers other than default
+    Has receivers other than default.
     """
 
     has_additional_contact_points: bool
     """
-    Has unmanaged contact points
+    Has unmanaged contact points.
     """
 
 
 @dataclass
 class ListGrafanaUsersResponse:
     """
-    List grafana users response
+    List grafana users response.
     """
 
     total_count: int
 
     grafana_users: List[GrafanaUser]
 
 
 @dataclass
 class ListTokensResponse:
     """
-    List tokens response
+    List tokens response.
     """
 
     total_count: int
 
     tokens: List[Token]
 
 
 @dataclass
 class Token:
     """
-    Token
+    Token.
     """
 
     id: str
 
     project_id: str
 
     name: str
@@ -202,15 +202,15 @@
 
     secret_key: Optional[str]
 
 
 @dataclass
 class TokenScopes:
     """
-    Token scopes
+    Token scopes.
     """
 
     query_metrics: bool
 
     write_metrics: bool
 
     setup_metrics_rules: bool
@@ -274,48 +274,48 @@
     token_id: str
 
 
 @dataclass
 class CreateContactPointRequest:
     project_id: Optional[str]
     """
-    Project ID
+    Project ID.
     """
 
     contact_point: Optional[ContactPoint]
     """
-    Contact point to create
+    Contact point to create.
     """
 
 
 @dataclass
 class ListContactPointsRequest:
     page: Optional[int]
     """
-    Page number
+    Page number.
     """
 
     page_size: Optional[int]
     """
-    Page size
+    Page size.
     """
 
     project_id: Optional[str]
     """
-    Project ID
+    Project ID.
     """
 
 
 @dataclass
 class DeleteContactPointRequest:
     project_id: Optional[str]
 
     contact_point: Optional[ContactPoint]
     """
-    Contact point to delete
+    Contact point to delete.
     """
 
 
 @dataclass
 class EnableManagedAlertsRequest:
     project_id: Optional[str]
```

### Comparing `scaleway_async-0.8.0/scaleway_async/container/v1beta1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/container/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/container/v1beta1/api.py` & `scaleway_async-0.9.0/scaleway_async/container/v1beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/container/v1beta1/content.py` & `scaleway_async-0.9.0/scaleway_async/container/v1beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/container/v1beta1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/container/v1beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/container/v1beta1/types.py` & `scaleway_async-0.9.0/scaleway_async/container/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/domain/v2beta1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/domain/v2beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/domain/v2beta1/api.py` & `scaleway_async-0.9.0/scaleway_async/domain/v2beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/domain/v2beta1/content.py` & `scaleway_async-0.9.0/scaleway_async/domain/v2beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/domain/v2beta1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/domain/v2beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/domain/v2beta1/types.py` & `scaleway_async-0.9.0/scaleway_async/domain/v2beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/flexibleip/v1alpha1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/flexibleip/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/flexibleip/v1alpha1/api.py` & `scaleway_async-0.9.0/scaleway_async/flexibleip/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/flexibleip/v1alpha1/content.py` & `scaleway_async-0.9.0/scaleway_async/flexibleip/v1alpha1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/flexibleip/v1alpha1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/flexibleip/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/flexibleip/v1alpha1/types.py` & `scaleway_async-0.9.0/scaleway_async/flexibleip/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/function/v1beta1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/function/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/function/v1beta1/api.py` & `scaleway_async-0.9.0/scaleway_async/function/v1beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/function/v1beta1/content.py` & `scaleway_async-0.9.0/scaleway_async/function/v1beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/function/v1beta1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/function/v1beta1/marshalling.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,20 @@
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("mnq_namespace_id")
     args["mnq_namespace_id"] = field
 
+    field = data.get("mnq_project_id")
+    args["mnq_project_id"] = field
+
+    field = data.get("mnq_region")
+    args["mnq_region"] = field
+
     field = data.get("subject")
     args["subject"] = field
 
     return TriggerMnqNatsClientConfig(**args)
 
 
 def unmarshal_TriggerMnqSqsClientConfig(data: Any) -> TriggerMnqSqsClientConfig:
@@ -96,14 +102,20 @@
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("mnq_namespace_id")
     args["mnq_namespace_id"] = field
 
+    field = data.get("mnq_project_id")
+    args["mnq_project_id"] = field
+
+    field = data.get("mnq_region")
+    args["mnq_region"] = field
+
     field = data.get("queue")
     args["queue"] = field
 
     return TriggerMnqSqsClientConfig(**args)
 
 
 def unmarshal_TriggerSqsClientConfig(data: Any) -> TriggerSqsClientConfig:
@@ -630,24 +642,28 @@
 
 def marshal_CreateTriggerRequestMnqNatsClientConfig(
     request: CreateTriggerRequestMnqNatsClientConfig,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     return {
         "mnq_namespace_id": request.mnq_namespace_id,
+        "mnq_project_id": request.mnq_project_id,
+        "mnq_region": request.mnq_region,
         "subject": request.subject,
     }
 
 
 def marshal_CreateTriggerRequestMnqSqsClientConfig(
     request: CreateTriggerRequestMnqSqsClientConfig,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     return {
         "mnq_namespace_id": request.mnq_namespace_id,
+        "mnq_project_id": request.mnq_project_id,
+        "mnq_region": request.mnq_region,
         "queue": request.queue,
     }
 
 
 def marshal_CreateTriggerRequestSqsClientConfig(
     request: CreateTriggerRequestSqsClientConfig,
     defaults: ProfileDefaults,
@@ -672,24 +688,28 @@
 
 def marshal_UpdateTriggerRequestMnqNatsClientConfig(
     request: UpdateTriggerRequestMnqNatsClientConfig,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     return {
         "mnq_namespace_id": request.mnq_namespace_id,
+        "mnq_project_id": request.mnq_project_id,
+        "mnq_region": request.mnq_region,
         "subject": request.subject,
     }
 
 
 def marshal_UpdateTriggerRequestMnqSqsClientConfig(
     request: UpdateTriggerRequestMnqSqsClientConfig,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     return {
         "mnq_namespace_id": request.mnq_namespace_id,
+        "mnq_project_id": request.mnq_project_id,
+        "mnq_region": request.mnq_region,
         "queue": request.queue,
     }
 
 
 def marshal_UpdateTriggerRequestSqsClientConfig(
     request: UpdateTriggerRequestSqsClientConfig,
     defaults: ProfileDefaults,
```

### Comparing `scaleway_async-0.8.0/scaleway_async/function/v1beta1/types.py` & `scaleway_async-0.9.0/scaleway_async/function/v1beta1/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,21 +237,29 @@
 
 @dataclass
 class CreateTriggerRequestMnqNatsClientConfig:
     mnq_namespace_id: str
 
     subject: str
 
+    mnq_project_id: str
+
+    mnq_region: str
+
 
 @dataclass
 class CreateTriggerRequestMnqSqsClientConfig:
     mnq_namespace_id: str
 
     queue: str
 
+    mnq_project_id: str
+
+    mnq_region: str
+
 
 @dataclass
 class CreateTriggerRequestSqsClientConfig:
     endpoint: str
 
     queue_url: str
 
@@ -598,21 +606,29 @@
 
 @dataclass
 class TriggerMnqNatsClientConfig:
     mnq_namespace_id: str
 
     subject: str
 
+    mnq_project_id: str
+
+    mnq_region: str
+
 
 @dataclass
 class TriggerMnqSqsClientConfig:
     mnq_namespace_id: str
 
     queue: str
 
+    mnq_project_id: str
+
+    mnq_region: str
+
 
 @dataclass
 class TriggerSqsClientConfig:
     endpoint: str
 
     queue_url: str
 
@@ -623,21 +639,29 @@
 
 @dataclass
 class UpdateTriggerRequestMnqNatsClientConfig:
     mnq_namespace_id: str
 
     subject: str
 
+    mnq_project_id: str
+
+    mnq_region: str
+
 
 @dataclass
 class UpdateTriggerRequestMnqSqsClientConfig:
     mnq_namespace_id: str
 
     queue: str
 
+    mnq_project_id: str
+
+    mnq_region: str
+
 
 @dataclass
 class UpdateTriggerRequestSqsClientConfig:
     endpoint: str
 
     queue_url: str
```

### Comparing `scaleway_async-0.8.0/scaleway_async/iam/v1alpha1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/iam/v1alpha1/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,65 +1,77 @@
 # This file was automatically generated. DO NOT EDIT.
 # If you have any remark or suggestion do not hesitate to open an issue.
 from .types import BearerType
 from .types import ListAPIKeysRequestOrderBy
 from .types import ListApplicationsRequestOrderBy
 from .types import ListGroupsRequestOrderBy
+from .types import ListJWTsRequestOrderBy
 from .types import ListPermissionSetsRequestOrderBy
 from .types import ListPoliciesRequestOrderBy
+from .types import ListQuotaRequestOrderBy
 from .types import ListSSHKeysRequestOrderBy
 from .types import ListUsersRequestOrderBy
 from .types import PermissionSetScopeType
 from .types import UserStatus
 from .types import UserType
 from .types import APIKey
 from .types import Application
 from .types import Group
+from .types import JWT
 from .types import ListAPIKeysResponse
 from .types import ListApplicationsResponse
 from .types import ListGroupsResponse
+from .types import ListJWTsResponse
 from .types import ListPermissionSetsResponse
 from .types import ListPoliciesResponse
+from .types import ListQuotaResponse
 from .types import ListRulesResponse
 from .types import ListSSHKeysResponse
 from .types import ListUsersResponse
 from .types import PermissionSet
 from .types import Policy
+from .types import Quotum
 from .types import Rule
 from .types import RuleSpecs
 from .types import SSHKey
 from .types import SetRulesResponse
 from .types import User
 from .api import IamV1Alpha1API
 
 __all__ = [
     "BearerType",
     "ListAPIKeysRequestOrderBy",
     "ListApplicationsRequestOrderBy",
     "ListGroupsRequestOrderBy",
+    "ListJWTsRequestOrderBy",
     "ListPermissionSetsRequestOrderBy",
     "ListPoliciesRequestOrderBy",
+    "ListQuotaRequestOrderBy",
     "ListSSHKeysRequestOrderBy",
     "ListUsersRequestOrderBy",
     "PermissionSetScopeType",
     "UserStatus",
     "UserType",
     "APIKey",
     "Application",
     "Group",
+    "JWT",
     "ListAPIKeysResponse",
     "ListApplicationsResponse",
     "ListGroupsResponse",
+    "ListJWTsResponse",
     "ListPermissionSetsResponse",
     "ListPoliciesResponse",
+    "ListQuotaResponse",
     "ListRulesResponse",
     "ListSSHKeysResponse",
     "ListUsersResponse",
     "PermissionSet",
     "Policy",
+    "Quotum",
     "Rule",
     "RuleSpecs",
     "SSHKey",
     "SetRulesResponse",
     "User",
     "IamV1Alpha1API",
 ]
```

### Comparing `scaleway_async-0.8.0/scaleway_async/iam/v1alpha1/api.py` & `scaleway_async-0.9.0/scaleway_async/iam/v1alpha1/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,31 +13,37 @@
     validate_path_param,
 )
 from .types import (
     BearerType,
     ListAPIKeysRequestOrderBy,
     ListApplicationsRequestOrderBy,
     ListGroupsRequestOrderBy,
+    ListJWTsRequestOrderBy,
     ListPermissionSetsRequestOrderBy,
     ListPoliciesRequestOrderBy,
+    ListQuotaRequestOrderBy,
     ListSSHKeysRequestOrderBy,
     ListUsersRequestOrderBy,
     APIKey,
     Application,
     Group,
+    JWT,
     ListAPIKeysResponse,
     ListApplicationsResponse,
     ListGroupsResponse,
+    ListJWTsResponse,
     ListPermissionSetsResponse,
     ListPoliciesResponse,
+    ListQuotaResponse,
     ListRulesResponse,
     ListSSHKeysResponse,
     ListUsersResponse,
     PermissionSet,
     Policy,
+    Quotum,
     Rule,
     RuleSpecs,
     SSHKey,
     SetRulesResponse,
     User,
     CreateSSHKeyRequest,
     UpdateSSHKeyRequest,
@@ -68,22 +74,26 @@
     marshal_UpdateApplicationRequest,
     marshal_UpdateGroupRequest,
     marshal_UpdatePolicyRequest,
     marshal_UpdateSSHKeyRequest,
     unmarshal_APIKey,
     unmarshal_Application,
     unmarshal_Group,
+    unmarshal_JWT,
     unmarshal_Policy,
+    unmarshal_Quotum,
     unmarshal_SSHKey,
     unmarshal_User,
     unmarshal_ListAPIKeysResponse,
     unmarshal_ListApplicationsResponse,
     unmarshal_ListGroupsResponse,
+    unmarshal_ListJWTsResponse,
     unmarshal_ListPermissionSetsResponse,
     unmarshal_ListPoliciesResponse,
+    unmarshal_ListQuotaResponse,
     unmarshal_ListRulesResponse,
     unmarshal_ListSSHKeysResponse,
     unmarshal_ListUsersResponse,
     unmarshal_SetRulesResponse,
 )
 
 
@@ -101,21 +111,21 @@
         organization_id: Optional[str] = None,
         name: Optional[str] = None,
         project_id: Optional[str] = None,
         disabled: Optional[bool] = None,
     ) -> ListSSHKeysResponse:
         """
         List SSH keys
-        :param order_by: Sort order of SSH keys
-        :param page: Requested page number. Value must be greater or equals to 1
-        :param page_size: Number of items per page. Value must be between 1 and 100
-        :param organization_id: Filter by organization ID
-        :param name: Name of group to find
-        :param project_id: Filter by project ID
-        :param disabled: Filter out disabled SSH keys or not
+        :param order_by: Sort order of SSH keys.
+        :param page: Requested page number. Value must be greater or equals to 1.
+        :param page_size: Number of items per page. Value must be between 1 and 100.
+        :param organization_id: Filter by organization ID.
+        :param name: Name of group to find.
+        :param project_id: Filter by project ID.
+        :param disabled: Filter out disabled SSH keys or not.
         :return: :class:`ListSSHKeysResponse <ListSSHKeysResponse>`
 
         Usage:
         ::
 
             result = await api.list_ssh_keys()
         """
@@ -147,21 +157,21 @@
         organization_id: Optional[str] = None,
         name: Optional[str] = None,
         project_id: Optional[str] = None,
         disabled: Optional[bool] = None,
     ) -> List[SSHKey]:
         """
         List SSH keys
-        :param order_by: Sort order of SSH keys
-        :param page: Requested page number. Value must be greater or equals to 1
-        :param page_size: Number of items per page. Value must be between 1 and 100
-        :param organization_id: Filter by organization ID
-        :param name: Name of group to find
-        :param project_id: Filter by project ID
-        :param disabled: Filter out disabled SSH keys or not
+        :param order_by: Sort order of SSH keys.
+        :param page: Requested page number. Value must be greater or equals to 1.
+        :param page_size: Number of items per page. Value must be between 1 and 100.
+        :param organization_id: Filter by organization ID.
+        :param name: Name of group to find.
+        :param project_id: Filter by project ID.
+        :param disabled: Filter out disabled SSH keys or not.
         :return: :class:`List[ListSSHKeysResponse] <List[ListSSHKeysResponse]>`
 
         Usage:
         ::
 
             result = await api.list_ssh_keys_all()
         """
@@ -186,17 +196,17 @@
         *,
         public_key: str,
         name: Optional[str] = None,
         project_id: Optional[str] = None,
     ) -> SSHKey:
         """
         Create an SSH key
-        :param name: The name of the SSH key. Max length is 1000
-        :param public_key: SSH public key. Currently ssh-rsa, ssh-dss (DSA), ssh-ed25519 and ecdsa keys with NIST curves are supported. Max length is 65000
-        :param project_id: Project owning the resource
+        :param name: The name of the SSH key. Max length is 1000.
+        :param public_key: SSH public key. Currently ssh-rsa, ssh-dss (DSA), ssh-ed25519 and ecdsa keys with NIST curves are supported. Max length is 65000.
+        :param project_id: Project owning the resource.
         :return: :class:`SSHKey <SSHKey>`
 
         Usage:
         ::
 
             result = await api.create_ssh_key(public_key="example")
         """
@@ -220,15 +230,15 @@
     async def get_ssh_key(
         self,
         *,
         ssh_key_id: str,
     ) -> SSHKey:
         """
         Get an SSH key
-        :param ssh_key_id: The ID of the SSH key
+        :param ssh_key_id: The ID of the SSH key.
         :return: :class:`SSHKey <SSHKey>`
 
         Usage:
         ::
 
             result = await api.get_ssh_key(ssh_key_id="example")
         """
@@ -249,16 +259,16 @@
         ssh_key_id: str,
         name: Optional[str] = None,
         disabled: Optional[bool] = None,
     ) -> SSHKey:
         """
         Update an SSH key
         :param ssh_key_id:
-        :param name: Name of the SSH key. Max length is 1000
-        :param disabled: Enable or disable the SSH key
+        :param name: Name of the SSH key. Max length is 1000.
+        :param disabled: Enable or disable the SSH key.
         :return: :class:`SSHKey <SSHKey>`
 
         Usage:
         ::
 
             result = await api.update_ssh_key(ssh_key_id="example")
         """
@@ -313,19 +323,19 @@
         page_size: Optional[int] = None,
         page: Optional[int] = None,
         organization_id: Optional[str] = None,
         user_ids: Optional[List[str]] = None,
     ) -> ListUsersResponse:
         """
         List users of an organization
-        :param order_by: Criteria for sorting results
-        :param page_size: Number of results per page. Value must be between 1 and 100
-        :param page: Number of page. Value must be greater or equals to 1
-        :param organization_id: ID of organization to filter
-        :param user_ids: Filter out by a list of ID
+        :param order_by: Criteria for sorting results.
+        :param page_size: Number of results per page. Value must be between 1 and 100.
+        :param page: Number of page. Value must be greater or equals to 1.
+        :param organization_id: ID of organization to filter.
+        :param user_ids: Filter out by a list of ID.
         :return: :class:`ListUsersResponse <ListUsersResponse>`
 
         Usage:
         ::
 
             result = await api.list_users()
         """
@@ -353,19 +363,19 @@
         page_size: Optional[int] = None,
         page: Optional[int] = None,
         organization_id: Optional[str] = None,
         user_ids: Optional[List[str]] = None,
     ) -> List[User]:
         """
         List users of an organization
-        :param order_by: Criteria for sorting results
-        :param page_size: Number of results per page. Value must be between 1 and 100
-        :param page: Number of page. Value must be greater or equals to 1
-        :param organization_id: ID of organization to filter
-        :param user_ids: Filter out by a list of ID
+        :param order_by: Criteria for sorting results.
+        :param page_size: Number of results per page. Value must be between 1 and 100.
+        :param page: Number of page. Value must be greater or equals to 1.
+        :param organization_id: ID of organization to filter.
+        :param user_ids: Filter out by a list of ID.
         :return: :class:`List[ListUsersResponse] <List[ListUsersResponse]>`
 
         Usage:
         ::
 
             result = await api.list_users_all()
         """
@@ -386,15 +396,15 @@
     async def get_user(
         self,
         *,
         user_id: str,
     ) -> User:
         """
         Retrieve a user from its ID
-        :param user_id: ID of user to find
+        :param user_id: ID of user to find.
         :return: :class:`User <User>`
 
         Usage:
         ::
 
             result = await api.get_user(user_id="example")
         """
@@ -412,15 +422,15 @@
     async def delete_user(
         self,
         *,
         user_id: str,
     ) -> Optional[None]:
         """
         Delete a guest user from an organization
-        :param user_id: ID of user to delete
+        :param user_id: ID of user to delete.
 
         Usage:
         ::
 
             result = await api.delete_user(user_id="example")
         """
 
@@ -443,21 +453,21 @@
         name: Optional[str] = None,
         organization_id: Optional[str] = None,
         editable: Optional[bool] = None,
         application_ids: Optional[List[str]] = None,
     ) -> ListApplicationsResponse:
         """
         List applications of an organization
-        :param order_by: Criteria for sorting results
-        :param page_size: Number of results per page. Value must be between 1 and 100
-        :param page: Number of page. Value must be greater to 1
-        :param name: Name of application to filter
-        :param organization_id: ID of organization to filter
-        :param editable: Filter out editable applications or not
-        :param application_ids: Filter out by a list of ID
+        :param order_by: Criteria for sorting results.
+        :param page_size: Number of results per page. Value must be between 1 and 100.
+        :param page: Number of page. Value must be greater to 1.
+        :param name: Name of application to filter.
+        :param organization_id: ID of organization to filter.
+        :param editable: Filter out editable applications or not.
+        :param application_ids: Filter out by a list of ID.
         :return: :class:`ListApplicationsResponse <ListApplicationsResponse>`
 
         Usage:
         ::
 
             result = await api.list_applications()
         """
@@ -489,21 +499,21 @@
         name: Optional[str] = None,
         organization_id: Optional[str] = None,
         editable: Optional[bool] = None,
         application_ids: Optional[List[str]] = None,
     ) -> List[Application]:
         """
         List applications of an organization
-        :param order_by: Criteria for sorting results
-        :param page_size: Number of results per page. Value must be between 1 and 100
-        :param page: Number of page. Value must be greater to 1
-        :param name: Name of application to filter
-        :param organization_id: ID of organization to filter
-        :param editable: Filter out editable applications or not
-        :param application_ids: Filter out by a list of ID
+        :param order_by: Criteria for sorting results.
+        :param page_size: Number of results per page. Value must be between 1 and 100.
+        :param page: Number of page. Value must be greater to 1.
+        :param name: Name of application to filter.
+        :param organization_id: ID of organization to filter.
+        :param editable: Filter out editable applications or not.
+        :param application_ids: Filter out by a list of ID.
         :return: :class:`List[ListApplicationsResponse] <List[ListApplicationsResponse]>`
 
         Usage:
         ::
 
             result = await api.list_applications_all()
         """
@@ -528,17 +538,17 @@
         *,
         description: str,
         name: Optional[str] = None,
         organization_id: Optional[str] = None,
     ) -> Application:
         """
         Create a new application
-        :param name: Name of application to create (max length is 64 chars)
-        :param organization_id: ID of organization
-        :param description: Description of application (max length is 200 chars)
+        :param name: Name of application to create (max length is 64 chars).
+        :param organization_id: ID of organization.
+        :param description: Description of application (max length is 200 chars).
         :return: :class:`Application <Application>`
 
         Usage:
         ::
 
             result = await api.create_application(description="example")
         """
@@ -562,15 +572,15 @@
     async def get_application(
         self,
         *,
         application_id: str,
     ) -> Application:
         """
         Get an existing application
-        :param application_id: ID of application to find
+        :param application_id: ID of application to find.
         :return: :class:`Application <Application>`
 
         Usage:
         ::
 
             result = await api.get_application(application_id="example")
         """
@@ -590,17 +600,17 @@
         *,
         application_id: str,
         name: Optional[str] = None,
         description: Optional[str] = None,
     ) -> Application:
         """
         Update an existing application
-        :param application_id: ID of application to update
-        :param name: New name of application (max length is 64 chars)
-        :param description: New description of application (max length is 200 chars)
+        :param application_id: ID of application to update.
+        :param name: New name of application (max length is 64 chars).
+        :param description: New description of application (max length is 200 chars).
         :return: :class:`Application <Application>`
 
         Usage:
         ::
 
             result = await api.update_application(application_id="example")
         """
@@ -626,15 +636,15 @@
     async def delete_application(
         self,
         *,
         application_id: str,
     ) -> Optional[None]:
         """
         Delete an application
-        :param application_id: ID of application to delete
+        :param application_id: ID of application to delete.
 
         Usage:
         ::
 
             result = await api.delete_application(application_id="example")
         """
 
@@ -658,22 +668,22 @@
         name: Optional[str] = None,
         application_ids: Optional[List[str]] = None,
         user_ids: Optional[List[str]] = None,
         group_ids: Optional[List[str]] = None,
     ) -> ListGroupsResponse:
         """
         List groups
-        :param order_by: Sort order of groups
-        :param page: Requested page number. Value must be greater or equals to 1
-        :param page_size: Number of items per page. Value must be between 1 and 100
-        :param organization_id: Filter by organization ID
-        :param name: Name of group to find
-        :param application_ids: Filter out by a list of application ID
-        :param user_ids: Filter out by a list of user ID
-        :param group_ids: Filter out by a list of group ID
+        :param order_by: Sort order of groups.
+        :param page: Requested page number. Value must be greater or equals to 1.
+        :param page_size: Number of items per page. Value must be between 1 and 100.
+        :param organization_id: Filter by organization ID.
+        :param name: Name of group to find.
+        :param application_ids: Filter out by a list of application ID.
+        :param user_ids: Filter out by a list of user ID.
+        :param group_ids: Filter out by a list of group ID.
         :return: :class:`ListGroupsResponse <ListGroupsResponse>`
 
         Usage:
         ::
 
             result = await api.list_groups()
         """
@@ -707,22 +717,22 @@
         name: Optional[str] = None,
         application_ids: Optional[List[str]] = None,
         user_ids: Optional[List[str]] = None,
         group_ids: Optional[List[str]] = None,
     ) -> List[Group]:
         """
         List groups
-        :param order_by: Sort order of groups
-        :param page: Requested page number. Value must be greater or equals to 1
-        :param page_size: Number of items per page. Value must be between 1 and 100
-        :param organization_id: Filter by organization ID
-        :param name: Name of group to find
-        :param application_ids: Filter out by a list of application ID
-        :param user_ids: Filter out by a list of user ID
-        :param group_ids: Filter out by a list of group ID
+        :param order_by: Sort order of groups.
+        :param page: Requested page number. Value must be greater or equals to 1.
+        :param page_size: Number of items per page. Value must be between 1 and 100.
+        :param organization_id: Filter by organization ID.
+        :param name: Name of group to find.
+        :param application_ids: Filter out by a list of application ID.
+        :param user_ids: Filter out by a list of user ID.
+        :param group_ids: Filter out by a list of group ID.
         :return: :class:`List[ListGroupsResponse] <List[ListGroupsResponse]>`
 
         Usage:
         ::
 
             result = await api.list_groups_all()
         """
@@ -748,17 +758,17 @@
         *,
         description: str,
         organization_id: Optional[str] = None,
         name: Optional[str] = None,
     ) -> Group:
         """
         Create a new group
-        :param organization_id: ID of organization linked to the group
-        :param name: Name of the group to create (max length is 64 chars). MUST be unique inside an organization
-        :param description: Description of the group to create (max length is 200 chars)
+        :param organization_id: ID of organization linked to the group.
+        :param name: Name of the group to create (max length is 64 chars). MUST be unique inside an organization.
+        :param description: Description of the group to create (max length is 200 chars).
         :return: :class:`Group <Group>`
 
         Usage:
         ::
 
             result = await api.create_group(description="example")
         """
@@ -782,15 +792,15 @@
     async def get_group(
         self,
         *,
         group_id: str,
     ) -> Group:
         """
         Get a group
-        :param group_id: ID of group
+        :param group_id: ID of group.
         :return: :class:`Group <Group>`
 
         Usage:
         ::
 
             result = await api.get_group(group_id="example")
         """
@@ -810,17 +820,17 @@
         *,
         group_id: str,
         name: Optional[str] = None,
         description: Optional[str] = None,
     ) -> Group:
         """
         Update a group
-        :param group_id: ID of group to update
-        :param name: New name for the group (max length is 64 chars). MUST be unique inside an organization
-        :param description: New description for the group (max length is 200 chars)
+        :param group_id: ID of group to update.
+        :param name: New name for the group (max length is 64 chars). MUST be unique inside an organization.
+        :param description: New description for the group (max length is 200 chars).
         :return: :class:`Group <Group>`
 
         Usage:
         ::
 
             result = await api.update_group(group_id="example")
         """
@@ -890,15 +900,15 @@
         *,
         group_id: str,
         user_id: Optional[str] = None,
         application_id: Optional[str] = None,
     ) -> Group:
         """
         Add a user of an application to a group
-        :param group_id: ID of group
+        :param group_id: ID of group.
         :param user_id: ID of the user to add.
 
         One-of ('member'): at most one of 'user_id', 'application_id' could be set.
         :param application_id: ID of the application to add.
 
         One-of ('member'): at most one of 'user_id', 'application_id' could be set.
         :return: :class:`Group <Group>`
@@ -932,15 +942,15 @@
         *,
         group_id: str,
         user_id: Optional[str] = None,
         application_id: Optional[str] = None,
     ) -> Group:
         """
         Remove a user or an application from a group
-        :param group_id: ID of group
+        :param group_id: ID of group.
         :param user_id: ID of the user to remove.
 
         One-of ('member'): at most one of 'user_id', 'application_id' could be set.
         :param application_id: ID of the application to remove.
 
         One-of ('member'): at most one of 'user_id', 'application_id' could be set.
         :return: :class:`Group <Group>`
@@ -972,15 +982,15 @@
     async def delete_group(
         self,
         *,
         group_id: str,
     ) -> Optional[None]:
         """
         Delete a group
-        :param group_id: ID of group to delete
+        :param group_id: ID of group to delete.
 
         Usage:
         ::
 
             result = await api.delete_group(group_id="example")
         """
 
@@ -1006,24 +1016,24 @@
         group_ids: Optional[List[str]] = None,
         application_ids: Optional[List[str]] = None,
         no_principal: Optional[bool] = None,
         policy_name: Optional[str] = None,
     ) -> ListPoliciesResponse:
         """
         List policies of an organization
-        :param order_by: Criteria for sorting results
-        :param page_size: Number of results per page. Value must be between 1 and 100
-        :param page: Number of page. Value must be greater to 1
-        :param organization_id: ID of organization to filter
-        :param editable: Filter out editable policies or not
-        :param user_ids: Filter out by a list of user ID
-        :param group_ids: Filter out by a list of group ID
-        :param application_ids: Filter out by a list of application ID
-        :param no_principal: True when the policy do not belong to any principal
-        :param policy_name: Name of policy to fetch
+        :param order_by: Criteria for sorting results.
+        :param page_size: Number of results per page. Value must be between 1 and 100.
+        :param page: Number of page. Value must be greater to 1.
+        :param organization_id: ID of organization to filter.
+        :param editable: Filter out editable policies or not.
+        :param user_ids: Filter out by a list of user ID.
+        :param group_ids: Filter out by a list of group ID.
+        :param application_ids: Filter out by a list of application ID.
+        :param no_principal: True when the policy do not belong to any principal.
+        :param policy_name: Name of policy to fetch.
         :return: :class:`ListPoliciesResponse <ListPoliciesResponse>`
 
         Usage:
         ::
 
             result = await api.list_policies()
         """
@@ -1061,24 +1071,24 @@
         group_ids: Optional[List[str]] = None,
         application_ids: Optional[List[str]] = None,
         no_principal: Optional[bool] = None,
         policy_name: Optional[str] = None,
     ) -> List[Policy]:
         """
         List policies of an organization
-        :param order_by: Criteria for sorting results
-        :param page_size: Number of results per page. Value must be between 1 and 100
-        :param page: Number of page. Value must be greater to 1
-        :param organization_id: ID of organization to filter
-        :param editable: Filter out editable policies or not
-        :param user_ids: Filter out by a list of user ID
-        :param group_ids: Filter out by a list of group ID
-        :param application_ids: Filter out by a list of application ID
-        :param no_principal: True when the policy do not belong to any principal
-        :param policy_name: Name of policy to fetch
+        :param order_by: Criteria for sorting results.
+        :param page_size: Number of results per page. Value must be between 1 and 100.
+        :param page: Number of page. Value must be greater to 1.
+        :param organization_id: ID of organization to filter.
+        :param editable: Filter out editable policies or not.
+        :param user_ids: Filter out by a list of user ID.
+        :param group_ids: Filter out by a list of group ID.
+        :param application_ids: Filter out by a list of application ID.
+        :param no_principal: True when the policy do not belong to any principal.
+        :param policy_name: Name of policy to fetch.
         :return: :class:`List[ListPoliciesResponse] <List[ListPoliciesResponse]>`
 
         Usage:
         ::
 
             result = await api.list_policies_all()
         """
@@ -1111,18 +1121,18 @@
         user_id: Optional[str] = None,
         group_id: Optional[str] = None,
         application_id: Optional[str] = None,
         no_principal: Optional[bool] = None,
     ) -> Policy:
         """
         Create a new policy
-        :param name: Name of policy to create (max length is 64 chars)
-        :param description: Description of policy to create (max length is 200 chars)
-        :param organization_id: ID of organization
-        :param rules: Rules of the policy to create
+        :param name: Name of policy to create (max length is 64 chars).
+        :param description: Description of policy to create (max length is 200 chars).
+        :param organization_id: ID of organization.
+        :param rules: Rules of the policy to create.
         :param user_id: ID of user, owner of the policy.
 
         One-of ('principal'): at most one of 'user_id', 'group_id', 'application_id', 'no_principal' could be set.
         :param group_id: ID of group, owner of the policy.
 
         One-of ('principal'): at most one of 'user_id', 'group_id', 'application_id', 'no_principal' could be set.
         :param application_id: ID of application, owner of the policy.
@@ -1163,15 +1173,15 @@
     async def get_policy(
         self,
         *,
         policy_id: str,
     ) -> Policy:
         """
         Get an existing policy
-        :param policy_id: Id of policy to search
+        :param policy_id: Id of policy to search.
         :return: :class:`Policy <Policy>`
 
         Usage:
         ::
 
             result = await api.get_policy(policy_id="example")
         """
@@ -1195,17 +1205,17 @@
         user_id: Optional[str] = None,
         group_id: Optional[str] = None,
         application_id: Optional[str] = None,
         no_principal: Optional[bool] = None,
     ) -> Policy:
         """
         Update an existing policy
-        :param policy_id: Id of policy to update
-        :param name: New name of policy (max length is 64 chars)
-        :param description: New description of policy (max length is 200 chars)
+        :param policy_id: Id of policy to update.
+        :param name: New name of policy (max length is 64 chars).
+        :param description: New description of policy (max length is 200 chars).
         :param user_id: New ID of user, owner of the policy.
 
         One-of ('principal'): at most one of 'user_id', 'group_id', 'application_id', 'no_principal' could be set.
         :param group_id: New ID of group, owner of the policy.
 
         One-of ('principal'): at most one of 'user_id', 'group_id', 'application_id', 'no_principal' could be set.
         :param application_id: New ID of application, owner of the policy.
@@ -1247,15 +1257,15 @@
     async def delete_policy(
         self,
         *,
         policy_id: str,
     ) -> Optional[None]:
         """
         Delete a policy
-        :param policy_id: Id of policy to delete
+        :param policy_id: Id of policy to delete.
 
         Usage:
         ::
 
             result = await api.delete_policy(policy_id="example")
         """
 
@@ -1296,16 +1306,16 @@
         self,
         *,
         policy_id: str,
         rules: List[RuleSpecs],
     ) -> SetRulesResponse:
         """
         Set rules of an existing policy
-        :param policy_id: Id of policy to update
-        :param rules: Rules of the policy to set
+        :param policy_id: Id of policy to update.
+        :param rules: Rules of the policy to set.
         :return: :class:`SetRulesResponse <SetRulesResponse>`
 
         Usage:
         ::
 
             result = await api.set_rules(
                 policy_id="example",
@@ -1333,17 +1343,17 @@
         *,
         policy_id: str,
         page_size: Optional[int] = None,
         page: Optional[int] = None,
     ) -> ListRulesResponse:
         """
         List rules of an existing policy
-        :param policy_id: Id of policy to search
-        :param page_size: Number of results per page. Value must be between 1 and 100
-        :param page: Number of page. Value must be greater to 1
+        :param policy_id: Id of policy to search.
+        :param page_size: Number of results per page. Value must be between 1 and 100.
+        :param page: Number of page. Value must be greater to 1.
         :return: :class:`ListRulesResponse <ListRulesResponse>`
 
         Usage:
         ::
 
             result = await api.list_rules(policy_id="example")
         """
@@ -1366,17 +1376,17 @@
         *,
         policy_id: str,
         page_size: Optional[int] = None,
         page: Optional[int] = None,
     ) -> List[Rule]:
         """
         List rules of an existing policy
-        :param policy_id: Id of policy to search
-        :param page_size: Number of results per page. Value must be between 1 and 100
-        :param page: Number of page. Value must be greater to 1
+        :param policy_id: Id of policy to search.
+        :param page_size: Number of results per page. Value must be between 1 and 100.
+        :param page: Number of page. Value must be greater to 1.
         :return: :class:`List[ListRulesResponse] <List[ListRulesResponse]>`
 
         Usage:
         ::
 
             result = await api.list_rules_all(policy_id="example")
         """
@@ -1398,18 +1408,18 @@
         order_by: ListPermissionSetsRequestOrderBy = ListPermissionSetsRequestOrderBy.NAME_ASC,
         page_size: Optional[int] = None,
         page: Optional[int] = None,
         organization_id: Optional[str] = None,
     ) -> ListPermissionSetsResponse:
         """
         List permission sets
-        :param order_by: Criteria for sorting results
-        :param page_size: Number of results per page. Value must be between 1 and 100
-        :param page: Number of page. Value must be greater to 1
-        :param organization_id: Filter by organization ID
+        :param order_by: Criteria for sorting results.
+        :param page_size: Number of results per page. Value must be between 1 and 100.
+        :param page: Number of page. Value must be greater to 1.
+        :param organization_id: Filter by organization ID.
         :return: :class:`ListPermissionSetsResponse <ListPermissionSetsResponse>`
 
         Usage:
         ::
 
             result = await api.list_permission_sets()
         """
@@ -1435,18 +1445,18 @@
         order_by: Optional[ListPermissionSetsRequestOrderBy] = None,
         page_size: Optional[int] = None,
         page: Optional[int] = None,
         organization_id: Optional[str] = None,
     ) -> List[PermissionSet]:
         """
         List permission sets
-        :param order_by: Criteria for sorting results
-        :param page_size: Number of results per page. Value must be between 1 and 100
-        :param page: Number of page. Value must be greater to 1
-        :param organization_id: Filter by organization ID
+        :param order_by: Criteria for sorting results.
+        :param page_size: Number of results per page. Value must be between 1 and 100.
+        :param page: Number of page. Value must be greater to 1.
+        :param organization_id: Filter by organization ID.
         :return: :class:`List[ListPermissionSetsResponse] <List[ListPermissionSetsResponse]>`
 
         Usage:
         ::
 
             result = await api.list_permission_sets_all()
         """
@@ -1477,30 +1487,30 @@
         access_key: Optional[str] = None,
         description: Optional[str] = None,
         bearer_id: Optional[str] = None,
         bearer_type: BearerType = BearerType.UNKNOWN_BEARER_TYPE,
     ) -> ListAPIKeysResponse:
         """
         List API keys
-        :param order_by: Criteria for sorting results
-        :param page: Number of page. Value must be greater or equals to 1
-        :param page_size: Number of results per page. Value must be between 1 and 100
-        :param organization_id: ID of organization
+        :param order_by: Criteria for sorting results.
+        :param page: Number of page. Value must be greater or equals to 1.
+        :param page_size: Number of results per page. Value must be between 1 and 100.
+        :param organization_id: ID of organization.
         :param application_id: ID of an application bearer.
 
         One-of ('bearer'): at most one of 'application_id', 'user_id' could be set.
         :param user_id: ID of a user bearer.
 
         One-of ('bearer'): at most one of 'application_id', 'user_id' could be set.
-        :param editable: Filter out editable API keys or not
-        :param expired: Filter out expired API keys or not
-        :param access_key: Filter out by access key
-        :param description: Filter out by description
-        :param bearer_id: Filter out by bearer ID
-        :param bearer_type: Filter out by type of bearer
+        :param editable: Filter out editable API keys or not.
+        :param expired: Filter out expired API keys or not.
+        :param access_key: Filter out by access key.
+        :param description: Filter out by description.
+        :param bearer_id: Filter out by bearer ID.
+        :param bearer_type: Filter out by type of bearer.
         :return: :class:`ListAPIKeysResponse <ListAPIKeysResponse>`
 
         Usage:
         ::
 
             result = await api.list_api_keys()
         """
@@ -1546,30 +1556,30 @@
         access_key: Optional[str] = None,
         description: Optional[str] = None,
         bearer_id: Optional[str] = None,
         bearer_type: Optional[BearerType] = None,
     ) -> List[APIKey]:
         """
         List API keys
-        :param order_by: Criteria for sorting results
-        :param page: Number of page. Value must be greater or equals to 1
-        :param page_size: Number of results per page. Value must be between 1 and 100
-        :param organization_id: ID of organization
+        :param order_by: Criteria for sorting results.
+        :param page: Number of page. Value must be greater or equals to 1.
+        :param page_size: Number of results per page. Value must be between 1 and 100.
+        :param organization_id: ID of organization.
         :param application_id: ID of an application bearer.
 
         One-of ('bearer'): at most one of 'application_id', 'user_id' could be set.
         :param user_id: ID of a user bearer.
 
         One-of ('bearer'): at most one of 'application_id', 'user_id' could be set.
-        :param editable: Filter out editable API keys or not
-        :param expired: Filter out expired API keys or not
-        :param access_key: Filter out by access key
-        :param description: Filter out by description
-        :param bearer_id: Filter out by bearer ID
-        :param bearer_type: Filter out by type of bearer
+        :param editable: Filter out editable API keys or not.
+        :param expired: Filter out expired API keys or not.
+        :param access_key: Filter out by access key.
+        :param description: Filter out by description.
+        :param bearer_id: Filter out by bearer ID.
+        :param bearer_type: Filter out by type of bearer.
         :return: :class:`List[ListAPIKeysResponse] <List[ListAPIKeysResponse]>`
 
         Usage:
         ::
 
             result = await api.list_api_keys_all()
         """
@@ -1607,17 +1617,17 @@
         Create an API key
         :param application_id: ID of application principal.
 
         One-of ('bearer'): at most one of 'application_id', 'user_id' could be set.
         :param user_id: ID of user principal.
 
         One-of ('bearer'): at most one of 'application_id', 'user_id' could be set.
-        :param expires_at: Expiration date of the API key
-        :param default_project_id: The default project ID to use with object storage
-        :param description: The description of the API key (max length is 200 chars)
+        :param expires_at: Expiration date of the API key.
+        :param default_project_id: The default project ID to use with object storage.
+        :param description: The description of the API key (max length is 200 chars).
         :return: :class:`APIKey <APIKey>`
 
         Usage:
         ::
 
             result = await api.create_api_key(description="example")
         """
@@ -1643,15 +1653,15 @@
     async def get_api_key(
         self,
         *,
         access_key: str,
     ) -> APIKey:
         """
         Get an API key
-        :param access_key: Access key to search for
+        :param access_key: Access key to search for.
         :return: :class:`APIKey <APIKey>`
 
         Usage:
         ::
 
             result = await api.get_api_key(access_key="example")
         """
@@ -1671,17 +1681,17 @@
         *,
         access_key: str,
         default_project_id: Optional[str] = None,
         description: Optional[str] = None,
     ) -> APIKey:
         """
         Update an API key
-        :param access_key: Access key to update
-        :param default_project_id: The new default project ID to set
-        :param description: The new description to update
+        :param access_key: Access key to update.
+        :param default_project_id: The new default project ID to set.
+        :param description: The new description to update.
         :return: :class:`APIKey <APIKey>`
 
         Usage:
         ::
 
             result = await api.update_api_key(access_key="example")
         """
@@ -1707,15 +1717,15 @@
     async def delete_api_key(
         self,
         *,
         access_key: str,
     ) -> Optional[None]:
         """
         Delete an API key
-        :param access_key: Access key to delete
+        :param access_key: Access key to delete.
 
         Usage:
         ::
 
             result = await api.delete_api_key(access_key="example")
         """
 
@@ -1724,7 +1734,237 @@
         res = self._request(
             "DELETE",
             f"/iam/v1alpha1/api-keys/{param_access_key}",
         )
 
         self._throw_on_error(res)
         return None
+
+    async def list_quota(
+        self,
+        *,
+        order_by: ListQuotaRequestOrderBy = ListQuotaRequestOrderBy.NAME_ASC,
+        page_size: Optional[int] = None,
+        page: Optional[int] = None,
+        organization_id: Optional[str] = None,
+    ) -> ListQuotaResponse:
+        """
+        List all quota in the organization with the associated limit
+        :param order_by: Criteria for sorting results.
+        :param page_size: Number of results per page. Value must be between 1 and 100.
+        :param page: Number of page. Value must be greater to 1.
+        :param organization_id: Filter by organization ID.
+        :return: :class:`ListQuotaResponse <ListQuotaResponse>`
+
+        Usage:
+        ::
+
+            result = await api.list_quota()
+        """
+
+        res = self._request(
+            "GET",
+            f"/iam/v1alpha1/quota",
+            params={
+                "order_by": order_by,
+                "organization_id": organization_id
+                or self.client.default_organization_id,
+                "page": page,
+                "page_size": page_size or self.client.default_page_size,
+            },
+        )
+
+        self._throw_on_error(res)
+        return unmarshal_ListQuotaResponse(res.json())
+
+    async def list_quota_all(
+        self,
+        *,
+        order_by: Optional[ListQuotaRequestOrderBy] = None,
+        page_size: Optional[int] = None,
+        page: Optional[int] = None,
+        organization_id: Optional[str] = None,
+    ) -> List[Quotum]:
+        """
+        List all quota in the organization with the associated limit
+        :param order_by: Criteria for sorting results.
+        :param page_size: Number of results per page. Value must be between 1 and 100.
+        :param page: Number of page. Value must be greater to 1.
+        :param organization_id: Filter by organization ID.
+        :return: :class:`List[ListQuotaResponse] <List[ListQuotaResponse]>`
+
+        Usage:
+        ::
+
+            result = await api.list_quota_all()
+        """
+
+        return await fetch_all_pages_async(
+            type=ListQuotaResponse,
+            key="quota",
+            fetcher=self.list_quota,
+            args={
+                "order_by": order_by,
+                "page_size": page_size,
+                "page": page,
+                "organization_id": organization_id,
+            },
+        )
+
+    async def get_quotum(
+        self,
+        *,
+        quotum_name: str,
+        organization_id: Optional[str] = None,
+    ) -> Quotum:
+        """
+        Get a quotum in the organization with the associated limit
+        :param quotum_name: Name of the quotum to get.
+        :param organization_id: ID of the organization.
+        :return: :class:`Quotum <Quotum>`
+
+        Usage:
+        ::
+
+            result = await api.get_quotum(quotum_name="example")
+        """
+
+        param_quotum_name = validate_path_param("quotum_name", quotum_name)
+
+        res = self._request(
+            "GET",
+            f"/iam/v1alpha1/quota/{param_quotum_name}",
+            params={
+                "organization_id": organization_id
+                or self.client.default_organization_id,
+            },
+        )
+
+        self._throw_on_error(res)
+        return unmarshal_Quotum(res.json())
+
+    async def list_jw_ts(
+        self,
+        *,
+        audience_id: str,
+        order_by: ListJWTsRequestOrderBy = ListJWTsRequestOrderBy.CREATED_AT_ASC,
+        page_size: Optional[int] = None,
+        page: Optional[int] = None,
+        expired: Optional[bool] = None,
+    ) -> ListJWTsResponse:
+        """
+        List JWTs
+        :param order_by: Criteria for sorting results.
+        :param audience_id: ID of the user to search.
+        :param page_size: Number of results per page. Value must be between 1 and 100.
+        :param page: Number of page. Value must be greater to 1.
+        :param expired: Filter out expired JWTs or not.
+        :return: :class:`ListJWTsResponse <ListJWTsResponse>`
+
+        Usage:
+        ::
+
+            result = await api.list_jw_ts(audience_id="example")
+        """
+
+        res = self._request(
+            "GET",
+            f"/iam/v1alpha1/jwts",
+            params={
+                "audience_id": audience_id,
+                "expired": expired,
+                "order_by": order_by,
+                "page": page,
+                "page_size": page_size or self.client.default_page_size,
+            },
+        )
+
+        self._throw_on_error(res)
+        return unmarshal_ListJWTsResponse(res.json())
+
+    async def list_jw_ts_all(
+        self,
+        *,
+        audience_id: str,
+        order_by: Optional[ListJWTsRequestOrderBy] = None,
+        page_size: Optional[int] = None,
+        page: Optional[int] = None,
+        expired: Optional[bool] = None,
+    ) -> List[JWT]:
+        """
+        List JWTs
+        :param order_by: Criteria for sorting results.
+        :param audience_id: ID of the user to search.
+        :param page_size: Number of results per page. Value must be between 1 and 100.
+        :param page: Number of page. Value must be greater to 1.
+        :param expired: Filter out expired JWTs or not.
+        :return: :class:`List[ListJWTsResponse] <List[ListJWTsResponse]>`
+
+        Usage:
+        ::
+
+            result = await api.list_jw_ts_all(audience_id="example")
+        """
+
+        return await fetch_all_pages_async(
+            type=ListJWTsResponse,
+            key="jwts",
+            fetcher=self.list_jw_ts,
+            args={
+                "audience_id": audience_id,
+                "order_by": order_by,
+                "page_size": page_size,
+                "page": page,
+                "expired": expired,
+            },
+        )
+
+    async def get_jwt(
+        self,
+        *,
+        jti: str,
+    ) -> JWT:
+        """
+        Get a JWT
+        :param jti: JWT ID of the JWT to get.
+        :return: :class:`JWT <JWT>`
+
+        Usage:
+        ::
+
+            result = await api.get_jwt(jti="example")
+        """
+
+        param_jti = validate_path_param("jti", jti)
+
+        res = self._request(
+            "GET",
+            f"/iam/v1alpha1/jwts/{param_jti}",
+        )
+
+        self._throw_on_error(res)
+        return unmarshal_JWT(res.json())
+
+    async def delete_jwt(
+        self,
+        *,
+        jti: str,
+    ) -> Optional[None]:
+        """
+        Delete a JWT
+        :param jti: JWT ID of the JWT to delete.
+
+        Usage:
+        ::
+
+            result = await api.delete_jwt(jti="example")
+        """
+
+        param_jti = validate_path_param("jti", jti)
+
+        res = self._request(
+            "DELETE",
+            f"/iam/v1alpha1/jwts/{param_jti}",
+        )
+
+        self._throw_on_error(res)
+        return None
```

### Comparing `scaleway_async-0.8.0/scaleway_async/iam/v1alpha1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/iam/v1alpha1/marshalling.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,24 +9,28 @@
     resolve_one_of,
 )
 from dateutil import parser
 from .types import (
     APIKey,
     Application,
     Group,
+    JWT,
     ListAPIKeysResponse,
     ListApplicationsResponse,
     ListGroupsResponse,
+    ListJWTsResponse,
     ListPermissionSetsResponse,
     ListPoliciesResponse,
+    ListQuotaResponse,
     ListRulesResponse,
     ListSSHKeysResponse,
     ListUsersResponse,
     PermissionSet,
     Policy,
+    Quotum,
     Rule,
     RuleSpecs,
     SSHKey,
     SetRulesResponse,
     User,
     CreateSSHKeyRequest,
     UpdateSSHKeyRequest,
@@ -155,14 +159,49 @@
 
     field = data.get("user_ids")
     args["user_ids"] = field
 
     return Group(**args)
 
 
+def unmarshal_JWT(data: Any) -> JWT:
+    if type(data) is not dict:
+        raise TypeError(
+            f"Unmarshalling the type 'JWT' failed as data isn't a dictionary."
+        )
+
+    args: Dict[str, Any] = {}
+
+    field = data.get("audience_id")
+    args["audience_id"] = field
+
+    field = data.get("created_at")
+    args["created_at"] = parser.isoparse(field) if type(field) is str else field
+
+    field = data.get("expires_at")
+    args["expires_at"] = parser.isoparse(field) if type(field) is str else field
+
+    field = data.get("ip")
+    args["ip"] = field
+
+    field = data.get("issuer_id")
+    args["issuer_id"] = field
+
+    field = data.get("jti")
+    args["jti"] = field
+
+    field = data.get("updated_at")
+    args["updated_at"] = parser.isoparse(field) if type(field) is str else field
+
+    field = data.get("user_agent")
+    args["user_agent"] = field
+
+    return JWT(**args)
+
+
 def unmarshal_PermissionSet(data: Any) -> PermissionSet:
     if type(data) is not dict:
         raise TypeError(
             f"Unmarshalling the type 'PermissionSet' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
@@ -234,14 +273,34 @@
 
     field = data.get("user_id")
     args["user_id"] = field
 
     return Policy(**args)
 
 
+def unmarshal_Quotum(data: Any) -> Quotum:
+    if type(data) is not dict:
+        raise TypeError(
+            f"Unmarshalling the type 'Quotum' failed as data isn't a dictionary."
+        )
+
+    args: Dict[str, Any] = {}
+
+    field = data.get("limit")
+    args["limit"] = field
+
+    field = data.get("name")
+    args["name"] = field
+
+    field = data.get("unlimited")
+    args["unlimited"] = field
+
+    return Quotum(**args)
+
+
 def unmarshal_Rule(data: Any) -> Rule:
     if type(data) is not dict:
         raise TypeError(
             f"Unmarshalling the type 'Rule' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
@@ -393,14 +452,31 @@
 
     field = data.get("total_count")
     args["total_count"] = field
 
     return ListGroupsResponse(**args)
 
 
+def unmarshal_ListJWTsResponse(data: Any) -> ListJWTsResponse:
+    if type(data) is not dict:
+        raise TypeError(
+            f"Unmarshalling the type 'ListJWTsResponse' failed as data isn't a dictionary."
+        )
+
+    args: Dict[str, Any] = {}
+
+    field = data.get("jwts")
+    args["jwts"] = [unmarshal_JWT(v) for v in data["jwts"]]
+
+    field = data.get("total_count")
+    args["total_count"] = field
+
+    return ListJWTsResponse(**args)
+
+
 def unmarshal_ListPermissionSetsResponse(data: Any) -> ListPermissionSetsResponse:
     if type(data) is not dict:
         raise TypeError(
             f"Unmarshalling the type 'ListPermissionSetsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
@@ -429,14 +505,31 @@
 
     field = data.get("total_count")
     args["total_count"] = field
 
     return ListPoliciesResponse(**args)
 
 
+def unmarshal_ListQuotaResponse(data: Any) -> ListQuotaResponse:
+    if type(data) is not dict:
+        raise TypeError(
+            f"Unmarshalling the type 'ListQuotaResponse' failed as data isn't a dictionary."
+        )
+
+    args: Dict[str, Any] = {}
+
+    field = data.get("quota")
+    args["quota"] = [unmarshal_Quotum(v) for v in data["quota"]]
+
+    field = data.get("total_count")
+    args["total_count"] = field
+
+    return ListQuotaResponse(**args)
+
+
 def unmarshal_ListRulesResponse(data: Any) -> ListRulesResponse:
     if type(data) is not dict:
         raise TypeError(
             f"Unmarshalling the type 'ListRulesResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
```

### Comparing `scaleway_async-0.8.0/scaleway_async/iam/v1alpha1/types.py` & `scaleway_async-0.9.0/scaleway_async/iam/v1alpha1/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,24 @@
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
+class ListJWTsRequestOrderBy(str, Enum):
+    CREATED_AT_ASC = "created_at_asc"
+    CREATED_AT_DESC = "created_at_desc"
+    UPDATED_AT_ASC = "updated_at_asc"
+    UPDATED_AT_DESC = "updated_at_desc"
+
+    def __str__(self) -> str:
+        return str(self.value)
+
+
 class ListPermissionSetsRequestOrderBy(str, Enum):
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
@@ -71,14 +81,22 @@
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
+class ListQuotaRequestOrderBy(str, Enum):
+    NAME_ASC = "name_asc"
+    NAME_DESC = "name_desc"
+
+    def __str__(self) -> str:
+        return str(self.value)
+
+
 class ListSSHKeysRequestOrderBy(str, Enum):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     UPDATED_AT_ASC = "updated_at_asc"
     UPDATED_AT_DESC = "updated_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
@@ -128,25 +146,25 @@
     def __str__(self) -> str:
         return str(self.value)
 
 
 @dataclass
 class APIKey:
     """
-    Api key
+    Api key.
     """
 
     access_key: str
     """
-    Access key of API key
+    Access key of API key.
     """
 
     secret_key: Optional[str]
     """
-    Secret key of API Key
+    Secret key of API Key.
     """
 
     application_id: Optional[str]
     """
     ID of application bearer.
     
     One-of ('bearer'): at most one of 'application_id', 'user_id' could be set.
@@ -157,364 +175,435 @@
     ID of user bearer.
     
     One-of ('bearer'): at most one of 'application_id', 'user_id' could be set.
     """
 
     description: str
     """
-    Description of API key
+    Description of API key.
     """
 
     created_at: Optional[datetime]
     """
-    Creation date and time of API key
+    Creation date and time of API key.
     """
 
     updated_at: Optional[datetime]
     """
-    Last update date and time of API key
+    Last update date and time of API key.
     """
 
     expires_at: Optional[datetime]
     """
-    Expiration date and time of API key
+    Expiration date and time of API key.
     """
 
     default_project_id: str
     """
-    The default project ID specified for this API key
+    The default project ID specified for this API key.
     """
 
     editable: bool
     """
-    Whether or not the API key is editable
+    Whether or not the API key is editable.
     """
 
     creation_ip: str
     """
-    IP Address of the device which created the API key
+    IP Address of the device which created the API key.
     """
 
 
 @dataclass
 class Application:
     """
-    Application
+    Application.
     """
 
     id: str
     """
-    ID of application
+    ID of application.
     """
 
     name: str
     """
-    Name of application
+    Name of application.
     """
 
     description: str
     """
-    Description of the application
+    Description of the application.
     """
 
     created_at: Optional[datetime]
     """
-    Creation date of application
+    Creation date of application.
     """
 
     updated_at: Optional[datetime]
     """
-    Last update date of application
+    Last update date of application.
     """
 
     organization_id: str
     """
-    ID of organization
+    ID of organization.
     """
 
     editable: bool
     """
-    Whether or not the application is editable
+    Whether or not the application is editable.
     """
 
     nb_api_keys: int
     """
-    Number of API keys owned by the application
+    Number of API keys owned by the application.
     """
 
 
 @dataclass
 class Group:
     """
-    Group
+    Group.
     """
 
     id: str
     """
-    ID of group
+    ID of group.
     """
 
     created_at: Optional[datetime]
     """
-    Creation date and time of group
+    Creation date and time of group.
     """
 
     updated_at: Optional[datetime]
     """
-    Last update date and time of group
+    Last update date and time of group.
     """
 
     organization_id: str
     """
-    ID of organization linked to the group
+    ID of organization linked to the group.
     """
 
     name: str
     """
-    Name of group
+    Name of group.
     """
 
     description: str
     """
-    Description of the group
+    Description of the group.
     """
 
     user_ids: List[str]
     """
-    IDs of users attached to this group
+    IDs of users attached to this group.
     """
 
     application_ids: List[str]
     """
-    IDs of applications attached to this group
+    IDs of applications attached to this group.
+    """
+
+
+@dataclass
+class JWT:
+    """
+    Jwt.
+    """
+
+    jti: str
+    """
+    JWT ID.
+    """
+
+    issuer_id: str
+    """
+    ID of the user who issued the JWT.
+    """
+
+    audience_id: str
+    """
+    ID of the user targeted by the JWT.
+    """
+
+    created_at: Optional[datetime]
+    """
+    Creation date of the JWT.
+    """
+
+    updated_at: Optional[datetime]
+    """
+    Last update date of the JWT.
+    """
+
+    expires_at: Optional[datetime]
+    """
+    Expiration date of the JWT.
+    """
+
+    ip: str
+    """
+    IP address used during the creation of the JWT.
+    """
+
+    user_agent: str
+    """
+    User-agent used during the creation of the JWT.
     """
 
 
 @dataclass
 class ListAPIKeysResponse:
     """
-    List api keys response
+    List api keys response.
     """
 
     api_keys: List[APIKey]
     """
-    List of API keys
+    List of API keys.
     """
 
     total_count: int
     """
-    Total count of API Keys
+    Total count of API Keys.
     """
 
 
 @dataclass
 class ListApplicationsResponse:
     """
-    List applications response
+    List applications response.
     """
 
     applications: List[Application]
     """
-    List of applications
+    List of applications.
     """
 
     total_count: int
     """
-    Total count of applications
+    Total count of applications.
     """
 
 
 @dataclass
 class ListGroupsResponse:
     """
-    List groups response
+    List groups response.
     """
 
     groups: List[Group]
     """
-    List of groups
+    List of groups.
     """
 
     total_count: int
     """
-    Total count of groups
+    Total count of groups.
     """
 
 
 @dataclass
+class ListJWTsResponse:
+    jwts: List[JWT]
+
+    total_count: int
+
+
+@dataclass
 class ListPermissionSetsResponse:
     """
-    List permission sets response
+    List permission sets response.
     """
 
     permission_sets: List[PermissionSet]
     """
-    List of permission sets
+    List of permission sets.
     """
 
     total_count: int
     """
-    Total count of permission sets
+    Total count of permission sets.
     """
 
 
 @dataclass
 class ListPoliciesResponse:
     """
-    List policies response
+    List policies response.
     """
 
     policies: List[Policy]
     """
-    List of policies
+    List of policies.
     """
 
     total_count: int
     """
-    Total count of policies
+    Total count of policies.
+    """
+
+
+@dataclass
+class ListQuotaResponse:
+    """
+    List quota response.
+    """
+
+    quota: List[Quotum]
+    """
+    List of quota.
+    """
+
+    total_count: int
+    """
+    Total count of quota.
     """
 
 
 @dataclass
 class ListRulesResponse:
     """
-    List rules response
+    List rules response.
     """
 
     rules: List[Rule]
     """
-    Rules of the policy
+    Rules of the policy.
     """
 
     total_count: int
     """
-    Total count of rules
+    Total count of rules.
     """
 
 
 @dataclass
 class ListSSHKeysResponse:
     """
-    List ssh keys response
+    List ssh keys response.
     """
 
     ssh_keys: List[SSHKey]
     """
-    List of SSH keys
+    List of SSH keys.
     """
 
     total_count: int
     """
-    Total count of SSH keys
+    Total count of SSH keys.
     """
 
 
 @dataclass
 class ListUsersResponse:
     """
-    List users response
+    List users response.
     """
 
     users: List[User]
     """
-    List of users
+    List of users.
     """
 
     total_count: int
     """
-    Total count of users
+    Total count of users.
     """
 
 
 @dataclass
 class PermissionSet:
     """
-    Permission set
+    Permission set.
     """
 
     id: str
     """
-    Id of permission set
+    Id of permission set.
     """
 
     name: str
     """
-    Name of permission set
+    Name of permission set.
     """
 
     scope_type: PermissionSetScopeType
     """
-    Scope of permission set
+    Scope of permission set.
     """
 
     description: str
     """
-    Description of permission set
+    Description of permission set.
     """
 
     categories: Optional[List[str]]
     """
-    Categories of permission set
+    Categories of permission set.
     """
 
 
 @dataclass
 class Policy:
     """
-    Policy
+    Policy.
     """
 
     id: str
     """
-    Id of policy
+    Id of policy.
     """
 
     name: str
     """
-    Name of policy
+    Name of policy.
     """
 
     description: str
     """
-    Description of policy
+    Description of policy.
     """
 
     organization_id: str
     """
-    Organization ID of policy
+    Organization ID of policy.
     """
 
     created_at: Optional[datetime]
     """
-    Creation date and time of policy
+    Creation date and time of policy.
     """
 
     updated_at: Optional[datetime]
     """
-    Last update date and time of policy
+    Last update date and time of policy.
     """
 
     editable: bool
     """
-    Editable status of policy
+    Editable status of policy.
     """
 
     nb_rules: int
     """
-    Number of rules of policy
+    Number of rules of policy.
     """
 
     nb_scopes: int
     """
-    Number of scopes of policy
+    Number of scopes of policy.
     """
 
     nb_permission_sets: int
     """
-    Number of permission sets of policy
+    Number of permission sets of policy.
     """
 
     user_id: Optional[str]
     """
     ID of user, owner of the policy.
     
     One-of ('principal'): at most one of 'user_id', 'group_id', 'application_id', 'no_principal' could be set.
@@ -539,32 +628,58 @@
     True when the policy do not belong to any principal.
     
     One-of ('principal'): at most one of 'user_id', 'group_id', 'application_id', 'no_principal' could be set.
     """
 
 
 @dataclass
+class Quotum:
+    """
+    Quotum.
+    """
+
+    name: str
+    """
+    Name of the quotum.
+    """
+
+    limit: Optional[int]
+    """
+    Max limit of the quotum.
+    
+    One-of ('value'): at most one of 'limit', 'unlimited' could be set.
+    """
+
+    unlimited: Optional[bool]
+    """
+    Whether the quotum is unlimited or not.
+    
+    One-of ('value'): at most one of 'limit', 'unlimited' could be set.
+    """
+
+
+@dataclass
 class Rule:
     """
-    Rule
+    Rule.
     """
 
     id: str
     """
-    Id of rule
+    Id of rule.
     """
 
     permission_set_names: Optional[List[str]]
     """
-    Names of permission sets bound to the rule
+    Names of permission sets bound to the rule.
     """
 
     permission_sets_scope_type: PermissionSetScopeType
     """
-    Permission_set_names have the same scope_type
+    Permission_set_names have the same scope_type.
     """
 
     project_ids: Optional[List[str]]
     """
     List of project IDs scoped to the rule.
     
     One-of ('scope'): at most one of 'project_ids', 'organization_id', 'account_root_user_id' could be set.
@@ -584,20 +699,20 @@
     One-of ('scope'): at most one of 'project_ids', 'organization_id', 'account_root_user_id' could be set.
     """
 
 
 @dataclass
 class RuleSpecs:
     """
-    Rule specs
+    Rule specs.
     """
 
     permission_set_names: Optional[List[str]]
     """
-    Names of permission sets bound to the rule
+    Names of permission sets bound to the rule.
     """
 
     project_ids: Optional[List[str]]
     """
     List of project IDs scoped to the rule.
     
     One-of ('scope'): at most one of 'project_ids', 'organization_id' could be set.
@@ -610,434 +725,434 @@
     One-of ('scope'): at most one of 'project_ids', 'organization_id' could be set.
     """
 
 
 @dataclass
 class SSHKey:
     """
-    Ssh key
+    Ssh key.
     """
 
     id: str
     """
-    ID of SSH key
+    ID of SSH key.
     """
 
     name: str
     """
-    Name of SSH key
+    Name of SSH key.
     """
 
     public_key: str
     """
-    Public key of SSH key
+    Public key of SSH key.
     """
 
     fingerprint: str
     """
-    Fingerprint of SSH key
+    Fingerprint of SSH key.
     """
 
     created_at: Optional[datetime]
     """
-    Creation date of SSH key
+    Creation date of SSH key.
     """
 
     updated_at: Optional[datetime]
     """
-    Last update date of SSH key
+    Last update date of SSH key.
     """
 
     organization_id: str
     """
-    ID of organization linked to the SSH key
+    ID of organization linked to the SSH key.
     """
 
     project_id: str
     """
-    ID of project linked to the SSH key
+    ID of project linked to the SSH key.
     """
 
     disabled: bool
     """
-    SSH key status
+    SSH key status.
     """
 
 
 @dataclass
 class SetRulesResponse:
     """
-    Set rules response
+    Set rules response.
     """
 
     rules: List[Rule]
     """
-    Rules of policy
+    Rules of policy.
     """
 
 
 @dataclass
 class User:
     """
-    User
+    User.
     """
 
     id: str
     """
-    ID of user
+    ID of user.
     """
 
     email: str
     """
-    Email of user
+    Email of user.
     """
 
     created_at: Optional[datetime]
     """
-    Creation date of user
+    Creation date of user.
     """
 
     updated_at: Optional[datetime]
     """
-    Last update date of user
+    Last update date of user.
     """
 
     organization_id: str
     """
-    ID of organization
+    ID of organization.
     """
 
     deletable: bool
     """
-    Deletion status of user. Owner user cannot be deleted
+    Deletion status of user. Owner user cannot be deleted.
     """
 
     last_login_at: Optional[datetime]
     """
-    Last login date
+    Last login date.
     """
 
     type_: UserType
     """
-    Type of the user
+    Type of the user.
     """
 
     two_factor_enabled: bool
     """
-    2FA enabled
+    2FA enabled.
     """
 
     status: UserStatus
     """
-    Status of invitation for the user
+    Status of invitation for the user.
     """
 
 
 @dataclass
 class ListSSHKeysRequest:
     order_by: Optional[ListSSHKeysRequestOrderBy]
     """
-    Sort order of SSH keys
+    Sort order of SSH keys.
     """
 
     page: Optional[int]
     """
-    Requested page number. Value must be greater or equals to 1
+    Requested page number. Value must be greater or equals to 1.
     """
 
     page_size: Optional[int]
     """
-    Number of items per page. Value must be between 1 and 100
+    Number of items per page. Value must be between 1 and 100.
     """
 
     organization_id: Optional[str]
     """
-    Filter by organization ID
+    Filter by organization ID.
     """
 
     name: Optional[str]
     """
-    Name of group to find
+    Name of group to find.
     """
 
     project_id: Optional[str]
     """
-    Filter by project ID
+    Filter by project ID.
     """
 
     disabled: Optional[bool]
     """
-    Filter out disabled SSH keys or not
+    Filter out disabled SSH keys or not.
     """
 
 
 @dataclass
 class CreateSSHKeyRequest:
     name: Optional[str]
     """
-    The name of the SSH key. Max length is 1000
+    The name of the SSH key. Max length is 1000.
     """
 
     public_key: str
     """
-    SSH public key. Currently ssh-rsa, ssh-dss (DSA), ssh-ed25519 and ecdsa keys with NIST curves are supported. Max length is 65000
+    SSH public key. Currently ssh-rsa, ssh-dss (DSA), ssh-ed25519 and ecdsa keys with NIST curves are supported. Max length is 65000.
     """
 
     project_id: Optional[str]
     """
-    Project owning the resource
+    Project owning the resource.
     """
 
 
 @dataclass
 class GetSSHKeyRequest:
     ssh_key_id: str
     """
-    The ID of the SSH key
+    The ID of the SSH key.
     """
 
 
 @dataclass
 class UpdateSSHKeyRequest:
     ssh_key_id: str
 
     name: Optional[str]
     """
-    Name of the SSH key. Max length is 1000
+    Name of the SSH key. Max length is 1000.
     """
 
     disabled: Optional[bool]
     """
-    Enable or disable the SSH key
+    Enable or disable the SSH key.
     """
 
 
 @dataclass
 class DeleteSSHKeyRequest:
     ssh_key_id: str
 
 
 @dataclass
 class ListUsersRequest:
     order_by: Optional[ListUsersRequestOrderBy]
     """
-    Criteria for sorting results
+    Criteria for sorting results.
     """
 
     page_size: Optional[int]
     """
-    Number of results per page. Value must be between 1 and 100
+    Number of results per page. Value must be between 1 and 100.
     """
 
     page: Optional[int]
     """
-    Number of page. Value must be greater or equals to 1
+    Number of page. Value must be greater or equals to 1.
     """
 
     organization_id: Optional[str]
     """
-    ID of organization to filter
+    ID of organization to filter.
     """
 
     user_ids: Optional[List[str]]
     """
-    Filter out by a list of ID
+    Filter out by a list of ID.
     """
 
 
 @dataclass
 class GetUserRequest:
     user_id: str
     """
-    ID of user to find
+    ID of user to find.
     """
 
 
 @dataclass
 class DeleteUserRequest:
     user_id: str
     """
-    ID of user to delete
+    ID of user to delete.
     """
 
 
 @dataclass
 class ListApplicationsRequest:
     order_by: Optional[ListApplicationsRequestOrderBy]
     """
-    Criteria for sorting results
+    Criteria for sorting results.
     """
 
     page_size: Optional[int]
     """
-    Number of results per page. Value must be between 1 and 100
+    Number of results per page. Value must be between 1 and 100.
     """
 
     page: Optional[int]
     """
-    Number of page. Value must be greater to 1
+    Number of page. Value must be greater to 1.
     """
 
     name: Optional[str]
     """
-    Name of application to filter
+    Name of application to filter.
     """
 
     organization_id: Optional[str]
     """
-    ID of organization to filter
+    ID of organization to filter.
     """
 
     editable: Optional[bool]
     """
-    Filter out editable applications or not
+    Filter out editable applications or not.
     """
 
     application_ids: Optional[List[str]]
     """
-    Filter out by a list of ID
+    Filter out by a list of ID.
     """
 
 
 @dataclass
 class CreateApplicationRequest:
     name: Optional[str]
     """
-    Name of application to create (max length is 64 chars)
+    Name of application to create (max length is 64 chars).
     """
 
     organization_id: Optional[str]
     """
-    ID of organization
+    ID of organization.
     """
 
     description: str
     """
-    Description of application (max length is 200 chars)
+    Description of application (max length is 200 chars).
     """
 
 
 @dataclass
 class GetApplicationRequest:
     application_id: str
     """
-    ID of application to find
+    ID of application to find.
     """
 
 
 @dataclass
 class UpdateApplicationRequest:
     application_id: str
     """
-    ID of application to update
+    ID of application to update.
     """
 
     name: Optional[str]
     """
-    New name of application (max length is 64 chars)
+    New name of application (max length is 64 chars).
     """
 
     description: Optional[str]
     """
-    New description of application (max length is 200 chars)
+    New description of application (max length is 200 chars).
     """
 
 
 @dataclass
 class DeleteApplicationRequest:
     application_id: str
     """
-    ID of application to delete
+    ID of application to delete.
     """
 
 
 @dataclass
 class ListGroupsRequest:
     order_by: Optional[ListGroupsRequestOrderBy]
     """
-    Sort order of groups
+    Sort order of groups.
     """
 
     page: Optional[int]
     """
-    Requested page number. Value must be greater or equals to 1
+    Requested page number. Value must be greater or equals to 1.
     """
 
     page_size: Optional[int]
     """
-    Number of items per page. Value must be between 1 and 100
+    Number of items per page. Value must be between 1 and 100.
     """
 
     organization_id: Optional[str]
     """
-    Filter by organization ID
+    Filter by organization ID.
     """
 
     name: Optional[str]
     """
-    Name of group to find
+    Name of group to find.
     """
 
     application_ids: Optional[List[str]]
     """
-    Filter out by a list of application ID
+    Filter out by a list of application ID.
     """
 
     user_ids: Optional[List[str]]
     """
-    Filter out by a list of user ID
+    Filter out by a list of user ID.
     """
 
     group_ids: Optional[List[str]]
     """
-    Filter out by a list of group ID
+    Filter out by a list of group ID.
     """
 
 
 @dataclass
 class CreateGroupRequest:
     organization_id: Optional[str]
     """
-    ID of organization linked to the group
+    ID of organization linked to the group.
     """
 
     name: Optional[str]
     """
-    Name of the group to create (max length is 64 chars). MUST be unique inside an organization
+    Name of the group to create (max length is 64 chars). MUST be unique inside an organization.
     """
 
     description: str
     """
-    Description of the group to create (max length is 200 chars)
+    Description of the group to create (max length is 200 chars).
     """
 
 
 @dataclass
 class GetGroupRequest:
     group_id: str
     """
-    ID of group
+    ID of group.
     """
 
 
 @dataclass
 class UpdateGroupRequest:
     group_id: str
     """
-    ID of group to update
+    ID of group to update.
     """
 
     name: Optional[str]
     """
-    New name for the group (max length is 64 chars). MUST be unique inside an organization
+    New name for the group (max length is 64 chars). MUST be unique inside an organization.
     """
 
     description: Optional[str]
     """
-    New description for the group (max length is 200 chars)
+    New description for the group (max length is 200 chars).
     """
 
 
 @dataclass
 class SetGroupMembersRequest:
     group_id: str
 
@@ -1046,15 +1161,15 @@
     application_ids: List[str]
 
 
 @dataclass
 class AddGroupMemberRequest:
     group_id: str
     """
-    ID of group
+    ID of group.
     """
 
     user_id: Optional[str]
     """
     ID of the user to add.
     
     One-of ('member'): at most one of 'user_id', 'application_id' could be set.
@@ -1068,15 +1183,15 @@
     """
 
 
 @dataclass
 class RemoveGroupMemberRequest:
     group_id: str
     """
-    ID of group
+    ID of group.
     """
 
     user_id: Optional[str]
     """
     ID of the user to remove.
     
     One-of ('member'): at most one of 'user_id', 'application_id' could be set.
@@ -1090,91 +1205,91 @@
     """
 
 
 @dataclass
 class DeleteGroupRequest:
     group_id: str
     """
-    ID of group to delete
+    ID of group to delete.
     """
 
 
 @dataclass
 class ListPoliciesRequest:
     order_by: Optional[ListPoliciesRequestOrderBy]
     """
-    Criteria for sorting results
+    Criteria for sorting results.
     """
 
     page_size: Optional[int]
     """
-    Number of results per page. Value must be between 1 and 100
+    Number of results per page. Value must be between 1 and 100.
     """
 
     page: Optional[int]
     """
-    Number of page. Value must be greater to 1
+    Number of page. Value must be greater to 1.
     """
 
     organization_id: Optional[str]
     """
-    ID of organization to filter
+    ID of organization to filter.
     """
 
     editable: Optional[bool]
     """
-    Filter out editable policies or not
+    Filter out editable policies or not.
     """
 
     user_ids: Optional[List[str]]
     """
-    Filter out by a list of user ID
+    Filter out by a list of user ID.
     """
 
     group_ids: Optional[List[str]]
     """
-    Filter out by a list of group ID
+    Filter out by a list of group ID.
     """
 
     application_ids: Optional[List[str]]
     """
-    Filter out by a list of application ID
+    Filter out by a list of application ID.
     """
 
     no_principal: Optional[bool]
     """
-    True when the policy do not belong to any principal
+    True when the policy do not belong to any principal.
     """
 
     policy_name: Optional[str]
     """
-    Name of policy to fetch
+    Name of policy to fetch.
     """
 
 
 @dataclass
 class CreatePolicyRequest:
     name: Optional[str]
     """
-    Name of policy to create (max length is 64 chars)
+    Name of policy to create (max length is 64 chars).
     """
 
     description: str
     """
-    Description of policy to create (max length is 200 chars)
+    Description of policy to create (max length is 200 chars).
     """
 
     organization_id: Optional[str]
     """
-    ID of organization
+    ID of organization.
     """
 
     rules: Optional[List[RuleSpecs]]
     """
-    Rules of the policy to create
+    Rules of the policy to create.
     """
 
     user_id: Optional[str]
     """
     ID of user, owner of the policy.
     
     One-of ('principal'): at most one of 'user_id', 'group_id', 'application_id', 'no_principal' could be set.
@@ -1202,33 +1317,33 @@
     """
 
 
 @dataclass
 class GetPolicyRequest:
     policy_id: str
     """
-    Id of policy to search
+    Id of policy to search.
     """
 
 
 @dataclass
 class UpdatePolicyRequest:
     policy_id: str
     """
-    Id of policy to update
+    Id of policy to update.
     """
 
     name: Optional[str]
     """
-    New name of policy (max length is 64 chars)
+    New name of policy (max length is 64 chars).
     """
 
     description: Optional[str]
     """
-    New description of policy (max length is 200 chars)
+    New description of policy (max length is 200 chars).
     """
 
     user_id: Optional[str]
     """
     New ID of user, owner of the policy.
     
     One-of ('principal'): at most one of 'user_id', 'group_id', 'application_id', 'no_principal' could be set.
@@ -1256,97 +1371,97 @@
     """
 
 
 @dataclass
 class DeletePolicyRequest:
     policy_id: str
     """
-    Id of policy to delete
+    Id of policy to delete.
     """
 
 
 @dataclass
 class ClonePolicyRequest:
     policy_id: str
 
 
 @dataclass
 class SetRulesRequest:
     policy_id: str
     """
-    Id of policy to update
+    Id of policy to update.
     """
 
     rules: List[RuleSpecs]
     """
-    Rules of the policy to set
+    Rules of the policy to set.
     """
 
 
 @dataclass
 class ListRulesRequest:
     policy_id: str
     """
-    Id of policy to search
+    Id of policy to search.
     """
 
     page_size: Optional[int]
     """
-    Number of results per page. Value must be between 1 and 100
+    Number of results per page. Value must be between 1 and 100.
     """
 
     page: Optional[int]
     """
-    Number of page. Value must be greater to 1
+    Number of page. Value must be greater to 1.
     """
 
 
 @dataclass
 class ListPermissionSetsRequest:
     order_by: Optional[ListPermissionSetsRequestOrderBy]
     """
-    Criteria for sorting results
+    Criteria for sorting results.
     """
 
     page_size: Optional[int]
     """
-    Number of results per page. Value must be between 1 and 100
+    Number of results per page. Value must be between 1 and 100.
     """
 
     page: Optional[int]
     """
-    Number of page. Value must be greater to 1
+    Number of page. Value must be greater to 1.
     """
 
     organization_id: Optional[str]
     """
-    Filter by organization ID
+    Filter by organization ID.
     """
 
 
 @dataclass
 class ListAPIKeysRequest:
     order_by: Optional[ListAPIKeysRequestOrderBy]
     """
-    Criteria for sorting results
+    Criteria for sorting results.
     """
 
     page: Optional[int]
     """
-    Number of page. Value must be greater or equals to 1
+    Number of page. Value must be greater or equals to 1.
     """
 
     page_size: Optional[int]
     """
-    Number of results per page. Value must be between 1 and 100
+    Number of results per page. Value must be between 1 and 100.
     """
 
     organization_id: Optional[str]
     """
-    ID of organization
+    ID of organization.
     """
 
     application_id: Optional[str]
     """
     ID of an application bearer.
     
     One-of ('bearer'): at most one of 'application_id', 'user_id' could be set.
@@ -1359,40 +1474,40 @@
     
     One-of ('bearer'): at most one of 'application_id', 'user_id' could be set.
     :deprecated
     """
 
     editable: Optional[bool]
     """
-    Filter out editable API keys or not
+    Filter out editable API keys or not.
     """
 
     expired: Optional[bool]
     """
-    Filter out expired API keys or not
+    Filter out expired API keys or not.
     """
 
     access_key: Optional[str]
     """
-    Filter out by access key
+    Filter out by access key.
     """
 
     description: Optional[str]
     """
-    Filter out by description
+    Filter out by description.
     """
 
     bearer_id: Optional[str]
     """
-    Filter out by bearer ID
+    Filter out by bearer ID.
     """
 
     bearer_type: Optional[BearerType]
     """
-    Filter out by type of bearer
+    Filter out by type of bearer.
     """
 
 
 @dataclass
 class CreateAPIKeyRequest:
     application_id: Optional[str]
     """
@@ -1406,53 +1521,133 @@
     ID of user principal.
     
     One-of ('bearer'): at most one of 'application_id', 'user_id' could be set.
     """
 
     expires_at: Optional[datetime]
     """
-    Expiration date of the API key
+    Expiration date of the API key.
     """
 
     default_project_id: Optional[str]
     """
-    The default project ID to use with object storage
+    The default project ID to use with object storage.
     """
 
     description: str
     """
-    The description of the API key (max length is 200 chars)
+    The description of the API key (max length is 200 chars).
     """
 
 
 @dataclass
 class GetAPIKeyRequest:
     access_key: str
     """
-    Access key to search for
+    Access key to search for.
     """
 
 
 @dataclass
 class UpdateAPIKeyRequest:
     access_key: str
     """
-    Access key to update
+    Access key to update.
     """
 
     default_project_id: Optional[str]
     """
-    The new default project ID to set
+    The new default project ID to set.
     """
 
     description: Optional[str]
     """
-    The new description to update
+    The new description to update.
     """
 
 
 @dataclass
 class DeleteAPIKeyRequest:
     access_key: str
     """
-    Access key to delete
+    Access key to delete.
+    """
+
+
+@dataclass
+class ListQuotaRequest:
+    order_by: Optional[ListQuotaRequestOrderBy]
+    """
+    Criteria for sorting results.
+    """
+
+    page_size: Optional[int]
+    """
+    Number of results per page. Value must be between 1 and 100.
+    """
+
+    page: Optional[int]
+    """
+    Number of page. Value must be greater to 1.
+    """
+
+    organization_id: Optional[str]
+    """
+    Filter by organization ID.
+    """
+
+
+@dataclass
+class GetQuotumRequest:
+    quotum_name: str
+    """
+    Name of the quotum to get.
+    """
+
+    organization_id: Optional[str]
+    """
+    ID of the organization.
+    """
+
+
+@dataclass
+class ListJWTsRequest:
+    order_by: Optional[ListJWTsRequestOrderBy]
+    """
+    Criteria for sorting results.
+    """
+
+    audience_id: str
+    """
+    ID of the user to search.
+    """
+
+    page_size: Optional[int]
+    """
+    Number of results per page. Value must be between 1 and 100.
+    """
+
+    page: Optional[int]
+    """
+    Number of page. Value must be greater to 1.
+    """
+
+    expired: Optional[bool]
+    """
+    Filter out expired JWTs or not.
+    """
+
+
+@dataclass
+class GetJWTRequest:
+    jti: str
+    """
+    JWT ID of the JWT to get.
+    """
+
+
+@dataclass
+class DeleteJWTRequest:
+    jti: str
+    """
+    JWT ID of the JWT to delete.
     """
```

### Comparing `scaleway_async-0.8.0/scaleway_async/instance/v1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/instance/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/instance/v1/api.py` & `scaleway_async-0.9.0/scaleway_async/instance/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/instance/v1/content.py` & `scaleway_async-0.9.0/scaleway_async/instance/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/instance/v1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/instance/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/instance/v1/types.py` & `scaleway_async-0.9.0/scaleway_async/instance/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/instance/v1/types_private.py` & `scaleway_async-0.9.0/scaleway_async/instance/v1/types_private.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/iot/v1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/iot/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/iot/v1/api.py` & `scaleway_async-0.9.0/scaleway_async/iot/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/iot/v1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/iot/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/iot/v1/types.py` & `scaleway_async-0.9.0/scaleway_async/iot/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/k8s/v1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/k8s/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/k8s/v1/api.py` & `scaleway_async-0.9.0/scaleway_async/k8s/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/k8s/v1/content.py` & `scaleway_async-0.9.0/scaleway_async/k8s/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/k8s/v1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/k8s/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/k8s/v1/types.py` & `scaleway_async-0.9.0/scaleway_async/k8s/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/k8s/v1/types_private.py` & `scaleway_async-0.9.0/scaleway_async/k8s/v1/types_private.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/lb/v1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/lb/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/lb/v1/api.py` & `scaleway_async-0.9.0/scaleway_async/lb/v1/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     ListLbPrivateNetworksResponse,
     ListLbTypesResponse,
     ListLbsResponse,
     ListRoutesResponse,
     ListSubscriberResponse,
     PrivateNetwork,
     PrivateNetworkDHCPConfig,
+    PrivateNetworkIpamConfig,
     PrivateNetworkStaticConfig,
     Route,
     RouteMatch,
     SetAclsResponse,
     Subscriber,
     SubscriberEmailConfig,
     SubscriberWebhookConfig,
@@ -3023,26 +3024,30 @@
         self,
         *,
         lb_id: str,
         private_network_id: str,
         region: Optional[Region] = None,
         static_config: Optional[PrivateNetworkStaticConfig] = None,
         dhcp_config: Optional[PrivateNetworkDHCPConfig] = None,
+        ipam_config: Optional[PrivateNetworkIpamConfig] = None,
     ) -> PrivateNetwork:
         """
         Add load balancer on instance private network
         :param region: Region to target. If none is passed will use default region from the config
         :param lb_id: Load balancer ID
         :param private_network_id: Set your instance private network id
         :param static_config: Define two local ip address of your choice for each load balancer instance.
 
-        One-of ('config'): at most one of 'static_config', 'dhcp_config' could be set.
+        One-of ('config'): at most one of 'static_config', 'dhcp_config', 'ipam_config' could be set.
         :param dhcp_config: Set to true if you want to let DHCP assign IP addresses.
 
-        One-of ('config'): at most one of 'static_config', 'dhcp_config' could be set.
+        One-of ('config'): at most one of 'static_config', 'dhcp_config', 'ipam_config' could be set.
+        :param ipam_config: For internal use only.
+
+        One-of ('config'): at most one of 'static_config', 'dhcp_config', 'ipam_config' could be set.
         :return: :class:`PrivateNetwork <PrivateNetwork>`
 
         Usage:
         ::
 
             result = await api.attach_private_network(
                 lb_id="example",
@@ -3064,14 +3069,15 @@
             body=marshal_AttachPrivateNetworkRequest(
                 AttachPrivateNetworkRequest(
                     lb_id=lb_id,
                     private_network_id=private_network_id,
                     region=region,
                     static_config=static_config,
                     dhcp_config=dhcp_config,
+                    ipam_config=ipam_config,
                 ),
                 self.client,
             ),
         )
 
         self._throw_on_error(res)
         return unmarshal_PrivateNetwork(res.json())
@@ -5880,26 +5886,30 @@
         self,
         *,
         lb_id: str,
         private_network_id: str,
         zone: Optional[Zone] = None,
         static_config: Optional[PrivateNetworkStaticConfig] = None,
         dhcp_config: Optional[PrivateNetworkDHCPConfig] = None,
+        ipam_config: Optional[PrivateNetworkIpamConfig] = None,
     ) -> PrivateNetwork:
         """
         Add load balancer on instance private network
         :param zone: Zone to target. If none is passed will use default zone from the config
         :param lb_id: Load balancer ID
         :param private_network_id: Set your instance private network id
         :param static_config: Define two local ip address of your choice for each load balancer instance.
 
-        One-of ('config'): at most one of 'static_config', 'dhcp_config' could be set.
+        One-of ('config'): at most one of 'static_config', 'dhcp_config', 'ipam_config' could be set.
         :param dhcp_config: Set to true if you want to let DHCP assign IP addresses.
 
-        One-of ('config'): at most one of 'static_config', 'dhcp_config' could be set.
+        One-of ('config'): at most one of 'static_config', 'dhcp_config', 'ipam_config' could be set.
+        :param ipam_config: For internal use only.
+
+        One-of ('config'): at most one of 'static_config', 'dhcp_config', 'ipam_config' could be set.
         :return: :class:`PrivateNetwork <PrivateNetwork>`
 
         Usage:
         ::
 
             result = await api.attach_private_network(
                 lb_id="example",
@@ -5919,14 +5929,15 @@
             body=marshal_ZonedApiAttachPrivateNetworkRequest(
                 ZonedApiAttachPrivateNetworkRequest(
                     lb_id=lb_id,
                     private_network_id=private_network_id,
                     zone=zone,
                     static_config=static_config,
                     dhcp_config=dhcp_config,
+                    ipam_config=ipam_config,
                 ),
                 self.client,
             ),
         )
 
         self._throw_on_error(res)
         return unmarshal_PrivateNetwork(res.json())
```

### Comparing `scaleway_async-0.8.0/scaleway_async/lb/v1/content.py` & `scaleway_async-0.9.0/scaleway_async/lb/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/lb/v1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/lb/v1/marshalling.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     ListLbPrivateNetworksResponse,
     ListLbTypesResponse,
     ListLbsResponse,
     ListRoutesResponse,
     ListSubscriberResponse,
     PrivateNetwork,
     PrivateNetworkDHCPConfig,
+    PrivateNetworkIpamConfig,
     PrivateNetworkStaticConfig,
     Route,
     RouteMatch,
     SetAclsResponse,
     Subscriber,
     SubscriberEmailConfig,
     SubscriberWebhookConfig,
@@ -715,14 +716,25 @@
         )
 
     args: Dict[str, Any] = {}
 
     return PrivateNetworkDHCPConfig(**args)
 
 
+def unmarshal_PrivateNetworkIpamConfig(data: Any) -> PrivateNetworkIpamConfig:
+    if type(data) is not dict:
+        raise TypeError(
+            f"Unmarshalling the type 'PrivateNetworkIpamConfig' failed as data isn't a dictionary."
+        )
+
+    args: Dict[str, Any] = {}
+
+    return PrivateNetworkIpamConfig(**args)
+
+
 def unmarshal_PrivateNetworkStaticConfig(data: Any) -> PrivateNetworkStaticConfig:
     if type(data) is not dict:
         raise TypeError(
             f"Unmarshalling the type 'PrivateNetworkStaticConfig' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
@@ -857,14 +869,19 @@
     args["created_at"] = parser.isoparse(field) if type(field) is str else field
 
     field = data.get("dhcp_config")
     args["dhcp_config"] = (
         unmarshal_PrivateNetworkDHCPConfig(field) if field is not None else None
     )
 
+    field = data.get("ipam_config")
+    args["ipam_config"] = (
+        unmarshal_PrivateNetworkIpamConfig(field) if field is not None else None
+    )
+
     field = data.get("lb")
     args["lb"] = unmarshal_Lb(field) if field is not None else None
 
     field = data.get("private_network_id")
     args["private_network_id"] = field
 
     field = data.get("static_config")
@@ -1295,14 +1312,21 @@
 def marshal_PrivateNetworkDHCPConfig(
     request: PrivateNetworkDHCPConfig,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     return {}
 
 
+def marshal_PrivateNetworkIpamConfig(
+    request: PrivateNetworkIpamConfig,
+    defaults: ProfileDefaults,
+) -> Dict[str, Any]:
+    return {}
+
+
 def marshal_PrivateNetworkStaticConfig(
     request: PrivateNetworkStaticConfig,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     return {
         "ip_address": request.ip_address,
     }
@@ -1354,14 +1378,15 @@
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     return {
         **resolve_one_of(
             [
                 OneOfPossibility("static_config", request.static_config),
                 OneOfPossibility("dhcp_config", request.dhcp_config),
+                OneOfPossibility("ipam_config", request.ipam_config),
             ]
         ),
     }
 
 
 def marshal_CreateAclRequest(
     request: CreateAclRequest,
@@ -1720,14 +1745,15 @@
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     return {
         **resolve_one_of(
             [
                 OneOfPossibility("static_config", request.static_config),
                 OneOfPossibility("dhcp_config", request.dhcp_config),
+                OneOfPossibility("ipam_config", request.ipam_config),
             ]
         ),
     }
 
 
 def marshal_ZonedApiCreateAclRequest(
     request: ZonedApiCreateAclRequest,
```

### Comparing `scaleway_async-0.8.0/scaleway_async/lb/v1/types.py` & `scaleway_async-0.9.0/scaleway_async/lb/v1/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1340,22 +1340,29 @@
     LoadBalancer object
     """
 
     static_config: Optional[PrivateNetworkStaticConfig]
     """
     Local ip address of load balancer instance.
     
-    One-of ('config'): at most one of 'static_config', 'dhcp_config' could be set.
+    One-of ('config'): at most one of 'static_config', 'dhcp_config', 'ipam_config' could be set.
     """
 
     dhcp_config: Optional[PrivateNetworkDHCPConfig]
     """
     Value set to true if load balancer instance use a DHCP.
     
-    One-of ('config'): at most one of 'static_config', 'dhcp_config' could be set.
+    One-of ('config'): at most one of 'static_config', 'dhcp_config', 'ipam_config' could be set.
+    """
+
+    ipam_config: Optional[PrivateNetworkIpamConfig]
+    """
+    Value set to true if load balancer instance use a DHCP.
+    
+    One-of ('config'): at most one of 'static_config', 'dhcp_config', 'ipam_config' could be set.
     """
 
     private_network_id: str
     """
     Instance private network id
     """
 
@@ -2983,22 +2990,29 @@
     Set your instance private network id
     """
 
     static_config: Optional[PrivateNetworkStaticConfig]
     """
     Define two local ip address of your choice for each load balancer instance.
     
-    One-of ('config'): at most one of 'static_config', 'dhcp_config' could be set.
+    One-of ('config'): at most one of 'static_config', 'dhcp_config', 'ipam_config' could be set.
     """
 
     dhcp_config: Optional[PrivateNetworkDHCPConfig]
     """
     Set to true if you want to let DHCP assign IP addresses.
     
-    One-of ('config'): at most one of 'static_config', 'dhcp_config' could be set.
+    One-of ('config'): at most one of 'static_config', 'dhcp_config', 'ipam_config' could be set.
+    """
+
+    ipam_config: Optional[PrivateNetworkIpamConfig]
+    """
+    For internal use only.
+    
+    One-of ('config'): at most one of 'static_config', 'dhcp_config', 'ipam_config' could be set.
     """
 
 
 @dataclass
 class DetachPrivateNetworkRequest:
     region: Optional[Region]
     """
@@ -4497,22 +4511,29 @@
     Set your instance private network id
     """
 
     static_config: Optional[PrivateNetworkStaticConfig]
     """
     Define two local ip address of your choice for each load balancer instance.
     
-    One-of ('config'): at most one of 'static_config', 'dhcp_config' could be set.
+    One-of ('config'): at most one of 'static_config', 'dhcp_config', 'ipam_config' could be set.
     """
 
     dhcp_config: Optional[PrivateNetworkDHCPConfig]
     """
     Set to true if you want to let DHCP assign IP addresses.
     
-    One-of ('config'): at most one of 'static_config', 'dhcp_config' could be set.
+    One-of ('config'): at most one of 'static_config', 'dhcp_config', 'ipam_config' could be set.
+    """
+
+    ipam_config: Optional[PrivateNetworkIpamConfig]
+    """
+    For internal use only.
+    
+    One-of ('config'): at most one of 'static_config', 'dhcp_config', 'ipam_config' could be set.
     """
 
 
 @dataclass
 class ZonedApiDetachPrivateNetworkRequest:
     zone: Optional[Zone]
     """
```

### Comparing `scaleway_async-0.8.0/scaleway_async/marketplace/v1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/marketplace/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/marketplace/v1/api.py` & `scaleway_async-0.9.0/scaleway_async/marketplace/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/marketplace/v1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/marketplace/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/marketplace/v1/types.py` & `scaleway_async-0.9.0/scaleway_async/marketplace/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/marketplace/v2/__init__.py` & `scaleway_async-0.9.0/scaleway_async/marketplace/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/marketplace/v2/api.py` & `scaleway_async-0.9.0/scaleway_async/marketplace/v2/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/marketplace/v2/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/marketplace/v2/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/marketplace/v2/types.py` & `scaleway_async-0.9.0/scaleway_async/marketplace/v2/types.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/mnq/v1alpha1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/mnq/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/mnq/v1alpha1/api.py` & `scaleway_async-0.9.0/scaleway_async/mnq/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/mnq/v1alpha1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/mnq/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/mnq/v1alpha1/types.py` & `scaleway_async-0.9.0/scaleway_async/mnq/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/rdb/v1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/rdb/v1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from .types import Endpoint
 from .types import EndpointDirectAccessDetails
 from .types import EndpointLoadBalancerDetails
 from .types import EndpointPrivateNetworkDetails
 from .types import EndpointSpec
 from .types import EndpointSpecLoadBalancer
 from .types import EndpointSpecPrivateNetwork
+from .types import EndpointSpecPrivateNetworkIpamConfig
 from .types import EngineSetting
 from .types import EngineVersion
 from .types import Instance
 from .types import InstanceLog
 from .types import InstanceMetrics
 from .types import InstanceSetting
 from .types import ListDatabaseBackupsResponse
@@ -63,14 +64,15 @@
 from .types import NodeTypeVolumeType
 from .types import PrepareInstanceLogsResponse
 from .types import Privilege
 from .types import ReadReplica
 from .types import ReadReplicaEndpointSpec
 from .types import ReadReplicaEndpointSpecDirectAccess
 from .types import ReadReplicaEndpointSpecPrivateNetwork
+from .types import ReadReplicaEndpointSpecPrivateNetworkIpamConfig
 from .types import SetInstanceACLRulesResponse
 from .types import SetInstanceSettingsResponse
 from .types import Snapshot
 from .types import UpgradableVersion
 from .types import User
 from .types import Volume
 from .content import DATABASE_BACKUP_TRANSIENT_STATUSES
@@ -116,14 +118,15 @@
     "Endpoint",
     "EndpointDirectAccessDetails",
     "EndpointLoadBalancerDetails",
     "EndpointPrivateNetworkDetails",
     "EndpointSpec",
     "EndpointSpecLoadBalancer",
     "EndpointSpecPrivateNetwork",
+    "EndpointSpecPrivateNetworkIpamConfig",
     "EngineSetting",
     "EngineVersion",
     "Instance",
     "InstanceLog",
     "InstanceMetrics",
     "InstanceSetting",
     "ListDatabaseBackupsResponse",
@@ -145,14 +148,15 @@
     "NodeTypeVolumeType",
     "PrepareInstanceLogsResponse",
     "Privilege",
     "ReadReplica",
     "ReadReplicaEndpointSpec",
     "ReadReplicaEndpointSpecDirectAccess",
     "ReadReplicaEndpointSpecPrivateNetwork",
+    "ReadReplicaEndpointSpecPrivateNetworkIpamConfig",
     "SetInstanceACLRulesResponse",
     "SetInstanceSettingsResponse",
     "Snapshot",
     "UpgradableVersion",
     "User",
     "Volume",
     "DATABASE_BACKUP_TRANSIENT_STATUSES",
```

### Comparing `scaleway_async-0.8.0/scaleway_async/rdb/v1/api.py` & `scaleway_async-0.9.0/scaleway_async/rdb/v1/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,15 @@
     UpdateUserRequest,
     CreateDatabaseRequest,
     SetPrivilegeRequest,
     CreateSnapshotRequest,
     UpdateSnapshotRequest,
     CreateInstanceFromSnapshotRequest,
     CreateEndpointRequest,
+    MigrateEndpointRequest,
 )
 from .content import (
     DATABASE_BACKUP_TRANSIENT_STATUSES,
     INSTANCE_LOG_TRANSIENT_STATUSES,
     INSTANCE_TRANSIENT_STATUSES,
     READ_REPLICA_TRANSIENT_STATUSES,
     SNAPSHOT_TRANSIENT_STATUSES,
@@ -107,14 +108,15 @@
     marshal_CreateInstanceRequest,
     marshal_CreateReadReplicaEndpointRequest,
     marshal_CreateReadReplicaRequest,
     marshal_CreateSnapshotRequest,
     marshal_CreateUserRequest,
     marshal_DeleteInstanceACLRulesRequest,
     marshal_DeleteInstanceSettingsRequest,
+    marshal_MigrateEndpointRequest,
     marshal_PrepareInstanceLogsRequest,
     marshal_PurgeInstanceLogsRequest,
     marshal_RestoreDatabaseBackupRequest,
     marshal_SetInstanceACLRulesRequest,
     marshal_SetInstanceSettingsRequest,
     marshal_SetPrivilegeRequest,
     marshal_UpdateDatabaseBackupRequest,
@@ -165,17 +167,17 @@
         name: Optional[str] = None,
         version: Optional[str] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> ListDatabaseEnginesResponse:
         """
         List available database engines
-        :param region: Region to target. If none is passed will use default region from the config
-        :param name: Name of the Database Engine
-        :param version: Version of the Database Engine
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param name: Name of the Database Engine.
+        :param version: Version of the Database Engine.
         :param page:
         :param page_size:
         :return: :class:`ListDatabaseEnginesResponse <ListDatabaseEnginesResponse>`
 
         Usage:
         ::
 
@@ -207,17 +209,17 @@
         name: Optional[str] = None,
         version: Optional[str] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[DatabaseEngine]:
         """
         List available database engines
-        :param region: Region to target. If none is passed will use default region from the config
-        :param name: Name of the Database Engine
-        :param version: Version of the Database Engine
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param name: Name of the Database Engine.
+        :param version: Version of the Database Engine.
         :param page:
         :param page_size:
         :return: :class:`List[ListDatabaseEnginesResponse] <List[ListDatabaseEnginesResponse]>`
 
         Usage:
         ::
 
@@ -243,16 +245,16 @@
         include_disabled_types: bool,
         region: Optional[Region] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> ListNodeTypesResponse:
         """
         List available node types
-        :param region: Region to target. If none is passed will use default region from the config
-        :param include_disabled_types: Whether or not to include disabled types
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param include_disabled_types: Whether or not to include disabled types.
         :param page:
         :param page_size:
         :return: :class:`ListNodeTypesResponse <ListNodeTypesResponse>`
 
         Usage:
         ::
 
@@ -282,16 +284,16 @@
         include_disabled_types: bool,
         region: Optional[Region] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[NodeType]:
         """
         List available node types
-        :param region: Region to target. If none is passed will use default region from the config
-        :param include_disabled_types: Whether or not to include disabled types
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param include_disabled_types: Whether or not to include disabled types.
         :param page:
         :param page_size:
         :return: :class:`List[ListNodeTypesResponse] <List[ListNodeTypesResponse]>`
 
         Usage:
         ::
 
@@ -320,20 +322,20 @@
         organization_id: Optional[str] = None,
         project_id: Optional[str] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> ListDatabaseBackupsResponse:
         """
         List database backups
-        :param region: Region to target. If none is passed will use default region from the config
-        :param name: Name of the database backups
-        :param order_by: Criteria to use when ordering database backups listing
-        :param instance_id: UUID of the instance
-        :param organization_id: Organization ID the database backups belongs to
-        :param project_id: Project ID the database backups belongs to
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param name: Name of the database backups.
+        :param order_by: Criteria to use when ordering database backups listing.
+        :param instance_id: UUID of the instance.
+        :param organization_id: Organization ID the database backups belongs to.
+        :param project_id: Project ID the database backups belongs to.
         :param page:
         :param page_size:
         :return: :class:`ListDatabaseBackupsResponse <ListDatabaseBackupsResponse>`
 
         Usage:
         ::
 
@@ -372,20 +374,20 @@
         organization_id: Optional[str] = None,
         project_id: Optional[str] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[DatabaseBackup]:
         """
         List database backups
-        :param region: Region to target. If none is passed will use default region from the config
-        :param name: Name of the database backups
-        :param order_by: Criteria to use when ordering database backups listing
-        :param instance_id: UUID of the instance
-        :param organization_id: Organization ID the database backups belongs to
-        :param project_id: Project ID the database backups belongs to
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param name: Name of the database backups.
+        :param order_by: Criteria to use when ordering database backups listing.
+        :param instance_id: UUID of the instance.
+        :param organization_id: Organization ID the database backups belongs to.
+        :param project_id: Project ID the database backups belongs to.
         :param page:
         :param page_size:
         :return: :class:`List[ListDatabaseBackupsResponse] <List[ListDatabaseBackupsResponse]>`
 
         Usage:
         ::
 
@@ -415,19 +417,19 @@
         database_name: str,
         region: Optional[Region] = None,
         name: Optional[str] = None,
         expires_at: Optional[datetime] = None,
     ) -> DatabaseBackup:
         """
         Create a database backup
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance
-        :param database_name: Name of the database you want to make a backup of
-        :param name: Name of the backup
-        :param expires_at: Expiration date (Format ISO 8601)
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance.
+        :param database_name: Name of the database you want to make a backup of.
+        :param name: Name of the backup.
+        :param expires_at: Expiration date (Format ISO 8601).
         :return: :class:`DatabaseBackup <DatabaseBackup>`
 
         Usage:
         ::
 
             result = await api.create_database_backup(
                 instance_id="example",
@@ -461,16 +463,16 @@
         self,
         *,
         database_backup_id: str,
         region: Optional[Region] = None,
     ) -> DatabaseBackup:
         """
         Get a database backup
-        :param region: Region to target. If none is passed will use default region from the config
-        :param database_backup_id: UUID of the database backup
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param database_backup_id: UUID of the database backup.
         :return: :class:`DatabaseBackup <DatabaseBackup>`
 
         Usage:
         ::
 
             result = await api.get_database_backup(database_backup_id="example")
         """
@@ -497,16 +499,16 @@
         region: Optional[Region] = None,
         options: Optional[
             WaitForOptions[DatabaseBackup, Union[bool, Awaitable[bool]]]
         ] = None,
     ) -> DatabaseBackup:
         """
         Waits for :class:`DatabaseBackup <DatabaseBackup>` to be in a final state.
-        :param region: Region to target. If none is passed will use default region from the config
-        :param database_backup_id: UUID of the database backup
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param database_backup_id: UUID of the database backup.
         :param options: The options for the waiter
         :return: :class:`DatabaseBackup <DatabaseBackup>`
 
         Usage:
         ::
 
             result = api.wait_for_database_backup(database_backup_id="example")
@@ -535,18 +537,18 @@
         database_backup_id: str,
         region: Optional[Region] = None,
         name: Optional[str] = None,
         expires_at: Optional[datetime] = None,
     ) -> DatabaseBackup:
         """
         Update a database backup
-        :param region: Region to target. If none is passed will use default region from the config
-        :param database_backup_id: UUID of the database backup to update
-        :param name: Name of the Database Backup
-        :param expires_at: Expiration date (Format ISO 8601)
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param database_backup_id: UUID of the database backup to update.
+        :param name: Name of the Database Backup.
+        :param expires_at: Expiration date (Format ISO 8601).
         :return: :class:`DatabaseBackup <DatabaseBackup>`
 
         Usage:
         ::
 
             result = await api.update_database_backup(database_backup_id="example")
         """
@@ -579,16 +581,16 @@
         self,
         *,
         database_backup_id: str,
         region: Optional[Region] = None,
     ) -> DatabaseBackup:
         """
         Delete a database backup
-        :param region: Region to target. If none is passed will use default region from the config
-        :param database_backup_id: UUID of the database backup to delete
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param database_backup_id: UUID of the database backup to delete.
         :return: :class:`DatabaseBackup <DatabaseBackup>`
 
         Usage:
         ::
 
             result = await api.delete_database_backup(database_backup_id="example")
         """
@@ -614,18 +616,18 @@
         database_backup_id: str,
         instance_id: str,
         region: Optional[Region] = None,
         database_name: Optional[str] = None,
     ) -> DatabaseBackup:
         """
         Restore a database backup
-        :param region: Region to target. If none is passed will use default region from the config
-        :param database_backup_id: Backup of a logical database
-        :param database_name: Defines the destination database in order to restore into a specified database, the default destination is set to the origin database of the backup
-        :param instance_id: Defines the rdb instance where the backup has to be restored
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param database_backup_id: Backup of a logical database.
+        :param database_name: Defines the destination database in order to restore into a specified database, the default destination is set to the origin database of the backup.
+        :param instance_id: Defines the rdb instance where the backup has to be restored.
         :return: :class:`DatabaseBackup <DatabaseBackup>`
 
         Usage:
         ::
 
             result = await api.restore_database_backup(
                 database_backup_id="example",
@@ -661,16 +663,16 @@
         self,
         *,
         database_backup_id: str,
         region: Optional[Region] = None,
     ) -> DatabaseBackup:
         """
         Export a database backup
-        :param region: Region to target. If none is passed will use default region from the config
-        :param database_backup_id: UUID of the database backup you want to export
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param database_backup_id: UUID of the database backup you want to export.
         :return: :class:`DatabaseBackup <DatabaseBackup>`
 
         Usage:
         ::
 
             result = await api.export_database_backup(database_backup_id="example")
         """
@@ -699,16 +701,16 @@
         enable_ha: Optional[bool] = None,
         volume_size: Optional[int] = None,
         volume_type: Optional[VolumeType] = None,
         upgradable_version_id: Optional[str] = None,
     ) -> Instance:
         """
         Upgrade your current instance specifications like node type, high availability, volume, or db engine version.
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance you want to upgrade
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance you want to upgrade.
         :param node_type: Node type of the instance you want to upgrade to.
 
         One-of ('upgrade_target'): at most one of 'node_type', 'enable_ha', 'volume_size', 'volume_type', 'upgradable_version_id' could be set.
         :param enable_ha: Set to true to enable high availability on your instance.
 
         One-of ('upgrade_target'): at most one of 'node_type', 'enable_ha', 'volume_size', 'volume_type', 'upgradable_version_id' could be set.
         :param volume_size: Increase your block storage volume size.
@@ -763,20 +765,20 @@
         organization_id: Optional[str] = None,
         project_id: Optional[str] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> ListInstancesResponse:
         """
         List instances
-        :param region: Region to target. If none is passed will use default region from the config
-        :param tags: List instance that have a given tags
-        :param name: List instance that match a given name pattern
-        :param order_by: Criteria to use when ordering instance listing
-        :param organization_id: Please use `project_id` instead
-        :param project_id: Project ID to list the instance of
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param tags: List instance that have a given tags.
+        :param name: List instance that match a given name pattern.
+        :param order_by: Criteria to use when ordering instance listing.
+        :param organization_id: Please use `project_id` instead.
+        :param project_id: Project ID to list the instance of.
         :param page:
         :param page_size:
         :return: :class:`ListInstancesResponse <ListInstancesResponse>`
 
         Usage:
         ::
 
@@ -815,20 +817,20 @@
         organization_id: Optional[str] = None,
         project_id: Optional[str] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[Instance]:
         """
         List instances
-        :param region: Region to target. If none is passed will use default region from the config
-        :param tags: List instance that have a given tags
-        :param name: List instance that match a given name pattern
-        :param order_by: Criteria to use when ordering instance listing
-        :param organization_id: Please use `project_id` instead
-        :param project_id: Project ID to list the instance of
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param tags: List instance that have a given tags.
+        :param name: List instance that match a given name pattern.
+        :param order_by: Criteria to use when ordering instance listing.
+        :param organization_id: Please use `project_id` instead.
+        :param project_id: Project ID to list the instance of.
         :param page:
         :param page_size:
         :return: :class:`List[ListInstancesResponse] <List[ListInstancesResponse]>`
 
         Usage:
         ::
 
@@ -855,16 +857,16 @@
         self,
         *,
         instance_id: str,
         region: Optional[Region] = None,
     ) -> Instance:
         """
         Get an instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance.
         :return: :class:`Instance <Instance>`
 
         Usage:
         ::
 
             result = await api.get_instance(instance_id="example")
         """
@@ -889,16 +891,16 @@
         region: Optional[Region] = None,
         options: Optional[
             WaitForOptions[Instance, Union[bool, Awaitable[bool]]]
         ] = None,
     ) -> Instance:
         """
         Waits for :class:`Instance <Instance>` to be in a final state.
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance.
         :param options: The options for the waiter
         :return: :class:`Instance <Instance>`
 
         Usage:
         ::
 
             result = api.wait_for_instance(instance_id="example")
@@ -937,34 +939,34 @@
         name: Optional[str] = None,
         tags: Optional[List[str]] = None,
         init_settings: Optional[List[InstanceSetting]] = None,
         init_endpoints: Optional[List[EndpointSpec]] = None,
     ) -> Instance:
         """
         Create an instance
-        :param region: Region to target. If none is passed will use default region from the config
+        :param region: Region to target. If none is passed will use default region from the config.
         :param organization_id: Please use `project_id` instead.
 
         One-of ('project_identifier'): at most one of 'organization_id', 'project_id' could be set.
         :param project_id: The project ID on which to create the instance.
 
         One-of ('project_identifier'): at most one of 'organization_id', 'project_id' could be set.
-        :param name: Name of the instance
-        :param engine: Database engine of the database (PostgreSQL, MySQL, ...)
-        :param user_name: Name of the user created when the instance is created
-        :param password: Password of the user
-        :param node_type: Type of node to use for the instance
-        :param is_ha_cluster: Whether or not High-Availability is enabled
-        :param disable_backup: Whether or not backups are disabled
-        :param tags: Tags to apply to the instance
-        :param init_settings: List of engine settings to be set at database initialisation
-        :param volume_type: Type of volume where data are stored (lssd, bssd, ...)
-        :param volume_size: Volume size when volume_type is not lssd
-        :param init_endpoints: One or multiple EndpointSpec used to expose your database instance. A load_balancer public endpoint is systematically created
-        :param backup_same_region: Store logical backups in the same region as the database instance
+        :param name: Name of the instance.
+        :param engine: Database engine of the database (PostgreSQL, MySQL, ...).
+        :param user_name: Name of the user created when the instance is created.
+        :param password: Password of the user.
+        :param node_type: Type of node to use for the instance.
+        :param is_ha_cluster: Whether or not High-Availability is enabled.
+        :param disable_backup: Whether or not backups are disabled.
+        :param tags: Tags to apply to the instance.
+        :param init_settings: List of engine settings to be set at database initialisation.
+        :param volume_type: Type of volume where data are stored (lssd, bssd, ...).
+        :param volume_size: Volume size when volume_type is not lssd.
+        :param init_endpoints: One or multiple EndpointSpec used to expose your database instance. A load_balancer public endpoint is systematically created.
+        :param backup_same_region: Store logical backups in the same region as the database instance.
         :return: :class:`Instance <Instance>`
 
         Usage:
         ::
 
             result = await api.create_instance(
                 engine="example",
@@ -1023,23 +1025,23 @@
         name: Optional[str] = None,
         tags: Optional[List[str]] = None,
         logs_policy: Optional[LogsPolicy] = None,
         backup_same_region: Optional[bool] = None,
     ) -> Instance:
         """
         Update an instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance to update
-        :param backup_schedule_frequency: In hours
-        :param backup_schedule_retention: In days
-        :param is_backup_schedule_disabled: Whether or not the backup schedule is disabled
-        :param name: Name of the instance
-        :param tags: Tags of a given instance
-        :param logs_policy: Logs policy of the instance
-        :param backup_same_region: Store logical backups in the same region as the database instance
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance to update.
+        :param backup_schedule_frequency: In hours.
+        :param backup_schedule_retention: In days.
+        :param is_backup_schedule_disabled: Whether or not the backup schedule is disabled.
+        :param name: Name of the instance.
+        :param tags: Tags of a given instance.
+        :param logs_policy: Logs policy of the instance.
+        :param backup_same_region: Store logical backups in the same region as the database instance.
         :return: :class:`Instance <Instance>`
 
         Usage:
         ::
 
             result = await api.update_instance(instance_id="example")
         """
@@ -1075,16 +1077,16 @@
         self,
         *,
         instance_id: str,
         region: Optional[Region] = None,
     ) -> Instance:
         """
         Delete an instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance to delete
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance to delete.
         :return: :class:`Instance <Instance>`
 
         Usage:
         ::
 
             result = await api.delete_instance(instance_id="example")
         """
@@ -1108,18 +1110,18 @@
         instance_id: str,
         name: str,
         region: Optional[Region] = None,
         node_type: Optional[str] = None,
     ) -> Instance:
         """
         Clone an instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance you want to clone
-        :param name: Name of the clone instance
-        :param node_type: Node type of the clone
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance you want to clone.
+        :param name: Name of the clone instance.
+        :param node_type: Node type of the clone.
         :return: :class:`Instance <Instance>`
 
         Usage:
         ::
 
             result = await api.clone_instance(
                 instance_id="example",
@@ -1153,16 +1155,16 @@
         self,
         *,
         instance_id: str,
         region: Optional[Region] = None,
     ) -> Instance:
         """
         Restart an instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance you want to restart
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance you want to restart.
         :return: :class:`Instance <Instance>`
 
         Usage:
         ::
 
             result = await api.restart_instance(instance_id="example")
         """
@@ -1184,16 +1186,16 @@
         self,
         *,
         instance_id: str,
         region: Optional[Region] = None,
     ) -> Optional[ScwFile]:
         """
         Get the TLS certificate of an instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance.
         :return: :class:`Optional[ScwFile] <Optional[ScwFile]>`
 
         Usage:
         ::
 
             result = await api.get_instance_certificate(instance_id="example")
         """
@@ -1216,16 +1218,16 @@
         self,
         *,
         instance_id: str,
         region: Optional[Region] = None,
     ) -> Optional[None]:
         """
         Renew the TLS certificate of an instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance you want logs of
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance you want logs of.
 
         Usage:
         ::
 
             result = await api.renew_instance_certificate(instance_id="example")
         """
 
@@ -1249,19 +1251,19 @@
         region: Optional[Region] = None,
         start_date: Optional[datetime] = None,
         end_date: Optional[datetime] = None,
         metric_name: Optional[str] = None,
     ) -> InstanceMetrics:
         """
         Get database instance metrics.
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance
-        :param start_date: Start date to gather metrics from
-        :param end_date: End date to gather metrics from
-        :param metric_name: Name of the metric to gather
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance.
+        :param start_date: Start date to gather metrics from.
+        :param end_date: End date to gather metrics from.
+        :param metric_name: Name of the metric to gather.
         :return: :class:`InstanceMetrics <InstanceMetrics>`
 
         Usage:
         ::
 
             result = await api.get_instance_metrics(instance_id="example")
         """
@@ -1289,17 +1291,17 @@
         *,
         instance_id: str,
         region: Optional[Region] = None,
         endpoint_spec: Optional[List[ReadReplicaEndpointSpec]] = None,
     ) -> ReadReplica:
         """
         You can only create a maximum of 3 read replicas for one instance.
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance you want a read replica of
-        :param endpoint_spec: Specification of the endpoint you want to create
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance you want a read replica of.
+        :param endpoint_spec: Specification of the endpoint you want to create.
         :return: :class:`ReadReplica <ReadReplica>`
 
         Usage:
         ::
 
             result = await api.create_read_replica(instance_id="example")
         """
@@ -1328,16 +1330,16 @@
         self,
         *,
         read_replica_id: str,
         region: Optional[Region] = None,
     ) -> ReadReplica:
         """
         Get a read replica
-        :param region: Region to target. If none is passed will use default region from the config
-        :param read_replica_id: UUID of the read replica
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param read_replica_id: UUID of the read replica.
         :return: :class:`ReadReplica <ReadReplica>`
 
         Usage:
         ::
 
             result = await api.get_read_replica(read_replica_id="example")
         """
@@ -1362,16 +1364,16 @@
         region: Optional[Region] = None,
         options: Optional[
             WaitForOptions[ReadReplica, Union[bool, Awaitable[bool]]]
         ] = None,
     ) -> ReadReplica:
         """
         Waits for :class:`ReadReplica <ReadReplica>` to be in a final state.
-        :param region: Region to target. If none is passed will use default region from the config
-        :param read_replica_id: UUID of the read replica
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param read_replica_id: UUID of the read replica.
         :param options: The options for the waiter
         :return: :class:`ReadReplica <ReadReplica>`
 
         Usage:
         ::
 
             result = api.wait_for_read_replica(read_replica_id="example")
@@ -1396,16 +1398,16 @@
         self,
         *,
         read_replica_id: str,
         region: Optional[Region] = None,
     ) -> ReadReplica:
         """
         Delete a read replica
-        :param region: Region to target. If none is passed will use default region from the config
-        :param read_replica_id: UUID of the read replica
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param read_replica_id: UUID of the read replica.
         :return: :class:`ReadReplica <ReadReplica>`
 
         Usage:
         ::
 
             result = await api.delete_read_replica(read_replica_id="example")
         """
@@ -1430,16 +1432,16 @@
         region: Optional[Region] = None,
     ) -> ReadReplica:
         """
         When you resync a read replica, first it is reset, and then its data is resynchronized from the primary node.
         Your read replica will be unavailable during the resync process. The duration of this process is proportional to your Database Instance size.
         The configured endpoints will not change.
 
-        :param region: Region to target. If none is passed will use default region from the config
-        :param read_replica_id: UUID of the read replica
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param read_replica_id: UUID of the read replica.
         :return: :class:`ReadReplica <ReadReplica>`
 
         Usage:
         ::
 
             result = await api.reset_read_replica(read_replica_id="example")
         """
@@ -1462,17 +1464,17 @@
         *,
         read_replica_id: str,
         endpoint_spec: List[ReadReplicaEndpointSpec],
         region: Optional[Region] = None,
     ) -> ReadReplica:
         """
         A read replica can have at most one direct access and one private network endpoint.
-        :param region: Region to target. If none is passed will use default region from the config
-        :param read_replica_id: UUID of the read replica
-        :param endpoint_spec: Specification of the endpoint you want to create
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param read_replica_id: UUID of the read replica.
+        :param endpoint_spec: Specification of the endpoint you want to create.
         :return: :class:`ReadReplica <ReadReplica>`
 
         Usage:
         ::
 
             result = await api.create_read_replica_endpoint(
                 read_replica_id="example",
@@ -1507,18 +1509,18 @@
         instance_id: str,
         region: Optional[Region] = None,
         start_date: Optional[datetime] = None,
         end_date: Optional[datetime] = None,
     ) -> PrepareInstanceLogsResponse:
         """
         Prepare your instance logs. Logs will be grouped on a minimum interval of a day.
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance you want logs of
-        :param start_date: Start datetime of your log. Format: `{year}-{month}-{day}T{hour}:{min}:{sec}[.{frac_sec}]Z`
-        :param end_date: End datetime of your log. Format: `{year}-{month}-{day}T{hour}:{min}:{sec}[.{frac_sec}]Z`
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance you want logs of.
+        :param start_date: Start datetime of your log. Format: `{year}-{month}-{day}T{hour}:{min}:{sec}[.{frac_sec}]Z`.
+        :param end_date: End datetime of your log. Format: `{year}-{month}-{day}T{hour}:{min}:{sec}[.{frac_sec}]Z`.
         :return: :class:`PrepareInstanceLogsResponse <PrepareInstanceLogsResponse>`
 
         Usage:
         ::
 
             result = await api.prepare_instance_logs(instance_id="example")
         """
@@ -1550,17 +1552,17 @@
         *,
         instance_id: str,
         order_by: ListInstanceLogsRequestOrderBy,
         region: Optional[Region] = None,
     ) -> ListInstanceLogsResponse:
         """
         List available logs of a given instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance you want logs of
-        :param order_by: Criteria to use when ordering instance logs listing
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance you want logs of.
+        :param order_by: Criteria to use when ordering instance logs listing.
         :return: :class:`ListInstanceLogsResponse <ListInstanceLogsResponse>`
 
         Usage:
         ::
 
             result = await api.list_instance_logs(
                 instance_id="example",
@@ -1588,16 +1590,16 @@
         self,
         *,
         instance_log_id: str,
         region: Optional[Region] = None,
     ) -> InstanceLog:
         """
         Get specific logs of a given instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_log_id: UUID of the instance_log you want
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_log_id: UUID of the instance_log you want.
         :return: :class:`InstanceLog <InstanceLog>`
 
         Usage:
         ::
 
             result = await api.get_instance_log(instance_log_id="example")
         """
@@ -1622,16 +1624,16 @@
         region: Optional[Region] = None,
         options: Optional[
             WaitForOptions[InstanceLog, Union[bool, Awaitable[bool]]]
         ] = None,
     ) -> InstanceLog:
         """
         Waits for :class:`InstanceLog <InstanceLog>` to be in a final state.
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_log_id: UUID of the instance_log you want
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_log_id: UUID of the instance_log you want.
         :param options: The options for the waiter
         :return: :class:`InstanceLog <InstanceLog>`
 
         Usage:
         ::
 
             result = api.wait_for_instance_log(instance_log_id="example")
@@ -1657,17 +1659,17 @@
         *,
         instance_id: str,
         region: Optional[Region] = None,
         log_name: Optional[str] = None,
     ) -> Optional[None]:
         """
         purge remote instances logs
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance you want logs of
-        :param log_name: Specific log name to purge
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance you want logs of.
+        :param log_name: Specific log name to purge.
 
         Usage:
         ::
 
             result = await api.purge_instance_logs(instance_id="example")
         """
 
@@ -1696,16 +1698,16 @@
         self,
         *,
         instance_id: str,
         region: Optional[Region] = None,
     ) -> ListInstanceLogsDetailsResponse:
         """
         List remote instances logs details
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance you want logs of
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance you want logs of.
         :return: :class:`ListInstanceLogsDetailsResponse <ListInstanceLogsDetailsResponse>`
 
         Usage:
         ::
 
             result = await api.list_instance_logs_details(instance_id="example")
         """
@@ -1728,17 +1730,17 @@
         *,
         instance_id: str,
         settings: List[InstanceSetting],
         region: Optional[Region] = None,
     ) -> AddInstanceSettingsResponse:
         """
         Add an instance setting
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance you want to add settings to
-        :param settings: Settings to add on the instance
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance you want to add settings to.
+        :param settings: Settings to add on the instance.
         :return: :class:`AddInstanceSettingsResponse <AddInstanceSettingsResponse>`
 
         Usage:
         ::
 
             result = await api.add_instance_settings(
                 instance_id="example",
@@ -1772,17 +1774,17 @@
         *,
         instance_id: str,
         setting_names: List[str],
         region: Optional[Region] = None,
     ) -> DeleteInstanceSettingsResponse:
         """
         Delete an instance setting
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance to delete settings from
-        :param setting_names: Settings names to delete
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance to delete settings from.
+        :param setting_names: Settings names to delete.
         :return: :class:`DeleteInstanceSettingsResponse <DeleteInstanceSettingsResponse>`
 
         Usage:
         ::
 
             result = await api.delete_instance_settings(
                 instance_id="example",
@@ -1816,17 +1818,17 @@
         *,
         instance_id: str,
         settings: List[InstanceSetting],
         region: Optional[Region] = None,
     ) -> SetInstanceSettingsResponse:
         """
         Set a given instance setting
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance where the settings has to be set
-        :param settings: Settings to define for the instance
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance where the settings has to be set.
+        :param settings: Settings to define for the instance.
         :return: :class:`SetInstanceSettingsResponse <SetInstanceSettingsResponse>`
 
         Usage:
         ::
 
             result = await api.set_instance_settings(
                 instance_id="example",
@@ -1861,16 +1863,16 @@
         instance_id: str,
         region: Optional[Region] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> ListInstanceACLRulesResponse:
         """
         List ACL rules of a given instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance.
         :param page:
         :param page_size:
         :return: :class:`ListInstanceACLRulesResponse <ListInstanceACLRulesResponse>`
 
         Usage:
         ::
 
@@ -1900,16 +1902,16 @@
         instance_id: str,
         region: Optional[Region] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[ACLRule]:
         """
         List ACL rules of a given instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance.
         :param page:
         :param page_size:
         :return: :class:`List[ListInstanceACLRulesResponse] <List[ListInstanceACLRulesResponse]>`
 
         Usage:
         ::
 
@@ -1933,17 +1935,17 @@
         *,
         instance_id: str,
         rules: List[ACLRuleRequest],
         region: Optional[Region] = None,
     ) -> AddInstanceACLRulesResponse:
         """
         Add an additional ACL rule to a database instance.
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance you want to add acl rules to
-        :param rules: ACLs rules to add to the instance
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance you want to add acl rules to.
+        :param rules: ACLs rules to add to the instance.
         :return: :class:`AddInstanceACLRulesResponse <AddInstanceACLRulesResponse>`
 
         Usage:
         ::
 
             result = await api.add_instance_acl_rules(
                 instance_id="example",
@@ -1977,17 +1979,17 @@
         *,
         instance_id: str,
         rules: List[ACLRuleRequest],
         region: Optional[Region] = None,
     ) -> SetInstanceACLRulesResponse:
         """
         Replace all the ACL rules of a database instance.
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance where the ACL rules has to be set
-        :param rules: ACL rules to define for the instance
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance where the ACL rules has to be set.
+        :param rules: ACL rules to define for the instance.
         :return: :class:`SetInstanceACLRulesResponse <SetInstanceACLRulesResponse>`
 
         Usage:
         ::
 
             result = await api.set_instance_acl_rules(
                 instance_id="example",
@@ -2021,17 +2023,17 @@
         *,
         instance_id: str,
         acl_rule_ips: List[str],
         region: Optional[Region] = None,
     ) -> DeleteInstanceACLRulesResponse:
         """
         Delete ACL rules of a given instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance you want to delete an ACL rules from
-        :param acl_rule_ips: ACL rules IP present on the instance
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance you want to delete an ACL rules from.
+        :param acl_rule_ips: ACL rules IP present on the instance.
         :return: :class:`DeleteInstanceACLRulesResponse <DeleteInstanceACLRulesResponse>`
 
         Usage:
         ::
 
             result = await api.delete_instance_acl_rules(
                 instance_id="example",
@@ -2068,18 +2070,18 @@
         name: Optional[str] = None,
         order_by: ListUsersRequestOrderBy = ListUsersRequestOrderBy.NAME_ASC,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> ListUsersResponse:
         """
         List users of a given instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance
-        :param name: Name of the user
-        :param order_by: Criteria to use when ordering users listing
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance.
+        :param name: Name of the user.
+        :param order_by: Criteria to use when ordering users listing.
         :param page:
         :param page_size:
         :return: :class:`ListUsersResponse <ListUsersResponse>`
 
         Usage:
         ::
 
@@ -2113,18 +2115,18 @@
         name: Optional[str] = None,
         order_by: Optional[ListUsersRequestOrderBy] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[User]:
         """
         List users of a given instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance
-        :param name: Name of the user
-        :param order_by: Criteria to use when ordering users listing
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance.
+        :param name: Name of the user.
+        :param order_by: Criteria to use when ordering users listing.
         :param page:
         :param page_size:
         :return: :class:`List[ListUsersResponse] <List[ListUsersResponse]>`
 
         Usage:
         ::
 
@@ -2152,19 +2154,19 @@
         name: str,
         password: str,
         is_admin: bool,
         region: Optional[Region] = None,
     ) -> User:
         """
         Create a user on a given instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance you want to create a user in
-        :param name: Name of the user you want to create
-        :param password: Password of the user you want to create
-        :param is_admin: Whether the user you want to create will have administrative privileges
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance you want to create a user in.
+        :param name: Name of the user you want to create.
+        :param password: Password of the user you want to create.
+        :param is_admin: Whether the user you want to create will have administrative privileges.
         :return: :class:`User <User>`
 
         Usage:
         ::
 
             result = await api.create_user(
                 instance_id="example",
@@ -2204,19 +2206,19 @@
         name: str,
         region: Optional[Region] = None,
         password: Optional[str] = None,
         is_admin: Optional[bool] = None,
     ) -> User:
         """
         Update a user on a given instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance the user belongs to
-        :param name: Name of the database user
-        :param password: Password of the database user
-        :param is_admin: Whether or not this user got administrative privileges
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance the user belongs to.
+        :param name: Name of the database user.
+        :param password: Password of the database user.
+        :param is_admin: Whether or not this user got administrative privileges.
         :return: :class:`User <User>`
 
         Usage:
         ::
 
             result = await api.update_user(
                 instance_id="example",
@@ -2253,17 +2255,17 @@
         *,
         instance_id: str,
         name: str,
         region: Optional[Region] = None,
     ) -> Optional[None]:
         """
         Delete a user on a given instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance to delete a user from
-        :param name: Name of the user
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance to delete a user from.
+        :param name: Name of the user.
 
         Usage:
         ::
 
             result = await api.delete_user(
                 instance_id="example",
                 name="example",
@@ -2294,20 +2296,20 @@
         owner: Optional[str] = None,
         order_by: ListDatabasesRequestOrderBy = ListDatabasesRequestOrderBy.NAME_ASC,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> ListDatabasesResponse:
         """
         List all database in a given instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance to list database of
-        :param name: Name of the database
-        :param managed: Whether or not the database is managed
-        :param owner: User that owns this database
-        :param order_by: Criteria to use when ordering database listing
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance to list database of.
+        :param name: Name of the database.
+        :param managed: Whether or not the database is managed.
+        :param owner: User that owns this database.
+        :param order_by: Criteria to use when ordering database listing.
         :param page:
         :param page_size:
         :return: :class:`ListDatabasesResponse <ListDatabasesResponse>`
 
         Usage:
         ::
 
@@ -2345,20 +2347,20 @@
         owner: Optional[str] = None,
         order_by: Optional[ListDatabasesRequestOrderBy] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[Database]:
         """
         List all database in a given instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance to list database of
-        :param name: Name of the database
-        :param managed: Whether or not the database is managed
-        :param owner: User that owns this database
-        :param order_by: Criteria to use when ordering database listing
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance to list database of.
+        :param name: Name of the database.
+        :param managed: Whether or not the database is managed.
+        :param owner: User that owns this database.
+        :param order_by: Criteria to use when ordering database listing.
         :param page:
         :param page_size:
         :return: :class:`List[ListDatabasesResponse] <List[ListDatabasesResponse]>`
 
         Usage:
         ::
 
@@ -2386,17 +2388,17 @@
         *,
         instance_id: str,
         name: str,
         region: Optional[Region] = None,
     ) -> Database:
         """
         Create a database in a given instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance where to create the database
-        :param name: Name of the database
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance where to create the database.
+        :param name: Name of the database.
         :return: :class:`Database <Database>`
 
         Usage:
         ::
 
             result = await api.create_database(
                 instance_id="example",
@@ -2430,17 +2432,17 @@
         *,
         instance_id: str,
         name: str,
         region: Optional[Region] = None,
     ) -> Optional[None]:
         """
         Delete a database in a given instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance where to delete the database
-        :param name: Name of the database to delete
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance where to delete the database.
+        :param name: Name of the database to delete.
 
         Usage:
         ::
 
             result = await api.delete_database(
                 instance_id="example",
                 name="example",
@@ -2470,21 +2472,21 @@
         page: Optional[int] = None,
         page_size: Optional[int] = None,
         database_name: Optional[str] = None,
         user_name: Optional[str] = None,
     ) -> ListPrivilegesResponse:
         """
         List privileges of a given user for a given database on a given instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance
-        :param order_by: Criteria to use when ordering privileges listing
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance.
+        :param order_by: Criteria to use when ordering privileges listing.
         :param page:
         :param page_size:
-        :param database_name: Name of the database
-        :param user_name: Name of the user
+        :param database_name: Name of the database.
+        :param user_name: Name of the user.
         :return: :class:`ListPrivilegesResponse <ListPrivilegesResponse>`
 
         Usage:
         ::
 
             result = await api.list_privileges(instance_id="example")
         """
@@ -2518,21 +2520,21 @@
         page: Optional[int] = None,
         page_size: Optional[int] = None,
         database_name: Optional[str] = None,
         user_name: Optional[str] = None,
     ) -> List[Privilege]:
         """
         List privileges of a given user for a given database on a given instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance
-        :param order_by: Criteria to use when ordering privileges listing
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance.
+        :param order_by: Criteria to use when ordering privileges listing.
         :param page:
         :param page_size:
-        :param database_name: Name of the database
-        :param user_name: Name of the user
+        :param database_name: Name of the database.
+        :param user_name: Name of the user.
         :return: :class:`List[ListPrivilegesResponse] <List[ListPrivilegesResponse]>`
 
         Usage:
         ::
 
             result = await api.list_privileges_all(instance_id="example")
         """
@@ -2559,19 +2561,19 @@
         database_name: str,
         user_name: str,
         permission: Permission,
         region: Optional[Region] = None,
     ) -> Privilege:
         """
         Set privileges of a given user for a given database on a given instance
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance
-        :param database_name: Name of the database
-        :param user_name: Name of the user
-        :param permission: Permission to set (Read, Read/Write, All, Custom)
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance.
+        :param database_name: Name of the database.
+        :param user_name: Name of the user.
+        :param permission: Permission to set (Read, Read/Write, All, Custom).
         :return: :class:`Privilege <Privilege>`
 
         Usage:
         ::
 
             result = await api.set_privilege(
                 instance_id="example",
@@ -2614,20 +2616,20 @@
         organization_id: Optional[str] = None,
         project_id: Optional[str] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> ListSnapshotsResponse:
         """
         List instance snapshots
-        :param region: Region to target. If none is passed will use default region from the config
-        :param name: Name of the snapshot
-        :param order_by: Criteria to use when ordering snapshot listing
-        :param instance_id: UUID of the instance
-        :param organization_id: Organization ID the snapshots belongs to
-        :param project_id: Project ID the snapshots belongs to
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param name: Name of the snapshot.
+        :param order_by: Criteria to use when ordering snapshot listing.
+        :param instance_id: UUID of the instance.
+        :param organization_id: Organization ID the snapshots belongs to.
+        :param project_id: Project ID the snapshots belongs to.
         :param page:
         :param page_size:
         :return: :class:`ListSnapshotsResponse <ListSnapshotsResponse>`
 
         Usage:
         ::
 
@@ -2666,20 +2668,20 @@
         organization_id: Optional[str] = None,
         project_id: Optional[str] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[Snapshot]:
         """
         List instance snapshots
-        :param region: Region to target. If none is passed will use default region from the config
-        :param name: Name of the snapshot
-        :param order_by: Criteria to use when ordering snapshot listing
-        :param instance_id: UUID of the instance
-        :param organization_id: Organization ID the snapshots belongs to
-        :param project_id: Project ID the snapshots belongs to
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param name: Name of the snapshot.
+        :param order_by: Criteria to use when ordering snapshot listing.
+        :param instance_id: UUID of the instance.
+        :param organization_id: Organization ID the snapshots belongs to.
+        :param project_id: Project ID the snapshots belongs to.
         :param page:
         :param page_size:
         :return: :class:`List[ListSnapshotsResponse] <List[ListSnapshotsResponse]>`
 
         Usage:
         ::
 
@@ -2706,16 +2708,16 @@
         self,
         *,
         snapshot_id: str,
         region: Optional[Region] = None,
     ) -> Snapshot:
         """
         Get an instance snapshot
-        :param region: Region to target. If none is passed will use default region from the config
-        :param snapshot_id: UUID of the snapshot
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param snapshot_id: UUID of the snapshot.
         :return: :class:`Snapshot <Snapshot>`
 
         Usage:
         ::
 
             result = await api.get_snapshot(snapshot_id="example")
         """
@@ -2740,16 +2742,16 @@
         region: Optional[Region] = None,
         options: Optional[
             WaitForOptions[Snapshot, Union[bool, Awaitable[bool]]]
         ] = None,
     ) -> Snapshot:
         """
         Waits for :class:`Snapshot <Snapshot>` to be in a final state.
-        :param region: Region to target. If none is passed will use default region from the config
-        :param snapshot_id: UUID of the snapshot
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param snapshot_id: UUID of the snapshot.
         :param options: The options for the waiter
         :return: :class:`Snapshot <Snapshot>`
 
         Usage:
         ::
 
             result = api.wait_for_snapshot(snapshot_id="example")
@@ -2776,18 +2778,18 @@
         instance_id: str,
         region: Optional[Region] = None,
         name: Optional[str] = None,
         expires_at: Optional[datetime] = None,
     ) -> Snapshot:
         """
         Create an instance snapshot
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance
-        :param name: Name of the snapshot
-        :param expires_at: Expiration date (Format ISO 8601)
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance.
+        :param name: Name of the snapshot.
+        :param expires_at: Expiration date (Format ISO 8601).
         :return: :class:`Snapshot <Snapshot>`
 
         Usage:
         ::
 
             result = await api.create_snapshot(instance_id="example")
         """
@@ -2820,18 +2822,18 @@
         snapshot_id: str,
         region: Optional[Region] = None,
         name: Optional[str] = None,
         expires_at: Optional[datetime] = None,
     ) -> Snapshot:
         """
         Update an instance snapshot
-        :param region: Region to target. If none is passed will use default region from the config
-        :param snapshot_id: UUID of the snapshot to update
-        :param name: Name of the snapshot
-        :param expires_at: Expiration date (Format ISO 8601)
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param snapshot_id: UUID of the snapshot to update.
+        :param name: Name of the snapshot.
+        :param expires_at: Expiration date (Format ISO 8601).
         :return: :class:`Snapshot <Snapshot>`
 
         Usage:
         ::
 
             result = await api.update_snapshot(snapshot_id="example")
         """
@@ -2862,16 +2864,16 @@
         self,
         *,
         snapshot_id: str,
         region: Optional[Region] = None,
     ) -> Snapshot:
         """
         Delete an instance snapshot
-        :param region: Region to target. If none is passed will use default region from the config
-        :param snapshot_id: UUID of the snapshot to delete
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param snapshot_id: UUID of the snapshot to delete.
         :return: :class:`Snapshot <Snapshot>`
 
         Usage:
         ::
 
             result = await api.delete_snapshot(snapshot_id="example")
         """
@@ -2896,19 +2898,19 @@
         instance_name: str,
         region: Optional[Region] = None,
         is_ha_cluster: Optional[bool] = None,
         node_type: Optional[str] = None,
     ) -> Instance:
         """
         Create a new instance from a given snapshot
-        :param region: Region to target. If none is passed will use default region from the config
-        :param snapshot_id: Block snapshot of the instance
-        :param instance_name: Name of the instance created with the snapshot
-        :param is_ha_cluster: Whether or not High-Availability is enabled on the new instance
-        :param node_type: The node type used to restore the snapshot
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param snapshot_id: Block snapshot of the instance.
+        :param instance_name: Name of the instance created with the snapshot.
+        :param is_ha_cluster: Whether or not High-Availability is enabled on the new instance.
+        :param node_type: The node type used to restore the snapshot.
         :return: :class:`Instance <Instance>`
 
         Usage:
         ::
 
             result = await api.create_instance_from_snapshot(
                 snapshot_id="example",
@@ -2944,17 +2946,17 @@
         *,
         instance_id: str,
         region: Optional[Region] = None,
         endpoint_spec: Optional[EndpointSpec] = None,
     ) -> Endpoint:
         """
         Create a new instance endpoint
-        :param region: Region to target. If none is passed will use default region from the config
-        :param instance_id: UUID of the instance you want to add endpoint to
-        :param endpoint_spec: Specification of the endpoint you want to create
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param instance_id: UUID of the instance you want to add endpoint to.
+        :param endpoint_spec: Specification of the endpoint you want to create.
         :return: :class:`Endpoint <Endpoint>`
 
         Usage:
         ::
 
             result = await api.create_endpoint(instance_id="example")
         """
@@ -2984,15 +2986,15 @@
         self,
         *,
         endpoint_id: str,
         region: Optional[Region] = None,
     ) -> Optional[None]:
         """
         Delete an instance endpoint
-        :param region: Region to target. If none is passed will use default region from the config
+        :param region: Region to target. If none is passed will use default region from the config.
         :param endpoint_id: This endpoint can also be used to delete a read replica endpoint.
 
         Usage:
         ::
 
             result = await api.delete_endpoint(endpoint_id="example")
         """
@@ -3014,16 +3016,16 @@
         self,
         *,
         endpoint_id: str,
         region: Optional[Region] = None,
     ) -> Endpoint:
         """
         Get an instance endpoint
-        :param region: Region to target. If none is passed will use default region from the config
-        :param endpoint_id: UUID of the endpoint you want to get
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param endpoint_id: UUID of the endpoint you want to get.
         :return: :class:`Endpoint <Endpoint>`
 
         Usage:
         ::
 
             result = await api.get_endpoint(endpoint_id="example")
         """
@@ -3036,7 +3038,51 @@
         res = self._request(
             "GET",
             f"/rdb/v1/regions/{param_region}/endpoints/{param_endpoint_id}",
         )
 
         self._throw_on_error(res)
         return unmarshal_Endpoint(res.json())
+
+    async def migrate_endpoint(
+        self,
+        *,
+        endpoint_id: str,
+        instance_id: str,
+        region: Optional[Region] = None,
+    ) -> Endpoint:
+        """
+        Migrate an existing instance endpoint to another instance
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param endpoint_id: UUID of the endpoint you want to migrate.
+        :param instance_id: UUID of the instance you want to attach the endpoint to.
+        :return: :class:`Endpoint <Endpoint>`
+
+        Usage:
+        ::
+
+            result = await api.migrate_endpoint(
+                endpoint_id="example",
+                instance_id="example",
+            )
+        """
+
+        param_region = validate_path_param(
+            "region", region or self.client.default_region
+        )
+        param_endpoint_id = validate_path_param("endpoint_id", endpoint_id)
+
+        res = self._request(
+            "POST",
+            f"/rdb/v1/regions/{param_region}/endpoints/{param_endpoint_id}/migrate",
+            body=marshal_MigrateEndpointRequest(
+                MigrateEndpointRequest(
+                    endpoint_id=endpoint_id,
+                    instance_id=instance_id,
+                    region=region,
+                ),
+                self.client,
+            ),
+        )
+
+        self._throw_on_error(res)
+        return unmarshal_Endpoint(res.json())
```

### Comparing `scaleway_async-0.8.0/scaleway_async/rdb/v1/content.py` & `scaleway_async-0.9.0/scaleway_async/rdb/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/rdb/v1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/rdb/v1/marshalling.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     Endpoint,
     EndpointDirectAccessDetails,
     EndpointLoadBalancerDetails,
     EndpointPrivateNetworkDetails,
     EndpointSpec,
     EndpointSpecLoadBalancer,
     EndpointSpecPrivateNetwork,
+    EndpointSpecPrivateNetworkIpamConfig,
     EngineSetting,
     EngineVersion,
     Instance,
     InstanceLog,
     InstanceMetrics,
     InstanceSetting,
     ListDatabaseBackupsResponse,
@@ -57,14 +58,15 @@
     NodeTypeVolumeType,
     PrepareInstanceLogsResponse,
     Privilege,
     ReadReplica,
     ReadReplicaEndpointSpec,
     ReadReplicaEndpointSpecDirectAccess,
     ReadReplicaEndpointSpecPrivateNetwork,
+    ReadReplicaEndpointSpecPrivateNetworkIpamConfig,
     SetInstanceACLRulesResponse,
     SetInstanceSettingsResponse,
     Snapshot,
     UpgradableVersion,
     User,
     Volume,
     CreateDatabaseBackupRequest,
@@ -88,14 +90,15 @@
     UpdateUserRequest,
     CreateDatabaseRequest,
     SetPrivilegeRequest,
     CreateSnapshotRequest,
     UpdateSnapshotRequest,
     CreateInstanceFromSnapshotRequest,
     CreateEndpointRequest,
+    MigrateEndpointRequest,
 )
 
 
 def unmarshal_EndpointDirectAccessDetails(data: Any) -> EndpointDirectAccessDetails:
     if type(data) is not dict:
         raise TypeError(
             f"Unmarshalling the type 'EndpointDirectAccessDetails' failed as data isn't a dictionary."
@@ -1143,28 +1146,47 @@
 
     field = data.get("settings")
     args["settings"] = [unmarshal_InstanceSetting(v) for v in data["settings"]]
 
     return SetInstanceSettingsResponse(**args)
 
 
+def marshal_EndpointSpecPrivateNetworkIpamConfig(
+    request: EndpointSpecPrivateNetworkIpamConfig,
+    defaults: ProfileDefaults,
+) -> Dict[str, Any]:
+    return {}
+
+
+def marshal_ReadReplicaEndpointSpecPrivateNetworkIpamConfig(
+    request: ReadReplicaEndpointSpecPrivateNetworkIpamConfig,
+    defaults: ProfileDefaults,
+) -> Dict[str, Any]:
+    return {}
+
+
 def marshal_EndpointSpecLoadBalancer(
     request: EndpointSpecLoadBalancer,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     return {}
 
 
 def marshal_EndpointSpecPrivateNetwork(
     request: EndpointSpecPrivateNetwork,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     return {
+        **resolve_one_of(
+            [
+                OneOfPossibility("service_ip", request.service_ip),
+                OneOfPossibility("ipam_config", request.ipam_config),
+            ]
+        ),
         "private_network_id": request.private_network_id,
-        "service_ip": request.service_ip,
     }
 
 
 def marshal_ReadReplicaEndpointSpecDirectAccess(
     request: ReadReplicaEndpointSpecDirectAccess,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
@@ -1172,16 +1194,21 @@
 
 
 def marshal_ReadReplicaEndpointSpecPrivateNetwork(
     request: ReadReplicaEndpointSpecPrivateNetwork,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     return {
+        **resolve_one_of(
+            [
+                OneOfPossibility("service_ip", request.service_ip),
+                OneOfPossibility("ipam_config", request.ipam_config),
+            ]
+        ),
         "private_network_id": request.private_network_id,
-        "service_ip": request.service_ip,
     }
 
 
 def marshal_ACLRuleRequest(
     request: ACLRuleRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
@@ -1411,14 +1438,23 @@
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     return {
         "setting_names": request.setting_names,
     }
 
 
+def marshal_MigrateEndpointRequest(
+    request: MigrateEndpointRequest,
+    defaults: ProfileDefaults,
+) -> Dict[str, Any]:
+    return {
+        "instance_id": request.instance_id,
+    }
+
+
 def marshal_PrepareInstanceLogsRequest(
     request: PrepareInstanceLogsRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     return {
         "end_date": request.end_date,
         "start_date": request.start_date,
```

### Comparing `scaleway_async-0.8.0/scaleway_async/rdb/v1/types.py` & `scaleway_async-0.9.0/scaleway_async/rdb/v1/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -205,15 +205,15 @@
 
     def __str__(self) -> str:
         return str(self.value)
 
 
 class ReadReplicaStatus(str, Enum):
     """
-    Read replica. status
+    Read replica. status.
     """
 
     UNKNOWN = "unknown"
     PROVISIONING = "provisioning"
     INITIALIZING = "initializing"
     READY = "ready"
     DELETING = "deleting"
@@ -270,32 +270,32 @@
 
     description: str
 
 
 @dataclass
 class AddInstanceACLRulesResponse:
     """
-    Add instance acl rules response
+    Add instance acl rules response.
     """
 
     rules: List[ACLRule]
     """
-    Rules enabled on the instance
+    Rules enabled on the instance.
     """
 
 
 @dataclass
 class AddInstanceSettingsResponse:
     """
-    Add instance settings response
+    Add instance settings response.
     """
 
     settings: List[InstanceSetting]
     """
-    Settings available on the instance
+    Settings available on the instance.
     """
 
 
 @dataclass
 class BackupSchedule:
     frequency: int
 
@@ -303,192 +303,192 @@
 
     disabled: bool
 
 
 @dataclass
 class Database:
     """
-    Database
+    Database.
     """
 
     name: str
     """
-    Name of the database
+    Name of the database.
     """
 
     owner: str
     """
-    Name of the owner of the database
+    Name of the owner of the database.
     """
 
     managed: bool
     """
-    Whether or not the database is managed or not
+    Whether or not the database is managed or not.
     """
 
     size: int
     """
-    Size of the database
+    Size of the database.
     """
 
 
 @dataclass
 class DatabaseBackup:
     """
-    Database backup
+    Database backup.
     """
 
     id: str
     """
-    UUID of the database backup
+    UUID of the database backup.
     """
 
     instance_id: str
     """
-    UUID of the instance
+    UUID of the instance.
     """
 
     database_name: str
     """
-    Name of the database of this backup
+    Name of the database of this backup.
     """
 
     name: str
     """
-    Name of the backup
+    Name of the backup.
     """
 
     status: DatabaseBackupStatus
     """
-    Status of the backup
+    Status of the backup.
     """
 
     size: Optional[int]
     """
-    Size of the database backup
+    Size of the database backup.
     """
 
     expires_at: Optional[datetime]
     """
-    Expiration date (Format ISO 8601)
+    Expiration date (Format ISO 8601).
     """
 
     created_at: Optional[datetime]
     """
-    Creation date (Format ISO 8601)
+    Creation date (Format ISO 8601).
     """
 
     updated_at: Optional[datetime]
     """
-    Updated date (Format ISO 8601)
+    Updated date (Format ISO 8601).
     """
 
     instance_name: str
     """
-    Name of the instance of the backup
+    Name of the instance of the backup.
     """
 
     download_url: Optional[str]
     """
-    URL you can download the backup from
+    URL you can download the backup from.
     """
 
     download_url_expires_at: Optional[datetime]
     """
-    Expiration date of the download link
+    Expiration date of the download link.
     """
 
     region: Region
     """
-    Region of this database backup
+    Region of this database backup.
     """
 
     same_region: bool
     """
-    Store logical backups in the same region as the source database instance
+    Store logical backups in the same region as the source database instance.
     """
 
 
 @dataclass
 class DatabaseEngine:
     """
-    Database engine
+    Database engine.
     """
 
     name: str
     """
-    Engine name
+    Engine name.
     """
 
     logo_url: str
     """
-    Engine logo URL
+    Engine logo URL.
     """
 
     versions: List[EngineVersion]
     """
-    Available versions
+    Available versions.
     """
 
     region: Region
     """
-    Region of this database engine
+    Region of this database engine.
     """
 
 
 @dataclass
 class DeleteInstanceACLRulesResponse:
     """
-    Delete instance acl rules response
+    Delete instance acl rules response.
     """
 
     rules: List[ACLRule]
     """
-    ACL rules present on the instance
+    ACL rules present on the instance.
     """
 
 
 @dataclass
 class DeleteInstanceSettingsResponse:
     """
-    Delete instance settings response
+    Delete instance settings response.
     """
 
     settings: List[InstanceSetting]
     """
-    Settings names to delete from the instance
+    Settings names to delete from the instance.
     """
 
 
 @dataclass
 class Endpoint:
     """
-    Endpoint
+    Endpoint.
     """
 
     id: str
     """
-    UUID of the endpoint
+    UUID of the endpoint.
     """
 
     ip: Optional[str]
     """
     IPv4 address of the endpoint.
     
     One-of ('address'): at most one of 'ip', 'hostname' could be set.
     """
 
     port: int
     """
-    TCP port of the endpoint
+    TCP port of the endpoint.
     """
 
     name: Optional[str]
     """
-    Name of the endpoint
+    Name of the endpoint.
     """
 
     private_network: Optional[EndpointPrivateNetworkDetails]
     """
     Private network details. One at the most per RDB instance or read replica (an RDB instance and its read replica can have different private networks). Cannot be updated (has to be deleted and recreated).
     
     One-of ('details'): at most one of 'private_network', 'load_balancer', 'direct_access' could be set.
@@ -525,37 +525,37 @@
 class EndpointLoadBalancerDetails:
     pass
 
 
 @dataclass
 class EndpointPrivateNetworkDetails:
     """
-    Endpoint. private network details
+    Endpoint. private network details.
     """
 
     private_network_id: str
     """
-    UUID of the private network
+    UUID of the private network.
     """
 
     service_ip: str
     """
-    CIDR notation of the endpoint IPv4 address
+    CIDR notation of the endpoint IPv4 address.
     """
 
     zone: Zone
     """
-    Private network zone
+    Private network zone.
     """
 
 
 @dataclass
 class EndpointSpec:
     """
-    Endpoint spec
+    Endpoint spec.
     """
 
     load_balancer: Optional[EndpointSpecLoadBalancer]
     """
     Load balancer endpoint specifications. Public endpoint for RDB instances which is systematically present. One per RDB instance.
     
     One-of ('spec'): at most one of 'load_balancer', 'private_network' could be set.
@@ -573,732 +573,746 @@
 class EndpointSpecLoadBalancer:
     pass
 
 
 @dataclass
 class EndpointSpecPrivateNetwork:
     """
-    Endpoint spec. private network
+    Endpoint spec. private network.
     """
 
     private_network_id: str
     """
-    UUID of the private network to be connected to the database instance
+    UUID of the private network to be connected to the database instance.
     """
 
-    service_ip: str
+    service_ip: Optional[str]
     """
     Endpoint IPv4 adress with a CIDR notation. Check documentation about IP and subnet limitation.
+    
+    One-of ('config'): at most one of 'service_ip', 'ipam_config' could be set.
     """
 
+    ipam_config: Optional[EndpointSpecPrivateNetworkIpamConfig]
+    """
+    Automated configuration of your private network endpoint with Scaleway IPAM service. One at the most per RDB instance or read replica (an RDB instance and its read replica can have different private networks). Cannot be updated (has to be deleted and recreated).
+    
+    One-of ('config'): at most one of 'service_ip', 'ipam_config' could be set.
+    """
+
+
+@dataclass
+class EndpointSpecPrivateNetworkIpamConfig:
+    pass
+
 
 @dataclass
 class EngineSetting:
     """
-    Engine setting
+    Engine setting.
     """
 
     name: str
     """
-    Setting name from database engine
+    Setting name from database engine.
     """
 
     default_value: str
     """
-    Value set when not specified
+    Value set when not specified.
     """
 
     hot_configurable: bool
     """
-    Setting can be applied without restarting
+    Setting can be applied without restarting.
     """
 
     description: str
     """
-    Setting description
+    Setting description.
     """
 
     property_type: EngineSettingPropertyType
     """
-    Setting type
+    Setting type.
     """
 
     unit: Optional[str]
     """
-    Setting base unit
+    Setting base unit.
     """
 
     string_constraint: Optional[str]
     """
-    Validation regex for string type settings
+    Validation regex for string type settings.
     """
 
     int_min: Optional[int]
     """
-    Minimum value for int types
+    Minimum value for int types.
     """
 
     int_max: Optional[int]
     """
-    Maximum value for int types
+    Maximum value for int types.
     """
 
     float_min: Optional[float]
     """
-    Minimum value for float types
+    Minimum value for float types.
     """
 
     float_max: Optional[float]
     """
-    Maximum value for float types
+    Maximum value for float types.
     """
 
 
 @dataclass
 class EngineVersion:
     """
-    Engine version
+    Engine version.
     """
 
     version: str
     """
-    Database engine version
+    Database engine version.
     """
 
     name: str
     """
-    Database engine name
+    Database engine name.
     """
 
     end_of_life: Optional[datetime]
     """
-    End of life date
+    End of life date.
     """
 
     available_settings: List[EngineSetting]
     """
-    Engine settings available to be set
+    Engine settings available to be set.
     """
 
     disabled: bool
     """
-    Disabled versions cannot be created
+    Disabled versions cannot be created.
     """
 
     beta: bool
     """
-    Beta status of engine version
+    Beta status of engine version.
     """
 
     available_init_settings: List[EngineSetting]
     """
-    Engine settings available to be set at database initialisation
+    Engine settings available to be set at database initialisation.
     """
 
 
 @dataclass
 class Instance:
     """
-    Instance
+    Instance.
     """
 
     created_at: Optional[datetime]
     """
-    Creation date (Format ISO 8601)
+    Creation date (Format ISO 8601).
     """
 
     volume: Optional[Volume]
     """
-    Volumes of the instance
+    Volumes of the instance.
     """
 
     region: Region
     """
-    Region the instance is in
+    Region the instance is in.
     """
 
     id: str
     """
-    UUID of the instance
+    UUID of the instance.
     """
 
     name: str
     """
-    Name of the instance
+    Name of the instance.
     """
 
     organization_id: str
     """
-    Organization ID the instance belongs to
+    Organization ID the instance belongs to.
     """
 
     project_id: str
     """
-    Project ID the instance belongs to
+    Project ID the instance belongs to.
     """
 
     status: InstanceStatus
     """
-    Status of the instance
+    Status of the instance.
     """
 
     engine: str
     """
-    Database engine of the database (PostgreSQL, MySQL, ...)
+    Database engine of the database (PostgreSQL, MySQL, ...).
     """
 
     upgradable_version: List[UpgradableVersion]
     """
-    Available database engine versions for upgrade
+    Available database engine versions for upgrade.
     """
 
     endpoint: Optional[Endpoint]
     """
-    Endpoint of the instance
+    Endpoint of the instance.
     :deprecated
     """
 
     tags: List[str]
     """
-    List of tags applied to the instance
+    List of tags applied to the instance.
     """
 
     settings: List[InstanceSetting]
     """
-    Advanced settings of the instance
+    Advanced settings of the instance.
     """
 
     backup_schedule: Optional[BackupSchedule]
     """
-    Backup schedule of the instance
+    Backup schedule of the instance.
     """
 
     is_ha_cluster: bool
     """
-    Whether or not High-Availability is enabled
+    Whether or not High-Availability is enabled.
     """
 
     read_replicas: List[ReadReplica]
     """
-    Read replicas of the instance
+    Read replicas of the instance.
     """
 
     node_type: str
     """
-    Node type of the instance
+    Node type of the instance.
     """
 
     init_settings: List[InstanceSetting]
     """
-    List of engine settings to be set at database initialisation
+    List of engine settings to be set at database initialisation.
     """
 
     endpoints: List[Endpoint]
     """
-    List of instance endpoints
+    List of instance endpoints.
     """
 
     logs_policy: Optional[LogsPolicy]
     """
-    Logs policy of the instance
+    Logs policy of the instance.
     """
 
     backup_same_region: bool
     """
-    Store logical backups in the same region as the database instance
+    Store logical backups in the same region as the database instance.
     """
 
     maintenances: List[Maintenance]
     """
-    List of instance maintenances
+    List of instance maintenances.
     """
 
 
 @dataclass
 class InstanceLog:
     """
-    Instance log
+    Instance log.
     """
 
     download_url: Optional[str]
     """
-    Presigned S3 URL to download your log file
+    Presigned S3 URL to download your log file.
     """
 
     id: str
     """
-    UUID of the instance log
+    UUID of the instance log.
     """
 
     status: InstanceLogStatus
     """
-    Status of the logs in a given instance
+    Status of the logs in a given instance.
     """
 
     node_name: str
     """
-    Name of the undelying node
+    Name of the undelying node.
     """
 
     expires_at: Optional[datetime]
     """
-    Expiration date (Format ISO 8601)
+    Expiration date (Format ISO 8601).
     """
 
     created_at: Optional[datetime]
     """
-    Creation date (Format ISO 8601)
+    Creation date (Format ISO 8601).
     """
 
     region: Region
     """
-    Region the instance is in
+    Region the instance is in.
     """
 
 
 @dataclass
 class InstanceMetrics:
     """
-    Instance metrics
+    Instance metrics.
     """
 
     timeseries: List[TimeSeries]
     """
-    Time series of metrics of a given instance
+    Time series of metrics of a given instance.
     """
 
 
 @dataclass
 class InstanceSetting:
     name: str
 
     value: str
 
 
 @dataclass
 class ListDatabaseBackupsResponse:
     """
-    List database backups response
+    List database backups response.
     """
 
     database_backups: List[DatabaseBackup]
     """
-    List of database backups
+    List of database backups.
     """
 
     total_count: int
     """
-    Total count of database backups available
+    Total count of database backups available.
     """
 
 
 @dataclass
 class ListDatabaseEnginesResponse:
     """
-    List database engines response
+    List database engines response.
     """
 
     engines: List[DatabaseEngine]
     """
-    List of the available database engines
+    List of the available database engines.
     """
 
     total_count: int
     """
-    Total count of database engines available
+    Total count of database engines available.
     """
 
 
 @dataclass
 class ListDatabasesResponse:
     """
-    List databases response
+    List databases response.
     """
 
     databases: List[Database]
     """
-    List of the databases
+    List of the databases.
     """
 
     total_count: int
     """
-    Total count of databases present on a given instance
+    Total count of databases present on a given instance.
     """
 
 
 @dataclass
 class ListInstanceACLRulesResponse:
     """
-    List instance acl rules response
+    List instance acl rules response.
     """
 
     rules: List[ACLRule]
     """
-    List of the ACL rules present on a given instance
+    List of the ACL rules present on a given instance.
     """
 
     total_count: int
     """
-    Total count of ACL rules present on a given instance
+    Total count of ACL rules present on a given instance.
     """
 
 
 @dataclass
 class ListInstanceLogsDetailsResponse:
     """
-    List instance logs details response
+    List instance logs details response.
     """
 
     details: List[ListInstanceLogsDetailsResponseInstanceLogDetail]
     """
-    Remote instance logs details
+    Remote instance logs details.
     """
 
 
 @dataclass
 class ListInstanceLogsDetailsResponseInstanceLogDetail:
     log_name: str
 
     size: int
 
 
 @dataclass
 class ListInstanceLogsResponse:
     """
-    List instance logs response
+    List instance logs response.
     """
 
     instance_logs: List[InstanceLog]
     """
-    Available logs in a given instance
+    Available logs in a given instance.
     """
 
 
 @dataclass
 class ListInstancesResponse:
     """
-    List instances response
+    List instances response.
     """
 
     instances: List[Instance]
     """
-    List all instances available in a given organization/project
+    List all instances available in a given organization/project.
     """
 
     total_count: int
     """
-    Total count of instances available in a given organization/project
+    Total count of instances available in a given organization/project.
     """
 
 
 @dataclass
 class ListNodeTypesResponse:
     """
-    List node types response
+    List node types response.
     """
 
     node_types: List[NodeType]
     """
-    Types of the node
+    Types of the node.
     """
 
     total_count: int
     """
-    Total count of node-types available
+    Total count of node-types available.
     """
 
 
 @dataclass
 class ListPrivilegesResponse:
     """
-    List privileges response
+    List privileges response.
     """
 
     privileges: List[Privilege]
     """
-    Privileges of a given user in a given database in a given instance
+    Privileges of a given user in a given database in a given instance.
     """
 
     total_count: int
     """
-    Total count of privileges present on a given database
+    Total count of privileges present on a given database.
     """
 
 
 @dataclass
 class ListSnapshotsResponse:
     """
-    List snapshots response
+    List snapshots response.
     """
 
     snapshots: List[Snapshot]
     """
-    List of snapshots
+    List of snapshots.
     """
 
     total_count: int
     """
-    Total count of snapshots available
+    Total count of snapshots available.
     """
 
 
 @dataclass
 class ListUsersResponse:
     """
-    List users response
+    List users response.
     """
 
     users: List[User]
     """
-    List of users in a given instance
+    List of users in a given instance.
     """
 
     total_count: int
     """
-    Total count of users present on a given instance
+    Total count of users present on a given instance.
     """
 
 
 @dataclass
 class LogsPolicy:
     """
-    Logs policy
+    Logs policy.
     """
 
     max_age_retention: Optional[int]
     """
-    Max age (in day) of remote logs to keep on the database instance
+    Max age (in day) of remote logs to keep on the database instance.
     """
 
     total_disk_retention: Optional[int]
     """
-    Max disk size of remote logs to keep on the database instance
+    Max disk size of remote logs to keep on the database instance.
     """
 
 
 @dataclass
 class Maintenance:
     """
-    Maintenance
+    Maintenance.
     """
 
     starts_at: Optional[datetime]
     """
-    Start date of the maintenance window
+    Start date of the maintenance window.
     """
 
     stops_at: Optional[datetime]
     """
-    End date of the maintenance window
+    End date of the maintenance window.
     """
 
     closed_at: Optional[datetime]
     """
-    Closed maintenance date
+    Closed maintenance date.
     """
 
     reason: str
     """
-    Maintenance information message
+    Maintenance information message.
     """
 
     status: MaintenanceStatus
     """
-    Status of the maintenance
+    Status of the maintenance.
     """
 
 
 @dataclass
 class NodeType:
     """
-    Node type
+    Node type.
     """
 
     name: str
     """
-    Node Type name identifier
+    Node Type name identifier.
     """
 
     stock_status: NodeTypeStock
     """
-    Current stock status for the Node Type
+    Current stock status for the Node Type.
     """
 
     description: str
     """
-    Current specs of the offer
+    Current specs of the offer.
     """
 
     vcpus: int
     """
-    Number of virtual CPUs
+    Number of virtual CPUs.
     """
 
     memory: int
     """
-    Quantity of RAM
+    Quantity of RAM.
     """
 
     volume_constraint: Optional[NodeTypeVolumeConstraintSizes]
     """
-    [deprecated] Node Type volume constraints
+    [deprecated] Node Type volume constraints.
     :deprecated
     """
 
     is_bssd_compatible: Optional[bool]
     """
-    The Node Type is compliant with Block Storage
+    The Node Type is compliant with Block Storage.
     :deprecated
     """
 
     disabled: bool
     """
-    The Node Type is currently disabled
+    The Node Type is currently disabled.
     """
 
     beta: bool
     """
-    The Node Type is currently in beta
+    The Node Type is currently in beta.
     """
 
     available_volume_types: List[NodeTypeVolumeType]
     """
-    Available storage options for the Node Type
+    Available storage options for the Node Type.
     """
 
     is_ha_required: bool
     """
-    The Node Type can be used only with high availability option
+    The Node Type can be used only with high availability option.
     """
 
     generation: NodeTypeGeneration
     """
-    Generation associated the NodeType offer
+    Generation associated the NodeType offer.
     """
 
     region: Region
     """
-    Region the Node Type is in
+    Region the Node Type is in.
     """
 
 
 @dataclass
 class NodeTypeVolumeConstraintSizes:
     """
-    Node type. volume constraint sizes
+    Node type. volume constraint sizes.
     """
 
     min_size: int
     """
-    [deprecated] Mimimum size required for the Volume
+    [deprecated] Mimimum size required for the Volume.
     """
 
     max_size: int
     """
-    [deprecated] Maximum size required for the Volume
+    [deprecated] Maximum size required for the Volume.
     """
 
 
 @dataclass
 class NodeTypeVolumeType:
     """
-    Node type. volume type
+    Node type. volume type.
     """
 
     type_: VolumeType
     """
-    Volume Type
+    Volume Type.
     """
 
     description: str
     """
-    The description of the Volume
+    The description of the Volume.
     """
 
     min_size: int
     """
-    Mimimum size required for the Volume
+    Mimimum size required for the Volume.
     """
 
     max_size: int
     """
-    Maximum size required for the Volume
+    Maximum size required for the Volume.
     """
 
     chunk_size: int
     """
-    Minimum increment level for a Block Storage volume size
+    Minimum increment level for a Block Storage volume size.
     """
 
 
 @dataclass
 class PrepareInstanceLogsResponse:
     """
-    Prepare instance logs response
+    Prepare instance logs response.
     """
 
     instance_logs: List[InstanceLog]
     """
-    Instance logs for a given instance between a start and an end date
+    Instance logs for a given instance between a start and an end date.
     """
 
 
 @dataclass
 class Privilege:
     """
-    Privilege
+    Privilege.
     """
 
     permission: Permission
     """
-    Permission (Read, Read/Write, All, Custom)
+    Permission (Read, Read/Write, All, Custom).
     """
 
     database_name: str
     """
-    Name of the database
+    Name of the database.
     """
 
     user_name: str
     """
-    Name of the user
+    Name of the user.
     """
 
 
 @dataclass
 class ReadReplica:
     """
-    Read replica
+    Read replica.
     """
 
     id: str
     """
-    UUID of the read replica
+    UUID of the read replica.
     """
 
     endpoints: List[Endpoint]
     """
-    Display read replica connection information
+    Display read replica connection information.
     """
 
     status: ReadReplicaStatus
     """
-    Read replica status
+    Read replica status.
     """
 
     region: Region
     """
-    Region the read replica is in
+    Region the read replica is in.
     """
 
 
 @dataclass
 class ReadReplicaEndpointSpec:
     """
-    Read replica endpoint spec
+    Read replica endpoint spec.
     """
 
     direct_access: Optional[ReadReplicaEndpointSpecDirectAccess]
     """
     Direct access endpoint specifications. Public endpoint reserved for read replicas. One per read replica.
     
     One-of ('spec'): at most one of 'direct_access', 'private_network' could be set.
@@ -1316,111 +1330,125 @@
 class ReadReplicaEndpointSpecDirectAccess:
     pass
 
 
 @dataclass
 class ReadReplicaEndpointSpecPrivateNetwork:
     """
-    Read replica endpoint spec. private network
+    Read replica endpoint spec. private network.
     """
 
     private_network_id: str
     """
-    UUID of the private network to be connected to the read replica
+    UUID of the private network to be connected to the read replica.
     """
 
-    service_ip: str
+    service_ip: Optional[str]
     """
     Endpoint IPv4 adress with a CIDR notation. Check documentation about IP and subnet limitations.
+    
+    One-of ('config'): at most one of 'service_ip', 'ipam_config' could be set.
+    """
+
+    ipam_config: Optional[ReadReplicaEndpointSpecPrivateNetworkIpamConfig]
+    """
+    Automated configuration of your private network endpoint with Scaleway IPAM service. One at the most per RDB instance or read replica (an RDB instance and its read replica can have different private networks). Cannot be updated (has to be deleted and recreated).
+    
+    One-of ('config'): at most one of 'service_ip', 'ipam_config' could be set.
     """
 
 
 @dataclass
+class ReadReplicaEndpointSpecPrivateNetworkIpamConfig:
+    pass
+
+
+@dataclass
 class SetInstanceACLRulesResponse:
     """
-    Set instance acl rules response
+    Set instance acl rules response.
     """
 
     rules: List[ACLRule]
     """
-    ACLs rules configured for an instance
+    ACLs rules configured for an instance.
     """
 
 
 @dataclass
 class SetInstanceSettingsResponse:
     """
-    Set instance settings response
+    Set instance settings response.
     """
 
     settings: List[InstanceSetting]
     """
-    Settings configured for a given instance
+    Settings configured for a given instance.
     """
 
 
 @dataclass
 class Snapshot:
     """
-    Snapshot
+    Snapshot.
     """
 
     id: str
     """
-    UUID of the snapshot
+    UUID of the snapshot.
     """
 
     instance_id: str
     """
-    UUID of the instance
+    UUID of the instance.
     """
 
     name: str
     """
-    Name of the snapshot
+    Name of the snapshot.
     """
 
     status: SnapshotStatus
     """
-    Status of the snapshot
+    Status of the snapshot.
     """
 
     size: Optional[int]
     """
-    Size of the snapshot
+    Size of the snapshot.
     """
 
     expires_at: Optional[datetime]
     """
-    Expiration date (Format ISO 8601)
+    Expiration date (Format ISO 8601).
     """
 
     created_at: Optional[datetime]
     """
-    Creation date (Format ISO 8601)
+    Creation date (Format ISO 8601).
     """
 
     updated_at: Optional[datetime]
     """
-    Updated date (Format ISO 8601)
+    Updated date (Format ISO 8601).
     """
 
     instance_name: str
     """
-    Name of the instance of the snapshot
+    Name of the instance of the snapshot.
     """
 
     node_type: str
     """
-    Source node type
+    Source node type.
     """
 
     region: Region
     """
-    Region of this snapshot
+    Region of this snapshot.
     """
 
 
 @dataclass
 class UpgradableVersion:
     id: str
 
@@ -1430,234 +1458,234 @@
 
     minor_version: str
 
 
 @dataclass
 class User:
     """
-    User
+    User.
     """
 
     name: str
     """
-    Name of the user (Length must be between 1 and 63 characters, The max Length is 32 for MySQL engines, First character must be an alphabet character (a-zA-Z), Your Username cannot start with '_rdb', Only a-zA-Z0-9_$- characters are accepted)
+    Name of the user (Length must be between 1 and 63 characters, The max Length is 32 for MySQL engines, First character must be an alphabet character (a-zA-Z), Your Username cannot start with '_rdb', Only a-zA-Z0-9_$- characters are accepted).
     """
 
     is_admin: bool
     """
-    Whether or not a user got administrative privileges on the database instance
+    Whether or not a user got administrative privileges on the database instance.
     """
 
 
 @dataclass
 class Volume:
     type_: VolumeType
 
     size: int
 
 
 @dataclass
 class ListDatabaseEnginesRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     name: Optional[str]
     """
-    Name of the Database Engine
+    Name of the Database Engine.
     """
 
     version: Optional[str]
     """
-    Version of the Database Engine
+    Version of the Database Engine.
     """
 
     page: Optional[int]
 
     page_size: Optional[int]
 
 
 @dataclass
 class ListNodeTypesRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     include_disabled_types: bool
     """
-    Whether or not to include disabled types
+    Whether or not to include disabled types.
     """
 
     page: Optional[int]
 
     page_size: Optional[int]
 
 
 @dataclass
 class ListDatabaseBackupsRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     name: Optional[str]
     """
-    Name of the database backups
+    Name of the database backups.
     """
 
     order_by: Optional[ListDatabaseBackupsRequestOrderBy]
     """
-    Criteria to use when ordering database backups listing
+    Criteria to use when ordering database backups listing.
     """
 
     instance_id: Optional[str]
     """
-    UUID of the instance
+    UUID of the instance.
     """
 
     organization_id: Optional[str]
     """
-    Organization ID the database backups belongs to
+    Organization ID the database backups belongs to.
     """
 
     project_id: Optional[str]
     """
-    Project ID the database backups belongs to
+    Project ID the database backups belongs to.
     """
 
     page: Optional[int]
 
     page_size: Optional[int]
 
 
 @dataclass
 class CreateDatabaseBackupRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance
+    UUID of the instance.
     """
 
     database_name: str
     """
-    Name of the database you want to make a backup of
+    Name of the database you want to make a backup of.
     """
 
     name: Optional[str]
     """
-    Name of the backup
+    Name of the backup.
     """
 
     expires_at: Optional[datetime]
     """
-    Expiration date (Format ISO 8601)
+    Expiration date (Format ISO 8601).
     """
 
 
 @dataclass
 class GetDatabaseBackupRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     database_backup_id: str
     """
-    UUID of the database backup
+    UUID of the database backup.
     """
 
 
 @dataclass
 class UpdateDatabaseBackupRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     database_backup_id: str
     """
-    UUID of the database backup to update
+    UUID of the database backup to update.
     """
 
     name: Optional[str]
     """
-    Name of the Database Backup
+    Name of the Database Backup.
     """
 
     expires_at: Optional[datetime]
     """
-    Expiration date (Format ISO 8601)
+    Expiration date (Format ISO 8601).
     """
 
 
 @dataclass
 class DeleteDatabaseBackupRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     database_backup_id: str
     """
-    UUID of the database backup to delete
+    UUID of the database backup to delete.
     """
 
 
 @dataclass
 class RestoreDatabaseBackupRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     database_backup_id: str
     """
-    Backup of a logical database
+    Backup of a logical database.
     """
 
     database_name: Optional[str]
     """
-    Defines the destination database in order to restore into a specified database, the default destination is set to the origin database of the backup
+    Defines the destination database in order to restore into a specified database, the default destination is set to the origin database of the backup.
     """
 
     instance_id: str
     """
-    Defines the rdb instance where the backup has to be restored
+    Defines the rdb instance where the backup has to be restored.
     """
 
 
 @dataclass
 class ExportDatabaseBackupRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     database_backup_id: str
     """
-    UUID of the database backup you want to export
+    UUID of the database backup you want to export.
     """
 
 
 @dataclass
 class UpgradeInstanceRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance you want to upgrade
+    UUID of the instance you want to upgrade.
     """
 
     node_type: Optional[str]
     """
     Node type of the instance you want to upgrade to.
     
     One-of ('upgrade_target'): at most one of 'node_type', 'enable_ha', 'volume_size', 'volume_type', 'upgradable_version_id' could be set.
@@ -1692,65 +1720,65 @@
     """
 
 
 @dataclass
 class ListInstancesRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     tags: Optional[List[str]]
     """
-    List instance that have a given tags
+    List instance that have a given tags.
     """
 
     name: Optional[str]
     """
-    List instance that match a given name pattern
+    List instance that match a given name pattern.
     """
 
     order_by: Optional[ListInstancesRequestOrderBy]
     """
-    Criteria to use when ordering instance listing
+    Criteria to use when ordering instance listing.
     """
 
     organization_id: Optional[str]
     """
-    Please use `project_id` instead
+    Please use `project_id` instead.
     """
 
     project_id: Optional[str]
     """
-    Project ID to list the instance of
+    Project ID to list the instance of.
     """
 
     page: Optional[int]
 
     page_size: Optional[int]
 
 
 @dataclass
 class GetInstanceRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance
+    UUID of the instance.
     """
 
 
 @dataclass
 class CreateInstanceRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     organization_id: Optional[str]
     """
     Please use `project_id` instead.
     
     One-of ('project_identifier'): at most one of 'organization_id', 'project_id' could be set.
@@ -1762,920 +1790,938 @@
     The project ID on which to create the instance.
     
     One-of ('project_identifier'): at most one of 'organization_id', 'project_id' could be set.
     """
 
     name: Optional[str]
     """
-    Name of the instance
+    Name of the instance.
     """
 
     engine: str
     """
-    Database engine of the database (PostgreSQL, MySQL, ...)
+    Database engine of the database (PostgreSQL, MySQL, ...).
     """
 
     user_name: str
     """
-    Name of the user created when the instance is created
+    Name of the user created when the instance is created.
     """
 
     password: str
     """
-    Password of the user
+    Password of the user.
     """
 
     node_type: str
     """
-    Type of node to use for the instance
+    Type of node to use for the instance.
     """
 
     is_ha_cluster: bool
     """
-    Whether or not High-Availability is enabled
+    Whether or not High-Availability is enabled.
     """
 
     disable_backup: bool
     """
-    Whether or not backups are disabled
+    Whether or not backups are disabled.
     """
 
     tags: Optional[List[str]]
     """
-    Tags to apply to the instance
+    Tags to apply to the instance.
     """
 
     init_settings: Optional[List[InstanceSetting]]
     """
-    List of engine settings to be set at database initialisation
+    List of engine settings to be set at database initialisation.
     """
 
     volume_type: VolumeType
     """
-    Type of volume where data are stored (lssd, bssd, ...)
+    Type of volume where data are stored (lssd, bssd, ...).
     """
 
     volume_size: int
     """
-    Volume size when volume_type is not lssd
+    Volume size when volume_type is not lssd.
     """
 
     init_endpoints: Optional[List[EndpointSpec]]
     """
-    One or multiple EndpointSpec used to expose your database instance. A load_balancer public endpoint is systematically created
+    One or multiple EndpointSpec used to expose your database instance. A load_balancer public endpoint is systematically created.
     """
 
     backup_same_region: bool
     """
-    Store logical backups in the same region as the database instance
+    Store logical backups in the same region as the database instance.
     """
 
 
 @dataclass
 class UpdateInstanceRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance to update
+    UUID of the instance to update.
     """
 
     backup_schedule_frequency: Optional[int]
     """
-    In hours
+    In hours.
     """
 
     backup_schedule_retention: Optional[int]
     """
-    In days
+    In days.
     """
 
     is_backup_schedule_disabled: Optional[bool]
     """
-    Whether or not the backup schedule is disabled
+    Whether or not the backup schedule is disabled.
     """
 
     name: Optional[str]
     """
-    Name of the instance
+    Name of the instance.
     """
 
     tags: Optional[List[str]]
     """
-    Tags of a given instance
+    Tags of a given instance.
     """
 
     logs_policy: Optional[LogsPolicy]
     """
-    Logs policy of the instance
+    Logs policy of the instance.
     """
 
     backup_same_region: Optional[bool]
     """
-    Store logical backups in the same region as the database instance
+    Store logical backups in the same region as the database instance.
     """
 
 
 @dataclass
 class DeleteInstanceRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance to delete
+    UUID of the instance to delete.
     """
 
 
 @dataclass
 class CloneInstanceRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance you want to clone
+    UUID of the instance you want to clone.
     """
 
     name: str
     """
-    Name of the clone instance
+    Name of the clone instance.
     """
 
     node_type: Optional[str]
     """
-    Node type of the clone
+    Node type of the clone.
     """
 
 
 @dataclass
 class RestartInstanceRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance you want to restart
+    UUID of the instance you want to restart.
     """
 
 
 @dataclass
 class GetInstanceCertificateRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance
+    UUID of the instance.
     """
 
 
 @dataclass
 class RenewInstanceCertificateRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance you want logs of
+    UUID of the instance you want logs of.
     """
 
 
 @dataclass
 class GetInstanceMetricsRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance
+    UUID of the instance.
     """
 
     start_date: Optional[datetime]
     """
-    Start date to gather metrics from
+    Start date to gather metrics from.
     """
 
     end_date: Optional[datetime]
     """
-    End date to gather metrics from
+    End date to gather metrics from.
     """
 
     metric_name: Optional[str]
     """
-    Name of the metric to gather
+    Name of the metric to gather.
     """
 
 
 @dataclass
 class CreateReadReplicaRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance you want a read replica of
+    UUID of the instance you want a read replica of.
     """
 
     endpoint_spec: Optional[List[ReadReplicaEndpointSpec]]
     """
-    Specification of the endpoint you want to create
+    Specification of the endpoint you want to create.
     """
 
 
 @dataclass
 class GetReadReplicaRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     read_replica_id: str
     """
-    UUID of the read replica
+    UUID of the read replica.
     """
 
 
 @dataclass
 class DeleteReadReplicaRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     read_replica_id: str
     """
-    UUID of the read replica
+    UUID of the read replica.
     """
 
 
 @dataclass
 class ResetReadReplicaRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     read_replica_id: str
     """
-    UUID of the read replica
+    UUID of the read replica.
     """
 
 
 @dataclass
 class CreateReadReplicaEndpointRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     read_replica_id: str
     """
-    UUID of the read replica
+    UUID of the read replica.
     """
 
     endpoint_spec: List[ReadReplicaEndpointSpec]
     """
-    Specification of the endpoint you want to create
+    Specification of the endpoint you want to create.
     """
 
 
 @dataclass
 class PrepareInstanceLogsRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance you want logs of
+    UUID of the instance you want logs of.
     """
 
     start_date: Optional[datetime]
     """
-    Start datetime of your log. Format: `{year}-{month}-{day}T{hour}:{min}:{sec}[.{frac_sec}]Z`
+    Start datetime of your log. Format: `{year}-{month}-{day}T{hour}:{min}:{sec}[.{frac_sec}]Z`.
     """
 
     end_date: Optional[datetime]
     """
-    End datetime of your log. Format: `{year}-{month}-{day}T{hour}:{min}:{sec}[.{frac_sec}]Z`
+    End datetime of your log. Format: `{year}-{month}-{day}T{hour}:{min}:{sec}[.{frac_sec}]Z`.
     """
 
 
 @dataclass
 class ListInstanceLogsRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance you want logs of
+    UUID of the instance you want logs of.
     """
 
     order_by: ListInstanceLogsRequestOrderBy
     """
-    Criteria to use when ordering instance logs listing
+    Criteria to use when ordering instance logs listing.
     """
 
 
 @dataclass
 class GetInstanceLogRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_log_id: str
     """
-    UUID of the instance_log you want
+    UUID of the instance_log you want.
     """
 
 
 @dataclass
 class PurgeInstanceLogsRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance you want logs of
+    UUID of the instance you want logs of.
     """
 
     log_name: Optional[str]
     """
-    Specific log name to purge
+    Specific log name to purge.
     """
 
 
 @dataclass
 class ListInstanceLogsDetailsRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance you want logs of
+    UUID of the instance you want logs of.
     """
 
 
 @dataclass
 class AddInstanceSettingsRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance you want to add settings to
+    UUID of the instance you want to add settings to.
     """
 
     settings: List[InstanceSetting]
     """
-    Settings to add on the instance
+    Settings to add on the instance.
     """
 
 
 @dataclass
 class DeleteInstanceSettingsRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance to delete settings from
+    UUID of the instance to delete settings from.
     """
 
     setting_names: List[str]
     """
-    Settings names to delete
+    Settings names to delete.
     """
 
 
 @dataclass
 class SetInstanceSettingsRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance where the settings has to be set
+    UUID of the instance where the settings has to be set.
     """
 
     settings: List[InstanceSetting]
     """
-    Settings to define for the instance
+    Settings to define for the instance.
     """
 
 
 @dataclass
 class ListInstanceACLRulesRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance
+    UUID of the instance.
     """
 
     page: Optional[int]
 
     page_size: Optional[int]
 
 
 @dataclass
 class AddInstanceACLRulesRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance you want to add acl rules to
+    UUID of the instance you want to add acl rules to.
     """
 
     rules: List[ACLRuleRequest]
     """
-    ACLs rules to add to the instance
+    ACLs rules to add to the instance.
     """
 
 
 @dataclass
 class SetInstanceACLRulesRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance where the ACL rules has to be set
+    UUID of the instance where the ACL rules has to be set.
     """
 
     rules: List[ACLRuleRequest]
     """
-    ACL rules to define for the instance
+    ACL rules to define for the instance.
     """
 
 
 @dataclass
 class DeleteInstanceACLRulesRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance you want to delete an ACL rules from
+    UUID of the instance you want to delete an ACL rules from.
     """
 
     acl_rule_ips: List[str]
     """
-    ACL rules IP present on the instance
+    ACL rules IP present on the instance.
     """
 
 
 @dataclass
 class ListUsersRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance
+    UUID of the instance.
     """
 
     name: Optional[str]
     """
-    Name of the user
+    Name of the user.
     """
 
     order_by: Optional[ListUsersRequestOrderBy]
     """
-    Criteria to use when ordering users listing
+    Criteria to use when ordering users listing.
     """
 
     page: Optional[int]
 
     page_size: Optional[int]
 
 
 @dataclass
 class CreateUserRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance you want to create a user in
+    UUID of the instance you want to create a user in.
     """
 
     name: str
     """
-    Name of the user you want to create
+    Name of the user you want to create.
     """
 
     password: str
     """
-    Password of the user you want to create
+    Password of the user you want to create.
     """
 
     is_admin: bool
     """
-    Whether the user you want to create will have administrative privileges
+    Whether the user you want to create will have administrative privileges.
     """
 
 
 @dataclass
 class UpdateUserRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance the user belongs to
+    UUID of the instance the user belongs to.
     """
 
     name: str
     """
-    Name of the database user
+    Name of the database user.
     """
 
     password: Optional[str]
     """
-    Password of the database user
+    Password of the database user.
     """
 
     is_admin: Optional[bool]
     """
-    Whether or not this user got administrative privileges
+    Whether or not this user got administrative privileges.
     """
 
 
 @dataclass
 class DeleteUserRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance to delete a user from
+    UUID of the instance to delete a user from.
     """
 
     name: str
     """
-    Name of the user
+    Name of the user.
     """
 
 
 @dataclass
 class ListDatabasesRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance to list database of
+    UUID of the instance to list database of.
     """
 
     name: Optional[str]
     """
-    Name of the database
+    Name of the database.
     """
 
     managed: Optional[bool]
     """
-    Whether or not the database is managed
+    Whether or not the database is managed.
     """
 
     owner: Optional[str]
     """
-    User that owns this database
+    User that owns this database.
     """
 
     order_by: Optional[ListDatabasesRequestOrderBy]
     """
-    Criteria to use when ordering database listing
+    Criteria to use when ordering database listing.
     """
 
     page: Optional[int]
 
     page_size: Optional[int]
 
 
 @dataclass
 class CreateDatabaseRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance where to create the database
+    UUID of the instance where to create the database.
     """
 
     name: str
     """
-    Name of the database
+    Name of the database.
     """
 
 
 @dataclass
 class DeleteDatabaseRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance where to delete the database
+    UUID of the instance where to delete the database.
     """
 
     name: str
     """
-    Name of the database to delete
+    Name of the database to delete.
     """
 
 
 @dataclass
 class ListPrivilegesRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance
+    UUID of the instance.
     """
 
     order_by: Optional[ListPrivilegesRequestOrderBy]
     """
-    Criteria to use when ordering privileges listing
+    Criteria to use when ordering privileges listing.
     """
 
     page: Optional[int]
 
     page_size: Optional[int]
 
     database_name: Optional[str]
     """
-    Name of the database
+    Name of the database.
     """
 
     user_name: Optional[str]
     """
-    Name of the user
+    Name of the user.
     """
 
 
 @dataclass
 class SetPrivilegeRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance
+    UUID of the instance.
     """
 
     database_name: str
     """
-    Name of the database
+    Name of the database.
     """
 
     user_name: str
     """
-    Name of the user
+    Name of the user.
     """
 
     permission: Permission
     """
-    Permission to set (Read, Read/Write, All, Custom)
+    Permission to set (Read, Read/Write, All, Custom).
     """
 
 
 @dataclass
 class ListSnapshotsRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     name: Optional[str]
     """
-    Name of the snapshot
+    Name of the snapshot.
     """
 
     order_by: Optional[ListSnapshotsRequestOrderBy]
     """
-    Criteria to use when ordering snapshot listing
+    Criteria to use when ordering snapshot listing.
     """
 
     instance_id: Optional[str]
     """
-    UUID of the instance
+    UUID of the instance.
     """
 
     organization_id: Optional[str]
     """
-    Organization ID the snapshots belongs to
+    Organization ID the snapshots belongs to.
     """
 
     project_id: Optional[str]
     """
-    Project ID the snapshots belongs to
+    Project ID the snapshots belongs to.
     """
 
     page: Optional[int]
 
     page_size: Optional[int]
 
 
 @dataclass
 class GetSnapshotRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     snapshot_id: str
     """
-    UUID of the snapshot
+    UUID of the snapshot.
     """
 
 
 @dataclass
 class CreateSnapshotRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance
+    UUID of the instance.
     """
 
     name: Optional[str]
     """
-    Name of the snapshot
+    Name of the snapshot.
     """
 
     expires_at: Optional[datetime]
     """
-    Expiration date (Format ISO 8601)
+    Expiration date (Format ISO 8601).
     """
 
 
 @dataclass
 class UpdateSnapshotRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     snapshot_id: str
     """
-    UUID of the snapshot to update
+    UUID of the snapshot to update.
     """
 
     name: Optional[str]
     """
-    Name of the snapshot
+    Name of the snapshot.
     """
 
     expires_at: Optional[datetime]
     """
-    Expiration date (Format ISO 8601)
+    Expiration date (Format ISO 8601).
     """
 
 
 @dataclass
 class DeleteSnapshotRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     snapshot_id: str
     """
-    UUID of the snapshot to delete
+    UUID of the snapshot to delete.
     """
 
 
 @dataclass
 class CreateInstanceFromSnapshotRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     snapshot_id: str
     """
-    Block snapshot of the instance
+    Block snapshot of the instance.
     """
 
     instance_name: str
     """
-    Name of the instance created with the snapshot
+    Name of the instance created with the snapshot.
     """
 
     is_ha_cluster: Optional[bool]
     """
-    Whether or not High-Availability is enabled on the new instance
+    Whether or not High-Availability is enabled on the new instance.
     """
 
     node_type: Optional[str]
     """
-    The node type used to restore the snapshot
+    The node type used to restore the snapshot.
     """
 
 
 @dataclass
 class CreateEndpointRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     instance_id: str
     """
-    UUID of the instance you want to add endpoint to
+    UUID of the instance you want to add endpoint to.
     """
 
     endpoint_spec: Optional[EndpointSpec]
     """
-    Specification of the endpoint you want to create
+    Specification of the endpoint you want to create.
     """
 
 
 @dataclass
 class DeleteEndpointRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     endpoint_id: str
     """
     This endpoint can also be used to delete a read replica endpoint.
     """
 
 
 @dataclass
 class GetEndpointRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     endpoint_id: str
     """
-    UUID of the endpoint you want to get
+    UUID of the endpoint you want to get.
+    """
+
+
+@dataclass
+class MigrateEndpointRequest:
+    region: Optional[Region]
+    """
+    Region to target. If none is passed will use default region from the config.
+    """
+
+    endpoint_id: str
+    """
+    UUID of the endpoint you want to migrate.
+    """
+
+    instance_id: str
+    """
+    UUID of the instance you want to attach the endpoint to.
     """
```

### Comparing `scaleway_async-0.8.0/scaleway_async/redis/v1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/redis/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/redis/v1/api.py` & `scaleway_async-0.9.0/scaleway_async/redis/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/redis/v1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/redis/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/redis/v1/types.py` & `scaleway_async-0.9.0/scaleway_async/redis/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/registry/v1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/registry/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/registry/v1/api.py` & `scaleway_async-0.9.0/scaleway_async/registry/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/registry/v1/content.py` & `scaleway_async-0.9.0/scaleway_async/registry/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/registry/v1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/registry/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/registry/v1/types.py` & `scaleway_async-0.9.0/scaleway_async/registry/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/secret/v1alpha1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/secret/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/secret/v1alpha1/api.py` & `scaleway_async-0.9.0/scaleway_async/secret/v1alpha1/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -51,19 +51,19 @@
         region: Optional[Region] = None,
         project_id: Optional[str] = None,
         tags: Optional[List[str]] = None,
         description: Optional[str] = None,
     ) -> Secret:
         """
         Create a Secret containing no versions
-        :param region: Region to target. If none is passed will use default region from the config
-        :param project_id: ID of the project containing the Secret
-        :param name: Name of the Secret
-        :param tags: List of tags associated to this Secret
-        :param description: Description of the Secret
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param project_id: ID of the project containing the Secret.
+        :param name: Name of the Secret.
+        :param tags: List of tags associated to this Secret.
+        :param description: Description of the Secret.
         :return: :class:`Secret <Secret>`
 
         Usage:
         ::
 
             result = await api.create_secret(name="example")
         """
@@ -94,16 +94,16 @@
         self,
         *,
         secret_id: str,
         region: Optional[Region] = None,
     ) -> Secret:
         """
         Get metadata of a Secret
-        :param region: Region to target. If none is passed will use default region from the config
-        :param secret_id: ID of the Secret
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param secret_id: ID of the Secret.
         :return: :class:`Secret <Secret>`
 
         Usage:
         ::
 
             result = await api.get_secret(secret_id="example")
         """
@@ -117,30 +117,61 @@
             "GET",
             f"/secret-manager/v1alpha1/regions/{param_region}/secrets/{param_secret_id}",
         )
 
         self._throw_on_error(res)
         return unmarshal_Secret(res.json())
 
+    async def get_secret_by_name(
+        self,
+        *,
+        secret_name: str,
+        region: Optional[Region] = None,
+    ) -> Secret:
+        """
+        Get metadata of a Secret
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param secret_name: Name of the Secret.
+        :return: :class:`Secret <Secret>`
+
+        Usage:
+        ::
+
+            result = await api.get_secret_by_name(secret_name="example")
+        """
+
+        param_region = validate_path_param(
+            "region", region or self.client.default_region
+        )
+        param_secret_name = validate_path_param("secret_name", secret_name)
+
+        res = self._request(
+            "GET",
+            f"/secret-manager/v1alpha1/regions/{param_region}/secrets-by-name/{param_secret_name}",
+        )
+
+        self._throw_on_error(res)
+        return unmarshal_Secret(res.json())
+
     async def update_secret(
         self,
         *,
         secret_id: str,
         region: Optional[Region] = None,
         name: Optional[str] = None,
         tags: Optional[List[str]] = None,
         description: Optional[str] = None,
     ) -> Secret:
         """
         Update metadata of a Secret
-        :param region: Region to target. If none is passed will use default region from the config
-        :param secret_id: ID of the Secret
-        :param name: New name of the Secret (optional)
-        :param tags: New list of tags associated to this Secret (optional)
-        :param description: Description of the Secret
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param secret_id: ID of the Secret.
+        :param name: New name of the Secret (optional).
+        :param tags: New list of tags associated to this Secret (optional).
+        :param description: Description of the Secret.
         :return: :class:`Secret <Secret>`
 
         Usage:
         ::
 
             result = await api.update_secret(secret_id="example")
         """
@@ -170,25 +201,27 @@
 
     async def list_secrets(
         self,
         *,
         region: Optional[Region] = None,
         organization_id: Optional[str] = None,
         project_id: Optional[str] = None,
+        name: Optional[str] = None,
         tags: Optional[List[str]] = None,
         order_by: ListSecretsRequestOrderBy = ListSecretsRequestOrderBy.NAME_ASC,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> ListSecretsResponse:
         """
         List Secrets
-        :param region: Region to target. If none is passed will use default region from the config
-        :param organization_id: ID of an organization to filter on (optional)
-        :param project_id: ID of a project to filter on (optional)
-        :param tags: List of tags to filter on (optional)
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param organization_id: ID of an organization to filter on (optional).
+        :param project_id: ID of a project to filter on (optional).
+        :param name: Secret name to filter on (optional).
+        :param tags: List of tags to filter on (optional).
         :param order_by:
         :param page:
         :param page_size:
         :return: :class:`ListSecretsResponse <ListSecretsResponse>`
 
         Usage:
         ::
@@ -200,14 +233,15 @@
             "region", region or self.client.default_region
         )
 
         res = self._request(
             "GET",
             f"/secret-manager/v1alpha1/regions/{param_region}/secrets",
             params={
+                "name": name,
                 "order_by": order_by,
                 "organization_id": organization_id
                 or self.client.default_organization_id,
                 "page": page,
                 "page_size": page_size or self.client.default_page_size,
                 "project_id": project_id or self.client.default_project_id,
                 "tags": tags,
@@ -219,25 +253,27 @@
 
     async def list_secrets_all(
         self,
         *,
         region: Optional[Region] = None,
         organization_id: Optional[str] = None,
         project_id: Optional[str] = None,
+        name: Optional[str] = None,
         tags: Optional[List[str]] = None,
         order_by: Optional[ListSecretsRequestOrderBy] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[Secret]:
         """
         List Secrets
-        :param region: Region to target. If none is passed will use default region from the config
-        :param organization_id: ID of an organization to filter on (optional)
-        :param project_id: ID of a project to filter on (optional)
-        :param tags: List of tags to filter on (optional)
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param organization_id: ID of an organization to filter on (optional).
+        :param project_id: ID of a project to filter on (optional).
+        :param name: Secret name to filter on (optional).
+        :param tags: List of tags to filter on (optional).
         :param order_by:
         :param page:
         :param page_size:
         :return: :class:`List[ListSecretsResponse] <List[ListSecretsResponse]>`
 
         Usage:
         ::
@@ -249,14 +285,15 @@
             type=ListSecretsResponse,
             key="secrets",
             fetcher=self.list_secrets,
             args={
                 "region": region,
                 "organization_id": organization_id,
                 "project_id": project_id,
+                "name": name,
                 "tags": tags,
                 "order_by": order_by,
                 "page": page,
                 "page_size": page_size,
             },
         )
 
@@ -264,16 +301,16 @@
         self,
         *,
         secret_id: str,
         region: Optional[Region] = None,
     ) -> Optional[None]:
         """
         Delete a secret
-        :param region: Region to target. If none is passed will use default region from the config
-        :param secret_id: ID of the Secret
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param secret_id: ID of the Secret.
 
         Usage:
         ::
 
             result = await api.delete_secret(secret_id="example")
         """
 
@@ -296,18 +333,18 @@
         secret_id: str,
         data: str,
         region: Optional[Region] = None,
         description: Optional[str] = None,
     ) -> SecretVersion:
         """
         Create a SecretVersion
-        :param region: Region to target. If none is passed will use default region from the config
-        :param secret_id: ID of the Secret
-        :param data: The base64-encoded secret payload of the SecretVersion
-        :param description: Description of the SecretVersion
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param secret_id: ID of the Secret.
+        :param data: The base64-encoded secret payload of the SecretVersion.
+        :param description: Description of the SecretVersion.
         :return: :class:`SecretVersion <SecretVersion>`
 
         Usage:
         ::
 
             result = await api.create_secret_version(
                 secret_id="example",
@@ -342,17 +379,17 @@
         *,
         secret_id: str,
         revision: str,
         region: Optional[Region] = None,
     ) -> SecretVersion:
         """
         Get metadata of a SecretVersion
-        :param region: Region to target. If none is passed will use default region from the config
-        :param secret_id: ID of the Secret
-        :param revision: Revision of the SecretVersion (may be a number or "latest")
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param secret_id: ID of the Secret.
+        :param revision: Revision of the SecretVersion (may be a number or "latest").
         :return: :class:`SecretVersion <SecretVersion>`
 
         Usage:
         ::
 
             result = await api.get_secret_version(
                 secret_id="example",
@@ -370,28 +407,65 @@
             "GET",
             f"/secret-manager/v1alpha1/regions/{param_region}/secrets/{param_secret_id}/versions/{param_revision}",
         )
 
         self._throw_on_error(res)
         return unmarshal_SecretVersion(res.json())
 
+    async def get_secret_version_by_name(
+        self,
+        *,
+        secret_name: str,
+        revision: str,
+        region: Optional[Region] = None,
+    ) -> SecretVersion:
+        """
+        Get metadata of a SecretVersion
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param secret_name: Name of the Secret.
+        :param revision: Revision of the SecretVersion (may be a number or "latest").
+        :return: :class:`SecretVersion <SecretVersion>`
+
+        Usage:
+        ::
+
+            result = await api.get_secret_version_by_name(
+                secret_name="example",
+                revision="example",
+            )
+        """
+
+        param_region = validate_path_param(
+            "region", region or self.client.default_region
+        )
+        param_secret_name = validate_path_param("secret_name", secret_name)
+        param_revision = validate_path_param("revision", revision)
+
+        res = self._request(
+            "GET",
+            f"/secret-manager/v1alpha1/regions/{param_region}/secrets-by-name/{param_secret_name}/versions/{param_revision}",
+        )
+
+        self._throw_on_error(res)
+        return unmarshal_SecretVersion(res.json())
+
     async def update_secret_version(
         self,
         *,
         secret_id: str,
         revision: str,
         region: Optional[Region] = None,
         description: Optional[str] = None,
     ) -> SecretVersion:
         """
         Update metadata of a SecretVersion
-        :param region: Region to target. If none is passed will use default region from the config
-        :param secret_id: ID of the Secret
-        :param revision: Revision of the SecretVersion (may be a number or "latest")
-        :param description: Description of the SecretVersion
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param secret_id: ID of the Secret.
+        :param revision: Revision of the SecretVersion (may be a number or "latest").
+        :param description: Description of the SecretVersion.
         :return: :class:`SecretVersion <SecretVersion>`
 
         Usage:
         ::
 
             result = await api.update_secret_version(
                 secret_id="example",
@@ -429,19 +503,19 @@
         region: Optional[Region] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
         status: Optional[List[SecretVersionStatus]] = None,
     ) -> ListSecretVersionsResponse:
         """
         List versions of a secret, not returning any sensitive data
-        :param region: Region to target. If none is passed will use default region from the config
-        :param secret_id: ID of the Secret
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param secret_id: ID of the Secret.
         :param page:
         :param page_size:
-        :param status: Filter results by status
+        :param status: Filter results by status.
         :return: :class:`ListSecretVersionsResponse <ListSecretVersionsResponse>`
 
         Usage:
         ::
 
             result = await api.list_secret_versions(secret_id="example")
         """
@@ -471,19 +545,19 @@
         region: Optional[Region] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
         status: Optional[List[SecretVersionStatus]] = None,
     ) -> List[SecretVersion]:
         """
         List versions of a secret, not returning any sensitive data
-        :param region: Region to target. If none is passed will use default region from the config
-        :param secret_id: ID of the Secret
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param secret_id: ID of the Secret.
         :param page:
         :param page_size:
-        :param status: Filter results by status
+        :param status: Filter results by status.
         :return: :class:`List[ListSecretVersionsResponse] <List[ListSecretVersionsResponse]>`
 
         Usage:
         ::
 
             result = await api.list_secret_versions_all(secret_id="example")
         """
@@ -497,26 +571,105 @@
                 "region": region,
                 "page": page,
                 "page_size": page_size,
                 "status": status,
             },
         )
 
+    async def list_secret_versions_by_name(
+        self,
+        *,
+        secret_name: str,
+        region: Optional[Region] = None,
+        page: Optional[int] = None,
+        page_size: Optional[int] = None,
+        status: Optional[List[SecretVersionStatus]] = None,
+    ) -> ListSecretVersionsResponse:
+        """
+        List versions of a secret, not returning any sensitive data
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param secret_name: Name of the Secret.
+        :param page:
+        :param page_size:
+        :param status: Filter results by status.
+        :return: :class:`ListSecretVersionsResponse <ListSecretVersionsResponse>`
+
+        Usage:
+        ::
+
+            result = await api.list_secret_versions_by_name(secret_name="example")
+        """
+
+        param_region = validate_path_param(
+            "region", region or self.client.default_region
+        )
+        param_secret_name = validate_path_param("secret_name", secret_name)
+
+        res = self._request(
+            "GET",
+            f"/secret-manager/v1alpha1/regions/{param_region}/secrets-by-name/{param_secret_name}/versions",
+            params={
+                "page": page,
+                "page_size": page_size or self.client.default_page_size,
+                "status": status,
+            },
+        )
+
+        self._throw_on_error(res)
+        return unmarshal_ListSecretVersionsResponse(res.json())
+
+    async def list_secret_versions_by_name_all(
+        self,
+        *,
+        secret_name: str,
+        region: Optional[Region] = None,
+        page: Optional[int] = None,
+        page_size: Optional[int] = None,
+        status: Optional[List[SecretVersionStatus]] = None,
+    ) -> List[SecretVersion]:
+        """
+        List versions of a secret, not returning any sensitive data
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param secret_name: Name of the Secret.
+        :param page:
+        :param page_size:
+        :param status: Filter results by status.
+        :return: :class:`List[ListSecretVersionsResponse] <List[ListSecretVersionsResponse]>`
+
+        Usage:
+        ::
+
+            result = await api.list_secret_versions_by_name_all(secret_name="example")
+        """
+
+        return await fetch_all_pages_async(
+            type=ListSecretVersionsResponse,
+            key="versions",
+            fetcher=self.list_secret_versions_by_name,
+            args={
+                "secret_name": secret_name,
+                "region": region,
+                "page": page,
+                "page_size": page_size,
+                "status": status,
+            },
+        )
+
     async def destroy_secret_version(
         self,
         *,
         secret_id: str,
         revision: str,
         region: Optional[Region] = None,
     ) -> SecretVersion:
         """
         Destroy a SecretVersion, permanently destroying the sensitive data
-        :param region: Region to target. If none is passed will use default region from the config
-        :param secret_id: ID of the Secret
-        :param revision: Revision of the SecretVersion (may be a number or "latest")
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param secret_id: ID of the Secret.
+        :param revision: Revision of the SecretVersion (may be a number or "latest").
         :return: :class:`SecretVersion <SecretVersion>`
 
         Usage:
         ::
 
             result = await api.destroy_secret_version(
                 secret_id="example",
@@ -543,17 +696,17 @@
         *,
         secret_id: str,
         revision: str,
         region: Optional[Region] = None,
     ) -> SecretVersion:
         """
         Enable a SecretVersion
-        :param region: Region to target. If none is passed will use default region from the config
-        :param secret_id: ID of the Secret
-        :param revision: Revision of the SecretVersion (may be a number or "latest")
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param secret_id: ID of the Secret.
+        :param revision: Revision of the SecretVersion (may be a number or "latest").
         :return: :class:`SecretVersion <SecretVersion>`
 
         Usage:
         ::
 
             result = await api.enable_secret_version(
                 secret_id="example",
@@ -580,17 +733,17 @@
         *,
         secret_id: str,
         revision: str,
         region: Optional[Region] = None,
     ) -> SecretVersion:
         """
         Disable a SecretVersion
-        :param region: Region to target. If none is passed will use default region from the config
-        :param secret_id: ID of the Secret
-        :param revision: Revision of the SecretVersion (may be a number or "latest")
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param secret_id: ID of the Secret.
+        :param revision: Revision of the SecretVersion (may be a number or "latest").
         :return: :class:`SecretVersion <SecretVersion>`
 
         Usage:
         ::
 
             result = await api.disable_secret_version(
                 secret_id="example",
@@ -617,17 +770,17 @@
         *,
         secret_id: str,
         revision: str,
         region: Optional[Region] = None,
     ) -> AccessSecretVersionResponse:
         """
         Access a SecretVersion, returning the sensitive data
-        :param region: Region to target. If none is passed will use default region from the config
-        :param secret_id: ID of the Secret
-        :param revision: Revision of the SecretVersion (may be a number or "latest")
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param secret_id: ID of the Secret.
+        :param revision: Revision of the SecretVersion (may be a number or "latest").
         :return: :class:`AccessSecretVersionResponse <AccessSecretVersionResponse>`
 
         Usage:
         ::
 
             result = await api.access_secret_version(
                 secret_id="example",
@@ -644,7 +797,44 @@
         res = self._request(
             "GET",
             f"/secret-manager/v1alpha1/regions/{param_region}/secrets/{param_secret_id}/versions/{param_revision}/access",
         )
 
         self._throw_on_error(res)
         return unmarshal_AccessSecretVersionResponse(res.json())
+
+    async def access_secret_version_by_name(
+        self,
+        *,
+        secret_name: str,
+        revision: str,
+        region: Optional[Region] = None,
+    ) -> AccessSecretVersionResponse:
+        """
+        Access a SecretVersion, returning the sensitive data
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param secret_name: Name of the Secret.
+        :param revision: Revision of the SecretVersion (may be a number or "latest").
+        :return: :class:`AccessSecretVersionResponse <AccessSecretVersionResponse>`
+
+        Usage:
+        ::
+
+            result = await api.access_secret_version_by_name(
+                secret_name="example",
+                revision="example",
+            )
+        """
+
+        param_region = validate_path_param(
+            "region", region or self.client.default_region
+        )
+        param_secret_name = validate_path_param("secret_name", secret_name)
+        param_revision = validate_path_param("revision", revision)
+
+        res = self._request(
+            "GET",
+            f"/secret-manager/v1alpha1/regions/{param_region}/secrets-by-name/{param_secret_name}/versions/{param_revision}/access",
+        )
+
+        self._throw_on_error(res)
+        return unmarshal_AccessSecretVersionResponse(res.json())
```

### Comparing `scaleway_async-0.8.0/scaleway_async/secret/v1alpha1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/secret/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/secret/v1alpha1/types.py` & `scaleway_async-0.9.0/scaleway_async/secret/v1alpha1/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,427 +41,501 @@
     def __str__(self) -> str:
         return str(self.value)
 
 
 @dataclass
 class AccessSecretVersionResponse:
     """
-    Access secret version response
+    Access secret version response.
     """
 
     secret_id: str
     """
-    ID of the Secret
+    ID of the Secret.
     """
 
     revision: int
     """
-    Revision of the SecretVersion
+    Revision of the SecretVersion.
     """
 
     data: str
     """
-    The base64-encoded secret payload of the SecretVersion
+    The base64-encoded secret payload of the SecretVersion.
     """
 
 
 @dataclass
 class ListSecretVersionsResponse:
     """
-    List secret versions response
+    List secret versions response.
     """
 
     total_count: int
     """
-    Count of all SecretVersions
+    Count of all SecretVersions.
     """
 
     versions: List[SecretVersion]
     """
-    Single page of SecretVersions
+    Single page of SecretVersions.
     """
 
 
 @dataclass
 class ListSecretsResponse:
     """
-    List secrets response
+    List secrets response.
     """
 
     total_count: int
     """
-    Count of all Secrets matching the requested criteria
+    Count of all Secrets matching the requested criteria.
     """
 
     secrets: List[Secret]
     """
-    Single page of Secrets matching the requested criteria
+    Single page of Secrets matching the requested criteria.
     """
 
 
 @dataclass
 class Secret:
     """
-    Secret
+    Secret.
     """
 
     id: str
     """
-    ID of the Secret
+    ID of the Secret.
     """
 
     project_id: str
     """
-    ID of the project containing the Secret
+    ID of the project containing the Secret.
     """
 
     name: str
     """
-    Name of the Secret
+    Name of the Secret.
     """
 
     status: SecretStatus
     """
     * `ready`: the Secret is ready.
     * `locked`: the Secret is locked.
-    
     """
 
     created_at: Optional[datetime]
     """
-    The time at which the Secret was created
+    The time at which the Secret was created.
     """
 
     updated_at: Optional[datetime]
     """
-    The time at which the Secret was updated
+    The time at which the Secret was updated.
     """
 
     tags: List[str]
     """
-    List of tags associated to this Secret
+    List of tags associated to this Secret.
     """
 
     region: Region
     """
-    Region of the Secret
+    Region of the Secret.
     """
 
     version_count: int
     """
-    The number of versions for this Secret
+    The number of versions for this Secret.
     """
 
     description: Optional[str]
     """
-    Description of the Secret
+    Description of the Secret.
     """
 
 
 @dataclass
 class SecretVersion:
     """
-    Secret version
+    Secret version.
     """
 
     secret_id: str
     """
-    ID of the Secret
+    ID of the Secret.
     """
 
     revision: int
     """
-    Revision of the SecretVersion
+    Revision of the SecretVersion.
     """
 
     status: SecretVersionStatus
     """
     * `unknown`: the SecretVersion is in an invalid state.
     * `enabled`: the SecretVersion is accessible.
     * `disabled`: the SecretVersion is not accessible but can be enabled.
     * `destroyed`: the SecretVersion is permanently destroyed.
-    
     """
 
     created_at: Optional[datetime]
     """
-    The time at which the SecretVersion was created
+    The time at which the SecretVersion was created.
     """
 
     updated_at: Optional[datetime]
     """
-    The time at which the SecretVersion was updated
+    The time at which the SecretVersion was updated.
     """
 
     description: Optional[str]
     """
-    Description of the SecretVersion
+    Description of the SecretVersion.
     """
 
 
 @dataclass
 class CreateSecretRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     project_id: Optional[str]
     """
-    ID of the project containing the Secret
+    ID of the project containing the Secret.
     """
 
     name: str
     """
-    Name of the Secret
+    Name of the Secret.
     """
 
     tags: Optional[List[str]]
     """
-    List of tags associated to this Secret
+    List of tags associated to this Secret.
     """
 
     description: Optional[str]
     """
-    Description of the Secret
+    Description of the Secret.
     """
 
 
 @dataclass
 class GetSecretRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     secret_id: str
     """
-    ID of the Secret
+    ID of the Secret.
+    """
+
+
+@dataclass
+class GetSecretByNameRequest:
+    region: Optional[Region]
+    """
+    Region to target. If none is passed will use default region from the config.
+    """
+
+    secret_name: str
+    """
+    Name of the Secret.
     """
 
 
 @dataclass
 class UpdateSecretRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     secret_id: str
     """
-    ID of the Secret
+    ID of the Secret.
     """
 
     name: Optional[str]
     """
-    New name of the Secret (optional)
+    New name of the Secret (optional).
     """
 
     tags: Optional[List[str]]
     """
-    New list of tags associated to this Secret (optional)
+    New list of tags associated to this Secret (optional).
     """
 
     description: Optional[str]
     """
-    Description of the Secret
+    Description of the Secret.
     """
 
 
 @dataclass
 class ListSecretsRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     organization_id: Optional[str]
     """
-    ID of an organization to filter on (optional)
+    ID of an organization to filter on (optional).
     """
 
     project_id: Optional[str]
     """
-    ID of a project to filter on (optional)
+    ID of a project to filter on (optional).
+    """
+
+    name: Optional[str]
+    """
+    Secret name to filter on (optional).
     """
 
     tags: Optional[List[str]]
     """
-    List of tags to filter on (optional)
+    List of tags to filter on (optional).
     """
 
     order_by: Optional[ListSecretsRequestOrderBy]
 
     page: Optional[int]
 
     page_size: Optional[int]
 
 
 @dataclass
 class DeleteSecretRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     secret_id: str
     """
-    ID of the Secret
+    ID of the Secret.
     """
 
 
 @dataclass
 class CreateSecretVersionRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     secret_id: str
     """
-    ID of the Secret
+    ID of the Secret.
     """
 
     data: str
     """
-    The base64-encoded secret payload of the SecretVersion
+    The base64-encoded secret payload of the SecretVersion.
     """
 
     description: Optional[str]
     """
-    Description of the SecretVersion
+    Description of the SecretVersion.
     """
 
 
 @dataclass
 class GetSecretVersionRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     secret_id: str
     """
-    ID of the Secret
+    ID of the Secret.
+    """
+
+    revision: str
+    """
+    Revision of the SecretVersion (may be a number or "latest").
+    """
+
+
+@dataclass
+class GetSecretVersionByNameRequest:
+    region: Optional[Region]
+    """
+    Region to target. If none is passed will use default region from the config.
+    """
+
+    secret_name: str
+    """
+    Name of the Secret.
     """
 
     revision: str
     """
-    Revision of the SecretVersion (may be a number or "latest")
+    Revision of the SecretVersion (may be a number or "latest").
     """
 
 
 @dataclass
 class UpdateSecretVersionRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     secret_id: str
     """
-    ID of the Secret
+    ID of the Secret.
     """
 
     revision: str
     """
-    Revision of the SecretVersion (may be a number or "latest")
+    Revision of the SecretVersion (may be a number or "latest").
     """
 
     description: Optional[str]
     """
-    Description of the SecretVersion
+    Description of the SecretVersion.
     """
 
 
 @dataclass
 class ListSecretVersionsRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     secret_id: str
     """
-    ID of the Secret
+    ID of the Secret.
+    """
+
+    page: Optional[int]
+
+    page_size: Optional[int]
+
+    status: Optional[List[SecretVersionStatus]]
+    """
+    Filter results by status.
+    """
+
+
+@dataclass
+class ListSecretVersionsByNameRequest:
+    region: Optional[Region]
+    """
+    Region to target. If none is passed will use default region from the config.
+    """
+
+    secret_name: str
+    """
+    Name of the Secret.
     """
 
     page: Optional[int]
 
     page_size: Optional[int]
 
     status: Optional[List[SecretVersionStatus]]
     """
-    Filter results by status
+    Filter results by status.
     """
 
 
 @dataclass
 class DestroySecretVersionRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     secret_id: str
     """
-    ID of the Secret
+    ID of the Secret.
     """
 
     revision: str
     """
-    Revision of the SecretVersion (may be a number or "latest")
+    Revision of the SecretVersion (may be a number or "latest").
     """
 
 
 @dataclass
 class EnableSecretVersionRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     secret_id: str
     """
-    ID of the Secret
+    ID of the Secret.
     """
 
     revision: str
     """
-    Revision of the SecretVersion (may be a number or "latest")
+    Revision of the SecretVersion (may be a number or "latest").
     """
 
 
 @dataclass
 class DisableSecretVersionRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     secret_id: str
     """
-    ID of the Secret
+    ID of the Secret.
     """
 
     revision: str
     """
-    Revision of the SecretVersion (may be a number or "latest")
+    Revision of the SecretVersion (may be a number or "latest").
     """
 
 
 @dataclass
 class AccessSecretVersionRequest:
     region: Optional[Region]
     """
-    Region to target. If none is passed will use default region from the config
+    Region to target. If none is passed will use default region from the config.
     """
 
     secret_id: str
     """
-    ID of the Secret
+    ID of the Secret.
+    """
+
+    revision: str
+    """
+    Revision of the SecretVersion (may be a number or "latest").
+    """
+
+
+@dataclass
+class AccessSecretVersionByNameRequest:
+    region: Optional[Region]
+    """
+    Region to target. If none is passed will use default region from the config.
+    """
+
+    secret_name: str
+    """
+    Name of the Secret.
     """
 
     revision: str
     """
-    Revision of the SecretVersion (may be a number or "latest")
+    Revision of the SecretVersion (may be a number or "latest").
     """
```

### Comparing `scaleway_async-0.8.0/scaleway_async/tem/v1alpha1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/tem/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/tem/v1alpha1/api.py` & `scaleway_async-0.9.0/scaleway_async/tem/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/tem/v1alpha1/content.py` & `scaleway_async-0.9.0/scaleway_async/tem/v1alpha1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/tem/v1alpha1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/tem/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/tem/v1alpha1/types.py` & `scaleway_async-0.9.0/scaleway_async/tem/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/test/v1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/test/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/test/v1/api.py` & `scaleway_async-0.9.0/scaleway_async/test/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/test/v1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/test/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/test/v1/types.py` & `scaleway_async-0.9.0/scaleway_async/test/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/vpc/v1/api.py` & `scaleway_async-0.9.0/scaleway_async/vpc/v1/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,23 +43,23 @@
         tags: Optional[List[str]] = None,
         organization_id: Optional[str] = None,
         project_id: Optional[str] = None,
         private_network_ids: Optional[List[str]] = None,
     ) -> ListPrivateNetworksResponse:
         """
         List private networks
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param order_by: The sort order of the returned private networks
-        :param page: The page number for the returned private networks
-        :param page_size: The maximum number of private networks per page
-        :param name: Filter private networks with names containing this string
-        :param tags: Filter private networks with one or more matching tags
-        :param organization_id: The organization ID on which to filter the returned private networks
-        :param project_id: The project ID on which to filter the returned private networks
-        :param private_network_ids: The PrivateNetwork IDs on which to filter the returned private networks
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param order_by: The sort order of the returned private networks.
+        :param page: The page number for the returned private networks.
+        :param page_size: The maximum number of private networks per page.
+        :param name: Filter private networks with names containing this string.
+        :param tags: Filter private networks with one or more matching tags.
+        :param organization_id: The organization ID on which to filter the returned private networks.
+        :param project_id: The project ID on which to filter the returned private networks.
+        :param private_network_ids: The PrivateNetwork IDs on which to filter the returned private networks.
         :return: :class:`ListPrivateNetworksResponse <ListPrivateNetworksResponse>`
 
         Usage:
         ::
 
             result = await api.list_private_networks()
         """
@@ -96,23 +96,23 @@
         tags: Optional[List[str]] = None,
         organization_id: Optional[str] = None,
         project_id: Optional[str] = None,
         private_network_ids: Optional[List[str]] = None,
     ) -> List[PrivateNetwork]:
         """
         List private networks
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param order_by: The sort order of the returned private networks
-        :param page: The page number for the returned private networks
-        :param page_size: The maximum number of private networks per page
-        :param name: Filter private networks with names containing this string
-        :param tags: Filter private networks with one or more matching tags
-        :param organization_id: The organization ID on which to filter the returned private networks
-        :param project_id: The project ID on which to filter the returned private networks
-        :param private_network_ids: The PrivateNetwork IDs on which to filter the returned private networks
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param order_by: The sort order of the returned private networks.
+        :param page: The page number for the returned private networks.
+        :param page_size: The maximum number of private networks per page.
+        :param name: Filter private networks with names containing this string.
+        :param tags: Filter private networks with one or more matching tags.
+        :param organization_id: The organization ID on which to filter the returned private networks.
+        :param project_id: The project ID on which to filter the returned private networks.
+        :param private_network_ids: The PrivateNetwork IDs on which to filter the returned private networks.
         :return: :class:`List[ListPrivateNetworksResponse] <List[ListPrivateNetworksResponse]>`
 
         Usage:
         ::
 
             result = await api.list_private_networks_all()
         """
@@ -141,19 +141,19 @@
         name: Optional[str] = None,
         project_id: Optional[str] = None,
         tags: Optional[List[str]] = None,
         subnets: Optional[List[str]] = None,
     ) -> PrivateNetwork:
         """
         Create a private network
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param name: The name of the private network
-        :param project_id: The project ID of the private network
-        :param tags: The private networks tags
-        :param subnets: Private network subnets CIDR
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param name: The name of the private network.
+        :param project_id: The project ID of the private network.
+        :param tags: The private networks tags.
+        :param subnets: Private network subnets CIDR.
         :return: :class:`PrivateNetwork <PrivateNetwork>`
 
         Usage:
         ::
 
             result = await api.create_private_network()
         """
@@ -182,16 +182,16 @@
         self,
         *,
         private_network_id: str,
         zone: Optional[Zone] = None,
     ) -> PrivateNetwork:
         """
         Get a private network
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param private_network_id: The private network id
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param private_network_id: The private network id.
         :return: :class:`PrivateNetwork <PrivateNetwork>`
 
         Usage:
         ::
 
             result = await api.get_private_network(private_network_id="example")
         """
@@ -216,19 +216,19 @@
         zone: Optional[Zone] = None,
         name: Optional[str] = None,
         tags: Optional[List[str]] = None,
         subnets: Optional[List[str]] = None,
     ) -> PrivateNetwork:
         """
         Update private network
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param private_network_id: The private network ID
-        :param name: The name of the private network
-        :param tags: The private networks tags
-        :param subnets: Private network subnets CIDR (deprecated)
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param private_network_id: The private network ID.
+        :param name: The name of the private network.
+        :param tags: The private networks tags.
+        :param subnets: Private network subnets CIDR (deprecated).
         :return: :class:`PrivateNetwork <PrivateNetwork>`
 
         Usage:
         ::
 
             result = await api.update_private_network(private_network_id="example")
         """
@@ -260,16 +260,16 @@
         self,
         *,
         private_network_id: str,
         zone: Optional[Zone] = None,
     ) -> Optional[None]:
         """
         Delete a private network
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param private_network_id: The private network ID
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param private_network_id: The private network ID.
 
         Usage:
         ::
 
             result = await api.delete_private_network(private_network_id="example")
         """
```

### Comparing `scaleway_async-0.8.0/scaleway_async/vpc/v1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/vpc/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/vpc/v1/types.py` & `scaleway_async-0.9.0/scaleway_async/vpc/v1/types.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,185 +28,185 @@
 
     total_count: int
 
 
 @dataclass
 class PrivateNetwork:
     """
-    Private network
+    Private network.
     """
 
     id: str
     """
-    The private network ID
+    The private network ID.
     """
 
     name: str
     """
-    The private network name
+    The private network name.
     """
 
     organization_id: str
     """
-    The private network organization
+    The private network organization.
     """
 
     project_id: str
     """
-    The private network project ID
+    The private network project ID.
     """
 
     zone: Zone
     """
-    The zone in which the private network is available
+    The zone in which the private network is available.
     """
 
     tags: List[str]
     """
-    The private network tags
+    The private network tags.
     """
 
     created_at: Optional[datetime]
     """
-    The private network creation date
+    The private network creation date.
     """
 
     updated_at: Optional[datetime]
     """
-    The last private network modification date
+    The last private network modification date.
     """
 
     subnets: List[str]
     """
-    Private network subnets CIDR
+    Private network subnets CIDR.
     """
 
 
 @dataclass
 class ListPrivateNetworksRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     order_by: Optional[ListPrivateNetworksRequestOrderBy]
     """
-    The sort order of the returned private networks
+    The sort order of the returned private networks.
     """
 
     page: Optional[int]
     """
-    The page number for the returned private networks
+    The page number for the returned private networks.
     """
 
     page_size: Optional[int]
     """
-    The maximum number of private networks per page
+    The maximum number of private networks per page.
     """
 
     name: Optional[str]
     """
-    Filter private networks with names containing this string
+    Filter private networks with names containing this string.
     """
 
     tags: Optional[List[str]]
     """
-    Filter private networks with one or more matching tags
+    Filter private networks with one or more matching tags.
     """
 
     organization_id: Optional[str]
     """
-    The organization ID on which to filter the returned private networks
+    The organization ID on which to filter the returned private networks.
     """
 
     project_id: Optional[str]
     """
-    The project ID on which to filter the returned private networks
+    The project ID on which to filter the returned private networks.
     """
 
     private_network_ids: Optional[List[str]]
     """
-    The PrivateNetwork IDs on which to filter the returned private networks
+    The PrivateNetwork IDs on which to filter the returned private networks.
     """
 
 
 @dataclass
 class CreatePrivateNetworkRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     name: Optional[str]
     """
-    The name of the private network
+    The name of the private network.
     """
 
     project_id: Optional[str]
     """
-    The project ID of the private network
+    The project ID of the private network.
     """
 
     tags: Optional[List[str]]
     """
-    The private networks tags
+    The private networks tags.
     """
 
     subnets: Optional[List[str]]
     """
-    Private network subnets CIDR
+    Private network subnets CIDR.
     """
 
 
 @dataclass
 class GetPrivateNetworkRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     private_network_id: str
     """
-    The private network id
+    The private network id.
     """
 
 
 @dataclass
 class UpdatePrivateNetworkRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     private_network_id: str
     """
-    The private network ID
+    The private network ID.
     """
 
     name: Optional[str]
     """
-    The name of the private network
+    The name of the private network.
     """
 
     tags: Optional[List[str]]
     """
-    The private networks tags
+    The private networks tags.
     """
 
     subnets: Optional[List[str]]
     """
-    Private network subnets CIDR (deprecated)
+    Private network subnets CIDR (deprecated).
     :deprecated
     """
 
 
 @dataclass
 class DeletePrivateNetworkRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     private_network_id: str
     """
-    The private network ID
+    The private network ID.
     """
```

### Comparing `scaleway_async-0.8.0/scaleway_async/vpcgw/v1/__init__.py` & `scaleway_async-0.9.0/scaleway_async/vpcgw/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/vpcgw/v1/api.py` & `scaleway_async-0.9.0/scaleway_async/vpcgw/v1/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,16 +58,16 @@
     UpdateIPRequest,
 )
 from .content import (
     GATEWAY_NETWORK_TRANSIENT_STATUSES,
     GATEWAY_TRANSIENT_STATUSES,
 )
 from .marshalling import (
-    marshal_CreateDHCPEntryRequest,
     marshal_CreateDHCPRequest,
+    marshal_CreateDHCPEntryRequest,
     marshal_CreateGatewayNetworkRequest,
     marshal_CreateGatewayRequest,
     marshal_CreateIPRequest,
     marshal_CreatePATRuleRequest,
     marshal_SetDHCPEntriesRequest,
     marshal_SetPATRulesRequest,
     marshal_UpdateDHCPEntryRequest,
@@ -112,25 +112,25 @@
         tags: Optional[List[str]] = None,
         type_: Optional[str] = None,
         status: GatewayStatus = GatewayStatus.UNKNOWN,
         private_network_id: Optional[str] = None,
     ) -> ListGatewaysResponse:
         """
         List VPC Public Gateways
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param order_by: Order in which to return results
-        :param page: Page number
-        :param page_size: Gateways per page
-        :param organization_id: Include only gateways in this organization
-        :param project_id: Include only gateways in this project
-        :param name: Filter gateways including this name
-        :param tags: Filter gateways with these tags
-        :param type_: Filter gateways of this type
-        :param status: Filter gateways in this status (unknown for any)
-        :param private_network_id: Filter gateways attached to this private network
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param order_by: Order in which to return results.
+        :param page: Page number.
+        :param page_size: Gateways per page.
+        :param organization_id: Include only gateways in this organization.
+        :param project_id: Include only gateways in this project.
+        :param name: Filter gateways including this name.
+        :param tags: Filter gateways with these tags.
+        :param type_: Filter gateways of this type.
+        :param status: Filter gateways in this status (unknown for any).
+        :param private_network_id: Filter gateways attached to this private network.
         :return: :class:`ListGatewaysResponse <ListGatewaysResponse>`
 
         Usage:
         ::
 
             result = await api.list_gateways()
         """
@@ -171,25 +171,25 @@
         tags: Optional[List[str]] = None,
         type_: Optional[str] = None,
         status: Optional[GatewayStatus] = None,
         private_network_id: Optional[str] = None,
     ) -> List[Gateway]:
         """
         List VPC Public Gateways
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param order_by: Order in which to return results
-        :param page: Page number
-        :param page_size: Gateways per page
-        :param organization_id: Include only gateways in this organization
-        :param project_id: Include only gateways in this project
-        :param name: Filter gateways including this name
-        :param tags: Filter gateways with these tags
-        :param type_: Filter gateways of this type
-        :param status: Filter gateways in this status (unknown for any)
-        :param private_network_id: Filter gateways attached to this private network
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param order_by: Order in which to return results.
+        :param page: Page number.
+        :param page_size: Gateways per page.
+        :param organization_id: Include only gateways in this organization.
+        :param project_id: Include only gateways in this project.
+        :param name: Filter gateways including this name.
+        :param tags: Filter gateways with these tags.
+        :param type_: Filter gateways of this type.
+        :param status: Filter gateways in this status (unknown for any).
+        :param private_network_id: Filter gateways attached to this private network.
         :return: :class:`List[ListGatewaysResponse] <List[ListGatewaysResponse]>`
 
         Usage:
         ::
 
             result = await api.list_gateways_all()
         """
@@ -217,16 +217,16 @@
         self,
         *,
         gateway_id: str,
         zone: Optional[Zone] = None,
     ) -> Gateway:
         """
         Get a VPC Public Gateway
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param gateway_id: ID of the gateway to fetch
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param gateway_id: ID of the gateway to fetch.
         :return: :class:`Gateway <Gateway>`
 
         Usage:
         ::
 
             result = await api.get_gateway(gateway_id="example")
         """
@@ -247,16 +247,16 @@
         *,
         gateway_id: str,
         zone: Optional[Zone] = None,
         options: Optional[WaitForOptions[Gateway, Union[bool, Awaitable[bool]]]] = None,
     ) -> Gateway:
         """
         Waits for :class:`Gateway <Gateway>` to be in a final state.
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param gateway_id: ID of the gateway to fetch
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param gateway_id: ID of the gateway to fetch.
         :param options: The options for the waiter
         :return: :class:`Gateway <Gateway>`
 
         Usage:
         ::
 
             result = api.wait_for_gateway(gateway_id="example")
@@ -289,24 +289,24 @@
         tags: Optional[List[str]] = None,
         upstream_dns_servers: Optional[List[str]] = None,
         ip_id: Optional[str] = None,
         bastion_port: Optional[int] = None,
     ) -> Gateway:
         """
         Create a VPC Public Gateway
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param project_id: Project to create the gateway into
-        :param name: Name of the gateway
-        :param tags: Tags for the gateway
-        :param type_: Gateway type
-        :param upstream_dns_servers: Override the gateway's default recursive DNS servers, if DNS features are enabled
-        :param ip_id: Attach an existing IP to the gateway
-        :param enable_smtp: Allow SMTP traffic to pass through the gateway
-        :param enable_bastion: Enable SSH bastion on the gateway
-        :param bastion_port: Port of the SSH bastion
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param project_id: Project to create the gateway into.
+        :param name: Name of the gateway.
+        :param tags: Tags for the gateway.
+        :param type_: Gateway type.
+        :param upstream_dns_servers: Override the gateway's default recursive DNS servers, if DNS features are enabled.
+        :param ip_id: Attach an existing IP to the gateway.
+        :param enable_smtp: Allow SMTP traffic to pass through the gateway.
+        :param enable_bastion: Enable SSH bastion on the gateway.
+        :param bastion_port: Port of the SSH bastion.
         :return: :class:`Gateway <Gateway>`
 
         Usage:
         ::
 
             result = await api.create_gateway(
                 type_="example",
@@ -350,22 +350,22 @@
         upstream_dns_servers: Optional[List[str]] = None,
         enable_bastion: Optional[bool] = None,
         bastion_port: Optional[int] = None,
         enable_smtp: Optional[bool] = None,
     ) -> Gateway:
         """
         Update a VPC Public Gateway
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param gateway_id: ID of the gateway to update
-        :param name: Name fo the gateway
-        :param tags: Tags for the gateway
-        :param upstream_dns_servers: Override the gateway's default recursive DNS servers, if DNS features are enabled
-        :param enable_bastion: Enable SSH bastion on the gateway
-        :param bastion_port: Port of the SSH bastion
-        :param enable_smtp: Allow SMTP traffic to pass through the gateway
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param gateway_id: ID of the gateway to update.
+        :param name: Name fo the gateway.
+        :param tags: Tags for the gateway.
+        :param upstream_dns_servers: Override the gateway's default recursive DNS servers, if DNS features are enabled.
+        :param enable_bastion: Enable SSH bastion on the gateway.
+        :param bastion_port: Port of the SSH bastion.
+        :param enable_smtp: Allow SMTP traffic to pass through the gateway.
         :return: :class:`Gateway <Gateway>`
 
         Usage:
         ::
 
             result = await api.update_gateway(gateway_id="example")
         """
@@ -399,19 +399,18 @@
         *,
         gateway_id: str,
         cleanup_dhcp: bool,
         zone: Optional[Zone] = None,
     ) -> Optional[None]:
         """
         Delete a VPC Public Gateway
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param gateway_id: ID of the gateway to delete
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param gateway_id: ID of the gateway to delete.
         :param cleanup_dhcp: Whether to cleanup attached DHCP configurations (if any, and if not attached to another Gateway Network).
 
-
         Usage:
         ::
 
             result = await api.delete_gateway(
                 gateway_id="example",
                 cleanup_dhcp=True,
             )
@@ -435,16 +434,16 @@
         self,
         *,
         gateway_id: str,
         zone: Optional[Zone] = None,
     ) -> Gateway:
         """
         Upgrade a VPC Public Gateway to the latest version
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param gateway_id: ID of the gateway to upgrade
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param gateway_id: ID of the gateway to upgrade.
         :return: :class:`Gateway <Gateway>`
 
         Usage:
         ::
 
             result = await api.upgrade_gateway(gateway_id="example")
         """
@@ -471,23 +470,23 @@
         private_network_id: Optional[str] = None,
         enable_masquerade: Optional[bool] = None,
         dhcp_id: Optional[str] = None,
         status: GatewayNetworkStatus = GatewayNetworkStatus.UNKNOWN,
     ) -> ListGatewayNetworksResponse:
         """
         List gateway connections to Private Networks
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param order_by: Order in which to return results
-        :param page: Page number
-        :param page_size: GatewayNetworks per page
-        :param gateway_id: Filter by gateway
-        :param private_network_id: Filter by private network
-        :param enable_masquerade: Filter by masquerade enablement
-        :param dhcp_id: Filter by DHCP configuration
-        :param status: Filter GatewayNetworks by this status (unknown for any)
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param order_by: Order in which to return results.
+        :param page: Page number.
+        :param page_size: GatewayNetworks per page.
+        :param gateway_id: Filter by gateway.
+        :param private_network_id: Filter by private network.
+        :param enable_masquerade: Filter by masquerade enablement.
+        :param dhcp_id: Filter by DHCP configuration.
+        :param status: Filter GatewayNetworks by this status (unknown for any).
         :return: :class:`ListGatewayNetworksResponse <ListGatewayNetworksResponse>`
 
         Usage:
         ::
 
             result = await api.list_gateway_networks()
         """
@@ -523,23 +522,23 @@
         private_network_id: Optional[str] = None,
         enable_masquerade: Optional[bool] = None,
         dhcp_id: Optional[str] = None,
         status: Optional[GatewayNetworkStatus] = None,
     ) -> List[GatewayNetwork]:
         """
         List gateway connections to Private Networks
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param order_by: Order in which to return results
-        :param page: Page number
-        :param page_size: GatewayNetworks per page
-        :param gateway_id: Filter by gateway
-        :param private_network_id: Filter by private network
-        :param enable_masquerade: Filter by masquerade enablement
-        :param dhcp_id: Filter by DHCP configuration
-        :param status: Filter GatewayNetworks by this status (unknown for any)
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param order_by: Order in which to return results.
+        :param page: Page number.
+        :param page_size: GatewayNetworks per page.
+        :param gateway_id: Filter by gateway.
+        :param private_network_id: Filter by private network.
+        :param enable_masquerade: Filter by masquerade enablement.
+        :param dhcp_id: Filter by DHCP configuration.
+        :param status: Filter GatewayNetworks by this status (unknown for any).
         :return: :class:`List[ListGatewayNetworksResponse] <List[ListGatewayNetworksResponse]>`
 
         Usage:
         ::
 
             result = await api.list_gateway_networks_all()
         """
@@ -565,16 +564,16 @@
         self,
         *,
         gateway_network_id: str,
         zone: Optional[Zone] = None,
     ) -> GatewayNetwork:
         """
         Get a gateway connection to a Private Network
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param gateway_network_id: ID of the GatewayNetwork to fetch
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param gateway_network_id: ID of the GatewayNetwork to fetch.
         :return: :class:`GatewayNetwork <GatewayNetwork>`
 
         Usage:
         ::
 
             result = await api.get_gateway_network(gateway_network_id="example")
         """
@@ -599,16 +598,16 @@
         zone: Optional[Zone] = None,
         options: Optional[
             WaitForOptions[GatewayNetwork, Union[bool, Awaitable[bool]]]
         ] = None,
     ) -> GatewayNetwork:
         """
         Waits for :class:`GatewayNetwork <GatewayNetwork>` to be in a final state.
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param gateway_network_id: ID of the GatewayNetwork to fetch
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param gateway_network_id: ID of the GatewayNetwork to fetch.
         :param options: The options for the waiter
         :return: :class:`GatewayNetwork <GatewayNetwork>`
 
         Usage:
         ::
 
             result = api.wait_for_gateway_network(gateway_network_id="example")
@@ -635,31 +634,34 @@
         self,
         *,
         gateway_id: str,
         private_network_id: str,
         enable_masquerade: bool,
         zone: Optional[Zone] = None,
         dhcp_id: Optional[str] = None,
+        dhcp: Optional[CreateDHCPRequest] = None,
         address: Optional[str] = None,
         enable_dhcp: Optional[bool] = None,
     ) -> GatewayNetwork:
         """
         Attach a gateway to a Private Network
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param gateway_id: Gateway to connect
-        :param private_network_id: Private Network to connect
-        :param enable_masquerade: Whether to enable masquerade on this network
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param gateway_id: Gateway to connect.
+        :param private_network_id: Private Network to connect.
+        :param enable_masquerade: Whether to enable masquerade on this network.
         :param dhcp_id: Existing configuration.
 
-        One-of ('ip_config'): at most one of 'dhcp_id', 'address' could be set.
+        One-of ('ip_config'): at most one of 'dhcp_id', 'dhcp', 'address' could be set.
+        :param dhcp: New DHCP configuration.
+
+        One-of ('ip_config'): at most one of 'dhcp_id', 'dhcp', 'address' could be set.
         :param address: Static IP address in CIDR format to to use without DHCP.
 
-        One-of ('ip_config'): at most one of 'dhcp_id', 'address' could be set.
+        One-of ('ip_config'): at most one of 'dhcp_id', 'dhcp', 'address' could be set.
         :param enable_dhcp: Whether to enable DHCP on this Private Network. Defaults to `true` if either `dhcp_id` or `dhcp` short: are present. If set to `true`, requires that either `dhcp_id` or `dhcp` to be present.
-
         :return: :class:`GatewayNetwork <GatewayNetwork>`
 
         Usage:
         ::
 
             result = await api.create_gateway_network(
                 gateway_id="example",
@@ -676,14 +678,15 @@
             body=marshal_CreateGatewayNetworkRequest(
                 CreateGatewayNetworkRequest(
                     gateway_id=gateway_id,
                     private_network_id=private_network_id,
                     enable_masquerade=enable_masquerade,
                     zone=zone,
                     dhcp_id=dhcp_id,
+                    dhcp=dhcp,
                     address=address,
                     enable_dhcp=enable_dhcp,
                 ),
                 self.client,
             ),
         )
 
@@ -698,21 +701,21 @@
         enable_masquerade: Optional[bool] = None,
         dhcp_id: Optional[str] = None,
         enable_dhcp: Optional[bool] = None,
         address: Optional[str] = None,
     ) -> GatewayNetwork:
         """
         Update a gateway connection to a Private Network
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param gateway_network_id: ID of the GatewayNetwork to update
-        :param enable_masquerade: New masquerade enablement
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param gateway_network_id: ID of the GatewayNetwork to update.
+        :param enable_masquerade: New masquerade enablement.
         :param dhcp_id: New DHCP configuration.
 
         One-of ('ip_config'): at most one of 'dhcp_id', 'address' could be set.
-        :param enable_dhcp: Whether to enable DHCP on the connected Private Network
+        :param enable_dhcp: Whether to enable DHCP on the connected Private Network.
         :param address: New static IP address.
 
         One-of ('ip_config'): at most one of 'dhcp_id', 'address' could be set.
         :return: :class:`GatewayNetwork <GatewayNetwork>`
 
         Usage:
         ::
@@ -749,19 +752,18 @@
         *,
         gateway_network_id: str,
         cleanup_dhcp: bool,
         zone: Optional[Zone] = None,
     ) -> Optional[None]:
         """
         Detach a gateway from a Private Network
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param gateway_network_id: GatewayNetwork to delete
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param gateway_network_id: GatewayNetwork to delete.
         :param cleanup_dhcp: Whether to cleanup the attached DHCP configuration (if any, and if not attached to another gateway_network).
 
-
         Usage:
         ::
 
             result = await api.delete_gateway_network(
                 gateway_network_id="example",
                 cleanup_dhcp=True,
             )
@@ -793,22 +795,22 @@
         organization_id: Optional[str] = None,
         project_id: Optional[str] = None,
         address: Optional[str] = None,
         has_address: Optional[str] = None,
     ) -> ListDHCPsResponse:
         """
         List DHCP configurations
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param order_by: Order in which to return results
-        :param page: Page number
-        :param page_size: DHCP configurations per page
-        :param organization_id: Include only DHCPs in this organization
-        :param project_id: Include only DHCPs in this project
-        :param address: Filter on gateway address
-        :param has_address: Filter on subnets containing address
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param order_by: Order in which to return results.
+        :param page: Page number.
+        :param page_size: DHCP configurations per page.
+        :param organization_id: Include only DHCPs in this organization.
+        :param project_id: Include only DHCPs in this project.
+        :param address: Filter on gateway address.
+        :param has_address: Filter on subnets containing address.
         :return: :class:`ListDHCPsResponse <ListDHCPsResponse>`
 
         Usage:
         ::
 
             result = await api.list_dhc_ps()
         """
@@ -843,22 +845,22 @@
         organization_id: Optional[str] = None,
         project_id: Optional[str] = None,
         address: Optional[str] = None,
         has_address: Optional[str] = None,
     ) -> List[DHCP]:
         """
         List DHCP configurations
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param order_by: Order in which to return results
-        :param page: Page number
-        :param page_size: DHCP configurations per page
-        :param organization_id: Include only DHCPs in this organization
-        :param project_id: Include only DHCPs in this project
-        :param address: Filter on gateway address
-        :param has_address: Filter on subnets containing address
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param order_by: Order in which to return results.
+        :param page: Page number.
+        :param page_size: DHCP configurations per page.
+        :param organization_id: Include only DHCPs in this organization.
+        :param project_id: Include only DHCPs in this project.
+        :param address: Filter on gateway address.
+        :param has_address: Filter on subnets containing address.
         :return: :class:`List[ListDHCPsResponse] <List[ListDHCPsResponse]>`
 
         Usage:
         ::
 
             result = await api.list_dhc_ps_all()
         """
@@ -883,16 +885,16 @@
         self,
         *,
         dhcp_id: str,
         zone: Optional[Zone] = None,
     ) -> DHCP:
         """
         Get a DHCP configuration
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param dhcp_id: ID of the DHCP config to fetch
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param dhcp_id: ID of the DHCP config to fetch.
         :return: :class:`DHCP <DHCP>`
 
         Usage:
         ::
 
             result = await api.get_dhcp(dhcp_id="example")
         """
@@ -925,34 +927,29 @@
         push_dns_server: Optional[bool] = None,
         dns_servers_override: Optional[List[str]] = None,
         dns_search: Optional[List[str]] = None,
         dns_local_name: Optional[str] = None,
     ) -> DHCP:
         """
         Create a DHCP configuration
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param project_id: Project to create the DHCP configuration in
-        :param subnet: Subnet for the DHCP server
-        :param address: Address of the DHCP server. This will be the gateway's address in the private network. Defaults to the first address of the subnet
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param project_id: Project to create the DHCP configuration in.
+        :param subnet: Subnet for the DHCP server.
+        :param address: Address of the DHCP server. This will be the gateway's address in the private network. Defaults to the first address of the subnet.
         :param pool_low: Low IP (included) of the dynamic address pool. Defaults to the second address of the subnet.
         :param pool_high: High IP (included) of the dynamic address pool. Defaults to the last address of the subnet.
         :param enable_dynamic: Whether to enable dynamic pooling of IPs. By turning the dynamic pool off, only pre-existing DHCP reservations will be handed out. Defaults to true.
-
         :param valid_lifetime: For how long, in seconds, will DHCP entries will be valid. Defaults to 1h (3600s).
         :param renew_timer: After how long, in seconds, a renew will be attempted. Must be 30s lower than `rebind_timer`. Defaults to 50m (3000s).
-
         :param rebind_timer: After how long, in seconds, a DHCP client will query for a new lease if previous renews fail. Must be 30s lower than `valid_lifetime`. Defaults to 51m (3060s).
-
-        :param push_default_route: Whether the gateway should push a default route to DHCP clients or only hand out IPs. Defaults to true
+        :param push_default_route: Whether the gateway should push a default route to DHCP clients or only hand out IPs. Defaults to true.
         :param push_dns_server: Whether the gateway should push custom DNS servers to clients. This allows for instance hostname -> IP resolution. Defaults to true.
-
-        :param dns_servers_override: Override the DNS server list pushed to DHCP clients, instead of the gateway itself
-        :param dns_search: Additional DNS search paths
+        :param dns_servers_override: Override the DNS server list pushed to DHCP clients, instead of the gateway itself.
+        :param dns_search: Additional DNS search paths.
         :param dns_local_name: TLD given to hostnames in the Private Network. Allowed characters are `a-z0-9-.`. Defaults to the slugified Private Network name if created along a GatewayNetwork, or else to `priv`.
-
         :return: :class:`DHCP <DHCP>`
 
         Usage:
         ::
 
             result = await api.create_dhcp(subnet="example")
         """
@@ -1004,31 +1001,28 @@
         push_dns_server: Optional[bool] = None,
         dns_servers_override: Optional[List[str]] = None,
         dns_search: Optional[List[str]] = None,
         dns_local_name: Optional[str] = None,
     ) -> DHCP:
         """
         Update a DHCP configuration
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param dhcp_id: DHCP config to update
-        :param subnet: Subnet for the DHCP server
-        :param address: Address of the DHCP server. This will be the gateway's address in the private network
-        :param pool_low: Low IP (included) of the dynamic address pool
-        :param pool_high: High IP (included) of the dynamic address pool
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param dhcp_id: DHCP config to update.
+        :param subnet: Subnet for the DHCP server.
+        :param address: Address of the DHCP server. This will be the gateway's address in the private network.
+        :param pool_low: Low IP (included) of the dynamic address pool.
+        :param pool_high: High IP (included) of the dynamic address pool.
         :param enable_dynamic: Whether to enable dynamic pooling of IPs. By turning the dynamic pool off, only pre-existing DHCP reservations will be handed out. Defaults to true.
-
-        :param valid_lifetime: How long, in seconds, DHCP entries will be valid for
+        :param valid_lifetime: How long, in seconds, DHCP entries will be valid for.
         :param renew_timer: After how long, in seconds, a renew will be attempted. Must be 30s lower than `rebind_timer`.
         :param rebind_timer: After how long, in seconds, a DHCP client will query for a new lease if previous renews fail. Must be 30s lower than `valid_lifetime`.
-
-        :param push_default_route: Whether the gateway should push a default route to DHCP clients or only hand out IPs
+        :param push_default_route: Whether the gateway should push a default route to DHCP clients or only hand out IPs.
         :param push_dns_server: Whether the gateway should push custom DNS servers to clients. This allows for instance hostname -> IP resolution.
-
-        :param dns_servers_override: Override the DNS server list pushed to DHCP clients, instead of the gateway itself
-        :param dns_search: Additional DNS search paths
+        :param dns_servers_override: Override the DNS server list pushed to DHCP clients, instead of the gateway itself.
+        :param dns_search: Additional DNS search paths.
         :param dns_local_name: TLD given to hostnames in the Private Network. Allowed characters are `a-z0-9-.`.
         :return: :class:`DHCP <DHCP>`
 
         Usage:
         ::
 
             result = await api.update_dhcp(dhcp_id="example")
@@ -1069,16 +1063,16 @@
         self,
         *,
         dhcp_id: str,
         zone: Optional[Zone] = None,
     ) -> Optional[None]:
         """
         Delete a DHCP configuration
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param dhcp_id: DHCP config id to delete
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param dhcp_id: DHCP config id to delete.
 
         Usage:
         ::
 
             result = await api.delete_dhcp(dhcp_id="example")
         """
 
@@ -1104,23 +1098,23 @@
         mac_address: Optional[str] = None,
         ip_address: Optional[str] = None,
         hostname: Optional[str] = None,
         type_: DHCPEntryType = DHCPEntryType.UNKNOWN,
     ) -> ListDHCPEntriesResponse:
         """
         List DHCP entries
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param order_by: Order in which to return results
-        :param page: Page number
-        :param page_size: DHCP entries per page
-        :param gateway_network_id: Filter entries based on the gateway network they are on
-        :param mac_address: Filter entries on their MAC address
-        :param ip_address: Filter entries on their IP address
-        :param hostname: Filter entries on their hostname substring
-        :param type_: Filter entries on their type
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param order_by: Order in which to return results.
+        :param page: Page number.
+        :param page_size: DHCP entries per page.
+        :param gateway_network_id: Filter entries based on the gateway network they are on.
+        :param mac_address: Filter entries on their MAC address.
+        :param ip_address: Filter entries on their IP address.
+        :param hostname: Filter entries on their hostname substring.
+        :param type_: Filter entries on their type.
         :return: :class:`ListDHCPEntriesResponse <ListDHCPEntriesResponse>`
 
         Usage:
         ::
 
             result = await api.list_dhcp_entries()
         """
@@ -1156,23 +1150,23 @@
         mac_address: Optional[str] = None,
         ip_address: Optional[str] = None,
         hostname: Optional[str] = None,
         type_: Optional[DHCPEntryType] = None,
     ) -> List[DHCPEntry]:
         """
         List DHCP entries
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param order_by: Order in which to return results
-        :param page: Page number
-        :param page_size: DHCP entries per page
-        :param gateway_network_id: Filter entries based on the gateway network they are on
-        :param mac_address: Filter entries on their MAC address
-        :param ip_address: Filter entries on their IP address
-        :param hostname: Filter entries on their hostname substring
-        :param type_: Filter entries on their type
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param order_by: Order in which to return results.
+        :param page: Page number.
+        :param page_size: DHCP entries per page.
+        :param gateway_network_id: Filter entries based on the gateway network they are on.
+        :param mac_address: Filter entries on their MAC address.
+        :param ip_address: Filter entries on their IP address.
+        :param hostname: Filter entries on their hostname substring.
+        :param type_: Filter entries on their type.
         :return: :class:`List[ListDHCPEntriesResponse] <List[ListDHCPEntriesResponse]>`
 
         Usage:
         ::
 
             result = await api.list_dhcp_entries_all()
         """
@@ -1198,16 +1192,16 @@
         self,
         *,
         dhcp_entry_id: str,
         zone: Optional[Zone] = None,
     ) -> DHCPEntry:
         """
         Get DHCP entries
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param dhcp_entry_id: ID of the DHCP entry to fetch
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param dhcp_entry_id: ID of the DHCP entry to fetch.
         :return: :class:`DHCPEntry <DHCPEntry>`
 
         Usage:
         ::
 
             result = await api.get_dhcp_entry(dhcp_entry_id="example")
         """
@@ -1229,18 +1223,18 @@
         gateway_network_id: str,
         mac_address: str,
         ip_address: str,
         zone: Optional[Zone] = None,
     ) -> DHCPEntry:
         """
         Create a static DHCP reservation
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param gateway_network_id: GatewayNetwork on which to create a DHCP reservation
-        :param mac_address: MAC address to give a static entry to
-        :param ip_address: IP address to give to the machine
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param gateway_network_id: GatewayNetwork on which to create a DHCP reservation.
+        :param mac_address: MAC address to give a static entry to.
+        :param ip_address: IP address to give to the machine.
         :return: :class:`DHCPEntry <DHCPEntry>`
 
         Usage:
         ::
 
             result = await api.create_dhcp_entry(
                 gateway_network_id="example",
@@ -1273,17 +1267,17 @@
         *,
         dhcp_entry_id: str,
         zone: Optional[Zone] = None,
         ip_address: Optional[str] = None,
     ) -> DHCPEntry:
         """
         Update a DHCP entry
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param dhcp_entry_id: DHCP entry ID to update
-        :param ip_address: New IP address to give to the machine
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param dhcp_entry_id: DHCP entry ID to update.
+        :param ip_address: New IP address to give to the machine.
         :return: :class:`DHCPEntry <DHCPEntry>`
 
         Usage:
         ::
 
             result = await api.update_dhcp_entry(dhcp_entry_id="example")
         """
@@ -1313,17 +1307,17 @@
         gateway_network_id: str,
         zone: Optional[Zone] = None,
         dhcp_entries: Optional[List[SetDHCPEntriesRequestEntry]] = None,
     ) -> SetDHCPEntriesResponse:
         """
         Set the list of DHCP reservations attached to a Gateway Network. Reservations are identified by their MAC address, and will sync the current DHCP entry list to the given list, creating, updating or deleting DHCP entries.
 
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param gateway_network_id: Gateway Network on which to set DHCP reservation list
-        :param dhcp_entries: New list of DHCP reservations
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param gateway_network_id: Gateway Network on which to set DHCP reservation list.
+        :param dhcp_entries: New list of DHCP reservations.
         :return: :class:`SetDHCPEntriesResponse <SetDHCPEntriesResponse>`
 
         Usage:
         ::
 
             result = await api.set_dhcp_entries(gateway_network_id="example")
         """
@@ -1350,16 +1344,16 @@
         self,
         *,
         dhcp_entry_id: str,
         zone: Optional[Zone] = None,
     ) -> Optional[None]:
         """
         Delete a DHCP reservation
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param dhcp_entry_id: DHCP entry ID to delete
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param dhcp_entry_id: DHCP entry ID to delete.
 
         Usage:
         ::
 
             result = await api.delete_dhcp_entry(dhcp_entry_id="example")
         """
 
@@ -1383,21 +1377,21 @@
         page_size: Optional[int] = None,
         gateway_id: Optional[str] = None,
         private_ip: Optional[str] = None,
         protocol: PATRuleProtocol = PATRuleProtocol.UNKNOWN,
     ) -> ListPATRulesResponse:
         """
         List PAT rules
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param order_by: Order in which to return results
-        :param page: Page number
-        :param page_size: PAT rules per page
-        :param gateway_id: Fetch rules for this gateway
-        :param private_ip: Fetch rules targeting this private ip
-        :param protocol: Fetch rules for this protocol
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param order_by: Order in which to return results.
+        :param page: Page number.
+        :param page_size: PAT rules per page.
+        :param gateway_id: Fetch rules for this gateway.
+        :param private_ip: Fetch rules targeting this private ip.
+        :param protocol: Fetch rules for this protocol.
         :return: :class:`ListPATRulesResponse <ListPATRulesResponse>`
 
         Usage:
         ::
 
             result = await api.list_pat_rules()
         """
@@ -1429,21 +1423,21 @@
         page_size: Optional[int] = None,
         gateway_id: Optional[str] = None,
         private_ip: Optional[str] = None,
         protocol: Optional[PATRuleProtocol] = None,
     ) -> List[PATRule]:
         """
         List PAT rules
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param order_by: Order in which to return results
-        :param page: Page number
-        :param page_size: PAT rules per page
-        :param gateway_id: Fetch rules for this gateway
-        :param private_ip: Fetch rules targeting this private ip
-        :param protocol: Fetch rules for this protocol
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param order_by: Order in which to return results.
+        :param page: Page number.
+        :param page_size: PAT rules per page.
+        :param gateway_id: Fetch rules for this gateway.
+        :param private_ip: Fetch rules targeting this private ip.
+        :param protocol: Fetch rules for this protocol.
         :return: :class:`List[ListPATRulesResponse] <List[ListPATRulesResponse]>`
 
         Usage:
         ::
 
             result = await api.list_pat_rules_all()
         """
@@ -1467,16 +1461,16 @@
         self,
         *,
         pat_rule_id: str,
         zone: Optional[Zone] = None,
     ) -> PATRule:
         """
         Get a PAT rule
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param pat_rule_id: PAT rule to get
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param pat_rule_id: PAT rule to get.
         :return: :class:`PATRule <PATRule>`
 
         Usage:
         ::
 
             result = await api.get_pat_rule(pat_rule_id="example")
         """
@@ -1500,20 +1494,20 @@
         private_ip: str,
         private_port: int,
         protocol: PATRuleProtocol,
         zone: Optional[Zone] = None,
     ) -> PATRule:
         """
         Create a PAT rule
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param gateway_id: Gateway on which to attach the rule to
-        :param public_port: Public port to listen on
-        :param private_ip: Private IP to forward data to
-        :param private_port: Private port to translate to
-        :param protocol: Protocol the rule should apply to
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param gateway_id: Gateway on which to attach the rule to.
+        :param public_port: Public port to listen on.
+        :param private_ip: Private IP to forward data to.
+        :param private_port: Private port to translate to.
+        :param protocol: Protocol the rule should apply to.
         :return: :class:`PATRule <PATRule>`
 
         Usage:
         ::
 
             result = await api.create_pat_rule(
                 gateway_id="example",
@@ -1553,20 +1547,20 @@
         zone: Optional[Zone] = None,
         public_port: Optional[int] = None,
         private_ip: Optional[str] = None,
         private_port: Optional[int] = None,
     ) -> PATRule:
         """
         Update a PAT rule
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param pat_rule_id: PAT rule to update
-        :param public_port: Public port to listen on
-        :param private_ip: Private IP to forward data to
-        :param private_port: Private port to translate to
-        :param protocol: Protocol the rule should apply to
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param pat_rule_id: PAT rule to update.
+        :param public_port: Public port to listen on.
+        :param private_ip: Private IP to forward data to.
+        :param private_port: Private port to translate to.
+        :param protocol: Protocol the rule should apply to.
         :return: :class:`PATRule <PATRule>`
 
         Usage:
         ::
 
             result = await api.update_pat_rule(
                 pat_rule_id="example",
@@ -1602,17 +1596,17 @@
         gateway_id: str,
         pat_rules: List[SetPATRulesRequestRule],
         zone: Optional[Zone] = None,
     ) -> SetPATRulesResponse:
         """
         Set the list of PAT rules attached to a Gateway. Rules are identified by their public port and protocol. This will sync the current PAT rule list with the givent list, creating, updating or deleting PAT rules.
 
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param gateway_id: Gateway on which to set the PAT rules
-        :param pat_rules: New list of PAT rules
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param gateway_id: Gateway on which to set the PAT rules.
+        :param pat_rules: New list of PAT rules.
         :return: :class:`SetPATRulesResponse <SetPATRulesResponse>`
 
         Usage:
         ::
 
             result = await api.set_pat_rules(
                 gateway_id="example",
@@ -1642,16 +1636,16 @@
         self,
         *,
         pat_rule_id: str,
         zone: Optional[Zone] = None,
     ) -> Optional[None]:
         """
         Delete a PAT rule
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param pat_rule_id: PAT rule to delete
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param pat_rule_id: PAT rule to delete.
 
         Usage:
         ::
 
             result = await api.delete_pat_rule(pat_rule_id="example")
         """
 
@@ -1669,15 +1663,15 @@
     async def list_gateway_types(
         self,
         *,
         zone: Optional[Zone] = None,
     ) -> ListGatewayTypesResponse:
         """
         List VPC Public Gateway types
-        :param zone: Zone to target. If none is passed will use default zone from the config
+        :param zone: Zone to target. If none is passed will use default zone from the config.
         :return: :class:`ListGatewayTypesResponse <ListGatewayTypesResponse>`
 
         Usage:
         ::
 
             result = await api.list_gateway_types()
         """
@@ -1703,23 +1697,23 @@
         project_id: Optional[str] = None,
         tags: Optional[List[str]] = None,
         reverse: Optional[str] = None,
         is_free: Optional[bool] = None,
     ) -> ListIPsResponse:
         """
         List IPs
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param order_by: Order in which to return results
-        :param page: Page number
-        :param page_size: IPs per page
-        :param organization_id: Include only IPs in this organization
-        :param project_id: Include only IPs in this project
-        :param tags: Filter IPs with these tags
-        :param reverse: Filter by reverse containing this string
-        :param is_free: Filter whether the IP is attached to a gateway or not
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param order_by: Order in which to return results.
+        :param page: Page number.
+        :param page_size: IPs per page.
+        :param organization_id: Include only IPs in this organization.
+        :param project_id: Include only IPs in this project.
+        :param tags: Filter IPs with these tags.
+        :param reverse: Filter by reverse containing this string.
+        :param is_free: Filter whether the IP is attached to a gateway or not.
         :return: :class:`ListIPsResponse <ListIPsResponse>`
 
         Usage:
         ::
 
             result = await api.list_i_ps()
         """
@@ -1756,23 +1750,23 @@
         project_id: Optional[str] = None,
         tags: Optional[List[str]] = None,
         reverse: Optional[str] = None,
         is_free: Optional[bool] = None,
     ) -> List[IP]:
         """
         List IPs
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param order_by: Order in which to return results
-        :param page: Page number
-        :param page_size: IPs per page
-        :param organization_id: Include only IPs in this organization
-        :param project_id: Include only IPs in this project
-        :param tags: Filter IPs with these tags
-        :param reverse: Filter by reverse containing this string
-        :param is_free: Filter whether the IP is attached to a gateway or not
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param order_by: Order in which to return results.
+        :param page: Page number.
+        :param page_size: IPs per page.
+        :param organization_id: Include only IPs in this organization.
+        :param project_id: Include only IPs in this project.
+        :param tags: Filter IPs with these tags.
+        :param reverse: Filter by reverse containing this string.
+        :param is_free: Filter whether the IP is attached to a gateway or not.
         :return: :class:`List[ListIPsResponse] <List[ListIPsResponse]>`
 
         Usage:
         ::
 
             result = await api.list_i_ps_all()
         """
@@ -1798,16 +1792,16 @@
         self,
         *,
         ip_id: str,
         zone: Optional[Zone] = None,
     ) -> IP:
         """
         Get an IP
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param ip_id: ID of the IP to get
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param ip_id: ID of the IP to get.
         :return: :class:`IP <IP>`
 
         Usage:
         ::
 
             result = await api.get_ip(ip_id="example")
         """
@@ -1828,17 +1822,17 @@
         *,
         zone: Optional[Zone] = None,
         project_id: Optional[str] = None,
         tags: Optional[List[str]] = None,
     ) -> IP:
         """
         Reserve an IP
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param project_id: Project to create the IP into
-        :param tags: Tags to give to the IP
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param project_id: Project to create the IP into.
+        :param tags: Tags to give to the IP.
         :return: :class:`IP <IP>`
 
         Usage:
         ::
 
             result = await api.create_ip()
         """
@@ -1868,19 +1862,19 @@
         zone: Optional[Zone] = None,
         tags: Optional[List[str]] = None,
         reverse: Optional[str] = None,
         gateway_id: Optional[str] = None,
     ) -> IP:
         """
         Update an IP
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param ip_id: ID of the IP to update
-        :param tags: Tags to give to the IP
-        :param reverse: Reverse to set on the IP. Empty string to unset
-        :param gateway_id: Gateway to attach the IP to. Empty string to detach
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param ip_id: ID of the IP to update.
+        :param tags: Tags to give to the IP.
+        :param reverse: Reverse to set on the IP. Empty string to unset.
+        :param gateway_id: Gateway to attach the IP to. Empty string to detach.
         :return: :class:`IP <IP>`
 
         Usage:
         ::
 
             result = await api.update_ip(ip_id="example")
         """
@@ -1910,16 +1904,16 @@
         self,
         *,
         ip_id: str,
         zone: Optional[Zone] = None,
     ) -> Optional[None]:
         """
         Delete an IP
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param ip_id: ID of the IP to delete
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param ip_id: ID of the IP to delete.
 
         Usage:
         ::
 
             result = await api.delete_ip(ip_id="example")
         """
 
@@ -1938,16 +1932,16 @@
         self,
         *,
         gateway_id: str,
         zone: Optional[Zone] = None,
     ) -> Gateway:
         """
         Refresh SSH keys of a VPC Public Gateway
-        :param zone: Zone to target. If none is passed will use default zone from the config
-        :param gateway_id: ID of the gateway that needs fresh ssh keys
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param gateway_id: ID of the gateway that needs fresh ssh keys.
         :return: :class:`Gateway <Gateway>`
 
         Usage:
         ::
 
             result = await api.refresh_ssh_keys(gateway_id="example")
         """
```

### Comparing `scaleway_async-0.8.0/scaleway_async/vpcgw/v1/content.py` & `scaleway_async-0.9.0/scaleway_async/vpcgw/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway_async-0.8.0/scaleway_async/vpcgw/v1/marshalling.py` & `scaleway_async-0.9.0/scaleway_async/vpcgw/v1/marshalling.py`

 * *Files 0% similar despite different names*

```diff
@@ -507,14 +507,36 @@
 
     field = data.get("pat_rules")
     args["pat_rules"] = [unmarshal_PATRule(v) for v in data["pat_rules"]]
 
     return SetPATRulesResponse(**args)
 
 
+def marshal_CreateDHCPRequest(
+    request: CreateDHCPRequest,
+    defaults: ProfileDefaults,
+) -> Dict[str, Any]:
+    return {
+        "address": request.address,
+        "dns_local_name": request.dns_local_name,
+        "dns_search": request.dns_search,
+        "dns_servers_override": request.dns_servers_override,
+        "enable_dynamic": request.enable_dynamic,
+        "pool_high": request.pool_high,
+        "pool_low": request.pool_low,
+        "project_id": request.project_id or defaults.default_project_id,
+        "push_default_route": request.push_default_route,
+        "push_dns_server": request.push_dns_server,
+        "rebind_timer": request.rebind_timer,
+        "renew_timer": request.renew_timer,
+        "subnet": request.subnet,
+        "valid_lifetime": request.valid_lifetime,
+    }
+
+
 def marshal_SetDHCPEntriesRequestEntry(
     request: SetDHCPEntriesRequestEntry,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     return {
         "ip_address": request.ip_address,
         "mac_address": request.mac_address,
@@ -540,44 +562,23 @@
     return {
         "gateway_network_id": request.gateway_network_id,
         "ip_address": request.ip_address,
         "mac_address": request.mac_address,
     }
 
 
-def marshal_CreateDHCPRequest(
-    request: CreateDHCPRequest,
-    defaults: ProfileDefaults,
-) -> Dict[str, Any]:
-    return {
-        "address": request.address,
-        "dns_local_name": request.dns_local_name,
-        "dns_search": request.dns_search,
-        "dns_servers_override": request.dns_servers_override,
-        "enable_dynamic": request.enable_dynamic,
-        "pool_high": request.pool_high,
-        "pool_low": request.pool_low,
-        "project_id": request.project_id or defaults.default_project_id,
-        "push_default_route": request.push_default_route,
-        "push_dns_server": request.push_dns_server,
-        "rebind_timer": request.rebind_timer,
-        "renew_timer": request.renew_timer,
-        "subnet": request.subnet,
-        "valid_lifetime": request.valid_lifetime,
-    }
-
-
 def marshal_CreateGatewayNetworkRequest(
     request: CreateGatewayNetworkRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     return {
         **resolve_one_of(
             [
                 OneOfPossibility("dhcp_id", request.dhcp_id),
+                OneOfPossibility("dhcp", request.dhcp),
                 OneOfPossibility("address", request.address),
             ]
         ),
         "enable_dhcp": request.enable_dhcp,
         "enable_masquerade": request.enable_masquerade,
         "gateway_id": request.gateway_id,
         "private_network_id": request.private_network_id,
```

### Comparing `scaleway_async-0.8.0/scaleway_async/vpcgw/v1/types.py` & `scaleway_async-0.9.0/scaleway_async/vpcgw/v1/types.py`

 * *Files 17% similar despite different names*

```diff
@@ -127,1086 +127,1081 @@
     def __str__(self) -> str:
         return str(self.value)
 
 
 @dataclass
 class DHCP:
     """
-    Dhcp
+    Dhcp.
     """
 
     id: str
     """
-    ID of the DHCP config
+    ID of the DHCP config.
     """
 
     organization_id: str
     """
-    Owning organization
+    Owning organization.
     """
 
     project_id: str
     """
-    Owning project
+    Owning project.
     """
 
     created_at: Optional[datetime]
     """
-    Configuration creation date
+    Configuration creation date.
     """
 
     updated_at: Optional[datetime]
     """
-    Configuration last modification date
+    Configuration last modification date.
     """
 
     subnet: str
     """
-    Subnet for the DHCP server
+    Subnet for the DHCP server.
     """
 
     address: str
     """
     Address of the DHCP server. This will be the gateway's address in the private network. It must be part of config's subnet.
-    
     """
 
     pool_low: str
     """
-    Low IP (included) of the dynamic address pool. Must be in the config's subnet
+    Low IP (included) of the dynamic address pool. Must be in the config's subnet.
     """
 
     pool_high: str
     """
-    High IP (included) of the dynamic address pool. Must be in the config's subnet
+    High IP (included) of the dynamic address pool. Must be in the config's subnet.
     """
 
     enable_dynamic: bool
     """
     Whether to enable dynamic pooling of IPs. By turning the dynamic pool off, only pre-existing DHCP reservations will be handed out.
-    
     """
 
     valid_lifetime: Optional[str]
     """
-    How long, in seconds, DHCP entries will be valid for
+    How long, in seconds, DHCP entries will be valid for.
     """
 
     renew_timer: Optional[str]
     """
     After how long, in seconds, a renew will be attempted. Must be 30s lower than `rebind_timer`.
-    
     """
 
     rebind_timer: Optional[str]
     """
     After how long, in seconds, a DHCP client will query for a new lease if previous renews fail. Must be 30s lower than `valid_lifetime`.
-    
     """
 
     push_default_route: bool
     """
-    Whether the gateway should push a default route to DHCP clients or only hand out IPs
+    Whether the gateway should push a default route to DHCP clients or only hand out IPs.
     """
 
     push_dns_server: bool
     """
     Whether the gateway should push custom DNS servers to clients. This allows for instance hostname -> IP resolution.
-    
     """
 
     dns_servers_override: List[str]
     """
-    Override the DNS server list pushed to DHCP clients, instead of the gateway itself
+    Override the DNS server list pushed to DHCP clients, instead of the gateway itself.
     """
 
     dns_search: List[str]
     """
-    Add search paths to the pushed DNS configuration
+    Add search paths to the pushed DNS configuration.
     """
 
     dns_local_name: str
     """
     TLD given to hostnames in the Private Network. If an instance with hostname `foo` gets a lease, and this is set to `bar`, `foo.bar` will resolve.
-    
     """
 
     zone: Zone
     """
-    Zone this configuration is available in
+    Zone this configuration is available in.
     """
 
 
 @dataclass
 class DHCPEntry:
     """
-    Dhcp entry
+    Dhcp entry.
     """
 
     id: str
     """
-    Entry ID
+    Entry ID.
     """
 
     created_at: Optional[datetime]
     """
-    Configuration creation date
+    Configuration creation date.
     """
 
     updated_at: Optional[datetime]
     """
-    Configuration last modification date
+    Configuration last modification date.
     """
 
     gateway_network_id: str
     """
-    Owning GatewayNetwork
+    Owning GatewayNetwork.
     """
 
     mac_address: str
     """
-    MAC address of the client machine
+    MAC address of the client machine.
     """
 
     ip_address: str
     """
-    Assigned IP address
+    Assigned IP address.
     """
 
     hostname: str
     """
-    Hostname of the client machine
+    Hostname of the client machine.
     """
 
     type_: DHCPEntryType
     """
-    Entry type, either static (DHCP reservation) or dynamic (DHCP lease)
+    Entry type, either static (DHCP reservation) or dynamic (DHCP lease).
     """
 
     zone: Zone
     """
-    Zone this entry is available in
+    Zone this entry is available in.
     """
 
 
 @dataclass
 class Gateway:
     """
-    Gateway
+    Gateway.
     """
 
     id: str
     """
-    ID of the gateway
+    ID of the gateway.
     """
 
     organization_id: str
     """
-    Owning organization
+    Owning organization.
     """
 
     project_id: str
     """
-    Owning project
+    Owning project.
     """
 
     created_at: Optional[datetime]
     """
-    Gateway creation date
+    Gateway creation date.
     """
 
     updated_at: Optional[datetime]
     """
-    Gateway last modification date
+    Gateway last modification date.
     """
 
     type_: Optional[GatewayType]
     """
-    Gateway type
+    Gateway type.
     """
 
     status: GatewayStatus
     """
-    Gateway's current status
+    Gateway's current status.
     """
 
     name: str
     """
-    Name of the gateway
+    Name of the gateway.
     """
 
     tags: List[str]
     """
-    Tags of the gateway
+    Tags of the gateway.
     """
 
     ip: Optional[IP]
     """
-    Public IP of the gateway
+    Public IP of the gateway.
     """
 
     gateway_networks: List[GatewayNetwork]
     """
-    GatewayNetworks attached to the gateway
+    GatewayNetworks attached to the gateway.
     """
 
     upstream_dns_servers: List[str]
     """
-    Override the gateway's default recursive DNS servers
+    Override the gateway's default recursive DNS servers.
     """
 
     version: Optional[str]
     """
-    Version of the running gateway software
+    Version of the running gateway software.
     """
 
     can_upgrade_to: Optional[str]
     """
-    Newly available gateway software version that can be updated to
+    Newly available gateway software version that can be updated to.
     """
 
     bastion_enabled: bool
     """
-    Whether SSH bastion is enabled on the gateway
+    Whether SSH bastion is enabled on the gateway.
     """
 
     bastion_port: int
     """
-    Port of the SSH bastion
+    Port of the SSH bastion.
     """
 
     smtp_enabled: bool
     """
-    Whether SMTP traffic is allowed to pass through the gateway
+    Whether SMTP traffic is allowed to pass through the gateway.
     """
 
     zone: Zone
     """
-    Zone the gateway is available in
+    Zone the gateway is available in.
     """
 
 
 @dataclass
 class GatewayNetwork:
     """
-    Gateway network
+    Gateway network.
     """
 
     id: str
     """
-    ID of the connection
+    ID of the connection.
     """
 
     created_at: Optional[datetime]
     """
-    Connection creation date
+    Connection creation date.
     """
 
     updated_at: Optional[datetime]
     """
-    Connection last modification date
+    Connection last modification date.
     """
 
     gateway_id: str
     """
-    ID of the connected gateway
+    ID of the connected gateway.
     """
 
     private_network_id: str
     """
-    ID of the connected private network
+    ID of the connected private network.
     """
 
     mac_address: Optional[str]
     """
-    MAC address of the gateway in the network (if the gateway is up and running)
+    MAC address of the gateway in the network (if the gateway is up and running).
     """
 
     enable_masquerade: bool
     """
-    Whether the gateway masquerades traffic for this network
+    Whether the gateway masquerades traffic for this network.
     """
 
     status: GatewayNetworkStatus
     """
-    Current status of the gateway network connection
+    Current status of the gateway network connection.
     """
 
     dhcp: Optional[DHCP]
     """
-    DHCP configuration for the connected private network
+    DHCP configuration for the connected private network.
     """
 
     enable_dhcp: bool
     """
-    Whether DHCP is enabled on the connected Private Network
+    Whether DHCP is enabled on the connected Private Network.
     """
 
     address: Optional[str]
     """
-    Address of the Gateway in CIDR form to use when DHCP is not used
+    Address of the Gateway in CIDR form to use when DHCP is not used.
     """
 
     zone: Zone
     """
-    Zone the connection lives in
+    Zone the connection lives in.
     """
 
 
 @dataclass
 class GatewayType:
     """
-    Gateway type
+    Gateway type.
     """
 
     name: str
     """
-    Type name
+    Type name.
     """
 
     bandwidth: int
     """
     Bandwidth, in bps, the gateway has. This is the public bandwidth to the outer internet, and the internal bandwidth to each connected Private Networks.
-    
     """
 
     zone: Zone
     """
-    Zone the type is available in
+    Zone the type is available in.
     """
 
 
 @dataclass
 class IP:
     """
-    Ip
+    Ip.
     """
 
     id: str
     """
-    IP ID
+    IP ID.
     """
 
     organization_id: str
     """
-    Owning organization
+    Owning organization.
     """
 
     project_id: str
     """
-    Owning project
+    Owning project.
     """
 
     created_at: Optional[datetime]
     """
-    Configuration creation date
+    Configuration creation date.
     """
 
     updated_at: Optional[datetime]
     """
-    Configuration last modification date
+    Configuration last modification date.
     """
 
     tags: List[str]
     """
-    Tags associated with the IP
+    Tags associated with the IP.
     """
 
     address: str
     """
-    The IP itself
+    The IP itself.
     """
 
     reverse: Optional[str]
     """
-    Reverse domain name for the IP address
+    Reverse domain name for the IP address.
     """
 
     gateway_id: Optional[str]
     """
-    Gateway associated to the IP
+    Gateway associated to the IP.
     """
 
     zone: Zone
     """
-    Zone this IP is available in
+    Zone this IP is available in.
     """
 
 
 @dataclass
 class ListDHCPEntriesResponse:
     """
-    List dhcp entries response
+    List dhcp entries response.
     """
 
     dhcp_entries: List[DHCPEntry]
     """
-    DHCP entries in this page
+    DHCP entries in this page.
     """
 
     total_count: int
     """
-    Total DHCP entries matching the filter
+    Total DHCP entries matching the filter.
     """
 
 
 @dataclass
 class ListDHCPsResponse:
     """
-    List dhc ps response
+    List dhc ps response.
     """
 
     dhcps: List[DHCP]
     """
-    First page of DHCP configs
+    First page of DHCP configs.
     """
 
     total_count: int
     """
-    Total DHCP configs matching the filter
+    Total DHCP configs matching the filter.
     """
 
 
 @dataclass
 class ListGatewayNetworksResponse:
     """
-    List gateway networks response
+    List gateway networks response.
     """
 
     gateway_networks: List[GatewayNetwork]
     """
-    GatewayNetworks in this page
+    GatewayNetworks in this page.
     """
 
     total_count: int
     """
-    Total GatewayNetworks count matching the filter
+    Total GatewayNetworks count matching the filter.
     """
 
 
 @dataclass
 class ListGatewayTypesResponse:
     """
-    List gateway types response
+    List gateway types response.
     """
 
     types: List[GatewayType]
     """
-    Available types of gateway
+    Available types of gateway.
     """
 
 
 @dataclass
 class ListGatewaysResponse:
     """
-    List gateways response
+    List gateways response.
     """
 
     gateways: List[Gateway]
     """
-    Gateways in this page
+    Gateways in this page.
     """
 
     total_count: int
     """
-    Total count of gateways matching the filter
+    Total count of gateways matching the filter.
     """
 
 
 @dataclass
 class ListIPsResponse:
     """
-    List i ps response
+    List i ps response.
     """
 
     ips: List[IP]
     """
-    IPs in this page
+    IPs in this page.
     """
 
     total_count: int
     """
-    Total IP count matching the filter
+    Total IP count matching the filter.
     """
 
 
 @dataclass
 class ListPATRulesResponse:
     """
-    List pat rules response
+    List pat rules response.
     """
 
     pat_rules: List[PATRule]
     """
-    This page of PAT rules matching the filter
+    This page of PAT rules matching the filter.
     """
 
     total_count: int
     """
-    Total PAT rules matching the filter
+    Total PAT rules matching the filter.
     """
 
 
 @dataclass
 class PATRule:
     """
-    Pat rule
+    Pat rule.
     """
 
     id: str
     """
-    Rule ID
+    Rule ID.
     """
 
     gateway_id: str
     """
-    Gateway the PAT rule applies to
+    Gateway the PAT rule applies to.
     """
 
     created_at: Optional[datetime]
     """
-    Rule creation date
+    Rule creation date.
     """
 
     updated_at: Optional[datetime]
     """
-    Rule last modification date
+    Rule last modification date.
     """
 
     public_port: int
     """
-    Public port to listen on
+    Public port to listen on.
     """
 
     private_ip: str
     """
-    Private IP to forward data to
+    Private IP to forward data to.
     """
 
     private_port: int
     """
-    Private port to translate to
+    Private port to translate to.
     """
 
     protocol: PATRuleProtocol
     """
-    Protocol the rule applies to
+    Protocol the rule applies to.
     """
 
     zone: Zone
     """
-    Zone this rule is available in
+    Zone this rule is available in.
     """
 
 
 @dataclass
 class SetDHCPEntriesRequestEntry:
     """
-    Set dhcp entries request. entry
+    Set dhcp entries request. entry.
     """
 
     mac_address: str
     """
     MAC address to give a static entry to. A matching entry will be upgraded to a reservation, and a matching reservation will be updated.
-    
     """
 
     ip_address: str
     """
-    IP address to give to the machine
+    IP address to give to the machine.
     """
 
 
 @dataclass
 class SetDHCPEntriesResponse:
     """
-    Set dhcp entries response
+    Set dhcp entries response.
     """
 
     dhcp_entries: List[DHCPEntry]
     """
-    List of DHCP entries
+    List of DHCP entries.
     """
 
 
 @dataclass
 class SetPATRulesRequestRule:
     """
-    Set pat rules request. rule
+    Set pat rules request. rule.
     """
 
     public_port: int
     """
     Public port to listen on. Uniquely identifies the rule, and a matching rule will be updated with the new parameters.
-    
     """
 
     private_ip: str
     """
-    Private IP to forward data to
+    Private IP to forward data to.
     """
 
     private_port: int
     """
-    Private port to translate to
+    Private port to translate to.
     """
 
     protocol: PATRuleProtocol
     """
-    Protocol the rule should apply to
+    Protocol the rule should apply to.
     """
 
 
 @dataclass
 class SetPATRulesResponse:
     """
-    Set pat rules response
+    Set pat rules response.
     """
 
     pat_rules: List[PATRule]
     """
-    List of PAT rules
+    List of PAT rules.
     """
 
 
 @dataclass
 class ListGatewaysRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     order_by: Optional[ListGatewaysRequestOrderBy]
     """
-    Order in which to return results
+    Order in which to return results.
     """
 
     page: Optional[int]
     """
-    Page number
+    Page number.
     """
 
     page_size: Optional[int]
     """
-    Gateways per page
+    Gateways per page.
     """
 
     organization_id: Optional[str]
     """
-    Include only gateways in this organization
+    Include only gateways in this organization.
     """
 
     project_id: Optional[str]
     """
-    Include only gateways in this project
+    Include only gateways in this project.
     """
 
     name: Optional[str]
     """
-    Filter gateways including this name
+    Filter gateways including this name.
     """
 
     tags: Optional[List[str]]
     """
-    Filter gateways with these tags
+    Filter gateways with these tags.
     """
 
     type_: Optional[str]
     """
-    Filter gateways of this type
+    Filter gateways of this type.
     """
 
     status: Optional[GatewayStatus]
     """
-    Filter gateways in this status (unknown for any)
+    Filter gateways in this status (unknown for any).
     """
 
     private_network_id: Optional[str]
     """
-    Filter gateways attached to this private network
+    Filter gateways attached to this private network.
     """
 
 
 @dataclass
 class GetGatewayRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     gateway_id: str
     """
-    ID of the gateway to fetch
+    ID of the gateway to fetch.
     """
 
 
 @dataclass
 class CreateGatewayRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     project_id: Optional[str]
     """
-    Project to create the gateway into
+    Project to create the gateway into.
     """
 
     name: Optional[str]
     """
-    Name of the gateway
+    Name of the gateway.
     """
 
     tags: Optional[List[str]]
     """
-    Tags for the gateway
+    Tags for the gateway.
     """
 
     type_: str
     """
-    Gateway type
+    Gateway type.
     """
 
     upstream_dns_servers: Optional[List[str]]
     """
-    Override the gateway's default recursive DNS servers, if DNS features are enabled
+    Override the gateway's default recursive DNS servers, if DNS features are enabled.
     """
 
     ip_id: Optional[str]
     """
-    Attach an existing IP to the gateway
+    Attach an existing IP to the gateway.
     """
 
     enable_smtp: bool
     """
-    Allow SMTP traffic to pass through the gateway
+    Allow SMTP traffic to pass through the gateway.
     """
 
     enable_bastion: bool
     """
-    Enable SSH bastion on the gateway
+    Enable SSH bastion on the gateway.
     """
 
     bastion_port: Optional[int]
     """
-    Port of the SSH bastion
+    Port of the SSH bastion.
     """
 
 
 @dataclass
 class UpdateGatewayRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     gateway_id: str
     """
-    ID of the gateway to update
+    ID of the gateway to update.
     """
 
     name: Optional[str]
     """
-    Name fo the gateway
+    Name fo the gateway.
     """
 
     tags: Optional[List[str]]
     """
-    Tags for the gateway
+    Tags for the gateway.
     """
 
     upstream_dns_servers: Optional[List[str]]
     """
-    Override the gateway's default recursive DNS servers, if DNS features are enabled
+    Override the gateway's default recursive DNS servers, if DNS features are enabled.
     """
 
     enable_bastion: Optional[bool]
     """
-    Enable SSH bastion on the gateway
+    Enable SSH bastion on the gateway.
     """
 
     bastion_port: Optional[int]
     """
-    Port of the SSH bastion
+    Port of the SSH bastion.
     """
 
     enable_smtp: Optional[bool]
     """
-    Allow SMTP traffic to pass through the gateway
+    Allow SMTP traffic to pass through the gateway.
     """
 
 
 @dataclass
 class DeleteGatewayRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     gateway_id: str
     """
-    ID of the gateway to delete
+    ID of the gateway to delete.
     """
 
     cleanup_dhcp: bool
     """
     Whether to cleanup attached DHCP configurations (if any, and if not attached to another Gateway Network).
-    
     """
 
 
 @dataclass
 class UpgradeGatewayRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     gateway_id: str
     """
-    ID of the gateway to upgrade
+    ID of the gateway to upgrade.
     """
 
 
 @dataclass
 class ListGatewayNetworksRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     order_by: Optional[ListGatewayNetworksRequestOrderBy]
     """
-    Order in which to return results
+    Order in which to return results.
     """
 
     page: Optional[int]
     """
-    Page number
+    Page number.
     """
 
     page_size: Optional[int]
     """
-    GatewayNetworks per page
+    GatewayNetworks per page.
     """
 
     gateway_id: Optional[str]
     """
-    Filter by gateway
+    Filter by gateway.
     """
 
     private_network_id: Optional[str]
     """
-    Filter by private network
+    Filter by private network.
     """
 
     enable_masquerade: Optional[bool]
     """
-    Filter by masquerade enablement
+    Filter by masquerade enablement.
     """
 
     dhcp_id: Optional[str]
     """
-    Filter by DHCP configuration
+    Filter by DHCP configuration.
     """
 
     status: Optional[GatewayNetworkStatus]
     """
-    Filter GatewayNetworks by this status (unknown for any)
+    Filter GatewayNetworks by this status (unknown for any).
     """
 
 
 @dataclass
 class GetGatewayNetworkRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     gateway_network_id: str
     """
-    ID of the GatewayNetwork to fetch
+    ID of the GatewayNetwork to fetch.
     """
 
 
 @dataclass
 class CreateGatewayNetworkRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     gateway_id: str
     """
-    Gateway to connect
+    Gateway to connect.
     """
 
     private_network_id: str
     """
-    Private Network to connect
+    Private Network to connect.
     """
 
     enable_masquerade: bool
     """
-    Whether to enable masquerade on this network
+    Whether to enable masquerade on this network.
     """
 
     dhcp_id: Optional[str]
     """
     Existing configuration.
     
-    One-of ('ip_config'): at most one of 'dhcp_id', 'address' could be set.
+    One-of ('ip_config'): at most one of 'dhcp_id', 'dhcp', 'address' could be set.
+    """
+
+    dhcp: Optional[CreateDHCPRequest]
+    """
+    New DHCP configuration.
+    
+    One-of ('ip_config'): at most one of 'dhcp_id', 'dhcp', 'address' could be set.
     """
 
     address: Optional[str]
     """
     Static IP address in CIDR format to to use without DHCP.
     
-    One-of ('ip_config'): at most one of 'dhcp_id', 'address' could be set.
+    One-of ('ip_config'): at most one of 'dhcp_id', 'dhcp', 'address' could be set.
     """
 
     enable_dhcp: Optional[bool]
     """
     Whether to enable DHCP on this Private Network. Defaults to `true` if either `dhcp_id` or `dhcp` short: are present. If set to `true`, requires that either `dhcp_id` or `dhcp` to be present.
-    
     """
 
 
 @dataclass
 class UpdateGatewayNetworkRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     gateway_network_id: str
     """
-    ID of the GatewayNetwork to update
+    ID of the GatewayNetwork to update.
     """
 
     enable_masquerade: Optional[bool]
     """
-    New masquerade enablement
+    New masquerade enablement.
     """
 
     dhcp_id: Optional[str]
     """
     New DHCP configuration.
     
     One-of ('ip_config'): at most one of 'dhcp_id', 'address' could be set.
     """
 
     enable_dhcp: Optional[bool]
     """
-    Whether to enable DHCP on the connected Private Network
+    Whether to enable DHCP on the connected Private Network.
     """
 
     address: Optional[str]
     """
     New static IP address.
     
     One-of ('ip_config'): at most one of 'dhcp_id', 'address' could be set.
     """
 
 
 @dataclass
 class DeleteGatewayNetworkRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     gateway_network_id: str
     """
-    GatewayNetwork to delete
+    GatewayNetwork to delete.
     """
 
     cleanup_dhcp: bool
     """
     Whether to cleanup the attached DHCP configuration (if any, and if not attached to another gateway_network).
-    
     """
 
 
 @dataclass
 class ListDHCPsRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     order_by: Optional[ListDHCPsRequestOrderBy]
     """
-    Order in which to return results
+    Order in which to return results.
     """
 
     page: Optional[int]
     """
-    Page number
+    Page number.
     """
 
     page_size: Optional[int]
     """
-    DHCP configurations per page
+    DHCP configurations per page.
     """
 
     organization_id: Optional[str]
     """
-    Include only DHCPs in this organization
+    Include only DHCPs in this organization.
     """
 
     project_id: Optional[str]
     """
-    Include only DHCPs in this project
+    Include only DHCPs in this project.
     """
 
     address: Optional[str]
     """
-    Filter on gateway address
+    Filter on gateway address.
     """
 
     has_address: Optional[str]
     """
-    Filter on subnets containing address
+    Filter on subnets containing address.
     """
 
 
 @dataclass
 class GetDHCPRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     dhcp_id: str
     """
-    ID of the DHCP config to fetch
+    ID of the DHCP config to fetch.
     """
 
 
 @dataclass
 class CreateDHCPRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     project_id: Optional[str]
     """
-    Project to create the DHCP configuration in
+    Project to create the DHCP configuration in.
     """
 
     subnet: str
     """
-    Subnet for the DHCP server
+    Subnet for the DHCP server.
     """
 
     address: Optional[str]
     """
-    Address of the DHCP server. This will be the gateway's address in the private network. Defaults to the first address of the subnet
+    Address of the DHCP server. This will be the gateway's address in the private network. Defaults to the first address of the subnet.
     """
 
     pool_low: Optional[str]
     """
     Low IP (included) of the dynamic address pool. Defaults to the second address of the subnet.
     """
 
@@ -1214,569 +1209,561 @@
     """
     High IP (included) of the dynamic address pool. Defaults to the last address of the subnet.
     """
 
     enable_dynamic: Optional[bool]
     """
     Whether to enable dynamic pooling of IPs. By turning the dynamic pool off, only pre-existing DHCP reservations will be handed out. Defaults to true.
-    
     """
 
     valid_lifetime: Optional[str]
     """
     For how long, in seconds, will DHCP entries will be valid. Defaults to 1h (3600s).
     """
 
     renew_timer: Optional[str]
     """
     After how long, in seconds, a renew will be attempted. Must be 30s lower than `rebind_timer`. Defaults to 50m (3000s).
-    
     """
 
     rebind_timer: Optional[str]
     """
     After how long, in seconds, a DHCP client will query for a new lease if previous renews fail. Must be 30s lower than `valid_lifetime`. Defaults to 51m (3060s).
-    
     """
 
     push_default_route: Optional[bool]
     """
-    Whether the gateway should push a default route to DHCP clients or only hand out IPs. Defaults to true
+    Whether the gateway should push a default route to DHCP clients or only hand out IPs. Defaults to true.
     """
 
     push_dns_server: Optional[bool]
     """
     Whether the gateway should push custom DNS servers to clients. This allows for instance hostname -> IP resolution. Defaults to true.
-    
     """
 
     dns_servers_override: Optional[List[str]]
     """
-    Override the DNS server list pushed to DHCP clients, instead of the gateway itself
+    Override the DNS server list pushed to DHCP clients, instead of the gateway itself.
     """
 
     dns_search: Optional[List[str]]
     """
-    Additional DNS search paths
+    Additional DNS search paths.
     """
 
     dns_local_name: Optional[str]
     """
     TLD given to hostnames in the Private Network. Allowed characters are `a-z0-9-.`. Defaults to the slugified Private Network name if created along a GatewayNetwork, or else to `priv`.
-    
     """
 
 
 @dataclass
 class UpdateDHCPRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     dhcp_id: str
     """
-    DHCP config to update
+    DHCP config to update.
     """
 
     subnet: Optional[str]
     """
-    Subnet for the DHCP server
+    Subnet for the DHCP server.
     """
 
     address: Optional[str]
     """
-    Address of the DHCP server. This will be the gateway's address in the private network
+    Address of the DHCP server. This will be the gateway's address in the private network.
     """
 
     pool_low: Optional[str]
     """
-    Low IP (included) of the dynamic address pool
+    Low IP (included) of the dynamic address pool.
     """
 
     pool_high: Optional[str]
     """
-    High IP (included) of the dynamic address pool
+    High IP (included) of the dynamic address pool.
     """
 
     enable_dynamic: Optional[bool]
     """
     Whether to enable dynamic pooling of IPs. By turning the dynamic pool off, only pre-existing DHCP reservations will be handed out. Defaults to true.
-    
     """
 
     valid_lifetime: Optional[str]
     """
-    How long, in seconds, DHCP entries will be valid for
+    How long, in seconds, DHCP entries will be valid for.
     """
 
     renew_timer: Optional[str]
     """
     After how long, in seconds, a renew will be attempted. Must be 30s lower than `rebind_timer`.
     """
 
     rebind_timer: Optional[str]
     """
     After how long, in seconds, a DHCP client will query for a new lease if previous renews fail. Must be 30s lower than `valid_lifetime`.
-    
     """
 
     push_default_route: Optional[bool]
     """
-    Whether the gateway should push a default route to DHCP clients or only hand out IPs
+    Whether the gateway should push a default route to DHCP clients or only hand out IPs.
     """
 
     push_dns_server: Optional[bool]
     """
     Whether the gateway should push custom DNS servers to clients. This allows for instance hostname -> IP resolution.
-    
     """
 
     dns_servers_override: Optional[List[str]]
     """
-    Override the DNS server list pushed to DHCP clients, instead of the gateway itself
+    Override the DNS server list pushed to DHCP clients, instead of the gateway itself.
     """
 
     dns_search: Optional[List[str]]
     """
-    Additional DNS search paths
+    Additional DNS search paths.
     """
 
     dns_local_name: Optional[str]
     """
     TLD given to hostnames in the Private Network. Allowed characters are `a-z0-9-.`.
     """
 
 
 @dataclass
 class DeleteDHCPRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     dhcp_id: str
     """
-    DHCP config id to delete
+    DHCP config id to delete.
     """
 
 
 @dataclass
 class ListDHCPEntriesRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     order_by: Optional[ListDHCPEntriesRequestOrderBy]
     """
-    Order in which to return results
+    Order in which to return results.
     """
 
     page: Optional[int]
     """
-    Page number
+    Page number.
     """
 
     page_size: Optional[int]
     """
-    DHCP entries per page
+    DHCP entries per page.
     """
 
     gateway_network_id: Optional[str]
     """
-    Filter entries based on the gateway network they are on
+    Filter entries based on the gateway network they are on.
     """
 
     mac_address: Optional[str]
     """
-    Filter entries on their MAC address
+    Filter entries on their MAC address.
     """
 
     ip_address: Optional[str]
     """
-    Filter entries on their IP address
+    Filter entries on their IP address.
     """
 
     hostname: Optional[str]
     """
-    Filter entries on their hostname substring
+    Filter entries on their hostname substring.
     """
 
     type_: Optional[DHCPEntryType]
     """
-    Filter entries on their type
+    Filter entries on their type.
     """
 
 
 @dataclass
 class GetDHCPEntryRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     dhcp_entry_id: str
     """
-    ID of the DHCP entry to fetch
+    ID of the DHCP entry to fetch.
     """
 
 
 @dataclass
 class CreateDHCPEntryRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     gateway_network_id: str
     """
-    GatewayNetwork on which to create a DHCP reservation
+    GatewayNetwork on which to create a DHCP reservation.
     """
 
     mac_address: str
     """
-    MAC address to give a static entry to
+    MAC address to give a static entry to.
     """
 
     ip_address: str
     """
-    IP address to give to the machine
+    IP address to give to the machine.
     """
 
 
 @dataclass
 class UpdateDHCPEntryRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     dhcp_entry_id: str
     """
-    DHCP entry ID to update
+    DHCP entry ID to update.
     """
 
     ip_address: Optional[str]
     """
-    New IP address to give to the machine
+    New IP address to give to the machine.
     """
 
 
 @dataclass
 class SetDHCPEntriesRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     gateway_network_id: str
     """
-    Gateway Network on which to set DHCP reservation list
+    Gateway Network on which to set DHCP reservation list.
     """
 
     dhcp_entries: Optional[List[SetDHCPEntriesRequestEntry]]
     """
-    New list of DHCP reservations
+    New list of DHCP reservations.
     """
 
 
 @dataclass
 class DeleteDHCPEntryRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     dhcp_entry_id: str
     """
-    DHCP entry ID to delete
+    DHCP entry ID to delete.
     """
 
 
 @dataclass
 class ListPATRulesRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     order_by: Optional[ListPATRulesRequestOrderBy]
     """
-    Order in which to return results
+    Order in which to return results.
     """
 
     page: Optional[int]
     """
-    Page number
+    Page number.
     """
 
     page_size: Optional[int]
     """
-    PAT rules per page
+    PAT rules per page.
     """
 
     gateway_id: Optional[str]
     """
-    Fetch rules for this gateway
+    Fetch rules for this gateway.
     """
 
     private_ip: Optional[str]
     """
-    Fetch rules targeting this private ip
+    Fetch rules targeting this private ip.
     """
 
     protocol: Optional[PATRuleProtocol]
     """
-    Fetch rules for this protocol
+    Fetch rules for this protocol.
     """
 
 
 @dataclass
 class GetPATRuleRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     pat_rule_id: str
     """
-    PAT rule to get
+    PAT rule to get.
     """
 
 
 @dataclass
 class CreatePATRuleRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     gateway_id: str
     """
-    Gateway on which to attach the rule to
+    Gateway on which to attach the rule to.
     """
 
     public_port: int
     """
-    Public port to listen on
+    Public port to listen on.
     """
 
     private_ip: str
     """
-    Private IP to forward data to
+    Private IP to forward data to.
     """
 
     private_port: int
     """
-    Private port to translate to
+    Private port to translate to.
     """
 
     protocol: PATRuleProtocol
     """
-    Protocol the rule should apply to
+    Protocol the rule should apply to.
     """
 
 
 @dataclass
 class UpdatePATRuleRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     pat_rule_id: str
     """
-    PAT rule to update
+    PAT rule to update.
     """
 
     public_port: Optional[int]
     """
-    Public port to listen on
+    Public port to listen on.
     """
 
     private_ip: Optional[str]
     """
-    Private IP to forward data to
+    Private IP to forward data to.
     """
 
     private_port: Optional[int]
     """
-    Private port to translate to
+    Private port to translate to.
     """
 
     protocol: PATRuleProtocol
     """
-    Protocol the rule should apply to
+    Protocol the rule should apply to.
     """
 
 
 @dataclass
 class SetPATRulesRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     gateway_id: str
     """
-    Gateway on which to set the PAT rules
+    Gateway on which to set the PAT rules.
     """
 
     pat_rules: List[SetPATRulesRequestRule]
     """
-    New list of PAT rules
+    New list of PAT rules.
     """
 
 
 @dataclass
 class DeletePATRuleRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     pat_rule_id: str
     """
-    PAT rule to delete
+    PAT rule to delete.
     """
 
 
 @dataclass
 class ListGatewayTypesRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
 
 @dataclass
 class ListIPsRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     order_by: Optional[ListIPsRequestOrderBy]
     """
-    Order in which to return results
+    Order in which to return results.
     """
 
     page: Optional[int]
     """
-    Page number
+    Page number.
     """
 
     page_size: Optional[int]
     """
-    IPs per page
+    IPs per page.
     """
 
     organization_id: Optional[str]
     """
-    Include only IPs in this organization
+    Include only IPs in this organization.
     """
 
     project_id: Optional[str]
     """
-    Include only IPs in this project
+    Include only IPs in this project.
     """
 
     tags: Optional[List[str]]
     """
-    Filter IPs with these tags
+    Filter IPs with these tags.
     """
 
     reverse: Optional[str]
     """
-    Filter by reverse containing this string
+    Filter by reverse containing this string.
     """
 
     is_free: Optional[bool]
     """
-    Filter whether the IP is attached to a gateway or not
+    Filter whether the IP is attached to a gateway or not.
     """
 
 
 @dataclass
 class GetIPRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     ip_id: str
     """
-    ID of the IP to get
+    ID of the IP to get.
     """
 
 
 @dataclass
 class CreateIPRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     project_id: Optional[str]
     """
-    Project to create the IP into
+    Project to create the IP into.
     """
 
     tags: Optional[List[str]]
     """
-    Tags to give to the IP
+    Tags to give to the IP.
     """
 
 
 @dataclass
 class UpdateIPRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     ip_id: str
     """
-    ID of the IP to update
+    ID of the IP to update.
     """
 
     tags: Optional[List[str]]
     """
-    Tags to give to the IP
+    Tags to give to the IP.
     """
 
     reverse: Optional[str]
     """
-    Reverse to set on the IP. Empty string to unset
+    Reverse to set on the IP. Empty string to unset.
     """
 
     gateway_id: Optional[str]
     """
-    Gateway to attach the IP to. Empty string to detach
+    Gateway to attach the IP to. Empty string to detach.
     """
 
 
 @dataclass
 class DeleteIPRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     ip_id: str
     """
-    ID of the IP to delete
+    ID of the IP to delete.
     """
 
 
 @dataclass
 class RefreshSSHKeysRequest:
     zone: Optional[Zone]
     """
-    Zone to target. If none is passed will use default zone from the config
+    Zone to target. If none is passed will use default zone from the config.
     """
 
     gateway_id: str
     """
-    ID of the gateway that needs fresh ssh keys
+    ID of the gateway that needs fresh ssh keys.
     """
```

### Comparing `scaleway_async-0.8.0/PKG-INFO` & `scaleway_async-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scaleway-async
-Version: 0.8.0
+Version: 0.9.0
 Summary: Scaleway SDK for Python
 License: BSD
 Author: Scaleway
 Author-email: opensource@scaleway.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

