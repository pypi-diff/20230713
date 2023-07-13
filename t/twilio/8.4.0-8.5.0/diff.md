# Comparing `tmp/twilio-8.4.0.tar.gz` & `tmp/twilio-8.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twilio-8.4.0.tar", last modified: Wed Jun 28 11:34:08 2023, max compression
+gzip compressed data, was "twilio-8.5.0.tar", last modified: Thu Jul 13 15:32:31 2023, max compression
```

## Comparing `twilio-8.4.0.tar` & `twilio-8.5.0.tar`

### file list

```diff
@@ -1,861 +1,873 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.848114 twilio-8.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-28 11:33:54.000000 twilio-8.4.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-28 11:33:54.000000 twilio-8.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-28 11:33:54.000000 twilio-8.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-06-28 11:34:08.848114 twilio-8.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-06-28 11:33:54.000000 twilio-8.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-28 11:34:08.848114 twilio-8.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1694 2023-06-28 11:33:54.000000 twilio-8.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.736111 twilio-8.4.0/twilio/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.740111 twilio-8.4.0/twilio/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/base/client_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/base/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/base/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/base/instance_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/base/instance_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/base/list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/base/obsolete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/base/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/base/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/base/values.py
--rw-r--r--   0 runner    (1001) docker     (123)    14614 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/base/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.740111 twilio-8.4.0/twilio/http/
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/http/async_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/http/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/http/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/http/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/http/validation_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.740111 twilio-8.4.0/twilio/jwt/
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/jwt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.740111 twilio-8.4.0/twilio/jwt/access_token/
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/jwt/access_token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/jwt/access_token/grants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.740111 twilio-8.4.0/twilio/jwt/client/
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/jwt/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.740111 twilio-8.4.0/twilio/jwt/taskrouter/
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/jwt/taskrouter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/jwt/taskrouter/capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.740111 twilio-8.4.0/twilio/jwt/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/jwt/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/request_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.740111 twilio-8.4.0/twilio/rest/
--rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.740111 twilio-8.4.0/twilio/rest/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/accounts/AccountsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/accounts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.740111 twilio-8.4.0/twilio/rest/accounts/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/accounts/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/accounts/v1/auth_token_promotion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.740111 twilio-8.4.0/twilio/rest/accounts/v1/credential/
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/accounts/v1/credential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19489 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/accounts/v1/credential/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    20007 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/accounts/v1/credential/public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/accounts/v1/secondary_auth_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.744111 twilio-8.4.0/twilio/rest/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/ApiBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.744111 twilio-8.4.0/twilio/rest/api/v2010/
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.744111 twilio-8.4.0/twilio/rest/api/v2010/account/
--rw-r--r--   0 runner    (1001) docker     (123)    36206 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.744111 twilio-8.4.0/twilio/rest/api/v2010/account/address/
--rw-r--r--   0 runner    (1001) docker     (123)    35858 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/address/dependent_phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    47553 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/application.py
--rw-r--r--   0 runner    (1001) docker     (123)    17274 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/authorized_connect_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.748111 twilio-8.4.0/twilio/rest/api/v2010/account/available_phone_number_country/
--rw-r--r--   0 runner    (1001) docker     (123)    21427 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46239 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/available_phone_number_country/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    46210 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)    45860 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py
--rw-r--r--   0 runner    (1001) docker     (123)    45930 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/available_phone_number_country/national.py
--rw-r--r--   0 runner    (1001) docker     (123)    46000 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py
--rw-r--r--   0 runner    (1001) docker     (123)    45930 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py
--rw-r--r--   0 runner    (1001) docker     (123)    45790 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/available_phone_number_country/voip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/balance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.748111 twilio-8.4.0/twilio/rest/api/v2010/account/call/
--rw-r--r--   0 runner    (1001) docker     (123)    92392 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/call/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/call/feedback.py
--rw-r--r--   0 runner    (1001) docker     (123)    13986 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/call/feedback_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    28363 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/call/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    23472 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/call/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)    38495 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/call/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)    77226 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/call/siprec.py
--rw-r--r--   0 runner    (1001) docker     (123)    77116 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/call/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/call/user_defined_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.752111 twilio-8.4.0/twilio/rest/api/v2010/account/conference/
--rw-r--r--   0 runner    (1001) docker     (123)    41186 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/conference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    75225 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/conference/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    32729 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/conference/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)    26539 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/connect_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.752111 twilio-8.4.0/twilio/rest/api/v2010/account/incoming_phone_number/
--rw-r--r--   0 runner    (1001) docker     (123)    73374 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.752111 twilio-8.4.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/
--rw-r--r--   0 runner    (1001) docker     (123)    20750 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18341 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    36935 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/incoming_phone_number/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    37019 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py
--rw-r--r--   0 runner    (1001) docker     (123)    37103 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py
--rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.752111 twilio-8.4.0/twilio/rest/api/v2010/account/message/
--rw-r--r--   0 runner    (1001) docker     (123)    53984 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/message/feedback.py
--rw-r--r--   0 runner    (1001) docker     (123)    27246 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/message/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/new_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/new_signing_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    27505 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    22199 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/outgoing_caller_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.752111 twilio-8.4.0/twilio/rest/api/v2010/account/queue/
--rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19131 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/queue/member.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.752111 twilio-8.4.0/twilio/rest/api/v2010/account/recording/
--rw-r--r--   0 runner    (1001) docker     (123)    37769 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/recording/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.752111 twilio-8.4.0/twilio/rest/api/v2010/account/recording/add_on_result/
--rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19233 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/recording/add_on_result/payload.py
--rw-r--r--   0 runner    (1001) docker     (123)    19008 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/recording/transcription.py
--rw-r--r--   0 runner    (1001) docker     (123)    26406 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/short_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/signing_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.752111 twilio-8.4.0/twilio/rest/api/v2010/account/sip/
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/sip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.752111 twilio-8.4.0/twilio/rest/api/v2010/account/sip/credential_list/
--rw-r--r--   0 runner    (1001) docker     (123)    21278 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/sip/credential_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22757 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/sip/credential_list/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.756111 twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/
--rw-r--r--   0 runner    (1001) docker     (123)    45116 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.756111 twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/auth_types/
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.756111 twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.756111 twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21048 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    19893 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.756111 twilio-8.4.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/
--rw-r--r--   0 runner    (1001) docker     (123)    21808 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26238 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/transcription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.756111 twilio-8.4.0/twilio/rest/api/v2010/account/usage/
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/usage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.756111 twilio-8.4.0/twilio/rest/api/v2010/account/usage/record/
--rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/usage/record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38339 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/usage/record/all_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    38247 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/usage/record/daily.py
--rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/usage/record/last_month.py
--rw-r--r--   0 runner    (1001) docker     (123)    38339 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/usage/record/monthly.py
--rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/usage/record/this_month.py
--rw-r--r--   0 runner    (1001) docker     (123)    38247 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/usage/record/today.py
--rw-r--r--   0 runner    (1001) docker     (123)    38293 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/usage/record/yearly.py
--rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/usage/record/yesterday.py
--rw-r--r--   0 runner    (1001) docker     (123)    49245 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/usage/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/api/v2010/account/validation_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.760111 twilio-8.4.0/twilio/rest/autopilot/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/autopilot/AutopilotBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/autopilot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.760111 twilio-8.4.0/twilio/rest/autopilot/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/autopilot/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.760111 twilio-8.4.0/twilio/rest/autopilot/v1/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)    35087 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/autopilot/v1/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/autopilot/v1/assistant/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/autopilot/v1/assistant/dialogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.760111 twilio-8.4.0/twilio/rest/autopilot/v1/assistant/field_type/
--rw-r--r--   0 runner    (1001) docker     (123)    23752 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/autopilot/v1/assistant/field_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22246 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/autopilot/v1/assistant/field_type/field_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    22851 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/autopilot/v1/assistant/model_build.py
--rw-r--r--   0 runner    (1001) docker     (123)    29877 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/autopilot/v1/assistant/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/autopilot/v1/assistant/style_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.760111 twilio-8.4.0/twilio/rest/autopilot/v1/assistant/task/
--rw-r--r--   0 runner    (1001) docker     (123)    28213 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/autopilot/v1/assistant/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20115 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/autopilot/v1/assistant/task/field.py
--rw-r--r--   0 runner    (1001) docker     (123)    27891 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/autopilot/v1/assistant/task/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/autopilot/v1/assistant/task/task_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/autopilot/v1/assistant/task/task_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    24728 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/autopilot/v1/assistant/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/autopilot/v1/restore_assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.760111 twilio-8.4.0/twilio/rest/bulkexports/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/bulkexports/BulkexportsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/bulkexports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.760111 twilio-8.4.0/twilio/rest/bulkexports/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/bulkexports/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.764112 twilio-8.4.0/twilio/rest/bulkexports/v1/export/
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/bulkexports/v1/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/bulkexports/v1/export/day.py
--rw-r--r--   0 runner    (1001) docker     (123)    17005 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/bulkexports/v1/export/export_custom_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/bulkexports/v1/export/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/bulkexports/v1/export_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.764112 twilio-8.4.0/twilio/rest/chat/
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.764112 twilio-8.4.0/twilio/rest/chat/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27856 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v1/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.764112 twilio-8.4.0/twilio/rest/chat/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    92674 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v1/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.764112 twilio-8.4.0/twilio/rest/chat/v1/service/channel/
--rw-r--r--   0 runner    (1001) docker     (123)    28967 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v1/service/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22312 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v1/service/channel/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    27709 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v1/service/channel/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    26356 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v1/service/channel/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    21831 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v1/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.764112 twilio-8.4.0/twilio/rest/chat/v1/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)    26317 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v1/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12925 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v1/service/user/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.764112 twilio-8.4.0/twilio/rest/chat/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27486 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v2/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.764112 twilio-8.4.0/twilio/rest/chat/v2/service/
--rw-r--r--   0 runner    (1001) docker     (123)    66570 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v2/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22118 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v2/service/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.768112 twilio-8.4.0/twilio/rest/chat/v2/service/channel/
--rw-r--r--   0 runner    (1001) docker     (123)    39123 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v2/service/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22292 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v2/service/channel/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v2/service/channel/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    37545 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v2/service/channel/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    33770 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v2/service/channel/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    22232 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v2/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.768112 twilio-8.4.0/twilio/rest/chat/v2/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)    29035 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v2/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21909 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v2/service/user/user_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    27050 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v2/service/user/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.768112 twilio-8.4.0/twilio/rest/chat/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/chat/v3/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.768112 twilio-8.4.0/twilio/rest/content/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/content/ContentBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/content/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.768112 twilio-8.4.0/twilio/rest/content/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/content/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.768112 twilio-8.4.0/twilio/rest/content/v1/content/
--rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/content/v1/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/content/v1/content/approval_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/content/v1/content_and_approvals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/content/v1/legacy_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.768112 twilio-8.4.0/twilio/rest/conversations/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/ConversationsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.768112 twilio-8.4.0/twilio/rest/conversations/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37619 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/address_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.772112 twilio-8.4.0/twilio/rest/conversations/v1/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/configuration/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.772112 twilio-8.4.0/twilio/rest/conversations/v1/conversation/
--rw-r--r--   0 runner    (1001) docker     (123)    42957 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/conversation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.772112 twilio-8.4.0/twilio/rest/conversations/v1/conversation/message/
--rw-r--r--   0 runner    (1001) docker     (123)    34972 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/conversation/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)    40116 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/conversation/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    27236 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/conversation/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    27935 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    18739 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/participant_conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20943 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.772112 twilio-8.4.0/twilio/rest/conversations/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22289 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/service/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.772112 twilio-8.4.0/twilio/rest/conversations/v1/service/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    16088 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/service/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24410 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/service/configuration/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/service/configuration/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.772112 twilio-8.4.0/twilio/rest/conversations/v1/service/conversation/
--rw-r--r--   0 runner    (1001) docker     (123)    44808 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/service/conversation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.772112 twilio-8.4.0/twilio/rest/conversations/v1/service/conversation/message/
--rw-r--r--   0 runner    (1001) docker     (123)    36629 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/service/conversation/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)    41799 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/service/conversation/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    28926 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/service/conversation/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    19530 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/service/participant_conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22534 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.772112 twilio-8.4.0/twilio/rest/conversations/v1/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)    29682 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26510 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/service/user/user_conversation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.776112 twilio-8.4.0/twilio/rest/conversations/v1/user/
--rw-r--r--   0 runner    (1001) docker     (123)    28016 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25215 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/conversations/v1/user/user_conversation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.776112 twilio-8.4.0/twilio/rest/events/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/events/EventsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.776112 twilio-8.4.0/twilio/rest/events/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/events/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15317 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/events/v1/event_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.776112 twilio-8.4.0/twilio/rest/events/v1/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/events/v1/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/events/v1/schema/schema_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.776112 twilio-8.4.0/twilio/rest/events/v1/sink/
--rw-r--r--   0 runner    (1001) docker     (123)    22872 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/events/v1/sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/events/v1/sink/sink_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/events/v1/sink/sink_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.776112 twilio-8.4.0/twilio/rest/events/v1/subscription/
--rw-r--r--   0 runner    (1001) docker     (123)    22609 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/events/v1/subscription/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/events/v1/subscription/subscribed_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.776112 twilio-8.4.0/twilio/rest/flex_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/FlexApiBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.780112 twilio-8.4.0/twilio/rest/flex_api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23439 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v1/assessments.py
--rw-r--r--   0 runner    (1001) docker     (123)    19793 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v1/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13488 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v1/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    46860 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v1/flex_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v1/insights_assessments_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v1/insights_conversations.py
--rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v1/insights_questionnaires.py
--rw-r--r--   0 runner    (1001) docker     (123)    21091 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v1/insights_questionnaires_category.py
--rw-r--r--   0 runner    (1001) docker     (123)    26772 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v1/insights_questionnaires_question.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v1/insights_segments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v1/insights_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v1/insights_settings_answer_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v1/insights_settings_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v1/insights_user_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.780112 twilio-8.4.0/twilio/rest/flex_api/v1/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v1/interaction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.780112 twilio-8.4.0/twilio/rest/flex_api/v1/interaction/interaction_channel/
--rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v1/web_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.780112 twilio-8.4.0/twilio/rest/flex_api/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/flex_api/v2/web_channels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.780112 twilio-8.4.0/twilio/rest/frontline_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/frontline_api/FrontlineApiBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/frontline_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.780112 twilio-8.4.0/twilio/rest/frontline_api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/frontline_api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/frontline_api/v1/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.780112 twilio-8.4.0/twilio/rest/insights/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/insights/InsightsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/insights/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.780112 twilio-8.4.0/twilio/rest/insights/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/insights/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.784112 twilio-8.4.0/twilio/rest/insights/v1/call/
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/insights/v1/call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17572 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/insights/v1/call/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/insights/v1/call/call_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/insights/v1/call/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    14822 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/insights/v1/call/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    46779 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/insights/v1/call_summaries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.784112 twilio-8.4.0/twilio/rest/insights/v1/conference/
--rw-r--r--   0 runner    (1001) docker     (123)    31370 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/insights/v1/conference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25248 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/insights/v1/conference/conference_participant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.784112 twilio-8.4.0/twilio/rest/insights/v1/room/
--rw-r--r--   0 runner    (1001) docker     (123)    25243 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/insights/v1/room/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17908 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/insights/v1/room/participant.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/insights/v1/setting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.784112 twilio-8.4.0/twilio/rest/ip_messaging/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/IpMessagingBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.784112 twilio-8.4.0/twilio/rest/ip_messaging/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v1/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.784112 twilio-8.4.0/twilio/rest/ip_messaging/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    62960 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v1/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.784112 twilio-8.4.0/twilio/rest/ip_messaging/v1/service/channel/
--rw-r--r--   0 runner    (1001) docker     (123)    24064 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v1/service/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v1/service/channel/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    21725 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v1/service/channel/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v1/service/channel/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    18855 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v1/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.784112 twilio-8.4.0/twilio/rest/ip_messaging/v1/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)    21365 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v1/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v1/service/user/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.784112 twilio-8.4.0/twilio/rest/ip_messaging/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v2/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.788112 twilio-8.4.0/twilio/rest/ip_messaging/v2/service/
--rw-r--r--   0 runner    (1001) docker     (123)    45390 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v2/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17907 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v2/service/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.788112 twilio-8.4.0/twilio/rest/ip_messaging/v2/service/channel/
--rw-r--r--   0 runner    (1001) docker     (123)    30568 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v2/service/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v2/service/channel/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    29520 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v2/service/channel/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    28798 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v2/service/channel/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v2/service/channel/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    18855 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v2/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.788112 twilio-8.4.0/twilio/rest/ip_messaging/v2/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)    24051 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v2/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v2/service/user/user_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    21476 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/ip_messaging/v2/service/user/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.788112 twilio-8.4.0/twilio/rest/lookups/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/lookups/LookupsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/lookups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.788112 twilio-8.4.0/twilio/rest/lookups/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/lookups/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/lookups/v1/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.788112 twilio-8.4.0/twilio/rest/lookups/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/lookups/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23018 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/lookups/v2/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.788112 twilio-8.4.0/twilio/rest/media/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/media/MediaBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/media/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.792112 twilio-8.4.0/twilio/rest/media/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/media/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26533 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/media/v1/media_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/media/v1/media_recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.792112 twilio-8.4.0/twilio/rest/media/v1/player_streamer/
--rw-r--r--   0 runner    (1001) docker     (123)    25414 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/media/v1/player_streamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/media/v1/player_streamer/playback_grant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.792112 twilio-8.4.0/twilio/rest/messaging/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/messaging/MessagingBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/messaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.792112 twilio-8.4.0/twilio/rest/messaging/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/messaging/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.792112 twilio-8.4.0/twilio/rest/messaging/v1/brand_registration/
--rw-r--r--   0 runner    (1001) docker     (123)    24289 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/messaging/v1/brand_registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19914 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/messaging/v1/brand_registration/brand_vetting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/messaging/v1/deactivations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10495 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/messaging/v1/domain_certs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13875 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/messaging/v1/domain_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/messaging/v1/domain_config_messaging_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/messaging/v1/external_campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/messaging/v1/linkshortening_messaging_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/messaging/v1/linkshortening_messaging_service_domain_association.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.792112 twilio-8.4.0/twilio/rest/messaging/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    54653 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/messaging/v1/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/messaging/v1/service/alpha_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/messaging/v1/service/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/messaging/v1/service/short_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    33638 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/messaging/v1/service/us_app_to_person.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/messaging/v1/usecase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.792112 twilio-8.4.0/twilio/rest/microvisor/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/microvisor/MicrovisorBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/microvisor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.796112 twilio-8.4.0/twilio/rest/microvisor/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/microvisor/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17838 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/microvisor/v1/account_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/microvisor/v1/account_secret.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.796112 twilio-8.4.0/twilio/rest/microvisor/v1/app/
--rw-r--r--   0 runner    (1001) docker     (123)    15664 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/microvisor/v1/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/microvisor/v1/app/app_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.796112 twilio-8.4.0/twilio/rest/microvisor/v1/device/
--rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/microvisor/v1/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/microvisor/v1/device/device_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    19030 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/microvisor/v1/device/device_secret.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.796112 twilio-8.4.0/twilio/rest/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/monitor/MonitorBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.796112 twilio-8.4.0/twilio/rest/monitor/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/monitor/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22723 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/monitor/v1/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    25437 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/monitor/v1/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.796112 twilio-8.4.0/twilio/rest/notify/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/notify/NotifyBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/notify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.796112 twilio-8.4.0/twilio/rest/notify/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/notify/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27961 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/notify/v1/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.796112 twilio-8.4.0/twilio/rest/notify/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    47060 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/notify/v1/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30272 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/notify/v1/service/binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    25490 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/notify/v1/service/notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.796112 twilio-8.4.0/twilio/rest/numbers/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/NumbersBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.796112 twilio-8.4.0/twilio/rest/numbers/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/v1/bulk_eligibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/v1/porting_bulk_portability.py
--rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/v1/porting_portability.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.800113 twilio-8.4.0/twilio/rest/numbers/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.800113 twilio-8.4.0/twilio/rest/numbers/v2/authorization_document/
--rw-r--r--   0 runner    (1001) docker     (123)    24508 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/v2/authorization_document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22095 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/v2/authorization_document/dependent_hosted_number_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    35471 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/v2/hosted_number_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.800113 twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.800113 twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/
--rw-r--r--   0 runner    (1001) docker     (123)    47502 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py
--rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/end_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/regulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22407 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.800113 twilio-8.4.0/twilio/rest/oauth/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/oauth/OauthBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/oauth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.800113 twilio-8.4.0/twilio/rest/oauth/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/oauth/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/oauth/v1/device_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/oauth/v1/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/oauth/v1/openid_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/oauth/v1/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/oauth/v1/user_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.804113 twilio-8.4.0/twilio/rest/preview/
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/PreviewBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.804113 twilio-8.4.0/twilio/rest/preview/deployed_devices/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/deployed_devices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.804113 twilio-8.4.0/twilio/rest/preview/deployed_devices/fleet/
--rw-r--r--   0 runner    (1001) docker     (123)    22442 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/deployed_devices/fleet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24118 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/deployed_devices/fleet/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    22163 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/deployed_devices/fleet/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    26656 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/deployed_devices/fleet/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    22726 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/deployed_devices/fleet/key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.804113 twilio-8.4.0/twilio/rest/preview/hosted_numbers/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/hosted_numbers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.804113 twilio-8.4.0/twilio/rest/preview/hosted_numbers/authorization_document/
--rw-r--r--   0 runner    (1001) docker     (123)    32009 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24829 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    48143 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/hosted_numbers/hosted_number_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.804113 twilio-8.4.0/twilio/rest/preview/marketplace/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/marketplace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.804113 twilio-8.4.0/twilio/rest/preview/marketplace/available_add_on/
--rw-r--r--   0 runner    (1001) docker     (123)    15067 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/marketplace/available_add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.804113 twilio-8.4.0/twilio/rest/preview/marketplace/installed_add_on/
--rw-r--r--   0 runner    (1001) docker     (123)    23293 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/marketplace/installed_add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.804113 twilio-8.4.0/twilio/rest/preview/sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.804113 twilio-8.4.0/twilio/rest/preview/sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)    22270 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/sync/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.804113 twilio-8.4.0/twilio/rest/preview/sync/service/document/
--rw-r--r--   0 runner    (1001) docker     (123)    20547 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/sync/service/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21455 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/sync/service/document/document_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.808113 twilio-8.4.0/twilio/rest/preview/sync/service/sync_list/
--rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/sync/service/sync_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24174 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/sync/service/sync_list/sync_list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.808113 twilio-8.4.0/twilio/rest/preview/sync/service/sync_map/
--rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/sync/service/sync_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24063 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/sync/service/sync_map/sync_map_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    21250 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.808113 twilio-8.4.0/twilio/rest/preview/understand/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/understand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.808113 twilio-8.4.0/twilio/rest/preview/understand/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)    35382 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/understand/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/understand/assistant/assistant_fallback_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/understand/assistant/assistant_initiation_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/understand/assistant/dialogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.808113 twilio-8.4.0/twilio/rest/preview/understand/assistant/field_type/
--rw-r--r--   0 runner    (1001) docker     (123)    22348 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/understand/assistant/field_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20410 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/understand/assistant/field_type/field_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/understand/assistant/model_build.py
--rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/understand/assistant/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/understand/assistant/style_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.808113 twilio-8.4.0/twilio/rest/preview/understand/assistant/task/
--rw-r--r--   0 runner    (1001) docker     (123)    26813 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/understand/assistant/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/understand/assistant/task/field.py
--rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/understand/assistant/task/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/understand/assistant/task/task_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/understand/assistant/task/task_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.812113 twilio-8.4.0/twilio/rest/preview/wireless/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/wireless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/wireless/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/wireless/rate_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.812113 twilio-8.4.0/twilio/rest/preview/wireless/sim/
--rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/wireless/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/preview/wireless/sim/usage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.812113 twilio-8.4.0/twilio/rest/pricing/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/pricing/PricingBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/pricing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.812113 twilio-8.4.0/twilio/rest/pricing/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/pricing/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.812113 twilio-8.4.0/twilio/rest/pricing/v1/messaging/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/pricing/v1/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/pricing/v1/messaging/country.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.812113 twilio-8.4.0/twilio/rest/pricing/v1/phone_number/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/pricing/v1/phone_number/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/pricing/v1/phone_number/country.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.812113 twilio-8.4.0/twilio/rest/pricing/v1/voice/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/pricing/v1/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/pricing/v1/voice/country.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/pricing/v1/voice/number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.812113 twilio-8.4.0/twilio/rest/pricing/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/pricing/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/pricing/v2/country.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/pricing/v2/number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.812113 twilio-8.4.0/twilio/rest/pricing/v2/voice/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/pricing/v2/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/pricing/v2/voice/country.py
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/pricing/v2/voice/number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.812113 twilio-8.4.0/twilio/rest/proxy/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/proxy/ProxyBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.812113 twilio-8.4.0/twilio/rest/proxy/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/proxy/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.812113 twilio-8.4.0/twilio/rest/proxy/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    38044 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/proxy/v1/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23754 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/proxy/v1/service/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.816113 twilio-8.4.0/twilio/rest/proxy/v1/service/session/
--rw-r--r--   0 runner    (1001) docker     (123)    27767 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/proxy/v1/service/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21109 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/proxy/v1/service/session/interaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.816113 twilio-8.4.0/twilio/rest/proxy/v1/service/session/participant/
--rw-r--r--   0 runner    (1001) docker     (123)    22765 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/proxy/v1/service/session/participant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23242 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/proxy/v1/service/session/participant/message_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    21333 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/proxy/v1/service/short_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.816113 twilio-8.4.0/twilio/rest/routes/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/routes/RoutesBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.816113 twilio-8.4.0/twilio/rest/routes/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/routes/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/routes/v2/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/routes/v2/sip_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/routes/v2/trunk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.816113 twilio-8.4.0/twilio/rest/serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/serverless/ServerlessBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.816113 twilio-8.4.0/twilio/rest/serverless/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/serverless/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.816113 twilio-8.4.0/twilio/rest/serverless/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/serverless/v1/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.816113 twilio-8.4.0/twilio/rest/serverless/v1/service/asset/
--rw-r--r--   0 runner    (1001) docker     (123)    20582 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/serverless/v1/service/asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16714 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/serverless/v1/service/asset/asset_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.816113 twilio-8.4.0/twilio/rest/serverless/v1/service/build/
--rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/serverless/v1/service/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/serverless/v1/service/build/build_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.816113 twilio-8.4.0/twilio/rest/serverless/v1/service/environment/
--rw-r--r--   0 runner    (1001) docker     (123)    21009 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/serverless/v1/service/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/serverless/v1/service/environment/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    20926 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/serverless/v1/service/environment/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/serverless/v1/service/environment/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.816113 twilio-8.4.0/twilio/rest/serverless/v1/service/function/
--rw-r--r--   0 runner    (1001) docker     (123)    20928 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/serverless/v1/service/function/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.820113 twilio-8.4.0/twilio/rest/serverless/v1/service/function/function_version/
--rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/serverless/v1/service/function/function_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.820113 twilio-8.4.0/twilio/rest/studio/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/StudioBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.820113 twilio-8.4.0/twilio/rest/studio/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.820113 twilio-8.4.0/twilio/rest/studio/v1/flow/
--rw-r--r--   0 runner    (1001) docker     (123)    16404 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/v1/flow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.820113 twilio-8.4.0/twilio/rest/studio/v1/flow/engagement/
--rw-r--r--   0 runner    (1001) docker     (123)    21366 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/v1/flow/engagement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/v1/flow/engagement/engagement_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.820113 twilio-8.4.0/twilio/rest/studio/v1/flow/engagement/step/
--rw-r--r--   0 runner    (1001) docker     (123)    17219 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/v1/flow/engagement/step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/v1/flow/engagement/step/step_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.820113 twilio-8.4.0/twilio/rest/studio/v1/flow/execution/
--rw-r--r--   0 runner    (1001) docker     (123)    27270 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/v1/flow/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/v1/flow/execution/execution_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.820113 twilio-8.4.0/twilio/rest/studio/v1/flow/execution/execution_step/
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.820113 twilio-8.4.0/twilio/rest/studio/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.820113 twilio-8.4.0/twilio/rest/studio/v2/flow/
--rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/v2/flow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.820113 twilio-8.4.0/twilio/rest/studio/v2/flow/execution/
--rw-r--r--   0 runner    (1001) docker     (123)    27154 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/v2/flow/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/v2/flow/execution/execution_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.820113 twilio-8.4.0/twilio/rest/studio/v2/flow/execution/execution_step/
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/v2/flow/flow_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/v2/flow/flow_test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/studio/v2/flow_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.820113 twilio-8.4.0/twilio/rest/supersim/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/supersim/SupersimBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/supersim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.824113 twilio-8.4.0/twilio/rest/supersim/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/supersim/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23623 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/supersim/v1/esim_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    35221 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/supersim/v1/fleet.py
--rw-r--r--   0 runner    (1001) docker     (123)    26640 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/supersim/v1/ip_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/supersim/v1/network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.824113 twilio-8.4.0/twilio/rest/supersim/v1/network_access_profile/
--rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/supersim/v1/network_access_profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19359 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/supersim/v1/settings_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.824113 twilio-8.4.0/twilio/rest/supersim/v1/sim/
--rw-r--r--   0 runner    (1001) docker     (123)    28732 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/supersim/v1/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12030 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/supersim/v1/sim/billing_period.py
--rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/supersim/v1/sim/sim_ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    23001 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/supersim/v1/sms_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    26841 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/supersim/v1/usage_record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.824113 twilio-8.4.0/twilio/rest/sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/sync/SyncBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.824113 twilio-8.4.0/twilio/rest/sync/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/sync/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.824113 twilio-8.4.0/twilio/rest/sync/v1/service/
--rw-r--r--   0 runner    (1001) docker     (123)    36623 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/sync/v1/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.824113 twilio-8.4.0/twilio/rest/sync/v1/service/document/
--rw-r--r--   0 runner    (1001) docker     (123)    25373 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/sync/v1/service/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/sync/v1/service/document/document_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.824113 twilio-8.4.0/twilio/rest/sync/v1/service/sync_list/
--rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/sync/v1/service/sync_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36671 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/sync/v1/service/sync_list/sync_list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    21826 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.828113 twilio-8.4.0/twilio/rest/sync/v1/service/sync_map/
--rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/sync/v1/service/sync_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37230 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/sync/v1/service/sync_map/sync_map_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    21754 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.828113 twilio-8.4.0/twilio/rest/sync/v1/service/sync_stream/
--rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/sync/v1/service/sync_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/sync/v1/service/sync_stream/stream_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.828113 twilio-8.4.0/twilio/rest/taskrouter/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/TaskrouterBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.828113 twilio-8.4.0/twilio/rest/taskrouter/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.828113 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)    44452 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25986 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)    32776 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.828113 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/task/
--rw-r--r--   0 runner    (1001) docker     (123)    51478 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79751 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/task/reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)    23470 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/task_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.828113 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/task_queue/
--rw-r--r--   0 runner    (1001) docker     (123)    39230 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13380 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21315 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.832113 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/worker/
--rw-r--r--   0 runner    (1001) docker     (123)    43912 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    77533 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/worker/reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22091 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.832113 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    34579 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19228 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    14701 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.832113 twilio-8.4.0/twilio/rest/trunking/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trunking/TrunkingBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trunking/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.832113 twilio-8.4.0/twilio/rest/trunking/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trunking/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.832113 twilio-8.4.0/twilio/rest/trunking/v1/trunk/
--rw-r--r--   0 runner    (1001) docker     (123)    39976 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trunking/v1/trunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18350 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trunking/v1/trunk/credential_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trunking/v1/trunk/ip_access_control_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    27739 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trunking/v1/trunk/origination_url.py
--rw-r--r--   0 runner    (1001) docker     (123)    22459 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trunking/v1/trunk/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trunking/v1/trunk/recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.832113 twilio-8.4.0/twilio/rest/trusthub/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trusthub/TrusthubBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trusthub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.836114 twilio-8.4.0/twilio/rest/trusthub/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trusthub/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.836114 twilio-8.4.0/twilio/rest/trusthub/v1/customer_profiles/
--rw-r--r--   0 runner    (1001) docker     (123)    30761 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trusthub/v1/customer_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23437 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19934 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py
--rw-r--r--   0 runner    (1001) docker     (123)    20560 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trusthub/v1/end_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trusthub/v1/end_user_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    13542 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trusthub/v1/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trusthub/v1/supporting_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trusthub/v1/supporting_document_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.836114 twilio-8.4.0/twilio/rest/trusthub/v1/trust_products/
--rw-r--r--   0 runner    (1001) docker     (123)    30206 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trusthub/v1/trust_products/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23131 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.836114 twilio-8.4.0/twilio/rest/verify/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/VerifyBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.836114 twilio-8.4.0/twilio/rest/verify/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/v2/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/v2/safelist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.840114 twilio-8.4.0/twilio/rest/verify/v2/service/
--rw-r--r--   0 runner    (1001) docker     (123)    55315 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/v2/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/v2/service/access_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.840114 twilio-8.4.0/twilio/rest/verify/v2/service/entity/
--rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/v2/service/entity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.840114 twilio-8.4.0/twilio/rest/verify/v2/service/entity/challenge/
--rw-r--r--   0 runner    (1001) docker     (123)    34458 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/v2/service/entity/challenge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/v2/service/entity/challenge/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    29593 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/v2/service/entity/factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16164 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/v2/service/entity/new_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/v2/service/messaging_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.840114 twilio-8.4.0/twilio/rest/verify/v2/service/rate_limit/
--rw-r--r--   0 runner    (1001) docker     (123)    21507 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/v2/service/rate_limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22242 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/v2/service/rate_limit/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    21417 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/v2/service/verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/v2/service/verification_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    25389 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/v2/service/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/v2/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    29432 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/v2/verification_attempt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/verify/v2/verification_attempts_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.840114 twilio-8.4.0/twilio/rest/video/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/video/VideoBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/video/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.840114 twilio-8.4.0/twilio/rest/video/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/video/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/video/v1/composition.py
--rw-r--r--   0 runner    (1001) docker     (123)    54707 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/video/v1/composition_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/video/v1/composition_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    27313 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/video/v1/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/video/v1/recording_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.840114 twilio-8.4.0/twilio/rest/video/v1/room/
--rw-r--r--   0 runner    (1001) docker     (123)    38074 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/video/v1/room/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.844114 twilio-8.4.0/twilio/rest/video/v1/room/participant/
--rw-r--r--   0 runner    (1001) docker     (123)    28698 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/video/v1/room/participant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/video/v1/room/participant/anonymize.py
--rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/video/v1/room/participant/published_track.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/video/v1/room/participant/subscribe_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    17079 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/video/v1/room/participant/subscribed_track.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/video/v1/room/recording_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    24746 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/video/v1/room/room_recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.844114 twilio-8.4.0/twilio/rest/voice/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/voice/VoiceBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/voice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.844114 twilio-8.4.0/twilio/rest/voice/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/voice/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/voice/v1/archived_call.py
--rw-r--r--   0 runner    (1001) docker     (123)    37359 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/voice/v1/byoc_trunk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.844114 twilio-8.4.0/twilio/rest/voice/v1/connection_policy/
--rw-r--r--   0 runner    (1001) docker     (123)    20484 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/voice/v1/connection_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29170 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/voice/v1/connection_policy/connection_policy_target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.844114 twilio-8.4.0/twilio/rest/voice/v1/dialing_permissions/
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/voice/v1/dialing_permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.844114 twilio-8.4.0/twilio/rest/voice/v1/dialing_permissions/country/
--rw-r--r--   0 runner    (1001) docker     (123)    26486 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/voice/v1/dialing_permissions/country/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/voice/v1/dialing_permissions/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    20413 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/voice/v1/ip_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    19429 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/voice/v1/source_ip_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.844114 twilio-8.4.0/twilio/rest/wireless/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/wireless/WirelessBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/wireless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.844114 twilio-8.4.0/twilio/rest/wireless/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/wireless/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27361 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/wireless/v1/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    29604 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/wireless/v1/rate_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.844114 twilio-8.4.0/twilio/rest/wireless/v1/sim/
--rw-r--r--   0 runner    (1001) docker     (123)    46125 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/wireless/v1/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/wireless/v1/sim/data_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/wireless/v1/sim/usage_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/rest/wireless/v1/usage_record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.848114 twilio-8.4.0/twilio/twiml/
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/twiml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/twiml/fax_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/twiml/messaging_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    82958 2023-06-28 11:33:54.000000 twilio-8.4.0/twilio/twiml/voice_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:08.736111 twilio-8.4.0/twilio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-06-28 11:34:08.000000 twilio-8.4.0/twilio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30754 2023-06-28 11:34:08.000000 twilio-8.4.0/twilio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 11:34:08.000000 twilio-8.4.0/twilio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 11:34:08.000000 twilio-8.4.0/twilio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-28 11:34:08.000000 twilio-8.4.0/twilio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.309839 twilio-8.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-13 15:32:19.000000 twilio-8.5.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-13 15:32:19.000000 twilio-8.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-13 15:32:19.000000 twilio-8.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-07-13 15:32:31.309839 twilio-8.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-07-13 15:32:19.000000 twilio-8.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-13 15:32:31.309839 twilio-8.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1694 2023-07-13 15:32:19.000000 twilio-8.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.161837 twilio-8.5.0/twilio/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.165837 twilio-8.5.0/twilio/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/base/client_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/base/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/base/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/base/instance_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/base/instance_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/base/list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/base/obsolete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/base/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/base/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/base/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14614 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/base/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.165837 twilio-8.5.0/twilio/http/
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/http/async_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/http/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/http/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/http/validation_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.169837 twilio-8.5.0/twilio/jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/jwt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.169837 twilio-8.5.0/twilio/jwt/access_token/
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/jwt/access_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/jwt/access_token/grants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.169837 twilio-8.5.0/twilio/jwt/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/jwt/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.169837 twilio-8.5.0/twilio/jwt/taskrouter/
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/jwt/taskrouter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/jwt/taskrouter/capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.169837 twilio-8.5.0/twilio/jwt/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/jwt/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/request_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.169837 twilio-8.5.0/twilio/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.169837 twilio-8.5.0/twilio/rest/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/accounts/AccountsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/accounts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.169837 twilio-8.5.0/twilio/rest/accounts/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/accounts/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/accounts/v1/auth_token_promotion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.169837 twilio-8.5.0/twilio/rest/accounts/v1/credential/
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/accounts/v1/credential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19489 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/accounts/v1/credential/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20007 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/accounts/v1/credential/public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/accounts/v1/secondary_auth_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.169837 twilio-8.5.0/twilio/rest/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/ApiBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.173838 twilio-8.5.0/twilio/rest/api/v2010/
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.173838 twilio-8.5.0/twilio/rest/api/v2010/account/
+-rw-r--r--   0 runner    (1001) docker     (123)    36206 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.173838 twilio-8.5.0/twilio/rest/api/v2010/account/address/
+-rw-r--r--   0 runner    (1001) docker     (123)    35858 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/address/dependent_phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47553 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17274 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/authorized_connect_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.177837 twilio-8.5.0/twilio/rest/api/v2010/account/available_phone_number_country/
+-rw-r--r--   0 runner    (1001) docker     (123)    21427 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46239 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/available_phone_number_country/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46210 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45860 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45930 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/available_phone_number_country/national.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46000 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45930 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45790 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/available_phone_number_country/voip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/balance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.181838 twilio-8.5.0/twilio/rest/api/v2010/account/call/
+-rw-r--r--   0 runner    (1001) docker     (123)    92392 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/call/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/call/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13986 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/call/feedback_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28363 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/call/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23472 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/call/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38495 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/call/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77226 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/call/siprec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77116 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/call/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/call/user_defined_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.181838 twilio-8.5.0/twilio/rest/api/v2010/account/conference/
+-rw-r--r--   0 runner    (1001) docker     (123)    41186 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/conference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75225 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/conference/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32729 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/conference/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26539 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/connect_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.181838 twilio-8.5.0/twilio/rest/api/v2010/account/incoming_phone_number/
+-rw-r--r--   0 runner    (1001) docker     (123)    73374 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.181838 twilio-8.5.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)    20750 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18341 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36935 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/incoming_phone_number/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37019 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37103 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.181838 twilio-8.5.0/twilio/rest/api/v2010/account/message/
+-rw-r--r--   0 runner    (1001) docker     (123)    53984 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/message/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27246 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/message/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/new_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/new_signing_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27505 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22199 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/outgoing_caller_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.185838 twilio-8.5.0/twilio/rest/api/v2010/account/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19131 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/queue/member.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.185838 twilio-8.5.0/twilio/rest/api/v2010/account/recording/
+-rw-r--r--   0 runner    (1001) docker     (123)    37769 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/recording/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.185838 twilio-8.5.0/twilio/rest/api/v2010/account/recording/add_on_result/
+-rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19233 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/recording/add_on_result/payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19008 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/recording/transcription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26406 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/short_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/signing_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.185838 twilio-8.5.0/twilio/rest/api/v2010/account/sip/
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/sip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.185838 twilio-8.5.0/twilio/rest/api/v2010/account/sip/credential_list/
+-rw-r--r--   0 runner    (1001) docker     (123)    21278 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/sip/credential_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22757 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/sip/credential_list/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.185838 twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)    45116 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.185838 twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/auth_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.185838 twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.189838 twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21048 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19893 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.189838 twilio-8.5.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/
+-rw-r--r--   0 runner    (1001) docker     (123)    21808 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26238 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/transcription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.189838 twilio-8.5.0/twilio/rest/api/v2010/account/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/usage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.189838 twilio-8.5.0/twilio/rest/api/v2010/account/usage/record/
+-rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/usage/record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38339 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/usage/record/all_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38247 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/usage/record/daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/usage/record/last_month.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38339 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/usage/record/monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/usage/record/this_month.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38247 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/usage/record/today.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38293 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/usage/record/yearly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/usage/record/yesterday.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49245 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/usage/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/api/v2010/account/validation_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.189838 twilio-8.5.0/twilio/rest/autopilot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/autopilot/AutopilotBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/autopilot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.193838 twilio-8.5.0/twilio/rest/autopilot/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/autopilot/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.193838 twilio-8.5.0/twilio/rest/autopilot/v1/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)    35087 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/autopilot/v1/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/autopilot/v1/assistant/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/autopilot/v1/assistant/dialogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.193838 twilio-8.5.0/twilio/rest/autopilot/v1/assistant/field_type/
+-rw-r--r--   0 runner    (1001) docker     (123)    23752 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/autopilot/v1/assistant/field_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22246 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/autopilot/v1/assistant/field_type/field_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22851 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/autopilot/v1/assistant/model_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29877 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/autopilot/v1/assistant/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/autopilot/v1/assistant/style_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.193838 twilio-8.5.0/twilio/rest/autopilot/v1/assistant/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    28213 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/autopilot/v1/assistant/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20115 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/autopilot/v1/assistant/task/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27891 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/autopilot/v1/assistant/task/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/autopilot/v1/assistant/task/task_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/autopilot/v1/assistant/task/task_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24728 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/autopilot/v1/assistant/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/autopilot/v1/restore_assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.197838 twilio-8.5.0/twilio/rest/bulkexports/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/bulkexports/BulkexportsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/bulkexports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.197838 twilio-8.5.0/twilio/rest/bulkexports/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/bulkexports/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.197838 twilio-8.5.0/twilio/rest/bulkexports/v1/export/
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/bulkexports/v1/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/bulkexports/v1/export/day.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17005 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/bulkexports/v1/export/export_custom_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/bulkexports/v1/export/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/bulkexports/v1/export_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.197838 twilio-8.5.0/twilio/rest/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.197838 twilio-8.5.0/twilio/rest/chat/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27856 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v1/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.197838 twilio-8.5.0/twilio/rest/chat/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    92674 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v1/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.197838 twilio-8.5.0/twilio/rest/chat/v1/service/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    28967 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v1/service/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22312 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v1/service/channel/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27709 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v1/service/channel/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26356 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v1/service/channel/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21831 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v1/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.201838 twilio-8.5.0/twilio/rest/chat/v1/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    26317 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v1/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12925 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v1/service/user/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.201838 twilio-8.5.0/twilio/rest/chat/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27486 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v2/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.201838 twilio-8.5.0/twilio/rest/chat/v2/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    66570 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v2/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22118 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v2/service/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.201838 twilio-8.5.0/twilio/rest/chat/v2/service/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    39123 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v2/service/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22292 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v2/service/channel/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v2/service/channel/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37545 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v2/service/channel/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33770 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v2/service/channel/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22232 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v2/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.201838 twilio-8.5.0/twilio/rest/chat/v2/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    29035 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v2/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21909 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v2/service/user/user_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27050 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v2/service/user/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.201838 twilio-8.5.0/twilio/rest/chat/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/chat/v3/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.205838 twilio-8.5.0/twilio/rest/content/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/content/ContentBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/content/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.205838 twilio-8.5.0/twilio/rest/content/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/content/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.205838 twilio-8.5.0/twilio/rest/content/v1/content/
+-rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/content/v1/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/content/v1/content/approval_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/content/v1/content_and_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/content/v1/legacy_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.205838 twilio-8.5.0/twilio/rest/conversations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/ConversationsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.205838 twilio-8.5.0/twilio/rest/conversations/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37619 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/address_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.205838 twilio-8.5.0/twilio/rest/conversations/v1/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/configuration/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.209838 twilio-8.5.0/twilio/rest/conversations/v1/conversation/
+-rw-r--r--   0 runner    (1001) docker     (123)    42957 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/conversation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.209838 twilio-8.5.0/twilio/rest/conversations/v1/conversation/message/
+-rw-r--r--   0 runner    (1001) docker     (123)    34972 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/conversation/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40116 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/conversation/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27236 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/conversation/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27935 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18739 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/participant_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20943 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.209838 twilio-8.5.0/twilio/rest/conversations/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22289 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/service/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.209838 twilio-8.5.0/twilio/rest/conversations/v1/service/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    16088 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/service/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24410 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/service/configuration/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/service/configuration/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.209838 twilio-8.5.0/twilio/rest/conversations/v1/service/conversation/
+-rw-r--r--   0 runner    (1001) docker     (123)    44808 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/service/conversation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.209838 twilio-8.5.0/twilio/rest/conversations/v1/service/conversation/message/
+-rw-r--r--   0 runner    (1001) docker     (123)    36629 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/service/conversation/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41799 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/service/conversation/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28926 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/service/conversation/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19530 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/service/participant_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22534 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.213838 twilio-8.5.0/twilio/rest/conversations/v1/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    29682 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26510 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/service/user/user_conversation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.213838 twilio-8.5.0/twilio/rest/conversations/v1/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    28016 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25215 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/conversations/v1/user/user_conversation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.213838 twilio-8.5.0/twilio/rest/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/events/EventsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.213838 twilio-8.5.0/twilio/rest/events/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/events/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15317 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/events/v1/event_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.213838 twilio-8.5.0/twilio/rest/events/v1/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/events/v1/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/events/v1/schema/schema_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.213838 twilio-8.5.0/twilio/rest/events/v1/sink/
+-rw-r--r--   0 runner    (1001) docker     (123)    22872 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/events/v1/sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/events/v1/sink/sink_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/events/v1/sink/sink_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.213838 twilio-8.5.0/twilio/rest/events/v1/subscription/
+-rw-r--r--   0 runner    (1001) docker     (123)    22609 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/events/v1/subscription/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/events/v1/subscription/subscribed_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.213838 twilio-8.5.0/twilio/rest/flex_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/FlexApiBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.217838 twilio-8.5.0/twilio/rest/flex_api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23439 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v1/assessments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19793 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v1/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13488 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v1/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46860 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v1/flex_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v1/insights_assessments_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v1/insights_conversations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v1/insights_questionnaires.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21091 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v1/insights_questionnaires_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26772 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v1/insights_questionnaires_question.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v1/insights_segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v1/insights_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v1/insights_settings_answer_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v1/insights_settings_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v1/insights_user_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.217838 twilio-8.5.0/twilio/rest/flex_api/v1/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v1/interaction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.217838 twilio-8.5.0/twilio/rest/flex_api/v1/interaction/interaction_channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v1/web_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.221838 twilio-8.5.0/twilio/rest/flex_api/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/flex_api/v2/web_channels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.221838 twilio-8.5.0/twilio/rest/frontline_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/frontline_api/FrontlineApiBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/frontline_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.221838 twilio-8.5.0/twilio/rest/frontline_api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/frontline_api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/frontline_api/v1/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.221838 twilio-8.5.0/twilio/rest/insights/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/insights/InsightsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/insights/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.221838 twilio-8.5.0/twilio/rest/insights/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/insights/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.221838 twilio-8.5.0/twilio/rest/insights/v1/call/
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/insights/v1/call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17572 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/insights/v1/call/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/insights/v1/call/call_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/insights/v1/call/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14822 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/insights/v1/call/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46779 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/insights/v1/call_summaries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.221838 twilio-8.5.0/twilio/rest/insights/v1/conference/
+-rw-r--r--   0 runner    (1001) docker     (123)    31370 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/insights/v1/conference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25248 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/insights/v1/conference/conference_participant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.225838 twilio-8.5.0/twilio/rest/insights/v1/room/
+-rw-r--r--   0 runner    (1001) docker     (123)    25243 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/insights/v1/room/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17908 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/insights/v1/room/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/insights/v1/setting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.225838 twilio-8.5.0/twilio/rest/intelligence/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/intelligence/IntelligenceBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/intelligence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.225838 twilio-8.5.0/twilio/rest/intelligence/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/intelligence/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32294 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/intelligence/v2/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.225838 twilio-8.5.0/twilio/rest/intelligence/v2/transcript/
+-rw-r--r--   0 runner    (1001) docker     (123)    29886 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/intelligence/v2/transcript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/intelligence/v2/transcript/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/intelligence/v2/transcript/operator_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/intelligence/v2/transcript/sentence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.225838 twilio-8.5.0/twilio/rest/ip_messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/IpMessagingBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.225838 twilio-8.5.0/twilio/rest/ip_messaging/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v1/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.225838 twilio-8.5.0/twilio/rest/ip_messaging/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    62960 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v1/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.229838 twilio-8.5.0/twilio/rest/ip_messaging/v1/service/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    24064 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v1/service/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v1/service/channel/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21725 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v1/service/channel/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v1/service/channel/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18855 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v1/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.229838 twilio-8.5.0/twilio/rest/ip_messaging/v1/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    21365 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v1/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v1/service/user/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.229838 twilio-8.5.0/twilio/rest/ip_messaging/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v2/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.229838 twilio-8.5.0/twilio/rest/ip_messaging/v2/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    45390 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v2/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17907 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v2/service/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.229838 twilio-8.5.0/twilio/rest/ip_messaging/v2/service/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)    30568 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v2/service/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v2/service/channel/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29520 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v2/service/channel/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28798 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v2/service/channel/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v2/service/channel/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18855 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v2/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.233838 twilio-8.5.0/twilio/rest/ip_messaging/v2/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    24051 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v2/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v2/service/user/user_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21476 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/ip_messaging/v2/service/user/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.233838 twilio-8.5.0/twilio/rest/lookups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/lookups/LookupsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/lookups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.233838 twilio-8.5.0/twilio/rest/lookups/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/lookups/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/lookups/v1/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.233838 twilio-8.5.0/twilio/rest/lookups/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/lookups/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23018 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/lookups/v2/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.233838 twilio-8.5.0/twilio/rest/media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/media/MediaBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/media/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.233838 twilio-8.5.0/twilio/rest/media/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/media/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26533 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/media/v1/media_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/media/v1/media_recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.233838 twilio-8.5.0/twilio/rest/media/v1/player_streamer/
+-rw-r--r--   0 runner    (1001) docker     (123)    25414 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/media/v1/player_streamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/media/v1/player_streamer/playback_grant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.233838 twilio-8.5.0/twilio/rest/messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/MessagingBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.237838 twilio-8.5.0/twilio/rest/messaging/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.237838 twilio-8.5.0/twilio/rest/messaging/v1/brand_registration/
+-rw-r--r--   0 runner    (1001) docker     (123)    24289 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/v1/brand_registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19914 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/v1/brand_registration/brand_vetting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/v1/deactivations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10495 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/v1/domain_certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13875 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/v1/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/v1/domain_config_messaging_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/v1/external_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/v1/linkshortening_messaging_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/v1/linkshortening_messaging_service_domain_association.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.237838 twilio-8.5.0/twilio/rest/messaging/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    54653 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/v1/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/v1/service/alpha_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/v1/service/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/v1/service/short_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33638 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/v1/service/us_app_to_person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55969 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/v1/tollfree_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/messaging/v1/usecase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.241838 twilio-8.5.0/twilio/rest/microvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/microvisor/MicrovisorBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/microvisor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.241838 twilio-8.5.0/twilio/rest/microvisor/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/microvisor/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17838 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/microvisor/v1/account_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/microvisor/v1/account_secret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.241838 twilio-8.5.0/twilio/rest/microvisor/v1/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    15664 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/microvisor/v1/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/microvisor/v1/app/app_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.241838 twilio-8.5.0/twilio/rest/microvisor/v1/device/
+-rw-r--r--   0 runner    (1001) docker     (123)    20851 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/microvisor/v1/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/microvisor/v1/device/device_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19030 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/microvisor/v1/device/device_secret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.241838 twilio-8.5.0/twilio/rest/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/monitor/MonitorBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.241838 twilio-8.5.0/twilio/rest/monitor/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/monitor/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22723 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/monitor/v1/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25437 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/monitor/v1/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.241838 twilio-8.5.0/twilio/rest/notify/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/notify/NotifyBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/notify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.241838 twilio-8.5.0/twilio/rest/notify/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/notify/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27961 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/notify/v1/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.241838 twilio-8.5.0/twilio/rest/notify/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    47060 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/notify/v1/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30272 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/notify/v1/service/binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25490 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/notify/v1/service/notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.245838 twilio-8.5.0/twilio/rest/numbers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/NumbersBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.245838 twilio-8.5.0/twilio/rest/numbers/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/v1/bulk_eligibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/v1/porting_bulk_portability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/v1/porting_portability.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.245838 twilio-8.5.0/twilio/rest/numbers/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.245838 twilio-8.5.0/twilio/rest/numbers/v2/authorization_document/
+-rw-r--r--   0 runner    (1001) docker     (123)    25226 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/v2/authorization_document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22095 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/v2/authorization_document/dependent_hosted_number_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35284 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/v2/hosted_number_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.245838 twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.249838 twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)    47502 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/end_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/regulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22407 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.249838 twilio-8.5.0/twilio/rest/oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/oauth/OauthBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/oauth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.249838 twilio-8.5.0/twilio/rest/oauth/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/oauth/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/oauth/v1/device_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/oauth/v1/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/oauth/v1/openid_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/oauth/v1/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/oauth/v1/user_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.249838 twilio-8.5.0/twilio/rest/preview/
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/PreviewBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.249838 twilio-8.5.0/twilio/rest/preview/deployed_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/deployed_devices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.253838 twilio-8.5.0/twilio/rest/preview/deployed_devices/fleet/
+-rw-r--r--   0 runner    (1001) docker     (123)    22442 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/deployed_devices/fleet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24118 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/deployed_devices/fleet/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22163 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/deployed_devices/fleet/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26656 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/deployed_devices/fleet/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22726 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/deployed_devices/fleet/key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.253838 twilio-8.5.0/twilio/rest/preview/hosted_numbers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/hosted_numbers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.253838 twilio-8.5.0/twilio/rest/preview/hosted_numbers/authorization_document/
+-rw-r--r--   0 runner    (1001) docker     (123)    32009 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24829 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48143 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/hosted_numbers/hosted_number_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.253838 twilio-8.5.0/twilio/rest/preview/marketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/marketplace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.253838 twilio-8.5.0/twilio/rest/preview/marketplace/available_add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)    15067 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/marketplace/available_add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.253838 twilio-8.5.0/twilio/rest/preview/marketplace/installed_add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)    23293 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/marketplace/installed_add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.253838 twilio-8.5.0/twilio/rest/preview/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.253838 twilio-8.5.0/twilio/rest/preview/sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    22270 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/sync/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.253838 twilio-8.5.0/twilio/rest/preview/sync/service/document/
+-rw-r--r--   0 runner    (1001) docker     (123)    20547 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/sync/service/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21455 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/sync/service/document/document_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.253838 twilio-8.5.0/twilio/rest/preview/sync/service/sync_list/
+-rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/sync/service/sync_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24174 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/sync/service/sync_list/sync_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.257839 twilio-8.5.0/twilio/rest/preview/sync/service/sync_map/
+-rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/sync/service/sync_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24063 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/sync/service/sync_map/sync_map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21250 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.257839 twilio-8.5.0/twilio/rest/preview/understand/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/understand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.257839 twilio-8.5.0/twilio/rest/preview/understand/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)    35382 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/understand/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/understand/assistant/assistant_fallback_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/understand/assistant/assistant_initiation_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/understand/assistant/dialogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.257839 twilio-8.5.0/twilio/rest/preview/understand/assistant/field_type/
+-rw-r--r--   0 runner    (1001) docker     (123)    22348 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/understand/assistant/field_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20410 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/understand/assistant/field_type/field_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/understand/assistant/model_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/understand/assistant/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/understand/assistant/style_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.261839 twilio-8.5.0/twilio/rest/preview/understand/assistant/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    26813 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/understand/assistant/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/understand/assistant/task/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/understand/assistant/task/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/understand/assistant/task/task_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/understand/assistant/task/task_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.261839 twilio-8.5.0/twilio/rest/preview/wireless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/wireless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/wireless/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/wireless/rate_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.261839 twilio-8.5.0/twilio/rest/preview/wireless/sim/
+-rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/wireless/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/preview/wireless/sim/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.261839 twilio-8.5.0/twilio/rest/pricing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/pricing/PricingBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/pricing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.261839 twilio-8.5.0/twilio/rest/pricing/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/pricing/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.261839 twilio-8.5.0/twilio/rest/pricing/v1/messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/pricing/v1/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/pricing/v1/messaging/country.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.261839 twilio-8.5.0/twilio/rest/pricing/v1/phone_number/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/pricing/v1/phone_number/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/pricing/v1/phone_number/country.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.261839 twilio-8.5.0/twilio/rest/pricing/v1/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/pricing/v1/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/pricing/v1/voice/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/pricing/v1/voice/number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.265838 twilio-8.5.0/twilio/rest/pricing/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/pricing/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/pricing/v2/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/pricing/v2/number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.265838 twilio-8.5.0/twilio/rest/pricing/v2/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/pricing/v2/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/pricing/v2/voice/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/pricing/v2/voice/number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.265838 twilio-8.5.0/twilio/rest/proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/proxy/ProxyBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.265838 twilio-8.5.0/twilio/rest/proxy/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/proxy/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.265838 twilio-8.5.0/twilio/rest/proxy/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    38044 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/proxy/v1/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23754 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/proxy/v1/service/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.265838 twilio-8.5.0/twilio/rest/proxy/v1/service/session/
+-rw-r--r--   0 runner    (1001) docker     (123)    27767 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/proxy/v1/service/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21109 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/proxy/v1/service/session/interaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.265838 twilio-8.5.0/twilio/rest/proxy/v1/service/session/participant/
+-rw-r--r--   0 runner    (1001) docker     (123)    22765 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/proxy/v1/service/session/participant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23242 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/proxy/v1/service/session/participant/message_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21333 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/proxy/v1/service/short_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.265838 twilio-8.5.0/twilio/rest/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/routes/RoutesBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.269839 twilio-8.5.0/twilio/rest/routes/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/routes/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/routes/v2/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/routes/v2/sip_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/routes/v2/trunk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.269839 twilio-8.5.0/twilio/rest/serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/serverless/ServerlessBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.269839 twilio-8.5.0/twilio/rest/serverless/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/serverless/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.269839 twilio-8.5.0/twilio/rest/serverless/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/serverless/v1/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.269839 twilio-8.5.0/twilio/rest/serverless/v1/service/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)    20582 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/serverless/v1/service/asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16714 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/serverless/v1/service/asset/asset_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.269839 twilio-8.5.0/twilio/rest/serverless/v1/service/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/serverless/v1/service/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/serverless/v1/service/build/build_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.269839 twilio-8.5.0/twilio/rest/serverless/v1/service/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)    21009 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/serverless/v1/service/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/serverless/v1/service/environment/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20926 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/serverless/v1/service/environment/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/serverless/v1/service/environment/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.269839 twilio-8.5.0/twilio/rest/serverless/v1/service/function/
+-rw-r--r--   0 runner    (1001) docker     (123)    20928 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/serverless/v1/service/function/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.269839 twilio-8.5.0/twilio/rest/serverless/v1/service/function/function_version/
+-rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/serverless/v1/service/function/function_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.273839 twilio-8.5.0/twilio/rest/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/StudioBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.273839 twilio-8.5.0/twilio/rest/studio/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.273839 twilio-8.5.0/twilio/rest/studio/v1/flow/
+-rw-r--r--   0 runner    (1001) docker     (123)    16404 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/v1/flow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.273839 twilio-8.5.0/twilio/rest/studio/v1/flow/engagement/
+-rw-r--r--   0 runner    (1001) docker     (123)    21366 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/v1/flow/engagement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/v1/flow/engagement/engagement_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.273839 twilio-8.5.0/twilio/rest/studio/v1/flow/engagement/step/
+-rw-r--r--   0 runner    (1001) docker     (123)    17219 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/v1/flow/engagement/step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/v1/flow/engagement/step/step_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.273839 twilio-8.5.0/twilio/rest/studio/v1/flow/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)    27270 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/v1/flow/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/v1/flow/execution/execution_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.273839 twilio-8.5.0/twilio/rest/studio/v1/flow/execution/execution_step/
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.273839 twilio-8.5.0/twilio/rest/studio/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.273839 twilio-8.5.0/twilio/rest/studio/v2/flow/
+-rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/v2/flow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.277839 twilio-8.5.0/twilio/rest/studio/v2/flow/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)    27154 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/v2/flow/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/v2/flow/execution/execution_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.277839 twilio-8.5.0/twilio/rest/studio/v2/flow/execution/execution_step/
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/v2/flow/flow_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/v2/flow/flow_test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/studio/v2/flow_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.277839 twilio-8.5.0/twilio/rest/supersim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/supersim/SupersimBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/supersim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.277839 twilio-8.5.0/twilio/rest/supersim/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/supersim/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23623 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/supersim/v1/esim_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35221 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/supersim/v1/fleet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26640 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/supersim/v1/ip_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/supersim/v1/network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.277839 twilio-8.5.0/twilio/rest/supersim/v1/network_access_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/supersim/v1/network_access_profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19359 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/supersim/v1/settings_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.277839 twilio-8.5.0/twilio/rest/supersim/v1/sim/
+-rw-r--r--   0 runner    (1001) docker     (123)    28732 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/supersim/v1/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12030 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/supersim/v1/sim/billing_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/supersim/v1/sim/sim_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23001 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/supersim/v1/sms_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26841 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/supersim/v1/usage_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.281839 twilio-8.5.0/twilio/rest/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/sync/SyncBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.281839 twilio-8.5.0/twilio/rest/sync/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/sync/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.281839 twilio-8.5.0/twilio/rest/sync/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    36623 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/sync/v1/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.281839 twilio-8.5.0/twilio/rest/sync/v1/service/document/
+-rw-r--r--   0 runner    (1001) docker     (123)    25373 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/sync/v1/service/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/sync/v1/service/document/document_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.281839 twilio-8.5.0/twilio/rest/sync/v1/service/sync_list/
+-rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/sync/v1/service/sync_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36671 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/sync/v1/service/sync_list/sync_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21826 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.281839 twilio-8.5.0/twilio/rest/sync/v1/service/sync_map/
+-rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/sync/v1/service/sync_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37230 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/sync/v1/service/sync_map/sync_map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21754 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.281839 twilio-8.5.0/twilio/rest/sync/v1/service/sync_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/sync/v1/service/sync_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/sync/v1/service/sync_stream/stream_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.281839 twilio-8.5.0/twilio/rest/taskrouter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/TaskrouterBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.281839 twilio-8.5.0/twilio/rest/taskrouter/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.285839 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)    44452 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25986 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32776 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.285839 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    51478 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79751 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/task/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23470 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/task_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.285839 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/task_queue/
+-rw-r--r--   0 runner    (1001) docker     (123)    39230 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13380 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21315 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.289839 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)    43912 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77533 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/worker/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22091 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.289839 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    34579 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19228 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14701 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.289839 twilio-8.5.0/twilio/rest/trunking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trunking/TrunkingBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trunking/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.289839 twilio-8.5.0/twilio/rest/trunking/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trunking/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.289839 twilio-8.5.0/twilio/rest/trunking/v1/trunk/
+-rw-r--r--   0 runner    (1001) docker     (123)    39976 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trunking/v1/trunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18350 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trunking/v1/trunk/credential_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trunking/v1/trunk/ip_access_control_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27739 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trunking/v1/trunk/origination_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22459 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trunking/v1/trunk/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trunking/v1/trunk/recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.293839 twilio-8.5.0/twilio/rest/trusthub/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trusthub/TrusthubBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trusthub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.293839 twilio-8.5.0/twilio/rest/trusthub/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trusthub/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.293839 twilio-8.5.0/twilio/rest/trusthub/v1/customer_profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)    30761 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trusthub/v1/customer_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23437 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19934 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20560 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trusthub/v1/end_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trusthub/v1/end_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13542 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trusthub/v1/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trusthub/v1/supporting_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trusthub/v1/supporting_document_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.293839 twilio-8.5.0/twilio/rest/trusthub/v1/trust_products/
+-rw-r--r--   0 runner    (1001) docker     (123)    30206 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trusthub/v1/trust_products/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23131 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.293839 twilio-8.5.0/twilio/rest/verify/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/VerifyBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.297839 twilio-8.5.0/twilio/rest/verify/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/v2/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/v2/safelist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.297839 twilio-8.5.0/twilio/rest/verify/v2/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    55315 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/v2/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/v2/service/access_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.297839 twilio-8.5.0/twilio/rest/verify/v2/service/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/v2/service/entity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.297839 twilio-8.5.0/twilio/rest/verify/v2/service/entity/challenge/
+-rw-r--r--   0 runner    (1001) docker     (123)    34458 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/v2/service/entity/challenge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/v2/service/entity/challenge/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29593 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/v2/service/entity/factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16164 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/v2/service/entity/new_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/v2/service/messaging_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.301839 twilio-8.5.0/twilio/rest/verify/v2/service/rate_limit/
+-rw-r--r--   0 runner    (1001) docker     (123)    21507 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/v2/service/rate_limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22242 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/v2/service/rate_limit/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21805 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/v2/service/verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/v2/service/verification_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25389 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/v2/service/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/v2/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29432 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/v2/verification_attempt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/verify/v2/verification_attempts_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.301839 twilio-8.5.0/twilio/rest/video/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/video/VideoBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/video/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.301839 twilio-8.5.0/twilio/rest/video/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/video/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/video/v1/composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54707 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/video/v1/composition_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/video/v1/composition_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27313 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/video/v1/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/video/v1/recording_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.301839 twilio-8.5.0/twilio/rest/video/v1/room/
+-rw-r--r--   0 runner    (1001) docker     (123)    38074 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/video/v1/room/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.301839 twilio-8.5.0/twilio/rest/video/v1/room/participant/
+-rw-r--r--   0 runner    (1001) docker     (123)    28698 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/video/v1/room/participant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/video/v1/room/participant/anonymize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/video/v1/room/participant/published_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/video/v1/room/participant/subscribe_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17079 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/video/v1/room/participant/subscribed_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/video/v1/room/recording_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24746 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/video/v1/room/room_recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.305839 twilio-8.5.0/twilio/rest/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/voice/VoiceBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/voice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.305839 twilio-8.5.0/twilio/rest/voice/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/voice/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/voice/v1/archived_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37359 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/voice/v1/byoc_trunk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.305839 twilio-8.5.0/twilio/rest/voice/v1/connection_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)    20484 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/voice/v1/connection_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29170 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/voice/v1/connection_policy/connection_policy_target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.305839 twilio-8.5.0/twilio/rest/voice/v1/dialing_permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/voice/v1/dialing_permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.305839 twilio-8.5.0/twilio/rest/voice/v1/dialing_permissions/country/
+-rw-r--r--   0 runner    (1001) docker     (123)    26486 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/voice/v1/dialing_permissions/country/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/voice/v1/dialing_permissions/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20413 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/voice/v1/ip_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19429 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/voice/v1/source_ip_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.305839 twilio-8.5.0/twilio/rest/wireless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/wireless/WirelessBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/wireless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.309839 twilio-8.5.0/twilio/rest/wireless/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/wireless/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27361 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/wireless/v1/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29604 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/wireless/v1/rate_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.309839 twilio-8.5.0/twilio/rest/wireless/v1/sim/
+-rw-r--r--   0 runner    (1001) docker     (123)    46125 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/wireless/v1/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/wireless/v1/sim/data_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/wireless/v1/sim/usage_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/rest/wireless/v1/usage_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.309839 twilio-8.5.0/twilio/twiml/
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/twiml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/twiml/fax_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/twiml/messaging_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82958 2023-07-13 15:32:19.000000 twilio-8.5.0/twilio/twiml/voice_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:32:31.161837 twilio-8.5.0/twilio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-07-13 15:32:31.000000 twilio-8.5.0/twilio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31173 2023-07-13 15:32:31.000000 twilio-8.5.0/twilio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:32:31.000000 twilio-8.5.0/twilio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-13 15:32:31.000000 twilio-8.5.0/twilio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 15:32:31.000000 twilio-8.5.0/twilio.egg-info/top_level.txt
```

### Comparing `twilio-8.4.0/AUTHORS.md` & `twilio-8.5.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/LICENSE` & `twilio-8.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/PKG-INFO` & `twilio-8.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twilio
-Version: 8.4.0
+Version: 8.5.0
 Summary: Twilio API client and TwiML generator
 Home-page: https://github.com/twilio/twilio-python/
 Author: Twilio
 Author-email: help@twilio.com
 Keywords: twilio,twiml
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `twilio-8.4.0/README.md` & `twilio-8.5.0/README.md`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/setup.py` & `twilio-8.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # python setup.py install
 #
 # You need to have the setuptools module installed. Try reading the setuptools
 # documentation: http://pypi.python.org/pypi/setuptools
 
 setup(
     name="twilio",
-    version="8.4.0",
+    version="8.5.0",
     description="Twilio API client and TwiML generator",
     author="Twilio",
     author_email="help@twilio.com",
     url="https://github.com/twilio/twilio-python/",
     keywords=["twilio", "twiml"],
     python_requires=">=3.7.0",
     install_requires=[
```

### Comparing `twilio-8.4.0/twilio/base/client_base.py` & `twilio-8.5.0/twilio/base/client_base.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/base/deserialize.py` & `twilio-8.5.0/twilio/base/deserialize.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/base/domain.py` & `twilio-8.5.0/twilio/base/domain.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/base/exceptions.py` & `twilio-8.5.0/twilio/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/base/obsolete.py` & `twilio-8.5.0/twilio/base/obsolete.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/base/page.py` & `twilio-8.5.0/twilio/base/page.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/base/serialize.py` & `twilio-8.5.0/twilio/base/serialize.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/base/version.py` & `twilio-8.5.0/twilio/base/version.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/http/__init__.py` & `twilio-8.5.0/twilio/http/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/http/async_http_client.py` & `twilio-8.5.0/twilio/http/async_http_client.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/http/http_client.py` & `twilio-8.5.0/twilio/http/http_client.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/http/request.py` & `twilio-8.5.0/twilio/http/request.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/http/response.py` & `twilio-8.5.0/twilio/http/response.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/http/validation_client.py` & `twilio-8.5.0/twilio/http/validation_client.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/jwt/__init__.py` & `twilio-8.5.0/twilio/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/jwt/access_token/__init__.py` & `twilio-8.5.0/twilio/jwt/access_token/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/jwt/access_token/grants.py` & `twilio-8.5.0/twilio/jwt/access_token/grants.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/jwt/client/__init__.py` & `twilio-8.5.0/twilio/jwt/client/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/jwt/taskrouter/__init__.py` & `twilio-8.5.0/twilio/jwt/taskrouter/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/jwt/taskrouter/capabilities.py` & `twilio-8.5.0/twilio/jwt/taskrouter/capabilities.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/jwt/validation/__init__.py` & `twilio-8.5.0/twilio/jwt/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/request_validator.py` & `twilio-8.5.0/twilio/request_validator.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/__init__.py` & `twilio-8.5.0/twilio/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/accounts/AccountsBase.py` & `twilio-8.5.0/twilio/rest/accounts/AccountsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/accounts/__init__.py` & `twilio-8.5.0/twilio/rest/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/accounts/v1/__init__.py` & `twilio-8.5.0/twilio/rest/accounts/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/accounts/v1/auth_token_promotion.py` & `twilio-8.5.0/twilio/rest/accounts/v1/auth_token_promotion.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/accounts/v1/credential/__init__.py` & `twilio-8.5.0/twilio/rest/accounts/v1/credential/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/accounts/v1/credential/aws.py` & `twilio-8.5.0/twilio/rest/accounts/v1/credential/aws.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/accounts/v1/credential/public_key.py` & `twilio-8.5.0/twilio/rest/accounts/v1/credential/public_key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/accounts/v1/secondary_auth_token.py` & `twilio-8.5.0/twilio/rest/accounts/v1/secondary_auth_token.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/ApiBase.py` & `twilio-8.5.0/twilio/rest/api/ApiBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/__init__.py` & `twilio-8.5.0/twilio/rest/api/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/address/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/address/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/address/dependent_phone_number.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/address/dependent_phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/application.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/application.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/authorized_connect_app.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/authorized_connect_app.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/available_phone_number_country/local.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/available_phone_number_country/local.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/available_phone_number_country/national.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/available_phone_number_country/national.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/available_phone_number_country/voip.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/available_phone_number_country/voip.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/balance.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/balance.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/call/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/call/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/call/event.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/call/event.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/call/feedback.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/call/feedback.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/call/feedback_summary.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/call/feedback_summary.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/call/notification.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/call/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/call/payment.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/call/payment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/call/recording.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/call/recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/call/siprec.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/call/siprec.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/call/stream.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/call/stream.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/call/user_defined_message.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/call/user_defined_message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/conference/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/conference/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/conference/participant.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/conference/participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/conference/recording.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/conference/recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/connect_app.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/connect_app.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/incoming_phone_number/local.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/incoming_phone_number/local.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/key.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/message/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/message/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/message/feedback.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/message/feedback.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/message/media.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/message/media.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/new_key.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/new_key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/new_signing_key.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/new_signing_key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/notification.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/outgoing_caller_id.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/outgoing_caller_id.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/queue/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/queue/member.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/queue/member.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/recording/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/recording/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/recording/add_on_result/payload.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/recording/add_on_result/payload.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/recording/transcription.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/recording/transcription.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/short_code.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/short_code.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/signing_key.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/signing_key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/sip/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/sip/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/sip/credential_list/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/sip/credential_list/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/sip/credential_list/credential.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/sip/credential_list/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/token.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/token.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/transcription.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/transcription.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/usage/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/usage/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/usage/record/__init__.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/usage/record/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/usage/record/all_time.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/usage/record/all_time.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/usage/record/daily.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/usage/record/daily.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/usage/record/last_month.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/usage/record/last_month.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/usage/record/monthly.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/usage/record/monthly.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/usage/record/this_month.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/usage/record/this_month.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/usage/record/today.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/usage/record/today.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/usage/record/yearly.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/usage/record/yearly.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/usage/record/yesterday.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/usage/record/yesterday.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/usage/trigger.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/usage/trigger.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/api/v2010/account/validation_request.py` & `twilio-8.5.0/twilio/rest/api/v2010/account/validation_request.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/autopilot/AutopilotBase.py` & `twilio-8.5.0/twilio/rest/autopilot/AutopilotBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/autopilot/__init__.py` & `twilio-8.5.0/twilio/rest/autopilot/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/autopilot/v1/__init__.py` & `twilio-8.5.0/twilio/rest/autopilot/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/autopilot/v1/assistant/__init__.py` & `twilio-8.5.0/twilio/rest/autopilot/v1/assistant/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/autopilot/v1/assistant/defaults.py` & `twilio-8.5.0/twilio/rest/autopilot/v1/assistant/defaults.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/autopilot/v1/assistant/dialogue.py` & `twilio-8.5.0/twilio/rest/autopilot/v1/assistant/dialogue.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/autopilot/v1/assistant/field_type/__init__.py` & `twilio-8.5.0/twilio/rest/autopilot/v1/assistant/field_type/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/autopilot/v1/assistant/field_type/field_value.py` & `twilio-8.5.0/twilio/rest/autopilot/v1/assistant/field_type/field_value.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/autopilot/v1/assistant/model_build.py` & `twilio-8.5.0/twilio/rest/autopilot/v1/assistant/model_build.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/autopilot/v1/assistant/query.py` & `twilio-8.5.0/twilio/rest/autopilot/v1/assistant/query.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/autopilot/v1/assistant/style_sheet.py` & `twilio-8.5.0/twilio/rest/autopilot/v1/assistant/style_sheet.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/autopilot/v1/assistant/task/__init__.py` & `twilio-8.5.0/twilio/rest/autopilot/v1/assistant/task/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/autopilot/v1/assistant/task/field.py` & `twilio-8.5.0/twilio/rest/autopilot/v1/assistant/task/field.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/autopilot/v1/assistant/task/sample.py` & `twilio-8.5.0/twilio/rest/autopilot/v1/assistant/task/sample.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/autopilot/v1/assistant/task/task_actions.py` & `twilio-8.5.0/twilio/rest/autopilot/v1/assistant/task/task_actions.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/autopilot/v1/assistant/task/task_statistics.py` & `twilio-8.5.0/twilio/rest/autopilot/v1/assistant/task/task_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/autopilot/v1/assistant/webhook.py` & `twilio-8.5.0/twilio/rest/autopilot/v1/assistant/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/autopilot/v1/restore_assistant.py` & `twilio-8.5.0/twilio/rest/autopilot/v1/restore_assistant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/bulkexports/BulkexportsBase.py` & `twilio-8.5.0/twilio/rest/bulkexports/BulkexportsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/bulkexports/__init__.py` & `twilio-8.5.0/twilio/rest/bulkexports/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/bulkexports/v1/__init__.py` & `twilio-8.5.0/twilio/rest/bulkexports/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/bulkexports/v1/export/__init__.py` & `twilio-8.5.0/twilio/rest/bulkexports/v1/export/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/bulkexports/v1/export/day.py` & `twilio-8.5.0/twilio/rest/bulkexports/v1/export/day.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/bulkexports/v1/export/export_custom_job.py` & `twilio-8.5.0/twilio/rest/bulkexports/v1/export/export_custom_job.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/bulkexports/v1/export/job.py` & `twilio-8.5.0/twilio/rest/bulkexports/v1/export/job.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/bulkexports/v1/export_configuration.py` & `twilio-8.5.0/twilio/rest/bulkexports/v1/export_configuration.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/ChatBase.py` & `twilio-8.5.0/twilio/rest/chat/ChatBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/__init__.py` & `twilio-8.5.0/twilio/rest/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v1/__init__.py` & `twilio-8.5.0/twilio/rest/chat/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v1/credential.py` & `twilio-8.5.0/twilio/rest/chat/v1/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v1/service/__init__.py` & `twilio-8.5.0/twilio/rest/chat/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v1/service/channel/__init__.py` & `twilio-8.5.0/twilio/rest/chat/v1/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v1/service/channel/invite.py` & `twilio-8.5.0/twilio/rest/chat/v1/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v1/service/channel/member.py` & `twilio-8.5.0/twilio/rest/chat/v1/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v1/service/channel/message.py` & `twilio-8.5.0/twilio/rest/chat/v1/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v1/service/role.py` & `twilio-8.5.0/twilio/rest/chat/v1/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v1/service/user/__init__.py` & `twilio-8.5.0/twilio/rest/chat/v1/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v1/service/user/user_channel.py` & `twilio-8.5.0/twilio/rest/chat/v1/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v2/__init__.py` & `twilio-8.5.0/twilio/rest/chat/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v2/credential.py` & `twilio-8.5.0/twilio/rest/chat/v2/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v2/service/__init__.py` & `twilio-8.5.0/twilio/rest/chat/v2/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v2/service/binding.py` & `twilio-8.5.0/twilio/rest/chat/v2/service/binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v2/service/channel/__init__.py` & `twilio-8.5.0/twilio/rest/chat/v2/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v2/service/channel/invite.py` & `twilio-8.5.0/twilio/rest/chat/v2/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v2/service/channel/member.py` & `twilio-8.5.0/twilio/rest/chat/v2/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v2/service/channel/message.py` & `twilio-8.5.0/twilio/rest/chat/v2/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v2/service/channel/webhook.py` & `twilio-8.5.0/twilio/rest/chat/v2/service/channel/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v2/service/role.py` & `twilio-8.5.0/twilio/rest/chat/v2/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v2/service/user/__init__.py` & `twilio-8.5.0/twilio/rest/chat/v2/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v2/service/user/user_binding.py` & `twilio-8.5.0/twilio/rest/chat/v2/service/user/user_binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v2/service/user/user_channel.py` & `twilio-8.5.0/twilio/rest/chat/v2/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v3/__init__.py` & `twilio-8.5.0/twilio/rest/chat/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/chat/v3/channel.py` & `twilio-8.5.0/twilio/rest/chat/v3/channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/content/ContentBase.py` & `twilio-8.5.0/twilio/rest/content/ContentBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/content/__init__.py` & `twilio-8.5.0/twilio/rest/content/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/content/v1/__init__.py` & `twilio-8.5.0/twilio/rest/content/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/content/v1/content/__init__.py` & `twilio-8.5.0/twilio/rest/content/v1/content/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/content/v1/content/approval_fetch.py` & `twilio-8.5.0/twilio/rest/content/v1/content/approval_fetch.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/content/v1/content_and_approvals.py` & `twilio-8.5.0/twilio/rest/content/v1/content_and_approvals.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/content/v1/legacy_content.py` & `twilio-8.5.0/twilio/rest/content/v1/legacy_content.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/ConversationsBase.py` & `twilio-8.5.0/twilio/rest/conversations/ConversationsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/__init__.py` & `twilio-8.5.0/twilio/rest/conversations/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/__init__.py` & `twilio-8.5.0/twilio/rest/conversations/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/address_configuration.py` & `twilio-8.5.0/twilio/rest/conversations/v1/address_configuration.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/configuration/__init__.py` & `twilio-8.5.0/twilio/rest/conversations/v1/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/configuration/webhook.py` & `twilio-8.5.0/twilio/rest/conversations/v1/configuration/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/conversation/__init__.py` & `twilio-8.5.0/twilio/rest/conversations/v1/conversation/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/conversation/message/__init__.py` & `twilio-8.5.0/twilio/rest/conversations/v1/conversation/message/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py` & `twilio-8.5.0/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/conversation/participant.py` & `twilio-8.5.0/twilio/rest/conversations/v1/conversation/participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/conversation/webhook.py` & `twilio-8.5.0/twilio/rest/conversations/v1/conversation/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/credential.py` & `twilio-8.5.0/twilio/rest/conversations/v1/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/participant_conversation.py` & `twilio-8.5.0/twilio/rest/conversations/v1/participant_conversation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/role.py` & `twilio-8.5.0/twilio/rest/conversations/v1/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/service/__init__.py` & `twilio-8.5.0/twilio/rest/conversations/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/service/binding.py` & `twilio-8.5.0/twilio/rest/conversations/v1/service/binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/service/configuration/__init__.py` & `twilio-8.5.0/twilio/rest/conversations/v1/service/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/service/configuration/notification.py` & `twilio-8.5.0/twilio/rest/conversations/v1/service/configuration/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/service/configuration/webhook.py` & `twilio-8.5.0/twilio/rest/conversations/v1/service/configuration/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/service/conversation/__init__.py` & `twilio-8.5.0/twilio/rest/conversations/v1/service/conversation/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/service/conversation/message/__init__.py` & `twilio-8.5.0/twilio/rest/conversations/v1/service/conversation/message/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py` & `twilio-8.5.0/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/service/conversation/participant.py` & `twilio-8.5.0/twilio/rest/conversations/v1/service/conversation/participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/service/conversation/webhook.py` & `twilio-8.5.0/twilio/rest/conversations/v1/service/conversation/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/service/participant_conversation.py` & `twilio-8.5.0/twilio/rest/conversations/v1/service/participant_conversation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/service/role.py` & `twilio-8.5.0/twilio/rest/conversations/v1/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/service/user/__init__.py` & `twilio-8.5.0/twilio/rest/conversations/v1/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/service/user/user_conversation.py` & `twilio-8.5.0/twilio/rest/conversations/v1/service/user/user_conversation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/user/__init__.py` & `twilio-8.5.0/twilio/rest/conversations/v1/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/conversations/v1/user/user_conversation.py` & `twilio-8.5.0/twilio/rest/conversations/v1/user/user_conversation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/events/EventsBase.py` & `twilio-8.5.0/twilio/rest/events/EventsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/events/__init__.py` & `twilio-8.5.0/twilio/rest/events/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/events/v1/__init__.py` & `twilio-8.5.0/twilio/rest/events/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/events/v1/event_type.py` & `twilio-8.5.0/twilio/rest/events/v1/event_type.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/events/v1/schema/__init__.py` & `twilio-8.5.0/twilio/rest/events/v1/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/events/v1/schema/schema_version.py` & `twilio-8.5.0/twilio/rest/events/v1/schema/schema_version.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/events/v1/sink/__init__.py` & `twilio-8.5.0/twilio/rest/events/v1/sink/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/events/v1/sink/sink_test.py` & `twilio-8.5.0/twilio/rest/events/v1/sink/sink_test.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/events/v1/sink/sink_validate.py` & `twilio-8.5.0/twilio/rest/events/v1/sink/sink_validate.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/events/v1/subscription/__init__.py` & `twilio-8.5.0/twilio/rest/events/v1/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/events/v1/subscription/subscribed_event.py` & `twilio-8.5.0/twilio/rest/events/v1/subscription/subscribed_event.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/FlexApiBase.py` & `twilio-8.5.0/twilio/rest/flex_api/FlexApiBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/__init__.py` & `twilio-8.5.0/twilio/rest/flex_api/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v1/__init__.py` & `twilio-8.5.0/twilio/rest/flex_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v1/assessments.py` & `twilio-8.5.0/twilio/rest/flex_api/v1/assessments.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v1/channel.py` & `twilio-8.5.0/twilio/rest/flex_api/v1/channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v1/configuration.py` & `twilio-8.5.0/twilio/rest/flex_api/v1/configuration.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v1/flex_flow.py` & `twilio-8.5.0/twilio/rest/flex_api/v1/flex_flow.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v1/insights_assessments_comment.py` & `twilio-8.5.0/twilio/rest/flex_api/v1/insights_assessments_comment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v1/insights_conversations.py` & `twilio-8.5.0/twilio/rest/flex_api/v1/insights_conversations.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v1/insights_questionnaires.py` & `twilio-8.5.0/twilio/rest/flex_api/v1/insights_questionnaires.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v1/insights_questionnaires_category.py` & `twilio-8.5.0/twilio/rest/flex_api/v1/insights_questionnaires_category.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v1/insights_questionnaires_question.py` & `twilio-8.5.0/twilio/rest/flex_api/v1/insights_questionnaires_question.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v1/insights_segments.py` & `twilio-8.5.0/twilio/rest/flex_api/v1/insights_segments.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v1/insights_session.py` & `twilio-8.5.0/twilio/rest/flex_api/v1/insights_session.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v1/insights_settings_answer_sets.py` & `twilio-8.5.0/twilio/rest/flex_api/v1/insights_settings_answer_sets.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v1/insights_settings_comment.py` & `twilio-8.5.0/twilio/rest/flex_api/v1/insights_settings_comment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v1/insights_user_roles.py` & `twilio-8.5.0/twilio/rest/flex_api/v1/insights_user_roles.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v1/interaction/__init__.py` & `twilio-8.5.0/twilio/rest/flex_api/v1/interaction/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     NOTE: This class is auto generated by OpenAPI Generator.
     https://openapi-generator.tech
     Do not edit the class manually.
 """
 
 
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Union
 from twilio.base import serialize, values
 from twilio.base.instance_context import InstanceContext
 from twilio.base.instance_resource import InstanceResource
 from twilio.base.list_resource import ListResource
 from twilio.base.version import Version
 
 from twilio.rest.flex_api.v1.interaction.interaction_channel import (
@@ -29,26 +29,30 @@
 
     """
     :ivar sid: The unique string created by Twilio to identify an Interaction resource, prefixed with KD.
     :ivar channel: A JSON object that defines the Interaction’s communication channel and includes details about the channel. See the [Outbound SMS](https://www.twilio.com/docs/flex/developer/conversations/interactions-api/interactions#agent-initiated-outbound-interactions) and [inbound (API-initiated)](https://www.twilio.com/docs/flex/developer/conversations/interactions-api/interactions#api-initiated-contact) Channel object examples.
     :ivar routing: A JSON Object representing the routing rules for the Interaction Channel. See [Outbound SMS Example](https://www.twilio.com/docs/flex/developer/conversations/interactions-api/interactions#agent-initiated-outbound-interactions) for an example Routing object. The Interactions resource uses TaskRouter for all routing functionality.   All attributes in the Routing object on your Interaction request body are added “as is” to the task. For a list of known attributes consumed by the Flex UI and/or Flex Insights, see [Known Task Attributes](https://www.twilio.com/docs/flex/developer/conversations/interactions-api#task-attributes).
     :ivar url:
     :ivar links:
+    :ivar interaction_context_sid:
     """
 
     def __init__(
         self, version: Version, payload: Dict[str, Any], sid: Optional[str] = None
     ):
         super().__init__(version)
 
         self.sid: Optional[str] = payload.get("sid")
         self.channel: Optional[Dict[str, object]] = payload.get("channel")
         self.routing: Optional[Dict[str, object]] = payload.get("routing")
         self.url: Optional[str] = payload.get("url")
         self.links: Optional[Dict[str, object]] = payload.get("links")
+        self.interaction_context_sid: Optional[str] = payload.get(
+            "interaction_context_sid"
+        )
 
         self._solution = {
             "sid": sid or self.sid,
         }
         self._context: Optional[InteractionContext] = None
 
     @property
@@ -187,53 +191,65 @@
         :param version: Version that contains the resource
 
         """
         super().__init__(version)
 
         self._uri = "/Interactions"
 
-    def create(self, channel: object, routing: object) -> InteractionInstance:
+    def create(
+        self,
+        channel: object,
+        routing: object,
+        interaction_context_sid: Union[str, object] = values.unset,
+    ) -> InteractionInstance:
         """
         Create the InteractionInstance
 
         :param channel: The Interaction's channel.
         :param routing: The Interaction's routing logic.
+        :param interaction_context_sid: The Interaction context sid is used for adding a context lookup sid
 
         :returns: The created InteractionInstance
         """
         data = values.of(
             {
                 "Channel": serialize.object(channel),
                 "Routing": serialize.object(routing),
+                "InteractionContextSid": interaction_context_sid,
             }
         )
 
         payload = self._version.create(
             method="POST",
             uri=self._uri,
             data=data,
         )
 
         return InteractionInstance(self._version, payload)
 
     async def create_async(
-        self, channel: object, routing: object
+        self,
+        channel: object,
+        routing: object,
+        interaction_context_sid: Union[str, object] = values.unset,
     ) -> InteractionInstance:
         """
         Asynchronously create the InteractionInstance
 
         :param channel: The Interaction's channel.
         :param routing: The Interaction's routing logic.
+        :param interaction_context_sid: The Interaction context sid is used for adding a context lookup sid
 
         :returns: The created InteractionInstance
         """
         data = values.of(
             {
                 "Channel": serialize.object(channel),
                 "Routing": serialize.object(routing),
+                "InteractionContextSid": interaction_context_sid,
             }
         )
 
         payload = await self._version.create_async(
             method="POST",
             uri=self._uri,
             data=data,
```

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py` & `twilio-8.5.0/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py` & `twilio-8.5.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py` & `twilio-8.5.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v1/web_channel.py` & `twilio-8.5.0/twilio/rest/flex_api/v1/web_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v2/__init__.py` & `twilio-8.5.0/twilio/rest/flex_api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/flex_api/v2/web_channels.py` & `twilio-8.5.0/twilio/rest/flex_api/v2/web_channels.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/frontline_api/FrontlineApiBase.py` & `twilio-8.5.0/twilio/rest/frontline_api/FrontlineApiBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/frontline_api/v1/__init__.py` & `twilio-8.5.0/twilio/rest/frontline_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/frontline_api/v1/user.py` & `twilio-8.5.0/twilio/rest/frontline_api/v1/user.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/insights/InsightsBase.py` & `twilio-8.5.0/twilio/rest/insights/InsightsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/insights/__init__.py` & `twilio-8.5.0/twilio/rest/insights/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/insights/v1/__init__.py` & `twilio-8.5.0/twilio/rest/insights/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/insights/v1/call/__init__.py` & `twilio-8.5.0/twilio/rest/insights/v1/call/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/insights/v1/call/annotation.py` & `twilio-8.5.0/twilio/rest/insights/v1/call/annotation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/insights/v1/call/call_summary.py` & `twilio-8.5.0/twilio/rest/insights/v1/call/call_summary.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/insights/v1/call/event.py` & `twilio-8.5.0/twilio/rest/insights/v1/call/event.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/insights/v1/call/metric.py` & `twilio-8.5.0/twilio/rest/insights/v1/call/metric.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/insights/v1/call_summaries.py` & `twilio-8.5.0/twilio/rest/insights/v1/call_summaries.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/insights/v1/conference/__init__.py` & `twilio-8.5.0/twilio/rest/insights/v1/conference/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/insights/v1/conference/conference_participant.py` & `twilio-8.5.0/twilio/rest/insights/v1/conference/conference_participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/insights/v1/room/__init__.py` & `twilio-8.5.0/twilio/rest/insights/v1/room/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/insights/v1/room/participant.py` & `twilio-8.5.0/twilio/rest/insights/v1/room/participant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/insights/v1/setting.py` & `twilio-8.5.0/twilio/rest/insights/v1/setting.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/IpMessagingBase.py` & `twilio-8.5.0/twilio/rest/ip_messaging/IpMessagingBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/__init__.py` & `twilio-8.5.0/twilio/rest/ip_messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v1/__init__.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v1/credential.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v1/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v1/service/__init__.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v1/service/channel/__init__.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v1/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v1/service/channel/invite.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v1/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v1/service/channel/member.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v1/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v1/service/channel/message.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v1/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v1/service/role.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v1/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v1/service/user/__init__.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v1/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v1/service/user/user_channel.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v1/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v2/__init__.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v2/credential.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v2/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v2/service/__init__.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v2/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v2/service/binding.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v2/service/binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v2/service/channel/__init__.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v2/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v2/service/channel/invite.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v2/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v2/service/channel/member.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v2/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v2/service/channel/message.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v2/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v2/service/channel/webhook.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v2/service/channel/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v2/service/role.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v2/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v2/service/user/__init__.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v2/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v2/service/user/user_binding.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v2/service/user/user_binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/ip_messaging/v2/service/user/user_channel.py` & `twilio-8.5.0/twilio/rest/ip_messaging/v2/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/lookups/LookupsBase.py` & `twilio-8.5.0/twilio/rest/lookups/LookupsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/lookups/v1/__init__.py` & `twilio-8.5.0/twilio/rest/lookups/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/lookups/v1/phone_number.py` & `twilio-8.5.0/twilio/rest/lookups/v1/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/lookups/v2/__init__.py` & `twilio-8.5.0/twilio/rest/lookups/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/lookups/v2/phone_number.py` & `twilio-8.5.0/twilio/rest/lookups/v2/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/media/MediaBase.py` & `twilio-8.5.0/twilio/rest/media/MediaBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/media/__init__.py` & `twilio-8.5.0/twilio/rest/media/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/media/v1/__init__.py` & `twilio-8.5.0/twilio/rest/media/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/media/v1/media_processor.py` & `twilio-8.5.0/twilio/rest/media/v1/media_processor.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/media/v1/media_recording.py` & `twilio-8.5.0/twilio/rest/media/v1/media_recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/media/v1/player_streamer/__init__.py` & `twilio-8.5.0/twilio/rest/media/v1/player_streamer/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/media/v1/player_streamer/playback_grant.py` & `twilio-8.5.0/twilio/rest/media/v1/player_streamer/playback_grant.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/messaging/MessagingBase.py` & `twilio-8.5.0/twilio/rest/messaging/MessagingBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/messaging/__init__.py` & `twilio-8.5.0/twilio/rest/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/messaging/v1/__init__.py` & `twilio-8.5.0/twilio/rest/messaging/v1/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from twilio.rest.messaging.v1.linkshortening_messaging_service import (
     LinkshorteningMessagingServiceList,
 )
 from twilio.rest.messaging.v1.linkshortening_messaging_service_domain_association import (
     LinkshorteningMessagingServiceDomainAssociationList,
 )
 from twilio.rest.messaging.v1.service import ServiceList
+from twilio.rest.messaging.v1.tollfree_verification import TollfreeVerificationList
 from twilio.rest.messaging.v1.usecase import UsecaseList
 
 
 class V1(Version):
     def __init__(self, domain: Domain):
         """
         Initialize the V1 version of Messaging
@@ -52,14 +53,15 @@
         self._linkshortening_messaging_service: Optional[
             LinkshorteningMessagingServiceList
         ] = None
         self._linkshortening_messaging_service_domain_association: Optional[
             LinkshorteningMessagingServiceDomainAssociationList
         ] = None
         self._services: Optional[ServiceList] = None
+        self._tollfree_verifications: Optional[TollfreeVerificationList] = None
         self._usecases: Optional[UsecaseList] = None
 
     @property
     def brand_registrations(self) -> BrandRegistrationList:
         if self._brand_registrations is None:
             self._brand_registrations = BrandRegistrationList(self)
         return self._brand_registrations
@@ -117,14 +119,20 @@
     @property
     def services(self) -> ServiceList:
         if self._services is None:
             self._services = ServiceList(self)
         return self._services
 
     @property
+    def tollfree_verifications(self) -> TollfreeVerificationList:
+        if self._tollfree_verifications is None:
+            self._tollfree_verifications = TollfreeVerificationList(self)
+        return self._tollfree_verifications
+
+    @property
     def usecases(self) -> UsecaseList:
         if self._usecases is None:
             self._usecases = UsecaseList(self)
         return self._usecases
 
     def __repr__(self) -> str:
         """
```

### Comparing `twilio-8.4.0/twilio/rest/messaging/v1/brand_registration/__init__.py` & `twilio-8.5.0/twilio/rest/messaging/v1/brand_registration/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py` & `twilio-8.5.0/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/messaging/v1/brand_registration/brand_vetting.py` & `twilio-8.5.0/twilio/rest/messaging/v1/brand_registration/brand_vetting.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/messaging/v1/deactivations.py` & `twilio-8.5.0/twilio/rest/messaging/v1/deactivations.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/messaging/v1/domain_certs.py` & `twilio-8.5.0/twilio/rest/messaging/v1/domain_certs.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/messaging/v1/domain_config.py` & `twilio-8.5.0/twilio/rest/messaging/v1/domain_config.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/messaging/v1/domain_config_messaging_service.py` & `twilio-8.5.0/twilio/rest/messaging/v1/domain_config_messaging_service.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/messaging/v1/external_campaign.py` & `twilio-8.5.0/twilio/rest/messaging/v1/external_campaign.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/messaging/v1/linkshortening_messaging_service.py` & `twilio-8.5.0/twilio/rest/messaging/v1/linkshortening_messaging_service.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/messaging/v1/linkshortening_messaging_service_domain_association.py` & `twilio-8.5.0/twilio/rest/messaging/v1/linkshortening_messaging_service_domain_association.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/messaging/v1/service/__init__.py` & `twilio-8.5.0/twilio/rest/messaging/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/messaging/v1/service/alpha_sender.py` & `twilio-8.5.0/twilio/rest/messaging/v1/service/alpha_sender.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/messaging/v1/service/phone_number.py` & `twilio-8.5.0/twilio/rest/messaging/v1/service/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/messaging/v1/service/short_code.py` & `twilio-8.5.0/twilio/rest/messaging/v1/service/short_code.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/messaging/v1/service/us_app_to_person.py` & `twilio-8.5.0/twilio/rest/messaging/v1/service/us_app_to_person.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py` & `twilio-8.5.0/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/messaging/v1/usecase.py` & `twilio-8.5.0/twilio/rest/messaging/v1/usecase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/microvisor/MicrovisorBase.py` & `twilio-8.5.0/twilio/rest/microvisor/MicrovisorBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/microvisor/__init__.py` & `twilio-8.5.0/twilio/rest/microvisor/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/microvisor/v1/__init__.py` & `twilio-8.5.0/twilio/rest/microvisor/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/microvisor/v1/account_config.py` & `twilio-8.5.0/twilio/rest/microvisor/v1/account_config.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/microvisor/v1/account_secret.py` & `twilio-8.5.0/twilio/rest/microvisor/v1/account_secret.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/microvisor/v1/app/__init__.py` & `twilio-8.5.0/twilio/rest/microvisor/v1/app/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/microvisor/v1/app/app_manifest.py` & `twilio-8.5.0/twilio/rest/microvisor/v1/app/app_manifest.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/microvisor/v1/device/__init__.py` & `twilio-8.5.0/twilio/rest/microvisor/v1/device/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -97,49 +97,55 @@
         return await self._proxy.fetch_async()
 
     def update(
         self,
         unique_name: Union[str, object] = values.unset,
         target_app: Union[str, object] = values.unset,
         logging_enabled: Union[bool, object] = values.unset,
+        restart_app: Union[bool, object] = values.unset,
     ) -> "DeviceInstance":
         """
         Update the DeviceInstance
 
         :param unique_name: A unique and addressable name to be assigned to this Device by the developer. It may be used in place of the Device SID.
         :param target_app: The SID or unique name of the App to be targeted to the Device.
         :param logging_enabled: A Boolean flag specifying whether to enable application logging. Logs will be enabled or extended for 24 hours.
+        :param restart_app: Set to true to restart the App running on the Device.
 
         :returns: The updated DeviceInstance
         """
         return self._proxy.update(
             unique_name=unique_name,
             target_app=target_app,
             logging_enabled=logging_enabled,
+            restart_app=restart_app,
         )
 
     async def update_async(
         self,
         unique_name: Union[str, object] = values.unset,
         target_app: Union[str, object] = values.unset,
         logging_enabled: Union[bool, object] = values.unset,
+        restart_app: Union[bool, object] = values.unset,
     ) -> "DeviceInstance":
         """
         Asynchronous coroutine to update the DeviceInstance
 
         :param unique_name: A unique and addressable name to be assigned to this Device by the developer. It may be used in place of the Device SID.
         :param target_app: The SID or unique name of the App to be targeted to the Device.
         :param logging_enabled: A Boolean flag specifying whether to enable application logging. Logs will be enabled or extended for 24 hours.
+        :param restart_app: Set to true to restart the App running on the Device.
 
         :returns: The updated DeviceInstance
         """
         return await self._proxy.update_async(
             unique_name=unique_name,
             target_app=target_app,
             logging_enabled=logging_enabled,
+            restart_app=restart_app,
         )
 
     @property
     def device_configs(self) -> DeviceConfigList:
         """
         Access the device_configs
         """
@@ -220,29 +226,32 @@
         )
 
     def update(
         self,
         unique_name: Union[str, object] = values.unset,
         target_app: Union[str, object] = values.unset,
         logging_enabled: Union[bool, object] = values.unset,
+        restart_app: Union[bool, object] = values.unset,
     ) -> DeviceInstance:
         """
         Update the DeviceInstance
 
         :param unique_name: A unique and addressable name to be assigned to this Device by the developer. It may be used in place of the Device SID.
         :param target_app: The SID or unique name of the App to be targeted to the Device.
         :param logging_enabled: A Boolean flag specifying whether to enable application logging. Logs will be enabled or extended for 24 hours.
+        :param restart_app: Set to true to restart the App running on the Device.
 
         :returns: The updated DeviceInstance
         """
         data = values.of(
             {
                 "UniqueName": unique_name,
                 "TargetApp": target_app,
                 "LoggingEnabled": logging_enabled,
+                "RestartApp": restart_app,
             }
         )
 
         payload = self._version.update(
             method="POST",
             uri=self._uri,
             data=data,
@@ -251,29 +260,32 @@
         return DeviceInstance(self._version, payload, sid=self._solution["sid"])
 
     async def update_async(
         self,
         unique_name: Union[str, object] = values.unset,
         target_app: Union[str, object] = values.unset,
         logging_enabled: Union[bool, object] = values.unset,
+        restart_app: Union[bool, object] = values.unset,
     ) -> DeviceInstance:
         """
         Asynchronous coroutine to update the DeviceInstance
 
         :param unique_name: A unique and addressable name to be assigned to this Device by the developer. It may be used in place of the Device SID.
         :param target_app: The SID or unique name of the App to be targeted to the Device.
         :param logging_enabled: A Boolean flag specifying whether to enable application logging. Logs will be enabled or extended for 24 hours.
+        :param restart_app: Set to true to restart the App running on the Device.
 
         :returns: The updated DeviceInstance
         """
         data = values.of(
             {
                 "UniqueName": unique_name,
                 "TargetApp": target_app,
                 "LoggingEnabled": logging_enabled,
+                "RestartApp": restart_app,
             }
         )
 
         payload = await self._version.update_async(
             method="POST",
             uri=self._uri,
             data=data,
```

### Comparing `twilio-8.4.0/twilio/rest/microvisor/v1/device/device_config.py` & `twilio-8.5.0/twilio/rest/microvisor/v1/device/device_config.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/microvisor/v1/device/device_secret.py` & `twilio-8.5.0/twilio/rest/microvisor/v1/device/device_secret.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/monitor/MonitorBase.py` & `twilio-8.5.0/twilio/rest/monitor/MonitorBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/monitor/__init__.py` & `twilio-8.5.0/twilio/rest/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/monitor/v1/__init__.py` & `twilio-8.5.0/twilio/rest/monitor/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/monitor/v1/alert.py` & `twilio-8.5.0/twilio/rest/monitor/v1/alert.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/monitor/v1/event.py` & `twilio-8.5.0/twilio/rest/monitor/v1/event.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/notify/NotifyBase.py` & `twilio-8.5.0/twilio/rest/notify/NotifyBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/notify/__init__.py` & `twilio-8.5.0/twilio/rest/notify/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/notify/v1/__init__.py` & `twilio-8.5.0/twilio/rest/notify/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/notify/v1/credential.py` & `twilio-8.5.0/twilio/rest/notify/v1/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/notify/v1/service/__init__.py` & `twilio-8.5.0/twilio/rest/notify/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/notify/v1/service/binding.py` & `twilio-8.5.0/twilio/rest/notify/v1/service/binding.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/notify/v1/service/notification.py` & `twilio-8.5.0/twilio/rest/notify/v1/service/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/numbers/NumbersBase.py` & `twilio-8.5.0/twilio/rest/numbers/NumbersBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/numbers/v1/__init__.py` & `twilio-8.5.0/twilio/rest/numbers/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/numbers/v1/bulk_eligibility.py` & `twilio-8.5.0/twilio/rest/numbers/v1/bulk_eligibility.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/numbers/v1/porting_bulk_portability.py` & `twilio-8.5.0/twilio/rest/numbers/v1/porting_bulk_portability.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/numbers/v1/porting_portability.py` & `twilio-8.5.0/twilio/rest/numbers/v1/porting_portability.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/numbers/v2/__init__.py` & `twilio-8.5.0/twilio/rest/numbers/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/numbers/v2/authorization_document/__init__.py` & `twilio-8.5.0/twilio/rest/numbers/v2/authorization_document/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,33 +277,38 @@
         self._uri = "/HostedNumber/AuthorizationDocuments"
 
     def create(
         self,
         address_sid: str,
         email: str,
         contact_phone_number: str,
+        hosted_number_order_sids: List[str],
         contact_title: Union[str, object] = values.unset,
         cc_emails: Union[List[str], object] = values.unset,
     ) -> AuthorizationDocumentInstance:
         """
         Create the AuthorizationDocumentInstance
 
         :param address_sid: A 34 character string that uniquely identifies the Address resource that is associated with this AuthorizationDocument.
         :param email: Email that this AuthorizationDocument will be sent to for signing.
         :param contact_phone_number: The contact phone number of the person authorized to sign the Authorization Document.
+        :param hosted_number_order_sids: A list of HostedNumberOrder sids that this AuthorizationDocument will authorize for hosting phone number capabilities on Twilio's platform.
         :param contact_title: The title of the person authorized to sign the Authorization Document for this phone number.
         :param cc_emails: Email recipients who will be informed when an Authorization Document has been sent and signed.
 
         :returns: The created AuthorizationDocumentInstance
         """
         data = values.of(
             {
                 "AddressSid": address_sid,
                 "Email": email,
                 "ContactPhoneNumber": contact_phone_number,
+                "HostedNumberOrderSids": serialize.map(
+                    hosted_number_order_sids, lambda e: e
+                ),
                 "ContactTitle": contact_title,
                 "CcEmails": serialize.map(cc_emails, lambda e: e),
             }
         )
 
         payload = self._version.create(
             method="POST",
@@ -314,33 +319,38 @@
         return AuthorizationDocumentInstance(self._version, payload)
 
     async def create_async(
         self,
         address_sid: str,
         email: str,
         contact_phone_number: str,
+        hosted_number_order_sids: List[str],
         contact_title: Union[str, object] = values.unset,
         cc_emails: Union[List[str], object] = values.unset,
     ) -> AuthorizationDocumentInstance:
         """
         Asynchronously create the AuthorizationDocumentInstance
 
         :param address_sid: A 34 character string that uniquely identifies the Address resource that is associated with this AuthorizationDocument.
         :param email: Email that this AuthorizationDocument will be sent to for signing.
         :param contact_phone_number: The contact phone number of the person authorized to sign the Authorization Document.
+        :param hosted_number_order_sids: A list of HostedNumberOrder sids that this AuthorizationDocument will authorize for hosting phone number capabilities on Twilio's platform.
         :param contact_title: The title of the person authorized to sign the Authorization Document for this phone number.
         :param cc_emails: Email recipients who will be informed when an Authorization Document has been sent and signed.
 
         :returns: The created AuthorizationDocumentInstance
         """
         data = values.of(
             {
                 "AddressSid": address_sid,
                 "Email": email,
                 "ContactPhoneNumber": contact_phone_number,
+                "HostedNumberOrderSids": serialize.map(
+                    hosted_number_order_sids, lambda e: e
+                ),
                 "ContactTitle": contact_title,
                 "CcEmails": serialize.map(cc_emails, lambda e: e),
             }
         )
 
         payload = await self._version.create_async(
             method="POST",
```

### Comparing `twilio-8.4.0/twilio/rest/numbers/v2/authorization_document/dependent_hosted_number_order.py` & `twilio-8.5.0/twilio/rest/numbers/v2/authorization_document/dependent_hosted_number_order.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/numbers/v2/hosted_number_order.py` & `twilio-8.5.0/twilio/rest/numbers/v2/hosted_number_order.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     :ivar signing_document_sid: A 34 character string that uniquely identifies the [Authorization Document](https://www.twilio.com/docs/api/phone-numbers/hosted-number-authorization-documents) the user needs to sign.
     :ivar phone_number: Phone number to be hosted. This must be in [E.164](https://en.wikipedia.org/wiki/E.164) format, e.g., +16175551212
     :ivar capabilities: 
     :ivar friendly_name: A 64 character string that is a human-readable text that describes this resource.
     :ivar status: 
     :ivar failure_reason: A message that explains why a hosted_number_order went to status \"action-required\"
     :ivar date_created: The date this resource was created, given as [GMT RFC 2822](http://www.ietf.org/rfc/rfc2822.txt) format.
-    :ivar sms_capability: Whether the SMS capability will be hosted on our platform. Can be `true` of `false`.
     :ivar date_updated: The date that this resource was updated, given as [GMT RFC 2822](http://www.ietf.org/rfc/rfc2822.txt) format.
     :ivar email: Email of the owner of this phone number that is being hosted.
     :ivar cc_emails: A list of emails that LOA document for this HostedNumberOrder will be carbon copied to.
     :ivar url: The URL of this HostedNumberOrder.
     :ivar contact_title: The title of the person authorized to sign the Authorization Document for this phone number.
     :ivar contact_phone_number: The contact phone number of the person authorized to sign the Authorization Document.
     :ivar bulk_hosting_request_sid: A 34 character string that uniquely identifies the bulk hosting request associated with this HostedNumberOrder.
@@ -74,15 +73,14 @@
         self.status: Optional["HostedNumberOrderInstance.Status"] = payload.get(
             "status"
         )
         self.failure_reason: Optional[str] = payload.get("failure_reason")
         self.date_created: Optional[datetime] = deserialize.iso8601_datetime(
             payload.get("date_created")
         )
-        self.sms_capability: Optional[bool] = payload.get("sms_capability")
         self.date_updated: Optional[datetime] = deserialize.iso8601_datetime(
             payload.get("date_updated")
         )
         self.email: Optional[str] = payload.get("email")
         self.cc_emails: Optional[List[str]] = payload.get("cc_emails")
         self.url: Optional[str] = payload.get("url")
         self.contact_title: Optional[str] = payload.get("contact_title")
```

### Comparing `twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/__init__.py` & `twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py` & `twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py` & `twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py` & `twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py` & `twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py` & `twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/end_user.py` & `twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/end_user.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py` & `twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/regulation.py` & `twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/regulation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py` & `twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py` & `twilio-8.5.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/oauth/OauthBase.py` & `twilio-8.5.0/twilio/rest/oauth/OauthBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/oauth/__init__.py` & `twilio-8.5.0/twilio/rest/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/oauth/v1/__init__.py` & `twilio-8.5.0/twilio/rest/oauth/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/oauth/v1/device_code.py` & `twilio-8.5.0/twilio/rest/oauth/v1/device_code.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/oauth/v1/oauth.py` & `twilio-8.5.0/twilio/rest/oauth/v1/oauth.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/oauth/v1/openid_discovery.py` & `twilio-8.5.0/twilio/rest/oauth/v1/openid_discovery.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/oauth/v1/token.py` & `twilio-8.5.0/twilio/rest/oauth/v1/token.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/oauth/v1/user_info.py` & `twilio-8.5.0/twilio/rest/oauth/v1/user_info.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/PreviewBase.py` & `twilio-8.5.0/twilio/rest/preview/PreviewBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/__init__.py` & `twilio-8.5.0/twilio/rest/preview/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/deployed_devices/__init__.py` & `twilio-8.5.0/twilio/rest/preview/deployed_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/deployed_devices/fleet/__init__.py` & `twilio-8.5.0/twilio/rest/preview/deployed_devices/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/deployed_devices/fleet/certificate.py` & `twilio-8.5.0/twilio/rest/preview/deployed_devices/fleet/certificate.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/deployed_devices/fleet/deployment.py` & `twilio-8.5.0/twilio/rest/preview/deployed_devices/fleet/deployment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/deployed_devices/fleet/device.py` & `twilio-8.5.0/twilio/rest/preview/deployed_devices/fleet/device.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/deployed_devices/fleet/key.py` & `twilio-8.5.0/twilio/rest/preview/deployed_devices/fleet/key.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/hosted_numbers/__init__.py` & `twilio-8.5.0/twilio/rest/preview/hosted_numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py` & `twilio-8.5.0/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py` & `twilio-8.5.0/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/hosted_numbers/hosted_number_order.py` & `twilio-8.5.0/twilio/rest/preview/hosted_numbers/hosted_number_order.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/marketplace/__init__.py` & `twilio-8.5.0/twilio/rest/preview/marketplace/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/marketplace/available_add_on/__init__.py` & `twilio-8.5.0/twilio/rest/preview/marketplace/available_add_on/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py` & `twilio-8.5.0/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/marketplace/installed_add_on/__init__.py` & `twilio-8.5.0/twilio/rest/preview/marketplace/installed_add_on/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py` & `twilio-8.5.0/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/sync/__init__.py` & `twilio-8.5.0/twilio/rest/preview/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/sync/service/__init__.py` & `twilio-8.5.0/twilio/rest/preview/sync/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/sync/service/document/__init__.py` & `twilio-8.5.0/twilio/rest/preview/sync/service/document/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/sync/service/document/document_permission.py` & `twilio-8.5.0/twilio/rest/preview/sync/service/document/document_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/sync/service/sync_list/__init__.py` & `twilio-8.5.0/twilio/rest/preview/sync/service/sync_list/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/sync/service/sync_list/sync_list_item.py` & `twilio-8.5.0/twilio/rest/preview/sync/service/sync_list/sync_list_item.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py` & `twilio-8.5.0/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/sync/service/sync_map/__init__.py` & `twilio-8.5.0/twilio/rest/preview/sync/service/sync_map/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/sync/service/sync_map/sync_map_item.py` & `twilio-8.5.0/twilio/rest/preview/sync/service/sync_map/sync_map_item.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py` & `twilio-8.5.0/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/understand/__init__.py` & `twilio-8.5.0/twilio/rest/preview/understand/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/understand/assistant/__init__.py` & `twilio-8.5.0/twilio/rest/preview/understand/assistant/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/understand/assistant/assistant_fallback_actions.py` & `twilio-8.5.0/twilio/rest/preview/understand/assistant/assistant_fallback_actions.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/understand/assistant/assistant_initiation_actions.py` & `twilio-8.5.0/twilio/rest/preview/understand/assistant/assistant_initiation_actions.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/understand/assistant/dialogue.py` & `twilio-8.5.0/twilio/rest/preview/understand/assistant/dialogue.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/understand/assistant/field_type/__init__.py` & `twilio-8.5.0/twilio/rest/preview/understand/assistant/field_type/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/understand/assistant/field_type/field_value.py` & `twilio-8.5.0/twilio/rest/preview/understand/assistant/field_type/field_value.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/understand/assistant/model_build.py` & `twilio-8.5.0/twilio/rest/preview/understand/assistant/model_build.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/understand/assistant/query.py` & `twilio-8.5.0/twilio/rest/preview/understand/assistant/query.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/understand/assistant/style_sheet.py` & `twilio-8.5.0/twilio/rest/preview/understand/assistant/style_sheet.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/understand/assistant/task/__init__.py` & `twilio-8.5.0/twilio/rest/preview/understand/assistant/task/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/understand/assistant/task/field.py` & `twilio-8.5.0/twilio/rest/preview/understand/assistant/task/field.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/understand/assistant/task/sample.py` & `twilio-8.5.0/twilio/rest/preview/understand/assistant/task/sample.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/understand/assistant/task/task_actions.py` & `twilio-8.5.0/twilio/rest/preview/understand/assistant/task/task_actions.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/understand/assistant/task/task_statistics.py` & `twilio-8.5.0/twilio/rest/preview/understand/assistant/task/task_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/wireless/__init__.py` & `twilio-8.5.0/twilio/rest/preview/wireless/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/wireless/command.py` & `twilio-8.5.0/twilio/rest/preview/wireless/command.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/wireless/rate_plan.py` & `twilio-8.5.0/twilio/rest/preview/wireless/rate_plan.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/wireless/sim/__init__.py` & `twilio-8.5.0/twilio/rest/preview/wireless/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/preview/wireless/sim/usage.py` & `twilio-8.5.0/twilio/rest/preview/wireless/sim/usage.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/pricing/PricingBase.py` & `twilio-8.5.0/twilio/rest/pricing/PricingBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/pricing/__init__.py` & `twilio-8.5.0/twilio/rest/pricing/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/pricing/v1/__init__.py` & `twilio-8.5.0/twilio/rest/pricing/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/pricing/v1/messaging/__init__.py` & `twilio-8.5.0/twilio/rest/pricing/v1/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/pricing/v1/messaging/country.py` & `twilio-8.5.0/twilio/rest/pricing/v1/messaging/country.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/pricing/v1/phone_number/__init__.py` & `twilio-8.5.0/twilio/rest/pricing/v1/phone_number/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/pricing/v1/phone_number/country.py` & `twilio-8.5.0/twilio/rest/pricing/v1/phone_number/country.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/pricing/v1/voice/__init__.py` & `twilio-8.5.0/twilio/rest/pricing/v1/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/pricing/v1/voice/country.py` & `twilio-8.5.0/twilio/rest/pricing/v1/voice/country.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/pricing/v1/voice/number.py` & `twilio-8.5.0/twilio/rest/pricing/v1/voice/number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/pricing/v2/__init__.py` & `twilio-8.5.0/twilio/rest/pricing/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/pricing/v2/country.py` & `twilio-8.5.0/twilio/rest/pricing/v2/country.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/pricing/v2/number.py` & `twilio-8.5.0/twilio/rest/pricing/v2/number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/pricing/v2/voice/__init__.py` & `twilio-8.5.0/twilio/rest/pricing/v2/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/pricing/v2/voice/country.py` & `twilio-8.5.0/twilio/rest/pricing/v2/voice/country.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/pricing/v2/voice/number.py` & `twilio-8.5.0/twilio/rest/pricing/v2/voice/number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/proxy/ProxyBase.py` & `twilio-8.5.0/twilio/rest/proxy/ProxyBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/proxy/v1/__init__.py` & `twilio-8.5.0/twilio/rest/proxy/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/proxy/v1/service/__init__.py` & `twilio-8.5.0/twilio/rest/proxy/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/proxy/v1/service/phone_number.py` & `twilio-8.5.0/twilio/rest/proxy/v1/service/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/proxy/v1/service/session/__init__.py` & `twilio-8.5.0/twilio/rest/proxy/v1/service/session/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/proxy/v1/service/session/interaction.py` & `twilio-8.5.0/twilio/rest/proxy/v1/service/session/interaction.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/proxy/v1/service/session/participant/__init__.py` & `twilio-8.5.0/twilio/rest/proxy/v1/service/session/participant/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/proxy/v1/service/session/participant/message_interaction.py` & `twilio-8.5.0/twilio/rest/proxy/v1/service/session/participant/message_interaction.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/proxy/v1/service/short_code.py` & `twilio-8.5.0/twilio/rest/proxy/v1/service/short_code.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/routes/RoutesBase.py` & `twilio-8.5.0/twilio/rest/routes/RoutesBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/routes/__init__.py` & `twilio-8.5.0/twilio/rest/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/routes/v2/__init__.py` & `twilio-8.5.0/twilio/rest/routes/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/routes/v2/phone_number.py` & `twilio-8.5.0/twilio/rest/routes/v2/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/routes/v2/sip_domain.py` & `twilio-8.5.0/twilio/rest/routes/v2/sip_domain.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/routes/v2/trunk.py` & `twilio-8.5.0/twilio/rest/routes/v2/trunk.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/serverless/ServerlessBase.py` & `twilio-8.5.0/twilio/rest/serverless/ServerlessBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/serverless/v1/__init__.py` & `twilio-8.5.0/twilio/rest/serverless/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/serverless/v1/service/__init__.py` & `twilio-8.5.0/twilio/rest/serverless/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/serverless/v1/service/asset/__init__.py` & `twilio-8.5.0/twilio/rest/serverless/v1/service/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/serverless/v1/service/asset/asset_version.py` & `twilio-8.5.0/twilio/rest/serverless/v1/service/asset/asset_version.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/serverless/v1/service/build/__init__.py` & `twilio-8.5.0/twilio/rest/serverless/v1/service/build/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/serverless/v1/service/build/build_status.py` & `twilio-8.5.0/twilio/rest/serverless/v1/service/build/build_status.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/serverless/v1/service/environment/__init__.py` & `twilio-8.5.0/twilio/rest/serverless/v1/service/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/serverless/v1/service/environment/deployment.py` & `twilio-8.5.0/twilio/rest/serverless/v1/service/environment/deployment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/serverless/v1/service/environment/log.py` & `twilio-8.5.0/twilio/rest/serverless/v1/service/environment/log.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/serverless/v1/service/environment/variable.py` & `twilio-8.5.0/twilio/rest/serverless/v1/service/environment/variable.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/serverless/v1/service/function/__init__.py` & `twilio-8.5.0/twilio/rest/serverless/v1/service/function/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/serverless/v1/service/function/function_version/__init__.py` & `twilio-8.5.0/twilio/rest/serverless/v1/service/function/function_version/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py` & `twilio-8.5.0/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/StudioBase.py` & `twilio-8.5.0/twilio/rest/studio/StudioBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/__init__.py` & `twilio-8.5.0/twilio/rest/studio/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/v1/__init__.py` & `twilio-8.5.0/twilio/rest/studio/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/v1/flow/__init__.py` & `twilio-8.5.0/twilio/rest/studio/v1/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/v1/flow/engagement/__init__.py` & `twilio-8.5.0/twilio/rest/studio/v1/flow/engagement/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/v1/flow/engagement/engagement_context.py` & `twilio-8.5.0/twilio/rest/studio/v1/flow/engagement/engagement_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/v1/flow/engagement/step/__init__.py` & `twilio-8.5.0/twilio/rest/studio/v1/flow/engagement/step/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/v1/flow/engagement/step/step_context.py` & `twilio-8.5.0/twilio/rest/studio/v1/flow/engagement/step/step_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/v1/flow/execution/__init__.py` & `twilio-8.5.0/twilio/rest/studio/v1/flow/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/v1/flow/execution/execution_context.py` & `twilio-8.5.0/twilio/rest/studio/v1/flow/execution/execution_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py` & `twilio-8.5.0/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py` & `twilio-8.5.0/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/v2/__init__.py` & `twilio-8.5.0/twilio/rest/studio/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/v2/flow/__init__.py` & `twilio-8.5.0/twilio/rest/studio/v2/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/v2/flow/execution/__init__.py` & `twilio-8.5.0/twilio/rest/studio/v2/flow/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/v2/flow/execution/execution_context.py` & `twilio-8.5.0/twilio/rest/studio/v2/flow/execution/execution_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py` & `twilio-8.5.0/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py` & `twilio-8.5.0/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/v2/flow/flow_revision.py` & `twilio-8.5.0/twilio/rest/studio/v2/flow/flow_revision.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/v2/flow/flow_test_user.py` & `twilio-8.5.0/twilio/rest/studio/v2/flow/flow_test_user.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/studio/v2/flow_validate.py` & `twilio-8.5.0/twilio/rest/studio/v2/flow_validate.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/supersim/SupersimBase.py` & `twilio-8.5.0/twilio/rest/supersim/SupersimBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/supersim/__init__.py` & `twilio-8.5.0/twilio/rest/supersim/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/supersim/v1/__init__.py` & `twilio-8.5.0/twilio/rest/supersim/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/supersim/v1/esim_profile.py` & `twilio-8.5.0/twilio/rest/supersim/v1/esim_profile.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/supersim/v1/fleet.py` & `twilio-8.5.0/twilio/rest/supersim/v1/fleet.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/supersim/v1/ip_command.py` & `twilio-8.5.0/twilio/rest/supersim/v1/ip_command.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/supersim/v1/network.py` & `twilio-8.5.0/twilio/rest/supersim/v1/network.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/supersim/v1/network_access_profile/__init__.py` & `twilio-8.5.0/twilio/rest/supersim/v1/network_access_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py` & `twilio-8.5.0/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/supersim/v1/settings_update.py` & `twilio-8.5.0/twilio/rest/supersim/v1/settings_update.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/supersim/v1/sim/__init__.py` & `twilio-8.5.0/twilio/rest/supersim/v1/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/supersim/v1/sim/billing_period.py` & `twilio-8.5.0/twilio/rest/supersim/v1/sim/billing_period.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/supersim/v1/sim/sim_ip_address.py` & `twilio-8.5.0/twilio/rest/supersim/v1/sim/sim_ip_address.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/supersim/v1/sms_command.py` & `twilio-8.5.0/twilio/rest/supersim/v1/sms_command.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/supersim/v1/usage_record.py` & `twilio-8.5.0/twilio/rest/supersim/v1/usage_record.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/sync/SyncBase.py` & `twilio-8.5.0/twilio/rest/sync/SyncBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/sync/v1/__init__.py` & `twilio-8.5.0/twilio/rest/sync/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/sync/v1/service/__init__.py` & `twilio-8.5.0/twilio/rest/sync/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/sync/v1/service/document/__init__.py` & `twilio-8.5.0/twilio/rest/sync/v1/service/document/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/sync/v1/service/document/document_permission.py` & `twilio-8.5.0/twilio/rest/sync/v1/service/document/document_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/sync/v1/service/sync_list/__init__.py` & `twilio-8.5.0/twilio/rest/sync/v1/service/sync_list/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/sync/v1/service/sync_list/sync_list_item.py` & `twilio-8.5.0/twilio/rest/sync/v1/service/sync_list/sync_list_item.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py` & `twilio-8.5.0/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/sync/v1/service/sync_map/__init__.py` & `twilio-8.5.0/twilio/rest/sync/v1/service/sync_map/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/sync/v1/service/sync_map/sync_map_item.py` & `twilio-8.5.0/twilio/rest/sync/v1/service/sync_map/sync_map_item.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py` & `twilio-8.5.0/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/sync/v1/service/sync_stream/__init__.py` & `twilio-8.5.0/twilio/rest/sync/v1/service/sync_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/sync/v1/service/sync_stream/stream_message.py` & `twilio-8.5.0/twilio/rest/sync/v1/service/sync_stream/stream_message.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/TaskrouterBase.py` & `twilio-8.5.0/twilio/rest/taskrouter/TaskrouterBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/__init__.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/__init__.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/activity.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/activity.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/event.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/event.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/task/__init__.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/task/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/task/reservation.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/task/reservation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/task_channel.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/task_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/worker/__init__.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/worker/reservation.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/worker/reservation.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py` & `twilio-8.5.0/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trunking/TrunkingBase.py` & `twilio-8.5.0/twilio/rest/trunking/TrunkingBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trunking/v1/__init__.py` & `twilio-8.5.0/twilio/rest/trunking/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trunking/v1/trunk/__init__.py` & `twilio-8.5.0/twilio/rest/trunking/v1/trunk/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trunking/v1/trunk/credential_list.py` & `twilio-8.5.0/twilio/rest/trunking/v1/trunk/credential_list.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trunking/v1/trunk/ip_access_control_list.py` & `twilio-8.5.0/twilio/rest/trunking/v1/trunk/ip_access_control_list.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trunking/v1/trunk/origination_url.py` & `twilio-8.5.0/twilio/rest/trunking/v1/trunk/origination_url.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trunking/v1/trunk/phone_number.py` & `twilio-8.5.0/twilio/rest/trunking/v1/trunk/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trunking/v1/trunk/recording.py` & `twilio-8.5.0/twilio/rest/trunking/v1/trunk/recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trusthub/TrusthubBase.py` & `twilio-8.5.0/twilio/rest/trusthub/TrusthubBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trusthub/__init__.py` & `twilio-8.5.0/twilio/rest/trusthub/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trusthub/v1/__init__.py` & `twilio-8.5.0/twilio/rest/trusthub/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trusthub/v1/customer_profiles/__init__.py` & `twilio-8.5.0/twilio/rest/trusthub/v1/customer_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py` & `twilio-8.5.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py` & `twilio-8.5.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py` & `twilio-8.5.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trusthub/v1/end_user.py` & `twilio-8.5.0/twilio/rest/trusthub/v1/end_user.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trusthub/v1/end_user_type.py` & `twilio-8.5.0/twilio/rest/trusthub/v1/end_user_type.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trusthub/v1/policies.py` & `twilio-8.5.0/twilio/rest/trusthub/v1/policies.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trusthub/v1/supporting_document.py` & `twilio-8.5.0/twilio/rest/trusthub/v1/supporting_document.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trusthub/v1/supporting_document_type.py` & `twilio-8.5.0/twilio/rest/trusthub/v1/supporting_document_type.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trusthub/v1/trust_products/__init__.py` & `twilio-8.5.0/twilio/rest/trusthub/v1/trust_products/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py` & `twilio-8.5.0/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py` & `twilio-8.5.0/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py` & `twilio-8.5.0/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/verify/VerifyBase.py` & `twilio-8.5.0/twilio/rest/verify/VerifyBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/verify/__init__.py` & `twilio-8.5.0/twilio/rest/verify/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/verify/v2/__init__.py` & `twilio-8.5.0/twilio/rest/verify/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/verify/v2/form.py` & `twilio-8.5.0/twilio/rest/verify/v2/form.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/verify/v2/safelist.py` & `twilio-8.5.0/twilio/rest/verify/v2/safelist.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/verify/v2/service/__init__.py` & `twilio-8.5.0/twilio/rest/verify/v2/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/verify/v2/service/access_token.py` & `twilio-8.5.0/twilio/rest/verify/v2/service/access_token.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/verify/v2/service/entity/__init__.py` & `twilio-8.5.0/twilio/rest/verify/v2/service/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/verify/v2/service/entity/challenge/__init__.py` & `twilio-8.5.0/twilio/rest/verify/v2/service/entity/challenge/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/verify/v2/service/entity/challenge/notification.py` & `twilio-8.5.0/twilio/rest/verify/v2/service/entity/challenge/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/verify/v2/service/entity/factor.py` & `twilio-8.5.0/twilio/rest/verify/v2/service/entity/factor.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/verify/v2/service/entity/new_factor.py` & `twilio-8.5.0/twilio/rest/verify/v2/service/entity/new_factor.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/verify/v2/service/messaging_configuration.py` & `twilio-8.5.0/twilio/rest/verify/v2/service/messaging_configuration.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/verify/v2/service/rate_limit/__init__.py` & `twilio-8.5.0/twilio/rest/verify/v2/service/rate_limit/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/verify/v2/service/rate_limit/bucket.py` & `twilio-8.5.0/twilio/rest/verify/v2/service/rate_limit/bucket.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/verify/v2/service/verification.py` & `twilio-8.5.0/twilio/rest/verify/v2/service/verification.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,18 @@
     class Channel(object):
         SMS = "sms"
         CALL = "call"
         EMAIL = "email"
         WHATSAPP = "whatsapp"
         SNA = "sna"
 
+    class RiskCheck(object):
+        ENABLE = "enable"
+        DISABLE = "disable"
+
     class Status(object):
         CANCELED = "canceled"
         APPROVED = "approved"
 
     """
     :ivar sid: The unique string that we created to identify the Verification resource.
     :ivar service_sid: The SID of the [Service](https://www.twilio.com/docs/verify/api/service) the resource is associated with.
@@ -315,14 +319,15 @@
         payee: Union[str, object] = values.unset,
         rate_limits: Union[object, object] = values.unset,
         channel_configuration: Union[object, object] = values.unset,
         app_hash: Union[str, object] = values.unset,
         template_sid: Union[str, object] = values.unset,
         template_custom_substitutions: Union[str, object] = values.unset,
         device_ip: Union[str, object] = values.unset,
+        risk_check: Union["VerificationInstance.RiskCheck", object] = values.unset,
     ) -> VerificationInstance:
         """
         Create the VerificationInstance
 
         :param to: The phone number or [email](https://www.twilio.com/docs/verify/email) to verify. Phone numbers must be in [E.164 format](https://www.twilio.com/docs/glossary/what-e164).
         :param channel: The verification method to use. One of: [`email`](https://www.twilio.com/docs/verify/email), `sms`, `whatsapp`, `call`, `sna` or `auto`.
         :param custom_friendly_name: A custom user defined friendly name that overwrites the existing one in the verification message
@@ -334,14 +339,15 @@
         :param payee: The payee of the associated PSD2 compliant transaction. Requires the PSD2 Service flag enabled.
         :param rate_limits: The custom key-value pairs of Programmable Rate Limits. Keys correspond to `unique_name` fields defined when [creating your Rate Limit](https://www.twilio.com/docs/verify/api/service-rate-limits). Associated value pairs represent values in the request that you are rate limiting on. You may include multiple Rate Limit values in each request.
         :param channel_configuration: [`email`](https://www.twilio.com/docs/verify/email) channel configuration in json format. The fields 'from' and 'from_name' are optional but if included the 'from' field must have a valid email address.
         :param app_hash: Your [App Hash](https://developers.google.com/identity/sms-retriever/verify#computing_your_apps_hash_string) to be appended at the end of your verification SMS body. Applies only to SMS. Example SMS body: `<#> Your AppName verification code is: 1234 He42w354ol9`.
         :param template_sid: The message [template](https://www.twilio.com/docs/verify/api/templates). If provided, will override the default template for the Service. SMS and Voice channels only.
         :param template_custom_substitutions: A stringified JSON object in which the keys are the template's special variables and the values are the variables substitutions.
         :param device_ip: Strongly encouraged if using the auto channel. The IP address of the client's device. If provided, it has to be a valid IPv4 or IPv6 address.
+        :param risk_check:
 
         :returns: The created VerificationInstance
         """
         data = values.of(
             {
                 "To": to,
                 "Channel": channel,
@@ -354,14 +360,15 @@
                 "Payee": payee,
                 "RateLimits": serialize.object(rate_limits),
                 "ChannelConfiguration": serialize.object(channel_configuration),
                 "AppHash": app_hash,
                 "TemplateSid": template_sid,
                 "TemplateCustomSubstitutions": template_custom_substitutions,
                 "DeviceIp": device_ip,
+                "RiskCheck": risk_check,
             }
         )
 
         payload = self._version.create(
             method="POST",
             uri=self._uri,
             data=data,
@@ -384,14 +391,15 @@
         payee: Union[str, object] = values.unset,
         rate_limits: Union[object, object] = values.unset,
         channel_configuration: Union[object, object] = values.unset,
         app_hash: Union[str, object] = values.unset,
         template_sid: Union[str, object] = values.unset,
         template_custom_substitutions: Union[str, object] = values.unset,
         device_ip: Union[str, object] = values.unset,
+        risk_check: Union["VerificationInstance.RiskCheck", object] = values.unset,
     ) -> VerificationInstance:
         """
         Asynchronously create the VerificationInstance
 
         :param to: The phone number or [email](https://www.twilio.com/docs/verify/email) to verify. Phone numbers must be in [E.164 format](https://www.twilio.com/docs/glossary/what-e164).
         :param channel: The verification method to use. One of: [`email`](https://www.twilio.com/docs/verify/email), `sms`, `whatsapp`, `call`, `sna` or `auto`.
         :param custom_friendly_name: A custom user defined friendly name that overwrites the existing one in the verification message
@@ -403,14 +411,15 @@
         :param payee: The payee of the associated PSD2 compliant transaction. Requires the PSD2 Service flag enabled.
         :param rate_limits: The custom key-value pairs of Programmable Rate Limits. Keys correspond to `unique_name` fields defined when [creating your Rate Limit](https://www.twilio.com/docs/verify/api/service-rate-limits). Associated value pairs represent values in the request that you are rate limiting on. You may include multiple Rate Limit values in each request.
         :param channel_configuration: [`email`](https://www.twilio.com/docs/verify/email) channel configuration in json format. The fields 'from' and 'from_name' are optional but if included the 'from' field must have a valid email address.
         :param app_hash: Your [App Hash](https://developers.google.com/identity/sms-retriever/verify#computing_your_apps_hash_string) to be appended at the end of your verification SMS body. Applies only to SMS. Example SMS body: `<#> Your AppName verification code is: 1234 He42w354ol9`.
         :param template_sid: The message [template](https://www.twilio.com/docs/verify/api/templates). If provided, will override the default template for the Service. SMS and Voice channels only.
         :param template_custom_substitutions: A stringified JSON object in which the keys are the template's special variables and the values are the variables substitutions.
         :param device_ip: Strongly encouraged if using the auto channel. The IP address of the client's device. If provided, it has to be a valid IPv4 or IPv6 address.
+        :param risk_check:
 
         :returns: The created VerificationInstance
         """
         data = values.of(
             {
                 "To": to,
                 "Channel": channel,
@@ -423,14 +432,15 @@
                 "Payee": payee,
                 "RateLimits": serialize.object(rate_limits),
                 "ChannelConfiguration": serialize.object(channel_configuration),
                 "AppHash": app_hash,
                 "TemplateSid": template_sid,
                 "TemplateCustomSubstitutions": template_custom_substitutions,
                 "DeviceIp": device_ip,
+                "RiskCheck": risk_check,
             }
         )
 
         payload = await self._version.create_async(
             method="POST",
             uri=self._uri,
             data=data,
```

### Comparing `twilio-8.4.0/twilio/rest/verify/v2/service/verification_check.py` & `twilio-8.5.0/twilio/rest/verify/v2/service/verification_check.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/verify/v2/service/webhook.py` & `twilio-8.5.0/twilio/rest/verify/v2/service/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/verify/v2/template.py` & `twilio-8.5.0/twilio/rest/verify/v2/template.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/verify/v2/verification_attempt.py` & `twilio-8.5.0/twilio/rest/verify/v2/verification_attempt.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/verify/v2/verification_attempts_summary.py` & `twilio-8.5.0/twilio/rest/verify/v2/verification_attempts_summary.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/video/VideoBase.py` & `twilio-8.5.0/twilio/rest/video/VideoBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/video/__init__.py` & `twilio-8.5.0/twilio/rest/video/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/video/v1/__init__.py` & `twilio-8.5.0/twilio/rest/video/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/video/v1/composition.py` & `twilio-8.5.0/twilio/rest/video/v1/composition.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/video/v1/composition_hook.py` & `twilio-8.5.0/twilio/rest/video/v1/composition_hook.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/video/v1/composition_settings.py` & `twilio-8.5.0/twilio/rest/video/v1/composition_settings.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/video/v1/recording.py` & `twilio-8.5.0/twilio/rest/video/v1/recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/video/v1/recording_settings.py` & `twilio-8.5.0/twilio/rest/video/v1/recording_settings.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/video/v1/room/__init__.py` & `twilio-8.5.0/twilio/rest/video/v1/room/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/video/v1/room/participant/__init__.py` & `twilio-8.5.0/twilio/rest/video/v1/room/participant/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/video/v1/room/participant/anonymize.py` & `twilio-8.5.0/twilio/rest/video/v1/room/participant/anonymize.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/video/v1/room/participant/published_track.py` & `twilio-8.5.0/twilio/rest/video/v1/room/participant/published_track.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/video/v1/room/participant/subscribe_rules.py` & `twilio-8.5.0/twilio/rest/video/v1/room/participant/subscribe_rules.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/video/v1/room/participant/subscribed_track.py` & `twilio-8.5.0/twilio/rest/video/v1/room/participant/subscribed_track.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/video/v1/room/recording_rules.py` & `twilio-8.5.0/twilio/rest/video/v1/room/recording_rules.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/video/v1/room/room_recording.py` & `twilio-8.5.0/twilio/rest/video/v1/room/room_recording.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/voice/VoiceBase.py` & `twilio-8.5.0/twilio/rest/voice/VoiceBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/voice/__init__.py` & `twilio-8.5.0/twilio/rest/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/voice/v1/__init__.py` & `twilio-8.5.0/twilio/rest/voice/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/voice/v1/archived_call.py` & `twilio-8.5.0/twilio/rest/voice/v1/archived_call.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/voice/v1/byoc_trunk.py` & `twilio-8.5.0/twilio/rest/voice/v1/byoc_trunk.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/voice/v1/connection_policy/__init__.py` & `twilio-8.5.0/twilio/rest/voice/v1/connection_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/voice/v1/connection_policy/connection_policy_target.py` & `twilio-8.5.0/twilio/rest/voice/v1/connection_policy/connection_policy_target.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/voice/v1/dialing_permissions/__init__.py` & `twilio-8.5.0/twilio/rest/voice/v1/dialing_permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py` & `twilio-8.5.0/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/voice/v1/dialing_permissions/country/__init__.py` & `twilio-8.5.0/twilio/rest/voice/v1/dialing_permissions/country/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py` & `twilio-8.5.0/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/voice/v1/dialing_permissions/settings.py` & `twilio-8.5.0/twilio/rest/voice/v1/dialing_permissions/settings.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/voice/v1/ip_record.py` & `twilio-8.5.0/twilio/rest/voice/v1/ip_record.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/voice/v1/source_ip_mapping.py` & `twilio-8.5.0/twilio/rest/voice/v1/source_ip_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/wireless/WirelessBase.py` & `twilio-8.5.0/twilio/rest/wireless/WirelessBase.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/wireless/__init__.py` & `twilio-8.5.0/twilio/rest/wireless/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/wireless/v1/__init__.py` & `twilio-8.5.0/twilio/rest/wireless/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/wireless/v1/command.py` & `twilio-8.5.0/twilio/rest/wireless/v1/command.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/wireless/v1/rate_plan.py` & `twilio-8.5.0/twilio/rest/wireless/v1/rate_plan.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/wireless/v1/sim/__init__.py` & `twilio-8.5.0/twilio/rest/wireless/v1/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/wireless/v1/sim/data_session.py` & `twilio-8.5.0/twilio/rest/wireless/v1/sim/data_session.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/wireless/v1/sim/usage_record.py` & `twilio-8.5.0/twilio/rest/wireless/v1/sim/usage_record.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/rest/wireless/v1/usage_record.py` & `twilio-8.5.0/twilio/rest/wireless/v1/usage_record.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/twiml/__init__.py` & `twilio-8.5.0/twilio/twiml/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/twiml/fax_response.py` & `twilio-8.5.0/twilio/twiml/fax_response.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/twiml/messaging_response.py` & `twilio-8.5.0/twilio/twiml/messaging_response.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio/twiml/voice_response.py` & `twilio-8.5.0/twilio/twiml/voice_response.py`

 * *Files identical despite different names*

### Comparing `twilio-8.4.0/twilio.egg-info/PKG-INFO` & `twilio-8.5.0/twilio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twilio
-Version: 8.4.0
+Version: 8.5.0
 Summary: Twilio API client and TwiML generator
 Home-page: https://github.com/twilio/twilio-python/
 Author: Twilio
 Author-email: help@twilio.com
 Keywords: twilio,twiml
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `twilio-8.4.0/twilio.egg-info/SOURCES.txt` & `twilio-8.5.0/twilio.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -267,14 +267,22 @@
 twilio/rest/insights/v1/call/call_summary.py
 twilio/rest/insights/v1/call/event.py
 twilio/rest/insights/v1/call/metric.py
 twilio/rest/insights/v1/conference/__init__.py
 twilio/rest/insights/v1/conference/conference_participant.py
 twilio/rest/insights/v1/room/__init__.py
 twilio/rest/insights/v1/room/participant.py
+twilio/rest/intelligence/IntelligenceBase.py
+twilio/rest/intelligence/__init__.py
+twilio/rest/intelligence/v2/__init__.py
+twilio/rest/intelligence/v2/service.py
+twilio/rest/intelligence/v2/transcript/__init__.py
+twilio/rest/intelligence/v2/transcript/media.py
+twilio/rest/intelligence/v2/transcript/operator_result.py
+twilio/rest/intelligence/v2/transcript/sentence.py
 twilio/rest/ip_messaging/IpMessagingBase.py
 twilio/rest/ip_messaging/__init__.py
 twilio/rest/ip_messaging/v1/__init__.py
 twilio/rest/ip_messaging/v1/credential.py
 twilio/rest/ip_messaging/v1/service/__init__.py
 twilio/rest/ip_messaging/v1/service/role.py
 twilio/rest/ip_messaging/v1/service/channel/__init__.py
@@ -315,14 +323,15 @@
 twilio/rest/messaging/v1/deactivations.py
 twilio/rest/messaging/v1/domain_certs.py
 twilio/rest/messaging/v1/domain_config.py
 twilio/rest/messaging/v1/domain_config_messaging_service.py
 twilio/rest/messaging/v1/external_campaign.py
 twilio/rest/messaging/v1/linkshortening_messaging_service.py
 twilio/rest/messaging/v1/linkshortening_messaging_service_domain_association.py
+twilio/rest/messaging/v1/tollfree_verification.py
 twilio/rest/messaging/v1/usecase.py
 twilio/rest/messaging/v1/brand_registration/__init__.py
 twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py
 twilio/rest/messaging/v1/brand_registration/brand_vetting.py
 twilio/rest/messaging/v1/service/__init__.py
 twilio/rest/messaging/v1/service/alpha_sender.py
 twilio/rest/messaging/v1/service/phone_number.py
```

