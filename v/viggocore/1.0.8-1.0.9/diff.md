# Comparing `tmp/viggocore-1.0.8.tar.gz` & `tmp/viggocore-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viggocore-1.0.8.tar", last modified: Fri Mar  3 18:25:38 2023, max compression
+gzip compressed data, was "viggocore-1.0.9.tar", last modified: Tue Mar  7 12:42:31 2023, max compression
```

## Comparing `viggocore-1.0.8.tar` & `viggocore-1.0.9.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.380940 viggocore-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-03 18:25:17.000000 viggocore-1.0.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-03 18:25:17.000000 viggocore-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-03 18:25:38.380940 viggocore-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-03 18:25:17.000000 viggocore-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 18:25:38.380940 viggocore-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-03-03 18:25:17.000000 viggocore-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.372940 viggocore-1.0.8/viggocore/
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.372940 viggocore-1.0.8/viggocore/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/bootstrap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.372940 viggocore-1.0.8/viggocore/bootstrap/default/
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/bootstrap/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/bootstrap/default/application.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/bootstrap/default/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/bootstrap/default/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/bootstrap/default/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/bootstrap/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/bootstrap/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/celery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.372940 viggocore-1.0.8/viggocore/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/common/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/common/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/common/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/common/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/common/operation_after_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.376940 viggocore-1.0.8/viggocore/common/subsystem/
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/common/subsystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/common/subsystem/apihandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/common/subsystem/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/common/subsystem/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/common/subsystem/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/common/subsystem/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/common/subsystem/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/common/subsystem/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/common/subsystem/router.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/common/subsystem/transaction_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.376940 viggocore-1.0.8/viggocore/subsystem/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.376940 viggocore-1.0.8/viggocore/subsystem/application/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/application/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/application/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/application/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/application/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.376940 viggocore-1.0.8/viggocore/subsystem/capability/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/capability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/capability/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/capability/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.376940 viggocore-1.0.8/viggocore/subsystem/domain/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/domain/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/domain/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/domain/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/domain/router.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/domain/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.376940 viggocore-1.0.8/viggocore/subsystem/domain_sequence/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/domain_sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/domain_sequence/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/domain_sequence/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/domain_sequence/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/domain_sequence/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/domain_sequence/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.376940 viggocore-1.0.8/viggocore/subsystem/file/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/file/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/file/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/file/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.376940 viggocore-1.0.8/viggocore/subsystem/file_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/file_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/file_sync/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.376940 viggocore-1.0.8/viggocore/subsystem/grant/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/grant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/grant/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.376940 viggocore-1.0.8/viggocore/subsystem/image/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/image/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/image/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/image/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/image/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/image/router.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/image/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.376940 viggocore-1.0.8/viggocore/subsystem/notification/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/notification/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.376940 viggocore-1.0.8/viggocore/subsystem/policy/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/policy/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.376940 viggocore-1.0.8/viggocore/subsystem/registration/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/registration/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/registration/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.380940 viggocore-1.0.8/viggocore/subsystem/role/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/role/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/role/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/role/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/role/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/role/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.380940 viggocore-1.0.8/viggocore/subsystem/route/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/route/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/route/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.380940 viggocore-1.0.8/viggocore/subsystem/tag/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/tag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/tag/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/tag/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/tag/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/tag/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.380940 viggocore-1.0.8/viggocore/subsystem/timeline_event/
--rwxr-xr-x   0 runner    (1001) docker     (123)      312 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/timeline_event/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1696 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/timeline_event/controller.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2767 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/timeline_event/manager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2798 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/timeline_event/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.380940 viggocore-1.0.8/viggocore/subsystem/token/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/token/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/token/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/token/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.380940 viggocore-1.0.8/viggocore/subsystem/user/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/user/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/user/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/user/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/user/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/subsystem/user/router.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.380940 viggocore-1.0.8/viggocore/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.380940 viggocore-1.0.8/viggocore/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/tests/functional/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/tests/functional/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/tests/functional/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/tests/functional/test_grants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/tests/functional/test_grants_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/tests/functional/test_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/tests/functional/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-03 18:25:17.000000 viggocore-1.0.8/viggocore/tests/functional/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:25:38.372940 viggocore-1.0.8/viggocore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-03 18:25:38.000000 viggocore-1.0.8/viggocore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-03-03 18:25:38.000000 viggocore-1.0.8/viggocore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 18:25:38.000000 viggocore-1.0.8/viggocore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-03 18:25:38.000000 viggocore-1.0.8/viggocore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-03 18:25:38.000000 viggocore-1.0.8/viggocore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.703433 viggocore-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-07 12:42:06.000000 viggocore-1.0.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-07 12:42:06.000000 viggocore-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-07 12:42:31.703433 viggocore-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-07 12:42:06.000000 viggocore-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 12:42:31.703433 viggocore-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-03-07 12:42:06.000000 viggocore-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.691433 viggocore-1.0.9/viggocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.691433 viggocore-1.0.9/viggocore/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/bootstrap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.695433 viggocore-1.0.9/viggocore/bootstrap/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/bootstrap/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/bootstrap/default/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/bootstrap/default/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/bootstrap/default/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/bootstrap/default/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/bootstrap/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/bootstrap/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/celery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.695433 viggocore-1.0.9/viggocore/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/common/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/common/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/common/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/common/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/common/operation_after_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.695433 viggocore-1.0.9/viggocore/common/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/common/subsystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/common/subsystem/apihandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/common/subsystem/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/common/subsystem/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/common/subsystem/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/common/subsystem/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/common/subsystem/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/common/subsystem/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/common/subsystem/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/common/subsystem/transaction_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.695433 viggocore-1.0.9/viggocore/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.695433 viggocore-1.0.9/viggocore/subsystem/application/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/application/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/application/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/application/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/application/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.695433 viggocore-1.0.9/viggocore/subsystem/capability/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/capability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/capability/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/capability/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.695433 viggocore-1.0.9/viggocore/subsystem/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/domain/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/domain/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/domain/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/domain/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/domain/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.699433 viggocore-1.0.9/viggocore/subsystem/domain_sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/domain_sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/domain_sequence/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/domain_sequence/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/domain_sequence/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/domain_sequence/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/domain_sequence/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.699433 viggocore-1.0.9/viggocore/subsystem/file/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/file/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/file/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/file/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.699433 viggocore-1.0.9/viggocore/subsystem/file_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/file_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/file_sync/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.699433 viggocore-1.0.9/viggocore/subsystem/grant/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/grant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/grant/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.699433 viggocore-1.0.9/viggocore/subsystem/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/image/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/image/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/image/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/image/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/image/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/image/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.699433 viggocore-1.0.9/viggocore/subsystem/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/notification/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.699433 viggocore-1.0.9/viggocore/subsystem/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/policy/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.699433 viggocore-1.0.9/viggocore/subsystem/registration/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/registration/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/registration/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.699433 viggocore-1.0.9/viggocore/subsystem/role/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/role/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/role/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/role/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/role/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/role/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.699433 viggocore-1.0.9/viggocore/subsystem/route/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/route/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/route/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.703433 viggocore-1.0.9/viggocore/subsystem/tag/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/tag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/tag/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/tag/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/tag/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/tag/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.703433 viggocore-1.0.9/viggocore/subsystem/timeline_event/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      312 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/timeline_event/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1696 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/timeline_event/controller.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2767 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/timeline_event/manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2798 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/timeline_event/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.703433 viggocore-1.0.9/viggocore/subsystem/token/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/token/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/token/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/token/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.703433 viggocore-1.0.9/viggocore/subsystem/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/user/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/user/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/user/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/user/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/subsystem/user/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.703433 viggocore-1.0.9/viggocore/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.703433 viggocore-1.0.9/viggocore/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/tests/functional/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/tests/functional/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/tests/functional/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/tests/functional/test_grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/tests/functional/test_grants_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/tests/functional/test_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/tests/functional/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-07 12:42:06.000000 viggocore-1.0.9/viggocore/tests/functional/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:42:31.691433 viggocore-1.0.9/viggocore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-07 12:42:31.000000 viggocore-1.0.9/viggocore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-03-07 12:42:31.000000 viggocore-1.0.9/viggocore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 12:42:31.000000 viggocore-1.0.9/viggocore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-07 12:42:31.000000 viggocore-1.0.9/viggocore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-07 12:42:31.000000 viggocore-1.0.9/viggocore.egg-info/top_level.txt
```

### Comparing `viggocore-1.0.8/LICENSE` & `viggocore-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/README.md` & `viggocore-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/setup.py` & `viggocore-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/__init__.py` & `viggocore-1.0.9/viggocore/__init__.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/bootstrap/__init__.py` & `viggocore-1.0.9/viggocore/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/bootstrap/default/__init__.py` & `viggocore-1.0.9/viggocore/bootstrap/default/__init__.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/bootstrap/default/application.py` & `viggocore-1.0.9/viggocore/bootstrap/default/application.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/bootstrap/default/domain.py` & `viggocore-1.0.9/viggocore/bootstrap/default/domain.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/bootstrap/default/policies.py` & `viggocore-1.0.9/viggocore/bootstrap/default/policies.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/bootstrap/default/user.py` & `viggocore-1.0.9/viggocore/bootstrap/default/user.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/bootstrap/roles.py` & `viggocore-1.0.9/viggocore/bootstrap/roles.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/bootstrap/routes.py` & `viggocore-1.0.9/viggocore/bootstrap/routes.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/celery.py` & `viggocore-1.0.9/viggocore/celery.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/common/controller.py` & `viggocore-1.0.9/viggocore/common/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/common/exception.py` & `viggocore-1.0.9/viggocore/common/exception.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/common/input.py` & `viggocore-1.0.9/viggocore/common/input.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/common/manager.py` & `viggocore-1.0.9/viggocore/common/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/common/operation_after_post.py` & `viggocore-1.0.9/viggocore/common/operation_after_post.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/common/subsystem/__init__.py` & `viggocore-1.0.9/viggocore/common/subsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/common/subsystem/apihandler.py` & `viggocore-1.0.9/viggocore/common/subsystem/apihandler.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/common/subsystem/controller.py` & `viggocore-1.0.9/viggocore/common/subsystem/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/common/subsystem/driver.py` & `viggocore-1.0.9/viggocore/common/subsystem/driver.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/common/subsystem/entity.py` & `viggocore-1.0.9/viggocore/common/subsystem/entity.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/common/subsystem/manager.py` & `viggocore-1.0.9/viggocore/common/subsystem/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/common/subsystem/operation.py` & `viggocore-1.0.9/viggocore/common/subsystem/operation.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/common/subsystem/pagination.py` & `viggocore-1.0.9/viggocore/common/subsystem/pagination.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/common/subsystem/router.py` & `viggocore-1.0.9/viggocore/common/subsystem/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/common/utils.py` & `viggocore-1.0.9/viggocore/common/utils.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/queue.py` & `viggocore-1.0.9/viggocore/queue.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/request.py` & `viggocore-1.0.9/viggocore/request.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/resources.py` & `viggocore-1.0.9/viggocore/resources.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/scheduler.py` & `viggocore-1.0.9/viggocore/scheduler.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/application/controller.py` & `viggocore-1.0.9/viggocore/subsystem/application/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/application/manager.py` & `viggocore-1.0.9/viggocore/subsystem/application/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/application/resource.py` & `viggocore-1.0.9/viggocore/subsystem/application/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/application/router.py` & `viggocore-1.0.9/viggocore/subsystem/application/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/capability/manager.py` & `viggocore-1.0.9/viggocore/subsystem/capability/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/capability/resource.py` & `viggocore-1.0.9/viggocore/subsystem/capability/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/domain/controller.py` & `viggocore-1.0.9/viggocore/subsystem/domain/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/domain/manager.py` & `viggocore-1.0.9/viggocore/subsystem/domain/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/domain/resource.py` & `viggocore-1.0.9/viggocore/subsystem/domain/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/domain/router.py` & `viggocore-1.0.9/viggocore/subsystem/domain/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/domain/tasks.py` & `viggocore-1.0.9/viggocore/subsystem/domain/tasks.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/domain_sequence/controller.py` & `viggocore-1.0.9/viggocore/subsystem/domain_sequence/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/domain_sequence/manager.py` & `viggocore-1.0.9/viggocore/subsystem/domain_sequence/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/domain_sequence/resource.py` & `viggocore-1.0.9/viggocore/subsystem/domain_sequence/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/domain_sequence/router.py` & `viggocore-1.0.9/viggocore/subsystem/domain_sequence/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/file/controller.py` & `viggocore-1.0.9/viggocore/subsystem/file/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/file/manager.py` & `viggocore-1.0.9/viggocore/subsystem/file/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/file/resource.py` & `viggocore-1.0.9/viggocore/subsystem/file/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/file_sync/resource.py` & `viggocore-1.0.9/viggocore/subsystem/file_sync/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/grant/resource.py` & `viggocore-1.0.9/viggocore/subsystem/grant/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/image/controller.py` & `viggocore-1.0.9/viggocore/subsystem/image/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/image/handler.py` & `viggocore-1.0.9/viggocore/subsystem/image/handler.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/image/manager.py` & `viggocore-1.0.9/viggocore/subsystem/image/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/image/resource.py` & `viggocore-1.0.9/viggocore/subsystem/image/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/image/router.py` & `viggocore-1.0.9/viggocore/subsystem/image/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/notification/resource.py` & `viggocore-1.0.9/viggocore/subsystem/notification/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/policy/resource.py` & `viggocore-1.0.9/viggocore/subsystem/policy/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/registration/controller.py` & `viggocore-1.0.9/viggocore/subsystem/registration/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/registration/router.py` & `viggocore-1.0.9/viggocore/subsystem/registration/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/role/controller.py` & `viggocore-1.0.9/viggocore/subsystem/role/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/role/manager.py` & `viggocore-1.0.9/viggocore/subsystem/role/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/role/resource.py` & `viggocore-1.0.9/viggocore/subsystem/role/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/route/manager.py` & `viggocore-1.0.9/viggocore/subsystem/route/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/route/resource.py` & `viggocore-1.0.9/viggocore/subsystem/route/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/tag/controller.py` & `viggocore-1.0.9/viggocore/subsystem/tag/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/tag/manager.py` & `viggocore-1.0.9/viggocore/subsystem/tag/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/tag/resource.py` & `viggocore-1.0.9/viggocore/subsystem/tag/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/tag/router.py` & `viggocore-1.0.9/viggocore/subsystem/tag/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/timeline_event/controller.py` & `viggocore-1.0.9/viggocore/subsystem/timeline_event/controller.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/timeline_event/manager.py` & `viggocore-1.0.9/viggocore/subsystem/timeline_event/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/timeline_event/resource.py` & `viggocore-1.0.9/viggocore/subsystem/timeline_event/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/token/manager.py` & `viggocore-1.0.9/viggocore/subsystem/token/manager.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/token/resource.py` & `viggocore-1.0.9/viggocore/subsystem/token/resource.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/token/router.py` & `viggocore-1.0.9/viggocore/subsystem/token/router.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/user/controller.py` & `viggocore-1.0.9/viggocore/subsystem/user/controller.py`

 * *Files 13% similar despite different names*

```diff
@@ -201,7 +201,59 @@
                                   status=exc.status)
 
         response = {"roles": [role.to_dict() for role in roles]}
 
         return flask.Response(response=json.dumps(response, default=str),
                               status=200,
                               mimetype="application/json")
+
+    def update_settings(self, id):
+        try:
+            data = flask.request.get_json()
+
+            settings = self.manager.update_settings(id=id, **data)
+            response = {'settings': settings}
+
+            return flask.Response(response=utils.to_json(response),
+                                  status=200,
+                                  mimetype="application/json")
+        except exception.ViggoCoreException as exc:
+            return flask.Response(response=exc.message,
+                                  status=exc.status)
+
+    def _get_keys_from_args(self):
+        keys = flask.request.args.get('keys')
+        if not keys:
+            raise exception.BadRequest(
+                'ERRO! The keys parameter was not passed correctly')
+        return list(filter(None, keys.split(',')))
+
+    def remove_settings(self, id):
+        try:
+            keys = self._get_keys_from_args()
+            kwargs = {'keys': keys}
+
+            settings = self.manager.remove_settings(id=id, **kwargs)
+            response = {'settings': settings}
+
+            return flask.Response(response=utils.to_json(response),
+                                  status=200,
+                                  mimetype="application/json")
+        except exception.ViggoCoreException as exc:
+            return flask.Response(response=exc.message,
+                                  status=exc.status)
+
+    def get_user_settings_by_keys(self, id):
+        try:
+            keys = self._get_keys_from_args()
+            kwargs = {'keys': keys}
+
+            settings = self.manager.get_user_settings_by_keys(
+                id=id, **kwargs)
+            response = {'id': id, 'settings': settings}
+
+            return flask.Response(response=utils.to_json(response),
+                                  status=200,
+                                  mimetype="application/json")
+        except exception.ViggoCoreException as exc:
+            return flask.Response(response=exc.message,
+                                  status=exc.status)
```

### Comparing `viggocore-1.0.8/viggocore/subsystem/user/email.py` & `viggocore-1.0.9/viggocore/subsystem/user/email.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/subsystem/user/manager.py` & `viggocore-1.0.9/viggocore/subsystem/user/manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -231,24 +231,83 @@
         self.domain = self.manager.api.domains().get(id=self.user.domain_id)
         if not self.domain:
             raise exception.OperationBadRequest()
 
         send_email(self.type_email, self.token.id, self.user, self.domain)
 
 
+class UpdateSettings(operation.Update):
+
+    def pre(self, session, id: str, **kwargs) -> bool:
+        self.settings = kwargs
+        if self.settings is None or not self.settings:
+            raise exception.BadRequest("Erro! There is not a setting")
+        return super().pre(session=session, id=id)
+
+    def do(self, session, **kwargs):
+        result = {}
+        for key, value in self.settings.items():
+            new_value = self.entity.update_setting(key, value)
+            result[key] = new_value
+        super().do(session)
+
+        return result
+
+
+class RemoveSettings(operation.Update):
+
+    def pre(self, session, id: str, **kwargs) -> bool:
+        self.keys = kwargs.get('keys', [])
+        if not self.keys:
+            raise exception.BadRequest('Erro! keys are empty')
+        super().pre(session, id=id)
+
+        return self.entity.is_stable()
+
+    def do(self, session, **kwargs):
+        result = {}
+        for key in self.keys:
+            value = self.entity.remove_setting(key)
+            result[key] = value
+        super().do(session=session)
+
+        return result
+
+
+class GetUserSettingsByKeys(operation.Get):
+
+    def pre(self, session, id, **kwargs):
+        self.keys = kwargs.get('keys', [])
+        if not self.keys:
+            raise exception.BadRequest('Erro! keys are empty')
+        return super().pre(session, id=id)
+
+    def do(self, session, **kwargs):
+        entity = super().do(session=session)
+        settings = {}
+        for key in self.keys:
+            value = entity.settings.get(key, None)
+            if value is not None:
+                settings[key] = value
+        return settings
+
+
 class Manager(manager.Manager):
 
     def __init__(self, driver):
         super(Manager, self).__init__(driver)
         self.create = Create(self)
         self.update_password = UpdatePassword(self)
         self.restore = Restore(self)
         self.reset = Reset(self)
         self.routes = Routes(self)
         self.upload_photo = UploadPhoto(self)
         self.delete_photo = DeletePhoto(self)
         self.notify = Notify(self)
         self.authorize = Authorization(self)
         self.roles = Roles(self)
+        self.update_settings = UpdateSettings(self)
+        self.remove_settings = RemoveSettings(self)
+        self.get_user_settings_by_keys = GetUserSettingsByKeys(self)
 
     def hash_password(self, password):
         return hashlib.sha256(password.encode('utf-8')).hexdigest()
```

### Comparing `viggocore-1.0.8/viggocore/system.py` & `viggocore-1.0.9/viggocore/system.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/tests/functional/fixtures.py` & `viggocore-1.0.9/viggocore/tests/functional/fixtures.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/tests/functional/test_base.py` & `viggocore-1.0.9/viggocore/tests/functional/test_base.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/tests/functional/test_domains.py` & `viggocore-1.0.9/viggocore/tests/functional/test_domains.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/tests/functional/test_grants.py` & `viggocore-1.0.9/viggocore/tests/functional/test_grants.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/tests/functional/test_grants_policies.py` & `viggocore-1.0.9/viggocore/tests/functional/test_grants_policies.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/tests/functional/test_policies.py` & `viggocore-1.0.9/viggocore/tests/functional/test_policies.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/tests/functional/test_roles.py` & `viggocore-1.0.9/viggocore/tests/functional/test_roles.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore/tests/functional/test_users.py` & `viggocore-1.0.9/viggocore/tests/functional/test_users.py`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore.egg-info/SOURCES.txt` & `viggocore-1.0.9/viggocore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `viggocore-1.0.8/viggocore.egg-info/requires.txt` & `viggocore-1.0.9/viggocore.egg-info/requires.txt`

 * *Files identical despite different names*

