# Comparing `tmp/ultima_scraper_collection-1.1.3.tar.gz` & `tmp/ultima_scraper_collection-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_collection-1.1.3.tar", max compression
+gzip compressed data, was "ultima_scraper_collection-2.0.0.tar", max compression
```

## Comparing `ultima_scraper_collection-1.1.3.tar` & `ultima_scraper_collection-2.0.0.tar`

### file list

```diff
@@ -1,72 +1,75 @@
--rw-r--r--   0        0        0      809 2023-06-15 09:42:46.743215 ultima_scraper_collection-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      293 2023-02-26 12:00:14.727199 ultima_scraper_collection-1.1.3/ultima_scraper_collection/__init__.py
--rw-r--r--   0        0        0     3098 2023-06-15 09:44:14.174056 ultima_scraper_collection-1.1.3/ultima_scraper_collection/config.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:41.007744 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:54.441267 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/__init__.py
--rw-r--r--   0        0        0        0 2023-03-06 01:27:30.462039 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/__init__.py
--rw-r--r--   0        0        0        0 2023-03-04 04:03:12.661102 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:54.461267 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/__init__.py
--rw-r--r--   0        0        0       38 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/README
--rw-r--r--   0        0        0     2150 2023-03-05 04:16:43.534861 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/script.py.mako
--rw-r--r--   0        0        0      662 2023-03-05 04:20:42.303797 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py
--rw-r--r--   0        0        0      941 2023-03-05 04:20:47.520466 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py
--rw-r--r--   0        0        0      861 2022-04-25 23:29:43.807242 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py
--rw-r--r--   0        0        0     3182 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py
--rw-r--r--   0        0        0     1651 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py
--rw-r--r--   0        0        0     1415 2023-03-05 04:20:57.727140 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py
--rw-r--r--   0        0        0     2201 2023-03-03 17:13:51.407142 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini
--rw-r--r--   0        0        0    77824 2023-02-14 03:46:10.695467 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db
--rw-r--r--   0        0        0        0 2023-03-10 12:28:15.033139 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 12:28:22.753355 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 12:27:11.408006 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/__init__.py
--rw-r--r--   0        0        0     2296 2023-03-10 12:28:05.882882 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/script.py.mako
--rw-r--r--   0        0        0     1769 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py
--rw-r--r--   0        0        0     1649 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini
--rw-r--r--   0        0        0      493 2023-03-10 12:30:45.700616 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/messages.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db
--rw-r--r--   0        0        0     2288 2023-03-10 12:32:59.654189 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/script.py.mako
--rw-r--r--   0        0        0     1762 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py
--rw-r--r--   0        0        0     1643 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini
--rw-r--r--   0        0        0      488 2023-03-10 12:32:58.467491 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/posts.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db
--rw-r--r--   0        0        0     2294 2023-03-10 12:32:46.997189 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/script.py.mako
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py
--rw-r--r--   0        0        0     1647 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py
--rw-r--r--   0        0        0     1766 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini
--rw-r--r--   0        0        0      490 2023-03-10 12:32:57.520800 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/stories.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db
--rw-r--r--   0        0        0        0 2022-12-05 14:27:20.696663 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/__init__.py
--rw-r--r--   0        0        0     1611 2023-06-03 17:34:00.273754 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py
--rw-r--r--   0        0        0     2764 2023-05-08 21:50:28.707049 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py
--rw-r--r--   0        0        0     2073 2023-04-20 22:22:10.068827 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py
--rw-r--r--   0        0        0     9956 2023-06-15 07:56:54.052868 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py
--rw-r--r--   0        0        0      442 2023-03-12 15:01:42.766490 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/database_manager.py
--rw-r--r--   0        0        0        0 2023-02-26 16:06:18.482305 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/datascraper_manager/__init__.py
--rw-r--r--   0        0        0     1576 2023-05-22 07:47:32.668760 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py
--rw-r--r--   0        0        0        0 2023-02-26 16:04:46.426896 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/datascraper_manager/datascrapers/__init__.py
--rw-r--r--   0        0        0     5344 2023-06-15 07:48:16.103922 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py
--rw-r--r--   0        0        0     5608 2023-06-15 07:49:47.587365 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py
--rw-r--r--   0        0        0    10668 2023-06-15 09:26:42.852114 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/download_manager.py
--rw-r--r--   0        0        0    13669 2023-05-14 19:55:15.091076 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/filesystem_manager.py
--rw-r--r--   0        0        0        0 2023-01-26 08:21:03.864558 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/metadata_manager/__init__.py
--rw-r--r--   0        0        0    29119 2023-06-10 18:24:38.563431 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py
--rw-r--r--   0        0        0     7134 2023-06-01 21:57:38.888076 ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/option_manager.py
--rw-r--r--   0        0        0        0 2023-03-14 06:55:35.872202 ultima_scraper_collection-1.1.3/ultima_scraper_collection/modules/__init__.py
--rw-r--r--   0        0        0    18351 2023-06-15 09:30:35.138093 ultima_scraper_collection-1.1.3/ultima_scraper_collection/modules/module_streamliner.py
--rw-r--r--   0        0        0        0 2023-02-26 16:07:35.717380 ultima_scraper_collection-1.1.3/ultima_scraper_collection/py.typed
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 ultima_scraper_collection-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      881 2023-07-12 18:52:02.405662 ultima_scraper_collection-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      293 2023-02-26 12:00:14.727199 ultima_scraper_collection-2.0.0/ultima_scraper_collection/__init__.py
+-rw-r--r--   0        0        0     3547 2023-07-13 05:55:18.678148 ultima_scraper_collection-2.0.0/ultima_scraper_collection/config.py
+-rw-r--r--   0        0        0        0 2023-07-12 11:29:22.237223 ultima_scraper_collection-2.0.0/ultima_scraper_collection/helpers/__init__.py
+-rw-r--r--   0        0        0     1216 2023-07-12 09:07:53.912599 ultima_scraper_collection-2.0.0/ultima_scraper_collection/helpers/main_helper.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:41.007744 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:54.441267 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-06 01:27:30.462039 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-04 04:03:12.661102 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:54.461267 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/__init__.py
+-rw-r--r--   0        0        0       38 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/README
+-rw-r--r--   0        0        0     2150 2023-03-05 04:16:43.534861 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0      662 2023-03-05 04:20:42.303797 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py
+-rw-r--r--   0        0        0      941 2023-03-05 04:20:47.520466 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py
+-rw-r--r--   0        0        0      861 2022-04-25 23:29:43.807242 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py
+-rw-r--r--   0        0        0     3182 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py
+-rw-r--r--   0        0        0     1651 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py
+-rw-r--r--   0        0        0     1415 2023-03-05 04:20:57.727140 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py
+-rw-r--r--   0        0        0     2201 2023-03-03 17:13:51.407142 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini
+-rw-r--r--   0        0        0    77824 2023-02-14 03:46:10.695467 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db
+-rw-r--r--   0        0        0        0 2023-03-10 12:28:15.033139 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-10 12:28:22.753355 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-10 12:27:11.408006 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/__init__.py
+-rw-r--r--   0        0        0     2296 2023-03-10 12:28:05.882882 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0     1769 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py
+-rw-r--r--   0        0        0     1649 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini
+-rw-r--r--   0        0        0      493 2023-03-10 12:30:45.700616 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/messages.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db
+-rw-r--r--   0        0        0     2288 2023-03-10 12:32:59.654189 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0     1762 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py
+-rw-r--r--   0        0        0     1643 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini
+-rw-r--r--   0        0        0      488 2023-03-10 12:32:58.467491 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/posts.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db
+-rw-r--r--   0        0        0     2294 2023-03-10 12:32:46.997189 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py
+-rw-r--r--   0        0        0     1647 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py
+-rw-r--r--   0        0        0     1766 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini
+-rw-r--r--   0        0        0      490 2023-03-10 12:32:57.520800 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/stories.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db
+-rw-r--r--   0        0        0        0 2022-12-05 14:27:20.696663 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/__init__.py
+-rw-r--r--   0        0        0     1611 2023-06-03 17:34:00.273754 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py
+-rw-r--r--   0        0        0     2764 2023-05-08 21:50:28.707049 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py
+-rw-r--r--   0        0        0     2073 2023-04-20 22:22:10.068827 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py
+-rw-r--r--   0        0        0     9956 2023-06-15 07:56:54.052868 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py
+-rw-r--r--   0        0        0      442 2023-03-12 15:01:42.766490 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/database_manager.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:06:18.482305 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/datascraper_manager/__init__.py
+-rw-r--r--   0        0        0     2293 2023-07-12 11:08:07.047292 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:04:46.426896 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/__init__.py
+-rw-r--r--   0        0        0     5349 2023-07-13 02:40:41.499162 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py
+-rw-r--r--   0        0        0     5637 2023-07-13 02:40:59.485296 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py
+-rw-r--r--   0        0        0    11385 2023-07-12 12:04:54.350746 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/download_manager.py
+-rw-r--r--   0        0        0    17461 2023-07-13 06:10:56.309738 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/filesystem_manager.py
+-rw-r--r--   0        0        0        0 2023-01-26 08:21:03.864558 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/metadata_manager/__init__.py
+-rw-r--r--   0        0        0    29639 2023-07-13 06:00:04.516010 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py
+-rw-r--r--   0        0        0     7127 2023-07-13 05:58:14.304809 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/option_manager.py
+-rw-r--r--   0        0        0     5769 2023-07-13 05:58:45.954199 ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/server_manager.py
+-rw-r--r--   0        0        0        0 2023-03-14 06:55:35.872202 ultima_scraper_collection-2.0.0/ultima_scraper_collection/modules/__init__.py
+-rw-r--r--   0        0        0    16177 2023-07-13 05:54:18.325942 ultima_scraper_collection-2.0.0/ultima_scraper_collection/modules/module_streamliner.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:07:35.717380 ultima_scraper_collection-2.0.0/ultima_scraper_collection/py.typed
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 ultima_scraper_collection-2.0.0/PKG-INFO
```

### Comparing `ultima_scraper_collection-1.1.3/pyproject.toml` & `ultima_scraper_collection-2.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 [tool.poetry]
 name = "ultima-scraper-collection"
-version = "1.1.3"
+version = "2.0.0"
 description = ""
 authors = [
     "DIGITALCRIMINALS <89371864+digitalcriminals@users.noreply.github.com>",
 ]
 packages = [{include = "ultima_scraper_collection"}]
 include = ["ultima_scraper_collection/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 
 sqlalchemy = "^2.0.1"
 psycopg2 = "^2.9.5"
 alembic = "^1.9.2"
 tqdm = "^4.65.0"
-ultima-scraper-api = "^1.1.1"
+ultima-scraper-api = "^2.0.0"
 ultima-scraper-renamer = "^1.1.0"
+ultima-scraper-db = "^0.1.0"
 ffmpeg-python = "^0.2.0"
 pydantic = "^1.10.9"
+netifaces = "^0.11.0"
+sshtunnel = "^0.4.0"
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.2"
 black = {version = "^23.3.0", allow-prereleases = true}
 
 [tool.semantic_release]
 version_toml = "pyproject.toml:tool.poetry.version"
```

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/config.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
-from pydantic import BaseModel
+from pydantic import BaseModel, StrictBool, StrictInt, StrictStr
 from ultima_scraper_api.config import (
-    FanslyAPI,
+    FanslyAPIConfig,
     GlobalAPI,
-    OnlyFansAPI,
+    OnlyFansAPIConfig,
     Settings,
     Sites,
     UltimaScraperAPIConfig,
 )
 
 
 class Jobs(BaseModel):
@@ -29,20 +29,20 @@
     path: Path | None = None
     minimum_space: int = -1
     store: bool = True
     overflow: bool = True
 
 
 class GlobalXPathSetup(BaseModel):
-    directories: list[Directory] = [Directory(path=Path().absolute())]
-    directory_format: str = ""
+    directories: list[Directory] = [Directory(path=Path("__user_data__").absolute())]
+    directory_format: Path = Path()
 
 
 class DownloadPathSetup(GlobalXPathSetup):
-    filename_format: str = ""
+    filename_format: Path = Path()
     text_length: int = 255
     date_format: str = "%Y-%m-%d"
     overwrite_files: bool = True
 
 
 class Trash(BaseModel):
     cleanup: bool = True
@@ -61,64 +61,85 @@
 
 
 class Downloader(ToolSettings):
     pass
 
 
 class SSHConnection(BaseModel):
+    username: str | None = None
+    private_key_filepath: Path | None = None
+    private_key_password: str | None = None
     host: str | None = None
     port: int = 22
-    username: str = "UltimaRoot"
-    private_key_filepath: Path | None = Path() or None
-    private_key_password: str | None = None
-    local_bind_port: list[int] = [10022]
 
 
 class DatabaseInfo(BaseModel):
-    name: str = "UltimaDB"
-    username: str = "postgres"
-    password: str = "password"
+    name: str = "ultima"
+    username: str | None = None
+    password: str | None = None
+    host: str = "localhost"
     port: int = 5432
+    ssh: SSHConnection = SSHConnection()
+
+
+class Database(BaseModel):
+    connection_info: DatabaseInfo = DatabaseInfo()
+    main: bool = True
+    active: bool = True
 
 
 class Tools(BaseModel):
     renamer: Renamer = Renamer()
     reformatter: Reformatter = Reformatter()
     downloader: Downloader = Downloader()
 
 
+auto_types = list[int | str] | StrictInt | StrictStr | StrictBool | None
+
+
+class GlobalAPI(GlobalAPI):
+    auto_profile_choice: auto_types = None
+    auto_performer_choice: auto_types = None
+    auto_content_choice: auto_types = None
+    auto_media_choice: auto_types = None
+    jobs = Jobs()
+    metadata_setup = GlobalXPathSetup()
+    metadata_setup.directory_format = (
+        "{site_name}/{first_letter}/{model_username}/Metadata"
+    )  # type: ignore
+    download_setup = DownloadPathSetup()
+    download_setup.directory_format = (
+        "{site_name}/{first_letter}/{model_username}/{api_type}/{value}/{media_type}"
+    )  # type: ignore
+    download_setup.filename_format = "{filename}.{ext}"  # type: ignore
+    video_quality = "source"
+    blacklists: list[str] = []
+
+
+class Sites(Sites):
+    class OnlyFansAPIConfig(OnlyFansAPIConfig, GlobalAPI):
+        pass
+
+    class FanslyAPIConfig(FanslyAPIConfig, GlobalAPI):
+        pass
+
+    onlyfans: OnlyFansAPIConfig = OnlyFansAPIConfig(auto_content_choice=True)
+    fansly: FanslyAPIConfig = FanslyAPIConfig()
+
+
+site_config_types = Sites.OnlyFansAPIConfig | Sites.FanslyAPIConfig
+
+
 class UltimaScraperCollectionConfig(UltimaScraperAPIConfig):
-    class _Settings(Settings):
+    class Settings(Settings):
         auto_site_choice: str = ""
+        databases: list[Database] = [Database()]
         tools: Tools = Tools()
         trash = Trash()
         infinite_loop: bool = False
-        exit_on_completetion: bool = True
-
-    class _Sites(Sites):
-        class _GlobalAPI(GlobalAPI):
-            auto_profile_choice: int | str | bool | None = None
-            auto_performer_choice: int | str | bool | None = None
-            auto_content_choice: int | str | bool | None = None
-            auto_media_choice: int | str | bool | None = None
-            jobs = Jobs()
-            metadata_setup = GlobalXPathSetup()
-            metadata_setup.directory_format = (
-                "{site_name}/{first_letter}/{model_username}/Metadata"
-            )
-            download_setup = DownloadPathSetup()
-            download_setup.directory_format = "{site_name}/{first_letter}/{model_username}/{api_type}/{value}/{media_type}"
-            download_setup.filename_format = "{filename}.{ext}"
-            video_quality = "source"
-            pass
-
-        class _OnlyFansAPI(OnlyFansAPI, _GlobalAPI):
-            pass
-
-        class _FanslyAPI(FanslyAPI, _GlobalAPI):
-            pass
+        exit_on_completion: bool = True
 
-        onlyfans: _OnlyFansAPI = _OnlyFansAPI()
-        fansly: _FanslyAPI = _FanslyAPI()
+        def get_main_database(self):
+            return [x for x in self.databases if x.main][0]
 
-    settings: _Settings = _Settings()
-    site_apis: _Sites = _Sites()
+    settings: Settings = Settings()
+    site_apis: Sites = Sites()
```

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,127 +1,135 @@
 from pathlib import Path
-from typing import Any, Union
+from typing import TYPE_CHECKING, Any
 
-from ultima_scraper_api.apis.fansly.classes.auth_model import AuthModel
-from ultima_scraper_api.apis.fansly.classes.message_model import create_message
-from ultima_scraper_api.apis.fansly.classes.post_model import create_post
-from ultima_scraper_api.apis.fansly.classes.story_model import create_story
-from ultima_scraper_api.apis.fansly.classes.user_model import create_user
-from ultima_scraper_api.apis.fansly.fansly import FanslyAPI
+from ultima_scraper_api.apis.onlyfans.onlyfans import OnlyFansAPI
+from ultima_scraper_renamer.reformat import ReformatManager
+
+from ultima_scraper_collection.config import Sites
 from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
     ContentMetadata,
+    ApiExtractor,
 )
 from ultima_scraper_collection.managers.option_manager import OptionManager
+from ultima_scraper_collection.managers.server_manager import ServerManager
 from ultima_scraper_collection.modules.module_streamliner import StreamlinedDatascraper
-from ultima_scraper_renamer.reformat import ReformatManager
 
+if TYPE_CHECKING:
+    from ultima_scraper_api.apis.onlyfans.classes.auth_model import AuthModel
+    from ultima_scraper_api.apis.onlyfans.classes.hightlight_model import (
+        create_highlight,
+    )
+    from ultima_scraper_api.apis.onlyfans.classes.message_model import create_message
+    from ultima_scraper_api.apis.onlyfans.classes.post_model import create_post
+    from ultima_scraper_api.apis.onlyfans.classes.story_model import create_story
+    from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
 
-class FanslyDataScraper(StreamlinedDatascraper):
-    def __init__(self, api: FanslyAPI, option_manager: OptionManager) -> None:
+
+class OnlyFansDataScraper(StreamlinedDatascraper):
+    def __init__(
+        self,
+        api: OnlyFansAPI,
+        option_manager: OptionManager,
+        server_manager: ServerManager,
+        site_config: Sites.OnlyFansAPIConfig,
+    ) -> None:
         self.api = api
         self.option_manager = option_manager
-        StreamlinedDatascraper.__init__(self, self)
+        self.site_config = site_config
+        StreamlinedDatascraper.__init__(self, self, server_manager)
 
     # Scrapes the API for content
     async def media_scraper(
         self,
-        post_result: Union[create_story, create_post, create_message],
-        subscription: create_user,
+        content_result: "create_story | create_post | create_message",
+        subscription: "create_user",
         api_type: str,
     ) -> dict[str, Any]:
+        api_type = self.api.convert_api_type_to_key(content_result)
         authed = subscription.get_authed()
-        api = authed.api
-        site_settings = api.get_site_settings()
-        if not site_settings:
-            return {}
+        site_config = self.site_config
         new_set: dict[str, Any] = {"content": []}
         directories: list[Path] = []
         if api_type == "Stories":
             pass
-        if api_type == "Archived":
-            pass
         if api_type == "Posts":
             pass
         if api_type == "Messages":
             pass
-        from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
-            Extractor,
-        )
 
-        content_metadata = ContentMetadata(post_result.id, api_type)
-        content_metadata.resolve_extractor(Extractor(post_result))
-        matches = [
-            s for s in site_settings.ignored_keywords if s in content_metadata.text
-        ]
-        if matches:
-            print("Ignoring - ", f"PostID: {content_metadata.content_id}")
-            return {}
+        content_metadata = ContentMetadata(content_result.id, api_type)
+        await content_metadata.resolve_extractor(ApiExtractor(content_result))
         for asset in content_metadata.medias:
             if asset.urls:
                 reformat_manager = ReformatManager(authed, self.filesystem_manager)
                 reformat_item = reformat_manager.prepare_reformat(asset)
                 file_directory = reformat_item.reformat(
-                    site_settings.file_directory_format
+                    site_config.download_setup.directory_format
                 )
                 reformat_item.directory = file_directory
-                file_path = reformat_item.reformat(site_settings.filename_format)
+                file_path = reformat_item.reformat(
+                    site_config.download_setup.filename_format
+                )
                 asset.directory = file_directory
                 asset.filename = file_path.name
 
                 if file_directory not in directories:
                     directories.append(file_directory)
         new_set["content"].append(content_metadata)
         new_set["directories"] = directories
         return new_set
 
-    async def get_all_stories(self, subscription: create_user):
+    async def get_all_stories(self, subscription: "create_user"):
         """
         get_all_stories(subscription: create_user)
 
-        This function returns a list of all stories and archived stories from the given subscription.
+        This function returns a list of all stories and highlights from the given subscription.
 
         Arguments:
         subscription (create_user): An instance of the create_user class.
 
         Returns:
-        list[create_story]: A list containing all stories and archived stories from the subscription.
+        list[create_highlight | create_story]: A list containing all stories and highlights from the subscription.
         """
-        master_set: list[create_story] = []
+        master_set: list[create_highlight | create_story] = []
         master_set.extend(await subscription.get_stories())
-        # master_set.extend(await subscription.get_archived_stories())
+        master_set.extend(await subscription.get_archived_stories())
+        highlights = await subscription.get_highlights()
+        valid_highlights: list[create_highlight | create_story] = []
+        for highlight in highlights:
+            resolved_highlight = await subscription.get_highlights(
+                hightlight_id=highlight.id
+            )
+            valid_highlights.extend(resolved_highlight)
+        master_set.extend(valid_highlights)
         return master_set
 
-    async def get_all_posts(self, subscription: create_user):
+    async def get_all_posts(self, subscription: "create_user"):
         temp_master_set = await subscription.get_posts()
-        collections = await subscription.get_collections()
-        for collection in collections:
-            temp_master_set.append(
-                await subscription.get_collection_content(collection)
-            )
+        # get_archived_posts uses normal posts
+        await subscription.get_archived_posts()
         return temp_master_set
 
     async def get_all_subscriptions(
         self,
-        authed: AuthModel,
+        authed: "AuthModel",
         identifiers: list[int | str] = [],
         refresh: bool = True,
     ):
         """
         get_all_subscriptions(authed: AuthModel, identifiers: list[int | str] = [], refresh: bool = True)
 
-        This function returns a list of all subscriptions, including both subscriptions and followings,
-        from the given authenticated user.
+        This function returns a list of all subscriptions from the given authenticated user.
 
         Arguments:
         authed (AuthModel): An instance of the AuthModel class.
         identifiers (list[int | str], optional): A list of identifiers (username or id) for the subscriptions. Defaults to an empty list.
         refresh (bool, optional): A flag indicating whether to refresh the list of subscriptions. Defaults to True.
 
         Returns:
-        list[create_subscription]: A list of all subscriptions, including both subscriptions and followings, from the authenticated user.
+        list[create_subscription]: A list of all subscriptions, sorted by expiredAt, from the authenticated user.
         """
-        authed.followed_users = await authed.get_followings(identifiers=identifiers)
         subscriptions = await authed.get_subscriptions(
             identifiers=identifiers, refresh=refresh, sub_type="active"
         )
-        subscriptions.sort(key=lambda x: x.ends_at)
+        subscriptions.sort(key=lambda x: x.subscribed_by_expire_date)
         return subscriptions
```

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,130 +1,130 @@
 from pathlib import Path
-from typing import Any, Union
+from typing import TYPE_CHECKING, Any
 
-from ultima_scraper_api.apis.onlyfans.classes.auth_model import AuthModel
-from ultima_scraper_api.apis.onlyfans.classes.hightlight_model import create_highlight
-from ultima_scraper_api.apis.onlyfans.classes.message_model import create_message
-from ultima_scraper_api.apis.onlyfans.classes.post_model import create_post
-from ultima_scraper_api.apis.onlyfans.classes.story_model import create_story
-from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
-from ultima_scraper_api.apis.onlyfans.onlyfans import OnlyFansAPI
+from ultima_scraper_api.apis.fansly.fansly import FanslyAPI
+from ultima_scraper_renamer.reformat import ReformatManager
+
+from ultima_scraper_collection.config import Sites
 from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
+    ApiExtractor,
     ContentMetadata,
 )
 from ultima_scraper_collection.managers.option_manager import OptionManager
+from ultima_scraper_collection.managers.server_manager import ServerManager
 from ultima_scraper_collection.modules.module_streamliner import StreamlinedDatascraper
-from ultima_scraper_renamer.reformat import ReformatManager
 
+if TYPE_CHECKING:
+    from ultima_scraper_api.apis.fansly.classes.auth_model import AuthModel
+    from ultima_scraper_api.apis.fansly.classes.message_model import create_message
+    from ultima_scraper_api.apis.fansly.classes.post_model import create_post
+    from ultima_scraper_api.apis.fansly.classes.story_model import create_story
+    from ultima_scraper_api.apis.fansly.classes.user_model import create_user
 
-class OnlyFansDataScraper(StreamlinedDatascraper):
-    def __init__(self, api: OnlyFansAPI, option_manager: OptionManager) -> None:
+
+class FanslyDataScraper(StreamlinedDatascraper):
+    def __init__(
+        self,
+        api: FanslyAPI,
+        option_manager: OptionManager,
+        server_manager: ServerManager,
+        site_config: Sites.FanslyAPIConfig,
+    ) -> None:
         self.api = api
         self.option_manager = option_manager
-        StreamlinedDatascraper.__init__(self, self)
+        self.site_config = site_config
+        StreamlinedDatascraper.__init__(self, self, server_manager)
 
     # Scrapes the API for content
     async def media_scraper(
         self,
-        post_result: Union[create_story, create_post, create_message],
-        subscription: create_user,
+        content_result: "create_story | create_post | create_message",
+        subscription: "create_user",
         api_type: str,
     ) -> dict[str, Any]:
-        api_type = self.api.convert_api_type_to_key(post_result)
         authed = subscription.get_authed()
-        api = authed.api
-        site_settings = api.get_site_settings()
-        if not site_settings:
-            return {}
+        site_config = self.site_config
         new_set: dict[str, Any] = {"content": []}
         directories: list[Path] = []
         if api_type == "Stories":
             pass
+        if api_type == "Archived":
+            pass
         if api_type == "Posts":
             pass
         if api_type == "Messages":
             pass
-        from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
-            Extractor,
-        )
 
-        content_metadata = ContentMetadata(post_result.id, api_type)
-        content_metadata.resolve_extractor(Extractor(post_result))
-        matches = [
-            s for s in site_settings.ignored_keywords if s in content_metadata.text
-        ]
-        if matches:
-            print("Ignoring - ", f"PostID: {content_metadata.content_id}")
-            return {}
+        content_metadata = ContentMetadata(content_result.id, api_type)
+        await content_metadata.resolve_extractor(ApiExtractor(content_result))
         for asset in content_metadata.medias:
             if asset.urls:
                 reformat_manager = ReformatManager(authed, self.filesystem_manager)
                 reformat_item = reformat_manager.prepare_reformat(asset)
                 file_directory = reformat_item.reformat(
-                    site_settings.file_directory_format
+                    site_config.download_setup.directory_format
                 )
                 reformat_item.directory = file_directory
-                file_path = reformat_item.reformat(site_settings.filename_format)
+                file_path = reformat_item.reformat(
+                    site_config.download_setup.filename_format
+                )
                 asset.directory = file_directory
                 asset.filename = file_path.name
 
                 if file_directory not in directories:
                     directories.append(file_directory)
         new_set["content"].append(content_metadata)
         new_set["directories"] = directories
         return new_set
 
-    async def get_all_stories(self, subscription: create_user):
+    async def get_all_stories(self, subscription: "create_user"):
         """
         get_all_stories(subscription: create_user)
 
-        This function returns a list of all stories and highlights from the given subscription.
+        This function returns a list of all stories and archived stories from the given subscription.
 
         Arguments:
         subscription (create_user): An instance of the create_user class.
 
         Returns:
-        list[create_highlight | create_story]: A list containing all stories and highlights from the subscription.
+        list[create_story]: A list containing all stories and archived stories from the subscription.
         """
-        master_set: list[create_highlight | create_story] = []
+        master_set: list["create_story"] = []
         master_set.extend(await subscription.get_stories())
-        master_set.extend(await subscription.get_archived_stories())
-        highlights = await subscription.get_highlights()
-        valid_highlights: list[create_highlight | create_story] = []
-        for highlight in highlights:
-            resolved_highlight = await subscription.get_highlights(
-                hightlight_id=highlight.id
-            )
-            valid_highlights.extend(resolved_highlight)
-        master_set.extend(valid_highlights)
+        # master_set.extend(await subscription.get_archived_stories())
         return master_set
 
-    async def get_all_posts(self, subscription: create_user):
+    async def get_all_posts(self, subscription: "create_user"):
         temp_master_set = await subscription.get_posts()
-        # get_archived_posts uses normal posts
-        await subscription.get_archived_posts()
+        collections = await subscription.get_collections()
+        for collection in collections:
+            temp_master_set.append(
+                await subscription.get_collection_content(collection)
+            )
         return temp_master_set
 
     async def get_all_subscriptions(
         self,
-        authed: AuthModel,
+        authed: "AuthModel",
         identifiers: list[int | str] = [],
         refresh: bool = True,
     ):
         """
         get_all_subscriptions(authed: AuthModel, identifiers: list[int | str] = [], refresh: bool = True)
 
-        This function returns a list of all subscriptions from the given authenticated user.
+        This function returns a list of all subscriptions, including both subscriptions and followings,
+        from the given authenticated user.
 
         Arguments:
         authed (AuthModel): An instance of the AuthModel class.
         identifiers (list[int | str], optional): A list of identifiers (username or id) for the subscriptions. Defaults to an empty list.
         refresh (bool, optional): A flag indicating whether to refresh the list of subscriptions. Defaults to True.
 
         Returns:
-        list[create_subscription]: A list of all subscriptions, sorted by expiredAt, from the authenticated user.
+        list[create_subscription]: A list of all subscriptions, including both subscriptions and followings, from the authenticated user.
         """
+        authed.followed_users = await authed.get_followings(identifiers=identifiers)
         subscriptions = await authed.get_subscriptions(
             identifiers=identifiers, refresh=refresh, sub_type="active"
         )
-        subscriptions.sort(key=lambda x: x.subscribed_by_expire_date)
+        subscriptions.sort(key=lambda x: x.ends_at)
         return subscriptions
```

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/download_manager.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/download_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,16 +42,17 @@
             for media_item in download_item.medias
         ]
         _result = await asyncio.gather(*final_list, return_exceptions=True)
 
     async def drm_download(self, download_item: MediaMetadata):
         content_metadata = download_item.__content_metadata__
         authed = self.authed
-        site_settings = authed.get_api().get_site_settings()
         reformat_manager = ReformatManager(authed, self.filesystem_manager)
+        assert reformat_manager.filesystem_manager.directory_manager
+        site_config = reformat_manager.filesystem_manager.directory_manager.site_config
         drm = authed.drm
         media_item = download_item.__raw__
         assert drm and media_item
         mpd = await drm.get_mpd(media_item)
         pssh = await drm.get_pssh(mpd)
         responses: list[ClientResponse] = []
 
@@ -65,17 +66,21 @@
             download_item.key = key
             video_url, audio_url = [
                 drm.get_video_url(mpd, media_item),
                 drm.get_audio_url(mpd, media_item),
             ]
             download_item.urls = [video_url]
             reformat_item = reformat_manager.prepare_reformat(download_item)
-            file_directory = reformat_item.reformat(site_settings.file_directory_format)
+            file_directory = reformat_item.reformat(
+                site_config.download_setup.directory_format
+            )
             reformat_item.directory = file_directory
-            file_path = reformat_item.reformat(site_settings.filename_format)
+            file_path = reformat_item.reformat(
+                site_config.download_setup.filename_format
+            )
             download_item.directory = file_directory
             download_item.filename = file_path.name
             for media_url in video_url, audio_url:
                 drm_download_item = copy.copy(download_item)
                 drm_download_item = reformat_manager.drm_format(
                     media_url, drm_download_item
                 )
@@ -87,28 +92,36 @@
                 responses.append(response)
         return responses
 
     async def download(self, download_item: MediaMetadata):
         attempt = 0
         content_metadata = download_item.__content_metadata__
         db_content = content_metadata.__db_content__
-        if not db_content or not download_item.id:
-            return
-        db_media = db_content.find_media(download_item.id)
-        if not db_media:
-            return
         if not download_item.urls:
             return
+        db_media = None
+        db_filepath = None
+        if db_content:
+            assert download_item.id
+            db_media = await db_content.find_media(download_item.id)
+            if not db_media:
+                return
+            db_filepath = await db_media.find_filepath(
+                db_content.id, content_metadata.api_type
+            )
+            assert db_filepath
+            db_filepath.preview = download_item.preview
+
         matches = ["us", "uk", "ca", "ca2", "de"]
         p_url = urlparse(download_item.urls[0])
 
         subdomain = p_url.hostname.split(".")[0]
         if any(subdomain in nm for nm in matches):
             return
-        download_item.__db_item__ = db_media
+        download_item.__db_media__ = db_media
 
         authed = self.authed
         authed_drm = authed.drm
 
         async with self.session_manager.semaphore:
             while attempt < self.session_manager.max_attempts + 1:
                 try:
@@ -168,16 +181,21 @@
                         if not formatted:
                             pass
                         final_size = download_path.stat().st_size
                     timestamp = db_media.created_at.timestamp()
                     await main_helper.format_file(
                         download_path, timestamp, self.reformat
                     )
-                    db_media.size = download_item.size = final_size
-                    db_media.downloaded = True
+                    if db_media and db_filepath:
+                        if not db_filepath.preview:
+                            db_media.size = download_item.size = final_size
+                        else:
+                            if final_size > db_media.size:
+                                db_media.size = final_size
+                        db_filepath.downloaded = True
                     break
                 except asyncio.TimeoutError as _e:
                     continue
 
     async def writer(
         self,
         result: ClientResponse,
@@ -188,27 +206,27 @@
             if download_item.drm and encrypted:
                 download_item = copy.copy(download_item)
                 download_item = self.reformat_manager.drm_format(
                     response.url.human_repr(), download_item
                 )
             assert download_item.directory and download_item.filename
             download_path = Path(download_item.directory, download_item.filename)
-            db_media = copy.copy(download_item.__db_item__)
+            db_media = copy.copy(download_item.__db_media__)
             db_media.directory = download_item.directory
             db_media.filename = download_item.filename
             download = await self.check(db_media, response)
             if not download:
                 return download_path, None
             failed = await self.filesystem_manager.write_data(response, download_path)
             return download_path, failed
 
     async def drm_check_downloaded(self, download_item: MediaMetadata):
         download_path = download_item.get_filepath()
         if download_path.exists():
-            if download_path.stat().st_size and download_item.__db_item__.size:
+            if download_path.stat().st_size and download_item.__db_media__.size:
                 return True
         return False
 
     async def check(self, download_item: TemplateMediaModel, response: ClientResponse):
         filepath = Path(download_item.directory, download_item.filename)
         response_status = False
         if response.status == 200:
```

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/filesystem_manager.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/filesystem_manager.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,33 +3,36 @@
 import copy
 import os
 import shutil
 from datetime import datetime
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Generator, Literal
 
+from ultima_scraper_api.classes.prepare_metadata import format_attributes
 import ultima_scraper_api
 from aiohttp.client_reqrep import ClientResponse
-from ultima_scraper_api.classes.prepare_directories import FormatTypes
 from ultima_scraper_api.helpers.main_helper import open_partial
 from ultima_scraper_api.managers.session_manager import EXCEPTION_TEMPLATE
 from ultima_scraper_renamer.reformat import ReformatItem
 
+
 if TYPE_CHECKING:
     api_types = ultima_scraper_api.api_types
     user_types = ultima_scraper_api.user_types
+    from ultima_scraper_collection import datascraper_types
+    from ultima_scraper_collection.config import site_config_types
 
 
 class FilesystemManager:
     def __init__(self) -> None:
         self.user_data_directory = Path("__user_data__")
         self.trash_directory = self.user_data_directory.joinpath("trash")
         self.profiles_directory = self.user_data_directory.joinpath("profiles")
         self.devices_directory = self.user_data_directory.joinpath("devices")
-        self.settings_directory = Path("__settings__")
+        self.settings_directory = Path("__user_data__")
         self.ignore_files = ["desktop.ini", ".DS_Store", ".DS_store", "@eaDir"]
         self.directory_manager: DirectoryManager | None = None
         self.directory_manager_users: dict[int, DirectoryManager] = {}
         self.file_manager_users: dict[int, FileManager] = {}
 
     def __iter__(self):
         for each in self.__dict__.values():
@@ -53,26 +56,25 @@
 
     def get_directory_manager(self, user_id: int):
         return self.directory_manager_users[user_id]
 
     def get_file_manager(self, user_id: int):
         return self.file_manager_users[user_id]
 
-    def activate_directory_manager(self, api: api_types):
-        from ultima_scraper_api.helpers import main_helper
+    def activate_directory_manager(self, site_config: site_config_types):
+        from ultima_scraper_collection.helpers import main_helper
 
-        site_settings = api.get_site_settings()
         root_metadata_directory = main_helper.check_space(
-            site_settings.metadata_directories
+            site_config.metadata_setup.directories
         )
         root_download_directory = main_helper.check_space(
-            site_settings.download_directories
+            site_config.download_setup.directories
         )
         self.directory_manager = DirectoryManager(
-            site_settings,
+            site_config,
             root_metadata_directory,
             root_download_directory,
         )
 
     def trash(self):
         pass
 
@@ -113,21 +115,24 @@
         else:
             if response.content_length:
                 pass
                 # progress_bar.update_total_size(-response.content_length)
             status_code = 2
         return status_code
 
-    async def create_directory_manager(self, api: api_types, user: user_types):
+    async def create_directory_manager(
+        self, datascraper: datascraper_types, user: user_types
+    ):
         # profile_directory = filesystem_directory_manager.profile.root_directory.joinpath(
         #     self.username
         # )
+        api = datascraper.api
         if self.directory_manager:
             directory_manager = DirectoryManager(
-                api.get_site_settings(),
+                datascraper.site_config,
                 self.directory_manager.root_metadata_directory,
                 self.directory_manager.root_download_directory,
             )
             option = {
                 "site_name": api.site_name,
                 "profile_username": user.username,
                 "model_username": user.username,
@@ -146,84 +151,79 @@
             # f_d_p_2.mkdir(parents=True, exist_ok=True)
             self.directory_manager_users[user.id] = directory_manager
             self.file_manager_users[user.id] = FileManager(directory_manager)
             return directory_manager
 
     async def format_directories(self, subscription: user_types) -> DirectoryManager:
         directory_manager = self.get_directory_manager(subscription.id)
+        site_config = directory_manager.site_config
         file_manager = self.get_file_manager(subscription.id)
         authed = subscription.get_authed()
         api = authed.api
-        site_settings = authed.api.get_site_settings()
-        if site_settings:
-            authed_username = authed.username
-            subscription_username = subscription.username
-            site_name = authed.api.site_name
-            reformat_item = ReformatItem()
-            reformat_item.site_name = site_name
-            reformat_item.profile_username = authed_username
-            reformat_item.model_username = subscription_username
-            reformat_item.date = datetime.today()
-            reformat_item.date_format = site_settings.date_format
-            reformat_item.text_length = site_settings.text_length
-            reformat_item.directory = directory_manager.root_metadata_directory
-            string = reformat_item.reformat(site_settings.metadata_directory_format)
-            directory_manager.user.metadata_directory = Path(string)
-            reformat_item_2 = copy.copy(reformat_item)
-            reformat_item_2.directory = directory_manager.root_download_directory
-            string = reformat_item_2.reformat(site_settings.file_directory_format)
-            formtatted_root_download_directory = reformat_item_2.remove_non_unique(
-                directory_manager, "file_directory_format"
-            )
-            directory_manager.user.download_directory = (
-                formtatted_root_download_directory
-            )
-            await file_manager.set_default_files(reformat_item, reformat_item_2)
-            _metadata_filepaths = await file_manager.find_metadata_files(
-                legacy_files=False
-            )
-            # I forgot why we need to set default file twice
-            await file_manager.set_default_files(reformat_item, reformat_item_2)
-            user_metadata_directory = directory_manager.user.metadata_directory
-            _user_download_directory = directory_manager.user.download_directory
-            legacy_metadata_directory = user_metadata_directory
+        authed_username = authed.username
+        subscription_username = subscription.username
+        site_name = authed.api.site_name
+        reformat_item = ReformatItem()
+        reformat_item.site_name = site_name
+        reformat_item.profile_username = authed_username
+        reformat_item.model_username = subscription_username
+        reformat_item.date = datetime.today()
+        download_setup = site_config.download_setup
+        reformat_item.date_format = download_setup.date_format
+        reformat_item.text_length = download_setup.text_length
+        reformat_item.directory = directory_manager.root_metadata_directory
+        metadata_setup = site_config.metadata_setup
+        string = reformat_item.reformat(metadata_setup.directory_format)
+        directory_manager.user.metadata_directory = Path(string)
+        reformat_item_2 = copy.copy(reformat_item)
+        reformat_item_2.directory = directory_manager.root_download_directory
+        string = reformat_item_2.reformat(metadata_setup.directory_format)
+        formtatted_root_download_directory = reformat_item_2.remove_non_unique(
+            directory_manager, "file_directory_format"
+        )
+        directory_manager.user.download_directory = formtatted_root_download_directory
+        await file_manager.set_default_files(reformat_item, reformat_item_2)
+        _metadata_filepaths = await file_manager.find_metadata_files(legacy_files=False)
+        # I forgot why we need to set default file twice
+        await file_manager.set_default_files(reformat_item, reformat_item_2)
+        user_metadata_directory = directory_manager.user.metadata_directory
+        _user_download_directory = directory_manager.user.download_directory
+        legacy_metadata_directory = user_metadata_directory
+        directory_manager.user.legacy_metadata_directories.append(
+            legacy_metadata_directory
+        )
+        items = api.ContentTypes().__dict__.items()
+        for api_type, _ in items:
+            legacy_metadata_directory_2 = user_metadata_directory.joinpath(api_type)
             directory_manager.user.legacy_metadata_directories.append(
-                legacy_metadata_directory
-            )
-            items = api.ContentTypes().__dict__.items()
-            for api_type, _ in items:
-                legacy_metadata_directory_2 = user_metadata_directory.joinpath(api_type)
-                directory_manager.user.legacy_metadata_directories.append(
-                    legacy_metadata_directory_2
-                )
-            legacy_model_directory = directory_manager.root_download_directory.joinpath(
-                site_name, subscription_username
-            )
-            directory_manager.user.legacy_download_directories.append(
-                legacy_model_directory
+                legacy_metadata_directory_2
             )
+        legacy_model_directory = directory_manager.root_download_directory.joinpath(
+            site_name, subscription_username
+        )
+        directory_manager.user.legacy_download_directories.append(
+            legacy_model_directory
+        )
         return directory_manager
 
 
-from ultima_scraper_api.classes.make_settings import SiteSettings
-
-
 class DirectoryManager:
     def __init__(
         self,
-        site_settings: SiteSettings,
+        site_config: site_config_types,
         root_metadata_directory: Path = Path(),
         root_download_directory: Path = Path(),
     ) -> None:
         self.root_directory = Path()
         self.root_metadata_directory = Path(root_metadata_directory)
         self.root_download_directory = Path(root_download_directory)
         # self.profile = self.ProfileDirectories(Path(profile_directory))
         self.user = self.UserDirectories()
-        formats = FormatTypes(site_settings)
+        self.site_config = site_config
+        formats = FormatTypes(site_config)
         string, status = formats.check_rules()
         if not status:
             print(string)
             exit(0)
         self.formats = formats
         pass
 
@@ -327,7 +327,103 @@
                         continue
                     new_list.append(filepath)
                 case ".json":
                     new_list.append(filepath)
                 case _:
                     pass
         return new_list
+
+
+class FormatTypes:
+    def __init__(self, site_settings: site_config_types) -> None:
+        self.metadata_directory_format = site_settings.metadata_setup.directory_format
+        self.file_directory_format = site_settings.download_setup.directory_format
+        self.filename_format = site_settings.download_setup.filename_format
+
+    def check_rules(self):
+        """Checks for invalid filepath
+
+        Returns:
+            tuple(str,bool): Returns a string which explains invalid filepath format
+        """
+        bool_status = True
+        wl = []
+        invalid_list = []
+        string = ""
+        for key, _value in self:
+            if key == "file_directory_format":
+                bl = format_attributes()
+                wl = [v for _k, v in bl.__dict__.items()]
+                bl = bl.whitelist(wl)
+                invalid_list = []
+                for b in bl:
+                    if b in self.file_directory_format.as_posix():
+                        invalid_list.append(b)
+            if key == "filename_format":
+                bl = format_attributes()
+                wl = [v for _k, v in bl.__dict__.items()]
+                bl = bl.whitelist(wl)
+                invalid_list = []
+                for b in bl:
+                    if b in self.filename_format.as_posix():
+                        invalid_list.append(b)
+            if key == "metadata_directory_format":
+                wl = [
+                    "{site_name}",
+                    "{first_letter}",
+                    "{model_id}",
+                    "{profile_username}",
+                    "{model_username}",
+                ]
+                bl = format_attributes().whitelist(wl)
+                invalid_list: list[str] = []
+                for b in bl:
+                    if b in self.metadata_directory_format.as_posix():
+                        invalid_list.append(b)
+            if invalid_list:
+                string += f"You cannot use {','.join(invalid_list)} in {key}. Use any from this list {','.join(wl)}"
+                bool_status = False
+
+        return string, bool_status
+
+    def check_unique(self):
+        values: list[str] = []
+        unique = []
+        new_format_copied = copy.deepcopy(self)
+        option: dict[str, Any] = {}
+        option["string"] = ""
+        option["bool_status"] = True
+        option["unique"] = new_format_copied
+        f = format_attributes()
+        for key, value in self:
+            value: Path
+            if key == "file_directory_format":
+                unique = ["{media_id}", "{model_username}"]
+                values = list(value.parts)
+                option["unique"].file_directory_format = unique
+            elif key == "filename_format":
+                values = []
+                unique = ["{media_id}", "{filename}"]
+                for _key2, value2 in f:
+                    if value2 in value.as_posix():
+                        values.append(value2)
+                option["unique"].filename_format = unique
+            elif key == "metadata_directory_format":
+                unique = ["{model_username}"]
+                values = list(value.parts)
+                option["unique"].metadata_directory_format = unique
+            if key != "filename_format":
+                e = [x for x in values if x in unique]
+            else:
+                e = [x for x in unique if x in values]
+            if e:
+                setattr(option["unique"], key, e)
+            else:
+                option[
+                    "string"
+                ] += f"{key} is a invalid format since it has no unique identifiers. Use any from this list {','.join(unique)}\n"
+                option["bool_status"] = False
+        return option
+
+    def __iter__(self):
+        for attr, value in self.__dict__.items():
+            yield attr, value
```

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,84 +1,123 @@
+import mimetypes
 from datetime import datetime
 from pathlib import Path
-from typing import Any
+from typing import Any, TypedDict
 from urllib.parse import ParseResult, urlparse
 
 import ultima_scraper_api
 from sqlalchemy import inspect
+from ultima_scraper_api.helpers import main_helper
+from ultima_scraper_db.databases.ultima.schemas.templates.site import (
+    MediaModel as DBMediaModel,
+)
+from ultima_scraper_db.databases.ultima.schemas.templates.site import (
+    MessageModel as DBMessageModel,
+)
+from ultima_scraper_db.databases.ultima.schemas.templates.site import (
+    PostModel as DBPostModel,
+)
+from ultima_scraper_db.databases.ultima.schemas.templates.site import (
+    StoryModel as DBStoryModel,
+)
+
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.sqlite_database import (
     DBCollection,
     SqliteDatabase,
 )
 from ultima_scraper_collection.managers.database_manager.database_manager import (
     DatabaseManager,
 )
 from ultima_scraper_collection.managers.filesystem_manager import FilesystemManager
 
 api_types = ultima_scraper_api.api_types
 user_types = ultima_scraper_api.user_types
 content_types = ultima_scraper_api.content_types
-from ultima_scraper_api.classes.prepare_metadata import format_content
-from ultima_scraper_api.helpers import main_helper
-from ultima_scraper_collection.managers.database_manager.connections.sqlite.models.api_model import (
-    ApiModel,
-)
-from ultima_scraper_collection.managers.database_manager.connections.sqlite.models.user_database import (
-    messages_table,
-)
 
 
-class MetadataExtractor:
-    def __init__(self, post_item: format_content.post_item) -> None:
-        self.item = post_item
+class DBContentExtractor:
+    def __init__(
+        self, content_item: DBMessageModel | DBPostModel | DBStoryModel
+    ) -> None:
+        self.item = content_item
+        self.__api__: api_types | None = None
 
     def get_id(self):
-        return self.item.post_id
+        return self.item.id
 
     def get_user_id(self):
-        return None
+        return self.item.user_id
 
     def get_text(self):
+        if isinstance(self.item, DBStoryModel):
+            return None
         return self.item.text
 
     def get_preview_ids(self):
         value: list[int] = []
         return value
 
     def resolve_archived(self):
         return False
 
     def get_date(self):
-        return self.item.createdAt
+        return self.item.created_at
 
-    def get_medias(self, content_metadata: "ContentMetadata"):
+    async def get_medias(self, content_metadata: "ContentMetadata"):
         final_assets: list[MediaMetadata] = []
-        for media in self.item.medias:
+        for media_item in self.item.media:
+            if not media_item.category:
+                from urllib.parse import urlparse
+
+                if not media_item.url:
+                    continue
+                parsed_url = urlparse(media_item.url)
+                path_ = parsed_url.path
+                type_, _encoding = mimetypes.guess_type(path_)
+                media_type = None
+                if type_:
+                    media_type, _subtype = type_.split("/")
+                assert media_type and self.__api__
+                true_media_type = self.__api__.MediaTypes().find_by_value(media_type)
+                pass
+            else:
+                true_media_type = media_item.category
+
             new_asset = MediaMetadata(
-                media.media_id,
-                media.media_type,
+                media_item.id,
+                true_media_type,
                 content_metadata,
-                created_at=content_metadata.created_at_string,
+                created_at=content_metadata.created_at,
+            )
+            new_asset.urls = [media_item.url]
+            filepath = await media_item.find_filepath(
+                content_metadata.content_id, content_metadata.api_type
             )
-            new_asset.urls = media.links
-            new_asset.directory = media.directory
-            new_asset.filename = media.filename
-            new_asset.size = media.size
+            if filepath:
+                pathed_filepath = Path(filepath.filepath)
+                new_asset.directory = pathed_filepath.parent
+                new_asset.filename = pathed_filepath.name
+            else:
+                pass
+            new_asset.size = media_item.size
             final_assets.append(new_asset)
         return final_assets
 
     def resolve_paid(self):
-        return self.item.paid
+        if not hasattr(self.item, "paid"):
+            return None
+        if isinstance(self.item, DBPostModel | DBMessageModel):
+            return self.item.paid
 
     def get_receiver_id(self):
-        if isinstance(self.item, messages_table):
-            return
+        if isinstance(self.item, DBMessageModel):
+            return self.item.receiver_id
 
 
-class Extractor:
+class ApiExtractor:
     def __init__(self, item: content_types) -> None:
         self.item = item
 
     def get_id(self):
         return self.item.id
 
     def get_user_id(self):
@@ -99,15 +138,15 @@
         elif isinstance(self.item, ultima_scraper_api.message_types):
             final_preview_ids = self.item.previews
         else:
             final_preview_ids = []
         return final_preview_ids
 
     def get_date(self):
-        temp_date = self.item.createdAt
+        temp_date = self.item.created_at
         assert temp_date
         if isinstance(temp_date, str):
             try:
                 temp_date = float(temp_date)
             except:
                 pass
         default_date = datetime.utcnow()
@@ -117,31 +156,39 @@
             if not temp_date:
                 temp_date = default_date
             if isinstance(temp_date, int):
                 timestamp = float(temp_date)
                 date_object = datetime.fromtimestamp(timestamp)
             elif isinstance(temp_date, float):
                 date_object = datetime.fromtimestamp(temp_date)
-            else:
+            elif isinstance(temp_date, str):
                 date_object = datetime.fromisoformat(temp_date)
-        final_date_string = date_object.isoformat()
-        return final_date_string
+            else:
+                date_object = temp_date
+        return date_object
 
-    def get_medias(self, content_metadata: "ContentMetadata"):
+    async def get_medias(self, content_metadata: "ContentMetadata"):
         final_assets: list[MediaMetadata] = []
         for asset_metadata in self.item.media:
             raw_media_type = asset_metadata["type"]
             if "mimetype" in asset_metadata:
                 raw_media_type: str = asset_metadata["mimetype"].split("/")[0]
             author = self.item.get_author()
             media_type = author.get_api().MediaTypes().find_by_value(raw_media_type)
             if "createdAt" in asset_metadata:
-                media_created_at = asset_metadata["createdAt"]
+                if isinstance(asset_metadata["createdAt"], str):
+                    media_created_at = datetime.fromisoformat(
+                        asset_metadata["createdAt"]
+                    )
+                else:
+                    media_created_at = datetime.fromtimestamp(
+                        asset_metadata["createdAt"]
+                    )
             else:
-                media_created_at = content_metadata.created_at_string
+                media_created_at = content_metadata.created_at
             new_asset = MediaMetadata(
                 asset_metadata["id"],
                 media_type,
                 content_metadata,
                 created_at=media_created_at,
             )
             main_url = self.item.url_picker(asset_metadata)
@@ -175,62 +222,56 @@
             archived = self.item.isArchived
         return archived
 
     def resolve_paid(self):
         if getattr(self.item, "price", 0):
             if all(media["canView"] for media in self.item.media):
                 return True
-        return False
+            return False
+        else:
+            return None
 
     def get_receiver_id(self):
         if isinstance(self.item, ultima_scraper_api.message_types):
             return self.item.get_receiver().id
 
 
 class ContentMetadata:
     def __init__(self, content_id: int, api_type: str) -> None:
         self.content_id = content_id
         self.user_id: int | None = None
         self.receiver_id: int | None = None
-        self.text: str = ""
+        self.text: str | None = None
         self.preview_media_ids: list[int] | list[dict[str, Any]] = []
         self.archived: bool = False
-        self.created_at_string: str = ""
         self.medias: list[MediaMetadata] = []
         self.api_type = api_type
         self.price: float | None = None
-        self.paid: bool = False
+        self.paid: bool | None = False
         self.deleted: bool = False
         self.__raw__: Any | None = None
         self.__soft__: Any = None
-        self.__db_content__: ApiModel | None = None
+        self.__db_content__: DBStoryModel | DBPostModel | DBMessageModel | None = None
         self.__legacy__ = False
 
-    def resolve_extractor(self, result: Extractor | MetadataExtractor):
+    async def resolve_extractor(self, result: ApiExtractor | DBContentExtractor):
         self.content_id = result.get_id()
         self.user_id = result.get_user_id()
         self.receiver_id = result.get_receiver_id()
         self.text = result.get_text()
         self.preview_media_ids = result.get_preview_ids()
         self.archived = result.resolve_archived()
-        self.created_at_string = result.get_date()
-        self.medias: list[MediaMetadata] = result.get_medias(self)
+        self.medias: list[MediaMetadata] = await result.get_medias(self)
         self.price = getattr(result.item, "price", 0) or 0
         self.paid = result.resolve_paid()
         self.deleted = False
+        self.created_at: datetime = result.get_date()
         self.__raw__: Any | None = None
         self.__soft__ = result.item
-
-    def add_media(
-        self, media_id: int, media_type: str, urls: list[str], preview: bool = False
-    ):
-        urls = [url for url in urls if url]
-        new_media = MediaMetadata(media_id, media_type, urls, preview, self.created_at)
-        self.medias.append(new_media)
-        return new_media
+        self.__media_types__ = None
 
     def find_media(self, media_id: int | None = None, urls: list[str] = []):
         for asset in self.medias:
             if asset.id == media_id:
                 return asset
         for asset in self.medias:
             for url in urls:
@@ -252,35 +293,36 @@
                 if found_url:
                     return asset
 
 
 class MediaMetadata:
     def __init__(
         self,
-        media_id: int,
+        media_id: int | None,
         media_type: str,
         content_metadata: ContentMetadata,
         urls: list[str] = [],
         preview: bool = False,
-        created_at: str = "",
+        created_at: datetime = ...,
         drm: bool = False,
     ) -> None:
         self.id = int(media_id) if media_id is not None else None
         self.media_type = media_type
         self.urls: list[str] = urls
         self.preview = preview
         self.directory: Path | None = None
         self.filename: str | None = None
         self.size = 0
         self.linked = None
         self.drm = drm
         self.key: str = ""
-        self.created_at = created_at or content_metadata.created_at_string
+        self.created_at = created_at or content_metadata.created_at
         self.__raw__: Any | None = None
         self.__content_metadata__ = content_metadata
+        self.__db_media__: DBMediaModel | None = None
 
     def find_by_url(self, url: ParseResult):
         for media_url in self.urls:
             media_url = urlparse(media_url)
             url_path = url.path
             if "Protected" in url.path:
                 index = url.path.index("/files")
@@ -358,29 +400,31 @@
                 new_metadata_filepath.parent.mkdir(parents=True, exist_ok=True)
                 self.filesystem_manager.move(legacy_filepath, new_metadata_filepath)
         await self.filesystem_manager.format_directories(self.subscription)
         await self.fix_archived_db()
         self.metadatas = self.find_metadatas()
 
     def fix_json(self):
-        def merge_statuses(unmerged_status):
+        def merge_statuses(unmerged_status: dict[str, Any]):
             merged_status: list[dict[str, Any]] = [
                 val for lst in unmerged_status.values() for val in lst
             ]
             return merged_status
 
         for metadata_filepath in self.metadatas:
             if (
                 metadata_filepath.suffix != ".json"
                 or "__legacy__" in metadata_filepath.parts
             ):
                 continue
             final_content_type = None
             archive = False
-            new_metadata_set = main_helper.import_json(metadata_filepath)
+            new_metadata_set: list[dict[str, Any]] | dict[
+                str, Any
+            ] = main_helper.import_json(metadata_filepath)
             content_types = self.subscription.get_api().ContentTypes().get_keys()
             final_stem = metadata_filepath.stem
             if final_stem[-1].isdigit():
                 final_stem = final_stem.removesuffix(f"_{final_stem[-1]}")
             if final_stem in content_types:
                 final_content_type = final_stem
             else:
@@ -394,38 +438,40 @@
                     pass
                 if not final_content_type:
                     # If we get an key error here, we need to move the json file to correct folder or we can resolve it by getting content_type by looking at the directory path
                     # directory_set = set()
                     # merged = merge_statuses(new_metadata_set)
                     # for item in merged:
                     #     directory_set.add(item["directory"])
-                    if (
-                        "type" in new_metadata_set
-                        and "content_type" not in new_metadata_set
-                    ):
-                        item = new_metadata_set["valid"][0]
-                        directory = item["directory"]
-                        content_types = self.subscription.get_api().ContentTypes()
-                        temp_content_type = content_types.path_to_key(Path(directory))
-                        if all(
-                            temp_content_type
-                            == content_types.path_to_key(Path(item["directory"]))
-                            for item in new_metadata_set["valid"]
+                    if isinstance(new_metadata_set, dict):
+                        if (
+                            "type" in new_metadata_set
+                            and "content_type" not in new_metadata_set
                         ):
-                            final_content_type = temp_content_type
-                    else:
-                        final_content_type = new_metadata_set["content_type"]
+                            item = new_metadata_set["valid"][0]
+                            directory = item["directory"]
+                            content_types = self.subscription.get_api().ContentTypes()
+                            temp_content_type = content_types.path_to_key(
+                                Path(directory)
+                            )
+                            if all(
+                                temp_content_type
+                                == content_types.path_to_key(Path(item["directory"]))
+                                for item in new_metadata_set["valid"]
+                            ):
+                                final_content_type = temp_content_type
+                        else:
+                            final_content_type = new_metadata_set["content_type"]
             assert (
                 final_content_type
             ), "Content type (Posts,etc) not set before fixing JSON"
+
             final_metadata_set = {}
             content_json = {}
             if isinstance(new_metadata_set, list):
-                if len(new_metadata_set) > 1:
-                    pass
                 for temp_set in new_metadata_set:
                     content_json[temp_set["type"]] = {
                         "valid": temp_set["valid"],
                         "invalid": temp_set["invalid"],
                     }
                 final_metadata_set["version"] = 1.8
                 final_metadata_set["content"] = content_json
@@ -440,15 +486,21 @@
                     "invalid": new_metadata_set["invalid"],
                 }
                 final_metadata_set["version"] = 1.9
                 final_metadata_set["content"] = content_json
                 pass
             elif "type" in new_metadata_set:
                 # Usually means there's another json file we'd have to merge into this, like Images.json and Videos.json.
-                temp_content_json = {
+
+                class MetadataType(TypedDict):
+                    version: float | None
+                    content_type: str
+                    content: dict[str, Any]
+
+                temp_content_json: MetadataType = {
                     "version": 2.0,
                     "content_type": final_content_type,
                     "content": {},
                 }
                 temp_content_json["content"][new_metadata_set["type"]] = {
                     "valid": new_metadata_set["valid"],
                     "invalid": new_metadata_set["invalid"],
@@ -456,27 +508,27 @@
                 content_json = temp_content_json["content"]
                 final_metadata_set = temp_content_json
                 pass
             else:
                 content_json = new_metadata_set.get("content", new_metadata_set)
             if final_metadata_set:
                 final_metadata_set["content_type"] = final_content_type
-                main_helper.export_json(final_metadata_set, metadata_filepath)
+                main_helper.export_json(final_metadata_set.__dict__, metadata_filepath)
             for media_type, status in content_json.items():
                 merged_status = merge_statuses(status)
                 if merged_status:
                     for item_json in merged_status:
                         if not final_content_type:
                             raise Exception("content type not found")
 
                         def assign_metadata(
                             content_metadata: ContentMetadata, item_json: dict[str, Any]
                         ):
                             content_metadata.__legacy__ = True
-                            content_metadata.created_at_string = item_json["postedAt"]
+                            content_metadata.created_at = item_json["postedAt"]
                             content_metadata.paid = item_json.get("paid", False)
                             content_metadata.price = item_json.get("price", 0)
                             content_metadata.text = item_json["text"]
                             content_metadata.user_id = self.subscription.id
                             content_metadata.archived = archive
                             for asset_json in item_json.get("medias", [item_json]):
                                 urls = asset_json.get("links") or []
@@ -527,51 +579,14 @@
                                     item_json["post_id"], final_content_type
                                 )
                                 self.legacy_content_metadatas.append(content_metadata)
                             assign_metadata(content_metadata, item_json)
 
         return self.legacy_content_metadatas
 
-    def fix_sqlite(self):
-        subscription = self.subscription
-        if not self.db_manager:
-            raise Exception("DatabaseManager has not been assigned")
-
-        api = subscription.get_api()
-        site_settings = api.get_site_settings()
-        config = api.config
-        if not (config and site_settings):
-            return
-        # We could put this in process_legacy_metadata
-        legacy_db_manager = DatabaseManager().get_sqlite_db(
-            legacy_metadata_path, legacy=True
-        )
-
-        final_result = legacy_db_manager.legacy_sqlite_updater(api_type, subscription)
-        for metadata in final_result:
-            content_metadata = ContentMetadata(metadata.post_id, api_type)
-            augh = content_metadata.resolve_extractor(MetadataExtractor(metadata))
-            pass
-        new_metadata_object.extend(final_result)
-        return new_metadata_object
-
-    def delete_metadatas(self):
-        for legacy_metadata in self.redundant_metadatas:
-            if self.subscription.get_api().get_site_settings().delete_legacy_metadata:
-                legacy_metadata.unlink()
-            else:
-                if legacy_metadata.exists():
-                    new_filepath = Path(
-                        legacy_metadata.parent,
-                        "__legacy__",
-                        legacy_metadata.name,
-                    )
-                    new_filepath.parent.mkdir(exist_ok=True)
-                    legacy_metadata.rename(new_filepath)
-
     async def fix_archived_db(
         self,
     ):
         api = self.subscription.get_api()
         directory_manager = self.filesystem_manager.get_directory_manager(
             self.subscription.id
         )
@@ -612,15 +627,15 @@
                             return
                         archived_result = archived_db_manager.session.query(
                             table_name
                         ).all()
                         for item in archived_result:
                             result2 = (
                                 modern_database_session.query(table_name)
-                                .filter(table_name.post_id == item.post_id)
+                                .filter(table_name.post_id == item.post_id)  # type: ignore
                                 .first()
                             )
                             if not result2:
                                 item2 = item.__dict__
                                 item2.pop("id")
                                 item2.pop("_sa_instance_state")
                                 item = table_name(**item2)
```

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/managers/option_manager.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/managers/option_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 from typing import Any
-
+from ultima_scraper_collection.config import auto_types
 
 class OptionManager:
     def __init__(self) -> None:
         self.performer_options: OptionsFormat | None = None
         self.subscription_options: OptionsFormat | None = None
         pass
 
     async def create_option(
         self,
         items: list[Any],
         options_type: str,
-        auto_choice: list[int | str] | int | str | bool = False,
+        auto_choice: auto_types = False,
     ):
         option = await OptionsFormat(items, options_type, auto_choice).formatter()
         return option
 
 
 class OptionsFormat:
     def __init__(
         self,
         items: list[Any],
         options_type: str,
-        auto_choice: list[int | str] | int | str | bool = False,
+        auto_choice: auto_types = False,
     ) -> None:
         self.items = items
         self.item_keys: list[str] = []
         self.string = ""
         self.options_type = options_type
         self.auto_choice = auto_choice
         self.final_choices = []
 
     async def formatter(self):
         options_type = self.options_type
         final_string = f"Choose {options_type.capitalize()}: 0 = All"
-        if type(self.auto_choice) == int:
-            self.auto_choice = str(self.auto_choice)
-
-        if isinstance(self.auto_choice, str):
-            self.auto_choice = [x for x in self.auto_choice.split(",") if x]
-            self.auto_choice = (
-                True
-                if any(x in ["0", "all"] for x in self.auto_choice)
-                else self.auto_choice
+        auto_choice = self.auto_choice
+        if type(auto_choice) == int:
+            auto_choice = str(auto_choice)
+
+        if isinstance(auto_choice, str):
+            auto_choice = [x for x in auto_choice.split(",") if x]
+            auto_choice = (
+                True if any(x in ["0", "all"] for x in auto_choice) else auto_choice
             )
 
-        if isinstance(self.auto_choice, list):
-            self.auto_choice = [x for x in self.auto_choice if x]
+        if isinstance(auto_choice, list):
+            auto_choice = [x for x in auto_choice if x]
+        self.auto_choice = auto_choice
 
         match options_type:
             case "sites":
                 self.item_keys = self.items
                 my_string = " | ".join(
                     map(lambda x: f"{self.items.index(x)+1} = {x}", self.items)
                 )
```

### Comparing `ultima_scraper_collection-1.1.3/ultima_scraper_collection/modules/module_streamliner.py` & `ultima_scraper_collection-2.0.0/ultima_scraper_collection/modules/module_streamliner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,44 @@
 from __future__ import annotations
 
 import copy
 from itertools import product
 from typing import Any, Optional
 
 import ultima_scraper_api
-import ultima_scraper_api.classes.make_settings as make_settings
-from sqlalchemy.exc import OperationalError
+from sqlalchemy import and_, or_, select
 from tqdm.asyncio import tqdm_asyncio
-from ultima_scraper_collection.managers.database_manager.connections.sqlite.models.api_model import (
-    ApiModel,
-)
-from ultima_scraper_collection.managers.database_manager.connections.sqlite.sqlite_database import (
-    DBCollection,
-)
-from ultima_scraper_collection.managers.database_manager.database_manager import (
-    DatabaseManager,
+from ultima_scraper_db.databases.ultima.schemas.templates.site import (
+    MessageModel as DBMessageModel,
 )
+
+from ultima_scraper_collection.config import site_config_types
 from ultima_scraper_collection.managers.download_manager import DownloadManager
 from ultima_scraper_collection.managers.filesystem_manager import FilesystemManager
 from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
     MetadataManager,
 )
-from ultima_scraper_renamer import renamer
+from ultima_scraper_collection.managers.server_manager import ServerManager
 
 auth_types = ultima_scraper_api.auth_types
 user_types = ultima_scraper_api.user_types
 message_types = ultima_scraper_api.message_types
 error_types = ultima_scraper_api.error_types
 subscription_types = ultima_scraper_api.subscription_types
-
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from ultima_scraper_collection.managers.datascraper_manager.datascrapers.fansly import (
         FanslyDataScraper,
     )
     from ultima_scraper_collection.managers.datascraper_manager.datascrapers.onlyfans import (
         OnlyFansDataScraper,
     )
     from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
         ContentMetadata,
-        MediaMetadata,
     )
 
     datascraper_types = OnlyFansDataScraper | FanslyDataScraper
 
 
 class download_session(tqdm_asyncio):
     def start(
@@ -67,34 +60,36 @@
     def update_total_size(self, tsize: Optional[int]):
         if tsize:
             tsize = int(tsize)
             self.total += tsize
 
 
 class StreamlinedDatascraper:
-    def __init__(self, datascraper: datascraper_types) -> None:
+    def __init__(
+        self, datascraper: datascraper_types, server_manager: ServerManager
+    ) -> None:
         self.datascraper = datascraper
         self.filesystem_manager = FilesystemManager()
         self.content_types = self.datascraper.api.ContentTypes()
         self.media_types = self.datascraper.api.MediaTypes()
         self.user_list: set[user_types] = set()
         self.metadata_manager_users: dict[int, MetadataManager] = {}
+        self.server_manager: ServerManager = server_manager
 
     async def configure_datascraper_jobs(self):
         api = self.datascraper.api
-        site_settings = api.get_site_settings()
-        available_jobs = site_settings.jobs.scrape
+        site_config = self.datascraper.site_config
+        available_jobs = site_config.jobs.scrape
         option_manager = self.datascraper.option_manager
         performer_options = option_manager.performer_options
+        assert option_manager.subscription_options
         valid_user_list: set[user_types] = set(
             option_manager.subscription_options.final_choices
         )
-        scraping_subscriptions = (
-            self.datascraper.api.get_site_settings().jobs.scrape.subscriptions
-        )
+        scraping_subscriptions = site_config.jobs.scrape.subscriptions
         identifiers = []
         if performer_options:
             identifiers = performer_options.return_auto_choice()
         if not available_jobs.subscriptions:
             for authed in api.auths:
                 authed.subscriptions = []
         if available_jobs.messages:
@@ -111,21 +106,15 @@
                 user.scrape_whitelist.append("Messages")
                 for user in chat_users
                 if not await user.is_subscribed() or not scraping_subscriptions
             ]
             [valid_user_list.add(x) for x in chat_users]
 
         if available_jobs.paid_contents:
-            from ultima_scraper_api.apis.onlyfans.classes.auth_model import (
-                AuthModel as OnlyFansAuthModel,
-            )
-
             for authed in self.datascraper.api.auths:
-                if not isinstance(authed, OnlyFansAuthModel):
-                    continue
                 paid_contents = await authed.get_paid_content()
                 if not isinstance(paid_contents, error_types):
                     for paid_content in paid_contents:
                         author = paid_content.get_author()
                         if identifiers:
                             found = await author.match_identifiers(identifiers)
                             if not found:
@@ -134,14 +123,23 @@
                             performer = authed.find_user_by_identifier(
                                 identifier=author.id,
                             )
                             if performer:
                                 performer.job_whitelist.append("PaidContents")
                                 performer.scrape_whitelist.clear()
                                 valid_user_list.add(performer)
+        from ultima_scraper_api.apis.fansly.classes.user_model import (
+            create_user as FYUserModel,
+        )
+
+        for user in valid_user_list:
+            if isinstance(user, FYUserModel) and user.following:
+                user.scrape_whitelist.clear()
+                pass
+            pass
         # Need to filter out own profile with is_performer,etc
         final_valid_user_set = {
             user
             for user in valid_user_list
             if user.username not in user.get_authed().blacklist
         }
 
@@ -166,16 +164,44 @@
             match content_type:
                 case "Stories":
                     temp_master_set.extend(await self.datascraper.get_all_stories(user))
                     pass
                 case "Posts":
                     temp_master_set = await self.datascraper.get_all_posts(user)
                 case "Messages":
-                    pass
-                    unrefined_set: list[message_types | Any] = await user.get_messages()
+                    site_db = await self.server_manager.get_site_db(
+                        authed.get_api().site_name
+                    )
+                    temp_db_messages = await site_db.session.scalars(
+                        select(DBMessageModel)
+                        .where(
+                            or_(
+                                and_(
+                                    DBMessageModel.user_id == authed.id,
+                                    DBMessageModel.receiver_id == user.id,
+                                ),
+                                and_(
+                                    DBMessageModel.user_id == user.id,
+                                    DBMessageModel.receiver_id == authed.id,
+                                ),
+                            )
+                        )
+                        .order_by(DBMessageModel.id.desc())
+                    )
+                    db_messages = temp_db_messages.all()
+                    last_db_message = None
+                    cutoff_id = None
+                    if db_messages:
+                        if all(x.verified for x in db_messages):
+                            last_db_message = db_messages[0]
+                            cutoff_id = last_db_message.id
+                    unrefined_set: list[message_types | Any] = await user.get_messages(
+                        cutoff_id=cutoff_id
+                    )
+
                     mass_messages = getattr(authed, "mass_messages")
                     if user.is_me() and mass_messages:
                         mass_messages = getattr(authed, "mass_messages")
                         # Need access to a creator's account to fix this
                         # unrefined_set2 = await self.datascraper.process_mass_messages(
                         #     authed,
                         #     mass_messages,
@@ -212,20 +238,14 @@
         metadata_manager: MetadataManager,
     ):
         if not master_set:
             return False
         # if  api_type != "Posts":
         #     return
         authed = subscription.get_authed()
-        subscription_directory_manager = self.filesystem_manager.get_directory_manager(
-            subscription.id
-        )
-        formatted_metadata_directory = (
-            subscription_directory_manager.user.metadata_directory
-        )
         unrefined_set = []
         with authed.get_pool() as pool:
             print(f"Processing Scraped {api_type}")
             tasks = pool.starmap(
                 self.datascraper.media_scraper,
                 product(
                     master_set,
@@ -235,194 +255,137 @@
             )
             settings = {"colour": "MAGENTA"}
             unrefined_set: list[dict[str, Any]] = await tqdm_asyncio.gather(
                 *tasks, **settings
             )
             new_metadata = metadata_manager.merge_content_and_directories(unrefined_set)
             final_content, _final_directories = new_metadata
-            metadata_path = formatted_metadata_directory.joinpath("user_data.db")
-            metadata_manager.db_manager = DatabaseManager().get_sqlite_db(metadata_path)
             if new_metadata:
                 new_metadata_content = final_content
-                metadata_manager.content_metadatas.extend(new_metadata_content)
-                subscription.scrape_manager.set_scraped(api_type, new_metadata_content)
+                subscription.content_manager.set_content(api_type, new_metadata_content)
                 if new_metadata_content:
-                    import_status = metadata_manager.db_manager.import_metadata(
-                        new_metadata_content, api_type
-                    )
-                    if import_status:
-                        Session = metadata_manager.db_manager.session_factory
-                        if authed.api.config.settings.helpers.renamer:
-                            print(f"{subscription.username}: Renaming files.")
-                            _new_metadata_object = await renamer.start(
-                                subscription,
-                                subscription_directory_manager,
-                                api_type,
-                                Session,
-                            )
-                        pass
+                    pass
             else:
                 print(f"No {api_type} found.")
         return True
 
     # Downloads scraped content
 
     async def prepare_downloads(self, performer: user_types, api_type: str):
-        metadata_manager = self.metadata_manager_users[performer.id]
-        global_settings = performer.get_api().get_global_settings()
-        site_settings = performer.get_api().get_site_settings()
-        if not (global_settings and site_settings):
+        current_job = performer.get_current_job()
+        if not getattr(performer.content_manager.categorized, api_type):
+            current_job.done = True
             return
+        api = performer.get_api()
+        assert current_job
+        site_db = await self.server_manager.get_site_db(api.site_name, self.datascraper)
+        db_user = await site_db.get_user(performer.id)
+        assert db_user
+        await db_user.awaitable_attrs.content_manager
+        db_contents = await db_user.content_manager.get_contents(api_type)
+        final_download_set: set[ContentMetadata] = set()
+        total_media_count = 0
+        download_media_count = 0
+        for db_content in db_contents:
+            await site_db.session.refresh(db_content, ["media"])
+            # To find duplicates, we must check if media belongs to any other content type via association table
+            found_content = performer.content_manager.find_content(
+                db_content.id, api_type
+            )
+            from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
+                ContentMetadata,
+                DBContentExtractor,
+            )
+
+            if found_content:
+                found_content.__db_content__ = db_content
+                final_download_set.add(found_content)
+                download_media_count += len(found_content.medias)
+            else:
+                continue
+                await db_content.awaitable_attrs.media
+                content_metadata = ContentMetadata(db_content.id, api_type)
+                extractor = DBContentExtractor(db_content)
+                extractor.__api__ = api
+                await content_metadata.resolve_extractor(extractor)
+                content_metadata.__db_content__ = db_content
+                final_download_set.add(content_metadata)
+                total_media_count += len(db_content.media)
+            pass
+
+        global_settings = performer.get_api().get_global_settings()
         filesystem_manager = self.datascraper.filesystem_manager
         performer_directory_manager = filesystem_manager.get_directory_manager(
             performer.id
         )
         directory = performer_directory_manager.user.download_directory
-        current_job = performer.get_current_job()
-
-        metadata_path = performer_directory_manager.user.metadata_directory.joinpath(
-            "user_data.db"
+        string = "Processing Download:\n"
+        string += f"Name: {performer.username} | Type: {api_type} | Downloading: {download_media_count} | Total: {total_media_count} | Directory: {directory}\n"
+        print(string)
+        download_manager = DownloadManager(
+            performer.get_authed(),
+            filesystem_manager,
+            final_download_set,
+            global_settings.tools.reformatter.active,
         )
-        user_data_db = DatabaseManager().get_sqlite_db(metadata_path)
-        if user_data_db and user_data_db.name.exists():
-            database_session = user_data_db.session
-            db_collection = DBCollection()
-            database = db_collection.database_picker("user_data")
-            api_table = database.table_picker(api_type)
-            media_table = database.media_table
-            overwrite_files = site_settings.overwrite_files
-            final_download_set: set[ContentMetadata] = set()
-            final_media_set: set[MediaMetadata] = set()
-            total_media_count = 0
-            if database:
-                db_content_dict = {}
-                db_posts: list[ApiModel] = database_session.query(api_table)
-                for db_post in db_posts:
-                    if db_post.post_id not in db_content_dict:
-                        db_content_dict[db_post.post_id] = db_post
-                    else:
-                        raise Exception("Duplicate key in db_content_dict")
-
-                content_metadatas = metadata_manager.content_metadatas
-                for content_metadata in content_metadatas:
-                    if content_metadata.api_type == api_type:
-                        db_post = db_content_dict[content_metadata.content_id]
-                        if content_metadata.content_id == db_post.post_id:
-                            content_metadata.__db_content__ = db_post
-                            db_media_query = (
-                                database_session.query(media_table)
-                                .filter(media_table.post_id == db_post.post_id)
-                                .filter(media_table.api_type == api_type)
-                            )
-                            if overwrite_files:
-                                db_post.medias = db_media_query.all()
-                            else:
-                                db_post.medias = db_media_query.filter(
-                                    media_table.downloaded == False
-                                ).all()
-                            if db_post.medias:
-                                final_download_set.add(content_metadata)
-                                [
-                                    final_media_set.add(x.id)
-                                    for x in content_metadata.medias
-                                ]
-                                total_media_count += len(content_metadata.medias)
-                download_manager = DownloadManager(
-                    performer.get_authed(),
-                    filesystem_manager,
-                    final_download_set,
-                    global_settings.helpers.reformat_media,
-                )
-                download_count = len(final_media_set)
-                duplicate_count = total_media_count - download_count
-                string = "Processing Download:\n"
-                string += f"Name: {performer.username} | Type: {api_type} | Downloading: {download_count} | Total: {total_media_count} | Duplicates: {duplicate_count} | Directory: {directory}\n"
-                if total_media_count:
-                    print(string)
-                    _result = await download_manager.bulk_download()
-                    pass
-                while True:
-                    try:
-                        database_session.commit()
-                        break
-                    except OperationalError:
-                        database_session.rollback()
-                database_session.close()
-            current_job.done = True
+        _result = await download_manager.bulk_download()
+        await site_db.session.commit()
+        current_job.done = True
+        return
 
     async def manage_subscriptions(
         self,
         authed: auth_types,
         identifiers: list[int | str] = [],
         refresh: bool = True,
     ):
         temp_subscriptions: list[subscription_types] = []
         results = await self.datascraper.get_all_subscriptions(
             authed, identifiers, refresh
         )
         site_settings = authed.api.get_site_settings()
         if not site_settings:
             return temp_subscriptions
-        ignore_type = site_settings.ignore_type
         results.sort(key=lambda x: x.user.is_me(), reverse=True)
         for result in results:
-            # await result.create_directory_manager(user=True)
-            subscribe_price = result.get_price()
-            if ignore_type in ["paid"]:
-                if subscribe_price > 0:
-                    continue
-            if ignore_type in ["free"]:
-                if subscribe_price == 0:
-                    continue
             temp_subscriptions.append(result)
         authed.subscriptions = temp_subscriptions
         return authed.subscriptions
 
     async def account_setup(
         self,
         auth: auth_types,
-        datascraper: datascraper_types,
-        site_settings: make_settings.SiteSettings,
+        site_config: site_config_types,
         identifiers: list[int | str] | list[str] = [],
-    ) -> tuple[bool, list[user_types]]:
+    ) -> tuple[bool, list[subscription_types]]:
         status = False
         subscriptions: list[subscription_types] = []
 
-        if auth.is_authed() and site_settings:
+        if auth.is_authed() and site_config:
             authed = auth
             # metadata_filepath = (
             #     authed.directory_manager.profile.metadata_directory.joinpath(
             #         "Mass Messages.json"
             #     )
             # )
             # if authed.isPerformer:
             #     imported = main_helper.import_json(metadata_filepath)
             #     if "auth" in imported:
             #         imported = imported["auth"]
             #     mass_messages = await authed.get_mass_messages(resume=imported)
             #     if mass_messages:
             #         main_helper.export_json(mass_messages, metadata_filepath)
-            authed.blacklist = await authed.get_blacklist(
-                authed.api.get_site_settings().blacklists
-            )
-            if identifiers or site_settings.jobs.scrape.subscriptions:
+            authed.blacklist = await authed.get_blacklist(site_config.blacklists)
+            if identifiers or site_config.jobs.scrape.subscriptions:
                 subscriptions.extend(
-                    await datascraper.manage_subscriptions(
+                    await self.manage_subscriptions(
                         authed, identifiers=identifiers  # type: ignore
                     )
                 )
             status = True
-        elif (
-            auth.auth_details.email
-            and auth.auth_details.password
-            and site_settings.browser.auth
-        ):
-            # domain = "https://onlyfans.com"
-            # oflogin.login(auth, domain, auth.session_manager.get_proxy())
-            pass
         return status, subscriptions
 
     async def get_chat_users(self):
         chat_users: list[user_types] = []
         for authed in self.datascraper.api.auths:
             chats = await authed.get_chats()
             for chat in chats:
```

### Comparing `ultima_scraper_collection-1.1.3/PKG-INFO` & `ultima_scraper_collection-2.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-collection
-Version: 1.1.3
+Version: 2.0.0
 Summary: 
 Author: DIGITALCRIMINALS
 Author-email: 89371864+digitalcriminals@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: alembic (>=1.9.2,<2.0.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
+Requires-Dist: netifaces (>=0.11.0,<0.12.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: sqlalchemy (>=2.0.1,<3.0.0)
+Requires-Dist: sshtunnel (>=0.4.0,<0.5.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Requires-Dist: ultima-scraper-api (>=1.1.1,<2.0.0)
+Requires-Dist: ultima-scraper-api (>=2.0.0,<3.0.0)
+Requires-Dist: ultima-scraper-db (>=0.1.0,<0.2.0)
 Requires-Dist: ultima-scraper-renamer (>=1.1.0,<2.0.0)
```

