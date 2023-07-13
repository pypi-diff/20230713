# Comparing `tmp/fabric-credmgr-client-1.6.0b1.tar.gz` & `tmp/fabric-credmgr-client-1.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-credmgr-client-1.6.0b1.tar", last modified: Wed Jul 12 19:47:38 2023, max compression
+gzip compressed data, was "fabric-credmgr-client-1.6.0b2.tar", last modified: Thu Jul 13 13:33:58 2023, max compression
```

## Comparing `fabric-credmgr-client-1.6.0b1.tar` & `fabric-credmgr-client-1.6.0b2.tar`

### file list

```diff
@@ -1,98 +1,98 @@
--rw-r--r--   0        0        0      794 2023-05-11 18:03:22.615968 fabric-credmgr-client-1.6.0b1/.gitignore
--rw-r--r--   0        0        0     1030 2023-05-11 18:03:22.616147 fabric-credmgr-client-1.6.0b1/.swagger-codegen-ignore
--rw-r--r--   0        0        0        7 2023-06-27 21:01:47.904517 fabric-credmgr-client-1.6.0b1/.swagger-codegen/VERSION
--rw-r--r--   0        0        0      349 2023-05-11 18:03:22.616544 fabric-credmgr-client-1.6.0b1/.travis.yml
--rw-r--r--   0        0        0     1071 2023-05-11 18:03:22.616706 fabric-credmgr-client-1.6.0b1/LICENSE
--rw-r--r--   0        0        0     4901 2023-07-03 21:15:47.092949 fabric-credmgr-client-1.6.0b1/README.md
--rw-r--r--   0        0        0     1315 2023-05-11 18:03:22.617177 fabric-credmgr-client-1.6.0b1/docs/DefaultApi.md
--rw-r--r--   0        0        0      343 2023-05-11 18:03:22.617302 fabric-credmgr-client-1.6.0b1/docs/Jwks.md
--rw-r--r--   0        0        0      600 2023-05-11 18:03:22.617403 fabric-credmgr-client-1.6.0b1/docs/JwksKeys.md
--rw-r--r--   0        0        0      331 2023-05-11 18:03:22.617518 fabric-credmgr-client-1.6.0b1/docs/Request.md
--rw-r--r--   0        0        0      329 2023-06-27 21:01:06.115302 fabric-credmgr-client-1.6.0b1/docs/RevokeList.md
--rw-r--r--   0        0        0      556 2023-05-11 18:03:22.617616 fabric-credmgr-client-1.6.0b1/docs/Status200OkNoContent.md
--rw-r--r--   0        0        0      404 2023-05-11 18:03:22.617743 fabric-credmgr-client-1.6.0b1/docs/Status200OkNoContentData.md
--rw-r--r--   0        0        0      498 2023-06-27 21:01:14.867751 fabric-credmgr-client-1.6.0b1/docs/Status200OkPaginated.md
--rw-r--r--   0        0        0      434 2023-05-11 18:03:22.617843 fabric-credmgr-client-1.6.0b1/docs/Status200OkSingle.md
--rw-r--r--   0        0        0      394 2023-05-11 18:03:22.617940 fabric-credmgr-client-1.6.0b1/docs/Status400BadRequest.md
--rw-r--r--   0        0        0      566 2023-05-11 18:03:22.618030 fabric-credmgr-client-1.6.0b1/docs/Status400BadRequestErrors.md
--rw-r--r--   0        0        0      560 2023-05-11 18:03:22.618124 fabric-credmgr-client-1.6.0b1/docs/Status401Unauthorized.md
--rw-r--r--   0        0        0      409 2023-05-11 18:03:22.618211 fabric-credmgr-client-1.6.0b1/docs/Status401UnauthorizedErrors.md
--rw-r--r--   0        0        0      551 2023-05-11 18:03:22.618321 fabric-credmgr-client-1.6.0b1/docs/Status403Forbidden.md
--rw-r--r--   0        0        0      403 2023-05-11 18:03:22.618447 fabric-credmgr-client-1.6.0b1/docs/Status403ForbiddenErrors.md
--rw-r--r--   0        0        0      548 2023-05-11 18:03:22.618553 fabric-credmgr-client-1.6.0b1/docs/Status404NotFound.md
--rw-r--r--   0        0        0      402 2023-05-11 18:03:22.618642 fabric-credmgr-client-1.6.0b1/docs/Status404NotFoundErrors.md
--rw-r--r--   0        0        0      581 2023-05-11 18:03:22.618726 fabric-credmgr-client-1.6.0b1/docs/Status500InternalServerError.md
--rw-r--r--   0        0        0      425 2023-05-11 18:03:22.618844 fabric-credmgr-client-1.6.0b1/docs/Status500InternalServerErrorErrors.md
--rw-r--r--   0        0        0      446 2023-05-11 18:03:22.618969 fabric-credmgr-client-1.6.0b1/docs/Success.md
--rw-r--r--   0        0        0      744 2023-07-03 21:09:18.881186 fabric-credmgr-client-1.6.0b1/docs/Token.md
--rw-r--r--   0        0        0      374 2023-06-27 21:01:33.064893 fabric-credmgr-client-1.6.0b1/docs/TokenPost.md
--rw-r--r--   0        0        0      339 2023-06-27 21:01:33.065465 fabric-credmgr-client-1.6.0b1/docs/Tokens.md
--rw-r--r--   0        0        0    12455 2023-07-03 21:25:53.675903 fabric-credmgr-client-1.6.0b1/docs/TokensApi.md
--rw-r--r--   0        0        0      352 2023-05-11 18:03:22.619490 fabric-credmgr-client-1.6.0b1/docs/Version.md
--rw-r--r--   0        0        0     1205 2023-05-11 18:03:22.619644 fabric-credmgr-client-1.6.0b1/docs/VersionApi.md
--rw-r--r--   0        0        0      346 2023-05-11 18:03:22.619831 fabric-credmgr-client-1.6.0b1/docs/VersionData.md
--rw-r--r--   0        0        0       50 2023-07-03 21:25:53.679973 fabric-credmgr-client-1.6.0b1/fabric_cm/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 18:03:22.620222 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/__init__.py
--rw-r--r--   0        0        0     9229 2023-07-05 18:31:15.572470 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/credmgr_proxy.py
--rw-r--r--   0        0        0     2789 2023-06-27 22:03:09.209097 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/__init__.py
--rw-r--r--   0        0        0      301 2023-05-11 18:03:22.621111 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/api/__init__.py
--rw-r--r--   0        0        0     3832 2023-05-11 18:03:22.621312 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/api/default_api.py
--rw-r--r--   0        0        0    29459 2023-07-05 15:55:57.673036 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/api/tokens_api.py
--rw-r--r--   0        0        0     3755 2023-05-11 18:03:22.621852 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/api/version_api.py
--rw-r--r--   0        0        0    25120 2023-07-05 15:48:03.304939 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/api_client.py
--rw-r--r--   0        0        0     8387 2023-07-05 13:37:18.798323 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/configuration.py
--rw-r--r--   0        0        0     2387 2023-06-27 22:04:30.468722 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/__init__.py
--rw-r--r--   0        0        0     2964 2023-05-11 18:03:22.622977 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/jwks.py
--rw-r--r--   0        0        0     6062 2023-05-11 18:03:22.623162 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/jwks_keys.py
--rw-r--r--   0        0        0     3299 2023-05-11 18:03:22.623362 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/request.py
--rw-r--r--   0        0        0     3420 2023-07-05 14:09:46.944095 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/revoke_list.py
--rw-r--r--   0        0        0     5011 2023-05-11 18:03:22.623647 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py
--rw-r--r--   0        0        0     3844 2023-05-11 18:03:22.623886 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py
--rw-r--r--   0        0        0     5594 2023-07-03 21:22:41.593440 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status200_ok_paginated.py
--rw-r--r--   0        0        0     4265 2023-05-11 18:03:22.624053 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py
--rw-r--r--   0        0        0     3175 2023-05-11 18:03:22.624285 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py
--rw-r--r--   0        0        0     5783 2023-05-11 18:03:22.624535 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py
--rw-r--r--   0        0        0     5075 2023-05-11 18:03:22.624762 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py
--rw-r--r--   0        0        0     3882 2023-05-11 18:03:22.624915 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py
--rw-r--r--   0        0        0     5006 2023-05-11 18:03:22.625098 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py
--rw-r--r--   0        0        0     3843 2023-05-11 18:03:22.625298 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py
--rw-r--r--   0        0        0     4983 2023-05-11 18:03:22.625479 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status404_not_found.py
--rw-r--r--   0        0        0     3831 2023-05-11 18:03:22.625691 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py
--rw-r--r--   0        0        0     5236 2023-05-11 18:03:22.625944 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py
--rw-r--r--   0        0        0     3975 2023-05-11 18:03:22.626141 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py
--rw-r--r--   0        0        0     9134 2023-07-03 21:17:56.081086 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/token.py
--rw-r--r--   0        0        0     4164 2023-07-03 21:22:20.475432 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/token_post.py
--rw-r--r--   0        0        0     3427 2023-07-05 14:11:56.417253 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/tokens.py
--rw-r--r--   0        0        0     3420 2023-05-11 18:03:22.626788 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/version.py
--rw-r--r--   0        0        0     3894 2023-05-11 18:03:22.627057 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/version_data.py
--rw-r--r--   0        0        0    13000 2023-05-11 18:03:22.627316 fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/rest.py
--rw-r--r--   0        0        0     1663 2023-05-11 18:03:22.627539 fabric-credmgr-client-1.6.0b1/git_push.sh
--rw-r--r--   0        0        0     1101 2023-05-11 18:07:49.170889 fabric-credmgr-client-1.6.0b1/pyproject.toml
--rw-r--r--   0        0        0       16 2023-06-27 21:02:53.084329 fabric-credmgr-client-1.6.0b1/test/__init__.py
--rw-r--r--   0        0        0      857 2023-05-11 18:03:22.628351 fabric-credmgr-client-1.6.0b1/test/test_default_api.py
--rw-r--r--   0        0        0      843 2023-05-11 18:03:22.628520 fabric-credmgr-client-1.6.0b1/test/test_jwks.py
--rw-r--r--   0        0        0      877 2023-05-11 18:03:22.628746 fabric-credmgr-client-1.6.0b1/test/test_jwks_keys.py
--rw-r--r--   0        0        0      867 2023-05-11 18:03:22.628966 fabric-credmgr-client-1.6.0b1/test/test_request.py
--rw-r--r--   0        0        0      879 2023-06-27 21:03:10.900714 fabric-credmgr-client-1.6.0b1/test/test_revoke_list.py
--rw-r--r--   0        0        0      977 2023-05-11 18:03:22.629156 fabric-credmgr-client-1.6.0b1/test/test_status200_ok_no_content.py
--rw-r--r--   0        0        0     1011 2023-05-11 18:03:22.629346 fabric-credmgr-client-1.6.0b1/test/test_status200_ok_no_content_data.py
--rw-r--r--   0        0        0      961 2023-06-27 21:03:24.185152 fabric-credmgr-client-1.6.0b1/test/test_status200_ok_paginated.py
--rw-r--r--   0        0        0      951 2023-05-11 18:03:22.629517 fabric-credmgr-client-1.6.0b1/test/test_status200_ok_single.py
--rw-r--r--   0        0        0      967 2023-05-11 18:03:22.629752 fabric-credmgr-client-1.6.0b1/test/test_status400_bad_request.py
--rw-r--r--   0        0        0     1017 2023-05-11 18:03:22.630042 fabric-credmgr-client-1.6.0b1/test/test_status400_bad_request_errors.py
--rw-r--r--   0        0        0      981 2023-05-11 18:03:22.630229 fabric-credmgr-client-1.6.0b1/test/test_status401_unauthorized.py
--rw-r--r--   0        0        0     1031 2023-05-11 18:03:22.630398 fabric-credmgr-client-1.6.0b1/test/test_status401_unauthorized_errors.py
--rw-r--r--   0        0        0      975 2023-05-11 18:03:22.630574 fabric-credmgr-client-1.6.0b1/test/test_status403_forbidden.py
--rw-r--r--   0        0        0     1025 2023-05-11 18:03:22.630852 fabric-credmgr-client-1.6.0b1/test/test_status403_forbidden_errors.py
--rw-r--r--   0        0        0      969 2023-05-11 18:03:22.631034 fabric-credmgr-client-1.6.0b1/test/test_status404_not_found.py
--rw-r--r--   0        0        0     1019 2023-05-11 18:03:22.631251 fabric-credmgr-client-1.6.0b1/test/test_status404_not_found_errors.py
--rw-r--r--   0        0        0     1059 2023-05-11 18:03:22.631443 fabric-credmgr-client-1.6.0b1/test/test_status500_internal_server_error.py
--rw-r--r--   0        0        0     1109 2023-05-11 18:03:22.631652 fabric-credmgr-client-1.6.0b1/test/test_status500_internal_server_error_errors.py
--rw-r--r--   0        0        0      869 2023-05-11 18:03:22.631826 fabric-credmgr-client-1.6.0b1/test/test_token.py
--rw-r--r--   0        0        0      877 2023-05-11 18:03:22.632046 fabric-credmgr-client-1.6.0b1/test/test_tokens.py
--rw-r--r--   0        0        0     1838 2023-07-03 21:16:41.118103 fabric-credmgr-client-1.6.0b1/test/test_tokens_api.py
--rw-r--r--   0        0        0      885 2023-05-11 18:03:22.632450 fabric-credmgr-client-1.6.0b1/test/test_version.py
--rw-r--r--   0        0        0      816 2023-05-11 18:03:22.632625 fabric-credmgr-client-1.6.0b1/test/test_version_api.py
--rw-r--r--   0        0        0      919 2023-05-11 18:03:22.632817 fabric-credmgr-client-1.6.0b1/test/test_version_data.py
--rw-r--r--   0        0        0      143 2023-05-11 18:03:22.632996 fabric-credmgr-client-1.6.0b1/tox.ini
--rw-r--r--   0        0        0     5885 1970-01-01 00:00:00.000000 fabric-credmgr-client-1.6.0b1/PKG-INFO
+-rw-r--r--   0        0        0      794 2023-05-11 18:03:22.615968 fabric-credmgr-client-1.6.0b2/.gitignore
+-rw-r--r--   0        0        0     1030 2023-05-11 18:03:22.616147 fabric-credmgr-client-1.6.0b2/.swagger-codegen-ignore
+-rw-r--r--   0        0        0        7 2023-06-27 21:01:47.904517 fabric-credmgr-client-1.6.0b2/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0      349 2023-05-11 18:03:22.616544 fabric-credmgr-client-1.6.0b2/.travis.yml
+-rw-r--r--   0        0        0     1071 2023-05-11 18:03:22.616706 fabric-credmgr-client-1.6.0b2/LICENSE
+-rw-r--r--   0        0        0     4901 2023-07-03 21:15:47.092949 fabric-credmgr-client-1.6.0b2/README.md
+-rw-r--r--   0        0        0     1315 2023-05-11 18:03:22.617177 fabric-credmgr-client-1.6.0b2/docs/DefaultApi.md
+-rw-r--r--   0        0        0      343 2023-05-11 18:03:22.617302 fabric-credmgr-client-1.6.0b2/docs/Jwks.md
+-rw-r--r--   0        0        0      600 2023-05-11 18:03:22.617403 fabric-credmgr-client-1.6.0b2/docs/JwksKeys.md
+-rw-r--r--   0        0        0      331 2023-05-11 18:03:22.617518 fabric-credmgr-client-1.6.0b2/docs/Request.md
+-rw-r--r--   0        0        0      329 2023-06-27 21:01:06.115302 fabric-credmgr-client-1.6.0b2/docs/RevokeList.md
+-rw-r--r--   0        0        0      556 2023-05-11 18:03:22.617616 fabric-credmgr-client-1.6.0b2/docs/Status200OkNoContent.md
+-rw-r--r--   0        0        0      404 2023-05-11 18:03:22.617743 fabric-credmgr-client-1.6.0b2/docs/Status200OkNoContentData.md
+-rw-r--r--   0        0        0      498 2023-06-27 21:01:14.867751 fabric-credmgr-client-1.6.0b2/docs/Status200OkPaginated.md
+-rw-r--r--   0        0        0      434 2023-05-11 18:03:22.617843 fabric-credmgr-client-1.6.0b2/docs/Status200OkSingle.md
+-rw-r--r--   0        0        0      394 2023-05-11 18:03:22.617940 fabric-credmgr-client-1.6.0b2/docs/Status400BadRequest.md
+-rw-r--r--   0        0        0      566 2023-05-11 18:03:22.618030 fabric-credmgr-client-1.6.0b2/docs/Status400BadRequestErrors.md
+-rw-r--r--   0        0        0      560 2023-05-11 18:03:22.618124 fabric-credmgr-client-1.6.0b2/docs/Status401Unauthorized.md
+-rw-r--r--   0        0        0      409 2023-05-11 18:03:22.618211 fabric-credmgr-client-1.6.0b2/docs/Status401UnauthorizedErrors.md
+-rw-r--r--   0        0        0      551 2023-05-11 18:03:22.618321 fabric-credmgr-client-1.6.0b2/docs/Status403Forbidden.md
+-rw-r--r--   0        0        0      403 2023-05-11 18:03:22.618447 fabric-credmgr-client-1.6.0b2/docs/Status403ForbiddenErrors.md
+-rw-r--r--   0        0        0      548 2023-05-11 18:03:22.618553 fabric-credmgr-client-1.6.0b2/docs/Status404NotFound.md
+-rw-r--r--   0        0        0      402 2023-05-11 18:03:22.618642 fabric-credmgr-client-1.6.0b2/docs/Status404NotFoundErrors.md
+-rw-r--r--   0        0        0      581 2023-05-11 18:03:22.618726 fabric-credmgr-client-1.6.0b2/docs/Status500InternalServerError.md
+-rw-r--r--   0        0        0      425 2023-05-11 18:03:22.618844 fabric-credmgr-client-1.6.0b2/docs/Status500InternalServerErrorErrors.md
+-rw-r--r--   0        0        0      446 2023-05-11 18:03:22.618969 fabric-credmgr-client-1.6.0b2/docs/Success.md
+-rw-r--r--   0        0        0      744 2023-07-03 21:09:18.881186 fabric-credmgr-client-1.6.0b2/docs/Token.md
+-rw-r--r--   0        0        0      374 2023-06-27 21:01:33.064893 fabric-credmgr-client-1.6.0b2/docs/TokenPost.md
+-rw-r--r--   0        0        0      339 2023-06-27 21:01:33.065465 fabric-credmgr-client-1.6.0b2/docs/Tokens.md
+-rw-r--r--   0        0        0    12455 2023-07-03 21:25:53.675903 fabric-credmgr-client-1.6.0b2/docs/TokensApi.md
+-rw-r--r--   0        0        0      352 2023-05-11 18:03:22.619490 fabric-credmgr-client-1.6.0b2/docs/Version.md
+-rw-r--r--   0        0        0     1205 2023-05-11 18:03:22.619644 fabric-credmgr-client-1.6.0b2/docs/VersionApi.md
+-rw-r--r--   0        0        0      346 2023-05-11 18:03:22.619831 fabric-credmgr-client-1.6.0b2/docs/VersionData.md
+-rw-r--r--   0        0        0       50 2023-07-13 13:33:43.250655 fabric-credmgr-client-1.6.0b2/fabric_cm/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 18:03:22.620222 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/__init__.py
+-rw-r--r--   0        0        0     9120 2023-07-13 13:33:36.122134 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/credmgr_proxy.py
+-rw-r--r--   0        0        0     2789 2023-06-27 22:03:09.209097 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/__init__.py
+-rw-r--r--   0        0        0      301 2023-05-11 18:03:22.621111 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/api/__init__.py
+-rw-r--r--   0        0        0     3832 2023-05-11 18:03:22.621312 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/api/default_api.py
+-rw-r--r--   0        0        0    29459 2023-07-05 15:55:57.673036 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/api/tokens_api.py
+-rw-r--r--   0        0        0     3755 2023-05-11 18:03:22.621852 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/api/version_api.py
+-rw-r--r--   0        0        0    25120 2023-07-05 15:48:03.304939 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/api_client.py
+-rw-r--r--   0        0        0     8387 2023-07-05 13:37:18.798323 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/configuration.py
+-rw-r--r--   0        0        0     2387 2023-06-27 22:04:30.468722 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/__init__.py
+-rw-r--r--   0        0        0     2964 2023-05-11 18:03:22.622977 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/jwks.py
+-rw-r--r--   0        0        0     6062 2023-05-11 18:03:22.623162 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/jwks_keys.py
+-rw-r--r--   0        0        0     3299 2023-05-11 18:03:22.623362 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/request.py
+-rw-r--r--   0        0        0     3420 2023-07-05 14:09:46.944095 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/revoke_list.py
+-rw-r--r--   0        0        0     5011 2023-05-11 18:03:22.623647 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py
+-rw-r--r--   0        0        0     3844 2023-05-11 18:03:22.623886 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py
+-rw-r--r--   0        0        0     5594 2023-07-03 21:22:41.593440 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status200_ok_paginated.py
+-rw-r--r--   0        0        0     4265 2023-05-11 18:03:22.624053 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py
+-rw-r--r--   0        0        0     3175 2023-05-11 18:03:22.624285 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py
+-rw-r--r--   0        0        0     5783 2023-05-11 18:03:22.624535 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py
+-rw-r--r--   0        0        0     5075 2023-05-11 18:03:22.624762 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py
+-rw-r--r--   0        0        0     3882 2023-05-11 18:03:22.624915 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py
+-rw-r--r--   0        0        0     5006 2023-05-11 18:03:22.625098 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py
+-rw-r--r--   0        0        0     3843 2023-05-11 18:03:22.625298 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py
+-rw-r--r--   0        0        0     4983 2023-05-11 18:03:22.625479 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status404_not_found.py
+-rw-r--r--   0        0        0     3831 2023-05-11 18:03:22.625691 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py
+-rw-r--r--   0        0        0     5236 2023-05-11 18:03:22.625944 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py
+-rw-r--r--   0        0        0     3975 2023-05-11 18:03:22.626141 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0     9134 2023-07-03 21:17:56.081086 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/token.py
+-rw-r--r--   0        0        0     4164 2023-07-03 21:22:20.475432 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/token_post.py
+-rw-r--r--   0        0        0     3427 2023-07-05 14:11:56.417253 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/tokens.py
+-rw-r--r--   0        0        0     3420 2023-05-11 18:03:22.626788 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/version.py
+-rw-r--r--   0        0        0     3894 2023-05-11 18:03:22.627057 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/version_data.py
+-rw-r--r--   0        0        0    13000 2023-05-11 18:03:22.627316 fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/rest.py
+-rw-r--r--   0        0        0     1663 2023-05-11 18:03:22.627539 fabric-credmgr-client-1.6.0b2/git_push.sh
+-rw-r--r--   0        0        0     1101 2023-05-11 18:07:49.170889 fabric-credmgr-client-1.6.0b2/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-06-27 21:02:53.084329 fabric-credmgr-client-1.6.0b2/test/__init__.py
+-rw-r--r--   0        0        0      857 2023-05-11 18:03:22.628351 fabric-credmgr-client-1.6.0b2/test/test_default_api.py
+-rw-r--r--   0        0        0      843 2023-05-11 18:03:22.628520 fabric-credmgr-client-1.6.0b2/test/test_jwks.py
+-rw-r--r--   0        0        0      877 2023-05-11 18:03:22.628746 fabric-credmgr-client-1.6.0b2/test/test_jwks_keys.py
+-rw-r--r--   0        0        0      867 2023-05-11 18:03:22.628966 fabric-credmgr-client-1.6.0b2/test/test_request.py
+-rw-r--r--   0        0        0      879 2023-06-27 21:03:10.900714 fabric-credmgr-client-1.6.0b2/test/test_revoke_list.py
+-rw-r--r--   0        0        0      977 2023-05-11 18:03:22.629156 fabric-credmgr-client-1.6.0b2/test/test_status200_ok_no_content.py
+-rw-r--r--   0        0        0     1011 2023-05-11 18:03:22.629346 fabric-credmgr-client-1.6.0b2/test/test_status200_ok_no_content_data.py
+-rw-r--r--   0        0        0      961 2023-06-27 21:03:24.185152 fabric-credmgr-client-1.6.0b2/test/test_status200_ok_paginated.py
+-rw-r--r--   0        0        0      951 2023-05-11 18:03:22.629517 fabric-credmgr-client-1.6.0b2/test/test_status200_ok_single.py
+-rw-r--r--   0        0        0      967 2023-05-11 18:03:22.629752 fabric-credmgr-client-1.6.0b2/test/test_status400_bad_request.py
+-rw-r--r--   0        0        0     1017 2023-05-11 18:03:22.630042 fabric-credmgr-client-1.6.0b2/test/test_status400_bad_request_errors.py
+-rw-r--r--   0        0        0      981 2023-05-11 18:03:22.630229 fabric-credmgr-client-1.6.0b2/test/test_status401_unauthorized.py
+-rw-r--r--   0        0        0     1031 2023-05-11 18:03:22.630398 fabric-credmgr-client-1.6.0b2/test/test_status401_unauthorized_errors.py
+-rw-r--r--   0        0        0      975 2023-05-11 18:03:22.630574 fabric-credmgr-client-1.6.0b2/test/test_status403_forbidden.py
+-rw-r--r--   0        0        0     1025 2023-05-11 18:03:22.630852 fabric-credmgr-client-1.6.0b2/test/test_status403_forbidden_errors.py
+-rw-r--r--   0        0        0      969 2023-05-11 18:03:22.631034 fabric-credmgr-client-1.6.0b2/test/test_status404_not_found.py
+-rw-r--r--   0        0        0     1019 2023-05-11 18:03:22.631251 fabric-credmgr-client-1.6.0b2/test/test_status404_not_found_errors.py
+-rw-r--r--   0        0        0     1059 2023-05-11 18:03:22.631443 fabric-credmgr-client-1.6.0b2/test/test_status500_internal_server_error.py
+-rw-r--r--   0        0        0     1109 2023-05-11 18:03:22.631652 fabric-credmgr-client-1.6.0b2/test/test_status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0      869 2023-05-11 18:03:22.631826 fabric-credmgr-client-1.6.0b2/test/test_token.py
+-rw-r--r--   0        0        0      877 2023-05-11 18:03:22.632046 fabric-credmgr-client-1.6.0b2/test/test_tokens.py
+-rw-r--r--   0        0        0     1838 2023-07-03 21:16:41.118103 fabric-credmgr-client-1.6.0b2/test/test_tokens_api.py
+-rw-r--r--   0        0        0      885 2023-05-11 18:03:22.632450 fabric-credmgr-client-1.6.0b2/test/test_version.py
+-rw-r--r--   0        0        0      816 2023-05-11 18:03:22.632625 fabric-credmgr-client-1.6.0b2/test/test_version_api.py
+-rw-r--r--   0        0        0      919 2023-05-11 18:03:22.632817 fabric-credmgr-client-1.6.0b2/test/test_version_data.py
+-rw-r--r--   0        0        0      143 2023-05-11 18:03:22.632996 fabric-credmgr-client-1.6.0b2/tox.ini
+-rw-r--r--   0        0        0     5885 1970-01-01 00:00:00.000000 fabric-credmgr-client-1.6.0b2/PKG-INFO
```

### Comparing `fabric-credmgr-client-1.6.0b1/.gitignore` & `fabric-credmgr-client-1.6.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/.swagger-codegen-ignore` & `fabric-credmgr-client-1.6.0b2/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/LICENSE` & `fabric-credmgr-client-1.6.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/README.md` & `fabric-credmgr-client-1.6.0b2/README.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/docs/DefaultApi.md` & `fabric-credmgr-client-1.6.0b2/docs/DefaultApi.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/docs/JwksKeys.md` & `fabric-credmgr-client-1.6.0b2/docs/JwksKeys.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/docs/Status200OkNoContent.md` & `fabric-credmgr-client-1.6.0b2/docs/Status200OkNoContent.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/docs/Status400BadRequestErrors.md` & `fabric-credmgr-client-1.6.0b2/docs/Status400BadRequestErrors.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/docs/Status401Unauthorized.md` & `fabric-credmgr-client-1.6.0b2/docs/Status401Unauthorized.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/docs/Status403Forbidden.md` & `fabric-credmgr-client-1.6.0b2/docs/Status403Forbidden.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/docs/Status404NotFound.md` & `fabric-credmgr-client-1.6.0b2/docs/Status404NotFound.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/docs/Status500InternalServerError.md` & `fabric-credmgr-client-1.6.0b2/docs/Status500InternalServerError.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/docs/Token.md` & `fabric-credmgr-client-1.6.0b2/docs/Token.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/docs/TokensApi.md` & `fabric-credmgr-client-1.6.0b2/docs/TokensApi.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/docs/VersionApi.md` & `fabric-credmgr-client-1.6.0b2/docs/VersionApi.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/credmgr_proxy.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/credmgr_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,22 +233,21 @@
                                                 offset=offset, token_hash=token_hash, project_id=project_id,
                                                 expires=expiry_time)
 
             return Status.OK, tokens.data if tokens.data is not None else []
         except Exception as e:
             return Status.FAILURE, e
 
-    def token_revoke_list(self, *, token: str, project_id: str) -> Tuple[Status, Union[Exception, List[str]]]:
+    def token_revoke_list(self, *, token: str, project_id: str = None) -> Tuple[Status, Union[Exception, List[str]]]:
         """
         Return list of revoked tokens for a user
         @return list of revoked tokens
         """
-        if token is None or project_id is None:
-            return Status.INVALID_ARGUMENTS, CredMgrException(f"Token {token} and "
-                                                              f"Project Id {project_id} must be specified")
+        if token is None:
+            return Status.INVALID_ARGUMENTS, CredMgrException(f"Token {token} must be specified")
 
         try:
             # Set the tokens
             self.__set_tokens(token=token)
 
             slices = self.tokens_api.tokens_revoke_list_get(project_id=project_id)
```

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/__init__.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/api/default_api.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/api/tokens_api.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/api/tokens_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/api/version_api.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/api/version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/api_client.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/configuration.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/__init__.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/jwks.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/jwks.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/jwks_keys.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/jwks_keys.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/request.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/revoke_list.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/revoke_list.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status200_ok_paginated.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status404_not_found.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/token.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/token.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/token_post.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/token_post.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/tokens.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/tokens.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/version.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/models/version_data.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/fabric_cm/credmgr/swagger_client/rest.py` & `fabric-credmgr-client-1.6.0b2/fabric_cm/credmgr/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/git_push.sh` & `fabric-credmgr-client-1.6.0b2/git_push.sh`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/pyproject.toml` & `fabric-credmgr-client-1.6.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_default_api.py` & `fabric-credmgr-client-1.6.0b2/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_jwks.py` & `fabric-credmgr-client-1.6.0b2/test/test_jwks.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_jwks_keys.py` & `fabric-credmgr-client-1.6.0b2/test/test_jwks_keys.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_request.py` & `fabric-credmgr-client-1.6.0b2/test/test_request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_revoke_list.py` & `fabric-credmgr-client-1.6.0b2/test/test_revoke_list.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_status200_ok_no_content.py` & `fabric-credmgr-client-1.6.0b2/test/test_status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_status200_ok_no_content_data.py` & `fabric-credmgr-client-1.6.0b2/test/test_status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_status200_ok_paginated.py` & `fabric-credmgr-client-1.6.0b2/test/test_status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_status200_ok_single.py` & `fabric-credmgr-client-1.6.0b2/test/test_status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_status400_bad_request.py` & `fabric-credmgr-client-1.6.0b2/test/test_status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_status400_bad_request_errors.py` & `fabric-credmgr-client-1.6.0b2/test/test_status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_status401_unauthorized.py` & `fabric-credmgr-client-1.6.0b2/test/test_status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_status401_unauthorized_errors.py` & `fabric-credmgr-client-1.6.0b2/test/test_status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_status403_forbidden.py` & `fabric-credmgr-client-1.6.0b2/test/test_status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_status403_forbidden_errors.py` & `fabric-credmgr-client-1.6.0b2/test/test_status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_status404_not_found.py` & `fabric-credmgr-client-1.6.0b2/test/test_status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_status404_not_found_errors.py` & `fabric-credmgr-client-1.6.0b2/test/test_status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_status500_internal_server_error.py` & `fabric-credmgr-client-1.6.0b2/test/test_status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_status500_internal_server_error_errors.py` & `fabric-credmgr-client-1.6.0b2/test/test_status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_token.py` & `fabric-credmgr-client-1.6.0b2/test/test_token.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_tokens.py` & `fabric-credmgr-client-1.6.0b2/test/test_tokens.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_tokens_api.py` & `fabric-credmgr-client-1.6.0b2/test/test_tokens_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_version.py` & `fabric-credmgr-client-1.6.0b2/test/test_version.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_version_api.py` & `fabric-credmgr-client-1.6.0b2/test/test_version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/test/test_version_data.py` & `fabric-credmgr-client-1.6.0b2/test/test_version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.6.0b1/PKG-INFO` & `fabric-credmgr-client-1.6.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric-credmgr-client
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: Fabric Control Framework
 Keywords: Fabric Credential Manager API
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

