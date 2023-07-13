# Comparing `tmp/trevorspray-2.0.8.tar.gz` & `tmp/trevorspray-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trevorspray-2.0.8.tar", max compression
+gzip compressed data, was "trevorspray-2.0.9.tar", max compression
```

## Comparing `trevorspray-2.0.8.tar` & `trevorspray-2.0.9.tar`

### file list

```diff
@@ -1,98 +1,98 @@
--rw-r--r--   0        0        0    35149 2020-09-23 15:46:29.895512 trevorspray-2.0.8/LICENSE
--rw-r--r--   0        0        0      709 2023-06-20 17:03:10.929231 trevorspray-2.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-20 15:38:56.221364 trevorspray-2.0.8/trevorspray/__init__.py
--rwxr-xr-x   0        0        0     9888 2023-06-20 16:20:19.141801 trevorspray-2.0.8/trevorspray/cli.py
--rw-r--r--   0        0        0      173 2023-06-20 15:41:48.178620 trevorspray-2.0.8/trevorspray/lib/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    10274 2022-02-05 01:19:08.134611 trevorspray-2.0.8/trevorspray/lib/__pycache__/discover.cpython-310.pyc
--rw-r--r--   0        0        0    19522 2023-06-20 16:59:20.506763 trevorspray-2.0.8/trevorspray/lib/__pycache__/discover.cpython-311.pyc
--rw-r--r--   0        0        0    10380 2022-02-02 18:01:43.844552 trevorspray-2.0.8/trevorspray/lib/__pycache__/discover.cpython-39.pyc
--rw-r--r--   0        0        0      328 2022-02-05 00:51:49.874543 trevorspray-2.0.8/trevorspray/lib/__pycache__/errors.cpython-310.pyc
--rw-r--r--   0        0        0      412 2023-06-20 16:59:20.433427 trevorspray-2.0.8/trevorspray/lib/__pycache__/errors.cpython-311.pyc
--rw-r--r--   0        0        0      324 2021-12-13 20:13:34.963665 trevorspray-2.0.8/trevorspray/lib/__pycache__/errors.cpython-39.pyc
--rw-r--r--   0        0        0     4148 2022-04-25 18:43:52.894020 trevorspray-2.0.8/trevorspray/lib/__pycache__/logger.cpython-310.pyc
--rw-r--r--   0        0        0     6951 2023-06-20 16:59:20.403427 trevorspray-2.0.8/trevorspray/lib/__pycache__/logger.cpython-311.pyc
--rw-r--r--   0        0        0     3625 2022-01-25 19:23:44.701631 trevorspray-2.0.8/trevorspray/lib/__pycache__/logger.cpython-39.pyc
--rw-r--r--   0        0        0     8383 2022-04-29 20:12:15.812195 trevorspray-2.0.8/trevorspray/lib/__pycache__/proxy.cpython-310.pyc
--rw-r--r--   0        0        0    18342 2023-06-20 16:59:20.520097 trevorspray-2.0.8/trevorspray/lib/__pycache__/proxy.cpython-311.pyc
--rw-r--r--   0        0        0     7910 2022-02-02 20:58:01.961663 trevorspray-2.0.8/trevorspray/lib/__pycache__/proxy.cpython-39.pyc
--rw-r--r--   0        0        0     4880 2022-01-25 18:16:33.441462 trevorspray-2.0.8/trevorspray/lib/__pycache__/sprayer.cpython-39.pyc
--rw-r--r--   0        0        0     6483 2022-04-25 18:43:53.020687 trevorspray-2.0.8/trevorspray/lib/__pycache__/trevor.cpython-310.pyc
--rw-r--r--   0        0        0    14051 2023-06-20 16:59:20.503430 trevorspray-2.0.8/trevorspray/lib/__pycache__/trevor.cpython-311.pyc
--rw-r--r--   0        0        0     6050 2022-02-02 18:57:32.781359 trevorspray-2.0.8/trevorspray/lib/__pycache__/trevor.cpython-39.pyc
--rw-r--r--   0        0        0     4672 2022-01-25 21:00:12.908541 trevorspray-2.0.8/trevorspray/lib/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0    12620 2023-06-20 16:20:19.195134 trevorspray-2.0.8/trevorspray/lib/discover.py
--rw-r--r--   0        0        0      744 2023-06-20 16:20:18.968468 trevorspray-2.0.8/trevorspray/lib/enumerators/__init__.py
--rw-r--r--   0        0        0      752 2022-02-05 00:51:49.937877 trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1322 2023-06-20 16:59:20.503430 trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      748 2022-02-01 21:14:34.331680 trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2215 2022-04-25 18:43:53.024021 trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-310.pyc
--rw-r--r--   0        0        0     3771 2023-06-20 16:59:20.506763 trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-311.pyc
--rw-r--r--   0        0        0     2177 2022-01-31 20:34:18.741622 trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-39.pyc
--rw-r--r--   0        0        0     2057 2022-04-25 18:43:53.024021 trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-310.pyc
--rw-r--r--   0        0        0     2859 2023-06-20 16:59:20.506763 trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-311.pyc
--rw-r--r--   0        0        0     2020 2022-02-01 21:21:47.395032 trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-39.pyc
--rw-r--r--   0        0        0     2503 2023-06-20 16:20:19.001802 trevorspray-2.0.8/trevorspray/lib/enumerators/onedrive.py
--rw-r--r--   0        0        0     1935 2023-06-20 16:20:18.988468 trevorspray-2.0.8/trevorspray/lib/enumerators/seamless_sso.py
--rw-r--r--   0        0        0       44 2023-06-20 16:20:18.948469 trevorspray-2.0.8/trevorspray/lib/errors.py
--rw-r--r--   0        0        0     4419 2023-06-20 16:20:19.028468 trevorspray-2.0.8/trevorspray/lib/logger.py
--rw-r--r--   0        0        0     1036 2022-02-05 00:51:49.937877 trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     1705 2023-06-20 16:59:20.503430 trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     1028 2022-01-27 17:15:46.627782 trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0    11619 2022-02-05 00:51:49.937877 trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/msol.cpython-310.pyc
--rw-r--r--   0        0        0    22400 2023-06-20 16:59:20.500096 trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/msol.cpython-311.pyc
--rw-r--r--   0        0        0    11403 2022-01-25 21:04:10.745217 trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/msol.cpython-39.pyc
--rw-r--r--   0        0        0      568 2023-06-20 16:20:18.965135 trevorspray-2.0.8/trevorspray/lib/looters/base.py
--rw-r--r--   0        0        0    16133 2023-06-20 16:20:19.215134 trevorspray-2.0.8/trevorspray/lib/looters/msol.py
--rw-r--r--   0        0        0    13015 2023-06-20 16:20:19.211801 trevorspray-2.0.8/trevorspray/lib/proxy.py
--rw-r--r--   0        0        0      765 2023-06-20 16:31:58.921533 trevorspray-2.0.8/trevorspray/lib/sprayers/__init__.py
--rw-r--r--   0        0        0      746 2022-02-05 00:51:49.874543 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1324 2023-06-20 16:59:20.430094 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      742 2022-02-01 21:14:34.305014 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3247 2022-02-07 14:54:28.512909 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/adfs.cpython-310.pyc
--rw-r--r--   0        0        0     5650 2023-06-20 16:59:20.460095 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/adfs.cpython-311.pyc
--rw-r--r--   0        0        0     3245 2022-02-03 20:11:00.807482 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/adfs.cpython-39.pyc
--rw-r--r--   0        0        0     4879 2022-04-25 18:43:52.970687 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-310.pyc
--rw-r--r--   0        0        0     9087 2023-06-20 16:59:20.456761 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-311.pyc
--rw-r--r--   0        0        0     4800 2022-02-03 20:22:37.297511 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-39.pyc
--rw-r--r--   0        0        0     3836 2022-02-07 14:54:28.479575 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     6895 2023-06-20 16:59:20.433427 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     3843 2022-02-03 20:01:13.737457 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     1289 2022-02-05 00:51:49.937877 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/example.cpython-310.pyc
--rw-r--r--   0        0        0     1784 2023-06-20 16:59:20.503430 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/example.cpython-311.pyc
--rw-r--r--   0        0        0     1271 2022-01-18 15:54:51.036838 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/example.cpython-39.pyc
--rw-r--r--   0        0        0     3743 2022-04-25 18:43:53.017354 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/msol.cpython-310.pyc
--rw-r--r--   0        0        0     5522 2023-06-20 16:59:20.496763 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/msol.cpython-311.pyc
--rw-r--r--   0        0        0     3688 2022-02-03 20:11:00.850815 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/msol.cpython-39.pyc
--rw-r--r--   0        0        0     2054 2022-02-07 14:54:28.512909 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/okta.cpython-310.pyc
--rw-r--r--   0        0        0     3386 2023-06-20 17:00:00.287891 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/okta.cpython-311.pyc
--rw-r--r--   0        0        0     2027 2022-02-03 21:46:45.294387 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/okta.cpython-39.pyc
--rw-r--r--   0        0        0     2842 2022-02-07 14:54:28.482909 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/owa.cpython-310.pyc
--rw-r--r--   0        0        0     4982 2023-06-20 16:59:20.433427 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/owa.cpython-311.pyc
--rw-r--r--   0        0        0     2752 2022-02-03 20:11:00.794149 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/owa.cpython-39.pyc
--rw-r--r--   0        0        0     3781 2023-06-20 16:20:19.031802 trevorspray-2.0.8/trevorspray/lib/sprayers/adfs.py
--rw-r--r--   0        0        0     7408 2023-06-20 16:20:19.078468 trevorspray-2.0.8/trevorspray/lib/sprayers/anyconnect.py
--rw-r--r--   0        0        0     4131 2023-06-20 16:20:19.061802 trevorspray-2.0.8/trevorspray/lib/sprayers/base.py
--rw-r--r--   0        0        0     1297 2023-06-20 16:20:18.995135 trevorspray-2.0.8/trevorspray/lib/sprayers/example.py
--rw-r--r--   0        0        0     5046 2023-06-20 16:20:19.058468 trevorspray-2.0.8/trevorspray/lib/sprayers/msol.py
--rw-r--r--   0        0        0     2250 2023-06-20 16:59:57.761155 trevorspray-2.0.8/trevorspray/lib/sprayers/okta.py
--rw-r--r--   0        0        0     3299 2023-06-20 16:20:19.061802 trevorspray-2.0.8/trevorspray/lib/sprayers/owa.py
--rw-r--r--   0        0        0     8564 2023-06-20 16:20:19.201801 trevorspray-2.0.8/trevorspray/lib/trevor.py
--rw-r--r--   0        0        0       91 2023-06-20 16:20:19.031802 trevorspray-2.0.8/trevorspray/lib/util/__init__.py
--rw-r--r--   0        0        0      274 2022-02-05 00:51:49.824543 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      330 2023-06-20 16:59:20.406760 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      272 2022-01-31 18:58:32.148049 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5749 2022-04-25 18:43:52.897354 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/misc.cpython-310.pyc
--rw-r--r--   0        0        0    11382 2023-06-20 16:59:20.406760 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/misc.cpython-311.pyc
--rw-r--r--   0        0        0     5534 2022-02-02 15:07:49.377447 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/misc.cpython-39.pyc
--rw-r--r--   0        0        0     6610 2022-02-05 00:51:49.874543 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-310.pyc
--rw-r--r--   0        0        0    11205 2023-06-20 16:59:20.430094 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-311.pyc
--rw-r--r--   0        0        0     6644 2022-01-28 21:23:31.518382 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-39.pyc
--rw-r--r--   0        0        0     1165 2022-01-31 16:20:46.034318 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/threading.cpython-39.pyc
--rw-r--r--   0        0        0     4855 2022-02-05 00:51:49.871210 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/threadpool.cpython-310.pyc
--rw-r--r--   0        0        0     9259 2023-06-20 16:59:20.430094 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/threadpool.cpython-311.pyc
--rw-r--r--   0        0        0     4807 2022-01-31 20:14:54.024908 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/threadpool.cpython-39.pyc
--rw-r--r--   0        0        0     5763 2023-06-20 16:20:19.168468 trevorspray-2.0.8/trevorspray/lib/util/misc.py
--rw-r--r--   0        0        0     7407 2023-06-20 16:20:19.128468 trevorspray-2.0.8/trevorspray/lib/util/ntlmdecoder.py
--rw-r--r--   0        0        0     4374 2023-06-20 16:20:19.151801 trevorspray-2.0.8/trevorspray/lib/util/threadpool.py
--rwxr-xr-x   0        0        0     2816 2020-10-15 19:54:12.675089 trevorspray-2.0.8/trevorspray/trevorproxy.py.bak
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 trevorspray-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2020-09-23 15:46:29.895512 trevorspray-2.0.9/LICENSE
+-rw-r--r--   0        0        0      709 2023-07-13 19:37:29.542379 trevorspray-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-20 15:38:56.221364 trevorspray-2.0.9/trevorspray/__init__.py
+-rwxr-xr-x   0        0        0     9888 2023-06-20 16:20:19.141801 trevorspray-2.0.9/trevorspray/cli.py
+-rw-r--r--   0        0        0      173 2023-06-20 15:41:48.178620 trevorspray-2.0.9/trevorspray/lib/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    10274 2022-02-05 01:19:08.134611 trevorspray-2.0.9/trevorspray/lib/__pycache__/discover.cpython-310.pyc
+-rw-r--r--   0        0        0    19522 2023-06-20 16:59:20.506763 trevorspray-2.0.9/trevorspray/lib/__pycache__/discover.cpython-311.pyc
+-rw-r--r--   0        0        0    10380 2022-02-02 18:01:43.844552 trevorspray-2.0.9/trevorspray/lib/__pycache__/discover.cpython-39.pyc
+-rw-r--r--   0        0        0      328 2022-02-05 00:51:49.874543 trevorspray-2.0.9/trevorspray/lib/__pycache__/errors.cpython-310.pyc
+-rw-r--r--   0        0        0      412 2023-06-20 16:59:20.433427 trevorspray-2.0.9/trevorspray/lib/__pycache__/errors.cpython-311.pyc
+-rw-r--r--   0        0        0      324 2021-12-13 20:13:34.963665 trevorspray-2.0.9/trevorspray/lib/__pycache__/errors.cpython-39.pyc
+-rw-r--r--   0        0        0     4148 2022-04-25 18:43:52.894020 trevorspray-2.0.9/trevorspray/lib/__pycache__/logger.cpython-310.pyc
+-rw-r--r--   0        0        0     6951 2023-06-20 16:59:20.403427 trevorspray-2.0.9/trevorspray/lib/__pycache__/logger.cpython-311.pyc
+-rw-r--r--   0        0        0     3625 2022-01-25 19:23:44.701631 trevorspray-2.0.9/trevorspray/lib/__pycache__/logger.cpython-39.pyc
+-rw-r--r--   0        0        0     8383 2022-04-29 20:12:15.812195 trevorspray-2.0.9/trevorspray/lib/__pycache__/proxy.cpython-310.pyc
+-rw-r--r--   0        0        0    18342 2023-06-20 16:59:20.520097 trevorspray-2.0.9/trevorspray/lib/__pycache__/proxy.cpython-311.pyc
+-rw-r--r--   0        0        0     7910 2022-02-02 20:58:01.961663 trevorspray-2.0.9/trevorspray/lib/__pycache__/proxy.cpython-39.pyc
+-rw-r--r--   0        0        0     4880 2022-01-25 18:16:33.441462 trevorspray-2.0.9/trevorspray/lib/__pycache__/sprayer.cpython-39.pyc
+-rw-r--r--   0        0        0     6483 2022-04-25 18:43:53.020687 trevorspray-2.0.9/trevorspray/lib/__pycache__/trevor.cpython-310.pyc
+-rw-r--r--   0        0        0    14051 2023-06-20 16:59:20.503430 trevorspray-2.0.9/trevorspray/lib/__pycache__/trevor.cpython-311.pyc
+-rw-r--r--   0        0        0     6050 2022-02-02 18:57:32.781359 trevorspray-2.0.9/trevorspray/lib/__pycache__/trevor.cpython-39.pyc
+-rw-r--r--   0        0        0     4672 2022-01-25 21:00:12.908541 trevorspray-2.0.9/trevorspray/lib/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0    12620 2023-06-20 16:20:19.195134 trevorspray-2.0.9/trevorspray/lib/discover.py
+-rw-r--r--   0        0        0      638 2023-07-13 14:36:03.130817 trevorspray-2.0.9/trevorspray/lib/enumerators/__init__.py
+-rw-r--r--   0        0        0      752 2022-02-05 00:51:49.937877 trevorspray-2.0.9/trevorspray/lib/enumerators/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1305 2023-07-13 14:34:28.083988 trevorspray-2.0.9/trevorspray/lib/enumerators/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      748 2022-02-01 21:14:34.331680 trevorspray-2.0.9/trevorspray/lib/enumerators/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2215 2022-04-25 18:43:53.024021 trevorspray-2.0.9/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-310.pyc
+-rw-r--r--   0        0        0     3771 2023-06-20 16:59:20.506763 trevorspray-2.0.9/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-311.pyc
+-rw-r--r--   0        0        0     2177 2022-01-31 20:34:18.741622 trevorspray-2.0.9/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-39.pyc
+-rw-r--r--   0        0        0     2057 2022-04-25 18:43:53.024021 trevorspray-2.0.9/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-310.pyc
+-rw-r--r--   0        0        0     2859 2023-06-20 16:59:20.506763 trevorspray-2.0.9/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-311.pyc
+-rw-r--r--   0        0        0     2020 2022-02-01 21:21:47.395032 trevorspray-2.0.9/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-39.pyc
+-rw-r--r--   0        0        0     2503 2023-06-20 16:20:19.001802 trevorspray-2.0.9/trevorspray/lib/enumerators/onedrive.py
+-rw-r--r--   0        0        0     1935 2023-06-20 16:20:18.988468 trevorspray-2.0.9/trevorspray/lib/enumerators/seamless_sso.py
+-rw-r--r--   0        0        0       44 2023-06-20 16:20:18.948469 trevorspray-2.0.9/trevorspray/lib/errors.py
+-rw-r--r--   0        0        0     4419 2023-06-20 16:20:19.028468 trevorspray-2.0.9/trevorspray/lib/logger.py
+-rw-r--r--   0        0        0     1036 2022-02-05 00:51:49.937877 trevorspray-2.0.9/trevorspray/lib/looters/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     1705 2023-06-20 16:59:20.503430 trevorspray-2.0.9/trevorspray/lib/looters/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1028 2022-01-27 17:15:46.627782 trevorspray-2.0.9/trevorspray/lib/looters/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0    11619 2022-02-05 00:51:49.937877 trevorspray-2.0.9/trevorspray/lib/looters/__pycache__/msol.cpython-310.pyc
+-rw-r--r--   0        0        0    22400 2023-06-20 16:59:20.500096 trevorspray-2.0.9/trevorspray/lib/looters/__pycache__/msol.cpython-311.pyc
+-rw-r--r--   0        0        0    11403 2022-01-25 21:04:10.745217 trevorspray-2.0.9/trevorspray/lib/looters/__pycache__/msol.cpython-39.pyc
+-rw-r--r--   0        0        0      568 2023-06-20 16:20:18.965135 trevorspray-2.0.9/trevorspray/lib/looters/base.py
+-rw-r--r--   0        0        0    16133 2023-06-20 16:20:19.215134 trevorspray-2.0.9/trevorspray/lib/looters/msol.py
+-rw-r--r--   0        0        0    13015 2023-06-20 16:20:19.211801 trevorspray-2.0.9/trevorspray/lib/proxy.py
+-rw-r--r--   0        0        0      655 2023-07-13 14:36:03.130817 trevorspray-2.0.9/trevorspray/lib/sprayers/__init__.py
+-rw-r--r--   0        0        0      746 2022-02-05 00:51:49.874543 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1153 2023-07-13 14:34:28.017337 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      742 2022-02-01 21:14:34.305014 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3247 2022-02-07 14:54:28.512909 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/adfs.cpython-310.pyc
+-rw-r--r--   0        0        0     5650 2023-06-20 16:59:20.460095 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/adfs.cpython-311.pyc
+-rw-r--r--   0        0        0     3245 2022-02-03 20:11:00.807482 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/adfs.cpython-39.pyc
+-rw-r--r--   0        0        0     4879 2022-04-25 18:43:52.970687 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-310.pyc
+-rw-r--r--   0        0        0     9087 2023-06-20 16:59:20.456761 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-311.pyc
+-rw-r--r--   0        0        0     4800 2022-02-03 20:22:37.297511 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-39.pyc
+-rw-r--r--   0        0        0     3836 2022-02-07 14:54:28.479575 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     6895 2023-06-20 16:59:20.433427 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     3843 2022-02-03 20:01:13.737457 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     1289 2022-02-05 00:51:49.937877 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/example.cpython-310.pyc
+-rw-r--r--   0        0        0     1784 2023-06-20 16:59:20.503430 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/example.cpython-311.pyc
+-rw-r--r--   0        0        0     1271 2022-01-18 15:54:51.036838 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/example.cpython-39.pyc
+-rw-r--r--   0        0        0     3743 2022-04-25 18:43:53.017354 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/msol.cpython-310.pyc
+-rw-r--r--   0        0        0     5522 2023-06-20 16:59:20.496763 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/msol.cpython-311.pyc
+-rw-r--r--   0        0        0     3688 2022-02-03 20:11:00.850815 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/msol.cpython-39.pyc
+-rw-r--r--   0        0        0     2054 2022-02-07 14:54:28.512909 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/okta.cpython-310.pyc
+-rw-r--r--   0        0        0     3386 2023-06-20 17:00:00.287891 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/okta.cpython-311.pyc
+-rw-r--r--   0        0        0     2027 2022-02-03 21:46:45.294387 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/okta.cpython-39.pyc
+-rw-r--r--   0        0        0     2842 2022-02-07 14:54:28.482909 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/owa.cpython-310.pyc
+-rw-r--r--   0        0        0     4982 2023-06-20 16:59:20.433427 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/owa.cpython-311.pyc
+-rw-r--r--   0        0        0     2752 2022-02-03 20:11:00.794149 trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/owa.cpython-39.pyc
+-rw-r--r--   0        0        0     3781 2023-06-20 16:20:19.031802 trevorspray-2.0.9/trevorspray/lib/sprayers/adfs.py
+-rw-r--r--   0        0        0     7408 2023-06-20 16:20:19.078468 trevorspray-2.0.9/trevorspray/lib/sprayers/anyconnect.py
+-rw-r--r--   0        0        0     4131 2023-06-20 16:20:19.061802 trevorspray-2.0.9/trevorspray/lib/sprayers/base.py
+-rw-r--r--   0        0        0     1297 2023-06-20 16:20:18.995135 trevorspray-2.0.9/trevorspray/lib/sprayers/example.py
+-rw-r--r--   0        0        0     5046 2023-06-20 16:20:19.058468 trevorspray-2.0.9/trevorspray/lib/sprayers/msol.py
+-rw-r--r--   0        0        0     2250 2023-06-20 16:59:57.761155 trevorspray-2.0.9/trevorspray/lib/sprayers/okta.py
+-rw-r--r--   0        0        0     3299 2023-06-20 16:20:19.061802 trevorspray-2.0.9/trevorspray/lib/sprayers/owa.py
+-rw-r--r--   0        0        0     8564 2023-06-20 16:20:19.201801 trevorspray-2.0.9/trevorspray/lib/trevor.py
+-rw-r--r--   0        0        0       91 2023-06-20 16:20:19.031802 trevorspray-2.0.9/trevorspray/lib/util/__init__.py
+-rw-r--r--   0        0        0      274 2022-02-05 00:51:49.824543 trevorspray-2.0.9/trevorspray/lib/util/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      330 2023-06-20 16:59:20.406760 trevorspray-2.0.9/trevorspray/lib/util/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      272 2022-01-31 18:58:32.148049 trevorspray-2.0.9/trevorspray/lib/util/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5749 2022-04-25 18:43:52.897354 trevorspray-2.0.9/trevorspray/lib/util/__pycache__/misc.cpython-310.pyc
+-rw-r--r--   0        0        0    11382 2023-06-20 16:59:20.406760 trevorspray-2.0.9/trevorspray/lib/util/__pycache__/misc.cpython-311.pyc
+-rw-r--r--   0        0        0     5534 2022-02-02 15:07:49.377447 trevorspray-2.0.9/trevorspray/lib/util/__pycache__/misc.cpython-39.pyc
+-rw-r--r--   0        0        0     6610 2022-02-05 00:51:49.874543 trevorspray-2.0.9/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-310.pyc
+-rw-r--r--   0        0        0    11205 2023-06-20 16:59:20.430094 trevorspray-2.0.9/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-311.pyc
+-rw-r--r--   0        0        0     6644 2022-01-28 21:23:31.518382 trevorspray-2.0.9/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-39.pyc
+-rw-r--r--   0        0        0     1165 2022-01-31 16:20:46.034318 trevorspray-2.0.9/trevorspray/lib/util/__pycache__/threading.cpython-39.pyc
+-rw-r--r--   0        0        0     4855 2022-02-05 00:51:49.871210 trevorspray-2.0.9/trevorspray/lib/util/__pycache__/threadpool.cpython-310.pyc
+-rw-r--r--   0        0        0     9259 2023-06-20 16:59:20.430094 trevorspray-2.0.9/trevorspray/lib/util/__pycache__/threadpool.cpython-311.pyc
+-rw-r--r--   0        0        0     4807 2022-01-31 20:14:54.024908 trevorspray-2.0.9/trevorspray/lib/util/__pycache__/threadpool.cpython-39.pyc
+-rw-r--r--   0        0        0     5763 2023-06-20 16:20:19.168468 trevorspray-2.0.9/trevorspray/lib/util/misc.py
+-rw-r--r--   0        0        0     7407 2023-06-20 16:20:19.128468 trevorspray-2.0.9/trevorspray/lib/util/ntlmdecoder.py
+-rw-r--r--   0        0        0     4374 2023-06-20 16:20:19.151801 trevorspray-2.0.9/trevorspray/lib/util/threadpool.py
+-rwxr-xr-x   0        0        0     2816 2020-10-15 19:54:12.675089 trevorspray-2.0.9/trevorspray/trevorproxy.py.bak
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 trevorspray-2.0.9/PKG-INFO
```

### Comparing `trevorspray-2.0.8/LICENSE` & `trevorspray-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/pyproject.toml` & `trevorspray-2.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trevorspray"
-version = "2.0.8"
+version = "2.0.9"
 description = "A modular password sprayer with threading, SSH proxying, loot modules, and more"
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 repository = "https://github.com/blacklanternsecurity/TREVORspray"
 homepage = "https://github.com/blacklanternsecurity/TREVORspray"
 
 [tool.poetry.dependencies]
```

### Comparing `trevorspray-2.0.8/trevorspray/cli.py` & `trevorspray-2.0.9/trevorspray/cli.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/__pycache__/discover.cpython-310.pyc` & `trevorspray-2.0.9/trevorspray/lib/__pycache__/discover.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/__pycache__/discover.cpython-311.pyc` & `trevorspray-2.0.9/trevorspray/lib/__pycache__/discover.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/__pycache__/discover.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/__pycache__/discover.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/__pycache__/logger.cpython-310.pyc` & `trevorspray-2.0.9/trevorspray/lib/__pycache__/logger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/__pycache__/logger.cpython-311.pyc` & `trevorspray-2.0.9/trevorspray/lib/__pycache__/logger.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/__pycache__/logger.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/__pycache__/logger.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/__pycache__/proxy.cpython-310.pyc` & `trevorspray-2.0.9/trevorspray/lib/__pycache__/proxy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/__pycache__/proxy.cpython-311.pyc` & `trevorspray-2.0.9/trevorspray/lib/__pycache__/proxy.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/__pycache__/proxy.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/__pycache__/proxy.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/__pycache__/sprayer.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/__pycache__/sprayer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/__pycache__/trevor.cpython-310.pyc` & `trevorspray-2.0.9/trevorspray/lib/__pycache__/trevor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/__pycache__/trevor.cpython-311.pyc` & `trevorspray-2.0.9/trevorspray/lib/__pycache__/trevor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/__pycache__/trevor.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/__pycache__/trevor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/__pycache__/util.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/__pycache__/util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/discover.py` & `trevorspray-2.0.9/trevorspray/lib/discover.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/enumerators/__init__.py` & `trevorspray-2.0.9/trevorspray/lib/enumerators/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,20 @@
-import os
 import importlib
 from pathlib import Path
 from ..sprayers.base import BaseSprayModule
 
 module_dir = Path(__file__).parent
-module_files = list(os.listdir(module_dir))
 module_choices = {}
 
-for file in module_files:
-    file = module_dir / file
-
-    if (
-        file.is_file()
-        and file.suffix.lower() == ".py"
-        and file.stem not in ["base", "__init__"]
-    ):
-        modules = importlib.import_module(f"lib.enumerators.{file.stem}", "trevorspray")
+for file in module_dir.glob("*.py"):
+    if file.is_file() and file.stem not in ["base", "__init__"]:
+        modules = importlib.import_module(
+            f"trevorspray.lib.enumerators.{file.stem}", "trevorspray"
+        )
 
         for m in modules.__dict__.keys():
             module = getattr(modules, m)
             try:
-                if BaseSprayModule in module.__bases__:
+                if BaseSprayModule in module.__mro__:
                     module_choices[file.stem] = module
             except AttributeError:
                 continue
```

### Comparing `trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/__init__.cpython-310.pyc` & `trevorspray-2.0.9/trevorspray/lib/enumerators/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/__init__.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/enumerators/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-310.pyc` & `trevorspray-2.0.9/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-311.pyc` & `trevorspray-2.0.9/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-310.pyc` & `trevorspray-2.0.9/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-311.pyc` & `trevorspray-2.0.9/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/enumerators/onedrive.py` & `trevorspray-2.0.9/trevorspray/lib/enumerators/onedrive.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/enumerators/seamless_sso.py` & `trevorspray-2.0.9/trevorspray/lib/enumerators/seamless_sso.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/logger.py` & `trevorspray-2.0.9/trevorspray/lib/logger.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/base.cpython-310.pyc` & `trevorspray-2.0.9/trevorspray/lib/looters/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/base.cpython-311.pyc` & `trevorspray-2.0.9/trevorspray/lib/looters/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/base.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/looters/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/msol.cpython-310.pyc` & `trevorspray-2.0.9/trevorspray/lib/looters/__pycache__/msol.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/msol.cpython-311.pyc` & `trevorspray-2.0.9/trevorspray/lib/looters/__pycache__/msol.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/msol.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/looters/__pycache__/msol.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/looters/base.py` & `trevorspray-2.0.9/trevorspray/lib/looters/base.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/looters/msol.py` & `trevorspray-2.0.9/trevorspray/lib/looters/msol.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/proxy.py` & `trevorspray-2.0.9/trevorspray/lib/proxy.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__init__.py` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,22 @@
-import os
 import importlib
 from pathlib import Path
 from .base import BaseSprayModule
 
 module_dir = Path(__file__).parent
-module_files = list(os.listdir(module_dir))
 module_choices = {}
 
-for file in module_files:
+for file in module_dir.glob("*.py"):
     file = module_dir / file
 
-    if (
-        file.is_file()
-        and file.suffix.lower() == ".py"
-        and file.stem not in ["base", "__init__"]
-    ):
+    if file.is_file() and file.stem not in ["base", "__init__"]:
         modules = importlib.import_module(
             f"trevorspray.lib.sprayers.{file.stem}", "trevorspray"
         )
 
         for m in modules.__dict__.keys():
             module = getattr(modules, m)
             try:
-                if BaseSprayModule in module.__bases__:
+                if BaseSprayModule in module.__mro__:
                     module_choices[file.stem] = module
             except AttributeError:
                 continue
```

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/__init__.cpython-310.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/__init__.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/adfs.cpython-310.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/adfs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/adfs.cpython-311.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/adfs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/adfs.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/adfs.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-310.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-311.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/base.cpython-310.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/base.cpython-311.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/base.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/example.cpython-310.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/example.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/example.cpython-311.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/example.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/example.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/example.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/msol.cpython-310.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/msol.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/msol.cpython-311.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/msol.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/msol.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/msol.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/okta.cpython-310.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/okta.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/okta.cpython-311.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/okta.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/okta.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/okta.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/owa.cpython-310.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/owa.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/owa.cpython-311.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/owa.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/owa.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/sprayers/__pycache__/owa.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/adfs.py` & `trevorspray-2.0.9/trevorspray/lib/sprayers/adfs.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/anyconnect.py` & `trevorspray-2.0.9/trevorspray/lib/sprayers/anyconnect.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/base.py` & `trevorspray-2.0.9/trevorspray/lib/sprayers/base.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/example.py` & `trevorspray-2.0.9/trevorspray/lib/sprayers/example.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/msol.py` & `trevorspray-2.0.9/trevorspray/lib/sprayers/msol.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/okta.py` & `trevorspray-2.0.9/trevorspray/lib/sprayers/okta.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/sprayers/owa.py` & `trevorspray-2.0.9/trevorspray/lib/sprayers/owa.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/trevor.py` & `trevorspray-2.0.9/trevorspray/lib/trevor.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/util/__pycache__/misc.cpython-310.pyc` & `trevorspray-2.0.9/trevorspray/lib/util/__pycache__/misc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/util/__pycache__/misc.cpython-311.pyc` & `trevorspray-2.0.9/trevorspray/lib/util/__pycache__/misc.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/util/__pycache__/misc.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/util/__pycache__/misc.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-310.pyc` & `trevorspray-2.0.9/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-311.pyc` & `trevorspray-2.0.9/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/util/__pycache__/threading.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/util/__pycache__/threading.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/util/__pycache__/threadpool.cpython-310.pyc` & `trevorspray-2.0.9/trevorspray/lib/util/__pycache__/threadpool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/util/__pycache__/threadpool.cpython-311.pyc` & `trevorspray-2.0.9/trevorspray/lib/util/__pycache__/threadpool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/util/__pycache__/threadpool.cpython-39.pyc` & `trevorspray-2.0.9/trevorspray/lib/util/__pycache__/threadpool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/util/misc.py` & `trevorspray-2.0.9/trevorspray/lib/util/misc.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/util/ntlmdecoder.py` & `trevorspray-2.0.9/trevorspray/lib/util/ntlmdecoder.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/lib/util/threadpool.py` & `trevorspray-2.0.9/trevorspray/lib/util/threadpool.py`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/trevorspray/trevorproxy.py.bak` & `trevorspray-2.0.9/trevorspray/trevorproxy.py.bak`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.8/PKG-INFO` & `trevorspray-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trevorspray
-Version: 2.0.8
+Version: 2.0.9
 Summary: A modular password sprayer with threading, SSH proxying, loot modules, and more
 Home-page: https://github.com/blacklanternsecurity/TREVORspray
 License: GPL-3.0
 Author: TheTechromancer
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

