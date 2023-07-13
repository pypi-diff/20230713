# Comparing `tmp/kuksa_client-0.4.0a4.tar.gz` & `tmp/kuksa_client-0.4.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuksa_client-0.4.0a4.tar", last modified: Wed Jun 28 08:56:56 2023, max compression
+gzip compressed data, was "kuksa_client-0.4.0a5.tar", last modified: Thu Jul 13 09:08:46 2023, max compression
```

## Comparing `kuksa_client-0.4.0a4.tar` & `kuksa_client-0.4.0a5.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-28 08:56:56.591435 kuksa_client-0.4.0a4/
--rw-r--r--   0 erik      (1000) erik      (1000)       35 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a4/MANIFEST.in
--rw-r--r--   0 erik      (1000) erik      (1000)    13411 2023-06-28 08:56:56.591435 kuksa_client-0.4.0a4/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)    12551 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a4/README.md
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-28 08:56:56.575442 kuksa_client-0.4.0a4/kuksa/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a4/kuksa/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-28 08:56:56.575442 kuksa_client-0.4.0a4/kuksa/val/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a4/kuksa/val/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-28 08:56:56.575442 kuksa_client-0.4.0a4/kuksa/val/v1/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a4/kuksa/val/v1/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     9993 2023-06-28 08:56:56.000000 kuksa_client-0.4.0a4/kuksa/val/v1/types_pb2.py
--rw-r--r--   0 erik      (1000) erik      (1000)      159 2023-06-28 08:56:56.000000 kuksa_client-0.4.0a4/kuksa/val/v1/types_pb2_grpc.py
--rw-r--r--   0 erik      (1000) erik      (1000)     4058 2023-06-28 08:56:56.000000 kuksa_client-0.4.0a4/kuksa/val/v1/val_pb2.py
--rw-r--r--   0 erik      (1000) erik      (1000)     8731 2023-06-28 08:56:56.000000 kuksa_client-0.4.0a4/kuksa/val/v1/val_pb2_grpc.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-28 08:56:56.579440 kuksa_client-0.4.0a4/kuksa_certificates/
--rw-r--r--   0 erik      (1000) erik      (1000)     1675 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a4/kuksa_certificates/CA.key
--rw-r--r--   0 erik      (1000) erik      (1000)     1342 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a4/kuksa_certificates/CA.pem
--rw-r--r--   0 erik      (1000) erik      (1000)     1679 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a4/kuksa_certificates/Client.key
--rw-r--r--   0 erik      (1000) erik      (1000)     1704 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a4/kuksa_certificates/Client.pem
--rw-r--r--   0 erik      (1000) erik      (1000)     3537 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a4/kuksa_certificates/README.md
--rw-r--r--   0 erik      (1000) erik      (1000)     1679 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a4/kuksa_certificates/Server.key
--rw-r--r--   0 erik      (1000) erik      (1000)     1704 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a4/kuksa_certificates/Server.pem
--rw-r--r--   0 erik      (1000) erik      (1000)      114 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a4/kuksa_certificates/__init__.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)     2023 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a4/kuksa_certificates/genCerts.sh
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-28 08:56:56.587436 kuksa_client-0.4.0a4/kuksa_certificates/jwt/
--rw-r--r--   0 erik      (1000) erik      (1000)      151 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a4/kuksa_certificates/jwt/all-read-write.json
--rw-r--r--   0 erik      (1000) erik      (1000)      875 2022-11-01 08:41:15.000000 kuksa_client-0.4.0a4/kuksa_certificates/jwt/all-read-write.json.token
--rwxr-xr-x   0 erik      (1000) erik      (1000)     1430 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a4/kuksa_certificates/jwt/createToken.py
--rw-r--r--   0 erik      (1000) erik      (1000)     3243 2022-11-01 08:46:13.000000 kuksa_client-0.4.0a4/kuksa_certificates/jwt/jwt.key
--rw-r--r--   0 erik      (1000) erik      (1000)      800 2022-11-01 08:46:13.000000 kuksa_client-0.4.0a4/kuksa_certificates/jwt/jwt.key.pub
--rwxr-xr-x   0 erik      (1000) erik      (1000)      901 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a4/kuksa_certificates/jwt/recreateJWTkeyPair.sh
--rw-r--r--   0 erik      (1000) erik      (1000)       34 2023-05-10 08:02:45.000000 kuksa_client-0.4.0a4/kuksa_certificates/jwt/requirements.txt
--rw-r--r--   0 erik      (1000) erik      (1000)      167 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a4/kuksa_certificates/jwt/single-read.json
--rw-r--r--   0 erik      (1000) erik      (1000)      895 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a4/kuksa_certificates/jwt/single-read.json.token
--rw-r--r--   0 erik      (1000) erik      (1000)      175 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a4/kuksa_certificates/jwt/super-admin.json
--rw-r--r--   0 erik      (1000) erik      (1000)      899 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a4/kuksa_certificates/jwt/super-admin.json.token
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-28 08:56:56.587436 kuksa_client-0.4.0a4/kuksa_client/
--rw-r--r--   0 erik      (1000) erik      (1000)     3929 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a4/kuksa_client/__init__.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)    25603 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a4/kuksa_client/__main__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     1708 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a4/kuksa_client/_metadata.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-28 08:56:56.591435 kuksa_client-0.4.0a4/kuksa_client/cli_backend/
--rw-r--r--   0 erik      (1000) erik      (1000)     2259 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a4/kuksa_client/cli_backend/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)    11695 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a4/kuksa_client/cli_backend/grpc.py
--rw-r--r--   0 erik      (1000) erik      (1000)     9892 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a4/kuksa_client/cli_backend/ws.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-28 08:56:56.591435 kuksa_client-0.4.0a4/kuksa_client/grpc/
--rw-r--r--   0 erik      (1000) erik      (1000)    39035 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a4/kuksa_client/grpc/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)    16627 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a4/kuksa_client/grpc/aio.py
--rw-r--r--   0 erik      (1000) erik      (1000)      385 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a4/kuksa_client/logging.ini
--rw-r--r--   0 erik      (1000) erik      (1000)      605 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a4/kuksa_client/logo
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-28 08:56:56.591435 kuksa_client-0.4.0a4/kuksa_client/ws/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a4/kuksa_client/ws/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-28 08:56:56.591435 kuksa_client-0.4.0a4/kuksa_client.egg-info/
--rw-r--r--   0 erik      (1000) erik      (1000)    13411 2023-06-28 08:56:56.000000 kuksa_client-0.4.0a4/kuksa_client.egg-info/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)     1534 2023-06-28 08:56:56.000000 kuksa_client-0.4.0a4/kuksa_client.egg-info/SOURCES.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-06-28 08:56:56.000000 kuksa_client-0.4.0a4/kuksa_client.egg-info/dependency_links.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       60 2023-06-28 08:56:56.000000 kuksa_client-0.4.0a4/kuksa_client.egg-info/entry_points.txt
--rw-r--r--   0 erik      (1000) erik      (1000)      212 2023-06-28 08:56:56.000000 kuksa_client-0.4.0a4/kuksa_client.egg-info/requires.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       44 2023-06-28 08:56:56.000000 kuksa_client-0.4.0a4/kuksa_client.egg-info/top_level.txt
--rw-r--r--   0 erik      (1000) erik      (1000)      625 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a4/pyproject.toml
--rw-r--r--   0 erik      (1000) erik      (1000)     1370 2023-06-28 08:56:56.591435 kuksa_client-0.4.0a4/setup.cfg
--rw-r--r--   0 erik      (1000) erik      (1000)     1168 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a4/setup.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-28 08:56:56.591435 kuksa_client-0.4.0a4/tests/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a4/tests/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2545 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a4/tests/conftest.py
--rw-r--r--   0 erik      (1000) erik      (1000)    63305 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a4/tests/test_grpc.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.381458 kuksa_client-0.4.0a5/
+-rw-r--r--   0 erik      (1000) erik      (1000)       35 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/MANIFEST.in
+-rw-r--r--   0 erik      (1000) erik      (1000)    15872 2023-07-13 09:08:46.381458 kuksa_client-0.4.0a5/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)    15012 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a5/README.md
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.357469 kuksa_client-0.4.0a5/kuksa/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.357469 kuksa_client-0.4.0a5/kuksa/val/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa/val/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.357469 kuksa_client-0.4.0a5/kuksa/val/v1/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa/val/v1/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     9993 2023-07-13 09:08:46.000000 kuksa_client-0.4.0a5/kuksa/val/v1/types_pb2.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      159 2023-07-13 09:08:46.000000 kuksa_client-0.4.0a5/kuksa/val/v1/types_pb2_grpc.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     4058 2023-07-13 09:08:46.000000 kuksa_client-0.4.0a5/kuksa/val/v1/val_pb2.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     8731 2023-07-13 09:08:46.000000 kuksa_client-0.4.0a5/kuksa/val/v1/val_pb2_grpc.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.365465 kuksa_client-0.4.0a5/kuksa_certificates/
+-rw-r--r--   0 erik      (1000) erik      (1000)     1675 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a5/kuksa_certificates/CA.key
+-rw-r--r--   0 erik      (1000) erik      (1000)     1342 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa_certificates/CA.pem
+-rw-r--r--   0 erik      (1000) erik      (1000)     1679 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a5/kuksa_certificates/Client.key
+-rw-r--r--   0 erik      (1000) erik      (1000)     1704 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a5/kuksa_certificates/Client.pem
+-rw-r--r--   0 erik      (1000) erik      (1000)     3537 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a5/kuksa_certificates/README.md
+-rw-r--r--   0 erik      (1000) erik      (1000)     1679 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a5/kuksa_certificates/Server.key
+-rw-r--r--   0 erik      (1000) erik      (1000)     1704 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a5/kuksa_certificates/Server.pem
+-rw-r--r--   0 erik      (1000) erik      (1000)      114 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa_certificates/__init__.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)     2023 2023-06-28 08:55:35.000000 kuksa_client-0.4.0a5/kuksa_certificates/genCerts.sh
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.373462 kuksa_client-0.4.0a5/kuksa_certificates/jwt/
+-rw-r--r--   0 erik      (1000) erik      (1000)      151 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/all-read-write.json
+-rw-r--r--   0 erik      (1000) erik      (1000)      875 2022-11-01 08:41:15.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/all-read-write.json.token
+-rwxr-xr-x   0 erik      (1000) erik      (1000)     1430 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/createToken.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     3243 2022-11-01 08:46:13.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/jwt.key
+-rw-r--r--   0 erik      (1000) erik      (1000)      800 2022-11-01 08:46:13.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/jwt.key.pub
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      901 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/recreateJWTkeyPair.sh
+-rw-r--r--   0 erik      (1000) erik      (1000)       34 2023-05-10 08:02:45.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/requirements.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)      167 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/single-read.json
+-rw-r--r--   0 erik      (1000) erik      (1000)      895 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/single-read.json.token
+-rw-r--r--   0 erik      (1000) erik      (1000)      175 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/super-admin.json
+-rw-r--r--   0 erik      (1000) erik      (1000)      899 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a5/kuksa_certificates/jwt/super-admin.json.token
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.377460 kuksa_client-0.4.0a5/kuksa_client/
+-rw-r--r--   0 erik      (1000) erik      (1000)     3848 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a5/kuksa_client/__init__.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)    26568 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a5/kuksa_client/__main__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1708 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa_client/_metadata.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.377460 kuksa_client-0.4.0a5/kuksa_client/cli_backend/
+-rw-r--r--   0 erik      (1000) erik      (1000)     2259 2023-06-30 10:33:26.000000 kuksa_client-0.4.0a5/kuksa_client/cli_backend/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    11747 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a5/kuksa_client/cli_backend/grpc.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     9903 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a5/kuksa_client/cli_backend/ws.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.377460 kuksa_client-0.4.0a5/kuksa_client/grpc/
+-rw-r--r--   0 erik      (1000) erik      (1000)    41063 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a5/kuksa_client/grpc/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    16665 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a5/kuksa_client/grpc/aio.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      385 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa_client/logging.ini
+-rw-r--r--   0 erik      (1000) erik      (1000)      605 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa_client/logo
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.377460 kuksa_client-0.4.0a5/kuksa_client/ws/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/kuksa_client/ws/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.377460 kuksa_client-0.4.0a5/kuksa_client.egg-info/
+-rw-r--r--   0 erik      (1000) erik      (1000)    15872 2023-07-13 09:08:46.000000 kuksa_client-0.4.0a5/kuksa_client.egg-info/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)     1558 2023-07-13 09:08:46.000000 kuksa_client-0.4.0a5/kuksa_client.egg-info/SOURCES.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-07-13 09:08:46.000000 kuksa_client-0.4.0a5/kuksa_client.egg-info/dependency_links.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       60 2023-07-13 09:08:46.000000 kuksa_client-0.4.0a5/kuksa_client.egg-info/entry_points.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)      212 2023-07-13 09:08:46.000000 kuksa_client-0.4.0a5/kuksa_client.egg-info/requires.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       44 2023-07-13 09:08:46.000000 kuksa_client-0.4.0a5/kuksa_client.egg-info/top_level.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)      625 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/pyproject.toml
+-rw-r--r--   0 erik      (1000) erik      (1000)     1370 2023-07-13 09:08:46.381458 kuksa_client-0.4.0a5/setup.cfg
+-rw-r--r--   0 erik      (1000) erik      (1000)     1768 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a5/setup.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-07-13 09:08:46.381458 kuksa_client-0.4.0a5/tests/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a5/tests/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2545 2023-06-30 09:22:49.000000 kuksa_client-0.4.0a5/tests/conftest.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     5949 2023-07-13 09:03:55.000000 kuksa_client-0.4.0a5/tests/test_datapoint.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    63305 2023-06-30 09:22:49.000000 kuksa_client-0.4.0a5/tests/test_grpc.py
```

### Comparing `kuksa_client-0.4.0a4/PKG-INFO` & `kuksa_client-0.4.0a5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuksa_client
-Version: 0.4.0a4
+Version: 0.4.0a5
 Summary: kuksa.val python clients and SDK
 Home-page: https://github.com/eclipse/kuksa.val
 Author: Sebastian Schildt, Naresh Nayak, Wenwen Chen
 Author-email: sebastian.schildt@de.bosch.com, naresh.nayak@de.bosch.com, wenwen.chen@de.bosch.com
 Project-URL: Source, https://github.com/eclipse/kuksa.val/tree/master/kuksa-client
 Project-URL: Bug Tracker, https://github.com/eclipse/kuksa.val/issues
 Classifier: Intended Audience :: Developers
@@ -198,14 +198,87 @@
 
 ```
 
 This is an example showing how some of the commands can be used:
 
 ![try kuksa-client out](https://raw.githubusercontent.com/eclipse/kuksa.val/master/doc/pictures/testclient_basic.gif "test client usage")
 
+### Syntax for specifying data in the command line interface
+
+Values used as argument to for example `setValue` shall match the type given. Quotes (single and double) are 
+generally not needed, except in a few special cases. A few valid examples on setting float is shown below:
+
+```
+setValue Vehicle.Speed 43
+setValue Vehicle.Speed "45"
+setValue Vehicle.Speed '45.2'
+```
+
+For strings escaped quotes are needed if you want quotes to be sent to Server/Databroker, like if you want to store
+`Almost "red"` as value. Alternatively you can use outer single quotes and inner double quotes.
+
+The two examples below are equal:
+
+```
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect 'Almost \"red\"'
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect 'Almost "red"'
+```
+
+Alternatively you can use inner single quotes, but then the value will be represented by double quotes (`Almost "blue"`)
+when stored anyhow.
+
+```
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect "Almost 'blue'"
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect "Almost \'blue\'"
+```
+
+If not using outer quotes the inner quotes will be lost, the examples below are equal.
+Leading/trialing spaces are ignored.
+
+```
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect Almost 'green'
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect Almost green
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect 'Almost green'
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect "Almost green"
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect 'Almost green         '
+```
+
+
+It is possible to set array values. Setting a string array with simple identifiers is not a problem. Also not if they
+contain blanks
+
+```
+// Array with two elements
+setValue Vehicle.OBD.DTCList [abc,def]
+// Array with two elements, "hello there" and "def"
+setValue Vehicle.OBD.DTCList [hello there,def]
+```
+
+Setting values that includes comma or quotation marks is more tricky, as the shell argument parser handling affects
+how they are interpreted. The recommended approach is to have outer quotes of one type and user inner quotes of the
+other type.
+
+Example 1: First item should be `hello, there`
+
+```
+setValue Vehicle.OBD.DTCList '[ "hello, there",def]'
+```
+
+Example 2: First item should be `hello, "there"`
+
+```
+setValue Vehicle.OBD.DTCList '["hello, \"there\"",def]'
+```
+
+Example 3: First item should be `hello, 'there'`
+
+```
+setValue Vehicle.OBD.DTCList "['hello, \'there\'',def]"
+```
+
 ### Updating VSS Structure
 
 Using the test client, it is also possible to update and extend the VSS data structure.
 More details can be found [here](https://github.com/eclipse/kuksa.val/blob/master/doc/KUKSA.val_server/liveUpdateVSSTree.md).
 
 **Note**: You can also use `setValue` to change the value of an array, but the value should not contains any non-quoted spaces. Consider the following examples:
```

### Comparing `kuksa_client-0.4.0a4/README.md` & `kuksa_client-0.4.0a5/kuksa_client.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: kuksa-client
+Version: 0.4.0a5
+Summary: kuksa.val python clients and SDK
+Home-page: https://github.com/eclipse/kuksa.val
+Author: Sebastian Schildt, Naresh Nayak, Wenwen Chen
+Author-email: sebastian.schildt@de.bosch.com, naresh.nayak@de.bosch.com, wenwen.chen@de.bosch.com
+Project-URL: Source, https://github.com/eclipse/kuksa.val/tree/master/kuksa-client
+Project-URL: Bug Tracker, https://github.com/eclipse/kuksa.val/issues
+Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: test
+
 # KUKSA.val Client
 ![kuksa.val Logo](https://raw.githubusercontent.com/eclipse/kuksa.val/0.2.5/doc/pictures/logo.png)
 
 `kuksa.val` is a part of the opensource project [Eclipse Kuksa](https://www.eclipse.org/kuksa/).
 More about `kuksa.val` can be found in the [repository](https://github.com/eclipse/kuksa.val).
 
 ## Introduction
@@ -178,14 +198,87 @@
 
 ```
 
 This is an example showing how some of the commands can be used:
 
 ![try kuksa-client out](https://raw.githubusercontent.com/eclipse/kuksa.val/master/doc/pictures/testclient_basic.gif "test client usage")
 
+### Syntax for specifying data in the command line interface
+
+Values used as argument to for example `setValue` shall match the type given. Quotes (single and double) are 
+generally not needed, except in a few special cases. A few valid examples on setting float is shown below:
+
+```
+setValue Vehicle.Speed 43
+setValue Vehicle.Speed "45"
+setValue Vehicle.Speed '45.2'
+```
+
+For strings escaped quotes are needed if you want quotes to be sent to Server/Databroker, like if you want to store
+`Almost "red"` as value. Alternatively you can use outer single quotes and inner double quotes.
+
+The two examples below are equal:
+
+```
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect 'Almost \"red\"'
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect 'Almost "red"'
+```
+
+Alternatively you can use inner single quotes, but then the value will be represented by double quotes (`Almost "blue"`)
+when stored anyhow.
+
+```
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect "Almost 'blue'"
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect "Almost \'blue\'"
+```
+
+If not using outer quotes the inner quotes will be lost, the examples below are equal.
+Leading/trialing spaces are ignored.
+
+```
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect Almost 'green'
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect Almost green
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect 'Almost green'
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect "Almost green"
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect 'Almost green         '
+```
+
+
+It is possible to set array values. Setting a string array with simple identifiers is not a problem. Also not if they
+contain blanks
+
+```
+// Array with two elements
+setValue Vehicle.OBD.DTCList [abc,def]
+// Array with two elements, "hello there" and "def"
+setValue Vehicle.OBD.DTCList [hello there,def]
+```
+
+Setting values that includes comma or quotation marks is more tricky, as the shell argument parser handling affects
+how they are interpreted. The recommended approach is to have outer quotes of one type and user inner quotes of the
+other type.
+
+Example 1: First item should be `hello, there`
+
+```
+setValue Vehicle.OBD.DTCList '[ "hello, there",def]'
+```
+
+Example 2: First item should be `hello, "there"`
+
+```
+setValue Vehicle.OBD.DTCList '["hello, \"there\"",def]'
+```
+
+Example 3: First item should be `hello, 'there'`
+
+```
+setValue Vehicle.OBD.DTCList "['hello, \'there\'',def]"
+```
+
 ### Updating VSS Structure
 
 Using the test client, it is also possible to update and extend the VSS data structure.
 More details can be found [here](https://github.com/eclipse/kuksa.val/blob/master/doc/KUKSA.val_server/liveUpdateVSSTree.md).
 
 **Note**: You can also use `setValue` to change the value of an array, but the value should not contains any non-quoted spaces. Consider the following examples:
```

### Comparing `kuksa_client-0.4.0a4/kuksa/val/v1/types_pb2.py` & `kuksa_client-0.4.0a5/kuksa/val/v1/types_pb2.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa/val/v1/val_pb2.py` & `kuksa_client-0.4.0a5/kuksa/val/v1/val_pb2.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa/val/v1/val_pb2_grpc.py` & `kuksa_client-0.4.0a5/kuksa/val/v1/val_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa_certificates/CA.key` & `kuksa_client-0.4.0a5/kuksa_certificates/CA.key`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa_certificates/CA.pem` & `kuksa_client-0.4.0a5/kuksa_certificates/CA.pem`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa_certificates/Client.key` & `kuksa_client-0.4.0a5/kuksa_certificates/Client.key`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa_certificates/Client.pem` & `kuksa_client-0.4.0a5/kuksa_certificates/Client.pem`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa_certificates/README.md` & `kuksa_client-0.4.0a5/kuksa_certificates/README.md`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa_certificates/Server.key` & `kuksa_client-0.4.0a5/kuksa_certificates/Server.key`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa_certificates/Server.pem` & `kuksa_client-0.4.0a5/kuksa_certificates/Server.pem`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa_certificates/genCerts.sh` & `kuksa_client-0.4.0a5/kuksa_certificates/genCerts.sh`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa_certificates/jwt/all-read-write.json.token` & `kuksa_client-0.4.0a5/kuksa_certificates/jwt/all-read-write.json.token`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa_certificates/jwt/createToken.py` & `kuksa_client-0.4.0a5/kuksa_certificates/jwt/createToken.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa_certificates/jwt/jwt.key` & `kuksa_client-0.4.0a5/kuksa_certificates/jwt/jwt.key`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa_certificates/jwt/jwt.key.pub` & `kuksa_client-0.4.0a5/kuksa_certificates/jwt/jwt.key.pub`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa_certificates/jwt/recreateJWTkeyPair.sh` & `kuksa_client-0.4.0a5/kuksa_certificates/jwt/recreateJWTkeyPair.sh`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa_certificates/jwt/single-read.json.token` & `kuksa_client-0.4.0a5/kuksa_certificates/jwt/single-read.json.token`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa_certificates/jwt/super-admin.json.token` & `kuksa_client-0.4.0a5/kuksa_certificates/jwt/super-admin.json.token`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa_client/__init__.py` & `kuksa_client-0.4.0a5/kuksa_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 ########################################################################
 
 import asyncio
-import json
-import os
-import queue
-import ssl
-import sys
 import threading
-import time
 from typing import Any
 from typing import Dict
 from typing import Iterable
-import uuid
-
-from kuksa_client._metadata import *
+from typing import Optional
 
 from . import cli_backend
 
 
 class KuksaClientThread(threading.Thread):
 
     # Constructor
@@ -48,15 +40,15 @@
     def checkConnection(self):
         return self.backend.checkConnection()
 
     def stop(self):
         self.backend.stop()
 
     # Do authorization by passing a jwt token or a token file
-    def authorize(self, token_or_tokenfile: str=None, timeout=5):
+    def authorize(self, token_or_tokenfile: Optional[str]=None, timeout=5):
         return self.backend.authorize(token_or_tokenfile, timeout)
 
     # Update VSS Tree Entry
     def updateVSSTree(self, jsonStr: str, timeout=5):
         return self.backend.updateVSSTree(jsonStr, timeout)
 
     # Update Meta Data of a given path
```

### Comparing `kuksa_client-0.4.0a4/kuksa_client/__main__.py` & `kuksa_client-0.4.0a5/kuksa_client/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -297,14 +297,28 @@
                     formatters.TerminalFormatter()))
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_setValue)
     def do_setValue(self, args):
         """Set the value of a path"""
         if self.checkConnection():
+            # If there is a blank before a single/double quote on the kuksa-client cli then
+            # the argparser shell will remove it, there is nothing we can do to it
+            # This gives off behavior for examples like:
+            # setValue Vehicle.OBD.DTCList [ "dtc1, dtc2", ddd]
+            # which will be treated as input of 3 elements
+            # The recommended approach is to have quotes (of a different type) around the whole value
+            # if your strings includes quotes, commas or other items
+            # setValue Vehicle.OBD.DTCList '[ "dtc1, dtc2", ddd]'
+            # or
+            # setValue Vehicle.OBD.DTCList "[ 'dtc1, dtc2', ddd]"
+            # If you really need to include a quote in the values use backslash and use the quote type
+            # you want as inner value:
+            # setValue Vehicle.OBD.DTCList "[ 'dtc1, \'dtc2', ddd]"
+            # Will result in two elements in the array; "dtc1, 'dtc2" and "ddd"
             value = str(' '.join(args.Value))
             resp = self.commThread.setValue(
                 args.Path, value, args.attribute)
             print(highlight(resp, lexers.JsonLexer(),
                   formatters.TerminalFormatter()))
         self.pathCompletionItems = []
```

### Comparing `kuksa_client-0.4.0a4/kuksa_client/_metadata.py` & `kuksa_client-0.4.0a5/kuksa_client/_metadata.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa_client/cli_backend/__init__.py` & `kuksa_client-0.4.0a5/kuksa_client/cli_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa_client/cli_backend/grpc.py` & `kuksa_client-0.4.0a5/kuksa_client/cli_backend/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import json
 import pathlib
 import queue
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Iterable
+from typing import Optional
 import uuid
 import os
 import re
 
 from kuksa_client import cli_backend
 import kuksa_client.grpc
 import kuksa_client.grpc.aio
@@ -140,20 +141,20 @@
                 entry_updates.append(kuksa_client.grpc.EntryUpdate(
                     entry=entry, fields=(field,)))
             requestArgs = {'updates': entry_updates}
             return self._sendReceiveMsg(("set", requestArgs), timeout)
         return json.dumps({"error": "Invalid Attribute"})
 
     # Function for authorization
-    def authorize(self, token_or_tokenfile:str =None, timeout=5):
+    def authorize(self, token_or_tokenfile:Optional[str] =None, timeout=5):
         if token_or_tokenfile is None:
             token_or_tokenfile = self.token_or_tokenfile
         if os.path.isfile(token_or_tokenfile):
-            token_or_tokenfile = pathlib.Path(token_or_tokenfile)
-            token = token_or_tokenfile.expanduser().read_text(encoding='utf-8').rstrip('\n')
+            token_or_tokenfile_path = pathlib.Path(token_or_tokenfile)
+            token = token_or_tokenfile_path.expanduser().read_text(encoding='utf-8').rstrip('\n')
         else:
             token = token_or_tokenfile
         requestArgs = {
             'token': token
         }
 
         return self._sendReceiveMsg(("authorize", requestArgs), timeout)
@@ -174,20 +175,20 @@
             }
             return self._sendReceiveMsg(("subscribe", requestArgs), timeout)
 
         return json.dumps({"error": "Invalid Attribute"})
 
     # Unsubscribe value changes of to a given path.
     # The subscription id from the response of the corresponding subscription request will be required
-    def unsubscribe(self, sub_id: int, timeout=5):
+    def unsubscribe(self, sub_id: str, timeout=5):
         try:
-            sub_id = uuid.UUID(sub_id)
+            sub_uuid = uuid.UUID(sub_id)
         except ValueError as exc:
             return json.dumps({"error": str(exc)})
-        requestArgs = {'subscription_id': sub_id}
+        requestArgs = {'subscription_id': sub_uuid}
         return self._sendReceiveMsg(("unsubscribe", requestArgs), timeout)
 
     def connect(self, timeout=5):
         requestArgs = {}
         return self._sendReceiveMsg(("connect", requestArgs), timeout)
 
     def disconnect(self, timeout=5):
```

### Comparing `kuksa_client-0.4.0a4/kuksa_client/cli_backend/ws.py` & `kuksa_client-0.4.0a5/kuksa_client/cli_backend/ws.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
     # Function to stop the communication
     def stop(self):
         self.wsConnected = False
         self.run = False
         print("Server disconnected.")
 
-    def disconnect(self):
+    def disconnect(self, _):
         self.stop()
 
     # Function to authorize against the kuksa.val server
     def authorize(self, token_or_tokenfile=None, timeout=2):
         if token_or_tokenfile is None:
             token_or_tokenfile = self.token_or_tokenfile
         if os.path.isfile(token_or_tokenfile):
@@ -224,15 +224,15 @@
 
         return res
 
     # Function to check connection
     def checkConnection(self):
         return self.wsConnected
 
-    async def connect(self):
+    async def connect(self, _=None):
         if not self.insecure:
             context = ssl.create_default_context()
             context.load_cert_chain(
                 certfile=self.certificate, keyfile=self.keyfile)
             context.load_verify_locations(cafile=self.cacertificate)
             # We want host name to match
             # For example certificates we use subjectAltName to make it match for Server, localahost and 127.0.0.1
```

### Comparing `kuksa_client-0.4.0a4/kuksa_client/grpc/__init__.py` & `kuksa_client-0.4.0a5/kuksa_client/grpc/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -311,69 +311,111 @@
         return cls(
             value=getattr(message, message.WhichOneof('value')),
             timestamp=message.timestamp.ToDatetime(
                 tzinfo=datetime.timezone.utc,
             ) if message.HasField('timestamp') else None,
         )
 
+
+    def cast_array_values(cast, array):
+        """
+        Parses array input and cast individual values to wanted type.
+        Note that input value to this function is not the same as given if you use kuksa-client command line
+        as parts (e.g. surrounding quotes) are removed by shell, and then do_setValue also do some magic.
+        """
+        array = array.strip('[]')
+
+        # Split the input string into separate values
+        # First alternative, not quotes including escaped single or double quote, ends at comma, whitespace or EOL
+        # Second group is double quoted string, may contain quoted strings and single quotes inside, ends at non-escaped
+        # double quote
+        # Third is similar but for single quote
+        # Using raw strings with surrounding single/double quotes to minimize need for escapes
+        pattern = r'(?:\\"|\\' + \
+                  r"'|[^'" + r'",])+|"(?:\\"|[^"])*"|' + \
+                  r"'(?:\\'|[^'])*'"
+        values = re.findall(pattern, array)
+        for item in values:
+            # We may in some cases match blanks, that is intended as we want to be able to write arguments like
+            # My Way
+            # ... without quotes
+            if item.strip() == '':
+                #skip
+                pass
+            else:
+                yield cast(item)
+
+    def cast_bool(value) -> bool:
+        if value in ('False', 'false', 'F', 'f'):
+            value = 0
+        return bool(value)
+
+    def cast_str(value) -> str:
+        """
+        Strip based on the following rules.
+        - Leading/Trailing blanks are removed
+        - If there are single or double quote at both start and end they are removed
+        - Finally any quote escapes are removed
+        """
+        new_val = value.strip()
+        if new_val.startswith('"') and new_val.endswith('"'):
+            new_val = new_val[1:-1]
+        if new_val.startswith("'") and new_val.endswith("'"):
+            new_val = new_val[1:-1]
+        # Replace escaped quotes with normal quotes
+        new_val = new_val.replace('\\\"', '\"')
+        new_val = new_val.replace("\\\'", "\'")
+        return new_val
+            
     def to_message(self, value_type: DataType) -> types_pb2.Datapoint:
         message = types_pb2.Datapoint()
 
         def set_array_attr(obj, attr, values):
             array = getattr(obj, attr)
             array.Clear()
             array.values.extend(values)
 
-        def cast_array_values(cast, array):
-            array = array.strip('[]')
-            pattern = r'(?:\\.|[^",])*"(?:\\.|[^"])*"|[^",]+'
-            values = re.findall(pattern, array)
-            for item in values:
-                if item == '':
-                    #skip
-                    pass
-                else:
-                    if cast == str:
-                        item = item.replace('\"', '').replace('\\', '"').strip()
-                    yield cast(item)
-
-        def cast_bool(value):
-            if value in ('False', 'false', 'F', 'f'):
-                value = 0
-            return bool(value)
-        
-        def cast_str(value):
-            return str(value).replace('\"', '').replace('\\', '"').strip()
-            
 
         field, set_field, cast_field = {
             DataType.INT8: ('int32', setattr, int),
             DataType.INT16: ('int32', setattr, int),
             DataType.INT32: ('int32', setattr, int),
             DataType.UINT8: ('uint32', setattr, int),
             DataType.UINT16: ('uint32', setattr, int),
             DataType.UINT32: ('uint32', setattr, int),
             DataType.UINT64: ('uint64', setattr, int),
             DataType.INT64: ('int64', setattr, int),
             DataType.FLOAT: ('float', setattr, float),
             DataType.DOUBLE: ('double', setattr, float),
-            DataType.BOOLEAN: ('bool', setattr, cast_bool),
-            DataType.STRING: ('string', setattr, cast_str),
-            DataType.INT8_ARRAY: ('int32_array', set_array_attr, lambda array: cast_array_values(int, array)),
-            DataType.INT16_ARRAY: ('int32_array', set_array_attr, lambda array: cast_array_values(int, array)),
-            DataType.INT32_ARRAY: ('int32_array', set_array_attr, lambda array: cast_array_values(int, array)),
-            DataType.UINT8_ARRAY: ('uint32_array', set_array_attr, lambda array: cast_array_values(int, array)),
-            DataType.UINT16_ARRAY: ('uint32_array', set_array_attr, lambda array: cast_array_values(int, array)),
-            DataType.UINT32_ARRAY: ('uint32_array', set_array_attr, lambda array: cast_array_values(int, array)),
-            DataType.UINT64_ARRAY: ('uint64_array', set_array_attr, lambda array: cast_array_values(int, array)),
-            DataType.INT64_ARRAY: ('int64_array', set_array_attr, lambda array: cast_array_values(int, array)),
-            DataType.FLOAT_ARRAY: ('float_array', set_array_attr, lambda array: cast_array_values(float, array)),
-            DataType.DOUBLE_ARRAY: ('double_array', set_array_attr, lambda array: cast_array_values(float, array)),
-            DataType.BOOLEAN_ARRAY: ('bool_array', set_array_attr, lambda array: cast_array_values(cast_bool, array)),
-            DataType.STRING_ARRAY: ('string_array', set_array_attr, lambda array: cast_array_values(str, array)),
+            DataType.BOOLEAN: ('bool', setattr, Datapoint.cast_bool),
+            DataType.STRING: ('string', setattr, Datapoint.cast_str),
+            DataType.INT8_ARRAY: ('int32_array', set_array_attr, 
+                                  lambda array: Datapoint.cast_array_values(int, array)),
+            DataType.INT16_ARRAY: ('int32_array', set_array_attr, 
+                                   lambda array: Datapoint.cast_array_values(int, array)),
+            DataType.INT32_ARRAY: ('int32_array', set_array_attr, 
+                                   lambda array: Datapoint.cast_array_values(int, array)),
+            DataType.UINT8_ARRAY: ('uint32_array', set_array_attr, 
+                                   lambda array: Datapoint.cast_array_values(int, array)),
+            DataType.UINT16_ARRAY: ('uint32_array', set_array_attr, 
+                                    lambda array: Datapoint.cast_array_values(int, array)),
+            DataType.UINT32_ARRAY: ('uint32_array', set_array_attr, 
+                                    lambda array: Datapoint.cast_array_values(int, array)),
+            DataType.UINT64_ARRAY: ('uint64_array', set_array_attr, 
+                                    lambda array: Datapoint.cast_array_values(int, array)),
+            DataType.INT64_ARRAY: ('int64_array', set_array_attr, 
+                                   lambda array: Datapoint.cast_array_values(int, array)),
+            DataType.FLOAT_ARRAY: ('float_array', set_array_attr, 
+                                   lambda array: Datapoint.cast_array_values(float, array)),
+            DataType.DOUBLE_ARRAY: ('double_array', set_array_attr, 
+                                    lambda array: Datapoint.cast_array_values(float, array)),
+            DataType.BOOLEAN_ARRAY: ('bool_array', set_array_attr, 
+                                     lambda array: Datapoint.cast_array_values(Datapoint.cast_bool, array)),
+            DataType.STRING_ARRAY: ('string_array', set_array_attr, 
+                                    lambda array: Datapoint.cast_array_values(Datapoint.cast_str, array)),
         }.get(value_type, (None, None, None))
         if self.value is not None:
             if all((field, set_field, cast_field)):
                 set_field(message, field, cast_field(self.value))
             else:
                 # Either DataType.TIMESTAMP, DataType.TIMESTAMP_ARRAY or DataType.UNSPECIFIED...
                 raise ValueError(
@@ -907,15 +949,15 @@
         except RpcError as exc:
             raise VSSClientError.from_grpc_error(exc) from exc
         logger.debug("%s: %s", type(resp).__name__, resp)
         self.authorization_header = self.get_authorization_header(token)
         return "Authenticated"
 
     @check_connected
-    def get_server_info(self, **rpc_kwargs) -> ServerInfo:
+    def get_server_info(self, **rpc_kwargs) -> Optional[ServerInfo]:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         """
         rpc_kwargs["metadata"] = self.generate_metadata_header(
             metadata=rpc_kwargs.get("metadata"))
```

### Comparing `kuksa_client-0.4.0a4/kuksa_client/grpc/aio.py` & `kuksa_client-0.4.0a5/kuksa_client/grpc/aio.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import logging
 from typing import AsyncIterator
 from typing import Callable
 from typing import Collection
 from typing import Dict
 from typing import Iterable
 from typing import List
+from typing import Optional
 import uuid
 
 import grpc
 from grpc.aio import AioRpcError
 
 from kuksa.val.v1 import val_pb2
 from kuksa.val.v1 import val_pb2_grpc
@@ -341,15 +342,15 @@
         except AioRpcError as exc:
             raise VSSClientError.from_grpc_error(exc) from exc
         logger.debug("%s: %s", type(resp).__name__, resp)
         self.authorization_header = self.get_authorization_header(token)
         return "Authenticated"
 
     @check_connected_async
-    async def get_server_info(self, **rpc_kwargs) -> ServerInfo:
+    async def get_server_info(self, **rpc_kwargs) -> Optional[ServerInfo]:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         """
         rpc_kwargs["metadata"] = self.generate_metadata_header(
             metadata=rpc_kwargs.get("metadata"))
```

### Comparing `kuksa_client-0.4.0a4/kuksa_client/logo` & `kuksa_client-0.4.0a5/kuksa_client/logo`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/kuksa_client.egg-info/PKG-INFO` & `kuksa_client-0.4.0a5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: kuksa-client
-Version: 0.4.0a4
-Summary: kuksa.val python clients and SDK
-Home-page: https://github.com/eclipse/kuksa.val
-Author: Sebastian Schildt, Naresh Nayak, Wenwen Chen
-Author-email: sebastian.schildt@de.bosch.com, naresh.nayak@de.bosch.com, wenwen.chen@de.bosch.com
-Project-URL: Source, https://github.com/eclipse/kuksa.val/tree/master/kuksa-client
-Project-URL: Bug Tracker, https://github.com/eclipse/kuksa.val/issues
-Classifier: Intended Audience :: Developers
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-
 # KUKSA.val Client
 ![kuksa.val Logo](https://raw.githubusercontent.com/eclipse/kuksa.val/0.2.5/doc/pictures/logo.png)
 
 `kuksa.val` is a part of the opensource project [Eclipse Kuksa](https://www.eclipse.org/kuksa/).
 More about `kuksa.val` can be found in the [repository](https://github.com/eclipse/kuksa.val).
 
 ## Introduction
@@ -198,14 +178,87 @@
 
 ```
 
 This is an example showing how some of the commands can be used:
 
 ![try kuksa-client out](https://raw.githubusercontent.com/eclipse/kuksa.val/master/doc/pictures/testclient_basic.gif "test client usage")
 
+### Syntax for specifying data in the command line interface
+
+Values used as argument to for example `setValue` shall match the type given. Quotes (single and double) are 
+generally not needed, except in a few special cases. A few valid examples on setting float is shown below:
+
+```
+setValue Vehicle.Speed 43
+setValue Vehicle.Speed "45"
+setValue Vehicle.Speed '45.2'
+```
+
+For strings escaped quotes are needed if you want quotes to be sent to Server/Databroker, like if you want to store
+`Almost "red"` as value. Alternatively you can use outer single quotes and inner double quotes.
+
+The two examples below are equal:
+
+```
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect 'Almost \"red\"'
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect 'Almost "red"'
+```
+
+Alternatively you can use inner single quotes, but then the value will be represented by double quotes (`Almost "blue"`)
+when stored anyhow.
+
+```
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect "Almost 'blue'"
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect "Almost \'blue\'"
+```
+
+If not using outer quotes the inner quotes will be lost, the examples below are equal.
+Leading/trialing spaces are ignored.
+
+```
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect Almost 'green'
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect Almost green
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect 'Almost green'
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect "Almost green"
+setValue Vehicle.Cabin.Light.InteractiveLightBar.Effect 'Almost green         '
+```
+
+
+It is possible to set array values. Setting a string array with simple identifiers is not a problem. Also not if they
+contain blanks
+
+```
+// Array with two elements
+setValue Vehicle.OBD.DTCList [abc,def]
+// Array with two elements, "hello there" and "def"
+setValue Vehicle.OBD.DTCList [hello there,def]
+```
+
+Setting values that includes comma or quotation marks is more tricky, as the shell argument parser handling affects
+how they are interpreted. The recommended approach is to have outer quotes of one type and user inner quotes of the
+other type.
+
+Example 1: First item should be `hello, there`
+
+```
+setValue Vehicle.OBD.DTCList '[ "hello, there",def]'
+```
+
+Example 2: First item should be `hello, "there"`
+
+```
+setValue Vehicle.OBD.DTCList '["hello, \"there\"",def]'
+```
+
+Example 3: First item should be `hello, 'there'`
+
+```
+setValue Vehicle.OBD.DTCList "['hello, \'there\'',def]"
+```
+
 ### Updating VSS Structure
 
 Using the test client, it is also possible to update and extend the VSS data structure.
 More details can be found [here](https://github.com/eclipse/kuksa.val/blob/master/doc/KUKSA.val_server/liveUpdateVSSTree.md).
 
 **Note**: You can also use `setValue` to change the value of an array, but the value should not contains any non-quoted spaces. Consider the following examples:
```

### Comparing `kuksa_client-0.4.0a4/kuksa_client.egg-info/SOURCES.txt` & `kuksa_client-0.4.0a5/kuksa_client.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -46,8 +46,9 @@
 kuksa_client/cli_backend/grpc.py
 kuksa_client/cli_backend/ws.py
 kuksa_client/grpc/__init__.py
 kuksa_client/grpc/aio.py
 kuksa_client/ws/__init__.py
 tests/__init__.py
 tests/conftest.py
+tests/test_datapoint.py
 tests/test_grpc.py
```

### Comparing `kuksa_client-0.4.0a4/pyproject.toml` & `kuksa_client-0.4.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/setup.cfg` & `kuksa_client-0.4.0a5/setup.cfg`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/tests/conftest.py` & `kuksa_client-0.4.0a5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a4/tests/test_grpc.py` & `kuksa_client-0.4.0a5/tests/test_grpc.py`

 * *Files identical despite different names*

