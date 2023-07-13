# Comparing `tmp/gdshoplib-2.0.3.tar.gz` & `tmp/gdshoplib-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdshoplib-2.0.3.tar", max compression
+gzip compressed data, was "gdshoplib-2.0.4.tar", max compression
```

## Comparing `gdshoplib-2.0.3.tar` & `gdshoplib-2.0.4.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     2004 2023-05-24 11:47:55.174891 gdshoplib-2.0.3/README.md
--rw-r--r--   0        0        0      210 2023-05-24 11:47:55.177560 gdshoplib-2.0.3/gdshoplib/__init__.py
--rw-r--r--   0        0        0       80 2023-01-03 20:04:30.238472 gdshoplib-2.0.3/gdshoplib/__main__.py
--rw-r--r--   0        0        0      117 2023-05-30 14:34:35.058893 gdshoplib-2.0.3/gdshoplib/activities/notion.py
--rw-r--r--   0        0        0        0 2023-01-01 19:36:37.507364 gdshoplib-2.0.3/gdshoplib/apps/__init__.py
--rw-r--r--   0        0        0      292 2023-05-24 11:47:55.179848 gdshoplib-2.0.3/gdshoplib/apps/crm/dialog.py
--rw-r--r--   0        0        0     3476 2023-05-24 11:47:55.182121 gdshoplib-2.0.3/gdshoplib/apps/crm/on_request.py
--rw-r--r--   0        0        0    10971 2023-07-13 20:19:45.468675 gdshoplib-2.0.3/gdshoplib/apps/crm/orders.py
--rw-r--r--   0        0        0      674 2023-05-24 11:47:55.186839 gdshoplib-2.0.3/gdshoplib/apps/crm/stats.py
--rw-r--r--   0        0        0      315 2023-05-24 11:47:55.189032 gdshoplib-2.0.3/gdshoplib/apps/delivery/delivery.py
--rw-r--r--   0        0        0        0 2022-11-29 21:45:29.003805 gdshoplib-2.0.3/gdshoplib/apps/finance/__init__.py
--rw-r--r--   0        0        0      206 2023-05-24 11:47:55.191346 gdshoplib-2.0.3/gdshoplib/apps/finance/storage.py
--rw-r--r--   0        0        0        0 2022-11-29 21:45:29.003925 gdshoplib-2.0.3/gdshoplib/apps/marketing/__init__.py
--rw-r--r--   0        0        0      163 2023-05-24 11:47:55.193504 gdshoplib-2.0.3/gdshoplib/apps/payments/payments.py
--rw-r--r--   0        0        0      378 2023-01-01 19:36:37.510481 gdshoplib-2.0.3/gdshoplib/apps/platforms/README.md
--rw-r--r--   0        0        0      665 2023-05-24 11:47:55.195540 gdshoplib-2.0.3/gdshoplib/apps/platforms/__init__.py
--rw-r--r--   0        0        0     1742 2023-05-24 11:47:55.197783 gdshoplib-2.0.3/gdshoplib/apps/platforms/avito.py
--rw-r--r--   0        0        0      113 2023-02-02 20:37:00.702563 gdshoplib-2.0.3/gdshoplib/apps/platforms/base.py
--rw-r--r--   0        0        0      152 2023-01-12 22:25:31.627980 gdshoplib-2.0.3/gdshoplib/apps/platforms/instagram.py
--rw-r--r--   0        0        0       95 2023-01-12 22:25:09.142423 gdshoplib-2.0.3/gdshoplib/apps/platforms/ok.py
--rw-r--r--   0        0        0      467 2023-05-24 11:47:55.199621 gdshoplib-2.0.3/gdshoplib/apps/platforms/sm.py
--rw-r--r--   0        0        0       95 2023-01-12 22:26:15.528644 gdshoplib-2.0.3/gdshoplib/apps/platforms/tg.py
--rw-r--r--   0        0        0      908 2023-05-24 11:47:55.201920 gdshoplib-2.0.3/gdshoplib/apps/platforms/ula.py
--rw-r--r--   0        0        0      512 2023-05-24 11:47:55.204568 gdshoplib-2.0.3/gdshoplib/apps/platforms/vk.py
--rw-r--r--   0        0        0     3373 2023-05-24 11:47:58.629272 gdshoplib-2.0.3/gdshoplib/apps/platforms/yam.py
--rw-r--r--   0        0        0      187 2023-01-01 19:36:37.519008 gdshoplib-2.0.3/gdshoplib/apps/products/README.md
--rw-r--r--   0        0        0        0 2022-11-29 21:45:29.004030 gdshoplib-2.0.3/gdshoplib/apps/products/__init__.py
--rw-r--r--   0        0        0     1931 2023-02-02 20:29:22.002155 gdshoplib-2.0.3/gdshoplib/apps/products/description.py
--rw-r--r--   0        0        0     5779 2023-07-12 22:35:57.507949 gdshoplib-2.0.3/gdshoplib/apps/products/media.py
--rw-r--r--   0        0        0     5168 2023-07-13 20:03:11.912355 gdshoplib-2.0.3/gdshoplib/apps/products/price.py
--rw-r--r--   0        0        0     5687 2023-05-30 20:06:07.280114 gdshoplib-2.0.3/gdshoplib/apps/products/product.py
--rw-r--r--   0        0        0     5947 2023-06-18 20:41:49.001382 gdshoplib-2.0.3/gdshoplib/apps/uploader/uploader.py
--rw-r--r--   0        0        0      562 2023-06-02 20:28:20.558582 gdshoplib-2.0.3/gdshoplib/cli/application.py
--rw-r--r--   0        0        0      243 2023-05-24 11:47:55.215449 gdshoplib-2.0.3/gdshoplib/cli/crm/application.py
--rw-r--r--   0        0        0     1098 2023-07-12 23:37:55.448098 gdshoplib-2.0.3/gdshoplib/cli/crm/order.py
--rw-r--r--   0        0        0      357 2023-05-24 11:47:55.219994 gdshoplib-2.0.3/gdshoplib/cli/crm/stats.py
--rw-r--r--   0        0        0      162 2023-05-24 11:47:55.222526 gdshoplib-2.0.3/gdshoplib/cli/finance/application.py
--rw-r--r--   0        0        0      383 2023-05-24 11:47:55.224775 gdshoplib-2.0.3/gdshoplib/cli/finance/store.py
--rw-r--r--   0        0        0      734 2023-05-30 20:06:07.282477 gdshoplib-2.0.3/gdshoplib/cli/product/application.py
--rw-r--r--   0        0        0     2239 2023-05-30 20:06:07.284766 gdshoplib-2.0.3/gdshoplib/cli/product/barcode_cli.py
--rw-r--r--   0        0        0     5334 2023-06-18 20:26:13.335384 gdshoplib-2.0.3/gdshoplib/cli/product/cache.py
--rw-r--r--   0        0        0     1963 2023-06-06 10:07:12.790146 gdshoplib-2.0.3/gdshoplib/cli/product/controle.py
--rw-r--r--   0        0        0     1797 2023-05-24 11:47:55.235444 gdshoplib-2.0.3/gdshoplib/cli/product/description.py
--rw-r--r--   0        0        0      672 2023-05-24 11:47:55.237453 gdshoplib-2.0.3/gdshoplib/cli/product/feed.py
--rw-r--r--   0        0        0     3091 2023-05-24 11:47:55.239401 gdshoplib-2.0.3/gdshoplib/cli/product/media.py
--rw-r--r--   0        0        0     1801 2023-07-09 23:42:39.264429 gdshoplib-2.0.3/gdshoplib/cli/product/price.py
--rw-r--r--   0        0        0      238 2023-05-24 11:47:55.243363 gdshoplib-2.0.3/gdshoplib/cli/service/application.py
--rw-r--r--   0        0        0      458 2023-06-02 20:27:44.870766 gdshoplib-2.0.3/gdshoplib/cli/service/avito.py
--rw-r--r--   0        0        0     1070 2023-06-02 22:30:11.800230 gdshoplib-2.0.3/gdshoplib/cli/service/vk.py
--rw-r--r--   0        0        0      962 2023-05-30 22:43:31.841649 gdshoplib-2.0.3/gdshoplib/cli/temporal/application.py
--rw-r--r--   0        0        0     1404 2023-06-13 21:49:15.384565 gdshoplib-2.0.3/gdshoplib/core/ecosystem.py
--rw-r--r--   0        0        0     3744 2023-07-13 20:02:49.341240 gdshoplib-2.0.3/gdshoplib/core/settings.py
--rw-r--r--   0        0        0        0 2023-01-01 19:36:37.525746 gdshoplib-2.0.3/gdshoplib/packages/__init__.py
--rw-r--r--   0        0        0     1320 2023-05-30 20:06:07.289858 gdshoplib-2.0.3/gdshoplib/packages/barcode_pack.py
--rw-r--r--   0        0        0     3829 2023-05-24 11:47:55.253311 gdshoplib-2.0.3/gdshoplib/packages/cache.py
--rw-r--r--   0        0        0     4177 2023-05-24 11:47:55.255216 gdshoplib-2.0.3/gdshoplib/packages/feed.py
--rw-r--r--   0        0        0      774 2023-01-01 19:36:37.530383 gdshoplib-2.0.3/gdshoplib/packages/lang.py
--rw-r--r--   0        0        0      148 2023-05-24 11:47:55.257504 gdshoplib-2.0.3/gdshoplib/packages/marker.py
--rw-r--r--   0        0        0     2362 2023-07-12 22:35:57.003635 gdshoplib-2.0.3/gdshoplib/packages/renderer.py
--rw-r--r--   0        0        0     3869 2023-06-15 19:46:00.483976 gdshoplib-2.0.3/gdshoplib/packages/s3.py
--rw-r--r--   0        0        0     1986 2023-06-18 20:25:34.332713 gdshoplib-2.0.3/gdshoplib/packages/s3v2.py
--rw-r--r--   0        0        0        0 2023-01-01 19:36:37.533334 gdshoplib-2.0.3/gdshoplib/services/__init__.py
--rw-r--r--   0        0        0     3746 2023-07-12 22:35:57.908452 gdshoplib-2.0.3/gdshoplib/services/avito/avito.py
--rw-r--r--   0        0        0        0 2023-07-04 21:57:07.519433 gdshoplib-2.0.3/gdshoplib/services/cdek/cdek.py
--rw-r--r--   0        0        0      106 2023-07-09 23:40:49.717481 gdshoplib-2.0.3/gdshoplib/services/gdshop/gdshop.py
--rw-r--r--   0        0        0     2821 2022-11-29 21:45:29.006810 gdshoplib-2.0.3/gdshoplib/services/notion/README.md
--rw-r--r--   0        0        0       50 2023-01-01 19:36:37.534464 gdshoplib-2.0.3/gdshoplib/services/notion/__init__.py
--rw-r--r--   0        0        0     1931 2023-07-12 21:53:17.811158 gdshoplib-2.0.3/gdshoplib/services/notion/base.py
--rw-r--r--   0        0        0      655 2023-06-11 10:01:55.572121 gdshoplib-2.0.3/gdshoplib/services/notion/block.py
--rw-r--r--   0        0        0     1174 2023-01-08 13:59:30.362864 gdshoplib-2.0.3/gdshoplib/services/notion/database.py
--rw-r--r--   0        0        0     1908 2023-07-12 22:35:57.809104 gdshoplib-2.0.3/gdshoplib/services/notion/manager.py
--rw-r--r--   0        0        0     2531 2023-05-24 11:47:55.273029 gdshoplib-2.0.3/gdshoplib/services/notion/models/props.py
--rw-r--r--   0        0        0     4027 2023-07-12 22:49:22.825924 gdshoplib-2.0.3/gdshoplib/services/notion/notion.py
--rw-r--r--   0        0        0    10195 2023-07-13 20:19:45.665950 gdshoplib-2.0.3/gdshoplib/services/notion/page.py
--rw-r--r--   0        0        0     2893 2023-05-24 11:47:55.277301 gdshoplib-2.0.3/gdshoplib/services/vk/market.py
--rw-r--r--   0        0        0     1825 2023-05-24 11:47:55.278048 gdshoplib-2.0.3/gdshoplib/services/vk/media.py
--rw-r--r--   0        0        0      986 2023-05-24 11:47:55.282128 gdshoplib-2.0.3/gdshoplib/services/vk/page.py
--rw-r--r--   0        0        0     2596 2023-05-24 11:47:55.285739 gdshoplib-2.0.3/gdshoplib/services/vk/stats.py
--rw-r--r--   0        0        0     2880 2023-05-24 11:47:58.644858 gdshoplib-2.0.3/gdshoplib/services/vk/stories.py
--rw-r--r--   0        0        0     2433 2023-07-12 22:35:57.881523 gdshoplib-2.0.3/gdshoplib/services/vk/vk.py
--rw-r--r--   0        0        0      104 2023-05-24 11:47:55.290271 gdshoplib-2.0.3/gdshoplib/services/ym/ym.py
--rw-r--r--   0        0        0      990 2023-07-09 23:40:49.720503 gdshoplib-2.0.3/gdshoplib/templates/basic.txt
--rw-r--r--   0        0        0      447 2023-05-24 11:47:55.298840 gdshoplib-2.0.3/gdshoplib/templates/instagram.txt
--rw-r--r--   0        0        0      990 2023-05-24 11:47:55.301319 gdshoplib-2.0.3/gdshoplib/templates/order_info.txt
--rw-r--r--   0        0        0      989 2023-05-24 11:47:55.305236 gdshoplib-2.0.3/gdshoplib/templates/ula.txt
--rw-r--r--   0        0        0     1052 2023-05-24 11:47:55.308271 gdshoplib-2.0.3/gdshoplib/templates/vk.txt
--rw-r--r--   0        0        0      470 2023-05-30 21:41:48.464779 gdshoplib-2.0.3/gdshoplib/workflows/notion.py
--rw-r--r--   0        0        0     1625 2023-07-13 20:03:19.980914 gdshoplib-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     3812 1970-01-01 00:00:00.000000 gdshoplib-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2004 2023-05-24 11:47:55.174891 gdshoplib-2.0.4/README.md
+-rw-r--r--   0        0        0      210 2023-05-24 11:47:55.177560 gdshoplib-2.0.4/gdshoplib/__init__.py
+-rw-r--r--   0        0        0       80 2023-01-03 20:04:30.238472 gdshoplib-2.0.4/gdshoplib/__main__.py
+-rw-r--r--   0        0        0      117 2023-05-30 14:34:35.058893 gdshoplib-2.0.4/gdshoplib/activities/notion.py
+-rw-r--r--   0        0        0        0 2023-01-01 19:36:37.507364 gdshoplib-2.0.4/gdshoplib/apps/__init__.py
+-rw-r--r--   0        0        0      292 2023-05-24 11:47:55.179848 gdshoplib-2.0.4/gdshoplib/apps/crm/dialog.py
+-rw-r--r--   0        0        0     3476 2023-05-24 11:47:55.182121 gdshoplib-2.0.4/gdshoplib/apps/crm/on_request.py
+-rw-r--r--   0        0        0    10971 2023-07-13 20:35:46.813516 gdshoplib-2.0.4/gdshoplib/apps/crm/orders.py
+-rw-r--r--   0        0        0      674 2023-05-24 11:47:55.186839 gdshoplib-2.0.4/gdshoplib/apps/crm/stats.py
+-rw-r--r--   0        0        0      315 2023-05-24 11:47:55.189032 gdshoplib-2.0.4/gdshoplib/apps/delivery/delivery.py
+-rw-r--r--   0        0        0        0 2022-11-29 21:45:29.003805 gdshoplib-2.0.4/gdshoplib/apps/finance/__init__.py
+-rw-r--r--   0        0        0      206 2023-05-24 11:47:55.191346 gdshoplib-2.0.4/gdshoplib/apps/finance/storage.py
+-rw-r--r--   0        0        0        0 2022-11-29 21:45:29.003925 gdshoplib-2.0.4/gdshoplib/apps/marketing/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-24 11:47:55.193504 gdshoplib-2.0.4/gdshoplib/apps/payments/payments.py
+-rw-r--r--   0        0        0      378 2023-01-01 19:36:37.510481 gdshoplib-2.0.4/gdshoplib/apps/platforms/README.md
+-rw-r--r--   0        0        0      665 2023-05-24 11:47:55.195540 gdshoplib-2.0.4/gdshoplib/apps/platforms/__init__.py
+-rw-r--r--   0        0        0     1742 2023-05-24 11:47:55.197783 gdshoplib-2.0.4/gdshoplib/apps/platforms/avito.py
+-rw-r--r--   0        0        0      113 2023-02-02 20:37:00.702563 gdshoplib-2.0.4/gdshoplib/apps/platforms/base.py
+-rw-r--r--   0        0        0      152 2023-01-12 22:25:31.627980 gdshoplib-2.0.4/gdshoplib/apps/platforms/instagram.py
+-rw-r--r--   0        0        0       95 2023-01-12 22:25:09.142423 gdshoplib-2.0.4/gdshoplib/apps/platforms/ok.py
+-rw-r--r--   0        0        0      467 2023-05-24 11:47:55.199621 gdshoplib-2.0.4/gdshoplib/apps/platforms/sm.py
+-rw-r--r--   0        0        0       95 2023-01-12 22:26:15.528644 gdshoplib-2.0.4/gdshoplib/apps/platforms/tg.py
+-rw-r--r--   0        0        0      908 2023-05-24 11:47:55.201920 gdshoplib-2.0.4/gdshoplib/apps/platforms/ula.py
+-rw-r--r--   0        0        0      512 2023-05-24 11:47:55.204568 gdshoplib-2.0.4/gdshoplib/apps/platforms/vk.py
+-rw-r--r--   0        0        0     3373 2023-05-24 11:47:58.629272 gdshoplib-2.0.4/gdshoplib/apps/platforms/yam.py
+-rw-r--r--   0        0        0      187 2023-01-01 19:36:37.519008 gdshoplib-2.0.4/gdshoplib/apps/products/README.md
+-rw-r--r--   0        0        0        0 2022-11-29 21:45:29.004030 gdshoplib-2.0.4/gdshoplib/apps/products/__init__.py
+-rw-r--r--   0        0        0     1931 2023-02-02 20:29:22.002155 gdshoplib-2.0.4/gdshoplib/apps/products/description.py
+-rw-r--r--   0        0        0     5779 2023-07-12 22:35:57.507949 gdshoplib-2.0.4/gdshoplib/apps/products/media.py
+-rw-r--r--   0        0        0     5169 2023-07-13 20:22:27.108468 gdshoplib-2.0.4/gdshoplib/apps/products/price.py
+-rw-r--r--   0        0        0     5687 2023-05-30 20:06:07.280114 gdshoplib-2.0.4/gdshoplib/apps/products/product.py
+-rw-r--r--   0        0        0     5947 2023-06-18 20:41:49.001382 gdshoplib-2.0.4/gdshoplib/apps/uploader/uploader.py
+-rw-r--r--   0        0        0      562 2023-06-02 20:28:20.558582 gdshoplib-2.0.4/gdshoplib/cli/application.py
+-rw-r--r--   0        0        0      243 2023-05-24 11:47:55.215449 gdshoplib-2.0.4/gdshoplib/cli/crm/application.py
+-rw-r--r--   0        0        0     1098 2023-07-12 23:37:55.448098 gdshoplib-2.0.4/gdshoplib/cli/crm/order.py
+-rw-r--r--   0        0        0      357 2023-05-24 11:47:55.219994 gdshoplib-2.0.4/gdshoplib/cli/crm/stats.py
+-rw-r--r--   0        0        0      162 2023-05-24 11:47:55.222526 gdshoplib-2.0.4/gdshoplib/cli/finance/application.py
+-rw-r--r--   0        0        0      383 2023-05-24 11:47:55.224775 gdshoplib-2.0.4/gdshoplib/cli/finance/store.py
+-rw-r--r--   0        0        0      734 2023-05-30 20:06:07.282477 gdshoplib-2.0.4/gdshoplib/cli/product/application.py
+-rw-r--r--   0        0        0     2239 2023-05-30 20:06:07.284766 gdshoplib-2.0.4/gdshoplib/cli/product/barcode_cli.py
+-rw-r--r--   0        0        0     5334 2023-06-18 20:26:13.335384 gdshoplib-2.0.4/gdshoplib/cli/product/cache.py
+-rw-r--r--   0        0        0     1963 2023-06-06 10:07:12.790146 gdshoplib-2.0.4/gdshoplib/cli/product/controle.py
+-rw-r--r--   0        0        0     1797 2023-05-24 11:47:55.235444 gdshoplib-2.0.4/gdshoplib/cli/product/description.py
+-rw-r--r--   0        0        0      672 2023-05-24 11:47:55.237453 gdshoplib-2.0.4/gdshoplib/cli/product/feed.py
+-rw-r--r--   0        0        0     3091 2023-05-24 11:47:55.239401 gdshoplib-2.0.4/gdshoplib/cli/product/media.py
+-rw-r--r--   0        0        0     1801 2023-07-09 23:42:39.264429 gdshoplib-2.0.4/gdshoplib/cli/product/price.py
+-rw-r--r--   0        0        0      238 2023-05-24 11:47:55.243363 gdshoplib-2.0.4/gdshoplib/cli/service/application.py
+-rw-r--r--   0        0        0      458 2023-06-02 20:27:44.870766 gdshoplib-2.0.4/gdshoplib/cli/service/avito.py
+-rw-r--r--   0        0        0     1070 2023-06-02 22:30:11.800230 gdshoplib-2.0.4/gdshoplib/cli/service/vk.py
+-rw-r--r--   0        0        0      962 2023-05-30 22:43:31.841649 gdshoplib-2.0.4/gdshoplib/cli/temporal/application.py
+-rw-r--r--   0        0        0     1404 2023-06-13 21:49:15.384565 gdshoplib-2.0.4/gdshoplib/core/ecosystem.py
+-rw-r--r--   0        0        0     3744 2023-07-13 20:02:49.341240 gdshoplib-2.0.4/gdshoplib/core/settings.py
+-rw-r--r--   0        0        0        0 2023-01-01 19:36:37.525746 gdshoplib-2.0.4/gdshoplib/packages/__init__.py
+-rw-r--r--   0        0        0     1320 2023-05-30 20:06:07.289858 gdshoplib-2.0.4/gdshoplib/packages/barcode_pack.py
+-rw-r--r--   0        0        0     3829 2023-05-24 11:47:55.253311 gdshoplib-2.0.4/gdshoplib/packages/cache.py
+-rw-r--r--   0        0        0     4177 2023-05-24 11:47:55.255216 gdshoplib-2.0.4/gdshoplib/packages/feed.py
+-rw-r--r--   0        0        0      774 2023-01-01 19:36:37.530383 gdshoplib-2.0.4/gdshoplib/packages/lang.py
+-rw-r--r--   0        0        0      148 2023-05-24 11:47:55.257504 gdshoplib-2.0.4/gdshoplib/packages/marker.py
+-rw-r--r--   0        0        0     2362 2023-07-12 22:35:57.003635 gdshoplib-2.0.4/gdshoplib/packages/renderer.py
+-rw-r--r--   0        0        0     3869 2023-06-15 19:46:00.483976 gdshoplib-2.0.4/gdshoplib/packages/s3.py
+-rw-r--r--   0        0        0     1986 2023-06-18 20:25:34.332713 gdshoplib-2.0.4/gdshoplib/packages/s3v2.py
+-rw-r--r--   0        0        0        0 2023-01-01 19:36:37.533334 gdshoplib-2.0.4/gdshoplib/services/__init__.py
+-rw-r--r--   0        0        0     3746 2023-07-12 22:35:57.908452 gdshoplib-2.0.4/gdshoplib/services/avito/avito.py
+-rw-r--r--   0        0        0        0 2023-07-04 21:57:07.519433 gdshoplib-2.0.4/gdshoplib/services/cdek/cdek.py
+-rw-r--r--   0        0        0      106 2023-07-09 23:40:49.717481 gdshoplib-2.0.4/gdshoplib/services/gdshop/gdshop.py
+-rw-r--r--   0        0        0     2821 2022-11-29 21:45:29.006810 gdshoplib-2.0.4/gdshoplib/services/notion/README.md
+-rw-r--r--   0        0        0       50 2023-01-01 19:36:37.534464 gdshoplib-2.0.4/gdshoplib/services/notion/__init__.py
+-rw-r--r--   0        0        0     1931 2023-07-12 21:53:17.811158 gdshoplib-2.0.4/gdshoplib/services/notion/base.py
+-rw-r--r--   0        0        0      655 2023-06-11 10:01:55.572121 gdshoplib-2.0.4/gdshoplib/services/notion/block.py
+-rw-r--r--   0        0        0     1174 2023-01-08 13:59:30.362864 gdshoplib-2.0.4/gdshoplib/services/notion/database.py
+-rw-r--r--   0        0        0     1908 2023-07-12 22:35:57.809104 gdshoplib-2.0.4/gdshoplib/services/notion/manager.py
+-rw-r--r--   0        0        0     2531 2023-05-24 11:47:55.273029 gdshoplib-2.0.4/gdshoplib/services/notion/models/props.py
+-rw-r--r--   0        0        0     4027 2023-07-12 22:49:22.825924 gdshoplib-2.0.4/gdshoplib/services/notion/notion.py
+-rw-r--r--   0        0        0    10195 2023-07-13 20:19:45.665950 gdshoplib-2.0.4/gdshoplib/services/notion/page.py
+-rw-r--r--   0        0        0     2893 2023-05-24 11:47:55.277301 gdshoplib-2.0.4/gdshoplib/services/vk/market.py
+-rw-r--r--   0        0        0     1825 2023-05-24 11:47:55.278048 gdshoplib-2.0.4/gdshoplib/services/vk/media.py
+-rw-r--r--   0        0        0      986 2023-05-24 11:47:55.282128 gdshoplib-2.0.4/gdshoplib/services/vk/page.py
+-rw-r--r--   0        0        0     2596 2023-05-24 11:47:55.285739 gdshoplib-2.0.4/gdshoplib/services/vk/stats.py
+-rw-r--r--   0        0        0     2880 2023-05-24 11:47:58.644858 gdshoplib-2.0.4/gdshoplib/services/vk/stories.py
+-rw-r--r--   0        0        0     2433 2023-07-12 22:35:57.881523 gdshoplib-2.0.4/gdshoplib/services/vk/vk.py
+-rw-r--r--   0        0        0      104 2023-05-24 11:47:55.290271 gdshoplib-2.0.4/gdshoplib/services/ym/ym.py
+-rw-r--r--   0        0        0      990 2023-07-09 23:40:49.720503 gdshoplib-2.0.4/gdshoplib/templates/basic.txt
+-rw-r--r--   0        0        0      447 2023-05-24 11:47:55.298840 gdshoplib-2.0.4/gdshoplib/templates/instagram.txt
+-rw-r--r--   0        0        0      990 2023-05-24 11:47:55.301319 gdshoplib-2.0.4/gdshoplib/templates/order_info.txt
+-rw-r--r--   0        0        0      989 2023-05-24 11:47:55.305236 gdshoplib-2.0.4/gdshoplib/templates/ula.txt
+-rw-r--r--   0        0        0     1052 2023-05-24 11:47:55.308271 gdshoplib-2.0.4/gdshoplib/templates/vk.txt
+-rw-r--r--   0        0        0      470 2023-05-30 21:41:48.464779 gdshoplib-2.0.4/gdshoplib/workflows/notion.py
+-rw-r--r--   0        0        0     1625 2023-07-13 20:22:45.524334 gdshoplib-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3812 1970-01-01 00:00:00.000000 gdshoplib-2.0.4/PKG-INFO
```

### Comparing `gdshoplib-2.0.3/README.md` & `gdshoplib-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/apps/crm/on_request.py` & `gdshoplib-2.0.4/gdshoplib/apps/crm/on_request.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/apps/crm/orders.py` & `gdshoplib-2.0.4/gdshoplib/apps/crm/orders.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/apps/crm/stats.py` & `gdshoplib-2.0.4/gdshoplib/apps/crm/stats.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/apps/platforms/__init__.py` & `gdshoplib-2.0.4/gdshoplib/apps/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/apps/platforms/avito.py` & `gdshoplib-2.0.4/gdshoplib/apps/platforms/avito.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/apps/platforms/ula.py` & `gdshoplib-2.0.4/gdshoplib/apps/platforms/ula.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/apps/platforms/vk.py` & `gdshoplib-2.0.4/gdshoplib/apps/platforms/vk.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/apps/platforms/yam.py` & `gdshoplib-2.0.4/gdshoplib/apps/platforms/yam.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/apps/products/description.py` & `gdshoplib-2.0.4/gdshoplib/apps/products/description.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/apps/products/media.py` & `gdshoplib-2.0.4/gdshoplib/apps/products/media.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/apps/products/price.py` & `gdshoplib-2.0.4/gdshoplib/apps/products/price.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         return wrap
 
     @property
     @psycho_price
     @round
     def now(self):
         date = datetime.date.today() - datetime.timedelta(days=6 * 30)
-        if self.product.edited_time.date() < date:
+        if self.product.created_time.date() < date:
             return self.real_gross
 
         discount = self.get_score()
         if discount:
             _now = self.profit + self.profit * (discount * 0.01)
             if _now < self.neitral:
                 return self.neitral
```

### Comparing `gdshoplib-2.0.3/gdshoplib/apps/products/product.py` & `gdshoplib-2.0.4/gdshoplib/apps/products/product.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/apps/uploader/uploader.py` & `gdshoplib-2.0.4/gdshoplib/apps/uploader/uploader.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/cli/application.py` & `gdshoplib-2.0.4/gdshoplib/cli/application.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/cli/crm/order.py` & `gdshoplib-2.0.4/gdshoplib/cli/crm/order.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/cli/product/application.py` & `gdshoplib-2.0.4/gdshoplib/cli/product/application.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/cli/product/barcode_cli.py` & `gdshoplib-2.0.4/gdshoplib/cli/product/barcode_cli.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/cli/product/cache.py` & `gdshoplib-2.0.4/gdshoplib/cli/product/cache.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/cli/product/controle.py` & `gdshoplib-2.0.4/gdshoplib/cli/product/controle.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/cli/product/description.py` & `gdshoplib-2.0.4/gdshoplib/cli/product/description.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/cli/product/feed.py` & `gdshoplib-2.0.4/gdshoplib/cli/product/feed.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/cli/product/media.py` & `gdshoplib-2.0.4/gdshoplib/cli/product/media.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/cli/product/price.py` & `gdshoplib-2.0.4/gdshoplib/cli/product/price.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/cli/service/vk.py` & `gdshoplib-2.0.4/gdshoplib/cli/service/vk.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/cli/temporal/application.py` & `gdshoplib-2.0.4/gdshoplib/cli/temporal/application.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/core/ecosystem.py` & `gdshoplib-2.0.4/gdshoplib/core/ecosystem.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/core/settings.py` & `gdshoplib-2.0.4/gdshoplib/core/settings.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/packages/barcode_pack.py` & `gdshoplib-2.0.4/gdshoplib/packages/barcode_pack.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/packages/cache.py` & `gdshoplib-2.0.4/gdshoplib/packages/cache.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/packages/feed.py` & `gdshoplib-2.0.4/gdshoplib/packages/feed.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/packages/lang.py` & `gdshoplib-2.0.4/gdshoplib/packages/lang.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/packages/renderer.py` & `gdshoplib-2.0.4/gdshoplib/packages/renderer.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/packages/s3.py` & `gdshoplib-2.0.4/gdshoplib/packages/s3.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/packages/s3v2.py` & `gdshoplib-2.0.4/gdshoplib/packages/s3v2.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/services/avito/avito.py` & `gdshoplib-2.0.4/gdshoplib/services/avito/avito.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/services/notion/README.md` & `gdshoplib-2.0.4/gdshoplib/services/notion/README.md`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/services/notion/base.py` & `gdshoplib-2.0.4/gdshoplib/services/notion/base.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/services/notion/block.py` & `gdshoplib-2.0.4/gdshoplib/services/notion/block.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/services/notion/database.py` & `gdshoplib-2.0.4/gdshoplib/services/notion/database.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/services/notion/manager.py` & `gdshoplib-2.0.4/gdshoplib/services/notion/manager.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/services/notion/models/props.py` & `gdshoplib-2.0.4/gdshoplib/services/notion/models/props.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/services/notion/notion.py` & `gdshoplib-2.0.4/gdshoplib/services/notion/notion.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/services/notion/page.py` & `gdshoplib-2.0.4/gdshoplib/services/notion/page.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/services/vk/market.py` & `gdshoplib-2.0.4/gdshoplib/services/vk/market.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/services/vk/media.py` & `gdshoplib-2.0.4/gdshoplib/services/vk/media.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/services/vk/page.py` & `gdshoplib-2.0.4/gdshoplib/services/vk/page.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/services/vk/stats.py` & `gdshoplib-2.0.4/gdshoplib/services/vk/stats.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/services/vk/stories.py` & `gdshoplib-2.0.4/gdshoplib/services/vk/stories.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/services/vk/vk.py` & `gdshoplib-2.0.4/gdshoplib/services/vk/vk.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/templates/basic.txt` & `gdshoplib-2.0.4/gdshoplib/templates/basic.txt`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/templates/order_info.txt` & `gdshoplib-2.0.4/gdshoplib/templates/order_info.txt`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/templates/ula.txt` & `gdshoplib-2.0.4/gdshoplib/templates/ula.txt`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/gdshoplib/templates/vk.txt` & `gdshoplib-2.0.4/gdshoplib/templates/vk.txt`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.3/pyproject.toml` & `gdshoplib-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gdshoplib"
-version = "2.0.3"
+version = "2.0.4"
 description = ""
 authors = ["Nikolay Baryshnikov <root@k0d.ru>"]
 packages=[
     { include = "gdshoplib" },
 ]
 license="MIT"
 readme="README.md"
```

### Comparing `gdshoplib-2.0.3/PKG-INFO` & `gdshoplib-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdshoplib
-Version: 2.0.3
+Version: 2.0.4
 Summary: 
 Home-page: https://github.com/p141592
 License: MIT
 Author: Nikolay Baryshnikov
 Author-email: root@k0d.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

