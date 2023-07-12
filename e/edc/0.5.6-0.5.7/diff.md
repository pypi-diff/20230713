# Comparing `tmp/edc-0.5.6.tar.gz` & `tmp/edc-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-0.5.6.tar", last modified: Wed Jul 12 18:09:21 2023, max compression
+gzip compressed data, was "edc-0.5.7.tar", last modified: Wed Jul 12 23:55:50 2023, max compression
```

## Comparing `edc-0.5.6.tar` & `edc-0.5.7.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 18:09:21.274747 edc-0.5.6/
--rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.5.6/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:49:20.000000 edc-0.5.6/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.5.6/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.5.6/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)    42627 2023-07-12 18:09:13.000000 edc-0.5.6/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.5.6/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.5.6/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)    38451 2023-07-12 18:09:21.274873 edc-0.5.6/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)    37628 2023-06-23 15:02:46.000000 edc-0.5.6/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 18:09:21.261691 edc-0.5.6/bin/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 18:09:21.264574 edc-0.5.6/bin/nginx/
--rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.5.6/bin/nginx/edc-sites.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.5.6/bin/nginx/edc-uat.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.5.6/bin/nginx/edc.conf
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 18:09:21.265268 edc-0.5.6/bin/scripts/
--rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.5.6/bin/scripts/dev_repos.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.5.6/bin/scripts/list_db_files.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.5.6/bin/scripts/restore_db_file.sh
--rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.5.6/bin/scripts/update_edc.sh
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 18:09:21.266435 edc-0.5.6/bin/systemd/
--rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.5.6/bin/systemd/celery-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.5.6/bin/systemd/celery.service
--rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.5.6/bin/systemd/celerybeat-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.5.6/bin/systemd/celerybeat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.5.6/bin/systemd/gunicorn-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.5.6/bin/systemd/gunicorn-uat.socket
--rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.5.6/bin/systemd/gunicorn.service
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.5.6/bin/systemd/gunicorn.socket
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 18:09:21.270643 edc-0.5.6/docs/
--rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.5.6/docs/Makefile
--rw-r--r--   0 erikvw     (501) staff       (20)    12969 2023-01-25 02:44:13.000000 edc-0.5.6/docs/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.5.6/docs/backup.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.5.6/docs/celery.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.5.6/docs/conda.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.5.6/docs/conf.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.5.6/docs/configure_web_services.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.5.6/docs/deploy_new_droplet.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.5.6/docs/dump_users.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.5.6/docs/exporting_encrypted_data.rst
--rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.5.6/docs/forms_reference.md
--rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.5.6/docs/index.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.5.6/docs/landing_page.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.5.6/docs/make.bat
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.5.6/docs/multisite_deployment.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.5.6/docs/prepare_database.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.5.6/docs/printing.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.5.6/docs/redis.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.5.6/docs/update_deployment.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 18:09:21.271531 edc-0.5.6/edc.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)    38451 2023-07-12 18:09:21.000000 edc-0.5.6/edc.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1508 2023-07-12 18:09:21.000000 edc-0.5.6/edc.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-12 18:09:21.000000 edc-0.5.6/edc.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.5.6/edc.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)     1916 2023-07-12 18:09:21.000000 edc-0.5.6/edc.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2023-07-12 18:09:21.000000 edc-0.5.6/edc.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 18:09:21.271662 edc-0.5.6/image/
--rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.5.6/image/icon-pycharm.png
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.5.6/pyproject.toml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 18:09:21.274206 edc-0.5.6/requirements.tests/
--rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.5.6/requirements.tests/coverage.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.5.6/requirements.tests/docs.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1053 2023-04-19 03:05:56.000000 edc-0.5.6/requirements.tests/edc.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     4100 2022-09-27 03:34:08.000000 edc-0.5.6/requirements.tests/edc_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.5.6/requirements.tests/edc_offline.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.5.6/requirements.tests/lint.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.5.6/requirements.tests/mysql.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.5.6/requirements.tests/postgres.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.5.6/requirements.tests/test_utils.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.5.6/requirements.tests/third_party_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.5.6/requirements.tests/tox.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     2959 2023-07-12 18:09:21.275241 edc-0.5.6/setup.cfg
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 18:09:21.274500 edc-0.5.6/utils/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.5.6/utils/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.5.6/utils/get_edc_requirements.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:55:50.245848 edc-0.5.7/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.5.7/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:49:20.000000 edc-0.5.7/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.5.7/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.5.7/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)    42694 2023-07-12 23:55:42.000000 edc-0.5.7/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.5.7/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.5.7/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)    38469 2023-07-12 23:55:50.245972 edc-0.5.7/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)    37646 2023-07-12 23:55:42.000000 edc-0.5.7/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:55:50.231897 edc-0.5.7/bin/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:55:50.235007 edc-0.5.7/bin/nginx/
+-rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.5.7/bin/nginx/edc-sites.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.5.7/bin/nginx/edc-uat.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.5.7/bin/nginx/edc.conf
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:55:50.235732 edc-0.5.7/bin/scripts/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.5.7/bin/scripts/dev_repos.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.5.7/bin/scripts/list_db_files.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.5.7/bin/scripts/restore_db_file.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.5.7/bin/scripts/update_edc.sh
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:55:50.237049 edc-0.5.7/bin/systemd/
+-rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.5.7/bin/systemd/celery-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.5.7/bin/systemd/celery.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.5.7/bin/systemd/celerybeat-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.5.7/bin/systemd/celerybeat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.5.7/bin/systemd/gunicorn-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.5.7/bin/systemd/gunicorn-uat.socket
+-rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.5.7/bin/systemd/gunicorn.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.5.7/bin/systemd/gunicorn.socket
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:55:50.241351 edc-0.5.7/docs/
+-rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.5.7/docs/Makefile
+-rw-r--r--   0 erikvw     (501) staff       (20)    12969 2023-01-25 02:44:13.000000 edc-0.5.7/docs/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.5.7/docs/backup.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.5.7/docs/celery.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.5.7/docs/conda.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.5.7/docs/conf.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.5.7/docs/configure_web_services.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.5.7/docs/deploy_new_droplet.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.5.7/docs/dump_users.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.5.7/docs/exporting_encrypted_data.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.5.7/docs/forms_reference.md
+-rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.5.7/docs/index.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.5.7/docs/landing_page.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.5.7/docs/make.bat
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.5.7/docs/multisite_deployment.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.5.7/docs/prepare_database.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.5.7/docs/printing.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.5.7/docs/redis.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.5.7/docs/update_deployment.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:55:50.242277 edc-0.5.7/edc.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)    38469 2023-07-12 23:55:50.000000 edc-0.5.7/edc.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1508 2023-07-12 23:55:50.000000 edc-0.5.7/edc.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-12 23:55:50.000000 edc-0.5.7/edc.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.5.7/edc.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)     1916 2023-07-12 23:55:50.000000 edc-0.5.7/edc.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2023-07-12 23:55:50.000000 edc-0.5.7/edc.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:55:50.242378 edc-0.5.7/image/
+-rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.5.7/image/icon-pycharm.png
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.5.7/pyproject.toml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:55:50.245319 edc-0.5.7/requirements.tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.5.7/requirements.tests/coverage.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.5.7/requirements.tests/docs.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1053 2023-04-19 03:05:56.000000 edc-0.5.7/requirements.tests/edc.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     4100 2022-09-27 03:34:08.000000 edc-0.5.7/requirements.tests/edc_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.5.7/requirements.tests/edc_offline.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.5.7/requirements.tests/lint.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.5.7/requirements.tests/mysql.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.5.7/requirements.tests/postgres.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.5.7/requirements.tests/test_utils.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.5.7/requirements.tests/third_party_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.5.7/requirements.tests/tox.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     2959 2023-07-12 23:55:50.246368 edc-0.5.7/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-12 23:55:50.245622 edc-0.5.7/utils/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.5.7/utils/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.5.7/utils/get_edc_requirements.py
```

### Comparing `edc-0.5.6/.gitignore` & `edc-0.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/.pre-commit-config.yaml` & `edc-0.5.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/CHANGES` & `edc-0.5.7/CHANGES`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changes
 -------
 
+0.5.7
+-----
+- change field `return_in_days` to `rx_days` (edc-rx)
+
 0.5.6
 -----
 - major refactor; eliminated use of TargetHandler classes; removed
   post processing validation checks no longer necessary with
   these fixes (edc-metadata)
 - raise addition exception if field not on source model (edc-reference)
```

### Comparing `edc-0.5.6/LICENSE` & `edc-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/PKG-INFO` & `edc-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.5.6
+Version: 0.5.7
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
@@ -32,36 +32,36 @@
 Refer to the specific open projects listed below for example EDC systems built with these modules.
 The more recent the trial the better the example.
 
 The codebase continues to evolve over many years of conducting clinical trials for mostly NIH-funded clinical trials through
 the `Harvard T Chan School of Public Health <https://aids.harvard.edu>`__, the
 `Botswana-Harvard AIDS Institute Partnership <https://aids.harvard.edu/research/bhp>`__
 in Gaborone, Botswana and the `London School of Hygiene and Tropical Medicine <https://lshtm.ac.uk>`__.
-Almost all trials were originally related to HIV/AIDS research. More recent work with the `RESPOND Africa Group <https://www.lstmed.ac.uk/RespondAfrica>`__ at both the  
+Almost all trials were originally related to HIV/AIDS research. More recent work with the `RESPOND Africa Group <https://www.lstmed.ac.uk/RespondAfrica>`__ at both the
 `Liverpool School of Tropical Medicine <https://lstm.ac.uk>`__ and the `University College London Institute for Global Health <https://www.ucl.ac.uk/global-health/>`__ has expanded into Diabetes (DM),
 Hypertension (HTN) and models of integrating care in Africa (https://inteafrica.org) for the
 three main chronic conditions -- HIV/DM/HTN.
 
 See also https://www.lstmed.ac.uk/RespondAfrica
 
 The implementations we have developed are mostly eSource systems rather than the traditional EDCs.
 
 The ``clinicedc`` for each trial consists of a subset of trial-specific modules that reference this module.
 
-(python 3.10+ and Django 4.1, see setup.cfg)
+(python 3.11, Django 4.2, MySQL 8+, see setup.cfg)
 
 
-Projects that use the EDC
--------------------------
-Recent examples of EDC's using this codebase:
+Projects that use ``clinicedc``
+-------------------------------
+Recent examples of ``clinicedc`` applications using this codebase:
 
 INTECOMM
 --------
 
-https://github.com/intecomm-trial/intecomm-edc (under-development (2022- )
+https://github.com/intecomm-trial/intecomm-edc (2022- )
 
 EFFECT
 ------
 Fluconazole plus flucytosine vs. fluconazole alone for cryptococcal antigen-positive patients identified through screening:
 
 A phase III randomised controlled trial
```

### Comparing `edc-0.5.6/README.rst` & `edc-0.5.7/edc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: edc
+Version: 0.5.7
+Summary: EDC core modules for clinicedc/edc projects.
+Home-page: https://github.com/clinicedc/edc
+Author: Erik van Widenfelt
+Author-email: ew2789@gmail.com
+License: GPL license, see LICENSE
+Keywords: django edc clinical trials research
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 4.2
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.10
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS
+
 |pypi| |downloads|
 
 clinicedc
 =========
 
 Here are a set of python modules that extend Django to empower you to build an EDC / eSource system to handle data
 collection and management for multi-site longitudinal clinical trials.
@@ -9,36 +32,36 @@
 Refer to the specific open projects listed below for example EDC systems built with these modules.
 The more recent the trial the better the example.
 
 The codebase continues to evolve over many years of conducting clinical trials for mostly NIH-funded clinical trials through
 the `Harvard T Chan School of Public Health <https://aids.harvard.edu>`__, the
 `Botswana-Harvard AIDS Institute Partnership <https://aids.harvard.edu/research/bhp>`__
 in Gaborone, Botswana and the `London School of Hygiene and Tropical Medicine <https://lshtm.ac.uk>`__.
-Almost all trials were originally related to HIV/AIDS research. More recent work with the `RESPOND Africa Group <https://www.lstmed.ac.uk/RespondAfrica>`__ at both the  
+Almost all trials were originally related to HIV/AIDS research. More recent work with the `RESPOND Africa Group <https://www.lstmed.ac.uk/RespondAfrica>`__ at both the
 `Liverpool School of Tropical Medicine <https://lstm.ac.uk>`__ and the `University College London Institute for Global Health <https://www.ucl.ac.uk/global-health/>`__ has expanded into Diabetes (DM),
 Hypertension (HTN) and models of integrating care in Africa (https://inteafrica.org) for the
 three main chronic conditions -- HIV/DM/HTN.
 
 See also https://www.lstmed.ac.uk/RespondAfrica
 
 The implementations we have developed are mostly eSource systems rather than the traditional EDCs.
 
 The ``clinicedc`` for each trial consists of a subset of trial-specific modules that reference this module.
 
-(python 3.10+ and Django 4.1, see setup.cfg)
+(python 3.11, Django 4.2, MySQL 8+, see setup.cfg)
 
 
-Projects that use the EDC
--------------------------
-Recent examples of EDC's using this codebase:
+Projects that use ``clinicedc``
+-------------------------------
+Recent examples of ``clinicedc`` applications using this codebase:
 
 INTECOMM
 --------
 
-https://github.com/intecomm-trial/intecomm-edc (under-development (2022- )
+https://github.com/intecomm-trial/intecomm-edc (2022- )
 
 EFFECT
 ------
 Fluconazole plus flucytosine vs. fluconazole alone for cryptococcal antigen-positive patients identified through screening:
 
 A phase III randomised controlled trial
```

### Comparing `edc-0.5.6/bin/nginx/edc-uat.conf` & `edc-0.5.7/bin/nginx/edc-uat.conf`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/bin/nginx/edc.conf` & `edc-0.5.7/bin/nginx/edc.conf`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/bin/scripts/dev_repos.sh` & `edc-0.5.7/bin/scripts/dev_repos.sh`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/bin/scripts/update_edc.sh` & `edc-0.5.7/bin/scripts/update_edc.sh`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/bin/systemd/celery-uat.service` & `edc-0.5.7/bin/systemd/celery-uat.service`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/bin/systemd/celery.service` & `edc-0.5.7/bin/systemd/celery.service`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/docs/Makefile` & `edc-0.5.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/docs/README.rst` & `edc-0.5.7/docs/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/docs/backup.rst` & `edc-0.5.7/docs/backup.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/docs/celery.rst` & `edc-0.5.7/docs/celery.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/docs/conda.rst` & `edc-0.5.7/docs/conda.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/docs/conf.py` & `edc-0.5.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/docs/configure_web_services.rst` & `edc-0.5.7/docs/configure_web_services.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/docs/deploy_new_droplet.rst` & `edc-0.5.7/docs/deploy_new_droplet.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/docs/exporting_encrypted_data.rst` & `edc-0.5.7/docs/exporting_encrypted_data.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/docs/forms_reference.md` & `edc-0.5.7/docs/forms_reference.md`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/docs/landing_page.rst` & `edc-0.5.7/docs/landing_page.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/docs/make.bat` & `edc-0.5.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/docs/prepare_database.rst` & `edc-0.5.7/docs/prepare_database.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/docs/printing.rst` & `edc-0.5.7/docs/printing.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/docs/update_deployment.rst` & `edc-0.5.7/docs/update_deployment.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/edc.egg-info/PKG-INFO` & `edc-0.5.7/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: edc
-Version: 0.5.6
-Summary: EDC core modules for clinicedc/edc projects.
-Home-page: https://github.com/clinicedc/edc
-Author: Erik van Widenfelt
-Author-email: ew2789@gmail.com
-License: GPL license, see LICENSE
-Keywords: django edc clinical trials research
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.2
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.10
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-License-File: AUTHORS
-
 |pypi| |downloads|
 
 clinicedc
 =========
 
 Here are a set of python modules that extend Django to empower you to build an EDC / eSource system to handle data
 collection and management for multi-site longitudinal clinical trials.
@@ -32,36 +9,36 @@
 Refer to the specific open projects listed below for example EDC systems built with these modules.
 The more recent the trial the better the example.
 
 The codebase continues to evolve over many years of conducting clinical trials for mostly NIH-funded clinical trials through
 the `Harvard T Chan School of Public Health <https://aids.harvard.edu>`__, the
 `Botswana-Harvard AIDS Institute Partnership <https://aids.harvard.edu/research/bhp>`__
 in Gaborone, Botswana and the `London School of Hygiene and Tropical Medicine <https://lshtm.ac.uk>`__.
-Almost all trials were originally related to HIV/AIDS research. More recent work with the `RESPOND Africa Group <https://www.lstmed.ac.uk/RespondAfrica>`__ at both the  
+Almost all trials were originally related to HIV/AIDS research. More recent work with the `RESPOND Africa Group <https://www.lstmed.ac.uk/RespondAfrica>`__ at both the
 `Liverpool School of Tropical Medicine <https://lstm.ac.uk>`__ and the `University College London Institute for Global Health <https://www.ucl.ac.uk/global-health/>`__ has expanded into Diabetes (DM),
 Hypertension (HTN) and models of integrating care in Africa (https://inteafrica.org) for the
 three main chronic conditions -- HIV/DM/HTN.
 
 See also https://www.lstmed.ac.uk/RespondAfrica
 
 The implementations we have developed are mostly eSource systems rather than the traditional EDCs.
 
 The ``clinicedc`` for each trial consists of a subset of trial-specific modules that reference this module.
 
-(python 3.10+ and Django 4.1, see setup.cfg)
+(python 3.11, Django 4.2, MySQL 8+, see setup.cfg)
 
 
-Projects that use the EDC
--------------------------
-Recent examples of EDC's using this codebase:
+Projects that use ``clinicedc``
+-------------------------------
+Recent examples of ``clinicedc`` applications using this codebase:
 
 INTECOMM
 --------
 
-https://github.com/intecomm-trial/intecomm-edc (under-development (2022- )
+https://github.com/intecomm-trial/intecomm-edc (2022- )
 
 EFFECT
 ------
 Fluconazole plus flucytosine vs. fluconazole alone for cryptococcal antigen-positive patients identified through screening:
 
 A phase III randomised controlled trial
```

### Comparing `edc-0.5.6/edc.egg-info/SOURCES.txt` & `edc-0.5.7/edc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/edc.egg-info/requires.txt` & `edc-0.5.7/edc.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 edc-qol==0.1.15
 edc-randomization==0.3.47
 edc-reference==0.3.20
 edc-refusal==0.1.13
 edc-registration==0.3.30
 edc-reportable==0.3.31
 edc-review-dashboard==0.3.19
-edc-rx==0.1.6
+edc-rx==0.1.7
 edc-screening==0.3.35
 edc-search==0.3.7
 edc-sites==0.3.25
 edc-subject-dashboard==0.3.38
 edc-subject-model-wrappers==0.3.15
 edc-timepoint==0.3.11
 edc-transfer==0.3.14
```

### Comparing `edc-0.5.6/image/icon-pycharm.png` & `edc-0.5.7/image/icon-pycharm.png`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/requirements.tests/edc.txt` & `edc-0.5.7/requirements.tests/edc.txt`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/requirements.tests/edc_dev.txt` & `edc-0.5.7/requirements.tests/edc_dev.txt`

 * *Files identical despite different names*

### Comparing `edc-0.5.6/setup.cfg` & `edc-0.5.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 	edc-qol==0.1.15
 	edc-randomization==0.3.47
 	edc-reference==0.3.20
 	edc-refusal==0.1.13
 	edc-registration==0.3.30
 	edc-reportable==0.3.31
 	edc-review-dashboard==0.3.19
-	edc-rx==0.1.6
+	edc-rx==0.1.7
 	edc-screening==0.3.35
 	edc-search==0.3.7
 	edc-sites==0.3.25
 	edc-subject-dashboard==0.3.38
 	edc-subject-model-wrappers==0.3.15
 	edc-timepoint==0.3.11
 	edc-transfer==0.3.14
```

### Comparing `edc-0.5.6/utils/get_edc_requirements.py` & `edc-0.5.7/utils/get_edc_requirements.py`

 * *Files identical despite different names*

