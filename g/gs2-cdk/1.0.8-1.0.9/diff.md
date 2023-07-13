# Comparing `tmp/gs2-cdk-1.0.8.tar.gz` & `tmp/gs2-cdk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gs2-cdk-1.0.8.tar", last modified: Mon Jan 23 16:54:13 2023, max compression
+gzip compressed data, was "gs2-cdk-1.0.9.tar", last modified: Tue Jan 31 06:28:11 2023, max compression
```

## Comparing `gs2-cdk-1.0.8.tar` & `gs2-cdk-1.0.9.tar`

### file list

```diff
@@ -1,604 +1,604 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.036736 gs2-cdk-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      368 2023-01-23 16:54:13.036736 gs2-cdk-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-23 16:54:13.036736 gs2-cdk-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1273 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.884736 gs2-cdk-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.892736 gs2-cdk-1.0.8/src/gs2_cdk/
--rw-r--r--   0 root         (0) root         (0)      226 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.892736 gs2-cdk-1.0.8/src/gs2_cdk/account/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/account/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.892736 gs2-cdk-1.0.8/src/gs2_cdk/account/model/
--rw-r--r--   0 root         (0) root         (0)     4469 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/account/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)      672 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/account/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.892736 gs2-cdk-1.0.8/src/gs2_cdk/account/ref/
--rw-r--r--   0 root         (0) root         (0)     1235 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/account/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/account/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.892736 gs2-cdk-1.0.8/src/gs2_cdk/account/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/account/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.892736 gs2-cdk-1.0.8/src/gs2_cdk/auth/
--rw-r--r--   0 root         (0) root         (0)      652 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/auth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.892736 gs2-cdk-1.0.8/src/gs2_cdk/auth/model/
--rw-r--r--   0 root         (0) root         (0)     1750 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/auth/model/AccessToken.py
--rw-r--r--   0 root         (0) root         (0)      680 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/auth/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.892736 gs2-cdk-1.0.8/src/gs2_cdk/auth/ref/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/auth/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.892736 gs2-cdk-1.0.8/src/gs2_cdk/auth/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/auth/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.896736 gs2-cdk-1.0.8/src/gs2_cdk/chat/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/chat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.896736 gs2-cdk-1.0.8/src/gs2_cdk/chat/model/
--rw-r--r--   0 root         (0) root         (0)     4557 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/chat/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     1532 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/chat/model/NotificationType.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/chat/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.896736 gs2-cdk-1.0.8/src/gs2_cdk/chat/ref/
--rw-r--r--   0 root         (0) root         (0)     1232 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/chat/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/chat/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.896736 gs2-cdk-1.0.8/src/gs2_cdk/chat/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/chat/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.896736 gs2-cdk-1.0.8/src/gs2_cdk/core/
--rw-r--r--   0 root         (0) root         (0)       41 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1234 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/core/func.py
--rw-r--r--   0 root         (0) root         (0)     6875 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/core/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.896736 gs2-cdk-1.0.8/src/gs2_cdk/datastore/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/datastore/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.896736 gs2-cdk-1.0.8/src/gs2_cdk/datastore/model/
--rw-r--r--   0 root         (0) root         (0)     2706 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/datastore/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)      672 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/datastore/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.896736 gs2-cdk-1.0.8/src/gs2_cdk/datastore/ref/
--rw-r--r--   0 root         (0) root         (0)     1237 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/datastore/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/datastore/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.896736 gs2-cdk-1.0.8/src/gs2_cdk/datastore/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/datastore/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.896736 gs2-cdk-1.0.8/src/gs2_cdk/dictionary/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/dictionary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.900736 gs2-cdk-1.0.8/src/gs2_cdk/dictionary/model/
--rw-r--r--   0 root         (0) root         (0)     1991 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/dictionary/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/dictionary/model/EntryModel.py
--rw-r--r--   0 root         (0) root         (0)     3348 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/dictionary/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)      813 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/dictionary/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.900736 gs2-cdk-1.0.8/src/gs2_cdk/dictionary/ref/
--rw-r--r--   0 root         (0) root         (0)     1739 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/dictionary/ref/EntryModelRef.py
--rw-r--r--   0 root         (0) root         (0)     1821 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/dictionary/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      664 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/dictionary/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.900736 gs2-cdk-1.0.8/src/gs2_cdk/dictionary/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)     1210 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/dictionary/stamp_sheet/AddEntriesByUserId.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/dictionary/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.900736 gs2-cdk-1.0.8/src/gs2_cdk/distributor/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/distributor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.900736 gs2-cdk-1.0.8/src/gs2_cdk/distributor/model/
--rw-r--r--   0 root         (0) root         (0)     2071 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/distributor/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     1305 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/distributor/model/DistributeResource.py
--rw-r--r--   0 root         (0) root         (0)     1866 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/distributor/model/DistributorModel.py
--rw-r--r--   0 root         (0) root         (0)     3444 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/distributor/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     3044 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/distributor/model/StampSheetResult.py
--rw-r--r--   0 root         (0) root         (0)     1077 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/distributor/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.904736 gs2-cdk-1.0.8/src/gs2_cdk/distributor/ref/
--rw-r--r--   0 root         (0) root         (0)     1416 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/distributor/ref/DistributorModelRef.py
--rw-r--r--   0 root         (0) root         (0)     1504 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/distributor/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      676 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/distributor/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.904736 gs2-cdk-1.0.8/src/gs2_cdk/distributor/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/distributor/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.904736 gs2-cdk-1.0.8/src/gs2_cdk/enhance/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/enhance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.904736 gs2-cdk-1.0.8/src/gs2_cdk/enhance/model/
--rw-r--r--   0 root         (0) root         (0)     1237 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/enhance/model/BonusRate.py
--rw-r--r--   0 root         (0) root         (0)     1972 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/enhance/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     1330 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/enhance/model/Material.py
--rw-r--r--   0 root         (0) root         (0)     3649 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/enhance/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     3273 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/enhance/model/RateModel.py
--rw-r--r--   0 root         (0) root         (0)      981 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/enhance/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.908736 gs2-cdk-1.0.8/src/gs2_cdk/enhance/ref/
--rw-r--r--   0 root         (0) root         (0)     2304 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/enhance/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)     1374 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/enhance/ref/RateModelRef.py
--rw-r--r--   0 root         (0) root         (0)      662 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/enhance/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.908736 gs2-cdk-1.0.8/src/gs2_cdk/enhance/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)     1469 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/enhance/stamp_sheet/CreateProgressByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/enhance/stamp_sheet/DeleteProgressByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/enhance/stamp_sheet/DirectEnhanceByUserId.py
--rw-r--r--   0 root         (0) root         (0)      759 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/enhance/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.908736 gs2-cdk-1.0.8/src/gs2_cdk/exchange/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/exchange/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.908736 gs2-cdk-1.0.8/src/gs2_cdk/exchange/model/
--rw-r--r--   0 root         (0) root         (0)     1974 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/exchange/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     3950 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/exchange/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     4418 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/exchange/model/RateModel.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/exchange/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.908736 gs2-cdk-1.0.8/src/gs2_cdk/exchange/ref/
--rw-r--r--   0 root         (0) root         (0)     2641 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/exchange/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)     1371 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/exchange/ref/RateModelRef.py
--rw-r--r--   0 root         (0) root         (0)      662 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/exchange/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.912736 gs2-cdk-1.0.8/src/gs2_cdk/exchange/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)     1237 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/exchange/stamp_sheet/CreateAwaitByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1251 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/exchange/stamp_sheet/DeleteAwaitByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1332 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/exchange/stamp_sheet/ExchangeByUserId.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/exchange/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.912736 gs2-cdk-1.0.8/src/gs2_cdk/experience/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/experience/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.912736 gs2-cdk-1.0.8/src/gs2_cdk/experience/model/
--rw-r--r--   0 root         (0) root         (0)     2056 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/experience/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     2222 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/experience/model/ExperienceModel.py
--rw-r--r--   0 root         (0) root         (0)     4413 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/experience/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     1305 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/experience/model/Threshold.py
--rw-r--r--   0 root         (0) root         (0)      921 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/experience/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.912736 gs2-cdk-1.0.8/src/gs2_cdk/experience/ref/
--rw-r--r--   0 root         (0) root         (0)     1409 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/experience/ref/ExperienceModelRef.py
--rw-r--r--   0 root         (0) root         (0)     2840 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/experience/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      756 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/experience/ref/ThresholdRef.py
--rw-r--r--   0 root         (0) root         (0)      713 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/experience/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.912736 gs2-cdk-1.0.8/src/gs2_cdk/experience/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)     1366 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/experience/stamp_sheet/AddExperienceByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/experience/stamp_sheet/AddRankCapByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/experience/stamp_sheet/SetRankCapByUserId.py
--rw-r--r--   0 root         (0) root         (0)      743 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/experience/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.912736 gs2-cdk-1.0.8/src/gs2_cdk/formation/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/formation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.916736 gs2-cdk-1.0.8/src/gs2_cdk/formation/model/
--rw-r--r--   0 root         (0) root         (0)     1446 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/formation/model/AcquireActionConfig.py
--rw-r--r--   0 root         (0) root         (0)     2303 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/formation/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/formation/model/FormModel.py
--rw-r--r--   0 root         (0) root         (0)     1994 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/formation/model/MoldModel.py
--rw-r--r--   0 root         (0) root         (0)     3807 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/formation/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     1437 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/formation/model/Slot.py
--rw-r--r--   0 root         (0) root         (0)     1483 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/formation/model/SlotModel.py
--rw-r--r--   0 root         (0) root         (0)     1957 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/formation/model/SlotWithSignature.py
--rw-r--r--   0 root         (0) root         (0)     1379 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/formation/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.916736 gs2-cdk-1.0.8/src/gs2_cdk/formation/ref/
--rw-r--r--   0 root         (0) root         (0)     2104 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/formation/ref/FormModelRef.py
--rw-r--r--   0 root         (0) root         (0)     2801 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/formation/ref/MoldModelRef.py
--rw-r--r--   0 root         (0) root         (0)     3786 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/formation/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/formation/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.920736 gs2-cdk-1.0.8/src/gs2_cdk/formation/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)     1493 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/formation/stamp_sheet/AcquireActionsToFormProperties.py
--rw-r--r--   0 root         (0) root         (0)     1543 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/formation/stamp_sheet/AcquireActionsToPropertyFormProperties.py
--rw-r--r--   0 root         (0) root         (0)     1238 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/formation/stamp_sheet/AddMoldCapacityByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1238 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/formation/stamp_sheet/SetMoldCapacityByUserId.py
--rw-r--r--   0 root         (0) root         (0)      872 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/formation/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.920736 gs2-cdk-1.0.8/src/gs2_cdk/friend/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/friend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.920736 gs2-cdk-1.0.8/src/gs2_cdk/friend/model/
--rw-r--r--   0 root         (0) root         (0)     5946 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/friend/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)      672 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/friend/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.920736 gs2-cdk-1.0.8/src/gs2_cdk/friend/ref/
--rw-r--r--   0 root         (0) root         (0)     1234 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/friend/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/friend/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.920736 gs2-cdk-1.0.8/src/gs2_cdk/friend/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/friend/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.920736 gs2-cdk-1.0.8/src/gs2_cdk/gateway/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/gateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.920736 gs2-cdk-1.0.8/src/gs2_cdk/gateway/model/
--rw-r--r--   0 root         (0) root         (0)     2606 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/gateway/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)      672 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/gateway/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.920736 gs2-cdk-1.0.8/src/gs2_cdk/gateway/ref/
--rw-r--r--   0 root         (0) root         (0)     1235 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/gateway/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/gateway/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.920736 gs2-cdk-1.0.8/src/gs2_cdk/gateway/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/gateway/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.920736 gs2-cdk-1.0.8/src/gs2_cdk/identifier/
--rw-r--r--   0 root         (0) root         (0)      887 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/identifier/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.924736 gs2-cdk-1.0.8/src/gs2_cdk/identifier/model/
--rw-r--r--   0 root         (0) root         (0)     1640 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/identifier/model/AttachSecurityPolicy.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/identifier/model/Identifier.py
--rw-r--r--   0 root         (0) root         (0)     2046 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/identifier/model/Password.py
--rw-r--r--   0 root         (0) root         (0)     1156 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/identifier/model/Policy.py
--rw-r--r--   0 root         (0) root         (0)     1138 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/identifier/model/ProjectToken.py
--rw-r--r--   0 root         (0) root         (0)     2499 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/identifier/model/SecurityPolicy.py
--rw-r--r--   0 root         (0) root         (0)     1871 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/identifier/model/Statement.py
--rw-r--r--   0 root         (0) root         (0)     3043 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/identifier/model/User.py
--rw-r--r--   0 root         (0) root         (0)     1247 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/identifier/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.924736 gs2-cdk-1.0.8/src/gs2_cdk/identifier/ref/
--rw-r--r--   0 root         (0) root         (0)     1194 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/identifier/ref/AttachSecurityPolicyRef.py
--rw-r--r--   0 root         (0) root         (0)      900 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/identifier/ref/IdentifierRef.py
--rw-r--r--   0 root         (0) root         (0)     1182 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/identifier/ref/PasswordRef.py
--rw-r--r--   0 root         (0) root         (0)     1253 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/identifier/ref/SecurityPolicyRef.py
--rw-r--r--   0 root         (0) root         (0)     1219 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/identifier/ref/UserRef.py
--rw-r--r--   0 root         (0) root         (0)      801 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/identifier/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.924736 gs2-cdk-1.0.8/src/gs2_cdk/identifier/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/identifier/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.924736 gs2-cdk-1.0.8/src/gs2_cdk/inbox/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inbox/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.928736 gs2-cdk-1.0.8/src/gs2_cdk/inbox/model/
--rw-r--r--   0 root         (0) root         (0)     2018 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inbox/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     2215 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inbox/model/GlobalMessage.py
--rw-r--r--   0 root         (0) root         (0)     4784 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inbox/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     1377 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inbox/model/TimeSpan.py
--rw-r--r--   0 root         (0) root         (0)      909 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inbox/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.928736 gs2-cdk-1.0.8/src/gs2_cdk/inbox/ref/
--rw-r--r--   0 root         (0) root         (0)     1430 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inbox/ref/GlobalMessageRef.py
--rw-r--r--   0 root         (0) root         (0)     2476 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inbox/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      670 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inbox/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.928736 gs2-cdk-1.0.8/src/gs2_cdk/inbox/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)     1187 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inbox/stamp_sheet/OpenMessageByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1528 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inbox/stamp_sheet/SendMessageByUserId.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inbox/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.928736 gs2-cdk-1.0.8/src/gs2_cdk/inventory/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inventory/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.928736 gs2-cdk-1.0.8/src/gs2_cdk/inventory/model/
--rw-r--r--   0 root         (0) root         (0)     2041 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inventory/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     2340 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inventory/model/InventoryModel.py
--rw-r--r--   0 root         (0) root         (0)     1913 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inventory/model/ItemModel.py
--rw-r--r--   0 root         (0) root         (0)     3604 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inventory/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)      917 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inventory/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.932736 gs2-cdk-1.0.8/src/gs2_cdk/inventory/ref/
--rw-r--r--   0 root         (0) root         (0)     5056 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inventory/ref/InventoryModelRef.py
--rw-r--r--   0 root         (0) root         (0)     4087 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inventory/ref/ItemModelRef.py
--rw-r--r--   0 root         (0) root         (0)     5061 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inventory/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      711 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inventory/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.932736 gs2-cdk-1.0.8/src/gs2_cdk/inventory/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)     1627 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inventory/stamp_sheet/AcquireItemSetByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inventory/stamp_sheet/AddCapacityByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1424 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inventory/stamp_sheet/AddReferenceOfByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1427 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inventory/stamp_sheet/ConsumeItemSetByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inventory/stamp_sheet/DeleteReferenceOfByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inventory/stamp_sheet/SetCapacityByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1503 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inventory/stamp_sheet/VerifyReferenceOfByUserId.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/inventory/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.932736 gs2-cdk-1.0.8/src/gs2_cdk/job_queue/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/job_queue/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.932736 gs2-cdk-1.0.8/src/gs2_cdk/job_queue/model/
--rw-r--r--   0 root         (0) root         (0)     1444 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/job_queue/model/JobEntry.py
--rw-r--r--   0 root         (0) root         (0)     1625 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/job_queue/model/JobResultBody.py
--rw-r--r--   0 root         (0) root         (0)     3245 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/job_queue/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)      860 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/job_queue/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.932736 gs2-cdk-1.0.8/src/gs2_cdk/job_queue/ref/
--rw-r--r--   0 root         (0) root         (0)     1579 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/job_queue/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/job_queue/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.936736 gs2-cdk-1.0.8/src/gs2_cdk/job_queue/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)     1202 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/job_queue/stamp_sheet/PushByUserId.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/job_queue/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.936736 gs2-cdk-1.0.8/src/gs2_cdk/key/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/key/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.936736 gs2-cdk-1.0.8/src/gs2_cdk/key/model/
--rw-r--r--   0 root         (0) root         (0)     2060 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/key/model/GitHubApiKey.py
--rw-r--r--   0 root         (0) root         (0)     2229 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/key/model/Key.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/key/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)      836 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/key/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.936736 gs2-cdk-1.0.8/src/gs2_cdk/key/ref/
--rw-r--r--   0 root         (0) root         (0)     1385 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/key/ref/GitHubApiKeyRef.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/key/ref/KeyRef.py
--rw-r--r--   0 root         (0) root         (0)     1303 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/key/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      695 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/key/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.936736 gs2-cdk-1.0.8/src/gs2_cdk/key/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/key/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.936736 gs2-cdk-1.0.8/src/gs2_cdk/limit/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/limit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.936736 gs2-cdk-1.0.8/src/gs2_cdk/limit/model/
--rw-r--r--   0 root         (0) root         (0)     1981 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/limit/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     4534 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/limit/model/LimitModel.py
--rw-r--r--   0 root         (0) root         (0)     2713 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/limit/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     1307 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/limit/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.940736 gs2-cdk-1.0.8/src/gs2_cdk/limit/ref/
--rw-r--r--   0 root         (0) root         (0)     1374 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/limit/ref/LimitModelRef.py
--rw-r--r--   0 root         (0) root         (0)     2329 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/limit/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      664 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/limit/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.940736 gs2-cdk-1.0.8/src/gs2_cdk/limit/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/limit/stamp_sheet/CountUpByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1244 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/limit/stamp_sheet/DeleteCounterByUserId.py
--rw-r--r--   0 root         (0) root         (0)      686 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/limit/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.940736 gs2-cdk-1.0.8/src/gs2_cdk/lock/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lock/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.940736 gs2-cdk-1.0.8/src/gs2_cdk/lock/model/
--rw-r--r--   0 root         (0) root         (0)     2357 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lock/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)      672 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lock/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.940736 gs2-cdk-1.0.8/src/gs2_cdk/lock/ref/
--rw-r--r--   0 root         (0) root         (0)     1232 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lock/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lock/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.940736 gs2-cdk-1.0.8/src/gs2_cdk/lock/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lock/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.940736 gs2-cdk-1.0.8/src/gs2_cdk/log/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/log/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.944736 gs2-cdk-1.0.8/src/gs2_cdk/log/model/
--rw-r--r--   0 root         (0) root         (0)     2092 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/log/model/AccessLog.py
--rw-r--r--   0 root         (0) root         (0)     1672 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/log/model/AccessLogCount.py
--rw-r--r--   0 root         (0) root         (0)     2122 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/log/model/ExecuteStampSheetLog.py
--rw-r--r--   0 root         (0) root         (0)     1908 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/log/model/ExecuteStampSheetLogCount.py
--rw-r--r--   0 root         (0) root         (0)     2068 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/log/model/ExecuteStampTaskLog.py
--rw-r--r--   0 root         (0) root         (0)     1903 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/log/model/ExecuteStampTaskLogCount.py
--rw-r--r--   0 root         (0) root         (0)     2292 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/log/model/IssueStampSheetLog.py
--rw-r--r--   0 root         (0) root         (0)     1898 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/log/model/IssueStampSheetLogCount.py
--rw-r--r--   0 root         (0) root         (0)     4118 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/log/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     1981 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/log/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.944736 gs2-cdk-1.0.8/src/gs2_cdk/log/ref/
--rw-r--r--   0 root         (0) root         (0)     1231 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/log/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/log/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.944736 gs2-cdk-1.0.8/src/gs2_cdk/log/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/log/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.944736 gs2-cdk-1.0.8/src/gs2_cdk/lottery/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lottery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.948736 gs2-cdk-1.0.8/src/gs2_cdk/lottery/model/
--rw-r--r--   0 root         (0) root         (0)     1653 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lottery/model/BoxItem.py
--rw-r--r--   0 root         (0) root         (0)     2349 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lottery/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     1504 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lottery/model/DrawnPrize.py
--rw-r--r--   0 root         (0) root         (0)     3522 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lottery/model/LotteryModel.py
--rw-r--r--   0 root         (0) root         (0)     3810 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lottery/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     3632 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lottery/model/Prize.py
--rw-r--r--   0 root         (0) root         (0)     1651 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lottery/model/PrizeLimit.py
--rw-r--r--   0 root         (0) root         (0)     1603 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lottery/model/PrizeTable.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lottery/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.948736 gs2-cdk-1.0.8/src/gs2_cdk/lottery/ref/
--rw-r--r--   0 root         (0) root         (0)     1808 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lottery/ref/LotteryModelRef.py
--rw-r--r--   0 root         (0) root         (0)     1707 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lottery/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lottery/ref/PrizeLimitRef.py
--rw-r--r--   0 root         (0) root         (0)     1447 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lottery/ref/PrizeTableRef.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lottery/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.948736 gs2-cdk-1.0.8/src/gs2_cdk/lottery/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)     1332 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lottery/stamp_sheet/DrawByUserId.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/lottery/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.952736 gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.952736 gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/
--rw-r--r--   0 root         (0) root         (0)     1226 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/Attribute.py
--rw-r--r--   0 root         (0) root         (0)     1365 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/AttributeRange.py
--rw-r--r--   0 root         (0) root         (0)     1915 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/CapacityOfRole.py
--rw-r--r--   0 root         (0) root         (0)     2016 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     1244 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/GameResult.py
--rw-r--r--   0 root         (0) root         (0)     6971 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     1835 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/Player.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/RatingModel.py
--rw-r--r--   0 root         (0) root         (0)     1269 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/SignedBallot.py
--rw-r--r--   0 root         (0) root         (0)     1377 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/TimeSpan.py
--rw-r--r--   0 root         (0) root         (0)     2447 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.956736 gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/ref/
--rw-r--r--   0 root         (0) root         (0)     1469 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)     1386 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/ref/RatingModelRef.py
--rw-r--r--   0 root         (0) root         (0)      666 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.956736 gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.956736 gs2-cdk-1.0.8/src/gs2_cdk/megaField/
--rw-r--r--   0 root         (0) root         (0)      778 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/megaField/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.964736 gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/
--rw-r--r--   0 root         (0) root         (0)     1887 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/AreaModel.py
--rw-r--r--   0 root         (0) root         (0)     1981 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     2421 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/Layer.py
--rw-r--r--   0 root         (0) root         (0)     1597 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/LayerModel.py
--rw-r--r--   0 root         (0) root         (0)     1537 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/MyPosition.py
--rw-r--r--   0 root         (0) root         (0)     2947 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     1341 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/Position.py
--rw-r--r--   0 root         (0) root         (0)     1401 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/Scope.py
--rw-r--r--   0 root         (0) root         (0)     1335 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/Vector.py
--rw-r--r--   0 root         (0) root         (0)      877 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.972736 gs2-cdk-1.0.8/src/gs2_cdk/megaField/ref/
--rw-r--r--   0 root         (0) root         (0)     1467 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/megaField/ref/AreaModelRef.py
--rw-r--r--   0 root         (0) root         (0)     1597 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/megaField/ref/LayerModelRef.py
--rw-r--r--   0 root         (0) root         (0)     1543 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/megaField/ref/LayerRef.py
--rw-r--r--   0 root         (0) root         (0)     1525 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/megaField/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)     1366 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/megaField/ref/NodeRef.py
--rw-r--r--   0 root         (0) root         (0)      763 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/megaField/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.972736 gs2-cdk-1.0.8/src/gs2_cdk/megaField/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/megaField/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.972736 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.984736 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/
--rw-r--r--   0 root         (0) root         (0)     1638 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/AreaModel.py
--rw-r--r--   0 root         (0) root         (0)     1978 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     2350 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/Layer.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/LayerModel.py
--rw-r--r--   0 root         (0) root         (0)     1510 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/MyPosition.py
--rw-r--r--   0 root         (0) root         (0)     2716 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/Position.py
--rw-r--r--   0 root         (0) root         (0)     1365 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/Scope.py
--rw-r--r--   0 root         (0) root         (0)     1288 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/Vector.py
--rw-r--r--   0 root         (0) root         (0)     1297 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.992736 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/ref/
--rw-r--r--   0 root         (0) root         (0)     1467 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/ref/AreaModelRef.py
--rw-r--r--   0 root         (0) root         (0)     1597 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/ref/LayerModelRef.py
--rw-r--r--   0 root         (0) root         (0)     1543 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/ref/LayerRef.py
--rw-r--r--   0 root         (0) root         (0)     1525 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)     1366 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/ref/NodeRef.py
--rw-r--r--   0 root         (0) root         (0)      763 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.992736 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mega_field/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.992736 gs2-cdk-1.0.8/src/gs2_cdk/mission/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mission/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.000736 gs2-cdk-1.0.8/src/gs2_cdk/mission/model/
--rw-r--r--   0 root         (0) root         (0)     1932 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mission/model/CounterModel.py
--rw-r--r--   0 root         (0) root         (0)     4235 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mission/model/CounterScopeModel.py
--rw-r--r--   0 root         (0) root         (0)     2432 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mission/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     5956 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mission/model/MissionGroupModel.py
--rw-r--r--   0 root         (0) root         (0)     2766 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mission/model/MissionTaskModel.py
--rw-r--r--   0 root         (0) root         (0)     4620 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mission/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     1781 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mission/model/ScopedValue.py
--rw-r--r--   0 root         (0) root         (0)     2489 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mission/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.000736 gs2-cdk-1.0.8/src/gs2_cdk/mission/ref/
--rw-r--r--   0 root         (0) root         (0)     1759 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mission/ref/CounterModelRef.py
--rw-r--r--   0 root         (0) root         (0)     1728 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mission/ref/MissionGroupModelRef.py
--rw-r--r--   0 root         (0) root         (0)     1608 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mission/ref/MissionTaskModelRef.py
--rw-r--r--   0 root         (0) root         (0)     2524 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mission/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mission/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.004736 gs2-cdk-1.0.8/src/gs2_cdk/mission/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)     1236 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mission/stamp_sheet/IncreaseCounterByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1271 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mission/stamp_sheet/ReceiveByUserId.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/mission/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.004736 gs2-cdk-1.0.8/src/gs2_cdk/money/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/money/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.004736 gs2-cdk-1.0.8/src/gs2_cdk/money/model/
--rw-r--r--   0 root         (0) root         (0)     4611 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/money/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     1252 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/money/model/WalletDetail.py
--rw-r--r--   0 root         (0) root         (0)      880 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/money/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.004736 gs2-cdk-1.0.8/src/gs2_cdk/money/ref/
--rw-r--r--   0 root         (0) root         (0)     2346 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/money/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/money/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.004736 gs2-cdk-1.0.8/src/gs2_cdk/money/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)     1253 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/money/stamp_sheet/DepositByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1217 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/money/stamp_sheet/RecordReceipt.py
--rw-r--r--   0 root         (0) root         (0)     1282 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/money/stamp_sheet/WithdrawByUserId.py
--rw-r--r--   0 root         (0) root         (0)      717 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/money/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.004736 gs2-cdk-1.0.8/src/gs2_cdk/news/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/news/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.004736 gs2-cdk-1.0.8/src/gs2_cdk/news/model/
--rw-r--r--   0 root         (0) root         (0)     2357 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/news/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)      672 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/news/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.004736 gs2-cdk-1.0.8/src/gs2_cdk/news/ref/
--rw-r--r--   0 root         (0) root         (0)     1232 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/news/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/news/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.004736 gs2-cdk-1.0.8/src/gs2_cdk/news/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/news/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.004736 gs2-cdk-1.0.8/src/gs2_cdk/quest/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/quest/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.008736 gs2-cdk-1.0.8/src/gs2_cdk/quest/model/
--rw-r--r--   0 root         (0) root         (0)     1738 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/quest/model/Contents.py
--rw-r--r--   0 root         (0) root         (0)     2042 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/quest/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     4045 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/quest/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     2049 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/quest/model/QuestGroupModel.py
--rw-r--r--   0 root         (0) root         (0)     3451 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/quest/model/QuestModel.py
--rw-r--r--   0 root         (0) root         (0)     1542 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/quest/model/Reward.py
--rw-r--r--   0 root         (0) root         (0)     1085 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/quest/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.008736 gs2-cdk-1.0.8/src/gs2_cdk/quest/ref/
--rw-r--r--   0 root         (0) root         (0)     2279 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/quest/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)     1667 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/quest/ref/QuestGroupModelRef.py
--rw-r--r--   0 root         (0) root         (0)     1544 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/quest/ref/QuestModelRef.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/quest/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.008736 gs2-cdk-1.0.8/src/gs2_cdk/quest/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)     1373 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/quest/stamp_sheet/CreateProgressByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1100 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/quest/stamp_sheet/DeleteProgressByUserId.py
--rw-r--r--   0 root         (0) root         (0)      702 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/quest/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.008736 gs2-cdk-1.0.8/src/gs2_cdk/ranking/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/ranking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.012736 gs2-cdk-1.0.8/src/gs2_cdk/ranking/model/
--rw-r--r--   0 root         (0) root         (0)     1358 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/ranking/model/CalculatedAt.py
--rw-r--r--   0 root         (0) root         (0)     6245 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/ranking/model/CategoryModel.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/ranking/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     2732 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/ranking/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     1233 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/ranking/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.012736 gs2-cdk-1.0.8/src/gs2_cdk/ranking/ref/
--rw-r--r--   0 root         (0) root         (0)     1402 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/ranking/ref/CategoryModelRef.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/ranking/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      670 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/ranking/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.012736 gs2-cdk-1.0.8/src/gs2_cdk/ranking/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/ranking/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.012736 gs2-cdk-1.0.8/src/gs2_cdk/realtime/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/realtime/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.012736 gs2-cdk-1.0.8/src/gs2_cdk/realtime/model/
--rw-r--r--   0 root         (0) root         (0)     3270 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/realtime/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     2809 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/realtime/model/Room.py
--rw-r--r--   0 root         (0) root         (0)      856 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/realtime/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.012736 gs2-cdk-1.0.8/src/gs2_cdk/realtime/ref/
--rw-r--r--   0 root         (0) root         (0)     1265 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/realtime/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)     1365 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/realtime/ref/RoomRef.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/realtime/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.012736 gs2-cdk-1.0.8/src/gs2_cdk/realtime/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/realtime/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.012736 gs2-cdk-1.0.8/src/gs2_cdk/schedule/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/schedule/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.016736 gs2-cdk-1.0.8/src/gs2_cdk/schedule/model/
--rw-r--r--   0 root         (0) root         (0)     1926 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/schedule/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     8509 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/schedule/model/Event.py
--rw-r--r--   0 root         (0) root         (0)     2692 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/schedule/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     1547 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/schedule/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.016736 gs2-cdk-1.0.8/src/gs2_cdk/schedule/ref/
--rw-r--r--   0 root         (0) root         (0)     1236 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/schedule/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/schedule/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.016736 gs2-cdk-1.0.8/src/gs2_cdk/schedule/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/schedule/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.016736 gs2-cdk-1.0.8/src/gs2_cdk/script/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/script/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.016736 gs2-cdk-1.0.8/src/gs2_cdk/script/model/
--rw-r--r--   0 root         (0) root         (0)     2361 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/script/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     2423 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/script/model/Script.py
--rw-r--r--   0 root         (0) root         (0)      748 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/script/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.016736 gs2-cdk-1.0.8/src/gs2_cdk/script/ref/
--rw-r--r--   0 root         (0) root         (0)     1267 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/script/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)     1377 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/script/ref/ScriptRef.py
--rw-r--r--   0 root         (0) root         (0)      656 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/script/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.016736 gs2-cdk-1.0.8/src/gs2_cdk/script/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/script/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.016736 gs2-cdk-1.0.8/src/gs2_cdk/serialKey/
--rw-r--r--   0 root         (0) root         (0)      778 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serialKey/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.020736 gs2-cdk-1.0.8/src/gs2_cdk/serialKey/model/
--rw-r--r--   0 root         (0) root         (0)     1638 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serialKey/model/CampaignModel.py
--rw-r--r--   0 root         (0) root         (0)     2031 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serialKey/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     2392 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serialKey/model/IssueJob.py
--rw-r--r--   0 root         (0) root         (0)     2967 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serialKey/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     5467 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serialKey/model/SerialKey.py
--rw-r--r--   0 root         (0) root         (0)      847 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serialKey/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.020736 gs2-cdk-1.0.8/src/gs2_cdk/serialKey/ref/
--rw-r--r--   0 root         (0) root         (0)     1492 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serialKey/ref/CampaignModelRef.py
--rw-r--r--   0 root         (0) root         (0)     1633 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serialKey/ref/IssueJobRef.py
--rw-r--r--   0 root         (0) root         (0)     1807 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serialKey/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)     1612 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serialKey/ref/SerialKeyRef.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serialKey/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.020736 gs2-cdk-1.0.8/src/gs2_cdk/serialKey/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)     1125 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serialKey/stamp_sheet/UseByUserId.py
--rw-r--r--   0 root         (0) root         (0)      621 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serialKey/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.020736 gs2-cdk-1.0.8/src/gs2_cdk/serial_key/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serial_key/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.020736 gs2-cdk-1.0.8/src/gs2_cdk/serial_key/model/
--rw-r--r--   0 root         (0) root         (0)     1546 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serial_key/model/CampaignModel.py
--rw-r--r--   0 root         (0) root         (0)     2028 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serial_key/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     2103 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serial_key/model/IssueJob.py
--rw-r--r--   0 root         (0) root         (0)     2736 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serial_key/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     4447 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serial_key/model/SerialKey.py
--rw-r--r--   0 root         (0) root         (0)     1344 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serial_key/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.024736 gs2-cdk-1.0.8/src/gs2_cdk/serial_key/ref/
--rw-r--r--   0 root         (0) root         (0)     1492 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serial_key/ref/CampaignModelRef.py
--rw-r--r--   0 root         (0) root         (0)     1633 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serial_key/ref/IssueJobRef.py
--rw-r--r--   0 root         (0) root         (0)     1807 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serial_key/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)     1612 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serial_key/ref/SerialKeyRef.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serial_key/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.024736 gs2-cdk-1.0.8/src/gs2_cdk/serial_key/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)     1135 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serial_key/stamp_sheet/UseByUserId.py
--rw-r--r--   0 root         (0) root         (0)      621 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/serial_key/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.024736 gs2-cdk-1.0.8/src/gs2_cdk/showcase/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/showcase/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.024736 gs2-cdk-1.0.8/src/gs2_cdk/showcase/model/
--rw-r--r--   0 root         (0) root         (0)     1965 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/showcase/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     3494 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/showcase/model/DisplayItem.py
--rw-r--r--   0 root         (0) root         (0)     3331 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/showcase/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     2039 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/showcase/model/SalesItem.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/showcase/model/SalesItemGroup.py
--rw-r--r--   0 root         (0) root         (0)     2064 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/showcase/model/Showcase.py
--rw-r--r--   0 root         (0) root         (0)     1335 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/showcase/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.028736 gs2-cdk-1.0.8/src/gs2_cdk/showcase/ref/
--rw-r--r--   0 root         (0) root         (0)     1377 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/showcase/ref/DisplayItemRef.py
--rw-r--r--   0 root         (0) root         (0)     1474 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/showcase/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)      948 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/showcase/ref/SalesItemGroupRef.py
--rw-r--r--   0 root         (0) root         (0)      943 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/showcase/ref/SalesItemRef.py
--rw-r--r--   0 root         (0) root         (0)      754 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/showcase/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.028736 gs2-cdk-1.0.8/src/gs2_cdk/showcase/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/showcase/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.028736 gs2-cdk-1.0.8/src/gs2_cdk/stamina/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.028736 gs2-cdk-1.0.8/src/gs2_cdk/stamina/model/
--rw-r--r--   0 root         (0) root         (0)     2011 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     1708 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/model/MaxStaminaTable.py
--rw-r--r--   0 root         (0) root         (0)     3101 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     1733 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/model/RecoverIntervalTable.py
--rw-r--r--   0 root         (0) root         (0)     1718 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/model/RecoverValueTable.py
--rw-r--r--   0 root         (0) root         (0)     3476 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/model/StaminaModel.py
--rw-r--r--   0 root         (0) root         (0)     1185 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.028736 gs2-cdk-1.0.8/src/gs2_cdk/stamina/ref/
--rw-r--r--   0 root         (0) root         (0)     1451 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/ref/MaxStaminaTableRef.py
--rw-r--r--   0 root         (0) root         (0)     4771 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)     1486 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/ref/RecoverIntervalTableRef.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/ref/RecoverValueTableRef.py
--rw-r--r--   0 root         (0) root         (0)     3687 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/ref/StaminaModelRef.py
--rw-r--r--   0 root         (0) root         (0)      835 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.032736 gs2-cdk-1.0.8/src/gs2_cdk/stamina/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)     1257 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/stamp_sheet/ConsumeStaminaByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/stamp_sheet/RaiseMaxValueByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1257 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/stamp_sheet/RecoverStaminaByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1239 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/stamp_sheet/SetMaxValueByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1297 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/stamp_sheet/SetRecoverIntervalByUserId.py
--rw-r--r--   0 root         (0) root         (0)     1259 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/stamp_sheet/SetRecoverValueByUserId.py
--rw-r--r--   0 root         (0) root         (0)      940 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/stamina/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.032736 gs2-cdk-1.0.8/src/gs2_cdk/version/
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/version/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.032736 gs2-cdk-1.0.8/src/gs2_cdk/version/model/
--rw-r--r--   0 root         (0) root         (0)     2011 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/version/model/CurrentMasterData.py
--rw-r--r--   0 root         (0) root         (0)     3642 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/version/model/Namespace.py
--rw-r--r--   0 root         (0) root         (0)     1913 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/version/model/SignTargetVersion.py
--rw-r--r--   0 root         (0) root         (0)     1516 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/version/model/Status.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/version/model/TargetVersion.py
--rw-r--r--   0 root         (0) root         (0)     1365 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/version/model/Version.py
--rw-r--r--   0 root         (0) root         (0)     4063 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/version/model/VersionModel.py
--rw-r--r--   0 root         (0) root         (0)     1431 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/version/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.036736 gs2-cdk-1.0.8/src/gs2_cdk/version/ref/
--rw-r--r--   0 root         (0) root         (0)     1472 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/version/ref/NamespaceRef.py
--rw-r--r--   0 root         (0) root         (0)     1415 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/version/ref/VersionModelRef.py
--rw-r--r--   0 root         (0) root         (0)      668 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/version/ref/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:13.036736 gs2-cdk-1.0.8/src/gs2_cdk/version/stamp_sheet/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 16:51:54.000000 gs2-cdk-1.0.8/src/gs2_cdk/version/stamp_sheet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 16:54:12.892736 gs2-cdk-1.0.8/src/gs2_cdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      368 2023-01-23 16:54:12.000000 gs2-cdk-1.0.8/src/gs2_cdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18738 2023-01-23 16:54:12.000000 gs2-cdk-1.0.8/src/gs2_cdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-23 16:54:12.000000 gs2-cdk-1.0.8/src/gs2_cdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-01-23 16:54:12.000000 gs2-cdk-1.0.8/src/gs2_cdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.279558 gs2-cdk-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      368 2023-01-31 06:28:11.279558 gs2-cdk-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-01-31 06:28:11.279558 gs2-cdk-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.219557 gs2-cdk-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.227558 gs2-cdk-1.0.9/src/gs2_cdk/
+-rw-r--r--   0 root         (0) root         (0)      226 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.227558 gs2-cdk-1.0.9/src/gs2_cdk/account/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/account/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/account/model/
+-rw-r--r--   0 root         (0) root         (0)     4469 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/account/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)      672 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/account/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/account/ref/
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/account/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/account/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/account/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/account/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/auth/
+-rw-r--r--   0 root         (0) root         (0)      652 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/auth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/auth/model/
+-rw-r--r--   0 root         (0) root         (0)     1750 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/auth/model/AccessToken.py
+-rw-r--r--   0 root         (0) root         (0)      680 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/auth/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/auth/ref/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/auth/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/auth/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/auth/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/chat/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/chat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/chat/model/
+-rw-r--r--   0 root         (0) root         (0)     4557 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/chat/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/chat/model/NotificationType.py
+-rw-r--r--   0 root         (0) root         (0)      788 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/chat/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/chat/ref/
+-rw-r--r--   0 root         (0) root         (0)     1232 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/chat/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/chat/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/chat/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/chat/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/core/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/core/func.py
+-rw-r--r--   0 root         (0) root         (0)     6875 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/core/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/datastore/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/datastore/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/datastore/model/
+-rw-r--r--   0 root         (0) root         (0)     2706 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/datastore/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)      672 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/datastore/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/datastore/ref/
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/datastore/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/datastore/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/datastore/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/datastore/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/dictionary/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/dictionary/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/dictionary/model/
+-rw-r--r--   0 root         (0) root         (0)     1991 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/dictionary/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/dictionary/model/EntryModel.py
+-rw-r--r--   0 root         (0) root         (0)     3348 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/dictionary/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)      813 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/dictionary/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/dictionary/ref/
+-rw-r--r--   0 root         (0) root         (0)     1739 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/dictionary/ref/EntryModelRef.py
+-rw-r--r--   0 root         (0) root         (0)     1821 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/dictionary/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      664 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/dictionary/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/dictionary/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)     1210 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/dictionary/stamp_sheet/AddEntriesByUserId.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/dictionary/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.231557 gs2-cdk-1.0.9/src/gs2_cdk/distributor/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/distributor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.235558 gs2-cdk-1.0.9/src/gs2_cdk/distributor/model/
+-rw-r--r--   0 root         (0) root         (0)     2071 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/distributor/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/distributor/model/DistributeResource.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/distributor/model/DistributorModel.py
+-rw-r--r--   0 root         (0) root         (0)     3444 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/distributor/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     3044 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/distributor/model/StampSheetResult.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/distributor/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.235558 gs2-cdk-1.0.9/src/gs2_cdk/distributor/ref/
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/distributor/ref/DistributorModelRef.py
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/distributor/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      676 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/distributor/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.235558 gs2-cdk-1.0.9/src/gs2_cdk/distributor/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/distributor/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.235558 gs2-cdk-1.0.9/src/gs2_cdk/enhance/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/enhance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.235558 gs2-cdk-1.0.9/src/gs2_cdk/enhance/model/
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/enhance/model/BonusRate.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/enhance/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     1330 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/enhance/model/Material.py
+-rw-r--r--   0 root         (0) root         (0)     3649 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/enhance/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     3273 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/enhance/model/RateModel.py
+-rw-r--r--   0 root         (0) root         (0)      981 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/enhance/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.235558 gs2-cdk-1.0.9/src/gs2_cdk/enhance/ref/
+-rw-r--r--   0 root         (0) root         (0)     2304 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/enhance/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/enhance/ref/RateModelRef.py
+-rw-r--r--   0 root         (0) root         (0)      662 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/enhance/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.235558 gs2-cdk-1.0.9/src/gs2_cdk/enhance/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/enhance/stamp_sheet/CreateProgressByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/enhance/stamp_sheet/DeleteProgressByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/enhance/stamp_sheet/DirectEnhanceByUserId.py
+-rw-r--r--   0 root         (0) root         (0)      759 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/enhance/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.235558 gs2-cdk-1.0.9/src/gs2_cdk/exchange/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/exchange/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.235558 gs2-cdk-1.0.9/src/gs2_cdk/exchange/model/
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/exchange/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     3950 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/exchange/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     4418 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/exchange/model/RateModel.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/exchange/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.235558 gs2-cdk-1.0.9/src/gs2_cdk/exchange/ref/
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/exchange/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/exchange/ref/RateModelRef.py
+-rw-r--r--   0 root         (0) root         (0)      662 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/exchange/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.235558 gs2-cdk-1.0.9/src/gs2_cdk/exchange/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/exchange/stamp_sheet/CreateAwaitByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/exchange/stamp_sheet/DeleteAwaitByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1332 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/exchange/stamp_sheet/ExchangeByUserId.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/exchange/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.235558 gs2-cdk-1.0.9/src/gs2_cdk/experience/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/experience/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.239558 gs2-cdk-1.0.9/src/gs2_cdk/experience/model/
+-rw-r--r--   0 root         (0) root         (0)     2056 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/experience/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     2222 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/experience/model/ExperienceModel.py
+-rw-r--r--   0 root         (0) root         (0)     4413 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/experience/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/experience/model/Threshold.py
+-rw-r--r--   0 root         (0) root         (0)      921 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/experience/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.239558 gs2-cdk-1.0.9/src/gs2_cdk/experience/ref/
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/experience/ref/ExperienceModelRef.py
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/experience/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      756 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/experience/ref/ThresholdRef.py
+-rw-r--r--   0 root         (0) root         (0)      713 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/experience/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.239558 gs2-cdk-1.0.9/src/gs2_cdk/experience/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/experience/stamp_sheet/AddExperienceByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/experience/stamp_sheet/AddRankCapByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/experience/stamp_sheet/SetRankCapByUserId.py
+-rw-r--r--   0 root         (0) root         (0)      743 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/experience/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.239558 gs2-cdk-1.0.9/src/gs2_cdk/formation/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/formation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.239558 gs2-cdk-1.0.9/src/gs2_cdk/formation/model/
+-rw-r--r--   0 root         (0) root         (0)     1446 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/formation/model/AcquireActionConfig.py
+-rw-r--r--   0 root         (0) root         (0)     2303 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/formation/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/formation/model/FormModel.py
+-rw-r--r--   0 root         (0) root         (0)     1994 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/formation/model/MoldModel.py
+-rw-r--r--   0 root         (0) root         (0)     3807 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/formation/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/formation/model/Slot.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/formation/model/SlotModel.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/formation/model/SlotWithSignature.py
+-rw-r--r--   0 root         (0) root         (0)     1379 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/formation/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.239558 gs2-cdk-1.0.9/src/gs2_cdk/formation/ref/
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/formation/ref/FormModelRef.py
+-rw-r--r--   0 root         (0) root         (0)     2801 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/formation/ref/MoldModelRef.py
+-rw-r--r--   0 root         (0) root         (0)     3786 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/formation/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/formation/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.239558 gs2-cdk-1.0.9/src/gs2_cdk/formation/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)     1493 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/formation/stamp_sheet/AcquireActionsToFormProperties.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/formation/stamp_sheet/AcquireActionsToPropertyFormProperties.py
+-rw-r--r--   0 root         (0) root         (0)     1238 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/formation/stamp_sheet/AddMoldCapacityByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1238 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/formation/stamp_sheet/SetMoldCapacityByUserId.py
+-rw-r--r--   0 root         (0) root         (0)      872 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/formation/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.239558 gs2-cdk-1.0.9/src/gs2_cdk/friend/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/friend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.239558 gs2-cdk-1.0.9/src/gs2_cdk/friend/model/
+-rw-r--r--   0 root         (0) root         (0)     5946 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/friend/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)      672 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/friend/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.243558 gs2-cdk-1.0.9/src/gs2_cdk/friend/ref/
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/friend/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/friend/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.243558 gs2-cdk-1.0.9/src/gs2_cdk/friend/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/friend/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.243558 gs2-cdk-1.0.9/src/gs2_cdk/gateway/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/gateway/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.243558 gs2-cdk-1.0.9/src/gs2_cdk/gateway/model/
+-rw-r--r--   0 root         (0) root         (0)     2606 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/gateway/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)      672 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/gateway/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.243558 gs2-cdk-1.0.9/src/gs2_cdk/gateway/ref/
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/gateway/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/gateway/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.243558 gs2-cdk-1.0.9/src/gs2_cdk/gateway/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/gateway/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.243558 gs2-cdk-1.0.9/src/gs2_cdk/identifier/
+-rw-r--r--   0 root         (0) root         (0)      887 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/identifier/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.243558 gs2-cdk-1.0.9/src/gs2_cdk/identifier/model/
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/identifier/model/AttachSecurityPolicy.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/identifier/model/Identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/identifier/model/Password.py
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/identifier/model/Policy.py
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/identifier/model/ProjectToken.py
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/identifier/model/SecurityPolicy.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/identifier/model/Statement.py
+-rw-r--r--   0 root         (0) root         (0)     3043 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/identifier/model/User.py
+-rw-r--r--   0 root         (0) root         (0)     1247 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/identifier/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.243558 gs2-cdk-1.0.9/src/gs2_cdk/identifier/ref/
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/identifier/ref/AttachSecurityPolicyRef.py
+-rw-r--r--   0 root         (0) root         (0)      900 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/identifier/ref/IdentifierRef.py
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/identifier/ref/PasswordRef.py
+-rw-r--r--   0 root         (0) root         (0)     1253 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/identifier/ref/SecurityPolicyRef.py
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/identifier/ref/UserRef.py
+-rw-r--r--   0 root         (0) root         (0)      801 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/identifier/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.243558 gs2-cdk-1.0.9/src/gs2_cdk/identifier/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/identifier/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.243558 gs2-cdk-1.0.9/src/gs2_cdk/inbox/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inbox/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.243558 gs2-cdk-1.0.9/src/gs2_cdk/inbox/model/
+-rw-r--r--   0 root         (0) root         (0)     2018 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inbox/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     2215 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inbox/model/GlobalMessage.py
+-rw-r--r--   0 root         (0) root         (0)     4784 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inbox/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     1377 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inbox/model/TimeSpan.py
+-rw-r--r--   0 root         (0) root         (0)      909 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inbox/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.243558 gs2-cdk-1.0.9/src/gs2_cdk/inbox/ref/
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inbox/ref/GlobalMessageRef.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inbox/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      670 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inbox/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.247558 gs2-cdk-1.0.9/src/gs2_cdk/inbox/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)     1187 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inbox/stamp_sheet/OpenMessageByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inbox/stamp_sheet/SendMessageByUserId.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inbox/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.247558 gs2-cdk-1.0.9/src/gs2_cdk/inventory/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inventory/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.247558 gs2-cdk-1.0.9/src/gs2_cdk/inventory/model/
+-rw-r--r--   0 root         (0) root         (0)     2041 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inventory/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inventory/model/InventoryModel.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inventory/model/ItemModel.py
+-rw-r--r--   0 root         (0) root         (0)     3604 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inventory/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)      917 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inventory/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.247558 gs2-cdk-1.0.9/src/gs2_cdk/inventory/ref/
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inventory/ref/InventoryModelRef.py
+-rw-r--r--   0 root         (0) root         (0)     4087 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inventory/ref/ItemModelRef.py
+-rw-r--r--   0 root         (0) root         (0)     5061 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inventory/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      711 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inventory/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.247558 gs2-cdk-1.0.9/src/gs2_cdk/inventory/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)     1627 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inventory/stamp_sheet/AcquireItemSetByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inventory/stamp_sheet/AddCapacityByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1424 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inventory/stamp_sheet/AddReferenceOfByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inventory/stamp_sheet/ConsumeItemSetByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inventory/stamp_sheet/DeleteReferenceOfByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inventory/stamp_sheet/SetCapacityByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1503 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inventory/stamp_sheet/VerifyReferenceOfByUserId.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/inventory/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.247558 gs2-cdk-1.0.9/src/gs2_cdk/job_queue/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/job_queue/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.247558 gs2-cdk-1.0.9/src/gs2_cdk/job_queue/model/
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/job_queue/model/JobEntry.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/job_queue/model/JobResultBody.py
+-rw-r--r--   0 root         (0) root         (0)     3245 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/job_queue/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)      860 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/job_queue/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.247558 gs2-cdk-1.0.9/src/gs2_cdk/job_queue/ref/
+-rw-r--r--   0 root         (0) root         (0)     1579 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/job_queue/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/job_queue/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.247558 gs2-cdk-1.0.9/src/gs2_cdk/job_queue/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/job_queue/stamp_sheet/PushByUserId.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/job_queue/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.247558 gs2-cdk-1.0.9/src/gs2_cdk/key/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/key/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.247558 gs2-cdk-1.0.9/src/gs2_cdk/key/model/
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/key/model/GitHubApiKey.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/key/model/Key.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/key/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)      836 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/key/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.251558 gs2-cdk-1.0.9/src/gs2_cdk/key/ref/
+-rw-r--r--   0 root         (0) root         (0)     1385 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/key/ref/GitHubApiKeyRef.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/key/ref/KeyRef.py
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/key/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/key/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.251558 gs2-cdk-1.0.9/src/gs2_cdk/key/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/key/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.251558 gs2-cdk-1.0.9/src/gs2_cdk/limit/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/limit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.251558 gs2-cdk-1.0.9/src/gs2_cdk/limit/model/
+-rw-r--r--   0 root         (0) root         (0)     1981 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/limit/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     4534 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/limit/model/LimitModel.py
+-rw-r--r--   0 root         (0) root         (0)     2713 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/limit/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     1307 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/limit/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.251558 gs2-cdk-1.0.9/src/gs2_cdk/limit/ref/
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/limit/ref/LimitModelRef.py
+-rw-r--r--   0 root         (0) root         (0)     2329 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/limit/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      664 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/limit/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.251558 gs2-cdk-1.0.9/src/gs2_cdk/limit/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/limit/stamp_sheet/CountUpByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1244 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/limit/stamp_sheet/DeleteCounterByUserId.py
+-rw-r--r--   0 root         (0) root         (0)      686 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/limit/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.251558 gs2-cdk-1.0.9/src/gs2_cdk/lock/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lock/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.251558 gs2-cdk-1.0.9/src/gs2_cdk/lock/model/
+-rw-r--r--   0 root         (0) root         (0)     2357 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lock/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)      672 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lock/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.251558 gs2-cdk-1.0.9/src/gs2_cdk/lock/ref/
+-rw-r--r--   0 root         (0) root         (0)     1232 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lock/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lock/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.251558 gs2-cdk-1.0.9/src/gs2_cdk/lock/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lock/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.251558 gs2-cdk-1.0.9/src/gs2_cdk/log/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/log/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.251558 gs2-cdk-1.0.9/src/gs2_cdk/log/model/
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/log/model/AccessLog.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/log/model/AccessLogCount.py
+-rw-r--r--   0 root         (0) root         (0)     2122 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/log/model/ExecuteStampSheetLog.py
+-rw-r--r--   0 root         (0) root         (0)     1908 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/log/model/ExecuteStampSheetLogCount.py
+-rw-r--r--   0 root         (0) root         (0)     2068 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/log/model/ExecuteStampTaskLog.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/log/model/ExecuteStampTaskLogCount.py
+-rw-r--r--   0 root         (0) root         (0)     2292 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/log/model/IssueStampSheetLog.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/log/model/IssueStampSheetLogCount.py
+-rw-r--r--   0 root         (0) root         (0)     4118 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/log/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/log/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.251558 gs2-cdk-1.0.9/src/gs2_cdk/log/ref/
+-rw-r--r--   0 root         (0) root         (0)     1231 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/log/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/log/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.251558 gs2-cdk-1.0.9/src/gs2_cdk/log/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/log/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.251558 gs2-cdk-1.0.9/src/gs2_cdk/lottery/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lottery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.255558 gs2-cdk-1.0.9/src/gs2_cdk/lottery/model/
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lottery/model/BoxItem.py
+-rw-r--r--   0 root         (0) root         (0)     2349 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lottery/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lottery/model/DrawnPrize.py
+-rw-r--r--   0 root         (0) root         (0)     3522 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lottery/model/LotteryModel.py
+-rw-r--r--   0 root         (0) root         (0)     3810 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lottery/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     3632 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lottery/model/Prize.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lottery/model/PrizeLimit.py
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lottery/model/PrizeTable.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lottery/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.255558 gs2-cdk-1.0.9/src/gs2_cdk/lottery/ref/
+-rw-r--r--   0 root         (0) root         (0)     1808 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lottery/ref/LotteryModelRef.py
+-rw-r--r--   0 root         (0) root         (0)     1707 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lottery/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lottery/ref/PrizeLimitRef.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lottery/ref/PrizeTableRef.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lottery/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.255558 gs2-cdk-1.0.9/src/gs2_cdk/lottery/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)     1332 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lottery/stamp_sheet/DrawByUserId.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/lottery/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.255558 gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.255558 gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/
+-rw-r--r--   0 root         (0) root         (0)     1226 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/Attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1365 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/AttributeRange.py
+-rw-r--r--   0 root         (0) root         (0)     1915 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/CapacityOfRole.py
+-rw-r--r--   0 root         (0) root         (0)     2016 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     1244 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/GameResult.py
+-rw-r--r--   0 root         (0) root         (0)     6971 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     1835 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/Player.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/RatingModel.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/SignedBallot.py
+-rw-r--r--   0 root         (0) root         (0)     1377 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/TimeSpan.py
+-rw-r--r--   0 root         (0) root         (0)     2447 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.255558 gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/ref/
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/ref/RatingModelRef.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.255558 gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.255558 gs2-cdk-1.0.9/src/gs2_cdk/megaField/
+-rw-r--r--   0 root         (0) root         (0)      778 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/megaField/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.259558 gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/
+-rw-r--r--   0 root         (0) root         (0)     1887 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/AreaModel.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     2421 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/Layer.py
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/LayerModel.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/MyPosition.py
+-rw-r--r--   0 root         (0) root         (0)     2947 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/Position.py
+-rw-r--r--   0 root         (0) root         (0)     1401 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/Scope.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/Vector.py
+-rw-r--r--   0 root         (0) root         (0)      877 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.259558 gs2-cdk-1.0.9/src/gs2_cdk/megaField/ref/
+-rw-r--r--   0 root         (0) root         (0)     1467 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/megaField/ref/AreaModelRef.py
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/megaField/ref/LayerModelRef.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/megaField/ref/LayerRef.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/megaField/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/megaField/ref/NodeRef.py
+-rw-r--r--   0 root         (0) root         (0)      763 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/megaField/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.259558 gs2-cdk-1.0.9/src/gs2_cdk/megaField/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/megaField/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.259558 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.259558 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/AreaModel.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/Layer.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/LayerModel.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/MyPosition.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/Position.py
+-rw-r--r--   0 root         (0) root         (0)     1365 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/Scope.py
+-rw-r--r--   0 root         (0) root         (0)     1288 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/Vector.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.259558 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/ref/
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/ref/AreaModelRef.py
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/ref/LayerModelRef.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/ref/LayerRef.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/ref/NodeRef.py
+-rw-r--r--   0 root         (0) root         (0)      763 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.259558 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mega_field/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.259558 gs2-cdk-1.0.9/src/gs2_cdk/mission/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mission/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.263558 gs2-cdk-1.0.9/src/gs2_cdk/mission/model/
+-rw-r--r--   0 root         (0) root         (0)     1932 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mission/model/CounterModel.py
+-rw-r--r--   0 root         (0) root         (0)     4235 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mission/model/CounterScopeModel.py
+-rw-r--r--   0 root         (0) root         (0)     2432 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mission/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     5956 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mission/model/MissionGroupModel.py
+-rw-r--r--   0 root         (0) root         (0)     2766 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mission/model/MissionTaskModel.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mission/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mission/model/ScopedValue.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mission/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.263558 gs2-cdk-1.0.9/src/gs2_cdk/mission/ref/
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mission/ref/CounterModelRef.py
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mission/ref/MissionGroupModelRef.py
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mission/ref/MissionTaskModelRef.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mission/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mission/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.263558 gs2-cdk-1.0.9/src/gs2_cdk/mission/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)     1236 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mission/stamp_sheet/IncreaseCounterByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mission/stamp_sheet/ReceiveByUserId.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/mission/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.263558 gs2-cdk-1.0.9/src/gs2_cdk/money/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/money/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.263558 gs2-cdk-1.0.9/src/gs2_cdk/money/model/
+-rw-r--r--   0 root         (0) root         (0)     4611 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/money/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/money/model/WalletDetail.py
+-rw-r--r--   0 root         (0) root         (0)      880 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/money/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.263558 gs2-cdk-1.0.9/src/gs2_cdk/money/ref/
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/money/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/money/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.263558 gs2-cdk-1.0.9/src/gs2_cdk/money/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)     1253 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/money/stamp_sheet/DepositByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1217 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/money/stamp_sheet/RecordReceipt.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/money/stamp_sheet/WithdrawByUserId.py
+-rw-r--r--   0 root         (0) root         (0)      717 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/money/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.263558 gs2-cdk-1.0.9/src/gs2_cdk/news/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/news/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.263558 gs2-cdk-1.0.9/src/gs2_cdk/news/model/
+-rw-r--r--   0 root         (0) root         (0)     2357 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/news/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)      672 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/news/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.263558 gs2-cdk-1.0.9/src/gs2_cdk/news/ref/
+-rw-r--r--   0 root         (0) root         (0)     1232 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/news/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/news/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.263558 gs2-cdk-1.0.9/src/gs2_cdk/news/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/news/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.263558 gs2-cdk-1.0.9/src/gs2_cdk/quest/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/quest/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.263558 gs2-cdk-1.0.9/src/gs2_cdk/quest/model/
+-rw-r--r--   0 root         (0) root         (0)     1738 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/quest/model/Contents.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/quest/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     4045 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/quest/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/quest/model/QuestGroupModel.py
+-rw-r--r--   0 root         (0) root         (0)     3451 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/quest/model/QuestModel.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/quest/model/Reward.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/quest/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.267558 gs2-cdk-1.0.9/src/gs2_cdk/quest/ref/
+-rw-r--r--   0 root         (0) root         (0)     2279 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/quest/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/quest/ref/QuestGroupModelRef.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/quest/ref/QuestModelRef.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/quest/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.267558 gs2-cdk-1.0.9/src/gs2_cdk/quest/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)     1373 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/quest/stamp_sheet/CreateProgressByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1100 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/quest/stamp_sheet/DeleteProgressByUserId.py
+-rw-r--r--   0 root         (0) root         (0)      702 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/quest/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.267558 gs2-cdk-1.0.9/src/gs2_cdk/ranking/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/ranking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.267558 gs2-cdk-1.0.9/src/gs2_cdk/ranking/model/
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/ranking/model/CalculatedAt.py
+-rw-r--r--   0 root         (0) root         (0)     6245 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/ranking/model/CategoryModel.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/ranking/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     2732 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/ranking/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     1233 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/ranking/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.267558 gs2-cdk-1.0.9/src/gs2_cdk/ranking/ref/
+-rw-r--r--   0 root         (0) root         (0)     1402 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/ranking/ref/CategoryModelRef.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/ranking/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      670 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/ranking/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.267558 gs2-cdk-1.0.9/src/gs2_cdk/ranking/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/ranking/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.267558 gs2-cdk-1.0.9/src/gs2_cdk/realtime/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/realtime/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.267558 gs2-cdk-1.0.9/src/gs2_cdk/realtime/model/
+-rw-r--r--   0 root         (0) root         (0)     3270 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/realtime/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     2809 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/realtime/model/Room.py
+-rw-r--r--   0 root         (0) root         (0)      856 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/realtime/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.267558 gs2-cdk-1.0.9/src/gs2_cdk/realtime/ref/
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/realtime/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)     1365 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/realtime/ref/RoomRef.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/realtime/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.267558 gs2-cdk-1.0.9/src/gs2_cdk/realtime/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/realtime/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.267558 gs2-cdk-1.0.9/src/gs2_cdk/schedule/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/schedule/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.267558 gs2-cdk-1.0.9/src/gs2_cdk/schedule/model/
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/schedule/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     8509 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/schedule/model/Event.py
+-rw-r--r--   0 root         (0) root         (0)     2692 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/schedule/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/schedule/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.267558 gs2-cdk-1.0.9/src/gs2_cdk/schedule/ref/
+-rw-r--r--   0 root         (0) root         (0)     1236 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/schedule/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/schedule/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.267558 gs2-cdk-1.0.9/src/gs2_cdk/schedule/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/schedule/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.267558 gs2-cdk-1.0.9/src/gs2_cdk/script/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/script/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.267558 gs2-cdk-1.0.9/src/gs2_cdk/script/model/
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/script/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     2423 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/script/model/Script.py
+-rw-r--r--   0 root         (0) root         (0)      748 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/script/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.271558 gs2-cdk-1.0.9/src/gs2_cdk/script/ref/
+-rw-r--r--   0 root         (0) root         (0)     1267 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/script/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)     1377 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/script/ref/ScriptRef.py
+-rw-r--r--   0 root         (0) root         (0)      656 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/script/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.271558 gs2-cdk-1.0.9/src/gs2_cdk/script/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/script/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.271558 gs2-cdk-1.0.9/src/gs2_cdk/serialKey/
+-rw-r--r--   0 root         (0) root         (0)      778 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serialKey/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.271558 gs2-cdk-1.0.9/src/gs2_cdk/serialKey/model/
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serialKey/model/CampaignModel.py
+-rw-r--r--   0 root         (0) root         (0)     2031 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serialKey/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     2392 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serialKey/model/IssueJob.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serialKey/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     5467 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serialKey/model/SerialKey.py
+-rw-r--r--   0 root         (0) root         (0)      847 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serialKey/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.271558 gs2-cdk-1.0.9/src/gs2_cdk/serialKey/ref/
+-rw-r--r--   0 root         (0) root         (0)     1492 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serialKey/ref/CampaignModelRef.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serialKey/ref/IssueJobRef.py
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serialKey/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serialKey/ref/SerialKeyRef.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serialKey/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.271558 gs2-cdk-1.0.9/src/gs2_cdk/serialKey/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serialKey/stamp_sheet/UseByUserId.py
+-rw-r--r--   0 root         (0) root         (0)      621 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serialKey/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.271558 gs2-cdk-1.0.9/src/gs2_cdk/serial_key/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serial_key/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.271558 gs2-cdk-1.0.9/src/gs2_cdk/serial_key/model/
+-rw-r--r--   0 root         (0) root         (0)     1546 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serial_key/model/CampaignModel.py
+-rw-r--r--   0 root         (0) root         (0)     2028 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serial_key/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serial_key/model/IssueJob.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serial_key/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     4447 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serial_key/model/SerialKey.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serial_key/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.271558 gs2-cdk-1.0.9/src/gs2_cdk/serial_key/ref/
+-rw-r--r--   0 root         (0) root         (0)     1492 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serial_key/ref/CampaignModelRef.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serial_key/ref/IssueJobRef.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serial_key/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serial_key/ref/SerialKeyRef.py
+-rw-r--r--   0 root         (0) root         (0)      707 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serial_key/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.271558 gs2-cdk-1.0.9/src/gs2_cdk/serial_key/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)     1135 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serial_key/stamp_sheet/UseByUserId.py
+-rw-r--r--   0 root         (0) root         (0)      621 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/serial_key/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.271558 gs2-cdk-1.0.9/src/gs2_cdk/showcase/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/showcase/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.275558 gs2-cdk-1.0.9/src/gs2_cdk/showcase/model/
+-rw-r--r--   0 root         (0) root         (0)     1965 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/showcase/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     3494 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/showcase/model/DisplayItem.py
+-rw-r--r--   0 root         (0) root         (0)     3331 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/showcase/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     2039 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/showcase/model/SalesItem.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/showcase/model/SalesItemGroup.py
+-rw-r--r--   0 root         (0) root         (0)     2064 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/showcase/model/Showcase.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/showcase/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.275558 gs2-cdk-1.0.9/src/gs2_cdk/showcase/ref/
+-rw-r--r--   0 root         (0) root         (0)     1377 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/showcase/ref/DisplayItemRef.py
+-rw-r--r--   0 root         (0) root         (0)     1474 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/showcase/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)      948 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/showcase/ref/SalesItemGroupRef.py
+-rw-r--r--   0 root         (0) root         (0)      943 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/showcase/ref/SalesItemRef.py
+-rw-r--r--   0 root         (0) root         (0)      754 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/showcase/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.275558 gs2-cdk-1.0.9/src/gs2_cdk/showcase/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/showcase/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.275558 gs2-cdk-1.0.9/src/gs2_cdk/stamina/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.275558 gs2-cdk-1.0.9/src/gs2_cdk/stamina/model/
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/model/MaxStaminaTable.py
+-rw-r--r--   0 root         (0) root         (0)     3101 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     1733 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/model/RecoverIntervalTable.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/model/RecoverValueTable.py
+-rw-r--r--   0 root         (0) root         (0)     3476 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/model/StaminaModel.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.275558 gs2-cdk-1.0.9/src/gs2_cdk/stamina/ref/
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/ref/MaxStaminaTableRef.py
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/ref/RecoverIntervalTableRef.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/ref/RecoverValueTableRef.py
+-rw-r--r--   0 root         (0) root         (0)     3687 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/ref/StaminaModelRef.py
+-rw-r--r--   0 root         (0) root         (0)      835 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.275558 gs2-cdk-1.0.9/src/gs2_cdk/stamina/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/stamp_sheet/ConsumeStaminaByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/stamp_sheet/RaiseMaxValueByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/stamp_sheet/RecoverStaminaByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/stamp_sheet/SetMaxValueByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/stamp_sheet/SetRecoverIntervalByUserId.py
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/stamp_sheet/SetRecoverValueByUserId.py
+-rw-r--r--   0 root         (0) root         (0)      940 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/stamina/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.275558 gs2-cdk-1.0.9/src/gs2_cdk/version/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/version/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.279558 gs2-cdk-1.0.9/src/gs2_cdk/version/model/
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/version/model/CurrentMasterData.py
+-rw-r--r--   0 root         (0) root         (0)     3642 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/version/model/Namespace.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/version/model/SignTargetVersion.py
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/version/model/Status.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/version/model/TargetVersion.py
+-rw-r--r--   0 root         (0) root         (0)     1365 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/version/model/Version.py
+-rw-r--r--   0 root         (0) root         (0)     4063 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/version/model/VersionModel.py
+-rw-r--r--   0 root         (0) root         (0)     1431 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/version/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.279558 gs2-cdk-1.0.9/src/gs2_cdk/version/ref/
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/version/ref/NamespaceRef.py
+-rw-r--r--   0 root         (0) root         (0)     1415 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/version/ref/VersionModelRef.py
+-rw-r--r--   0 root         (0) root         (0)      668 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/version/ref/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.279558 gs2-cdk-1.0.9/src/gs2_cdk/version/stamp_sheet/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-01-31 06:26:16.000000 gs2-cdk-1.0.9/src/gs2_cdk/version/stamp_sheet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 06:28:11.227558 gs2-cdk-1.0.9/src/gs2_cdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      368 2023-01-31 06:28:11.000000 gs2-cdk-1.0.9/src/gs2_cdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18738 2023-01-31 06:28:11.000000 gs2-cdk-1.0.9/src/gs2_cdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-31 06:28:11.000000 gs2-cdk-1.0.9/src/gs2_cdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-01-31 06:28:11.000000 gs2-cdk-1.0.9/src/gs2_cdk.egg-info/top_level.txt
```

### Comparing `gs2-cdk-1.0.8/setup.py` & `gs2-cdk-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from setuptools import setup, find_packages
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='gs2-cdk',
-    version='1.0.8',
+    version='1.0.9',
     package_dir={'': 'src'},
     py_modules=["gs2-cdk"],
     packages=find_packages('src'),
     install_requires=[
     ],
     tests_require=[],
     license='Apache License 2.0',
```

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/account/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/account/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/account/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/account/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/account/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/account/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/account/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/account/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/account/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/account/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/account/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/account/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/auth/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/auth/model/AccessToken.py` & `gs2-cdk-1.0.9/src/gs2_cdk/auth/model/AccessToken.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/auth/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/auth/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/auth/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/auth/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/auth/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/auth/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/chat/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/chat/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/chat/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/chat/model/NotificationType.py` & `gs2-cdk-1.0.9/src/gs2_cdk/chat/model/NotificationType.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/chat/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/chat/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/chat/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/chat/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/chat/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/chat/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/chat/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/chat/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/core/func.py` & `gs2-cdk-1.0.9/src/gs2_cdk/core/func.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/core/model.py` & `gs2-cdk-1.0.9/src/gs2_cdk/core/model.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/datastore/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/datastore/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/datastore/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/datastore/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/datastore/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/datastore/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/datastore/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/datastore/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/datastore/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/datastore/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/datastore/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/dictionary/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/dictionary/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/dictionary/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/dictionary/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/dictionary/model/EntryModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/dictionary/model/EntryModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/dictionary/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/dictionary/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/dictionary/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/dictionary/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/dictionary/ref/EntryModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/dictionary/ref/EntryModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/dictionary/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/dictionary/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/dictionary/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/dictionary/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/dictionary/stamp_sheet/AddEntriesByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/dictionary/stamp_sheet/AddEntriesByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/dictionary/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/dictionary/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/distributor/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/distributor/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/distributor/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/distributor/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/distributor/model/DistributeResource.py` & `gs2-cdk-1.0.9/src/gs2_cdk/distributor/model/DistributeResource.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/distributor/model/DistributorModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/distributor/model/DistributorModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/distributor/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/distributor/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/distributor/model/StampSheetResult.py` & `gs2-cdk-1.0.9/src/gs2_cdk/distributor/model/StampSheetResult.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/distributor/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/distributor/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/distributor/ref/DistributorModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/distributor/ref/DistributorModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/distributor/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/distributor/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/distributor/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/distributor/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/distributor/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/distributor/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/enhance/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/enhance/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/enhance/model/BonusRate.py` & `gs2-cdk-1.0.9/src/gs2_cdk/enhance/model/BonusRate.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/enhance/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/enhance/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/enhance/model/Material.py` & `gs2-cdk-1.0.9/src/gs2_cdk/enhance/model/Material.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/enhance/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/enhance/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/enhance/model/RateModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/enhance/model/RateModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/enhance/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/enhance/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/enhance/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/enhance/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/enhance/ref/RateModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/enhance/ref/RateModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/enhance/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/enhance/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/enhance/stamp_sheet/CreateProgressByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/enhance/stamp_sheet/CreateProgressByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/enhance/stamp_sheet/DeleteProgressByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/enhance/stamp_sheet/DeleteProgressByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/enhance/stamp_sheet/DirectEnhanceByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/enhance/stamp_sheet/DirectEnhanceByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/enhance/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/enhance/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/exchange/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/exchange/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/exchange/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/exchange/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/exchange/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/exchange/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/exchange/model/RateModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/exchange/model/RateModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/exchange/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/exchange/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/exchange/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/exchange/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/exchange/ref/RateModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/exchange/ref/RateModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/exchange/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/exchange/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/exchange/stamp_sheet/CreateAwaitByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/exchange/stamp_sheet/CreateAwaitByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/exchange/stamp_sheet/DeleteAwaitByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/exchange/stamp_sheet/DeleteAwaitByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/exchange/stamp_sheet/ExchangeByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/exchange/stamp_sheet/ExchangeByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/exchange/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/exchange/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/experience/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/experience/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/experience/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/experience/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/experience/model/ExperienceModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/experience/model/ExperienceModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/experience/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/experience/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/experience/model/Threshold.py` & `gs2-cdk-1.0.9/src/gs2_cdk/experience/model/Threshold.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/experience/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/experience/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/experience/ref/ExperienceModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/experience/ref/ExperienceModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/experience/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/experience/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/experience/ref/ThresholdRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/experience/ref/ThresholdRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/experience/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/experience/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/experience/stamp_sheet/AddExperienceByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/experience/stamp_sheet/AddExperienceByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/experience/stamp_sheet/AddRankCapByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/experience/stamp_sheet/AddRankCapByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/experience/stamp_sheet/SetRankCapByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/experience/stamp_sheet/SetRankCapByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/experience/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/experience/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/formation/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/formation/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/formation/model/AcquireActionConfig.py` & `gs2-cdk-1.0.9/src/gs2_cdk/formation/model/AcquireActionConfig.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/formation/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/formation/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/formation/model/FormModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/formation/model/FormModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/formation/model/MoldModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/formation/model/MoldModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/formation/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/formation/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/formation/model/Slot.py` & `gs2-cdk-1.0.9/src/gs2_cdk/formation/model/Slot.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/formation/model/SlotModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/formation/model/SlotModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/formation/model/SlotWithSignature.py` & `gs2-cdk-1.0.9/src/gs2_cdk/formation/model/SlotWithSignature.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/formation/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/formation/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/formation/ref/FormModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/formation/ref/FormModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/formation/ref/MoldModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/formation/ref/MoldModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/formation/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/formation/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/formation/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/formation/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/formation/stamp_sheet/AcquireActionsToFormProperties.py` & `gs2-cdk-1.0.9/src/gs2_cdk/formation/stamp_sheet/AcquireActionsToFormProperties.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/formation/stamp_sheet/AcquireActionsToPropertyFormProperties.py` & `gs2-cdk-1.0.9/src/gs2_cdk/formation/stamp_sheet/AcquireActionsToPropertyFormProperties.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/formation/stamp_sheet/AddMoldCapacityByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/formation/stamp_sheet/AddMoldCapacityByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/formation/stamp_sheet/SetMoldCapacityByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/formation/stamp_sheet/SetMoldCapacityByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/formation/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/formation/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/friend/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/friend/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/friend/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/friend/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/friend/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/friend/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/friend/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/friend/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/friend/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/friend/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/friend/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/friend/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/gateway/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/gateway/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/gateway/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/gateway/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/gateway/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/gateway/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/gateway/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/gateway/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/gateway/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/gateway/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/gateway/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/identifier/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/identifier/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/identifier/model/AttachSecurityPolicy.py` & `gs2-cdk-1.0.9/src/gs2_cdk/identifier/model/AttachSecurityPolicy.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/identifier/model/Identifier.py` & `gs2-cdk-1.0.9/src/gs2_cdk/identifier/model/Identifier.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/identifier/model/Password.py` & `gs2-cdk-1.0.9/src/gs2_cdk/identifier/model/Password.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/identifier/model/Policy.py` & `gs2-cdk-1.0.9/src/gs2_cdk/identifier/model/Policy.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/identifier/model/ProjectToken.py` & `gs2-cdk-1.0.9/src/gs2_cdk/identifier/model/ProjectToken.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/identifier/model/SecurityPolicy.py` & `gs2-cdk-1.0.9/src/gs2_cdk/identifier/model/SecurityPolicy.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/identifier/model/Statement.py` & `gs2-cdk-1.0.9/src/gs2_cdk/identifier/model/Statement.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/identifier/model/User.py` & `gs2-cdk-1.0.9/src/gs2_cdk/identifier/model/User.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/identifier/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/identifier/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/identifier/ref/AttachSecurityPolicyRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/identifier/ref/AttachSecurityPolicyRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/identifier/ref/IdentifierRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/identifier/ref/IdentifierRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/identifier/ref/PasswordRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/identifier/ref/PasswordRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/identifier/ref/SecurityPolicyRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/identifier/ref/SecurityPolicyRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/identifier/ref/UserRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/identifier/ref/UserRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/identifier/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/identifier/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/identifier/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/identifier/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inbox/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inbox/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inbox/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inbox/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inbox/model/GlobalMessage.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inbox/model/GlobalMessage.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inbox/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inbox/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inbox/model/TimeSpan.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inbox/model/TimeSpan.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inbox/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inbox/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inbox/ref/GlobalMessageRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inbox/ref/GlobalMessageRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inbox/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inbox/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inbox/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inbox/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inbox/stamp_sheet/OpenMessageByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inbox/stamp_sheet/OpenMessageByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inbox/stamp_sheet/SendMessageByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inbox/stamp_sheet/SendMessageByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inbox/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inbox/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inventory/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inventory/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inventory/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inventory/model/InventoryModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inventory/model/InventoryModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inventory/model/ItemModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inventory/model/ItemModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inventory/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inventory/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inventory/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inventory/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inventory/ref/InventoryModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inventory/ref/InventoryModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inventory/ref/ItemModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inventory/ref/ItemModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inventory/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inventory/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inventory/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inventory/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inventory/stamp_sheet/AcquireItemSetByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inventory/stamp_sheet/AcquireItemSetByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inventory/stamp_sheet/AddCapacityByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inventory/stamp_sheet/AddCapacityByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inventory/stamp_sheet/AddReferenceOfByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inventory/stamp_sheet/AddReferenceOfByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inventory/stamp_sheet/ConsumeItemSetByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inventory/stamp_sheet/ConsumeItemSetByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inventory/stamp_sheet/DeleteReferenceOfByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inventory/stamp_sheet/DeleteReferenceOfByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inventory/stamp_sheet/SetCapacityByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inventory/stamp_sheet/SetCapacityByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inventory/stamp_sheet/VerifyReferenceOfByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inventory/stamp_sheet/VerifyReferenceOfByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/inventory/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/inventory/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/job_queue/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/job_queue/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/job_queue/model/JobEntry.py` & `gs2-cdk-1.0.9/src/gs2_cdk/job_queue/model/JobEntry.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/job_queue/model/JobResultBody.py` & `gs2-cdk-1.0.9/src/gs2_cdk/job_queue/model/JobResultBody.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/job_queue/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/job_queue/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/job_queue/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/job_queue/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/job_queue/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/job_queue/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/job_queue/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/job_queue/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/job_queue/stamp_sheet/PushByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/job_queue/stamp_sheet/PushByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/job_queue/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/job_queue/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/key/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/key/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/key/model/GitHubApiKey.py` & `gs2-cdk-1.0.9/src/gs2_cdk/key/model/GitHubApiKey.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/key/model/Key.py` & `gs2-cdk-1.0.9/src/gs2_cdk/key/model/Key.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/key/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/key/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/key/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/key/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/key/ref/GitHubApiKeyRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/key/ref/GitHubApiKeyRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/key/ref/KeyRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/key/ref/KeyRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/key/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/key/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/key/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/key/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/key/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/key/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/limit/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/limit/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/limit/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/limit/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/limit/model/LimitModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/limit/model/LimitModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/limit/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/limit/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/limit/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/limit/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/limit/ref/LimitModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/limit/ref/LimitModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/limit/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/limit/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/limit/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/limit/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/limit/stamp_sheet/CountUpByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/limit/stamp_sheet/CountUpByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/limit/stamp_sheet/DeleteCounterByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/limit/stamp_sheet/DeleteCounterByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/limit/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/limit/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lock/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lock/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lock/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lock/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lock/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lock/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lock/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lock/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lock/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lock/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lock/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lock/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/log/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/log/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/log/model/AccessLog.py` & `gs2-cdk-1.0.9/src/gs2_cdk/log/model/AccessLog.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/log/model/AccessLogCount.py` & `gs2-cdk-1.0.9/src/gs2_cdk/log/model/AccessLogCount.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/log/model/ExecuteStampSheetLog.py` & `gs2-cdk-1.0.9/src/gs2_cdk/log/model/ExecuteStampSheetLog.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/log/model/ExecuteStampSheetLogCount.py` & `gs2-cdk-1.0.9/src/gs2_cdk/log/model/ExecuteStampSheetLogCount.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/log/model/ExecuteStampTaskLog.py` & `gs2-cdk-1.0.9/src/gs2_cdk/log/model/ExecuteStampTaskLog.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/log/model/ExecuteStampTaskLogCount.py` & `gs2-cdk-1.0.9/src/gs2_cdk/log/model/ExecuteStampTaskLogCount.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/log/model/IssueStampSheetLog.py` & `gs2-cdk-1.0.9/src/gs2_cdk/log/model/IssueStampSheetLog.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/log/model/IssueStampSheetLogCount.py` & `gs2-cdk-1.0.9/src/gs2_cdk/log/model/IssueStampSheetLogCount.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/log/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/log/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/log/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/log/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/log/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/log/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/log/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/log/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/log/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/log/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lottery/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lottery/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lottery/model/BoxItem.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lottery/model/BoxItem.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lottery/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lottery/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lottery/model/DrawnPrize.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lottery/model/DrawnPrize.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lottery/model/LotteryModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lottery/model/LotteryModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lottery/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lottery/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lottery/model/Prize.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lottery/model/Prize.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lottery/model/PrizeLimit.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lottery/model/PrizeLimit.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lottery/model/PrizeTable.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lottery/model/PrizeTable.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lottery/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lottery/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lottery/ref/LotteryModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lottery/ref/LotteryModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lottery/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lottery/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lottery/ref/PrizeLimitRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lottery/ref/PrizeLimitRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lottery/ref/PrizeTableRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lottery/ref/PrizeTableRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lottery/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lottery/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lottery/stamp_sheet/DrawByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lottery/stamp_sheet/DrawByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/lottery/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/lottery/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/Attribute.py` & `gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/Attribute.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/AttributeRange.py` & `gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/AttributeRange.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/CapacityOfRole.py` & `gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/CapacityOfRole.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/GameResult.py` & `gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/GameResult.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/Player.py` & `gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/Player.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/RatingModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/RatingModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/SignedBallot.py` & `gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/SignedBallot.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/TimeSpan.py` & `gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/TimeSpan.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/ref/RatingModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/ref/RatingModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/matchmaking/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/matchmaking/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/megaField/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/megaField/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/AreaModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/AreaModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/Layer.py` & `gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/Layer.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/LayerModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/LayerModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/MyPosition.py` & `gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/MyPosition.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/Position.py` & `gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/Position.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/Scope.py` & `gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/Scope.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/Vector.py` & `gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/Vector.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/megaField/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/megaField/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/megaField/ref/AreaModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/megaField/ref/AreaModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/megaField/ref/LayerModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/megaField/ref/LayerModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/megaField/ref/LayerRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/megaField/ref/LayerRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/megaField/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/megaField/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/megaField/ref/NodeRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/megaField/ref/NodeRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/megaField/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/megaField/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/megaField/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/megaField/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mega_field/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mega_field/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/AreaModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/AreaModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/Layer.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/Layer.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/LayerModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/LayerModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/MyPosition.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/MyPosition.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/Position.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/Position.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/Scope.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/Scope.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/Vector.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/Vector.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mega_field/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mega_field/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mega_field/ref/AreaModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mega_field/ref/NamespaceRef.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,28 +11,36 @@
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from __future__ import annotations
 from typing import *
 
 from ...core.func import GetAttr, Join
-from .LayerModelRef import LayerModelRef
+from .AreaModelRef import AreaModelRef
+from .NodeRef import NodeRef
+from .LayerRef import LayerRef
 
 
-class AreaModelRef:
+class NamespaceRef:
     namespace_name: str
-    area_model_name: str
 
     def __init__(
         self,
         namespace_name: str,
-        area_model_name: str,
     ):
         self.namespace_name = namespace_name
-        self.area_model_name = area_model_name
+
+    def area_model(
+        self,
+        area_model_name: str,
+    ) -> AreaModelRef:
+        return AreaModelRef(
+            self.namespace_name,
+            area_model_name,
+        )
 
     def grn(
         self,
     ) -> str:
         return Join(
             ":",
             [
@@ -42,13 +50,10 @@
                 ).str(
                 ),
                 GetAttr.owner_id(
                 ).str(
                 ),
                 "megaField",
                 self.namespace_name,
-                "model",
-                "area",
-                self.area_model_name,
             ],
         ).str(
         )
```

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mega_field/ref/LayerModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mega_field/ref/LayerModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mega_field/ref/LayerRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mega_field/ref/LayerRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mega_field/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/ranking/ref/NamespaceRef.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,35 +11,33 @@
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from __future__ import annotations
 from typing import *
 
 from ...core.func import GetAttr, Join
-from .AreaModelRef import AreaModelRef
-from .NodeRef import NodeRef
-from .LayerRef import LayerRef
+from .CategoryModelRef import CategoryModelRef
 
 
 class NamespaceRef:
     namespace_name: str
 
     def __init__(
         self,
         namespace_name: str,
     ):
         self.namespace_name = namespace_name
 
-    def area_model(
+    def category_model(
         self,
-        area_model_name: str,
-    ) -> AreaModelRef:
-        return AreaModelRef(
+        category_name: str,
+    ) -> CategoryModelRef:
+        return CategoryModelRef(
             self.namespace_name,
-            area_model_name,
+            category_name,
         )
 
     def grn(
         self,
     ) -> str:
         return Join(
             ":",
@@ -48,12 +46,12 @@
                 "gs2",
                 GetAttr.region(
                 ).str(
                 ),
                 GetAttr.owner_id(
                 ).str(
                 ),
-                "megaField",
+                "ranking",
                 self.namespace_name,
             ],
         ).str(
         )
```

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mega_field/ref/NodeRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mega_field/ref/NodeRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mega_field/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mega_field/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mega_field/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mega_field/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mission/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mission/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mission/model/CounterModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mission/model/CounterModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mission/model/CounterScopeModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mission/model/CounterScopeModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mission/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mission/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mission/model/MissionGroupModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mission/model/MissionGroupModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mission/model/MissionTaskModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mission/model/MissionTaskModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mission/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mission/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mission/model/ScopedValue.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mission/model/ScopedValue.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mission/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mission/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mission/ref/CounterModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mission/ref/CounterModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mission/ref/MissionGroupModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mission/ref/MissionGroupModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mission/ref/MissionTaskModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mission/ref/MissionTaskModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mission/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mission/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mission/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mission/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mission/stamp_sheet/IncreaseCounterByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mission/stamp_sheet/IncreaseCounterByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mission/stamp_sheet/ReceiveByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mission/stamp_sheet/ReceiveByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/mission/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mission/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/money/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/money/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/money/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/money/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/money/model/WalletDetail.py` & `gs2-cdk-1.0.9/src/gs2_cdk/money/model/WalletDetail.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/money/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/money/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/money/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/money/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/money/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/money/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/money/stamp_sheet/DepositByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/money/stamp_sheet/DepositByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/money/stamp_sheet/RecordReceipt.py` & `gs2-cdk-1.0.9/src/gs2_cdk/money/stamp_sheet/RecordReceipt.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/money/stamp_sheet/WithdrawByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/money/stamp_sheet/WithdrawByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/money/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/money/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/news/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/news/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/news/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/news/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/news/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/news/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/news/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/news/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/news/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/news/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/news/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/news/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/quest/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/quest/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/quest/model/Contents.py` & `gs2-cdk-1.0.9/src/gs2_cdk/quest/model/Contents.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/quest/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/quest/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/quest/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/quest/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/quest/model/QuestGroupModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/quest/model/QuestGroupModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/quest/model/QuestModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/quest/model/QuestModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/quest/model/Reward.py` & `gs2-cdk-1.0.9/src/gs2_cdk/quest/model/Reward.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/quest/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/quest/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/quest/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/quest/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/quest/ref/QuestGroupModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/quest/ref/QuestGroupModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/quest/ref/QuestModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/quest/ref/QuestModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/quest/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/quest/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/quest/stamp_sheet/CreateProgressByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/quest/stamp_sheet/CreateProgressByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/quest/stamp_sheet/DeleteProgressByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/quest/stamp_sheet/DeleteProgressByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/quest/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/quest/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/ranking/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/ranking/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/ranking/model/CalculatedAt.py` & `gs2-cdk-1.0.9/src/gs2_cdk/ranking/model/CalculatedAt.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/ranking/model/CategoryModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/ranking/model/CategoryModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/ranking/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/ranking/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/ranking/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/ranking/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/ranking/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/ranking/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/ranking/ref/CategoryModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/ranking/ref/CategoryModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/ranking/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/script/ref/NamespaceRef.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,47 +11,38 @@
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from __future__ import annotations
 from typing import *
 
 from ...core.func import GetAttr, Join
-from .CategoryModelRef import CategoryModelRef
+from .ScriptRef import ScriptRef
 
 
 class NamespaceRef:
     namespace_name: str
 
     def __init__(
         self,
         namespace_name: str,
     ):
         self.namespace_name = namespace_name
 
-    def category_model(
-        self,
-        category_name: str,
-    ) -> CategoryModelRef:
-        return CategoryModelRef(
-            self.namespace_name,
-            category_name,
-        )
-
     def grn(
         self,
     ) -> str:
         return Join(
             ":",
             [
                 "grn",
                 "gs2",
                 GetAttr.region(
                 ).str(
                 ),
                 GetAttr.owner_id(
                 ).str(
                 ),
-                "ranking",
+                "script",
                 self.namespace_name,
             ],
         ).str(
         )
```

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/ranking/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/ranking/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/ranking/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/ranking/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/realtime/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/realtime/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/realtime/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/realtime/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/realtime/model/Room.py` & `gs2-cdk-1.0.9/src/gs2_cdk/realtime/model/Room.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/realtime/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/realtime/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/realtime/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/realtime/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/realtime/ref/RoomRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/realtime/ref/RoomRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/realtime/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/realtime/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/realtime/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/realtime/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/schedule/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/schedule/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/schedule/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/schedule/model/Event.py` & `gs2-cdk-1.0.9/src/gs2_cdk/schedule/model/Event.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/schedule/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/schedule/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/schedule/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/schedule/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/schedule/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/schedule/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/schedule/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/schedule/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/schedule/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/schedule/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/script/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/script/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/script/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/script/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/script/model/Script.py` & `gs2-cdk-1.0.9/src/gs2_cdk/script/model/Script.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/script/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/script/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/script/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/version/ref/NamespaceRef.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,38 +11,47 @@
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from __future__ import annotations
 from typing import *
 
 from ...core.func import GetAttr, Join
-from .ScriptRef import ScriptRef
+from .VersionModelRef import VersionModelRef
 
 
 class NamespaceRef:
     namespace_name: str
 
     def __init__(
         self,
         namespace_name: str,
     ):
         self.namespace_name = namespace_name
 
+    def version_model(
+        self,
+        version_name: str,
+    ) -> VersionModelRef:
+        return VersionModelRef(
+            self.namespace_name,
+            version_name,
+        )
+
     def grn(
         self,
     ) -> str:
         return Join(
             ":",
             [
                 "grn",
                 "gs2",
                 GetAttr.region(
                 ).str(
                 ),
                 GetAttr.owner_id(
                 ).str(
                 ),
-                "script",
+                "version",
                 self.namespace_name,
             ],
         ).str(
         )
```

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/script/ref/ScriptRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/script/ref/ScriptRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/script/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/script/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/script/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/script/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serialKey/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serialKey/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serialKey/model/CampaignModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serialKey/model/CampaignModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serialKey/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serialKey/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serialKey/model/IssueJob.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serialKey/model/IssueJob.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serialKey/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serialKey/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serialKey/model/SerialKey.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serialKey/model/SerialKey.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serialKey/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serialKey/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serialKey/ref/CampaignModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serialKey/ref/CampaignModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serialKey/ref/IssueJobRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serialKey/ref/IssueJobRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serialKey/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serialKey/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serialKey/ref/SerialKeyRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serialKey/ref/SerialKeyRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serialKey/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serialKey/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serialKey/stamp_sheet/UseByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serialKey/stamp_sheet/UseByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serialKey/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serialKey/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serial_key/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serial_key/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serial_key/model/CampaignModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serial_key/model/CampaignModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serial_key/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serial_key/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serial_key/model/IssueJob.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serial_key/model/IssueJob.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serial_key/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serial_key/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serial_key/model/SerialKey.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serial_key/model/SerialKey.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serial_key/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/version/model/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from .Namespace import Namespace
 from .options.NamespaceOptions import NamespaceOptions
-from .IssueJob import IssueJob
-from .options.IssueJobOptions import IssueJobOptions
-from .enum.IssueJobStatus import IssueJobStatus
-from .SerialKey import SerialKey
-from .options.SerialKeyOptions import SerialKeyOptions
-from .enum.SerialKeyStatus import SerialKeyStatus
-from .options.SerialKeyStatusIsActiveOptions import SerialKeyStatusIsActiveOptions
-from .options.SerialKeyStatusIsUsedOptions import SerialKeyStatusIsUsedOptions
-from .options.SerialKeyStatusIsInactiveOptions import SerialKeyStatusIsInactiveOptions
-from .CampaignModel import CampaignModel
-from .options.CampaignModelOptions import CampaignModelOptions
+from .Version import Version
+from .options.VersionOptions import VersionOptions
+from .VersionModel import VersionModel
+from .options.VersionModelOptions import VersionModelOptions
+from .enum.VersionModelScope import VersionModelScope
+from .options.VersionModelScopeIsPassiveOptions import VersionModelScopeIsPassiveOptions
+from .options.VersionModelScopeIsActiveOptions import VersionModelScopeIsActiveOptions
+from .Status import Status
+from .options.StatusOptions import StatusOptions
+from .TargetVersion import TargetVersion
+from .options.TargetVersionOptions import TargetVersionOptions
+from .SignTargetVersion import SignTargetVersion
+from .options.SignTargetVersionOptions import SignTargetVersionOptions
 from .CurrentMasterData import CurrentMasterData
```

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serial_key/ref/CampaignModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serial_key/ref/CampaignModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serial_key/ref/IssueJobRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serial_key/ref/IssueJobRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serial_key/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serial_key/ref/NamespaceRef.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from __future__ import annotations
 from typing import *
 
 from ...core.func import GetAttr, Join
 from .CampaignModelRef import CampaignModelRef
-from .SerialKeyRef import SerialKeyRef
 from ..stamp_sheet.UseByUserId import UseByUserId
 
 
 class NamespaceRef:
     namespace_name: str
 
     def __init__(
```

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serial_key/ref/SerialKeyRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serial_key/ref/SerialKeyRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serial_key/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serial_key/ref/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from .NamespaceRef import NamespaceRef
 from .IssueJobRef import IssueJobRef
-from .SerialKeyRef import SerialKeyRef
 from .CampaignModelRef import CampaignModelRef
```

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serial_key/stamp_sheet/UseByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serial_key/stamp_sheet/UseByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/serial_key/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/serial_key/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/showcase/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/showcase/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/showcase/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/showcase/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/showcase/model/DisplayItem.py` & `gs2-cdk-1.0.9/src/gs2_cdk/showcase/model/DisplayItem.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/showcase/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/showcase/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/showcase/model/SalesItem.py` & `gs2-cdk-1.0.9/src/gs2_cdk/showcase/model/SalesItem.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/showcase/model/SalesItemGroup.py` & `gs2-cdk-1.0.9/src/gs2_cdk/showcase/model/SalesItemGroup.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/showcase/model/Showcase.py` & `gs2-cdk-1.0.9/src/gs2_cdk/showcase/model/Showcase.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/showcase/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/showcase/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/showcase/ref/DisplayItemRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/showcase/ref/DisplayItemRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/showcase/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/showcase/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/showcase/ref/SalesItemGroupRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/showcase/ref/SalesItemGroupRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/showcase/ref/SalesItemRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/showcase/ref/SalesItemRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/showcase/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/showcase/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/showcase/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/showcase/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/model/MaxStaminaTable.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/model/MaxStaminaTable.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/model/RecoverIntervalTable.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/model/RecoverIntervalTable.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/model/RecoverValueTable.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/model/RecoverValueTable.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/model/StaminaModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/model/StaminaModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/model/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/ref/MaxStaminaTableRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/ref/MaxStaminaTableRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/ref/NamespaceRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/ref/RecoverIntervalTableRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/ref/RecoverIntervalTableRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/ref/RecoverValueTableRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/ref/RecoverValueTableRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/ref/StaminaModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/ref/StaminaModelRef.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/stamp_sheet/ConsumeStaminaByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/stamp_sheet/ConsumeStaminaByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/stamp_sheet/RaiseMaxValueByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/stamp_sheet/RaiseMaxValueByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/stamp_sheet/RecoverStaminaByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/stamp_sheet/RecoverStaminaByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/stamp_sheet/SetMaxValueByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/stamp_sheet/SetMaxValueByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/stamp_sheet/SetRecoverIntervalByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/stamp_sheet/SetRecoverIntervalByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/stamp_sheet/SetRecoverValueByUserId.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/stamp_sheet/SetRecoverValueByUserId.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/stamina/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/stamina/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/version/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/version/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/version/model/CurrentMasterData.py` & `gs2-cdk-1.0.9/src/gs2_cdk/version/model/CurrentMasterData.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/version/model/Namespace.py` & `gs2-cdk-1.0.9/src/gs2_cdk/version/model/Namespace.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/version/model/SignTargetVersion.py` & `gs2-cdk-1.0.9/src/gs2_cdk/version/model/SignTargetVersion.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/version/model/Status.py` & `gs2-cdk-1.0.9/src/gs2_cdk/version/model/Status.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/version/model/TargetVersion.py` & `gs2-cdk-1.0.9/src/gs2_cdk/version/model/TargetVersion.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/version/model/Version.py` & `gs2-cdk-1.0.9/src/gs2_cdk/version/model/Version.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/version/model/VersionModel.py` & `gs2-cdk-1.0.9/src/gs2_cdk/version/model/VersionModel.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/version/ref/NamespaceRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/version/ref/VersionModelRef.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,34 +11,27 @@
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from __future__ import annotations
 from typing import *
 
 from ...core.func import GetAttr, Join
-from .VersionModelRef import VersionModelRef
 
 
-class NamespaceRef:
+class VersionModelRef:
     namespace_name: str
+    version_name: str
 
     def __init__(
         self,
         namespace_name: str,
+        version_name: str,
     ):
         self.namespace_name = namespace_name
-
-    def version_model(
-        self,
-        version_name: str,
-    ) -> VersionModelRef:
-        return VersionModelRef(
-            self.namespace_name,
-            version_name,
-        )
+        self.version_name = version_name
 
     def grn(
         self,
     ) -> str:
         return Join(
             ":",
             [
@@ -48,10 +41,13 @@
                 ).str(
                 ),
                 GetAttr.owner_id(
                 ).str(
                 ),
                 "version",
                 self.namespace_name,
+                "model",
+                "version",
+                self.version_name,
             ],
         ).str(
         )
```

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/version/ref/VersionModelRef.py` & `gs2-cdk-1.0.9/src/gs2_cdk/mega_field/ref/AreaModelRef.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,27 +11,38 @@
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from __future__ import annotations
 from typing import *
 
 from ...core.func import GetAttr, Join
+from .LayerModelRef import LayerModelRef
 
 
-class VersionModelRef:
+class AreaModelRef:
     namespace_name: str
-    version_name: str
+    area_model_name: str
 
     def __init__(
         self,
         namespace_name: str,
-        version_name: str,
+        area_model_name: str,
     ):
         self.namespace_name = namespace_name
-        self.version_name = version_name
+        self.area_model_name = area_model_name
+
+    def layer_model(
+        self,
+        layer_model_name: str,
+    ) -> LayerModelRef:
+        return LayerModelRef(
+            self.namespace_name,
+            self.area_model_name,
+            layer_model_name,
+        )
 
     def grn(
         self,
     ) -> str:
         return Join(
             ":",
             [
@@ -39,15 +50,15 @@
                 "gs2",
                 GetAttr.region(
                 ).str(
                 ),
                 GetAttr.owner_id(
                 ).str(
                 ),
-                "version",
+                "megaField",
                 self.namespace_name,
                 "model",
-                "version",
-                self.version_name,
+                "area",
+                self.area_model_name,
             ],
         ).str(
         )
```

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/version/ref/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/version/ref/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk/version/stamp_sheet/__init__.py` & `gs2-cdk-1.0.9/src/gs2_cdk/version/stamp_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-cdk-1.0.8/src/gs2_cdk.egg-info/SOURCES.txt` & `gs2-cdk-1.0.9/src/gs2_cdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

