# Comparing `tmp/foursight_core-4.3.0.2b5.tar.gz` & `tmp/foursight_core-4.3.0.2b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.3.0.2b5.tar", max compression
+gzip compressed data, was "foursight_core-4.3.0.2b6.tar", max compression
```

## Comparing `foursight_core-4.3.0.2b5.tar` & `foursight_core-4.3.0.2b6.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1083 2023-07-02 11:05:17.039921 foursight_core-4.3.0.2b5/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0       69 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/app.py
--rw-r--r--   0        0        0   103622 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/app_utils.py
--rw-r--r--   0        0        0     1283 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/boto_s3.py
--rw-r--r--   0        0        0     1305 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/boto_sqs.py
--rw-r--r--   0        0        0     2589 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     7293 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11929 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/decorators.py
--rw-r--r--   0        0        0    15846 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/deploy.py
--rw-r--r--   0        0        0     8169 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/environment.py
--rw-r--r--   0        0        0    11948 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5597 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/package.py
--rw-r--r--   0        0        0    16912 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     6629 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    22994 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3065 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6104 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28009 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20464 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3952 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     6213 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4720 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     4096 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     3516 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9466 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0     5216 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0    88080 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    11210 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8025 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    35908 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4805 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11953 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1862184 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/routes.py
--rw-r--r--   0        0        0    22941 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/run_result.py
--rw-r--r--   0        0        0     6380 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     5442 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1500 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/pyproject.toml
--rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 foursight_core-4.3.0.2b5/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-02 11:28:50.142682 foursight_core-4.3.0.2b6/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-07-02 11:28:50.150683 foursight_core-4.3.0.2b6/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-07-02 11:28:50.150683 foursight_core-4.3.0.2b6/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0       69 2023-07-02 11:28:50.150683 foursight_core-4.3.0.2b6/foursight_core/app.py
+-rw-r--r--   0        0        0   103608 2023-07-02 11:28:50.150683 foursight_core-4.3.0.2b6/foursight_core/app_utils.py
+-rw-r--r--   0        0        0     1283 2023-07-02 11:28:50.150683 foursight_core-4.3.0.2b6/foursight_core/boto_s3.py
+-rw-r--r--   0        0        0     1305 2023-07-02 11:28:50.150683 foursight_core-4.3.0.2b6/foursight_core/boto_sqs.py
+-rw-r--r--   0        0        0     2589 2023-07-02 11:28:50.150683 foursight_core-4.3.0.2b6/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2023-07-02 11:28:50.150683 foursight_core-4.3.0.2b6/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2023-07-02 11:28:50.150683 foursight_core-4.3.0.2b6/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     7293 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    11929 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/decorators.py
+-rw-r--r--   0        0        0    15846 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8169 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/environment.py
+-rw-r--r--   0        0        0    11948 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5597 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/mapping.json
+-rw-r--r--   0        0        0     1014 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/package.py
+-rw-r--r--   0        0        0    16912 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0     6629 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0    22994 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3061 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6098 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28009 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    20464 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3952 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     6373 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4720 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0     4096 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0     3516 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0     9466 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0     5214 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    87984 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    11210 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0     8025 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0    35908 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0     4805 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0      806 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    11953 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1862228 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/routes.py
+-rw-r--r--   0        0        0    22941 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/run_result.py
+-rw-r--r--   0        0        0     6380 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0     5282 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     5442 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1500 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/pyproject.toml
+-rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 foursight_core-4.3.0.2b6/PKG-INFO
```

### Comparing `foursight_core-4.3.0.2b5/LICENSE.txt` & `foursight_core-4.3.0.2b6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/abstract_connection.py` & `foursight_core-4.3.0.2b6/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/app_utils.py` & `foursight_core-4.3.0.2b6/foursight_core/app_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,16 +45,16 @@
 from .deploy import Deploy
 from .environment import Environment
 from .fs_connection import FSConnection
 from .s3_connection import S3Connection
 from .react.api.auth import Auth
 from .react.api.react_api import ReactApi
 from .react.api.datetime_utils import (
-    convert_time_t_to_local_datetime_string,
-    convert_utc_datetime_to_local_datetime_string
+    convert_time_t_to_utc_datetime_string,
+    convert_utc_datetime_to_utc_datetime_string
 )
 from .routes import Routes
 from .route_prefixes import CHALICE_LOCAL
 from .sqs_utils import SQS
 from .stage import Stage
 
 
@@ -235,16 +235,16 @@
                 if issuer:
                     name = jwt_decoded.get(issuer + "name")
                     if name:
                         first_name = name.get("name_first")
                         last_name = name.get("name_last")
                 subject = jwt_decoded.get("sub")
                 audience = jwt_decoded.get("aud")
-                issued_time = convert_time_t_to_local_datetime_string(jwt_decoded.get("iat"))
-                expiration_time = convert_time_t_to_local_datetime_string(jwt_decoded.get("exp"))
+                issued_time = convert_time_t_to_utc_datetime_string(jwt_decoded.get("iat"))
+                expiration_time = convert_time_t_to_utc_datetime_string(jwt_decoded.get("exp"))
         except Exception as e:
             self.note_non_fatal_error_for_ui_info(e, 'get_logged_in_user_info')
         return {"email_address": email_address,
                 "email_verified": email_verified,
                 "first_name": first_name,
                 "last_name": last_name,
                 "issuer": issuer,
@@ -781,18 +781,18 @@
             boto_lambda = boto3.client("lambda")
             lambda_info = boto_lambda.get_function(FunctionName=lambda_name)
             if lambda_info:
                 lambda_arn = lambda_info["Configuration"]["FunctionArn"]
                 lambda_tags = boto_lambda.list_tags(Resource=lambda_arn)["Tags"]
                 lambda_last_modified_tag = lambda_tags.get("last_modified")
                 if lambda_last_modified_tag:
-                    lambda_last_modified = convert_utc_datetime_to_local_datetime_string(lambda_last_modified_tag)
+                    lambda_last_modified = convert_utc_datetime_to_utc_datetime_string(lambda_last_modified_tag)
                 else:
                     lambda_last_modified = lambda_info["Configuration"]["LastModified"]
-                    lambda_last_modified = convert_utc_datetime_to_local_datetime_string(lambda_last_modified)
+                    lambda_last_modified = convert_utc_datetime_to_utc_datetime_string(lambda_last_modified)
                 return lambda_last_modified
         except Exception as e:
             logger.warning(f"Error getting lambda ({lambda_name}) last modified time: {e}")
         return None
 
     # ===== ROUTE RUNNING FUNCTIONS =====
 
@@ -1135,15 +1135,15 @@
             #         "principals_edit": principals_edit
             #     })
             users.append({
                 "email_address": user_record.get("email"),
                 "first_name": user_record.get("first_name"),
                 "last_name": user_record.get("last_name"),
                 "uuid": user_record.get("uuid"),
-                "modified": convert_utc_datetime_to_local_datetime_string(last_modified)})
+                "modified": convert_utc_datetime_to_utc_datetime_string(last_modified)})
         users = sorted(users, key=lambda key: key["email_address"])
         template = self.jin_env.get_template('users.html')
         html_resp.body = template.render(
             request=request,
             version=self.get_app_version(),
             package=self.APP_PACKAGE_NAME,
             env=environ,
```

### Comparing `foursight_core-4.3.0.2b5/foursight_core/boto_s3.py` & `foursight_core-4.3.0.2b6/foursight_core/boto_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/boto_sqs.py` & `foursight_core-4.3.0.2b6/foursight_core/boto_sqs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/buckets.py` & `foursight_core-4.3.0.2b6/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/check_schema.py` & `foursight_core-4.3.0.2b6/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/check_utils.py` & `foursight_core-4.3.0.2b6/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.3.0.2b6/foursight_core/checks/access_key_expiration_detection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.3.0.2b6/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/checks/ecs_checks.py` & `foursight_core-4.3.0.2b6/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.3.0.2b6/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.3.0.2b6/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.3.0.2b6/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/checks/scaling_checks.py` & `foursight_core-4.3.0.2b6/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/checks/test_checks.py` & `foursight_core-4.3.0.2b6/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/decorators.py` & `foursight_core-4.3.0.2b6/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/deploy.py` & `foursight_core-4.3.0.2b6/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/environment.py` & `foursight_core-4.3.0.2b6/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/es_connection.py` & `foursight_core-4.3.0.2b6/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/exceptions.py` & `foursight_core-4.3.0.2b6/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/fs_connection.py` & `foursight_core-4.3.0.2b6/foursight_core/fs_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/identity.py` & `foursight_core-4.3.0.2b6/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/mapping.json` & `foursight_core-4.3.0.2b6/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/package.py` & `foursight_core-4.3.0.2b6/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/auth.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/auth.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/auth0_config.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/auth0_config.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/aws_network.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/aws_s3.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/aws_s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from typing import Optional
-from .datetime_utils import convert_utc_datetime_to_local_datetime_string
+from .datetime_utils import convert_utc_datetime_to_utc_datetime_string
 from ...boto_s3 import boto_s3_client, boto_s3_resource
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 
 class AwsS3:
@@ -28,15 +28,15 @@
             if bucket_keys:
                 bucket_keys = bucket_keys.get("Contents")
                 if bucket_keys:
                     for bucket_key in sorted(bucket_keys, key=lambda item: item["Key"]):
                         results.append({
                             "key": bucket_key["Key"],
                             "size": bucket_key["Size"],
-                            "modified": convert_utc_datetime_to_local_datetime_string(bucket_key["LastModified"])
+                            "modified": convert_utc_datetime_to_utc_datetime_string(bucket_key["LastModified"])
                         })
 
         except Exception as e:
             logger.error(f"Exception getting S3 bucket key list: {e}")
         return results
 
     SHOW_BUCKET_KEY_CONTENT_MAX_SIZE_BYTES = 50000
```

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/aws_stacks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import boto3
-from .datetime_utils import convert_utc_datetime_to_local_datetime_string
+from .datetime_utils import convert_utc_datetime_to_utc_datetime_string
 from .yaml_utils import load_yaml
 from collections import OrderedDict
 from dcicutils.function_cache_decorator import function_cache
 from dcicutils.obfuscation_utils import obfuscate_dict
 from typing import Optional, Union
 
 
@@ -31,16 +31,16 @@
     """
     return {
         "name": stack.name,
         "id": stack.stack_id,
         "description": stack.description,
         "role_arn": stack.role_arn,
         "status": stack.stack_status,
-        "updated": convert_utc_datetime_to_local_datetime_string(stack.last_updated_time),
-        "created": convert_utc_datetime_to_local_datetime_string(stack.creation_time)
+        "updated": convert_utc_datetime_to_utc_datetime_string(stack.last_updated_time),
+        "created": convert_utc_datetime_to_utc_datetime_string(stack.creation_time)
     }
 
 
 @function_cache
 def aws_get_stack(stack_name_or_object: Union[str, object]) -> dict:
     """
     Returns all detailed info for the given AWS CloudFormation stack name,
```

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/checks.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/cognito.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/datetime_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import datetime
 import dateutil.parser as dateutil_parser
 import pytz
 from typing import Optional, Union
-import tzlocal
 
 
 EPOCH = datetime.datetime.utcfromtimestamp(0)  # I.e.: 1970-01-01 00:00:00 UTC
-LOCAL_TIMEZONE_NAME = tzlocal.get_localzone_name()
 
 
-def convert_utc_datetime_to_datetime_string(t: Union[datetime.datetime, str], tzname: str) -> Optional[str]:
+def _convert_utc_datetime_to_datetime_string(t: Union[datetime.datetime, str],
+                                             tzname: Optional[str] = None) -> Optional[str]:
     """
     Converts the given datetime object OR string, which is ASSUMED to by in the UTC timezone,
     into a datetime string in the given/named timezone, and returns its value in a form that looks
     like 2022-08-22 13:25:34 EDT. If the argument is a string it is ASSUMED to have a value which
     looks like 2022-08-22T14:24:49.000+0000; this is (for example) the format we get from AWS via
     boto3 (e.g. for a lambda last-modified value) or from values in ElasticSearch.
 
     :param t: A datetime object or string value ASSUMED to be in the UTC timezone.
+    :param tzname: A timezone name (string); default to UTC if unspecified.
     :return: A datetime string in the given timezone formatted like: 2022-08-22 13:25:34 EDT
     """
     def make_utc_aware_datetime(t: datetime) -> datetime:
         return t.replace(tzinfo=pytz.UTC)
     try:
         if isinstance(t, str):
             #
@@ -32,44 +32,46 @@
             # dateutil.parser is more forgiving so using that now.
             #
             # if ".0000000" in t:
             #     t = t.replace(".0000000", ".000000")
             # t = datetime.datetime.strptime(t, "%Y-%m-%dT%H:%M:%S.%f%z")
             #
             t = dateutil_parser.parse(t)
-        t = make_utc_aware_datetime(t).astimezone(pytz.timezone(tzname))
+        tz = pytz.timezone(tzname) if tzname else pytz.UTC
+        t = make_utc_aware_datetime(t).astimezone(tz)
         return t.strftime("%Y-%m-%d %H:%M:%S %Z")
-    except Exception:
+    except Exception as e:
         return None
 
 
-def convert_utc_datetime_to_local_datetime_string(t: Union[datetime.datetime, str]) -> Optional[str]:
+def convert_utc_datetime_to_utc_datetime_string(t: Union[datetime.datetime, str]) -> Optional[str]:
     """
-    Same as convert_utc_datetime_to_datetime_string (above) but specifically for the local timezone.
+    Same as _convert_utc_datetime_to_datetime_string (above) but explicitly for the UTC timezone.
     """
-    return convert_utc_datetime_to_datetime_string(t, LOCAL_TIMEZONE_NAME)
+    return _convert_utc_datetime_to_datetime_string(t)
 
 
-def convert_time_t_to_datetime_string(time_t: int, tzname: str) -> Optional[str]:
+def convert_time_t_to_datetime_string(time_t: int, tzname: Optional[str] = None) -> Optional[str]:
     """
     Converts the given "epoch" time (seconds since 1970-01-01T00:00:00Z)
     integer value to a datetime string in the given/named timezone,
     and returns its value in a form that looks like 2022-08-22 13:25:34 EDT.
 
     :param time_t: Epoch time value (i.e. seconds since 1970-01-01T00:00:00Z)
+    :param tzname: A timezone name (string); default to UTC if unspecified.
     :return: A datetime string in the given timezone formatted like: 2022-08-22 13:25:34 EDT
     """
-    return convert_utc_datetime_to_datetime_string(convert_time_t_to_datetime(time_t), tzname)
+    return _convert_utc_datetime_to_datetime_string(convert_time_t_to_datetime(time_t), tzname)
 
 
-def convert_time_t_to_local_datetime_string(time_t: int) -> Optional[str]:
+def convert_time_t_to_utc_datetime_string(time_t: int) -> Optional[str]:
     """
-    Same as convert_time_t_to_datetime_string (above) but specifically for the local timezone.
+    Same as convert_time_t_to_datetime_string (above) but explicitly for the UTC timezone.
     """
-    return convert_time_t_to_datetime_string(time_t, LOCAL_TIMEZONE_NAME)
+    return convert_time_t_to_datetime_string(time_t)
 
 
 def convert_iso_datetime_string_to_datetime(value: str) -> Optional[datetime.datetime]:
     """
     Returns a datetime object, in the UTC timezone, for the given (assumed)
     ISO 8601 conforming datetime string; if an error occurs (e.g. if the
     given value is not ISO 8601 conforming) then returns None.
```

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/encryption.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/envs.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/envs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/gac.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/misc_utils.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/portal_access_key_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pytz
 from dcicutils import ff_utils
 from dcicutils.misc_utils import future_datetime
 from typing import Optional, Tuple
 from ...app import app
 from .datetime_utils import (
     convert_iso_datetime_string_to_datetime as normalize_portal_datetime,
-    convert_utc_datetime_to_local_datetime_string as datetime_to_string
+    convert_utc_datetime_to_utc_datetime_string as datetime_to_string
 )
 
 
 _PORTAL_ACCESS_KEY_NAME = "access_key_foursight"
 _PORTAL_ACCESS_KEY_USER_EMAIL = "foursight.app@gmail.com"
 _PORTAL_ACCESS_KEY_EXPIRES_SOON_WARNING_DAYS = 12
```

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/react_api.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/react_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,16 +37,15 @@
     aws_get_stack_resources, aws_get_stack_template,
 )
 from .checks import Checks
 from .cognito import get_cognito_oauth_config, handle_cognito_oauth_callback
 from .cookie_utils import create_delete_cookie_string, read_cookie, read_cookie_bool, read_cookie_int
 from .datetime_utils import (
     convert_uptime_to_datetime,
-    convert_utc_datetime_to_local_datetime_string,
-    LOCAL_TIMEZONE_NAME
+    convert_utc_datetime_to_utc_datetime_string
 )
 from .encryption import Encryption
 from .encoding_utils import base64_decode_to_json
 from .gac import Gac
 from .misc_utils import (
     get_base_url,
     is_running_locally,
@@ -372,15 +371,15 @@
                     data_portal["ssl_certificate_error"] = True
                 portal_url = env_utils_get_portal_url(env)
                 data_portal["url"] = portal_url
                 data_portal["ssl_certificate"] = get_ssl_certificate_info(portal_url)
                 if data_portal["ssl_certificate"]:
                     data_portal["ssl_certificate"]["name"] = "Portal"
                     data_portal["ssl_certificate"]["exception"] = e
-        data["timestamp"] = convert_utc_datetime_to_local_datetime_string(datetime.datetime.utcnow())
+        data["timestamp"] = convert_utc_datetime_to_utc_datetime_string(datetime.datetime.utcnow())
         import tzlocal # xyzzy temporary
         data["timezone"] = tzlocal.get_localzone_name()
         test_mode_access_key_simulate_error = read_cookie_bool(request, "test_mode_access_key_simulate_error")
         if auth.get("user_exception"): # or test_mode_access_key_simulate_error:
             # Since this call to get the Portal access key info can be relatively expensive, we don't want to
             # do it on every /header API call; so we only call it if, according to the user's authtoken cookie,
             # an exception was experienced when trying to authorize the user (via envs.get_user_auth_info) on
@@ -425,15 +424,14 @@
                     "aws_account_number": aws_credentials.get("aws_account_number"),
                     "aws_account_name": aws_credentials.get("aws_account_name"),
                     "aws_access_key_id": aws_credentials.get("aws_access_key_id"),
                     "re_captcha_key": os.environ.get("reCaptchaKey", None)
                 },
                 "launched": app.core.init_load_time,
                 "deployed": app.core.get_lambda_last_modified(),
-                "timezone": LOCAL_TIMEZONE_NAME,
                 "accounts_file": self._get_accounts_file_name()
             },
             "versions": self._get_versions_object(),
             "portal": {
                 "url": portal_url,
                 "health_url": portal_base_url + "/health?format=json",
                 "health_ui_url": portal_base_url + "/health"
@@ -641,16 +639,16 @@
             "uuid": user.get("uuid"),
             "title": user.get("title"),
             "groups": user.get("groups"),
             "project": user.get("project"),
             "institution": user.get("user_institution"),
             "roles": user.get("project_roles"),
             "status": user.get("status"),
-            "updated": convert_utc_datetime_to_local_datetime_string(updated),
-            "created": convert_utc_datetime_to_local_datetime_string(user.get("date_created"))
+            "updated": convert_utc_datetime_to_utc_datetime_string(updated),
+            "created": convert_utc_datetime_to_utc_datetime_string(user.get("date_created"))
         }
 
     def _create_user_record_from_input(self, user: dict, include_deletes: bool = False) -> dict:
         """
         Canonicalizes and returns the given user record from our UI into the
         common format suitable for insert/update to our database. Modifies input.
         Please see comment above (in _create_user_record_for_output) WRT roles.
@@ -992,15 +990,15 @@
         check_results = check_results.get_latest_result()
         if not check_results:
             return self.create_success_response({})
         uuid = check_results["uuid"]
         if check_results.get("action"):
             check_results["action_title"] = " ".join(check_results["action"].split("_")).title()
         check_datetime = datetime.datetime.strptime(uuid, "%Y-%m-%dT%H:%M:%S.%f")
-        check_datetime = convert_utc_datetime_to_local_datetime_string(check_datetime)
+        check_datetime = convert_utc_datetime_to_utc_datetime_string(check_datetime)
         check_results["timestamp"] = check_datetime
         return self.create_success_response(check_results)
 
     def reactapi_checks_history_uuid(self, request: dict, env: str, check: str, uuid: str) -> Response:
         """
         Called from react_routes for endpoint: GET /{env}/checks/{check}/history/{uuid}
         Returns the check result for the given check (name) and uuid.
@@ -1086,15 +1084,15 @@
                     if isinstance(item, dict):
                         uuid = item.get("uuid")
                         duration = item.get("runtime_seconds")
                         state = item.get("queue_action")
                         break
                 if uuid:
                     timestamp = datetime.datetime.strptime(uuid, "%Y-%m-%dT%H:%M:%S.%f")
-                    timestamp = convert_utc_datetime_to_local_datetime_string(timestamp)
+                    timestamp = convert_utc_datetime_to_utc_datetime_string(timestamp)
                     results.append({
                         "check": check_name,
                         "title": check_title,
                         "group": group_name,
                         "status": status,
                         "state": state,
                         "uuid": uuid,
@@ -1131,15 +1129,15 @@
         # queue_attr = app.core.sqs.get_sqs_attributes(app.core.sqs.get_sqs_queue().url)
         for item in history:
             for subitem in item:
                 if isinstance(subitem, dict):
                     uuid = subitem.get("uuid")
                     if uuid:
                         timestamp = datetime.datetime.strptime(uuid, "%Y-%m-%dT%H:%M:%S.%f")
-                        timestamp = convert_utc_datetime_to_local_datetime_string(timestamp)
+                        timestamp = convert_utc_datetime_to_utc_datetime_string(timestamp)
                         subitem["timestamp"] = timestamp
         body = {
             "env": env,
             "history_kwargs": history_kwargs,
             "paging": {
                 "total": total,
                 "count": len(history),
@@ -1449,15 +1447,15 @@
                 "portal": portal_health_json.get("project_version"),
                 "snovault": portal_health_json.get("snovault_version"),
                 "dcicutils": portal_health_json.get("utils_version"),
                 "python": portal_health_json.get("python_version")
             }
             portal_uptime = portal_health_json.get("uptime")
             portal_started = convert_uptime_to_datetime(portal_uptime)
-            response["portal"]["started"] = convert_utc_datetime_to_local_datetime_string(portal_started)
+            response["portal"]["started"] = convert_utc_datetime_to_utc_datetime_string(portal_started)
             response["portal"]["identity"] = portal_health_json.get("identity")
             response["portal"]["elasticsearch"] = portal_health_json.get("elasticsearch")
             response["portal"]["database"] = portal_health_json.get("database")
             response["portal"]["health"] = portal_health_json
             foursight_url = get_foursight_base_url(portal_health_json.get("foursight"))
             response["portal"]["foursight_url"] = foursight_url
             return foursight_url
@@ -1685,27 +1683,27 @@
             for deployment in service.get("deployments", []):
                 if (not most_recent_update_at or
                     (deployment.get("updatedAt") and deployment.get("updatedAt") > most_recent_update_at)):
                     most_recent_update_at = deployment.get("updatedAt")
                 deployments.append({
                     "id": deployment.get("id"),
                     "task": deployment.get("taskDefinition"),
-                    "created": convert_utc_datetime_to_local_datetime_string(deployment.get("createdAt")),
-                    "updated": convert_utc_datetime_to_local_datetime_string(deployment.get("updatedAt"))
+                    "created": convert_utc_datetime_to_utc_datetime_string(deployment.get("createdAt")),
+                    "updated": convert_utc_datetime_to_utc_datetime_string(deployment.get("updatedAt"))
                 })
             if (not most_recent_deployment_at or
                 (most_recent_update_at and most_recent_update_at > most_recent_deployment_at)):
                 most_recent_deployment_at = most_recent_update_at
             response["services"].append({
                 "arn": service_arn,
                 "name": service.get("serviceName"),
                 "deployments": deployments
             })
         if most_recent_deployment_at:
-            response["most_recent_deployed"] = convert_utc_datetime_to_local_datetime_string(most_recent_deployment_at)
+            response["most_recent_deployed"] = convert_utc_datetime_to_utc_datetime_string(most_recent_deployment_at)
         return self.create_success_response(response)
 
     def reactapi_reload_lambda(self, request: dict) -> Response:
         """
         Called from react_routes for endpoint: GET /__reloadlambda__
         Kicks off a reload of the given lambda name. For troubleshooting only.
         """
```

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/react_api_base.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/react_api_base.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/react_routes.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/react_routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/react_ui.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.3.0.2b6/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/ui/index.html` & `foursight_core-4.3.0.2b6/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.3.0.2b6/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.3.0.2b6/foursight_core/react/ui/static/js/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.86e7492f.js.LICENSE.txt */ ! function() {
+/*! For license information please see main.57815041.js.LICENSE.txt */ ! function() {
     var e = {
             3339: function(e, t, n) {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.RawSha256 = void 0;
                 var r = n(3277),
@@ -47883,18 +47883,97 @@
                     }))
                 },
                 Ra = t.createContext({}),
                 Fa = function() {
                     var e = (0, t.useContext)(Ra);
                     return e ? e[0] : {}
                 },
-                Ba = function() {
+                Ba = {
+                    FormatDateTime: function(e) {
+                        var n = e.verbose,
+                            r = void 0 !== n && n,
+                            o = e.timezone,
+                            i = void 0 === o || o,
+                            a = l((0, t.useState)(new Date), 2),
+                            s = a[0],
+                            u = a[1];
+                        return (0, t.useEffect)((function() {
+                            var e = setInterval((function() {
+                                return u(new Date)
+                            }), 1100);
+                            return function() {
+                                return clearInterval(e)
+                            }
+                        }), []), (0, wo.jsx)(wo.Fragment, {
+                            children: uo.FormatDateTime(s, r, i)
+                        })
+                    },
+                    FormatDuration: function(e) {
+                        var n = e.start,
+                            r = void 0 === n ? null : n,
+                            o = e.end,
+                            i = void 0 === o ? null : o,
+                            a = e.verbose,
+                            s = void 0 !== a && a,
+                            u = e.fallback,
+                            c = void 0 === u ? "" : u,
+                            d = e.prefix,
+                            p = void 0 === d ? "" : d,
+                            f = e.suffix,
+                            h = void 0 === f ? "" : f,
+                            g = e.tooltip,
+                            y = void 0 !== g && g;
+                        "datetime" === p && (p = uo.FormatDateTime(r || i) + " |");
+                        var m = l((0, t.useState)(new Date), 2),
+                            v = m[0],
+                            M = m[1];
+                        return (0, t.useEffect)((function() {
+                            var e = setInterval((function() {
+                                M(new Date)
+                            }), 1100);
+                            return function() {
+                                return clearInterval(e)
+                            }
+                        }), []), (0, wo.jsx)(wo.Fragment, {
+                            children: (0, wo.jsxs)("span", {
+                                id: y ? "tooltip-timestamp-".concat(r || i) : "",
+                                "data-text": uo.FormatDateTime(r || i),
+                                children: [uo.FormatDuration(r || v, i || v, s, c, p, h), (0, wo.jsx)(oa, {
+                                    id: "tooltip-timestamp-".concat(r || i),
+                                    text: uo.FormatDateTime(r || i)
+                                })]
+                            })
+                        })
+                    }
+                },
+                Ya = Ba,
+                Qa = !1,
+                Ga = !0,
+                Wa = {
+                    Now: function() {
+                        return new Date
+                    },
+                    Format: function(e) {
+                        return uo.FormatDateTime(e, Qa, Ga, true)
+                    },
+                    Format24: function(e) {
+                        return uo.FormatDateTime(e, Qa, Ga, true)
+                    },
+                    Format12: function(e) {
+                        return uo.FormatDateTime(e, Qa, Ga, false)
+                    },
+                    FormatVerbose: function(e) {
+                        return uo.FormatDateTime(e, true, Ga, false)
+                    },
+                    Live: Ya.FormatDateTime
+                },
+                Ha = function() {
                     return [Array.from(La(Ca)[0].values())]
                 },
-                Ya = function(e) {
+                Va = function(e) {
                     return {
                         __get: function(t, n, r, o) {
                             var i = e.findIndex((function(e) {
                                 return e.type === t
                             }));
                             if (i >= 0) {
                                 var a = n ? "".concat(t, ".").concat(n) : t;
@@ -47907,16 +47986,16 @@
                                     }
                                 }
                             }
                             return null
                         }
                     }
                 },
-                Qa = function(e) {
-                    e = Ya(e);
+                Za = function(e) {
+                    e = Va(e);
                     var n = l((0, t.useState)([]), 2),
                         r = n[0],
                         o = n[1];
                     return (0, t.useState)({
                         count: function() {
                             return r.length
                         },
@@ -47961,23 +48040,23 @@
                         __unselect: function(e) {
                             var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null,
                                 n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : null;
                             null == n && (n = this.__lookup(e, t)), n >= 0 && (r.splice(n, 1), o(p(r)))
                         }
                     })[0]
                 },
-                Ga = function(e) {
+                qa = function(e) {
                     var t;
                     return "function" == typeof e && (e = e()), (null === (t = e) || void 0 === t ? void 0 : t.constructor) === Object ? e : {}
                 },
-                Wa = function(e, t) {
+                Ja = function(e, t) {
                     return "function" == typeof e && (e = e()), void 0 !== e ? e : {}
                 };
 
-            function Ha(e) {
+            function Ka(e) {
                 var t, n, r = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : void 0,
                     o = !(arguments.length > 2 && void 0 !== arguments[2]) || arguments[2];
                 if (Object.is(e, r))
                     if ((null === (n = e) || void 0 === n ? void 0 : n.constructor) === Object) e = nt({}, e);
                     else if (Array.isArray(e)) {
                     e = function(e) {
                         var t = p(e),
@@ -47991,24 +48070,24 @@
                             }
                         return t
                     }(e)
                 } else "function" === typeof e && (e = e(r));
                 else(null === (t = e) || void 0 === t ? void 0 : t.constructor) === Object && (null === r || void 0 === r ? void 0 : r.constructor) === Object && o && (e = nt(nt({}, r), e));
                 return e
             }
-            var Va = function(e, n) {
+            var Xa = function(e, n) {
                     var r = !0 === (null === e || void 0 === e ? void 0 : e.__keyedState) ? !0 === e.__keyedStateUsage ? e : e.keyed("default") : null,
-                        o = r ? r.__state() ? r.__state() : Wa(n) : Ga(e),
+                        o = r ? r.__state() ? r.__state() : Ja(n) : qa(e),
                         i = l((0, t.useState)(o), 2),
                         a = i[0],
                         s = i[1];
                     return (0, t.useEffect)((function() {
-                        o && r && !r.__state() && r.__updateState(Ha(o, a, !0))
+                        o && r && !r.__state() && r.__updateState(Ka(o, a, !0))
                     }), []), r ? [a, function(e) {
-                        e = Ha(e, a, !0), s(e), r.__updateState(e)
+                        e = Ka(e, a, !0), s(e), r.__updateState(e)
                     }] : {
                         __keyedState: !0,
                         key: null,
                         keyed: function(e) {
                             var t;
                             if (!0 === this.__keyedState) {
                                 (null === (t = e) || void 0 === t ? void 0 : t.constructor) === String && 0 !== e.length || (e = "default");
@@ -48032,15 +48111,15 @@
                                         return a[e]
                                     }
                                 }
                             }
                         }
                     }
                 },
-                Za = function() {
+                $a = function() {
                     var e = l($e(), 2),
                         t = e[0],
                         n = e[1];
 
                     function r(e) {
                         var t = new URLSearchParams(window.location.search);
                         return wt.HasValue(e) ? t.get(e) : t.toString()
@@ -48091,18 +48170,18 @@
                                             s = a.indexOf(t); - 1 !== s && (a.splice(s, 1), o(e, a.join(",")))
                                     } else i(e)
                             }(e, arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null)
                         }
                     }
                 };
 
-            function qa(e) {
+            function es(e) {
                 return /^\*+$/.test(e)
             }
-            var Ja = function(e) {
+            var ts = function(e) {
                     var t = Ua("/aws/secrets", {
                         cache: !0
                     });
                     return (0, wo.jsxs)(wo.Fragment, {
                         children: [(0, wo.jsx)("div", {
                             children: (0, wo.jsx)("b", {
                                 children: "AWS Secrets"
@@ -48133,36 +48212,36 @@
                                         iff: r + 1 < t.length
                                     })]
                                 })
                             }))]
                         })]
                     })
                 },
-                Ka = function(e) {
+                ns = function(e) {
                     var t, n, r, o, i = Ua("/info", {
                         cache: !0
                     });
-                    return (0, wo.jsx)($a, {
+                    return (0, wo.jsx)(os, {
                         name: null === (t = i.data) || void 0 === t || null === (n = t.gac) || void 0 === n ? void 0 : n.name,
                         values: null === (r = i.data) || void 0 === r || null === (o = r.gac) || void 0 === o ? void 0 : o.values,
                         hide: e.hide
                     })
                 },
-                Xa = function(e) {
+                rs = function(e) {
                     var t = Ua(e.name ? "/aws/secrets/".concat(e.name) : null, {
                         cache: !1
                     });
-                    return e.name ? (0, wo.jsx)($a, {
+                    return e.name ? (0, wo.jsx)(os, {
                         name: e.name,
                         values: null === t || void 0 === t ? void 0 : t.data,
                         hide: e.hide,
                         embedded: e.embedded
                     }) : null
                 },
-                $a = function(e) {
+                os = function(e) {
                     var t;
                     return (0, wo.jsxs)("div", {
                         style: {
                             maxWidth: "100%",
                             marginBottom: e.embedded ? "2pt" : "8pt"
                         },
                         children: [!e.embedded && (0, wo.jsxs)("div", {
@@ -48201,15 +48280,15 @@
                                 style: {
                                     marginBottom: "1pt"
                                 },
                                 children: null === (t = Object.keys(e.values)) || void 0 === t ? void 0 : t.map((function(t) {
                                     return (0, wo.jsxs)("li", {
                                         children: [(0, wo.jsx)("b", {
                                             children: t
-                                        }), " ", (0, wo.jsx)("br", {}), qa(e.values[t]) ? (0, wo.jsx)("span", {
+                                        }), " ", (0, wo.jsx)("br", {}), es(e.values[t]) ? (0, wo.jsx)("span", {
                                             style: {
                                                 color: "red"
                                             },
                                             children: "REDACTED"
                                         }) : e.values[t]]
                                     }, t)
                                 }))
@@ -48221,19 +48300,19 @@
                                     label: "Loading secrets"
                                 })
                             })
                         })]
                     })
                 };
 
-            function es(e, t) {
+            function is(e, t) {
                 var n, r, o, i, a, s, u, l;
                 return !Dt.IsNull(null === e || void 0 === e || null === (n = e.app) || void 0 === n || null === (r = n.credentials) || void 0 === r ? void 0 : r.aws_account_number) && !Dt.IsNull(null === t || void 0 === t || null === (o = t.data) || void 0 === o || null === (i = o.foursight) || void 0 === i ? void 0 : i.aws_account_number) && (null === e || void 0 === e || null === (a = e.app) || void 0 === a || null === (s = a.credentials) || void 0 === s ? void 0 : s.aws_account_number) === (null === t || void 0 === t || null === (u = t.data) || void 0 === u || null === (l = u.foursight) || void 0 === l ? void 0 : l.aws_account_number)
             }
-            var ts = function(e) {
+            var as = function(e) {
                     var t = e.portalAccessKeyResponse;
                     return t ? t.invalid ? (0, wo.jsx)("b", {
                         style: {
                             color: "red"
                         },
                         children: "Invalid"
                     }) : t.expired ? (0, wo.jsx)("b", {
@@ -48241,24 +48320,24 @@
                             color: "red"
                         },
                         children: "Expired"
                     }) : t.expires_at ? t.expires_soon ? (0, wo.jsxs)("span", {
                         style: {
                             color: "red"
                         },
-                        children: ["Expires ", uo.FromNow(t.expires_at), " ", po.RightArrow, " ", t.expires_at]
+                        children: ["Expires ", uo.FromNow(t.expires_at), " ", po.RightArrow, " ", Wa.Format(t.expires_at)]
                     }) : (0, wo.jsxs)(wo.Fragment, {
-                        children: ["Expires ", uo.FromNow(t.expires_at), " ", po.RightArrow, " ", t.expires_at]
+                        children: ["Expires ", uo.FromNow(t.expires_at), " ", po.RightArrow, " ", Wa.Format(t.expires_at)]
                     }) : (0, wo.jsx)(wo.Fragment, {
                         children: "No expiration"
                     }) : (0, wo.jsx)(wo.Fragment, {
                         children: "\u2013"
                     })
                 },
-                ns = function(e) {
+                ss = function(e) {
                     var t = e.url,
                         n = Ua(t ? "/certificates?hostname=".concat(t) : null);
                     Jr()();
                     return t && t.startsWith("https://") && (0, wo.jsxs)("small", {
                         children: [(0, wo.jsx)("small", {
                             style: {
                                 marginLeft: "3pt",
@@ -48293,15 +48372,15 @@
                                     u = null === (o = n.data[0]) || void 0 === o ? void 0 : o.expires_at;
                                 return i ? "SSL certificate is invalid!" : a ? "SSL certificate expired ".concat(uo.Ago(u), " (").concat(u, ")") : s ? "SSL certificate expires ".concat(uo.FromNow(u), " (").concat(u, ") -> Soon!") : "SSL certificate expires ".concat(uo.FromNow(u), " (").concat(u, ")")
                             }()),
                             position: "top"
                         })]
                     })
                 },
-                rs = function(e) {
+                us = function(e) {
                     var t = e.bucket,
                         n = e.name,
                         r = e.line,
                         o = void 0 === r || r;
                     return t ? (0, wo.jsxs)(wo.Fragment, {
                         children: [n && (0, wo.jsxs)(wo.Fragment, {
                             children: [(0, wo.jsx)("b", {
@@ -48319,15 +48398,15 @@
                             href: "https://s3.console.aws.amazon.com/s3/buckets/".concat(t),
                             style: {
                                 marginLeft: "4pt"
                             }
                         }), o && (0, wo.jsx)("br", {})]
                     }) : (0, wo.jsx)(wo.Fragment, {})
                 },
-                os = function(e) {
+                ls = function(e) {
                     var t = e.title,
                         n = e.value,
                         r = e.additionalValue,
                         o = e.externalLink,
                         i = e.children,
                         a = e.tooltip,
                         s = void 0 === a ? null : a,
@@ -48381,15 +48460,15 @@
                                 id: y,
                                 text: g,
                                 position: "top"
                             })]
                         })]
                     })
                 },
-                is = function(e) {
+                cs = function(e) {
                     var t = e.title,
                         n = e.version,
                         r = e.show;
                     return (void 0 === r || r) && n ? (0, wo.jsxs)("tr", {
                         children: [(0, wo.jsxs)("td", {
                             style: {
                                 whiteSpace: "nowrap",
@@ -48403,26 +48482,26 @@
                                 })
                             }) : (0, wo.jsx)(wo.Fragment, {
                                 children: po.EmptySet
                             })
                         })]
                     }) : (0, wo.jsx)(wo.Fragment, {})
                 },
-                as = function(e) {
+                ds = function(e) {
                     var n = e.header,
                         r = e.info,
                         o = (e.name, l((0, t.useState)(!1), 2)),
                         i = o[0],
                         a = o[1];
 
                     function s() {
                         a(!i)
                     }
                     return (0, wo.jsx)(wo.Fragment, {
-                        children: es(n, r) && (0, wo.jsxs)(wo.Fragment, {
+                        children: is(n, r) && (0, wo.jsxs)(wo.Fragment, {
                             children: [(0, wo.jsx)("small", {
                                 style: {
                                     marginLeft: "3pt",
                                     marginRight: "3pt"
                                 },
                                 children: "|"
                             }), i ? (0, wo.jsx)(wo.Fragment, {
@@ -48435,36 +48514,36 @@
                                 children: (0, wo.jsxs)("span", {
                                     onClick: s,
                                     className: "pointer",
                                     children: ["Secrets ", (0, wo.jsx)("b", {
                                         children: po.UpArrow
                                     })]
                                 })
-                            }), i && (0, wo.jsx)(Xa, {
+                            }), i && (0, wo.jsx)(rs, {
                                 name: r.get("foursight.identity"),
                                 embedded: !0
                             })]
                         })
                     })
                 },
-                ss = function(e) {
+                ps = function(e) {
                     var n, r, o = e.header,
                         i = e.info,
                         a = l((0, t.useState)(!1), 2),
                         s = a[0],
                         u = a[1];
 
                     function c() {
                         u(!s)
                     }
-                    var d = es(o, i) ? null === o || void 0 === o || null === (n = o.auth) || void 0 === n || null === (r = n.known_envs) || void 0 === r ? void 0 : r.sort((function(e, t) {
+                    var d = is(o, i) ? null === o || void 0 === o || null === (n = o.auth) || void 0 === n || null === (r = n.known_envs) || void 0 === r ? void 0 : r.sort((function(e, t) {
                         return e.full_name > t.full_name ? 1 : -1
                     })) : null;
                     return (0, wo.jsx)(wo.Fragment, {
-                        children: es(o, i) && (0, wo.jsxs)(wo.Fragment, {
+                        children: is(o, i) && (0, wo.jsxs)(wo.Fragment, {
                             children: [(0, wo.jsx)("small", {
                                 style: {
                                     marginLeft: "3pt",
                                     marginRight: "3pt"
                                 },
                                 children: "|"
                             }), s ? (0, wo.jsx)(wo.Fragment, {
@@ -48508,15 +48587,15 @@
                                         })
                                     }))
                                 })
                             })]
                         })
                     })
                 },
-                us = function() {
+                fs = function() {
                     return (0, wo.jsxs)(wo.Fragment, {
                         children: [(0, wo.jsx)("tr", {
                             children: (0, wo.jsx)("td", {
                                 style: {
                                     paddingTop: "4pt"
                                 }
                             })
@@ -48532,15 +48611,15 @@
                                 style: {
                                     paddingTop: "4pt"
                                 }
                             })
                         })]
                     })
                 },
-                ls = function(e) {
+                hs = function(e) {
                     var n, r, o, i, a, s, u = e.header,
                         c = e.info,
                         d = (e.foursightUrl, Ua("/portal_access_key")),
                         p = l((0, t.useState)(!1), 2),
                         f = p[0],
                         h = p[1],
                         g = l((0, t.useState)(!1), 2);
@@ -48558,15 +48637,15 @@
                         style: {
                             width: "100%"
                         },
                         children: (0, wo.jsxs)("tbody", {
                             style: {
                                 whiteSpace: "nowrap"
                             },
-                            children: [(0, wo.jsxs)(os, {
+                            children: [(0, wo.jsxs)(ls, {
                                 title: "foursight" === c.get("foursight.package") ? "Foursight-Fourfront" : "Foursight-CGAP",
                                 value: c.get("foursight.url"),
                                 externalLink: c.get("foursight.url"),
                                 small: !1,
                                 children: [(0, wo.jsx)("small", {
                                     style: {
                                         marginLeft: "3pt",
@@ -48584,18 +48663,18 @@
                                         children: "API"
                                     }), (0, wo.jsx)(la, {
                                         href: "".concat(c.get("foursight.url"), "/reactapi/header"),
                                         style: {
                                             marginLeft: "4pt"
                                         }
                                     })]
-                                }), (0, wo.jsx)(ns, {
+                                }), (0, wo.jsx)(ss, {
                                     url: c.get("foursight.url")
                                 })]
-                            }), (0, wo.jsxs)(os, {
+                            }), (0, wo.jsxs)(ls, {
                                 title: "foursight" === c.get("foursight.package") ? "Fourfront" : "CGAP-Portal",
                                 value: c.get("portal.url"),
                                 externalLink: c.get("portal.url"),
                                 small: !1,
                                 children: ["\xa0|\xa0", (0, wo.jsxs)("small", {
                                     children: [(0, wo.jsx)("a", {
                                         style: {
@@ -48633,67 +48712,67 @@
                                         children: "Indexer"
                                     }), "\xa0", (0, wo.jsx)(la, {
                                         href: "".concat(c.get("portal.url"), "/indexing_status?format=json"),
                                         style: {
                                             marginLeft: "1pt"
                                         }
                                     })]
-                                }), (0, wo.jsx)(ns, {
+                                }), (0, wo.jsx)(ss, {
                                     url: c.get("portal.url")
                                 })]
-                            }), (0, wo.jsx)(os, {
+                            }), (0, wo.jsx)(ls, {
                                 title: "Elasticsearch",
                                 value: null === (n = c.get("portal.elasticsearch")) || void 0 === n ? void 0 : n.replace(/:443$/, ""),
                                 additionalValue: c.get("foursight.es_cluster"),
                                 externalLink: "https://us-east-1.console.aws.amazon.com/aos/home?region=us-east-1#opensearch/domains/".concat(c.get("foursight.es_cluster") ? c.get("foursight.es_cluster") : "")
-                            }), (0, wo.jsx)(os, {
+                            }), (0, wo.jsx)(ls, {
                                 title: "RDS (Foursight)",
                                 value: c.get("foursight.rds"),
                                 externalLink: "https://us-east-1.console.aws.amazon.com/rds/home?region=us-east-1#databases:",
                                 show: !(null !== (r = c.get("portal.health.database")) && void 0 !== r && r.startsWith(c.get("foursight.rds")))
-                            }), (0, wo.jsx)(os, {
+                            }), (0, wo.jsx)(ls, {
                                 title: "RDS",
                                 value: c.get("portal.health.database"),
                                 additionalValue: c.get("foursight.rds_name"),
                                 externalLink: "https://us-east-1.console.aws.amazon.com/rds/home?region=us-east-1#database:id=".concat(c.get("foursight.rds_name"), ";is-cluster=false")
-                            }), (0, wo.jsx)(os, {
+                            }), (0, wo.jsx)(ls, {
                                 title: "Redis",
                                 value: c.get("foursight.redis_url"),
                                 externalLink: "https://us-east-1.console.aws.amazon.com/memorydb/home?region=us-east-1#/clusters"
-                            }), (0, wo.jsx)(os, {
+                            }), (0, wo.jsx)(ls, {
                                 title: "SQS",
                                 value: c.get("foursight.sqs_url"),
                                 externalLink: "https://us-east-1.console.aws.amazon.com/sqs/v2/home?region=us-east-1#/queues/".concat(encodeURIComponent(c.get("foursight.sqs_url")))
-                            }), (0, wo.jsx)(us, {}), (0, wo.jsx)(os, {
+                            }), (0, wo.jsx)(fs, {}), (0, wo.jsx)(ls, {
                                 title: c.get("foursight.identity") == c.get("portal.identity") ? "Identity" : "Foursight Identity",
                                 value: c.get("foursight.identity"),
-                                externalLink: es(u, c) ? "https://us-east-1.console.aws.amazon.com/secretsmanager/secret?name=".concat(c.get("foursight.identity"), "&region=us-east-1#") : "".concat(c.get("foursight.url"), "/react/").concat(c.get("foursight.default_env.name"), "/aws/infrastructure?secrets=").concat(c.get("foursight.identity")),
-                                children: (0, wo.jsx)(as, {
+                                externalLink: is(u, c) ? "https://us-east-1.console.aws.amazon.com/secretsmanager/secret?name=".concat(c.get("foursight.identity"), "&region=us-east-1#") : "".concat(c.get("foursight.url"), "/react/").concat(c.get("foursight.default_env.name"), "/aws/infrastructure?secrets=").concat(c.get("foursight.identity")),
+                                children: (0, wo.jsx)(ds, {
                                     header: u,
                                     info: c,
                                     name: c.get("foursight.identity"),
                                     embedded: !0
                                 })
                             }), c.get("foursight.identity") != c.get("portal.identity") && (0, wo.jsx)(wo.Fragment, {
-                                children: (0, wo.jsx)(os, {
+                                children: (0, wo.jsx)(ls, {
                                     title: "Portal Identity",
                                     value: c.get("portal.identity"),
-                                    externalLink: es(u, c) ? "https://us-east-1.console.aws.amazon.com/secretsmanager/secret?name=".concat(c.get("portal.identity"), "&region=us-east-1#") : "".concat(c.get("foursight.url"), "/react/").concat(c.get("foursight.default_env.name"), "/aws/infrastructure?secrets=").concat(c.get("portal.identity")),
-                                    children: (0, wo.jsx)(as, {
+                                    externalLink: is(u, c) ? "https://us-east-1.console.aws.amazon.com/secretsmanager/secret?name=".concat(c.get("portal.identity"), "&region=us-east-1#") : "".concat(c.get("foursight.url"), "/react/").concat(c.get("foursight.default_env.name"), "/aws/infrastructure?secrets=").concat(c.get("portal.identity")),
+                                    children: (0, wo.jsx)(ds, {
                                         header: u,
                                         info: c,
                                         name: c.get("portal.identity"),
                                         embedded: !0
                                     })
                                 })
-                            }), (0, wo.jsx)(os, {
+                            }), (0, wo.jsx)(ls, {
                                 title: "Stack Name",
                                 value: c.get("foursight.stack"),
                                 externalLink: "https://us-east-1.console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/stackinfo?filteringStatus=active&viewNested=true&stackId=".concat(c.get("foursight.stack"))
-                            }), (0, wo.jsxs)(os, {
+                            }), (0, wo.jsxs)(ls, {
                                 title: "Global Env Bucket",
                                 value: c.get("foursight.s3.global_env_bucket"),
                                 externalLink: "https://s3.console.aws.amazon.com/s3/buckets/".concat(c.get("foursight.s3.global_env_bucket"), "?region=us-east-1&tab=objects"),
                                 tooltip: ["S3 Bucket Org: ".concat(c.get("foursight.s3.bucket_org")), "bucket-org-".concat(c.get("foursight.s3.bucket_org"))],
                                 children: [(0, wo.jsx)("small", {
                                     style: {
                                         marginLeft: "3pt",
@@ -48711,70 +48790,70 @@
                                             background: "inherit",
                                             border: "1pt gray dotted",
                                             marginTop: "2pt",
                                             marginBottom: "2pt",
                                             padding: "4pt",
                                             color: "inherit"
                                         },
-                                        children: [(0, wo.jsx)(rs, {
+                                        children: [(0, wo.jsx)(us, {
                                             name: "System",
                                             bucket: c.get("foursight.s3.buckets.sys_bucket")
-                                        }), (0, wo.jsx)(rs, {
+                                        }), (0, wo.jsx)(us, {
                                             name: "Output",
                                             bucket: c.get("foursight.s3.buckets.outfile_bucket")
-                                        }), (0, wo.jsx)(rs, {
+                                        }), (0, wo.jsx)(us, {
                                             name: "Metadata",
                                             bucket: c.get("foursight.s3.buckets.metadata_bucket")
-                                        }), (0, wo.jsx)(rs, {
+                                        }), (0, wo.jsx)(us, {
                                             name: "Blobs",
                                             bucket: c.get("foursight.s3.buckets.blob_bucket")
-                                        }), (0, wo.jsx)(rs, {
+                                        }), (0, wo.jsx)(us, {
                                             name: "Raw",
                                             bucket: c.get("foursight.s3.buckets.raw_file_bucket")
-                                        }), (0, wo.jsx)(rs, {
+                                        }), (0, wo.jsx)(us, {
                                             name: "Results",
                                             bucket: c.get("foursight.s3.buckets.results_bucket")
-                                        }), (0, wo.jsx)(rs, {
+                                        }), (0, wo.jsx)(us, {
                                             name: "Tibanna CWLs",
                                             bucket: c.get("foursight.s3.buckets.tibanna_cwls_bucket")
-                                        }), (0, wo.jsx)(rs, {
+                                        }), (0, wo.jsx)(us, {
                                             name: "Tibanna Output",
                                             bucket: c.get("foursight.s3.buckets.tibanna_output_bucket")
                                         })]
                                     })]
                                 }) : (0, wo.jsx)(wo.Fragment, {
                                     children: (0, wo.jsxs)("span", {
                                         onClick: y,
                                         className: "pointer",
                                         children: ["Buckets ", (0, wo.jsx)("b", {
                                             children: po.UpArrow
                                         })]
                                     })
                                 })]
-                            }), (0, wo.jsx)(os, {
+                            }), (0, wo.jsx)(ls, {
                                 title: "Bucket Encryption ID",
                                 value: c.get("foursight.s3.encrypt_key_id"),
                                 externalLink: "https://us-east-1.console.aws.amazon.com/kms/home?region=us-east-1#/kms/keys/".concat(c.get("foursight.s3.encrypt_key_id")),
                                 tooltip: ["S3 Bucket Encryption Key ID", "tooltip-encryption-key-".concat(c.get("foursight.aws_account_number"))],
                                 showEmpty: !0
-                            }), (0, wo.jsx)(us, {}), (0, wo.jsx)(os, {
+                            }), (0, wo.jsx)(fs, {}), (0, wo.jsx)(ls, {
                                 title: "AWS Account",
                                 value: c.get("foursight.aws_account_number"),
                                 additionalValue: c.get("foursight.aws_account_name"),
                                 externalLink: "https://us-east-1.console.aws.amazon.com/billing/home#/account",
                                 bold: !0
-                            }), (0, wo.jsx)(os, {
+                            }), (0, wo.jsx)(ls, {
                                 title: "Default Environment",
                                 value: c.get("foursight.default_env.full_name"),
                                 additionalValue: c.get("foursight.env_count") ? "".concat(c.get("foursight.env_count"), " total") : "",
-                                children: (0, wo.jsx)(ss, {
+                                children: (0, wo.jsx)(ps, {
                                     header: u,
                                     info: c
                                 })
-                            }), (0, wo.jsxs)(os, {
+                            }), (0, wo.jsxs)(ls, {
                                 title: "Auth0 Client ID",
                                 value: c.get("foursight.auth0_client"),
                                 externalLink: "".concat(c.get("foursight.url"), "/reactapi/auth0_config"),
                                 children: ["\xa0|\xa0", (0, wo.jsx)("a", {
                                     style: {
                                         color: "inherit"
                                     },
@@ -48784,30 +48863,30 @@
                                     children: "Portal"
                                 }), (0, wo.jsx)(la, {
                                     href: "".concat(c.get("portal.url"), "/auth0_config?format=json"),
                                     style: {
                                         marginLeft: "4pt"
                                     }
                                 })]
-                            }), (0, wo.jsx)(os, {
+                            }), (0, wo.jsx)(ls, {
                                 title: "reCAPTCHA Key ID",
                                 value: c.get("foursight.re_captcha_key")
                             }), (0, wo.jsxs)("tr", {
                                 style: {
                                     fontSize: "small"
                                 },
                                 children: [(0, wo.jsx)("td", {
                                     style: {
                                         paddingRight: "10pt"
                                     },
                                     children: "Portal Access Key:"
                                 }), (0, wo.jsxs)("td", {
-                                    children: [es(u, c) && !d.loading && (0, wo.jsxs)(wo.Fragment, {
+                                    children: [is(u, c) && !d.loading && (0, wo.jsxs)(wo.Fragment, {
                                         children: [d.get("key"), "\xa0|\xa0"]
-                                    }), (0, wo.jsx)(ts, {
+                                    }), (0, wo.jsx)(as, {
                                         portalAccessKeyResponse: c.get("foursight.portal_access_key")
                                     }), (0, wo.jsx)(la, {
                                         href: "".concat(c.get("foursight.url"), "/react/").concat(c.get("foursight.default_env.name"), "/portal_access_key"),
                                         style: {
                                             marginLeft: "6pt"
                                         }
                                     }), (0, wo.jsxs)("span", {
@@ -48834,102 +48913,102 @@
                                         }), (0, wo.jsx)(oa, {
                                             id: "tooltip-s3-access-ke",
                                             text: "Location of Portal access key in AWS S3.",
                                             position: "bottom"
                                         })]
                                     })]
                                 })]
-                            }), (0, wo.jsx)(us, {}), (0, wo.jsx)(os, {
+                            }), (0, wo.jsx)(fs, {}), (0, wo.jsx)(ls, {
                                 title: "Foursight Deployed",
-                                value: "".concat(c.get("foursight.deployed"), " ").concat(po.RightArrow, " ").concat(uo.Ago(c.get("foursight.deployed"))),
+                                value: "".concat(Wa.Format(c.get("foursight.deployed")), " ").concat(po.RightArrow, " ").concat(uo.Ago(c.get("foursight.deployed"))),
                                 show: !!c.get("foursight.deployed")
-                            }), (0, wo.jsx)(os, {
+                            }), (0, wo.jsx)(ls, {
                                 title: "Portal Deployed",
-                                value: "".concat(c.get("portal.started"), " ").concat(po.RightArrow, " ").concat(uo.Ago(c.get("portal.started")))
+                                value: "".concat(Wa.Format(c.get("portal.started")), " ").concat(po.RightArrow, " ").concat(uo.Ago(c.get("portal.started")))
                             })]
                         })
                     })
                 },
-                cs = function(e) {
+                gs = function(e) {
                     var t = e.info;
                     return !t || t.loading ? (0, wo.jsx)(wo.Fragment, {}) : (0, wo.jsx)("table", {
                         style: {
                             width: "100%",
                             margin: "0",
                             padding: "0"
                         },
                         children: (0, wo.jsxs)("tbody", {
                             style: {
                                 fontSize: "small",
                                 verticalAlign: "top",
                                 whiteSpace: "nowrap"
                             },
-                            children: [(0, wo.jsx)(is, {
+                            children: [(0, wo.jsx)(cs, {
                                 title: t.get("foursight.package"),
                                 version: t.get("foursight.versions.foursight")
-                            }), (0, wo.jsx)(is, {
+                            }), (0, wo.jsx)(cs, {
                                 title: "foursight-core",
                                 version: t.get("foursight.versions.foursight_core")
-                            }), (0, wo.jsx)(is, {
+                            }), (0, wo.jsx)(cs, {
                                 title: "dcicutils",
                                 version: t.get("foursight.versions.dcicutils")
-                            }), (0, wo.jsx)(is, {
+                            }), (0, wo.jsx)(cs, {
                                 title: "tibanna",
                                 version: t.get("foursight.versions.tibanna")
-                            }), (0, wo.jsx)(is, {
+                            }), (0, wo.jsx)(cs, {
                                 title: "tibanna_ff",
                                 version: t.get("foursight.versions.tibanna_ff")
-                            }), (0, wo.jsx)(is, {
+                            }), (0, wo.jsx)(cs, {
                                 title: "boto3",
                                 version: t.get("foursight.versions.boto3")
-                            }), (0, wo.jsx)(is, {
+                            }), (0, wo.jsx)(cs, {
                                 title: "botocore",
                                 version: t.get("foursight.versions.botocore")
-                            }), (0, wo.jsx)(is, {
+                            }), (0, wo.jsx)(cs, {
                                 title: "chalice",
                                 version: t.get("foursight.versions.chalice")
-                            }), (0, wo.jsx)(is, {
+                            }), (0, wo.jsx)(cs, {
                                 title: "redis",
                                 version: t.get("foursight.versions.redis")
-                            }), (0, wo.jsx)(is, {
+                            }), (0, wo.jsx)(cs, {
                                 title: "python",
                                 version: t.get("foursight.versions.python")
-                            }), (0, wo.jsx)(us, {}), (0, wo.jsx)(is, {
+                            }), (0, wo.jsx)(fs, {}), (0, wo.jsx)(cs, {
                                 title: "portal",
                                 version: t.get("portal.versions.portal")
-                            }), (0, wo.jsx)(is, {
+                            }), (0, wo.jsx)(cs, {
                                 title: "portal-project",
                                 version: t.get("portal.health.project_version"),
                                 show: t.get("portal.health.project_version") != t.get("portal.versions.portal")
-                            }), (0, wo.jsx)(is, {
+                            }), (0, wo.jsx)(cs, {
                                 title: "snovault",
                                 version: t.get("portal.versions.snovault")
-                            }), (0, wo.jsx)(is, {
+                            }), (0, wo.jsx)(cs, {
                                 title: "dcicutils",
                                 version: t.get("portal.versions.dcicutils")
-                            }), (0, wo.jsx)(is, {
+                            }), (0, wo.jsx)(cs, {
                                 title: "python",
                                 version: t.get("portal.health.python_version")
-                            }), (0, wo.jsx)(us, {}), (0, wo.jsx)(is, {
+                            }), (0, wo.jsx)(fs, {}), (0, wo.jsx)(cs, {
                                 title: "elasticsearch-server",
                                 version: t.get("foursight.versions.elasticsearch_server")
-                            }), (0, wo.jsx)(is, {
+                            }), (0, wo.jsx)(cs, {
                                 title: "elasticsearch",
                                 version: t.get("foursight.versions.elasticsearch")
-                            }), (0, wo.jsx)(is, {
+                            }), (0, wo.jsx)(cs, {
                                 title: "elasticsearch-dsl",
                                 version: t.get("foursight.versions.elasticsearch_dsl")
-                            }), (0, wo.jsx)(is, {
+                            }), (0, wo.jsx)(cs, {
                                 title: "redis-server",
                                 version: t.get("foursight.versions.redis_server")
                             })]
                         })
                     })
                 },
-                ds = function(e) {
+                ys = function(e) {
                     var n, r, o, i, a, s, u = e.account,
                         l = e.header,
                         c = e.foursightUrl,
                         d = e.all,
                         p = e.decrementAccountCount,
                         f = e.brighten,
                         h = Ua("/accounts/".concat(u.id), {
@@ -48937,26 +49016,26 @@
                                 return p()
                             },
                             cache: !0,
                             nofetch: !0
                         });
                     return (0, t.useEffect)((function() {
                         h.fetch()
-                    }), []), d || es(l, h) ? (0, wo.jsx)(wo.Fragment, {
+                    }), []), d || is(l, h) ? (0, wo.jsx)(wo.Fragment, {
                         children: (0, wo.jsxs)("div", {
                             className: function(e, t) {
                                 var n, r;
-                                return es(e, t) && (null === e || void 0 === e || null === (n = e.app) || void 0 === n ? void 0 : n.stage) === (null === t || void 0 === t || null === (r = t.data) || void 0 === r ? void 0 : r.stage)
+                                return is(e, t) && (null === e || void 0 === e || null === (n = e.app) || void 0 === n ? void 0 : n.stage) === (null === t || void 0 === t || null === (r = t.data) || void 0 === r ? void 0 : r.stage)
                             }(l, h) ? "box" : "box lighten",
                             style: {
                                 marginTop: "4pt",
                                 marginBottom: "8pt",
                                 filter: f ? "brightness(1.1)" : ""
                             },
-                            children: [es(l, h) ? (0, wo.jsxs)(wo.Fragment, {
+                            children: [is(l, h) ? (0, wo.jsxs)(wo.Fragment, {
                                 children: [(0, wo.jsx)("b", {
                                     id: "tooltip-current-".concat(u.name, "-").concat(null === h || void 0 === h || null === (n = h.data) || void 0 === n ? void 0 : n.stage),
                                     children: (null === (r = h.data) || void 0 === r ? void 0 : r.name) || u.name
                                 }), (0, wo.jsx)(oa, {
                                     id: "tooltip-current-".concat(u.name, "-").concat(null === h || void 0 === h || null === (o = h.data) || void 0 === o ? void 0 : o.stage),
                                     text: "This is your current account: ".concat(h.get("foursight.aws_account_number")),
                                     position: "top"
@@ -49061,15 +49140,15 @@
                                         style: {
                                             verticalAlign: "top"
                                         },
                                         children: [(0, wo.jsx)("td", {
                                             style: {
                                                 width: "80%"
                                             },
-                                            children: (0, wo.jsx)(ls, {
+                                            children: (0, wo.jsx)(hs, {
                                                 header: l,
                                                 info: h,
                                                 foursightUrl: c
                                             })
                                         }), (0, wo.jsx)("td", {
                                             style: {
                                                 paddingLeft: "6pt",
@@ -49083,15 +49162,15 @@
                                         }), (0, wo.jsx)("td", {
                                             style: {
                                                 width: "30%",
                                                 paddingLeft: "8pt",
                                                 textAlign: "top",
                                                 verticalAlign: "top"
                                             },
-                                            children: (0, wo.jsx)(cs, {
+                                            children: (0, wo.jsx)(gs, {
                                                 info: h,
                                                 header: l
                                             })
                                         })]
                                     })
                                 })
                             }), (null === (s = h.data) || void 0 === s ? void 0 : s.__showraw) && (0, wo.jsxs)(wo.Fragment, {
@@ -49108,15 +49187,15 @@
                                     },
                                     children: Ia.Format(h.data)
                                 })]
                             })]
                         })
                     }) : null
                 },
-                ps = function(e) {
+                ms = function(e) {
                     var n, r, o, i, a, s, u, c, d, p, f, h, g, y, m = e.header,
                         v = Ua(rn.Url("/accounts"), {
                             method: "POST",
                             nofetch: !0
                         }),
                         M = Ua(rn.Url("/accounts_file"), {
                             nocache: !0
@@ -49133,15 +49212,15 @@
                         }),
                         S = l((0, t.useState)(0), 2),
                         k = S[0],
                         C = S[1],
                         E = l((0, t.useState)(!0), 2),
                         T = E[0],
                         A = E[1],
-                        z = l(Ba(), 1)[0],
+                        z = l(Ha(), 1)[0],
                         O = l((0, t.useState)(!1), 2),
                         _ = O[0],
                         U = O[1];
 
                     function P() {
                         C((function(e) {
                             return e - 1
@@ -49379,15 +49458,15 @@
                                         children: Ia.Format({})
                                     })
                                 })]
                             })]
                         }), L.length > 0 ? (0, wo.jsxs)(wo.Fragment, {
                             children: [null === L || void 0 === L ? void 0 : L.map((function(e, n) {
                                 return (0, wo.jsx)(t.Fragment, {
-                                    children: (0, wo.jsx)(ds, {
+                                    children: (0, wo.jsx)(ys, {
                                         account: e,
                                         header: m,
                                         all: I,
                                         decrementAccountCount: P,
                                         foursightUrl: e.foursight_url
                                     })
                                 }, e.id)
@@ -49418,141 +49497,141 @@
                                 }) : (0, wo.jsx)(wo.Fragment, {
                                     children: "No accounts info found."
                                 })
                             })
                         })]
                     })
                 },
-                fs = function(e) {
+                vs = function(e) {
                     var t = Fa();
                     return (0, wo.jsx)("div", {
                         className: "container",
-                        children: (0, wo.jsx)(ps, {
+                        children: (0, wo.jsx)(ms, {
                             header: t
                         })
                     })
                 },
-                hs = function() {
+                Ms = function() {
                     var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : null,
                         t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null,
                         n = Ta(),
                         r = Aa();
 
                     function o(o, i) {
                         return _a(e, t, o, i, (function() {}), (function() {}), (function() {}), (function() {}), (function() {}), n, r, !0)
                     }
                     return function(e, t) {
                         return Oa(o(e, t))
                     }
                 },
-                gs = {
+                js = {
                     fontSize: "11pt",
                     verticalAlign: "top",
                     paddingBottom: "2pt",
                     paddingRight: "10pt",
                     whiteSpace: "nowrap"
                 },
-                ys = nt(nt({}, gs), {}, {
+                bs = nt(nt({}, js), {}, {
                     textAlign: "right"
                 }),
-                ms = function(e) {
+                ws = function(e) {
                     var t, n = e.cache,
-                        r = hs();
+                        r = Ms();
                     return (0, wo.jsx)(wo.Fragment, {
                         children: (0, wo.jsxs)("tr", {
                             children: [(0, wo.jsx)("td", {
-                                style: gs,
+                                style: js,
                                 children: n.name
                             }), (0, wo.jsx)("td", {
-                                style: ys,
+                                style: bs,
                                 children: n.hits > 0 ? n.hits : (0, wo.jsx)(wo.Fragment, {
                                     children: "\u2013"
                                 })
                             }), (0, wo.jsx)("td", {
-                                style: ys,
+                                style: bs,
                                 children: n.misses > 0 ? n.misses : (0, wo.jsx)(wo.Fragment, {
                                     children: "\u2013"
                                 })
                             }), (0, wo.jsx)("td", {
-                                style: ys,
+                                style: bs,
                                 children: n.size > 0 ? n.size : (0, wo.jsx)(wo.Fragment, {
                                     children: "\u2013"
                                 })
                             }), (0, wo.jsxs)("td", {
-                                style: gs,
+                                style: js,
                                 id: "tooltip-updated-".concat(n.name),
                                 children: [(0, wo.jsx)(oa, {
                                     id: "tooltip-updated-".concat(n.name),
                                     position: "bottom",
                                     text: "Last time function was actually called."
                                 }), n.updated || (0, wo.jsx)(wo.Fragment, {
                                     children: "\u2013"
                                 })]
                             }), (0, wo.jsxs)("td", {
-                                style: ys,
+                                style: bs,
                                 id: "tooltip-duration-".concat(n.name),
                                 children: [(0, wo.jsx)(oa, {
                                     id: "tooltip-duration-".concat(n.name),
                                     position: "bottom",
                                     text: "Duration of last actual function call."
                                 }), n.duration ? (null === (t = n.duration) || void 0 === t ? void 0 : t.toFixed(1)) + " ms" : (0, wo.jsx)(wo.Fragment, {
                                     children: "\u2013"
                                 })]
                             }), (0, wo.jsx)("td", {
-                                style: ys,
+                                style: bs,
                                 children: n.maxsize >= Number.MAX_SAFE_INTEGER ? (0, wo.jsx)(wo.Fragment, {
                                     children: po.Infinity
                                 }) : (0, wo.jsx)(wo.Fragment, {
                                     children: n.maxsize
                                 })
                             }), (0, wo.jsx)("td", {
-                                style: ys,
+                                style: bs,
                                 children: n.ttl || (0, wo.jsx)(wo.Fragment, {
                                     children: "\u2013"
                                 })
                             }), (0, wo.jsx)("td", {
-                                style: ys,
+                                style: bs,
                                 children: n.ttl_none || (0, wo.jsx)(wo.Fragment, {
                                     children: "\u2013"
                                 })
                             }), (0, wo.jsx)("td", {
-                                style: gs,
+                                style: js,
                                 children: n.nocache_none ? (0, wo.jsx)(wo.Fragment, {
                                     children: "Yes"
                                 }) : (0, wo.jsx)(wo.Fragment, {
                                     children: "\u2013"
                                 })
                             }), (0, wo.jsx)("td", {
-                                style: gs,
+                                style: js,
                                 children: n.nocache_other ? (0, wo.jsx)(wo.Fragment, {
                                     children: "Yes"
                                 }) : (0, wo.jsx)(wo.Fragment, {
                                     children: "\u2013"
                                 })
                             }), (0, wo.jsx)("td", {
-                                style: gs,
+                                style: js,
                                 children: (0, wo.jsx)("span", {
                                     onClick: function() {
                                         return t = n.name, r("//__functioncacheclear__?name=".concat(t)), void e.refresh();
                                         var t
                                     },
                                     className: "pointer",
                                     children: "Clear"
                                 })
                             })]
                         })
                     })
                 },
-                vs = function(e) {
+                xs = function(e) {
                     var n = Ua("//__functioncache__"),
-                        r = hs(),
+                        r = Ms(),
                         o = l((0, t.useState)(!1), 2),
                         i = o[0],
                         a = o[1],
-                        s = nt(nt({}, gs), {}, {
+                        s = nt(nt({}, js), {}, {
                             verticalAlign: "bottom",
                             fontWeight: "bold",
                             textDecoration: "underline"
                         });
 
                     function u() {
                         n.refresh()
@@ -49634,15 +49713,15 @@
                                         }), (0, wo.jsx)("td", {
                                             style: s,
                                             children: "Action"
                                         })]
                                     })
                                 }), (0, wo.jsx)("tbody", {
                                     children: n.map((function(e) {
-                                        return (0, wo.jsx)(ms, {
+                                        return (0, wo.jsx)(ws, {
                                             cache: e,
                                             refresh: u
                                         }, e.name)
                                     }))
                                 })]
                             }), i && (0, wo.jsxs)(wo.Fragment, {
                                 children: [(0, wo.jsx)(aa, {
@@ -49657,93 +49736,14 @@
                                     },
                                     children: no.Format(n.data)
                                 })]
                             })]
                         })]
                     })
                 },
-                Ms = {
-                    FormatDateTime: function(e) {
-                        var n = e.verbose,
-                            r = void 0 !== n && n,
-                            o = e.timezone,
-                            i = void 0 === o || o,
-                            a = l((0, t.useState)(new Date), 2),
-                            s = a[0],
-                            u = a[1];
-                        return (0, t.useEffect)((function() {
-                            var e = setInterval((function() {
-                                return u(new Date)
-                            }), 1100);
-                            return function() {
-                                return clearInterval(e)
-                            }
-                        }), []), (0, wo.jsx)(wo.Fragment, {
-                            children: uo.FormatDateTime(s, r, i)
-                        })
-                    },
-                    FormatDuration: function(e) {
-                        var n = e.start,
-                            r = void 0 === n ? null : n,
-                            o = e.end,
-                            i = void 0 === o ? null : o,
-                            a = e.verbose,
-                            s = void 0 !== a && a,
-                            u = e.fallback,
-                            c = void 0 === u ? "" : u,
-                            d = e.prefix,
-                            p = void 0 === d ? "" : d,
-                            f = e.suffix,
-                            h = void 0 === f ? "" : f,
-                            g = e.tooltip,
-                            y = void 0 !== g && g;
-                        "datetime" === p && (p = uo.FormatDateTime(r || i) + " |");
-                        var m = l((0, t.useState)(new Date), 2),
-                            v = m[0],
-                            M = m[1];
-                        return (0, t.useEffect)((function() {
-                            var e = setInterval((function() {
-                                M(new Date)
-                            }), 1100);
-                            return function() {
-                                return clearInterval(e)
-                            }
-                        }), []), (0, wo.jsx)(wo.Fragment, {
-                            children: (0, wo.jsxs)("span", {
-                                id: y ? "tooltip-timestamp-".concat(r || i) : "",
-                                "data-text": uo.FormatDateTime(r || i),
-                                children: [uo.FormatDuration(r || v, i || v, s, c, p, h), (0, wo.jsx)(oa, {
-                                    id: "tooltip-timestamp-".concat(r || i),
-                                    text: uo.FormatDateTime(r || i)
-                                })]
-                            })
-                        })
-                    }
-                },
-                js = Ms,
-                bs = !1,
-                ws = !0,
-                xs = {
-                    Now: function() {
-                        return new Date
-                    },
-                    Format: function(e) {
-                        return uo.FormatDateTime(e, bs, ws, true)
-                    },
-                    Format24: function(e) {
-                        return uo.FormatDateTime(e, bs, ws, true)
-                    },
-                    Format12: function(e) {
-                        return uo.FormatDateTime(e, bs, ws, false)
-                    },
-                    FormatVerbose: function(e) {
-                        return uo.FormatDateTime(e, true, ws, false)
-                    },
-                    Live: js.FormatDateTime
-                },
                 Ns = function(e) {
                     var t = e.columns,
                         n = e.list,
                         r = e.update,
                         o = e.refresh,
                         i = e.sort,
                         a = void 0 === i ? null : i,
@@ -50232,15 +50232,15 @@
                                                             }), (0, wo.jsxs)("td", {
                                                                 align: "right",
                                                                 children: [e.size, "\xa0\xa0"]
                                                             }), (0, wo.jsxs)("td", {
                                                                 style: {
                                                                     whiteSpace: "nowrap"
                                                                 },
-                                                                children: [xs.Format(e.modified), "\xa0\xa0"]
+                                                                children: [Wa.Format(e.modified), "\xa0\xa0"]
                                                             })]
                                                         }, n), n < r.keys.length - 1 && (0, wo.jsxs)(wo.Fragment, {
                                                             children: [(0, wo.jsx)("tr", {
                                                                 children: (0, wo.jsx)("td", {
                                                                     style: {
                                                                         paddingTop: "4pt"
                                                                     }
@@ -50518,15 +50518,15 @@
                         children: n
                     })
                 },
                 Es = {
                     Ago: uo.Ago,
                     Format: uo.FormatDuration,
                     FromNow: uo.FromNow,
-                    Live: js.FormatDuration
+                    Live: Ya.FormatDuration
                 };
 
             function Ts(e) {
                 e.update()
             }
 
             function As(e) {
@@ -51220,15 +51220,15 @@
                                         id: "tooltip-latest-result-timestamp ".concat(i.name),
                                         children: i.__result.get("timestamp")
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-latest-result ".concat(i.name),
                                         text: "Click to " + (i.__showingResultDetails ? "hide" : "show") + " latest result."
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-latest-result-timestamp ".concat(i.name),
-                                        text: Es.Format(i.__result.get("timestamp"), xs.Now(), !0, null, null, "ago")
+                                        text: Es.Format(i.__result.get("timestamp"), Wa.Now(), !0, null, null, "ago")
                                     })]
                                 }), i.__showingResultDetails && (0, wo.jsx)(wo.Fragment, {
                                     children: i.__result.get("uuid") ? (0, wo.jsx)(wo.Fragment, {
                                         children: d ? (0, wo.jsx)(wo.Fragment, {
                                             children: i.__result.get("action") ? (0, wo.jsxs)(wo.Fragment, {
                                                 children: ["\xa0|\xa0", (0, wo.jsx)("span", {
                                                     id: "tooltip-view-latest-result-summary ".concat(i.name),
@@ -51652,15 +51652,15 @@
                 tu = function(e) {
                     var t = e.check,
                         n = e.env,
                         r = e.groupList,
                         o = e.historyList,
                         i = e.style,
                         a = l(Ls(), 1)[0],
-                        s = hs();
+                        s = Ms();
                     if (t.__queueingCheckRun) return t.__queueingCheckRun && (0, wo.jsxs)("div", {
                         className: "check-run-wait-button",
                         style: i,
                         children: [(0, wo.jsx)("span", {
                             id: "tooltip-queueing",
                             children: (0, wo.jsx)("i", {
                                 children: "Queueing"
@@ -51972,15 +51972,15 @@
                                         id: "tooltip-view-run-uuid-2 ".concat(n.name),
                                         onClick: function() {
                                             return s(!a)
                                         },
                                         style: {
                                             cursor: "pointer"
                                         },
-                                        children: xs.Format(n.__queuedCheckRun + "+00:00")
+                                        children: Wa.Format(n.__queuedCheckRun + "+00:00")
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-view-run-uuid-1 ".concat(n.name),
                                         text: "Click to " + (a ? "hide" : "show") + " UUID for this check run.",
                                         position: "bottom"
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-view-run-uuid-2 ".concat(n.name),
                                         text: "Click to " + (a ? "hide" : "show") + " UUID for this check run.",
@@ -52079,15 +52079,15 @@
                                         id: "tooltip-view-run-action-uuid-2 ".concat(n.name),
                                         onClick: function() {
                                             return s(!a)
                                         },
                                         style: {
                                             cursor: "pointer"
                                         },
-                                        children: xs.Format(n.__queuedActionRun + "+00:00")
+                                        children: Wa.Format(n.__queuedActionRun + "+00:00")
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-view-run-action-uuid-1 ".concat(n.name),
                                         text: "Click to " + (a ? "hide" : "show") + " UUID for this action run.",
                                         position: "bottom"
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-view-run-action-uuid-2 ".concat(n.name),
                                         text: "Click to " + (a ? "hide" : "show") + " UUID for this action run.",
@@ -52400,15 +52400,15 @@
                                                                 id: "tooltip-history-timestamp-".concat(i.name, "-").concat(n),
                                                                 onClick: function() {
                                                                     u(i, e, l(e), a)
                                                                 },
                                                                 style: {
                                                                     cursor: "pointer"
                                                                 },
-                                                                children: xs.Format(d(e))
+                                                                children: Wa.Format(d(e))
                                                             }), (0, wo.jsx)(oa, {
                                                                 id: "tooltip-history-timestamp-".concat(i.name, "-").concat(n),
                                                                 text: uo.Ago(d(e)),
                                                                 position: "right",
                                                                 shape: "squared"
                                                             }), "\xa0\xa0"]
                                                         }), (0, wo.jsxs)("td", {
@@ -52844,15 +52844,15 @@
                         i = e.groupList,
                         a = e.fetchResult,
                         s = e.runActionAllowedState,
                         u = l((0, t.useState)(!1), 2),
                         c = u[0],
                         d = u[1],
                         p = l(Ls(), 1)[0],
-                        f = hs();
+                        f = Ms();
 
                     function h() {
                         if (c) {
                             var e;
                             d(!1);
                             var t = null === (e = r.__result) || void 0 === e ? void 0 : e.get("action");
                             t && (Hs(r, t, o, i, f), s[1](!1))
@@ -53537,15 +53537,15 @@
                                                                 style: {
                                                                     width: "20%"
                                                                 },
                                                                 children: [ks.Format(e.timestamp), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
                                                                     children: uo.Format(e.timestamp)
                                                                 }), (0, wo.jsx)(oa, {
                                                                     id: "recent-runs-timestamp ".concat(i),
-                                                                    text: Es.Format(e.timestamp, xs.Now(), !0, null, null, "agoy")
+                                                                    text: Es.Format(e.timestamp, Wa.Now(), !0, null, null, "agoy")
                                                                 }), "\xa0\xa0"]
                                                             }), (0, wo.jsxs)("td", {
                                                                 style: {
                                                                     width: "45%"
                                                                 },
                                                                 children: [(0, wo.jsx)("b", {
                                                                     style: {
@@ -53914,15 +53914,15 @@
                                                 children: [(0, wo.jsx)("td", {
                                                     style: c,
                                                     children: "Updated:"
                                                 }), (0, wo.jsx)("td", {
                                                     style: l,
                                                     children: (0, wo.jsx)("span", {
                                                         id: "tooltip-lambda-updated-".concat(u.lambda_name),
-                                                        children: xs.Format(u.lambda_modified)
+                                                        children: Wa.Format(u.lambda_modified)
                                                     })
                                                 }), (0, wo.jsx)(oa, {
                                                     id: "tooltip-lambda-updated-".concat(u.lambda_name),
                                                     text: uo.Ago(u.lambda_modified),
                                                     position: "right",
                                                     shape: "squared"
                                                 })]
@@ -55639,15 +55639,15 @@
                                                             id: "tooltip-timestamp-".concat(n),
                                                             onClick: function() {
                                                                 return E(i, e, a(e))
                                                             },
                                                             style: {
                                                                 cursor: "pointer"
                                                             },
-                                                            children: xs.Format(u(e))
+                                                            children: Wa.Format(u(e))
                                                         }), (0, wo.jsx)(oa, {
                                                             id: "tooltip-timestamp-".concat(n),
                                                             text: uo.Ago(u(e)),
                                                             position: "right",
                                                             shape: "squared"
                                                         }), "\xa0\xa0"]
                                                     }), (0, wo.jsxs)("td", {
@@ -56683,15 +56683,15 @@
                         })]
                     })
                 },
                 Uu = function(e) {
                     var n, r, o, i, a, s, u, c, d, p, f, h, g, y, m, v, M, j, b, w, x, N, I, D, L, S, k = Fa(),
                         C = Iu(),
                         E = Me(),
-                        T = l(Ba(), 1)[0],
+                        T = l(Ha(), 1)[0],
                         A = tn.IsFoursightFourfront(k) ? "#14533C" : "#143C53",
                         z = ln.LightenDarkenColor(ln.GetBackgroundColor(), -10);
                     return (0, wo.jsx)(wo.Fragment, {
                         children: k.loading ? (0, wo.jsxs)("div", {
                             style: {
                                 width: "100%"
                             },
@@ -56970,15 +56970,15 @@
                                                 style: {
                                                     paddingRight: "10pt",
                                                     whiteSpace: "nowrap",
                                                     color: "#D6EAF8"
                                                 },
                                                 align: "right",
                                                 children: [(0, wo.jsx)("small", {
-                                                    children: (0, wo.jsx)(xs.Live, {
+                                                    children: (0, wo.jsx)(Wa.Live, {
                                                         verbose: !0,
                                                         timezone: !1
                                                     })
                                                 }), (null === (c = k.app) || void 0 === c || null === (d = c.credentials) || void 0 === d ? void 0 : d.aws_account_name) && (0, wo.jsxs)(wo.Fragment, {
                                                     children: ["\xa0|\xa0", (0, wo.jsx)(qe, {
                                                         id: "tooltip-header-account",
                                                         to: $r.Path("/login"),
@@ -57541,15 +57541,15 @@
                                     top: "4pt",
                                     bottom: "10pt"
                                 }), D && (0, wo.jsx)(wo.Fragment, {
                                     children: (0, wo.jsx)("div", {
                                         style: {
                                             marginBottom: "12pt"
                                         },
-                                        children: (0, wo.jsx)(ds, {
+                                        children: (0, wo.jsx)(ys, {
                                             account: N,
                                             header: w,
                                             decrementAccountCount: function() {},
                                             all: !0,
                                             brighten: !0
                                         })
                                     })
@@ -58014,15 +58014,15 @@
                         ie = l((0, t.useState)(!1), 2),
                         ae = ie[0],
                         se = ie[1],
                         ue = l((0, t.useState)(!1), 2),
                         le = ue[0],
                         ce = ue[1],
                         de = Ua("/portal_access_key"),
-                        pe = hs();
+                        pe = Ms();
                     return te.error ? (0, wo.jsx)(ua, {
                         error: te.error,
                         message: "Error loading info from Foursight API"
                     }) : (0, wo.jsxs)("div", {
                         className: "container",
                         children: [(0, wo.jsxs)(Fu, {
                             info: te,
@@ -58489,15 +58489,15 @@
                             }), (0, wo.jsx)(Bu, {
                                 name: "Size",
                                 value: te.get("app.lambda.lambda_code_size"),
                                 monospace: !0,
                                 size: "2"
                             }), (0, wo.jsx)(Bu, {
                                 name: "Modified",
-                                value: xs.Format(te.get("app.lambda.lambda_modified")),
+                                value: Wa.Format(te.get("app.lambda.lambda_modified")),
                                 monospace: !0,
                                 size: "2"
                             }), (0, wo.jsx)(Bu, {
                                 name: "Role",
                                 value: te.get("app.lambda.lambda_role"),
                                 monospace: !0,
                                 size: "2"
@@ -58562,15 +58562,15 @@
                             }), (0, wo.jsx)(oa, {
                                 id: "tooltip-info-clear",
                                 position: "bottom",
                                 size: "small",
                                 text: "Click to clear any server-side caches."
                             }), (0, wo.jsx)(Bu, {
                                 name: "App Deployed At",
-                                value: rn.IsLocal() ? "running locally" + (ft.IsLocalCrossOrigin() ? " (cross-origin)" : "") : xs.Format(null === (B = ee.app) || void 0 === B ? void 0 : B.deployed) + Es.Format(null === (Y = ee.app) || void 0 === Y ? void 0 : Y.deployed, new Date, !0, "just now", "|", "ago"),
+                                value: rn.IsLocal() ? "running locally" + (ft.IsLocalCrossOrigin() ? " (cross-origin)" : "") : Wa.Format(null === (B = ee.app) || void 0 === B ? void 0 : B.deployed) + Es.Format(null === (Y = ee.app) || void 0 === Y ? void 0 : Y.deployed, new Date, !0, "just now", "|", "ago"),
                                 monospace: !0,
                                 copy: !0,
                                 optional: !0,
                                 size: "2"
                             }), (0, wo.jsx)(Bu, {
                                 name: "App Launched At",
                                 value: (null === (Q = ee.app) || void 0 === Q ? void 0 : Q.launched) + Es.Format(null === (G = ee.app) || void 0 === G ? void 0 : G.launched, new Date, !0, "just now", "|", "ago"),
@@ -58668,15 +58668,15 @@
                             }) : (0, wo.jsx)("span", {})
                         }), (null === ($ = ee.app) || void 0 === $ ? void 0 : $.accounts) && (0, wo.jsx)("div", {
                             className: "container",
                             style: {
                                 marginTop: "4pt"
                             },
                             children: ae ? (0, wo.jsx)(wo.Fragment, {
-                                children: (0, wo.jsx)(ps, {})
+                                children: (0, wo.jsx)(ms, {})
                             }) : (0, wo.jsxs)(wo.Fragment, {
                                 children: [(0, wo.jsx)("b", {
                                     onClick: function() {
                                         return se(!0)
                                     },
                                     style: {
                                         cursor: "pointer"
@@ -66893,15 +66893,15 @@
                             }))]
                         })]
                     })
                 },
                 mf = function(e) {
                     var t = e.vpc,
                         n = e.keyedState,
-                        r = l(Va(n), 2),
+                        r = l(Xa(n), 2),
                         o = r[0],
                         i = r[1],
                         a = function(e) {
                             return o[e]
                         },
                         s = function(e) {
                             return i(et({}, e, !o[e]))
@@ -67197,15 +67197,15 @@
                             }))]
                         })]
                     })
                 },
                 Mf = function(e) {
                     var t = e.subnet,
                         n = e.keyedState,
-                        r = l(Va(n), 2),
+                        r = l(Xa(n), 2),
                         o = r[0],
                         i = r[1],
                         a = function() {
                             return o["showTags"]
                         };
                     return (0, wo.jsx)(wo.Fragment, {
                         children: (0, wo.jsxs)("div", {
@@ -67407,15 +67407,15 @@
                             }))]
                         })]
                     })
                 },
                 bf = function(e) {
                     var t = e.securityGroup,
                         n = e.keyedState,
-                        r = l(Va(n), 2),
+                        r = l(Xa(n), 2),
                         o = r[0],
                         i = r[1],
                         a = function(e) {
                             return o[e]
                         },
                         s = function(e) {
                             return i(et({}, e, !o[e]))
@@ -67847,15 +67847,15 @@
                         })]
                     })
                 },
                 Df = function(e) {
                     var t, n, r, o, i, a, s, u, c, d, p, f, h = e.stackName,
                         g = e.keyedState,
                         y = e.hide,
-                        m = l(Va(g), 2),
+                        m = l(Xa(g), 2),
                         v = m[0],
                         M = m[1],
                         j = Ua("/aws/stacks/".concat(h), {
                             cache: !0
                         }),
                         b = function(e) {
                             return v[e]
@@ -68430,15 +68430,15 @@
                                     children: "Deployed"
                                 }), ": ", null === (o = i.data) || void 0 === o ? void 0 : o.most_recent_deployed]
                             })
                         })
                     })
                 },
                 Af = function(e) {
-                    var t, n = l(Va(e.keyedState), 2),
+                    var t, n = l(Xa(e.keyedState), 2),
                         r = n[0],
                         o = n[1],
                         i = function() {
                             return r["detail"]
                         },
                         a = e.commonInitialSubstring ? null === (t = e.cluster) || void 0 === t ? void 0 : t.replace(e.commonInitialSubstring, "") : e.cluster;
                     return (0, wo.jsxs)("div", {
@@ -68513,16 +68513,16 @@
                                     })]
                                 }, e)
                             }))]
                         })]
                     })
                 },
                 Of = function() {
-                    var e = Va(),
-                        n = Za(),
+                    var e = Xa(),
+                        n = $a(),
                         r = [{
                             type: "stack",
                             create: function(e, t, n, r) {
                                 var o = r.keyedState;
                                 return (0, wo.jsx)(Df, {
                                     stackName: e,
                                     keyedState: o.keyed(t),
@@ -68566,22 +68566,22 @@
                                     keyedState: o.keyed(t),
                                     hide: n
                                 })
                             }
                         }, {
                             type: "gac",
                             create: function(e, t, n, r) {
-                                return (0, wo.jsx)(Ka, {
+                                return (0, wo.jsx)(ns, {
                                     hide: n
                                 })
                             }
                         }, {
                             type: "secrets",
                             create: function(e, t, r, o) {
-                                return (0, wo.jsx)(Xa, {
+                                return (0, wo.jsx)(rs, {
                                     name: e,
                                     hide: function() {
                                         return n.unsetList("secrets", e), r()
                                     }
                                 })
                             }
                         }, {
@@ -68597,16 +68597,16 @@
                                 var o = r.keyedState;
                                 return (0, wo.jsx)(zf, {
                                     keyedState: o.keyed(t),
                                     hide: n
                                 })
                             }
                         }],
-                        o = Qa(r),
-                        i = Qa(r);
+                        o = Za(r),
+                        i = Za(r);
                     var a = function() {
                             return o.toggle("vpcs")
                         },
                         s = function() {
                             return o.toggle("ecosystem")
                         };
                     return (0, t.useEffect)((function() {
@@ -68668,15 +68668,15 @@
                                     }), (0, wo.jsx)(hf, {
                                         showEcsClusters: function() {
                                             return o.selected("ecs-clusters")
                                         },
                                         toggleEcsClusters: function() {
                                             return o.toggle("ecs-clusters")
                                         }
-                                    }), (0, wo.jsx)(Ja, {
+                                    }), (0, wo.jsx)(ts, {
                                         toggleSecrets: function(e) {
                                             return o.toggle("secrets", e) ? n.setList("secrets", e) : n.unsetList("secrets", e)
                                         },
                                         selectedSecrets: function(e) {
                                             return o.selected("secrets", e)
                                         }
                                     }), (0, wo.jsx)(If, {
@@ -69152,21 +69152,21 @@
                             map: function(e) {
                                 return t.statusTitle(e)
                             }
                         }, {
                             label: "Created",
                             name: "created",
                             map: function(e) {
-                                return xs.Format(e)
+                                return Wa.Format(e)
                             }
                         }, {
                             label: "Updated",
                             name: "updated",
                             map: function(e) {
-                                return xs.Format(e)
+                                return Wa.Format(e)
                             }
                         }, {
                             label: "UUID",
                             name: "uuid"
                         }];
                     return tn.IsFoursightFourfront(Fa()) && (n = n.filter((function(e) {
                         return "institution" !== e.name && "project" !== e.name && "roles" !== e.name && "role" !== e.name
@@ -70024,15 +70024,15 @@
                                 o((function(t) {
                                     var n, r = c(t);
                                     try {
                                         for (r.s(); !(n = r.n()).done;) {
                                             var o, i = n.value;
                                             "email" === i.name ? i.value = e.email : "first_name" === i.name ? i.value = e.first_name : "last_name" === i.name ? i.value = e.last_name : "admin" === i.name ? i.value = !(null === (o = e.groups) || void 0 === o || !o.includes("admin")) : "project" === i.name ? i.value = e.project : "role" === i.name ? i.value = function(t) {
                                                 return void 0 === t || null === t ? "-" : f.userRole(e, t || (null === e || void 0 === e ? void 0 : e.project)) || "-"
-                                            } : "institution" === i.name ? i.value = e.institution : "status" === i.name ? i.value = e.status : "created" === i.name ? i.value = xs.Format(e.created) : "updated" === i.name ? i.value = xs.Format(e.updated) : "uuid" === i.name && (i.value = e.uuid)
+                                            } : "institution" === i.name ? i.value = e.institution : "status" === i.name ? i.value = e.status : "created" === i.name ? i.value = Wa.Format(e.created) : "updated" === i.name ? i.value = Wa.Format(e.updated) : "uuid" === i.name && (i.value = e.uuid)
                                         }
                                     } catch (a) {
                                         r.e(a)
                                     } finally {
                                         r.f()
                                     }
                                     return p(t)
@@ -70662,15 +70662,15 @@
                                         path: "/api/react/:environ",
                                         element: (0, wo.jsx)(ze, {
                                             to: t()
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/accounts",
                                         element: (0, wo.jsx)(wa.AuthorizationRequired, {
-                                            children: (0, wo.jsx)(fs, {})
+                                            children: (0, wo.jsx)(vs, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/env",
                                         element: (0, wo.jsx)(wa.KnownEnvRequired, {
                                             children: (0, wo.jsx)(Du, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
@@ -70752,15 +70752,15 @@
                                         path: "/api/react/:environ/portal_access_key",
                                         element: (0, wo.jsx)(wa.KnownEnvRequired, {
                                             children: (0, wo.jsx)(Ff, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/apicache",
                                         element: (0, wo.jsx)(wa.AuthorizationRequired, {
-                                            children: (0, wo.jsx)(vs, {})
+                                            children: (0, wo.jsx)(xs, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/forbidden",
                                         element: (0, wo.jsx)(Su, {})
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/error",
                                         element: (0, wo.jsx)(ma, {})
```

### Comparing `foursight_core-4.3.0.2b5/foursight_core/route_prefixes.py` & `foursight_core-4.3.0.2b6/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/routes.py` & `foursight_core-4.3.0.2b6/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/run_result.py` & `foursight_core-4.3.0.2b6/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/s3_connection.py` & `foursight_core-4.3.0.2b6/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/schedule_decorator.py` & `foursight_core-4.3.0.2b6/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/sqs_utils.py` & `foursight_core-4.3.0.2b6/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/stage.py` & `foursight_core-4.3.0.2b6/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/templates/base.html` & `foursight_core-4.3.0.2b6/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/templates/header.html` & `foursight_core-4.3.0.2b6/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/templates/history.html` & `foursight_core-4.3.0.2b6/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/templates/info.html` & `foursight_core-4.3.0.2b6/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/templates/unused.html` & `foursight_core-4.3.0.2b6/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/templates/user.html` & `foursight_core-4.3.0.2b6/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/templates/users.html` & `foursight_core-4.3.0.2b6/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/templates/view_checks.html` & `foursight_core-4.3.0.2b6/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/foursight_core/templates/view_groups.html` & `foursight_core-4.3.0.2b6/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b5/pyproject.toml` & `foursight_core-4.3.0.2b6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.3.0.2b5"  # TODO: To become 4.4.0
+version = "4.3.0.2b6"  # TODO: To become 4.4.0
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
```

### Comparing `foursight_core-4.3.0.2b5/PKG-INFO` & `foursight_core-4.3.0.2b6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.3.0.2b5
+Version: 4.3.0.2b6
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

