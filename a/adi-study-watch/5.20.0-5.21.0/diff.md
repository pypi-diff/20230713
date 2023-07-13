# Comparing `tmp/adi_study_watch-5.20.0.tar.gz` & `tmp/adi_study_watch-5.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adi_study_watch-5.20.0.tar", last modified: Tue Jun  6 11:07:08 2023, max compression
+gzip compressed data, was "adi_study_watch-5.21.0.tar", last modified: Thu Jul 13 10:08:59 2023, max compression
```

## Comparing `adi_study_watch-5.20.0.tar` & `adi_study_watch-5.21.0.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:08.720837 adi_study_watch-5.20.0/
--rw-rw-rw-   0        0        0    11357 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/LICENSE
--rw-rw-rw-   0        0        0       26 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4906 2023-06-06 11:07:08.720316 adi_study_watch-5.20.0/PKG-INFO
--rw-rw-rw-   0        0        0     3946 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.276860 adi_study_watch-5.20.0/adi_study_watch/
--rw-rw-rw-   0        0        0     2455 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.698931 adi_study_watch-5.20.0/adi_study_watch/application/
--rw-rw-rw-   0        0        0     2433 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/__init__.py
--rw-rw-rw-   0        0        0    12909 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/ad7156_application.py
--rw-rw-rw-   0        0        0    21849 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/adp5360_application.py
--rw-rw-rw-   0        0        0    61330 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/adpd_application.py
--rw-rw-rw-   0        0        0    16906 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/adxl_application.py
--rw-rw-rw-   0        0        0    31604 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/bia_application.py
--rw-rw-rw-   0        0        0     8706 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/common_application.py
--rw-rw-rw-   0        0        0    16102 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/common_stream.py
--rw-rw-rw-   0        0        0    11866 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/csv_logging.py
--rw-rw-rw-   0        0        0    16612 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/ecg_application.py
--rw-rw-rw-   0        0        0    40888 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/eda_application.py
--rw-rw-rw-   0        0        0    45469 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/fs_application.py
--rw-rw-rw-   0        0        0    17171 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/low_touch_application.py
--rw-rw-rw-   0        0        0     7365 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/pedometer_application.py
--rw-rw-rw-   0        0        0    31426 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/pm_application.py
--rw-rw-rw-   0        0        0    21584 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/ppg_application.py
--rw-rw-rw-   0        0        0     9199 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/sqi_application.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.700930 adi_study_watch-5.20.0/adi_study_watch/application/study_watch/
--rw-rw-rw-   0        0        0        0 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/study_watch/__init__.py
--rw-rw-rw-   0        0        0    23553 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/temperature_application.py
--rw-rw-rw-   0        0        0    53996 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/test_application.py
--rw-rw-rw-   0        0        0    21411 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/user0_application.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.716483 adi_study_watch-5.20.0/adi_study_watch/application/vsm_mb_sb/
--rw-rw-rw-   0        0        0        0 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/vsm_mb_sb/__init__.py
--rw-rw-rw-   0        0        0     4261 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/application/vsm_mb_sb/pm_application.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.775754 adi_study_watch-5.20.0/adi_study_watch/core/
--rw-rw-rw-   0        0        0     2433 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/__init__.py
--rw-rw-rw-   0        0        0     4699 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/ble_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.962659 adi_study_watch-5.20.0/adi_study_watch/core/data_types/
--rw-rw-rw-   0        0        0        0 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/data_types/__init__.py
--rw-rw-rw-   0        0        0     2299 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/data_types/array.py
--rw-rw-rw-   0        0        0      868 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/data_types/binary.py
--rw-rw-rw-   0        0        0      318 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/data_types/data_type.py
--rw-rw-rw-   0        0        0     1334 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/data_types/decimal.py
--rw-rw-rw-   0        0        0     1888 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/data_types/enums.py
--rw-rw-rw-   0        0        0     2351 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/data_types/integer.py
--rw-rw-rw-   0        0        0     1044 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/data_types/string.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:08.222107 adi_study_watch-5.20.0/adi_study_watch/core/enums/
--rw-rw-rw-   0        0        0     2433 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/__init__.py
--rw-rw-rw-   0        0        0     2761 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/ad7156_enums.py
--rw-rw-rw-   0        0        0     3547 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/adp5360_enums.py
--rw-rw-rw-   0        0        0     5833 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/adpd_enums.py
--rw-rw-rw-   0        0        0     3048 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/adxl_enums.py
--rw-rw-rw-   0        0        0     4727 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/bia_enums.py
--rw-rw-rw-   0        0        0     2735 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/board_enums.py
--rw-rw-rw-   0        0        0    11046 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/common_enums.py
--rw-rw-rw-   0        0        0     3982 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/dcb_enums.py
--rw-rw-rw-   0        0        0     3192 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/display_enums.py
--rw-rw-rw-   0        0        0     2763 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/ecg_enums.py
--rw-rw-rw-   0        0        0     5307 2023-06-06 11:05:57.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/eda_enums.py
--rw-rw-rw-   0        0        0     7281 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/fs_enums.py
--rw-rw-rw-   0        0        0     3417 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/low_touch_enum.py
--rw-rw-rw-   0        0        0     2775 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/pedometer_enums.py
--rw-rw-rw-   0        0        0     8417 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/pm_enums.py
--rw-rw-rw-   0        0        0     3176 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/ppg_enums.py
--rw-rw-rw-   0        0        0     3113 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/sqi_enum.py
--rw-rw-rw-   0        0        0     4186 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/enums/user0_enums.py
--rw-rw-rw-   0        0        0    12382 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packet_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:08.450430 adi_study_watch-5.20.0/adi_study_watch/core/packets/
--rw-rw-rw-   0        0        0     2433 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/__init__.py
--rw-rw-rw-   0        0        0     4688 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/ad7156_packets.py
--rw-rw-rw-   0        0        0     9561 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/adp5360_packets.py
--rw-rw-rw-   0        0        0    25594 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/adpd_packets.py
--rw-rw-rw-   0        0        0     9655 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/adxl_packets.py
--rw-rw-rw-   0        0        0    10847 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/bia_packets.py
--rw-rw-rw-   0        0        0     7423 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/command_packet.py
--rw-rw-rw-   0        0        0     6745 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/common_packets.py
--rw-rw-rw-   0        0        0     4082 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/display_packets.py
--rw-rw-rw-   0        0        0     5828 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/ecg_packets.py
--rw-rw-rw-   0        0        0    17881 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/eda_packets.py
--rw-rw-rw-   0        0        0    23528 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/fs_packets.py
--rw-rw-rw-   0        0        0     9273 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/low_touch_packets.py
--rw-rw-rw-   0        0        0    16534 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/pm_packets.py
--rw-rw-rw-   0        0        0     7905 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/ppg_packets.py
--rw-rw-rw-   0        0        0     3301 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/sqi_packets.py
--rw-rw-rw-   0        0        0    40236 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/stream_data_packets.py
--rw-rw-rw-   0        0        0     6036 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/temperature_packets.py
--rw-rw-rw-   0        0        0    13524 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/packets/user0_packets.py
--rw-rw-rw-   0        0        0     8121 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/core/utils.py
--rw-rw-rw-   0        0        0    39364 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/adi_study_watch/sdk.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:07.366666 adi_study_watch-5.20.0/adi_study_watch.egg-info/
--rw-rw-rw-   0        0        0     4906 2023-06-06 11:07:07.000000 adi_study_watch-5.20.0/adi_study_watch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3976 2023-06-06 11:07:07.000000 adi_study_watch-5.20.0/adi_study_watch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 11:07:07.000000 adi_study_watch-5.20.0/adi_study_watch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 11:07:07.000000 adi_study_watch-5.20.0/adi_study_watch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 11:07:07.000000 adi_study_watch-5.20.0/adi_study_watch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 11:07:08.721360 adi_study_watch-5.20.0/setup.cfg
--rw-rw-rw-   0        0        0     1457 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:07:08.718226 adi_study_watch-5.20.0/tests/
--rw-rw-rw-   0        0        0     3677 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_ad7156_application.py
--rw-rw-rw-   0        0        0     8168 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_adpd_application.py
--rw-rw-rw-   0        0        0     4754 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_adxl_application.py
--rw-rw-rw-   0        0        0     5975 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_application.py
--rw-rw-rw-   0        0        0     3852 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_bcm_application.py
--rw-rw-rw-   0        0        0     4420 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_ecg_application.py
--rw-rw-rw-   0        0        0     5557 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_eda_application.py
--rw-rw-rw-   0        0        0     4665 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_fs_application.py
--rw-rw-rw-   0        0        0     3154 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_pedometer_application.py
--rw-rw-rw-   0        0        0     4870 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_pm_application.py
--rw-rw-rw-   0        0        0     4056 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_ppg_application.py
--rw-rw-rw-   0        0        0     3599 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_sqi_application.py
--rw-rw-rw-   0        0        0     3365 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_temperature_application.py
--rw-rw-rw-   0        0        0     3770 2023-06-06 11:05:58.000000 adi_study_watch-5.20.0/tests/test_user0_application.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:08:59.546061 adi_study_watch-5.21.0/
+-rw-rw-rw-   0        0        0    11357 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/LICENSE
+-rw-rw-rw-   0        0        0       26 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4906 2023-07-13 10:08:59.546061 adi_study_watch-5.21.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3946 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 10:08:58.808069 adi_study_watch-5.21.0/adi_study_watch/
+-rw-rw-rw-   0        0        0     2455 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:08:59.015843 adi_study_watch-5.21.0/adi_study_watch/application/
+-rw-rw-rw-   0        0        0     2433 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/__init__.py
+-rw-rw-rw-   0        0        0    12909 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/ad7156_application.py
+-rw-rw-rw-   0        0        0    21849 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/adp5360_application.py
+-rw-rw-rw-   0        0        0    61330 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/adpd_application.py
+-rw-rw-rw-   0        0        0    16906 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/adxl_application.py
+-rw-rw-rw-   0        0        0    31604 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/bia_application.py
+-rw-rw-rw-   0        0        0     8706 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/common_application.py
+-rw-rw-rw-   0        0        0    16102 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/common_stream.py
+-rw-rw-rw-   0        0        0    11866 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/csv_logging.py
+-rw-rw-rw-   0        0        0    16612 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/ecg_application.py
+-rw-rw-rw-   0        0        0    39870 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/eda_application.py
+-rw-rw-rw-   0        0        0    45469 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/fs_application.py
+-rw-rw-rw-   0        0        0    17171 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/low_touch_application.py
+-rw-rw-rw-   0        0        0     7365 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/pedometer_application.py
+-rw-rw-rw-   0        0        0    31496 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/pm_application.py
+-rw-rw-rw-   0        0        0    21584 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/ppg_application.py
+-rw-rw-rw-   0        0        0     9199 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/sqi_application.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:08:59.017813 adi_study_watch-5.21.0/adi_study_watch/application/study_watch/
+-rw-rw-rw-   0        0        0        0 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/study_watch/__init__.py
+-rw-rw-rw-   0        0        0    23553 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/temperature_application.py
+-rw-rw-rw-   0        0        0    58657 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/test_application.py
+-rw-rw-rw-   0        0        0    21411 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/user0_application.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:08:59.027467 adi_study_watch-5.21.0/adi_study_watch/application/vsm_mb_sb/
+-rw-rw-rw-   0        0        0        0 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/vsm_mb_sb/__init__.py
+-rw-rw-rw-   0        0        0     4261 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/application/vsm_mb_sb/pm_application.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:08:59.055038 adi_study_watch-5.21.0/adi_study_watch/core/
+-rw-rw-rw-   0        0        0     2433 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/__init__.py
+-rw-rw-rw-   0        0        0     4699 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/ble_manager.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:08:59.113196 adi_study_watch-5.21.0/adi_study_watch/core/data_types/
+-rw-rw-rw-   0        0        0        0 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/data_types/__init__.py
+-rw-rw-rw-   0        0        0     2299 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/data_types/array.py
+-rw-rw-rw-   0        0        0      868 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/data_types/binary.py
+-rw-rw-rw-   0        0        0      318 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/data_types/data_type.py
+-rw-rw-rw-   0        0        0     1334 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/data_types/decimal.py
+-rw-rw-rw-   0        0        0     1888 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/data_types/enums.py
+-rw-rw-rw-   0        0        0     2351 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/data_types/integer.py
+-rw-rw-rw-   0        0        0     1044 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/data_types/string.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:08:59.263996 adi_study_watch-5.21.0/adi_study_watch/core/enums/
+-rw-rw-rw-   0        0        0     2433 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/enums/__init__.py
+-rw-rw-rw-   0        0        0     2761 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/enums/ad7156_enums.py
+-rw-rw-rw-   0        0        0     3547 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/enums/adp5360_enums.py
+-rw-rw-rw-   0        0        0     5833 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/enums/adpd_enums.py
+-rw-rw-rw-   0        0        0     3048 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/enums/adxl_enums.py
+-rw-rw-rw-   0        0        0     4727 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/enums/bia_enums.py
+-rw-rw-rw-   0        0        0     2735 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/enums/board_enums.py
+-rw-rw-rw-   0        0        0    11046 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/enums/common_enums.py
+-rw-rw-rw-   0        0        0     3982 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/enums/dcb_enums.py
+-rw-rw-rw-   0        0        0     3192 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/enums/display_enums.py
+-rw-rw-rw-   0        0        0     2763 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/enums/ecg_enums.py
+-rw-rw-rw-   0        0        0     5381 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/enums/eda_enums.py
+-rw-rw-rw-   0        0        0     7281 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/enums/fs_enums.py
+-rw-rw-rw-   0        0        0     3417 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/enums/low_touch_enum.py
+-rw-rw-rw-   0        0        0     2775 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/enums/pedometer_enums.py
+-rw-rw-rw-   0        0        0     8762 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/enums/pm_enums.py
+-rw-rw-rw-   0        0        0     3176 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/enums/ppg_enums.py
+-rw-rw-rw-   0        0        0     3113 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/enums/sqi_enum.py
+-rw-rw-rw-   0        0        0     4186 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/enums/user0_enums.py
+-rw-rw-rw-   0        0        0    12382 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/packet_manager.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:08:59.427688 adi_study_watch-5.21.0/adi_study_watch/core/packets/
+-rw-rw-rw-   0        0        0     2433 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/packets/__init__.py
+-rw-rw-rw-   0        0        0     4688 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/packets/ad7156_packets.py
+-rw-rw-rw-   0        0        0     9561 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/packets/adp5360_packets.py
+-rw-rw-rw-   0        0        0    25594 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/packets/adpd_packets.py
+-rw-rw-rw-   0        0        0     9655 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/packets/adxl_packets.py
+-rw-rw-rw-   0        0        0    10847 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/packets/bia_packets.py
+-rw-rw-rw-   0        0        0     7423 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/packets/command_packet.py
+-rw-rw-rw-   0        0        0     6745 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/packets/common_packets.py
+-rw-rw-rw-   0        0        0     4082 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/packets/display_packets.py
+-rw-rw-rw-   0        0        0     5828 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/packets/ecg_packets.py
+-rw-rw-rw-   0        0        0    17881 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/packets/eda_packets.py
+-rw-rw-rw-   0        0        0    23528 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/packets/fs_packets.py
+-rw-rw-rw-   0        0        0     9273 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/packets/low_touch_packets.py
+-rw-rw-rw-   0        0        0    17129 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/packets/pm_packets.py
+-rw-rw-rw-   0        0        0     7905 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/packets/ppg_packets.py
+-rw-rw-rw-   0        0        0     3301 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/packets/sqi_packets.py
+-rw-rw-rw-   0        0        0    40236 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/packets/stream_data_packets.py
+-rw-rw-rw-   0        0        0     6036 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/packets/temperature_packets.py
+-rw-rw-rw-   0        0        0    13524 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/packets/user0_packets.py
+-rw-rw-rw-   0        0        0     8121 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/adi_study_watch/core/utils.py
+-rw-rw-rw-   0        0        0    39364 2023-07-13 09:37:47.000000 adi_study_watch-5.21.0/adi_study_watch/sdk.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:08:58.826628 adi_study_watch-5.21.0/adi_study_watch.egg-info/
+-rw-rw-rw-   0        0        0     4906 2023-07-13 10:08:58.000000 adi_study_watch-5.21.0/adi_study_watch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3976 2023-07-13 10:08:58.000000 adi_study_watch-5.21.0/adi_study_watch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 10:08:58.000000 adi_study_watch-5.21.0/adi_study_watch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 10:08:58.000000 adi_study_watch-5.21.0/adi_study_watch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-13 10:08:58.000000 adi_study_watch-5.21.0/adi_study_watch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 10:08:59.547062 adi_study_watch-5.21.0/setup.cfg
+-rw-rw-rw-   0        0        0     1456 2023-07-13 09:37:47.000000 adi_study_watch-5.21.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:08:59.544093 adi_study_watch-5.21.0/tests/
+-rw-rw-rw-   0        0        0     3677 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/tests/test_ad7156_application.py
+-rw-rw-rw-   0        0        0     8168 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/tests/test_adpd_application.py
+-rw-rw-rw-   0        0        0     4754 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/tests/test_adxl_application.py
+-rw-rw-rw-   0        0        0     5975 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/tests/test_application.py
+-rw-rw-rw-   0        0        0     3852 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/tests/test_bcm_application.py
+-rw-rw-rw-   0        0        0     4420 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/tests/test_ecg_application.py
+-rw-rw-rw-   0        0        0     5557 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/tests/test_eda_application.py
+-rw-rw-rw-   0        0        0     4665 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/tests/test_fs_application.py
+-rw-rw-rw-   0        0        0     3154 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/tests/test_pedometer_application.py
+-rw-rw-rw-   0        0        0     4870 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/tests/test_pm_application.py
+-rw-rw-rw-   0        0        0     4056 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/tests/test_ppg_application.py
+-rw-rw-rw-   0        0        0     3599 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/tests/test_sqi_application.py
+-rw-rw-rw-   0        0        0     3365 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/tests/test_temperature_application.py
+-rw-rw-rw-   0        0        0     3770 2023-07-13 09:37:07.000000 adi_study_watch-5.21.0/tests/test_user0_application.py
```

### Comparing `adi_study_watch-5.20.0/LICENSE` & `adi_study_watch-5.21.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/PKG-INFO` & `adi_study_watch-5.21.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adi_study_watch
-Version: 5.20.0
+Version: 5.21.0
 Summary: ADI study watch python SDK
 Home-page: https://github.com/analogdevicesinc/study-watch-sdk
 Author: Analog Devices, Inc.
 Author-email: healthcare-support@analog.com
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `adi_study_watch-5.20.0/README.md` & `adi_study_watch-5.21.0/README.md`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/__init__.py` & `adi_study_watch-5.21.0/adi_study_watch/__init__.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/__init__.py` & `adi_study_watch-5.21.0/adi_study_watch/application/__init__.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/ad7156_application.py` & `adi_study_watch-5.21.0/adi_study_watch/application/ad7156_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/adp5360_application.py` & `adi_study_watch-5.21.0/adi_study_watch/application/adp5360_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/adpd_application.py` & `adi_study_watch-5.21.0/adi_study_watch/application/adpd_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/adxl_application.py` & `adi_study_watch-5.21.0/adi_study_watch/application/adxl_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/bia_application.py` & `adi_study_watch-5.21.0/adi_study_watch/application/bia_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/common_application.py` & `adi_study_watch-5.21.0/adi_study_watch/application/common_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/common_stream.py` & `adi_study_watch-5.21.0/adi_study_watch/application/common_stream.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/csv_logging.py` & `adi_study_watch-5.21.0/adi_study_watch/application/csv_logging.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/ecg_application.py` & `adi_study_watch-5.21.0/adi_study_watch/application/ecg_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/eda_application.py` & `adi_study_watch-5.21.0/adi_study_watch/application/eda_application.py`

 * *Files 1% similar despite different names*

```diff
@@ -987,30 +987,7 @@
             sdk = SDK("COM4")
             application = sdk.get_eda_application()
             x = application.load_device_configuration()
         """
         request_packet = CommandPacket(self._destination, EDACommand.LOAD_DCFG_REQ)
         response_packet = CommandPacket(self._destination, EDACommand.LOAD_DCFG_RES)
         return self._send_packet(request_packet, response_packet)
-
-    def set_power_mode(self, power_mode: EDAPowerMode) -> Dict:
-        """
-        Control the AD5940 ICs power state: to make it enter Hibernate or wakeup state.
-        EPHY_LDO turn On needs to be done prior to this.
-
-        :param power_mode: power mode, use get_supported_power_modes() to get all supported power modes.
-        :return: A response packet as dictionary.
-        :rtype: Dict
-
-        .. code-block:: python3
-            :emphasize-lines: 5
-
-            from adi_study_watch import SDK
-
-            sdk = SDK("COM4")
-            application = sdk.get_eda_application()
-            x = application.set_power_mode(application.POWER_SLEEP)
-        """
-        request_packet = EDASleepWakeupPacket(self._destination, EDACommand.CONTROL_AD5940_SLEEP_WAKEUP_REQ)
-        request_packet.set_payload("power_mode", power_mode)
-        response_packet = EDASleepWakeupPacket(self._destination, EDACommand.CONTROL_AD5940_SLEEP_WAKEUP_RES)
-        return self._send_packet(request_packet, response_packet)
```

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/fs_application.py` & `adi_study_watch-5.21.0/adi_study_watch/application/fs_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/low_touch_application.py` & `adi_study_watch-5.21.0/adi_study_watch/application/low_touch_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/pedometer_application.py` & `adi_study_watch-5.21.0/adi_study_watch/application/pedometer_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/pm_application.py` & `adi_study_watch-5.21.0/adi_study_watch/application/pm_application.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 # ******************************************************************************
 
 import time
 import logging
 from datetime import datetime
 from typing import Dict, List
 
+from ..core.enums.pm_enums import LDO, ElectrodeSwitch, ControlStatus
 from ..core.enums.dcb_enums import DCBCommand
 from .common_application import CommonApplication
 from ..core.enums.pm_enums import PMCommand, ChipID
 from ..core.packets.command_packet import CommandPacket
 from ..core.packets.common_packets import VersionPacket
 from ..core.enums.common_enums import Application, CommonCommand
 from ..core.packets.pm_packets import MCUVersionPacket, SystemInfoPacket, DateTimePacket, SyncTimerPacket, \
```

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/ppg_application.py` & `adi_study_watch-5.21.0/adi_study_watch/application/ppg_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/sqi_application.py` & `adi_study_watch-5.21.0/adi_study_watch/application/sqi_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/temperature_application.py` & `adi_study_watch-5.21.0/adi_study_watch/application/temperature_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/test_application.py` & `adi_study_watch-5.21.0/adi_study_watch/application/test_application.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,32 +39,35 @@
 import time
 import logging
 from typing import List, Dict, Callable, Optional
 
 from tqdm import tqdm
 
 from .fs_application import FSApplication
+from ..core.enums.eda_enums import EDAPowerMode, EDACommand
 from ..core.enums.ppg_enums import PPGCommand
 from ..core.enums.bia_enums import BIACommand
 from ..core.enums.adxl_enums import ADXLCommand
 from .common_application import CommonApplication
 from ..core.enums.fs_enums import FSCommand, FSStatus
 from ..core.packets.common_packets import StreamPacket
+from ..core.packets.eda_packets import EDASleepWakeupPacket
 from ..core.packets.ppg_packets import PPGStatesPacket
 from ..core.packets.command_packet import CommandPacket
 from ..core.enums.adpd_enums import ADPDCommand, ADPDLed
 from ..core.enums.display_enums import DisplayColor, DisplayCommand
 from ..core.packets.adpd_packets import AgcInfoPacket, TestCommandPacket
 from ..core.packets.bia_packets import FDSStatusPacket, DCBTimingInfoPacket
 from ..core.enums.pm_enums import PMCommand, PowerMode, LDO, ElectrodeSwitch
 from ..core.packets.display_packets import SetDisplayPacket, EnableDisplayPacket
 from ..core.packets.fs_packets import StreamDebugInfoPacket, FileInfoResponsePacket, \
     SystemAppFSUSBStreamInfoResponsePacket, SystemAppDebugInfoResponsePacket
 from ..core.enums.common_enums import Application, CommonCommand, Stream, CommonStatus
-from ..core.packets.pm_packets import LDOControlPacket, SwitchControlPacket, PingPacket
+from ..core.packets.pm_packets import LDOControlPacket, SwitchControlPacket, PingPacket, DG2502SWStatusPacket, \
+    LDOStatusPacket
 from ..core.packets.stream_data_packets import KeyStreamDataPacket, CapSenseStreamDataPacket
 from ..core.packets.pm_packets import AppsHealthPacket, ControlPacket, PowerStatePacket
 from ..core.packets.fs_packets import PatternWritePacket, DebugInfoPacket, BadBlockPacket, PageInfoRequestPacket, \
     PageInfoResponsePacket, FileInfoRequestPacket, SystemTestInfoRequestPacket, SystemTestInfoResponsePacket
 
 logger = logging.getLogger(__name__)
 
@@ -75,14 +78,18 @@
     RED = DisplayColor.RED
     GREEN = DisplayColor.GREEN
     BLUE = DisplayColor.BLUE
 
     POWER_MODE_ACTIVE = PowerMode.ACTIVE
     POWER_MODE_HIBERNATE = PowerMode.HIBERNATE
     POWER_MODE_SHUTDOWN = PowerMode.SHUTDOWN
+    
+    POWER_INVALID = EDAPowerMode.POWER_INVALID
+    POWER_SLEEP = EDAPowerMode.POWER_SLEEP
+    POWER_WAKEUP = EDAPowerMode.POWER_WAKEUP
 
     LDO_FS = LDO.FS
     LDO_OPTICAL = LDO.OPTICAL
     LDO_EPHYZ = LDO.EPHYZ
 
     SWITCH_AD8233 = ElectrodeSwitch.AD8233
     SWITCH_AD5940 = ElectrodeSwitch.AD5940
@@ -193,15 +200,15 @@
             from adi_study_watch import SDK
 
             sdk = SDK("COM4")
             application = sdk.get_test_application()
             x = application.get_supported_power_states()
             print(x)
             # [<PowerState.ACTIVE_MODE: ['0x0']>, ... , <PowerState.SHUTDOWN_MODE: ['0x3']>]
-            x = application.set_power_mode(application.ACTIVE_MODE)
+            x = application.watch_set_power_mode(application.ACTIVE_MODE)
             print(x["payload"]["power_state"])
             # PowerState.ACTIVE_MODE
 
         """
         request_packet = PowerStatePacket(Application.PM, PMCommand.SET_POWER_STATE_REQ)
         request_packet.set_payload("power_state", power_state)
         response_packet = PowerStatePacket(Application.PM, PMCommand.SET_POWER_STATE_RES)
@@ -1375,7 +1382,120 @@
         for x in test_list:
             request_list[x - 1] = 1
         request_packet = SystemTestInfoRequestPacket(self._destination, FSCommand.DEVELOPER_TEST_REQ)
         request_packet.set_payload("skipped_test_list", request_list)
         response_packet = SystemTestInfoResponsePacket(self._destination, FSCommand.DEVELOPER_TEST_RES)
         return self._send_packet_multi_response(request_packet, response_packet, packet_limit=20, timeout=600)
 
+    def get_electrode_switch_status(self, sw_name: ElectrodeSwitch) -> Dict:
+        """
+        Get the status of switches, whether its enabled / disabled.
+
+        :param sw_name: get sw_name, use get_supported_switches() to list all support ldo.
+        :type sw_name: ElectrodeSwitch
+        :return: A response packet as dictionary.
+        :rtype: Dict
+
+        .. code-block:: python3
+            :emphasize-lines: 5
+
+            from adi_study_watch import SDK
+
+            sdk = SDK("COM4")
+            application = sdk.get_pm_application()
+            x = application.get_supported_switches()
+            x = application.get_electrode_switch_status(application.SWITCH_AD8233)
+
+        """
+        request_packet = DG2502SWStatusPacket(Application.PM, PMCommand.DG2502_SW_STATUS_REQ)
+        request_packet.set_payload("sw_name", sw_name)
+        response_packet = DG2502SWStatusPacket(Application.PM, PMCommand.DG2502_SW_STATUS_RES)
+        return self._send_packet(request_packet, response_packet)
+
+    def get_ldo_status(self, ldo: LDO):
+        """
+        Get the status of LDO, whether its enabled / disabled.
+
+        :param ldo: get ldo num, use get_supported_ldo() to list all support ldo.
+        :type ldo: LDO
+        :return: A response packet as dictionary.
+        :rtype: Dict
+
+        .. code-block:: python3
+            :emphasize-lines: 5
+
+            from adi_study_watch import SDK
+
+            sdk = SDK("COM4")
+            application = sdk.get_pm_application()
+            x = application.get_supported_ldo()
+            x = application.get_ldo_status(application.LDO_OPTICAL)
+
+        """
+        request_packet = LDOStatusPacket(Application.PM, PMCommand.LDO_STATUS_CHECK_REQ)
+        request_packet.set_payload('ldo_num', ldo)
+        response_packet = LDOStatusPacket(Application.PM, PMCommand.LDO_STATUS_CHECK_RES)
+        return self._send_packet(request_packet, response_packet)
+
+    @staticmethod
+    def get_supported_power_modes() -> List[EDAPowerMode]:
+        """
+        List all supported power mode for EDA.
+
+        :return: Array of power modes enums.
+        :rtype: List
+
+        .. code-block:: python3
+            :emphasize-lines: 5
+
+            from adi_study_watch import SDK
+
+            sdk = SDK("COM4")
+            application = sdk.get_test_application()
+            x = application.get_supported_power_modes()
+            print(x)
+        """
+        return [TestApplication.POWER_INVALID, TestApplication.POWER_SLEEP, TestApplication.POWER_WAKEUP]
+
+    def eda_set_power_mode(self, power_mode: EDAPowerMode) -> Dict:
+        """
+        Control the AD5940 ICs power state: to make it enter Hibernate or wakeup state.
+        EPHY_LDO turn On needs to be done prior to this.
+
+        :param power_mode: power mode, use get_supported_power_modes() to get all supported power modes.
+        :return: A response packet as dictionary.
+        :rtype: Dict
+
+        .. code-block:: python3
+            :emphasize-lines: 5
+
+            from adi_study_watch import SDK
+
+            sdk = SDK("COM4")
+            application = sdk.get_test_application()
+            x = application.set_power_mode(application.POWER_SLEEP)
+        """
+        request_packet = EDASleepWakeupPacket(Application.EDA, EDACommand.CONTROL_AD5940_SLEEP_WAKEUP_REQ)
+        request_packet.set_payload("power_mode", power_mode)
+        response_packet = EDASleepWakeupPacket(Application.EDA, EDACommand.CONTROL_AD5940_SLEEP_WAKEUP_RES)
+        return self._send_packet(request_packet, response_packet)
+
+    def eda_get_power_status(self) -> Dict:
+        """
+        Check the AD5940 ICs power state: whether it is in Hibernate or wakeup state.
+        EPHY_LDO turn On needs to be done prior to this, if it is off previously.
+
+        :return: A response packet as dictionary.
+        :rtype: Dict
+
+        .. code-block:: python3
+            :emphasize-lines: 5
+
+            from adi_study_watch import SDK
+
+            sdk = SDK("COM4")
+            application = sdk.get_test_application()
+            x = application.eda_get_power_status()
+        """
+        request_packet = EDASleepWakeupPacket(Application.EDA, EDACommand.SLEEP_WAKEUP_STATUS_REQ)
+        response_packet = EDASleepWakeupPacket(Application.EDA, EDACommand.SLEEP_WAKEUP_STATUS_RES)
+        return self._send_packet(request_packet, response_packet)
```

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/user0_application.py` & `adi_study_watch-5.21.0/adi_study_watch/application/user0_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/application/vsm_mb_sb/pm_application.py` & `adi_study_watch-5.21.0/adi_study_watch/application/vsm_mb_sb/pm_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/__init__.py` & `adi_study_watch-5.21.0/adi_study_watch/core/__init__.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/ble_manager.py` & `adi_study_watch-5.21.0/adi_study_watch/core/ble_manager.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/data_types/array.py` & `adi_study_watch-5.21.0/adi_study_watch/core/data_types/array.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/data_types/binary.py` & `adi_study_watch-5.21.0/adi_study_watch/core/data_types/binary.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/data_types/decimal.py` & `adi_study_watch-5.21.0/adi_study_watch/core/data_types/decimal.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/data_types/enums.py` & `adi_study_watch-5.21.0/adi_study_watch/core/data_types/enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/data_types/integer.py` & `adi_study_watch-5.21.0/adi_study_watch/core/data_types/integer.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/data_types/string.py` & `adi_study_watch-5.21.0/adi_study_watch/core/data_types/string.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/enums/__init__.py` & `adi_study_watch-5.21.0/adi_study_watch/core/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/enums/ad7156_enums.py` & `adi_study_watch-5.21.0/adi_study_watch/core/enums/ad7156_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/enums/adp5360_enums.py` & `adi_study_watch-5.21.0/adi_study_watch/core/enums/adp5360_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/enums/adpd_enums.py` & `adi_study_watch-5.21.0/adi_study_watch/core/enums/adpd_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/enums/adxl_enums.py` & `adi_study_watch-5.21.0/adi_study_watch/core/enums/adxl_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/enums/bia_enums.py` & `adi_study_watch-5.21.0/adi_study_watch/core/enums/bia_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/enums/board_enums.py` & `adi_study_watch-5.21.0/adi_study_watch/core/enums/board_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/enums/common_enums.py` & `adi_study_watch-5.21.0/adi_study_watch/core/enums/common_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/enums/dcb_enums.py` & `adi_study_watch-5.21.0/adi_study_watch/core/enums/dcb_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/enums/display_enums.py` & `adi_study_watch-5.21.0/adi_study_watch/core/enums/display_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/enums/ecg_enums.py` & `adi_study_watch-5.21.0/adi_study_watch/core/enums/ecg_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/enums/eda_enums.py` & `adi_study_watch-5.21.0/adi_study_watch/core/enums/eda_enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,14 +70,16 @@
     GET_RTIA_TABLE_FDS_RES = [0x59]
     GET_RTIA_TABLE_RAM_REQ = [0x5A]
     GET_RTIA_TABLE_RAM_RES = [0x5B]
     DELETE_RTIA_TABLE_IN_FDS_REQ = [0x5C]
     DELETE_RTIA_TABLE_IN_FDS_RES = [0x5D]
     CONTROL_AD5940_SLEEP_WAKEUP_REQ = [0x62]
     CONTROL_AD5940_SLEEP_WAKEUP_RES = [0x63]
+    SLEEP_WAKEUP_STATUS_REQ = [0x64]
+    SLEEP_WAKEUP_STATUS_RES = [0x65]
 
     def __repr__(self):
         return "<%s.%s: %r>" % (self.__class__.__name__, self._name_, utils.convert_int_array_to_hex(self._value_))
 
 
 class EDAPowerMode(Enum):
     """
```

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/enums/fs_enums.py` & `adi_study_watch-5.21.0/adi_study_watch/core/enums/fs_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/enums/low_touch_enum.py` & `adi_study_watch-5.21.0/adi_study_watch/core/enums/low_touch_enum.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/enums/pedometer_enums.py` & `adi_study_watch-5.21.0/adi_study_watch/core/enums/pedometer_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/enums/pm_enums.py` & `adi_study_watch-5.21.0/adi_study_watch/core/enums/pm_enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,18 @@
     LOAD_CFG_RES = [0xB0]
     FDS_ERASE_REQ = [0xB1]
     FDS_ERASE_RES = [0xB2]
     GET_CONNECTED_TOOL_ADDR_REQ = [0xB3]
     GET_CONNECTED_TOOL_ADDR_RES = [0xB4]
     GET_BOOTLOADER_VERSION_REQ = [0xB5]
     GET_BOOTLOADER_VERSION_RES = [0xB6]
+    LDO_STATUS_CHECK_REQ = [0xB7]
+    LDO_STATUS_CHECK_RES = [0xB8]
+    DG2502_SW_STATUS_REQ = [0xB9]
+    DG2502_SW_STATUS_RES = [0xBA]
 
     def __repr__(self):
         return "<%s.%s: %r>" % (self.__class__.__name__, self._name_, utils.convert_int_array_to_hex(self._value_))
 
 
 class PMStatus(Enum):
     """
@@ -203,14 +207,22 @@
     OPTICAL = [0x2]
     EPHYZ = [0x3]
 
     def __repr__(self):
         return "<%s.%s: %r>" % (self.__class__.__name__, self._name_, utils.convert_int_array_to_hex(self._value_))
 
 
+class ControlStatus(Enum):
+    ENABLE = [0x1]
+    DISABLE = [0x0]
+
+    def __repr__(self):
+        return "<%s.%s: %r>" % (self.__class__.__name__, self._name_, utils.convert_int_array_to_hex(self._value_))
+
+
 class ChipID(Enum):
     """
     ChipID Enum
     """
     ADXL362 = [0x1]
     ADPD4K = [0x2]
     ADP5360 = [0x3]
```

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/enums/ppg_enums.py` & `adi_study_watch-5.21.0/adi_study_watch/core/enums/ppg_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/enums/sqi_enum.py` & `adi_study_watch-5.21.0/adi_study_watch/core/enums/sqi_enum.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/enums/user0_enums.py` & `adi_study_watch-5.21.0/adi_study_watch/core/enums/user0_enums.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/packet_manager.py` & `adi_study_watch-5.21.0/adi_study_watch/core/packet_manager.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/packets/__init__.py` & `adi_study_watch-5.21.0/adi_study_watch/core/packets/__init__.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/packets/ad7156_packets.py` & `adi_study_watch-5.21.0/adi_study_watch/core/packets/ad7156_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/packets/adp5360_packets.py` & `adi_study_watch-5.21.0/adi_study_watch/core/packets/adp5360_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/packets/adpd_packets.py` & `adi_study_watch-5.21.0/adi_study_watch/core/packets/adpd_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/packets/adxl_packets.py` & `adi_study_watch-5.21.0/adi_study_watch/core/packets/adxl_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/packets/bia_packets.py` & `adi_study_watch-5.21.0/adi_study_watch/core/packets/bia_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/packets/command_packet.py` & `adi_study_watch-5.21.0/adi_study_watch/core/packets/command_packet.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/packets/common_packets.py` & `adi_study_watch-5.21.0/adi_study_watch/core/packets/common_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/packets/display_packets.py` & `adi_study_watch-5.21.0/adi_study_watch/core/packets/display_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/packets/ecg_packets.py` & `adi_study_watch-5.21.0/adi_study_watch/core/packets/ecg_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/packets/eda_packets.py` & `adi_study_watch-5.21.0/adi_study_watch/core/packets/eda_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/packets/fs_packets.py` & `adi_study_watch-5.21.0/adi_study_watch/core/packets/fs_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/packets/low_touch_packets.py` & `adi_study_watch-5.21.0/adi_study_watch/core/packets/low_touch_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/packets/pm_packets.py` & `adi_study_watch-5.21.0/adi_study_watch/core/packets/pm_packets.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from ..data_types.array import Array
 from ..data_types.enums import Enums
 from ..data_types.integer import Int
 from ..data_types.binary import Binary
 from ..data_types.string import String
 from .command_packet import CommandPacket
 from ..enums.common_enums import Application
-from ..enums.pm_enums import MCUType, ElectrodeSwitch, LDO, ChipID, PowerMode
+from ..enums.pm_enums import MCUType, ElectrodeSwitch, LDO, ChipID, PowerMode, ControlStatus
 
 
 class AppsHealthPacket(CommandPacket):
     """
     Packet Structure:
 
     .. code-block::
@@ -459,7 +459,21 @@
         self._config['payload']['bootloader_version'] = Int(4)
 
 
 class ToolAddressPacket(CommandPacket):
     def __init__(self, destination=None, command=None):
         super().__init__(destination, command)
         self._config['payload']['tool_address'] = Enums(2, enum_class=Application, reverse=True)
+
+
+class LDOStatusPacket(CommandPacket):
+    def __init__(self, destination=None, command=None):
+        super().__init__(destination, command)
+        self._config['payload']['ldo_num'] = Enums(1, enum_class=LDO)
+        self._config['payload']['ldo_status'] = Int(1)
+
+
+class DG2502SWStatusPacket(CommandPacket):
+    def __init__(self, destination=None, command=None):
+        super().__init__(destination, command)
+        self._config['payload']['sw_name'] = Enums(1, enum_class=ElectrodeSwitch)
+        self._config['payload']['sw_status'] = Enums(1, enum_class=ControlStatus)
```

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/packets/ppg_packets.py` & `adi_study_watch-5.21.0/adi_study_watch/core/packets/ppg_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/packets/sqi_packets.py` & `adi_study_watch-5.21.0/adi_study_watch/core/packets/sqi_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/packets/stream_data_packets.py` & `adi_study_watch-5.21.0/adi_study_watch/core/packets/stream_data_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/packets/temperature_packets.py` & `adi_study_watch-5.21.0/adi_study_watch/core/packets/temperature_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/packets/user0_packets.py` & `adi_study_watch-5.21.0/adi_study_watch/core/packets/user0_packets.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/core/utils.py` & `adi_study_watch-5.21.0/adi_study_watch/core/utils.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/adi_study_watch/sdk.py` & `adi_study_watch-5.21.0/adi_study_watch/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     """
 
     READING_LOG = 0
     JOINING_CSV = 1
 
     STUDY_WATCH = Board.STUDY_WATCH
     VSM_MB_SB = Board.VSM_MB_SB
-    __version__ = "5.20.0"
+    __version__ = "5.21.0"
 
     def __init__(self, serial_port_address: str, mac_address: str = None, baud_rate: int = 921600,
                  board=Board.STUDY_WATCH, logging_filename: str = None, debug: bool = False,
                  sync_date_time=True, check_version=True, ble_vendor_id: int = 0x0456, ble_product_id: int = 0x2CFE,
                  ble_serial_number: str = None, ble_timeout: int = 10, check_existing_connection=True, **kwargs):
         """
         Creates a SDK object
@@ -211,17 +211,17 @@
     @staticmethod
     def _check_version(version):
         if version["payload"]["status"] == CommonStatus.NO_RESPONSE:
             raise Exception("Can't establish connection to the study watch.")
 
         supported_version = f"{version['payload']['major_version']}.{version['payload']['minor_version']}." \
                             f"{version['payload']['patch_version']}"
-        if not supported_version == "5.20.0":
+        if not supported_version == "5.21.0":
             logger.warning(f"Current firmware is not fully compatible with this SDK Version.\n"
-                           f"Supported Firmware Version :: 5.20.0\n"
+                           f"Supported Firmware Version :: 5.21.0\n"
                            f"Current Firmware Version :: {supported_version}\n"
                            f"SDK Version :: {SDK.__version__}\n")
 
     def _subscribe_alarms(self):
         for app in [Application.ADP5360, Application.FS, Application.ADPD, Application.PM]:
             packet_id = self._get_packet_id(CommonCommand.ALARM_NOTIFICATION, app)
             self._packet_manager.subscribe(packet_id, self._alarms_callback)
```

### Comparing `adi_study_watch-5.20.0/adi_study_watch.egg-info/PKG-INFO` & `adi_study_watch-5.21.0/adi_study_watch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adi-study-watch
-Version: 5.20.0
+Version: 5.21.0
 Summary: ADI study watch python SDK
 Home-page: https://github.com/analogdevicesinc/study-watch-sdk
 Author: Analog Devices, Inc.
 Author-email: healthcare-support@analog.com
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `adi_study_watch-5.20.0/adi_study_watch.egg-info/SOURCES.txt` & `adi_study_watch-5.21.0/adi_study_watch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/setup.py` & `adi_study_watch-5.21.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="adi_study_watch",
-    version="5.20.0",
+    version="5.21.0",
     author="Analog Devices, Inc.",
     author_email="healthcare-support@analog.com",
     license='Apache License, Version 2.0',
     description="ADI study watch python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/analogdevicesinc/study-watch-sdk",
@@ -31,8 +31,8 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Intended Audience :: Healthcare Industry',
         'Topic :: Software Development :: Libraries',
     ],
     python_requires='>=3.6',
     install_requires=['pyserial==3.5', 'tqdm==4.61.0', 'libusb1==3.0.0'],
-)
+)
```

### Comparing `adi_study_watch-5.20.0/tests/test_ad7156_application.py` & `adi_study_watch-5.21.0/tests/test_ad7156_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/tests/test_adpd_application.py` & `adi_study_watch-5.21.0/tests/test_adpd_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/tests/test_adxl_application.py` & `adi_study_watch-5.21.0/tests/test_adxl_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/tests/test_application.py` & `adi_study_watch-5.21.0/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/tests/test_bcm_application.py` & `adi_study_watch-5.21.0/tests/test_bcm_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/tests/test_ecg_application.py` & `adi_study_watch-5.21.0/tests/test_ecg_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/tests/test_eda_application.py` & `adi_study_watch-5.21.0/tests/test_eda_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/tests/test_fs_application.py` & `adi_study_watch-5.21.0/tests/test_fs_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/tests/test_pedometer_application.py` & `adi_study_watch-5.21.0/tests/test_pedometer_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/tests/test_pm_application.py` & `adi_study_watch-5.21.0/tests/test_pm_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/tests/test_ppg_application.py` & `adi_study_watch-5.21.0/tests/test_ppg_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/tests/test_sqi_application.py` & `adi_study_watch-5.21.0/tests/test_sqi_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/tests/test_temperature_application.py` & `adi_study_watch-5.21.0/tests/test_temperature_application.py`

 * *Files identical despite different names*

### Comparing `adi_study_watch-5.20.0/tests/test_user0_application.py` & `adi_study_watch-5.21.0/tests/test_user0_application.py`

 * *Files identical despite different names*

