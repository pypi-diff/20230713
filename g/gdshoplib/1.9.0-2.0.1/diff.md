# Comparing `tmp/gdshoplib-1.9.0.tar.gz` & `tmp/gdshoplib-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdshoplib-1.9.0.tar", max compression
+gzip compressed data, was "gdshoplib-2.0.1.tar", max compression
```

## Comparing `gdshoplib-1.9.0.tar` & `gdshoplib-2.0.1.tar`

### file list

```diff
@@ -1,48 +1,89 @@
--rw-r--r--   0        0        0     1855 2023-01-02 14:26:10.856806 gdshoplib-1.9.0/README.md
--rw-r--r--   0        0        0      195 2023-01-03 20:09:44.498187 gdshoplib-1.9.0/gdshoplib/__init__.py
--rw-r--r--   0        0        0       80 2023-01-03 20:04:30.238472 gdshoplib-1.9.0/gdshoplib/__main__.py
--rw-r--r--   0        0        0        0 2023-01-01 19:36:37.507364 gdshoplib-1.9.0/gdshoplib/apps/__init__.py
--rw-r--r--   0        0        0        0 2022-11-29 21:45:29.003805 gdshoplib-1.9.0/gdshoplib/apps/finance/__init__.py
--rw-r--r--   0        0        0        0 2022-11-29 21:45:29.003925 gdshoplib-1.9.0/gdshoplib/apps/marketing/__init__.py
--rw-r--r--   0        0        0     1234 2023-01-03 19:49:37.886499 gdshoplib-1.9.0/gdshoplib/apps/platform.py
--rw-r--r--   0        0        0      378 2023-01-01 19:36:37.510481 gdshoplib-1.9.0/gdshoplib/apps/platforms/README.md
--rw-r--r--   0        0        0      435 2023-01-01 19:36:37.511353 gdshoplib-1.9.0/gdshoplib/apps/platforms/__init__.py
--rw-r--r--   0        0        0     1573 2023-01-06 17:56:48.286983 gdshoplib-1.9.0/gdshoplib/apps/platforms/avito.py
--rw-r--r--   0        0        0      388 2023-01-01 19:36:37.513182 gdshoplib-1.9.0/gdshoplib/apps/platforms/base.py
--rw-r--r--   0        0        0      221 2023-01-01 19:36:37.513924 gdshoplib-1.9.0/gdshoplib/apps/platforms/instagram.py
--rw-r--r--   0        0        0      164 2023-01-01 19:36:37.514817 gdshoplib-1.9.0/gdshoplib/apps/platforms/ok.py
--rw-r--r--   0        0        0      164 2023-01-01 19:36:37.515587 gdshoplib-1.9.0/gdshoplib/apps/platforms/tg.py
--rw-r--r--   0        0        0      924 2023-01-01 19:36:37.516436 gdshoplib-1.9.0/gdshoplib/apps/platforms/ula.py
--rw-r--r--   0        0        0      200 2023-01-01 19:36:37.517154 gdshoplib-1.9.0/gdshoplib/apps/platforms/vk.py
--rw-r--r--   0        0        0      174 2023-01-01 19:36:37.517919 gdshoplib-1.9.0/gdshoplib/apps/platforms/yam.py
--rw-r--r--   0        0        0     4849 2023-01-12 18:21:47.686707 gdshoplib-1.9.0/gdshoplib/apps/product.py
--rw-r--r--   0        0        0      187 2023-01-01 19:36:37.519008 gdshoplib-1.9.0/gdshoplib/apps/products/README.md
--rw-r--r--   0        0        0        0 2022-11-29 21:45:29.004030 gdshoplib-1.9.0/gdshoplib/apps/products/__init__.py
--rw-r--r--   0        0        0     1931 2023-01-01 19:36:37.520803 gdshoplib-1.9.0/gdshoplib/apps/products/description.py
--rw-r--r--   0        0        0     2160 2023-01-01 20:08:35.653603 gdshoplib-1.9.0/gdshoplib/apps/products/media.py
--rw-r--r--   0        0        0     3730 2023-01-12 19:28:36.751691 gdshoplib-1.9.0/gdshoplib/apps/products/price.py
--rw-r--r--   0        0        0     9381 2023-01-12 18:21:47.691820 gdshoplib-1.9.0/gdshoplib/cli/application.py
--rw-r--r--   0        0        0     3401 2023-01-12 18:21:47.694016 gdshoplib-1.9.0/gdshoplib/core/settings.py
--rw-r--r--   0        0        0        0 2023-01-01 19:36:37.525746 gdshoplib-1.9.0/gdshoplib/packages/__init__.py
--rw-r--r--   0        0        0     3063 2023-01-09 20:19:16.166687 gdshoplib-1.9.0/gdshoplib/packages/cache.py
--rw-r--r--   0        0        0     2822 2023-01-06 17:56:22.155056 gdshoplib-1.9.0/gdshoplib/packages/feed.py
--rw-r--r--   0        0        0      774 2023-01-01 19:36:37.530383 gdshoplib-1.9.0/gdshoplib/packages/lang.py
--rw-r--r--   0        0        0     1820 2023-01-01 23:04:08.211299 gdshoplib-1.9.0/gdshoplib/packages/s3.py
--rw-r--r--   0        0        0        0 2023-01-01 19:36:37.533334 gdshoplib-1.9.0/gdshoplib/services/__init__.py
--rw-r--r--   0        0        0     2821 2022-11-29 21:45:29.006810 gdshoplib-1.9.0/gdshoplib/services/notion/README.md
--rw-r--r--   0        0        0       50 2023-01-01 19:36:37.534464 gdshoplib-1.9.0/gdshoplib/services/notion/__init__.py
--rw-r--r--   0        0        0     1729 2023-01-08 13:59:30.361038 gdshoplib-1.9.0/gdshoplib/services/notion/base.py
--rw-r--r--   0        0        0      655 2023-01-08 13:59:30.361846 gdshoplib-1.9.0/gdshoplib/services/notion/block.py
--rw-r--r--   0        0        0     1174 2023-01-08 13:59:30.362864 gdshoplib-1.9.0/gdshoplib/services/notion/database.py
--rw-r--r--   0        0        0     1296 2023-01-08 13:59:30.363533 gdshoplib-1.9.0/gdshoplib/services/notion/manager.py
--rw-r--r--   0        0        0     2981 2023-01-08 13:59:30.364304 gdshoplib-1.9.0/gdshoplib/services/notion/notion.py
--rw-r--r--   0        0        0     7375 2023-01-12 19:28:36.931278 gdshoplib-1.9.0/gdshoplib/services/notion/page.py
--rw-r--r--   0        0        0      811 2023-01-09 19:33:42.813057 gdshoplib-1.9.0/gdshoplib/services/vk/market.py
--rw-r--r--   0        0        0     2318 2023-01-08 18:33:35.656110 gdshoplib-1.9.0/gdshoplib/services/vk/vk.py
--rw-r--r--   0        0        0     1046 2023-01-08 13:59:30.366542 gdshoplib-1.9.0/gdshoplib/templates/basic.txt
--rw-r--r--   0        0        0      446 2023-01-06 19:31:05.484065 gdshoplib-1.9.0/gdshoplib/templates/instagram.txt
--rw-r--r--   0        0        0     1045 2023-01-08 13:59:30.367558 gdshoplib-1.9.0/gdshoplib/templates/ula.txt
--rw-r--r--   0        0        0     1108 2023-01-08 13:59:30.368645 gdshoplib-1.9.0/gdshoplib/templates/vk.txt
--rw-r--r--   0        0        0     1426 2023-01-12 19:28:29.421278 gdshoplib-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     3274 1970-01-01 00:00:00.000000 gdshoplib-1.9.0/setup.py
--rw-r--r--   0        0        0     3301 1970-01-01 00:00:00.000000 gdshoplib-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2004 2023-05-24 11:47:55.174891 gdshoplib-2.0.1/README.md
+-rw-r--r--   0        0        0      210 2023-05-24 11:47:55.177560 gdshoplib-2.0.1/gdshoplib/__init__.py
+-rw-r--r--   0        0        0       80 2023-01-03 20:04:30.238472 gdshoplib-2.0.1/gdshoplib/__main__.py
+-rw-r--r--   0        0        0      117 2023-05-30 14:34:35.058893 gdshoplib-2.0.1/gdshoplib/activities/notion.py
+-rw-r--r--   0        0        0        0 2023-01-01 19:36:37.507364 gdshoplib-2.0.1/gdshoplib/apps/__init__.py
+-rw-r--r--   0        0        0      292 2023-05-24 11:47:55.179848 gdshoplib-2.0.1/gdshoplib/apps/crm/dialog.py
+-rw-r--r--   0        0        0     3476 2023-05-24 11:47:55.182121 gdshoplib-2.0.1/gdshoplib/apps/crm/on_request.py
+-rw-r--r--   0        0        0    10293 2023-07-12 22:35:57.575594 gdshoplib-2.0.1/gdshoplib/apps/crm/orders.py
+-rw-r--r--   0        0        0      674 2023-05-24 11:47:55.186839 gdshoplib-2.0.1/gdshoplib/apps/crm/stats.py
+-rw-r--r--   0        0        0      315 2023-05-24 11:47:55.189032 gdshoplib-2.0.1/gdshoplib/apps/delivery/delivery.py
+-rw-r--r--   0        0        0        0 2022-11-29 21:45:29.003805 gdshoplib-2.0.1/gdshoplib/apps/finance/__init__.py
+-rw-r--r--   0        0        0      206 2023-05-24 11:47:55.191346 gdshoplib-2.0.1/gdshoplib/apps/finance/storage.py
+-rw-r--r--   0        0        0        0 2022-11-29 21:45:29.003925 gdshoplib-2.0.1/gdshoplib/apps/marketing/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-24 11:47:55.193504 gdshoplib-2.0.1/gdshoplib/apps/payments/payments.py
+-rw-r--r--   0        0        0      378 2023-01-01 19:36:37.510481 gdshoplib-2.0.1/gdshoplib/apps/platforms/README.md
+-rw-r--r--   0        0        0      665 2023-05-24 11:47:55.195540 gdshoplib-2.0.1/gdshoplib/apps/platforms/__init__.py
+-rw-r--r--   0        0        0     1742 2023-05-24 11:47:55.197783 gdshoplib-2.0.1/gdshoplib/apps/platforms/avito.py
+-rw-r--r--   0        0        0      113 2023-02-02 20:37:00.702563 gdshoplib-2.0.1/gdshoplib/apps/platforms/base.py
+-rw-r--r--   0        0        0      152 2023-01-12 22:25:31.627980 gdshoplib-2.0.1/gdshoplib/apps/platforms/instagram.py
+-rw-r--r--   0        0        0       95 2023-01-12 22:25:09.142423 gdshoplib-2.0.1/gdshoplib/apps/platforms/ok.py
+-rw-r--r--   0        0        0      467 2023-05-24 11:47:55.199621 gdshoplib-2.0.1/gdshoplib/apps/platforms/sm.py
+-rw-r--r--   0        0        0       95 2023-01-12 22:26:15.528644 gdshoplib-2.0.1/gdshoplib/apps/platforms/tg.py
+-rw-r--r--   0        0        0      908 2023-05-24 11:47:55.201920 gdshoplib-2.0.1/gdshoplib/apps/platforms/ula.py
+-rw-r--r--   0        0        0      512 2023-05-24 11:47:55.204568 gdshoplib-2.0.1/gdshoplib/apps/platforms/vk.py
+-rw-r--r--   0        0        0     3373 2023-05-24 11:47:58.629272 gdshoplib-2.0.1/gdshoplib/apps/platforms/yam.py
+-rw-r--r--   0        0        0      187 2023-01-01 19:36:37.519008 gdshoplib-2.0.1/gdshoplib/apps/products/README.md
+-rw-r--r--   0        0        0        0 2022-11-29 21:45:29.004030 gdshoplib-2.0.1/gdshoplib/apps/products/__init__.py
+-rw-r--r--   0        0        0     1931 2023-02-02 20:29:22.002155 gdshoplib-2.0.1/gdshoplib/apps/products/description.py
+-rw-r--r--   0        0        0     5779 2023-07-12 22:35:57.507949 gdshoplib-2.0.1/gdshoplib/apps/products/media.py
+-rw-r--r--   0        0        0     4891 2023-07-09 23:40:49.713961 gdshoplib-2.0.1/gdshoplib/apps/products/price.py
+-rw-r--r--   0        0        0     5687 2023-05-30 20:06:07.280114 gdshoplib-2.0.1/gdshoplib/apps/products/product.py
+-rw-r--r--   0        0        0     5947 2023-06-18 20:41:49.001382 gdshoplib-2.0.1/gdshoplib/apps/uploader/uploader.py
+-rw-r--r--   0        0        0      562 2023-06-02 20:28:20.558582 gdshoplib-2.0.1/gdshoplib/cli/application.py
+-rw-r--r--   0        0        0      243 2023-05-24 11:47:55.215449 gdshoplib-2.0.1/gdshoplib/cli/crm/application.py
+-rw-r--r--   0        0        0      815 2023-07-12 22:05:54.854926 gdshoplib-2.0.1/gdshoplib/cli/crm/order.py
+-rw-r--r--   0        0        0      357 2023-05-24 11:47:55.219994 gdshoplib-2.0.1/gdshoplib/cli/crm/stats.py
+-rw-r--r--   0        0        0      162 2023-05-24 11:47:55.222526 gdshoplib-2.0.1/gdshoplib/cli/finance/application.py
+-rw-r--r--   0        0        0      383 2023-05-24 11:47:55.224775 gdshoplib-2.0.1/gdshoplib/cli/finance/store.py
+-rw-r--r--   0        0        0      734 2023-05-30 20:06:07.282477 gdshoplib-2.0.1/gdshoplib/cli/product/application.py
+-rw-r--r--   0        0        0     2239 2023-05-30 20:06:07.284766 gdshoplib-2.0.1/gdshoplib/cli/product/barcode_cli.py
+-rw-r--r--   0        0        0     5334 2023-06-18 20:26:13.335384 gdshoplib-2.0.1/gdshoplib/cli/product/cache.py
+-rw-r--r--   0        0        0     1963 2023-06-06 10:07:12.790146 gdshoplib-2.0.1/gdshoplib/cli/product/controle.py
+-rw-r--r--   0        0        0     1797 2023-05-24 11:47:55.235444 gdshoplib-2.0.1/gdshoplib/cli/product/description.py
+-rw-r--r--   0        0        0      672 2023-05-24 11:47:55.237453 gdshoplib-2.0.1/gdshoplib/cli/product/feed.py
+-rw-r--r--   0        0        0     3091 2023-05-24 11:47:55.239401 gdshoplib-2.0.1/gdshoplib/cli/product/media.py
+-rw-r--r--   0        0        0     1801 2023-07-09 23:42:39.264429 gdshoplib-2.0.1/gdshoplib/cli/product/price.py
+-rw-r--r--   0        0        0      238 2023-05-24 11:47:55.243363 gdshoplib-2.0.1/gdshoplib/cli/service/application.py
+-rw-r--r--   0        0        0      458 2023-06-02 20:27:44.870766 gdshoplib-2.0.1/gdshoplib/cli/service/avito.py
+-rw-r--r--   0        0        0     1070 2023-06-02 22:30:11.800230 gdshoplib-2.0.1/gdshoplib/cli/service/vk.py
+-rw-r--r--   0        0        0      962 2023-05-30 22:43:31.841649 gdshoplib-2.0.1/gdshoplib/cli/temporal/application.py
+-rw-r--r--   0        0        0     1404 2023-06-13 21:49:15.384565 gdshoplib-2.0.1/gdshoplib/core/ecosystem.py
+-rw-r--r--   0        0        0     3744 2023-07-09 23:43:15.959486 gdshoplib-2.0.1/gdshoplib/core/settings.py
+-rw-r--r--   0        0        0        0 2023-01-01 19:36:37.525746 gdshoplib-2.0.1/gdshoplib/packages/__init__.py
+-rw-r--r--   0        0        0     1320 2023-05-30 20:06:07.289858 gdshoplib-2.0.1/gdshoplib/packages/barcode_pack.py
+-rw-r--r--   0        0        0     3829 2023-05-24 11:47:55.253311 gdshoplib-2.0.1/gdshoplib/packages/cache.py
+-rw-r--r--   0        0        0     4177 2023-05-24 11:47:55.255216 gdshoplib-2.0.1/gdshoplib/packages/feed.py
+-rw-r--r--   0        0        0      774 2023-01-01 19:36:37.530383 gdshoplib-2.0.1/gdshoplib/packages/lang.py
+-rw-r--r--   0        0        0      148 2023-05-24 11:47:55.257504 gdshoplib-2.0.1/gdshoplib/packages/marker.py
+-rw-r--r--   0        0        0     2362 2023-07-12 22:35:57.003635 gdshoplib-2.0.1/gdshoplib/packages/renderer.py
+-rw-r--r--   0        0        0     3869 2023-06-15 19:46:00.483976 gdshoplib-2.0.1/gdshoplib/packages/s3.py
+-rw-r--r--   0        0        0     1986 2023-06-18 20:25:34.332713 gdshoplib-2.0.1/gdshoplib/packages/s3v2.py
+-rw-r--r--   0        0        0        0 2023-01-01 19:36:37.533334 gdshoplib-2.0.1/gdshoplib/services/__init__.py
+-rw-r--r--   0        0        0     3746 2023-07-12 22:35:57.908452 gdshoplib-2.0.1/gdshoplib/services/avito/avito.py
+-rw-r--r--   0        0        0        0 2023-07-04 21:57:07.519433 gdshoplib-2.0.1/gdshoplib/services/cdek/cdek.py
+-rw-r--r--   0        0        0      106 2023-07-09 23:40:49.717481 gdshoplib-2.0.1/gdshoplib/services/gdshop/gdshop.py
+-rw-r--r--   0        0        0     2821 2022-11-29 21:45:29.006810 gdshoplib-2.0.1/gdshoplib/services/notion/README.md
+-rw-r--r--   0        0        0       50 2023-01-01 19:36:37.534464 gdshoplib-2.0.1/gdshoplib/services/notion/__init__.py
+-rw-r--r--   0        0        0     1931 2023-07-12 21:53:17.811158 gdshoplib-2.0.1/gdshoplib/services/notion/base.py
+-rw-r--r--   0        0        0      655 2023-06-11 10:01:55.572121 gdshoplib-2.0.1/gdshoplib/services/notion/block.py
+-rw-r--r--   0        0        0     1174 2023-01-08 13:59:30.362864 gdshoplib-2.0.1/gdshoplib/services/notion/database.py
+-rw-r--r--   0        0        0     1908 2023-07-12 22:35:57.809104 gdshoplib-2.0.1/gdshoplib/services/notion/manager.py
+-rw-r--r--   0        0        0     2531 2023-05-24 11:47:55.273029 gdshoplib-2.0.1/gdshoplib/services/notion/models/props.py
+-rw-r--r--   0        0        0     4027 2023-06-15 16:00:30.490577 gdshoplib-2.0.1/gdshoplib/services/notion/notion.py
+-rw-r--r--   0        0        0    10019 2023-07-12 22:35:57.783869 gdshoplib-2.0.1/gdshoplib/services/notion/page.py
+-rw-r--r--   0        0        0     2893 2023-05-24 11:47:55.277301 gdshoplib-2.0.1/gdshoplib/services/vk/market.py
+-rw-r--r--   0        0        0     1825 2023-05-24 11:47:55.278048 gdshoplib-2.0.1/gdshoplib/services/vk/media.py
+-rw-r--r--   0        0        0      986 2023-05-24 11:47:55.282128 gdshoplib-2.0.1/gdshoplib/services/vk/page.py
+-rw-r--r--   0        0        0     2596 2023-05-24 11:47:55.285739 gdshoplib-2.0.1/gdshoplib/services/vk/stats.py
+-rw-r--r--   0        0        0     2880 2023-05-24 11:47:58.644858 gdshoplib-2.0.1/gdshoplib/services/vk/stories.py
+-rw-r--r--   0        0        0     2433 2023-07-12 22:35:57.881523 gdshoplib-2.0.1/gdshoplib/services/vk/vk.py
+-rw-r--r--   0        0        0      104 2023-05-24 11:47:55.290271 gdshoplib-2.0.1/gdshoplib/services/ym/ym.py
+-rw-r--r--   0        0        0      990 2023-07-09 23:40:49.720503 gdshoplib-2.0.1/gdshoplib/templates/basic.txt
+-rw-r--r--   0        0        0      447 2023-05-24 11:47:55.298840 gdshoplib-2.0.1/gdshoplib/templates/instagram.txt
+-rw-r--r--   0        0        0      990 2023-05-24 11:47:55.301319 gdshoplib-2.0.1/gdshoplib/templates/order_info.txt
+-rw-r--r--   0        0        0      989 2023-05-24 11:47:55.305236 gdshoplib-2.0.1/gdshoplib/templates/ula.txt
+-rw-r--r--   0        0        0     1052 2023-05-24 11:47:55.308271 gdshoplib-2.0.1/gdshoplib/templates/vk.txt
+-rw-r--r--   0        0        0      470 2023-05-30 21:41:48.464779 gdshoplib-2.0.1/gdshoplib/workflows/notion.py
+-rw-r--r--   0        0        0     1625 2023-07-12 22:21:48.070153 gdshoplib-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3812 1970-01-01 00:00:00.000000 gdshoplib-2.0.1/PKG-INFO
```

### Comparing `gdshoplib-1.9.0/README.md` & `gdshoplib-2.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 - [ ] Информация о состоянии счетов
 - [ ] Операций с финансами
 - [ ] Статистика по финансам за периоды + Прогнозы
 - [ ] Расчет и контроль бюджетов
 - [ ] Сбор информации с площадок по финансам
 - [ ] Генерация отчетов
-- [x] Генерация цен по коэфицентам
+- [x] Балловый метод ценообразования
 
 ## Marketing
 
 - [ ] Статистика рекламных компаний
 - [ ] Управление рекламными компаниями
 - [ ] Статистика воронок
 - [ ] Выгрузка информации с площадок
@@ -39,8 +39,18 @@
 
 
 # Полезные ссылки
 
 ## Описание товарного фида
 
 https://yandex.ru/support/partnermarket/export/yml.html
-https://drive.google.com/file/d/1kkKa0KU7iNOszyC2oQSGmHNwp3sRGKFb/view
+https://drive.google.com/file/d/1kkKa0KU7iNOszyC2oQSGmHNwp3sRGKFb/view
+
+
+# FAQ
+
+ImportError: Unable to find zbar shared library
+
+```
+mkdir ~/lib
+ln -s $(brew --prefix zbar)/lib/libzbar.dylib ~/lib/libzbar.dylib
+```
```

### Comparing `gdshoplib-1.9.0/gdshoplib/apps/platforms/avito.py` & `gdshoplib-2.0.1/gdshoplib/apps/platforms/avito.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 from lxml import etree, objectify
 
-from gdshoplib.apps.platforms.base import BasePlatformManager
+from gdshoplib.apps.platforms.base import Platform
 from gdshoplib.packages.feed import Feed
 
 
-class AvitoManager(BasePlatformManager, Feed):
+class AvitoManager(Platform, Feed):
     KEY = "AVITO"
 
     def get_root(self):
         root = etree.Element("Ads")
         objectify.deannotate(root, cleanup_namespaces=True, xsi_nil=True)
         root.attrib["target"] = "Avito"
         root.attrib["formatVersion"] = "3"
         return root
 
     def get_offer(self, product):
         appt = objectify.Element("Ad")
         appt.Id = product.sku
         appt.Title = product.name
         appt.Category = self.feed_settings.AVITO_CATEGORY
+        appt.ListingFee = "Package"
+        appt.AdStatus = "Free"
+        appt.ContactMethod = "По телефону и в сообщениях"
         appt.Condition = "Новое"
         appt.Description = product.description.render(self)
         appt.Address = self.feed_settings.ADDRESS
         appt.Price = product.price.now
         appt.ManagerName = self.feed_settings.MANAGER_NAME
         appt.ContactPhone = self.feed_settings.PHONE
+        appt.Stock = product.quantity
 
         images = objectify.Element("Images")
         for image in product.images:
             i = objectify.Element("Image")
-            i.attrib["url"] = image.get_url()
+            i.attrib["url"] = self.get_media_url(image)
             images.append(i)
 
         appt.append(images)
 
         objectify.deannotate(appt, cleanup_namespaces=True, xsi_nil=True)
         return appt
 
-    def get_feed(self, products):
-        for product in products:
+    def get_feed(self):
+        for product in self.products:
             self.root.append(self.get_offer(product))
+
         return etree.tostring(
             self.root,
             pretty_print=True,
             encoding="utf-8",
             xml_declaration=True,
             standalone=True,
         )
```

### Comparing `gdshoplib-1.9.0/gdshoplib/apps/platforms/ula.py` & `gdshoplib-2.0.1/gdshoplib/apps/platforms/ula.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from lxml import objectify
 
-from gdshoplib.apps.platforms.base import BasePlatformManager
+from gdshoplib.apps.platforms.base import Platform
 from gdshoplib.packages.feed import Feed
 
 
-class UlaManager(BasePlatformManager, Feed):
+class UlaManager(Platform):  # , Feed):
     DESCRIPTION_TEMPLATE = "ula.txt"
     KEY = "ULA"
 
     def get_shop(self):
         shop = objectify.Element("shop")
         objectify.deannotate(shop, cleanup_namespaces=True, xsi_nil=True)
```

### Comparing `gdshoplib-1.9.0/gdshoplib/apps/product.py` & `gdshoplib-2.0.1/gdshoplib/apps/products/product.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 from random import randrange
 
 from gdshoplib.apps.products.description import ProductDescription
 from gdshoplib.apps.products.media import ProductMedia
 from gdshoplib.apps.products.price import Price
 from gdshoplib.core.settings import ProductSettings
+from gdshoplib.packages.barcode_pack import Barcode
 from gdshoplib.services.notion.database import Database
 from gdshoplib.services.notion.page import Page
 
 
 class Product(Page):
     SETTINGS = ProductSettings()
 
@@ -49,14 +50,21 @@
     def query(cls, filter=None, params=None, notion=None):
         for page in Database(cls.SETTINGS.PRODUCT_DB, notion=notion).pages(
             filter=filter, params=params
         ):
             yield cls(page["id"], notion=page.notion, parent=page.parent)
 
     @property
+    def barcode(self):
+        if self.barcode_code_field:
+            return Barcode(self.barcode_code_field)
+        if self.barcode_image_field:
+            return Barcode.read(self.barcode_image_field.image)
+
+    @property
     def media(self):
         return [*self.images, *self.videos]
 
     @property
     def videos(self):
         if not self._videos:
             self._videos = list(
@@ -129,29 +137,38 @@
                 if self.id != page.id:
                     self._kit.append(
                         Product(page.id, notion=self.notion, parent=self.parent)
                     )
         return self._kit
 
     @property
+    def platforms(self):
+        # Получить платформы из фида и вернуть объект класса <Platform>
+        ...
+
+    @property
     def badges(self):
         if not self.badge_field:
             return
 
         if not self._badges:
             self._badges = []
             for page in self.badge_field:
                 if self.id != page.id:
                     self._badges.append(
                         Page(page.id, notion=self.notion, parent=self.parent)
                     )
         return self._badges
 
     def available(self):
-        return bool(self.quantity)
+        return bool(
+            self.quantity
+            and self.status_publication == "Публикация"
+            and self.status_description == "Готово"
+        )
 
     def generate_sku(self):
         # Сгенерировать SKU на основе продукта
         # Категория.Бренд.Цена_покупки.месяц_добавления.год_добавления.случайные_4_числа
 
         sku = (
             f"{self.brand.title.upper() if self.brand else ''}"
@@ -163,11 +180,22 @@
 
     def __str__(self) -> str:
         return f"{self.__class__}: {self.sku}"
 
     def __repr__(self) -> str:
         return f"{self.__class__}: {self.sku}"
 
+    def warm(self):
+        self.price.now
+        self.kit
+        self.notes
+        self.specifications
+        self.tags
+        self.media
+        self.description
+        self.brand.title
+        self.description.warm_description_blocks()
+
 
 class SKUDuplicate(Exception):
     # Если найден товар с одинаковым SKU
     ...
```

### Comparing `gdshoplib-1.9.0/gdshoplib/apps/products/description.py` & `gdshoplib-2.0.1/gdshoplib/apps/products/description.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.9.0/gdshoplib/core/settings.py` & `gdshoplib-2.0.1/gdshoplib/core/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     MONTH_SALE_RATE: int = 9
     TURNOVER_RATE: int = 5
 
 
 class NotionSettings(BaseSettings):
     NOTION_SECRET_TOKEN: str
     CACHE_ENABLED: bool = True
+    KAFKA_BROKER: Optional[str]
+    KAFKA_TOPIC: Optional[str] = "notion"
 
 
 class FeedSettings(BaseSettings):
     PHONE: str = "+7 499 384 44 03"
     ADDRESS: str = "Москва, ул. Крупской, 4к1"
     MANAGER_NAME: str = "Менеджер магазина"
     SHOP_NAME: str = "Grey Dream Horse Shop (Конный магазин)"
@@ -42,38 +44,42 @@
     CACHE_DSN: Optional[str]
     CACHE_HSTORE: str = "notion"
     CACHE_SYSTEM_HSTORE: str = "gdshoplib"
 
 
 class ProductSettings(BaseSettings):
     PRODUCT_DB: str = "2d1707fb-877d-4d83-8ae6-3c3d00ff5091"
+    CATEGORY_DB: str = "df41f1da-bb07-414c-ab64-b8928643f6ce"
+
+
+class CRMSettings(BaseSettings):
+    CRM_DB: str = "19cd70dd-a78e-46e1-848e-482ecc76d2fd"
 
 
 class PriceSettins(BaseSettings):
     # Базовые коэфиценты цены
     PRICE_VAT_RATIO: float = 0.16
     PRICE_NEITRAL_RATIO: float = 0.40
     PRICE_PROFIT_RATIO: float = 0.60
-    EURO_PRICE: int = 72
+    EURO_PRICE: int = 102
 
 
 class RecurrentCommonExpenseSettings(BaseSettings):
     # Общие месячные расходы
-    CLOUD_HOSTING_MONTH: int = 2400
-    PLATFORMS_MONTH: int = 2000
+    CLOUD_HOSTING_MONTH: int = 300
     AD_MONTH: int = 3000  # Рассход на общие рекламные компании
 
     def all(self):
         return sum([self.CLOUD_HOSTING_MONTH, self.PLATFORMS_MONTH, self.AD_MONTH])
 
 
 class RecurrentSKUExpenseSettings(BaseSettings):
     # Расходы на каждую товарную позицию
     AVITO_SKU_PRICE: int = (
-        2495 / 83
+        4495 / 83
     )  # (общее количество затрат на просмотры в месяц) / (количество товаров)
     ULA_SKU_PRICE: int = 20
     PACKING_PRICE: int = 20
 
     def all(self):
         return sum([self.AVITO_SKU_PRICE, self.ULA_SKU_PRICE])
 
@@ -95,15 +101,22 @@
 
 
 class VKSettings(BaseSettings):
     VK_BASEPATH: str = "https://api.vk.com/method/"
     VK_API_VERSION: str = "5.131"
     VK_GROUP_ID: str = "215870481"
     VK_CLIENT_ID: str = "51521300"
-    VK_USER_SCOPE: str = "notify,friends,photos,audio,video,stories,pages,status,notes,wall,ads,offline,docs,groups,notifications,stats,email,market"
+    VK_USER_SCOPE: str = "notify,friends,photos,audio,video,stories,pages,status,notes,wall,ads,offline,docs,groups,\
+notifications,stats,email,market"
     VK_SECRET_KEY: Optional[str]
     VK_USER_ACCESS_TOKEN: Optional[str]
+    VK_CATEGORY_ID: int = 1006
 
 
 class AVITOSettings(BaseSettings):
     AVITO_CLIENT_ID: str = "PjsDDbv2OD294pmW1aak"
     AVITO_SECRET: str
+    AVITO_USER_ID: int = 337375
+
+
+class EcosystemSettings(BaseSettings):
+    TEMPORAL_URL: str = "10.10.0.6:7233"
```

### Comparing `gdshoplib-1.9.0/gdshoplib/packages/cache.py` & `gdshoplib-2.0.1/gdshoplib/packages/cache.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 import re
+import time
 
 import orjson as json
 import redis
 
 from gdshoplib.core.settings import CacheSettings
 
 
@@ -19,29 +20,56 @@
 class KeyDBCache(BaseCache):
     CONNECT = None
 
     def __init__(self, namespace=None):
         self.settings = CacheSettings()
         self.namespace = namespace or self.settings.CACHE_HSTORE
         self.system_namespace = self.settings.CACHE_SYSTEM_HSTORE
+        self._update_time = None
+
+    def subscribe(self, topic):
+        p = self.connect.pubsub()
+        try:
+            p.subscribe(topic)
+            while True:
+                message = p.get_message()
+                if message:
+                    yield json.loads(str(message["data"]))
+                time.sleep(0.001)
+        finally:
+            p.close()
+
+    def publish(self, topic, value):
+        self.connect.publish(topic, json.dumps(value))
 
     @staticmethod
     def update_time_key(id, /, type):
         return f"{type}:{id}_update_time"
 
+    def set_update_start(self):
+        self._update_time = datetime.datetime.now(datetime.timezone.utc)
+
+    def clean_update(self):
+        self._update_time = None
+
+    @property
+    def update_time(self):
+        if self._update_time:
+            return self._update_time
+        return datetime.datetime.now(datetime.timezone.utc)
+
     def get_update_time(self, id, /, type):
         value = self.connect.hget(
             self.settings.CACHE_SYSTEM_HSTORE, self.update_time_key(id, type)
         )
         if value:
             return json.loads(value)
 
     def set_update_time(self, id, /, type):
-        now = datetime.datetime.now(datetime.timezone.utc)
-        content = json.dumps(now)
+        content = json.dumps(self.update_time)
         self.connect.hset(
             self.settings.CACHE_SYSTEM_HSTORE, self.update_time_key(id, type), content
         )
 
     def clean_system_cache(self):
         self.connect.delete(self.settings.CACHE_SYSTEM_HSTORE)
```

### Comparing `gdshoplib-1.9.0/gdshoplib/packages/feed.py` & `gdshoplib-2.0.1/gdshoplib/apps/platforms/yam.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,92 @@
-import datetime
+import re
 
 from lxml import etree, objectify
 
-from gdshoplib.core.settings import FeedSettings
-
-
-class Feed:
-    DESCRIPTION_TEMPLATE = "basic.txt"
-
-    def __init__(self):
-        self.feed_settings = FeedSettings()
-        self.root = self.get_root()
-
-    def get_root(self):
-        root = etree.Element("yml_catalog")
-        objectify.deannotate(root, cleanup_namespaces=True, xsi_nil=True)
-        root.attrib["date"] = str(datetime.datetime.now())
-        return root
+from gdshoplib.apps.platforms.base import Platform
+from gdshoplib.core.settings import ProductSettings
+from gdshoplib.packages.feed import Feed
+from gdshoplib.services.notion.database import Database
+
+
+class YandexMarketManager(Platform, Feed):
+    KEY = "YAM"
+
+    def get_categories(self):
+        categories = Database(ProductSettings().CATEGORY_DB).pages()
+        return [(self.fetch_id(i.id), i.title) for i in categories]
+
+    @staticmethod
+    def fetch_id(id):
+        return str(sum([int(i) for i in re.sub(r"\D*", "", id)]))
+
+    @property
+    def product_filter(self):
+        return dict(status_description="Готово", status_publication="Публикация")
 
     def get_shop(self):
         shop = objectify.Element("shop")
 
         shop.name = self.feed_settings.SHOP_NAME
         shop.company = self.feed_settings.COMPANY_NAME
         shop.url = self.feed_settings.SHOP_URL
+
         currencies = objectify.Element("currencies")
         currency = etree.Element("currency")
         currency.attrib["id"] = "RUB"
         currency.attrib["rate"] = "1"
         objectify.deannotate(currency, cleanup_namespaces=True, xsi_nil=True)
         objectify.deannotate(currencies, cleanup_namespaces=True, xsi_nil=True)
         currencies.append(currency)
         shop.currencies = currencies
+
+        categories = objectify.Element("categories")
+        for ind, k in enumerate(
+            ["Все товары", "Спорт и отдых", "Конный спорт"], start=1
+        ):
+            category = etree.Element("category")
+            category.attrib["id"] = str(ind)
+            if ind - 1 != 0:
+                category.attrib["parentId"] = str(ind - 1)
+            category.text = k
+            categories.append(category)
+
+        for _id, name in self.get_categories():
+            category = etree.Element("category")
+            category.attrib["id"] = _id
+            category.attrib["parentId"] = "3"
+            category.text = name
+            objectify.deannotate(category, cleanup_namespaces=True, xsi_nil=True)
+            categories.append(category)
+
+        shop.categories = categories
         objectify.deannotate(shop, cleanup_namespaces=True, xsi_nil=True)
 
         return shop
 
-    def get_offers(self, products):
-        offers = etree.Element("offers")
-        objectify.deannotate(offers, cleanup_namespaces=True, xsi_nil=True)
-        for product in products:
-            offers.append(self.get_offer(product))
-
-        return offers
-
-    @classmethod
-    def get_old_price(cls, product):
-        if (
-            product.price.now <= product.price.profit / 1.05
-        ):  # Старую цену можно указывать, только если разница больше 5%
-            return product.price.profit
-
     def get_offer(self, product):
         appt = objectify.Element("offer")
         appt.attrib["id"] = product.sku
-        appt.attrib["available"] = str(product.available()).lower()
+        appt.count = product.quantity
+        if product.quantity == 0:
+            appt.attrib["type"] = "on.demand"
+
         appt.currencyId = "RUB"
         appt.price = product.price.now
-        appt.title = product.name
-        appt.name = product.name
-        appt.vendor = product.brand.title
-        appt.delivery = "true"
-        appt.description = product.description.generate(self)
-
         if self.get_old_price(product):
             appt.oldprice = self.get_old_price(product)
 
         for image in product.images:
-            appt.addattr("picture", image.get_url())
+            appt.addattr("picture", self.get_media_url(image))
+
+        appt.name = product.name
+        appt.description = product.description.generate(self)
+        appt.vendor = product.brand.title
+        appt.categoryId = self.fetch_id(product.categories[0].id)
+        appt.barcode = product.barcode.code if product.barcode else 0
+        appt.dimensions = (
+            product.dimensions if product.dimensions else "0/0/0"
+        )  # Длина, ширина, высота в упаковке.
+        appt.weight = product.weight if product.weight else 0
 
         objectify.deannotate(appt, cleanup_namespaces=True, xsi_nil=True)
         return appt
-
-    def get_feed(self, products):
-        shop = self.get_shop()
-        shop.append(self.get_offers(products))
-        self.root.append(shop)
-        return etree.tostring(
-            self.root,
-            pretty_print=True,
-            encoding="utf-8",
-            xml_declaration=True,
-            standalone=True,
-        )
```

### Comparing `gdshoplib-1.9.0/gdshoplib/packages/lang.py` & `gdshoplib-2.0.1/gdshoplib/packages/lang.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.9.0/gdshoplib/packages/s3.py` & `gdshoplib-2.0.1/gdshoplib/services/notion/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,68 @@
-import boto3
-from botocore.exceptions import ClientError
+from gdshoplib.services.notion.notion import Notion
 
-from gdshoplib.core.settings import S3Settings
 
+class BasePage:
+    def __init__(self, id, *, notion=None, parent=None):
+        self.properties = None
+        self.id = id
+        self.notion = notion or Notion()
+        self.parent = parent
+        self.history = {}
+        self.change_log = {}
+        self.initialize()
 
-class S3:
-    def __init__(self, data):
-        self.data = data
-        self.content = None
-        self.s3_settings = S3Settings()
-        self.__session = None
-        self.__client = None
-
-    @property
-    def session(self):
-        if not self.__session:
-            self.__session = boto3.session.Session()
-
-        return self.__session
-
-    @property
-    def s3(self):
-        if not self.__client:
-            self.__client = self.session.client(
-                service_name="s3",
-                endpoint_url=self.s3_settings.ENDPOINT_URL,
-                aws_access_key_id=self.s3_settings.ACCESS_KEY,
-                aws_secret_access_key=self.s3_settings.SECRET_KEY,
-            )
-        return self.__client
-
-    def put(self):
-        return self.s3.put_object(
-            Bucket=self.s3_settings.BUCKET_NAME,
-            Key=self.data.file_key,
-            Body=self.data.content,
-            ACL="public-read",
-            StorageClass="COLD",
-            ContentType=self.data.mime,
-        )
+    def initialize(self):
+        self.page = self.get_source()
 
-    def exists(self):
-        try:
-            self.s3.head_object(
-                Bucket=self.s3_settings.BUCKET_NAME, Key=self.data.file_key
-            )
-        except ClientError:
-            return False
-        else:
-            return True
+    def get_source(self):
+        return self.notion.get_page(self.id)
+
+    def __str__(self) -> str:
+        return f"{self.__class__}: {self.id}"
+
+    def __repr__(self) -> str:
+        return f"{self.__class__}: {self.id}"
 
-    def get(self):
+    def __getitem__(self, key):
         try:
-            return self.s3.get_object(
-                Bucket=self.s3_settings.BUCKET_NAME, Key=self.data.file_key
-            )
-        except ClientError as ex:
-            if ex.response["Error"]["Code"] == "NoSuchKey":
-                return None
-            raise ex
-
-    def delete(self):
-        return self.s3.delete_object(
-            Bucket=self.s3_settings.BUCKET_NAME, Key=self.data.file_key
-        )
+            return super(BasePage, self).__getattribute__(key)
+        except AttributeError:
+            return self.__getattr__(key)
+
+    def __getattr__(self, name: str):
+        if self.page and name in self.page.keys():
+            return self.page[name]
+
+        if self.properties:
+            return self.properties[name]
+
+        raise AttributeError
+
+    def __enter__(self):
+        self.notion.cache.set_update_start()
+        return self
+
+    def __exit__(self, exc_type, exc_value, exc_tb):
+        if not exc_type:
+            self.set_update_time()
+        self.notion.cache.clean_update()
+
+    def get_update_time(self):
+        return self.notion.cache.get_update_time(self.id, type=self.__class__.__name__)
+
+    def set_update_time(self):
+        return self.notion.cache.set_update_time(self.id, type=self.__class__.__name__)
+
+    def edited_filter(self):
+        update_time = self.get_update_time()
+        if not update_time:
+            return None
+        return {
+            "filter": {
+                "timestamp": "last_edited_time",
+                "last_edited_time": {"after": update_time},
+            },
+            "sorts": [
+                {"direction": "ascending", "timestamp": "last_edited_time"},
+            ],
+        }
```

### Comparing `gdshoplib-1.9.0/gdshoplib/services/notion/README.md` & `gdshoplib-2.0.1/gdshoplib/services/notion/README.md`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.9.0/gdshoplib/services/notion/block.py` & `gdshoplib-2.0.1/gdshoplib/services/notion/block.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.9.0/gdshoplib/services/notion/database.py` & `gdshoplib-2.0.1/gdshoplib/services/notion/database.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-1.9.0/gdshoplib/services/notion/manager.py` & `gdshoplib-2.0.1/gdshoplib/services/notion/manager.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,75 @@
 import logging
 
+import backoff
+
 import requests as r
 
 logger = logging.getLogger(__name__)
 
 
 class RequestManager:
     BASE_URL = "https://api.notion.com/v1/"
 
+    @backoff.on_exception(
+        backoff.expo,
+        (
+            r.ReadTimeout,
+            r.ConnectTimeout,
+            r.Timeout,
+            r.JSONDecodeError,
+            r.ConnectionError,
+            r.HTTPError,
+        ),
+        max_tries=8,
+    )
     def make_request(self, path, *, method, params=None):
         _path = f"{self.BASE_URL}{path}"
         _params = (
             dict(params=params) or {}
             if method.upper() == "GET"
             else dict(json=params) or {}
         )
 
         _r = r.request(
             method,
             _path,
             headers=self.get_headers(),
+            timeout=10.0,
             **_params,
         )
-        if not _r.ok:
-            logger.warning(_r.json())
-            if _r.status_code == 404:
-                raise NotFoundException
-            assert (
-                False
-            ), f"Запрос {method.upper()} {_path} прошел с ошибкой {_r.status_code}/n"
+        if _r.status_code == 404:
+            raise NotFoundException
+
+        try:
+            _r.raise_for_status()
+        except Exception as e:
+            logger.exception(e)
+            raise e
         return _r.json()
 
     def pagination(self, url, *, params=None, **kwargs):
         _params = params or {}
         response = None
         result = []
         while True:
             response = self.make_request(url, params=_params, **kwargs)
             result.extend(response["results"])
 
             if not response.get("has_more"):
                 return result
             _params["start_cursor"] = response["next_cursor"]
 
+    def pagination_iterator(self, url, *, params=None, **kwargs):
+        _params = params or {}
+        while True:
+            response = self.make_request(url, params=_params, **kwargs)
+            result = response["results"]
+            yield from result
+
+            if not response.get("has_more"):
+                return
+            _params["start_cursor"] = response["next_cursor"]
+
 
 class NotFoundException(Exception):
     ...
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gdshoplib-1.9.0/gdshoplib/services/vk/vk.py` & `gdshoplib-2.0.1/gdshoplib/services/vk/vk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 import webbrowser
 
 import requests
-
 from gdshoplib.core.settings import VKSettings
 
 logger = logging.getLogger(__name__)
 
 
 class VKNotFoundException(Exception):
     ...
@@ -15,22 +14,24 @@
 class VK:
     def __init__(self):
         self.settings = VKSettings()
 
     def auth_headers(self):
         return {"Authorization": f"Bearer {self.settings.VK_USER_ACCESS_TOKEN}"}
 
-    def request(self, method, params=None):
+    def request(self, method, params=None, url=None, http_method=None, files=None):
         _params = {"v": self.settings.VK_API_VERSION}
         _params.update(params or {})
 
-        r = requests.get(
-            f"{self.settings.VK_BASEPATH}{method}",
+        r = requests.request(
+            http_method or "get",
+            url or f"{self.settings.VK_BASEPATH}{method}",
             params=_params,
             headers=self.auth_headers(),
+            files=files or {},
         )
 
         if not r.ok:
             logger.warning(r.json())
             if r.status_code == 404:
                 raise VKNotFoundException
```

### Comparing `gdshoplib-1.9.0/gdshoplib/templates/basic.txt` & `gdshoplib-2.0.1/gdshoplib/templates/basic.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 {% if product.quantity == 0 %}📦 Под заказ 📦
 
-{% endif %}{{ product.name }}{% if product.price.current_discount and product.quantity > 0 %}
+{% endif %}{{ product.name }}{% if product.price.current_discount and product.quantity > 0 and product.price.current_discount > 4 %}
 Цена указана со скидкой: {{ product.price.current_discount }}% {% endif %}
 
 {% if product.brand %}Бренд: {{product.brand.title}}{% endif %}{% if product.collection %}
 Коллекция: {{product.collection}}{% endif %}{% if product.size %}
 Размер: {{product.size}}{% endif %}{% if product.color %}
 Цвет: {{product.color}}{% endif %}
 
 {% if product.short_description %}{{product.short_description}}{% endif %}
 {% if product.specifications %}{% for material in product.specifications %}
-- {{material}}{% endfor %}{% endif %}
+- {{material}}{% endfor %}{% endif %}{% if product.notes %}{% for note in product.notes %}
+- {{note}}{% endfor %}{% endif %}
 
 Доставка в любой город России
 Местонахождение магазина, Москва
 
-Бесплатная доставка — для подписчиков любого из наших сообществ
-Скидка 10% — При покупке больше 30к
-
 Артикул: {{product.sku}}
```

### Comparing `gdshoplib-1.9.0/gdshoplib/templates/ula.txt` & `gdshoplib-2.0.1/gdshoplib/templates/ula.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 {% if product.quantity == 0 %}📦 Под заказ 📦
-{% endif %}{{ product.name }}{% if product.price.current_discount and product.quantity > 0 %}
+{% endif %}{{ product.name }}{% if product.price.current_discount and product.quantity > 0 and product.price.current_discount > 4 %}
 Цена указана со скидкой: {{ product.price.current_discount }}% {% endif %}
 
 {% if product.brand %}Бренд: {{product.brand.title}}{% endif %}{% if product.collection %}
 Коллекция: {{product.collection}}{% endif %}{% if product.size %}
 Размер: {{product.size}}{% endif %}{% if product.color %}
 Цвет: {{product.color}}{% endif %}
 
 {% if product.short_description %}{{product.short_description}}{% endif %}
 {% if product.specifications %}{% for material in product.specifications %}
-- {{material}}{% endfor %}{% endif %}
+- {{material}}{% endfor %}{% endif %}{% if product.notes %}{% for note in product.notes %}
+- {{note}}{% endfor %}{% endif %}
 
 Доставка в любой город России
 Местонахождение магазина, Москва
 
-Бесплатная доставка — для подписчиков любого из наших сообществ
-Скидка 10% — При покупке больше 30к
-
 Артикул: {{product.sku}}
```

### Comparing `gdshoplib-1.9.0/gdshoplib/templates/vk.txt` & `gdshoplib-2.0.1/gdshoplib/templates/order_info.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 {% if product.quantity == 0 %}📦 Под заказ 📦
-{% endif %}{{ product.name }}{% if product.price.current_discount and product.quantity > 0 %}
+
+{% endif %}{{ product.name }}{% if product.price.current_discount and product.quantity > 0 and product.price.current_discount > 4 %}
 Цена указана со скидкой: {{ product.price.current_discount }}% {% endif %}
 
 {% if product.brand %}Бренд: {{product.brand.title}}{% endif %}{% if product.collection %}
 Коллекция: {{product.collection}}{% endif %}{% if product.size %}
 Размер: {{product.size}}{% endif %}{% if product.color %}
 Цвет: {{product.color}}{% endif %}
 
 {% if product.short_description %}{{product.short_description}}{% endif %}
 {% if product.specifications %}{% for material in product.specifications %}
-- {{material}}{% endfor %}{% endif %}
+- {{material}}{% endfor %}{% endif %}{% if product.notes %}{% for note in product.notes %}
+- {{note}}{% endfor %}{% endif %}
 
 Доставка в любой город России
 Местонахождение магазина, Москва
 
-Бесплатная доставка — для подписчиков любого из наших сообществ
-Скидка 10% — При покупке больше 30к
-
-{% if product.short_description %}
-{% for tag in product.tags %}#{{tag}} {% endfor %}{%endif%}
+Артикул: {{product.sku}}
```

### Comparing `gdshoplib-1.9.0/pyproject.toml` & `gdshoplib-2.0.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gdshoplib"
-version = "1.9.0"
+version = "2.0.1"
 description = ""
 authors = ["Nikolay Baryshnikov <root@k0d.ru>"]
 packages=[
     { include = "gdshoplib" },
 ]
 license="MIT"
 readme="README.md"
@@ -13,17 +13,14 @@
 classifiers=[
     "License :: OSI Approved :: MIT License",
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Natural Language :: Russian",
     "Natural Language :: English",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.scripts]
 gdshoplib = "gdshoplib:application"
 
 [tool.poetry.dependencies]
@@ -38,22 +35,36 @@
 isort = "^5.10.1"
 lxml = "^4.9.1"
 redis = "^4.3.5"
 orjson = "^3.8.3"
 boto3 = "^1.26.32"
 python-magic = "^0.4.27"
 python-dateutil = "^2.8.2"
+validators = "^0.20.0"
+backoff = "^2.2.1"
+loguru = "^0.6.0"
+numpy = "^1.24.2"
+qrcode = {version = "^7.4.2", extras = ["pil"]}
+python-barcode = "^0.14.0"
+pyzbar = "^0.1.9"
+opencv-python = "^4.7.0.72"
+kafka-python = "^2.0.2"
+msgpack = "^1.0.5"
+ujson = "^5.7.0"
+temporalio = "^1.2.0"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^5.0.4"
 pytest = "^7.2.0"
 pytest-mock = "^3.10.0"
 pytest-cov = "^4.0.0"
 black = "^22.10.0"
 snakeviz = "^2.1.1"
 pytest-profiling = "^1.7.0"
+pytest-lazy-fixture = "^0.6.3"
+ipykernel = "^6.20.1"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

