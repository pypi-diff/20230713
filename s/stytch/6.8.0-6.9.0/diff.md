# Comparing `tmp/stytch-6.8.0.tar.gz` & `tmp/stytch-6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stytch-6.8.0.tar", last modified: Thu Apr 27 15:23:04 2023, max compression
+gzip compressed data, was "stytch-6.9.0.tar", last modified: Wed May 31 19:24:08 2023, max compression
```

## Comparing `stytch-6.8.0.tar` & `stytch-6.9.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.458717 stytch-6.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-27 15:22:27.000000 stytch-6.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-27 15:23:04.458717 stytch-6.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-27 15:22:27.000000 stytch-6.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 15:23:04.458717 stytch-6.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-27 15:22:27.000000 stytch-6.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.446716 stytch-6.8.0/stytch/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.450716 stytch-6.8.0/stytch/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    28137 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/otp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)    17096 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    13713 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/totps.py
--rw-r--r--   0 runner    (1001) docker     (123)    24338 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/users.py
--rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/api/webauthn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.450716 stytch-6.8.0/stytch/b2b/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.454716 stytch-6.8.0/stytch/b2b/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/discovery_intermediate_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/discovery_organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/magic_links_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    16357 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/magic_links_email_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    49021 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)    17130 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.454716 stytch-6.8.0/stytch/b2b/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.454716 stytch-6.8.0/stytch/b2b/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/discovery_intermediate_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/discovery_organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/magic_links_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/magic_links_email_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/b2b/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.454716 stytch-6.8.0/stytch/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/core/api_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.454716 stytch-6.8.0/stytch/core/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/core/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/core/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.458717 stytch-6.8.0/stytch/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/crypto_wallets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/magic_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/magic_links_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/otp.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/otp_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/otp_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/otp_whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/passwords_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/passwords_existing_password.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/passwords_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/totps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/models/webauthn.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 15:22:27.000000 stytch-6.8.0/stytch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.450716 stytch-6.8.0/stytch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-27 15:23:04.000000 stytch-6.8.0/stytch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-27 15:23:04.000000 stytch-6.8.0/stytch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:23:04.000000 stytch-6.8.0/stytch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 15:23:04.000000 stytch-6.8.0/stytch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 15:23:04.000000 stytch-6.8.0/stytch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:23:04.458717 stytch-6.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-04-27 15:22:27.000000 stytch-6.8.0/test/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-04-27 15:22:27.000000 stytch-6.8.0/test/test_integration_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.179835 stytch-6.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-31 19:23:52.000000 stytch-6.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-31 19:24:08.179835 stytch-6.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-31 19:23:52.000000 stytch-6.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-31 19:24:08.179835 stytch-6.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-31 19:23:52.000000 stytch-6.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.171835 stytch-6.9.0/stytch/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.175835 stytch-6.9.0/stytch/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28137 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17096 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13713 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/totps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24338 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/api/webauthn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.175835 stytch-6.9.0/stytch/b2b/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.175835 stytch-6.9.0/stytch/b2b/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16357 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49021 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17130 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.175835 stytch-6.9.0/stytch/b2b/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.175835 stytch-6.9.0/stytch/b2b/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/b2b/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.179835 stytch-6.9.0/stytch/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/core/api_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.179835 stytch-6.9.0/stytch/core/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/core/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/core/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.179835 stytch-6.9.0/stytch/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/totps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/models/webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 19:23:52.000000 stytch-6.9.0/stytch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.171835 stytch-6.9.0/stytch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-31 19:24:08.000000 stytch-6.9.0/stytch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-31 19:24:08.000000 stytch-6.9.0/stytch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:24:08.000000 stytch-6.9.0/stytch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-31 19:24:08.000000 stytch-6.9.0/stytch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 19:24:08.000000 stytch-6.9.0/stytch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:24:08.179835 stytch-6.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-05-31 19:23:52.000000 stytch-6.9.0/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-05-31 19:23:52.000000 stytch-6.9.0/test/test_integration_async.py
```

### Comparing `stytch-6.8.0/LICENSE.txt` & `stytch-6.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/PKG-INFO` & `stytch-6.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 6.8.0
+Version: 6.9.0
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-6.8.0/README.md` & `stytch-6.9.0/README.md`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/setup.py` & `stytch-6.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/api/crypto_wallets.py` & `stytch-6.9.0/stytch/api/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/api/magic_links.py` & `stytch-6.9.0/stytch/api/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/api/magic_links_email.py` & `stytch-6.9.0/stytch/api/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/api/oauth.py` & `stytch-6.9.0/stytch/api/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/api/otp.py` & `stytch-6.9.0/stytch/api/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/api/otp_email.py` & `stytch-6.9.0/stytch/api/otp_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/api/otp_sms.py` & `stytch-6.9.0/stytch/api/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/api/otp_whatsapp.py` & `stytch-6.9.0/stytch/api/otp_whatsapp.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/api/passwords.py` & `stytch-6.9.0/stytch/api/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/api/passwords_email.py` & `stytch-6.9.0/stytch/api/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/api/passwords_existing_password.py` & `stytch-6.9.0/stytch/api/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/api/passwords_session.py` & `stytch-6.9.0/stytch/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/api/sessions.py` & `stytch-6.9.0/stytch/api/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/api/totps.py` & `stytch-6.9.0/stytch/api/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/api/users.py` & `stytch-6.9.0/stytch/api/users.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/api/webauthn.py` & `stytch-6.9.0/stytch/api/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/api/discovery.py` & `stytch-6.9.0/stytch/b2b/api/discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/api/discovery_intermediate_sessions.py` & `stytch-6.9.0/stytch/b2b/api/discovery_intermediate_sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/api/discovery_organizations.py` & `stytch-6.9.0/stytch/b2b/api/discovery_organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/api/magic_links.py` & `stytch-6.9.0/stytch/b2b/api/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/api/magic_links_discovery.py` & `stytch-6.9.0/stytch/b2b/api/magic_links_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/api/magic_links_email.py` & `stytch-6.9.0/stytch/b2b/api/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/api/magic_links_email_discovery.py` & `stytch-6.9.0/stytch/b2b/api/magic_links_email_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/api/organizations.py` & `stytch-6.9.0/stytch/b2b/api/organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/api/passwords.py` & `stytch-6.9.0/stytch/b2b/api/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/api/passwords_email.py` & `stytch-6.9.0/stytch/b2b/api/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/api/passwords_existing_password.py` & `stytch-6.9.0/stytch/b2b/api/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/api/passwords_session.py` & `stytch-6.9.0/stytch/b2b/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/api/sessions.py` & `stytch-6.9.0/stytch/b2b/api/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/client.py` & `stytch-6.9.0/stytch/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,73 @@
 #!/usr/bin/env python3
 
 import warnings
+from typing import Optional
 
-from stytch.b2b.api.magic_links import MagicLinks
-from stytch.b2b.api.organizations import Organizations
-from stytch.b2b.api.passwords import Passwords
-from stytch.b2b.api.sessions import Sessions
-from stytch.b2b.api.discovery import Discovery
+from stytch.api.crypto_wallets import CryptoWallets
+from stytch.api.magic_links import MagicLinks
+from stytch.api.oauth import OAuth
+from stytch.api.otp import OTP
+from stytch.api.passwords import Passwords
+from stytch.api.sessions import Sessions
+from stytch.api.totps import TOTPs
+from stytch.api.users import Users
+from stytch.api.webauthn import WebAuthn
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
 class Client:
     """
-    Stytch B2B API Python client.
+    Stytch API Python client.
 
     Learn more at https://stytch.com/docs
     """
 
     def __init__(
         self,
         project_id: str,
         secret: str,
-        environment: str,
+        environment: Optional[str] = None,
         suppress_warnings: bool = False,
     ):
-        base_url = self._env_url(environment, suppress_warnings)
+        base_url = self._env_url(project_id, environment, suppress_warnings)
         api_base = ApiBase(base_url)
         sync_client = SyncClient(project_id, secret)
         async_client = AsyncClient(project_id, secret)
 
+        self.users = Users(api_base, sync_client, async_client)
         self.magic_links = MagicLinks(api_base, sync_client, async_client)
-        self.organizations = Organizations(api_base, sync_client, async_client)
+        self.oauth = OAuth(api_base, sync_client, async_client)
+        self.otps = OTP(api_base, sync_client, async_client)
         self.sessions = Sessions(api_base, sync_client, async_client)
+        self.webauthn = WebAuthn(api_base, sync_client, async_client)
+        self.totps = TOTPs(api_base, sync_client, async_client)
+        self.crypto_wallets = CryptoWallets(api_base, sync_client, async_client)
         self.passwords = Passwords(api_base, sync_client, async_client)
-        self.discovery = Discovery(api_base, sync_client, async_client)
 
     @classmethod
-    def _env_url(cls, env: str, suppress_warnings: bool = False) -> str:
+    def _env_url(
+        cls, project_id: str, env: Optional[str] = None, suppress_warnings: bool = False
+    ) -> str:
         """Resolve the base URL for the Stytch API environment."""
+        live_api = "https://api.stytch.com/v1/"
+        test_api = "https://test.stytch.com/v1/"
+        test_warning = "Test version of Stytch not intended for production use"
+
+        if env is None:
+            if project_id.startswith("project-live-"):
+                return live_api
+            else:
+                if not suppress_warnings:
+                    warnings.warn(test_warning)
+                return test_api
 
         # Supported production environments
         if env == "test":
             if not suppress_warnings:
-                warnings.warn("Test version of Stytch not intended for production use")
-            return "https://test.stytch.com/v1/b2b/"
+                warnings.warn(test_warning)
+            return test_api
         elif env == "live":
-            return "https://api.stytch.com/v1/b2b/"
+            return live_api
 
         return env
```

### Comparing `stytch-6.8.0/stytch/b2b/core/models.py` & `stytch-6.9.0/stytch/b2b/core/models.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/models/discovery_intermediate_sessions.py` & `stytch-6.9.0/stytch/b2b/models/discovery_intermediate_sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/models/discovery_organizations.py` & `stytch-6.9.0/stytch/b2b/models/discovery_organizations.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/models/magic_links.py` & `stytch-6.9.0/stytch/b2b/models/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/models/magic_links_discovery.py` & `stytch-6.9.0/stytch/b2b/models/magic_links_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/models/magic_links_email.py` & `stytch-6.9.0/stytch/b2b/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/models/organizations.py` & `stytch-6.9.0/stytch/b2b/models/organizations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-from typing import List
+from typing import Dict, List
 
 from stytch.b2b.core.models import Member, Organization
 from stytch.core.models import ResponseBase, SearchResultsMetadata
 
 
 class CreateResponse(ResponseBase):
     """Response fields beyond those defined in `ResponseBase`:
@@ -128,8 +128,9 @@
 
     - `members`: An array of Member objects.
 
     - `results_metadata`: Metadata relevant to your search query.
     """  # noqa
 
     members: List[Member]
+    organizations: Dict[str, Organization]
     results_metadata: SearchResultsMetadata
```

### Comparing `stytch-6.8.0/stytch/b2b/models/passwords.py` & `stytch-6.9.0/stytch/b2b/models/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/models/passwords_email.py` & `stytch-6.9.0/stytch/b2b/models/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/models/passwords_existing_password.py` & `stytch-6.9.0/stytch/b2b/models/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/models/passwords_session.py` & `stytch-6.9.0/stytch/b2b/models/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/b2b/models/sessions.py` & `stytch-6.9.0/stytch/b2b/models/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/core/http/client.py` & `stytch-6.9.0/stytch/core/http/client.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/core/models.py` & `stytch-6.9.0/stytch/core/models.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/models/crypto_wallets.py` & `stytch-6.9.0/stytch/models/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/models/magic_links.py` & `stytch-6.9.0/stytch/models/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/models/magic_links_email.py` & `stytch-6.9.0/stytch/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/models/oauth.py` & `stytch-6.9.0/stytch/models/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/models/passwords.py` & `stytch-6.9.0/stytch/models/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/models/sessions.py` & `stytch-6.9.0/stytch/models/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/models/totps.py` & `stytch-6.9.0/stytch/models/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/models/users.py` & `stytch-6.9.0/stytch/models/users.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch/models/webauthn.py` & `stytch-6.9.0/stytch/models/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/stytch.egg-info/PKG-INFO` & `stytch-6.9.0/stytch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 6.8.0
+Version: 6.9.0
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-6.8.0/stytch.egg-info/SOURCES.txt` & `stytch-6.9.0/stytch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/test/test_integration.py` & `stytch-6.9.0/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `stytch-6.8.0/test/test_integration_async.py` & `stytch-6.9.0/test/test_integration_async.py`

 * *Files identical despite different names*

