# Comparing `tmp/mgtron-2.19.5.tar.gz` & `tmp/mgtron-2.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgtron-2.19.5.tar", last modified: Tue Jul 11 20:54:07 2023, max compression
+gzip compressed data, was "mgtron-2.20.0.tar", last modified: Thu Jul 13 17:43:10 2023, max compression
```

## Comparing `mgtron-2.19.5.tar` & `mgtron-2.20.0.tar`

### file list

```diff
@@ -1,113 +1,114 @@
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.822219 mgtron-2.19.5/
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.625548 mgtron-2.19.5/.github/
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.638882 mgtron-2.19.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      602 2023-06-23 15:16:00.000000 mgtron-2.19.5/.github/ISSUE_TEMPLATE/mgtron--.md
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1524 2023-06-23 15:16:00.000000 mgtron-2.19.5/.github/ISSUE_TEMPLATE/mgtron_issue.yml
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.638882 mgtron-2.19.5/.github/workflows/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      520 2023-06-30 12:43:52.000000 mgtron-2.19.5/.github/workflows/black_actions.yml
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      830 2023-06-30 12:43:52.000000 mgtron-2.19.5/.github/workflows/pypi_action.yml
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      387 2023-07-10 14:37:39.000000 mgtron-2.19.5/.gitignore
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9254 2023-07-10 21:07:07.000000 mgtron-2.19.5/CHANGELOG.md
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      957 2023-06-23 15:16:00.000000 mgtron-2.19.5/LICENSE.rst
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4198 2023-07-11 20:54:07.822219 mgtron-2.19.5/PKG-INFO
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3699 2023-06-23 15:16:00.000000 mgtron-2.19.5/README.md
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.652216 mgtron-2.19.5/docs/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    17614 2023-06-23 15:16:01.000000 mgtron-2.19.5/docs/MGTron Command Description.docx
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    23088 2023-06-23 15:16:01.000000 mgtron-2.19.5/docs/MGTron Function Descriptions.docx
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.662216 mgtron-2.19.5/mgtron.egg-info/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4198 2023-07-11 20:54:07.000000 mgtron-2.19.5/mgtron.egg-info/PKG-INFO
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2334 2023-07-11 20:54:07.000000 mgtron-2.19.5/mgtron.egg-info/SOURCES.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        1 2023-07-11 20:54:07.000000 mgtron-2.19.5/mgtron.egg-info/dependency_links.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       37 2023-07-11 20:54:07.000000 mgtron-2.19.5/mgtron.egg-info/entry_points.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2085 2023-07-11 20:54:07.000000 mgtron-2.19.5/mgtron.egg-info/requires.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       19 2023-07-11 20:54:07.000000 mgtron-2.19.5/mgtron.egg-info/top_level.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1161 2023-07-10 14:37:39.000000 mgtron-2.19.5/pyproject.toml
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2022 2023-07-10 17:50:34.000000 mgtron-2.19.5/requirements.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       38 2023-07-11 20:54:07.822219 mgtron-2.19.5/setup.cfg
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.665549 mgtron-2.19.5/src/
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        1 2023-06-28 15:56:43.000000 mgtron-2.19.5/src/__init__.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.738884 mgtron-2.19.5/src/assets/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    83964 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/assets/CA logo without subtext.JPG
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    65978 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/assets/CA_subheading.png
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 12776672 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/assets/blueio_rs
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1303 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/assets/init_cellantenna.sh
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      723 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/assets/log_read
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      291 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/assets/mgtron.desktop
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2655 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/assets/mgtron.svg
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    67646 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/assets/network-wireless.ico
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 11314288 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/assets/wifi_rs
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.782218 mgtron-2.19.5/src/ble/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/ble/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3130 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/ble/ble_data.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     8527 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/ble/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      859 2023-06-30 12:43:53.000000 mgtron-2.19.5/src/ble/scanning.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.795551 mgtron-2.19.5/src/db/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/channel_1.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/channel_2.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/channel_3.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/channel_4.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/channel_5.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/channel_6.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/channel_7.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/channel_8.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10853 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/db/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2516 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/init_db.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10906 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/long_save.json
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/long_save.json.lock
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    49152 2023-07-10 14:18:59.000000 mgtron-2.19.5/src/db/mgtron_db.db
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9055 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/db/models.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1170 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/quick_save.json
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.798885 mgtron-2.19.5/src/globals/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/globals/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3642 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/globals/helpers.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.798885 mgtron-2.19.5/src/gui/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       80 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/__init__.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.805551 mgtron-2.19.5/src/gui/_configs/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/card_1.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/card_2.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/card_3.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/card_4.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/card_5.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/card_6.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      263 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/card_7.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/card_8.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       98 2023-06-21 12:37:32.000000 mgtron-2.19.5/src/gui/_configs/card_config.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      317 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/mission_alpha.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      292 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/mission_bravo.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      324 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/mission_charlie.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      312 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/mission_delta.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      273 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/mission_echo.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      313 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/mission_fox.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      279 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/mission_golf.ini
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.812218 mgtron-2.19.5/src/gui/fonts/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1260156 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/fonts/MesloLGS NF Bold Italic.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1251424 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/fonts/MesloLGS NF Italic.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1292408 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/fonts/MesloLGS NF Regular.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    51299 2023-07-11 18:27:32.000000 mgtron-2.19.5/src/gui/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10970 2023-07-10 20:18:55.000000 mgtron-2.19.5/src/gui/interface.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    43845 2023-07-11 18:29:09.000000 mgtron-2.19.5/src/main.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.815552 mgtron-2.19.5/src/tests/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       33 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/tests/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       70 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/tests/test_ble.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    63110 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/tests/test_configfiles.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    19824 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/tests/test_helpers.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.815552 mgtron-2.19.5/src/wifi/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/wifi/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      507 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/wifi/chasing.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    15668 2023-07-11 20:30:06.000000 mgtron-2.19.5/src/wifi/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9516 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/wifi/scanning.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.625548 mgtron-2.19.5/venv/
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.818885 mgtron-2.19.5/venv/bin/
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      665 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2html.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      787 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2html4.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1122 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2html5.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      864 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2latex.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      687 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2man.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      853 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2odt.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      659 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      672 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      708 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2s5.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      944 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2xetex.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      673 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2xml.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      741 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rstpep2html.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.724422 mgtron-2.20.0/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.697754 mgtron-2.20.0/.github/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.697754 mgtron-2.20.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      602 2023-06-23 15:16:00.000000 mgtron-2.20.0/.github/ISSUE_TEMPLATE/mgtron--.md
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1524 2023-06-23 15:16:00.000000 mgtron-2.20.0/.github/ISSUE_TEMPLATE/mgtron_issue.yml
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.697754 mgtron-2.20.0/.github/workflows/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      520 2023-06-30 12:43:52.000000 mgtron-2.20.0/.github/workflows/black_actions.yml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      830 2023-06-30 12:43:52.000000 mgtron-2.20.0/.github/workflows/pypi_action.yml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      409 2023-07-13 17:42:32.000000 mgtron-2.20.0/.gitignore
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9474 2023-07-13 17:42:32.000000 mgtron-2.20.0/CHANGELOG.md
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      957 2023-06-23 15:16:00.000000 mgtron-2.20.0/LICENSE.rst
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4198 2023-07-13 17:43:10.724422 mgtron-2.20.0/PKG-INFO
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3699 2023-06-23 15:16:00.000000 mgtron-2.20.0/README.md
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.697754 mgtron-2.20.0/docs/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    17614 2023-06-23 15:16:01.000000 mgtron-2.20.0/docs/MGTron Command Description.docx
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    23088 2023-06-23 15:16:01.000000 mgtron-2.20.0/docs/MGTron Function Descriptions.docx
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.701088 mgtron-2.20.0/mgtron.egg-info/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4198 2023-07-13 17:43:10.000000 mgtron-2.20.0/mgtron.egg-info/PKG-INFO
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2376 2023-07-13 17:43:10.000000 mgtron-2.20.0/mgtron.egg-info/SOURCES.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        1 2023-07-13 17:43:10.000000 mgtron-2.20.0/mgtron.egg-info/dependency_links.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       37 2023-07-13 17:43:10.000000 mgtron-2.20.0/mgtron.egg-info/entry_points.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2085 2023-07-13 17:43:10.000000 mgtron-2.20.0/mgtron.egg-info/requires.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       19 2023-07-13 17:43:10.000000 mgtron-2.20.0/mgtron.egg-info/top_level.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1161 2023-07-10 14:37:39.000000 mgtron-2.20.0/pyproject.toml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2022 2023-07-10 17:50:34.000000 mgtron-2.20.0/requirements.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       38 2023-07-13 17:43:10.724422 mgtron-2.20.0/setup.cfg
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.701088 mgtron-2.20.0/src/
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        1 2023-06-28 15:56:43.000000 mgtron-2.20.0/src/__init__.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.707754 mgtron-2.20.0/src/assets/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    83964 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/assets/CA logo without subtext.JPG
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    65978 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/assets/CA_subheading.png
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)   141680 2023-07-13 17:42:32.000000 mgtron-2.20.0/src/assets/MGTron Command Description.pdf
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 12776672 2023-07-10 14:37:39.000000 mgtron-2.20.0/src/assets/blueio_rs
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1303 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/assets/init_cellantenna.sh
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      723 2023-07-10 14:37:39.000000 mgtron-2.20.0/src/assets/log_read
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      291 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/assets/mgtron.desktop
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2655 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/assets/mgtron.svg
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    67646 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/assets/network-wireless.ico
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 11314288 2023-07-10 14:37:39.000000 mgtron-2.20.0/src/assets/wifi_rs
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.714421 mgtron-2.20.0/src/ble/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/ble/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3130 2023-07-10 14:37:39.000000 mgtron-2.20.0/src/ble/ble_data.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     8527 2023-07-13 17:42:32.000000 mgtron-2.20.0/src/ble/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      859 2023-06-30 12:43:53.000000 mgtron-2.20.0/src/ble/scanning.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.717755 mgtron-2.20.0/src/db/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/channel_1.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/channel_2.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/channel_3.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/channel_4.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/channel_5.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/channel_6.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/channel_7.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/channel_8.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10863 2023-07-13 17:42:32.000000 mgtron-2.20.0/src/db/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2516 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/init_db.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10906 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/long_save.json
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/long_save.json.lock
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    49152 2023-07-13 17:23:31.000000 mgtron-2.20.0/src/db/mgtron_db.db
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9064 2023-07-13 17:42:32.000000 mgtron-2.20.0/src/db/models.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1170 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/quick_save.json
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.717755 mgtron-2.20.0/src/globals/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/globals/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3642 2023-07-10 14:37:39.000000 mgtron-2.20.0/src/globals/helpers.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.717755 mgtron-2.20.0/src/gui/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       80 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/__init__.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.717755 mgtron-2.20.0/src/gui/_configs/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/card_1.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/card_2.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/card_3.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/card_4.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/card_5.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/card_6.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      263 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/card_7.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/card_8.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       98 2023-06-21 12:37:32.000000 mgtron-2.20.0/src/gui/_configs/card_config.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      317 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/mission_alpha.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      292 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/mission_bravo.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      324 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/mission_charlie.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      312 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/mission_delta.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      273 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/mission_echo.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      313 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/mission_fox.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      279 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/mission_golf.ini
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.721088 mgtron-2.20.0/src/gui/fonts/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1260156 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/fonts/MesloLGS NF Bold Italic.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1251424 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/fonts/MesloLGS NF Italic.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1292408 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/fonts/MesloLGS NF Regular.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    51305 2023-07-13 17:42:32.000000 mgtron-2.20.0/src/gui/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10946 2023-07-13 17:42:32.000000 mgtron-2.20.0/src/gui/interface.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    43803 2023-07-13 17:42:32.000000 mgtron-2.20.0/src/main.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.721088 mgtron-2.20.0/src/tests/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       33 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/tests/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       70 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/tests/test_ble.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    63110 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/tests/test_configfiles.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    19802 2023-07-13 17:42:32.000000 mgtron-2.20.0/src/tests/test_helpers.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.721088 mgtron-2.20.0/src/wifi/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/wifi/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      507 2023-07-10 14:37:39.000000 mgtron-2.20.0/src/wifi/chasing.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    17393 2023-07-13 17:42:32.000000 mgtron-2.20.0/src/wifi/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9518 2023-07-13 17:42:32.000000 mgtron-2.20.0/src/wifi/scanning.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.697754 mgtron-2.20.0/venv/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.724422 mgtron-2.20.0/venv/bin/
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      665 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2html.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      787 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2html4.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1122 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2html5.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      864 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2latex.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      687 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2man.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      853 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2odt.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      659 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      672 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      708 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2s5.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      944 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      673 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2xml.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      741 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rstpep2html.py
```

### Comparing `mgtron-2.19.5/.github/ISSUE_TEMPLATE/mgtron--.md` & `mgtron-2.20.0/.github/ISSUE_TEMPLATE/mgtron--.md`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/.github/ISSUE_TEMPLATE/mgtron_issue.yml` & `mgtron-2.20.0/.github/ISSUE_TEMPLATE/mgtron_issue.yml`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/.github/workflows/black_actions.yml` & `mgtron-2.20.0/.github/workflows/black_actions.yml`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/.github/workflows/pypi_action.yml` & `mgtron-2.20.0/.github/workflows/pypi_action.yml`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/CHANGELOG.md` & `mgtron-2.20.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,21 @@
 
 ✴️ MINOR version when you add functionality in a backwards compatible manner
 
 ✳️ PATCH version when you make backwards compatible bug fixes.
 
 -------------------------------------------------------------------------------
 
+## ✴️️️ [2.20.0] - 2023 JUNE 13
+
+- feat: wifi scan results can be toggled
+- feat: allow repetitive scan of wifi signals.
+- fix: autosend/chase w/ previous cancelled selected ssid
+- chore: removed erroneous code
+
 ## ✳️ [2.19.4] - 2023 JULY 10
 
 - Add scrollbar to the wifi scan results.
 - Status indicator properly sends zero to power on the Teensy.
 
 ## ✳️ [2.19.1] - 2023 JULY 10
```

### Comparing `mgtron-2.19.5/LICENSE.rst` & `mgtron-2.20.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/PKG-INFO` & `mgtron-2.20.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgtron
-Version: 2.19.5
+Version: 2.20.0
 Summary: Package for MGTron GUI, a user interface for signal generation
 Author-email: Christerpher Hunter <chunter@cellantenna.com>
 Project-URL: Source, https://github.com/cellantenna/mg_tron
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
```

### Comparing `mgtron-2.19.5/README.md` & `mgtron-2.20.0/README.md`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/docs/MGTron Command Description.docx` & `mgtron-2.20.0/docs/MGTron Command Description.docx`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/docs/MGTron Function Descriptions.docx` & `mgtron-2.20.0/docs/MGTron Function Descriptions.docx`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/mgtron.egg-info/PKG-INFO` & `mgtron-2.20.0/mgtron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgtron
-Version: 2.19.5
+Version: 2.20.0
 Summary: Package for MGTron GUI, a user interface for signal generation
 Author-email: Christerpher Hunter <chunter@cellantenna.com>
 Project-URL: Source, https://github.com/cellantenna/mg_tron
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
```

### Comparing `mgtron-2.19.5/mgtron.egg-info/SOURCES.txt` & `mgtron-2.20.0/mgtron.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 mgtron.egg-info/entry_points.txt
 mgtron.egg-info/requires.txt
 mgtron.egg-info/top_level.txt
 src/__init__.py
 src/main.py
 src/assets/CA logo without subtext.JPG
 src/assets/CA_subheading.png
+src/assets/MGTron Command Description.pdf
 src/assets/blueio_rs
 src/assets/init_cellantenna.sh
 src/assets/log_read
 src/assets/mgtron.desktop
 src/assets/mgtron.svg
 src/assets/network-wireless.ico
 src/assets/wifi_rs
```

### Comparing `mgtron-2.19.5/mgtron.egg-info/requires.txt` & `mgtron-2.20.0/mgtron.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/pyproject.toml` & `mgtron-2.20.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/requirements.txt` & `mgtron-2.20.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/src/assets/CA logo without subtext.JPG` & `mgtron-2.20.0/src/assets/CA logo without subtext.JPG`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/src/assets/CA_subheading.png` & `mgtron-2.20.0/src/assets/CA_subheading.png`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/src/assets/blueio_rs` & `mgtron-2.20.0/src/assets/blueio_rs`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/src/assets/init_cellantenna.sh` & `mgtron-2.20.0/src/assets/init_cellantenna.sh`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/src/assets/log_read` & `mgtron-2.20.0/src/assets/log_read`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/src/assets/mgtron.svg` & `mgtron-2.20.0/src/assets/mgtron.svg`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/src/assets/network-wireless.ico` & `mgtron-2.20.0/src/assets/network-wireless.ico`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/src/assets/wifi_rs` & `mgtron-2.20.0/src/assets/wifi_rs`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/src/ble/ble_data.py` & `mgtron-2.20.0/src/ble/ble_data.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/src/ble/helpers.py` & `mgtron-2.20.0/src/ble/helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from datetime import datetime
 from typing import Callable
 
 import json
 import time
 import logging
 import requests
-
+import tabulate 
+tabulate.PRESERVE_WHITESPACE = True
 from decouple import config
 
 from colorama import Fore as F
 
 import dearpygui.dearpygui as dpg
 
 from .ble_data import ble_data_complete
@@ -116,58 +117,58 @@
                 with dpg.child_window(
                     tag="ble_labels",
                     pos=(0, 0),
                     width=880,
                     height=715,
                 ):
                     dpg.add_text(
-                        default_value=" " * 14 + "MAC" + " " * 5 + "|" +
-                        " " * 2 +
-                        "MANUFACTURER" + " " * 1 + "|" + " " +
-                        "RSSI" + " " * 2 + "|" + " " * 12 + "DATE",
+                        default_value=" " * 7 + "MAC" + " " * 7 + "|" +
+                        " " * 4 +
+                        "MANUFACTURER" + " " * 3 + "|" + " " +
+                        "RSSI" + " "  + "|" + " " * 2 + "DATE",
                         label="BLUETOOTH LIST",
                     )
                     dpg.add_text(
                         default_value='-'*89
                     )
 
                 with dpg.child_window(
                     tag="ble_list",
-                    no_scrollbar=True,
+                    no_scrollbar=False,
                     pos=(0, 60),
                     width=880,
                     height=680,
                 ):
 
                     # Get the BLE dict information and print to GUI
                     all_data: dict = ble_data_complete()
-
-                    for i, data in enumerate(all_data, start=1):
-
-                        try:
-                            # MAC | MANUFACTURER | RSSI | DATE
-                            print_to_user = f"{i}. "\
-                                f"{data[0]}"\
-                                f"{' '* (1 if i > 9 else 2)}|"\
-                                f"{' '* (1 if i > 9 else 1)}"\
-                                f"{data[1][0]}"\
-                                f"{' '* (14 - len(data[1][0]) + 1) if i > 9 else ' ' * (15 - len(data[1][0]))}|"\
-                                f"  {data[1][1]}  | "\
-                                f" {datetime.now().strftime('%H:%M:%S')}"
-                        except TypeError:
-                            print_to_user = f"{i}. "\
-                                "NO CONNECTION ESTABLISHED"
-
-                        loggei.info(data)
-
+                    converted_data = []
+                    for i in all_data:
+                        new_list = []
+                        new_list.append(i[0])
+                        new_list.append(i[1][0])
+                        new_list.append(i[1][1])
+                        new_list.append(f" {datetime.now().strftime('%H:%M:%S')}")
+
+                        converted_data.append(new_list)
+
+                    for i in converted_data:
+                        mac_diff = 18 - len(i[1])
+                        if len(i[0]) < 18:
+                            i[0] += " " * mac_diff
                         dpg.add_text(
-                            default_value=print_to_user
+                            # tag=i[1],  # Causes issue on re-scan
+                            default_value=tabulate.tabulate(
+                                [i],
+                                stralign="left",
+                                tablefmt="plain",
+                                ),
                         )
                         dpg.add_text(
-                            default_value='-' * 78
+                            default_value=" "
                         )
 
     except SystemError:
         loggei.error(msg="Bluetooth scan window not found")
         return
 
 
@@ -175,15 +176,15 @@
     """Generate the Bluetooth frequencies."""
     loggei.info(msg="SCANNING...")
 
     try:
         dpg.delete_item(item="12")
     except SystemError:
         loggei.error(msg="Bluetooth scan window not found")
-        print("quitting")
+        loggei("quitting")
         return
 
     # Find the bluetooth signals and their frequencies
     bluetooth_blocker_init: list[tuple[int, int, int]] = [
         (2402, 100, 20),
         (2426, 100, 20),
         (2480, 100, 20),
```

### Comparing `mgtron-2.19.5/src/ble/scanning.py` & `mgtron-2.20.0/src/ble/scanning.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/src/db/helpers.py` & `mgtron-2.20.0/src/db/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         loggey.info("Save Complete")
 
 
 def quick_load(sender, app_data, user_data) -> None:
     """Load the last daved data."""
     saved_data: list = []
 
-    print(f"\nsending: {sender}")
+    # print(f"\nsending: {sender}")
     # print(f"app_data: {app_data}")
     # print(f"user_data: {user_data}\n")
 
     try:
         loggey.info("Opening the quick save file: quick_save.json")
         with open(file=f"{ROOT}/db/quick_save.json") as file:
             saved_data = json.loads(file.read())
@@ -178,15 +178,15 @@
     )
 
 
 def custom_load(sender, app_data=None, user_data=None) -> None:
     """Load config /w a custom name."""
     loggey.info("%s() executed", custom_load.__name__)
 
-    print(f"\nsender: {sender}")
+    # print(f"\nsender: {sender}")
 
     loggey.debug(msg="Attempting to load custom save data")
 
     custom_load_to_sql: list[str] = []
     try:
         custom_load_to_sql = get_sql_save_names()
     except sqlite3.DatabaseError:
@@ -310,17 +310,17 @@
         sender=None,
         app_data=None,
         user_data: tuple[str, int] = (str(), int()),
 ) -> None:
     """Delete the chosen database item."""
     loggey.debug(msg=f"{delete_it.__name__}() executed")
 
-    print(f"Sender: {sender}")
-    print(f"App data: {app_data}")
-    print(f"User data: {user_data[0]}")
+    # print(f"Sender: {sender}")
+    # print(f"App data: {app_data}")
+    # print(f"User data: {user_data[0]}")
 
     # Delete the selected item from the database
     delete_sql_save_data(save_name=user_data[0], db_path=DB_PATH)
 
 
 def check_and_load_config(button_name: str) -> dict[str, list]:
     """Check database for config button as the name of the saved config."""
```

### Comparing `mgtron-2.19.5/src/db/init_db.sql` & `mgtron-2.20.0/src/db/init_db.sql`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/src/db/long_save.json` & `mgtron-2.20.0/src/db/long_save.json`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/src/db/mgtron_db.db` & `mgtron-2.20.0/src/db/mgtron_db.db`

 * *Files 10% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -85,17 +85,17 @@
     save_name_id TEXT NOT NULL,
     frequency REAL NOT NULL,
     power INTEGER NOT NULL,
     bandwidth INTEGER NOT NULL
 );
 INSERT INTO channel_8 VALUES(2,'wifi test 0',1604.9500000000000454,100,100);
 DELETE FROM sqlite_sequence;
-INSERT INTO sqlite_sequence VALUES('save_name',2);
-INSERT INTO sqlite_sequence VALUES('channel_1',2);
-INSERT INTO sqlite_sequence VALUES('channel_2',2);
-INSERT INTO sqlite_sequence VALUES('channel_3',2);
-INSERT INTO sqlite_sequence VALUES('channel_4',2);
-INSERT INTO sqlite_sequence VALUES('channel_5',2);
-INSERT INTO sqlite_sequence VALUES('channel_6',2);
-INSERT INTO sqlite_sequence VALUES('channel_7',2);
-INSERT INTO sqlite_sequence VALUES('channel_8',2);
+INSERT INTO sqlite_sequence VALUES('save_name',3);
+INSERT INTO sqlite_sequence VALUES('channel_1',3);
+INSERT INTO sqlite_sequence VALUES('channel_2',3);
+INSERT INTO sqlite_sequence VALUES('channel_3',3);
+INSERT INTO sqlite_sequence VALUES('channel_4',3);
+INSERT INTO sqlite_sequence VALUES('channel_5',3);
+INSERT INTO sqlite_sequence VALUES('channel_6',3);
+INSERT INTO sqlite_sequence VALUES('channel_7',3);
+INSERT INTO sqlite_sequence VALUES('channel_8',3);
 COMMIT;
```

### Comparing `mgtron-2.19.5/src/db/models.py` & `mgtron-2.20.0/src/db/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                     input_data[0]["date"],
                     input_data[0]["date"],
                     input_data[0]["save_name"],
                 ),
             )
         except sqlite3.IntegrityError as e:
             # modal popup a dearpygui window
-            print(e)
+            loggit.error(e)
             # return
 
         save_name_id = input_data[0]["save_name"]
 
         # Insert into the channel tables using the save_name_id as a
         # foreign key
         cursor.execute(
@@ -254,15 +254,15 @@
 
 def delete_sql_save_data(save_name: str, db_path: str | Path = db_path):
     """Delete a save name from the database."""
     loggit.debug("%s()", delete_sql_save_data.__name__)
 
     loggit.info("Deleting save name %s from the database.", save_name)
 
-    print(f"Deleting save name {save_name} from the database.")
+    # print(f"Deleting save name {save_name} from the database.")
 
     with sqlite3.connect(db_path) as conn:
         cursor = conn.cursor()
 
         cursor.execute("DELETE FROM save_name WHERE name = ?", (save_name,))
         cursor.execute(
             "DELETE FROM\
```

### Comparing `mgtron-2.19.5/src/db/quick_save.json` & `mgtron-2.20.0/src/db/quick_save.json`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/src/globals/helpers.py` & `mgtron-2.20.0/src/globals/helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/src/gui/fonts/MesloLGS NF Bold Italic.ttf` & `mgtron-2.20.0/src/gui/fonts/MesloLGS NF Bold Italic.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/src/gui/fonts/MesloLGS NF Italic.ttf` & `mgtron-2.20.0/src/gui/fonts/MesloLGS NF Italic.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/src/gui/fonts/MesloLGS NF Regular.ttf` & `mgtron-2.20.0/src/gui/fonts/MesloLGS NF Regular.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/src/gui/helpers.py` & `mgtron-2.20.0/src/gui/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -495,23 +495,23 @@
     BLE_SCAN_WIN: str = "12"
 
     loggey.info("sender: %s", sender)
     loggey.info("app_data: %s", app_data)
     loggey.info("user_data: %s", user_data)
 
     if dpg.does_alias_exist(alias=WIFI_SCAN_WIN):
-        print("Calling wifi_factory")
+        # print("Calling wifi_factory")
         user_data[0](app_data=callstack_helper)
 
     elif dpg.does_alias_exist(alias=BLE_SCAN_WIN):
-        print("ble button pressed")
+        # print("ble button pressed")
         user_data[1](callstack_helper)
 
     else:
-        print("no special case")
+        # print("no special case")
 
         for i in range(1, 9):
             validate_user_input(channel=i)
 
         # This broke when in a for loop
         callstack_helper(channel=1)
         callstack_helper(channel=2)
```

### Comparing `mgtron-2.19.5/src/gui/interface.py` & `mgtron-2.20.0/src/gui/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,23 +84,22 @@
     sleep(0.095)  # Allow time to read and execute via serial *REQUIRED*
 
     try:
         # If the teensy is corrupted the GUI freezes here
         logger.debug(msg=f"Attempting to open serial connection {NAME}()")
         with serial.Serial() as ser:
             ser.port = PORT.strip()
-            ser.timeout = 0.8  # seconds
             logger.debug(msg=f"Serial device set | {NAME}()")
 
             ser.baudrate = BAUDRATE
             logger.debug(msg=f"baudrate set | {NAME}()")
 
             ser.timeout = 0.8  # seconds
             logger.debug(msg=f"timeout set | {NAME}()")
-            # ser.flush()  # bypass connection issues
+            ser.flush()  # bypass connection issues #! REMOVE FOR PROD
             ser.open()
             logger.debug(msg=f"serial connection open | {NAME}()")
 
             # print(" ".join([arg for arg in args]).encode("utf-8"))
             ser.write(" ".join([arg for arg in args]).encode("utf-8"))
             ser.write("\n".encode("utf-8"))
```

### Comparing `mgtron-2.19.5/src/main.py` & `mgtron-2.20.0/src/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from .gui.helpers import send_all_channels
 from .gui.helpers import send_vals
 from .gui.helpers import auto_send
 from .gui.helpers import tooltips
 
 from .wifi.helpers import wifi_scan_jam
 from .wifi.helpers import wifi_factory
-# from .wifi.helpers import wifi_kill_all
 
 from .db.helpers import custom_save
 from .db.helpers import quick_load
 from .db.helpers import quick_save
 from .db.helpers import custom_load
 from .db.helpers import delete_chosen
```

### Comparing `mgtron-2.19.5/src/tests/test_configfiles.py` & `mgtron-2.20.0/src/tests/test_configfiles.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/src/tests/test_helpers.py` & `mgtron-2.20.0/src/tests/test_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from pathlib import Path
 import sqlite3
 import pytest
-from src.db.models import delete_sql_save_data, get_sql_details
-from src.db.models import get_sql_save_names
-from src.db.models import save_to_database
-from src.gui.helpers import BANDS
-from src.gui.helpers import convert_power
-from src.gui.helpers import FREQ
-from src.gui.helpers import NAME
-from src.gui.helpers import POWS
-from src.gui.helpers import kill_channel
-from src.gui.helpers import version_getter
-from src.interface import format_output
+from ..db.models import delete_sql_save_data, get_sql_details
+from ..db.models import get_sql_save_names
+from ..db.models import save_to_database
+from ..gui.helpers import BANDS
+from ..gui.helpers import convert_power
+from ..gui.helpers import FREQ
+from ..gui.helpers import NAME
+from ..gui.helpers import POWS
+from ..gui.helpers import kill_channel
+from ..gui.helpers import version_getter
+from ..interface import format_output
 
 scan_results: dict = {}  # find_signals_and_frequencies()
 
 test_db_path: str | Path = Path("test.db")
 
 
 def test_kill_channel() -> None:
```

### Comparing `mgtron-2.19.5/src/wifi/helpers.py` & `mgtron-2.20.0/src/wifi/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 
 def wifi_scan_jam(sender) -> None:
     """Scan the local wifi channels and jam them."""
     loggei.info(msg="Scan jammer method called")
 
     colwidth_delineate = 4
     wifi_button_width = 669
-    #  Determine if the scan is in progress
 
     disble_select_btns(*WIFI_BTNS_LIST, _dpg=dpg)
     #  Determine if the scan is in progress; toggle button
 
     if dpg.get_item_theme(item=sender) == orng_btn_theme:
         dpg.bind_item_theme(
             item="mssn_scan_jam",
@@ -96,19 +95,52 @@
     else:
         # Turn the button Orange
         dpg.bind_item_theme(
             item=sender,
             theme=orng_btn_theme,
         )
 
+        delete_scan_aliases()
+
         scan_window(colwidth_delineate, wifi_button_width)
 
         loggei.debug(msg="WiFi scan jammer method finished")
 
 
+def delete_scan_aliases(alias_file="wifi_scan_aliases.yml") -> None:
+    """Delete the wifi scan aliases."""
+    loggei.info("%s()", delete_scan_aliases.__name__)
+
+    try:
+        # Read the contents of the YAML file
+        with open(alias_file, "r") as read_file:
+            alias_data = yaml.load(
+                stream=read_file,
+                Loader=yaml.FullLoader
+            )
+
+            [dpg.delete_item(item=i) for i in alias_data]
+            loggei.debug(msg="WiFi scan aliases deleted")
+
+    except (yaml.parser.ParserError, FileNotFoundError):
+        loggei.error(
+            "%s() failed to read alias file",
+            wifi_scan_jam.__name__
+        )
+
+    try:
+        os.remove(alias_file)  # Delete the file
+        loggei.debug(msg="WiFi scan alias file deleted")
+    except FileNotFoundError:
+        loggei.error(
+            "%s() failed to delete alias file",
+            wifi_scan_jam.__name__
+        )
+
+
 def scan_window(colwidth_delineate, wifi_button_width) -> None:
     """Create a window to display the scan results."""
     loggei.info("%s()", scan_window.__name__)
 
     with dpg.window(
         tag=129,
         no_scrollbar=False,
@@ -196,21 +228,19 @@
         if len(i[2]) < 4:
             i[2] += " " * channel_diff
         if len(i[4]) < 3:
             i[4] += " " * signal_diff
         if len(i[5]) == 0:
             i[5] = "Open"
 
-        # print(f"{[i]}")
-
         temp_list = []
         temp_list.append(i)
 
         dpg.add_button(
-            # tag=i[1],  # Causes issue on re-scan
+            tag=i[1],  # Causes issue on re-scan unless deleted
             parent=129,
             label=tabulate.tabulate(
                 [i],
                 stralign="left",
                 tablefmt="plain",
                 maxcolwidths=[
                     None,
@@ -219,24 +249,29 @@
                     None,
                     None,
                     4,
                 ]),
             width=880,
             height=60,
             callback=indicate_tagged_results,
-            user_data=(i, 3),
+            user_data=(i, i[1]),
         )
 
+        with open("wifi_scan_aliases.yml", "a") as outfile:
+            yaml.dump(
+                data={i[1]: i[0]},
+                stream=outfile,
+            )
+
 
 def indicate_tagged_results(sender, app_data, user_data: list[str]) -> None:
     """Change the color of the sender."""
     loggei.debug("%s()", indicate_tagged_results.__name__)
 
     loggei.info("User data: %s", user_data)
-    print(f"{F.YELLOW}User data{R}: {user_data}")
 
     # Make a toggle of the selected buttons
     if dpg.get_item_theme(item=sender) == blue_btn_theme:
         # Turn the button green
         dpg.bind_item_theme(
             item=sender,
             theme=None,
@@ -245,28 +280,34 @@
         # Turn the button blue
         dpg.bind_item_theme(
             item=sender,
             theme=blue_btn_theme,
         )
 
     # Turn user_data into a dict with user_data[0] as the key
-    user_data = {
+    user_datas = {
         user_data[0][0]: {
             "MAC": user_data[0][1],
             "CH": user_data[0][2],
             "FREQ": user_data[0][3].split(" ")[0],
             "SIGNAL": user_data[0][4],
             "SECURITY": user_data[0][5],
         }
     }
 
+    # all_tags: list = [i for i in user_data[1][1]]
+
+    # [print(f"{F.YELLOW}All tags:{R}: {i}") for i in all_tags]
+
+    # print(f"{F.YELLOW}Converted data:{R}: {user_data[1]}")
+
     # Write the data to a yml file
     with open("wifi_scan_results.yml", "a") as outfile:
         yaml.dump(
-            data=user_data,
+            data=user_datas,
             stream=outfile,
         )
 
     loggei.debug("%s() exiting", indicate_tagged_results.__name__)
 
 
 def return_indicated_results() -> dict[str, dict[str, str]]:
@@ -277,25 +318,37 @@
     selected_scan_results = yaml.load(
         stream=open("wifi_scan_results.yml", "r"),
         Loader=yaml.FullLoader,
     )
 
     os.remove("wifi_scan_results.yml")
 
-    return selected_scan_results
+    alias_dict: dict[str, dict[str, str]] = dict()
+
+    # Get all of the alias themes
+    for iterite, color in enumerate(selected_scan_results.items(), start=1):
+        if dpg.get_item_theme(color[1]["MAC"]):
+            alias_dict.update({color[0]: color[1]})
+
+    # print(f"\n{F.YELLOW}Aliases: {R}{alias_dict}")
+    # print(f"{F.YELLOW}Selected scan results: {R}{selected_scan_results}")
+
+    return alias_dict
 
 
 def activate_wifi_chase() -> None:
     """Send all the requisite information to the MGTron board."""
     loggei.debug("%s()", activate_wifi_chase.__name__)
 
-    user_data = return_indicated_results()
+    user_data: dict[str, dict[str, str]] = return_indicated_results()
 
     ssid: list[str] = list(user_data.keys())
 
+    # print(f"{F.YELLOW}SSID to search: {R}{ssid}")
+
     try:
         dpg.delete_item(item=129)
         dpg.delete_item(item="128")
     except SystemError as e:
         loggei.error("System error: %s", e)
 
     channel_list: list[int] = discern_avail_channels(dpg)
@@ -307,36 +360,38 @@
         channel_list: list[int] = [1, 2, 3, 4, 5, 6, 7, 8]
 
     count: int = 4  # len(user_data.keys())
 
     tracker = 0
     while tracker != count:
 
-        # if tracker >= 1:
-
-        try:
-            dpg.delete_item(item=129)
-            dpg.delete_item(item="128")
-        except SystemError as e:
-            loggei.error("System error: %s", e)
-
-        print(f"{F.CYAN}New scan: {tracker}{R}")
-        # Get the chase frequencies
-        chase_freqs: list[float] = threaded_scan(
-            _dpg=dpg,
-            linux_data=post_ssid,
-            ssid=ssid
-        )
-        # else:
+        if tracker >= 1:
 
-        # chase_freqs: list[float] = [
-        # float(i.get("FREQ")) for i in user_data.values()
-        # ]
+            try:
+                dpg.delete_item(item=129)
+                dpg.delete_item(item="128")
+            except SystemError as e:
+                loggei.error("System error: %s", e)
+
+                # print(f"{F.CYAN}New scan: {tracker + 1}{R}")
+                # Get the chase frequencies
+                chase_freqs: list[float] = threaded_scan(
+                    _dpg=dpg,
+                    linux_data=post_ssid,
+                    ssid=ssid
+                )
+
+                # print("\nChase freqs:", set(chase_freqs))
+        else:
+
+            chase_freqs: list[float] = [
+                float(i.get("FREQ")) for i in user_data.values()
+            ]
 
-        print("\nChase freqs:", set(chase_freqs))
+            # print("\nChase freqs:", set(chase_freqs))
 
         disable_scanning_mode(enable_btns=False)
 
         # Take advantage of the dedup characteristics of a set
         chase_freqs: set[float] = set(chase_freqs)
 
         # Chase three times
@@ -520,20 +575,18 @@
     """Take in the request and discern the appropriate wifi action."""
     loggei.debug("%s()", wifi_factory.__name__)
 
     WIFI_BTN_SELECT_YAML = pathlib.Path("wifi_scan_results.yml")
 
     # Check if the wifi button select yaml file exists
     if not pathlib.Path.exists(WIFI_BTN_SELECT_YAML):
-        print("No wifi button select yaml file found")
         loggei.info("calling wifi_kill_all()")
         wifi_kill_all(app_data)
 
     else:
-        print("Wifi button select yaml file found")
         loggei.info("calling wifi_chase()")
         activate_wifi_chase()
 
 
 def main():
     """Run the main program."""
     loggei.info(msg="Main method called")
```

### Comparing `mgtron-2.19.5/src/wifi/scanning.py` & `mgtron-2.20.0/src/wifi/scanning.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,21 +313,21 @@
 
 def dedup_freqs(freq_and_strength: dict[int, float]) -> dict[int, float]:
     """Deduplicate the frequencies of wifi scan results."""
     loggey.debug("%s()", dedup_freqs.__name__)
 
     freqs_returned: dict[int, float] = dict()
 
-    print(f"{F.CYAN}Freq & Strength prior to dedup: {freq_and_strength}{R}")
+    loggey.info(f"{F.CYAN}init Freq & Strength: {freq_and_strength}{R}")
 
     for strength, freq in freq_and_strength.items():
         if freq not in freqs_returned.values():
             freqs_returned.update({strength: freq})
 
-    print(f"{F.CYAN}Freq & Strength deduped: {freqs_returned}{R}")
+    loggey.info(f"{F.CYAN}Freq & Strength deduped: {freqs_returned}{R}")
 
     return freqs_returned
 
 
 def main():
     """Run the module as a script."""
     # data = find_signals_and_frequencies()
```

### Comparing `mgtron-2.19.5/venv/bin/rst2html.py` & `mgtron-2.20.0/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/venv/bin/rst2html4.py` & `mgtron-2.20.0/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/venv/bin/rst2html5.py` & `mgtron-2.20.0/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/venv/bin/rst2latex.py` & `mgtron-2.20.0/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/venv/bin/rst2man.py` & `mgtron-2.20.0/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/venv/bin/rst2odt.py` & `mgtron-2.20.0/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/venv/bin/rst2odt_prepstyles.py` & `mgtron-2.20.0/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/venv/bin/rst2pseudoxml.py` & `mgtron-2.20.0/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/venv/bin/rst2s5.py` & `mgtron-2.20.0/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/venv/bin/rst2xetex.py` & `mgtron-2.20.0/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/venv/bin/rst2xml.py` & `mgtron-2.20.0/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.5/venv/bin/rstpep2html.py` & `mgtron-2.20.0/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

