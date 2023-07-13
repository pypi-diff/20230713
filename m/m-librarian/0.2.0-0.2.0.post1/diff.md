# Comparing `tmp/m_librarian-0.2.0.tar.gz` & `tmp/m_librarian-0.2.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/m_librarian-0.2.0.tar", last modified: Sat Dec 24 11:41:46 2022, max compression
+gzip compressed data, was "dist/m_librarian-0.2.0.post1.tar", last modified: Thu Jul 13 17:35:30 2023, max compression
```

## Comparing `m_librarian-0.2.0.tar` & `m_librarian-0.2.0.post1.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2022-12-24 11:41:46.000000 m_librarian-0.2.0/
--rw-r--r--   0 phd       (1000) phd       (1000)      399 2022-12-24 11:36:46.000000 m_librarian-0.2.0/Makefile
--rwxr-xr-x   0 phd       (1000) phd       (1000)     3161 2022-10-27 16:40:12.000000 m_librarian-0.2.0/setup.py
--rw-r--r--   0 phd       (1000) phd       (1000)     1698 2018-06-11 13:54:59.000000 m_librarian-0.2.0/m_librarian.conf.sample
--rw-r--r--   0 phd       (1000) phd       (1000)      212 2022-12-24 11:41:46.000000 m_librarian-0.2.0/setup.cfg
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2022-12-24 11:41:46.000000 m_librarian-0.2.0/docs-ru/
--rw-r--r--   0 phd       (1000) phd       (1000)     7068 2016-03-31 15:20:09.000000 m_librarian-0.2.0/docs-ru/Makefile
--rw-r--r--   0 phd       (1000) phd       (1000)     1009 2018-04-08 18:02:53.000000 m_librarian-0.2.0/docs-ru/index.rst
--rw-r--r--   0 phd       (1000) phd       (1000)     2901 2022-12-24 11:41:10.000000 m_librarian-0.2.0/docs-ru/news.rst
--rw-r--r--   0 phd       (1000) phd       (1000)     9199 2017-04-26 18:12:07.000000 m_librarian-0.2.0/docs-ru/conf.py
--rw-r--r--   0 phd       (1000) phd       (1000)    14760 2018-06-04 19:28:26.000000 m_librarian-0.2.0/docs-ru/command_line.rst
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2022-12-24 11:41:46.000000 m_librarian-0.2.0/docs-ru/api/
--rw-r--r--   0 phd       (1000) phd       (1000)      153 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs-ru/api/m_librarian.download.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      147 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs-ru/api/m_librarian.config.rst
--rw-r--r--   0 phd       (1000) phd       (1000)       70 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs-ru/api/modules.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      147 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs-ru/api/m_librarian.search.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      150 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs-ru/api/m_librarian.web.app.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      141 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs-ru/api/m_librarian.pbar.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      141 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs-ru/api/m_librarian.glst.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      156 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs-ru/api/m_librarian.web.utils.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      138 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs-ru/api/m_librarian.inp.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      253 2018-04-24 21:42:46.000000 m_librarian-0.2.0/docs-ru/api/m_librarian.web.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      147 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs-ru/api/m_librarian.compat.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      135 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs-ru/api/m_librarian.db.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      422 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs-ru/api/m_librarian.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      165 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs-ru/api/m_librarian.translations.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      159 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs-ru/api/m_librarian.web.server.rst
--rw-r--r--   0 phd       (1000) phd       (1000)     5045 2018-06-11 12:07:21.000000 m_librarian-0.2.0/docs-ru/before_begin.rst
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2022-12-24 11:41:46.000000 m_librarian-0.2.0/scripts/
--rwxr-xr-x   0 phd       (1000) phd       (1000)    15370 2021-02-21 17:36:09.000000 m_librarian-0.2.0/scripts/ml-search.py
--rwxr-xr-x   0 phd       (1000) phd       (1000)      754 2018-05-10 21:51:58.000000 m_librarian-0.2.0/scripts/ml-initdb.py
--rwxr-xr-x   0 phd       (1000) phd       (1000)     1871 2018-05-10 21:51:58.000000 m_librarian-0.2.0/scripts/ml-import.py
--rwxr-xr-x   0 phd       (1000) phd       (1000)     1062 2018-04-08 22:11:23.000000 m_librarian-0.2.0/scripts/ml-web.py
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2022-12-24 11:41:46.000000 m_librarian-0.2.0/tests/
--rw-r--r--   0 phd       (1000) phd       (1000)       40 2016-09-20 20:57:08.000000 m_librarian-0.2.0/tests/Makefile
--rw-r--r--   0 phd       (1000) phd       (1000)       59 2016-09-11 19:15:35.000000 m_librarian-0.2.0/tests/test_config.conf
--rw-r--r--   0 phd       (1000) phd       (1000)      362 2018-05-16 21:30:48.000000 m_librarian-0.2.0/tests/test_inp.py
--rw-r--r--   0 phd       (1000) phd       (1000)      170 2018-04-22 20:43:29.000000 m_librarian-0.2.0/tests/conftest.py
--rw-r--r--   0 phd       (1000) phd       (1000)      271 2018-04-22 20:57:43.000000 m_librarian-0.2.0/tests/test_translations.py
--rw-r--r--   0 phd       (1000) phd       (1000)      437 2018-06-11 13:54:59.000000 m_librarian-0.2.0/tests/test_format.py
--rw-r--r--   0 phd       (1000) phd       (1000)      686 2018-05-16 21:30:48.000000 m_librarian-0.2.0/tests/test.inpx
--rw-r--r--   0 phd       (1000) phd       (1000)      218 2018-05-10 21:51:58.000000 m_librarian-0.2.0/tests/test_glst.py
--rw-r--r--   0 phd       (1000) phd       (1000)      203 2016-04-06 19:50:10.000000 m_librarian-0.2.0/tests/bad.inpx
--rw-r--r--   0 phd       (1000) phd       (1000)      281 2016-09-20 20:57:40.000000 m_librarian-0.2.0/tests/test_config.py
--rw-r--r--   0 phd       (1000) phd       (1000)      938 2016-09-20 20:57:40.000000 m_librarian-0.2.0/tests/test_search.py
--rw-r--r--   0 phd       (1000) phd       (1000)      707 2018-04-22 20:43:29.000000 m_librarian-0.2.0/tests/dbutils.py
--rwxr-xr-x   0 phd       (1000) phd       (1000)      353 2016-05-29 18:33:05.000000 m_librarian-0.2.0/mk-distr
--rw-r--r--   0 phd       (1000) phd       (1000)    17989 2015-12-19 23:23:45.000000 m_librarian-0.2.0/COPYING
--rw-r--r--   0 phd       (1000) phd       (1000)     2722 2022-12-24 11:41:46.000000 m_librarian-0.2.0/PKG-INFO
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2022-12-24 11:41:46.000000 m_librarian-0.2.0/docs/
--rw-r--r--   0 phd       (1000) phd       (1000)     7068 2016-03-31 15:20:09.000000 m_librarian-0.2.0/docs/Makefile
--rw-r--r--   0 phd       (1000) phd       (1000)      809 2018-03-22 19:26:32.000000 m_librarian-0.2.0/docs/index.rst
--rw-r--r--   0 phd       (1000) phd       (1000)     3865 2022-12-24 11:41:10.000000 m_librarian-0.2.0/docs/news.rst
--rw-r--r--   0 phd       (1000) phd       (1000)     1123 2018-04-24 21:31:51.000000 m_librarian-0.2.0/docs/install.rst
--rw-r--r--   0 phd       (1000) phd       (1000)     9199 2017-04-26 18:12:07.000000 m_librarian-0.2.0/docs/conf.py
--rw-r--r--   0 phd       (1000) phd       (1000)     8960 2018-06-04 19:28:26.000000 m_librarian-0.2.0/docs/command_line.rst
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2022-12-24 11:41:46.000000 m_librarian-0.2.0/docs/api/
--rw-r--r--   0 phd       (1000) phd       (1000)      153 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs/api/m_librarian.download.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      147 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs/api/m_librarian.config.rst
--rw-r--r--   0 phd       (1000) phd       (1000)       70 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs/api/modules.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      147 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs/api/m_librarian.search.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      150 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs/api/m_librarian.web.app.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      141 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs/api/m_librarian.pbar.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      141 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs/api/m_librarian.glst.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      156 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs/api/m_librarian.web.utils.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      138 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs/api/m_librarian.inp.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      253 2018-04-24 21:42:46.000000 m_librarian-0.2.0/docs/api/m_librarian.web.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      147 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs/api/m_librarian.compat.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      135 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs/api/m_librarian.db.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      422 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs/api/m_librarian.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      165 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs/api/m_librarian.translations.rst
--rw-r--r--   0 phd       (1000) phd       (1000)      159 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs/api/m_librarian.web.server.rst
--rw-r--r--   0 phd       (1000) phd       (1000)     2000 2018-06-11 12:07:21.000000 m_librarian-0.2.0/docs/before_begin.rst
--rwxr-xr-x   0 phd       (1000) phd       (1000)      216 2018-04-08 19:35:19.000000 m_librarian-0.2.0/docs/genapidocs
--rw-r--r--   0 phd       (1000) phd       (1000)      254 2018-06-11 14:06:04.000000 m_librarian-0.2.0/TODO
--rw-r--r--   0 phd       (1000) phd       (1000)      933 2022-12-17 19:50:43.000000 m_librarian-0.2.0/README.rus.txt
--rw-r--r--   0 phd       (1000) phd       (1000)      958 2022-10-27 16:40:12.000000 m_librarian-0.2.0/tox.ini
--rw-r--r--   0 phd       (1000) phd       (1000)      485 2019-03-27 23:15:10.000000 m_librarian-0.2.0/MANIFEST.in
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2022-12-24 11:41:46.000000 m_librarian-0.2.0/m_librarian.egg-info/
--rw-r--r--   0 phd       (1000) phd       (1000)       12 2022-12-24 11:41:46.000000 m_librarian-0.2.0/m_librarian.egg-info/top_level.txt
--rw-r--r--   0 phd       (1000) phd       (1000)      150 2022-12-24 11:41:46.000000 m_librarian-0.2.0/m_librarian.egg-info/requires.txt
--rw-r--r--   0 phd       (1000) phd       (1000)     3256 2022-12-24 11:41:46.000000 m_librarian-0.2.0/m_librarian.egg-info/SOURCES.txt
--rw-r--r--   0 phd       (1000) phd       (1000)        1 2022-12-24 11:41:46.000000 m_librarian-0.2.0/m_librarian.egg-info/dependency_links.txt
--rw-r--r--   0 phd       (1000) phd       (1000)     2722 2022-12-24 11:41:46.000000 m_librarian-0.2.0/m_librarian.egg-info/PKG-INFO
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2022-12-24 11:41:46.000000 m_librarian-0.2.0/m_librarian/
--rwxr-xr-x   0 phd       (1000) phd       (1000)     2035 2018-05-16 21:16:33.000000 m_librarian-0.2.0/m_librarian/glst.py
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2022-12-24 11:41:46.000000 m_librarian-0.2.0/m_librarian/glst/
--rw-r--r--   0 phd       (1000) phd       (1000)    13685 2018-05-10 21:51:58.000000 m_librarian-0.2.0/m_librarian/glst/genres_fb2_flibusta.glst
--rw-r--r--   0 phd       (1000) phd       (1000)     1278 2015-12-25 19:41:29.000000 m_librarian-0.2.0/m_librarian/glst/License.txt
--rw-r--r--   0 phd       (1000) phd       (1000)     8606 2015-12-25 19:41:29.000000 m_librarian-0.2.0/m_librarian/glst/genres_nonfb2.glst
--rw-r--r--   0 phd       (1000) phd       (1000)    15035 2018-05-10 21:51:58.000000 m_librarian-0.2.0/m_librarian/glst/genres_fb2_librusec.glst
--rw-r--r--   0 phd       (1000) phd       (1000)      930 2018-05-11 23:12:27.000000 m_librarian-0.2.0/m_librarian/glst/README.rus.txt
--rw-r--r--   0 phd       (1000) phd       (1000)      651 2018-03-22 19:26:32.000000 m_librarian-0.2.0/m_librarian/pbar.py
--rw-r--r--   0 phd       (1000) phd       (1000)     4174 2018-06-04 19:28:26.000000 m_librarian-0.2.0/m_librarian/inp.py
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2022-12-24 11:41:46.000000 m_librarian-0.2.0/m_librarian/web/
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2022-12-24 11:41:46.000000 m_librarian-0.2.0/m_librarian/web/static/
--rw-r--r--   0 phd       (1000) phd       (1000)      788 2018-06-11 13:54:59.000000 m_librarian-0.2.0/m_librarian/web/static/style.css
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2022-12-24 11:41:46.000000 m_librarian-0.2.0/m_librarian/web/views/
--rw-r--r--   0 phd       (1000) phd       (1000)      276 2020-12-22 22:54:01.000000 m_librarian-0.2.0/m_librarian/web/views/Makefile
--rw-r--r--   0 phd       (1000) phd       (1000)      124 2018-04-08 00:40:50.000000 m_librarian-0.2.0/m_librarian/web/views/download.tmpl
--rw-r--r--   0 phd       (1000) phd       (1000)     1056 2018-05-26 16:57:44.000000 m_librarian-0.2.0/m_librarian/web/views/search_authors_form.tmpl
--rw-r--r--   0 phd       (1000) phd       (1000)     8412 2018-06-11 12:07:21.000000 m_librarian-0.2.0/m_librarian/web/views/list_authors.py
--rw-r--r--   0 phd       (1000) phd       (1000)     5939 2018-05-26 17:22:49.000000 m_librarian-0.2.0/m_librarian/web/views/index.py
--rw-r--r--   0 phd       (1000) phd       (1000)     9890 2018-06-10 23:31:08.000000 m_librarian-0.2.0/m_librarian/web/views/search_books_form.py
--rw-r--r--   0 phd       (1000) phd       (1000)     2455 2022-12-17 19:33:31.000000 m_librarian-0.2.0/m_librarian/web/views/list_books.tmpl
--rw-r--r--   0 phd       (1000) phd       (1000)    12594 2022-12-17 19:33:31.000000 m_librarian-0.2.0/m_librarian/web/views/list_books.py
--rw-r--r--   0 phd       (1000) phd       (1000)     5672 2018-05-26 17:22:49.000000 m_librarian-0.2.0/m_librarian/web/views/search_books.py
--rw-r--r--   0 phd       (1000) phd       (1000)        2 2018-04-01 19:12:23.000000 m_librarian-0.2.0/m_librarian/web/views/__init__.py
--rw-r--r--   0 phd       (1000) phd       (1000)     1297 2018-06-10 23:31:08.000000 m_librarian-0.2.0/m_librarian/web/views/search_books_form.tmpl
--rw-r--r--   0 phd       (1000) phd       (1000)     5529 2020-12-23 01:33:00.000000 m_librarian-0.2.0/m_librarian/web/views/layout.py
--rw-r--r--   0 phd       (1000) phd       (1000)      209 2018-05-26 17:22:49.000000 m_librarian-0.2.0/m_librarian/web/views/search_books.tmpl
--rw-r--r--   0 phd       (1000) phd       (1000)      221 2018-04-05 21:24:17.000000 m_librarian-0.2.0/m_librarian/web/views/search_authors.tmpl
--rw-r--r--   0 phd       (1000) phd       (1000)      354 2018-05-26 17:22:49.000000 m_librarian-0.2.0/m_librarian/web/views/index.tmpl
--rw-r--r--   0 phd       (1000) phd       (1000)     8462 2018-05-26 16:57:44.000000 m_librarian-0.2.0/m_librarian/web/views/search_authors_form.py
--rw-r--r--   0 phd       (1000) phd       (1000)     5471 2018-04-08 00:40:50.000000 m_librarian-0.2.0/m_librarian/web/views/download.py
--rw-r--r--   0 phd       (1000) phd       (1000)      975 2018-06-11 12:07:21.000000 m_librarian-0.2.0/m_librarian/web/views/list_authors.tmpl
--rw-r--r--   0 phd       (1000) phd       (1000)     5704 2018-04-05 21:24:17.000000 m_librarian-0.2.0/m_librarian/web/views/search_authors.py
--rw-r--r--   0 phd       (1000) phd       (1000)     1037 2020-12-23 01:33:00.000000 m_librarian-0.2.0/m_librarian/web/views/layout.tmpl
--rw-r--r--   0 phd       (1000) phd       (1000)     1395 2019-05-11 16:34:37.000000 m_librarian-0.2.0/m_librarian/web/utils.py
--rw-r--r--   0 phd       (1000) phd       (1000)      799 2018-04-01 19:12:23.000000 m_librarian-0.2.0/m_librarian/web/server.py
--rw-r--r--   0 phd       (1000) phd       (1000)     5103 2022-12-17 17:06:02.000000 m_librarian-0.2.0/m_librarian/web/app.py
--rw-r--r--   0 phd       (1000) phd       (1000)        2 2018-04-01 18:01:27.000000 m_librarian-0.2.0/m_librarian/web/__init__.py
--rwxr-xr-x   0 phd       (1000) phd       (1000)     2719 2018-06-10 23:31:08.000000 m_librarian-0.2.0/m_librarian/config.py
--rw-r--r--   0 phd       (1000) phd       (1000)      647 2020-12-24 22:43:29.000000 m_librarian-0.2.0/m_librarian/translations.py
--rwxr-xr-x   0 phd       (1000) phd       (1000)     8385 2018-06-11 13:54:59.000000 m_librarian-0.2.0/m_librarian/db.py
--rw-r--r--   0 phd       (1000) phd       (1000)       22 2022-12-24 11:41:10.000000 m_librarian-0.2.0/m_librarian/__version__.py
--rw-r--r--   0 phd       (1000) phd       (1000)     4107 2018-06-10 23:31:08.000000 m_librarian-0.2.0/m_librarian/search.py
--rw-r--r--   0 phd       (1000) phd       (1000)      241 2016-07-25 12:50:49.000000 m_librarian-0.2.0/m_librarian/compat.py
--rw-r--r--   0 phd       (1000) phd       (1000)        2 2015-12-15 20:52:19.000000 m_librarian-0.2.0/m_librarian/__init__.py
--rwxr-xr-x   0 phd       (1000) phd       (1000)     3756 2018-06-11 13:54:59.000000 m_librarian-0.2.0/m_librarian/download.py
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2022-12-24 11:41:46.000000 m_librarian-0.2.0/m_librarian/translations_dir/
--rw-r--r--   0 phd       (1000) phd       (1000)      137 2020-12-24 22:43:29.000000 m_librarian-0.2.0/m_librarian/translations_dir/Makefile
--rw-r--r--   0 phd       (1000) phd       (1000)     2017 2020-12-24 22:43:29.000000 m_librarian-0.2.0/m_librarian/translations_dir/ru.mo
--rw-r--r--   0 phd       (1000) phd       (1000)     2007 2020-12-24 22:43:29.000000 m_librarian-0.2.0/m_librarian/translations_dir/ru.po
--rw-r--r--   0 phd       (1000) phd       (1000)      725 2022-10-30 19:02:31.000000 m_librarian-0.2.0/README.rst
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/
+-rw-r--r--   0 phd       (1000) phd       (1000)      399 2022-12-24 11:36:46.000000 m_librarian-0.2.0.post1/Makefile
+-rwxr-xr-x   0 phd       (1000) phd       (1000)     3156 2023-03-01 14:02:37.000000 m_librarian-0.2.0.post1/setup.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     1698 2018-06-11 13:54:59.000000 m_librarian-0.2.0.post1/m_librarian.conf.sample
+-rw-r--r--   0 phd       (1000) phd       (1000)      212 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/setup.cfg
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/docs-ru/
+-rw-r--r--   0 phd       (1000) phd       (1000)     7068 2016-03-31 15:20:09.000000 m_librarian-0.2.0.post1/docs-ru/Makefile
+-rw-r--r--   0 phd       (1000) phd       (1000)     1009 2018-04-08 18:02:53.000000 m_librarian-0.2.0.post1/docs-ru/index.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)     3044 2023-07-13 17:20:24.000000 m_librarian-0.2.0.post1/docs-ru/news.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)     9199 2017-04-26 18:12:07.000000 m_librarian-0.2.0.post1/docs-ru/conf.py
+-rw-r--r--   0 phd       (1000) phd       (1000)    14760 2018-06-04 19:28:26.000000 m_librarian-0.2.0.post1/docs-ru/command_line.rst
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/docs-ru/api/
+-rw-r--r--   0 phd       (1000) phd       (1000)      153 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs-ru/api/m_librarian.download.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      147 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs-ru/api/m_librarian.config.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)       70 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs-ru/api/modules.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      147 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs-ru/api/m_librarian.search.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      150 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs-ru/api/m_librarian.web.app.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      141 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs-ru/api/m_librarian.pbar.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      141 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs-ru/api/m_librarian.glst.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      156 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs-ru/api/m_librarian.web.utils.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      138 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs-ru/api/m_librarian.inp.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      253 2018-04-24 21:42:46.000000 m_librarian-0.2.0.post1/docs-ru/api/m_librarian.web.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      147 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs-ru/api/m_librarian.compat.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      135 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs-ru/api/m_librarian.db.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      422 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs-ru/api/m_librarian.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      165 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs-ru/api/m_librarian.translations.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      159 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs-ru/api/m_librarian.web.server.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)     5045 2018-06-11 12:07:21.000000 m_librarian-0.2.0.post1/docs-ru/before_begin.rst
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/scripts/
+-rwxr-xr-x   0 phd       (1000) phd       (1000)    15370 2021-02-21 17:36:09.000000 m_librarian-0.2.0.post1/scripts/ml-search.py
+-rwxr-xr-x   0 phd       (1000) phd       (1000)      754 2018-05-10 21:51:58.000000 m_librarian-0.2.0.post1/scripts/ml-initdb.py
+-rwxr-xr-x   0 phd       (1000) phd       (1000)     1871 2018-05-10 21:51:58.000000 m_librarian-0.2.0.post1/scripts/ml-import.py
+-rwxr-xr-x   0 phd       (1000) phd       (1000)     1062 2018-04-08 22:11:23.000000 m_librarian-0.2.0.post1/scripts/ml-web.py
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/tests/
+-rw-r--r--   0 phd       (1000) phd       (1000)       40 2016-09-20 20:57:08.000000 m_librarian-0.2.0.post1/tests/Makefile
+-rw-r--r--   0 phd       (1000) phd       (1000)       59 2016-09-11 19:15:35.000000 m_librarian-0.2.0.post1/tests/test_config.conf
+-rw-r--r--   0 phd       (1000) phd       (1000)      362 2018-05-16 21:30:48.000000 m_librarian-0.2.0.post1/tests/test_inp.py
+-rw-r--r--   0 phd       (1000) phd       (1000)      170 2018-04-22 20:43:29.000000 m_librarian-0.2.0.post1/tests/conftest.py
+-rw-r--r--   0 phd       (1000) phd       (1000)      271 2018-04-22 20:57:43.000000 m_librarian-0.2.0.post1/tests/test_translations.py
+-rw-r--r--   0 phd       (1000) phd       (1000)      437 2018-06-11 13:54:59.000000 m_librarian-0.2.0.post1/tests/test_format.py
+-rw-r--r--   0 phd       (1000) phd       (1000)      686 2018-05-16 21:30:48.000000 m_librarian-0.2.0.post1/tests/test.inpx
+-rw-r--r--   0 phd       (1000) phd       (1000)      218 2018-05-10 21:51:58.000000 m_librarian-0.2.0.post1/tests/test_glst.py
+-rw-r--r--   0 phd       (1000) phd       (1000)      203 2016-04-06 19:50:10.000000 m_librarian-0.2.0.post1/tests/bad.inpx
+-rw-r--r--   0 phd       (1000) phd       (1000)      281 2016-09-20 20:57:40.000000 m_librarian-0.2.0.post1/tests/test_config.py
+-rw-r--r--   0 phd       (1000) phd       (1000)      938 2016-09-20 20:57:40.000000 m_librarian-0.2.0.post1/tests/test_search.py
+-rw-r--r--   0 phd       (1000) phd       (1000)      707 2018-04-22 20:43:29.000000 m_librarian-0.2.0.post1/tests/dbutils.py
+-rwxr-xr-x   0 phd       (1000) phd       (1000)      353 2016-05-29 18:33:05.000000 m_librarian-0.2.0.post1/mk-distr
+-rw-r--r--   0 phd       (1000) phd       (1000)    17989 2015-12-19 23:23:45.000000 m_librarian-0.2.0.post1/COPYING
+-rw-r--r--   0 phd       (1000) phd       (1000)     2734 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/PKG-INFO
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/docs/
+-rw-r--r--   0 phd       (1000) phd       (1000)     7068 2016-03-31 15:20:09.000000 m_librarian-0.2.0.post1/docs/Makefile
+-rw-r--r--   0 phd       (1000) phd       (1000)      809 2018-03-22 19:26:32.000000 m_librarian-0.2.0.post1/docs/index.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)     4035 2023-07-13 17:20:24.000000 m_librarian-0.2.0.post1/docs/news.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)     1123 2018-04-24 21:31:51.000000 m_librarian-0.2.0.post1/docs/install.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)     9199 2017-04-26 18:12:07.000000 m_librarian-0.2.0.post1/docs/conf.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     8960 2018-06-04 19:28:26.000000 m_librarian-0.2.0.post1/docs/command_line.rst
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/docs/api/
+-rw-r--r--   0 phd       (1000) phd       (1000)      153 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs/api/m_librarian.download.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      147 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs/api/m_librarian.config.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)       70 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs/api/modules.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      147 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs/api/m_librarian.search.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      150 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs/api/m_librarian.web.app.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      141 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs/api/m_librarian.pbar.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      141 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs/api/m_librarian.glst.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      156 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs/api/m_librarian.web.utils.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      138 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs/api/m_librarian.inp.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      253 2018-04-24 21:42:46.000000 m_librarian-0.2.0.post1/docs/api/m_librarian.web.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      147 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs/api/m_librarian.compat.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      135 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs/api/m_librarian.db.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      422 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs/api/m_librarian.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      165 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs/api/m_librarian.translations.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)      159 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs/api/m_librarian.web.server.rst
+-rw-r--r--   0 phd       (1000) phd       (1000)     2000 2018-06-11 12:07:21.000000 m_librarian-0.2.0.post1/docs/before_begin.rst
+-rwxr-xr-x   0 phd       (1000) phd       (1000)      216 2018-04-08 19:35:19.000000 m_librarian-0.2.0.post1/docs/genapidocs
+-rw-r--r--   0 phd       (1000) phd       (1000)      254 2018-06-11 14:06:04.000000 m_librarian-0.2.0.post1/TODO
+-rw-r--r--   0 phd       (1000) phd       (1000)      933 2022-12-17 19:50:43.000000 m_librarian-0.2.0.post1/README.rus.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)      958 2022-10-27 16:40:12.000000 m_librarian-0.2.0.post1/tox.ini
+-rw-r--r--   0 phd       (1000) phd       (1000)      485 2019-03-27 23:15:10.000000 m_librarian-0.2.0.post1/MANIFEST.in
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/m_librarian.egg-info/
+-rw-r--r--   0 phd       (1000) phd       (1000)       12 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/m_librarian.egg-info/top_level.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)      145 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/m_librarian.egg-info/requires.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)     3256 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/m_librarian.egg-info/SOURCES.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)        1 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/m_librarian.egg-info/dependency_links.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)     2734 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/m_librarian.egg-info/PKG-INFO
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/m_librarian/
+-rwxr-xr-x   0 phd       (1000) phd       (1000)     2035 2018-05-16 21:16:33.000000 m_librarian-0.2.0.post1/m_librarian/glst.py
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/m_librarian/glst/
+-rw-r--r--   0 phd       (1000) phd       (1000)    13685 2018-05-10 21:51:58.000000 m_librarian-0.2.0.post1/m_librarian/glst/genres_fb2_flibusta.glst
+-rw-r--r--   0 phd       (1000) phd       (1000)     1278 2015-12-25 19:41:29.000000 m_librarian-0.2.0.post1/m_librarian/glst/License.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)     8606 2015-12-25 19:41:29.000000 m_librarian-0.2.0.post1/m_librarian/glst/genres_nonfb2.glst
+-rw-r--r--   0 phd       (1000) phd       (1000)    15035 2018-05-10 21:51:58.000000 m_librarian-0.2.0.post1/m_librarian/glst/genres_fb2_librusec.glst
+-rw-r--r--   0 phd       (1000) phd       (1000)      930 2018-05-11 23:12:27.000000 m_librarian-0.2.0.post1/m_librarian/glst/README.rus.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)      651 2018-03-22 19:26:32.000000 m_librarian-0.2.0.post1/m_librarian/pbar.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     4174 2018-06-04 19:28:26.000000 m_librarian-0.2.0.post1/m_librarian/inp.py
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/m_librarian/web/
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/m_librarian/web/static/
+-rw-r--r--   0 phd       (1000) phd       (1000)      788 2018-06-11 13:54:59.000000 m_librarian-0.2.0.post1/m_librarian/web/static/style.css
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/m_librarian/web/views/
+-rw-r--r--   0 phd       (1000) phd       (1000)      276 2020-12-22 22:54:01.000000 m_librarian-0.2.0.post1/m_librarian/web/views/Makefile
+-rw-r--r--   0 phd       (1000) phd       (1000)      124 2018-04-08 00:40:50.000000 m_librarian-0.2.0.post1/m_librarian/web/views/download.tmpl
+-rw-r--r--   0 phd       (1000) phd       (1000)     1056 2018-05-26 16:57:44.000000 m_librarian-0.2.0.post1/m_librarian/web/views/search_authors_form.tmpl
+-rw-r--r--   0 phd       (1000) phd       (1000)     8412 2018-06-11 12:07:21.000000 m_librarian-0.2.0.post1/m_librarian/web/views/list_authors.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     5939 2018-05-26 17:22:49.000000 m_librarian-0.2.0.post1/m_librarian/web/views/index.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     9890 2018-06-10 23:31:08.000000 m_librarian-0.2.0.post1/m_librarian/web/views/search_books_form.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     2455 2022-12-17 19:33:31.000000 m_librarian-0.2.0.post1/m_librarian/web/views/list_books.tmpl
+-rw-r--r--   0 phd       (1000) phd       (1000)    12594 2022-12-17 19:33:31.000000 m_librarian-0.2.0.post1/m_librarian/web/views/list_books.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     5672 2018-05-26 17:22:49.000000 m_librarian-0.2.0.post1/m_librarian/web/views/search_books.py
+-rw-r--r--   0 phd       (1000) phd       (1000)        2 2018-04-01 19:12:23.000000 m_librarian-0.2.0.post1/m_librarian/web/views/__init__.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     1297 2018-06-10 23:31:08.000000 m_librarian-0.2.0.post1/m_librarian/web/views/search_books_form.tmpl
+-rw-r--r--   0 phd       (1000) phd       (1000)     5529 2020-12-23 01:33:00.000000 m_librarian-0.2.0.post1/m_librarian/web/views/layout.py
+-rw-r--r--   0 phd       (1000) phd       (1000)      209 2018-05-26 17:22:49.000000 m_librarian-0.2.0.post1/m_librarian/web/views/search_books.tmpl
+-rw-r--r--   0 phd       (1000) phd       (1000)      221 2018-04-05 21:24:17.000000 m_librarian-0.2.0.post1/m_librarian/web/views/search_authors.tmpl
+-rw-r--r--   0 phd       (1000) phd       (1000)      354 2018-05-26 17:22:49.000000 m_librarian-0.2.0.post1/m_librarian/web/views/index.tmpl
+-rw-r--r--   0 phd       (1000) phd       (1000)     8462 2018-05-26 16:57:44.000000 m_librarian-0.2.0.post1/m_librarian/web/views/search_authors_form.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     5471 2018-04-08 00:40:50.000000 m_librarian-0.2.0.post1/m_librarian/web/views/download.py
+-rw-r--r--   0 phd       (1000) phd       (1000)      975 2018-06-11 12:07:21.000000 m_librarian-0.2.0.post1/m_librarian/web/views/list_authors.tmpl
+-rw-r--r--   0 phd       (1000) phd       (1000)     5704 2018-04-05 21:24:17.000000 m_librarian-0.2.0.post1/m_librarian/web/views/search_authors.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     1037 2020-12-23 01:33:00.000000 m_librarian-0.2.0.post1/m_librarian/web/views/layout.tmpl
+-rw-r--r--   0 phd       (1000) phd       (1000)     1395 2019-05-11 16:34:37.000000 m_librarian-0.2.0.post1/m_librarian/web/utils.py
+-rw-r--r--   0 phd       (1000) phd       (1000)      799 2018-04-01 19:12:23.000000 m_librarian-0.2.0.post1/m_librarian/web/server.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     5103 2022-12-17 17:06:02.000000 m_librarian-0.2.0.post1/m_librarian/web/app.py
+-rw-r--r--   0 phd       (1000) phd       (1000)        2 2018-04-01 18:01:27.000000 m_librarian-0.2.0.post1/m_librarian/web/__init__.py
+-rwxr-xr-x   0 phd       (1000) phd       (1000)     2719 2018-06-10 23:31:08.000000 m_librarian-0.2.0.post1/m_librarian/config.py
+-rw-r--r--   0 phd       (1000) phd       (1000)      647 2020-12-24 22:43:29.000000 m_librarian-0.2.0.post1/m_librarian/translations.py
+-rwxr-xr-x   0 phd       (1000) phd       (1000)     8385 2018-06-11 13:54:59.000000 m_librarian-0.2.0.post1/m_librarian/db.py
+-rw-r--r--   0 phd       (1000) phd       (1000)       28 2023-07-13 17:32:16.000000 m_librarian-0.2.0.post1/m_librarian/__version__.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     4107 2018-06-10 23:31:08.000000 m_librarian-0.2.0.post1/m_librarian/search.py
+-rw-r--r--   0 phd       (1000) phd       (1000)      241 2016-07-25 12:50:49.000000 m_librarian-0.2.0.post1/m_librarian/compat.py
+-rw-r--r--   0 phd       (1000) phd       (1000)        2 2015-12-15 20:52:19.000000 m_librarian-0.2.0.post1/m_librarian/__init__.py
+-rwxr-xr-x   0 phd       (1000) phd       (1000)     3756 2018-06-11 13:54:59.000000 m_librarian-0.2.0.post1/m_librarian/download.py
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-07-13 17:35:30.000000 m_librarian-0.2.0.post1/m_librarian/translations_dir/
+-rw-r--r--   0 phd       (1000) phd       (1000)      137 2020-12-24 22:43:29.000000 m_librarian-0.2.0.post1/m_librarian/translations_dir/Makefile
+-rw-r--r--   0 phd       (1000) phd       (1000)     2017 2020-12-24 22:43:29.000000 m_librarian-0.2.0.post1/m_librarian/translations_dir/ru.mo
+-rw-r--r--   0 phd       (1000) phd       (1000)     2007 2020-12-24 22:43:29.000000 m_librarian-0.2.0.post1/m_librarian/translations_dir/ru.po
+-rw-r--r--   0 phd       (1000) phd       (1000)      725 2022-10-30 19:02:31.000000 m_librarian-0.2.0.post1/README.rst
```

### Comparing `m_librarian-0.2.0/setup.py` & `m_librarian-0.2.0.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,10 +73,10 @@
     install_requires=[
         'SQLObject>=2.2.1; python_version=="2.7"',
         'SQLObject>=3.0.0; python_version>="3.4"',
         'm_lib.defenc>=1.0',
     ],
     extras_require={
         'pbar': ['m_lib>=3.1'],
-        'web': ['bottle', 'Cheetah3'],
+        'web': ['bottle', 'CT3'],
     },
 )
```

### Comparing `m_librarian-0.2.0/m_librarian.conf.sample` & `m_librarian-0.2.0.post1/m_librarian.conf.sample`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/docs-ru/Makefile` & `m_librarian-0.2.0.post1/docs-ru/Makefile`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/docs-ru/index.rst` & `m_librarian-0.2.0.post1/docs-ru/index.rst`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/docs-ru/news.rst` & `m_librarian-0.2.0.post1/docs-ru/news.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Новости
 =======
 
+Версия 0.2.0.post1
+------------------
+
+* GHActions: Устанавливать все версии Python и PyPy из ``conda-forge``.
+
 Версия 0.2.0 (2022-12-24)
 -------------------------
 
 * Переключать чекбоксы для книг по сериям, для всех книг автора или все.
 
 * Python 3.11.
```

### Comparing `m_librarian-0.2.0/docs-ru/conf.py` & `m_librarian-0.2.0.post1/docs-ru/conf.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/docs-ru/command_line.rst` & `m_librarian-0.2.0.post1/docs-ru/command_line.rst`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/docs-ru/before_begin.rst` & `m_librarian-0.2.0.post1/docs-ru/before_begin.rst`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/scripts/ml-search.py` & `m_librarian-0.2.0.post1/scripts/ml-search.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/scripts/ml-initdb.py` & `m_librarian-0.2.0.post1/scripts/ml-initdb.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/scripts/ml-import.py` & `m_librarian-0.2.0.post1/scripts/ml-import.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/scripts/ml-web.py` & `m_librarian-0.2.0.post1/scripts/ml-web.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/tests/test.inpx` & `m_librarian-0.2.0.post1/tests/test.inpx`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/tests/test_search.py` & `m_librarian-0.2.0.post1/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/tests/dbutils.py` & `m_librarian-0.2.0.post1/tests/dbutils.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/COPYING` & `m_librarian-0.2.0.post1/COPYING`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/PKG-INFO` & `m_librarian-0.2.0.post1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: m_librarian
-Version: 0.2.0
+Version: 0.2.0.post1
 Summary: m_Librarian for LibRusEc/Flibusta libraries
 Home-page: https://phdru.name/Software/Python/m_librarian/
 Author: Oleg Broytman
 Author-email: phd@phdru.name
 License: GPL
 Project-URL: Issue tracker, https://github.com/phdru/m_librarian/issues
 Project-URL: Homepage, https://phdru.name/Software/Python/m_librarian/
 Project-URL: Documentation, https://phdru.name/Software/Python/m_librarian/docs/
 Project-URL: Github repo, https://github.com/phdru/m_librarian
 Project-URL: Git repo, https://git.phdru.name/m_librarian.git/
-Project-URL: Download, https://pypi.org/project/m_librarian/0.2.0/
+Project-URL: Download, https://pypi.org/project/m_librarian/0.2.0.post1/
 Project-URL: Russian docs, https://phdru.name/Software/Python/m_librarian/docs/ru/
 Description: m_Librarian.
         
         Author: Oleg Broytman <phd@phdru.name>.
         
         Copyright (C) 2015-2022 PhiloSoft Design.
```

### Comparing `m_librarian-0.2.0/docs/Makefile` & `m_librarian-0.2.0.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/docs/index.rst` & `m_librarian-0.2.0.post1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/docs/news.rst` & `m_librarian-0.2.0.post1/docs/news.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 News
 ====
 
+Version 0.2.0.post1
+-------------------
+
+* GHActions: Install everything from ``conda``.
+  All required Python and PyPy versions are now available from ``conda-forge``.
+
 Version 0.2.0 (2022-12-24)
 --------------------------
 
 * Toggle checkboxes for books in series, for an author or all.
 
 * Python 3.11.
```

### Comparing `m_librarian-0.2.0/docs/install.rst` & `m_librarian-0.2.0.post1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/docs/conf.py` & `m_librarian-0.2.0.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/docs/command_line.rst` & `m_librarian-0.2.0.post1/docs/command_line.rst`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/docs/before_begin.rst` & `m_librarian-0.2.0.post1/docs/before_begin.rst`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/README.rus.txt` & `m_librarian-0.2.0.post1/README.rus.txt`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/tox.ini` & `m_librarian-0.2.0.post1/tox.ini`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian.egg-info/SOURCES.txt` & `m_librarian-0.2.0.post1/m_librarian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian.egg-info/PKG-INFO` & `m_librarian-0.2.0.post1/m_librarian.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: m-librarian
-Version: 0.2.0
+Version: 0.2.0.post1
 Summary: m_Librarian for LibRusEc/Flibusta libraries
 Home-page: https://phdru.name/Software/Python/m_librarian/
 Author: Oleg Broytman
 Author-email: phd@phdru.name
 License: GPL
 Project-URL: Issue tracker, https://github.com/phdru/m_librarian/issues
 Project-URL: Homepage, https://phdru.name/Software/Python/m_librarian/
 Project-URL: Documentation, https://phdru.name/Software/Python/m_librarian/docs/
 Project-URL: Github repo, https://github.com/phdru/m_librarian
 Project-URL: Git repo, https://git.phdru.name/m_librarian.git/
-Project-URL: Download, https://pypi.org/project/m_librarian/0.2.0/
+Project-URL: Download, https://pypi.org/project/m_librarian/0.2.0.post1/
 Project-URL: Russian docs, https://phdru.name/Software/Python/m_librarian/docs/ru/
 Description: m_Librarian.
         
         Author: Oleg Broytman <phd@phdru.name>.
         
         Copyright (C) 2015-2022 PhiloSoft Design.
```

### Comparing `m_librarian-0.2.0/m_librarian/glst.py` & `m_librarian-0.2.0.post1/m_librarian/glst.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/glst/genres_fb2_flibusta.glst` & `m_librarian-0.2.0.post1/m_librarian/glst/genres_fb2_flibusta.glst`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/glst/License.txt` & `m_librarian-0.2.0.post1/m_librarian/glst/License.txt`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/glst/genres_nonfb2.glst` & `m_librarian-0.2.0.post1/m_librarian/glst/genres_nonfb2.glst`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/glst/genres_fb2_librusec.glst` & `m_librarian-0.2.0.post1/m_librarian/glst/genres_fb2_librusec.glst`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/glst/README.rus.txt` & `m_librarian-0.2.0.post1/m_librarian/glst/README.rus.txt`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/pbar.py` & `m_librarian-0.2.0.post1/m_librarian/pbar.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/inp.py` & `m_librarian-0.2.0.post1/m_librarian/inp.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/web/static/style.css` & `m_librarian-0.2.0.post1/m_librarian/web/static/style.css`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/web/views/search_authors_form.tmpl` & `m_librarian-0.2.0.post1/m_librarian/web/views/search_authors_form.tmpl`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/web/views/list_authors.py` & `m_librarian-0.2.0.post1/m_librarian/web/views/list_authors.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/web/views/index.py` & `m_librarian-0.2.0.post1/m_librarian/web/views/index.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/web/views/search_books_form.py` & `m_librarian-0.2.0.post1/m_librarian/web/views/search_books_form.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/web/views/list_books.tmpl` & `m_librarian-0.2.0.post1/m_librarian/web/views/list_books.tmpl`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/web/views/list_books.py` & `m_librarian-0.2.0.post1/m_librarian/web/views/list_books.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/web/views/search_books.py` & `m_librarian-0.2.0.post1/m_librarian/web/views/search_books.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/web/views/search_books_form.tmpl` & `m_librarian-0.2.0.post1/m_librarian/web/views/search_books_form.tmpl`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/web/views/layout.py` & `m_librarian-0.2.0.post1/m_librarian/web/views/layout.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/web/views/search_authors_form.py` & `m_librarian-0.2.0.post1/m_librarian/web/views/search_authors_form.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/web/views/download.py` & `m_librarian-0.2.0.post1/m_librarian/web/views/download.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/web/views/list_authors.tmpl` & `m_librarian-0.2.0.post1/m_librarian/web/views/list_authors.tmpl`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/web/views/search_authors.py` & `m_librarian-0.2.0.post1/m_librarian/web/views/search_authors.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/web/views/layout.tmpl` & `m_librarian-0.2.0.post1/m_librarian/web/views/layout.tmpl`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/web/utils.py` & `m_librarian-0.2.0.post1/m_librarian/web/utils.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/web/server.py` & `m_librarian-0.2.0.post1/m_librarian/web/server.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/web/app.py` & `m_librarian-0.2.0.post1/m_librarian/web/app.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/config.py` & `m_librarian-0.2.0.post1/m_librarian/config.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/translations.py` & `m_librarian-0.2.0.post1/m_librarian/translations.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/db.py` & `m_librarian-0.2.0.post1/m_librarian/db.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/search.py` & `m_librarian-0.2.0.post1/m_librarian/search.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/download.py` & `m_librarian-0.2.0.post1/m_librarian/download.py`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/translations_dir/ru.mo` & `m_librarian-0.2.0.post1/m_librarian/translations_dir/ru.mo`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/m_librarian/translations_dir/ru.po` & `m_librarian-0.2.0.post1/m_librarian/translations_dir/ru.po`

 * *Files identical despite different names*

### Comparing `m_librarian-0.2.0/README.rst` & `m_librarian-0.2.0.post1/README.rst`

 * *Files identical despite different names*

