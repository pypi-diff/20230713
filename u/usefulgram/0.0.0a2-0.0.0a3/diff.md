# Comparing `tmp/usefulgram-0.0.0a2.tar.gz` & `tmp/usefulgram-0.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usefulgram-0.0.0a2.tar", max compression
+gzip compressed data, was "usefulgram-0.0.0a3.tar", max compression
```

## Comparing `usefulgram-0.0.0a2.tar` & `usefulgram-0.0.0a3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1077 2023-07-07 20:49:54.066720 usefulgram-0.0.0a2/LICENSE
--rw-r--r--   0        0        0      735 2023-07-12 21:35:49.321894 usefulgram-0.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     2252 2023-07-07 21:36:03.207522 usefulgram-0.0.0a2/README.md
--rw-r--r--   0        0        0      145 2023-07-12 21:22:14.352712 usefulgram-0.0.0a2/usefulgram/__init__.py
--rw-r--r--   0        0        0       30 2023-07-07 21:21:58.969929 usefulgram-0.0.0a2/usefulgram/const/__init__.py
--rw-r--r--   0        0        0      192 2023-06-18 20:21:06.663801 usefulgram-0.0.0a2/usefulgram/const/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      207 2023-07-12 20:52:05.669860 usefulgram-0.0.0a2/usefulgram/const/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      626 2023-06-25 23:36:03.804852 usefulgram-0.0.0a2/usefulgram/const/__pycache__/const.cpython-310.pyc
--rw-r--r--   0        0        0      825 2023-07-12 20:52:05.670858 usefulgram-0.0.0a2/usefulgram/const/__pycache__/const.cpython-311.pyc
--rw-r--r--   0        0        0      300 2023-06-25 20:25:25.579092 usefulgram-0.0.0a2/usefulgram/const/const.py
--rw-r--r--   0        0        0      170 2023-07-07 21:21:58.932059 usefulgram-0.0.0a2/usefulgram/exceptions/__init__.py
--rw-r--r--   0        0        0      348 2023-06-19 16:50:03.414405 usefulgram-0.0.0a2/usefulgram/exceptions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      412 2023-07-12 20:52:05.683100 usefulgram-0.0.0a2/usefulgram/exceptions/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      525 2023-06-19 16:50:03.415402 usefulgram-0.0.0a2/usefulgram/exceptions/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0      697 2023-07-12 20:52:05.686587 usefulgram-0.0.0a2/usefulgram/exceptions/__pycache__/exceptions.cpython-311.pyc
--rw-r--r--   0        0        0      457 2023-06-19 16:49:59.041300 usefulgram-0.0.0a2/usefulgram/exceptions/exceptions.py
--rw-r--r--   0        0        0      168 2023-07-07 21:21:58.956995 usefulgram-0.0.0a2/usefulgram/filters/__init__.py
--rw-r--r--   0        0        0      400 2023-07-12 20:52:05.690132 usefulgram-0.0.0a2/usefulgram/filters/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1796 2023-07-12 20:52:05.694121 usefulgram-0.0.0a2/usefulgram/filters/__pycache__/database_filters.cpython-311.pyc
--rw-r--r--   0        0        0     6545 2023-07-12 20:52:05.692126 usefulgram-0.0.0a2/usefulgram/filters/__pycache__/parse_filters.cpython-311.pyc
--rw-r--r--   0        0        0      784 2023-06-25 19:32:18.676643 usefulgram-0.0.0a2/usefulgram/filters/database_filters.py
--rw-r--r--   0        0        0     4056 2023-06-25 23:43:09.415451 usefulgram-0.0.0a2/usefulgram/filters/parse_filters.py
--rw-r--r--   0        0        0       60 2023-07-07 21:21:58.951007 usefulgram-0.0.0a2/usefulgram/keyboard/__init__.py
--rw-r--r--   0        0        0      255 2023-07-01 22:52:11.609139 usefulgram-0.0.0a2/usefulgram/keyboard/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      285 2023-07-12 20:52:05.671855 usefulgram-0.0.0a2/usefulgram/keyboard/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4586 2023-07-01 22:56:43.331106 usefulgram-0.0.0a2/usefulgram/keyboard/__pycache__/builder.cpython-310.pyc
--rw-r--r--   0        0        0     7446 2023-07-12 20:52:05.674141 usefulgram-0.0.0a2/usefulgram/keyboard/__pycache__/builder.cpython-311.pyc
--rw-r--r--   0        0        0     4266 2023-07-01 22:56:42.398599 usefulgram-0.0.0a2/usefulgram/keyboard/builder.py
--rw-r--r--   0        0        0       43 2023-07-07 21:21:58.939012 usefulgram-0.0.0a2/usefulgram/lazy/__init__.py
--rw-r--r--   0        0        0      203 2023-06-25 23:40:11.949558 usefulgram-0.0.0a2/usefulgram/lazy/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      219 2023-07-12 20:52:04.890650 usefulgram-0.0.0a2/usefulgram/lazy/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5110 2023-06-25 23:40:11.952550 usefulgram-0.0.0a2/usefulgram/lazy/__pycache__/lazy_editing.cpython-310.pyc
--rw-r--r--   0        0        0     9884 2023-07-12 20:52:04.893360 usefulgram-0.0.0a2/usefulgram/lazy/__pycache__/lazy_editing.cpython-311.pyc
--rw-r--r--   0        0        0     9580 2023-07-07 12:31:08.803453 usefulgram-0.0.0a2/usefulgram/lazy/lazy_editing.py
--rw-r--r--   0        0        0       89 2023-07-07 21:21:58.945022 usefulgram-0.0.0a2/usefulgram/middlewares/__init__.py
--rw-r--r--   0        0        0      297 2023-07-12 20:52:05.696116 usefulgram-0.0.0a2/usefulgram/middlewares/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1802 2023-07-12 20:52:05.697113 usefulgram-0.0.0a2/usefulgram/middlewares/__pycache__/stacker.cpython-311.pyc
--rw-r--r--   0        0        0     2783 2023-07-12 21:24:59.345583 usefulgram-0.0.0a2/usefulgram/middlewares/__pycache__/trottling.cpython-311.pyc
--rw-r--r--   0        0        0      847 2023-06-25 23:39:58.644717 usefulgram-0.0.0a2/usefulgram/middlewares/stacker.py
--rw-r--r--   0        0        0     1505 2023-07-12 21:23:58.601508 usefulgram-0.0.0a2/usefulgram/middlewares/trottling.py
--rw-r--r--   0        0        0       44 2023-07-07 21:21:58.963945 usefulgram-0.0.0a2/usefulgram/parsing/__init__.py
--rw-r--r--   0        0        0      210 2023-07-01 22:52:11.613096 usefulgram-0.0.0a2/usefulgram/parsing/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      223 2023-07-12 20:52:05.678130 usefulgram-0.0.0a2/usefulgram/parsing/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2658 2023-06-25 23:36:03.801859 usefulgram-0.0.0a2/usefulgram/parsing/__pycache__/decode.cpython-310.pyc
--rw-r--r--   0        0        0     4832 2023-07-12 20:52:05.680124 usefulgram-0.0.0a2/usefulgram/parsing/__pycache__/decode.cpython-311.pyc
--rw-r--r--   0        0        0     2676 2023-07-01 22:52:11.616112 usefulgram-0.0.0a2/usefulgram/parsing/__pycache__/encode.cpython-310.pyc
--rw-r--r--   0        0        0     4281 2023-07-12 20:52:05.682127 usefulgram-0.0.0a2/usefulgram/parsing/__pycache__/encode.cpython-311.pyc
--rw-r--r--   0        0        0     2776 2023-06-25 20:24:32.926642 usefulgram-0.0.0a2/usefulgram/parsing/decode.py
--rw-r--r--   0        0        0     2514 2023-06-25 20:24:32.941577 usefulgram-0.0.0a2/usefulgram/parsing/encode.py
--rw-r--r--   0        0        0       52 2023-06-18 09:35:26.952475 usefulgram-0.0.0a2/usefulgram/utils/__init__.py
--rw-r--r--   0        0        0      198 2023-06-18 09:35:27.816247 usefulgram-0.0.0a2/usefulgram/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      230 2023-07-12 20:52:05.687137 usefulgram-0.0.0a2/usefulgram/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      559 2023-06-18 09:36:47.317788 usefulgram-0.0.0a2/usefulgram/utils/__pycache__/autorepr.cpython-310.pyc
--rw-r--r--   0        0        0      909 2023-07-12 20:52:05.689134 usefulgram-0.0.0a2/usefulgram/utils/__pycache__/autorepr.cpython-311.pyc
--rw-r--r--   0        0        0      233 2023-06-18 09:36:46.396163 usefulgram-0.0.0a2/usefulgram/utils/autorepr.py
--rw-r--r--   0        0        0     3093 1970-01-01 00:00:00.000000 usefulgram-0.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-07 20:49:54.066720 usefulgram-0.0.0a3/LICENSE
+-rw-r--r--   0        0        0      735 2023-07-12 23:25:02.804630 usefulgram-0.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0     2252 2023-07-07 21:36:03.207522 usefulgram-0.0.0a3/README.md
+-rw-r--r--   0        0        0      247 2023-07-12 21:45:25.235118 usefulgram-0.0.0a3/usefulgram/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-07 21:21:58.969929 usefulgram-0.0.0a3/usefulgram/enums/__init__.py
+-rw-r--r--   0        0        0      192 2023-06-18 20:21:06.663801 usefulgram-0.0.0a3/usefulgram/enums/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      207 2023-07-12 20:52:05.669860 usefulgram-0.0.0a3/usefulgram/enums/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      626 2023-06-25 23:36:03.804852 usefulgram-0.0.0a3/usefulgram/enums/__pycache__/const.cpython-310.pyc
+-rw-r--r--   0        0        0      825 2023-07-12 20:52:05.670858 usefulgram-0.0.0a3/usefulgram/enums/__pycache__/const.cpython-311.pyc
+-rw-r--r--   0        0        0      300 2023-06-25 20:25:25.579092 usefulgram-0.0.0a3/usefulgram/enums/const.py
+-rw-r--r--   0        0        0      170 2023-07-07 21:21:58.932059 usefulgram-0.0.0a3/usefulgram/exceptions/__init__.py
+-rw-r--r--   0        0        0      348 2023-06-19 16:50:03.414405 usefulgram-0.0.0a3/usefulgram/exceptions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      412 2023-07-12 20:52:05.683100 usefulgram-0.0.0a3/usefulgram/exceptions/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      525 2023-06-19 16:50:03.415402 usefulgram-0.0.0a3/usefulgram/exceptions/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0      697 2023-07-12 20:52:05.686587 usefulgram-0.0.0a3/usefulgram/exceptions/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0      457 2023-06-19 16:49:59.041300 usefulgram-0.0.0a3/usefulgram/exceptions/exceptions.py
+-rw-r--r--   0        0        0      168 2023-07-07 21:21:58.956995 usefulgram-0.0.0a3/usefulgram/filters/__init__.py
+-rw-r--r--   0        0        0      400 2023-07-12 20:52:05.690132 usefulgram-0.0.0a3/usefulgram/filters/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1796 2023-07-12 20:52:05.694121 usefulgram-0.0.0a3/usefulgram/filters/__pycache__/database_filters.cpython-311.pyc
+-rw-r--r--   0        0        0     6545 2023-07-12 23:43:20.285814 usefulgram-0.0.0a3/usefulgram/filters/__pycache__/parse_filters.cpython-311.pyc
+-rw-r--r--   0        0        0      784 2023-06-25 19:32:18.676643 usefulgram-0.0.0a3/usefulgram/filters/database_filters.py
+-rw-r--r--   0        0        0     4056 2023-07-12 23:43:19.426659 usefulgram-0.0.0a3/usefulgram/filters/parse_filters.py
+-rw-r--r--   0        0        0       60 2023-07-07 21:21:58.951007 usefulgram-0.0.0a3/usefulgram/keyboard/__init__.py
+-rw-r--r--   0        0        0      255 2023-07-01 22:52:11.609139 usefulgram-0.0.0a3/usefulgram/keyboard/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      285 2023-07-12 20:52:05.671855 usefulgram-0.0.0a3/usefulgram/keyboard/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4586 2023-07-01 22:56:43.331106 usefulgram-0.0.0a3/usefulgram/keyboard/__pycache__/builder.cpython-310.pyc
+-rw-r--r--   0        0        0     8156 2023-07-12 22:54:24.105242 usefulgram-0.0.0a3/usefulgram/keyboard/__pycache__/builder.cpython-311.pyc
+-rw-r--r--   0        0        0     4836 2023-07-12 22:54:23.162090 usefulgram-0.0.0a3/usefulgram/keyboard/builder.py
+-rw-r--r--   0        0        0       43 2023-07-07 21:21:58.939012 usefulgram-0.0.0a3/usefulgram/lazy/__init__.py
+-rw-r--r--   0        0        0      203 2023-06-25 23:40:11.949558 usefulgram-0.0.0a3/usefulgram/lazy/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      219 2023-07-12 20:52:04.890650 usefulgram-0.0.0a3/usefulgram/lazy/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5110 2023-06-25 23:40:11.952550 usefulgram-0.0.0a3/usefulgram/lazy/__pycache__/lazy_editing.cpython-310.pyc
+-rw-r--r--   0        0        0     9884 2023-07-12 21:45:25.379199 usefulgram-0.0.0a3/usefulgram/lazy/__pycache__/lazy_editing.cpython-311.pyc
+-rw-r--r--   0        0        0     9580 2023-07-12 21:45:25.228138 usefulgram-0.0.0a3/usefulgram/lazy/lazy_editing.py
+-rw-r--r--   0        0        0       89 2023-07-07 21:21:58.945022 usefulgram-0.0.0a3/usefulgram/middlewares/__init__.py
+-rw-r--r--   0        0        0      297 2023-07-12 20:52:05.696116 usefulgram-0.0.0a3/usefulgram/middlewares/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1802 2023-07-12 20:52:05.697113 usefulgram-0.0.0a3/usefulgram/middlewares/__pycache__/stacker.cpython-311.pyc
+-rw-r--r--   0        0        0     2783 2023-07-12 21:45:26.170753 usefulgram-0.0.0a3/usefulgram/middlewares/__pycache__/trottling.cpython-311.pyc
+-rw-r--r--   0        0        0      847 2023-06-25 23:39:58.644717 usefulgram-0.0.0a3/usefulgram/middlewares/stacker.py
+-rw-r--r--   0        0        0     1505 2023-07-12 21:45:25.238959 usefulgram-0.0.0a3/usefulgram/middlewares/trottling.py
+-rw-r--r--   0        0        0       44 2023-07-07 21:21:58.963945 usefulgram-0.0.0a3/usefulgram/parsing/__init__.py
+-rw-r--r--   0        0        0      210 2023-07-01 22:52:11.613096 usefulgram-0.0.0a3/usefulgram/parsing/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      223 2023-07-12 20:52:05.678130 usefulgram-0.0.0a3/usefulgram/parsing/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2658 2023-06-25 23:36:03.801859 usefulgram-0.0.0a3/usefulgram/parsing/__pycache__/decode.cpython-310.pyc
+-rw-r--r--   0        0        0     4860 2023-07-12 23:37:41.723037 usefulgram-0.0.0a3/usefulgram/parsing/__pycache__/decode.cpython-311.pyc
+-rw-r--r--   0        0        0     2676 2023-07-01 22:52:11.616112 usefulgram-0.0.0a3/usefulgram/parsing/__pycache__/encode.cpython-310.pyc
+-rw-r--r--   0        0        0     4281 2023-07-12 21:45:26.163773 usefulgram-0.0.0a3/usefulgram/parsing/__pycache__/encode.cpython-311.pyc
+-rw-r--r--   0        0        0     2803 2023-07-12 23:37:40.829073 usefulgram-0.0.0a3/usefulgram/parsing/decode.py
+-rw-r--r--   0        0        0     2514 2023-07-12 21:45:25.242944 usefulgram-0.0.0a3/usefulgram/parsing/encode.py
+-rw-r--r--   0        0        0       52 2023-06-18 09:35:26.952475 usefulgram-0.0.0a3/usefulgram/utils/__init__.py
+-rw-r--r--   0        0        0      198 2023-06-18 09:35:27.816247 usefulgram-0.0.0a3/usefulgram/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      230 2023-07-12 20:52:05.687137 usefulgram-0.0.0a3/usefulgram/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      559 2023-06-18 09:36:47.317788 usefulgram-0.0.0a3/usefulgram/utils/__pycache__/autorepr.cpython-310.pyc
+-rw-r--r--   0        0        0      909 2023-07-12 20:52:05.689134 usefulgram-0.0.0a3/usefulgram/utils/__pycache__/autorepr.cpython-311.pyc
+-rw-r--r--   0        0        0      233 2023-06-18 09:36:46.396163 usefulgram-0.0.0a3/usefulgram/utils/autorepr.py
+-rw-r--r--   0        0        0     3093 1970-01-01 00:00:00.000000 usefulgram-0.0.0a3/PKG-INFO
```

### Comparing `usefulgram-0.0.0a2/LICENSE` & `usefulgram-0.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a2/pyproject.toml` & `usefulgram-0.0.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "usefulgram"
-version = "0.0.0a2"
+version = "0.0.0a3"
 description = "Like aiogram but more easy"
 license = "MIT"
 authors = ["Alexandr Bortnik <sambonsttt@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/Sethis/usefulgram"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `usefulgram-0.0.0a2/README.md` & `usefulgram-0.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a2/usefulgram/const/__pycache__/const.cpython-310.pyc` & `usefulgram-0.0.0a3/usefulgram/enums/__pycache__/const.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a2/usefulgram/const/__pycache__/const.cpython-311.pyc` & `usefulgram-0.0.0a3/usefulgram/enums/__pycache__/const.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a2/usefulgram/exceptions/__pycache__/exceptions.cpython-310.pyc` & `usefulgram-0.0.0a3/usefulgram/exceptions/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a2/usefulgram/exceptions/__pycache__/exceptions.cpython-311.pyc` & `usefulgram-0.0.0a3/usefulgram/exceptions/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a2/usefulgram/filters/__pycache__/database_filters.cpython-311.pyc` & `usefulgram-0.0.0a3/usefulgram/filters/__pycache__/database_filters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a2/usefulgram/filters/__pycache__/parse_filters.cpython-311.pyc` & `usefulgram-0.0.0a3/usefulgram/filters/__pycache__/parse_filters.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0dd19864 (Sun Jun 25 23:43:09 2023 UTC)
+moddate:  0x973aaf64 (Wed Jul 12 23:43:19 2023 UTC)
 files sz: 4056
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `usefulgram-0.0.0a2/usefulgram/filters/database_filters.py` & `usefulgram-0.0.0a3/usefulgram/filters/database_filters.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a2/usefulgram/filters/parse_filters.py` & `usefulgram-0.0.0a3/usefulgram/filters/parse_filters.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a2/usefulgram/keyboard/__pycache__/builder.cpython-310.pyc` & `usefulgram-0.0.0a3/usefulgram/keyboard/__pycache__/builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a2/usefulgram/keyboard/__pycache__/builder.cpython-311.pyc` & `usefulgram-0.0.0a3/usefulgram/keyboard/__pycache__/builder.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x2aafa064 (Sat Jul  1 22:56:42 2023 UTC)
-files sz: 4266
+moddate:  0x1f2faf64 (Wed Jul 12 22:54:23 2023 UTC)
+files sz: 4836
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a030100640064026c046d
@@ -102,42 +102,42 @@
                146 LOAD_CONST              11 (<code object Button, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 26>)
                148 MAKE_FUNCTION            0
                150 LOAD_CONST              12 ('Button')
                152 PRECALL                  2
                156 CALL                     2
                166 STORE_NAME              26 (Button)
    
-    69         168 PUSH_NULL
+    92         168 PUSH_NULL
                170 LOAD_BUILD_CLASS
-               172 LOAD_CONST              13 (<code object ReplyButton, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 69>)
+               172 LOAD_CONST              13 (<code object ReplyButton, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 92>)
                174 MAKE_FUNCTION            0
                176 LOAD_CONST              14 ('ReplyButton')
                178 PRECALL                  2
                182 CALL                     2
                192 STORE_NAME              27 (ReplyButton)
    
-    84         194 PUSH_NULL
+   107         194 PUSH_NULL
                196 LOAD_BUILD_CLASS
-               198 LOAD_CONST              15 (<code object Row, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 84>)
+               198 LOAD_CONST              15 (<code object Row, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 107>)
                200 MAKE_FUNCTION            0
                202 LOAD_CONST              16 ('Row')
                204 PRECALL                  2
                208 CALL                     2
                218 STORE_NAME              28 (Row)
    
-   107         220 PUSH_NULL
+   130         220 PUSH_NULL
                222 LOAD_BUILD_CLASS
-               224 LOAD_CONST              17 (<code object _Builder, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 107>)
+               224 LOAD_CONST              17 (<code object _Builder, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 130>)
                226 MAKE_FUNCTION            0
                228 LOAD_CONST              18 ('_Builder')
                230 PRECALL                  2
                234 CALL                     2
                244 STORE_NAME              29 (_Builder)
    
-   147         246 PUSH_NULL
+   170         246 PUSH_NULL
                248 LOAD_NAME               29 (_Builder)
                250 PRECALL                  0
                254 CALL                     0
                264 STORE_NAME              30 (Builder)
                266 LOAD_CONST              19 (None)
                268 RETURN_VALUE
    consts
@@ -182,27 +182,31 @@
          filename   'C:\\work\\usefulgram\\usefulgram\\keyboard\\builder.py'
          name       'check_buttons_type'
          firstlineno 21
          lnotab 0x020120010eff
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 16
+         stacksize : 15
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c00000065056503190000
             00000000000000650464023c000000650565031900000000000000000065
             0464033c000000650665076503650865096404650a650b650c650d660819
             0000000000000000006405660219000000000000000000650464063c0000
             00650e6503650f660219000000000000000000650464073c000000650365
-            0464083c0000000900641164046409640a9c026401650364026505650319
-            000000000000000000640b65076503650865096404650a650b650c650d66
-            081900000000000000000064036505650319000000000000000000640865
-            03640c650e6503650f660219000000000000000000660c640d84075a1064
-            0e84005a11640f65126602641084045a1364045300
+            0464083c000000640464046409640a9c0364016507650365086602190000
+            00000000000000640b65076503650865096404650a650b650c650d660819
+            000000000000000000640265056503190000000000000000006403650565
+            031900000000000000000064086503640c650e6503650f66021900000000
+            0000000000660c640d84065a10640e84005a116512640265056503190000
+            00000000000000640b650665076503650865096404650a650b650c650d66
+            08190000000000000000006405660219000000000000000000640f650565
+            0319000000000000000000660664108404a6000000ab0000000000000000
+            005a13640f65146602641184045a1564045300
           26           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Button')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
@@ -258,312 +262,432 @@
                      142 STORE_SUBSCR
          
           33         146 LOAD_NAME                3 (str)
                      148 LOAD_NAME                4 (__annotations__)
                      150 LOAD_CONST               8 ('separator')
                      152 STORE_SUBSCR
          
-          36         156 NOP
+          38         156 LOAD_CONST               4 (None)
          
-          35         158 LOAD_CONST              17 ((None,))
+          39         158 LOAD_CONST               4 (None)
+                     160 LOAD_CONST               9 ('/')
          
-          38         160 LOAD_CONST               4 (None)
-                     162 LOAD_CONST               9 ('/')
-         
-          35         164 LOAD_CONST              10 (('url', 'separator'))
-                     166 BUILD_CONST_KEY_MAP      2
-                     168 LOAD_CONST               1 ('text')
-         
-          36         170 LOAD_NAME                3 (str)
-         
-          35         172 LOAD_CONST               2 ('prefix')
-         
-          36         174 LOAD_NAME                5 (Optional)
-                     176 LOAD_NAME                3 (str)
-                     178 BINARY_SUBSCR
-         
-          35         188 LOAD_CONST              11 ('args')
-         
-          37         190 LOAD_NAME                7 (Union)
-                     192 LOAD_NAME                3 (str)
-                     194 LOAD_NAME                8 (int)
-                     196 LOAD_NAME                9 (bool)
-                     198 LOAD_CONST               4 (None)
-                     200 LOAD_NAME               10 (datetime)
-                     202 LOAD_NAME               11 (date)
-                     204 LOAD_NAME               12 (time)
-                     206 LOAD_NAME               13 (object)
-                     208 BUILD_TUPLE              8
-                     210 BINARY_SUBSCR
-         
-          35         220 LOAD_CONST               3 ('url')
-         
-          38         222 LOAD_NAME                5 (Optional)
-                     224 LOAD_NAME                3 (str)
-                     226 BINARY_SUBSCR
-         
-          35         236 LOAD_CONST               8 ('separator')
-         
-          38         238 LOAD_NAME                3 (str)
-         
-          35         240 LOAD_CONST              12 ('kwargs')
-         
-          39         242 LOAD_NAME               14 (dict)
-                     244 LOAD_NAME                3 (str)
-                     246 LOAD_NAME               15 (Any)
-                     248 BUILD_TUPLE              2
-                     250 BINARY_SUBSCR
-         
-          35         260 BUILD_TUPLE             12
-                     262 LOAD_CONST              13 (<code object __init__, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 35>)
-                     264 MAKE_FUNCTION            7 (defaults, kwdefaults, annotations)
-                     266 STORE_NAME              16 (__init__)
-         
-          52         268 LOAD_CONST              14 (<code object __repr__, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 52>)
-                     270 MAKE_FUNCTION            0
-                     272 STORE_NAME              17 (__repr__)
-         
-          55         274 LOAD_CONST              15 ('return')
-                     276 LOAD_NAME               18 (InlineKeyboardButton)
-                     278 BUILD_TUPLE              2
-                     280 LOAD_CONST              16 (<code object get_buttons, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 55>)
-                     282 MAKE_FUNCTION            4 (annotations)
-                     284 STORE_NAME              19 (get_buttons)
-                     286 LOAD_CONST               4 (None)
-                     288 RETURN_VALUE
+          35         162 LOAD_CONST              10 (('prefix', 'url', 'separator'))
+                     164 BUILD_CONST_KEY_MAP      3
+                     166 LOAD_CONST               1 ('text')
+         
+          36         168 LOAD_NAME                7 (Union)
+                     170 LOAD_NAME                3 (str)
+                     172 LOAD_NAME                8 (int)
+                     174 BUILD_TUPLE              2
+                     176 BINARY_SUBSCR
+         
+          35         186 LOAD_CONST              11 ('args')
+         
+          37         188 LOAD_NAME                7 (Union)
+                     190 LOAD_NAME                3 (str)
+                     192 LOAD_NAME                8 (int)
+                     194 LOAD_NAME                9 (bool)
+                     196 LOAD_CONST               4 (None)
+                     198 LOAD_NAME               10 (datetime)
+                     200 LOAD_NAME               11 (date)
+                     202 LOAD_NAME               12 (time)
+                     204 LOAD_NAME               13 (object)
+                     206 BUILD_TUPLE              8
+                     208 BINARY_SUBSCR
+         
+          35         218 LOAD_CONST               2 ('prefix')
+         
+          38         220 LOAD_NAME                5 (Optional)
+                     222 LOAD_NAME                3 (str)
+                     224 BINARY_SUBSCR
+         
+          35         234 LOAD_CONST               3 ('url')
+         
+          39         236 LOAD_NAME                5 (Optional)
+                     238 LOAD_NAME                3 (str)
+                     240 BINARY_SUBSCR
+         
+          35         250 LOAD_CONST               8 ('separator')
+         
+          39         252 LOAD_NAME                3 (str)
+         
+          35         254 LOAD_CONST              12 ('kwargs')
+         
+          40         256 LOAD_NAME               14 (dict)
+                     258 LOAD_NAME                3 (str)
+                     260 LOAD_NAME               15 (Any)
+                     262 BUILD_TUPLE              2
+                     264 BINARY_SUBSCR
+         
+          35         274 BUILD_TUPLE             12
+                     276 LOAD_CONST              13 (<code object __init__, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 35>)
+                     278 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     280 STORE_NAME              16 (__init__)
+         
+          58         282 LOAD_CONST              14 (<code object __repr__, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 58>)
+                     284 MAKE_FUNCTION            0
+                     286 STORE_NAME              17 (__repr__)
+         
+          61         288 LOAD_NAME               18 (staticmethod)
+         
+          62         290 LOAD_CONST               2 ('prefix')
+         
+          63         292 LOAD_NAME                5 (Optional)
+                     294 LOAD_NAME                3 (str)
+                     296 BINARY_SUBSCR
+         
+          62         306 LOAD_CONST              11 ('args')
+         
+          64         308 LOAD_NAME                6 (tuple)
+                     310 LOAD_NAME                7 (Union)
+                     312 LOAD_NAME                3 (str)
+                     314 LOAD_NAME                8 (int)
+                     316 LOAD_NAME                9 (bool)
+                     318 LOAD_CONST               4 (None)
+                     320 LOAD_NAME               10 (datetime)
+                     322 LOAD_NAME               11 (date)
+                     324 LOAD_NAME               12 (time)
+                     326 LOAD_NAME               13 (object)
+                     328 BUILD_TUPLE              8
+                     330 BINARY_SUBSCR
+                     340 LOAD_CONST               5 (Ellipsis)
+                     342 BUILD_TUPLE              2
+                     344 BINARY_SUBSCR
+         
+          62         354 LOAD_CONST              15 ('return')
+         
+          65         356 LOAD_NAME                5 (Optional)
+                     358 LOAD_NAME                3 (str)
+                     360 BINARY_SUBSCR
+         
+          62         370 BUILD_TUPLE              6
+                     372 LOAD_CONST              16 (<code object _get_prefix, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 61>)
+                     374 MAKE_FUNCTION            4 (annotations)
+         
+          61         376 PRECALL                  0
+                     380 CALL                     0
+         
+          62         390 STORE_NAME              19 (_get_prefix)
+         
+          78         392 LOAD_CONST              15 ('return')
+                     394 LOAD_NAME               20 (InlineKeyboardButton)
+                     396 BUILD_TUPLE              2
+                     398 LOAD_CONST              17 (<code object get_buttons, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 78>)
+                     400 MAKE_FUNCTION            4 (annotations)
+                     402 STORE_NAME              21 (get_buttons)
+                     404 LOAD_CONST               4 (None)
+                     406 RETURN_VALUE
          consts
             'Button'
             'text'
             'prefix'
             'url'
             None
             Ellipsis
             'additional'
             'other'
             'separator'
             '/'
-            ('url', 'separator')
+            ('prefix', 'url', 'separator')
             'args'
             'kwargs'
             code
-               argcount  : 3
+               argcount  : 2
                nlocals   : 7
                stacksize : 5
                flags     : 15
                code
-                  0x97007401000000000000000000007c027c037c066603a6010000ab0100
-                  00000000000000730774020000000000000000000082017c017c005f0200
-                  000000000000007c027c005f0300000000000000007c037c005f04000000
-                  00000000007c057c005f0500000000000000007c067c005f060000000000
-                  0000007c047c005f07000000000000000064005300
+                  0x97007c00a00000000000000000000000000000000000000000007c027c
+                  05a6020000ab0200000000000000007d027403000000000000000000007c
+                  01740400000000000000000000a6020000ab020000000000000000720f74
+                  07000000000000000000007c01a6010000ab0100000000000000007d0174
+                  09000000000000000000007c027c037c066603a6010000ab010000000000
+                  0000007307740a0000000000000000000082017c017c005f060000000000
+                  0000007c027c005f0700000000000000007c037c005f0800000000000000
+                  007c057c005f0900000000000000007c067c005f0a00000000000000007c
+                  047c005f0b000000000000000064005300
                 35           0 RESUME                   0
                
-                42           2 LOAD_GLOBAL              1 (NULL + any)
-                            14 LOAD_FAST                2 (prefix)
-                            16 LOAD_FAST                3 (url)
-                            18 LOAD_FAST                6 (kwargs)
-                            20 BUILD_TUPLE              3
-                            22 PRECALL                  1
-                            26 CALL                     1
-                            36 POP_JUMP_FORWARD_IF_TRUE     7 (to 52)
-               
-                43          38 LOAD_GLOBAL              2 (NoOneButtonParamIsFilled)
-                            50 RAISE_VARARGS            1
-               
-                45     >>   52 LOAD_FAST                1 (text)
-                            54 LOAD_FAST                0 (self)
-                            56 STORE_ATTR               2 (text)
-               
-                46          66 LOAD_FAST                2 (prefix)
-                            68 LOAD_FAST                0 (self)
-                            70 STORE_ATTR               3 (prefix)
-               
-                47          80 LOAD_FAST                3 (url)
-                            82 LOAD_FAST                0 (self)
-                            84 STORE_ATTR               4 (url)
-               
-                48          94 LOAD_FAST                5 (args)
-                            96 LOAD_FAST                0 (self)
-                            98 STORE_ATTR               5 (additional)
-               
-                49         108 LOAD_FAST                6 (kwargs)
-                           110 LOAD_FAST                0 (self)
-                           112 STORE_ATTR               6 (other)
-               
-                50         122 LOAD_FAST                4 (separator)
-                           124 LOAD_FAST                0 (self)
-                           126 STORE_ATTR               7 (separator)
-                           136 LOAD_CONST               0 (None)
-                           138 RETURN_VALUE
+                43           2 LOAD_FAST                0 (self)
+                             4 LOAD_METHOD              0 (_get_prefix)
+                            26 LOAD_FAST                2 (prefix)
+                            28 LOAD_FAST                5 (args)
+                            30 PRECALL                  2
+                            34 CALL                     2
+                            44 STORE_FAST               2 (prefix)
+               
+                45          46 LOAD_GLOBAL              3 (NULL + isinstance)
+                            58 LOAD_FAST                1 (text)
+                            60 LOAD_GLOBAL              4 (int)
+                            72 PRECALL                  2
+                            76 CALL                     2
+                            86 POP_JUMP_FORWARD_IF_FALSE    15 (to 118)
+               
+                46          88 LOAD_GLOBAL              7 (NULL + str)
+                           100 LOAD_FAST                1 (text)
+                           102 PRECALL                  1
+                           106 CALL                     1
+                           116 STORE_FAST               1 (text)
+               
+                48     >>  118 LOAD_GLOBAL              9 (NULL + any)
+                           130 LOAD_FAST                2 (prefix)
+                           132 LOAD_FAST                3 (url)
+                           134 LOAD_FAST                6 (kwargs)
+                           136 BUILD_TUPLE              3
+                           138 PRECALL                  1
+                           142 CALL                     1
+                           152 POP_JUMP_FORWARD_IF_TRUE     7 (to 168)
+               
+                49         154 LOAD_GLOBAL             10 (NoOneButtonParamIsFilled)
+                           166 RAISE_VARARGS            1
+               
+                51     >>  168 LOAD_FAST                1 (text)
+                           170 LOAD_FAST                0 (self)
+                           172 STORE_ATTR               6 (text)
+               
+                52         182 LOAD_FAST                2 (prefix)
+                           184 LOAD_FAST                0 (self)
+                           186 STORE_ATTR               7 (prefix)
+               
+                53         196 LOAD_FAST                3 (url)
+                           198 LOAD_FAST                0 (self)
+                           200 STORE_ATTR               8 (url)
+               
+                54         210 LOAD_FAST                5 (args)
+                           212 LOAD_FAST                0 (self)
+                           214 STORE_ATTR               9 (additional)
+               
+                55         224 LOAD_FAST                6 (kwargs)
+                           226 LOAD_FAST                0 (self)
+                           228 STORE_ATTR              10 (other)
+               
+                56         238 LOAD_FAST                4 (separator)
+                           240 LOAD_FAST                0 (self)
+                           242 STORE_ATTR              11 (separator)
+                           252 LOAD_CONST               0 (None)
+                           254 RETURN_VALUE
                consts
                   None
-               names      ('any', 'NoOneButtonParamIsFilled', 'text', 'prefix', 'url', 'additional', 'other', 'separator')
+               names      ('_get_prefix', 'isinstance', 'int', 'str', 'any', 'NoOneButtonParamIsFilled', 'text', 'prefix', 'url', 'additional', 'other', 'separator')
                varnames   ('self', 'text', 'prefix', 'url', 'separator', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\work\\usefulgram\\usefulgram\\keyboard\\builder.py'
                name       '__init__'
                firstlineno 35
-               lnotab 0x020724010e020e010e010e010e010e01
+               lnotab 0x02082c022a011e0224010e020e010e010e010e010e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c00a6010000ab0100000000000000
                   005300
-                52           0 RESUME                   0
+                58           0 RESUME                   0
                
-                53           2 LOAD_GLOBAL              1 (NULL + autorepr)
+                59           2 LOAD_GLOBAL              1 (NULL + autorepr)
                             14 LOAD_FAST                0 (self)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 RETURN_VALUE
                consts
                   None
                names      ('autorepr',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\work\\usefulgram\\usefulgram\\keyboard\\builder.py'
                name       '__repr__'
-               firstlineno 52
+               firstlineno 58
                lnotab 0x0201
             'return'
             code
+               argcount  : 2
+               nlocals   : 4
+               stacksize : 4
+               flags     : 3
+               code
+                  0x97007c0081027c0053007c0144005d1d7d027c02a00000000000000000
+                  000000000000000000000000006401a6010000ab0100000000000000007d
+                  037c0381047c036302010053008c1e64005300
+                61           0 RESUME                   0
+               
+                67           2 LOAD_FAST                0 (prefix)
+                             4 POP_JUMP_FORWARD_IF_NONE     2 (to 10)
+               
+                68           6 LOAD_FAST                0 (prefix)
+                             8 RETURN_VALUE
+               
+                70     >>   10 LOAD_FAST                1 (args)
+                            12 GET_ITER
+                       >>   14 FOR_ITER                29 (to 74)
+                            16 STORE_FAST               2 (obj)
+               
+                71          18 LOAD_FAST                2 (obj)
+                            20 LOAD_METHOD              0 (__getattribute__)
+                            42 LOAD_CONST               1 ('prefix')
+                            44 PRECALL                  1
+                            48 CALL                     1
+                            58 STORE_FAST               3 (result)
+               
+                73          60 LOAD_FAST                3 (result)
+                            62 POP_JUMP_FORWARD_IF_NONE     4 (to 72)
+               
+                74          64 LOAD_FAST                3 (result)
+                            66 SWAP                     2
+                            68 POP_TOP
+                            70 RETURN_VALUE
+               
+                73     >>   72 JUMP_BACKWARD           30 (to 14)
+               
+                76     >>   74 LOAD_CONST               0 (None)
+                            76 RETURN_VALUE
+               consts
+                  None
+                  'prefix'
+               names      ('__getattribute__',)
+               varnames   ('prefix', 'args', 'obj', 'result')
+               freevars   ()
+               cellvars   ()
+               filename   'C:\\work\\usefulgram\\usefulgram\\keyboard\\builder.py'
+               name       '_get_prefix'
+               firstlineno 61
+               lnotab 0x02060401040208012a02040108ff0203
+            code
                argcount  : 1
                nlocals   : 2
                stacksize : 7
                flags     : 3
                code
                   0x97007c006a00000000000000000081207403000000000000000000007c
                   006a00000000000000000067017c006a020000000000000000a201520064
                   017c006a03000000000000000069018e017d016e0264007d017409000000
                   0000000000000064037c006a0500000000000000007c006a060000000000
                   0000007c0164029c037c006a070000000000000000a4018e015300
-                55           0 RESUME                   0
+                78           0 RESUME                   0
                
-                56           2 LOAD_FAST                0 (self)
+                79           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (prefix)
                             14 POP_JUMP_FORWARD_IF_NONE    32 (to 80)
                
-                57          16 LOAD_GLOBAL              3 (NULL + CallbackData)
+                80          16 LOAD_GLOBAL              3 (NULL + CallbackData)
                
-                58          28 LOAD_FAST                0 (self)
+                81          28 LOAD_FAST                0 (self)
                             30 LOAD_ATTR                0 (prefix)
                
-                57          40 BUILD_LIST               1
+                80          40 BUILD_LIST               1
                
-                58          42 LOAD_FAST                0 (self)
+                81          42 LOAD_FAST                0 (self)
                             44 LOAD_ATTR                2 (additional)
                
-                57          54 LIST_EXTEND              1
+                80          54 LIST_EXTEND              1
                             56 LIST_TO_TUPLE
                             58 LOAD_CONST               1 ('separator')
                
-                59          60 LOAD_FAST                0 (self)
+                82          60 LOAD_FAST                0 (self)
                             62 LOAD_ATTR                3 (separator)
                
-                57          72 BUILD_MAP                1
+                80          72 BUILD_MAP                1
                             74 CALL_FUNCTION_EX         1
                             76 STORE_FAST               1 (callback_data)
                             78 JUMP_FORWARD             2 (to 84)
                
-                62     >>   80 LOAD_CONST               0 (None)
+                85     >>   80 LOAD_CONST               0 (None)
                             82 STORE_FAST               1 (callback_data)
                
-                64     >>   84 LOAD_GLOBAL              9 (NULL + InlineKeyboardButton)
+                87     >>   84 LOAD_GLOBAL              9 (NULL + InlineKeyboardButton)
                             96 LOAD_CONST               3 (())
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                5 (text)
                            110 LOAD_FAST                0 (self)
                            112 LOAD_ATTR                6 (url)
                
-                65         122 LOAD_FAST                1 (callback_data)
+                88         122 LOAD_FAST                1 (callback_data)
                
-                64         124 LOAD_CONST               2 (('text', 'url', 'callback_data'))
+                87         124 LOAD_CONST               2 (('text', 'url', 'callback_data'))
                            126 BUILD_CONST_KEY_MAP      3
                
-                66         128 LOAD_FAST                0 (self)
+                89         128 LOAD_FAST                0 (self)
                            130 LOAD_ATTR                7 (other)
                
-                64         140 DICT_MERGE               1
+                87         140 DICT_MERGE               1
                            142 CALL_FUNCTION_EX         1
                            144 RETURN_VALUE
                consts
                   None
                   'separator'
                   ('text', 'url', 'callback_data')
                   ()
                names      ('prefix', 'CallbackData', 'additional', 'separator', 'InlineKeyboardButton', 'text', 'url', 'other')
                varnames   ('self', 'callback_data')
                freevars   ()
                cellvars   ()
                filename   'C:\\work\\usefulgram\\usefulgram\\keyboard\\builder.py'
                name       'get_buttons'
-               firstlineno 55
+               firstlineno 78
                lnotab 0x02010e010c010cff02010cff06020cfe08050402260102ff04020cfe
-            (None,)
-         names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'Optional', 'tuple', 'Union', 'int', 'bool', 'datetime', 'date', 'time', 'object', 'dict', 'Any', '__init__', '__repr__', 'InlineKeyboardButton', 'get_buttons')
+         names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'Optional', 'tuple', 'Union', 'int', 'bool', 'datetime', 'date', 'time', 'object', 'dict', 'Any', '__init__', '__repr__', 'staticmethod', '_get_prefix', 'InlineKeyboardButton', 'get_buttons')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\work\\usefulgram\\usefulgram\\keyboard\\builder.py'
          name       'Button'
          firstlineno 26
          lnotab
-            0x0c010a01160116010e0106ff0c0102ff14021a010a0302ff020304fd06
-            0102ff02010eff02021efe02030efd020302fd020412fc08110603
+            0x0c010a01160116010e0106ff0c0102ff14021a010a05020104fc060112
+            ff02021efe02030efd02040efc020402fc020512fb08170603020102010e
+            ff02022efe02030efd06ff0e010210
       'Button'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c00000065056503650666
             0219000000000000000000650464023c000000640165036602640384045a
             07640484005a08640565096602640684045a0a64075300
-          69           0 RESUME                   0
+          92           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ReplyButton')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          70          12 LOAD_NAME                3 (str)
+          93          12 LOAD_NAME                3 (str)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('text')
                       18 STORE_SUBSCR
          
-          71          22 LOAD_NAME                5 (dict)
+          94          22 LOAD_NAME                5 (dict)
                       24 LOAD_NAME                3 (str)
                       26 LOAD_NAME                6 (Any)
                       28 BUILD_TUPLE              2
                       30 BINARY_SUBSCR
                       40 LOAD_NAME                4 (__annotations__)
                       42 LOAD_CONST               2 ('other')
                       44 STORE_SUBSCR
          
-          73          48 LOAD_CONST               1 ('text')
+          96          48 LOAD_CONST               1 ('text')
                       50 LOAD_NAME                3 (str)
                       52 BUILD_TUPLE              2
-                      54 LOAD_CONST               3 (<code object __init__, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 73>)
+                      54 LOAD_CONST               3 (<code object __init__, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 96>)
                       56 MAKE_FUNCTION            4 (annotations)
                       58 STORE_NAME               7 (__init__)
          
-          77          60 LOAD_CONST               4 (<code object __repr__, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 77>)
+         100          60 LOAD_CONST               4 (<code object __repr__, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 100>)
                       62 MAKE_FUNCTION            0
                       64 STORE_NAME               8 (__repr__)
          
-          80          66 LOAD_CONST               5 ('return')
+         103          66 LOAD_CONST               5 ('return')
                       68 LOAD_NAME                9 (KeyboardButton)
                       70 BUILD_TUPLE              2
-                      72 LOAD_CONST               6 (<code object get_buttons, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 80>)
+                      72 LOAD_CONST               6 (<code object get_buttons, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 103>)
                       74 MAKE_FUNCTION            4 (annotations)
                       76 STORE_NAME              10 (get_buttons)
                       78 LOAD_CONST               7 (None)
                       80 RETURN_VALUE
          consts
             'ReplyButton'
             'text'
@@ -572,72 +696,72 @@
                argcount  : 2
                nlocals   : 3
                stacksize : 2
                flags     : 11
                code
                   0x97007c017c005f0000000000000000007c027c005f0100000000000000
                   0064005300
-                73           0 RESUME                   0
+                96           0 RESUME                   0
                
-                74           2 LOAD_FAST                1 (text)
+                97           2 LOAD_FAST                1 (text)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (text)
                
-                75          16 LOAD_FAST                2 (kwargs)
+                98          16 LOAD_FAST                2 (kwargs)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (other)
                             30 LOAD_CONST               0 (None)
                             32 RETURN_VALUE
                consts
                   None
                names      ('text', 'other')
                varnames   ('self', 'text', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\work\\usefulgram\\usefulgram\\keyboard\\builder.py'
                name       '__init__'
-               firstlineno 73
+               firstlineno 96
                lnotab 0x02010e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c00a6010000ab0100000000000000
                   005300
-                77           0 RESUME                   0
+               100           0 RESUME                   0
                
-                78           2 LOAD_GLOBAL              1 (NULL + autorepr)
+               101           2 LOAD_GLOBAL              1 (NULL + autorepr)
                             14 LOAD_FAST                0 (self)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 RETURN_VALUE
                consts
                   None
                names      ('autorepr',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\work\\usefulgram\\usefulgram\\keyboard\\builder.py'
                name       '__repr__'
-               firstlineno 77
+               firstlineno 100
                lnotab 0x0201
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x9700740100000000000000000000640264017c006a0100000000000000
                   0069017c006a020000000000000000a4018e015300
-                80           0 RESUME                   0
+               103           0 RESUME                   0
                
-                81           2 LOAD_GLOBAL              1 (NULL + KeyboardButton)
+               104           2 LOAD_GLOBAL              1 (NULL + KeyboardButton)
                             14 LOAD_CONST               2 (())
                             16 LOAD_CONST               1 ('text')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (text)
                             30 BUILD_MAP                1
                             32 LOAD_FAST                0 (self)
                             34 LOAD_ATTR                2 (other)
@@ -650,88 +774,88 @@
                   ()
                names      ('KeyboardButton', 'text', 'other')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\work\\usefulgram\\usefulgram\\keyboard\\builder.py'
                name       'get_buttons'
-               firstlineno 80
+               firstlineno 103
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'dict', 'Any', '__init__', '__repr__', 'KeyboardButton', 'get_buttons')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\work\\usefulgram\\usefulgram\\keyboard\\builder.py'
          name       'ReplyButton'
-         firstlineno 69
+         firstlineno 92
          lnotab 0x0c010a011a020c040603
       'ReplyButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0255006503650465051900000000000000000065
             04650619000000000000000000660219000000000000000000650764013c
             000000650365086509660219000000000000000000650764023c00000064
             036503650965086602190000000000000000006602640484045a0a640584
             005a0b640665046505190000000000000000006602640784045a0c640853
             00
-          84           0 RESUME                   0
+         107           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Row')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          85          12 LOAD_NAME                3 (Union)
+         108          12 LOAD_NAME                3 (Union)
                       14 LOAD_NAME                4 (list)
                       16 LOAD_NAME                5 (InlineKeyboardButton)
                       18 BINARY_SUBSCR
                       28 LOAD_NAME                4 (list)
                       30 LOAD_NAME                6 (KeyboardButton)
                       32 BINARY_SUBSCR
                       42 BUILD_TUPLE              2
                       44 BINARY_SUBSCR
                       54 LOAD_NAME                7 (__annotations__)
                       56 LOAD_CONST               1 ('buttons')
                       58 STORE_SUBSCR
          
-          86          62 LOAD_NAME                3 (Union)
+         109          62 LOAD_NAME                3 (Union)
                       64 LOAD_NAME                8 (Button)
                       66 LOAD_NAME                9 (ReplyButton)
                       68 BUILD_TUPLE              2
                       70 BINARY_SUBSCR
                       80 LOAD_NAME                7 (__annotations__)
                       82 LOAD_CONST               2 ('first_button_instance')
                       84 STORE_SUBSCR
          
-          88          88 LOAD_CONST               3 ('args')
+         111          88 LOAD_CONST               3 ('args')
                       90 LOAD_NAME                3 (Union)
                       92 LOAD_NAME                9 (ReplyButton)
                       94 LOAD_NAME                8 (Button)
                       96 BUILD_TUPLE              2
                       98 BINARY_SUBSCR
                      108 BUILD_TUPLE              2
-                     110 LOAD_CONST               4 (<code object __init__, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 88>)
+                     110 LOAD_CONST               4 (<code object __init__, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 111>)
                      112 MAKE_FUNCTION            4 (annotations)
                      114 STORE_NAME              10 (__init__)
          
-         100         116 LOAD_CONST               5 (<code object __repr__, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 100>)
+         123         116 LOAD_CONST               5 (<code object __repr__, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 123>)
                      118 MAKE_FUNCTION            0
                      120 STORE_NAME              11 (__repr__)
          
-         103         122 LOAD_CONST               6 ('return')
+         126         122 LOAD_CONST               6 ('return')
                      124 LOAD_NAME                4 (list)
                      126 LOAD_NAME                5 (InlineKeyboardButton)
                      128 BINARY_SUBSCR
                      138 BUILD_TUPLE              2
-                     140 LOAD_CONST               7 (<code object get_rows, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 103>)
+                     140 LOAD_CONST               7 (<code object get_rows, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 126>)
                      142 MAKE_FUNCTION            4 (annotations)
                      144 STORE_NAME              12 (get_rows)
                      146 LOAD_CONST               8 (None)
                      148 RETURN_VALUE
          consts
             'Row'
             'buttons'
@@ -746,210 +870,210 @@
                   0x970067007c005f0000000000000000007c016401190000000000000000
                   007d027c027c005f0100000000000000007c0144005d4b7d037405000000
                   000000000000007c037407000000000000000000007c02a6010000ab0100
                   00000000000000a6020000ab02000000000000000001007c006a00000000
                   0000000000a00400000000000000000000000000000000000000007c03a0
                   050000000000000000000000000000000000000000a6000000ab00000000
                   0000000000a6010000ab01000000000000000001008c4c64005300
-                88           0 RESUME                   0
+               111           0 RESUME                   0
                
-                89           2 BUILD_LIST               0
+               112           2 BUILD_LIST               0
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (buttons)
                
-                91          16 LOAD_FAST                1 (args)
+               114          16 LOAD_FAST                1 (args)
                             18 LOAD_CONST               1 (0)
                             20 BINARY_SUBSCR
                             30 STORE_FAST               2 (first_button)
                
-                93          32 LOAD_FAST                2 (first_button)
+               116          32 LOAD_FAST                2 (first_button)
                             34 LOAD_FAST                0 (self)
                             36 STORE_ATTR               1 (first_button_instance)
                
-                95          46 LOAD_FAST                1 (args)
+               118          46 LOAD_FAST                1 (args)
                             48 GET_ITER
                        >>   50 FOR_ITER                75 (to 202)
                             52 STORE_FAST               3 (button)
                
-                96          54 LOAD_GLOBAL              5 (NULL + check_buttons_type)
+               119          54 LOAD_GLOBAL              5 (NULL + check_buttons_type)
                             66 LOAD_FAST                3 (button)
                             68 LOAD_GLOBAL              7 (NULL + type)
                             80 LOAD_FAST                2 (first_button)
                             82 PRECALL                  1
                             86 CALL                     1
                             96 PRECALL                  2
                            100 CALL                     2
                            110 POP_TOP
                
-                98         112 LOAD_FAST                0 (self)
+               121         112 LOAD_FAST                0 (self)
                            114 LOAD_ATTR                0 (buttons)
                            124 LOAD_METHOD              4 (append)
                            146 LOAD_FAST                3 (button)
                            148 LOAD_METHOD              5 (get_buttons)
                            170 PRECALL                  0
                            174 CALL                     0
                            184 PRECALL                  1
                            188 CALL                     1
                            198 POP_TOP
                            200 JUMP_BACKWARD           76 (to 50)
                
-                95     >>  202 LOAD_CONST               0 (None)
+               118     >>  202 LOAD_CONST               0 (None)
                            204 RETURN_VALUE
                consts
                   None
                   0
                names      ('buttons', 'first_button_instance', 'check_buttons_type', 'type', 'append', 'get_buttons')
                varnames   ('self', 'args', 'first_button', 'button')
                freevars   ()
                cellvars   ()
                filename   'C:\\work\\usefulgram\\usefulgram\\keyboard\\builder.py'
                name       '__init__'
-               firstlineno 88
+               firstlineno 111
                lnotab 0x02010e0210020e0208013a025afd
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c00a6010000ab0100000000000000
                   005300
-               100           0 RESUME                   0
+               123           0 RESUME                   0
                
-               101           2 LOAD_GLOBAL              1 (NULL + autorepr)
+               124           2 LOAD_GLOBAL              1 (NULL + autorepr)
                             14 LOAD_FAST                0 (self)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 RETURN_VALUE
                consts
                   None
                names      ('autorepr',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\work\\usefulgram\\usefulgram\\keyboard\\builder.py'
                name       '__repr__'
-               firstlineno 100
+               firstlineno 123
                lnotab 0x0201
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               103           0 RESUME                   0
+               126           0 RESUME                   0
                
-               104           2 LOAD_FAST                0 (self)
+               127           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (buttons)
                             14 RETURN_VALUE
                consts
                   None
                names      ('buttons',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\work\\usefulgram\\usefulgram\\keyboard\\builder.py'
                name       'get_rows'
-               firstlineno 103
+               firstlineno 126
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'Union', 'list', 'InlineKeyboardButton', 'KeyboardButton', '__annotations__', 'Button', 'ReplyButton', '__init__', '__repr__', 'get_rows')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\work\\usefulgram\\usefulgram\\keyboard\\builder.py'
          name       'Row'
-         firstlineno 84
+         firstlineno 107
          lnotab 0x0c0132011a021c0c0603
       'Row'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 11
          flags     : 0
          code
             0x970065005a0164005a02650309000900640b6402650465056506650766
             021900000000000000000019000000000000000000640365046508190000
             00000000000000640465056509650a660219000000000000000000660664
             058405a6000000ab0000000000000000005a0b6401640664079c02640865
             0c64096504650d190000000000000000006403650864046505650e650f66
             02190000000000000000006608640a84065a1064015300
-         107           0 RESUME                   0
+         130           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('_Builder')
                        8 STORE_NAME               2 (__qualname__)
          
-         108          10 LOAD_NAME                3 (staticmethod)
+         131          10 LOAD_NAME                3 (staticmethod)
          
-         110          12 NOP
+         133          12 NOP
          
-         111          14 NOP
+         134          14 NOP
          
-         109          16 LOAD_CONST              11 ((None, None))
+         132          16 LOAD_CONST              11 ((None, None))
                       18 LOAD_CONST               2 ('first_row_button_ins')
          
-         110          20 LOAD_NAME                4 (Optional)
+         133          20 LOAD_NAME                4 (Optional)
                       22 LOAD_NAME                5 (Union)
                       24 LOAD_NAME                6 (Button)
                       26 LOAD_NAME                7 (ReplyButton)
                       28 BUILD_TUPLE              2
                       30 BINARY_SUBSCR
                       40 BINARY_SUBSCR
          
-         109          50 LOAD_CONST               3 ('is_callback')
+         132          50 LOAD_CONST               3 ('is_callback')
          
-         111          52 LOAD_NAME                4 (Optional)
+         134          52 LOAD_NAME                4 (Optional)
                       54 LOAD_NAME                8 (bool)
                       56 BINARY_SUBSCR
          
-         109          66 LOAD_CONST               4 ('return')
+         132          66 LOAD_CONST               4 ('return')
          
-         112          68 LOAD_NAME                5 (Union)
+         135          68 LOAD_NAME                5 (Union)
                       70 LOAD_NAME                9 (InlineKeyboardBuilder)
                       72 LOAD_NAME               10 (ReplyKeyboardBuilder)
                       74 BUILD_TUPLE              2
                       76 BINARY_SUBSCR
          
-         109          86 BUILD_TUPLE              6
-                      88 LOAD_CONST               5 (<code object _get_builder, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 108>)
+         132          86 BUILD_TUPLE              6
+                      88 LOAD_CONST               5 (<code object _get_builder, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 131>)
                       90 MAKE_FUNCTION            5 (defaults, annotations)
          
-         108          92 PRECALL                  0
+         131          92 PRECALL                  0
                       96 CALL                     0
          
-         109         106 STORE_NAME              11 (_get_builder)
+         132         106 STORE_NAME              11 (_get_builder)
          
-         124         108 LOAD_CONST               1 (None)
+         147         108 LOAD_CONST               1 (None)
          
-         125         110 LOAD_CONST               6 (True)
+         148         110 LOAD_CONST               6 (True)
          
-         124         112 LOAD_CONST               7 (('adjust', 'is_callback'))
+         147         112 LOAD_CONST               7 (('adjust', 'is_callback'))
                      114 BUILD_CONST_KEY_MAP      2
                      116 LOAD_CONST               8 ('rows')
                      118 LOAD_NAME               12 (Row)
                      120 LOAD_CONST               9 ('adjust')
                      122 LOAD_NAME                4 (Optional)
                      124 LOAD_NAME               13 (int)
                      126 BINARY_SUBSCR
                      136 LOAD_CONST               3 ('is_callback')
          
-         125         138 LOAD_NAME                8 (bool)
+         148         138 LOAD_NAME                8 (bool)
          
-         124         140 LOAD_CONST               4 ('return')
+         147         140 LOAD_CONST               4 ('return')
          
-         126         142 LOAD_NAME                5 (Union)
+         149         142 LOAD_NAME                5 (Union)
                      144 LOAD_NAME               14 (InlineKeyboardMarkup)
                      146 LOAD_NAME               15 (ReplyKeyboardMarkup)
                      148 BUILD_TUPLE              2
                      150 BINARY_SUBSCR
          
-         124         160 BUILD_TUPLE              8
-                     162 LOAD_CONST              10 (<code object __call__, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 124>)
+         147         160 BUILD_TUPLE              8
+                     162 LOAD_CONST              10 (<code object __call__, file "C:\work\usefulgram\usefulgram\keyboard\builder.py", line 147>)
                      164 MAKE_FUNCTION            6 (kwdefaults, annotations)
                      166 STORE_NAME              16 (__call__)
                      168 LOAD_CONST               1 (None)
                      170 RETURN_VALUE
          consts
             '_Builder'
             None
@@ -964,62 +1088,62 @@
                code
                   0x97007401000000000000000000007c00740200000000000000000000a6
                   020000ab02000000000000000073047c0164017500720e74050000000000
                   0000000000a6000000ab0000000000000000005300740100000000000000
                   0000007c00740600000000000000000000a6020000ab0200000000000000
                   0073047c0164027500720e740900000000000000000000a6000000ab0000
                   000000000000005300740a000000000000000000008201
-               108           0 RESUME                   0
+               131           0 RESUME                   0
                
-               114           2 LOAD_GLOBAL              1 (NULL + isinstance)
+               137           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                0 (first_row_button_ins)
                             16 LOAD_GLOBAL              2 (Button)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 POP_JUMP_FORWARD_IF_TRUE     4 (to 52)
                             44 LOAD_FAST                1 (is_callback)
                             46 LOAD_CONST               1 (True)
                             48 IS_OP                    0
                             50 POP_JUMP_FORWARD_IF_FALSE    14 (to 80)
                
-               115     >>   52 LOAD_GLOBAL              5 (NULL + InlineKeyboardBuilder)
+               138     >>   52 LOAD_GLOBAL              5 (NULL + InlineKeyboardBuilder)
                             64 PRECALL                  0
                             68 CALL                     0
                             78 RETURN_VALUE
                
-               117     >>   80 LOAD_GLOBAL              1 (NULL + isinstance)
+               140     >>   80 LOAD_GLOBAL              1 (NULL + isinstance)
                             92 LOAD_FAST                0 (first_row_button_ins)
                             94 LOAD_GLOBAL              6 (ReplyButton)
                            106 PRECALL                  2
                            110 CALL                     2
                            120 POP_JUMP_FORWARD_IF_TRUE     4 (to 130)
                
-               118         122 LOAD_FAST                1 (is_callback)
+               141         122 LOAD_FAST                1 (is_callback)
                            124 LOAD_CONST               2 (False)
                            126 IS_OP                    0
                            128 POP_JUMP_FORWARD_IF_FALSE    14 (to 158)
                
-               120     >>  130 LOAD_GLOBAL              9 (NULL + ReplyKeyboardBuilder)
+               143     >>  130 LOAD_GLOBAL              9 (NULL + ReplyKeyboardBuilder)
                            142 PRECALL                  0
                            146 CALL                     0
                            156 RETURN_VALUE
                
-               122     >>  158 LOAD_GLOBAL             10 (UnknownButtonType)
+               145     >>  158 LOAD_GLOBAL             10 (UnknownButtonType)
                            170 RAISE_VARARGS            1
                consts
                   None
                   True
                   False
                names      ('isinstance', 'Button', 'InlineKeyboardBuilder', 'ReplyButton', 'ReplyKeyboardBuilder', 'UnknownButtonType')
                varnames   ('first_row_button_ins', 'is_callback')
                freevars   ()
                cellvars   ()
                filename   'C:\\work\\usefulgram\\usefulgram\\keyboard\\builder.py'
                name       '_get_builder'
-               firstlineno 108
+               firstlineno 131
                lnotab 0x020632011c022a0108021c02
             True
             ('adjust', 'is_callback')
             'rows'
             'adjust'
             code
                argcount  : 1
@@ -1037,88 +1161,88 @@
                   076a030000000000000000740b000000000000000000007c05a6010000ab
                   010000000000000000a6020000ab020000000000000000010002007c066a
                   0600000000000000007c07a0070000000000000000000000000000000000
                   000000a6000000ab0000000000000000008e0001008c417c0181157c06a0
                   0800000000000000000000000000000000000000007c01a6010000ab0100
                   00000000000000010002007c066a020000000000000000640369007c04a4
                   018e015300
-               124           0 RESUME                   0
+               147           0 RESUME                   0
                
-               128           2 LOAD_GLOBAL              1 (NULL + len)
+               151           2 LOAD_GLOBAL              1 (NULL + len)
                             14 LOAD_FAST                3 (rows)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 LOAD_CONST               1 (0)
                             32 COMPARE_OP               2 (==)
                             38 POP_JUMP_FORWARD_IF_FALSE    40 (to 120)
                
-               129          40 LOAD_FAST                0 (self)
+               152          40 LOAD_FAST                0 (self)
                             42 LOAD_METHOD              1 (_get_builder)
                             64 LOAD_FAST                2 (is_callback)
                             66 KW_NAMES                 2
                             68 PRECALL                  1
                             72 CALL                     1
                             82 LOAD_METHOD              2 (as_markup)
                            104 PRECALL                  0
                            108 CALL                     0
                            118 RETURN_VALUE
                
-               131     >>  120 LOAD_FAST                3 (rows)
+               154     >>  120 LOAD_FAST                3 (rows)
                            122 LOAD_CONST               1 (0)
                            124 BINARY_SUBSCR
                            134 LOAD_ATTR                3 (first_button_instance)
                            144 STORE_FAST               5 (first_row_button_instance)
                
-               133         146 LOAD_FAST                0 (self)
+               156         146 LOAD_FAST                0 (self)
                            148 LOAD_METHOD              1 (_get_builder)
                            170 LOAD_FAST                5 (first_row_button_instance)
                            172 PRECALL                  1
                            176 CALL                     1
                            186 STORE_FAST               6 (builder)
                
-               135         188 LOAD_FAST                3 (rows)
+               158         188 LOAD_FAST                3 (rows)
                            190 GET_ITER
                        >>  192 FOR_ITER                64 (to 322)
                            194 STORE_FAST               7 (row)
                
-               136         196 LOAD_GLOBAL              9 (NULL + check_buttons_type)
+               159         196 LOAD_GLOBAL              9 (NULL + check_buttons_type)
                            208 LOAD_FAST                7 (row)
                            210 LOAD_ATTR                3 (first_button_instance)
                
-               137         220 LOAD_GLOBAL             11 (NULL + type)
+               160         220 LOAD_GLOBAL             11 (NULL + type)
                            232 LOAD_FAST                5 (first_row_button_instance)
                            234 PRECALL                  1
                            238 CALL                     1
                
-               136         248 PRECALL                  2
+               159         248 PRECALL                  2
                            252 CALL                     2
                            262 POP_TOP
                
-               139         264 PUSH_NULL
+               162         264 PUSH_NULL
                            266 LOAD_FAST                6 (builder)
                            268 LOAD_ATTR                6 (row)
                            278 LOAD_FAST                7 (row)
                            280 LOAD_METHOD              7 (get_rows)
                            302 PRECALL                  0
                            306 CALL                     0
                            316 CALL_FUNCTION_EX         0
                            318 POP_TOP
                            320 JUMP_BACKWARD           65 (to 192)
                
-               141     >>  322 LOAD_FAST                1 (adjust)
+               164     >>  322 LOAD_FAST                1 (adjust)
                            324 POP_JUMP_FORWARD_IF_NONE    21 (to 368)
                
-               142         326 LOAD_FAST                6 (builder)
+               165         326 LOAD_FAST                6 (builder)
                            328 LOAD_METHOD              8 (adjust)
                            350 LOAD_FAST                1 (adjust)
                            352 PRECALL                  1
                            356 CALL                     1
                            366 POP_TOP
                
-               144     >>  368 PUSH_NULL
+               167     >>  368 PUSH_NULL
                            370 LOAD_FAST                6 (builder)
                            372 LOAD_ATTR                2 (as_markup)
                            382 LOAD_CONST               3 (())
                            384 BUILD_MAP                0
                            386 LOAD_FAST                4 (kwargs)
                            388 DICT_MERGE               1
                            390 CALL_FUNCTION_EX         1
@@ -1130,30 +1254,30 @@
                   ()
                names      ('len', '_get_builder', 'as_markup', 'first_button_instance', 'check_buttons_type', 'type', 'row', 'get_rows', 'adjust')
                varnames   ('self', 'adjust', 'is_callback', 'rows', 'kwargs', 'first_row_button_instance', 'builder', 'row')
                freevars   ()
                cellvars   ()
                filename   'C:\\work\\usefulgram\\usefulgram\\keyboard\\builder.py'
                name       '__call__'
-               firstlineno 124
+               firstlineno 147
                lnotab 0x0204260150021a022a02080118011cff10033a0204012a02
             (None, None)
          names      ('__name__', '__module__', '__qualname__', 'staticmethod', 'Optional', 'Union', 'Button', 'ReplyButton', 'bool', 'InlineKeyboardBuilder', 'ReplyKeyboardBuilder', '_get_builder', 'Row', 'int', 'InlineKeyboardMarkup', 'ReplyKeyboardMarkup', '__call__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\work\\usefulgram\\usefulgram\\keyboard\\builder.py'
          name       '_Builder'
-         firstlineno 107
+         firstlineno 130
          lnotab
             0x0a010202020102fe04011eff02020efe020312fd06ff0e01020f020102
             ff1a0102ff020212fe
       '_Builder'
       None
    names      ('typing', 'Optional', 'Any', 'Union', 'datetime', 'date', 'time', 'aiogram.types', 'InlineKeyboardButton', 'InlineKeyboardMarkup', 'KeyboardButton', 'ReplyKeyboardMarkup', 'aiogram.utils.keyboard', 'InlineKeyboardBuilder', 'ReplyKeyboardBuilder', 'usefulgram.parsing.encode', 'CallbackData', 'usefulgram.exceptions', 'DifferentButtonsInMatrix', 'UnknownButtonType', 'NoOneButtonParamIsFilled', 'usefulgram.utils', 'autorepr', 'object', 'type', 'check_buttons_type', 'Button', 'ReplyButton', 'Row', '_Builder', 'Builder')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\work\\usefulgram\\usefulgram\\keyboard\\builder.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020214021402180410020c0114050c0310051a2b1a0f1a171a28
+   lnotab 0x00ff020214021402180410020c0114050c0310051a421a0f1a171a28
```

### Comparing `usefulgram-0.0.0a2/usefulgram/keyboard/builder.py` & `usefulgram-0.0.0a3/usefulgram/keyboard/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,214 +54,250 @@
 00000350: 2020 2064 6174 652c 2074 696d 652c 206f     date, time, o
 00000360: 626a 6563 745d 2c20 2e2e 2e5d 0d0a 2020  bject], ...]..  
 00000370: 2020 6f74 6865 723a 2064 6963 745b 7374    other: dict[st
 00000380: 722c 2041 6e79 5d0d 0a20 2020 2073 6570  r, Any]..    sep
 00000390: 6172 6174 6f72 3a20 7374 720d 0a0d 0a20  arator: str.... 
 000003a0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
 000003b0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-000003c0: 6c66 2c20 7465 7874 3a20 7374 722c 2070  lf, text: str, p
-000003d0: 7265 6669 783a 204f 7074 696f 6e61 6c5b  refix: Optional[
-000003e0: 7374 725d 203d 204e 6f6e 652c 0d0a 2020  str] = None,..  
-000003f0: 2020 2020 2020 2020 2020 2a61 7267 733a            *args:
-00000400: 2055 6e69 6f6e 5b73 7472 2c20 696e 742c   Union[str, int,
-00000410: 2062 6f6f 6c2c 204e 6f6e 652c 2064 6174   bool, None, dat
-00000420: 6574 696d 652c 2064 6174 652c 2074 696d  etime, date, tim
-00000430: 652c 206f 626a 6563 745d 2c0d 0a20 2020  e, object],..   
-00000440: 2020 2020 2020 2020 2075 726c 3a20 4f70           url: Op
-00000450: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00000460: 6e65 2c20 7365 7061 7261 746f 723a 2073  ne, separator: s
-00000470: 7472 203d 2022 2f22 2c0d 0a20 2020 2020  tr = "/",..     
-00000480: 2020 2020 2020 202a 2a6b 7761 7267 733a         **kwargs:
-00000490: 2064 6963 745b 7374 722c 2041 6e79 5d0d   dict[str, Any].
-000004a0: 0a20 2020 2020 2020 2020 2020 2029 3a0d  .            ):.
-000004b0: 0a0d 0a20 2020 2020 2020 2069 6620 6e6f  ...        if no
-000004c0: 7420 616e 7928 2870 7265 6669 782c 2075  t any((prefix, u
-000004d0: 726c 2c20 6b77 6172 6773 2929 3a0d 0a20  rl, kwargs)):.. 
-000004e0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000004f0: 204e 6f4f 6e65 4275 7474 6f6e 5061 7261   NoOneButtonPara
-00000500: 6d49 7346 696c 6c65 640d 0a0d 0a20 2020  mIsFilled....   
-00000510: 2020 2020 2073 656c 662e 7465 7874 203d       self.text =
-00000520: 2074 6578 740d 0a20 2020 2020 2020 2073   text..        s
-00000530: 656c 662e 7072 6566 6978 203d 2070 7265  elf.prefix = pre
-00000540: 6669 780d 0a20 2020 2020 2020 2073 656c  fix..        sel
-00000550: 662e 7572 6c20 3d20 7572 6c0d 0a20 2020  f.url = url..   
-00000560: 2020 2020 2073 656c 662e 6164 6469 7469       self.additi
-00000570: 6f6e 616c 203d 2061 7267 730d 0a20 2020  onal = args..   
-00000580: 2020 2020 2073 656c 662e 6f74 6865 7220       self.other 
-00000590: 3d20 6b77 6172 6773 0d0a 2020 2020 2020  = kwargs..      
-000005a0: 2020 7365 6c66 2e73 6570 6172 6174 6f72    self.separator
-000005b0: 203d 2073 6570 6172 6174 6f72 0d0a 0d0a   = separator....
-000005c0: 2020 2020 6465 6620 5f5f 7265 7072 5f5f      def __repr__
-000005d0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-000005e0: 2072 6574 7572 6e20 6175 746f 7265 7072   return autorepr
-000005f0: 2873 656c 6629 0d0a 0d0a 2020 2020 6465  (self)....    de
-00000600: 6620 6765 745f 6275 7474 6f6e 7328 7365  f get_buttons(se
-00000610: 6c66 2920 2d3e 2049 6e6c 696e 654b 6579  lf) -> InlineKey
-00000620: 626f 6172 6442 7574 746f 6e3a 0d0a 2020  boardButton:..  
-00000630: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-00000640: 6566 6978 2069 7320 6e6f 7420 4e6f 6e65  efix is not None
-00000650: 3a0d 0a20 2020 2020 2020 2020 2020 2063  :..            c
-00000660: 616c 6c62 6163 6b5f 6461 7461 203d 2043  allback_data = C
-00000670: 616c 6c62 6163 6b44 6174 6128 0d0a 2020  allbackData(..  
-00000680: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00000690: 6c66 2e70 7265 6669 782c 202a 7365 6c66  lf.prefix, *self
-000006a0: 2e61 6464 6974 696f 6e61 6c2c 0d0a 2020  .additional,..  
-000006b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000006c0: 7061 7261 746f 723d 7365 6c66 2e73 6570  parator=self.sep
-000006d0: 6172 6174 6f72 290d 0a0d 0a20 2020 2020  arator)....     
-000006e0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-000006f0: 2020 2020 2020 6361 6c6c 6261 636b 5f64        callback_d
-00000700: 6174 6120 3d20 4e6f 6e65 0d0a 0d0a 2020  ata = None....  
-00000710: 2020 2020 2020 7265 7475 726e 2049 6e6c        return Inl
-00000720: 696e 654b 6579 626f 6172 6442 7574 746f  ineKeyboardButto
-00000730: 6e28 7465 7874 3d73 656c 662e 7465 7874  n(text=self.text
-00000740: 2c20 7572 6c3d 7365 6c66 2e75 726c 2c0d  , url=self.url,.
-00000750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000770: 2020 2020 2063 616c 6c62 6163 6b5f 6461       callback_da
-00000780: 7461 3d63 616c 6c62 6163 6b5f 6461 7461  ta=callback_data
-00000790: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000007a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007b0: 2020 2020 2020 202a 2a73 656c 662e 6f74         **self.ot
-000007c0: 6865 7229 0d0a 0d0a 0d0a 636c 6173 7320  her)......class 
-000007d0: 5265 706c 7942 7574 746f 6e3a 0d0a 2020  ReplyButton:..  
-000007e0: 2020 7465 7874 3a20 7374 720d 0a20 2020    text: str..   
-000007f0: 206f 7468 6572 3a20 6469 6374 5b73 7472   other: dict[str
-00000800: 2c20 416e 795d 0d0a 0d0a 2020 2020 6465  , Any]....    de
-00000810: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00000820: 2074 6578 743a 2073 7472 2c20 2a2a 6b77   text: str, **kw
-00000830: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
-00000840: 7365 6c66 2e74 6578 7420 3d20 7465 7874  self.text = text
-00000850: 0d0a 2020 2020 2020 2020 7365 6c66 2e6f  ..        self.o
-00000860: 7468 6572 203d 206b 7761 7267 730d 0a0d  ther = kwargs...
-00000870: 0a20 2020 2064 6566 205f 5f72 6570 725f  .    def __repr_
-00000880: 5f28 7365 6c66 293a 0d0a 2020 2020 2020  _(self):..      
-00000890: 2020 7265 7475 726e 2061 7574 6f72 6570    return autorep
-000008a0: 7228 7365 6c66 290d 0a0d 0a20 2020 2064  r(self)....    d
-000008b0: 6566 2067 6574 5f62 7574 746f 6e73 2873  ef get_buttons(s
-000008c0: 656c 6629 202d 3e20 4b65 7962 6f61 7264  elf) -> Keyboard
-000008d0: 4275 7474 6f6e 3a0d 0a20 2020 2020 2020  Button:..       
-000008e0: 2072 6574 7572 6e20 4b65 7962 6f61 7264   return Keyboard
-000008f0: 4275 7474 6f6e 2874 6578 743d 7365 6c66  Button(text=self
-00000900: 2e74 6578 742c 202a 2a73 656c 662e 6f74  .text, **self.ot
-00000910: 6865 7229 0d0a 0d0a 0d0a 636c 6173 7320  her)......class 
-00000920: 526f 773a 0d0a 2020 2020 6275 7474 6f6e  Row:..    button
-00000930: 733a 2055 6e69 6f6e 5b6c 6973 745b 496e  s: Union[list[In
-00000940: 6c69 6e65 4b65 7962 6f61 7264 4275 7474  lineKeyboardButt
-00000950: 6f6e 5d2c 206c 6973 745b 4b65 7962 6f61  on], list[Keyboa
-00000960: 7264 4275 7474 6f6e 5d5d 0d0a 2020 2020  rdButton]]..    
-00000970: 6669 7273 745f 6275 7474 6f6e 5f69 6e73  first_button_ins
-00000980: 7461 6e63 653a 2055 6e69 6f6e 5b42 7574  tance: Union[But
-00000990: 746f 6e2c 2052 6570 6c79 4275 7474 6f6e  ton, ReplyButton
-000009a0: 5d0d 0a0d 0a20 2020 2064 6566 205f 5f69  ]....    def __i
-000009b0: 6e69 745f 5f28 7365 6c66 2c20 2a61 7267  nit__(self, *arg
-000009c0: 733a 2055 6e69 6f6e 5b52 6570 6c79 4275  s: Union[ReplyBu
-000009d0: 7474 6f6e 2c20 4275 7474 6f6e 5d29 3a0d  tton, Button]):.
-000009e0: 0a20 2020 2020 2020 2073 656c 662e 6275  .        self.bu
-000009f0: 7474 6f6e 7320 3d20 5b5d 0d0a 0d0a 2020  ttons = []....  
-00000a00: 2020 2020 2020 6669 7273 745f 6275 7474        first_butt
-00000a10: 6f6e 203d 2061 7267 735b 305d 0d0a 0d0a  on = args[0]....
-00000a20: 2020 2020 2020 2020 7365 6c66 2e66 6972          self.fir
-00000a30: 7374 5f62 7574 746f 6e5f 696e 7374 616e  st_button_instan
-00000a40: 6365 203d 2066 6972 7374 5f62 7574 746f  ce = first_butto
-00000a50: 6e0d 0a0d 0a20 2020 2020 2020 2066 6f72  n....        for
-00000a60: 2062 7574 746f 6e20 696e 2061 7267 733a   button in args:
-00000a70: 0d0a 2020 2020 2020 2020 2020 2020 6368  ..            ch
-00000a80: 6563 6b5f 6275 7474 6f6e 735f 7479 7065  eck_buttons_type
-00000a90: 2862 7574 746f 6e2c 2074 7970 6528 6669  (button, type(fi
-00000aa0: 7273 745f 6275 7474 6f6e 2929 0d0a 0d0a  rst_button))....
-00000ab0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00000ac0: 2e62 7574 746f 6e73 2e61 7070 656e 6428  .buttons.append(
-00000ad0: 6275 7474 6f6e 2e67 6574 5f62 7574 746f  button.get_butto
-00000ae0: 6e73 2829 290d 0a0d 0a20 2020 2064 6566  ns())....    def
-00000af0: 205f 5f72 6570 725f 5f28 7365 6c66 293a   __repr__(self):
-00000b00: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00000b10: 2061 7574 6f72 6570 7228 7365 6c66 290d   autorepr(self).
-00000b20: 0a0d 0a20 2020 2064 6566 2067 6574 5f72  ...    def get_r
-00000b30: 6f77 7328 7365 6c66 2920 2d3e 206c 6973  ows(self) -> lis
-00000b40: 745b 496e 6c69 6e65 4b65 7962 6f61 7264  t[InlineKeyboard
-00000b50: 4275 7474 6f6e 5d3a 0d0a 2020 2020 2020  Button]:..      
-00000b60: 2020 7265 7475 726e 2073 656c 662e 6275    return self.bu
-00000b70: 7474 6f6e 730d 0a0d 0a0d 0a63 6c61 7373  ttons......class
-00000b80: 205f 4275 696c 6465 723a 0d0a 2020 2020   _Builder:..    
-00000b90: 4073 7461 7469 636d 6574 686f 640d 0a20  @staticmethod.. 
-00000ba0: 2020 2064 6566 205f 6765 745f 6275 696c     def _get_buil
-00000bb0: 6465 7228 0d0a 2020 2020 2020 2020 2020  der(..          
-00000bc0: 2020 6669 7273 745f 726f 775f 6275 7474    first_row_butt
-00000bd0: 6f6e 5f69 6e73 3a20 4f70 7469 6f6e 616c  on_ins: Optional
-00000be0: 5b55 6e69 6f6e 5b42 7574 746f 6e2c 2052  [Union[Button, R
-00000bf0: 6570 6c79 4275 7474 6f6e 5d5d 203d 204e  eplyButton]] = N
-00000c00: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
-00000c10: 2020 6973 5f63 616c 6c62 6163 6b3a 204f    is_callback: O
-00000c20: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
-00000c30: 4e6f 6e65 0d0a 2020 2020 2920 2d3e 2055  None..    ) -> U
-00000c40: 6e69 6f6e 5b49 6e6c 696e 654b 6579 626f  nion[InlineKeybo
-00000c50: 6172 6442 7569 6c64 6572 2c20 5265 706c  ardBuilder, Repl
-00000c60: 794b 6579 626f 6172 6442 7569 6c64 6572  yKeyboardBuilder
-00000c70: 5d3a 0d0a 0d0a 2020 2020 2020 2020 6966  ]:....        if
-00000c80: 2069 7369 6e73 7461 6e63 6528 6669 7273   isinstance(firs
-00000c90: 745f 726f 775f 6275 7474 6f6e 5f69 6e73  t_row_button_ins
-00000ca0: 2c20 4275 7474 6f6e 2920 6f72 2069 735f  , Button) or is_
-00000cb0: 6361 6c6c 6261 636b 2069 7320 5472 7565  callback is True
-00000cc0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00000cd0: 6574 7572 6e20 496e 6c69 6e65 4b65 7962  eturn InlineKeyb
-00000ce0: 6f61 7264 4275 696c 6465 7228 290d 0a0d  oardBuilder()...
-00000cf0: 0a20 2020 2020 2020 2069 6620 2869 7369  .        if (isi
-00000d00: 6e73 7461 6e63 6528 6669 7273 745f 726f  nstance(first_ro
-00000d10: 775f 6275 7474 6f6e 5f69 6e73 2c20 5265  w_button_ins, Re
-00000d20: 706c 7942 7574 746f 6e29 0d0a 2020 2020  plyButton)..    
-00000d30: 2020 2020 2020 2020 2020 2020 6f72 2069              or i
-00000d40: 735f 6361 6c6c 6261 636b 2069 7320 4661  s_callback is Fa
-00000d50: 6c73 6529 3a0d 0a0d 0a20 2020 2020 2020  lse):....       
-00000d60: 2020 2020 2072 6574 7572 6e20 5265 706c       return Repl
-00000d70: 794b 6579 626f 6172 6442 7569 6c64 6572  yKeyboardBuilder
-00000d80: 2829 0d0a 0d0a 2020 2020 2020 2020 7261  ()....        ra
-00000d90: 6973 6520 556e 6b6e 6f77 6e42 7574 746f  ise UnknownButto
-00000da0: 6e54 7970 650d 0a0d 0a20 2020 2064 6566  nType....    def
-00000db0: 205f 5f63 616c 6c5f 5f28 7365 6c66 2c20   __call__(self, 
-00000dc0: 2a72 6f77 733a 2052 6f77 2c20 6164 6a75  *rows: Row, adju
-00000dd0: 7374 3a20 4f70 7469 6f6e 616c 5b69 6e74  st: Optional[int
-00000de0: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
-00000df0: 2020 2020 2020 2020 2020 2020 6973 5f63              is_c
-00000e00: 616c 6c62 6163 6b3a 2062 6f6f 6c20 3d20  allback: bool = 
-00000e10: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
-00000e20: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
-00000e30: 2920 2d3e 2055 6e69 6f6e 5b49 6e6c 696e  ) -> Union[Inlin
-00000e40: 654b 6579 626f 6172 644d 6172 6b75 702c  eKeyboardMarkup,
-00000e50: 2052 6570 6c79 4b65 7962 6f61 7264 4d61   ReplyKeyboardMa
-00000e60: 726b 7570 5d3a 0d0a 0d0a 2020 2020 2020  rkup]:....      
-00000e70: 2020 6966 206c 656e 2872 6f77 7329 203d    if len(rows) =
-00000e80: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
-00000e90: 2020 7265 7475 726e 2073 656c 662e 5f67    return self._g
-00000ea0: 6574 5f62 7569 6c64 6572 2869 735f 6361  et_builder(is_ca
-00000eb0: 6c6c 6261 636b 3d69 735f 6361 6c6c 6261  llback=is_callba
-00000ec0: 636b 292e 6173 5f6d 6172 6b75 7028 290d  ck).as_markup().
-00000ed0: 0a0d 0a20 2020 2020 2020 2066 6972 7374  ...        first
-00000ee0: 5f72 6f77 5f62 7574 746f 6e5f 696e 7374  _row_button_inst
-00000ef0: 616e 6365 203d 2072 6f77 735b 305d 2e66  ance = rows[0].f
-00000f00: 6972 7374 5f62 7574 746f 6e5f 696e 7374  irst_button_inst
-00000f10: 616e 6365 0d0a 0d0a 2020 2020 2020 2020  ance....        
-00000f20: 6275 696c 6465 7220 3d20 7365 6c66 2e5f  builder = self._
-00000f30: 6765 745f 6275 696c 6465 7228 6669 7273  get_builder(firs
-00000f40: 745f 726f 775f 6275 7474 6f6e 5f69 6e73  t_row_button_ins
-00000f50: 7461 6e63 6529 0d0a 0d0a 2020 2020 2020  tance)....      
-00000f60: 2020 666f 7220 726f 7720 696e 2072 6f77    for row in row
-00000f70: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00000f80: 6368 6563 6b5f 6275 7474 6f6e 735f 7479  check_buttons_ty
-00000f90: 7065 2872 6f77 2e66 6972 7374 5f62 7574  pe(row.first_but
-00000fa0: 746f 6e5f 696e 7374 616e 6365 2c0d 0a20  ton_instance,.. 
-00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fc0: 2020 2020 2020 2020 2020 2020 2020 7479                ty
-00000fd0: 7065 2866 6972 7374 5f72 6f77 5f62 7574  pe(first_row_but
-00000fe0: 746f 6e5f 696e 7374 616e 6365 2929 0d0a  ton_instance))..
-00000ff0: 0d0a 2020 2020 2020 2020 2020 2020 6275  ..            bu
-00001000: 696c 6465 722e 726f 7728 2a72 6f77 2e67  ilder.row(*row.g
-00001010: 6574 5f72 6f77 7328 2929 0d0a 0d0a 2020  et_rows())....  
-00001020: 2020 2020 2020 6966 2061 646a 7573 7420        if adjust 
-00001030: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-00001040: 2020 2020 2020 2020 2020 6275 696c 6465            builde
-00001050: 722e 6164 6a75 7374 2861 646a 7573 7429  r.adjust(adjust)
-00001060: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
-00001070: 726e 2062 7569 6c64 6572 2e61 735f 6d61  rn builder.as_ma
-00001080: 726b 7570 282a 2a6b 7761 7267 7329 0d0a  rkup(**kwargs)..
-00001090: 0d0a 0d0a 4275 696c 6465 7220 3d20 5f42  ....Builder = _B
-000010a0: 7569 6c64 6572 2829 0d0a                 uilder()..
+000003c0: 6c66 2c20 7465 7874 3a20 556e 696f 6e5b  lf, text: Union[
+000003d0: 7374 722c 2069 6e74 5d2c 0d0a 2020 2020  str, int],..    
+000003e0: 2020 2020 2020 2020 2a61 7267 733a 2055          *args: U
+000003f0: 6e69 6f6e 5b73 7472 2c20 696e 742c 2062  nion[str, int, b
+00000400: 6f6f 6c2c 204e 6f6e 652c 2064 6174 6574  ool, None, datet
+00000410: 696d 652c 2064 6174 652c 2074 696d 652c  ime, date, time,
+00000420: 206f 626a 6563 745d 2c0d 0a20 2020 2020   object],..     
+00000430: 2020 2020 2020 2070 7265 6669 783a 204f         prefix: O
+00000440: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00000450: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
+00000460: 2020 7572 6c3a 204f 7074 696f 6e61 6c5b    url: Optional[
+00000470: 7374 725d 203d 204e 6f6e 652c 2073 6570  str] = None, sep
+00000480: 6172 6174 6f72 3a20 7374 7220 3d20 222f  arator: str = "/
+00000490: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000004a0: 2a2a 6b77 6172 6773 3a20 6469 6374 5b73  **kwargs: dict[s
+000004b0: 7472 2c20 416e 795d 0d0a 2020 2020 2020  tr, Any]..      
+000004c0: 2020 2020 2020 293a 0d0a 0d0a 2020 2020        ):....    
+000004d0: 2020 2020 7072 6566 6978 203d 2073 656c      prefix = sel
+000004e0: 662e 5f67 6574 5f70 7265 6669 7828 7072  f._get_prefix(pr
+000004f0: 6566 6978 2c20 6172 6773 290d 0a0d 0a20  efix, args).... 
+00000500: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00000510: 616e 6365 2874 6578 742c 2069 6e74 293a  ance(text, int):
+00000520: 0d0a 2020 2020 2020 2020 2020 2020 7465  ..            te
+00000530: 7874 203d 2073 7472 2874 6578 7429 0d0a  xt = str(text)..
+00000540: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+00000550: 2061 6e79 2828 7072 6566 6978 2c20 7572   any((prefix, ur
+00000560: 6c2c 206b 7761 7267 7329 293a 0d0a 2020  l, kwargs)):..  
+00000570: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00000580: 4e6f 4f6e 6542 7574 746f 6e50 6172 616d  NoOneButtonParam
+00000590: 4973 4669 6c6c 6564 0d0a 0d0a 2020 2020  IsFilled....    
+000005a0: 2020 2020 7365 6c66 2e74 6578 7420 3d20      self.text = 
+000005b0: 7465 7874 0d0a 2020 2020 2020 2020 7365  text..        se
+000005c0: 6c66 2e70 7265 6669 7820 3d20 7072 6566  lf.prefix = pref
+000005d0: 6978 0d0a 2020 2020 2020 2020 7365 6c66  ix..        self
+000005e0: 2e75 726c 203d 2075 726c 0d0a 2020 2020  .url = url..    
+000005f0: 2020 2020 7365 6c66 2e61 6464 6974 696f      self.additio
+00000600: 6e61 6c20 3d20 6172 6773 0d0a 2020 2020  nal = args..    
+00000610: 2020 2020 7365 6c66 2e6f 7468 6572 203d      self.other =
+00000620: 206b 7761 7267 730d 0a20 2020 2020 2020   kwargs..       
+00000630: 2073 656c 662e 7365 7061 7261 746f 7220   self.separator 
+00000640: 3d20 7365 7061 7261 746f 720d 0a0d 0a20  = separator.... 
+00000650: 2020 2064 6566 205f 5f72 6570 725f 5f28     def __repr__(
+00000660: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00000670: 7265 7475 726e 2061 7574 6f72 6570 7228  return autorepr(
+00000680: 7365 6c66 290d 0a0d 0a20 2020 2040 7374  self)....    @st
+00000690: 6174 6963 6d65 7468 6f64 0d0a 2020 2020  aticmethod..    
+000006a0: 6465 6620 5f67 6574 5f70 7265 6669 7828  def _get_prefix(
+000006b0: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+000006c0: 6566 6978 3a20 4f70 7469 6f6e 616c 5b73  efix: Optional[s
+000006d0: 7472 5d2c 0d0a 2020 2020 2020 2020 2020  tr],..          
+000006e0: 2020 6172 6773 3a20 7475 706c 655b 556e    args: tuple[Un
+000006f0: 696f 6e5b 7374 722c 2069 6e74 2c20 626f  ion[str, int, bo
+00000700: 6f6c 2c20 4e6f 6e65 2c20 6461 7465 7469  ol, None, dateti
+00000710: 6d65 2c20 6461 7465 2c20 7469 6d65 2c20  me, date, time, 
+00000720: 6f62 6a65 6374 5d2c 202e 2e2e 5d0d 0a20  object], ...].. 
+00000730: 2020 2029 202d 3e20 4f70 7469 6f6e 616c     ) -> Optional
+00000740: 5b73 7472 5d3a 0d0a 0d0a 2020 2020 2020  [str]:....      
+00000750: 2020 6966 2070 7265 6669 7820 6973 206e    if prefix is n
+00000760: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00000770: 2020 2020 2020 7265 7475 726e 2070 7265        return pre
+00000780: 6669 780d 0a0d 0a20 2020 2020 2020 2066  fix....        f
+00000790: 6f72 206f 626a 2069 6e20 6172 6773 3a0d  or obj in args:.
+000007a0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000007b0: 756c 7420 3d20 6f62 6a2e 5f5f 6765 7461  ult = obj.__geta
+000007c0: 7474 7269 6275 7465 5f5f 2822 7072 6566  ttribute__("pref
+000007d0: 6978 2229 0d0a 0d0a 2020 2020 2020 2020  ix")....        
+000007e0: 2020 2020 6966 2072 6573 756c 7420 6973      if result is
+000007f0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00000800: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00000810: 726e 2072 6573 756c 740d 0a0d 0a20 2020  rn result....   
+00000820: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00000830: 0d0a 0d0a 2020 2020 6465 6620 6765 745f  ....    def get_
+00000840: 6275 7474 6f6e 7328 7365 6c66 2920 2d3e  buttons(self) ->
+00000850: 2049 6e6c 696e 654b 6579 626f 6172 6442   InlineKeyboardB
+00000860: 7574 746f 6e3a 0d0a 2020 2020 2020 2020  utton:..        
+00000870: 6966 2073 656c 662e 7072 6566 6978 2069  if self.prefix i
+00000880: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+00000890: 2020 2020 2020 2020 2063 616c 6c62 6163           callbac
+000008a0: 6b5f 6461 7461 203d 2043 616c 6c62 6163  k_data = Callbac
+000008b0: 6b44 6174 6128 0d0a 2020 2020 2020 2020  kData(..        
+000008c0: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+000008d0: 6669 782c 202a 7365 6c66 2e61 6464 6974  fix, *self.addit
+000008e0: 696f 6e61 6c2c 0d0a 2020 2020 2020 2020  ional,..        
+000008f0: 2020 2020 2020 2020 7365 7061 7261 746f          separato
+00000900: 723d 7365 6c66 2e73 6570 6172 6174 6f72  r=self.separator
+00000910: 290d 0a0d 0a20 2020 2020 2020 2065 6c73  )....        els
+00000920: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00000930: 6361 6c6c 6261 636b 5f64 6174 6120 3d20  callback_data = 
+00000940: 4e6f 6e65 0d0a 0d0a 2020 2020 2020 2020  None....        
+00000950: 7265 7475 726e 2049 6e6c 696e 654b 6579  return InlineKey
+00000960: 626f 6172 6442 7574 746f 6e28 7465 7874  boardButton(text
+00000970: 3d73 656c 662e 7465 7874 2c20 7572 6c3d  =self.text, url=
+00000980: 7365 6c66 2e75 726c 2c0d 0a20 2020 2020  self.url,..     
+00000990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000009b0: 616c 6c62 6163 6b5f 6461 7461 3d63 616c  allback_data=cal
+000009c0: 6c62 6163 6b5f 6461 7461 2c0d 0a20 2020  lback_data,..   
+000009d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009f0: 202a 2a73 656c 662e 6f74 6865 7229 0d0a   **self.other)..
+00000a00: 0d0a 0d0a 636c 6173 7320 5265 706c 7942  ....class ReplyB
+00000a10: 7574 746f 6e3a 0d0a 2020 2020 7465 7874  utton:..    text
+00000a20: 3a20 7374 720d 0a20 2020 206f 7468 6572  : str..    other
+00000a30: 3a20 6469 6374 5b73 7472 2c20 416e 795d  : dict[str, Any]
+00000a40: 0d0a 0d0a 2020 2020 6465 6620 5f5f 696e  ....    def __in
+00000a50: 6974 5f5f 2873 656c 662c 2074 6578 743a  it__(self, text:
+00000a60: 2073 7472 2c20 2a2a 6b77 6172 6773 293a   str, **kwargs):
+00000a70: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+00000a80: 6578 7420 3d20 7465 7874 0d0a 2020 2020  ext = text..    
+00000a90: 2020 2020 7365 6c66 2e6f 7468 6572 203d      self.other =
+00000aa0: 206b 7761 7267 730d 0a0d 0a20 2020 2064   kwargs....    d
+00000ab0: 6566 205f 5f72 6570 725f 5f28 7365 6c66  ef __repr__(self
+00000ac0: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
+00000ad0: 726e 2061 7574 6f72 6570 7228 7365 6c66  rn autorepr(self
+00000ae0: 290d 0a0d 0a20 2020 2064 6566 2067 6574  )....    def get
+00000af0: 5f62 7574 746f 6e73 2873 656c 6629 202d  _buttons(self) -
+00000b00: 3e20 4b65 7962 6f61 7264 4275 7474 6f6e  > KeyboardButton
+00000b10: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+00000b20: 6e20 4b65 7962 6f61 7264 4275 7474 6f6e  n KeyboardButton
+00000b30: 2874 6578 743d 7365 6c66 2e74 6578 742c  (text=self.text,
+00000b40: 202a 2a73 656c 662e 6f74 6865 7229 0d0a   **self.other)..
+00000b50: 0d0a 0d0a 636c 6173 7320 526f 773a 0d0a  ....class Row:..
+00000b60: 2020 2020 6275 7474 6f6e 733a 2055 6e69      buttons: Uni
+00000b70: 6f6e 5b6c 6973 745b 496e 6c69 6e65 4b65  on[list[InlineKe
+00000b80: 7962 6f61 7264 4275 7474 6f6e 5d2c 206c  yboardButton], l
+00000b90: 6973 745b 4b65 7962 6f61 7264 4275 7474  ist[KeyboardButt
+00000ba0: 6f6e 5d5d 0d0a 2020 2020 6669 7273 745f  on]]..    first_
+00000bb0: 6275 7474 6f6e 5f69 6e73 7461 6e63 653a  button_instance:
+00000bc0: 2055 6e69 6f6e 5b42 7574 746f 6e2c 2052   Union[Button, R
+00000bd0: 6570 6c79 4275 7474 6f6e 5d0d 0a0d 0a20  eplyButton].... 
+00000be0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00000bf0: 7365 6c66 2c20 2a61 7267 733a 2055 6e69  self, *args: Uni
+00000c00: 6f6e 5b52 6570 6c79 4275 7474 6f6e 2c20  on[ReplyButton, 
+00000c10: 4275 7474 6f6e 5d29 3a0d 0a20 2020 2020  Button]):..     
+00000c20: 2020 2073 656c 662e 6275 7474 6f6e 7320     self.buttons 
+00000c30: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00000c40: 6669 7273 745f 6275 7474 6f6e 203d 2061  first_button = a
+00000c50: 7267 735b 305d 0d0a 0d0a 2020 2020 2020  rgs[0]....      
+00000c60: 2020 7365 6c66 2e66 6972 7374 5f62 7574    self.first_but
+00000c70: 746f 6e5f 696e 7374 616e 6365 203d 2066  ton_instance = f
+00000c80: 6972 7374 5f62 7574 746f 6e0d 0a0d 0a20  irst_button.... 
+00000c90: 2020 2020 2020 2066 6f72 2062 7574 746f         for butto
+00000ca0: 6e20 696e 2061 7267 733a 0d0a 2020 2020  n in args:..    
+00000cb0: 2020 2020 2020 2020 6368 6563 6b5f 6275          check_bu
+00000cc0: 7474 6f6e 735f 7479 7065 2862 7574 746f  ttons_type(butto
+00000cd0: 6e2c 2074 7970 6528 6669 7273 745f 6275  n, type(first_bu
+00000ce0: 7474 6f6e 2929 0d0a 0d0a 2020 2020 2020  tton))....      
+00000cf0: 2020 2020 2020 7365 6c66 2e62 7574 746f        self.butto
+00000d00: 6e73 2e61 7070 656e 6428 6275 7474 6f6e  ns.append(button
+00000d10: 2e67 6574 5f62 7574 746f 6e73 2829 290d  .get_buttons()).
+00000d20: 0a0d 0a20 2020 2064 6566 205f 5f72 6570  ...    def __rep
+00000d30: 725f 5f28 7365 6c66 293a 0d0a 2020 2020  r__(self):..    
+00000d40: 2020 2020 7265 7475 726e 2061 7574 6f72      return autor
+00000d50: 6570 7228 7365 6c66 290d 0a0d 0a20 2020  epr(self)....   
+00000d60: 2064 6566 2067 6574 5f72 6f77 7328 7365   def get_rows(se
+00000d70: 6c66 2920 2d3e 206c 6973 745b 496e 6c69  lf) -> list[Inli
+00000d80: 6e65 4b65 7962 6f61 7264 4275 7474 6f6e  neKeyboardButton
+00000d90: 5d3a 0d0a 2020 2020 2020 2020 7265 7475  ]:..        retu
+00000da0: 726e 2073 656c 662e 6275 7474 6f6e 730d  rn self.buttons.
+00000db0: 0a0d 0a0d 0a63 6c61 7373 205f 4275 696c  .....class _Buil
+00000dc0: 6465 723a 0d0a 2020 2020 4073 7461 7469  der:..    @stati
+00000dd0: 636d 6574 686f 640d 0a20 2020 2064 6566  cmethod..    def
+00000de0: 205f 6765 745f 6275 696c 6465 7228 0d0a   _get_builder(..
+00000df0: 2020 2020 2020 2020 2020 2020 6669 7273              firs
+00000e00: 745f 726f 775f 6275 7474 6f6e 5f69 6e73  t_row_button_ins
+00000e10: 3a20 4f70 7469 6f6e 616c 5b55 6e69 6f6e  : Optional[Union
+00000e20: 5b42 7574 746f 6e2c 2052 6570 6c79 4275  [Button, ReplyBu
+00000e30: 7474 6f6e 5d5d 203d 204e 6f6e 652c 0d0a  tton]] = None,..
+00000e40: 2020 2020 2020 2020 2020 2020 6973 5f63              is_c
+00000e50: 616c 6c62 6163 6b3a 204f 7074 696f 6e61  allback: Optiona
+00000e60: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0d0a  l[bool] = None..
+00000e70: 2020 2020 2920 2d3e 2055 6e69 6f6e 5b49      ) -> Union[I
+00000e80: 6e6c 696e 654b 6579 626f 6172 6442 7569  nlineKeyboardBui
+00000e90: 6c64 6572 2c20 5265 706c 794b 6579 626f  lder, ReplyKeybo
+00000ea0: 6172 6442 7569 6c64 6572 5d3a 0d0a 0d0a  ardBuilder]:....
+00000eb0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00000ec0: 7461 6e63 6528 6669 7273 745f 726f 775f  tance(first_row_
+00000ed0: 6275 7474 6f6e 5f69 6e73 2c20 4275 7474  button_ins, Butt
+00000ee0: 6f6e 2920 6f72 2069 735f 6361 6c6c 6261  on) or is_callba
+00000ef0: 636b 2069 7320 5472 7565 3a0d 0a20 2020  ck is True:..   
+00000f00: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00000f10: 496e 6c69 6e65 4b65 7962 6f61 7264 4275  InlineKeyboardBu
+00000f20: 696c 6465 7228 290d 0a0d 0a20 2020 2020  ilder()....     
+00000f30: 2020 2069 6620 2869 7369 6e73 7461 6e63     if (isinstanc
+00000f40: 6528 6669 7273 745f 726f 775f 6275 7474  e(first_row_butt
+00000f50: 6f6e 5f69 6e73 2c20 5265 706c 7942 7574  on_ins, ReplyBut
+00000f60: 746f 6e29 0d0a 2020 2020 2020 2020 2020  ton)..          
+00000f70: 2020 2020 2020 6f72 2069 735f 6361 6c6c        or is_call
+00000f80: 6261 636b 2069 7320 4661 6c73 6529 3a0d  back is False):.
+00000f90: 0a0d 0a20 2020 2020 2020 2020 2020 2072  ...            r
+00000fa0: 6574 7572 6e20 5265 706c 794b 6579 626f  eturn ReplyKeybo
+00000fb0: 6172 6442 7569 6c64 6572 2829 0d0a 0d0a  ardBuilder()....
+00000fc0: 2020 2020 2020 2020 7261 6973 6520 556e          raise Un
+00000fd0: 6b6e 6f77 6e42 7574 746f 6e54 7970 650d  knownButtonType.
+00000fe0: 0a0d 0a20 2020 2064 6566 205f 5f63 616c  ...    def __cal
+00000ff0: 6c5f 5f28 7365 6c66 2c20 2a72 6f77 733a  l__(self, *rows:
+00001000: 2052 6f77 2c20 6164 6a75 7374 3a20 4f70   Row, adjust: Op
+00001010: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+00001020: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
+00001030: 2020 2020 2020 6973 5f63 616c 6c62 6163        is_callbac
+00001040: 6b3a 2062 6f6f 6c20 3d20 5472 7565 2c0d  k: bool = True,.
+00001050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001060: 2020 2a2a 6b77 6172 6773 2920 2d3e 2055    **kwargs) -> U
+00001070: 6e69 6f6e 5b49 6e6c 696e 654b 6579 626f  nion[InlineKeybo
+00001080: 6172 644d 6172 6b75 702c 2052 6570 6c79  ardMarkup, Reply
+00001090: 4b65 7962 6f61 7264 4d61 726b 7570 5d3a  KeyboardMarkup]:
+000010a0: 0d0a 0d0a 2020 2020 2020 2020 6966 206c  ....        if l
+000010b0: 656e 2872 6f77 7329 203d 3d20 303a 0d0a  en(rows) == 0:..
+000010c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000010d0: 726e 2073 656c 662e 5f67 6574 5f62 7569  rn self._get_bui
+000010e0: 6c64 6572 2869 735f 6361 6c6c 6261 636b  lder(is_callback
+000010f0: 3d69 735f 6361 6c6c 6261 636b 292e 6173  =is_callback).as
+00001100: 5f6d 6172 6b75 7028 290d 0a0d 0a20 2020  _markup()....   
+00001110: 2020 2020 2066 6972 7374 5f72 6f77 5f62       first_row_b
+00001120: 7574 746f 6e5f 696e 7374 616e 6365 203d  utton_instance =
+00001130: 2072 6f77 735b 305d 2e66 6972 7374 5f62   rows[0].first_b
+00001140: 7574 746f 6e5f 696e 7374 616e 6365 0d0a  utton_instance..
+00001150: 0d0a 2020 2020 2020 2020 6275 696c 6465  ..        builde
+00001160: 7220 3d20 7365 6c66 2e5f 6765 745f 6275  r = self._get_bu
+00001170: 696c 6465 7228 6669 7273 745f 726f 775f  ilder(first_row_
+00001180: 6275 7474 6f6e 5f69 6e73 7461 6e63 6529  button_instance)
+00001190: 0d0a 0d0a 2020 2020 2020 2020 666f 7220  ....        for 
+000011a0: 726f 7720 696e 2072 6f77 733a 0d0a 2020  row in rows:..  
+000011b0: 2020 2020 2020 2020 2020 6368 6563 6b5f            check_
+000011c0: 6275 7474 6f6e 735f 7479 7065 2872 6f77  buttons_type(row
+000011d0: 2e66 6972 7374 5f62 7574 746f 6e5f 696e  .first_button_in
+000011e0: 7374 616e 6365 2c0d 0a20 2020 2020 2020  stance,..       
+000011f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001200: 2020 2020 2020 2020 7479 7065 2866 6972          type(fir
+00001210: 7374 5f72 6f77 5f62 7574 746f 6e5f 696e  st_row_button_in
+00001220: 7374 616e 6365 2929 0d0a 0d0a 2020 2020  stance))....    
+00001230: 2020 2020 2020 2020 6275 696c 6465 722e          builder.
+00001240: 726f 7728 2a72 6f77 2e67 6574 5f72 6f77  row(*row.get_row
+00001250: 7328 2929 0d0a 0d0a 2020 2020 2020 2020  s())....        
+00001260: 6966 2061 646a 7573 7420 6973 206e 6f74  if adjust is not
+00001270: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00001280: 2020 2020 6275 696c 6465 722e 6164 6a75      builder.adju
+00001290: 7374 2861 646a 7573 7429 0d0a 0d0a 2020  st(adjust)....  
+000012a0: 2020 2020 2020 7265 7475 726e 2062 7569        return bui
+000012b0: 6c64 6572 2e61 735f 6d61 726b 7570 282a  lder.as_markup(*
+000012c0: 2a6b 7761 7267 7329 0d0a 0d0a 0d0a 4275  *kwargs)......Bu
+000012d0: 696c 6465 7220 3d20 5f42 7569 6c64 6572  ilder = _Builder
+000012e0: 2829 0d0a                                ()..
```

### Comparing `usefulgram-0.0.0a2/usefulgram/lazy/__pycache__/lazy_editing.cpython-310.pyc` & `usefulgram-0.0.0a3/usefulgram/lazy/__pycache__/lazy_editing.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a2/usefulgram/lazy/__pycache__/lazy_editing.cpython-311.pyc` & `usefulgram-0.0.0a3/usefulgram/lazy/__pycache__/lazy_editing.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8c05a864 (Fri Jul  7 12:31:08 2023 UTC)
+moddate:  0xf51eaf64 (Wed Jul 12 21:45:25 2023 UTC)
 files sz: 9580
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
@@ -74,15 +74,15 @@
                102 IMPORT_NAME             17 (aiogram.exceptions)
                104 IMPORT_FROM             18 (TelegramBadRequest)
                106 STORE_NAME              18 (TelegramBadRequest)
                108 POP_TOP
    
     23         110 LOAD_CONST               0 (0)
                112 LOAD_CONST               8 (('Const',))
-               114 IMPORT_NAME             19 (usefulgram.const)
+               114 IMPORT_NAME             19 (usefulgram.enums)
                116 IMPORT_FROM             20 (Const)
                118 STORE_NAME              20 (Const)
                120 POP_TOP
    
     26         122 PUSH_NULL
                124 LOAD_BUILD_CLASS
                126 LOAD_CONST               9 (<code object LazyEditing, file "C:\work\usefulgram\usefulgram\lazy\lazy_editing.py", line 26>)
@@ -1640,15 +1640,15 @@
             010201020102fa040102ff02010eff02020efe02030efd02040efc02050e
             fb020602fa06ff0e01022102030201020102fc040102ff020202fe02030e
             fd020402fc06ff0e01020e0201020102010201020102f9040202fe02020e
             fe02030efd02040efc02050efb02060efa020702f9020802f8081b02011a
             ff0e0102070201020102010201020102010201020102f704010eff02020e
             fe02030efd02040efc02050efb020602fa02070ef9020802f8020902f7
       'LazyEditing'
-   names      ('typing', 'Optional', 'datetime', 'timedelta', 'asyncio', 'contextlib', 'suppress', 'aiogram.types', 'CallbackQuery', 'Message', 'InputMediaPhoto', 'InputMediaVideo', 'FSInputFile', 'InlineKeyboardMarkup', 'UNSET', 'aiogram.enums.chat_type', 'ChatType', 'aiogram.exceptions', 'TelegramBadRequest', 'usefulgram.const', 'Const', 'LazyEditing')
+   names      ('typing', 'Optional', 'datetime', 'timedelta', 'asyncio', 'contextlib', 'suppress', 'aiogram.types', 'CallbackQuery', 'Message', 'InputMediaPhoto', 'InputMediaVideo', 'FSInputFile', 'InlineKeyboardMarkup', 'UNSET', 'aiogram.enums.chat_type', 'ChatType', 'aiogram.exceptions', 'TelegramBadRequest', 'usefulgram.enums', 'Const', 'LazyEditing')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\work\\usefulgram\\usefulgram\\lazy\\lazy_editing.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02030c01100208020c0224090c020c020c03
```

### Comparing `usefulgram-0.0.0a2/usefulgram/lazy/lazy_editing.py` & `usefulgram-0.0.0a3/usefulgram/lazy/lazy_editing.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     InlineKeyboardMarkup,
     UNSET
 )
 from aiogram.enums.chat_type import ChatType
 
 from aiogram.exceptions import TelegramBadRequest
 
-from usefulgram.const import Const
+from usefulgram.enums import Const
 
 
 class LazyEditing:
     callback: CallbackQuery
 
     def __init__(self, callback: CallbackQuery):
         self.callback = callback
```

### Comparing `usefulgram-0.0.0a2/usefulgram/middlewares/__pycache__/stacker.cpython-311.pyc` & `usefulgram-0.0.0a3/usefulgram/middlewares/__pycache__/stacker.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a2/usefulgram/middlewares/__pycache__/trottling.cpython-311.pyc` & `usefulgram-0.0.0a3/usefulgram/middlewares/__pycache__/trottling.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xee19af64 (Wed Jul 12 21:23:58 2023 UTC)
+moddate:  0xf51eaf64 (Wed Jul 12 21:45:25 2023 UTC)
 files sz: 1505
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -57,15 +57,15 @@
                 74 IMPORT_NAME             14 (cachetools)
                 76 IMPORT_FROM             15 (TTLCache)
                 78 STORE_NAME              15 (TTLCache)
                 80 POP_TOP
    
     15          82 LOAD_CONST               1 (0)
                 84 LOAD_CONST               6 (('Const',))
-                86 IMPORT_NAME             16 (usefulgram.const)
+                86 IMPORT_NAME             16 (usefulgram.enums)
                 88 IMPORT_FROM             17 (Const)
                 90 STORE_NAME              17 (Const)
                 92 POP_TOP
    
     18          94 PUSH_NULL
                 96 LOAD_BUILD_CLASS
                 98 LOAD_CONST               7 (<code object ThrottlingMiddleware, file "C:\work\usefulgram\usefulgram\middlewares\trottling.py", line 18>)
@@ -377,15 +377,15 @@
          name       'ThrottlingMiddleware'
          firstlineno 18
          lnotab
             0x0a0104010e021a04020232fe020302fd020412fc02050efb081502010e
             ff0e01
       'ThrottlingMiddleware'
       None
-   names      ('__doc__', 'typing', 'Callable', 'Dict', 'Any', 'Awaitable', 'MutableMapping', 'Optional', 'aiogram', 'BaseMiddleware', 'aiogram.types', 'TelegramObject', 'CallbackQuery', 'User', 'cachetools', 'TTLCache', 'usefulgram.const', 'Const', 'ThrottlingMiddleware')
+   names      ('__doc__', 'typing', 'Callable', 'Dict', 'Any', 'Awaitable', 'MutableMapping', 'Optional', 'aiogram', 'BaseMiddleware', 'aiogram.types', 'TelegramObject', 'CallbackQuery', 'User', 'cachetools', 'TTLCache', 'usefulgram.enums', 'Const', 'ThrottlingMiddleware')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\work\\usefulgram\\usefulgram\\middlewares\\trottling.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff0203040520020c0114020c020c03
```

### Comparing `usefulgram-0.0.0a2/usefulgram/middlewares/stacker.py` & `usefulgram-0.0.0a3/usefulgram/middlewares/stacker.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a2/usefulgram/middlewares/trottling.py` & `usefulgram-0.0.0a3/usefulgram/middlewares/trottling.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Callable, Dict, Any, Awaitable, MutableMapping, Optional
 
 from aiogram import BaseMiddleware
 from aiogram.types import TelegramObject, CallbackQuery, User
 
 from cachetools import TTLCache
 
-from usefulgram.const import Const
+from usefulgram.enums import Const
 
 
 class ThrottlingMiddleware(BaseMiddleware):
     RATE_LIMIT = 0.7
     ANSWER_TEXT = Const.TROTTLING_ANSWER
 
     def __init__(self, rate_limit: float = RATE_LIMIT, answer_text: str = ANSWER_TEXT) -> None:
```

### Comparing `usefulgram-0.0.0a2/usefulgram/parsing/__pycache__/decode.cpython-310.pyc` & `usefulgram-0.0.0a3/usefulgram/parsing/__pycache__/decode.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a2/usefulgram/parsing/__pycache__/decode.cpython-311.pyc` & `usefulgram-0.0.0a3/usefulgram/parsing/__pycache__/decode.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x80a29864 (Sun Jun 25 20:24:32 2023 UTC)
-files sz: 2776
+moddate:  0x4439af64 (Wed Jul 12 23:37:40 2023 UTC)
+files sz: 2803
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d025a026d035a036d
@@ -29,15 +29,15 @@
                 26 STORE_NAME               3 (date)
                 28 IMPORT_FROM              4 (time)
                 30 STORE_NAME               4 (time)
                 32 POP_TOP
    
      6          34 LOAD_CONST               0 (0)
                 36 LOAD_CONST               3 (('Const',))
-                38 IMPORT_NAME              5 (usefulgram.const)
+                38 IMPORT_NAME              5 (usefulgram.enums)
                 40 IMPORT_FROM              6 (Const)
                 42 STORE_NAME               6 (Const)
                 44 POP_TOP
    
      8          46 LOAD_CONST               0 (0)
                 48 LOAD_CONST               4 (('BaseModel',))
                 50 IMPORT_NAME              7 (pydantic)
@@ -465,20 +465,20 @@
                argcount  : 4
                nlocals   : 8
                stacksize : 5
                flags     : 3
                code
                   0x970069007d047c03720a7c006a0000000000000000007c0464013c0000
                   0064027d057403000000000000000000007c017c02a6020000ab02000000
-                  000000000044005d485c0200007d067d077c0664016b0200000000721402
-                  007c077c006a000000000000000000a6010000ab0100000000000000007c
-                  047c063c0000008c1f7c00a0020000000000000000000000000000000000
-                  0000007c006a0300000000000000007c05190000000000000000007c07a6
-                  020000ab0200000000000000007c047c063c0000007c0564037a0d00007d
-                  058c497c045300
+                  000000000044005d535c0200007d067d077c0664016b0200000000721f7c
+                  00a00200000000000000000000000000000000000000007c006a00000000
+                  00000000007c07a6020000ab0200000000000000007c047c063c0000008c
+                  2a7c00a00200000000000000000000000000000000000000007c006a0300
+                  000000000000007c05190000000000000000007c07a6020000ab02000000
+                  00000000007c047c063c0000007c0564037a0d00007d058c547c045300
                 51           0 RESUME                   0
                
                 56           2 BUILD_MAP                0
                              4 STORE_FAST               4 (return_param)
                
                 58           6 LOAD_FAST                3 (add_prefix)
                              8 POP_JUMP_FORWARD_IF_FALSE    10 (to 30)
@@ -494,72 +494,73 @@
                
                 63          34 LOAD_GLOBAL              3 (NULL + zip)
                             46 LOAD_FAST                1 (keys)
                             48 LOAD_FAST                2 (objects_type)
                             50 PRECALL                  2
                             54 CALL                     2
                             64 GET_ITER
-                       >>   66 FOR_ITER                72 (to 212)
+                       >>   66 FOR_ITER                83 (to 234)
                             68 UNPACK_SEQUENCE          2
                             72 STORE_FAST               6 (key)
                             74 STORE_FAST               7 (obj_type)
                
                 64          76 LOAD_FAST                6 (key)
                             78 LOAD_CONST               1 ('prefix')
                             80 COMPARE_OP               2 (==)
-                            86 POP_JUMP_FORWARD_IF_FALSE    20 (to 128)
+                            86 POP_JUMP_FORWARD_IF_FALSE    31 (to 150)
                
-                65          88 PUSH_NULL
-                            90 LOAD_FAST                7 (obj_type)
-                            92 LOAD_FAST                0 (self)
-                            94 LOAD_ATTR                0 (prefix)
-                           104 PRECALL                  1
-                           108 CALL                     1
-                           118 LOAD_FAST                4 (return_param)
-                           120 LOAD_FAST                6 (key)
-                           122 STORE_SUBSCR
-               
-                67         126 JUMP_BACKWARD           31 (to 66)
-               
-                69     >>  128 LOAD_FAST                0 (self)
-                           130 LOAD_METHOD              2 (_convert_str_to_type)
-               
-                70         152 LOAD_FAST                0 (self)
-                           154 LOAD_ATTR                3 (additional)
-                           164 LOAD_FAST                5 (additional_value)
-                           166 BINARY_SUBSCR
-                           176 LOAD_FAST                7 (obj_type)
-               
-                69         178 PRECALL                  2
-                           182 CALL                     2
-                           192 LOAD_FAST                4 (return_param)
-                           194 LOAD_FAST                6 (key)
-                           196 STORE_SUBSCR
-               
-                73         200 LOAD_FAST                5 (additional_value)
-                           202 LOAD_CONST               3 (1)
-                           204 BINARY_OP               13 (+=)
-                           208 STORE_FAST               5 (additional_value)
-                           210 JUMP_BACKWARD           73 (to 66)
+                65          88 LOAD_FAST                0 (self)
+                            90 LOAD_METHOD              2 (_convert_str_to_type)
+                           112 LOAD_FAST                0 (self)
+                           114 LOAD_ATTR                0 (prefix)
+                           124 LOAD_FAST                7 (obj_type)
+                           126 PRECALL                  2
+                           130 CALL                     2
+                           140 LOAD_FAST                4 (return_param)
+                           142 LOAD_FAST                6 (key)
+                           144 STORE_SUBSCR
+               
+                67         148 JUMP_BACKWARD           42 (to 66)
+               
+                69     >>  150 LOAD_FAST                0 (self)
+                           152 LOAD_METHOD              2 (_convert_str_to_type)
+               
+                70         174 LOAD_FAST                0 (self)
+                           176 LOAD_ATTR                3 (additional)
+                           186 LOAD_FAST                5 (additional_value)
+                           188 BINARY_SUBSCR
+                           198 LOAD_FAST                7 (obj_type)
+               
+                69         200 PRECALL                  2
+                           204 CALL                     2
+                           214 LOAD_FAST                4 (return_param)
+                           216 LOAD_FAST                6 (key)
+                           218 STORE_SUBSCR
+               
+                73         222 LOAD_FAST                5 (additional_value)
+                           224 LOAD_CONST               3 (1)
+                           226 BINARY_OP               13 (+=)
+                           230 STORE_FAST               5 (additional_value)
+                           232 JUMP_BACKWARD           84 (to 66)
                
-                75     >>  212 LOAD_FAST                4 (return_param)
-                           214 RETURN_VALUE
+                75     >>  234 LOAD_FAST                4 (return_param)
+                           236 RETURN_VALUE
                consts
                   None
                   'prefix'
                   0
                   1
                names      ('prefix', 'zip', '_convert_str_to_type', 'additional')
                varnames   ('self', 'keys', 'objects_type', 'add_prefix', 'return_param', 'additional_value', 'key', 'obj_type')
                freevars   ()
                cellvars   ()
                filename   'C:\\work\\usefulgram\\usefulgram\\parsing\\decode.py'
                name       '_iter_key_and_type'
                firstlineno 51
-               lnotab 0x020504020401140204022a010c012602020218011aff16040c02
+               lnotab 0x020504020401140204022a010c013c02020218011aff16040c02
             False
             'format_objects'
             code
                argcount  : 3
                nlocals   : 7
                stacksize : 5
                flags     : 3
@@ -682,15 +683,15 @@
          name       'DecodeCallbackData'
          firstlineno 12
          lnotab
             0x0c010a01160202012eff0e0102071203201802010eff02010eff020202
             fe020312fd081a260a02011aff0e01
       'DecodeCallbackData'
       None
-   names      ('typing', 'Union', 'datetime', 'date', 'time', 'usefulgram.const', 'Const', 'pydantic', 'BaseModel', 'dataclasses', 'dataclass', 'DecodeCallbackData')
+   names      ('typing', 'Union', 'datetime', 'date', 'time', 'usefulgram.enums', 'Const', 'pydantic', 'BaseModel', 'dataclasses', 'dataclass', 'DecodeCallbackData')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\work\\usefulgram\\usefulgram\\parsing\\decode.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02030c0114020c020c010c03
```

### Comparing `usefulgram-0.0.0a2/usefulgram/parsing/__pycache__/encode.cpython-310.pyc` & `usefulgram-0.0.0a3/usefulgram/parsing/__pycache__/encode.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a2/usefulgram/parsing/__pycache__/encode.cpython-311.pyc` & `usefulgram-0.0.0a3/usefulgram/parsing/__pycache__/encode.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x80a29864 (Sun Jun 25 20:24:32 2023 UTC)
+moddate:  0xf51eaf64 (Wed Jul 12 21:45:25 2023 UTC)
 files sz: 2514
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
@@ -45,15 +45,15 @@
                 50 STORE_NAME               7 (TooMoreCharacters)
                 52 IMPORT_FROM              8 (RecursionObjectParse)
                 54 STORE_NAME               8 (RecursionObjectParse)
                 56 POP_TOP
    
     10          58 LOAD_CONST               0 (0)
                 60 LOAD_CONST               5 (('Const',))
-                62 IMPORT_NAME              9 (usefulgram.const)
+                62 IMPORT_NAME              9 (usefulgram.enums)
                 64 IMPORT_FROM             10 (Const)
                 66 STORE_NAME              10 (Const)
                 68 POP_TOP
    
     13          70 PUSH_NULL
                 72 LOAD_BUILD_CLASS
                 74 LOAD_CONST               6 (<code object _Additional, file "C:\work\usefulgram\usefulgram\parsing\encode.py", line 13>)
@@ -663,15 +663,15 @@
          filename   'C:\\work\\usefulgram\\usefulgram\\parsing\\encode.py'
          name       '_CallbackData'
          firstlineno 68
          lnotab
             0x0a010201020102ff020102ff020102ff020202fe06ff0e01020602010e
             ff0e01020d02fd060102ff02021efe020302fd020302fd
       '_CallbackData'
-   names      ('sys', 'typing', 'Union', 'datetime', 'date', 'time', 'usefulgram.exceptions', 'TooMoreCharacters', 'RecursionObjectParse', 'usefulgram.const', 'Const', '_Additional', '_CallbackData', 'AdditionalInstance', 'CallbackData')
+   names      ('sys', 'typing', 'Union', 'datetime', 'date', 'time', 'usefulgram.exceptions', 'TooMoreCharacters', 'RecursionObjectParse', 'usefulgram.enums', 'Const', '_Additional', '_CallbackData', 'AdditionalInstance', 'CallbackData')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\work\\usefulgram\\usefulgram\\parsing\\encode.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020308020c02140210010c031a371a211401
```

### Comparing `usefulgram-0.0.0a2/usefulgram/parsing/decode.py` & `usefulgram-0.0.0a3/usefulgram/parsing/decode.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
 from typing import Union
 from datetime import datetime, date, time
 
-from usefulgram.const import Const
+from usefulgram.enums import Const
 
 from pydantic import BaseModel
 from dataclasses import dataclass
 
 
 class DecodeCallbackData:
     prefix: str
@@ -58,15 +58,15 @@
         if add_prefix:
             return_param["prefix"] = self.prefix
 
         additional_value = 0
 
         for key, obj_type in zip(keys, objects_type):
             if key == "prefix":
-                return_param[key] = obj_type(self.prefix)
+                return_param[key] = self._convert_str_to_type(self.prefix, obj_type)
 
                 continue
 
             return_param[key] = self._convert_str_to_type(
                 self.additional[additional_value], obj_type
             )
```

### Comparing `usefulgram-0.0.0a2/usefulgram/parsing/encode.py` & `usefulgram-0.0.0a3/usefulgram/parsing/encode.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 
 from typing import Union
 
 from datetime import date, time, datetime
 
 from usefulgram.exceptions import TooMoreCharacters, RecursionObjectParse
-from usefulgram.const import Const
+from usefulgram.enums import Const
 
 
 class _Additional:
     def _object_to_str(self, item: object) -> str:
         annotations_keys = list(item.__annotations__.keys())
 
         result = ""
```

### Comparing `usefulgram-0.0.0a2/usefulgram/utils/__pycache__/autorepr.cpython-310.pyc` & `usefulgram-0.0.0a3/usefulgram/utils/__pycache__/autorepr.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a2/usefulgram/utils/__pycache__/autorepr.cpython-311.pyc` & `usefulgram-0.0.0a3/usefulgram/utils/__pycache__/autorepr.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a2/PKG-INFO` & `usefulgram-0.0.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usefulgram
-Version: 0.0.0a2
+Version: 0.0.0a3
 Summary: Like aiogram but more easy
 Home-page: https://github.com/Sethis/usefulgram
 License: MIT
 Author: Alexandr Bortnik
 Author-email: sambonsttt@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

