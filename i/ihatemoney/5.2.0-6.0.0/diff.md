# Comparing `tmp/ihatemoney-5.2.0.tar.gz` & `tmp/ihatemoney-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ihatemoney-5.2.0.tar", last modified: Thu Apr  7 19:30:02 2022, max compression
+gzip compressed data, was "ihatemoney-6.0.0.tar", last modified: Thu Jul 13 14:11:49 2023, max compression
```

## Comparing `ihatemoney-5.2.0.tar` & `ihatemoney-6.0.0.tar`

### file list

```diff
@@ -1,292 +1,319 @@
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.207369 ihatemoney-5.2.0/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      894 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/CONTRIBUTORS
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1781 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/LICENSE
--rw-r--r--   0 zorun     (1000) zorun     (1000)      205 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/MANIFEST.in
--rw-r--r--   0 zorun     (1000) zorun     (1000)      795 2022-04-07 19:30:02.207369 ihatemoney-5.2.0/PKG-INFO
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2014 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/README.md
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.183369 ihatemoney-5.2.0/ihatemoney/
--rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/__init__.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.183369 ihatemoney-5.2.0/ihatemoney/api/
--rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/api/__init__.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     6122 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/api/common.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.183369 ihatemoney-5.2.0/ihatemoney/api/v1/
--rw-r--r--   0 zorun     (1000) zorun     (1000)       53 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/api/v1/__init__.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1115 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/api/v1/resources.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)       97 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/babel.cfg
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.183369 ihatemoney-5.2.0/ihatemoney/conf-templates/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      641 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/conf-templates/apache-vhost.conf.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      192 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/conf-templates/gunicorn.conf.py.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2170 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/conf-templates/ihatemoney.cfg.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      752 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/conf-templates/nginx.conf.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      186 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/conf-templates/supervisord.conf.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1547 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/currency_convertor.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      745 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/default_settings.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      544 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/emails.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    15791 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/forms.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     6043 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/history.py
--rwxr-xr-x   0 zorun     (1000) zorun     (1000)     2406 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/manage.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.183369 ihatemoney-5.2.0/ihatemoney/migrations/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      790 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/migrations/alembic.ini
--rwxr-xr-x   0 zorun     (1000) zorun     (1000)     3014 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/migrations/env.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.187369 ihatemoney-5.2.0/ihatemoney/migrations/versions/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      614 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/migrations/versions/26d6a218c329_.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     8427 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/migrations/versions/2dcb0c0048dc_autologger.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      627 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/migrations/versions/6c6fb2b7f229_.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2002 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/migrations/versions/927ed575acbd_add_currencies.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      963 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/migrations/versions/a67119aa3ee5_migrate_negative_weights.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      625 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/migrations/versions/afbf27e6ef20_add_bill_import_date_field.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1085 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/migrations/versions/b78f8a8bdb16_hash_project_passwords.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2537 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/migrations/versions/b9a10d5d63ce_.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1629 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/migrations/versions/cb038f79982e_sqlite_autoincrement.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      977 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/migrations/versions/f629c8ef4ab0_initialize_all_members_weights_to_1.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    26777 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/models.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     8205 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/run.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.187369 ihatemoney-5.2.0/ihatemoney/static/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.187369 ihatemoney-5.2.0/ihatemoney/static/css/
--rw-r--r--   0 zorun     (1000) zorun     (1000)   155758 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/css/bootstrap.min.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)    14225 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/css/datatables.min.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)      298 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/css/download_mobile_app.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)     9165 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/css/main.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2185 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/css/tagsinput.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1742 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/favicon.ico
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.187369 ihatemoney-5.2.0/ihatemoney/static/fonts/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     4582 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/fonts/OFL.txt
--rw-r--r--   0 zorun     (1000) zorun     (1000)    40370 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/fonts/comfortaa-regular-webfont.eot
--rw-r--r--   0 zorun     (1000) zorun     (1000)    81869 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/fonts/comfortaa-regular-webfont.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)    20920 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/fonts/comfortaa-regular-webfont.woff
--rw-r--r--   0 zorun     (1000) zorun     (1000)      777 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/fonts/fontfaces.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)    63744 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/fonts/lobster-webfont.eot
--rw-r--r--   0 zorun     (1000) zorun     (1000)    77893 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/fonts/lobster-webfont.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)    33380 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/fonts/lobster-webfont.woff
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.191369 ihatemoney-5.2.0/ihatemoney/static/images/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      155 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/add.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)    12353 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/app-store.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)     5634 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/bill.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      518 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/book.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      890 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/cog.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      144 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/delete.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      143 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/deleter.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      167 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/edit.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)     6681 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/f-droid.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      557 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/file-alt.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1272 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/file-csv-solid.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      692 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/git.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1458 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/globe.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)    69751 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/google-play.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)     5814 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/indicate.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1304 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/legal.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      356 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/mobile-alt.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      293 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/paper-plane.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      319 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/plus.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      183 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/reactivate.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3505 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/read.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)     7325 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/share.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      259 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/show.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      158 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/sort_asc.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      146 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/sort_asc_disabled.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      199 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/sort_both.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      157 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/sort_desc.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      144 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/sort_desc_disabled.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      291 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/images/x.svg
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.191369 ihatemoney-5.2.0/ihatemoney/static/js/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    58072 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/js/bootstrap.min.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)    84649 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/js/datatables.min.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)      326 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/js/ihatemoney.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)    89501 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/js/jquery-3.6.0.min.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)    21004 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/js/popper.min.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)    10060 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/js/tagsinput.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24989 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/js/tether.min.js
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.191369 ihatemoney-5.2.0/ihatemoney/static/photoswipe/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.191369 ihatemoney-5.2.0/ihatemoney/static/photoswipe/default-skin/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    11607 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/photoswipe/default-skin/default-skin.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)      547 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/photoswipe/default-skin/default-skin.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1554 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/photoswipe/default-skin/default-skin.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      866 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/photoswipe/default-skin/preloader.gif
--rw-r--r--   0 zorun     (1000) zorun     (1000)     9878 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/photoswipe/photoswipe-ui-default.min.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)     4137 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/photoswipe/photoswipe.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)    31904 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/photoswipe/photoswipe.min.js
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.195369 ihatemoney-5.2.0/ihatemoney/static/showcase/
--rw-r--r--   0 zorun     (1000) zorun     (1000)   110452 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/showcase/1.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)    80684 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/showcase/2.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)    79206 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/showcase/3.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)    74018 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/showcase/4.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)    85550 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/showcase/5.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)   116502 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/showcase/6.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)    91376 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/showcase/7.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)    93966 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/showcase/8.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)   132986 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/static/showcase/9.webp
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.199369 ihatemoney-5.2.0/ihatemoney/templates/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      508 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/404.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      381 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/add_bill.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      266 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/add_member.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      340 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/admin.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      456 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/authenticate.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      195 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/create_project.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1650 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/dashboard.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      253 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/display_errors.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1274 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/download_mobile_app.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      384 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/edit_member.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3574 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/edit_project.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     8659 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/forms.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)    14239 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/history.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3241 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/home.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      628 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/invitation_mail.en.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      663 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/invitation_mail.fr.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)     9003 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/layout.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     7914 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/list_bills.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      298 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/password_reminder.en.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      308 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/password_reminder.fr.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      189 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/password_reminder.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      296 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/password_reminder_sent.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      240 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/recent_projects.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      458 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/reminder_mail.en.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      462 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/reminder_mail.fr.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      278 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/reset_password.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1819 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/send_invites.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      649 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/settle_bills.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3333 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/showcase.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2537 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/sidebar_table_layout.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1323 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/templates/statistics.html
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.199369 ihatemoney-5.2.0/ihatemoney/tests/
--rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/tests/__init__.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    31636 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/tests/api_test.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    59286 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/tests/budget_test.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.199369 ihatemoney-5.2.0/ihatemoney/tests/common/
--rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/tests/common/__init__.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      455 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/tests/common/help_functions.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3229 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/tests/common/ihatemoney_testcase.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24602 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/tests/history_test.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      247 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/tests/ihatemoney.cfg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      243 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/tests/ihatemoney_envvar.cfg
--rw-r--r--   0 zorun     (1000) zorun     (1000)    22461 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/tests/import_test.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    14077 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/tests/main_test.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.175369 ihatemoney-5.2.0/ihatemoney/translations/bn_BD/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.199369 ihatemoney-5.2.0/ihatemoney/translations/bn_BD/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2301 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    17660 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.175369 ihatemoney-5.2.0/ihatemoney/translations/cs/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.199369 ihatemoney-5.2.0/ihatemoney/translations/cs/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     4565 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    18391 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/de/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.199369 ihatemoney-5.2.0/ihatemoney/translations/de/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    23518 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    26145 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/el/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.199369 ihatemoney-5.2.0/ihatemoney/translations/el/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    11957 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24682 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/eo/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.203369 ihatemoney-5.2.0/ihatemoney/translations/eo/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    16894 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/eo/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    23526 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/eo/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/es/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.203369 ihatemoney-5.2.0/ihatemoney/translations/es/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     5017 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    18305 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/es_419/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.203369 ihatemoney-5.2.0/ihatemoney/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    16090 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/es_419/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24488 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/es_419/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/fa/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.203369 ihatemoney-5.2.0/ihatemoney/translations/fa/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      411 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    15365 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/fr/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.203369 ihatemoney-5.2.0/ihatemoney/translations/fr/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24073 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    32663 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/hi/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.203369 ihatemoney-5.2.0/ihatemoney/translations/hi/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24585 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/hi/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    34005 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/hi/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/id/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.203369 ihatemoney-5.2.0/ihatemoney/translations/id/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    21305 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/id/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24569 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/id/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/it/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.203369 ihatemoney-5.2.0/ihatemoney/translations/it/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    17004 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24379 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/ja/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.203369 ihatemoney-5.2.0/ihatemoney/translations/ja/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    17381 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    25107 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/kn/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.203369 ihatemoney-5.2.0/ihatemoney/translations/kn/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     6978 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/kn/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    19687 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/kn/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/ms/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.203369 ihatemoney-5.2.0/ihatemoney/translations/ms/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1784 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/ms/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    16363 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/ms/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/nb_NO/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.203369 ihatemoney-5.2.0/ihatemoney/translations/nb_NO/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    14524 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    28725 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/nl/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.203369 ihatemoney-5.2.0/ihatemoney/translations/nl/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    14078 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/nl/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    22967 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/nl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/pl/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.203369 ihatemoney-5.2.0/ihatemoney/translations/pl/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    18389 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24548 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/pt/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.207369 ihatemoney-5.2.0/ihatemoney/translations/pt/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    16149 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    23642 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/pt_BR/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.207369 ihatemoney-5.2.0/ihatemoney/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    19014 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24003 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/ru/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.207369 ihatemoney-5.2.0/ihatemoney/translations/ru/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    20310 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    29284 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/sr/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.207369 ihatemoney-5.2.0/ihatemoney/translations/sr/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3671 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/sr/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    17512 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/sr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/sv/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.207369 ihatemoney-5.2.0/ihatemoney/translations/sv/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    11708 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    21022 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/ta/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.207369 ihatemoney-5.2.0/ihatemoney/translations/ta/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     9168 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/ta/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    23154 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/ta/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/te/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.207369 ihatemoney-5.2.0/ihatemoney/translations/te/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      469 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/te/LC_MESSAGES/messages.mo
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/th/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.207369 ihatemoney-5.2.0/ihatemoney/translations/th/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     4044 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/th/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    17480 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/th/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/tr/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.207369 ihatemoney-5.2.0/ihatemoney/translations/tr/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    23495 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    25991 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/uk/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.207369 ihatemoney-5.2.0/ihatemoney/translations/uk/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     5457 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    20047 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.179369 ihatemoney-5.2.0/ihatemoney/translations/zh_Hans/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.207369 ihatemoney-5.2.0/ihatemoney/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    19376 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    23011 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.po
--rw-r--r--   0 zorun     (1000) zorun     (1000)    15376 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/utils.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3596 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/versioning.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    29273 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/web.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)       66 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney/wsgi.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2022-04-07 19:30:02.183369 ihatemoney-5.2.0/ihatemoney.egg-info/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      795 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney.egg-info/PKG-INFO
--rw-r--r--   0 zorun     (1000) zorun     (1000)     8795 2022-04-07 19:30:02.000000 ihatemoney-5.2.0/ihatemoney.egg-info/SOURCES.txt
--rw-r--r--   0 zorun     (1000) zorun     (1000)        1 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney.egg-info/dependency_links.txt
--rw-r--r--   0 zorun     (1000) zorun     (1000)      229 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney.egg-info/entry_points.txt
--rw-r--r--   0 zorun     (1000) zorun     (1000)        1 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney.egg-info/not-zip-safe
--rw-r--r--   0 zorun     (1000) zorun     (1000)      665 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney.egg-info/requires.txt
--rw-r--r--   0 zorun     (1000) zorun     (1000)       11 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/ihatemoney.egg-info/top_level.txt
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1946 2022-04-07 19:30:02.207369 ihatemoney-5.2.0/setup.cfg
--rw-r--r--   0 zorun     (1000) zorun     (1000)       38 2022-04-07 19:30:01.000000 ihatemoney-5.2.0/setup.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      945 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/CONTRIBUTORS
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1781 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/LICENSE
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      205 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/MANIFEST.in
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      847 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/PKG-INFO
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2183 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/README.md
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/__init__.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/api/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/api/__init__.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6122 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/api/common.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/api/v1/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)       53 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/api/v1/__init__.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1115 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/api/v1/resources.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)       97 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/babel.cfg
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/conf-templates/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      641 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/conf-templates/apache-vhost.conf.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      192 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/conf-templates/gunicorn.conf.py.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2170 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/conf-templates/ihatemoney.cfg.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      752 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/conf-templates/nginx.conf.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      186 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/conf-templates/supervisord.conf.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1844 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/currency_convertor.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      845 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/default_settings.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      544 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/emails.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    15851 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/forms.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6041 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/history.py
+-rwxr-xr-x   0 zorun     (1000) zorun     (1000)     2406 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/manage.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/migrations/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      790 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/alembic.ini
+-rwxr-xr-x   0 zorun     (1000) zorun     (1000)     3014 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/env.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.738748 ihatemoney-6.0.0/ihatemoney/migrations/versions/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      614 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/versions/26d6a218c329_.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     8427 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/versions/2dcb0c0048dc_autologger.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      627 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/versions/6c6fb2b7f229_.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2002 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/versions/927ed575acbd_add_currencies.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      963 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/versions/a67119aa3ee5_migrate_negative_weights.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      625 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/versions/afbf27e6ef20_add_bill_import_date_field.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1085 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/versions/b78f8a8bdb16_hash_project_passwords.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2537 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/versions/b9a10d5d63ce_.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1629 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/versions/cb038f79982e_sqlite_autoincrement.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      977 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/versions/f629c8ef4ab0_initialize_all_members_weights_to_1.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    26923 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/models.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3498 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/monkeypath_continuum.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     8632 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/run.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.738748 ihatemoney-6.0.0/ihatemoney/static/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.738748 ihatemoney-6.0.0/ihatemoney/static/css/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)   155758 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/css/bootstrap.min.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    14225 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/css/datatables.min.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      298 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/css/download_mobile_app.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     9387 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/css/main.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2185 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/css/tagsinput.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6742 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/favicon.ico
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.738748 ihatemoney-6.0.0/ihatemoney/static/fonts/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     4582 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/fonts/OFL.txt
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    40370 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/fonts/comfortaa-regular-webfont.eot
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    81869 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/fonts/comfortaa-regular-webfont.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    20920 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/fonts/comfortaa-regular-webfont.woff
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      777 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/fonts/fontfaces.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    63744 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/fonts/lobster-webfont.eot
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    77893 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/fonts/lobster-webfont.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    33380 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/fonts/lobster-webfont.woff
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.742748 ihatemoney-6.0.0/ihatemoney/static/images/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      155 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/add.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    12353 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/app-store.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     5634 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/bill.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      518 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/book.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      890 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/cog.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      144 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/delete.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      143 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/deleter.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      167 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/edit.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6681 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/f-droid.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      557 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/file-alt.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1272 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/file-csv-solid.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      692 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/git.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1458 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/globe.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    69751 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/google-play.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     5814 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/indicate.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1304 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/legal.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      356 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/mobile-alt.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      293 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/paper-plane.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      319 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/plus.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      183 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/reactivate.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3505 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/read.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     7325 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/share.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      259 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/show.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      158 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/sort_asc.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      146 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/sort_asc_disabled.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      199 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/sort_both.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      157 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/sort_desc.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      144 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/sort_desc_disabled.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      291 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/x.svg
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.742748 ihatemoney-6.0.0/ihatemoney/static/js/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    58072 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/js/bootstrap.min.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    84649 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/js/datatables.min.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      326 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/js/ihatemoney.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    89501 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/js/jquery-3.6.0.min.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    21004 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/js/popper.min.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    10060 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/js/tagsinput.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24989 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/js/tether.min.js
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.742748 ihatemoney-6.0.0/ihatemoney/static/photoswipe/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.742748 ihatemoney-6.0.0/ihatemoney/static/photoswipe/default-skin/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    11607 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/photoswipe/default-skin/default-skin.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      547 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/photoswipe/default-skin/default-skin.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1554 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/photoswipe/default-skin/default-skin.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      866 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/photoswipe/default-skin/preloader.gif
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     9878 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/photoswipe/photoswipe-ui-default.min.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     4137 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/photoswipe/photoswipe.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    31904 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/photoswipe/photoswipe.min.js
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.742748 ihatemoney-6.0.0/ihatemoney/static/showcase/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)   110452 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/showcase/1.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    80684 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/showcase/2.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    79206 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/showcase/3.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    74018 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/showcase/4.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    85550 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/showcase/5.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)   116502 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/showcase/6.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    91376 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/showcase/7.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    93966 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/showcase/8.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)   132986 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/showcase/9.webp
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/templates/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      508 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/404.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      381 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/add_bill.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      266 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/add_member.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      340 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/admin.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      456 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/authenticate.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      195 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/create_project.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2047 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/dashboard.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      253 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/display_errors.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1274 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/download_mobile_app.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      384 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/edit_member.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3183 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/edit_project.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     8805 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/forms.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      819 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/helpers.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    14239 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/history.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3242 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/home.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      628 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/invitation_mail.en.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      663 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/invitation_mail.fr.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     9363 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/layout.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     8094 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/list_bills.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      298 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/password_reminder.en.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      308 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/password_reminder.fr.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      189 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/password_reminder.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      296 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/password_reminder_sent.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      240 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/recent_projects.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      458 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/reminder_mail.en.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      462 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/reminder_mail.fr.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      278 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/reset_password.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2188 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/send_invites.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      649 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/settle_bills.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3333 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/showcase.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2537 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/sidebar_table_layout.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1323 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/statistics.html
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/tests/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/__init__.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    31635 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/api_test.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    61406 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/budget_test.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/tests/common/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/common/__init__.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      455 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/common/help_functions.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3642 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/common/ihatemoney_testcase.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24616 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/history_test.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      247 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/ihatemoney.cfg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      243 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/ihatemoney_envvar.cfg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    23512 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/import_test.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    15296 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/main_test.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/bn/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/bn/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3752 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/bn/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    16617 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/bn/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/bn_BD/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/bn_BD/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2301 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    17660 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/ca/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24065 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24506 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/cs/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     4843 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    18430 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/de/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/de/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    22234 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    26149 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/el/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/el/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    11957 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24682 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/eo/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/eo/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    16894 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/eo/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    23526 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/eo/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/es/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/es/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    10759 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    20609 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/es_419/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/es_419/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    23847 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/es_419/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    26146 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/es_419/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/fa/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     5193 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    17711 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/fr/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24071 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    32655 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/he/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/he/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    10940 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/he/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    19036 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/he/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/hi/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/hi/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24585 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/hi/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    34005 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/hi/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/hu/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6439 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    17198 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/id/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/id/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    21642 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/id/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24706 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/id/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/it/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/it/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    17631 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24667 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/ja/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    17381 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    25107 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/kn/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/kn/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6978 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/kn/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    19687 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/kn/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/ms/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/ms/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1784 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ms/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    16363 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ms/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/nb_NO/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/nb_NO/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    14524 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    28725 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/nl/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    14078 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/nl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    22967 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/nl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/pl/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    23425 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    25665 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/pt/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    22033 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    25016 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/pt_BR/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    21501 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24893 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/ru/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    27299 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    31641 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/sr/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/sr/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3671 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/sr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    17512 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/sr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/sv/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    19864 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    23702 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/ta/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/ta/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     9168 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ta/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    23154 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ta/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/te/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/te/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    11737 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/te/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    22790 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/te/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/th/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/th/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     4044 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/th/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    17480 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/th/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/tr/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    23498 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    25984 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/uk/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6939 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    20672 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/ur/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/ur/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1266 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ur/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    15034 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ur/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/vi/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/vi/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      471 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/vi/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    14545 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/vi/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/zh_Hans/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    20113 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    23264 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.po
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    14648 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/utils.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3596 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/versioning.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    30464 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/web.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)       66 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/wsgi.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney.egg-info/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      847 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney.egg-info/PKG-INFO
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     9525 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney.egg-info/SOURCES.txt
+-rw-r--r--   0 zorun     (1000) zorun     (1000)        1 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney.egg-info/dependency_links.txt
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      229 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney.egg-info/entry_points.txt
+-rw-r--r--   0 zorun     (1000) zorun     (1000)        1 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney.egg-info/not-zip-safe
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      708 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney.egg-info/requires.txt
+-rw-r--r--   0 zorun     (1000) zorun     (1000)       11 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney.egg-info/top_level.txt
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2038 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/setup.cfg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)       38 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/setup.py
```

### Comparing `ihatemoney-5.2.0/CONTRIBUTORS` & `ihatemoney-6.0.0/CONTRIBUTORS`

 * *Files 10% similar despite different names*

```diff
@@ -13,27 +13,30 @@
 Baptiste Jonglez
 Benjamin Bouvier
 Berteh
 bmatticus
 Brice Maron
 Byron Ullauri
 Carey Metcalfe
+cbrosnan
 Daniel Schreiber
 DavidRThrashJr
 donkers
 Edwin Smulders
 Elizabeth Sherrock
 eMerzh
+Erwan Lacoudre
 Feth AREZKI
 Frédéric Sureau
 Gianluca De Cola
 Glandos
 Heimen Stoffels
 James Leong
 Jocelyn Delalande
+Lod
 Luc Didry
 Lucas Verney
 Marien Fressinaud
 Mathieu Leplatre
 mcnesium
 mduret
 Mesut Akcan
@@ -42,14 +45,16 @@
 Nicolas Ferrari
 Nikos Epping
 Peter Maksymowsky
 Quentin Roy
 Rémy HUBSCHER
 Richard Coates
 Salamandar
+Saroj Regmi
 THANOS SIOURDAKIS
 Toover
 Xavier Mehrenberger
 Youe Graillot
 zorun
+Zottelchen
 
 The manual drawings are from Coline Billon, they are under CC BY 4.0.
```

### Comparing `ihatemoney-5.2.0/LICENSE` & `ihatemoney-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/PKG-INFO` & `ihatemoney-6.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ihatemoney
-Version: 5.2.0
+Version: 6.0.0
 Summary: A simple shared budget manager web application.
 Home-page: https://github.com/spiral-project/ihatemoney
 Author: Alexis Métaireau & contributors
 Author-email: alexis@notmyidea.org
 License: Custom BSD Beerware
 Description: UNKNOWN
 Keywords: web,budget
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Provides-Extra: database
 Provides-Extra: dev
 Provides-Extra: doc
```

### Comparing `ihatemoney-5.2.0/README.md` & `ihatemoney-6.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,25 +18,29 @@
 
 The code is distributed under a BSD *beerware* derivative: if you meet
 the people in person and you want to pay them a craft beer, you are
 highly encouraged to do so.
 
 ## Requirements
 
--   **Python**: version 3.6 to 3.9.
+-   **Python**: version 3.7 to 3.11.
 -   **Backends**: SQLite, PostgreSQL, MariaDB (version 10.3.2 or above),
     Memory.
 
 ## Contributing
 
 Do you wish to contribute to IHateMoney? Fantastic! There's a lot of
 very useful help on the official
 [contributing](https://ihatemoney.readthedocs.io/en/latest/contributing.html)
 page.
 
 You can also [donate some
 money](https://liberapay.com/IHateMoney/donate). All funds will be used
 to maintain the [hosted version](https://ihatemoney.org).
 
+**Join the other contributors.**
+
+[![](https://contrib.rocks/image?repo=spiral-project/ihatemoney)](https://github.com/spiral-project/ihatemoney/graphs/contributors)
+ 
 ## Translation status
 
 [![Translation status for each language](https://hosted.weblate.org/widgets/i-hate-money/-/i-hate-money/multi-blue.svg)](https://hosted.weblate.org/engage/i-hate-money/?utm_source=widget)
```

### Comparing `ihatemoney-5.2.0/ihatemoney/api/common.py` & `ihatemoney-6.0.0/ihatemoney/api/common.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/api/v1/resources.py` & `ihatemoney-6.0.0/ihatemoney/api/v1/resources.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/conf-templates/apache-vhost.conf.j2` & `ihatemoney-6.0.0/ihatemoney/conf-templates/apache-vhost.conf.j2`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/conf-templates/ihatemoney.cfg.j2` & `ihatemoney-6.0.0/ihatemoney/conf-templates/ihatemoney.cfg.j2`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/conf-templates/nginx.conf.j2` & `ihatemoney-6.0.0/ihatemoney/conf-templates/nginx.conf.j2`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/currency_convertor.py` & `ihatemoney-6.0.0/ihatemoney/currency_convertor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import traceback
+import warnings
+
 from cachetools import TTLCache, cached
 import requests
 
 
 class Singleton(type):
     _instances = {}
 
@@ -17,15 +20,22 @@
     api_url = "https://api.exchangerate.host/latest?base=USD"
 
     def __init__(self):
         pass
 
     @cached(cache=TTLCache(maxsize=1, ttl=86400))
     def get_rates(self):
-        rates = requests.get(self.api_url).json()["rates"]
+        try:
+            rates = requests.get(self.api_url).json()["rates"]
+        except Exception:
+            warnings.warn(
+                f"Call to {self.api_url} failed: {traceback.format_exc(limit=0).strip()}"
+            )
+            # In case of any exception, let's have an empty value
+            rates = {}
         rates[self.no_currency] = 1.0
         return rates
 
     def get_currencies(self, with_no_currency=True):
         rates = [
             rate
             for rate in self.get_rates()
```

### Comparing `ihatemoney-5.2.0/ihatemoney/emails.py` & `ihatemoney-6.0.0/ihatemoney/emails.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/forms.py` & `ihatemoney-6.0.0/ihatemoney/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     Optional,
     ValidationError,
 )
 
 from ihatemoney.currency_convertor import CurrencyConverter
 from ihatemoney.models import Bill, LoggingMode, Person, Project
 from ihatemoney.utils import (
+    em_surround,
     eval_arithmetic_expression,
     render_localized_currency,
     slugify,
 )
 
 
 def strip_filter(string):
@@ -249,15 +250,15 @@
 
 class ProjectFormWithCaptcha(ProjectForm):
     captcha = StringField(
         _("Which is a real currency: Euro or Petro dollar?"), default=""
     )
 
     def validate_captcha(self, field):
-        if not field.data.lower() == _("euro"):
+        if not field.data.lower() == _("euro").lower():
             message = _("Please, validate the captcha to proceed.")
             raise ValidationError(Markup(message))
 
 
 class DestructiveActionProjectForm(FlaskForm):
     """Used for any important "delete" action linked to a project:
 
@@ -290,15 +291,17 @@
 class AuthenticationForm(FlaskForm):
     id = StringField(_("Project identifier"), validators=[DataRequired()])
     password = PasswordField(_("Private code"), validators=[DataRequired()])
     submit = SubmitField(_("Get in"))
 
 
 class AdminAuthenticationForm(FlaskForm):
-    admin_password = PasswordField(_("Admin password"), validators=[DataRequired()])
+    admin_password = PasswordField(
+        _("Admin password"), validators=[DataRequired()], render_kw={"autofocus": True}
+    )
     submit = SubmitField(_("Get in"))
 
 
 class PasswordReminder(FlaskForm):
     id = StringField(_("Project identifier"), validators=[DataRequired()])
     submit = SubmitField(_("Send me the code by email"))
 
@@ -380,17 +383,15 @@
             ),
         )
 
     def set_default(self):
         self.payed_for.data = self.payed_for.default
 
     def validate_amount(self, field):
-        if field.data == "0":
-            raise ValidationError(_("Bills can't be null"))
-        elif decimal.Decimal(field.data) > decimal.MAX_EMAX:
+        if decimal.Decimal(field.data) > decimal.MAX_EMAX:
             # See https://github.com/python-babel/babel/issues/821
             raise ValidationError(f"Result is too high: {field.data}")
 
 
 class MemberForm(FlaskForm):
     name = StringField(_("Name"), validators=[DataRequired()], filters=[strip_filter])
 
@@ -435,15 +436,19 @@
 
     def validate_emails(self, field):
         for email in [email.strip() for email in self.emails.data.split(",")]:
             try:
                 email_validator.validate_email(email)
             except email_validator.EmailNotValidError:
                 raise ValidationError(
-                    _("The email %(email)s is not valid", email=email)
+                    _("The email %(email)s is not valid", email=em_surround(email))
                 )
 
 
+class LogoutForm(FlaskForm):
+    submit = SubmitField(_("Logout"))
+
+
 class EmptyForm(FlaskForm):
     """Used for CSRF validation"""
 
     pass
```

### Comparing `ihatemoney-5.2.0/ihatemoney/history.py` & `ihatemoney-6.0.0/ihatemoney/history.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
                         if (
                             "amount" in changeset
                             and "converted_amount" in changeset
                             and changeset["amount"] == changeset["converted_amount"]
                         ):
                             del changeset["converted_amount"]
 
-                    for (prop, (val_before, val_after)) in changeset.items():
+                    for prop, (val_before, val_after) in changeset.items():
                         if human_readable_names:
                             if prop == "payer_id":
                                 prop = "payer"
                                 if val_after is not None:
                                     val_after = describe_version(version.payer)
                                 if version.previous and val_before is not None:
                                     val_before = describe_version(
```

### Comparing `ihatemoney-5.2.0/ihatemoney/manage.py` & `ihatemoney-6.0.0/ihatemoney/manage.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/migrations/alembic.ini` & `ihatemoney-6.0.0/ihatemoney/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/migrations/env.py` & `ihatemoney-6.0.0/ihatemoney/migrations/env.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/migrations/versions/26d6a218c329_.py` & `ihatemoney-6.0.0/ihatemoney/migrations/versions/26d6a218c329_.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/migrations/versions/2dcb0c0048dc_autologger.py` & `ihatemoney-6.0.0/ihatemoney/migrations/versions/2dcb0c0048dc_autologger.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/migrations/versions/6c6fb2b7f229_.py` & `ihatemoney-6.0.0/ihatemoney/migrations/versions/6c6fb2b7f229_.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/migrations/versions/927ed575acbd_add_currencies.py` & `ihatemoney-6.0.0/ihatemoney/migrations/versions/927ed575acbd_add_currencies.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/migrations/versions/a67119aa3ee5_migrate_negative_weights.py` & `ihatemoney-6.0.0/ihatemoney/migrations/versions/a67119aa3ee5_migrate_negative_weights.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/migrations/versions/afbf27e6ef20_add_bill_import_date_field.py` & `ihatemoney-6.0.0/ihatemoney/migrations/versions/afbf27e6ef20_add_bill_import_date_field.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/migrations/versions/b78f8a8bdb16_hash_project_passwords.py` & `ihatemoney-6.0.0/ihatemoney/migrations/versions/b78f8a8bdb16_hash_project_passwords.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/migrations/versions/b9a10d5d63ce_.py` & `ihatemoney-6.0.0/ihatemoney/migrations/versions/b9a10d5d63ce_.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/migrations/versions/cb038f79982e_sqlite_autoincrement.py` & `ihatemoney-6.0.0/ihatemoney/migrations/versions/cb038f79982e_sqlite_autoincrement.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/migrations/versions/f629c8ef4ab0_initialize_all_members_weights_to_1.py` & `ihatemoney-6.0.0/ihatemoney/migrations/versions/f629c8ef4ab0_initialize_all_members_weights_to_1.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/models.py` & `ihatemoney-6.0.0/ihatemoney/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,31 @@
 from sqlalchemy import orm
 from sqlalchemy.sql import func
 from sqlalchemy_continuum import make_versioned, version_class
 from sqlalchemy_continuum.plugins import FlaskPlugin
 from werkzeug.security import generate_password_hash
 
 from ihatemoney.currency_convertor import CurrencyConverter
+from ihatemoney.monkeypath_continuum import PatchedTransactionFactory
 from ihatemoney.utils import get_members, same_bill
 from ihatemoney.versioning import (
     ConditionalVersioningManager,
     LoggingMode,
     get_ip_if_allowed,
     version_privacy_predicate,
 )
 
 make_versioned(
     user_cls=None,
     manager=ConditionalVersioningManager(
         # Conditionally Disable the versioning based on each
         # project's privacy preferences
         tracking_predicate=version_privacy_predicate,
+        # MonkeyPatching
+        transaction_cls=PatchedTransactionFactory(),
     ),
     plugins=[
         FlaskPlugin(
             # Redirect to our own function, which respects user preferences
             # on IP address collection
             remote_addr_factory=get_ip_if_allowed,
             # Suppress the plugin's attempt to grab a user id,
@@ -533,15 +536,15 @@
         db.session.commit()
 
         operations = (
             ("Georg", 200, ("Amina", "Georg", "Alice"), "Food shopping"),
             ("Alice", 20, ("Amina", "Alice"), "Beer !"),
             ("Amina", 50, ("Amina", "Alice", "Georg"), "AMAP"),
         )
-        for (payer, amount, owers, what) in operations:
+        for payer, amount, owers, what in operations:
             db.session.add(
                 Bill(
                     amount=amount,
                     original_currency=project.default_currency,
                     owers=[members[name] for name in owers],
                     payer_id=members[payer].id,
                     project_default_currency=project.default_currency,
```

### Comparing `ihatemoney-5.2.0/ihatemoney/run.py` & `ihatemoney-6.0.0/ihatemoney/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime
 import os
 import os.path
 import warnings
 
 from babel.dates import LOCALTZ
 from flask import Flask, g, render_template, request, session
 from flask_babel import Babel, format_currency
@@ -17,14 +18,15 @@
 from ihatemoney.api.v1 import api as apiv1
 from ihatemoney.currency_convertor import CurrencyConverter
 from ihatemoney.models import db
 from ihatemoney.utils import (
     IhmJSONEncoder,
     PrefixedWSGI,
     em_surround,
+    limiter,
     locale_from_iso,
     localize_list,
     minimal_round,
     static_include,
 )
 from ihatemoney.web import main as web_interface
 
@@ -80,15 +82,14 @@
     else:
         app.config.from_pyfile("ihatemoney.cfg", silent=True)
     # Configure custom JSONEncoder used by the API
     app.config["RESTFUL_JSON"] = {"cls": IhmJSONEncoder}
 
 
 def validate_configuration(app):
-
     if app.config["SECRET_KEY"] == default_settings.SECRET_KEY:
         warnings.warn(
             "Running a server without changing the SECRET_KEY can lead to"
             + " user impersonation. Please update your configuration file.",
             UserWarning,
         )
     # Deprecations
@@ -140,14 +141,16 @@
     # If we need to load external JS/CSS/image resources, it needs to be added here, see
     # https://github.com/wntrblm/flask-talisman#content-security-policy
     csp = {
         "default-src": ["'self'"],
         # We have several inline javascript scripts :(
         "script-src": ["'self'", "'unsafe-inline'"],
         "object-src": "'none'",
+        "img-src": ["'self'", "data:"],
+        "style-src": ["'self'", "'unsafe-inline'"],
     }
 
     Talisman(
         app,
         # Forcing HTTPS is the job of a reverse proxy
         force_https=False,
         # This is handled separately through the SESSION_COOKIE_SECURE Flask setting
@@ -164,14 +167,15 @@
     # with a forged X-FORWARDED-FOR header
     app.wsgi_app = ProxyFix(app.wsgi_app)
 
     validate_configuration(app)
     app.register_blueprint(web_interface)
     app.register_blueprint(apiv1)
     app.register_error_handler(404, page_not_found)
+    limiter.init_app(app)
 
     # Configure the a, root="main"pplication
     setup_database(app)
 
     # Setup Currency Cache
     CurrencyConverter()
 
@@ -181,27 +185,44 @@
 
     # Jinja filters
     app.jinja_env.globals["static_include"] = static_include
     app.jinja_env.globals["locale_from_iso"] = locale_from_iso
     app.jinja_env.filters["minimal_round"] = minimal_round
     app.jinja_env.filters["em_surround"] = lambda text: Markup(em_surround(text))
     app.jinja_env.filters["localize_list"] = localize_list
+    app.jinja_env.filters["from_timestamp"] = datetime.fromtimestamp
 
     # Translations and time zone (used to display dates).  The timezone is
     # taken from the BABEL_DEFAULT_TIMEZONE settings, and falls back to
     # the local timezone of the server OS by using LOCALTZ.
 
     # On some bare systems, LOCALTZ is a fake object unusable by Flask-Babel, so use UTC instead
     default_timezone = "UTC"
     try:
         pytz.timezone(str(LOCALTZ))
         default_timezone = str(LOCALTZ)
     except pytz.exceptions.UnknownTimeZoneError:
         pass
-    babel = Babel(app, default_timezone=default_timezone)
+
+    def get_locale():
+        # get the lang from the session if defined, fallback on the browser "accept
+        # languages" header.
+        lang = session.get(
+            "lang",
+            request.accept_languages.best_match(app.config["SUPPORTED_LANGUAGES"]),
+        )
+        setattr(g, "lang", lang)
+        return lang
+
+    if hasattr(Babel, "localeselector"):
+        # Compatibility for flask-babel <= 2
+        babel = Babel(app, default_timezone=default_timezone)
+        babel.localeselector(get_locale)
+    else:
+        Babel(app, default_timezone=default_timezone, locale_selector=get_locale)
 
     # Undocumented currencyformat filter from flask_babel is forwarding to Babel format_currency
     # We overwrite it to remove the currency sign ¤ when there is no currency
     @pass_context
     def currency(context, number, currency=None, *args, **kwargs):
         if currency is None:
             currency = context.get("g").project.default_currency
@@ -214,25 +235,14 @@
             currency if currency != CurrencyConverter.no_currency else "",
             *args,
             **kwargs,
         ).strip()
 
     app.jinja_env.filters["currency"] = currency
 
-    @babel.localeselector
-    def get_locale():
-        # get the lang from the session if defined, fallback on the browser "accept
-        # languages" header.
-        lang = session.get(
-            "lang",
-            request.accept_languages.best_match(app.config["SUPPORTED_LANGUAGES"]),
-        )
-        setattr(g, "lang", lang)
-        return lang
-
     return app
 
 
 def main():
     app = create_app()
     app.run(host="0.0.0.0", debug=True)
```

### Comparing `ihatemoney-5.2.0/ihatemoney/static/css/bootstrap.min.css` & `ihatemoney-6.0.0/ihatemoney/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/css/datatables.min.css` & `ihatemoney-6.0.0/ihatemoney/static/css/datatables.min.css`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/css/main.css` & `ihatemoney-6.0.0/ihatemoney/static/css/main.css`

 * *Files 15% similar despite different names*

```diff
@@ -10,26 +10,30 @@
 }
 
 /* Navbar */
 
 .navbar-brand span {
   color: #abe128;
 }
+
 .navbar h1 {
   font-size: 1rem;
   margin: 0;
   padding: 0;
 }
+
 .navbar .secondary-nav {
   text-align: right;
   flex-direction: row-reverse;
 }
+
 .secondary-nav .nav-link {
   padding: 0.5rem 1rem;
 }
+
 .navbar-brand {
   font-family: "Lobster", arial, serif;
   font-size: 1.5rem;
 }
 
 @media (min-width: 992px) {
   .projects-item {
@@ -47,23 +51,25 @@
   font-family: "Comfortaa", arial, serif;
   margin-top: 1em;
   margin-bottom: 0.5em;
   color: #000;
   font-size: 2.4em;
 }
 
-#header .tryout, #header .showcase {
+#header .tryout,
+#header .showcase {
   color: #fff;
   background-color: #414141;
   border-color: #414141;
   margin-left: 3px;
   margin-right: 3px;
 }
 
-#header .tryout:hover, #header .showcase:hover {
+#header .tryout:hover,
+#header .showcase:hover {
   background-color: #606060;
   border-color: #606060;
   cursor: pointer;
 }
 
 #header .showcaseimg {
   width: 55px;
@@ -87,17 +93,19 @@
 }
 
 /* Sidebar */
 
 .balance tr td {
   font-weight: bold;
 }
+
 .positive {
   color: green;
 }
+
 .negative {
   color: red;
 }
 
 .sidebar {
   background-color: #abe128;
   background-position: center bottom;
@@ -109,14 +117,15 @@
   flex-direction: column;
 }
 
 .sidebar_content {
   flex: 1 1 auto;
   overflow-y: auto;
 }
+
 .identifier {
   margin-bottom: 15px;
 }
 
 @media (min-width: 768px) {
   .sidebar {
     position: fixed;
@@ -139,45 +148,50 @@
   margin-top: 1rem;
 }
 
 /* Home */
 .home-container {
   background: linear-gradient(150deg, #abe128 0%, #43ca61 100%);
 }
+
 .home {
   padding-top: 1em;
   padding-bottom: 3em;
 }
+
 #authentication-form legend {
   text-align: right;
 }
 
 .home .card {
   min-width: 25em;
   border: 0;
   border-radius: 0;
   box-shadow: 0px 0px 10px rgba(83, 88, 93, 0.4);
   margin-right: 25px;
   margin-bottom: 20px;
   margin-left: 25px;
 }
+
 @media (max-width: 450px) {
   .home .card {
     min-width: unset;
   }
 }
+
 /* Other */
 
 #bills {
   color: black;
 }
 
 .empty-bill {
   margin-top: 5rem !important;
 }
+
 .empty-bill .card {
   border: 0;
 }
 
 .empty-bill .billimg svg {
   fill: lightgray;
   height: 6em;
@@ -246,32 +260,36 @@
   text-align: center;
   line-height: 35px;
 
   margin-left: 3px;
   border-radius: 50%;
   opacity: 0.5;
 }
+
 @-moz-document url-prefix() {
+
   /** Firefox style fix **/
   footer .footer-right a {
     padding-top: 2px;
   }
 }
+
 footer .footer-right a:hover {
   opacity: 1;
 }
 
 footer .footer-left {
   padding-top: 6px;
   line-height: 35px;
 }
 
 /* If you don't want the footer to be responsive, remove these media queries */
 
 @media (max-width: 600px) {
+
   footer .footer-left,
   footer .footer-right {
     text-align: center;
   }
 
   footer .footer-right {
     float: none;
@@ -287,38 +305,48 @@
 .btn-primary[data-toggle="modal"] {
   color: #fff;
 }
 
 .bill-actions {
   padding-top: 10px;
   text-align: center;
+  column-gap: 8px;
+  min-height: 56px;
+
+  /* To be able to set absolute element positionning for confirm deletion */
+  position: relative;
 }
 
-.bill-actions > form > .delete,
-.bill-actions > .edit,
-.bill-actions > .show {
+.bill-actions>form>.delete,
+.bill-actions>.edit,
+.bill-actions>.show {
   font-size: 0px;
   display: block;
   width: 16px;
   height: 16px;
-  margin: 2px;
-  margin-left: 5px;
-  float: left;
   border: none;
 }
 
-.bill-actions > form > .delete {
+.bill-actions .confirm {
+  position: absolute;
+  top: 4px;
+  left: 4px;
+  width: calc(100% - 8px);
+  height: calc(100% - 8px);
+}
+
+.bill-actions>form>.delete {
   background: url("../images/delete.png") no-repeat right;
 }
 
-.bill-actions > .edit {
+.bill-actions>.edit {
   background: url("../images/edit.png") no-repeat right;
 }
 
-.bill-actions > .show {
+.bill-actions>.show {
   background: url("../images/show.png") no-repeat right;
 }
 
 #bill_table,
 #monthly_stats,
 #history_table {
   margin-top: 30px;
@@ -330,67 +358,69 @@
   position: sticky;
   top: 4em;
   z-index: 1;
   background-color: rgba(255, 255, 255, 0.75);
 }
 
 @media (min-width: 768px) {
+
   .split_bills,
   #table_overflow.statistics {
     /* The table is shifted to left, so add the spacer width on the right to match */
     width: calc(100% + 15px);
   }
 }
 
-.project-actions > .delete,
-.project-actions > .edit,
-.project-actions > .show {
+.project-actions>form>.delete,
+.project-actions>.edit,
+.project-actions>.show {
   font-size: 0px;
   display: block;
   width: 16px;
   height: 16px;
   margin: 2px;
   margin-left: 5px;
   float: left;
 }
 
-.project-actions > .delete {
+.project-actions>form>.delete {
   background: url("../images/delete.png") no-repeat right;
+  border: 0px !important;
 }
 
-.project-actions > .edit {
+.project-actions>.edit {
   background: url("../images/edit.png") no-repeat right;
 }
 
-.project-actions > .show {
+.project-actions>.show {
   background: url("../images/show.png") no-repeat right;
 }
 
-.history_icon > .delete,
-.history_icon > .add,
-.history_icon > .edit {
+.history_icon>.delete,
+.history_icon>.add,
+.history_icon>.edit {
   font-size: 0px;
   display: block;
   width: 16px;
   height: 16px;
   margin: 2px;
   margin-right: 10px;
   margin-top: 3px;
   float: left;
 }
 
-.history_icon > .delete {
+.history_icon>.delete {
   background: url("../images/delete.png") no-repeat right;
 }
 
-.history_icon > .edit {
+.history_icon>.edit {
   background: url("../images/edit.png") no-repeat right;
 }
 
-.history_icon > .add {
+.history_icon>.add {
   background: url("../images/add.png") no-repeat right;
 }
 
 .history_text {
   display: table-cell;
 }
 
@@ -447,15 +477,15 @@
 }
 
 .balance.table {
   table-layout: fixed;
   margin-top: 30px;
 }
 
-#bill-form > fieldset {
+#bill-form>fieldset {
   margin-top: 10px;
 }
 
 .flash {
   z-index: 1031;
 }
 
@@ -471,72 +501,89 @@
 .balance.table tr:hover .action,
 tr:hover .extra-info {
   visibility: visible;
 }
 
 /* Fluid Offsets for Boostrap */
 
-.row-fluid > [class*="span"]:not([class*="offset"]):first-child {
+.row-fluid>[class*="span"]:not([class*="offset"]):first-child {
   margin-left: 0;
 }
-.row-fluid > .offset12 {
+
+.row-fluid>.offset12 {
   margin-left: 100%;
 }
-.row-fluid > .offset11 {
+
+.row-fluid>.offset11 {
   margin-left: 93.5%;
 }
-.row-fluid > .offset10 {
+
+.row-fluid>.offset10 {
   margin-left: 85%;
 }
-.row-fluid > .offset9 {
+
+.row-fluid>.offset9 {
   margin-left: 76.5%;
 }
-.row-fluid > .offset8 {
+
+.row-fluid>.offset8 {
   margin-left: 68%;
 }
-.row-fluid > .offset7 {
+
+.row-fluid>.offset7 {
   margin-left: 59.5%;
 }
-.row-fluid > .offset6 {
+
+.row-fluid>.offset6 {
   margin-left: 51%;
 }
-.row-fluid > .offset5 {
+
+.row-fluid>.offset5 {
   margin-left: 42.5%;
 }
-.row-fluid > .offset4 {
+
+.row-fluid>.offset4 {
   margin-left: 34%;
 }
-.row-fluid > .offset3 {
+
+.row-fluid>.offset3 {
   margin-left: 25.5%;
 }
-.row-fluid > .offset2 {
+
+.row-fluid>.offset2 {
   margin-left: 17%;
 }
-.row-fluid > .offset1 {
+
+.row-fluid>.offset1 {
   margin-left: 8.5%;
 }
 
 .globe-europe svg {
   fill: rgba(255, 255, 255, 0.5);
 }
+
 .navbar-nav .dropdown-toggle:hover .globe-europe svg {
   fill: rgba(255, 255, 255, 0.75);
 }
-.navbar-dark .navbar-nav .show > .nav-link svg {
+
+.navbar-dark .navbar-nav .show>.nav-link svg {
   fill: white;
 }
+
 .navbar-dark .dropdown-menu {
   max-height: 50vh;
   overflow-y: auto;
 }
+
 .icon svg {
   display: inline-block;
   border-bottom: 0.2em solid transparent;
   height: 1.2em;
-  width: 1.2em; /* protection for IE11 */
+  width: 1.2em;
+  /* protection for IE11 */
 }
 
 .icon.high svg {
   height: 2em;
   margin-top: -0.2em;
   margin-bottom: -0.2em;
 }
@@ -544,25 +591,28 @@
 .download-project .icon svg {
   fill: white;
 }
 
 .icon.before-text svg {
   margin-right: 3px;
 }
+
 footer .icon svg {
   fill: white;
 }
+
 .icon.icon-white {
   fill: white;
 }
 
 .icon.icon-red {
   fill: #dc3545;
 }
-.btn:hover .icon.icon-red  {
+
+.btn:hover .icon.icon-red {
   fill: white !important;
 }
 
 /* align the first column */
 #monthly_stats tr *:first-child {
   text-align: right;
   width: 200px;
@@ -578,10 +628,11 @@
 
 /* edit settings */
 
 .edit-project form {
   margin-top: 1em;
   margin-bottom: 3em;
 }
+
 .edit-project .custom-file {
   margin-bottom: 2em;
-}
+}
```

### Comparing `ihatemoney-5.2.0/ihatemoney/static/css/tagsinput.css` & `ihatemoney-6.0.0/ihatemoney/static/css/tagsinput.css`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/fonts/OFL.txt` & `ihatemoney-6.0.0/ihatemoney/static/fonts/OFL.txt`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/fonts/comfortaa-regular-webfont.eot` & `ihatemoney-6.0.0/ihatemoney/static/fonts/comfortaa-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/fonts/comfortaa-regular-webfont.svg` & `ihatemoney-6.0.0/ihatemoney/static/fonts/comfortaa-regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/fonts/comfortaa-regular-webfont.woff` & `ihatemoney-6.0.0/ihatemoney/static/fonts/comfortaa-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/fonts/fontfaces.css` & `ihatemoney-6.0.0/ihatemoney/static/fonts/fontfaces.css`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/fonts/lobster-webfont.eot` & `ihatemoney-6.0.0/ihatemoney/static/fonts/lobster-webfont.eot`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/fonts/lobster-webfont.svg` & `ihatemoney-6.0.0/ihatemoney/static/fonts/lobster-webfont.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/fonts/lobster-webfont.woff` & `ihatemoney-6.0.0/ihatemoney/static/fonts/lobster-webfont.woff`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/images/app-store.svg` & `ihatemoney-6.0.0/ihatemoney/static/images/app-store.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/images/bill.svg` & `ihatemoney-6.0.0/ihatemoney/static/images/bill.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/images/book.svg` & `ihatemoney-6.0.0/ihatemoney/static/images/book.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/images/cog.svg` & `ihatemoney-6.0.0/ihatemoney/static/images/cog.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/images/f-droid.svg` & `ihatemoney-6.0.0/ihatemoney/static/images/f-droid.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/images/file-alt.svg` & `ihatemoney-6.0.0/ihatemoney/static/images/file-alt.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/images/file-csv-solid.svg` & `ihatemoney-6.0.0/ihatemoney/static/images/file-csv-solid.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/images/git.svg` & `ihatemoney-6.0.0/ihatemoney/static/images/git.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/images/globe.svg` & `ihatemoney-6.0.0/ihatemoney/static/images/globe.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/images/google-play.png` & `ihatemoney-6.0.0/ihatemoney/static/images/google-play.png`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/images/indicate.svg` & `ihatemoney-6.0.0/ihatemoney/static/images/indicate.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/images/legal.svg` & `ihatemoney-6.0.0/ihatemoney/static/images/legal.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/images/read.svg` & `ihatemoney-6.0.0/ihatemoney/static/images/read.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/images/share.svg` & `ihatemoney-6.0.0/ihatemoney/static/images/share.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/js/bootstrap.min.js` & `ihatemoney-6.0.0/ihatemoney/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/js/datatables.min.js` & `ihatemoney-6.0.0/ihatemoney/static/js/datatables.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/js/jquery-3.6.0.min.js` & `ihatemoney-6.0.0/ihatemoney/static/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/js/popper.min.js` & `ihatemoney-6.0.0/ihatemoney/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/js/tagsinput.js` & `ihatemoney-6.0.0/ihatemoney/static/js/tagsinput.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/js/tether.min.js` & `ihatemoney-6.0.0/ihatemoney/static/js/tether.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/photoswipe/default-skin/default-skin.css` & `ihatemoney-6.0.0/ihatemoney/static/photoswipe/default-skin/default-skin.css`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/photoswipe/default-skin/default-skin.png` & `ihatemoney-6.0.0/ihatemoney/static/photoswipe/default-skin/default-skin.png`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/photoswipe/default-skin/default-skin.svg` & `ihatemoney-6.0.0/ihatemoney/static/photoswipe/default-skin/default-skin.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/photoswipe/default-skin/preloader.gif` & `ihatemoney-6.0.0/ihatemoney/static/photoswipe/default-skin/preloader.gif`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/photoswipe/photoswipe-ui-default.min.js` & `ihatemoney-6.0.0/ihatemoney/static/photoswipe/photoswipe-ui-default.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/photoswipe/photoswipe.css` & `ihatemoney-6.0.0/ihatemoney/static/photoswipe/photoswipe.css`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/photoswipe/photoswipe.min.js` & `ihatemoney-6.0.0/ihatemoney/static/photoswipe/photoswipe.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/showcase/1.webp` & `ihatemoney-6.0.0/ihatemoney/static/showcase/1.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/showcase/2.webp` & `ihatemoney-6.0.0/ihatemoney/static/showcase/2.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/showcase/3.webp` & `ihatemoney-6.0.0/ihatemoney/static/showcase/3.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/showcase/4.webp` & `ihatemoney-6.0.0/ihatemoney/static/showcase/4.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/showcase/5.webp` & `ihatemoney-6.0.0/ihatemoney/static/showcase/5.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/showcase/6.webp` & `ihatemoney-6.0.0/ihatemoney/static/showcase/6.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/showcase/7.webp` & `ihatemoney-6.0.0/ihatemoney/static/showcase/7.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/showcase/8.webp` & `ihatemoney-6.0.0/ihatemoney/static/showcase/8.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/static/showcase/9.webp` & `ihatemoney-6.0.0/ihatemoney/static/showcase/9.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/templates/dashboard.html` & `ihatemoney-6.0.0/ihatemoney/templates/dashboard.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,54 @@
 {% extends "layout.html" %}
 {% block content %}
 {% if is_admin_dashboard_activated %}
 <table id="bill_table" class="table table-striped">
-    <thead><tr><th>{{ _("Project") }}</th><th>{{ _("Number of participants") }}</th><th>{{ _("Number of bills") }}</th><th>{{_("Newest bill")}}</th><th>{{_("Oldest bill")}}</th><th>{{_("Actions")}}</th></tr></thead>
+    <thead>
+        <tr>
+            <th>{{ _("Project") }}</th>
+            <th>{{ _("Number of participants") }}</th>
+            <th>{{ _("Number of bills") }}</th>
+            <th>{{_("Newest bill")}}</th>
+            <th>{{_("Oldest bill")}}</th>
+            <th>{{_("Actions")}}</th>
+        </tr>
+    </thead>
     <tbody>{% for project in projects|sort(attribute='name') %}
         <tr>
-        <td><a href="{{ url_for(".list_bills", project_id=project.id) }}" title="{{ project.name }}">{{ project.name }}</a></td><td>{{ project.members | count }}</td><td>{{ project.get_bills_unordered().count() }}</td>
-        {% if project.has_bills() %}
-        <td>{{ project.get_bills().all()[0].date }}</td>
-        <td>{{ project.get_bills().all()[-1].date }}</td>
-        {% else %}
-        <td></td>
-        <td></td>
-        {% endif %}
-        <td class="project-actions">
-            <a class="edit" href="{{ url_for(".edit_project", project_id=project.id) }}" title="{{ _("edit") }}">{{ _('edit') }}</a>
-            <a class="delete" href="{{ url_for(".delete_project", project_id=project.id) }}" title="{{ _("delete") }}">{{ _('delete') }}</a>
-            <a class="show" href="{{ url_for(".list_bills", project_id=project.id) }}" title="{{ _("show") }}">{{ _('show') }}</a>
-        </td>
+            <td><a href="{{ url_for('.list_bills', project_id=project.id) }}"
+                    title="{{ project.name }}">{{project.name}}</a></td>
+            <td>{{ project.members | count }}</td>
+            <td>{{ project.get_bills_unordered().count() }}</td>
+            {% if project.has_bills() %}
+            <td>{{ project.get_bills().all()[0].date }}</td>
+            <td>{{ project.get_bills().all()[-1].date }}</td>
+            {% else %}
+            <td></td>
+            <td></td>
+            {% endif %}
+            <td class="project-actions">
+                <a class="edit" href="{{ url_for('.edit_project', project_id=project.id) }}" title=" {{ _('edit')}}">{{
+                    _('edit') }}</a>
+
+                <form id="delete-project" class="form-horizontal" action="{{ url_for('.dashboard_delete_project',
+                    project_id=project.id) }}" method="post">
+
+                    <button class="delete">{{ _("Delete project") }}</button>
+                </form>
+                <a class="show" href="{{ url_for('.list_bills', project_id=project.id) }}" title="{{ _(" show") }}">{{
+                    _('show') }}</a>
+            </td>
         </tr>
-    {% endfor %}
+        {% endfor %}
     </tbody>
 </table>
 <script language="JavaScript">
-$(document).ready(function() {
-    $('#bill_table').DataTable({
-        paging: true
-    });
-})
+    $(document).ready(function () {
+        $('#bill_table').DataTable({
+            paging: true
+        });
+    })
 </script>
 {% else %}
 <div class="alert alert-danger">{{ _("The Dashboard is currently deactivated.") }}</div>
 {% endif %}
-{% endblock %}
+{% endblock %}
```

### Comparing `ihatemoney-5.2.0/ihatemoney/templates/download_mobile_app.html` & `ihatemoney-6.0.0/ihatemoney/templates/download_mobile_app.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/templates/forms.html` & `ihatemoney-6.0.0/ihatemoney/templates/forms.html`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,19 @@
             {{ input(form.original_currency, inline=True, class="form-control custom-select") }}
         {% endif %}
         {{ input(form.external_link, inline=True) }}
     </details>
     </fieldset>
     <div class="actions">
         {{ form.submit(class="btn btn-primary") }}
-        {% if not edit %} {{ form.submit2(class="btn btn-light") }}{% endif %}
+        {% if edit %} 
+            <a href="{{ url_for(".list_bills") }}" class="btn btn-outline-secondary"> {{_("Cancel") }} </a>
+        {% else %} 
+            {{ form.submit2(class="btn btn-light") }}
+        {% endif %}
     </div>
 
 {% endmacro %}
 
 {% macro add_member(form) %}
 {{ form.hidden_tag() }}
     {% include "display_errors.html" %}
```

#### html2text {}

```diff
@@ -60,16 +60,17 @@
 (attribute='1') %}
  % if checked %}checked{% endif %} class="form-check-input" value="{{key}}"
 id="payed_for-{{key}}"/> {{value}}
 {% endfor %}
  {{ _("More options") }} {% if g.project.default_currency != "XXX" %} {{ input
 (form.original_currency, inline=True, class="form-control custom-select") }} {%
 endif %} {{ input(form.external_link, inline=True) }}
-{{ form.submit(class="btn btn-primary") }} {% if not edit %} {{ form.submit2
-(class="btn btn-light") }}{% endif %}
+{{ form.submit(class="btn btn-primary") }} {% if edit %}
+list_bills") }}" class="btn btn-outline-secondary"> {{_("Cancel") }}
+ {% else %} {{ form.submit2(class="btn btn-light") }} {% endif %}
 {% endmacro %} {% macro add_member(form) %} {{ form.hidden_tag() }} {% include
 "display_errors.html" %}
 _("Add participant") {{ form.name(placeholder=_("Add participant"),
 class="form-control") }}
 {{ _("Add") }}
 {% endmacro %} {% macro edit_member(form, title=True) %}  {% if title %}{{ _
 ("Edit this participant") }}{% endif %} {% include "display_errors.html" %} {
```

### Comparing `ihatemoney-5.2.0/ihatemoney/templates/history.html` & `ihatemoney-6.0.0/ihatemoney/templates/history.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/templates/home.html` & `ihatemoney-6.0.0/ihatemoney/templates/home.html`

 * *Files 2% similar despite different names*

```diff
@@ -89,12 +89,12 @@
       </div>
     </div>
   </div>
 </main>
 {% endblock %}
 {% block js %}
 $('#creation-form #password').tooltip({
-    title: '{{ _("Don\\'t reuse a personal password. Choose a private code and send it to your friends")}}',
+    title: "{{ _("Don\\'t reuse a personal password. Choose a private code and send it to your friends") }}",
     trigger: 'focus',
     placement: 'right'
 });
 {% endblock %}
```

#### html2text {}

```diff
@@ -15,10 +15,10 @@
   {{ forms.authenticate(auth_form, home=True) }}
  {{ _("Log in") }}  {{__("can't_remember_your_password?")_}}
 {{ _("Create a new project") }}
 {% if is_public_project_creation_allowed %}
  {{ forms.create_project(project_form, home=True) }}
  {{ _("Create") }}
 {% else %} {{__("Create_a_new_project")_}} {% endif %}
- {% endblock %} {% block js %} $('#creation-form #password').tooltip({ title: '
+ {% endblock %} {% block js %} $('#creation-form #password').tooltip({ title: "
 {{ _("Don\\'t reuse a personal password. Choose a private code and send it to
-your friends")}}', trigger: 'focus', placement: 'right' }); {% endblock %}
+your friends") }}", trigger: 'focus', placement: 'right' }); {% endblock %}
```

### Comparing `ihatemoney-5.2.0/ihatemoney/templates/invitation_mail.en.j2` & `ihatemoney-6.0.0/ihatemoney/templates/invitation_mail.en.j2`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/templates/invitation_mail.fr.j2` & `ihatemoney-6.0.0/ihatemoney/templates/invitation_mail.fr.j2`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/templates/layout.html` & `ihatemoney-6.0.0/ihatemoney/templates/layout.html`

 * *Files 3% similar despite different names*

```diff
@@ -101,43 +101,51 @@
               </a>
             </li>
             {% if g.project %}
             <li><a class="dropdown-item" href="{{ url_for("main.history") }}">{{ _("History") }}</a></li>
             <li><a class="dropdown-item" href="{{ url_for("main.edit_project") }}">{{ _("Settings") }}</a></li>
             {% endif %}
 
-            {% if session['projects'] and not ((session['projects'] | length) == 1 and g.project and session['projects'][0][0] == g.project.id) %}
+            {% if session['projects'] and not ((session['projects'] | length) == 1 and g.project and g.project.id in session['projects']) %}
             <li class="dropdown-divider"></li>
             <li class="dropdown-header">{{ _('Other projects :') }}</li>
-              {% for id, name in session['projects'] %}
+              {% for id, name in session['projects'].items() %}
                 {% if not g.project or id != g.project.id %}
                 <li><a class="dropdown-item" href="{{ url_for("main.list_bills", project_id=id) }}">{{ _("switch to") }} {{ name }}</a></li>
                 {% endif %}
               {% endfor %}
             {% endif %}
             <li class="dropdown-divider"></li>
             {% if session['is_admin'] %}
             <li><a class="dropdown-item" href="{{ url_for("main.dashboard") }}">{{ _("Dashboard") }}</a></li>
             {% endif %}
             <li>
-              <a class="dropdown-item" href="{{ url_for("main.exit") }}">
-                {{ _("Logout") }}
-              </a>
+              <form action="{{ url_for("main.exit") }}" method="post">
+                {{ g.logout_form.hidden_tag() }}
+                {{ g.logout_form.submit(class="dropdown-item") }}
+              </form>
             </li>
           </ul>
         </li>
       {% endif %}
       </ul>
     </div>
   </nav>
 
   <div class="container-fluid flex-shrink-0 {% if request.url_rule.endpoint == 'main.home' %} home-container {% endif %}">
   {% block body %}
       <main class="content offset-1 col-10">
+      {% if breached_limit %}
+        <p class="alert alert-danger">
+          {{ limit_message }}<br />
+          {{ _("Please retry after %(date)s.", date=breached_limit.reset_at  | from_timestamp | datetimeformat("short") )}}
+        </p>
+      {% else %}
       {% block content %}{% endblock %}
+      {% endif %}
       </main>
   {% endblock %}
   </div>
 
   {% if not messages_shown %}
   {{ flash_messages(classes="w-100 justify-content-center") }}
   {% endif %}
```

### Comparing `ihatemoney-5.2.0/ihatemoney/templates/list_bills.html` & `ihatemoney-6.0.0/ihatemoney/templates/list_bills.html`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,20 @@
 
     var unhighlight_owers = function(){
         $('[id^="bal-member-"]').removeClass("ower_line payer_line");
     };
 
     $('#bill_table tbody tr').hover(highlight_owers, unhighlight_owers);
 
+    {% include "helpers.js" %}
+    confirm_action(".delete-bill", { exclude_classes: "action delete", add_classes: "btn btn-sm" });
+
 {% endblock %}
 
+
 {% block sidebar %}
     <div class="sidebar_content">
         <form id="add-member-form" action="{{ url_for(".add_member") }}" method="post" class="py-3">
             {{ forms.add_member(member_form) }}
         </form>
 
         <div id="table_overflow">
@@ -131,17 +135,17 @@
                 {%- endif %}</td>
                 <td>
                     <span data-toggle="tooltip" data-placement="top"
                         title="{{ weighted_bill_amount(bill, weights, g.project.default_currency, bill.converted_amount) if bill.original_currency != g.project.default_currency else '' }}">
                         {{ weighted_bill_amount(bill, weights) }}
                     </span>
                 </td>
-                <td class="bill-actions">
+                <td class="bill-actions d-flex align-items-center">
                     <a class="edit" href="{{ url_for(".edit_bill", bill_id=bill.id) }}" title="{{ _("edit") }}">{{ _('edit') }}</a>
-                    <form action="{{ url_for(".delete_bill", bill_id=bill.id) }}" method="POST">
+                    <form class="delete-bill" action="{{ url_for(".delete_bill", bill_id=bill.id) }}" method="POST">
                         {{ csrf_form.csrf_token }}
                         <button class="action delete" type="submit" title="{{ _("delete") }}"></button>
                     </form>
                     {% if bill.external_link %}
                     <a class="show" href="{{ bill.external_link }}" ref="noopener" target="_blank" title="{{ _("show") }}">{{ _('show') }} </a>
                     {% endif %}
                 </td>
```

### Comparing `ihatemoney-5.2.0/ihatemoney/templates/send_invites.html` & `ihatemoney-6.0.0/ihatemoney/templates/send_invites.html`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,23 @@
                 <a href="{{ url_for(".join_project", _external=True, project_id=g.project.id, token=g.project.generate_token()) }}">
                     {{ url_for(".join_project", _external=True, project_id=g.project.id, token=g.project.generate_token()) }}
                 </a>
             </td>
         </tr>
         <tr>
             <td>
+                <h3>{{ _('Scan QR code') }}</h3>
+                <p><small>{% trans download_mobile=url_for(".mobile") %}On a mobile device, with <a href="{{ download_mobile }}">a compatible app installed</a>.{% endtrans %}</small></p>
+            </td>
+            <td>
+                {{ qrcode | safe }}
+            </td>
+        </tr>
+        <tr>
+            <td>
                 <h3>{{ _('Send via Emails') }}</h3>
             </td>
             <td>
                 <p>{{ _("Specify a (comma separated) list of email adresses you want to notify about the
                 creation of this budget management project and we will send them an email for you.") }}</p>
                 {% include "display_errors.html" %}
                 <form class="invites form-horizontal" method="post" accept-charset="utf-8">
```

### Comparing `ihatemoney-5.2.0/ihatemoney/templates/settle_bills.html` & `ihatemoney-6.0.0/ihatemoney/templates/settle_bills.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/templates/showcase.html` & `ihatemoney-6.0.0/ihatemoney/templates/showcase.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/templates/sidebar_table_layout.html` & `ihatemoney-6.0.0/ihatemoney/templates/sidebar_table_layout.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/templates/statistics.html` & `ihatemoney-6.0.0/ihatemoney/templates/statistics.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/tests/api_test.py` & `ihatemoney-6.0.0/ihatemoney/tests/api_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,14 @@
         self.assertTrue(400, resp.status_code)
         self.assertEqual(
             '{"contact_email": ["Invalid email address."]}\n', resp.data.decode("utf-8")
         )
 
         # create it
         with self.app.mail.record_messages() as outbox:
-
             resp = self.api_create("raclette")
             self.assertTrue(201, resp.status_code)
 
             # Check that email messages have been sent.
             self.assertEqual(len(outbox), 1)
             self.assertEqual(outbox[0].recipients, ["raclette@notmyidea.org"])
 
@@ -923,15 +922,15 @@
                 "what": "fromage",
                 "payer": "1",
                 "payed_for": ["1"],
                 "amount": "0",
             },
             headers=self.get_auth("raclette"),
         )
-        self.assertStatus(400, req)
+        self.assertStatus(201, req)
 
     def test_project_creation_with_mixed_case(self):
         self.api_create("Raclette")
         # get information about it
         resp = self.client.get(
             "/api/projects/Raclette", headers=self.get_auth("Raclette")
         )
```

### Comparing `ihatemoney-5.2.0/ihatemoney/tests/budget_test.py` & `ihatemoney-6.0.0/ihatemoney/tests/budget_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from collections import defaultdict
 import datetime
 import re
-from time import sleep
 import unittest
 from urllib.parse import urlparse, urlunparse
 
-from flask import session
+from flask import session, url_for
 import pytest
 from werkzeug.security import check_password_hash, generate_password_hash
 
 from ihatemoney import models
 from ihatemoney.currency_convertor import CurrencyConverter
 from ihatemoney.tests.common.help_functions import extract_link
 from ihatemoney.tests.common.ihatemoney_testcase import IhatemoneyTestCase
@@ -19,15 +18,14 @@
 class BudgetTestCase(IhatemoneyTestCase):
     def test_notifications(self):
         """Test that the notifications are sent, and that email addresses
         are checked properly.
         """
         # sending a message to one person
         with self.app.mail.record_messages() as outbox:
-
             # create a project
             self.login("raclette")
 
             self.post_project("raclette")
             resp = self.client.post(
                 "/raclette/invite",
                 data={"emails": "zorglub@notmyidea.org"},
@@ -54,15 +52,32 @@
                 outbox[0].recipients, ["zorglub@notmyidea.org", "toto@notmyidea.org"]
             )
 
         # mail address checking
         with self.app.mail.record_messages() as outbox:
             response = self.client.post("/raclette/invite", data={"emails": "toto"})
             self.assertEqual(len(outbox), 0)  # no message sent
-            self.assertIn("The email toto is not valid", response.data.decode("utf-8"))
+            self.assertIn(
+                'The email <em class="font-italic">toto</em> is not valid',
+                response.data.decode("utf-8"),
+            )
+
+        # mail address checking for escaping
+        with self.app.mail.record_messages() as outbox:
+            response = self.client.post(
+                "/raclette/invite",
+                data={"emails": "<img src=x onerror=alert(document.domain)>"},
+            )
+            self.assertEqual(len(outbox), 0)  # no message sent
+            self.assertIn(
+                'The email <em class="font-italic">'
+                "&lt;img src=x onerror=alert(document.domain)&gt;"
+                "</em> is not valid",
+                response.data.decode("utf-8"),
+            )
 
         # mixing good and wrong addresses shouldn't send any messages
         with self.app.mail.record_messages() as outbox:
             self.client.post(
                 "/raclette/invite", data={"emails": "zorglub@notmyidea.org, zorglub"}
             )  # not valid
 
@@ -75,67 +90,88 @@
         self.post_project("raclette")
         with self.app.mail.record_messages() as outbox:
             self.client.post("/raclette/invite", data={"emails": "toto@notmyidea.org"})
             self.assertEqual(len(outbox), 1)
             url_start = outbox[0].body.find("You can log in using this link: ") + 32
             url_end = outbox[0].body.find(".\n", url_start)
             url = outbox[0].body[url_start:url_end]
-        self.client.get("/exit")
+        self.client.post("/exit")
         # Test that we got a valid token
         resp = self.client.get(url, follow_redirects=True)
         self.assertIn(
             'You probably want to <a href="/raclette/members/add"',
             resp.data.decode("utf-8"),
         )
         # Test empty and invalid tokens
-        self.client.get("/exit")
+        self.client.post("/exit")
         # Use another project_id
         parsed_url = urlparse(url)
         resp = self.client.get(
             urlunparse(
                 parsed_url._replace(
                     path=parsed_url.path.replace("raclette/", "invalid_project/")
                 )
             ),
             follow_redirects=True,
         )
-        assert "Create a new project" in resp.data.decode("utf-8")
+        self.assertIn("Create a new project", resp.data.decode("utf-8"))
 
         # A token MUST have a point between payload and signature
         resp = self.client.get("/raclette/join/token.invalid", follow_redirects=True)
         self.assertIn("Provided token is invalid", resp.data.decode("utf-8"))
 
+    def test_multiple_join(self):
+        """Test that joining multiple times a project
+        doesn't add it multiple times in the session"""
+        self.login("raclette")
+        self.post_project("raclette")
+        project = self.get_project("raclette")
+        invite_link = url_for(
+            ".join_project", project_id="raclette", token=project.generate_token()
+        )
+
+        self.post_project("tartiflette")
+        self.client.get(invite_link)
+        data = self.client.get("/tartiflette/").data.decode("utf-8")
+        # First join is OK
+        self.assertIn('href="/raclette/"', data)
+
+        # Second join shouldn't add a double link
+        self.client.get(invite_link)
+        data = self.client.get("/tartiflette/").data.decode("utf-8")
+        self.assertEqual(data.count('href="/raclette/"'), 1)
+
     def test_invite_code_invalidation(self):
         """Test that invitation link expire after code change"""
         self.login("raclette")
         self.post_project("raclette")
         response = self.client.get("/raclette/invite").data.decode("utf-8")
         link = extract_link(response, "share the following link")
 
-        self.client.get("/exit")
+        self.client.post("/exit")
         response = self.client.get(link)
         # Link is valid
-        assert response.status_code == 302
+        self.assertEqual(response.status_code, 302)
 
         # Change password to invalidate token
         # Other data are required, but useless for the test
         response = self.client.post(
             "/raclette/edit",
             data={
                 "name": "raclette",
                 "contact_email": "zorglub@notmyidea.org",
                 "password": "didoudida",
                 "default_currency": "XXX",
             },
             follow_redirects=True,
         )
-        assert response.status_code == 200
-        assert "alert-danger" not in response.data.decode("utf-8")
+        self.assertEqual(response.status_code, 200)
+        self.assertNotIn("alert-danger", response.data.decode("utf-8"))
 
-        self.client.get("/exit")
+        self.client.post("/exit")
         response = self.client.get(link, follow_redirects=True)
         # Link is invalid
         self.assertIn("Provided token is invalid", response.data.decode("utf-8"))
 
     def test_password_reminder(self):
         # test that it is possible to have an email containing the password of a
         # project in case people forget it (and it happens!)
@@ -275,15 +311,14 @@
             # session is updated
             self.assertTrue(session["raclette"])
 
             # project is created
             self.assertEqual(len(models.Project.query.all()), 1)
 
     def test_project_deletion(self):
-
         with self.client as c:
             c.post(
                 "/create",
                 data={
                     "name": "raclette party",
                     "id": "raclette",
                     "password": "party",
@@ -494,16 +529,20 @@
                 "/authenticate", data={"id": "raclette", "password": "raclette"}
             )
 
             self.assertNotIn("Authentication", resp.data.decode("utf-8"))
             self.assertIn("raclette", session)
             self.assertTrue(session["raclette"])
 
+            # logout should work with POST only
+            resp = c.get("/exit")
+            self.assertStatus(405, resp)
+
             # logout should wipe the session out
-            c.get("/exit")
+            c.post("/exit")
             self.assertNotIn("raclette", session)
 
         # test that with admin credentials, one can access every project
         self.app.config["ADMIN_PASSWORD"] = generate_password_hash("pass")
         with self.client as c:
             resp = c.post("/admin?goto=%2Fraclette", data={"admin_password": "pass"})
             self.assertNotIn("Authentication", resp.data.decode("utf-8"))
@@ -555,30 +594,31 @@
         self.client.post("/admin?goto=%2Fcreate", data={"admin_password": "wrong"})
         self.client.post("/admin?goto=%2Fcreate", data={"admin_password": "wrong"})
         resp = self.client.post(
             "/admin?goto=%2Fcreate", data={"admin_password": "wrong"}
         )
 
         self.assertIn(
-            "Too many failed login attempts, please retry later.",
+            "Too many failed login attempts.",
             resp.data.decode("utf-8"),
         )
-        # Change throttling delay
-        from ihatemoney.web import login_throttler
+        # Try with limiter disabled
+        from ihatemoney.utils import limiter
 
-        login_throttler._delay = 0.005
-        # Wait for delay to expire and retry logging in
-        sleep(1)
-        resp = self.client.post(
-            "/admin?goto=%2Fcreate", data={"admin_password": "wrong"}
-        )
-        self.assertNotIn(
-            "Too many failed login attempts, please retry later.",
-            resp.data.decode("utf-8"),
-        )
+        try:
+            limiter.enabled = False
+            resp = self.client.post(
+                "/admin?goto=%2Fcreate", data={"admin_password": "wrong"}
+            )
+            self.assertNotIn(
+                "Too many failed login attempts.",
+                resp.data.decode("utf-8"),
+            )
+        finally:
+            limiter.enabled = True
 
     def test_manage_bills(self):
         self.post_project("raclette")
 
         # add two participants
         self.client.post("/raclette/members/add", data={"name": "zorglub"})
         self.client.post("/raclette/members/add", data={"name": "fred"})
@@ -882,26 +922,38 @@
             "/admin?goto=%2Fdashboard",
             data={"admin_password": "adminpass"},
             follow_redirects=True,
         )
         self.assertIn('<div class="alert alert-danger">', resp.data.decode("utf-8"))
 
         # test access to the dashboard when it is activated
-        self.app.config["ACTIVATE_ADMIN_DASHBOARD"] = True
-        self.app.config["ADMIN_PASSWORD"] = generate_password_hash("adminpass")
-        resp = self.client.post(
-            "/admin?goto=%2Fdashboard",
-            data={"admin_password": "adminpass"},
-            follow_redirects=True,
-        )
+        self.enable_admin()
+        resp = self.client.get("/dashboard")
         self.assertIn(
-            "<thead><tr><th>Project</th><th>Number of participants",
+            """<thead>
+        <tr>
+            <th>Project</th>
+            <th>Number of participants</th>""",
             resp.data.decode("utf-8"),
         )
 
+    def test_dashboard_project_deletion(self):
+        self.post_project("raclette")
+        self.enable_admin()
+        resp = self.client.get("/dashboard")
+        pattern = re.compile(r"<form id=\"delete-project\" [^>]*?action=\"(.*?)\"")
+        match = pattern.search(resp.data.decode("utf-8"))
+        self.assertIsNotNone(match)
+        self.assertIsNotNone(match.group(1))
+
+        resp = self.client.post(match.group(1))
+
+        # project removed
+        self.assertEqual(len(models.Project.query.all()), 0)
+
     def test_statistics_page(self):
         self.post_project("raclette")
         response = self.client.get("/raclette/statistics")
         self.assertEqual(response.status_code, 200)
 
     def test_statistics(self):
         # Output is checked with the USD sign
@@ -1138,15 +1190,15 @@
         members = defaultdict(int)
         # We should have the same values between transactions and project balances
         for t in transactions:
             members[t["ower"]] -= t["amount"]
             members[t["receiver"]] += t["amount"]
         balance = self.get_project("raclette").balance
         for m, a in members.items():
-            assert abs(a - balance[m.id]) < 0.01
+            self.assertAlmostEqual(a, balance[m.id], delta=0.01)
         return
 
     def test_settle_zero(self):
         self.post_project("raclette")
 
         # add participants
         self.client.post("/raclette/members/add", data={"name": "zorglub"})
@@ -1221,15 +1273,15 @@
             },
         )
         # Ensure it has been created
         raclette = self.get_project("raclette")
         self.assertEqual(raclette.get_bills().count(), 1)
 
         # Log out
-        self.client.get("/exit")
+        self.client.post("/exit")
 
         # Create and log in as another project
         self.post_project("tartiflette")
 
         modified_bill = {
             "date": "2018-12-31",
             "what": "roblochon",
@@ -1259,28 +1311,28 @@
         # Additional check that the bill was indeed not modified or deleted
         bill = models.Bill.query.filter(models.Bill.id == 1).one()
         self.assertEqual(bill.what, "fromage à raclette")
 
         # Use the correct credentials to modify and delete the bill.
         # This ensures that modifying and deleting the bill can actually work
 
-        self.client.get("/exit")
+        self.client.post("/exit")
         self.client.post(
             "/authenticate", data={"id": "raclette", "password": "raclette"}
         )
         self.client.post("/raclette/edit/1", data=modified_bill)
         bill = models.Bill.query.filter(models.Bill.id == 1).one_or_none()
         self.assertNotEqual(bill, None, "bill not found")
         self.assertEqual(bill.what, "roblochon")
         self.client.post("/raclette/delete/1")
         bill = models.Bill.query.filter(models.Bill.id == 1).one_or_none()
         self.assertEqual(bill, None)
 
         # Switch back to the second project
-        self.client.get("/exit")
+        self.client.post("/exit")
         self.client.post(
             "/authenticate", data={"id": "tartiflette", "password": "tartiflette"}
         )
         modified_member = {
             "name": "bulgroz",
             "weight": 42,
         }
@@ -1307,27 +1359,26 @@
         member = models.Person.query.filter(models.Person.id == 1).one_or_none()
         self.assertNotEqual(member, None, "member not found")
         self.assertEqual(member.name, "zorglub")
         self.assertTrue(member.activated)
 
         # Use the correct credentials to modify and delete the member.
         # This ensures that modifying and deleting the member can actually work
-        self.client.get("/exit")
+        self.client.post("/exit")
         self.client.post(
             "/authenticate", data={"id": "raclette", "password": "raclette"}
         )
         self.client.post("/raclette/members/1/edit", data=modified_member)
         member = models.Person.query.filter(models.Person.id == 1).one()
         self.assertEqual(member.name, "bulgroz")
         self.client.post("/raclette/members/1/delete")
         member = models.Person.query.filter(models.Person.id == 1).one_or_none()
         self.assertEqual(member, None)
 
     def test_currency_switch(self):
-
         # A project should be editable
         self.post_project("raclette")
 
         # add participants
         self.client.post("/raclette/members/add", data={"name": "zorglub"})
         self.client.post("/raclette/members/add", data={"name": "fred"})
         self.client.post("/raclette/members/add", data={"name": "tata"})
@@ -1366,43 +1417,43 @@
             },
         )
 
         project = self.get_project("raclette")
 
         # First all converted_amount should be the same as amount, with no currency
         for bill in project.get_bills():
-            assert bill.original_currency == CurrencyConverter.no_currency
-            assert bill.amount == bill.converted_amount
+            self.assertEqual(bill.original_currency, CurrencyConverter.no_currency)
+            self.assertEqual(bill.amount, bill.converted_amount)
 
         # Then, switch to EUR, all bills must have been changed to this currency
         project.switch_currency("EUR")
         for bill in project.get_bills():
-            assert bill.original_currency == "EUR"
-            assert bill.amount == bill.converted_amount
+            self.assertEqual(bill.original_currency, "EUR")
+            self.assertEqual(bill.amount, bill.converted_amount)
 
         # Add a bill in EUR, the current default currency
         self.client.post(
             "/raclette/add",
             data={
                 "date": "2017-01-01",
                 "what": "refund from EUR",
                 "payer": 3,
                 "payed_for": [2],
                 "amount": "20",
                 "original_currency": "EUR",
             },
         )
         last_bill = project.get_bills().first()
-        assert last_bill.converted_amount == last_bill.amount
+        self.assertEqual(last_bill.converted_amount, last_bill.amount)
 
         # Erase all currencies
         project.switch_currency(CurrencyConverter.no_currency)
         for bill in project.get_bills():
-            assert bill.original_currency == CurrencyConverter.no_currency
-            assert bill.amount == bill.converted_amount
+            self.assertEqual(bill.original_currency, CurrencyConverter.no_currency)
+            self.assertEqual(bill.amount, bill.converted_amount)
 
         # Let's go back to EUR to test conversion
         project.switch_currency("EUR")
         # This is a bill in CAD
         self.client.post(
             "/raclette/add",
             data={
@@ -1414,24 +1465,24 @@
                 "original_currency": "CAD",
             },
         )
         last_bill = project.get_bills().first()
         expected_amount = self.converter.exchange_currency(
             last_bill.amount, "CAD", "EUR"
         )
-        assert last_bill.converted_amount == expected_amount
+        self.assertEqual(last_bill.converted_amount, expected_amount)
 
         # Switch to USD. Now, NO bill should be in USD, since they already had a currency
         project.switch_currency("USD")
         for bill in project.get_bills():
-            assert bill.original_currency != "USD"
+            self.assertNotEqual(bill.original_currency, "USD")
             expected_amount = self.converter.exchange_currency(
                 bill.amount, bill.original_currency, "USD"
             )
-            assert bill.converted_amount == expected_amount
+            self.assertEqual(bill.converted_amount, expected_amount)
 
         # Switching back to no currency must fail
         with pytest.raises(ValueError):
             project.switch_currency(CurrencyConverter.no_currency)
 
         # It also must fails with a nice error using the form
         resp = self.client.post(
@@ -1446,15 +1497,14 @@
         )
         # A user displayed error should be generated, and its currency should be the same.
         self.assertStatus(200, resp)
         self.assertIn('<p class="alert alert-danger">', resp.data.decode("utf-8"))
         self.assertEqual(self.get_project("raclette").default_currency, "USD")
 
     def test_currency_switch_to_bill_currency(self):
-
         # Default currency is 'XXX', but we should start from a project with a currency
         self.post_project("raclette", default_currency="USD")
 
         # add participants
         self.client.post("/raclette/members/add", data={"name": "zorglub"})
         self.client.post("/raclette/members/add", data={"name": "fred"})
 
@@ -1470,25 +1520,25 @@
                 "original_currency": "EUR",
             },
         )
 
         project = self.get_project("raclette")
 
         bill = project.get_bills().first()
-        assert bill.converted_amount == self.converter.exchange_currency(
-            bill.amount, "EUR", "USD"
+        self.assertEqual(
+            self.converter.exchange_currency(bill.amount, "EUR", "USD"),
+            bill.converted_amount,
         )
 
         # And switch project to the currency from the bill we created
         project.switch_currency("EUR")
         bill = project.get_bills().first()
-        assert bill.converted_amount == bill.amount
+        self.assertEqual(bill.converted_amount, bill.amount)
 
     def test_currency_switch_to_no_currency(self):
-
         # Default currency is 'XXX', but we should start from a project with a currency
         self.post_project("raclette", default_currency="USD")
 
         # add participants
         self.client.post("/raclette/members/add", data={"name": "zorglub"})
         self.client.post("/raclette/members/add", data={"name": "fred"})
 
@@ -1516,51 +1566,52 @@
                 "original_currency": "EUR",
             },
         )
 
         project = self.get_project("raclette")
 
         for bill in project.get_bills_unordered():
-            assert bill.converted_amount == self.converter.exchange_currency(
-                bill.amount, "EUR", "USD"
+            self.assertEqual(
+                self.converter.exchange_currency(bill.amount, "EUR", "USD"),
+                bill.converted_amount,
             )
 
         # And switch project to no currency: amount should be equal to what was submitted
         project.switch_currency(CurrencyConverter.no_currency)
         no_currency_bills = [
             (bill.amount, bill.converted_amount) for bill in project.get_bills()
         ]
-        assert no_currency_bills == [(5.0, 5.0), (10.0, 10.0)]
+        self.assertEqual(no_currency_bills, [(5.0, 5.0), (10.0, 10.0)])
 
     def test_amount_is_null(self):
         self.post_project("raclette")
 
         # add participants
         self.client.post("/raclette/members/add", data={"name": "zorglub"})
 
         # null amount
-        resp = self.client.post(
+        self.client.post(
             "/raclette/add",
             data={
                 "date": "2016-12-31",
                 "what": "fromage à raclette",
                 "payer": 1,
                 "payed_for": [1],
                 "amount": "0",
                 "original_currency": "EUR",
             },
         )
-        assert '<p class="alert alert-danger">' in resp.data.decode("utf-8")
 
-        resp = self.client.get("/raclette/")
-        # No bills, the previous one was not added
-        assert "No bills" in resp.data.decode("utf-8")
+        # Bill should have been accepted
+        project = self.get_project("raclette")
+        self.assertEqual(project.get_bills().count(), 1)
+        last_bill = project.get_bills().first()
+        self.assertEqual(last_bill.amount, 0)
 
     def test_decimals_on_weighted_members_list(self):
-
         self.post_project("raclette")
 
         # add three users with different weights
         self.client.post(
             "/raclette/members/add", data={"name": "zorglub", "weight": 1.0}
         )
         self.client.post("/raclette/members/add", data={"name": "tata", "weight": 1.10})
@@ -1593,17 +1644,17 @@
                 "what": "fromage à raclette",
                 "payer": 1,
                 "payed_for": [1],
                 "amount": "9347242149381274732472348728748723473278472843.12",
                 "original_currency": "EUR",
             },
         )
-        assert '<p class="alert alert-danger">' in resp.data.decode("utf-8")
+        self.assertIn('<p class="alert alert-danger">', resp.data.decode("utf-8"))
 
         # Without any check, the following request will fail.
         resp = self.client.get("/raclette/")
         # No bills, the previous one was not added
-        assert "No bills" in resp.data.decode("utf-8")
+        self.assertIn("No bills", resp.data.decode("utf-8"))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `ihatemoney-5.2.0/ihatemoney/tests/common/ihatemoney_testcase.py` & `ihatemoney-6.0.0/ihatemoney/tests/common/ihatemoney_testcase.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from ihatemoney import models
 from ihatemoney.currency_convertor import CurrencyConverter
 from ihatemoney.run import create_app, db
 
 
 class BaseTestCase(TestCase):
-
     SECRET_KEY = "TEST SESSION"
     SQLALCHEMY_DATABASE_URI = os.environ.get(
         "TESTING_SQLALCHEMY_DATABASE_URI", "sqlite://"
     )
     ENABLE_CAPTCHA = False
 
     def create_app(self):
@@ -99,13 +98,24 @@
         return models.Project.query.get(id)
 
 
 class IhatemoneyTestCase(BaseTestCase):
     TESTING = True
     WTF_CSRF_ENABLED = False  # Simplifies the tests.
 
-    def assertStatus(self, expected, resp, url=""):
+    def assertStatus(self, expected, resp, url=None):
+        if url is None:
+            url = resp.request.path
         return self.assertEqual(
             expected,
             resp.status_code,
             f"{url} expected {expected}, got {resp.status_code}",
         )
+
+    def enable_admin(self, password="adminpass"):
+        self.app.config["ACTIVATE_ADMIN_DASHBOARD"] = True
+        self.app.config["ADMIN_PASSWORD"] = generate_password_hash(password)
+        return self.client.post(
+            "/admin?goto=%2Fdashboard",
+            data={"admin_password": password},
+            follow_redirects=True,
+        )
```

### Comparing `ihatemoney-5.2.0/ihatemoney/tests/history_test.py` & `ihatemoney-6.0.0/ihatemoney/tests/history_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             new_data["project_history"] = "y"
             if logging_preference == LoggingMode.RECORD_IP:
                 new_data["ip_recording"] = "y"
 
         # Disable History
         resp = self.client.post("/demo/edit", data=new_data, follow_redirects=True)
         self.assertEqual(resp.status_code, 200)
-        self.assertNotIn("danger", resp.data.decode("utf-8"))
+        self.assertNotIn("alert-danger", resp.data.decode("utf-8"))
 
         resp = self.client.get("/demo/edit")
         self.assertEqual(resp.status_code, 200)
         if logging_preference == LoggingMode.DISABLED:
             self.assertIn('<input id="project_history"', resp.data.decode("utf-8"))
         else:
             self.assertIn(
@@ -469,15 +469,14 @@
         resp = self.client.get("/demo/history")
         self.assertEqual(resp.status_code, 200)
         self.assertIn(
             f"Participant {em_surround('new name')} removed", resp.data.decode("utf-8")
         )
 
     def test_double_bill_double_person_edit_second(self):
-
         # add two members
         self.client.post("/demo/members/add", data={"name": "User 1"})
         self.client.post("/demo/members/add", data={"name": "User 2"})
 
         # add two bills
         self.client.post(
             "/demo/add",
@@ -653,12 +652,12 @@
         )
 
         # Recreate it
         self.post_project("raclette", password="party")
 
         # History should be equal to project creation
         history_list = history.get_history(self.get_project("raclette"))
-        assert len(history_list) == 1
+        self.assertEqual(len(history_list), 1)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `ihatemoney-5.2.0/ihatemoney/tests/import_test.py` & `ihatemoney-6.0.0/ihatemoney/tests/import_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -592,14 +592,46 @@
         received_lines = resp.data.decode("utf-8").split("\n")
 
         for i, line in enumerate(expected):
             self.assertEqual(
                 set(line.split(",")), set(received_lines[i].strip("\r").split(","))
             )
 
+    def test_export_escape_formulae(self):
+        self.post_project("raclette", default_currency="EUR")
+
+        # add participants
+        self.client.post("/raclette/members/add", data={"name": "zorglub"})
+
+        # create bills
+        self.client.post(
+            "/raclette/add",
+            data={
+                "date": "2016-12-31",
+                "what": "=COS(36)",
+                "payer": 1,
+                "payed_for": [1],
+                "amount": "10.0",
+                "original_currency": "EUR",
+            },
+        )
+
+        # generate csv export of bills
+        resp = self.client.get("/raclette/export/bills.csv")
+        expected = [
+            "date,what,amount,currency,payer_name,payer_weight,owers",
+            "2016-12-31,'=COS(36),10.0,EUR,zorglub,1.0,zorglub",
+        ]
+        received_lines = resp.data.decode("utf-8").split("\n")
+
+        for i, line in enumerate(expected):
+            self.assertEqual(
+                set(line.split(",")), set(received_lines[i].strip("\r").split(","))
+            )
+
 
 class ImportTestCaseJSON(CommonTestCase.Import):
     def generate_form_data(self, data):
         return {"file": (list_of_dicts2json(data), "test.json")}
 
 
 class ImportTestCaseCSV(CommonTestCase.Import):
```

### Comparing `ihatemoney-5.2.0/ihatemoney/tests/main_test.py` & `ihatemoney-6.0.0/ihatemoney/tests/main_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,27 +149,26 @@
                 "what": "delicatessen",
                 "payer": 1,
                 "payed_for": [1, 2],
                 "amount": "10",
             },
         )
         project = models.Project.query.get_by_name(name="raclette")
-        for (weight, bill) in project.get_bill_weights().all():
+        for weight, bill in project.get_bill_weights().all():
             if bill.what == "red wine":
                 pay_each_expected = 20 / 2
                 self.assertEqual(bill.amount / weight, pay_each_expected)
             if bill.what == "fromage à raclette":
                 pay_each_expected = 10 / 4
                 self.assertEqual(bill.amount / weight, pay_each_expected)
             if bill.what == "delicatessen":
                 pay_each_expected = 10 / 3
                 self.assertEqual(bill.amount / weight, pay_each_expected)
 
     def test_bill_pay_each(self):
-
         self.post_project("raclette")
 
         # add members
         self.client.post("/raclette/members/add", data={"name": "zorglub", "weight": 2})
         self.client.post("/raclette/members/add", data={"name": "fred"})
         self.client.post("/raclette/members/add", data={"name": "tata"})
         # Add a member with a balance=0 :
@@ -297,67 +296,84 @@
                 "Invite people to join this project", resp.data.decode("utf-8")
             )
 
 
 class CaptchaTestCase(IhatemoneyTestCase):
     ENABLE_CAPTCHA = True
 
+    def test_project_creation_with_captcha_case_insensitive(self):
+        # Test that case doesn't matter
+        # Patch the lazy_gettext as it is imported as '_' in forms for captcha value check
+        with patch("ihatemoney.forms._", new=lambda x: "ÉÙÜẞ"), self.client as c:
+            c.post(
+                "/create",
+                data={
+                    "name": "raclette party",
+                    "id": "raclette",
+                    "password": "party",
+                    "contact_email": "raclette@notmyidea.org",
+                    "default_currency": "USD",
+                    "captcha": "éùüß",
+                },
+            )
+            self.assertEqual(len(models.Project.query.all()), 1)
+
     def test_project_creation_with_captcha(self):
         with self.client as c:
             c.post(
                 "/create",
                 data={
                     "name": "raclette party",
                     "id": "raclette",
                     "password": "party",
                     "contact_email": "raclette@notmyidea.org",
                     "default_currency": "USD",
                 },
             )
-            assert len(models.Project.query.all()) == 0
+            self.assertEqual(len(models.Project.query.all()), 0)
 
             c.post(
                 "/create",
                 data={
                     "name": "raclette party",
                     "id": "raclette",
                     "password": "party",
                     "contact_email": "raclette@notmyidea.org",
                     "default_currency": "USD",
                     "captcha": "nope",
                 },
             )
-            assert len(models.Project.query.all()) == 0
+            self.assertEqual(len(models.Project.query.all()), 0)
 
             c.post(
                 "/create",
                 data={
                     "name": "raclette party",
                     "id": "raclette",
                     "password": "party",
                     "contact_email": "raclette@notmyidea.org",
                     "default_currency": "USD",
                     "captcha": "euro",
                 },
             )
-            assert len(models.Project.query.all()) == 1
+            self.assertEqual(len(models.Project.query.all()), 1)
 
     def test_api_project_creation_does_not_need_captcha(self):
         self.client.get("/")
         resp = self.client.post(
             "/api/projects",
             data={
                 "name": "raclette",
                 "id": "raclette",
                 "password": "raclette",
                 "contact_email": "raclette@notmyidea.org",
             },
         )
         self.assertTrue(resp.status, 201)
-        assert len(models.Project.query.all()) == 1
+        self.assertEqual(len(models.Project.query.all()), 1)
 
 
 class TestCurrencyConverter(unittest.TestCase):
     converter = CurrencyConverter()
     mock_data = {
         "USD": 1,
         "EUR": 0.8,
@@ -378,10 +394,20 @@
             ["USD", "EUR", "CAD", "PLN", CurrencyConverter.no_currency],
         )
 
     def test_exchange_currency(self):
         result = self.converter.exchange_currency(100, "USD", "EUR")
         self.assertEqual(result, 80.0)
 
+    def test_failing_remote(self):
+        rates = {}
+        with patch("requests.Response.json", new=lambda _: {}), self.assertWarns(
+            UserWarning
+        ):
+            # we need a non-patched converter, but it seems that MagickMock
+            # is mocking EVERY instance of the class method. Too bad.
+            rates = CurrencyConverter.get_rates(self.converter)
+        self.assertDictEqual(rates, {CurrencyConverter.no_currency: 1})
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/cs/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/cs/LC_MESSAGES/messages.mo`

 * *Files 26% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,21 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
+"Project-Id-Version: Czech (I Hate Money)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-10-26 23:38+0200\n"
-"PO-Revision-Date: 2021-09-05 13:34+0000\n"
-"Last-Translator: Clonewayx <fillip1@seznam.cz>\n"
-"Language: cs\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: Czech <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/cs/>\n"
-"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2\n"
+"Language: cs\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
+"Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
+"X-Generator: Weblate 4.14.2\n"
 
 msgid "A link to an external document, related to this bill"
 msgstr "Externí odkaz k této účtence"
 
 msgid ""
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
@@ -162,15 +161,15 @@
 msgid "The email %(email)s is not valid"
 msgstr "Toto (%(email)s) není validní e-mail"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
-"Tento projekt nemůže být nastaven na  'bez měny' protože obsahuje účty v "
+"Tento projekt nemůže být nastaven na 'bez měny' protože obsahuje účty v "
 "různých měnáh."
 
 msgid "This project does not exists"
 msgstr "Tento projekt neexistuje"
 
 msgid "Too many failed login attempts, please retry later."
 msgstr "Příliš mnoho pokusů, zkuste to později."
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/cs/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/cs/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2021-09-05 13:34+0000\n"
-"Last-Translator: Clonewayx <fillip1@seznam.cz>\n"
+"PO-Revision-Date: 2022-11-07 10:07+0000\n"
+"Last-Translator: Moshi Moshi <ifeeltiredboss@gmail.com>\n"
+"Language-Team: Czech <https://hosted.weblate.org/projects/i-hate-money/"
+"i-hate-money/cs/>\n"
 "Language: cs\n"
-"Language-Team: Czech <https://hosted.weblate.org/projects/i-hate-money/i"
-"-hate-money/cs/>\n"
-"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
+"X-Generator: Weblate 4.14.2\n"
 "Generated-By: Babel 2.9.0\n"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr "Neplatná částka nebo výraz. Pouze čísla a operátory + - * / jsou přípustná"
 
@@ -44,15 +44,15 @@
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
-"Tento projekt nemůže být nastaven na  'bez měny' protože obsahuje účty v "
+"Tento projekt nemůže být nastaven na 'bez měny' protože obsahuje účty v "
 "různých měnáh."
 
 msgid "Import previously exported JSON file"
 msgstr "Import exportovaného JSON souboru"
 
 msgid "Import"
 msgstr "Import"
@@ -1029,8 +1029,7 @@
 #~ msgstr ""
 
 #~ msgid "Edit this member"
 #~ msgstr ""
 
 #~ msgid "Participants to notify"
 #~ msgstr ""
-
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/de/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/de/LC_MESSAGES/messages.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: German <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.10-dev\n"
+"X-Generator: Weblate 5.0-dev\n"
 
 msgid ""
 "\n"
 "            <i>The table below reflects actions recorded prior to disabling "
 "project history. You can\n"
 "            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
 "target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
@@ -109,17 +109,14 @@
 
 msgid "Amount"
 msgstr "Betrag"
 
 msgid "Amount in %(currency)s"
 msgstr "Betrag in %(currency)s"
 
-msgid "Amount paid"
-msgstr "Betrag"
-
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
 "                The rest of the project history will be unaffected. This "
 "action cannot be undone."
 msgstr ""
 "Bist du sicher, dass alle aufgezeichneten IP-Adressen dieses Projekts "
@@ -130,17 +127,14 @@
 msgid ""
 "Are you sure you want to erase all history for this project? This action "
 "cannot be undone."
 msgstr ""
 "Bist du sicher, dass der gesamte Projektverlauf gelöscht werden soll? Dies "
 "kann nicht rückgängig gemacht werden."
 
-msgid "Are you sure?"
-msgstr "Bist du sicher?"
-
 msgid "Authentication"
 msgstr "Authentifizierung"
 
 msgid "Back to the list"
 msgstr "Zurück zur Liste"
 
 msgid "Balance"
@@ -385,26 +379,14 @@
 
 msgid "IP address recording can be enabled on the settings page"
 msgstr "IP-Adresserfassung kann in den Einstellungen aktiviert werden"
 
 msgid "Identifier:"
 msgstr "ID:"
 
-msgid "Import"
-msgstr "Importieren"
-
-msgid "Import JSON"
-msgstr "JSON importieren"
-
-msgid "Import previously exported JSON file"
-msgstr "Zuvor exportierte JSON-Datei importieren"
-
-msgid "Invalid JSON"
-msgstr "Ungültiges JSON"
-
 msgid "Invalid private code."
 msgstr "ungültiger privater Code."
 
 msgid "Invalid token"
 msgstr "Ungültiger Token"
 
 msgid "Invite people"
@@ -662,31 +644,14 @@
 msgstr ""
 "Einige der folgenden Einträge enthalten IP-Adressen, wenngleich die IP-"
 "Erfassung dieses Projekts deaktiviert ist. "
 
 msgid "Someone probably cleared the project history."
 msgstr "Wahrscheinlich hat jemand den Projektverlauf gelöscht."
 
-msgid ""
-"Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
-msgstr ""
-"Entschuldigung, es trat ein Fehler beim Senden der E-Mail zur Passwort "
-"Zurücksetzung auf. Bitte überprüfe die E-Mail Konfiguration des Servers oder "
-"kontaktiere einen Administrator."
-
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. Please "
-"check the email configuration of the server or contact the administrator."
-msgstr ""
-"Entschuldigung, es trat ein Fehler beim Versenden der Einladungsmails auf. "
-"Bitte überprüfe die E-Mail Konfiguration des Servers oder kontaktiere einen "
-"Administrator."
-
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "Entschuldigung, wir können die angefragte Seite nicht finden."
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify about "
 "the\n"
 "                creation of this budget management project and we will send "
@@ -729,17 +694,14 @@
 
 msgid "The email %(email)s is not valid"
 msgstr "Die E-Mail-Adresse(n) %(email)s ist/sind nicht gültig"
 
 msgid "The participant name is invalid"
 msgstr "Der Benutzername ist ungültig"
 
-msgid "The project identifier is %(project)s"
-msgstr "Die Projektkennung ist %(project)s"
-
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "Das Projekt existiert nicht, willst du"
 
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "Das Administrator-Passwort ist nicht korrekt. Noch %(num)d Versuch(e) "
 "verbleibend."
@@ -765,18 +727,14 @@
 
 msgid "Time"
 msgstr "Zeit"
 
 msgid "To whom?"
 msgstr "An wen?"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr ""
-"Zu viele fehlgeschlagene Anmeldeversuche, bitte versuche es später nochmal."
-
 msgid "Try out the demo"
 msgstr "Demo ausprobieren"
 
 msgid "Unknown error"
 msgstr "Unbekannter Fehler"
 
 msgid "Unknown project"
@@ -859,15 +817,15 @@
 msgid "add participants"
 msgstr "Teilnehmer hinzufügen"
 
 msgid "can't remember your password?"
 msgstr "Kannst du dich nicht an dein Passwort erinnern?"
 
 msgid "create it"
-msgstr "Erstellen"
+msgstr "es erstellen"
 
 msgid "deactivate"
 msgstr "deaktivieren"
 
 msgid "delete"
 msgstr "Löschen"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/de/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/de/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2021-11-29 23:53+0000\n"
-"Last-Translator: Jannik Lang <jannik.lang@posteo.de>\n"
+"PO-Revision-Date: 2023-07-09 19:50+0000\n"
+"Last-Translator: Sebastian Lay <mail@sebastian-lay.de>\n"
 "Language-Team: German <https://hosted.weblate.org/projects/i-hate-money/"
 "i-hate-money/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.10-dev\n"
+"X-Generator: Weblate 5.0-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Kein gültiger Betrag oder Ausdruck. Es werden nur Zahlen und die "
@@ -375,15 +375,15 @@
 msgid "Authentication"
 msgstr "Authentifizierung"
 
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "Das Projekt existiert nicht, willst du"
 
 msgid "create it"
-msgstr "Erstellen"
+msgstr "es erstellen"
 
 msgid "?"
 msgstr "?"
 
 msgid "Create a new project"
 msgstr "Neues Projekt erstellen"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/el/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/el/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/eo/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/eo/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/eo/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/eo/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/es/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/hu/LC_MESSAGES/messages.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,303 +1,307 @@
-
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2021-04-14 08:27+0000\n"
-"Last-Translator: fcoterroba <fcoterroba@gmail.com>\n"
-"Language: es\n"
-"Language-Team: Spanish <https://hosted.weblate.org/projects/i-hate-"
-"money/i-hate-money/es/>\n"
-"Plural-Forms: nplurals=2; plural=n != 1\n"
+"POT-Creation-Date: 2023-01-22 21:15+0200\n"
+"PO-Revision-Date: 2023-04-19 11:51+0000\n"
+"Last-Translator: Gergely Kocsis <koger23@gmail.com>\n"
+"Language-Team: Hungarian <https://hosted.weblate.org/projects/i-hate-money/"
+"i-hate-money/hu/>\n"
+"Language: hu\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
+"Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.0\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
-"Cantidad o expresión no válida. Solo se aceptan números y los operadores "
-"+ - * /."
+"Érvénytelen mennyiség vagy kifejezés. Csak számok és műveleti jelek ( + - * "
+"/) megengedettek."
 
 msgid "Project name"
-msgstr "Nombre del proyecto"
+msgstr "A projekt neve"
 
-#, fuzzy
 msgid "New private code"
-msgstr "Código privado"
+msgstr "Új titkos kód"
 
 msgid "Enter a new code if you want to change it"
-msgstr ""
+msgstr "Adj meg egy új kódot, ha meg akarod változtatni"
 
 msgid "Email"
-msgstr "Correo electrónico"
+msgstr "Email"
 
 msgid "Enable project history"
-msgstr "Habilitar historial del proyecto"
+msgstr "Projekt történet bekapcsolása"
 
 msgid "Use IP tracking for project history"
-msgstr "Usar trackeo IP para historial de proyecto"
+msgstr "IP nyomkövetés használata a projekt előzményekhez"
 
 msgid "Default Currency"
-msgstr "Moneda por defecto"
+msgstr "Alapértelmezett Pénznem"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
+"Alapértelmezett pénznem beállítása lehetővé teszi a számlák közötti "
+"pénzváltást"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
+"A projekt nem állítható pénznem nélkülire, mert számlákat és több pénznemet "
+"is tartalmaz."
 
 msgid "Import previously exported JSON file"
-msgstr "Importar .JSON previamente exportado"
+msgstr "Korábban exportált JSON fájl importálása"
 
 msgid "Import"
-msgstr "Importar"
+msgstr ""
 
 msgid "Project identifier"
-msgstr "Identificador del proyecto"
+msgstr "Projekt azonosító"
 
 msgid "Private code"
-msgstr "Código privado"
+msgstr "Titkos kód"
 
 msgid "Create the project"
-msgstr "Crear proyecto"
+msgstr "Projekt létrehozása"
 
 #, python-format
 msgid ""
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
 msgstr ""
-"Un proyecto con este identificador (\"%(project)s\") ya existe. Elija un "
-"nuevo identificador, por favor."
+"Már létezik egy projekt ezzel az azonosítóval (\"%(project)s\"). Kérjük, "
+"válasszon más azonosítót"
 
 msgid "Which is a real currency: Euro or Petro dollar?"
-msgstr ""
+msgstr "Melyik valódi pénznem, az euró vagy a petrodollár?"
 
-#, fuzzy
 msgid "euro"
-msgstr "Período"
+msgstr "euró"
 
 msgid "Please, validate the captcha to proceed."
-msgstr ""
+msgstr "Kérlek validáld a captcha-t a folytatáshoz."
 
 msgid "Enter private code to confirm deletion"
-msgstr ""
+msgstr "Add meg a titkos kódot a törlés megerősítéséhez"
 
 msgid "Unknown error"
-msgstr ""
+msgstr "Ismeretlen hiba"
 
-#, fuzzy
 msgid "Invalid private code."
-msgstr "Código privado"
+msgstr "Érvénytelen titkos kód."
 
+#, fuzzy
 msgid "Get in"
-msgstr ""
+msgstr "Szállj be"
 
 msgid "Admin password"
-msgstr "Contraseña de administrador"
+msgstr "Adminisztrátori jelszó"
 
 msgid "Send me the code by email"
-msgstr "Envíame el código por correo electrónico"
+msgstr "Kód küldése e-mailben"
 
 msgid "This project does not exists"
-msgstr "Proyecto inexistente"
+msgstr "Ez a projekt nem létezik"
 
 msgid "Password mismatch"
-msgstr "La contraseña no coincide"
+msgstr "A jelszavak nem egyeznek"
 
 msgid "Password"
-msgstr "Contraseña"
+msgstr "Jelszó"
 
 msgid "Password confirmation"
-msgstr "Confirmar contraseña"
+msgstr "Jelszó megerősítése"
 
 msgid "Reset password"
-msgstr "Reestablecer contraseña"
+msgstr "Jelszó visszaállítása"
 
 msgid "Date"
-msgstr "Fecha"
+msgstr "Dátum"
 
 msgid "What?"
-msgstr "¿Qué?"
+msgstr "Mi?"
 
 msgid "Payer"
-msgstr ""
+msgstr "Fizető"
 
 msgid "Amount paid"
-msgstr "Cantidad pagada"
+msgstr "Kifizetett összeg"
 
 msgid "Currency"
-msgstr "Divisa"
+msgstr "Pénznem"
 
 msgid "External link"
-msgstr "Enlace externo"
+msgstr "Külső hivatkozás"
 
 msgid "A link to an external document, related to this bill"
-msgstr ""
+msgstr "A számlához kapcsolódó külső dokumentum linkje"
 
 msgid "For whom?"
-msgstr "¿Para quién?"
+msgstr "Kinek?"
 
 msgid "Submit"
-msgstr ""
+msgstr "Mentés"
 
 msgid "Submit and add a new one"
-msgstr ""
+msgstr "Mentés és új hozzáadása"
 
 #, python-format
 msgid "Project default: %(currency)s"
-msgstr ""
+msgstr "Projekt alapértelmezés: %(currency)s"
 
 msgid "Bills can't be null"
-msgstr ""
+msgstr "A számla nem lehet üres"
 
 msgid "Name"
-msgstr "Nombre"
+msgstr "Név"
 
 msgid "Weights should be positive"
-msgstr ""
+msgstr "A súlyoknak pozitív értékűnek kell lenni"
 
 msgid "Weight"
-msgstr ""
+msgstr "Súly"
 
 msgid "Add"
-msgstr "Añadir"
+msgstr "Hozzáadás"
 
 msgid "The participant name is invalid"
-msgstr ""
+msgstr "A résztvevő neve érvénytelen"
 
 msgid "This project already have this participant"
-msgstr ""
+msgstr "Ez a résztvevő már szerepel ebben a projektben"
 
 msgid "People to notify"
-msgstr ""
+msgstr "Értesítendő személyek"
 
 msgid "Send invites"
-msgstr "Enviar invitaciones"
+msgstr "Meghívók küldése"
 
 #, python-format
 msgid "The email %(email)s is not valid"
-msgstr "El correo %(email)s no es válido"
+msgstr "Érvénytelen e-mail cím: %(email)s"
 
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
-msgstr ""
+msgstr "{dual_object_0} és {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
-msgstr ""
+msgstr "{previous_object} és {end_object}"
 
 #. Two items in a middle of a list with more than 5 objects
 msgid "{previous_object}, {next_object}"
-msgstr ""
+msgstr "{previous_object}, {next_object}"
 
 #. First two items of a list with more than 3 items
 msgid "{start_object}, {next_object}"
-msgstr ""
+msgstr "{start_object}, {next_object}"
 
 msgid "No Currency"
-msgstr ""
+msgstr "Nincs pénznem"
 
 #. Form error with only one error
 msgid "{prefix}: {error}"
-msgstr ""
+msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
-msgstr ""
+msgstr "{prefix}:<br />{errors}"
 
 msgid "Too many failed login attempts, please retry later."
 msgstr ""
+"Túl sok sikertelen bejelentkezési kísérlet, kérlek, próbáld újra később."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
-msgstr ""
+msgstr "Az admin jelszó érvénytelen. Csak %(num)d próbálkozásod maradt."
 
 msgid "Provided token is invalid"
-msgstr ""
+msgstr "A megadott token érvénytelen"
 
 msgid "This private code is not the right one"
-msgstr ""
+msgstr "Ez a titkos kód nem megfelelő"
 
 #, python-format
 msgid "You have just created '%(project)s' to share your expenses"
-msgstr ""
+msgstr "Létrehoztál egy projektet '%(project)s' a kiadásaid megosztására"
 
 msgid "A reminder email has just been sent to you"
-msgstr ""
+msgstr "Az emlékeztető e-mailt kiküldtük"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
+"Megpróbáltuk az emlékeztető e-mailt kiküldeni, de hiba történt. Ettől még "
+"használhatod a megszokott módon a projektet."
 
 #, python-format
 msgid "The project identifier is %(project)s"
 msgstr ""
 
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
 "instructions. Please check the email configuration of the server or "
 "contact the administrator."
 msgstr ""
 
 msgid "No token provided"
-msgstr ""
+msgstr "Nincs token megadva"
 
 msgid "Invalid token"
-msgstr ""
+msgstr "Érvénytelen token"
 
 msgid "Unknown project"
-msgstr ""
+msgstr "Ismeretlen projekt"
 
 msgid "Password successfully reset."
-msgstr ""
+msgstr "Jelszó sikeresen visszaállítva."
 
 msgid "Project successfully uploaded"
-msgstr ""
+msgstr "Projekt sikeresen feltöltve"
 
 msgid "Invalid JSON"
 msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 
 msgid "Project successfully deleted"
-msgstr ""
+msgstr "Projekt sikeresen törölve"
 
 msgid "Error deleting project"
-msgstr ""
+msgstr "Hiba történt a projekt törlésekor"
 
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
-msgstr ""
+msgstr "Meghívtak a következő projektbe %(project)s a kiadásaid megosztására"
 
 msgid "Your invitations have been sent"
-msgstr ""
+msgstr "A meghívóid sikeresen kiküldve"
 
 msgid ""
 "Sorry, there was an error while trying to send the invitation emails. "
 "Please check the email configuration of the server or contact the "
 "administrator."
 msgstr ""
 
 #, python-format
 msgid "%(member)s has been added"
-msgstr ""
+msgstr "%(member)s hozzáadva"
 
 msgid "Error activating participant"
-msgstr ""
+msgstr "Hiba történt a résztvevő aktiválása közben"
 
 #, python-format
 msgid "%(name)s is part of this project again"
 msgstr ""
 
 msgid "Error removing participant"
 msgstr ""
@@ -324,21 +328,19 @@
 
 msgid "The bill has been deleted"
 msgstr ""
 
 msgid "The bill has been modified"
 msgstr ""
 
-#, fuzzy
 msgid "Error deleting project history"
-msgstr "Habilitar historial del proyecto"
+msgstr ""
 
-#, fuzzy
 msgid "Deleted project history."
-msgstr "Habilitar historial del proyecto"
+msgstr ""
 
 msgid "Error deleting recorded IP addresses"
 msgstr ""
 
 msgid "Deleted recorded IP addresses in project history."
 msgstr ""
 
@@ -350,77 +352,73 @@
 
 msgid "Back to the list"
 msgstr ""
 
 msgid "Administration tasks are currently disabled."
 msgstr ""
 
-#, fuzzy
 msgid "Authentication"
-msgstr "Documentación"
+msgstr ""
 
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr ""
 
 msgid "create it"
 msgstr ""
 
 msgid "?"
 msgstr ""
 
 msgid "Create a new project"
 msgstr ""
 
 msgid "Project"
-msgstr "Proyecto"
+msgstr ""
 
-#, fuzzy
 msgid "Number of participants"
-msgstr "añadir participantes"
+msgstr ""
 
 msgid "Number of bills"
 msgstr ""
 
 msgid "Newest bill"
 msgstr ""
 
 msgid "Oldest bill"
 msgstr ""
 
 msgid "Actions"
-msgstr "Acciones"
+msgstr ""
 
 msgid "edit"
-msgstr "editar"
+msgstr ""
 
 msgid "delete"
-msgstr "eliminar"
+msgstr ""
 
 msgid "show"
-msgstr "mostrar"
+msgstr ""
 
 msgid "The Dashboard is currently deactivated."
 msgstr ""
 
-#, fuzzy
 msgid "Download Mobile Application"
-msgstr "Aplicación móvil"
+msgstr ""
 
 msgid "Get it on"
 msgstr ""
 
 msgid "Are you sure?"
 msgstr ""
 
 msgid "Edit project"
 msgstr ""
 
-#, fuzzy
 msgid "Delete project"
-msgstr "Editar el proyecto"
+msgstr ""
 
 msgid "Import JSON"
 msgstr ""
 
 msgid "Choose file"
 msgstr ""
 
@@ -439,64 +437,63 @@
 msgid "Download the list of transactions needed to settle the current bills."
 msgstr ""
 
 msgid "Can't remember the password?"
 msgstr ""
 
 msgid "Cancel"
-msgstr "Cancelar"
+msgstr ""
 
 msgid "Privacy Settings"
-msgstr "Ajustes de privacidad"
+msgstr ""
 
 msgid "Edit the project"
-msgstr "Editar el proyecto"
+msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
 msgid "Edit this bill"
-msgstr "Editar esta factura"
+msgstr ""
 
 msgid "Add a bill"
-msgstr "Añadir una factura"
+msgstr ""
 
 msgid "Everyone"
 msgstr ""
 
 msgid "No one"
 msgstr ""
 
 msgid "More options"
 msgstr ""
 
 msgid "Add participant"
-msgstr "Añadir participante"
+msgstr ""
 
-#, fuzzy
 msgid "Edit this participant"
-msgstr "Añadir participante"
+msgstr ""
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr ""
 
 msgid "Send the invitations"
-msgstr "Enviar invitaciones"
+msgstr ""
 
 msgid "Download"
-msgstr "Descargar"
+msgstr ""
 
 msgid "Disabled Project History"
-msgstr "Historial del proyecto desactivado"
+msgstr ""
 
 msgid "Disabled Project History & IP Address Recording"
 msgstr ""
 
 msgid "Enabled Project History"
-msgstr "Historial del proyecto activado"
+msgstr ""
 
 msgid "Disabled IP Address Recording"
 msgstr ""
 
 msgid "Enabled Project History & IP Address Recording"
 msgstr ""
 
@@ -524,15 +521,15 @@
 "action cannot be undone."
 msgstr ""
 
 msgid "Confirm deletion"
 msgstr ""
 
 msgid "Close"
-msgstr "Cerrar"
+msgstr ""
 
 msgid "Delete Confirmation"
 msgstr ""
 
 msgid ""
 "Are you sure you want to erase all history for this project? This action "
 "cannot be undone."
@@ -582,31 +579,31 @@
 msgid "No IP Addresses to erase"
 msgstr ""
 
 msgid "Delete Stored IP Addresses"
 msgstr ""
 
 msgid "Time"
-msgstr "Hora"
+msgstr ""
 
 msgid "Event"
-msgstr "Evento"
+msgstr ""
 
 msgid "IP address recording can be enabled on the settings page"
 msgstr ""
 
 msgid "IP address recording can be disabled on the settings page"
 msgstr ""
 
 msgid "From IP"
 msgstr ""
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project %(name)s added"
-msgstr "Nombre del proyecto"
+msgstr ""
 
 #, python-format
 msgid "Bill %(name)s added"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s added"
@@ -643,19 +640,19 @@
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
 msgid "Amount"
-msgstr "Cantidad"
+msgstr ""
 
 #, python-format
 msgid "Amount in %(currency)s"
-msgstr "Cantidad en %(currency)s"
+msgstr ""
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s modified"
@@ -699,85 +696,83 @@
 msgid "Going on holidays with friends?"
 msgstr ""
 
 msgid "Simply sharing money with others?"
 msgstr ""
 
 msgid "We can help!"
-msgstr "Podemos ayudar!"
+msgstr ""
 
 msgid "Log in to an existing project"
-msgstr "Acceder a un proyecto existente"
+msgstr ""
 
 msgid "Log in"
 msgstr ""
 
 msgid "can't remember your password?"
-msgstr "¿no recuerdas tu contraseña?"
+msgstr ""
 
 msgid "Create"
-msgstr "Crear"
+msgstr ""
 
 msgid ""
 "Don\\'t reuse a personal password. Choose a private code and send it to "
 "your friends"
 msgstr ""
-"No reutilizes una contraseña personal. Escoge un código privado i envíalo"
-" a tus amigos"
 
 msgid "Account manager"
 msgstr ""
 
 msgid "Bills"
-msgstr "Facturas"
+msgstr ""
 
 msgid "Settle"
 msgstr ""
 
 msgid "Statistics"
-msgstr "Estadísticas"
+msgstr ""
 
 msgid "Languages"
-msgstr "Idiomas"
+msgstr ""
 
 msgid "Projects"
-msgstr "Proyectos"
+msgstr ""
 
 msgid "Start a new project"
 msgstr ""
 
 msgid "History"
-msgstr "Historia"
+msgstr ""
 
 msgid "Settings"
-msgstr "Ajustes"
+msgstr ""
 
 msgid "Other projects :"
-msgstr "Otros proyectos :"
+msgstr ""
 
 msgid "switch to"
-msgstr "cambiar a"
+msgstr ""
 
 msgid "Dashboard"
 msgstr ""
 
 msgid "Logout"
 msgstr ""
 
 msgid "Code"
-msgstr "Código"
+msgstr ""
 
 msgid "Mobile Application"
-msgstr "Aplicación móvil"
+msgstr ""
 
 msgid "Documentation"
-msgstr "Documentación"
+msgstr ""
 
 msgid "Administation Dashboard"
-msgstr "Panel de administración"
+msgstr ""
 
 msgid "Legal information"
 msgstr ""
 
 msgid "\"I hate money\" is free software"
 msgstr ""
 
@@ -803,15 +798,15 @@
 msgid "Newer bills"
 msgstr ""
 
 msgid "Older bills"
 msgstr ""
 
 msgid "When?"
-msgstr "¿Cuándo?"
+msgstr ""
 
 msgid "Who paid?"
 msgstr ""
 
 msgid "For what?"
 msgstr ""
 
@@ -823,61 +818,61 @@
 msgstr ""
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr ""
 
 msgid "No bills"
-msgstr "Sin facturas"
+msgstr ""
 
 msgid "Nothing to list yet."
-msgstr "No hay nada que mostrar todavía."
+msgstr ""
 
 msgid "You probably want to"
-msgstr "Probablemente quieras"
+msgstr ""
 
 msgid "add a bill"
-msgstr "añadir una factura"
+msgstr ""
 
 msgid "add participants"
-msgstr "añadir participantes"
+msgstr ""
 
 msgid "Password reminder"
 msgstr ""
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
 msgstr ""
 
 msgid "Return to home page"
-msgstr "Volver a la página de inicio"
+msgstr ""
 
 msgid "Your projects"
-msgstr "Tus proyectos"
+msgstr ""
 
 msgid "Reset your password"
-msgstr "Reestablecer tu contraseña"
+msgstr ""
 
 msgid "Invite people to join this project"
 msgstr ""
 
 msgid "Share Identifier & code"
-msgstr "Compartir identificador i código"
+msgstr ""
 
 msgid ""
 "You can share the project identifier and the private code by any "
 "communication means."
 msgstr ""
 
 msgid "Identifier:"
-msgstr "Identificador:"
+msgstr ""
 
 msgid "Share the Link"
-msgstr "Compartir el enlace"
+msgstr ""
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 
 msgid "Send via Emails"
 msgstr ""
 
@@ -888,137 +883,32 @@
 "send them an email for you."
 msgstr ""
 
 msgid "Who pays?"
 msgstr ""
 
 msgid "To whom?"
-msgstr "¿Para quién?"
+msgstr ""
 
 msgid "Who?"
-msgstr "¿Quién?"
+msgstr ""
 
 msgid "Balance"
 msgstr ""
 
 msgid "deactivate"
-msgstr "desactivar"
+msgstr ""
 
 msgid "reactivate"
-msgstr "reactivar"
+msgstr ""
 
 msgid "Paid"
-msgstr "Pagado"
+msgstr ""
 
 msgid "Spent"
-msgstr "Gastado"
+msgstr ""
 
 msgid "Expenses by Month"
-msgstr "Gastos por mes"
+msgstr ""
 
 msgid "Period"
-msgstr "Período"
-
-#~ msgid "Participant"
-#~ msgstr "Participante"
-
-#~ msgid "Bill"
-#~ msgstr "Factura"
-
-#~ msgid "Select all"
-#~ msgstr "Seleccionar todo"
-
-#~ msgid "Select none"
-#~ msgstr ""
-
-#~ msgid "changed"
-#~ msgstr ""
-
-#~ msgid "from"
-#~ msgstr "de"
-
-#~ msgid "to"
-#~ msgstr "para"
-
-#~ msgid "Confirm Delete"
-#~ msgstr ""
-
-#~ msgid "Added"
-#~ msgstr "Añadido"
-
-#~ msgid "Removed"
-#~ msgstr "Eliminado"
-
-#~ msgid "and"
-#~ msgstr ""
-
-#~ msgid "owers list"
-#~ msgstr ""
-
-#~ msgid "added"
-#~ msgstr "añadido"
-
-#~ msgid "Project renamed to"
-#~ msgstr ""
-
-#~ msgid "Project contact email changed to"
-#~ msgstr ""
-
-#~ msgid "deactivated"
-#~ msgstr ""
-
-#~ msgid "reactivated"
-#~ msgstr ""
-
-#~ msgid "renamed to"
-#~ msgstr ""
-
-#~ msgid "External link changed to"
-#~ msgstr ""
-
-#~ msgid "modified"
-#~ msgstr "modificado"
-
-#~ msgid "removed"
-#~ msgstr "eliminado"
-
-#~ msgid "changed in a unknown way"
-#~ msgstr ""
-
-#~ msgid "You either provided a bad token or no project identifier."
-#~ msgstr ""
-
-#~ msgid "User name incorrect"
-#~ msgstr "Usuario incorrecto"
-
-#~ msgid "This project already have this member"
-#~ msgstr ""
-
-#~ msgid "People to notify"
-#~ msgstr ""
-
-#~ msgid "Error activating member"
-#~ msgstr ""
-
-#~ msgid "Error removing member"
-#~ msgstr ""
-
-#~ msgid ""
-#~ "User '%(name)s' has been deactivated. It"
-#~ " will still appear in the users "
-#~ "list until its balance becomes zero."
-#~ msgstr ""
-
-#~ msgid "User '%(name)s' has been removed"
-#~ msgstr ""
-
-#~ msgid "User '%(name)s' has been edited"
-#~ msgstr ""
-
-#~ msgid "Number of members"
-#~ msgstr ""
-
-#~ msgid "Edit this member"
-#~ msgstr "Editar miembro"
-
-#~ msgid "Participants to notify"
-#~ msgstr "añadir participantes"
+msgstr ""
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/es_419/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/es_419/LC_MESSAGES/messages.mo`

 * *Files 23% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,21 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
+"Project-Id-Version: Spanish (Latin America) (I Hate Money)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2020-11-11 16:28+0000\n"
-"Last-Translator: Puyma <puyma@amyup.xyz>\n"
-"Language: es_419\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: Spanish (Latin America) <https://hosted.weblate.org/projects/"
 "i-hate-money/i-hate-money/es_419/>\n"
-"Plural-Forms: nplurals=2; plural=n != 1\n"
+"Language: es_419\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
+"Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.12-dev\n"
 
 msgid ""
 "\n"
 "            <i>The table below reflects actions recorded prior to disabling "
 "project history. You can\n"
 "            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
 "target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
@@ -43,14 +42,17 @@
 "i> \n"
 "            <a href=\"%(url)s\">en la página de ajustes</a>\n"
 "            "
 
 msgid "\"I hate money\" is free software"
 msgstr "\"I hate money\" es un software libre"
 
+msgid "%(amount)s each"
+msgstr "%(amount)s cada uno"
+
 msgid "%(member)s has been added"
 msgstr "Se añadieron %(member)s"
 
 msgid "%(name)s is part of this project again"
 msgstr "%(name)s es parte de este nuevo proyecto"
 
 msgid "?"
@@ -102,15 +104,18 @@
 msgid "Administation Dashboard"
 msgstr "Panel de administración"
 
 msgid "Administration tasks are currently disabled."
 msgstr "Las tareas de administración están actualmente deshabilitadas."
 
 msgid "Amount"
-msgstr "Monto"
+msgstr "Cantidad"
+
+msgid "Amount in %(currency)s"
+msgstr "Cantidad en %(currency)s"
 
 msgid "Amount paid"
 msgstr "Cantidad pagada"
 
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
@@ -125,20 +130,54 @@
 msgid ""
 "Are you sure you want to erase all history for this project? This action "
 "cannot be undone."
 msgstr ""
 "Por favor confirme la eliminación completa del historial del proyecto. Esta "
 "acción es irreversible."
 
+msgid "Are you sure?"
+msgstr "¿Estás segura?"
+
+msgid "Authentication"
+msgstr "Autenticación"
+
 msgid "Back to the list"
 msgstr "Volver a la lista"
 
 msgid "Balance"
 msgstr "Balance"
 
+msgid "Bill %(name)s added"
+msgstr "La factura %(name)s ha sido agregada"
+
+msgid "Bill %(name)s changed in an unknown way"
+msgstr "Factura %(name)s se cambió de manera desconocida"
+
+msgid "Bill %(name)s modified"
+msgstr "La factura %(name)s ha sido modificada"
+
+msgid "Bill %(name)s removed"
+msgstr "Factura %(name)s removida"
+
+msgid "Bill %(name)s renamed to %(new_description)s"
+msgstr "Factura %(name)s renombrada a %(new_description)s"
+
+msgid "Bill %(name)s: %(property_name)s changed from %(before)s to %(after)s"
+msgstr ""
+"Factura %(name)s: %(property_name)s ha cambiado de %(before)s a %(after)s"
+
+msgid "Bill %(name)s: %(property_name)s changed to %(after)s"
+msgstr "Factura %(name)s:%(property_name)s ha cambiado a %(after)s"
+
+msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
+msgstr "Factura%(name)s: añadida %(owers_list_str)s a la lista de dueños"
+
+msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
+msgstr "Factura %(name)s: removida %(owers_list_str)s de la lista de dueños"
+
 msgid "Bill items"
 msgstr "Elementos de factura"
 
 msgid "Bills"
 msgstr "Facturas"
 
 msgid "Bills can't be null"
@@ -146,14 +185,20 @@
 
 msgid "Can't remember the password?"
 msgstr "¿No recuerdas la contraseña?"
 
 msgid "Cancel"
 msgstr "Cancelar"
 
+msgid ""
+"Cannot add bills in multiple currencies to a project without default currency"
+msgstr ""
+"No se pueden agregar facturas en varias monedas a un proyecto sin la moneda "
+"predeterminada"
+
 msgid "Choose file"
 msgstr "Escoger un archivo"
 
 msgid "Clear Project History"
 msgstr "Borrar el historial del proyecto"
 
 msgid "Close"
@@ -161,14 +206,17 @@
 
 msgid "Code"
 msgstr "Código"
 
 msgid "Confirm Remove IP Adresses"
 msgstr "Confirmar eliminación de direcciones IP"
 
+msgid "Confirm deletion"
+msgstr "Confirmar la eliminación"
+
 msgid "Create"
 msgstr "Crear"
 
 msgid "Create a new project"
 msgstr "Crear un nuevo proyecto"
 
 msgid "Create the project"
@@ -188,32 +236,51 @@
 
 msgid "Delete Confirmation"
 msgstr "Confirmación de eliminación"
 
 msgid "Delete Stored IP Addresses"
 msgstr "Borrar direcciones IP registradas"
 
+msgid "Delete project"
+msgstr "Borrar proyecto"
+
 msgid "Delete stored IP addresses"
 msgstr "Borrar las direcciones IP registradas"
 
+msgid "Deleted project history."
+msgstr "Historial del proyecto eliminada."
+
+msgid "Deleted recorded IP addresses in project history."
+msgstr "Direcciones IP eliminadas en el historial del proyecto."
+
 msgid "Disabled IP Address Recording"
 msgstr "Registro de direcciones IP activo"
 
 msgid "Disabled Project History"
 msgstr "Historial de proyecto activo"
 
 msgid "Disabled Project History & IP Address Recording"
 msgstr "Historial de proyecto y registros de dirección IP inactivos"
 
 msgid "Documentation"
 msgstr "Documentación"
 
+msgid ""
+"Don\\'t reuse a personal password. Choose a private code and send it to your "
+"friends"
+msgstr ""
+"No reutilice una contraseña personal. Elija un código privado y envíelo a "
+"sus amigos"
+
 msgid "Download"
 msgstr "Descargar"
 
+msgid "Download Mobile Application"
+msgstr "Instalar aplicación móvil"
+
 msgid "Download project's data"
 msgstr "Descargar datos del proyecto"
 
 msgid "Download the list of bills with owner, amount, reason,... "
 msgstr ""
 "Descargue la lista de facturas con el propietario, importe, motivo,... "
 
@@ -227,14 +294,17 @@
 
 msgid "Edit the project"
 msgstr "Editar el proyecto"
 
 msgid "Edit this bill"
 msgstr "Editar esta factura"
 
+msgid "Edit this participant"
+msgstr "Editar este participante"
+
 msgid "Email"
 msgstr "Correo Electrónico"
 
 msgid "Enable project history"
 msgstr "Habilitar historial del proyecto"
 
 msgid "Enabled IP Address Recording"
@@ -242,19 +312,43 @@
 
 msgid "Enabled Project History"
 msgstr "Historial de proyecto activo"
 
 msgid "Enabled Project History & IP Address Recording"
 msgstr "Historial de proyecto y registros de dirección IP activos"
 
+msgid "Enter a new code if you want to change it"
+msgstr "Entra un nuevo código si tu quieres cambiarlo"
+
+msgid "Enter private code to confirm deletion"
+msgstr "Introduzca el código privado para confirmar la eliminación"
+
+msgid "Error activating participant"
+msgstr "Error activando participante"
+
+msgid "Error deleting bill"
+msgstr "Error eliminando factura"
+
+msgid "Error deleting project"
+msgstr "Error al borrar poryecto"
+
+msgid "Error deleting project history"
+msgstr "Error al eliminar el historial del proyecto"
+
+msgid "Error deleting recorded IP addresses"
+msgstr "Error al eliminar direcciones IP registradas"
+
+msgid "Error removing participant"
+msgstr "Error eliminando participante"
+
 msgid "Event"
 msgstr "Evento"
 
 msgid "Everyone"
-msgstr "Todo el mundo"
+msgstr "Todos"
 
 msgid "Everyone but %(excluded)s"
 msgstr "Todo el mundo menos %(excluded)s"
 
 msgid "Expenses by Month"
 msgstr "Gastos por mes"
 
@@ -269,14 +363,17 @@
 
 msgid "From IP"
 msgstr "IP de origen"
 
 msgid "Get in"
 msgstr "Entrar"
 
+msgid "Get it on"
+msgstr "Conseguir en"
+
 msgid "Going on holidays with friends?"
 msgstr "¿Te vas de vacaciones con amigos?"
 
 msgid "History"
 msgstr "Historial"
 
 msgid "History Settings Changed"
@@ -303,26 +400,32 @@
 
 msgid "Import previously exported JSON file"
 msgstr "Importar archivo JSON previamente exportado"
 
 msgid "Invalid JSON"
 msgstr "JSON inválido"
 
+msgid "Invalid private code."
+msgstr "Código privado inválido."
+
 msgid "Invalid token"
 msgstr "Token no válido"
 
 msgid "Invite people"
 msgstr "Invitar personas"
 
 msgid "Invite people to join this project"
 msgstr "Invita a personas a unirse a este proyecto"
 
 msgid "Languages"
 msgstr "Idiomas"
 
+msgid "Legal information"
+msgstr "Información legal"
+
 msgid "Log in"
 msgstr "Inicia sesión"
 
 msgid "Log in to an existing project"
 msgstr "Iniciar sesión en un proyecto existente"
 
 msgid "Logout"
@@ -330,17 +433,23 @@
 
 msgid "Manage your shared <br />expenses, easily"
 msgstr "Gestione sus gastos compartidos <br />fácilmente"
 
 msgid "Mobile Application"
 msgstr "Aplicación móvil"
 
+msgid "More options"
+msgstr "Más opciones"
+
 msgid "Name"
 msgstr "Nombre"
 
+msgid "New private code"
+msgstr "Nuevo código privado"
+
 msgid "Newer bills"
 msgstr "Nuevas facturas"
 
 msgid "Newest bill"
 msgstr "Factura más reciente"
 
 msgid "No Currency"
@@ -351,14 +460,17 @@
 
 msgid "No bills"
 msgstr "Sin facturas"
 
 msgid "No history to erase"
 msgstr "No hay historial para borrar"
 
+msgid "No one"
+msgstr "Ninguno"
+
 msgid "No token provided"
 msgstr "No se proporciono ningún token"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
@@ -370,26 +482,68 @@
 
 msgid "Nothing to list yet."
 msgstr "Aún no hay nada que listar."
 
 msgid "Number of bills"
 msgstr "Número de facturas"
 
+msgid "Number of participants"
+msgstr "Número de participantes"
+
 msgid "Older bills"
 msgstr "Facturas anteriores"
 
 msgid "Oldest bill"
 msgstr "Factura más antigua"
 
 msgid "Other projects :"
 msgstr "Otros proyectos :"
 
 msgid "Paid"
 msgstr "Pagado"
 
+msgid "Participant %(name)s added"
+msgstr "Participante %(name)s añadido"
+
+msgid "Participant %(name)s changed in an unknown way"
+msgstr "Participante %(name)s se cambió de manera desconocida"
+
+msgid "Participant %(name)s deactivated"
+msgstr "Participante %(name)s desactivad@"
+
+msgid "Participant %(name)s modified"
+msgstr "Participante %(name)s modificad@"
+
+msgid "Participant %(name)s reactivated"
+msgstr "Participante %(name)s reactivad@"
+
+msgid "Participant %(name)s removed"
+msgstr "Participante %(name)s removid@"
+
+msgid "Participant %(name)s renamed to %(new_name)s"
+msgstr "Participante %(name)s se ha renombrado a %(new_name)s"
+
+msgid ""
+"Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
+msgstr ""
+"Participante %(name)s: peso cambiado de %(old_weight)s a %(new_weight)s"
+
+msgid ""
+"Participant '%(name)s' has been deactivated. It will still appear in the "
+"list until its balance reach zero."
+msgstr ""
+"El participante '%(name)s' ha sido desactivado. Seguirá apareciendo en la "
+"lista hasta que su saldo llegue a cero."
+
+msgid "Participant '%(name)s' has been modified"
+msgstr "El participante '%(name)s' ha sido modificado"
+
+msgid "Participant '%(name)s' has been removed"
+msgstr "Se ha eliminado al participante '%(name)s'"
+
 msgid "Password"
 msgstr "Contraseña"
 
 msgid "Password confirmation"
 msgstr "Confirmar contraseña"
 
 msgid "Password mismatch"
@@ -400,50 +554,71 @@
 
 msgid "Password successfully reset."
 msgstr "Contraseña restablecida con éxito."
 
 msgid "Payer"
 msgstr "Paga"
 
+msgid "People to notify"
+msgstr "Personas para notificar"
+
 msgid "Period"
 msgstr "Período"
 
+msgid "Please, validate the captcha to proceed."
+msgstr "Por favor, completa el captcha para seguir."
+
 msgid "Privacy Settings"
 msgstr "Ajustes de privacidad"
 
 msgid "Private code"
 msgstr "Código privado"
 
 msgid "Project"
 msgstr "Proyecto"
 
+msgid "Project %(name)s added"
+msgstr "Proyecto %(name)s añadido"
+
+msgid "Project %(name)s changed in an unknown way"
+msgstr "Proyecto %(name)s se cambió de manera desconocida"
+
+msgid "Project contact email changed to %(new_email)s"
+msgstr "Correo electrónico del proyecto se ha cambiado a %(new_email)s"
+
 msgid "Project default: %(currency)s"
 msgstr "moneda predeterminada del projecto: %(currency)s"
 
 msgid "Project identifier"
 msgstr "Identificador de proyecto"
 
 msgid "Project name"
 msgstr "Nombre del Proyecto"
 
 msgid "Project private code changed"
 msgstr "Se cambió el código privado del proyecto"
 
+msgid "Project renamed to %(new_project_name)s"
+msgstr "Proyecto renombrado a %(new_project_name)s"
+
 msgid "Project settings modified"
 msgstr "Ajustes del proyecto modificados"
 
 msgid "Project successfully deleted"
 msgstr "Proyecto eliminado correctamente"
 
 msgid "Project successfully uploaded"
 msgstr "El proyecto se subió exitosamente"
 
 msgid "Projects"
 msgstr "Proyectos"
 
+msgid "Provided token is invalid"
+msgstr "La muestra proporcionada no es válida"
+
 msgid "Reset password"
 msgstr "Restablecer contraseña"
 
 msgid "Reset your password"
 msgstr "Restablecer su contraseña"
 
 msgid "Return to home page"
@@ -457,14 +632,19 @@
 
 msgid "Send the invitations"
 msgstr "Enviar las invitaciones"
 
 msgid "Send via Emails"
 msgstr "Enviar por correo electrónico"
 
+msgid "Setting a default currency enables currency conversion between bills"
+msgstr ""
+"Establecer una moneda predeterminada permite la conversión de divisas entre "
+"facturas"
+
 msgid "Settings"
 msgstr "Configuración"
 
 msgid "Settle"
 msgstr "Resolver"
 
 msgid "Settle plans"
@@ -490,17 +670,18 @@
 msgstr "Es probable que alguien borrara el historial del proyecto."
 
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
 "instructions. Please check the email configuration of the server or contact "
 "the administrator."
 msgstr ""
-"Lo sentimos, se produjo un error durante el envío del email con las "
-"instrucciones de restablecimiento de contraseña. Por favor verifica la "
-"configuración del servidor o contacta el administrador"
+"Lo sentimos, hubo un error al enviarle un correo electrónico con las "
+"instrucciones de restablecimiento de contraseña. Compruebe la configuración "
+"de correo electrónico del servidor o póngase en contacto con el "
+"administrador."
 
 msgid ""
 "Sorry, there was an error while trying to send the invitation emails. Please "
 "check the email configuration of the server or contact the administrator."
 msgstr ""
 "Lo sentimos, hubo un error cuando intentamos enviarle correos de invitación. "
 "Por favor, revise la configuración de correo en el servidor o contactese con "
@@ -549,45 +730,64 @@
 
 msgid "The bill has been modified"
 msgstr "La factura ha sido modificada"
 
 msgid "The email %(email)s is not valid"
 msgstr "El correo electrónico %(email)s no es válido"
 
+msgid "The participant name is invalid"
+msgstr "El nombre del participante no es válido"
+
 msgid "The project identifier is %(project)s"
 msgstr "El identificador del proyecto es %(project)s"
 
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "El proyecto al que intentas acceder no existe, ¿quieres"
 
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "Esta contraseña de administrador no es la correcta. Solo quedan %(num)d "
 "intentos."
 
 msgid "This private code is not the right one"
 msgstr "Este código privado no es el correcto"
 
+msgid "This project already have this participant"
+msgstr "Este proyecto ya tiene a este participante"
+
+msgid ""
+"This project cannot be set to 'no currency' because it contains bills in "
+"multiple currencies."
+msgstr ""
+"Este proyecto no se puede establecer en 'ninguna moneda' porque contiene "
+"facturas en varias monedas."
+
 msgid "This project does not exists"
 msgstr "Este proyecto no existe"
 
+msgid "This will remove all bills and participants in this project!"
+msgstr "Esto va a remover todas las facturas y participantes en este proyecto!"
+
 msgid "Time"
 msgstr "Hora"
 
 msgid "To whom?"
 msgstr "¿A quién?"
 
 msgid "Too many failed login attempts, please retry later."
 msgstr ""
 "Demasiados intentos fallidos de inicio de sesión, vuelva a intentarlo más "
 "tarde."
 
 msgid "Try out the demo"
 msgstr "Prueba la demo"
 
+msgid "Unknown error"
+msgstr "Error desconocido"
+
 msgid "Unknown project"
 msgstr "Proyecto desconocido"
 
 msgid "Use IP tracking for project history"
 msgstr "Registrar la IPs para el historial del proyecto"
 
 msgid "We can help!"
@@ -608,14 +808,17 @@
 
 msgid "What?"
 msgstr "¿Qué?"
 
 msgid "When?"
 msgstr "¿Cuando?"
 
+msgid "Which is a real currency: Euro or Petro dollar?"
+msgstr "¿Cuál es una moneda real: euro o petro dólar?"
+
 msgid "Who paid?"
 msgstr "¿Quién pagó?"
 
 msgid "Who pays?"
 msgstr "¿Quién paga?"
 
 msgid "Who?"
@@ -671,21 +874,45 @@
 
 msgid "delete"
 msgstr "Eliminar"
 
 msgid "edit"
 msgstr "Editar"
 
+msgid "euro"
+msgstr "Euro"
+
 msgid "john.doe@example.com, mary.moe@site.com"
-msgstr "juan.perez@example.com, ana.rodriguez@site.com"
+msgstr "john.doe@example.com, mary.moe@site.com"
 
 msgid "reactivate"
 msgstr "Reactivar"
 
+msgid "show"
+msgstr "enseñar"
+
 msgid "switch to"
 msgstr "cambiar a"
 
 msgid "you can contribute and improve it!"
 msgstr "puedes contribuir y mejorarlo!"
 
 msgid "you sure?"
 msgstr "¿Estás seguro?"
+
+msgid "{dual_object_0} and {dual_object_1}"
+msgstr "{dual_object_0} y {dual_object_1}"
+
+msgid "{prefix}: {error}"
+msgstr "{prefijo}: {error}"
+
+msgid "{prefix}:<br />{errors}"
+msgstr "{prefijo}:<br />{errores}"
+
+msgid "{previous_object}, and {end_object}"
+msgstr "{previous_object}, y {end_object}"
+
+msgid "{previous_object}, {next_object}"
+msgstr "{previous_object}, {next_object}"
+
+msgid "{start_object}, {next_object}"
+msgstr "{start_object}, {next_object}"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/es_419/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/es_419/LC_MESSAGES/messages.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2020-11-11 16:28+0000\n"
-"Last-Translator: Puyma <puyma@amyup.xyz>\n"
+"PO-Revision-Date: 2022-04-11 17:12+0000\n"
+"Last-Translator: Santiago José Gutiérrez Llanos <gutierrezapata17@gmail.com>"
+"\n"
+"Language-Team: Spanish (Latin America) <https://hosted.weblate.org/projects/"
+"i-hate-money/i-hate-money/es_419/>\n"
 "Language: es_419\n"
-"Language-Team: Spanish (Latin America) "
-"<https://hosted.weblate.org/projects/i-hate-money/i-hate-money/es_419/>\n"
-"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.12-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "No es una cantidad o expresión válida. Solo se aceptan números y los "
 "operadores + - * /."
 
 msgid "Project name"
 msgstr "Nombre del Proyecto"
 
-#, fuzzy
 msgid "New private code"
-msgstr "Código privado"
+msgstr "Nuevo código privado"
 
 msgid "Enter a new code if you want to change it"
-msgstr ""
+msgstr "Entra un nuevo código si tu quieres cambiarlo"
 
 msgid "Email"
 msgstr "Correo Electrónico"
 
 msgid "Enable project history"
 msgstr "Habilitar historial del proyecto"
 
@@ -42,19 +42,23 @@
 msgstr "Registrar la IPs para el historial del proyecto"
 
 msgid "Default Currency"
 msgstr "Moneda por defecto"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
+"Establecer una moneda predeterminada permite la conversión de divisas entre "
+"facturas"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
+"Este proyecto no se puede establecer en 'ninguna moneda' porque contiene "
+"facturas en varias monedas."
 
 msgid "Import previously exported JSON file"
 msgstr "Importar archivo JSON previamente exportado"
 
 msgid "Import"
 msgstr "Importar"
 
@@ -72,33 +76,30 @@
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
 msgstr ""
 "Ya existe un proyecto con este identificador (\"%(project)s\"). Por "
 "favor, elija un nuevo identificador"
 
 msgid "Which is a real currency: Euro or Petro dollar?"
-msgstr ""
+msgstr "¿Cuál es una moneda real: euro o petro dólar?"
 
-#, fuzzy
 msgid "euro"
-msgstr "Período"
+msgstr "Euro"
 
 msgid "Please, validate the captcha to proceed."
-msgstr ""
+msgstr "Por favor, completa el captcha para seguir."
 
 msgid "Enter private code to confirm deletion"
-msgstr ""
+msgstr "Introduzca el código privado para confirmar la eliminación"
 
-#, fuzzy
 msgid "Unknown error"
-msgstr "Proyecto desconocido"
+msgstr "Error desconocido"
 
-#, fuzzy
 msgid "Invalid private code."
-msgstr "Código privado"
+msgstr "Código privado inválido."
 
 msgid "Get in"
 msgstr "Entrar"
 
 msgid "Admin password"
 msgstr "Contraseña de Administrador"
 
@@ -165,72 +166,70 @@
 
 msgid "Weight"
 msgstr "Peso"
 
 msgid "Add"
 msgstr "Agregar"
 
-#, fuzzy
 msgid "The participant name is invalid"
-msgstr "Se ha eliminado al usuario '%(name)s'"
+msgstr "El nombre del participante no es válido"
 
-#, fuzzy
 msgid "This project already have this participant"
-msgstr "Este proyecto ya tiene a este miembro"
+msgstr "Este proyecto ya tiene a este participante"
 
 msgid "People to notify"
-msgstr ""
+msgstr "Personas para notificar"
 
 msgid "Send invites"
 msgstr "Enviar invitaciones"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "El correo electrónico %(email)s no es válido"
 
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
-msgstr ""
+msgstr "{dual_object_0} y {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
-msgstr ""
+msgstr "{previous_object}, y {end_object}"
 
 #. Two items in a middle of a list with more than 5 objects
 msgid "{previous_object}, {next_object}"
-msgstr ""
+msgstr "{previous_object}, {next_object}"
 
 #. First two items of a list with more than 3 items
 msgid "{start_object}, {next_object}"
-msgstr ""
+msgstr "{start_object}, {next_object}"
 
 msgid "No Currency"
 msgstr "no moneda"
 
 #. Form error with only one error
 msgid "{prefix}: {error}"
-msgstr ""
+msgstr "{prefijo}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
-msgstr ""
+msgstr "{prefijo}:<br />{errores}"
 
 msgid "Too many failed login attempts, please retry later."
 msgstr ""
 "Demasiados intentos fallidos de inicio de sesión, vuelva a intentarlo más"
 " tarde."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "Esta contraseña de administrador no es la correcta. Solo quedan %(num)d "
 "intentos."
 
 msgid "Provided token is invalid"
-msgstr ""
+msgstr "La muestra proporcionada no es válida"
 
 msgid "This private code is not the right one"
 msgstr "Este código privado no es el correcto"
 
 #, python-format
 msgid "You have just created '%(project)s' to share your expenses"
 msgstr "Acabas de crear '%(project)s' para compartir tus gastos"
@@ -250,17 +249,18 @@
 msgstr "El identificador del proyecto es %(project)s"
 
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
 "instructions. Please check the email configuration of the server or "
 "contact the administrator."
 msgstr ""
-"Lo sentimos, se produjo un error durante el envío del email con las "
-"instrucciones de restablecimiento de contraseña. Por favor verifica la "
-"configuración del servidor o contacta el administrador"
+"Lo sentimos, hubo un error al enviarle un correo electrónico con las "
+"instrucciones de restablecimiento de contraseña. Compruebe la configuración "
+"de correo electrónico del servidor o póngase en contacto con el "
+"administrador."
 
 msgid "No token provided"
 msgstr "No se proporciono ningún token"
 
 msgid "Invalid token"
 msgstr "Token no válido"
 
@@ -276,20 +276,22 @@
 msgid "Invalid JSON"
 msgstr "JSON inválido"
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
+"No se pueden agregar facturas en varias monedas a un proyecto sin la moneda "
+"predeterminada"
 
 msgid "Project successfully deleted"
 msgstr "Proyecto eliminado correctamente"
 
 msgid "Error deleting project"
-msgstr ""
+msgstr "Error al borrar poryecto"
 
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "Usted ha sido invitado a compartir sus gastos para %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "Sus invitaciones han sido enviadas"
@@ -304,81 +306,77 @@
 " contactese con el administrador."
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr "Se añadieron %(member)s"
 
 msgid "Error activating participant"
-msgstr ""
+msgstr "Error activando participante"
 
 #, python-format
 msgid "%(name)s is part of this project again"
 msgstr "%(name)s es parte de este nuevo proyecto"
 
 msgid "Error removing participant"
-msgstr ""
+msgstr "Error eliminando participante"
 
-#, fuzzy, python-format
+#, python-format
 msgid ""
 "Participant '%(name)s' has been deactivated. It will still appear in the "
 "list until its balance reach zero."
 msgstr ""
-"El usuario '%(name)s' ha sido desactivado. Seguirá apareciendo en la "
-"lista de usuarios hasta que su saldo sea cero."
+"El participante '%(name)s' ha sido desactivado. Seguirá apareciendo en la "
+"lista hasta que su saldo llegue a cero."
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant '%(name)s' has been removed"
-msgstr "Se ha eliminado al usuario '%(name)s'"
+msgstr "Se ha eliminado al participante '%(name)s'"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant '%(name)s' has been modified"
-msgstr "Se ha eliminado al usuario '%(name)s'"
+msgstr "El participante '%(name)s' ha sido modificado"
 
 msgid "The bill has been added"
 msgstr "La factura ha sido agregada"
 
 msgid "Error deleting bill"
-msgstr ""
+msgstr "Error eliminando factura"
 
 msgid "The bill has been deleted"
 msgstr "La factura ha sido eliminada"
 
 msgid "The bill has been modified"
 msgstr "La factura ha sido modificada"
 
-#, fuzzy
 msgid "Error deleting project history"
-msgstr "Habilitar historial del proyecto"
+msgstr "Error al eliminar el historial del proyecto"
 
-#, fuzzy
 msgid "Deleted project history."
-msgstr "Habilitar historial del proyecto"
+msgstr "Historial del proyecto eliminada."
 
-#, fuzzy
 msgid "Error deleting recorded IP addresses"
-msgstr "Borrar las direcciones IP registradas"
+msgstr "Error al eliminar direcciones IP registradas"
 
 msgid "Deleted recorded IP addresses in project history."
-msgstr ""
+msgstr "Direcciones IP eliminadas en el historial del proyecto."
 
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "Lo sentimos, no hemos encontrado la página que has solicitado."
 
 msgid "The best thing to do is probably to get back to the main page."
 msgstr "Lo mejor que puede hacer es volver a la página principal."
 
 msgid "Back to the list"
 msgstr "Volver a la lista"
 
 msgid "Administration tasks are currently disabled."
 msgstr "Las tareas de administración están actualmente deshabilitadas."
 
-#, fuzzy
 msgid "Authentication"
-msgstr "Documentación"
+msgstr "Autenticación"
 
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "El proyecto al que intentas acceder no existe, ¿quieres"
 
 msgid "create it"
 msgstr "crearlo"
 
@@ -387,17 +385,16 @@
 
 msgid "Create a new project"
 msgstr "Crear un nuevo proyecto"
 
 msgid "Project"
 msgstr "Proyecto"
 
-#, fuzzy
 msgid "Number of participants"
-msgstr "agregar participantes"
+msgstr "Número de participantes"
 
 msgid "Number of bills"
 msgstr "Número de facturas"
 
 msgid "Newest bill"
 msgstr "Factura más reciente"
 
@@ -410,37 +407,33 @@
 msgid "edit"
 msgstr "Editar"
 
 msgid "delete"
 msgstr "Eliminar"
 
 msgid "show"
-msgstr ""
+msgstr "enseñar"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "El panel está desactivado actualmente."
 
-#, fuzzy
 msgid "Download Mobile Application"
-msgstr "Aplicación móvil"
+msgstr "Instalar aplicación móvil"
 
-#, fuzzy
 msgid "Get it on"
-msgstr "Entrar"
+msgstr "Conseguir en"
 
-#, fuzzy
 msgid "Are you sure?"
-msgstr "¿Estás seguro?"
+msgstr "¿Estás segura?"
 
 msgid "Edit project"
 msgstr "Editar proyecto"
 
-#, fuzzy
 msgid "Delete project"
-msgstr "Editar proyecto"
+msgstr "Borrar proyecto"
 
 msgid "Import JSON"
 msgstr "Importar JSON"
 
 msgid "Choose file"
 msgstr "Escoger un archivo"
 
@@ -470,40 +463,39 @@
 msgid "Privacy Settings"
 msgstr "Ajustes de privacidad"
 
 msgid "Edit the project"
 msgstr "Editar el proyecto"
 
 msgid "This will remove all bills and participants in this project!"
-msgstr ""
+msgstr "Esto va a remover todas las facturas y participantes en este proyecto!"
 
 msgid "Edit this bill"
 msgstr "Editar esta factura"
 
 msgid "Add a bill"
 msgstr "Agregar una factura"
 
 msgid "Everyone"
-msgstr "Todo el mundo"
+msgstr "Todos"
 
 msgid "No one"
-msgstr ""
+msgstr "Ninguno"
 
 msgid "More options"
-msgstr ""
+msgstr "Más opciones"
 
 msgid "Add participant"
 msgstr "Añadir participante"
 
-#, fuzzy
 msgid "Edit this participant"
-msgstr "Añadir participante"
+msgstr "Editar este participante"
 
 msgid "john.doe@example.com, mary.moe@site.com"
-msgstr "juan.perez@example.com, ana.rodriguez@site.com"
+msgstr "john.doe@example.com, mary.moe@site.com"
 
 msgid "Send the invitations"
 msgstr "Enviar las invitaciones"
 
 msgid "Download"
 msgstr "Descargar"
 
@@ -527,18 +519,19 @@
 
 msgid "History Settings Changed"
 msgstr "Se cambiaron los ajustes del historial"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed from %(before)s to %(after)s"
 msgstr ""
+"Factura %(name)s: %(property_name)s ha cambiado de %(before)s a %(after)s"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed to %(after)s"
-msgstr ""
+msgstr "Factura %(name)s:%(property_name)s ha cambiado a %(after)s"
 
 msgid "Confirm Remove IP Adresses"
 msgstr "Confirmar eliminación de direcciones IP"
 
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
@@ -546,17 +539,16 @@
 "action cannot be undone."
 msgstr ""
 "Por favor confirme la eliminación completa del registro de direcciones IP"
 " del proyecto.\n"
 "                El resto de historial del proyecto no será afectado. Este"
 " cambio es irreversible."
 
-#, fuzzy
 msgid "Confirm deletion"
-msgstr "Confirmar eliminación"
+msgstr "Confirmar la eliminación"
 
 msgid "Close"
 msgstr "Cerrar"
 
 msgid "Delete Confirmation"
 msgstr "Confirmación de eliminación"
 
@@ -565,19 +557,19 @@
 "cannot be undone."
 msgstr ""
 "Por favor confirme la eliminación completa del historial del proyecto. "
 "Esta acción es irreversible."
 
 #, python-format
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
-msgstr ""
+msgstr "Factura%(name)s: añadida %(owers_list_str)s a la lista de dueños"
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
-msgstr ""
+msgstr "Factura %(name)s: removida %(owers_list_str)s de la lista de dueños"
 
 #, python-format
 msgid ""
 "\n"
 "            <i>This project has history disabled. New actions won't "
 "appear below. You can enable history on the</i>\n"
 "            <a href=\"%(url)s\">settings page</a>\n"
@@ -640,94 +632,94 @@
 
 msgid "IP address recording can be disabled on the settings page"
 msgstr "El registro de direcciones IP se puede desactivar en la página de ajustes"
 
 msgid "From IP"
 msgstr "IP de origen"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project %(name)s added"
-msgstr "Nombre del Proyecto"
+msgstr "Proyecto %(name)s añadido"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s added"
-msgstr "La factura ha sido agregada"
+msgstr "La factura %(name)s ha sido agregada"
 
 #, python-format
 msgid "Participant %(name)s added"
-msgstr ""
+msgstr "Participante %(name)s añadido"
 
 msgid "Project private code changed"
 msgstr "Se cambió el código privado del proyecto"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project renamed to %(new_project_name)s"
-msgstr "El identificador del proyecto es %(new_project_name)s"
+msgstr "Proyecto renombrado a %(new_project_name)s"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project contact email changed to %(new_email)s"
-msgstr "Se cambió el correo electrónico de contacto a"
+msgstr "Correo electrónico del proyecto se ha cambiado a %(new_email)s"
 
 msgid "Project settings modified"
 msgstr "Ajustes del proyecto modificados"
 
 #, python-format
 msgid "Participant %(name)s deactivated"
-msgstr ""
+msgstr "Participante %(name)s desactivad@"
 
 #, python-format
 msgid "Participant %(name)s reactivated"
-msgstr ""
+msgstr "Participante %(name)s reactivad@"
 
 #, python-format
 msgid "Participant %(name)s renamed to %(new_name)s"
-msgstr ""
+msgstr "Participante %(name)s se ha renombrado a %(new_name)s"
 
 #, python-format
 msgid "Bill %(name)s renamed to %(new_description)s"
-msgstr ""
+msgstr "Factura %(name)s renombrada a %(new_description)s"
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
-msgstr ""
+msgstr "Participante %(name)s: peso cambiado de %(old_weight)s a %(new_weight)s"
 
 msgid "Amount"
-msgstr "Monto"
+msgstr "Cantidad"
 
 #, python-format
 msgid "Amount in %(currency)s"
-msgstr ""
+msgstr "Cantidad en %(currency)s"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s modified"
-msgstr "La factura ha sido modificada"
+msgstr "La factura %(name)s ha sido modificada"
 
 #, python-format
 msgid "Participant %(name)s modified"
-msgstr ""
+msgstr "Participante %(name)s modificad@"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s removed"
-msgstr "Se ha eliminado al usuario '%(name)s'"
+msgstr "Factura %(name)s removida"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant %(name)s removed"
-msgstr "Se ha eliminado al usuario '%(name)s'"
+msgstr "Participante %(name)s removid@"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project %(name)s changed in an unknown way"
-msgstr "se cambió de manera desconocida"
+msgstr "Proyecto %(name)s se cambió de manera desconocida"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s changed in an unknown way"
-msgstr "se cambió de manera desconocida"
+msgstr "Factura %(name)s se cambió de manera desconocida"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant %(name)s changed in an unknown way"
-msgstr "se cambió de manera desconocida"
+msgstr "Participante %(name)s se cambió de manera desconocida"
 
 msgid "Nothing to list"
 msgstr "Nada por listar"
 
 msgid "Someone probably cleared the project history."
 msgstr "Es probable que alguien borrara el historial del proyecto."
 
@@ -761,14 +753,16 @@
 msgid "Create"
 msgstr "Crear"
 
 msgid ""
 "Don\\'t reuse a personal password. Choose a private code and send it to "
 "your friends"
 msgstr ""
+"No reutilice una contraseña personal. Elija un código privado y envíelo a "
+"sus amigos"
 
 msgid "Account manager"
 msgstr "Gestor de cuentas"
 
 msgid "Bills"
 msgstr "Facturas"
 
@@ -813,27 +807,26 @@
 
 msgid "Documentation"
 msgstr "Documentación"
 
 msgid "Administation Dashboard"
 msgstr "Panel de administración"
 
-#, fuzzy
 msgid "Legal information"
-msgstr "Confirmación de eliminación"
+msgstr "Información legal"
 
 msgid "\"I hate money\" is free software"
 msgstr "\"I hate money\" es un software libre"
 
 msgid "you can contribute and improve it!"
 msgstr "puedes contribuir y mejorarlo!"
 
 #, python-format
 msgid "%(amount)s each"
-msgstr ""
+msgstr "%(amount)s cada uno"
 
 msgid "you sure?"
 msgstr "¿Estás seguro?"
 
 msgid "Invite people"
 msgstr "Invitar personas"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/fa/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/ur/LC_MESSAGES/messages.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Automatically generated\n"
-"Language: fa\n"
-"Language-Team: none\n"
-"Plural-Forms: nplurals=1; plural=0\n"
+"POT-Creation-Date: 2022-07-02 10:57+0200\n"
+"PO-Revision-Date: 2022-07-03 10:18+0000\n"
+"Last-Translator: Shafiq Azeez <fubukishirouk@gmail.com>\n"
+"Language-Team: Urdu <https://hosted.weblate.org/projects/i-hate-money/"
+"i-hate-money/ur/>\n"
+"Language: ur\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
+"Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.0\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.13.1-dev\n"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 
 msgid "Project name"
-msgstr ""
+msgstr "منصوبےکانام"
 
 msgid "New private code"
 msgstr ""
 
 msgid "Enter a new code if you want to change it"
 msgstr ""
 
 msgid "Email"
-msgstr ""
+msgstr "برقی خط (ای ميل)"
 
 msgid "Enable project history"
 msgstr ""
 
 msgid "Use IP tracking for project history"
 msgstr ""
 
@@ -78,15 +78,15 @@
 msgid "Please, validate the captcha to proceed."
 msgstr ""
 
 msgid "Enter private code to confirm deletion"
 msgstr ""
 
 msgid "Unknown error"
-msgstr ""
+msgstr "نامعلوم خرابی"
 
 msgid "Invalid private code."
 msgstr ""
 
 msgid "Get in"
 msgstr ""
 
@@ -111,39 +111,39 @@
 msgid "Reset password"
 msgstr ""
 
 msgid "Date"
 msgstr ""
 
 msgid "What?"
-msgstr ""
+msgstr "کیا؟"
 
 msgid "Payer"
-msgstr ""
+msgstr "قیمت ادا کرنے والا"
 
 msgid "Amount paid"
-msgstr ""
+msgstr "ادا شدہ قیمت"
 
 msgid "Currency"
-msgstr ""
+msgstr "سکہ رائج الوقت (کرنسی)"
 
 msgid "External link"
-msgstr ""
+msgstr "بیرونی لنک"
 
 msgid "A link to an external document, related to this bill"
-msgstr ""
+msgstr "اس رسید کے لیے بیرونی رستاویز کا لنک"
 
 msgid "For whom?"
-msgstr ""
+msgstr "کس کے لیے؟"
 
 msgid "Submit"
-msgstr ""
+msgstr "جمع کروائیں"
 
 msgid "Submit and add a new one"
-msgstr ""
+msgstr "جمع کرکے ایک اور نیا اندراج کروائیں"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr ""
 
 msgid "Bills can't be null"
 msgstr ""
@@ -896,50 +896,7 @@
 msgstr ""
 
 msgid "Expenses by Month"
 msgstr ""
 
 msgid "Period"
 msgstr ""
-
-#~ msgid "You either provided a bad token or no project identifier."
-#~ msgstr ""
-
-#~ msgid "\"I hate money\" is a free software"
-#~ msgstr ""
-
-#~ msgid "User name incorrect"
-#~ msgstr ""
-
-#~ msgid "This project already have this member"
-#~ msgstr ""
-
-#~ msgid "People to notify"
-#~ msgstr ""
-
-#~ msgid "Error activating member"
-#~ msgstr ""
-
-#~ msgid "Error removing member"
-#~ msgstr ""
-
-#~ msgid ""
-#~ "User '%(name)s' has been deactivated. It"
-#~ " will still appear in the users "
-#~ "list until its balance becomes zero."
-#~ msgstr ""
-
-#~ msgid "User '%(name)s' has been removed"
-#~ msgstr ""
-
-#~ msgid "User '%(name)s' has been edited"
-#~ msgstr ""
-
-#~ msgid "Number of members"
-#~ msgstr ""
-
-#~ msgid "Edit this member"
-#~ msgstr ""
-
-#~ msgid "Participants to notify"
-#~ msgstr ""
-
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/fr/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/fr/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: French <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.10-dev\n"
+"X-Generator: Weblate 4.16-dev\n"
 
 msgid ""
 "\n"
 "            <i>The table below reflects actions recorded prior to disabling "
 "project history. You can\n"
 "            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
 "target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
@@ -484,15 +484,15 @@
 msgid "Nothing to list yet."
 msgstr "Rien à lister pour le moment."
 
 msgid "Number of bills"
 msgstr "Nombre de factures"
 
 msgid "Number of participants"
-msgstr "ajouter des participant⋅es"
+msgstr "Nombre de participant⋅es"
 
 msgid "Older bills"
 msgstr "Factures précédentes"
 
 msgid "Oldest bill"
 msgstr "Facture la plus ancienne"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/fr/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/fr/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # Alexis Métaireau <alexis@notmyidea.org>, 2011.
 # Adrien CLERC, 2018.
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2021-11-25 23:51+0000\n"
-"Last-Translator: Alexis Metaireau <alexis@notmyidea.org>\n"
+"PO-Revision-Date: 2023-01-29 15:17+0000\n"
+"Last-Translator: Glandos <bugs-github@antipoul.fr>\n"
 "Language-Team: French <https://hosted.weblate.org/projects/i-hate-money/"
 "i-hate-money/fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.10-dev\n"
+"X-Generator: Weblate 4.16-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Ceci n'est pas un montant ou une expression valide. Seuls les nombres et "
@@ -386,15 +386,15 @@
 msgid "Create a new project"
 msgstr "Créer un nouveau projet"
 
 msgid "Project"
 msgstr "Projet"
 
 msgid "Number of participants"
-msgstr "ajouter des participant⋅es"
+msgstr "Nombre de participant⋅es"
 
 msgid "Number of bills"
 msgstr "Nombre de factures"
 
 msgid "Newest bill"
 msgstr "Facture la plus récente"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/hi/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/hi/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/hi/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/hi/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/id/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/id/LC_MESSAGES/messages.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Indonesian <https://hosted.weblate.org/projects/i-hate-money/"
 "i-hate-money/id/>\n"
 "Language: id\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.10-dev\n"
+"X-Generator: Weblate 4.12-dev\n"
 
 msgid ""
 "\n"
 "            <i>The table below reflects actions recorded prior to disabling "
 "project history. You can\n"
 "            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
 "target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
@@ -597,14 +597,18 @@
 
 msgid "Send the invitations"
 msgstr "Kirim undangan"
 
 msgid "Send via Emails"
 msgstr "Kirim melalui surel"
 
+msgid "Setting a default currency enables currency conversion between bills"
+msgstr ""
+"Menetapkan mata uang default memungkinkan konversi mata uang antar tagihan"
+
 msgid "Settings"
 msgstr "Pengaturan"
 
 msgid "Settle"
 msgstr "Atur"
 
 msgid "Settle plans"
@@ -759,14 +763,17 @@
 
 msgid "What?"
 msgstr "Apa?"
 
 msgid "When?"
 msgstr "Kapan?"
 
+msgid "Which is a real currency: Euro or Petro dollar?"
+msgstr "Manakah mata uang riil: Euro atau dolar Petro?"
+
 msgid "Who paid?"
 msgstr "Siapa yang bayar?"
 
 msgid "Who pays?"
 msgstr "Siapa membayar?"
 
 msgid "Who?"
@@ -821,14 +828,17 @@
 
 msgid "delete"
 msgstr "hapus"
 
 msgid "edit"
 msgstr "ubah"
 
+msgid "euro"
+msgstr "Euro"
+
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "john.doe@example.com, mary.moe@site.com"
 
 msgid "reactivate"
 msgstr "aktivasi ulang"
 
 msgid "show"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/id/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/id/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2021-11-23 00:51+0000\n"
-"Last-Translator: whenwesober <naomi16i_1298q@cikuh.com>\n"
+"PO-Revision-Date: 2022-04-11 17:12+0000\n"
+"Last-Translator: Santiago José Gutiérrez Llanos <gutierrezapata17@gmail.com>"
+"\n"
 "Language-Team: Indonesian <https://hosted.weblate.org/projects/i-hate-money/"
 "i-hate-money/id/>\n"
 "Language: id\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.10-dev\n"
+"X-Generator: Weblate 4.12-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Bukan jumlah atau operator yang valid. Hanya angka dan operator + -* / "
@@ -41,14 +42,15 @@
 msgstr "Gunakan pelacakan IP untuk riwayat proyek"
 
 msgid "Default Currency"
 msgstr "Mata Uang Standar"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
+"Menetapkan mata uang default memungkinkan konversi mata uang antar tagihan"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Proyek ini tidak dapat disetel ke 'tanpa mata uang' karena berisi tagihan"
 " dalam berbagai mata uang."
@@ -73,19 +75,18 @@
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
 msgstr ""
 "Sebuah proyek dengan ID ini (\"%(project)s\") sudah ada. Silakan pilih ID"
 " baru"
 
 msgid "Which is a real currency: Euro or Petro dollar?"
-msgstr ""
+msgstr "Manakah mata uang riil: Euro atau dolar Petro?"
 
-#, fuzzy
 msgid "euro"
-msgstr "Periode"
+msgstr "Euro"
 
 msgid "Please, validate the captcha to proceed."
 msgstr "Mohon, silahkan validasi captcha untuk melanjutkan."
 
 msgid "Enter private code to confirm deletion"
 msgstr "Masukkan kode pribadi untuk mengkonfirmasi penghapusan"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/it/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/it/LC_MESSAGES/messages.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Italian <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/it/>\n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.10-dev\n"
+"X-Generator: Weblate 4.14-dev\n"
 
 msgid ""
 "\n"
 "            <i>The table below reflects actions recorded prior to disabling "
 "project history. You can\n"
 "            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
 "target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
@@ -251,14 +251,17 @@
 
 msgid "Enabled Project History"
 msgstr "Cronologia Progetto Abilitata"
 
 msgid "Enabled Project History & IP Address Recording"
 msgstr "Storico Progetto & Registrazione Indirizzo IP Abilitato"
 
+msgid "Enter a new code if you want to change it"
+msgstr "Inserisci un nuovo codice se lo vuoi modificare"
+
 msgid "Event"
 msgstr "Evento"
 
 msgid "Everyone"
 msgstr "Tutti"
 
 msgid "Everyone but %(excluded)s"
@@ -411,14 +414,17 @@
 
 msgid "Payer"
 msgstr "Pagatore"
 
 msgid "Period"
 msgstr "Periodo"
 
+msgid "Please, validate the captcha to proceed."
+msgstr "Si prega di validare il captcha per procedere."
+
 msgid "Privacy Settings"
 msgstr "Impostazioni Privacy"
 
 msgid "Private code"
 msgstr "Codice privato"
 
 msgid "Project"
@@ -468,14 +474,19 @@
 
 msgid "Send the invitations"
 msgstr "Spedisci gli inviti"
 
 msgid "Send via Emails"
 msgstr "Inviare via Email"
 
+msgid "Setting a default currency enables currency conversion between bills"
+msgstr ""
+"Impostando una valuta predefinita abilita la conversione della valuta tra le "
+"fatture"
+
 msgid "Settings"
 msgstr "Impostazioni"
 
 msgid "Settle"
 msgstr "Liquidazioni"
 
 msgid "Settle plans"
@@ -567,14 +578,21 @@
 msgstr ""
 "Questa password di amministrazione non è quella corretta. Solo %(num)d "
 "tentativi rimasti."
 
 msgid "This private code is not the right one"
 msgstr "Questo codice privato non è quello corretto"
 
+msgid ""
+"This project cannot be set to 'no currency' because it contains bills in "
+"multiple currencies."
+msgstr ""
+"Questo progetto non può essere impostato come 'nessuna valuta' perché "
+"contiene fatture in più valute."
+
 msgid "This project does not exists"
 msgstr "Questo progetto non esiste"
 
 msgid "Time"
 msgstr "Ora"
 
 msgid "To whom?"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/it/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/it/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2021-11-25 23:51+0000\n"
-"Last-Translator: Paolo Campetto <fbok61hw@anonaddy.me>\n"
+"PO-Revision-Date: 2022-07-12 15:18+0000\n"
+"Last-Translator: Matteo Piotto <piotto@gmail.com>\n"
 "Language-Team: Italian <https://hosted.weblate.org/projects/i-hate-money/"
 "i-hate-money/it/>\n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.10-dev\n"
+"X-Generator: Weblate 4.14-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Quantità o espressione non valida. Solo numeri e operatori + - * / "
@@ -26,15 +26,15 @@
 msgstr "Nome del progetto"
 
 #, fuzzy
 msgid "New private code"
 msgstr "Codice privato"
 
 msgid "Enter a new code if you want to change it"
-msgstr ""
+msgstr "Inserisci un nuovo codice se lo vuoi modificare"
 
 msgid "Email"
 msgstr "Email"
 
 msgid "Enable project history"
 msgstr "Attivare la cronologia del progetto"
 
@@ -42,19 +42,23 @@
 msgstr "Utilizzare la localizzazione IP per lo storico del progetto"
 
 msgid "Default Currency"
 msgstr "Valuta predefinita"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
+"Impostando una valuta predefinita abilita la conversione della valuta tra le "
+"fatture"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
+"Questo progetto non può essere impostato come 'nessuna valuta' perché "
+"contiene fatture in più valute."
 
 msgid "Import previously exported JSON file"
 msgstr "Importare il file JSON esportato precedentemente"
 
 msgid "Import"
 msgstr "Importare"
 
@@ -79,15 +83,15 @@
 msgstr ""
 
 #, fuzzy
 msgid "euro"
 msgstr "Periodo"
 
 msgid "Please, validate the captcha to proceed."
-msgstr ""
+msgstr "Si prega di validare il captcha per procedere."
 
 msgid "Enter private code to confirm deletion"
 msgstr ""
 
 #, fuzzy
 msgid "Unknown error"
 msgstr "Progetto non conosciuto"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/ja/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/ja/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/kn/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/kn/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/kn/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/kn/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/ms/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/ms/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/ms/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/ms/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/nl/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/nl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/nl/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/nl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/pl/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/pl/LC_MESSAGES/messages.mo`

 * *Files 22% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "hate-money/pl/>\n"
 "Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.11-dev\n"
+"X-Generator: Weblate 4.14.1\n"
 
 msgid ""
 "\n"
 "            <i>The table below reflects actions recorded prior to disabling "
 "project history. You can\n"
 "            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
 "target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
@@ -129,20 +129,54 @@
 msgid ""
 "Are you sure you want to erase all history for this project? This action "
 "cannot be undone."
 msgstr ""
 "Czy na pewno chcesz usunąć całą historię tego projektu? Nie można cofnąć tej "
 "akcji."
 
+msgid "Are you sure?"
+msgstr "Czy jesteś pewien?"
+
+msgid "Authentication"
+msgstr "Uwierzytelnianie"
+
 msgid "Back to the list"
 msgstr "Powrót do listy"
 
 msgid "Balance"
 msgstr "Saldo"
 
+msgid "Bill %(name)s added"
+msgstr "Dodano rachunek %(name)s"
+
+msgid "Bill %(name)s changed in an unknown way"
+msgstr "Nazwa rachunku %(name)s zmieniła się w nieznany sposób"
+
+msgid "Bill %(name)s modified"
+msgstr "Rachunek %(name)s zmodyfikowany"
+
+msgid "Bill %(name)s removed"
+msgstr "Rachunek „%(name)s” został usunięty"
+
+msgid "Bill %(name)s renamed to %(new_description)s"
+msgstr "Rachunek %(name)s zmienił nazwę na %(new_description)s"
+
+msgid "Bill %(name)s: %(property_name)s changed from %(before)s to %(after)s"
+msgstr ""
+"Rachunek %(name)s: %(property_name)s zmieniono z %(before)s na %(after)s"
+
+msgid "Bill %(name)s: %(property_name)s changed to %(after)s"
+msgstr "Rachunek %(name)s: %(property_name)s zmieniony na %(after)s"
+
+msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
+msgstr "Bill %(name)s: dodano %(owers_list_str)s do listy właścicieli"
+
+msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
+msgstr "Bill %(name)s: usunięto %(owers_list_str)s z listy właścicieli"
+
 msgid "Bill items"
 msgstr "Zawartość rachunku"
 
 msgid "Bills"
 msgstr "Rachunki"
 
 msgid "Bills can't be null"
@@ -150,14 +184,19 @@
 
 msgid "Can't remember the password?"
 msgstr "Nie pamiętasz hasła?"
 
 msgid "Cancel"
 msgstr "Anuluj"
 
+msgid ""
+"Cannot add bills in multiple currencies to a project without default currency"
+msgstr ""
+"Nie można dodawać rachunków w wielu walutach do projektu bez waluty domyślnej"
+
 msgid "Choose file"
 msgstr "Wybierz plik"
 
 msgid "Clear Project History"
 msgstr "Wyczyść historię projektu"
 
 msgid "Close"
@@ -165,14 +204,17 @@
 
 msgid "Code"
 msgstr "Kod"
 
 msgid "Confirm Remove IP Adresses"
 msgstr "Potwierdź usunięcie adresów IP"
 
+msgid "Confirm deletion"
+msgstr "Potwierdź usunięcie"
+
 msgid "Create"
 msgstr "Stwórz"
 
 msgid "Create a new project"
 msgstr "Stwórz nowy projekt"
 
 msgid "Create the project"
@@ -192,17 +234,26 @@
 
 msgid "Delete Confirmation"
 msgstr "Usuń potwierdzenie"
 
 msgid "Delete Stored IP Addresses"
 msgstr "Usuń przechowywane adresy IP"
 
+msgid "Delete project"
+msgstr "Usuń projekt"
+
 msgid "Delete stored IP addresses"
 msgstr "Usuń przechowywane adresy IP"
 
+msgid "Deleted project history."
+msgstr "Usunięto historię projektu."
+
+msgid "Deleted recorded IP addresses in project history."
+msgstr "Usunięto zarejestrowane adresy IP z historii projektu."
+
 msgid "Disabled IP Address Recording"
 msgstr "Wyłączona rejestracja adresu IP"
 
 msgid "Disabled Project History"
 msgstr "Wyłączona historia projektu"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -217,14 +268,17 @@
 msgstr ""
 "Nie używaj ponownie osobistego hasła. Wybierz kod prywatny i wyślij go "
 "znajomym"
 
 msgid "Download"
 msgstr "Pobierz"
 
+msgid "Download Mobile Application"
+msgstr "Pobierz aplikację mobilną"
+
 msgid "Download project's data"
 msgstr "Pobierz dane projektu"
 
 msgid "Download the list of bills with owner, amount, reason,... "
 msgstr "Pobierz listę rachunków z właścicielem, kwotą, powodem,... "
 
 msgid "Download the list of transactions needed to settle the current bills."
@@ -236,14 +290,17 @@
 
 msgid "Edit the project"
 msgstr "Edytuj projekt"
 
 msgid "Edit this bill"
 msgstr "Edytuj ten rachunek"
 
+msgid "Edit this participant"
+msgstr "Edytuj tego uczestnika"
+
 msgid "Email"
 msgstr "E-mail"
 
 msgid "Enable project history"
 msgstr "Włącz historię projektu"
 
 msgid "Enabled IP Address Recording"
@@ -257,14 +314,32 @@
 
 msgid "Enter a new code if you want to change it"
 msgstr "Wprowadź nowy kod jeżeli chcesz go zmienić"
 
 msgid "Enter private code to confirm deletion"
 msgstr "Wprowadź kod prywatny w celu potwierdzenia usunięcia"
 
+msgid "Error activating participant"
+msgstr "Błąd podczas aktywacji uczestnika"
+
+msgid "Error deleting bill"
+msgstr "Błąd podczas usuwania rachunku"
+
+msgid "Error deleting project"
+msgstr "Błąd podczas usuwania projektu"
+
+msgid "Error deleting project history"
+msgstr "Błąd podczas usuwania historii projektu"
+
+msgid "Error deleting recorded IP addresses"
+msgstr "Błąd podczas usuwania zarejestrowanych adresów IP"
+
+msgid "Error removing participant"
+msgstr "Błąd podczas usuwania uczestnika"
+
 msgid "Event"
 msgstr "Wydarzenie"
 
 msgid "Everyone"
 msgstr "Wszyscy"
 
 msgid "Everyone but %(excluded)s"
@@ -284,14 +359,17 @@
 
 msgid "From IP"
 msgstr "Z IP"
 
 msgid "Get in"
 msgstr "Wejdź"
 
+msgid "Get it on"
+msgstr "Pobierz na"
+
 msgid "Going on holidays with friends?"
 msgstr "Jedziesz na wakacje ze znajomymi?"
 
 msgid "History"
 msgstr "Historia"
 
 msgid "History Settings Changed"
@@ -332,14 +410,17 @@
 
 msgid "Invite people to join this project"
 msgstr "Zaproś ludzi do dołączenia do tego projektu"
 
 msgid "Languages"
 msgstr "Języki"
 
+msgid "Legal information"
+msgstr "Informacje prawne"
+
 msgid "Log in"
 msgstr "Zaloguj się"
 
 msgid "Log in to an existing project"
 msgstr "Zaloguj się do istniejącego projektu"
 
 msgid "Logout"
@@ -347,14 +428,17 @@
 
 msgid "Manage your shared <br />expenses, easily"
 msgstr "Łatwo zarządzaj wspólnymi <br /> wydatkami"
 
 msgid "Mobile Application"
 msgstr "Aplikacja mobilna"
 
+msgid "More options"
+msgstr "Więcej opcji"
+
 msgid "Name"
 msgstr "Nazwa"
 
 msgid "New private code"
 msgstr "Nowy kod prywatny"
 
 msgid "Newer bills"
@@ -371,14 +455,17 @@
 
 msgid "No bills"
 msgstr "Brak rachunków"
 
 msgid "No history to erase"
 msgstr "Brak historii do usunięcia"
 
+msgid "No one"
+msgstr "Nikt"
+
 msgid "No token provided"
 msgstr "Nie podano tokena"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
@@ -390,26 +477,67 @@
 
 msgid "Nothing to list yet."
 msgstr "Nie ma jeszcze żadnej listy."
 
 msgid "Number of bills"
 msgstr "Liczba rachunków"
 
+msgid "Number of participants"
+msgstr "Liczba uczestników"
+
 msgid "Older bills"
 msgstr "Starsze rachunki"
 
 msgid "Oldest bill"
 msgstr "Najstarszy rachunek"
 
 msgid "Other projects :"
 msgstr "Inne projekty:"
 
 msgid "Paid"
 msgstr "Zapłacone"
 
+msgid "Participant %(name)s added"
+msgstr "Dodano uczestnika %(name)s"
+
+msgid "Participant %(name)s changed in an unknown way"
+msgstr "Nazwa uczestnika %(name)s zmieniła się w nieznany sposób"
+
+msgid "Participant %(name)s deactivated"
+msgstr "Uczestnik %(name)s dezaktywowany"
+
+msgid "Participant %(name)s modified"
+msgstr "Uczestnik %(name)s zmodyfikowany"
+
+msgid "Participant %(name)s reactivated"
+msgstr "Uczestnik %(name)s reaktywowany"
+
+msgid "Participant %(name)s removed"
+msgstr "Uczestnik „%(name)s” został usunięty"
+
+msgid "Participant %(name)s renamed to %(new_name)s"
+msgstr "Uczestnikowi %(name)s zmieniono nazwę na %(new_name)s"
+
+msgid ""
+"Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
+msgstr "Uczestnik %(name)s: zmiana wagi z %(old_weight)s na %(new_weight)s"
+
+msgid ""
+"Participant '%(name)s' has been deactivated. It will still appear in the "
+"list until its balance reach zero."
+msgstr ""
+"Uczestnik „%(name)s” został wyłączony. Będzie nadal pojawiać się na liście "
+"użytkowników, dopóki jego saldo nie wyniesie zero."
+
+msgid "Participant '%(name)s' has been modified"
+msgstr "Uczestnik „%(name)s” został usunięty"
+
+msgid "Participant '%(name)s' has been removed"
+msgstr "Uczestnik „%(name)s” został usunięty"
+
 msgid "Password"
 msgstr "Hasło"
 
 msgid "Password confirmation"
 msgstr "Potwierdzenie hasła"
 
 msgid "Password mismatch"
@@ -438,38 +566,54 @@
 
 msgid "Private code"
 msgstr "Kod prywatny"
 
 msgid "Project"
 msgstr "Projekt"
 
+msgid "Project %(name)s added"
+msgstr "Dodano projekt %(name)s"
+
+msgid "Project %(name)s changed in an unknown way"
+msgstr "Nazwa projektu %(name)s zmieniła się w nieznany sposób"
+
+msgid "Project contact email changed to %(new_email)s"
+msgstr ""
+"Adres e-mail osoby kontaktowej projektu został zmieniony na %(new_email)s"
+
 msgid "Project default: %(currency)s"
 msgstr "Wartość domyślna projektu: %(currency)s"
 
 msgid "Project identifier"
 msgstr "Identyfikator projektu"
 
 msgid "Project name"
 msgstr "Nazwa projektu"
 
 msgid "Project private code changed"
 msgstr "Prywatny kod projektu został zmieniony"
 
+msgid "Project renamed to %(new_project_name)s"
+msgstr "Nazwa projektu zmieniona na %(new_project_name)s"
+
 msgid "Project settings modified"
 msgstr "Zmieniono ustawienia projektu"
 
 msgid "Project successfully deleted"
 msgstr "Projekt został pomyślnie usunięty"
 
 msgid "Project successfully uploaded"
 msgstr "Projekt został pomyślnie przesłany"
 
 msgid "Projects"
 msgstr "Projekty"
 
+msgid "Provided token is invalid"
+msgstr "Podany token jest niepoprawny"
+
 msgid "Reset password"
 msgstr "Zmień hasło"
 
 msgid "Reset your password"
 msgstr "Zresetuj swoje hasło"
 
 msgid "Return to home page"
@@ -609,14 +753,18 @@
 msgstr ""
 "Ten projekt nie może zostać oznaczony jako 'bez waluty', ponieważ zawiera on "
 "rachunki w różnych walutach."
 
 msgid "This project does not exists"
 msgstr "Ten projekt nie istnieje"
 
+msgid "This will remove all bills and participants in this project!"
+msgstr ""
+"Spowoduje to usunięcie wszystkich rachunków i uczestników tego projektu!"
+
 msgid "Time"
 msgstr "Czas"
 
 msgid "To whom?"
 msgstr "Komu?"
 
 msgid "Too many failed login attempts, please retry later."
@@ -738,7 +886,25 @@
 msgstr "przełącz na"
 
 msgid "you can contribute and improve it!"
 msgstr "możesz przyczynić się i je ulepszyć!"
 
 msgid "you sure?"
 msgstr "jesteś pewny?"
+
+msgid "{dual_object_0} and {dual_object_1}"
+msgstr "{dual_object_0} i {dual_object_1}"
+
+msgid "{prefix}: {error}"
+msgstr "{prefix}: {error}"
+
+msgid "{prefix}:<br />{errors}"
+msgstr "{prefix}:<br />{errors}"
+
+msgid "{previous_object}, and {end_object}"
+msgstr "{previous_object} i {end_object}"
+
+msgid "{previous_object}, {next_object}"
+msgstr "{previous_object}, {next_object}"
+
+msgid "{start_object}, {next_object}"
+msgstr "{start_object}, {next_object}"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/pl/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/pl/LC_MESSAGES/messages.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2022-01-20 20:55+0000\n"
-"Last-Translator: Piotr <promantix@gmail.com>\n"
+"PO-Revision-Date: 2022-09-27 14:19+0000\n"
+"Last-Translator: Andrzej Ochodek <andrzej.ochodek@gmail.com>\n"
 "Language-Team: Polish <https://hosted.weblate.org/projects/i-hate-money/"
 "i-hate-money/pl/>\n"
 "Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.11-dev\n"
+"X-Generator: Weblate 4.14.1\n"
 "Generated-By: Babel 2.9.0\n"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Niepoprawna kwota lub wyrażenie. Akceptowane są tylko liczby i operatory "
@@ -183,48 +183,48 @@
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "Ten email %(email)s jest nieprawidłowy"
 
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
-msgstr ""
+msgstr "{dual_object_0} i {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
-msgstr ""
+msgstr "{previous_object} i {end_object}"
 
 #. Two items in a middle of a list with more than 5 objects
 msgid "{previous_object}, {next_object}"
-msgstr ""
+msgstr "{previous_object}, {next_object}"
 
 #. First two items of a list with more than 3 items
 msgid "{start_object}, {next_object}"
-msgstr ""
+msgstr "{start_object}, {next_object}"
 
 msgid "No Currency"
 msgstr "Brak walut"
 
 #. Form error with only one error
 msgid "{prefix}: {error}"
-msgstr ""
+msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
-msgstr ""
+msgstr "{prefix}:<br />{errors}"
 
 msgid "Too many failed login attempts, please retry later."
 msgstr "Zbyt wiele nieudanych prób logowania, spróbuj ponownie później."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "To hasło administratora jest nieprawidłowe. Pozostało tylko %(num)d prób."
 
 msgid "Provided token is invalid"
-msgstr ""
+msgstr "Podany token jest niepoprawny"
 
 msgid "This private code is not the right one"
 msgstr "Ten prywatny kod jest niewłaściwy"
 
 #, python-format
 msgid "You have just created '%(project)s' to share your expenses"
 msgstr "Właśnie utworzyłeś „%(project)s”, aby podzielić się wydatkami"
@@ -270,20 +270,21 @@
 msgid "Invalid JSON"
 msgstr "Niepoprawny JSON"
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
+"Nie można dodawać rachunków w wielu walutach do projektu bez waluty domyślnej"
 
 msgid "Project successfully deleted"
 msgstr "Projekt został pomyślnie usunięty"
 
 msgid "Error deleting project"
-msgstr ""
+msgstr "Błąd podczas usuwania projektu"
 
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "Zostałeś zaproszony do podzielenia się swoimi wydatkami w %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "Twoje zaproszenia zostały wysłane"
@@ -298,65 +299,62 @@
 "administratorem."
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr "%(member)s został dodany"
 
 msgid "Error activating participant"
-msgstr ""
+msgstr "Błąd podczas aktywacji uczestnika"
 
 #, python-format
 msgid "%(name)s is part of this project again"
 msgstr "%(name)s jest ponownie częścią tego projektu"
 
 msgid "Error removing participant"
-msgstr ""
+msgstr "Błąd podczas usuwania uczestnika"
 
-#, fuzzy, python-format
+#, python-format
 msgid ""
 "Participant '%(name)s' has been deactivated. It will still appear in the "
 "list until its balance reach zero."
 msgstr ""
-"Użytkownik „%(name)s” został dezaktywowany. Będzie nadal pojawiać się na "
-"liście użytkowników, dopóki jego saldo nie wyniesie zero."
+"Uczestnik „%(name)s” został wyłączony. Będzie nadal pojawiać się na liście "
+"użytkowników, dopóki jego saldo nie wyniesie zero."
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant '%(name)s' has been removed"
-msgstr "Użytkownik „%(name)s” został usunięty"
+msgstr "Uczestnik „%(name)s” został usunięty"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant '%(name)s' has been modified"
-msgstr "Użytkownik „%(name)s” został usunięty"
+msgstr "Uczestnik „%(name)s” został usunięty"
 
 msgid "The bill has been added"
 msgstr "Rachunek został dodany"
 
 msgid "Error deleting bill"
-msgstr ""
+msgstr "Błąd podczas usuwania rachunku"
 
 msgid "The bill has been deleted"
 msgstr "Rachunek został usunięty"
 
 msgid "The bill has been modified"
 msgstr "Rachunek został zmieniony"
 
-#, fuzzy
 msgid "Error deleting project history"
-msgstr "Włącz historię projektu"
+msgstr "Błąd podczas usuwania historii projektu"
 
-#, fuzzy
 msgid "Deleted project history."
-msgstr "Włącz historię projektu"
+msgstr "Usunięto historię projektu."
 
-#, fuzzy
 msgid "Error deleting recorded IP addresses"
-msgstr "Usuń przechowywane adresy IP"
+msgstr "Błąd podczas usuwania zarejestrowanych adresów IP"
 
 msgid "Deleted recorded IP addresses in project history."
-msgstr ""
+msgstr "Usunięto zarejestrowane adresy IP z historii projektu."
 
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "Niestety nie udało nam się znaleźć strony, o którą prosiłeś."
 
 msgid "The best thing to do is probably to get back to the main page."
 msgstr ""
 "Najlepszą rzeczą do zrobienia jest prawdopodobnie powrót do strony "
@@ -364,17 +362,16 @@
 
 msgid "Back to the list"
 msgstr "Powrót do listy"
 
 msgid "Administration tasks are currently disabled."
 msgstr "Zadania administracyjne są obecnie wyłączone."
 
-#, fuzzy
 msgid "Authentication"
-msgstr "Dokumentacja"
+msgstr "Uwierzytelnianie"
 
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "Projekt, do którego próbujesz uzyskać dostęp, nie istnieje, czy chcesz"
 
 msgid "create it"
 msgstr "stworzyć go"
 
@@ -383,17 +380,16 @@
 
 msgid "Create a new project"
 msgstr "Stwórz nowy projekt"
 
 msgid "Project"
 msgstr "Projekt"
 
-#, fuzzy
 msgid "Number of participants"
-msgstr "dodać członków"
+msgstr "Liczba uczestników"
 
 msgid "Number of bills"
 msgstr "Liczba rachunków"
 
 msgid "Newest bill"
 msgstr "Najnowszy rachunek"
 
@@ -411,32 +407,28 @@
 
 msgid "show"
 msgstr "pokaż"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "Pulpit nawigacyjny jest obecnie dezaktywowany."
 
-#, fuzzy
 msgid "Download Mobile Application"
-msgstr "Aplikacja mobilna"
+msgstr "Pobierz aplikację mobilną"
 
-#, fuzzy
 msgid "Get it on"
-msgstr "Wejdź"
+msgstr "Pobierz na"
 
-#, fuzzy
 msgid "Are you sure?"
-msgstr "jesteś pewny?"
+msgstr "Czy jesteś pewien?"
 
 msgid "Edit project"
 msgstr "Edytuj projekt"
 
-#, fuzzy
 msgid "Delete project"
-msgstr "Edytuj projekt"
+msgstr "Usuń projekt"
 
 msgid "Import JSON"
 msgstr "Importuj JSON"
 
 msgid "Choose file"
 msgstr "Wybierz plik"
 
@@ -465,36 +457,36 @@
 msgstr "Ustawienia prywatności"
 
 msgid "Edit the project"
 msgstr "Edytuj projekt"
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
+"Spowoduje to usunięcie wszystkich rachunków i uczestników tego projektu!"
 
 msgid "Edit this bill"
 msgstr "Edytuj ten rachunek"
 
 msgid "Add a bill"
 msgstr "Dodaj rachunek"
 
 msgid "Everyone"
 msgstr "Wszyscy"
 
 msgid "No one"
-msgstr ""
+msgstr "Nikt"
 
 msgid "More options"
-msgstr ""
+msgstr "Więcej opcji"
 
 msgid "Add participant"
 msgstr "Dodaj uczestnika"
 
-#, fuzzy
 msgid "Edit this participant"
-msgstr "Dodaj uczestnika"
+msgstr "Edytuj tego uczestnika"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "jan.kowalski@przykład.com, anna.nowak@strona.com"
 
 msgid "Send the invitations"
 msgstr "Wyślij zaproszenia"
 
@@ -521,18 +513,19 @@
 
 msgid "History Settings Changed"
 msgstr "Ustawienia historii zmienione"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed from %(before)s to %(after)s"
 msgstr ""
+"Rachunek %(name)s: %(property_name)s zmieniono z %(before)s na %(after)s"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed to %(after)s"
-msgstr ""
+msgstr "Rachunek %(name)s: %(property_name)s zmieniony na %(after)s"
 
 msgid "Confirm Remove IP Adresses"
 msgstr "Potwierdź usunięcie adresów IP"
 
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
@@ -540,15 +533,14 @@
 "action cannot be undone."
 msgstr ""
 "Czy na pewno chcesz usunąć wszystkie zarejestrowane adresy IP z tego "
 "projektu?\n"
 "                 Pozostała część historii projektu pozostanie "
 "niezmieniona. Nie można cofnąć tej akcji."
 
-#, fuzzy
 msgid "Confirm deletion"
 msgstr "Potwierdź usunięcie"
 
 msgid "Close"
 msgstr "Zamknij"
 
 msgid "Delete Confirmation"
@@ -559,19 +551,19 @@
 "cannot be undone."
 msgstr ""
 "Czy na pewno chcesz usunąć całą historię tego projektu? Nie można cofnąć "
 "tej akcji."
 
 #, python-format
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
-msgstr ""
+msgstr "Bill %(name)s: dodano %(owers_list_str)s do listy właścicieli"
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
-msgstr ""
+msgstr "Bill %(name)s: usunięto %(owers_list_str)s z listy właścicieli"
 
 #, python-format
 msgid ""
 "\n"
 "            <i>This project has history disabled. New actions won't "
 "appear below. You can enable history on the</i>\n"
 "            <a href=\"%(url)s\">settings page</a>\n"
@@ -633,94 +625,95 @@
 
 msgid "IP address recording can be disabled on the settings page"
 msgstr "Rejestrowanie adresu IP można wyłączyć na stronie ustawień"
 
 msgid "From IP"
 msgstr "Z IP"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project %(name)s added"
-msgstr "Nazwa projektu"
+msgstr "Dodano projekt %(name)s"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s added"
-msgstr "Rachunek został dodany"
+msgstr "Dodano rachunek %(name)s"
 
 #, python-format
 msgid "Participant %(name)s added"
-msgstr ""
+msgstr "Dodano uczestnika %(name)s"
 
 msgid "Project private code changed"
 msgstr "Prywatny kod projektu został zmieniony"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project renamed to %(new_project_name)s"
-msgstr "Identyfikator projektu to %(new_project_name)s"
+msgstr "Nazwa projektu zmieniona na %(new_project_name)s"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project contact email changed to %(new_email)s"
-msgstr "Kontaktowy adres email projektu został zmieniony na"
+msgstr ""
+"Adres e-mail osoby kontaktowej projektu został zmieniony na %(new_email)s"
 
 msgid "Project settings modified"
 msgstr "Zmieniono ustawienia projektu"
 
 #, python-format
 msgid "Participant %(name)s deactivated"
-msgstr ""
+msgstr "Uczestnik %(name)s dezaktywowany"
 
 #, python-format
 msgid "Participant %(name)s reactivated"
-msgstr ""
+msgstr "Uczestnik %(name)s reaktywowany"
 
 #, python-format
 msgid "Participant %(name)s renamed to %(new_name)s"
-msgstr ""
+msgstr "Uczestnikowi %(name)s zmieniono nazwę na %(new_name)s"
 
 #, python-format
 msgid "Bill %(name)s renamed to %(new_description)s"
-msgstr ""
+msgstr "Rachunek %(name)s zmienił nazwę na %(new_description)s"
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
-msgstr ""
+msgstr "Uczestnik %(name)s: zmiana wagi z %(old_weight)s na %(new_weight)s"
 
 msgid "Amount"
 msgstr "Ilość"
 
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "Ilość w %(currency)s"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s modified"
-msgstr "Rachunek został zmieniony"
+msgstr "Rachunek %(name)s zmodyfikowany"
 
 #, python-format
 msgid "Participant %(name)s modified"
-msgstr ""
+msgstr "Uczestnik %(name)s zmodyfikowany"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s removed"
-msgstr "Użytkownik „%(name)s” został usunięty"
+msgstr "Rachunek „%(name)s” został usunięty"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant %(name)s removed"
-msgstr "Użytkownik „%(name)s” został usunięty"
+msgstr "Uczestnik „%(name)s” został usunięty"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project %(name)s changed in an unknown way"
-msgstr "zmieniony w nieznany sposób"
+msgstr "Nazwa projektu %(name)s zmieniła się w nieznany sposób"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s changed in an unknown way"
-msgstr "zmieniony w nieznany sposób"
+msgstr "Nazwa rachunku %(name)s zmieniła się w nieznany sposób"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant %(name)s changed in an unknown way"
-msgstr "zmieniony w nieznany sposób"
+msgstr "Nazwa uczestnika %(name)s zmieniła się w nieznany sposób"
 
 msgid "Nothing to list"
 msgstr "Nic na liście"
 
 msgid "Someone probably cleared the project history."
 msgstr "Ktoś prawdopodobnie wyczyścił historię projektu."
 
@@ -808,17 +801,16 @@
 
 msgid "Documentation"
 msgstr "Dokumentacja"
 
 msgid "Administation Dashboard"
 msgstr "Kokpit administracyjny"
 
-#, fuzzy
 msgid "Legal information"
-msgstr "Usuń potwierdzenie"
+msgstr "Informacje prawne"
 
 msgid "\"I hate money\" is free software"
 msgstr "„I Hate Money” to darmowe oprogramowanie"
 
 msgid "you can contribute and improve it!"
 msgstr "możesz przyczynić się i je ulepszyć!"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/pt/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/pt/LC_MESSAGES/messages.mo`

 * *Files 23% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,21 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
+"Project-Id-Version: Portuguese (I Hate Money)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2020-10-05 12:12+0000\n"
-"Last-Translator: ssantos <ssantos@web.de>\n"
-"Language: pt\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: Portuguese <https://hosted.weblate.org/projects/i-hate-money/"
 "i-hate-money/pt/>\n"
-"Plural-Forms: nplurals=2; plural=n > 1\n"
+"Language: pt\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
+"Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Plural-Forms: nplurals=2; plural=n > 1;\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 msgid ""
 "\n"
 "            <i>The table below reflects actions recorded prior to disabling "
 "project history. You can\n"
 "            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
 "target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
@@ -55,15 +54,15 @@
 msgid "%(name)s is part of this project again"
 msgstr "%(name)s faz parte deste projeto novamente"
 
 msgid "?"
 msgstr "?"
 
 msgid "A link to an external document, related to this bill"
-msgstr "Ligação para um documento externo, relacionado à essa conta"
+msgstr "Ligação para um documento externo, relacionado a essa fatura"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your emails."
 msgstr ""
 "Uma ligação para redefinir a sua palavra-passe foi enviado a si, por favor "
 "verifique os seus e-mails."
 
@@ -83,18 +82,18 @@
 msgid "Actions"
 msgstr "Ações"
 
 msgid "Add"
 msgstr "Adicionar"
 
 msgid "Add a bill"
-msgstr "Adicionar uma conta"
+msgstr "Adicionar uma fatura"
 
 msgid "Add a new bill"
-msgstr "Adicionar uma nova conta"
+msgstr "Adicionar uma nova fatura"
 
 msgid "Add participant"
 msgstr "Adicionar participante"
 
 msgid "Added on %(date)s"
 msgstr "Adicionado em %(date)s"
 
@@ -109,17 +108,14 @@
 
 msgid "Amount"
 msgstr "Quantia"
 
 msgid "Amount in %(currency)s"
 msgstr "Quantia em %(currency)s"
 
-msgid "Amount paid"
-msgstr "Quantia paga"
-
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
 "                The rest of the project history will be unaffected. This "
 "action cannot be undone."
 msgstr ""
 "Tem certeza que deseja apagar todos os endereços IP gravados deste projeto?\n"
@@ -129,35 +125,72 @@
 msgid ""
 "Are you sure you want to erase all history for this project? This action "
 "cannot be undone."
 msgstr ""
 "Tem certeza que deseja apagar todo o histórico deste projeto? Esta ação não "
 "pode ser desfeita."
 
+msgid "Authentication"
+msgstr "Autenticação"
+
 msgid "Back to the list"
 msgstr "Voltar para a lista"
 
 msgid "Balance"
 msgstr "Saldo"
 
+msgid "Bill %(name)s added"
+msgstr "Conta %(name)s adicionada"
+
+msgid "Bill %(name)s changed in an unknown way"
+msgstr "Conta %(name)s modificado de maneira desconhecida"
+
+msgid "Bill %(name)s modified"
+msgstr "Conta %(name)s modificada"
+
+msgid "Bill %(name)s removed"
+msgstr "Fatura %(name)s removida"
+
+msgid "Bill %(name)s renamed to %(new_description)s"
+msgstr "Fatura %(name)s renomeada a %(new_description)s"
+
+msgid "Bill %(name)s: %(property_name)s changed from %(before)s to %(after)s"
+msgstr "Fatura %(name)s: %(property_name)s alterado de %(before)s a %(after)s"
+
+msgid "Bill %(name)s: %(property_name)s changed to %(after)s"
+msgstr "Fatura %(name)s: %(property_name)s alterado a %(after)s"
+
+msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
+msgstr ""
+"Fatura %(name)s: adicionado %(owers_list_str)s à lista de proprietários"
+
+msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
+msgstr "Fatura %(name)s: removido %(owers_list_str)s da lista de proprietários"
+
 msgid "Bill items"
-msgstr "Itens da conta"
+msgstr "Itens da fatura"
 
 msgid "Bills"
 msgstr "Contas"
 
 msgid "Bills can't be null"
 msgstr "Contas não podem ser null"
 
 msgid "Can't remember the password?"
 msgstr "Esqueceu a palavra-passe?"
 
 msgid "Cancel"
 msgstr "Cancelar"
 
+msgid ""
+"Cannot add bills in multiple currencies to a project without default currency"
+msgstr ""
+"Não é possível adicionar faturas em várias moedas a um projeto sem moeda "
+"padrão"
+
 msgid "Choose file"
 msgstr "Escolher ficheiro"
 
 msgid "Clear Project History"
 msgstr "Limpar Histórico do Projeto"
 
 msgid "Close"
@@ -165,14 +198,17 @@
 
 msgid "Code"
 msgstr "Código"
 
 msgid "Confirm Remove IP Adresses"
 msgstr "Confirmar a remoção dos Endereços IP"
 
+msgid "Confirm deletion"
+msgstr "Confirmar exclusão"
+
 msgid "Create"
 msgstr "Criar"
 
 msgid "Create a new project"
 msgstr "Criar um projeto"
 
 msgid "Create the project"
@@ -192,17 +228,26 @@
 
 msgid "Delete Confirmation"
 msgstr "Deletar Confirmação"
 
 msgid "Delete Stored IP Addresses"
 msgstr "Deletar endereços IP gravados"
 
+msgid "Delete project"
+msgstr "Apagarr projeto"
+
 msgid "Delete stored IP addresses"
 msgstr "Deletar endereços IP gravados"
 
+msgid "Deleted project history."
+msgstr "Histórico do projeto apagado."
+
+msgid "Deleted recorded IP addresses in project history."
+msgstr "Endereços IP gravados apagados no histórico do projeto."
+
 msgid "Disabled IP Address Recording"
 msgstr "Gravação do Endereço IP Desativada"
 
 msgid "Disabled Project History"
 msgstr "Histórico do Projeto Desativado"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -217,32 +262,39 @@
 msgstr ""
 "Não reutilize uma palavra-passe pessoal. Escolha um código privado e envie-o "
 "para seus amigos"
 
 msgid "Download"
 msgstr "Descarregar"
 
+msgid "Download Mobile Application"
+msgstr "Descarregar Aplicação Mobile"
+
 msgid "Download project's data"
 msgstr "Descarregar dados do projeto"
 
 msgid "Download the list of bills with owner, amount, reason,... "
-msgstr "Descarregar a lista de contas com dono, quantia, motivo,... "
+msgstr "Descarregar a lista de faturas com dono, quantia, motivo,... "
 
 msgid "Download the list of transactions needed to settle the current bills."
 msgstr ""
-"Descarregar a lista de transações necessárias para liquidar as contas atuais."
+"Descarregar a lista de transações necessárias para liquidar as faturas "
+"atuais."
 
 msgid "Edit project"
 msgstr "Editar projeto"
 
 msgid "Edit the project"
 msgstr "Editar o projeto"
 
 msgid "Edit this bill"
-msgstr "Editar esta conta"
+msgstr "Editar esta fatura"
+
+msgid "Edit this participant"
+msgstr "Editar este participante"
 
 msgid "Email"
 msgstr "E-mail"
 
 msgid "Enable project history"
 msgstr "Ativar histórico do projeto"
 
@@ -251,14 +303,38 @@
 
 msgid "Enabled Project History"
 msgstr "Histórico do Projeto Ativado"
 
 msgid "Enabled Project History & IP Address Recording"
 msgstr "Histórico do Projeto Ativado & Gravação do Endereço IP"
 
+msgid "Enter a new code if you want to change it"
+msgstr "Digite um novo código se quiser alterá-lo"
+
+msgid "Enter private code to confirm deletion"
+msgstr "Digite o código privado para confirmar a exclusão"
+
+msgid "Error activating participant"
+msgstr "Erro ao ativar o participante"
+
+msgid "Error deleting bill"
+msgstr "Erro ao apagar a fatura"
+
+msgid "Error deleting project"
+msgstr "Erro ao apagar o projeto"
+
+msgid "Error deleting project history"
+msgstr "Erro ao apagar o histórico do projeto"
+
+msgid "Error deleting recorded IP addresses"
+msgstr "Erro ao apagar endereços IP gravados"
+
+msgid "Error removing participant"
+msgstr "Erro ao remover o participante"
+
 msgid "Event"
 msgstr "Evento"
 
 msgid "Everyone"
 msgstr "Todos"
 
 msgid "Everyone but %(excluded)s"
@@ -278,14 +354,17 @@
 
 msgid "From IP"
 msgstr "Do IP"
 
 msgid "Get in"
 msgstr "Entrar"
 
+msgid "Get it on"
+msgstr "Vamos"
+
 msgid "Going on holidays with friends?"
 msgstr "Indo para o feriado com os amigos?"
 
 msgid "History"
 msgstr "Histórico"
 
 msgid "History Settings Changed"
@@ -300,38 +379,32 @@
 
 msgid "IP address recording can be enabled on the settings page"
 msgstr "A gravação do endereço IP pode ser ativada na página de configurações"
 
 msgid "Identifier:"
 msgstr "Identificador:"
 
-msgid "Import"
-msgstr "Importar"
-
-msgid "Import JSON"
-msgstr "Importar JSON"
-
-msgid "Import previously exported JSON file"
-msgstr "Importar ficheiro JSON exportado anteriormente"
-
-msgid "Invalid JSON"
-msgstr "JSON inválido"
+msgid "Invalid private code."
+msgstr "Código privado inválido."
 
 msgid "Invalid token"
 msgstr "Token inválido"
 
 msgid "Invite people"
 msgstr "Convidar pessoas"
 
 msgid "Invite people to join this project"
 msgstr "Convide pessoas para participar deste projeto"
 
 msgid "Languages"
 msgstr "Linguagens"
 
+msgid "Legal information"
+msgstr "Informações legais"
+
 msgid "Log in"
 msgstr "Conecte-se"
 
 msgid "Log in to an existing project"
 msgstr "Conecte-se num projeto existente"
 
 msgid "Logout"
@@ -339,66 +412,117 @@
 
 msgid "Manage your shared <br />expenses, easily"
 msgstr "Modifique suas despesas <br />compartilhadas, facilmente"
 
 msgid "Mobile Application"
 msgstr "Aplicação Mobile"
 
+msgid "More options"
+msgstr "Mais opções"
+
 msgid "Name"
 msgstr "Nome"
 
+msgid "New private code"
+msgstr "Código privado novo"
+
 msgid "Newer bills"
 msgstr "Contas mais recentes"
 
 msgid "Newest bill"
 msgstr "Conta mais recente"
 
 msgid "No Currency"
 msgstr "Sem Moeda"
 
 msgid "No IP Addresses to erase"
 msgstr "Não há endereços IP para apagar"
 
 msgid "No bills"
-msgstr "Sem contas"
+msgstr "Sem faturas"
 
 msgid "No history to erase"
 msgstr "Não há histórico para apagar"
 
+msgid "No one"
+msgstr "Ninguem"
+
 msgid "No token provided"
 msgstr "Nenhum token fornecido"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Expressão ou montante inválido. Apenas números e os operadores +=*/ são "
-"aceitos."
+"aceites."
 
 msgid "Nothing to list"
 msgstr "Nada a listar"
 
 msgid "Nothing to list yet."
 msgstr "Nada para listar ainda."
 
 msgid "Number of bills"
-msgstr "Quantidade de contas"
+msgstr "Quantidade de faturas"
+
+msgid "Number of participants"
+msgstr "Quantidade de participantes"
 
 msgid "Older bills"
 msgstr "Contas mais antigas"
 
 msgid "Oldest bill"
 msgstr "Conta mais antiga"
 
 msgid "Other projects :"
 msgstr "Outros projetos:"
 
 msgid "Paid"
 msgstr "Pago"
 
+msgid "Participant %(name)s added"
+msgstr "Participante %(name)s adicionado"
+
+msgid "Participant %(name)s changed in an unknown way"
+msgstr "Participante %(name)s modificado de maneira desconhecida"
+
+msgid "Participant %(name)s deactivated"
+msgstr "Participante %(name)s desativado"
+
+msgid "Participant %(name)s modified"
+msgstr "Participante %(name)s modificado"
+
+msgid "Participant %(name)s reactivated"
+msgstr "Participante %(name)s reativado"
+
+msgid "Participant %(name)s removed"
+msgstr "Participante %(name)s removido"
+
+msgid "Participant %(name)s renamed to %(new_name)s"
+msgstr "Participante %(name)s renomeado a %(new_name)s"
+
+msgid ""
+"Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
+msgstr ""
+"Participante %(name)s: peso alterado de %(old_weight)s a %(new_weight)s"
+
+msgid ""
+"Participant '%(name)s' has been deactivated. It will still appear in the "
+"list until its balance reach zero."
+msgstr ""
+"O participante '%(name)s' foi desativado. Ele ainda aparecerá na lista até "
+"que o saldo dele seja zero."
+
+msgid "Participant '%(name)s' has been modified"
+msgstr "O participante '%(name)s' foi modificado"
+
+msgid "Participant '%(name)s' has been removed"
+msgstr "O participante '%(name)s' foi removido"
+
 msgid "Password"
 msgstr "Palavra-passe"
 
 msgid "Password confirmation"
 msgstr "Confirmação da palavra-passe"
 
 msgid "Password mismatch"
@@ -409,38 +533,56 @@
 
 msgid "Password successfully reset."
 msgstr "Palavra-passe redefinida corretamente."
 
 msgid "Payer"
 msgstr "Pagador"
 
+msgid "People to notify"
+msgstr "Pessoas a notificar"
+
 msgid "Period"
 msgstr "Período"
 
+msgid "Please, validate the captcha to proceed."
+msgstr "Por favor, valide o captcha para prosseguir."
+
 msgid "Privacy Settings"
 msgstr "Configurações de Privacidade"
 
 msgid "Private code"
 msgstr "Código privado"
 
 msgid "Project"
 msgstr "Projeto"
 
+msgid "Project %(name)s added"
+msgstr "Projeto %(name)s adicionado"
+
+msgid "Project %(name)s changed in an unknown way"
+msgstr "Projeto %(name)s modificado de maneira desconhecida"
+
+msgid "Project contact email changed to %(new_email)s"
+msgstr "O email de contato do projeto foi alterado para %(new_email)s"
+
 msgid "Project default: %(currency)s"
 msgstr "Projeto predefinido: %(currency)s"
 
 msgid "Project identifier"
 msgstr "Identificador do projeto"
 
 msgid "Project name"
 msgstr "Nome do projeto"
 
 msgid "Project private code changed"
 msgstr "Código privado do projeto alterado"
 
+msgid "Project renamed to %(new_project_name)s"
+msgstr "Projeto renomeado a %(new_project_name)s"
+
 msgid "Project settings modified"
 msgstr "Configurações do projeto alteradas"
 
 msgid "Project successfully deleted"
 msgstr "Projeto deletado com sucesso"
 
 msgid "Project successfully uploaded"
@@ -466,14 +608,17 @@
 
 msgid "Send the invitations"
 msgstr "Enviar os convites"
 
 msgid "Send via Emails"
 msgstr "Enviar via E-mails"
 
+msgid "Setting a default currency enables currency conversion between bills"
+msgstr "Definir uma moeda padrão permite a conversão de moeda entre faturas"
+
 msgid "Settings"
 msgstr "Configurações"
 
 msgid "Settle"
 msgstr "Estabelecer"
 
 msgid "Settle plans"
@@ -494,30 +639,14 @@
 msgstr ""
 "Algumas das entradas abaixo contém endereços IP, mesmo este projeto tendo a "
 "gravação de IP desativada. "
 
 msgid "Someone probably cleared the project history."
 msgstr "Alguém provavelmente limpou o histórico do projeto."
 
-msgid ""
-"Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
-msgstr ""
-"Desculpe, houve um erro ao te enviar um email com as instruções de "
-"redefinição de palavra-passe. Por favor, confira a configuração de e-mail do "
-"servidor ou entre em contato com um administrador."
-
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. Please "
-"check the email configuration of the server or contact the administrator."
-msgstr ""
-"Desculpe, houve um erro ao enviar os convites via e-mail. Por favor, confira "
-"a configuração de email do servidor ou entre em contato com um administrador."
-
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "Desculpe, não foi possível encontrar a página que solicitou."
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify about "
 "the\n"
 "                creation of this budget management project and we will send "
@@ -547,55 +676,67 @@
 msgstr "O Painel de Controle atualmente está desativado."
 
 msgid "The best thing to do is probably to get back to the main page."
 msgstr ""
 "É provável que a melhor coisa a fazer seja voltar para a página inicial."
 
 msgid "The bill has been added"
-msgstr "A conta foi adicionada"
+msgstr "A fatura foi adicionada"
 
 msgid "The bill has been deleted"
-msgstr "A conta foi deletada"
+msgstr "A fatura foi apagada"
 
 msgid "The bill has been modified"
-msgstr "A conta foi modificada"
+msgstr "A fatura foi modificada"
 
 msgid "The email %(email)s is not valid"
 msgstr "O email %(email)s não é válido"
 
-msgid "The project identifier is %(project)s"
-msgstr "O identificador do projeto é %(project)s"
+msgid "The participant name is invalid"
+msgstr "O nome do participante é inválido"
 
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "O projeto que está tentando acessar não existe, quer"
 
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "Esta palavra-passe de administrador não é a correta. Apenas %(num)d "
 "tentativas restantes."
 
 msgid "This private code is not the right one"
 msgstr "Este código privado não é o correto"
 
+msgid "This project already have this participant"
+msgstr "Este projeto já tem este participante"
+
+msgid ""
+"This project cannot be set to 'no currency' because it contains bills in "
+"multiple currencies."
+msgstr ""
+"Este projeto não pode ser definido como 'sem moeda' porque contém faturas em "
+"várias moedas."
+
 msgid "This project does not exists"
 msgstr "Este projeto não existe"
 
+msgid "This will remove all bills and participants in this project!"
+msgstr "Isso removerá todas as faturas e os participantes deste projeto!"
+
 msgid "Time"
 msgstr "Tempo"
 
 msgid "To whom?"
 msgstr "A quem?"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr ""
-"Muitas tentativas de login falhas, por favor, tente novamente mais tarde."
-
 msgid "Try out the demo"
 msgstr "Experimente a demonstração"
 
+msgid "Unknown error"
+msgstr "Erro desconhecido"
+
 msgid "Unknown project"
 msgstr "Projeto desconhecido"
 
 msgid "Use IP tracking for project history"
 msgstr "Usar rastreamento de IP para o histórico do projeto"
 
 msgid "We can help!"
@@ -616,14 +757,17 @@
 
 msgid "What?"
 msgstr "O quê?"
 
 msgid "When?"
 msgstr "Quando?"
 
+msgid "Which is a real currency: Euro or Petro dollar?"
+msgstr "Qual é uma moeda real: Euro ou Petrodólar?"
+
 msgid "Who paid?"
 msgstr "Quem pagou?"
 
 msgid "Who pays?"
 msgstr "Quem paga?"
 
 msgid "Who?"
@@ -659,15 +803,15 @@
 msgid "Your invitations have been sent"
 msgstr "Seus convites foram enviados"
 
 msgid "Your projects"
 msgstr "Seus projetos"
 
 msgid "add a bill"
-msgstr "adicionar uma conta"
+msgstr "adicionar uma fatura"
 
 msgid "add participants"
 msgstr "adicionar participantes"
 
 msgid "can't remember your password?"
 msgstr "não se consegue lembrar da sua palavra-passe?"
 
@@ -679,14 +823,17 @@
 
 msgid "delete"
 msgstr "deletar"
 
 msgid "edit"
 msgstr "editar"
 
+msgid "euro"
+msgstr "euro"
+
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "flano.tal@exemplo.com, flana.maria@site.com"
 
 msgid "reactivate"
 msgstr "reativar"
 
 msgid "show"
@@ -696,7 +843,25 @@
 msgstr "mudar para"
 
 msgid "you can contribute and improve it!"
 msgstr "Pode contribuir para melhorá-lo!"
 
 msgid "you sure?"
 msgstr "tem certeza?"
+
+msgid "{dual_object_0} and {dual_object_1}"
+msgstr "{dual_object_0} e {dual_object_1"
+
+msgid "{prefix}: {error}"
+msgstr "{prefix}: {error}"
+
+msgid "{prefix}:<br />{errors}"
+msgstr "{prefix}:<br />{errors}"
+
+msgid "{previous_object}, and {end_object}"
+msgstr "{previous_object} e {end_object}"
+
+msgid "{previous_object}, {next_object}"
+msgstr "{previous_object}, {next_object}"
+
+msgid "{start_object}, {next_object}"
+msgstr "{start_object}, {next_object}"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/pt/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/pt/LC_MESSAGES/messages.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,61 @@
-
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2020-10-05 12:12+0000\n"
-"Last-Translator: ssantos <ssantos@web.de>\n"
+"PO-Revision-Date: 2023-05-05 00:47+0000\n"
+"Last-Translator: MurkBRA <anjo1077@gmail.com>\n"
+"Language-Team: Portuguese <https://hosted.weblate.org/projects/i-hate-money/"
+"i-hate-money/pt/>\n"
 "Language: pt\n"
-"Language-Team: Portuguese <https://hosted.weblate.org/projects/i-hate-"
-"money/i-hate-money/pt/>\n"
-"Plural-Forms: nplurals=2; plural=n > 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=n > 1;\n"
+"X-Generator: Weblate 4.18-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Expressão ou montante inválido. Apenas números e os operadores +=*/ são "
-"aceitos."
+"aceites."
 
 msgid "Project name"
 msgstr "Nome do projeto"
 
-#, fuzzy
 msgid "New private code"
-msgstr "Código privado"
+msgstr "Código privado novo"
 
 msgid "Enter a new code if you want to change it"
-msgstr ""
+msgstr "Digite um novo código se quiser alterá-lo"
 
 msgid "Email"
 msgstr "E-mail"
 
 msgid "Enable project history"
 msgstr "Ativar histórico do projeto"
 
 msgid "Use IP tracking for project history"
 msgstr "Usar rastreamento de IP para o histórico do projeto"
 
 msgid "Default Currency"
 msgstr "Moeda predefinida"
 
 msgid "Setting a default currency enables currency conversion between bills"
-msgstr ""
+msgstr "Definir uma moeda padrão permite a conversão de moeda entre faturas"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
+"Este projeto não pode ser definido como 'sem moeda' porque contém faturas em "
+"várias moedas."
 
 msgid "Import previously exported JSON file"
 msgstr "Importar ficheiro JSON exportado anteriormente"
 
 msgid "Import"
 msgstr "Importar"
 
@@ -72,33 +73,30 @@
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
 msgstr ""
 "Um projeto com este identificador (\"%(project)s\") já existe. Por favor "
 "escolha um novo identificador"
 
 msgid "Which is a real currency: Euro or Petro dollar?"
-msgstr ""
+msgstr "Qual é uma moeda real: Euro ou Petrodólar?"
 
-#, fuzzy
 msgid "euro"
-msgstr "Período"
+msgstr "euro"
 
 msgid "Please, validate the captcha to proceed."
-msgstr ""
+msgstr "Por favor, valide o captcha para prosseguir."
 
 msgid "Enter private code to confirm deletion"
-msgstr ""
+msgstr "Digite o código privado para confirmar a exclusão"
 
-#, fuzzy
 msgid "Unknown error"
-msgstr "Projeto desconhecido"
+msgstr "Erro desconhecido"
 
-#, fuzzy
 msgid "Invalid private code."
-msgstr "Código privado"
+msgstr "Código privado inválido."
 
 msgid "Get in"
 msgstr "Entrar"
 
 msgid "Admin password"
 msgstr "Palavra-passe do administrador"
 
@@ -135,15 +133,15 @@
 msgid "Currency"
 msgstr "Moeda"
 
 msgid "External link"
 msgstr "Ligação externa"
 
 msgid "A link to an external document, related to this bill"
-msgstr "Ligação para um documento externo, relacionado à essa conta"
+msgstr "Ligação para um documento externo, relacionado a essa fatura"
 
 msgid "For whom?"
 msgstr "Para quem?"
 
 msgid "Submit"
 msgstr "Enviar"
 
@@ -165,70 +163,69 @@
 
 msgid "Weight"
 msgstr "Peso"
 
 msgid "Add"
 msgstr "Adicionar"
 
-#, fuzzy
 msgid "The participant name is invalid"
-msgstr "Utilizador '%(name)s' foi removido"
+msgstr "O nome do participante é inválido"
 
-#, fuzzy
 msgid "This project already have this participant"
-msgstr "Este projeto já tem este membro"
+msgstr "Este projeto já tem este participante"
 
 msgid "People to notify"
-msgstr ""
+msgstr "Pessoas a notificar"
 
 msgid "Send invites"
 msgstr "Enviar convites"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "O email %(email)s não é válido"
 
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
-msgstr ""
+msgstr "{dual_object_0} e {dual_object_1"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
-msgstr ""
+msgstr "{previous_object} e {end_object}"
 
 #. Two items in a middle of a list with more than 5 objects
 msgid "{previous_object}, {next_object}"
-msgstr ""
+msgstr "{previous_object}, {next_object}"
 
 #. First two items of a list with more than 3 items
 msgid "{start_object}, {next_object}"
-msgstr ""
+msgstr "{start_object}, {next_object}"
 
 msgid "No Currency"
 msgstr "Sem Moeda"
 
 #. Form error with only one error
 msgid "{prefix}: {error}"
-msgstr ""
+msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
-msgstr ""
+msgstr "{prefix}:<br />{errors}"
 
 msgid "Too many failed login attempts, please retry later."
 msgstr "Muitas tentativas de login falhas, por favor, tente novamente mais tarde."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "Esta palavra-passe de administrador não é a correta. Apenas %(num)d "
 "tentativas restantes."
 
+#, fuzzy
 msgid "Provided token is invalid"
-msgstr ""
+msgstr "O token fornecido é inválido"
 
 msgid "This private code is not the right one"
 msgstr "Este código privado não é o correto"
 
 #, python-format
 msgid "You have just created '%(project)s' to share your expenses"
 msgstr "Acabou de criar '%(project)s' para compartilhar as suas despesas"
@@ -274,20 +271,22 @@
 msgid "Invalid JSON"
 msgstr "JSON inválido"
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
+"Não é possível adicionar faturas em várias moedas a um projeto sem moeda "
+"padrão"
 
 msgid "Project successfully deleted"
 msgstr "Projeto deletado com sucesso"
 
 msgid "Error deleting project"
-msgstr ""
+msgstr "Erro ao apagar o projeto"
 
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "Foi convidado a compartilhar suas despesas com %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "Seus convites foram enviados"
@@ -302,81 +301,77 @@
 "administrador."
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr "%(member)s foram adicionados"
 
 msgid "Error activating participant"
-msgstr ""
+msgstr "Erro ao ativar o participante"
 
 #, python-format
 msgid "%(name)s is part of this project again"
 msgstr "%(name)s faz parte deste projeto novamente"
 
 msgid "Error removing participant"
-msgstr ""
+msgstr "Erro ao remover o participante"
 
-#, fuzzy, python-format
+#, python-format
 msgid ""
 "Participant '%(name)s' has been deactivated. It will still appear in the "
 "list until its balance reach zero."
 msgstr ""
-"Utilizador '%(name)s' foi desativado. Ele continuará aparecendo na lista "
-"de utilizadores até que o seu balanço seja zero."
+"O participante '%(name)s' foi desativado. Ele ainda aparecerá na lista até "
+"que o saldo dele seja zero."
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant '%(name)s' has been removed"
-msgstr "Utilizador '%(name)s' foi removido"
+msgstr "O participante '%(name)s' foi removido"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant '%(name)s' has been modified"
-msgstr "Utilizador '%(name)s' foi removido"
+msgstr "O participante '%(name)s' foi modificado"
 
 msgid "The bill has been added"
-msgstr "A conta foi adicionada"
+msgstr "A fatura foi adicionada"
 
 msgid "Error deleting bill"
-msgstr ""
+msgstr "Erro ao apagar a fatura"
 
 msgid "The bill has been deleted"
-msgstr "A conta foi deletada"
+msgstr "A fatura foi apagada"
 
 msgid "The bill has been modified"
-msgstr "A conta foi modificada"
+msgstr "A fatura foi modificada"
 
-#, fuzzy
 msgid "Error deleting project history"
-msgstr "Ativar histórico do projeto"
+msgstr "Erro ao apagar o histórico do projeto"
 
-#, fuzzy
 msgid "Deleted project history."
-msgstr "Ativar histórico do projeto"
+msgstr "Histórico do projeto apagado."
 
-#, fuzzy
 msgid "Error deleting recorded IP addresses"
-msgstr "Deletar endereços IP gravados"
+msgstr "Erro ao apagar endereços IP gravados"
 
 msgid "Deleted recorded IP addresses in project history."
-msgstr ""
+msgstr "Endereços IP gravados apagados no histórico do projeto."
 
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "Desculpe, não foi possível encontrar a página que solicitou."
 
 msgid "The best thing to do is probably to get back to the main page."
 msgstr "É provável que a melhor coisa a fazer seja voltar para a página inicial."
 
 msgid "Back to the list"
 msgstr "Voltar para a lista"
 
 msgid "Administration tasks are currently disabled."
 msgstr "Tarefas de administração estão atualmente desativadas."
 
-#, fuzzy
 msgid "Authentication"
-msgstr "Documentação"
+msgstr "Autenticação"
 
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "O projeto que está tentando acessar não existe, quer"
 
 msgid "create it"
 msgstr "Criar"
 
@@ -385,20 +380,19 @@
 
 msgid "Create a new project"
 msgstr "Criar um projeto"
 
 msgid "Project"
 msgstr "Projeto"
 
-#, fuzzy
 msgid "Number of participants"
-msgstr "adicionar participantes"
+msgstr "Quantidade de participantes"
 
 msgid "Number of bills"
-msgstr "Quantidade de contas"
+msgstr "Quantidade de faturas"
 
 msgid "Newest bill"
 msgstr "Conta mais recente"
 
 msgid "Oldest bill"
 msgstr "Conta mais antiga"
 
@@ -413,54 +407,50 @@
 
 msgid "show"
 msgstr "exibir"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "O Painel de Controle atualmente está desativado."
 
-#, fuzzy
 msgid "Download Mobile Application"
-msgstr "Aplicação Mobile"
+msgstr "Descarregar Aplicação Mobile"
 
-#, fuzzy
 msgid "Get it on"
-msgstr "Entrar"
+msgstr "Vamos"
 
-#, fuzzy
 msgid "Are you sure?"
-msgstr "tem certeza?"
+msgstr "Tem certeza?"
 
 msgid "Edit project"
 msgstr "Editar projeto"
 
-#, fuzzy
 msgid "Delete project"
-msgstr "Editar projeto"
+msgstr "Apagarr projeto"
 
 msgid "Import JSON"
 msgstr "Importar JSON"
 
 msgid "Choose file"
 msgstr "Escolher ficheiro"
 
 msgid "Download project's data"
 msgstr "Descarregar dados do projeto"
 
 msgid "Bill items"
-msgstr "Itens da conta"
+msgstr "Itens da fatura"
 
 msgid "Download the list of bills with owner, amount, reason,... "
-msgstr "Descarregar a lista de contas com dono, quantia, motivo,... "
+msgstr "Descarregar a lista de faturas com dono, quantia, motivo,... "
 
 msgid "Settle plans"
 msgstr "Estabelecer planos"
 
 msgid "Download the list of transactions needed to settle the current bills."
 msgstr ""
-"Descarregar a lista de transações necessárias para liquidar as contas "
+"Descarregar a lista de transações necessárias para liquidar as faturas "
 "atuais."
 
 msgid "Can't remember the password?"
 msgstr "Esqueceu a palavra-passe?"
 
 msgid "Cancel"
 msgstr "Cancelar"
@@ -468,37 +458,36 @@
 msgid "Privacy Settings"
 msgstr "Configurações de Privacidade"
 
 msgid "Edit the project"
 msgstr "Editar o projeto"
 
 msgid "This will remove all bills and participants in this project!"
-msgstr ""
+msgstr "Isso removerá todas as faturas e os participantes deste projeto!"
 
 msgid "Edit this bill"
-msgstr "Editar esta conta"
+msgstr "Editar esta fatura"
 
 msgid "Add a bill"
-msgstr "Adicionar uma conta"
+msgstr "Adicionar uma fatura"
 
 msgid "Everyone"
 msgstr "Todos"
 
 msgid "No one"
-msgstr ""
+msgstr "Ninguem"
 
 msgid "More options"
-msgstr ""
+msgstr "Mais opções"
 
 msgid "Add participant"
 msgstr "Adicionar participante"
 
-#, fuzzy
 msgid "Edit this participant"
-msgstr "Adicionar participante"
+msgstr "Editar este participante"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "flano.tal@exemplo.com, flana.maria@site.com"
 
 msgid "Send the invitations"
 msgstr "Enviar os convites"
 
@@ -524,19 +513,19 @@
 msgstr "Gravação do Endereço IP Ativada"
 
 msgid "History Settings Changed"
 msgstr "Configurações do Histórico Alteradas"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed from %(before)s to %(after)s"
-msgstr ""
+msgstr "Fatura %(name)s: %(property_name)s alterado de %(before)s a %(after)s"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed to %(after)s"
-msgstr ""
+msgstr "Fatura %(name)s: %(property_name)s alterado a %(after)s"
 
 msgid "Confirm Remove IP Adresses"
 msgstr "Confirmar a remoção dos Endereços IP"
 
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
@@ -544,17 +533,16 @@
 "action cannot be undone."
 msgstr ""
 "Tem certeza que deseja apagar todos os endereços IP gravados deste "
 "projeto?\n"
 "                O resto do histórico do projeto não será afetado. Esta "
 "ação não pode ser desfeita."
 
-#, fuzzy
 msgid "Confirm deletion"
-msgstr "Confirmar apagar"
+msgstr "Confirmar exclusão"
 
 msgid "Close"
 msgstr "Fechar"
 
 msgid "Delete Confirmation"
 msgstr "Deletar Confirmação"
 
@@ -563,19 +551,19 @@
 "cannot be undone."
 msgstr ""
 "Tem certeza que deseja apagar todo o histórico deste projeto? Esta ação "
 "não pode ser desfeita."
 
 #, python-format
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
-msgstr ""
+msgstr "Fatura %(name)s: adicionado %(owers_list_str)s à lista de proprietários"
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
-msgstr ""
+msgstr "Fatura %(name)s: removido %(owers_list_str)s da lista de proprietários"
 
 #, python-format
 msgid ""
 "\n"
 "            <i>This project has history disabled. New actions won't "
 "appear below. You can enable history on the</i>\n"
 "            <a href=\"%(url)s\">settings page</a>\n"
@@ -637,94 +625,94 @@
 
 msgid "IP address recording can be disabled on the settings page"
 msgstr "A gravação do endereço IP pode ser desativada na página de configurações"
 
 msgid "From IP"
 msgstr "Do IP"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project %(name)s added"
-msgstr "Nome do projeto"
+msgstr "Projeto %(name)s adicionado"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s added"
-msgstr "A conta foi adicionada"
+msgstr "Conta %(name)s adicionada"
 
 #, python-format
 msgid "Participant %(name)s added"
-msgstr ""
+msgstr "Participante %(name)s adicionado"
 
 msgid "Project private code changed"
 msgstr "Código privado do projeto alterado"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project renamed to %(new_project_name)s"
-msgstr "O identificador do projeto é %(new_project_name)s"
+msgstr "Projeto renomeado a %(new_project_name)s"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project contact email changed to %(new_email)s"
-msgstr "O email de contato do projeto foi alterado para"
+msgstr "O email de contato do projeto foi alterado para %(new_email)s"
 
 msgid "Project settings modified"
 msgstr "Configurações do projeto alteradas"
 
 #, python-format
 msgid "Participant %(name)s deactivated"
-msgstr ""
+msgstr "Participante %(name)s desativado"
 
 #, python-format
 msgid "Participant %(name)s reactivated"
-msgstr ""
+msgstr "Participante %(name)s reativado"
 
 #, python-format
 msgid "Participant %(name)s renamed to %(new_name)s"
-msgstr ""
+msgstr "Participante %(name)s renomeado a %(new_name)s"
 
 #, python-format
 msgid "Bill %(name)s renamed to %(new_description)s"
-msgstr ""
+msgstr "Fatura %(name)s renomeada a %(new_description)s"
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
-msgstr ""
+msgstr "Participante %(name)s: peso alterado de %(old_weight)s a %(new_weight)s"
 
 msgid "Amount"
 msgstr "Quantia"
 
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "Quantia em %(currency)s"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s modified"
-msgstr "A conta foi modificada"
+msgstr "Conta %(name)s modificada"
 
 #, python-format
 msgid "Participant %(name)s modified"
-msgstr ""
+msgstr "Participante %(name)s modificado"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s removed"
-msgstr "Utilizador '%(name)s' foi removido"
+msgstr "Fatura %(name)s removida"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant %(name)s removed"
-msgstr "Utilizador '%(name)s' foi removido"
+msgstr "Participante %(name)s removido"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project %(name)s changed in an unknown way"
-msgstr "modificado de maneira desconhecida"
+msgstr "Projeto %(name)s modificado de maneira desconhecida"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s changed in an unknown way"
-msgstr "modificado de maneira desconhecida"
+msgstr "Conta %(name)s modificado de maneira desconhecida"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant %(name)s changed in an unknown way"
-msgstr "modificado de maneira desconhecida"
+msgstr "Participante %(name)s modificado de maneira desconhecida"
 
 msgid "Nothing to list"
 msgstr "Nada a listar"
 
 msgid "Someone probably cleared the project history."
 msgstr "Alguém provavelmente limpou o histórico do projeto."
 
@@ -812,17 +800,16 @@
 
 msgid "Documentation"
 msgstr "Documentação"
 
 msgid "Administation Dashboard"
 msgstr "Painel de Administração"
 
-#, fuzzy
 msgid "Legal information"
-msgstr "Deletar Confirmação"
+msgstr "Informações legais"
 
 msgid "\"I hate money\" is free software"
 msgstr "\"I hate money\" é um software livre"
 
 msgid "you can contribute and improve it!"
 msgstr "Pode contribuir para melhorá-lo!"
 
@@ -836,15 +823,15 @@
 msgid "Invite people"
 msgstr "Convidar pessoas"
 
 msgid "You should start by adding participants"
 msgstr "Deveria começar adicionando pessoas"
 
 msgid "Add a new bill"
-msgstr "Adicionar uma nova conta"
+msgstr "Adicionar uma nova fatura"
 
 msgid "Newer bills"
 msgstr "Contas mais recentes"
 
 msgid "Older bills"
 msgstr "Contas mais antigas"
 
@@ -865,24 +852,24 @@
 msgstr "Adicionado em %(date)s"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr "Todos menos %(excluded)s"
 
 msgid "No bills"
-msgstr "Sem contas"
+msgstr "Sem faturas"
 
 msgid "Nothing to list yet."
 msgstr "Nada para listar ainda."
 
 msgid "You probably want to"
 msgstr "Provavelmente gostaria de"
 
 msgid "add a bill"
-msgstr "adicionar uma conta"
+msgstr "adicionar uma fatura"
 
 msgid "add participants"
 msgstr "adicionar participantes"
 
 msgid "Password reminder"
 msgstr "Lembrete de palavra-passe"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.mo`

 * *Files 19% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Portuguese (Brazil) <https://hosted.weblate.org/projects/i-"
 "hate-money/i-hate-money/pt_BR/>\n"
 "Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.12-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 msgid ""
 "\n"
 "            <i>The table below reflects actions recorded prior to disabling "
 "project history. You can\n"
 "            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
 "target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
@@ -108,17 +108,14 @@
 
 msgid "Amount"
 msgstr "Quantia"
 
 msgid "Amount in %(currency)s"
 msgstr "Quantia em %(currency)s"
 
-msgid "Amount paid"
-msgstr "Quantia paga"
-
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
 "                The rest of the project history will be unaffected. This "
 "action cannot be undone."
 msgstr ""
 "Você tem certeza que deseja deletar todos os endereços IP gravados deste "
@@ -129,14 +126,17 @@
 msgid ""
 "Are you sure you want to erase all history for this project? This action "
 "cannot be undone."
 msgstr ""
 "Tem certeza que deseja apagar todo o histórico deste projeto? Esta ação não "
 "pode ser desfeita."
 
+msgid "Authentication"
+msgstr "Autenticação"
+
 msgid "Back to the list"
 msgstr "Voltar para a lista"
 
 msgid "Balance"
 msgstr "Saldo"
 
 msgid "Bill %(name)s added"
@@ -144,14 +144,32 @@
 
 msgid "Bill %(name)s changed in an unknown way"
 msgstr "Conta %(name)s modificado de maneira desconhecida"
 
 msgid "Bill %(name)s modified"
 msgstr "Conta %(name)s modificada"
 
+msgid "Bill %(name)s removed"
+msgstr "Conta '%(name)s' foi removida"
+
+msgid "Bill %(name)s renamed to %(new_description)s"
+msgstr "Conta %(name)s renomeada para %(new_description)s"
+
+msgid "Bill %(name)s: %(property_name)s changed from %(before)s to %(after)s"
+msgstr "Conta %(name)s: %(property_name)s mudou de %(before)s para %(after)s"
+
+msgid "Bill %(name)s: %(property_name)s changed to %(after)s"
+msgstr "Conta %(name)s: %(property_name)s mudou para %(after)s"
+
+msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
+msgstr "Conta %(name)s: adicionou %(owers_list_str)s a lista de devedores"
+
+msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
+msgstr "Conta %(name)s: removeu %(owers_list_str)s da lista de devedores"
+
 msgid "Bill items"
 msgstr "Itens da conta"
 
 msgid "Bills"
 msgstr "Contas"
 
 msgid "Bills can't be null"
@@ -174,14 +192,17 @@
 
 msgid "Code"
 msgstr "Código"
 
 msgid "Confirm Remove IP Adresses"
 msgstr "Confirmar a remoção dos Endereços IP"
 
+msgid "Confirm deletion"
+msgstr "Confirmar exclusão"
+
 msgid "Create"
 msgstr "Criar"
 
 msgid "Create a new project"
 msgstr "Criar um novo projeto"
 
 msgid "Create the project"
@@ -201,20 +222,26 @@
 
 msgid "Delete Confirmation"
 msgstr "Deletar Confirmação"
 
 msgid "Delete Stored IP Addresses"
 msgstr "Deletar endereços IP salvos"
 
+msgid "Delete project"
+msgstr "Excluir projeto"
+
 msgid "Delete stored IP addresses"
 msgstr "Deletar endereços IP salvos"
 
 msgid "Deleted project history."
 msgstr "Histórico do projeto apagado."
 
+msgid "Deleted recorded IP addresses in project history."
+msgstr "Endereços IP salvos no histórico de projeto deletados."
+
 msgid "Disabled IP Address Recording"
 msgstr "Gravação do Endereço IP Desativada"
 
 msgid "Disabled Project History"
 msgstr "Histórico do Projeto Desativado"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -229,14 +256,17 @@
 msgstr ""
 "Não reutilize uma senha pessoal. Escolha um código privado e envie-o para "
 "seus amigos"
 
 msgid "Download"
 msgstr "Baixar"
 
+msgid "Download Mobile Application"
+msgstr "Baixar o APP"
+
 msgid "Download project's data"
 msgstr "Baixar dados do projeto"
 
 msgid "Download the list of bills with owner, amount, reason,... "
 msgstr "Baixar a lista de contas com dono, quantia, motivo,... "
 
 msgid "Download the list of transactions needed to settle the current bills."
@@ -248,14 +278,17 @@
 
 msgid "Edit the project"
 msgstr "Editar o projeto"
 
 msgid "Edit this bill"
 msgstr "Editar esta conta"
 
+msgid "Edit this participant"
+msgstr "Editar usuário"
+
 msgid "Email"
 msgstr "E-mail"
 
 msgid "Enable project history"
 msgstr "Ativar histórico do projeto"
 
 msgid "Enabled IP Address Recording"
@@ -264,19 +297,37 @@
 msgid "Enabled Project History"
 msgstr "Histórico do Projeto Ativado"
 
 msgid "Enabled Project History & IP Address Recording"
 msgstr "Histórico do Projeto Ativado & Gravação do Endereço IP"
 
 msgid "Enter a new code if you want to change it"
-msgstr "Digite um novo código se quiser alterá-lo"
+msgstr "Insira um novo código se quiser alterá-lo"
 
 msgid "Enter private code to confirm deletion"
 msgstr "Digite o código privado para confirmar a exclusão"
 
+msgid "Error activating participant"
+msgstr "Erro ao ativar usuário"
+
+msgid "Error deleting bill"
+msgstr "Erro ao excluir conta"
+
+msgid "Error deleting project"
+msgstr "Erro ao excluir o projeto"
+
+msgid "Error deleting project history"
+msgstr "Erro ao deletar o histórico do projeto"
+
+msgid "Error deleting recorded IP addresses"
+msgstr "Erro ao excluir endereços IP salvos"
+
+msgid "Error removing participant"
+msgstr "Erro ao remover usuário"
+
 msgid "Event"
 msgstr "Evento"
 
 msgid "Everyone"
 msgstr "Todos"
 
 msgid "Everyone but %(excluded)s"
@@ -296,14 +347,17 @@
 
 msgid "From IP"
 msgstr "Do IP"
 
 msgid "Get in"
 msgstr "Entrar"
 
+msgid "Get it on"
+msgstr "Pegue agora"
+
 msgid "Going on holidays with friends?"
 msgstr "Indo para o feriado com os amigos?"
 
 msgid "History"
 msgstr "Histórico"
 
 msgid "History Settings Changed"
@@ -318,26 +372,14 @@
 
 msgid "IP address recording can be enabled on the settings page"
 msgstr "A gravação do endereço IP pode ser ativada na página de configurações"
 
 msgid "Identifier:"
 msgstr "Identificador:"
 
-msgid "Import"
-msgstr "Importar"
-
-msgid "Import JSON"
-msgstr "Importar JSON"
-
-msgid "Import previously exported JSON file"
-msgstr "Importar arquivo JSON exportado anteriormente"
-
-msgid "Invalid JSON"
-msgstr "JSON inválido"
-
 msgid "Invalid private code."
 msgstr "Código privado inválido."
 
 msgid "Invalid token"
 msgstr "Token inválido"
 
 msgid "Invite people"
@@ -345,14 +387,17 @@
 
 msgid "Invite people to join this project"
 msgstr "Convide pessoas para participar deste projeto"
 
 msgid "Languages"
 msgstr "Linguagens"
 
+msgid "Legal information"
+msgstr "Informações legais"
+
 msgid "Log in"
 msgstr "Conecte-se"
 
 msgid "Log in to an existing project"
 msgstr "Conecte-se em um projeto existente"
 
 msgid "Logout"
@@ -360,14 +405,17 @@
 
 msgid "Manage your shared <br />expenses, easily"
 msgstr "Modifique suas despesas <br />compartilhadas, facilmente"
 
 msgid "Mobile Application"
 msgstr "Aplicação Mobile"
 
+msgid "More options"
+msgstr "Mais opções"
+
 msgid "Name"
 msgstr "Nome"
 
 msgid "New private code"
 msgstr "Código privado novo"
 
 msgid "Newer bills"
@@ -384,14 +432,17 @@
 
 msgid "No bills"
 msgstr "Sem contas"
 
 msgid "No history to erase"
 msgstr "Não há histórico para apagar"
 
+msgid "No one"
+msgstr "Ninguém"
+
 msgid "No token provided"
 msgstr "Nenhum token fornecido"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
@@ -403,29 +454,58 @@
 
 msgid "Nothing to list yet."
 msgstr "Nada para listar ainda."
 
 msgid "Number of bills"
 msgstr "Número de contas"
 
+msgid "Number of participants"
+msgstr "Número de usuários"
+
 msgid "Older bills"
 msgstr "Contas mais antigas"
 
 msgid "Oldest bill"
 msgstr "Conta mais antiga"
 
 msgid "Other projects :"
 msgstr "Outros projetos:"
 
 msgid "Paid"
 msgstr "Pago"
 
+msgid "Participant %(name)s added"
+msgstr "Usuário %(name)s adicionado"
+
 msgid "Participant %(name)s changed in an unknown way"
 msgstr "Participante %(name)s modificado de maneira desconhecida"
 
+msgid "Participant %(name)s deactivated"
+msgstr "Usuário %(name)s desativado"
+
+msgid "Participant %(name)s modified"
+msgstr "Usuário %(name)s modificado"
+
+msgid "Participant %(name)s reactivated"
+msgstr "Usuário %(name)s reativado"
+
+msgid "Participant %(name)s renamed to %(new_name)s"
+msgstr "Usuário %(name)s renomeado para %(new_name)s"
+
+msgid ""
+"Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
+msgstr "Usuário %(name)s: a carga mudou de %(old_weight)s para %(new_weight)s"
+
+msgid ""
+"Participant '%(name)s' has been deactivated. It will still appear in the "
+"list until its balance reach zero."
+msgstr ""
+"Usuário '%(name)s' foi desativado. Ele continuará aparecendo na lista de "
+"usuários até que seu saldo seja zero."
+
 msgid "Password"
 msgstr "Senha"
 
 msgid "Password confirmation"
 msgstr "Confirmação da senha"
 
 msgid "Password mismatch"
@@ -475,26 +555,32 @@
 
 msgid "Project name"
 msgstr "Nome do projeto"
 
 msgid "Project private code changed"
 msgstr "Código privado do projeto alterado"
 
+msgid "Project renamed to %(new_project_name)s"
+msgstr "Projeto renomeado para %(new_project_name)s"
+
 msgid "Project settings modified"
 msgstr "Configurações do projeto alteradas"
 
 msgid "Project successfully deleted"
 msgstr "Projeto deletado com sucesso"
 
 msgid "Project successfully uploaded"
 msgstr "Projeto enviado corretamente"
 
 msgid "Projects"
 msgstr "Projetos"
 
+msgid "Provided token is invalid"
+msgstr "Token invalido"
+
 msgid "Reset password"
 msgstr "Redefinir senha"
 
 msgid "Reset your password"
 msgstr "Redefinir sua senha"
 
 msgid "Return to home page"
@@ -539,30 +625,14 @@
 msgstr ""
 "Algumas das entradas abaixo contém endereços IP, mesmo este projeto tendo a "
 "gravação de IP desativada. "
 
 msgid "Someone probably cleared the project history."
 msgstr "Alguém provavelmente limpou o histórico do projeto."
 
-msgid ""
-"Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
-msgstr ""
-"Desculpe, houve um erro ao te enviar um email com as instruções de "
-"redefinição de senha. Por favor, confira a configuração de e-mail do "
-"servidor ou entre em contato com um administrador."
-
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. Please "
-"check the email configuration of the server or contact the administrator."
-msgstr ""
-"Desculpe, houve um erro ao enviar os convites via e-mail. Por favor, confira "
-"a configuração de email do servidor ou entre em contato com um administrador."
-
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "Desculpe, não foi possível encontrar a página que você solicitou."
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify about "
 "the\n"
 "                creation of this budget management project and we will send "
@@ -603,48 +673,50 @@
 
 msgid "The bill has been modified"
 msgstr "A conta foi modificada"
 
 msgid "The email %(email)s is not valid"
 msgstr "O email %(email)s não é válido"
 
-msgid "The project identifier is %(project)s"
-msgstr "O identificador do projeto é %(project)s"
+msgid "The participant name is invalid"
+msgstr "'%(name)s' não é um usuário válido"
 
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "O projeto que você está tentando acessar não existe, você quer"
 
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "Esta senha de administrador não é a correta. Apenas %(num)d tentativas "
 "restantes."
 
 msgid "This private code is not the right one"
 msgstr "Este código privado não é o correto"
 
+msgid "This project already have this participant"
+msgstr "'%(name)s' já está no projeto"
+
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
-"Este projeto não pode ser definido como 'sem moeda' porque contém contas em "
+"O projeto não pode ser definido como 'sem moeda' porque contém contas em "
 "várias moedas."
 
 msgid "This project does not exists"
 msgstr "Este projeto não existe"
 
+msgid "This will remove all bills and participants in this project!"
+msgstr "Isso vai remover todas as contas e participantes desse projeto!"
+
 msgid "Time"
 msgstr "Tempo"
 
 msgid "To whom?"
 msgstr "Para quem?"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr ""
-"Muitas tentativas de login falhas, por favor, tente novamente mais tarde."
-
 msgid "Try out the demo"
 msgstr "Experimente a demonstração"
 
 msgid "Unknown error"
 msgstr "Erro desconhecido"
 
 msgid "Unknown project"
@@ -757,7 +829,25 @@
 msgstr "mudar para"
 
 msgid "you can contribute and improve it!"
 msgstr "você pode contribuir para melhorá-lo!"
 
 msgid "you sure?"
 msgstr "tem certeza?"
+
+msgid "{dual_object_0} and {dual_object_1}"
+msgstr "{dual_object_0} e {dual_object_1}"
+
+msgid "{prefix}: {error}"
+msgstr "{prefix}: {error}"
+
+msgid "{prefix}:<br />{errors}"
+msgstr "{prefix}:<br />{errors}"
+
+msgid "{previous_object}, and {end_object}"
+msgstr "{previous_object}, e {end_object}"
+
+msgid "{previous_object}, {next_object}"
+msgstr "{previous_object}, {next_object}"
+
+msgid "{start_object}, {next_object}"
+msgstr "{start_object}, {next_object}"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2022-03-13 14:59+0000\n"
-"Last-Translator: Vinícius A. L. Souza <me@viniciusals.com>\n"
+"PO-Revision-Date: 2023-05-05 00:47+0000\n"
+"Last-Translator: MurkBRA <anjo1077@gmail.com>\n"
 "Language-Team: Portuguese (Brazil) <https://hosted.weblate.org/projects/"
 "i-hate-money/i-hate-money/pt_BR/>\n"
 "Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.12-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Expressão ou montante inválido. Apenas números e os operadores +=*/ são "
@@ -25,15 +25,15 @@
 msgid "Project name"
 msgstr "Nome do projeto"
 
 msgid "New private code"
 msgstr "Código privado novo"
 
 msgid "Enter a new code if you want to change it"
-msgstr "Digite um novo código se quiser alterá-lo"
+msgstr "Insira um novo código se quiser alterá-lo"
 
 msgid "Email"
 msgstr "E-mail"
 
 msgid "Enable project history"
 msgstr "Ativar histórico do projeto"
 
@@ -46,15 +46,15 @@
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr "Definir uma moeda padrão permite a conversão de moeda entre contas"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
-"Este projeto não pode ser definido como 'sem moeda' porque contém contas em "
+"O projeto não pode ser definido como 'sem moeda' porque contém contas em "
 "várias moedas."
 
 msgid "Import previously exported JSON file"
 msgstr "Importar arquivo JSON exportado anteriormente"
 
 msgid "Import"
 msgstr "Importar"
@@ -163,70 +163,68 @@
 
 msgid "Weight"
 msgstr "Peso"
 
 msgid "Add"
 msgstr "Adicionar"
 
-#, fuzzy
 msgid "The participant name is invalid"
-msgstr "Usuário '%(name)s' foi removido"
+msgstr "'%(name)s' não é um usuário válido"
 
-#, fuzzy
 msgid "This project already have this participant"
-msgstr "Este projeto já tem este membro"
+msgstr "'%(name)s' já está no projeto"
 
 msgid "People to notify"
 msgstr "Pessoas para notificar"
 
 msgid "Send invites"
 msgstr "Enviar convites"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "O email %(email)s não é válido"
 
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
-msgstr ""
+msgstr "{dual_object_0} e {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
-msgstr ""
+msgstr "{previous_object}, e {end_object}"
 
 #. Two items in a middle of a list with more than 5 objects
 msgid "{previous_object}, {next_object}"
-msgstr ""
+msgstr "{previous_object}, {next_object}"
 
 #. First two items of a list with more than 3 items
 msgid "{start_object}, {next_object}"
-msgstr ""
+msgstr "{start_object}, {next_object}"
 
 msgid "No Currency"
 msgstr "Sem Moeda"
 
 #. Form error with only one error
 msgid "{prefix}: {error}"
-msgstr ""
+msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
-msgstr ""
+msgstr "{prefix}:<br />{errors}"
 
 msgid "Too many failed login attempts, please retry later."
 msgstr "Muitas tentativas de login falhas, por favor, tente novamente mais tarde."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "Esta senha de administrador não é a correta. Apenas %(num)d tentativas "
 "restantes."
 
 msgid "Provided token is invalid"
-msgstr ""
+msgstr "Token invalido"
 
 msgid "This private code is not the right one"
 msgstr "Este código privado não é o correto"
 
 #, python-format
 msgid "You have just created '%(project)s' to share your expenses"
 msgstr "Você acabou de criar '%(project)s' para compartilhar suas despesas"
@@ -268,24 +266,27 @@
 
 msgid "Project successfully uploaded"
 msgstr "Projeto enviado corretamente"
 
 msgid "Invalid JSON"
 msgstr "JSON inválido"
 
+#, fuzzy
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
+"Não é possível adicionar contas em várias moedas a um projeto sem moeda "
+"padrão"
 
 msgid "Project successfully deleted"
 msgstr "Projeto deletado com sucesso"
 
 msgid "Error deleting project"
-msgstr ""
+msgstr "Erro ao excluir o projeto"
 
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "Você foi convidado a compartilhar suas despesas com %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "Seus convites foram enviados"
@@ -300,80 +301,77 @@
 "administrador."
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr "%(member)s foram adicionados"
 
 msgid "Error activating participant"
-msgstr ""
+msgstr "Erro ao ativar usuário"
 
 #, python-format
 msgid "%(name)s is part of this project again"
 msgstr "%(name)s faz parte deste projeto novamente"
 
 msgid "Error removing participant"
-msgstr ""
+msgstr "Erro ao remover usuário"
 
-#, fuzzy, python-format
+#, python-format
 msgid ""
 "Participant '%(name)s' has been deactivated. It will still appear in the "
 "list until its balance reach zero."
 msgstr ""
 "Usuário '%(name)s' foi desativado. Ele continuará aparecendo na lista de "
-"usuários até que o seu balanço seja zero."
+"usuários até que seu saldo seja zero."
 
 #, fuzzy, python-format
 msgid "Participant '%(name)s' has been removed"
 msgstr "Usuário '%(name)s' foi removido"
 
 #, fuzzy, python-format
 msgid "Participant '%(name)s' has been modified"
 msgstr "Usuário '%(name)s' foi removido"
 
 msgid "The bill has been added"
 msgstr "A conta foi adicionada"
 
 msgid "Error deleting bill"
-msgstr ""
+msgstr "Erro ao excluir conta"
 
 msgid "The bill has been deleted"
 msgstr "A conta foi deletada"
 
 msgid "The bill has been modified"
 msgstr "A conta foi modificada"
 
-#, fuzzy
 msgid "Error deleting project history"
-msgstr "Ativar histórico do projeto"
+msgstr "Erro ao deletar o histórico do projeto"
 
 msgid "Deleted project history."
 msgstr "Histórico do projeto apagado."
 
-#, fuzzy
 msgid "Error deleting recorded IP addresses"
-msgstr "Deletar endereços IP salvos"
+msgstr "Erro ao excluir endereços IP salvos"
 
 msgid "Deleted recorded IP addresses in project history."
-msgstr ""
+msgstr "Endereços IP salvos no histórico de projeto deletados."
 
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "Desculpe, não foi possível encontrar a página que você solicitou."
 
 msgid "The best thing to do is probably to get back to the main page."
 msgstr "É provável que a melhor coisa a fazer seja voltar para a página inicial."
 
 msgid "Back to the list"
 msgstr "Voltar para a lista"
 
 msgid "Administration tasks are currently disabled."
 msgstr "Tarefas de administração estão atualmente desativadas."
 
-#, fuzzy
 msgid "Authentication"
-msgstr "Documentação"
+msgstr "Autenticação"
 
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "O projeto que você está tentando acessar não existe, você quer"
 
 msgid "create it"
 msgstr "Criar"
 
@@ -382,17 +380,16 @@
 
 msgid "Create a new project"
 msgstr "Criar um novo projeto"
 
 msgid "Project"
 msgstr "Projeto"
 
-#, fuzzy
 msgid "Number of participants"
-msgstr "adicionar participantes"
+msgstr "Número de usuários"
 
 msgid "Number of bills"
 msgstr "Número de contas"
 
 msgid "Newest bill"
 msgstr "Conta mais recente"
 
@@ -410,32 +407,29 @@
 
 msgid "show"
 msgstr "exibir"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "O Painel de Controle atualmente está desativado."
 
-#, fuzzy
 msgid "Download Mobile Application"
-msgstr "Aplicação Mobile"
+msgstr "Baixar o APP"
 
-#, fuzzy
 msgid "Get it on"
-msgstr "Entrar"
+msgstr "Pegue agora"
 
 #, fuzzy
 msgid "Are you sure?"
 msgstr "tem certeza?"
 
 msgid "Edit project"
 msgstr "Editar projeto"
 
-#, fuzzy
 msgid "Delete project"
-msgstr "Editar projeto"
+msgstr "Excluir projeto"
 
 msgid "Import JSON"
 msgstr "Importar JSON"
 
 msgid "Choose file"
 msgstr "Escolher arquivo"
 
@@ -463,37 +457,36 @@
 msgid "Privacy Settings"
 msgstr "Configurações de Privacidade"
 
 msgid "Edit the project"
 msgstr "Editar o projeto"
 
 msgid "This will remove all bills and participants in this project!"
-msgstr ""
+msgstr "Isso vai remover todas as contas e participantes desse projeto!"
 
 msgid "Edit this bill"
 msgstr "Editar esta conta"
 
 msgid "Add a bill"
 msgstr "Adicionar uma conta"
 
 msgid "Everyone"
 msgstr "Todos"
 
 msgid "No one"
-msgstr ""
+msgstr "Ninguém"
 
 msgid "More options"
-msgstr ""
+msgstr "Mais opções"
 
 msgid "Add participant"
 msgstr "Adicionar participante"
 
-#, fuzzy
 msgid "Edit this participant"
-msgstr "Adicionar participante"
+msgstr "Editar usuário"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "john.doe@example.com, mary.moe@site.com"
 
 msgid "Send the invitations"
 msgstr "Enviar os convites"
 
@@ -519,19 +512,19 @@
 msgstr "Gravação do Endereço IP Ativada"
 
 msgid "History Settings Changed"
 msgstr "Configurações do Histórico Alteradas"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed from %(before)s to %(after)s"
-msgstr ""
+msgstr "Conta %(name)s: %(property_name)s mudou de %(before)s para %(after)s"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed to %(after)s"
-msgstr ""
+msgstr "Conta %(name)s: %(property_name)s mudou para %(after)s"
 
 msgid "Confirm Remove IP Adresses"
 msgstr "Confirmar a remoção dos Endereços IP"
 
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
@@ -539,17 +532,16 @@
 "action cannot be undone."
 msgstr ""
 "Você tem certeza que deseja deletar todos os endereços IP gravados deste "
 "projeto?\n"
 "                O resto do histórico do projeto não será afetado. Esta "
 "ação não pode ser desfeita."
 
-#, fuzzy
 msgid "Confirm deletion"
-msgstr "Confirmar Exclusão"
+msgstr "Confirmar exclusão"
 
 msgid "Close"
 msgstr "Fechar"
 
 msgid "Delete Confirmation"
 msgstr "Deletar Confirmação"
 
@@ -558,19 +550,19 @@
 "cannot be undone."
 msgstr ""
 "Tem certeza que deseja apagar todo o histórico deste projeto? Esta ação "
 "não pode ser desfeita."
 
 #, python-format
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
-msgstr ""
+msgstr "Conta %(name)s: adicionou %(owers_list_str)s a lista de devedores"
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
-msgstr ""
+msgstr "Conta %(name)s: removeu %(owers_list_str)s da lista de devedores"
 
 #, python-format
 msgid ""
 "\n"
 "            <i>This project has history disabled. New actions won't "
 "appear below. You can enable history on the</i>\n"
 "            <a href=\"%(url)s\">settings page</a>\n"
@@ -642,68 +634,68 @@
 
 #, python-format
 msgid "Bill %(name)s added"
 msgstr "Conta %(name)s adicionada"
 
 #, python-format
 msgid "Participant %(name)s added"
-msgstr ""
+msgstr "Usuário %(name)s adicionado"
 
 msgid "Project private code changed"
 msgstr "Código privado do projeto alterado"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project renamed to %(new_project_name)s"
-msgstr "O identificador do projeto é %(new_project_name)s"
+msgstr "Projeto renomeado para %(new_project_name)s"
 
 #, python-format
 msgid "Project contact email changed to %(new_email)s"
 msgstr "O email de contato do projeto foi alterado para %(new_email)s"
 
 msgid "Project settings modified"
 msgstr "Configurações do projeto alteradas"
 
 #, python-format
 msgid "Participant %(name)s deactivated"
-msgstr ""
+msgstr "Usuário %(name)s desativado"
 
 #, python-format
 msgid "Participant %(name)s reactivated"
-msgstr ""
+msgstr "Usuário %(name)s reativado"
 
 #, python-format
 msgid "Participant %(name)s renamed to %(new_name)s"
-msgstr ""
+msgstr "Usuário %(name)s renomeado para %(new_name)s"
 
 #, python-format
 msgid "Bill %(name)s renamed to %(new_description)s"
-msgstr ""
+msgstr "Conta %(name)s renomeada para %(new_description)s"
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
-msgstr ""
+msgstr "Usuário %(name)s: a carga mudou de %(old_weight)s para %(new_weight)s"
 
 msgid "Amount"
 msgstr "Quantia"
 
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "Quantia em %(currency)s"
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr "Conta %(name)s modificada"
 
 #, python-format
 msgid "Participant %(name)s modified"
-msgstr ""
+msgstr "Usuário %(name)s modificado"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s removed"
-msgstr "Usuário '%(name)s' foi removido"
+msgstr "Conta '%(name)s' foi removida"
 
 #, fuzzy, python-format
 msgid "Participant %(name)s removed"
 msgstr "Usuário '%(name)s' foi removido"
 
 #, python-format
 msgid "Project %(name)s changed in an unknown way"
@@ -807,17 +799,16 @@
 
 msgid "Documentation"
 msgstr "Documentação"
 
 msgid "Administation Dashboard"
 msgstr "Painel de Administração"
 
-#, fuzzy
 msgid "Legal information"
-msgstr "Deletar Confirmação"
+msgstr "Informações legais"
 
 msgid "\"I hate money\" is free software"
 msgstr "\"I hate money\" é um software livre"
 
 msgid "you can contribute and improve it!"
 msgstr "você pode contribuir para melhorá-lo!"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/ru/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/ru/LC_MESSAGES/messages.mo`

 * *Files 19% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,23 +1,22 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
+"Project-Id-Version: Russian (I Hate Money)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2021-09-20 12:38+0000\n"
-"Last-Translator: Роман Прокопов <pochta.romana.iz.vyborga@gmail.com>\n"
-"Language: ru\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: Russian <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/ru/>\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2\n"
+"Language: ru\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
+"Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 msgid ""
 "\n"
 "            <i>The table below reflects actions recorded prior to disabling "
 "project history. You can\n"
 "            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
 "target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
@@ -41,18 +40,18 @@
 "\n"
 "            <i>У этого проекта история отключена. Новые действия не появятся "
 "ниже. Вы можете включить историю в</i>\n"
 "            <a href=\"%(url)s\">настройках</a>\n"
 "            "
 
 msgid "\"I hate money\" is free software"
-msgstr "\" I hate money \" - бесплатная программа"
+msgstr "«I hate money» — это бесплатная и свободная программа"
 
 msgid "%(amount)s each"
-msgstr "%(amount)s по каждому"
+msgstr "%(amount)s с каждого"
 
 msgid "%(member)s has been added"
 msgstr "%(member)s был добавлен"
 
 msgid "%(name)s is part of this project again"
 msgstr "%(name)s снова часть этого проекта"
 
@@ -109,17 +108,14 @@
 
 msgid "Amount"
 msgstr "Количество"
 
 msgid "Amount in %(currency)s"
 msgstr "Количество в %(currency)s"
 
-msgid "Amount paid"
-msgstr "Уплаченная сумма"
-
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
 "                The rest of the project history will be unaffected. This "
 "action cannot be undone."
 msgstr ""
 "Вы уверены, что хотите удалить все записанные IP-адреса из этого проекта?\n"
@@ -128,20 +124,53 @@
 
 msgid ""
 "Are you sure you want to erase all history for this project? This action "
 "cannot be undone."
 msgstr ""
 "Вы уверены, что хотите стереть историю проекта? Это действие нельзя отменить."
 
+msgid "Authentication"
+msgstr "Аутентификация"
+
 msgid "Back to the list"
 msgstr "Вернутся к списку"
 
 msgid "Balance"
 msgstr "Баланс"
 
+msgid "Bill %(name)s added"
+msgstr "Счёт %(name)s добавлен"
+
+msgid "Bill %(name)s changed in an unknown way"
+msgstr "Счёт %(name)s изменён неизвестным образом"
+
+msgid "Bill %(name)s modified"
+msgstr "Счёт %(name)s изменён"
+
+msgid "Bill %(name)s removed"
+msgstr "Счёт %(name)s удалён"
+
+msgid "Bill %(name)s renamed to %(new_description)s"
+msgstr "Счёт %(name)s переименован в %(new_description)s"
+
+msgid "Bill %(name)s: %(property_name)s changed from %(before)s to %(after)s"
+msgstr ""
+"Счёт %(name)s: Атрибут «%(property_name)s» изменён с %(before)s на %(after)s"
+
+msgid "Bill %(name)s: %(property_name)s changed to %(after)s"
+msgstr "Счёт %(name)s: Атрибут «%(property_name)s» изменён на %(after)s"
+
+msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
+msgstr ""
+"Счёт %(name)s: Участник(и) %(owers_list_str)s добавлен(ы) в список должников"
+
+msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
+msgstr ""
+"Счёт %(name)s: Участник(и) %(owers_list_str)s удален(ы) из списка должников"
+
 msgid "Bill items"
 msgstr "Пункты счета"
 
 msgid "Bills"
 msgstr "Счета"
 
 msgid "Bills can't be null"
@@ -149,14 +178,20 @@
 
 msgid "Can't remember the password?"
 msgstr "Не помните пароль?"
 
 msgid "Cancel"
 msgstr "Отменить"
 
+msgid ""
+"Cannot add bills in multiple currencies to a project without default currency"
+msgstr ""
+"Невозможно добавить счета в нескольких валютах в проект без валюты по "
+"умолчанию"
+
 msgid "Choose file"
 msgstr "Выбрать файл"
 
 msgid "Clear Project History"
 msgstr "Стереть историю проекта"
 
 msgid "Close"
@@ -164,14 +199,17 @@
 
 msgid "Code"
 msgstr "Код"
 
 msgid "Confirm Remove IP Adresses"
 msgstr "Подтвердите удаление IP-адресов"
 
+msgid "Confirm deletion"
+msgstr "Подтвердить удаление"
+
 msgid "Create"
 msgstr "Создать"
 
 msgid "Create a new project"
 msgstr "Создать новый проект"
 
 msgid "Create the project"
@@ -191,17 +229,26 @@
 
 msgid "Delete Confirmation"
 msgstr "Подтверждение удаления"
 
 msgid "Delete Stored IP Addresses"
 msgstr "Удалить сохраненные IP-адреса"
 
+msgid "Delete project"
+msgstr "Удалить проект"
+
 msgid "Delete stored IP addresses"
 msgstr "Удалить сохраненные IP-адреса"
 
+msgid "Deleted project history."
+msgstr "История проекта удалена."
+
+msgid "Deleted recorded IP addresses in project history."
+msgstr "Записанные IP-адреса удалены из истории проекта."
+
 msgid "Disabled IP Address Recording"
 msgstr "Выключить запись IP-адрессов"
 
 msgid "Disabled Project History"
 msgstr "История отключенных проектов"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -216,32 +263,40 @@
 msgstr ""
 "Не используйте повторно личный пароль. Выберите приватный код и отправьте "
 "его своим друзьям"
 
 msgid "Download"
 msgstr "Скачать"
 
+msgid "Download Mobile Application"
+msgstr "Скачать мобильное приложение"
+
 msgid "Download project's data"
 msgstr "Скачать данные проекта"
 
 msgid "Download the list of bills with owner, amount, reason,... "
 msgstr "Скачать список счетов с владельцем, суммой, причиной, .. "
 
 msgid "Download the list of transactions needed to settle the current bills."
-msgstr "Скачать список переводов нужных, чтобы урегулировать данные счета."
+msgstr ""
+"Скачать список переводов, необходимых для взаимного расчёта по текущим "
+"счетам."
 
 msgid "Edit project"
 msgstr "Изменить проект"
 
 msgid "Edit the project"
 msgstr "Изменить проект"
 
 msgid "Edit this bill"
 msgstr "Изменить счёт"
 
+msgid "Edit this participant"
+msgstr "Редактировать участника"
+
 msgid "Email"
 msgstr "Email"
 
 msgid "Enable project history"
 msgstr "Включить историю проекта"
 
 msgid "Enabled IP Address Recording"
@@ -249,41 +304,68 @@
 
 msgid "Enabled Project History"
 msgstr "Включить историю проекта"
 
 msgid "Enabled Project History & IP Address Recording"
 msgstr "Включить историю проекта и запись IP адрессов"
 
+msgid "Enter a new code if you want to change it"
+msgstr "Введите новый код, если хотите его изменить"
+
+msgid "Enter private code to confirm deletion"
+msgstr "Введите приватный код, чтобы подтвердить удаление"
+
+msgid "Error activating participant"
+msgstr "Ошибка активации участника"
+
+msgid "Error deleting bill"
+msgstr "Ошибка при удалении счета"
+
+msgid "Error deleting project"
+msgstr "Ошибка при удалении проекта"
+
+msgid "Error deleting project history"
+msgstr "Ошибка при удалении истории проекта"
+
+msgid "Error deleting recorded IP addresses"
+msgstr "Ошибка при удалении записанных IP-адресов"
+
+msgid "Error removing participant"
+msgstr "Ошибка при удалении участника"
+
 msgid "Event"
 msgstr "Событие"
 
 msgid "Everyone"
-msgstr "Каждый"
+msgstr "За всех"
 
 msgid "Everyone but %(excluded)s"
-msgstr "Каждый, кроме %(excluded)s"
+msgstr "За всех, кроме %(excluded)s"
 
 msgid "Expenses by Month"
 msgstr "Расходы по месяцам"
 
 msgid "External link"
 msgstr "Внешняя ссылка"
 
 msgid "For what?"
 msgstr "За что?"
 
 msgid "For whom?"
-msgstr "Кому?"
+msgstr "За кого?"
 
 msgid "From IP"
 msgstr "От IP"
 
 msgid "Get in"
 msgstr "Войти"
 
+msgid "Get it on"
+msgstr "Доступно в"
+
 msgid "Going on holidays with friends?"
 msgstr "Собираетесь в отпуск с друзьями?"
 
 msgid "History"
 msgstr "История"
 
 msgid "History Settings Changed"
@@ -297,38 +379,32 @@
 
 msgid "IP address recording can be enabled on the settings page"
 msgstr "Запись IP-адреса может быть включена на странице настроек"
 
 msgid "Identifier:"
 msgstr "Идентификатор:"
 
-msgid "Import"
-msgstr "Импортировать"
-
-msgid "Import JSON"
-msgstr "Импортировать JSON"
-
-msgid "Import previously exported JSON file"
-msgstr "Импортировать ранее экспортированный JSON файл"
-
-msgid "Invalid JSON"
-msgstr "Неправильный JSON"
+msgid "Invalid private code."
+msgstr "Неверный приватный код."
 
 msgid "Invalid token"
 msgstr "Неправильный токен"
 
 msgid "Invite people"
 msgstr "Пригласите людей"
 
 msgid "Invite people to join this project"
 msgstr "Пригласите людей присоединиться к этому проекту"
 
 msgid "Languages"
 msgstr "Языки"
 
+msgid "Legal information"
+msgstr "Юридическая информация"
+
 msgid "Log in"
 msgstr "Войти"
 
 msgid "Log in to an existing project"
 msgstr "Войти в существующий проект"
 
 msgid "Logout"
@@ -336,14 +412,17 @@
 
 msgid "Manage your shared <br />expenses, easily"
 msgstr "Управляйте своими общими <br />расходами проще"
 
 msgid "Mobile Application"
 msgstr "Мобильное приложение"
 
+msgid "More options"
+msgstr "Другие варианты"
+
 msgid "Name"
 msgstr "Имя"
 
 msgid "New private code"
 msgstr "Новый приватный код"
 
 msgid "Newer bills"
@@ -360,14 +439,17 @@
 
 msgid "No bills"
 msgstr "Нет счетов"
 
 msgid "No history to erase"
 msgstr "Нечего стирать"
 
+msgid "No one"
+msgstr "Ни за кого"
+
 msgid "No token provided"
 msgstr "Не предоставлен токен"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
@@ -378,26 +460,67 @@
 
 msgid "Nothing to list yet."
 msgstr "Нечего перечислять еще."
 
 msgid "Number of bills"
 msgstr "Число счетов"
 
+msgid "Number of participants"
+msgstr "Количество участников"
+
 msgid "Older bills"
 msgstr "Старые счета"
 
 msgid "Oldest bill"
 msgstr "Старейший счёт"
 
 msgid "Other projects :"
 msgstr "Остальные проекты :"
 
 msgid "Paid"
 msgstr "Оплачено"
 
+msgid "Participant %(name)s added"
+msgstr "Пользователь %(name)s добавлен"
+
+msgid "Participant %(name)s changed in an unknown way"
+msgstr "Пользователь %(name)s изменён неизвестным образом"
+
+msgid "Participant %(name)s deactivated"
+msgstr "Пользователь %(name)s отключён"
+
+msgid "Participant %(name)s modified"
+msgstr "Пользователь %(name)s изменён"
+
+msgid "Participant %(name)s reactivated"
+msgstr "Пользователь %(name)s подключён"
+
+msgid "Participant %(name)s removed"
+msgstr "Пользователь %(name)s удалён"
+
+msgid "Participant %(name)s renamed to %(new_name)s"
+msgstr "Пользователь %(name)s переименован в %(new_name)s"
+
+msgid ""
+"Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
+msgstr "Участник %(name)s: масса изменена с %(old_weight)s на %(new_weight)s"
+
+msgid ""
+"Participant '%(name)s' has been deactivated. It will still appear in the "
+"list until its balance reach zero."
+msgstr ""
+"Участник «%(name)s» был деактивирован. Он будет отображаться в списке до тех "
+"пор, пока его баланс не станет равным нулю."
+
+msgid "Participant '%(name)s' has been modified"
+msgstr "Пользователь «%(name)s» был удалён"
+
+msgid "Participant '%(name)s' has been removed"
+msgstr "Участник «%(name)s» был удалён"
+
 msgid "Password"
 msgstr "Пароль"
 
 msgid "Password confirmation"
 msgstr "Подтвердите пароль"
 
 msgid "Password mismatch"
@@ -408,50 +531,71 @@
 
 msgid "Password successfully reset."
 msgstr "Пароль успешно восстановлен."
 
 msgid "Payer"
 msgstr "Плательщик"
 
+msgid "People to notify"
+msgstr "Кого уведомить"
+
 msgid "Period"
 msgstr "Период"
 
+msgid "Please, validate the captcha to proceed."
+msgstr "Пожалуйста, подтвердите капчу, чтобы продолжить."
+
 msgid "Privacy Settings"
 msgstr "Настройки приватности"
 
 msgid "Private code"
 msgstr "Приватный код"
 
 msgid "Project"
 msgstr "Проект"
 
+msgid "Project %(name)s added"
+msgstr "Проект %(name)s добавлен"
+
+msgid "Project %(name)s changed in an unknown way"
+msgstr "Проект %(name)s изменён неизвестным образом"
+
+msgid "Project contact email changed to %(new_email)s"
+msgstr "Контактная почта проекта изменена на %(new_email)s"
+
 msgid "Project default: %(currency)s"
 msgstr "По умолчанию для проекта: %(currency)s"
 
 msgid "Project identifier"
 msgstr "Идентификатор проекта"
 
 msgid "Project name"
 msgstr "Имя проекта"
 
 msgid "Project private code changed"
 msgstr "Приватный код проекта изменен"
 
+msgid "Project renamed to %(new_project_name)s"
+msgstr "Проект переименован в %(new_project_name)s"
+
 msgid "Project settings modified"
 msgstr "Настройки проекта изменены"
 
 msgid "Project successfully deleted"
 msgstr "Проект удалён"
 
 msgid "Project successfully uploaded"
 msgstr "Проект успешно загружен"
 
 msgid "Projects"
 msgstr "Проекты"
 
+msgid "Provided token is invalid"
+msgstr "Предоставленный токен недействителен"
+
 msgid "Reset password"
 msgstr "Восстановить пароль"
 
 msgid "Reset your password"
 msgstr "Восстановить пароль"
 
 msgid "Return to home page"
@@ -465,59 +609,46 @@
 
 msgid "Send the invitations"
 msgstr "Отправить приглашения"
 
 msgid "Send via Emails"
 msgstr "Отправить по почте"
 
+msgid "Setting a default currency enables currency conversion between bills"
+msgstr ""
+"Установка валюты по умолчанию позволяет конвертировать валюту между счетами"
+
 msgid "Settings"
 msgstr "Настройки"
 
 msgid "Settle"
-msgstr "Оплаты"
+msgstr "Взаиморасчёт"
 
 msgid "Settle plans"
-msgstr "Планы оплаты"
+msgstr "Планы взаиморасчёта"
 
 msgid "Share Identifier & code"
 msgstr "Поделиться идентификатором и кодом"
 
 msgid "Share the Link"
 msgstr "Поделиться ссылкой"
 
 msgid "Simply sharing money with others?"
-msgstr "Просто делиться деньгами с другими?"
+msgstr "Просто делитесь деньгами с другими?"
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 "Некоторые записи ниже содержат IP-адреса, хотя в этом проекте запись IP "
 "отключена. "
 
 msgid "Someone probably cleared the project history."
 msgstr "Кто-то скорее всего стёр историю проекта."
 
-msgid ""
-"Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
-msgstr ""
-"К сожалению, при отправке вам электронного письма с инструкциями по сбросу "
-"пароля произошла ошибка. Пожалуйста, проверьте конфигурацию электронной "
-"почты сервера или свяжитесь с администратором."
-
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. Please "
-"check the email configuration of the server or contact the administrator."
-msgstr ""
-"К сожалению, при отправке электронных писем с приглашениями произошла "
-"ошибка. Пожалуйста, проверьте конфигурацию электронной почты сервера или "
-"свяжитесь с администратором."
-
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "К сожалению, нам не удалось найти страницу, которую вы запросили."
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify about "
 "the\n"
 "                creation of this budget management project and we will send "
@@ -557,42 +688,55 @@
 
 msgid "The bill has been modified"
 msgstr "Счёт был изменён"
 
 msgid "The email %(email)s is not valid"
 msgstr "Email %(email)s не правильный"
 
-msgid "The project identifier is %(project)s"
-msgstr "Идентификатор проекта: %(project)s"
+msgid "The participant name is invalid"
+msgstr "Неверное имя участника"
 
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr ""
 "Проект, к которому вы пытаетесь получить доступ, не существует, вы хотите"
 
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "Этот пароль администратора неправильный. Осталось только %(num)d попыток."
 
 msgid "This private code is not the right one"
 msgstr "Этот приватный код не подходит"
 
+msgid "This project already have this participant"
+msgstr "В этом проекте уже есть такой участник"
+
+msgid ""
+"This project cannot be set to 'no currency' because it contains bills in "
+"multiple currencies."
+msgstr ""
+"Для этого проекта нельзя установить режим «без валюты», так как он содержит "
+"счета в нескольких валютах."
+
 msgid "This project does not exists"
 msgstr "Такой проект не существует"
 
+msgid "This will remove all bills and participants in this project!"
+msgstr "Все счета и участники этого проекта будут удалены!"
+
 msgid "Time"
 msgstr "Время"
 
 msgid "To whom?"
 msgstr "Кому?"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr "Слишком много неудачных попыток входа, попробуйте позже."
-
 msgid "Try out the demo"
-msgstr "Попробуйте"
+msgstr "Попробуйте демо-версию"
+
+msgid "Unknown error"
+msgstr "Неизвестная ошибка"
 
 msgid "Unknown project"
 msgstr "Неизвестный проект"
 
 msgid "Use IP tracking for project history"
 msgstr "Использовать отслеживание по IP для истории проекта"
 
@@ -614,14 +758,17 @@
 
 msgid "What?"
 msgstr "Что?"
 
 msgid "When?"
 msgstr "Когда?"
 
+msgid "Which is a real currency: Euro or Petro dollar?"
+msgstr "Какая валюта настоящая: евро или нефтедоллар?"
+
 msgid "Who paid?"
 msgstr "Кто заплатил?"
 
 msgid "Who pays?"
 msgstr "Кто платит?"
 
 msgid "Who?"
@@ -676,14 +823,17 @@
 
 msgid "delete"
 msgstr "удалить"
 
 msgid "edit"
 msgstr "изменить"
 
+msgid "euro"
+msgstr "евро"
+
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "john.doe@example.com, mary.moe@site.com"
 
 msgid "reactivate"
 msgstr "включить"
 
 msgid "show"
@@ -693,7 +843,25 @@
 msgstr "сменён на"
 
 msgid "you can contribute and improve it!"
 msgstr "вы можете способствовать развитию и улучшать её!"
 
 msgid "you sure?"
 msgstr "вы уверены?"
+
+msgid "{dual_object_0} and {dual_object_1}"
+msgstr "{dual_object_0} и {dual_object_1}"
+
+msgid "{prefix}: {error}"
+msgstr "{prefix}: {error}"
+
+msgid "{prefix}:<br />{errors}"
+msgstr "{prefix}:<br />{errors}"
+
+msgid "{previous_object}, and {end_object}"
+msgstr "{previous_object}, и {end_object}"
+
+msgid "{previous_object}, {next_object}"
+msgstr "{previous_object}, {next_object}"
+
+msgid "{start_object}, {next_object}"
+msgstr "{start_object}, {next_object}"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/ru/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/ru/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2021-09-20 12:38+0000\n"
-"Last-Translator: Роман Прокопов <pochta.romana.iz.vyborga@gmail.com>\n"
+"PO-Revision-Date: 2023-05-07 23:52+0000\n"
+"Last-Translator: Egor Dubenetskiy <egor@banka.space>\n"
+"Language-Team: Russian <https://hosted.weblate.org/projects/i-hate-money/"
+"i-hate-money/ru/>\n"
 "Language: ru\n"
-"Language-Team: Russian <https://hosted.weblate.org/projects/i-hate-"
-"money/i-hate-money/ru/>\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 4.18-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Недопустимая сумма выражения. Принимаются только цифры и операторы + - * "
@@ -26,15 +26,15 @@
 msgid "Project name"
 msgstr "Имя проекта"
 
 msgid "New private code"
 msgstr "Новый приватный код"
 
 msgid "Enter a new code if you want to change it"
-msgstr ""
+msgstr "Введите новый код, если хотите его изменить"
 
 msgid "Email"
 msgstr "Email"
 
 msgid "Enable project history"
 msgstr "Включить историю проекта"
 
@@ -42,19 +42,22 @@
 msgstr "Использовать отслеживание по IP для истории проекта"
 
 msgid "Default Currency"
 msgstr "Валюта по умолчанию"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
+"Установка валюты по умолчанию позволяет конвертировать валюту между счетами"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
+"Для этого проекта нельзя установить режим «без валюты», так как он содержит "
+"счета в нескольких валютах."
 
 msgid "Import previously exported JSON file"
 msgstr "Импортировать ранее экспортированный JSON файл"
 
 msgid "Import"
 msgstr "Импортировать"
 
@@ -72,33 +75,30 @@
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
 msgstr ""
 "Проект с идентификатором (\"%(project)s\") уже существует. Пожалуйста, "
 "выберете новый идентификатор"
 
 msgid "Which is a real currency: Euro or Petro dollar?"
-msgstr ""
+msgstr "Какая валюта настоящая: евро или нефтедоллар?"
 
-#, fuzzy
 msgid "euro"
-msgstr "Период"
+msgstr "евро"
 
 msgid "Please, validate the captcha to proceed."
-msgstr ""
+msgstr "Пожалуйста, подтвердите капчу, чтобы продолжить."
 
 msgid "Enter private code to confirm deletion"
-msgstr ""
+msgstr "Введите приватный код, чтобы подтвердить удаление"
 
-#, fuzzy
 msgid "Unknown error"
-msgstr "Неизвестный проект"
+msgstr "Неизвестная ошибка"
 
-#, fuzzy
 msgid "Invalid private code."
-msgstr "Приватный код"
+msgstr "Неверный приватный код."
 
 msgid "Get in"
 msgstr "Войти"
 
 msgid "Admin password"
 msgstr "Пароль администратора"
 
@@ -138,15 +138,15 @@
 msgid "External link"
 msgstr "Внешняя ссылка"
 
 msgid "A link to an external document, related to this bill"
 msgstr "Ссылка на внешний документ, относящийся к этому счёту"
 
 msgid "For whom?"
-msgstr "Кому?"
+msgstr "За кого?"
 
 msgid "Submit"
 msgstr "Отправить"
 
 msgid "Submit and add a new one"
 msgstr "Отправить и добавить новый"
 
@@ -165,68 +165,66 @@
 
 msgid "Weight"
 msgstr "Вес"
 
 msgid "Add"
 msgstr "Добавить"
 
-#, fuzzy
 msgid "The participant name is invalid"
-msgstr "Пользователь '%(name)s' был удалён"
+msgstr "Неверное имя участника"
 
-#, fuzzy
 msgid "This project already have this participant"
 msgstr "В этом проекте уже есть такой участник"
 
 msgid "People to notify"
-msgstr ""
+msgstr "Кого уведомить"
 
 msgid "Send invites"
 msgstr "Отправить приглашения"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "Email %(email)s не правильный"
 
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
-msgstr ""
+msgstr "{dual_object_0} и {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
-msgstr ""
+msgstr "{previous_object}, и {end_object}"
 
 #. Two items in a middle of a list with more than 5 objects
 msgid "{previous_object}, {next_object}"
-msgstr ""
+msgstr "{previous_object}, {next_object}"
 
 #. First two items of a list with more than 3 items
 msgid "{start_object}, {next_object}"
-msgstr ""
+msgstr "{start_object}, {next_object}"
 
 msgid "No Currency"
 msgstr "Нет валюты"
 
 #. Form error with only one error
 msgid "{prefix}: {error}"
-msgstr ""
+msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
-msgstr ""
+msgstr "{prefix}:<br />{errors}"
 
 msgid "Too many failed login attempts, please retry later."
 msgstr "Слишком много неудачных попыток входа, попробуйте позже."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "Этот пароль администратора неправильный. Осталось только %(num)d попыток."
 
 msgid "Provided token is invalid"
-msgstr ""
+msgstr "Предоставленный токен недействителен"
 
 msgid "This private code is not the right one"
 msgstr "Этот приватный код не подходит"
 
 #, python-format
 msgid "You have just created '%(project)s' to share your expenses"
 msgstr "Вы только что создали '%(project)s' , чтобы разделить расходы"
@@ -273,20 +271,22 @@
 msgid "Invalid JSON"
 msgstr "Неправильный JSON"
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
+"Невозможно добавить счета в нескольких валютах в проект без валюты по "
+"умолчанию"
 
 msgid "Project successfully deleted"
 msgstr "Проект удалён"
 
 msgid "Error deleting project"
-msgstr ""
+msgstr "Ошибка при удалении проекта"
 
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "Вас пригласили разделить расходы в проект %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "Ваш код приглашения был отправлен"
@@ -301,81 +301,77 @@
 "свяжитесь с администратором."
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr "%(member)s был добавлен"
 
 msgid "Error activating participant"
-msgstr ""
+msgstr "Ошибка активации участника"
 
 #, python-format
 msgid "%(name)s is part of this project again"
 msgstr "%(name)s снова часть этого проекта"
 
 msgid "Error removing participant"
-msgstr ""
+msgstr "Ошибка при удалении участника"
 
-#, fuzzy, python-format
+#, python-format
 msgid ""
 "Participant '%(name)s' has been deactivated. It will still appear in the "
 "list until its balance reach zero."
 msgstr ""
-"Пользователь '%(name)s' был деактивирован. Он будет отображаться в списке"
-" пользователей до тех пор, пока его баланс не станет равным нулю."
+"Участник «%(name)s» был деактивирован. Он будет отображаться в списке до тех "
+"пор, пока его баланс не станет равным нулю."
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant '%(name)s' has been removed"
-msgstr "Пользователь '%(name)s' был удалён"
+msgstr "Участник «%(name)s» был удалён"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant '%(name)s' has been modified"
-msgstr "Пользователь '%(name)s' был удалён"
+msgstr "Пользователь «%(name)s» был удалён"
 
 msgid "The bill has been added"
 msgstr "Счёт был добавлен"
 
 msgid "Error deleting bill"
-msgstr ""
+msgstr "Ошибка при удалении счета"
 
 msgid "The bill has been deleted"
 msgstr "Счёт был удалён"
 
 msgid "The bill has been modified"
 msgstr "Счёт был изменён"
 
-#, fuzzy
 msgid "Error deleting project history"
-msgstr "Включить историю проекта"
+msgstr "Ошибка при удалении истории проекта"
 
-#, fuzzy
 msgid "Deleted project history."
-msgstr "Включить историю проекта"
+msgstr "История проекта удалена."
 
-#, fuzzy
 msgid "Error deleting recorded IP addresses"
-msgstr "Удалить сохраненные IP-адреса"
+msgstr "Ошибка при удалении записанных IP-адресов"
 
 msgid "Deleted recorded IP addresses in project history."
-msgstr ""
+msgstr "Записанные IP-адреса удалены из истории проекта."
 
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "К сожалению, нам не удалось найти страницу, которую вы запросили."
 
 msgid "The best thing to do is probably to get back to the main page."
 msgstr "Лучше всего вернуться на главную страницу."
 
 msgid "Back to the list"
 msgstr "Вернутся к списку"
 
 msgid "Administration tasks are currently disabled."
 msgstr "Задачи администратора в данный момент отключены."
 
-#, fuzzy
 msgid "Authentication"
-msgstr "Документация"
+msgstr "Аутентификация"
 
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "Проект, к которому вы пытаетесь получить доступ, не существует, вы хотите"
 
 msgid "create it"
 msgstr "создать его"
 
@@ -384,17 +380,16 @@
 
 msgid "Create a new project"
 msgstr "Создать новый проект"
 
 msgid "Project"
 msgstr "Проект"
 
-#, fuzzy
 msgid "Number of participants"
-msgstr "добавить пользователя"
+msgstr "Количество участников"
 
 msgid "Number of bills"
 msgstr "Число счетов"
 
 msgid "Newest bill"
 msgstr "Новейший счёт"
 
@@ -412,32 +407,29 @@
 
 msgid "show"
 msgstr "показать"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "Панель инструментов в данный момент отключена."
 
-#, fuzzy
 msgid "Download Mobile Application"
-msgstr "Мобильное приложение"
+msgstr "Скачать мобильное приложение"
 
-#, fuzzy
 msgid "Get it on"
-msgstr "Войти"
+msgstr "Доступно в"
 
 #, fuzzy
 msgid "Are you sure?"
 msgstr "вы уверены?"
 
 msgid "Edit project"
 msgstr "Изменить проект"
 
-#, fuzzy
 msgid "Delete project"
-msgstr "Изменить проект"
+msgstr "Удалить проект"
 
 msgid "Import JSON"
 msgstr "Импортировать JSON"
 
 msgid "Choose file"
 msgstr "Выбрать файл"
 
@@ -447,55 +439,56 @@
 msgid "Bill items"
 msgstr "Пункты счета"
 
 msgid "Download the list of bills with owner, amount, reason,... "
 msgstr "Скачать список счетов с владельцем, суммой, причиной, .. "
 
 msgid "Settle plans"
-msgstr "Планы оплаты"
+msgstr "Планы взаиморасчёта"
 
 msgid "Download the list of transactions needed to settle the current bills."
-msgstr "Скачать список переводов нужных, чтобы урегулировать данные счета."
+msgstr ""
+"Скачать список переводов, необходимых для взаимного расчёта по текущим "
+"счетам."
 
 msgid "Can't remember the password?"
 msgstr "Не помните пароль?"
 
 msgid "Cancel"
 msgstr "Отменить"
 
 msgid "Privacy Settings"
 msgstr "Настройки приватности"
 
 msgid "Edit the project"
 msgstr "Изменить проект"
 
 msgid "This will remove all bills and participants in this project!"
-msgstr ""
+msgstr "Все счета и участники этого проекта будут удалены!"
 
 msgid "Edit this bill"
 msgstr "Изменить счёт"
 
 msgid "Add a bill"
 msgstr "Добавить счёт"
 
 msgid "Everyone"
-msgstr "Каждый"
+msgstr "За всех"
 
 msgid "No one"
-msgstr ""
+msgstr "Ни за кого"
 
 msgid "More options"
-msgstr ""
+msgstr "Другие варианты"
 
 msgid "Add participant"
 msgstr "Добавить участника"
 
-#, fuzzy
 msgid "Edit this participant"
-msgstr "Добавить участника"
+msgstr "Редактировать участника"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "john.doe@example.com, mary.moe@site.com"
 
 msgid "Send the invitations"
 msgstr "Отправить приглашения"
 
@@ -522,18 +515,19 @@
 
 msgid "History Settings Changed"
 msgstr "Настройки истории изменены"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed from %(before)s to %(after)s"
 msgstr ""
+"Счёт %(name)s: Атрибут «%(property_name)s» изменён с %(before)s на %(after)s"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed to %(after)s"
-msgstr ""
+msgstr "Счёт %(name)s: Атрибут «%(property_name)s» изменён на %(after)s"
 
 msgid "Confirm Remove IP Adresses"
 msgstr "Подтвердите удаление IP-адресов"
 
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
@@ -541,15 +535,14 @@
 "action cannot be undone."
 msgstr ""
 "Вы уверены, что хотите удалить все записанные IP-адреса из этого проекта?"
 "\n"
 "                Остальная часть истории проекта не будет затронута. Это "
 "действие не может быть отменено."
 
-#, fuzzy
 msgid "Confirm deletion"
 msgstr "Подтвердить удаление"
 
 msgid "Close"
 msgstr "Закрыть"
 
 msgid "Delete Confirmation"
@@ -561,18 +554,20 @@
 msgstr ""
 "Вы уверены, что хотите стереть историю проекта? Это действие нельзя "
 "отменить."
 
 #, python-format
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
+"Счёт %(name)s: Участник(и) %(owers_list_str)s добавлен(ы) в список должников"
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
+"Счёт %(name)s: Участник(и) %(owers_list_str)s удален(ы) из списка должников"
 
 #, python-format
 msgid ""
 "\n"
 "            <i>This project has history disabled. New actions won't "
 "appear below. You can enable history on the</i>\n"
 "            <a href=\"%(url)s\">settings page</a>\n"
@@ -634,115 +629,115 @@
 
 msgid "IP address recording can be disabled on the settings page"
 msgstr "Запись IP-адреса может быть отключена на странице настроек"
 
 msgid "From IP"
 msgstr "От IP"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project %(name)s added"
-msgstr "Имя проекта"
+msgstr "Проект %(name)s добавлен"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s added"
-msgstr "Счёт был добавлен"
+msgstr "Счёт %(name)s добавлен"
 
 #, python-format
 msgid "Participant %(name)s added"
-msgstr ""
+msgstr "Пользователь %(name)s добавлен"
 
 msgid "Project private code changed"
 msgstr "Приватный код проекта изменен"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project renamed to %(new_project_name)s"
-msgstr "Идентификатор проекта: %(new_project_name)s"
+msgstr "Проект переименован в %(new_project_name)s"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project contact email changed to %(new_email)s"
-msgstr "Контактная почта проекта изменена на"
+msgstr "Контактная почта проекта изменена на %(new_email)s"
 
 msgid "Project settings modified"
 msgstr "Настройки проекта изменены"
 
 #, python-format
 msgid "Participant %(name)s deactivated"
-msgstr ""
+msgstr "Пользователь %(name)s отключён"
 
 #, python-format
 msgid "Participant %(name)s reactivated"
-msgstr ""
+msgstr "Пользователь %(name)s подключён"
 
 #, python-format
 msgid "Participant %(name)s renamed to %(new_name)s"
-msgstr ""
+msgstr "Пользователь %(name)s переименован в %(new_name)s"
 
 #, python-format
 msgid "Bill %(name)s renamed to %(new_description)s"
-msgstr ""
+msgstr "Счёт %(name)s переименован в %(new_description)s"
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
-msgstr ""
+msgstr "Участник %(name)s: масса изменена с %(old_weight)s на %(new_weight)s"
 
 msgid "Amount"
 msgstr "Количество"
 
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "Количество в %(currency)s"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s modified"
-msgstr "Счёт был изменён"
+msgstr "Счёт %(name)s изменён"
 
 #, python-format
 msgid "Participant %(name)s modified"
-msgstr ""
+msgstr "Пользователь %(name)s изменён"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s removed"
-msgstr "Пользователь '%(name)s' был удалён"
+msgstr "Счёт %(name)s удалён"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant %(name)s removed"
-msgstr "Пользователь '%(name)s' был удалён"
+msgstr "Пользователь %(name)s удалён"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project %(name)s changed in an unknown way"
-msgstr "изменилось неизвестным образом"
+msgstr "Проект %(name)s изменён неизвестным образом"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s changed in an unknown way"
-msgstr "изменилось неизвестным образом"
+msgstr "Счёт %(name)s изменён неизвестным образом"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant %(name)s changed in an unknown way"
-msgstr "изменилось неизвестным образом"
+msgstr "Пользователь %(name)s изменён неизвестным образом"
 
 msgid "Nothing to list"
 msgstr "Нечего перечислять"
 
 msgid "Someone probably cleared the project history."
 msgstr "Кто-то скорее всего стёр историю проекта."
 
 msgid "Manage your shared <br />expenses, easily"
 msgstr "Управляйте своими общими <br />расходами проще"
 
 msgid "Try out the demo"
-msgstr "Попробуйте"
+msgstr "Попробуйте демо-версию"
 
 msgid "You're sharing a house?"
 msgstr "Вы живете в одном доме с другими людьми?"
 
 msgid "Going on holidays with friends?"
 msgstr "Собираетесь в отпуск с друзьями?"
 
 msgid "Simply sharing money with others?"
-msgstr "Просто делиться деньгами с другими?"
+msgstr "Просто делитесь деньгами с другими?"
 
 msgid "We can help!"
 msgstr "Мы поможем!"
 
 msgid "Log in to an existing project"
 msgstr "Войти в существующий проект"
 
@@ -765,15 +760,15 @@
 msgid "Account manager"
 msgstr "Менеджер аккаунтов"
 
 msgid "Bills"
 msgstr "Счета"
 
 msgid "Settle"
-msgstr "Оплаты"
+msgstr "Взаиморасчёт"
 
 msgid "Statistics"
 msgstr "Статистика"
 
 msgid "Languages"
 msgstr "Языки"
 
@@ -809,27 +804,26 @@
 
 msgid "Documentation"
 msgstr "Документация"
 
 msgid "Administation Dashboard"
 msgstr "Панель инструментов администратора"
 
-#, fuzzy
 msgid "Legal information"
-msgstr "Подтверждение удаления"
+msgstr "Юридическая информация"
 
 msgid "\"I hate money\" is free software"
-msgstr "\" I hate money \" - бесплатная программа"
+msgstr "«I hate money» — это бесплатная и свободная программа"
 
 msgid "you can contribute and improve it!"
 msgstr "вы можете способствовать развитию и улучшать её!"
 
 #, python-format
 msgid "%(amount)s each"
-msgstr "%(amount)s по каждому"
+msgstr "%(amount)s с каждого"
 
 msgid "you sure?"
 msgstr "вы уверены?"
 
 msgid "Invite people"
 msgstr "Пригласите людей"
 
@@ -859,15 +853,15 @@
 
 #, python-format
 msgid "Added on %(date)s"
 msgstr "Добавлено %(date)s"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
-msgstr "Каждый, кроме %(excluded)s"
+msgstr "За всех, кроме %(excluded)s"
 
 msgid "No bills"
 msgstr "Нет счетов"
 
 msgid "Nothing to list yet."
 msgstr "Нечего перечислять еще."
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/sr/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/sr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/sr/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/sr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/sv/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/es/LC_MESSAGES/messages.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,516 +1,526 @@
-
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2021-07-20 14:32+0000\n"
-"Last-Translator: Kristoffer Grundström "
-"<swedishsailfishosuser@tutanota.com>\n"
-"Language: sv\n"
-"Language-Team: Swedish <https://hosted.weblate.org/projects/i-hate-"
-"money/i-hate-money/sv/>\n"
-"Plural-Forms: nplurals=2; plural=n != 1\n"
+"PO-Revision-Date: 2022-11-14 05:48+0000\n"
+"Last-Translator: Sabtag3 <dioni1984@yahoo.com>\n"
+"Language-Team: Spanish <https://hosted.weblate.org/projects/i-hate-money/"
+"i-hate-money/es/>\n"
+"Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.15-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
+"Cantidad o expresión no válida. Solo se aceptan números y los operadores "
+"+ - * /."
 
 msgid "Project name"
-msgstr "Namn på projektet"
+msgstr "Nombre del proyecto"
 
 msgid "New private code"
-msgstr "Ny privat kod"
+msgstr "Nuevo código privado"
 
 msgid "Enter a new code if you want to change it"
-msgstr "Ange en ny kod om du vill ändra den"
+msgstr "Ingrese un nuevo código si desea cambiarlo"
 
 msgid "Email"
-msgstr "E-post"
+msgstr "Correo electrónico"
 
 msgid "Enable project history"
-msgstr "Aktiva projekthistorik"
+msgstr "Habilitar historial del proyecto"
 
 msgid "Use IP tracking for project history"
-msgstr "Använd IP-spårning för projekthistorik"
+msgstr "Usar trackeo IP para historial de proyecto"
 
 msgid "Default Currency"
-msgstr "Standardvaluta"
+msgstr "Moneda por defecto"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
+"Establecer una moneda predeterminada permite la conversión de moneda entre "
+"facturas"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
+"Este proyecto no se puede configurar como \"sin moneda\" porque contiene "
+"facturas en varias monedas."
 
 msgid "Import previously exported JSON file"
-msgstr "Importera tidigare exporterad JSON-fil"
+msgstr "Importar .JSON previamente exportado"
 
 msgid "Import"
-msgstr "Importera"
+msgstr "Importar"
 
 msgid "Project identifier"
-msgstr "Projektidentifierare"
+msgstr "Identificador del proyecto"
 
 msgid "Private code"
-msgstr "Privat kod"
+msgstr "Código privado"
 
 msgid "Create the project"
-msgstr "Skapa projektet"
+msgstr "Crear proyecto"
 
 #, python-format
 msgid ""
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
 msgstr ""
-"Ett projekt med den här identifieraren (\"%(project)s\") finns redan. "
-"Vänligen välj en annan identifierare"
+"Un proyecto con este identificador (\"%(project)s\") ya existe. Elija un "
+"nuevo identificador, por favor."
 
 msgid "Which is a real currency: Euro or Petro dollar?"
-msgstr ""
+msgstr "¿Cuál es una moneda real: el euro o el petrodólar?"
 
-#, fuzzy
 msgid "euro"
-msgstr "Period"
+msgstr "Euro"
 
 msgid "Please, validate the captcha to proceed."
-msgstr ""
+msgstr "Por favor, valide el captcha para proceder."
 
 msgid "Enter private code to confirm deletion"
-msgstr "Ange privat kod för att bekräfta borttagning"
+msgstr "Ingrese el código privado para confirmar la eliminación"
 
 msgid "Unknown error"
-msgstr "Okänt fel"
+msgstr "Error desconocido"
 
 msgid "Invalid private code."
-msgstr "Ogiltig privat kod."
+msgstr "Código privado no válido."
 
 msgid "Get in"
-msgstr ""
+msgstr "Entra"
 
 msgid "Admin password"
-msgstr "Lösenord för admin"
+msgstr "Contraseña de administrador"
 
 msgid "Send me the code by email"
-msgstr "Skicka koden till mig via e-post"
+msgstr "Envíame el código por correo electrónico"
 
 msgid "This project does not exists"
-msgstr "Det här projektet finns inte"
+msgstr "Proyecto inexistente"
 
 msgid "Password mismatch"
-msgstr "Lösenordet matchar inte"
+msgstr "La contraseña no coincide"
 
 msgid "Password"
-msgstr "Lösenord"
+msgstr "Contraseña"
 
 msgid "Password confirmation"
-msgstr "Lösenordsbekräftelse"
+msgstr "Confirmar contraseña"
 
 msgid "Reset password"
-msgstr "Återställ lösenord"
+msgstr "Reestablecer contraseña"
 
 msgid "Date"
-msgstr "Datum"
+msgstr "Fecha"
 
 msgid "What?"
-msgstr "Vad?"
+msgstr "¿Qué?"
 
 msgid "Payer"
-msgstr "Betalare"
+msgstr "Pagador"
 
 msgid "Amount paid"
-msgstr "Betald summa"
+msgstr "Cantidad pagada"
 
 msgid "Currency"
-msgstr "Valuta"
+msgstr "Divisa"
 
 msgid "External link"
-msgstr "Extern länk"
+msgstr "Enlace externo"
 
 msgid "A link to an external document, related to this bill"
-msgstr "En länk till ett externt dokument, relaterad till den här räkningen"
+msgstr "Un enlace para un documento externo relacionado con esta cuenta/factura"
 
 msgid "For whom?"
-msgstr "För vem?"
+msgstr "¿Para quién?"
 
 msgid "Submit"
-msgstr "Skicka in"
+msgstr "Enviar"
 
 msgid "Submit and add a new one"
-msgstr "Skicka in och lägg till en ny"
+msgstr "Enviar y agregar uno nuevo"
 
 #, python-format
 msgid "Project default: %(currency)s"
-msgstr ""
+msgstr "Valor predeterminado del proyecto: %(currency)s"
 
 msgid "Bills can't be null"
-msgstr "Räkningar kan inte vara null"
+msgstr ""
 
 msgid "Name"
-msgstr "Namn"
+msgstr "Nombre"
 
 msgid "Weights should be positive"
-msgstr "Vikter borde vara positiva"
+msgstr "Los pesos deben ser positivos"
 
 msgid "Weight"
-msgstr "Vikt"
+msgstr "Peso"
 
 msgid "Add"
-msgstr "Lägg till"
+msgstr "Añadir"
 
-#, fuzzy
 msgid "The participant name is invalid"
-msgstr "Användaren '%(name)s' har tagits bort"
+msgstr "El nombre del participante es invalido"
 
-#, fuzzy
 msgid "This project already have this participant"
-msgstr "Det här projektet har redan den här medlemmen"
+msgstr "Este proyecto ya tiene a este participante"
 
 msgid "People to notify"
-msgstr ""
+msgstr "Personas a las que notificar"
 
 msgid "Send invites"
-msgstr "Skicka inbjudningar"
+msgstr "Enviar invitaciones"
 
 #, python-format
 msgid "The email %(email)s is not valid"
-msgstr ""
+msgstr "El correo %(email)s no es válido"
 
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
-msgstr ""
+msgstr "{doble_objecto_0} y {doble_objecto_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
-msgstr ""
+msgstr "{objecto_previo}, and {fin_objecto}"
 
 #. Two items in a middle of a list with more than 5 objects
 msgid "{previous_object}, {next_object}"
-msgstr ""
+msgstr "{objecto_previo}, y {proximo_objecto}"
 
 #. First two items of a list with more than 3 items
 msgid "{start_object}, {next_object}"
-msgstr ""
+msgstr "{comienzo_objecto}, {proximo_objecto}"
 
 msgid "No Currency"
-msgstr "Ingen valuta"
+msgstr "Sin moneda"
 
 #. Form error with only one error
 msgid "{prefix}: {error}"
-msgstr ""
+msgstr "{prefijo}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
-msgstr ""
+msgstr "{prefijo}:<br />{errores}"
 
 msgid "Too many failed login attempts, please retry later."
-msgstr "För många misslyckade inloggningsförsök, försök igen senare."
+msgstr ""
+"Demasiados intentos de inicio de sesión fallidos, por favor reinténtelo más "
+"tarde"
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
-"Det här lösenordet för admin är inte det rätta. Endast %(num)d försök "
-"kvar."
+"Esta contraseña de administrador no es la correcta. Solo %(num)d intentos "
+"restantes."
 
 msgid "Provided token is invalid"
-msgstr ""
+msgstr "El token proporcionado no es válido"
 
 msgid "This private code is not the right one"
-msgstr "Den här privata koden är inte den rätta"
+msgstr "Este código privado no es el correcto"
 
 #, python-format
 msgid "You have just created '%(project)s' to share your expenses"
-msgstr "Du har just skapat '%(project)s' för att dela ut dina kostnader"
+msgstr "Acabas de crear '%(project)s' para compartir tus gastos"
 
 msgid "A reminder email has just been sent to you"
-msgstr "Ett e-postmeddelande med påminnelse har just skickats till dig"
+msgstr "Se te acaba de enviar un email recordatorio"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
-"Vi försökte skicka en påminnelse till din e-postadress, men det uppstod "
-"ett fel. Du kan fortfarande använda det här projektet normalt."
+"Intentamos enviarte un email recordatorio, pero se produjo un error. Puedes "
+"continuar usando el proyecto normalmente"
 
 #, python-format
 msgid "The project identifier is %(project)s"
-msgstr "Projektets identifierare är %(project)s"
+msgstr "El identificador del proyecto es %(project)s"
 
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
 "instructions. Please check the email configuration of the server or "
 "contact the administrator."
 msgstr ""
+"Lo sentimos, se ha producido un error al enviarle un correo electrónico con "
+"instrucciones para restablecer la contraseña. Compruebe la configuración de "
+"correo electrónico del servidor o póngase en contacto con el administrador."
 
 msgid "No token provided"
-msgstr "Ingen symbol tillhandahölls"
+msgstr "No se proporciona ningún token"
 
 msgid "Invalid token"
-msgstr "Ogiltig symbol"
+msgstr "Token invalido"
 
 msgid "Unknown project"
-msgstr "Okänt projekt"
+msgstr "Proyecto desconocido"
 
 msgid "Password successfully reset."
-msgstr "Återställningen av lösenordet lyckades."
+msgstr "La contraseña se restableció correctamente."
 
 msgid "Project successfully uploaded"
-msgstr "Uppladdningen av projektet lyckades"
+msgstr "Proyecto cargado correctamente"
 
 msgid "Invalid JSON"
-msgstr "Ogiltig JSON"
+msgstr "JSON invalido"
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
+"No se pueden agregar billetes en varias monedas a un proyecto sin la moneda "
+"predeterminada"
 
 msgid "Project successfully deleted"
-msgstr "Borttagningen av projektet lyckades"
+msgstr "Proyecto eliminado correctamente"
 
 msgid "Error deleting project"
-msgstr ""
+msgstr "Error al eliminar el proyecto"
 
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
-msgstr "Du har bjudits in att dela ut dina kostnader för %(project)s"
+msgstr "Ha sido invitado a compartir sus gastos para %(project)s"
 
 msgid "Your invitations have been sent"
-msgstr "Dina inbjudningar har skickats"
+msgstr "Sus invitaciones han sido enviadas"
 
 msgid ""
 "Sorry, there was an error while trying to send the invitation emails. "
 "Please check the email configuration of the server or contact the "
 "administrator."
 msgstr ""
+"Lo sentimos, se ha producido un error al intentar enviar los correos "
+"electrónicos de invitación. Compruebe la configuración de correo electrónico "
+"del servidor o póngase en contacto con el administrador."
 
 #, python-format
 msgid "%(member)s has been added"
-msgstr "%(member)s har lagts till"
+msgstr ""
 
 msgid "Error activating participant"
 msgstr ""
 
 #, python-format
 msgid "%(name)s is part of this project again"
-msgstr "%(name)s är en del av det här projektet igen"
+msgstr ""
 
 msgid "Error removing participant"
 msgstr ""
 
 #, python-format
 msgid ""
 "Participant '%(name)s' has been deactivated. It will still appear in the "
 "list until its balance reach zero."
 msgstr ""
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant '%(name)s' has been removed"
-msgstr "Användaren '%(name)s' har tagits bort"
+msgstr ""
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant '%(name)s' has been modified"
-msgstr "Användaren '%(name)s' har tagits bort"
+msgstr ""
 
 msgid "The bill has been added"
-msgstr "Räkningen har lagts till"
+msgstr ""
 
 msgid "Error deleting bill"
 msgstr ""
 
 msgid "The bill has been deleted"
-msgstr "Räkningen har tagits bort"
+msgstr ""
 
 msgid "The bill has been modified"
-msgstr "Räkningen har blivit modifierad"
+msgstr ""
 
 #, fuzzy
 msgid "Error deleting project history"
-msgstr "Aktiva projekthistorik"
+msgstr "Habilitar historial del proyecto"
 
 #, fuzzy
 msgid "Deleted project history."
-msgstr "Aktiva projekthistorik"
+msgstr "Habilitar historial del proyecto"
 
-#, fuzzy
 msgid "Error deleting recorded IP addresses"
-msgstr "Ta bort lagrade IP-adresser"
+msgstr ""
 
 msgid "Deleted recorded IP addresses in project history."
 msgstr ""
 
 msgid "Sorry, we were unable to find the page you've asked for."
-msgstr "Ledsen, men vi kunde inte hitta sidan som du frågade efter."
+msgstr ""
 
 msgid "The best thing to do is probably to get back to the main page."
-msgstr "Det bästa du kan göra är förmodligen att gå tillbaka till huvudsidan."
+msgstr ""
 
 msgid "Back to the list"
-msgstr "Tillbaka till listan"
+msgstr ""
 
 msgid "Administration tasks are currently disabled."
 msgstr ""
 
 #, fuzzy
 msgid "Authentication"
-msgstr "Dokumentation"
+msgstr "Documentación"
 
 msgid "The project you are trying to access do not exist, do you want to"
-msgstr "Projektet som du försöker komma åt finns inte, vill du"
+msgstr ""
 
 msgid "create it"
-msgstr "skapa det"
+msgstr ""
 
 msgid "?"
-msgstr "?"
+msgstr ""
 
 msgid "Create a new project"
-msgstr "Skapa ett nytt projekt"
+msgstr ""
 
 msgid "Project"
-msgstr "Projekt"
+msgstr "Proyecto"
 
 #, fuzzy
 msgid "Number of participants"
-msgstr "lägg till deltagare"
+msgstr "añadir participantes"
 
 msgid "Number of bills"
-msgstr "Antalet räkningar"
+msgstr ""
 
 msgid "Newest bill"
-msgstr "Nyaste räkningen"
+msgstr ""
 
 msgid "Oldest bill"
-msgstr "Äldsta räkningen"
+msgstr ""
 
 msgid "Actions"
-msgstr "Åtgärder"
+msgstr "Acciones"
 
 msgid "edit"
-msgstr "redigera"
+msgstr "editar"
 
 msgid "delete"
-msgstr "ta bort"
+msgstr "eliminar"
 
 msgid "show"
-msgstr "visa"
+msgstr "mostrar"
 
 msgid "The Dashboard is currently deactivated."
-msgstr "Instrumentpanelen är för närvarande inaktiverad."
+msgstr ""
 
 #, fuzzy
 msgid "Download Mobile Application"
-msgstr "Mobilapplikation"
+msgstr "Aplicación móvil"
 
 msgid "Get it on"
 msgstr ""
 
-#, fuzzy
 msgid "Are you sure?"
-msgstr "säker?"
+msgstr ""
 
 msgid "Edit project"
-msgstr "Redigera projekt"
+msgstr ""
 
 #, fuzzy
 msgid "Delete project"
-msgstr "Redigera projekt"
+msgstr "Editar el proyecto"
 
 msgid "Import JSON"
-msgstr "Importera JSON"
+msgstr ""
 
 msgid "Choose file"
-msgstr "Välj fil"
+msgstr ""
 
 msgid "Download project's data"
-msgstr "Ladda ner projektets data"
+msgstr ""
 
 msgid "Bill items"
 msgstr ""
 
 msgid "Download the list of bills with owner, amount, reason,... "
 msgstr ""
 
 msgid "Settle plans"
 msgstr ""
 
 msgid "Download the list of transactions needed to settle the current bills."
 msgstr ""
 
 msgid "Can't remember the password?"
-msgstr "Kan du inte komma ihåg lösenordet?"
+msgstr ""
 
 msgid "Cancel"
-msgstr "Avbryt"
+msgstr "Cancelar"
 
 msgid "Privacy Settings"
-msgstr "Inställningar för privatliv"
+msgstr "Ajustes de privacidad"
 
 msgid "Edit the project"
-msgstr "Redigera projektet"
+msgstr "Editar el proyecto"
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
 msgid "Edit this bill"
-msgstr "Redigera den här räkningen"
+msgstr "Editar esta factura"
 
 msgid "Add a bill"
-msgstr "Lägg till en räkning"
+msgstr "Añadir una factura"
 
 msgid "Everyone"
-msgstr "Alla"
+msgstr ""
 
 msgid "No one"
 msgstr ""
 
 msgid "More options"
 msgstr ""
 
 msgid "Add participant"
-msgstr "Lägg till deltagare"
+msgstr "Añadir participante"
 
 #, fuzzy
 msgid "Edit this participant"
-msgstr "Lägg till deltagare"
+msgstr "Añadir participante"
 
 msgid "john.doe@example.com, mary.moe@site.com"
-msgstr "john.doe@exempel.com, mary.moe@sida.com"
+msgstr ""
 
 msgid "Send the invitations"
-msgstr "Skicka inbjudningarna"
+msgstr "Enviar invitaciones"
 
 msgid "Download"
-msgstr "Ladda ner"
+msgstr "Descargar"
 
 msgid "Disabled Project History"
-msgstr "Inaktiverade projekthistorik"
+msgstr "Historial del proyecto desactivado"
 
 msgid "Disabled Project History & IP Address Recording"
-msgstr "Inaktiverade projekthistorik och inspelning av IP-adress"
+msgstr ""
 
 msgid "Enabled Project History"
-msgstr "Aktiverade projekthistorik"
+msgstr "Historial del proyecto activado"
 
 msgid "Disabled IP Address Recording"
-msgstr "Inaktiverade inspelning av IP-adress"
+msgstr ""
 
 msgid "Enabled Project History & IP Address Recording"
-msgstr "Aktiverade projekthistorik & inspelning av IP-adress"
+msgstr ""
 
 msgid "Enabled IP Address Recording"
-msgstr "Aktiverade inspelning av IP-adress"
+msgstr ""
 
 msgid "History Settings Changed"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed from %(before)s to %(after)s"
 msgstr ""
@@ -525,30 +535,27 @@
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
 "                The rest of the project history will be unaffected. This "
 "action cannot be undone."
 msgstr ""
 
-#, fuzzy
 msgid "Confirm deletion"
-msgstr "Bekräfta borttagning"
+msgstr ""
 
 msgid "Close"
-msgstr "Stäng"
+msgstr "Cerrar"
 
 msgid "Delete Confirmation"
-msgstr "Ta bort bekräftelse"
+msgstr ""
 
 msgid ""
 "Are you sure you want to erase all history for this project? This action "
 "cannot be undone."
 msgstr ""
-"Är du säker på att du vill ta bort alla historik för det här projektet? "
-"Den här åtgärden kan inte göras ogjord."
 
 #, python-format
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
@@ -573,72 +580,70 @@
 "            "
 msgstr ""
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
-"Några poster här nedan innehåller IP-adresser, fastän det här projektet "
-"har IP-inspelning inaktiverat. "
 
 msgid "Delete stored IP addresses"
-msgstr "Ta bort lagrade IP-adresser"
+msgstr ""
 
 msgid "No history to erase"
-msgstr "Ingen historik att ta bort"
+msgstr ""
 
 msgid "Clear Project History"
-msgstr "Rensa projektets historik"
+msgstr ""
 
 msgid "No IP Addresses to erase"
-msgstr "Inga IP-adresser att ta bort"
+msgstr ""
 
 msgid "Delete Stored IP Addresses"
 msgstr ""
 
 msgid "Time"
-msgstr "Tid"
+msgstr "Hora"
 
 msgid "Event"
-msgstr "Händelse"
+msgstr "Evento"
 
 msgid "IP address recording can be enabled on the settings page"
 msgstr ""
 
 msgid "IP address recording can be disabled on the settings page"
 msgstr ""
 
 msgid "From IP"
-msgstr "Från IP"
+msgstr ""
 
 #, fuzzy, python-format
 msgid "Project %(name)s added"
-msgstr "Namn på projektet"
+msgstr "Nombre del proyecto"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s added"
-msgstr "Räkningen har lagts till"
+msgstr ""
 
 #, python-format
 msgid "Participant %(name)s added"
 msgstr ""
 
 msgid "Project private code changed"
-msgstr "Projektets privata kod ändrades"
+msgstr ""
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project renamed to %(new_project_name)s"
-msgstr "Projektets identifierare är %(new_project_name)s"
+msgstr ""
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project contact email changed to %(new_email)s"
-msgstr "Projektets e-post för kontakt ändrades till"
+msgstr ""
 
 msgid "Project settings modified"
-msgstr "Projektets inställningar ändrades"
+msgstr ""
 
 #, python-format
 msgid "Participant %(name)s deactivated"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s reactivated"
@@ -653,342 +658,382 @@
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
 msgid "Amount"
-msgstr "Summa"
+msgstr "Cantidad"
 
 #, python-format
 msgid "Amount in %(currency)s"
-msgstr "Summa i %(currency)s"
+msgstr "Cantidad en %(currency)s"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s modified"
-msgstr "Räkningen har blivit modifierad"
+msgstr ""
 
 #, python-format
 msgid "Participant %(name)s modified"
 msgstr ""
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s removed"
-msgstr "Användaren '%(name)s' har tagits bort"
+msgstr ""
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant %(name)s removed"
-msgstr "Användaren '%(name)s' har tagits bort"
+msgstr ""
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project %(name)s changed in an unknown way"
-msgstr "ändrades på ett okänt sätt"
+msgstr ""
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s changed in an unknown way"
-msgstr "ändrades på ett okänt sätt"
+msgstr ""
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant %(name)s changed in an unknown way"
-msgstr "ändrades på ett okänt sätt"
+msgstr ""
 
 msgid "Nothing to list"
-msgstr "Inget att lista"
+msgstr ""
 
 msgid "Someone probably cleared the project history."
 msgstr ""
 
 msgid "Manage your shared <br />expenses, easily"
-msgstr "Hantera dina utdelade <br />kostnader, lätt"
+msgstr ""
 
 msgid "Try out the demo"
-msgstr "Prova demot"
+msgstr ""
 
 msgid "You're sharing a house?"
-msgstr "Delar du ett hus?"
+msgstr ""
 
 msgid "Going on holidays with friends?"
-msgstr "Ska du på semester med dina vänner?"
+msgstr ""
 
 msgid "Simply sharing money with others?"
-msgstr "Delar du helt enkelt pengar med andra?"
+msgstr ""
 
 msgid "We can help!"
-msgstr "Vi kan hjälpa!"
+msgstr "Podemos ayudar!"
 
 msgid "Log in to an existing project"
-msgstr "Logga in i ett befintligt projekt"
+msgstr "Acceder a un proyecto existente"
 
 msgid "Log in"
-msgstr "Logga in"
+msgstr ""
 
 msgid "can't remember your password?"
-msgstr "kan du inte komma ihåg ditt lösenord?"
+msgstr "¿no recuerdas tu contraseña?"
 
 msgid "Create"
-msgstr "Skapa"
+msgstr "Crear"
 
 msgid ""
 "Don\\'t reuse a personal password. Choose a private code and send it to "
 "your friends"
 msgstr ""
+"No reutilizes una contraseña personal. Escoge un código privado i envíalo"
+" a tus amigos"
 
 msgid "Account manager"
-msgstr "Kontoansvarig"
+msgstr ""
 
 msgid "Bills"
-msgstr "Räkningar"
+msgstr "Facturas"
 
 msgid "Settle"
 msgstr ""
 
 msgid "Statistics"
-msgstr "Statistik"
+msgstr "Estadísticas"
 
 msgid "Languages"
-msgstr "Språk"
+msgstr "Idiomas"
 
 msgid "Projects"
-msgstr "Projekt"
+msgstr "Proyectos"
 
 msgid "Start a new project"
-msgstr "Starta ett nytt projekt"
+msgstr ""
 
 msgid "History"
-msgstr "Historik"
+msgstr "Historia"
 
 msgid "Settings"
-msgstr "Inställningar"
+msgstr "Ajustes"
 
 msgid "Other projects :"
-msgstr "Andra projekt :"
+msgstr "Otros proyectos :"
 
 msgid "switch to"
-msgstr "byt till"
+msgstr "cambiar a"
 
 msgid "Dashboard"
-msgstr "Instrumentpanel"
+msgstr ""
 
 msgid "Logout"
-msgstr "Logga ut"
+msgstr ""
 
 msgid "Code"
-msgstr "Kod"
+msgstr "Código"
 
 msgid "Mobile Application"
-msgstr "Mobilapplikation"
+msgstr "Aplicación móvil"
 
 msgid "Documentation"
-msgstr "Dokumentation"
+msgstr "Documentación"
 
 msgid "Administation Dashboard"
-msgstr ""
+msgstr "Panel de administración"
 
-#, fuzzy
 msgid "Legal information"
-msgstr "Ta bort bekräftelse"
+msgstr ""
 
 msgid "\"I hate money\" is free software"
-msgstr "\"Jag hatar pengar\" är en fri mjukvara"
+msgstr ""
 
 msgid "you can contribute and improve it!"
-msgstr "du kan bidra och förbättra det!"
+msgstr ""
 
 #, python-format
 msgid "%(amount)s each"
-msgstr "%(amount)s var"
+msgstr ""
 
 msgid "you sure?"
-msgstr "säker?"
+msgstr ""
 
 msgid "Invite people"
-msgstr "Bjud in personer"
+msgstr ""
 
 msgid "You should start by adding participants"
-msgstr "Du borde börja med att lägga till deltagare"
+msgstr ""
 
 msgid "Add a new bill"
-msgstr "Lägg till en ny räkning"
+msgstr ""
 
 msgid "Newer bills"
-msgstr "Nyare räkningar"
+msgstr ""
 
 msgid "Older bills"
-msgstr "Äldre räkningar"
+msgstr ""
 
 msgid "When?"
-msgstr "När?"
+msgstr "¿Cuándo?"
 
 msgid "Who paid?"
-msgstr "Vem betalade?"
+msgstr ""
 
 msgid "For what?"
-msgstr "För vad?"
+msgstr ""
 
 msgid "How much?"
-msgstr "Hur mycket?"
+msgstr ""
 
 #, python-format
 msgid "Added on %(date)s"
-msgstr "Lades till %(date)s"
+msgstr ""
 
 #, python-format
 msgid "Everyone but %(excluded)s"
-msgstr "Alla förutom %(excluded)s"
+msgstr ""
 
 msgid "No bills"
-msgstr "Inga räkningar"
+msgstr "Sin facturas"
 
 msgid "Nothing to list yet."
-msgstr "Ingenting att lista än."
+msgstr "No hay nada que mostrar todavía."
 
 msgid "You probably want to"
-msgstr "Du kanske vill"
+msgstr "Probablemente quieras"
 
 msgid "add a bill"
-msgstr "lägg till en räkning"
+msgstr "añadir una factura"
 
 msgid "add participants"
-msgstr "lägg till deltagare"
+msgstr "añadir participantes"
 
 msgid "Password reminder"
-msgstr "Lösenordspåminnare"
+msgstr ""
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
 msgstr ""
 
 msgid "Return to home page"
-msgstr "Återgå till första-sidan"
+msgstr "Volver a la página de inicio"
 
 msgid "Your projects"
-msgstr "Dina projekt"
+msgstr "Tus proyectos"
 
 msgid "Reset your password"
-msgstr "Återställ ditt lösenord"
+msgstr "Reestablecer tu contraseña"
 
 msgid "Invite people to join this project"
-msgstr "Bjud in personer att ansluta till det här projektet"
+msgstr ""
 
 msgid "Share Identifier & code"
-msgstr "Dela ut identifierare & kod"
+msgstr "Compartir identificador i código"
 
 msgid ""
 "You can share the project identifier and the private code by any "
 "communication means."
 msgstr ""
 
 msgid "Identifier:"
-msgstr "Identifierare:"
+msgstr "Identificador:"
 
 msgid "Share the Link"
-msgstr "Dela ut länken"
+msgstr "Compartir el enlace"
 
 msgid "You can directly share the following link via your prefered medium"
-msgstr "Du kan direkt dela ut följande länk via föredraget media"
+msgstr ""
 
 msgid "Send via Emails"
 msgstr ""
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
 "send them an email for you."
 msgstr ""
 
 msgid "Who pays?"
-msgstr "Vem betalar?"
+msgstr ""
 
 msgid "To whom?"
-msgstr "Till vem?"
+msgstr "¿Para quién?"
 
 msgid "Who?"
-msgstr "Vem?"
+msgstr "¿Quién?"
 
 msgid "Balance"
-msgstr "Saldo"
+msgstr ""
 
 msgid "deactivate"
-msgstr "inaktivera"
+msgstr "desactivar"
 
 msgid "reactivate"
-msgstr "återaktivera"
+msgstr "reactivar"
 
 msgid "Paid"
-msgstr "Betald"
+msgstr "Pagado"
 
 msgid "Spent"
-msgstr ""
+msgstr "Gastado"
 
 msgid "Expenses by Month"
-msgstr "Kostnader per månad"
+msgstr "Gastos por mes"
 
 msgid "Period"
-msgstr "Period"
+msgstr "Período"
 
 #~ msgid "Participant"
-#~ msgstr "Deltagare"
+#~ msgstr "Participante"
 
 #~ msgid "Bill"
-#~ msgstr "Räkning"
+#~ msgstr "Factura"
 
 #~ msgid "Select all"
-#~ msgstr "Välj alla"
+#~ msgstr "Seleccionar todo"
 
 #~ msgid "Select none"
-#~ msgstr "Välj ingen"
+#~ msgstr ""
 
 #~ msgid "changed"
 #~ msgstr ""
 
 #~ msgid "from"
-#~ msgstr "från"
+#~ msgstr "de"
 
 #~ msgid "to"
-#~ msgstr "till"
+#~ msgstr "para"
+
+#~ msgid "Confirm Delete"
+#~ msgstr ""
 
 #~ msgid "Added"
-#~ msgstr "Lades till"
+#~ msgstr "Añadido"
 
 #~ msgid "Removed"
-#~ msgstr "Togs bort"
+#~ msgstr "Eliminado"
 
 #~ msgid "and"
-#~ msgstr "och"
+#~ msgstr ""
 
 #~ msgid "owers list"
 #~ msgstr ""
 
 #~ msgid "added"
-#~ msgstr "lades till"
+#~ msgstr "añadido"
 
 #~ msgid "Project renamed to"
-#~ msgstr "Projektet döptes om till"
+#~ msgstr ""
+
+#~ msgid "Project contact email changed to"
+#~ msgstr ""
 
 #~ msgid "deactivated"
-#~ msgstr "inaktiverades"
+#~ msgstr ""
 
 #~ msgid "reactivated"
-#~ msgstr "återaktiverades"
+#~ msgstr ""
 
 #~ msgid "renamed to"
-#~ msgstr "döptes om till"
+#~ msgstr ""
 
 #~ msgid "External link changed to"
-#~ msgstr "Extern länk ändrades till"
+#~ msgstr ""
 
 #~ msgid "modified"
-#~ msgstr "ändrades"
+#~ msgstr "modificado"
 
 #~ msgid "removed"
-#~ msgstr "togs bort"
+#~ msgstr "eliminado"
+
+#~ msgid "changed in a unknown way"
+#~ msgstr ""
 
 #~ msgid "You either provided a bad token or no project identifier."
 #~ msgstr ""
 
 #~ msgid "User name incorrect"
-#~ msgstr "Användarnamnet felaktigt"
+#~ msgstr "Usuario incorrecto"
+
+#~ msgid "This project already have this member"
+#~ msgstr ""
 
 #~ msgid "People to notify"
-#~ msgstr "Personer att meddela"
+#~ msgstr ""
+
+#~ msgid "Error activating member"
+#~ msgstr ""
+
+#~ msgid "Error removing member"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "User '%(name)s' has been deactivated. It"
+#~ " will still appear in the users "
+#~ "list until its balance becomes zero."
+#~ msgstr ""
+
+#~ msgid "User '%(name)s' has been removed"
+#~ msgstr ""
+
+#~ msgid "User '%(name)s' has been edited"
+#~ msgstr ""
+
+#~ msgid "Number of members"
+#~ msgstr ""
+
+#~ msgid "Edit this member"
+#~ msgstr "Editar miembro"
+
+#~ msgid "Participants to notify"
+#~ msgstr "añadir participantes"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/ta/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/ta/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/ta/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/ta/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/th/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/th/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/th/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/th/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/tr/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/tr/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Turkish <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/tr/>\n"
 "Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.9-dev\n"
+"X-Generator: Weblate 4.14.2\n"
 
 msgid ""
 "\n"
 "            <i>The table below reflects actions recorded prior to disabling "
 "project history. You can\n"
 "            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
 "target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
@@ -432,15 +432,15 @@
 msgid "Mobile Application"
 msgstr "Telefon Uygulaması"
 
 msgid "More options"
 msgstr "Diğer seçenekler"
 
 msgid "Name"
-msgstr "İsim"
+msgstr "Ad"
 
 msgid "New private code"
 msgstr "Yeni özel kod"
 
 msgid "Newer bills"
 msgstr "Daha yeni faturalar"
 
@@ -465,16 +465,16 @@
 msgid "No token provided"
 msgstr "Belirteç sağlanmadı"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
-"Geçerli bir miktar veya ifade değil. Sadece rakamlar ve + - * / operatörler "
-"kabul edilir."
+"Geçerli bir miktar veya ifade değil. Yalnızca rakamlar ve + - * / "
+"operatörleri kabul edilir."
 
 msgid "Nothing to list"
 msgstr "Listelenecek bir şey yok"
 
 msgid "Nothing to list yet."
 msgstr "Henüz listelenecek bir şey yok."
 
@@ -734,15 +734,15 @@
 msgid "The project identifier is %(project)s"
 msgstr "Proje tanımlayıcısı %(project)s"
 
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "Erişmeye çalıştığınız proje mevcut değil, ister misiniz"
 
 msgid "This admin password is not the right one. Only %(num)d attempts left."
-msgstr "Bu yönetici parolası doğru değil. Sadece %(num)d tane deneme kaldı."
+msgstr "Bu yönetici parolası doğru değil. Yalnızca %(num)d tane deneme kaldı."
 
 msgid "This private code is not the right one"
 msgstr "Bu özel kod doğru değil"
 
 msgid "This project already have this participant"
 msgstr "Bu projede bu katılımcı zaten var"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/tr/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/tr/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2021-11-07 16:52+0000\n"
-"Last-Translator: Oğuz Ersen <oguzersen@protonmail.com>\n"
+"PO-Revision-Date: 2022-11-07 10:07+0000\n"
+"Last-Translator: Oğuz Ersen <oguz@ersen.moe>\n"
 "Language-Team: Turkish <https://hosted.weblate.org/projects/i-hate-money/"
 "i-hate-money/tr/>\n"
 "Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.9-dev\n"
+"X-Generator: Weblate 4.14.2\n"
 "Generated-By: Babel 2.9.0\n"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
-"Geçerli bir miktar veya ifade değil. Sadece rakamlar ve + - * / "
-"operatörler kabul edilir."
+"Geçerli bir miktar veya ifade değil. Yalnızca rakamlar ve + - * / "
+"operatörleri kabul edilir."
 
 msgid "Project name"
 msgstr "Proje adı"
 
 msgid "New private code"
 msgstr "Yeni özel kod"
 
@@ -154,15 +154,15 @@
 msgid "Project default: %(currency)s"
 msgstr "Proje öntanımlı değeri: %(currency)s"
 
 msgid "Bills can't be null"
 msgstr "Faturalar boş olamaz"
 
 msgid "Name"
-msgstr "İsim"
+msgstr "Ad"
 
 msgid "Weights should be positive"
 msgstr "Ağırlıklar pozitif olmalıdır"
 
 msgid "Weight"
 msgstr "Ağırlık"
 
@@ -215,15 +215,15 @@
 msgid "Too many failed login attempts, please retry later."
 msgstr ""
 "Çok fazla başarısız oturum açma denemesi, lütfen daha sonra tekrar "
 "deneyin."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
-msgstr "Bu yönetici parolası doğru değil. Sadece %(num)d tane deneme kaldı."
+msgstr "Bu yönetici parolası doğru değil. Yalnızca %(num)d tane deneme kaldı."
 
 msgid "Provided token is invalid"
 msgstr "Sağlanan belirteç geçersiz"
 
 msgid "This private code is not the right one"
 msgstr "Bu özel kod doğru değil"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/uk/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/uk/LC_MESSAGES/messages.mo`

 * *Files 26% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,23 +1,22 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
+"Project-Id-Version: Ukrainian (I Hate Money)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2020-05-21 18:48+0000\n"
-"Last-Translator: Andrew Zaplitnyak <zaplitnyak@gmail.com>\n"
-"Language: uk\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: Ukrainian <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/uk/>\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2\n"
+"Language: uk\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
+"Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 4.14.1-dev\n"
 
 msgid "%(member)s has been added"
 msgstr "%(member)s додано"
 
 msgid "%(name)s is part of this project again"
 msgstr "%(name)s знову частина цього проекту"
 
@@ -49,22 +48,28 @@
 msgid "Currency"
 msgstr "Валюта"
 
 msgid "Date"
 msgstr "Дата"
 
 msgid "Default Currency"
-msgstr "Стандартна валюта"
+msgstr "Валюта по замовчуванню"
 
 msgid "Email"
 msgstr "Е-пошта"
 
 msgid "Enable project history"
 msgstr "Ввімкнути історію проєкту"
 
+msgid "Enter a new code if you want to change it"
+msgstr "Введіть новий код якщо бажаєте його змінити"
+
+msgid "Enter private code to confirm deletion"
+msgstr "Введіть приватний ключ для підтвердження видалення."
+
 msgid "External link"
 msgstr "Зовнішнє посилання"
 
 msgid "For whom?"
 msgstr "Для кого?"
 
 msgid "Get in"
@@ -75,20 +80,26 @@
 
 msgid "Import previously exported JSON file"
 msgstr "Імпортувати попередньо експортований JSON файл"
 
 msgid "Invalid JSON"
 msgstr "Недійсний JSON"
 
+msgid "Invalid private code."
+msgstr "Помилковий приватний ключ"
+
 msgid "Invalid token"
 msgstr "Недійсний токен"
 
 msgid "Name"
 msgstr "Назва"
 
+msgid "New private code"
+msgstr "Новий приватний код"
+
 msgid "No Currency"
 msgstr "Немає валюти"
 
 msgid "No token provided"
 msgstr "Не надано токен"
 
 msgid ""
@@ -107,14 +118,17 @@
 
 msgid "Password successfully reset."
 msgstr "Пароль з успіхом відновлено."
 
 msgid "Payer"
 msgstr "Платник"
 
+msgid "Please, validate the captcha to proceed."
+msgstr "Будь ласка, заповніть капчу для продовження."
+
 msgid "Private code"
 msgstr "Приватний код"
 
 msgid "Project"
 msgstr "Проєкт"
 
 msgid "Project default: %(currency)s"
@@ -137,14 +151,18 @@
 
 msgid "Send invites"
 msgstr "Відправити запрошення"
 
 msgid "Send me the code by email"
 msgstr "Надішліть мені код електронною поштою"
 
+msgid "Setting a default currency enables currency conversion between bills"
+msgstr ""
+"Встановлення типової валюти уможливлює конвертацію валюти між векселями"
+
 msgid "Submit"
 msgstr "Підтвердити"
 
 msgid "Submit and add a new one"
 msgstr "Підтвердити та додати ще один"
 
 msgid "The email %(email)s is not valid"
@@ -155,25 +173,35 @@
 
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "Цей пароль адміністратора не вірний. Залишилося тільки %(num)d спроб."
 
 msgid "This private code is not the right one"
 msgstr "Цей приватний код не підходить"
 
+msgid ""
+"This project cannot be set to 'no currency' because it contains bills in "
+"multiple currencies."
+msgstr ""
+"Цей проект не може бути встановлено у значення \"Без валюти\", оскільки він "
+"містить декілько валют в рахунках."
+
 msgid "This project does not exists"
 msgstr "Цей проєкт не існує"
 
 msgid "Too many failed login attempts, please retry later."
 msgstr "Забагато невдалих спроб увійти, будь ласка спробуйте пізніше."
 
+msgid "Unknown error"
+msgstr "Невідома помилка"
+
 msgid "Unknown project"
 msgstr "Невідомий проєкт"
 
 msgid "Use IP tracking for project history"
-msgstr "Слідкувати за мережевою адресою(IP) для історії проєкту"
+msgstr "Слідкувати за IP адресою для історії проєкту"
 
 msgid "Weight"
 msgstr "Вага"
 
 msgid "Weights should be positive"
 msgstr "Вага має бути додатною"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/uk/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/uk/LC_MESSAGES/messages.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,60 @@
-
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2020-05-21 18:48+0000\n"
-"Last-Translator: Andrew Zaplitnyak <zaplitnyak@gmail.com>\n"
+"PO-Revision-Date: 2022-09-17 10:24+0000\n"
+"Last-Translator: Dmytro Onopa <dmytro.onopa@gmail.com>\n"
+"Language-Team: Ukrainian <https://hosted.weblate.org/projects/i-hate-money/"
+"i-hate-money/uk/>\n"
 "Language: uk\n"
-"Language-Team: Ukrainian <https://hosted.weblate.org/projects/i-hate-"
-"money/i-hate-money/uk/>\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
+"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 4.14.1-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr "Не вірна сума чи вираз. Приймаються тільки числа та оператори + - * /."
 
 msgid "Project name"
 msgstr "Назва проєкту"
 
-#, fuzzy
 msgid "New private code"
-msgstr "Приватний код"
+msgstr "Новий приватний код"
 
 msgid "Enter a new code if you want to change it"
-msgstr ""
+msgstr "Введіть новий код якщо бажаєте його змінити"
 
 msgid "Email"
 msgstr "Е-пошта"
 
 msgid "Enable project history"
 msgstr "Ввімкнути історію проєкту"
 
 msgid "Use IP tracking for project history"
-msgstr "Слідкувати за мережевою адресою(IP) для історії проєкту"
+msgstr "Слідкувати за IP адресою для історії проєкту"
 
 msgid "Default Currency"
-msgstr "Стандартна валюта"
+msgstr "Валюта по замовчуванню"
 
 msgid "Setting a default currency enables currency conversion between bills"
-msgstr ""
+msgstr "Встановлення типової валюти уможливлює конвертацію валюти між векселями"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
+"Цей проект не може бути встановлено у значення \"Без валюти\", оскільки він "
+"містить декілько валют в рахунках."
 
 msgid "Import previously exported JSON file"
 msgstr "Імпортувати попередньо експортований JSON файл"
 
 msgid "Import"
 msgstr "Імпортувати"
 
@@ -77,26 +78,24 @@
 msgid "Which is a real currency: Euro or Petro dollar?"
 msgstr ""
 
 msgid "euro"
 msgstr ""
 
 msgid "Please, validate the captcha to proceed."
-msgstr ""
+msgstr "Будь ласка, заповніть капчу для продовження."
 
 msgid "Enter private code to confirm deletion"
-msgstr ""
+msgstr "Введіть приватний ключ для підтвердження видалення."
 
-#, fuzzy
 msgid "Unknown error"
-msgstr "Невідомий проєкт"
+msgstr "Невідома помилка"
 
-#, fuzzy
 msgid "Invalid private code."
-msgstr "Приватний код"
+msgstr "Помилковий приватний ключ"
 
 msgid "Get in"
 msgstr "Отримати в"
 
 msgid "Admin password"
 msgstr "Пароль адміністратора"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.0/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Chinese (Simplified) <https://hosted.weblate.org/projects/i-"
 "hate-money/i-hate-money/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.11-dev\n"
+"X-Generator: Weblate 4.14-dev\n"
 
 msgid ""
 "\n"
 "            <i>The table below reflects actions recorded prior to disabling "
 "project history. You can\n"
 "            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
 "target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
@@ -170,14 +170,18 @@
 
 msgid "Can't remember the password?"
 msgstr "忘记密码？"
 
 msgid "Cancel"
 msgstr "取消"
 
+msgid ""
+"Cannot add bills in multiple currencies to a project without default currency"
+msgstr "无法在没有设置默认货币的项目中添加多种货币的账单"
+
 msgid "Choose file"
 msgstr "选择文件"
 
 msgid "Clear Project History"
 msgstr "清除项目历史"
 
 msgid "Close"
@@ -496,17 +500,23 @@
 
 msgid "Password successfully reset."
 msgstr "密码重置成功。"
 
 msgid "Payer"
 msgstr "支付人"
 
+msgid "People to notify"
+msgstr "需要通知的人"
+
 msgid "Period"
 msgstr "期间"
 
+msgid "Please, validate the captcha to proceed."
+msgstr "请输入验证码以继续。"
+
 msgid "Privacy Settings"
 msgstr "隐私设置"
 
 msgid "Private code"
 msgstr "共享密钥"
 
 msgid "Project"
@@ -544,14 +554,17 @@
 
 msgid "Project successfully uploaded"
 msgstr "项目成功上传"
 
 msgid "Projects"
 msgstr "项目"
 
+msgid "Provided token is invalid"
+msgstr "所提供的口令无效"
+
 msgid "Reset password"
 msgstr "密码重置"
 
 msgid "Reset your password"
 msgstr "重设密码"
 
 msgid "Return to home page"
@@ -565,14 +578,17 @@
 
 msgid "Send the invitations"
 msgstr "发送邀请"
 
 msgid "Send via Emails"
 msgstr "邮件发送"
 
+msgid "Setting a default currency enables currency conversion between bills"
+msgstr "设置默认货币可实现账单之间的货币转换"
+
 msgid "Settings"
 msgstr "设置"
 
 msgid "Settle"
 msgstr "解决"
 
 msgid "Settle plans"
@@ -714,14 +730,17 @@
 
 msgid "What?"
 msgstr "什么？"
 
 msgid "When?"
 msgstr "什么时候？"
 
+msgid "Which is a real currency: Euro or Petro dollar?"
+msgstr "以下哪种是真实的货币：欧元还是“石油美元”？"
+
 msgid "Who paid?"
 msgstr "谁付的钱？"
 
 msgid "Who pays?"
 msgstr "谁付款？"
 
 msgid "Who?"
@@ -773,14 +792,17 @@
 
 msgid "delete"
 msgstr "删除"
 
 msgid "edit"
 msgstr "编辑"
 
+msgid "euro"
+msgstr "欧元"
+
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "john.doe@example.com, mary.moe@site.com"
 
 msgid "reactivate"
 msgstr "激活"
 
 msgid "show"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.po` & `ihatemoney-6.0.0/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2022-01-24 05:55+0000\n"
-"Last-Translator: yzqzss <yzqzss@yandex.com>\n"
+"PO-Revision-Date: 2022-07-21 05:15+0000\n"
+"Last-Translator: z.liu <zwliu07@live.com>\n"
 "Language-Team: Chinese (Simplified) <https://hosted.weblate.org/projects/"
 "i-hate-money/i-hate-money/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.11-dev\n"
+"X-Generator: Weblate 4.14-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr "金额或符号无效。仅限数字与+-*/符号。"
 
@@ -38,15 +38,15 @@
 msgid "Use IP tracking for project history"
 msgstr "用IP追踪项目历史"
 
 msgid "Default Currency"
 msgstr "默认货币"
 
 msgid "Setting a default currency enables currency conversion between bills"
-msgstr ""
+msgstr "设置默认货币可实现账单之间的货币转换"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr "此项目不能设置为“无货币”，因为它包含多种货币的账单。"
 
 msgid "Import previously exported JSON file"
@@ -67,22 +67,21 @@
 #, python-format
 msgid ""
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
 msgstr "账目(“%(project)s”)已存在，请选择一个新名称"
 
 msgid "Which is a real currency: Euro or Petro dollar?"
-msgstr ""
+msgstr "以下哪种是真实的货币：欧元还是“石油美元”？"
 
-#, fuzzy
 msgid "euro"
-msgstr "期间"
+msgstr "欧元"
 
 msgid "Please, validate the captcha to proceed."
-msgstr ""
+msgstr "请输入验证码以继续。"
 
 msgid "Enter private code to confirm deletion"
 msgstr "请输入专用代码以确认删除"
 
 msgid "Unknown error"
 msgstr "未知错误"
 
@@ -167,15 +166,15 @@
 msgstr "成员 %(name)s 被重新激活"
 
 #, fuzzy
 msgid "This project already have this participant"
 msgstr "此项目已经包含此成员了"
 
 msgid "People to notify"
-msgstr ""
+msgstr "需要通知的人"
 
 msgid "Send invites"
 msgstr "发送邀请"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "此邮箱%(email)s不存在"
@@ -211,15 +210,15 @@
 msgstr "登录失败次数过多，请稍后重试。"
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "管理密码有误，只剩 %(num)d次尝试机会。"
 
 msgid "Provided token is invalid"
-msgstr ""
+msgstr "所提供的口令无效"
 
 msgid "This private code is not the right one"
 msgstr "专用码不正确"
 
 #, python-format
 msgid "You have just created '%(project)s' to share your expenses"
 msgstr "你新建了一个‘%(project)s'来分担你的花费"
@@ -259,15 +258,15 @@
 
 msgid "Invalid JSON"
 msgstr "JSON无效"
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
-msgstr ""
+msgstr "无法在没有设置默认货币的项目中添加多种货币的账单"
 
 msgid "Project successfully deleted"
 msgstr "项目成功删除"
 
 msgid "Error deleting project"
 msgstr "删除项目时出错"
```

### Comparing `ihatemoney-5.2.0/ihatemoney/utils.py` & `ihatemoney-6.0.0/ihatemoney/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 import ast
 import csv
-from datetime import datetime, timedelta
 import email.utils
 from enum import Enum
 from io import BytesIO, StringIO, TextIOWrapper
 from json import JSONEncoder, dumps
 import operator
 import os
 import re
 import smtplib
 import socket
 
 from babel import Locale
 from babel.numbers import get_currency_name, get_currency_symbol
 from flask import current_app, flash, redirect, render_template
 from flask_babel import get_locale, lazy_gettext as _
+from flask_limiter import Limiter
+from flask_limiter.util import get_remote_address
 import jinja2
 from markupsafe import Markup, escape
 from werkzeug.exceptions import HTTPException
 from werkzeug.routing import RoutingException
 
+limiter = limiter = Limiter(
+    current_app,
+    key_func=get_remote_address,
+    storage_uri="memory://",
+)
+
 
 def slugify(value):
     """Normalizes string, converts to lowercase, removes non-alpha characters,
     and converts spaces to hyphens.
     """
     if isinstance(value, str):
         import unicodedata
@@ -53,23 +60,27 @@
     """Helper to flash a message for email errors. It will also show the
     admin email as a contact if MAIL_DEFAULT_SENDER is set to not the
     default value and SHOW_ADMIN_EMAIL is True.
     """
     (admin_name, admin_email) = email.utils.parseaddr(
         current_app.config.get("MAIL_DEFAULT_SENDER")
     )
-    error_extension = "."
+    error_extension = _("Please check the email configuration of the server.")
     if admin_email != "admin@example.com" and current_app.config.get(
         "SHOW_ADMIN_EMAIL"
     ):
-        error_extension = f" or contact the administrator at {admin_email}."
+        error_extension = _(
+            "Please check the email configuration of the server "
+            "or contact the administrator: %(admin_email)s",
+            admin_email=admin_email,
+        )
 
     flash(
-        _(
-            f"{error_message} Please check the email configuration of the server{error_extension}"
+        "{error_message} {error_extension}".format(
+            error_message=error_message, error_extension=error_extension
         ),
         category=category,
     )
 
 
 class Redirect303(HTTPException, RoutingException):
 
@@ -148,27 +159,41 @@
 def list_of_dicts2json(dict_to_convert):
     """Take a list of dictionnaries and turns it into
     a json in-memory file
     """
     return BytesIO(dumps(dict_to_convert).encode("utf-8"))
 
 
+def escape_csv_formulae(value):
+    # See https://owasp.org/www-community/attacks/CSV_Injection
+    if (
+        value
+        and isinstance(value, str)
+        and value[0] in ["=", "+", "-", "@", "\t", "\n"]
+    ):
+        return f"'{value}"
+    return value
+
+
 def list_of_dicts2csv(dict_to_convert):
     """Take a list of dictionnaries and turns it into
     a csv in-memory file, assume all dict have the same keys
     """
     # CSV writer has a different behavior in PY2 and PY3
     # http://stackoverflow.com/a/37974772
     try:
         csv_file = StringIO()
         # using list() for py3.4 compat. Otherwise, writerows() fails
         # (expecting a sequence getting a view)
         csv_data = [list(dict_to_convert[0].keys())]
         for dic in dict_to_convert:
-            csv_data.append([dic[h] for h in dict_to_convert[0].keys()])
+            csv_data.append(
+                [escape_csv_formulae(dic[h]) for h in dict_to_convert[0].keys()]
+            )
+            # csv_data.append([dic[h] for h in dict_to_convert[0].keys()])
     except (KeyError, IndexError):
         csv_data = []
     writer = csv.writer(csv_file)
     writer.writerows(csv_data)
     csv_file.seek(0)
     csv_file = BytesIO(csv_file.getvalue().encode("utf-8"))
     return csv_file
@@ -195,53 +220,14 @@
         r["amount"] = float(r["amount"])
         r["payer_weight"] = float(r["payer_weight"])
         r["owers"] = [o.strip() for o in r["owers"].split(",")]
         result.append(r)
     return result
 
 
-class LoginThrottler:
-    """Simple login throttler used to limit authentication attempts based on client's ip address.
-    When using multiple workers, remaining number of attempts can get inconsistent
-    but will still be limited to num_workers * max_attempts.
-    """
-
-    def __init__(self, max_attempts=3, delay=1):
-        self._max_attempts = max_attempts
-        # Delay in minutes before resetting the attempts counter
-        self._delay = delay
-        self._attempts = {}
-
-    def get_remaining_attempts(self, ip):
-        return self._max_attempts - self._attempts.get(ip, [datetime.now(), 0])[1]
-
-    def increment_attempts_counter(self, ip):
-        # Reset all attempt counters when they get hungry for memory
-        if len(self._attempts) > 10000:
-            self.__init__()
-        if self._attempts.get(ip) is None:
-            # Store first attempt date and number of attempts since
-            self._attempts[ip] = [datetime.now(), 0]
-        self._attempts.get(ip)[1] += 1
-
-    def is_login_allowed(self, ip):
-        if self._attempts.get(ip) is None:
-            return True
-        # When the delay is expired, reset the counter
-        if datetime.now() - self._attempts.get(ip)[0] > timedelta(minutes=self._delay):
-            self.reset(ip)
-            return True
-        if self._attempts.get(ip)[1] >= self._max_attempts:
-            return False
-        return True
-
-    def reset(self, ip):
-        self._attempts.pop(ip, None)
-
-
 def create_jinja_env(folder, strict_rendering=False):
     """Creates and return a Jinja2 Environment object, used, to load the
     templates.
 
     :param strict_rendering:
         if set to `True`, all templates which use an undefined variable will
         throw an exception (default to `False`).
```

### Comparing `ihatemoney-5.2.0/ihatemoney/versioning.py` & `ihatemoney-6.0.0/ihatemoney/versioning.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-5.2.0/ihatemoney/web.py` & `ihatemoney-6.0.0/ihatemoney/web.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,70 +7,73 @@
 Basically, this blueprint takes care of the authentication and provides
 some shortcuts to make your life better when coding (see `pull_project`
 and `add_project_id` for a quick overview)
 """
 from functools import wraps
 import json
 import os
+from urllib.parse import urlparse, urlunparse
 
 from flask import (
     Blueprint,
     abort,
     current_app,
     flash,
     g,
+    make_response,
     redirect,
     render_template,
     request,
     send_file,
     send_from_directory,
     session,
     url_for,
 )
 from flask_babel import gettext as _
 from flask_mail import Message
+import qrcode
+import qrcode.image.svg
 from sqlalchemy_continuum import Operation
 from werkzeug.exceptions import NotFound
 from werkzeug.security import check_password_hash, generate_password_hash
 
 from ihatemoney.currency_convertor import CurrencyConverter
 from ihatemoney.emails import send_creation_email
 from ihatemoney.forms import (
     AdminAuthenticationForm,
     AuthenticationForm,
     DestructiveActionProjectForm,
     EditProjectForm,
     EmptyForm,
     ImportProjectForm,
     InviteForm,
+    LogoutForm,
     MemberForm,
     PasswordReminder,
     ProjectForm,
     ProjectFormWithCaptcha,
     ResetPasswordForm,
     get_billform_for,
 )
 from ihatemoney.history import get_history, get_history_queries, purge_history
 from ihatemoney.models import Bill, LoggingMode, Person, Project, db
 from ihatemoney.utils import (
-    LoginThrottler,
     Redirect303,
     csv2list_of_dicts,
     flash_email_error,
     format_form_errors,
+    limiter,
     list_of_dicts2csv,
     list_of_dicts2json,
     render_localized_template,
     send_email,
 )
 
 main = Blueprint("main", __name__)
 
-login_throttler = LoginThrottler(max_attempts=3, delay=1)
-
 
 def requires_admin(bypass=None):
     """Require admin permissions for @requires_admin decorated endpoints.
 
     This has no effect if the ADMIN_PASSWORD is empty.
 
     :param bypass: Used to conditionnaly bypass the admin authentication.
@@ -115,14 +118,15 @@
     in order to use it in the layout template.
     """
 
     g.show_admin_dashboard_link = (
         current_app.config["ACTIVATE_ADMIN_DASHBOARD"]
         and current_app.config["ADMIN_PASSWORD"]
     )
+    g.logout_form = LogoutForm()
 
 
 @main.url_value_preprocessor
 def pull_project(endpoint, values):
     """When a request contains a project_id value, transform it directly
     into a project by checking the credentials stored in the session.
 
@@ -152,77 +156,86 @@
 
 
 @main.route("/healthcheck", methods=["GET"])
 def health():
     return "OK"
 
 
+def admin_limit(limit):
+    return make_response(
+        render_template(
+            "admin.html",
+            breached_limit=limit,
+            limit_message=_("Too many failed login attempts."),
+        )
+    )
+
+
 @main.route("/admin", methods=["GET", "POST"])
+@limiter.limit(
+    "3/minute",
+    on_breach=admin_limit,
+    methods=["POST"],
+)
 def admin():
     """Admin authentication.
 
     When ADMIN_PASSWORD is empty, admin authentication is deactivated.
     """
     form = AdminAuthenticationForm()
     goto = request.args.get("goto", url_for(".home"))
     is_admin_auth_enabled = bool(current_app.config["ADMIN_PASSWORD"])
-    if request.method == "POST":
-        client_ip = request.remote_addr
-        if not login_throttler.is_login_allowed(client_ip):
-            msg = _("Too many failed login attempts, please retry later.")
-            form["admin_password"].errors = [msg]
-            return render_template(
-                "admin.html",
-                form=form,
-                admin_auth=True,
-                is_admin_auth_enabled=is_admin_auth_enabled,
-            )
-        if form.validate():
-            # Valid password
-            if check_password_hash(
-                current_app.config["ADMIN_PASSWORD"], form.admin_password.data
-            ):
-                session["is_admin"] = True
-                session.update()
-                login_throttler.reset(client_ip)
-                return redirect(goto)
-            # Invalid password
-            login_throttler.increment_attempts_counter(client_ip)
+    if request.method == "POST" and form.validate():
+        # Valid password
+        if check_password_hash(
+            current_app.config["ADMIN_PASSWORD"], form.admin_password.data
+        ):
+            session["is_admin"] = True
+            session.update()
+            return redirect(goto)
+        if limiter.current_limit is not None:
             msg = _(
                 "This admin password is not the right one. Only %(num)d attempts left.",
-                num=login_throttler.get_remaining_attempts(client_ip),
+                # If the limiter is disabled, there is no current limit
+                num=limiter.current_limit.remaining,
             )
             form["admin_password"].errors = [msg]
     return render_template(
         "admin.html",
         form=form,
         admin_auth=True,
         is_admin_auth_enabled=is_admin_auth_enabled,
     )
 
 
+def set_authorized_project(project: Project):
+    # maintain a list of visited projects
+    new_project = {project.id: project.name}
+    if "projects" not in session:
+        session["projects"] = new_project
+    else:
+        # add the project on the top of the list
+        session["projects"] = {**new_project, **session["projects"]}
+    session[project.id] = True
+    # Set session to permanent to make language choice persist
+    session.permanent = True
+    session.update()
+
+
 @main.route("/<project_id>/join/<string:token>", methods=["GET"])
 def join_project(token):
     project_id = g.project.id
     verified_project_id = Project.verify_token(
         token, token_type="auth", project_id=project_id
     )
     if verified_project_id != project_id:
         flash(_("Provided token is invalid"), "danger")
         return redirect("/")
 
-    # maintain a list of visited projects
-    if "projects" not in session:
-        session["projects"] = []
-    # add the project on the top of the list
-    session["projects"].insert(0, (project_id, g.project.name))
-    session[project_id] = True
-    # Set session to permanent to make language choice persist
-    session.permanent = True
-    session.update()
+    set_authorized_project(g.project)
     return redirect(url_for(".list_bills"))
 
 
 @main.route("/authenticate", methods=["GET", "POST"])
 def authenticate(project_id=None):
     """Authentication form"""
     form = AuthenticationForm()
@@ -243,23 +256,15 @@
     if session.get(project_id):
         setattr(g, "project", project)
         return redirect(url_for(".list_bills"))
 
     # else do form authentication authentication
     is_post_auth = request.method == "POST" and form.validate()
     if is_post_auth and check_password_hash(project.password, form.password.data):
-        # maintain a list of visited projects
-        if "projects" not in session:
-            session["projects"] = []
-        # add the project on the top of the list
-        session["projects"].insert(0, (project_id, project.name))
-        session[project_id] = True
-        # Set session to permanent to make language choice persist
-        session.permanent = True
-        session.update()
+        set_authorized_project(project)
         setattr(g, "project", project)
         return redirect(url_for(".list_bills"))
     if is_post_auth and not check_password_hash(project.password, form.password.data):
         msg = _("This private code is not the right one")
         form["password"].errors = [msg]
 
     return render_template("authenticate.html", form=form)
@@ -327,16 +332,18 @@
                 flash(
                     _("A reminder email has just been sent to you"), category="success"
                 )
             else:
                 # Display the error as a simple "info" alert, because it's
                 # not critical and doesn't prevent using the project.
                 flash_email_error(
-                    "We tried to send you an reminder email, but there was an error. "
-                    "You can still use the project normally.",
+                    _(
+                        "We tried to send you an reminder email, but there was an error. "
+                        "You can still use the project normally."
+                    ),
                     category="info",
                 )
             return redirect(url_for(".list_bills", project_id=project.id))
 
     return render_template("create_project.html", form=form)
 
 
@@ -354,16 +361,18 @@
                 recipients=[project.contact_email],
             )
             success = send_email(remind_message)
             if success:
                 return redirect(url_for(".password_reminder_sent"))
             else:
                 flash_email_error(
-                    "Sorry, there was an error while sending you an email with "
-                    "password reset instructions."
+                    _(
+                        "Sorry, there was an error while sending you an email with "
+                        "password reset instructions."
+                    )
                 )
                 # Fall-through: we stay on the same page and display the form again
     return render_template("password_reminder.html", form=form)
 
 
 @main.route("/password-reminder-sent", methods=["GET"])
 def password_reminder_sent():
@@ -460,15 +469,17 @@
             ]
             currencies = set()
             for b in bills:
                 if b.get("currency", "") in ["", "XXX"]:
                     b["currency"] = g.project.default_currency
                 for a in attr:
                     if a not in b:
-                        raise ValueError(_("Missing attribute {}").format(a))
+                        raise ValueError(
+                            _("Missing attribute: %(attribute)s", attribute=a)
+                        )
                 currencies.add(b["currency"])
 
             # Additional checks if project has no default currency
             if g.project.default_currency == CurrencyConverter.no_currency:
                 # If bills have currencies, they must be consistent
                 if len(currencies - {CurrencyConverter.no_currency}) >= 2:
                     raise ValueError(
@@ -485,15 +496,15 @@
 
             flash(_("Project successfully uploaded"))
             return redirect(url_for("main.list_bills"))
         except ValueError as b:
             flash(b.args[0], category="danger")
     else:
         for component, errors in form.errors.items():
-            flash(_(component + ": ") + ", ".join(errors), category="danger")
+            flash(component + ": " + ", ".join(errors), category="danger")
     return redirect(request.headers.get("Referer") or url_for(".edit_project"))
 
 
 @main.route("/<project_id>/delete", methods=["POST"])
 def delete_project():
     form = DestructiveActionProjectForm(id=g.project.id)
     if form.validate():
@@ -527,19 +538,31 @@
     return send_file(
         file2export,
         download_name=f"{g.project.id}-{file}.{format}",
         as_attachment=True,
     )
 
 
-@main.route("/exit")
+@main.route("/exit", methods=["GET", "POST"])
 def exit():
-    # delete the session
-    session.clear()
-    return redirect(url_for(".home"))
+    # We must test it manually, because otherwise, it creates a project "exit"
+    if request.method == "GET":
+        abort(405)
+
+    form = LogoutForm()
+    if form.validate():
+        # delete the session
+        session.clear()
+        return redirect(url_for(".home"))
+    else:
+        flash(
+            format_form_errors(form, _("Unable to logout")),
+            category="danger",
+        )
+        return redirect(request.headers.get("Referer") or url_for(".home"))
 
 
 @main.route("/demo")
 def demo():
     """
     Authenticate the user for the demonstration project and redirects to
     the bills list for this project.
@@ -565,32 +588,49 @@
     form = InviteForm()
 
     if request.method == "POST":
         if form.validate():
             # send the email
             message_body = render_localized_template("invitation_mail")
             message_title = _(
-                "You have been invited to share your " "expenses for %(project)s",
+                "You have been invited to share your expenses for %(project)s",
                 project=g.project.name,
             )
             msg = Message(
                 message_title,
                 body=message_body,
                 recipients=[email.strip() for email in form.emails.data.split(",")],
             )
             success = send_email(msg)
             if success:
                 flash(_("Your invitations have been sent"), category="success")
                 return redirect(url_for(".list_bills"))
             else:
                 flash_email_error(
-                    "Sorry, there was an error while trying to send the invitation emails."
+                    _(
+                        "Sorry, there was an error while trying to send the invitation emails."
+                    )
                 )
                 # Fall-through: we stay on the same page and display the form again
-    return render_template("send_invites.html", form=form)
+
+    # Generate the SVG QRCode.
+    invite_link = url_for(
+        ".join_project",
+        project_id=g.project.id,
+        token=g.project.generate_token(),
+        _external=True,
+    )
+    invite_link = urlunparse(urlparse(invite_link)._replace(scheme="ihatemoney"))
+    qr = qrcode.QRCode(image_factory=qrcode.image.svg.SvgPathImage)
+    qr.add_data(invite_link)
+    qr.make(fit=True)
+    img = qr.make_image(attrib={"class": "qrcode"})
+    qrcode_svg = img.to_string().decode()
+
+    return render_template("send_invites.html", form=form, qrcode=qrcode_svg)
 
 
 @main.route("/<project_id>/")
 def list_bills():
     bill_form = get_billform_for(g.project)
     # Used for CSRF validation
     csrf_form = EmptyForm()
@@ -761,15 +801,18 @@
 
 @main.route("/lang/<lang>")
 def change_lang(lang):
     if lang in current_app.config["SUPPORTED_LANGUAGES"]:
         session["lang"] = lang
         session.update()
     else:
-        flash(_(f"{lang} is not a supported language"), category="warning")
+        flash(
+            _("%(lang)s is not a supported language", lang=lang),
+            category="warning",
+        )
 
     return redirect(request.headers.get("Referer") or url_for(".home"))
 
 
 @main.route("/<project_id>/settle_bills")
 def settle_bill():
     """Compute the sum each one have to pay to each other and display it"""
@@ -852,18 +895,27 @@
 @main.route("/dashboard")
 @requires_admin()
 def dashboard():
     is_admin_dashboard_activated = current_app.config["ACTIVATE_ADMIN_DASHBOARD"]
     return render_template(
         "dashboard.html",
         projects=Project.query.all(),
+        delete_project_form=DestructiveActionProjectForm,
         is_admin_dashboard_activated=is_admin_dashboard_activated,
     )
 
 
+@main.route("/dashboard/<project_id>/delete", methods=["POST"])
+@requires_admin()
+def dashboard_delete_project():
+    g.project.remove_project()
+    flash(_("Project successfully deleted"))
+    return redirect(request.headers.get("Referer") or url_for(".home"))
+
+
 @main.route("/favicon.ico")
 def favicon():
     return send_from_directory(
         os.path.join(main.root_path, "static"),
         "favicon.ico",
         mimetype="image/vnd.microsoft.icon",
     )
```

### Comparing `ihatemoney-5.2.0/ihatemoney.egg-info/PKG-INFO` & `ihatemoney-6.0.0/ihatemoney.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ihatemoney
-Version: 5.2.0
+Version: 6.0.0
 Summary: A simple shared budget manager web application.
 Home-page: https://github.com/spiral-project/ihatemoney
 Author: Alexis Métaireau & contributors
 Author-email: alexis@notmyidea.org
 License: Custom BSD Beerware
 Description: UNKNOWN
 Keywords: web,budget
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Provides-Extra: database
 Provides-Extra: dev
 Provides-Extra: doc
```

### Comparing `ihatemoney-5.2.0/ihatemoney.egg-info/SOURCES.txt` & `ihatemoney-6.0.0/ihatemoney.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ihatemoney/currency_convertor.py
 ihatemoney/default_settings.py
 ihatemoney/emails.py
 ihatemoney/forms.py
 ihatemoney/history.py
 ihatemoney/manage.py
 ihatemoney/models.py
+ihatemoney/monkeypath_continuum.py
 ihatemoney/run.py
 ihatemoney/utils.py
 ihatemoney/versioning.py
 ihatemoney/web.py
 ihatemoney/wsgi.py
 ihatemoney.egg-info/PKG-INFO
 ihatemoney.egg-info/SOURCES.txt
@@ -120,14 +121,15 @@
 ihatemoney/templates/create_project.html
 ihatemoney/templates/dashboard.html
 ihatemoney/templates/display_errors.html
 ihatemoney/templates/download_mobile_app.html
 ihatemoney/templates/edit_member.html
 ihatemoney/templates/edit_project.html
 ihatemoney/templates/forms.html
+ihatemoney/templates/helpers.js
 ihatemoney/templates/history.html
 ihatemoney/templates/home.html
 ihatemoney/templates/invitation_mail.en.j2
 ihatemoney/templates/invitation_mail.fr.j2
 ihatemoney/templates/layout.html
 ihatemoney/templates/list_bills.html
 ihatemoney/templates/password_reminder.en.j2
@@ -150,16 +152,20 @@
 ihatemoney/tests/ihatemoney.cfg
 ihatemoney/tests/ihatemoney_envvar.cfg
 ihatemoney/tests/import_test.py
 ihatemoney/tests/main_test.py
 ihatemoney/tests/common/__init__.py
 ihatemoney/tests/common/help_functions.py
 ihatemoney/tests/common/ihatemoney_testcase.py
+ihatemoney/translations/bn/LC_MESSAGES/messages.mo
+ihatemoney/translations/bn/LC_MESSAGES/messages.po
 ihatemoney/translations/bn_BD/LC_MESSAGES/messages.mo
 ihatemoney/translations/bn_BD/LC_MESSAGES/messages.po
+ihatemoney/translations/ca/LC_MESSAGES/messages.mo
+ihatemoney/translations/ca/LC_MESSAGES/messages.po
 ihatemoney/translations/cs/LC_MESSAGES/messages.mo
 ihatemoney/translations/cs/LC_MESSAGES/messages.po
 ihatemoney/translations/de/LC_MESSAGES/messages.mo
 ihatemoney/translations/de/LC_MESSAGES/messages.po
 ihatemoney/translations/el/LC_MESSAGES/messages.mo
 ihatemoney/translations/el/LC_MESSAGES/messages.po
 ihatemoney/translations/eo/LC_MESSAGES/messages.mo
@@ -168,16 +174,20 @@
 ihatemoney/translations/es/LC_MESSAGES/messages.po
 ihatemoney/translations/es_419/LC_MESSAGES/messages.mo
 ihatemoney/translations/es_419/LC_MESSAGES/messages.po
 ihatemoney/translations/fa/LC_MESSAGES/messages.mo
 ihatemoney/translations/fa/LC_MESSAGES/messages.po
 ihatemoney/translations/fr/LC_MESSAGES/messages.mo
 ihatemoney/translations/fr/LC_MESSAGES/messages.po
+ihatemoney/translations/he/LC_MESSAGES/messages.mo
+ihatemoney/translations/he/LC_MESSAGES/messages.po
 ihatemoney/translations/hi/LC_MESSAGES/messages.mo
 ihatemoney/translations/hi/LC_MESSAGES/messages.po
+ihatemoney/translations/hu/LC_MESSAGES/messages.mo
+ihatemoney/translations/hu/LC_MESSAGES/messages.po
 ihatemoney/translations/id/LC_MESSAGES/messages.mo
 ihatemoney/translations/id/LC_MESSAGES/messages.po
 ihatemoney/translations/it/LC_MESSAGES/messages.mo
 ihatemoney/translations/it/LC_MESSAGES/messages.po
 ihatemoney/translations/ja/LC_MESSAGES/messages.mo
 ihatemoney/translations/ja/LC_MESSAGES/messages.po
 ihatemoney/translations/kn/LC_MESSAGES/messages.mo
@@ -199,15 +209,20 @@
 ihatemoney/translations/sr/LC_MESSAGES/messages.mo
 ihatemoney/translations/sr/LC_MESSAGES/messages.po
 ihatemoney/translations/sv/LC_MESSAGES/messages.mo
 ihatemoney/translations/sv/LC_MESSAGES/messages.po
 ihatemoney/translations/ta/LC_MESSAGES/messages.mo
 ihatemoney/translations/ta/LC_MESSAGES/messages.po
 ihatemoney/translations/te/LC_MESSAGES/messages.mo
+ihatemoney/translations/te/LC_MESSAGES/messages.po
 ihatemoney/translations/th/LC_MESSAGES/messages.mo
 ihatemoney/translations/th/LC_MESSAGES/messages.po
 ihatemoney/translations/tr/LC_MESSAGES/messages.mo
 ihatemoney/translations/tr/LC_MESSAGES/messages.po
 ihatemoney/translations/uk/LC_MESSAGES/messages.mo
 ihatemoney/translations/uk/LC_MESSAGES/messages.po
+ihatemoney/translations/ur/LC_MESSAGES/messages.mo
+ihatemoney/translations/ur/LC_MESSAGES/messages.po
+ihatemoney/translations/vi/LC_MESSAGES/messages.mo
+ihatemoney/translations/vi/LC_MESSAGES/messages.po
 ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.mo
 ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.po
```

### Comparing `ihatemoney-5.2.0/setup.cfg` & `ihatemoney-6.0.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,74 @@
 [metadata]
 name = ihatemoney
-version = 5.2.0
+version = 6.0.0
 url = https://github.com/spiral-project/ihatemoney
 description = A simple shared budget manager web application.
 long_description = file: README.rst, CHANGELOG.rst
 author = Alexis Métaireau & contributors
 author_email = alexis@notmyidea.org
 keywords = web, budget
 license = Custom BSD Beerware
 classifiers = 
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 
 [options]
 packages = find:
 include_package_data = True
 zip_safe = False
 install_requires = 
 	blinker>=1.4,<2
 	cachetools>=4.1,<5
 	debts>=0.5,<1
-	email_validator>=1.0,<2
-	Flask-Babel>=1.0,<3
+	email_validator>=1.0,<3
+	Flask-Babel>=1.0,<4
 	Flask-Cors>=3.0.8,<4
+	Flask-Limiter>=2.6,<3
 	Flask-Mail>=0.9.1,<1
-	Flask-Migrate>=2.5.3,<4  # Not following semantic versioning (e.g. https://github.com/miguelgrinberg/flask-migrate/commit/1af28ba273de6c88544623b8dc02dd539340294b)
+	Flask-Migrate>=2.5.3,<5  # Not following semantic versioning (e.g. https://github.com/miguelgrinberg/flask-migrate/commit/1af28ba273de6c88544623b8dc02dd539340294b)
 	Flask-RESTful>=0.3.9,<1
 	Flask-SQLAlchemy>=2.4,<3
 	Flask-Talisman>=0.8,<2
 	Flask-WTF>=0.14.3,<2
 	WTForms>=2.3.1,<3.1
-	Flask>=2,<3
+	Flask>=2,<2.3
+	Werkzeug>=2,<2.3
 	itsdangerous>=2,<3
 	Jinja2>=3,<4
-	requests>=2.22,<3
+	qrcode>=7.1,<8
+	requests>=2.25,<3
 	SQLAlchemy-Continuum>=1.3.12,<2
-	SQLAlchemy>=1.3.0,<1.4  # New 1.4 changes API, see #728
+	SQLAlchemy>=1.3.0,<1.5  # New 1.4 changes API, see #728
 	python-dateutil
 
 [options.extras_require]
 database = 
-	psycopg2-binary>=2.9,<3
+	psycopg2-binary>=2.9.2,<3
 	PyMySQL>=0.9,<1.1
 dev = 
-	black>=19.10b0 ; python_version >= '3.6'
-	flake8>=3.7.9
+	black==23.3.0
+	flake8==5.0.4
+	isort==5.11.5
+	vermin==1.5.2
 	Flask-Testing>=0.8.1
-	isort>=5.0.0
 	pytest>=6.2.5
 	tox>=3.14.6
 	zest.releaser>=6.20.1
-	vermin
 doc = 
-	Sphinx==4.4.0
-	docutils==0.17.1
-	myst-parser
+	Sphinx>=7.0.1,<8
+	docutils==0.20.1
+	myst-parser>=2,<3
 
 [options.entry_points]
 flask.commands = 
 	generate_password_hash = ihatemoney.manage:password_hash
 	generate-config = ihatemoney.manage:generate_config
 console_scripts = 
 	ihatemoney = ihatemoney.manage:cli
```

