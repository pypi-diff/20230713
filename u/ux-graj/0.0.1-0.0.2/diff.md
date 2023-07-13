# Comparing `tmp/ux-graj-0.0.1.tar.gz` & `tmp/ux-graj-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ux-graj-0.0.1.tar", last modified: Thu Jul 13 13:43:56 2023, max compression
+gzip compressed data, was "ux-graj-0.0.2.tar", last modified: Thu Jul 13 15:21:26 2023, max compression
```

## Comparing `ux-graj-0.0.1.tar` & `ux-graj-0.0.2.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 13:43:56.604479 ux-graj-0.0.1/
--rw-rw-rw-   0        0        0     1096 2022-08-25 09:38:05.000000 ux-graj-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       27 2023-07-13 11:48:35.000000 ux-graj-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7585 2023-07-13 13:43:56.602181 ux-graj-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7300 2023-07-13 11:18:02.000000 ux-graj-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 13:43:55.537265 ux-graj-0.0.1/blendedUx/
--rw-rw-rw-   0        0        0      107 2023-07-13 12:14:39.000000 ux-graj-0.0.1/blendedUx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:43:55.598650 ux-graj-0.0.1/blendedUx/blended_flask/
--rw-rw-rw-   0        0        0      160 2023-07-13 13:32:53.000000 ux-graj-0.0.1/blendedUx/blended_flask/__init__.py
--rw-rw-rw-   0        0        0     1208 2023-07-13 13:32:53.000000 ux-graj-0.0.1/blendedUx/blended_flask/app.py
--rw-rw-rw-   0        0        0     3758 2023-07-13 13:32:53.000000 ux-graj-0.0.1/blendedUx/blended_flask/bl_flask_app.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:43:55.673892 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/
--rw-rw-rw-   0        0        0        0 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:43:55.789306 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/backend/
--rw-rw-rw-   0        0        0       24 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/backend/__init__.py
--rw-rw-rw-   0        0        0    44898 2023-07-13 13:32:53.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/backend/backend.py
--rw-rw-rw-   0        0        0     8056 2023-07-13 13:32:53.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/backend/intermediary.py
--rw-rw-rw-   0        0        0     1016 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/backend/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:43:55.836632 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/controller/
--rw-rw-rw-   0        0        0       27 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/controller/__init__.py
--rw-rw-rw-   0        0        0   150877 2023-07-13 13:32:53.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/controller/controller.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:43:55.918753 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/exceptions/
--rw-rw-rw-   0        0        0       25 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/exceptions/__init__.py
--rw-rw-rw-   0        0        0      456 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/exceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:43:55.925991 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/functions/
--rw-rw-rw-   0        0        0       26 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/functions/__init__.py
--rw-rw-rw-   0        0        0      655 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/functions/functions.py
--rw-rw-rw-   0        0        0    24684 2023-07-13 13:32:53.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/initializer.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:43:55.945608 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/network/
--rw-rw-rw-   0        0        0       24 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/network/__init__.py
--rw-rw-rw-   0        0        0    36830 2023-07-13 13:32:53.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/network/network.py
--rw-rw-rw-   0        0        0      102 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/network/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:43:55.977824 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/
--rw-rw-rw-   0        0        0     6577 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/__init__.py
--rw-rw-rw-   0        0        0    21458 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/api_client.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:43:55.993858 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/
--rw-rw-rw-   0        0        0      152 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/__init__.py
--rw-rw-rw-   0        0        0   141226 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/accounts_api.py
--rw-rw-rw-   0        0        0   242470 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/packages_api.py
--rw-rw-rw-   0        0        0     7574 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/configuration.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:43:56.493659 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/
--rw-rw-rw-   0        0        0     5530 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/__init__.py
--rw-rw-rw-   0        0        0     8007 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account.py
--rw-rw-rw-   0        0        0     5983 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invite_pending.py
--rw-rw-rw-   0        0        0     4369 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invites_pending_list.py
--rw-rw-rw-   0        0        0     4168 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/accounts.py
--rw-rw-rw-   0        0        0    10818 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition.py
--rw-rw-rw-   0        0        0     3597 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response.py
--rw-rw-rw-   0        0        0    10364 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response_data.py
--rw-rw-rw-   0        0        0     4303 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/activationchallenge.py
--rw-rw-rw-   0        0        0     7352 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/active_account.py
--rw-rw-rw-   0        0        0     3547 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_account.py
--rw-rw-rw-   0        0        0     3489 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_admin.py
--rw-rw-rw-   0        0        0     4114 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_license.py
--rw-rw-rw-   0        0        0     5149 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_pending.py
--rw-rw-rw-   0        0        0     3543 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_rating.py
--rw-rw-rw-   0        0        0     7377 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/all_license_price.py
--rw-rw-rw-   0        0        0    22811 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/blended_package.py
--rw-rw-rw-   0        0        0     3503 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body.py
--rw-rw-rw-   0        0        0     3727 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body_1.py
--rw-rw-rw-   0        0        0     7110 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages.py
--rw-rw-rw-   0        0        0    12189 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages_error.py
--rw-rw-rw-   0        0        0    18472 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/canonical_version.py
--rw-rw-rw-   0        0        0     3615 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_current_account.py
--rw-rw-rw-   0        0        0     3735 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_privilege.py
--rw-rw-rw-   0        0        0     5504 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_account.py
--rw-rw-rw-   0        0        0     4973 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_canonical.py
--rw-rw-rw-   0        0        0     4853 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_package.py
--rw-rw-rw-   0        0        0     7008 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_version.py
--rw-rw-rw-   0        0        0     5695 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies.py
--rw-rw-rw-   0        0        0     4261 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies_list.py
--rw-rw-rw-   0        0        0    11135 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail.py
--rw-rw-rw-   0        0        0     5279 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail_dependency_of_package.py
--rw-rw-rw-   0        0        0     4151 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/documents.py
--rw-rw-rw-   0        0        0     4125 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error.py
--rw-rw-rw-   0        0        0     5150 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response400.py
--rw-rw-rw-   0        0        0     5198 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response401.py
--rw-rw-rw-   0        0        0     9159 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response409.py
--rw-rw-rw-   0        0        0     9152 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response412.py
--rw-rw-rw-   0        0        0     6037 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response500.py
--rw-rw-rw-   0        0        0     8824 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/failed_dependency_error.py
--rw-rw-rw-   0        0        0     4246 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_account.py
--rw-rw-rw-   0        0        0     3645 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_canonical_version.py
--rw-rw-rw-   0        0        0     7652 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_current_account.py
--rw-rw-rw-   0        0        0     4399 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_dependency_packages.py
--rw-rw-rw-   0        0        0     9790 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_draft.py
--rw-rw-rw-   0        0        0     4256 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_licenses.py
--rw-rw-rw-   0        0        0     4308 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_pending_user.py
--rw-rw-rw-   0        0        0     4239 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_ratings.py
--rw-rw-rw-   0        0        0     4201 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_user.py
--rw-rw-rw-   0        0        0     4286 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_validators.py
--rw-rw-rw-   0        0        0    10246 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_package.py
--rw-rw-rw-   0        0        0     4251 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_packages.py
--rw-rw-rw-   0        0        0     3735 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/inline_response_200.py
--rw-rw-rw-   0        0        0     5230 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/license.py
--rw-rw-rw-   0        0        0     4598 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/like.py
--rw-rw-rw-   0        0        0     5095 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/login.py
--rw-rw-rw-   0        0        0     3651 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/logout.py
--rw-rw-rw-   0        0        0     4919 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/new_draft.py
--rw-rw-rw-   0        0        0     2986 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/operands.py
--rw-rw-rw-   0        0        0     6127 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_detail_data.py
--rw-rw-rw-   0        0        0     5293 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_images.py
--rw-rw-rw-   0        0        0     4181 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/packages.py
--rw-rw-rw-   0        0        0     5560 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_user.py
--rw-rw-rw-   0        0        0     4212 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_users.py
--rw-rw-rw-   0        0        0    10618 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication.py
--rw-rw-rw-   0        0        0    14020 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_error.py
--rw-rw-rw-   0        0        0    17540 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_validation_error.py
--rw-rw-rw-   0        0        0     8618 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version.py
--rw-rw-rw-   0        0        0     8540 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version_error.py
--rw-rw-rw-   0        0        0     4303 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions.py
--rw-rw-rw-   0        0        0     4368 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions_error.py
--rw-rw-rw-   0        0        0     5025 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications.py
--rw-rw-rw-   0        0        0     7275 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications_error.py
--rw-rw-rw-   0        0        0     5218 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/rating.py
--rw-rw-rw-   0        0        0    13040 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reject_acquisition_package.py
--rw-rw-rw-   0        0        0     4502 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/remove_pending.py
--rw-rw-rw-   0        0        0     3659 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_account_verification_link.py
--rw-rw-rw-   0        0        0     5940 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_invite.py
--rw-rw-rw-   0        0        0     3624 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reset_password.py
--rw-rw-rw-   0        0        0    16618 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_result.py
--rw-rw-rw-   0        0        0     5002 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_results.py
--rw-rw-rw-   0        0        0     5133 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/session_data.py
--rw-rw-rw-   0        0        0     4390 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/share_approval_list_error.py
--rw-rw-rw-   0        0        0     9362 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_account.py
--rw-rw-rw-   0        0        0     4385 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_accounts_list.py
--rw-rw-rw-   0        0        0     9033 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_account.py
--rw-rw-rw-   0        0        0     4935 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_draft.py
--rw-rw-rw-   0        0        0     3569 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_license.py
--rw-rw-rw-   0        0        0     6351 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_package.py
--rw-rw-rw-   0        0        0     4537 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_publication.py
--rw-rw-rw-   0        0        0     3780 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_version.py
--rw-rw-rw-   0        0        0     4799 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/upload_media.py
--rw-rw-rw-   0        0        0    12227 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/user.py
--rw-rw-rw-   0        0        0     4121 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/users.py
--rw-rw-rw-   0        0        0     8930 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator.py
--rw-rw-rw-   0        0        0     6347 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_detail.py
--rw-rw-rw-   0        0        0     6614 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_plan.py
--rw-rw-rw-   0        0        0     9282 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_sets_in_badge.py
--rw-rw-rw-   0        0        0    17690 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/version.py
--rw-rw-rw-   0        0        0     4152 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/versions.py
--rw-rw-rw-   0        0        0     9542 2023-04-24 05:51:06.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/rest.py
--rw-rw-rw-   0        0        0     3319 2023-07-13 13:32:53.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/tests.py
--rw-rw-rw-   0        0        0    11975 2023-07-06 12:33:23.000000 ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/transform_image.py
--rw-rw-rw-   0        0        0     4612 2023-07-13 13:32:53.000000 ux-graj-0.0.1/blendedUx/blended_flask/functions.py
--rw-rw-rw-   0        0        0      329 2023-05-03 09:50:10.000000 ux-graj-0.0.1/blendedUx/blended_flask/settings.py
--rw-rw-rw-   0        0        0     3799 2023-07-13 13:32:53.000000 ux-graj-0.0.1/blendedUx/blended_flask/utils.py
--rw-rw-rw-   0        0        0       42 2023-07-13 13:43:56.604479 ux-graj-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1064 2023-07-13 13:42:00.000000 ux-graj-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:43:56.596627 ux-graj-0.0.1/ux_graj.egg-info/
--rw-rw-rw-   0        0        0     7585 2023-07-13 13:43:55.000000 ux-graj-0.0.1/ux_graj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10118 2023-07-13 13:43:55.000000 ux-graj-0.0.1/ux_graj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 13:43:55.000000 ux-graj-0.0.1/ux_graj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      212 2023-07-13 13:43:55.000000 ux-graj-0.0.1/ux_graj.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-13 13:43:55.000000 ux-graj-0.0.1/ux_graj.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 15:21:26.751287 ux-graj-0.0.2/
+-rw-rw-rw-   0        0        0     1096 2022-08-25 09:38:05.000000 ux-graj-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-07-13 11:48:35.000000 ux-graj-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7387 2023-07-13 15:21:26.749283 ux-graj-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7102 2023-07-13 14:53:38.000000 ux-graj-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 15:21:20.244433 ux-graj-0.0.2/blendedUx/
+-rw-rw-rw-   0        0        0      107 2023-07-13 12:14:39.000000 ux-graj-0.0.2/blendedUx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:21:20.354182 ux-graj-0.0.2/blendedUx/blended_flask/
+-rw-rw-rw-   0        0        0      160 2023-07-13 13:32:53.000000 ux-graj-0.0.2/blendedUx/blended_flask/__init__.py
+-rw-rw-rw-   0        0        0     1208 2023-07-13 13:32:53.000000 ux-graj-0.0.2/blendedUx/blended_flask/app.py
+-rw-rw-rw-   0        0        0     3758 2023-07-13 13:32:53.000000 ux-graj-0.0.2/blendedUx/blended_flask/bl_flask_app.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:21:20.382512 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/
+-rw-rw-rw-   0        0        0        0 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:21:20.470294 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/backend/
+-rw-rw-rw-   0        0        0       24 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/backend/__init__.py
+-rw-rw-rw-   0        0        0    44898 2023-07-13 13:32:53.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/backend/backend.py
+-rw-rw-rw-   0        0        0     8056 2023-07-13 13:32:53.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/backend/intermediary.py
+-rw-rw-rw-   0        0        0     1016 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/backend/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:21:20.544455 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/controller/
+-rw-rw-rw-   0        0        0       27 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/controller/__init__.py
+-rw-rw-rw-   0        0        0   150877 2023-07-13 13:32:53.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/controller/controller.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:21:20.550473 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/exceptions/
+-rw-rw-rw-   0        0        0       25 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      456 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/exceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:21:20.554470 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/functions/
+-rw-rw-rw-   0        0        0       26 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/functions/__init__.py
+-rw-rw-rw-   0        0        0      655 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/functions/functions.py
+-rw-rw-rw-   0        0        0    24684 2023-07-13 13:32:53.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/initializer.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:21:20.587324 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/network/
+-rw-rw-rw-   0        0        0       24 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/network/__init__.py
+-rw-rw-rw-   0        0        0    36830 2023-07-13 13:32:53.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/network/network.py
+-rw-rw-rw-   0        0        0      102 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/network/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:21:20.690828 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/
+-rw-rw-rw-   0        0        0     6577 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/__init__.py
+-rw-rw-rw-   0        0        0    21458 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/api_client.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:21:20.824500 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/
+-rw-rw-rw-   0        0        0      152 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/__init__.py
+-rw-rw-rw-   0        0        0   141226 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/accounts_api.py
+-rw-rw-rw-   0        0        0   242470 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/packages_api.py
+-rw-rw-rw-   0        0        0     7574 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/configuration.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:21:26.442674 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/
+-rw-rw-rw-   0        0        0     5530 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/__init__.py
+-rw-rw-rw-   0        0        0     8007 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account.py
+-rw-rw-rw-   0        0        0     5983 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invite_pending.py
+-rw-rw-rw-   0        0        0     4369 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invites_pending_list.py
+-rw-rw-rw-   0        0        0     4168 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/accounts.py
+-rw-rw-rw-   0        0        0    10818 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition.py
+-rw-rw-rw-   0        0        0     3597 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response.py
+-rw-rw-rw-   0        0        0    10364 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response_data.py
+-rw-rw-rw-   0        0        0     4303 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/activationchallenge.py
+-rw-rw-rw-   0        0        0     7352 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/active_account.py
+-rw-rw-rw-   0        0        0     3547 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_account.py
+-rw-rw-rw-   0        0        0     3489 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_admin.py
+-rw-rw-rw-   0        0        0     4114 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_license.py
+-rw-rw-rw-   0        0        0     5149 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_pending.py
+-rw-rw-rw-   0        0        0     3543 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_rating.py
+-rw-rw-rw-   0        0        0     7377 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/all_license_price.py
+-rw-rw-rw-   0        0        0    22811 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/blended_package.py
+-rw-rw-rw-   0        0        0     3503 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body.py
+-rw-rw-rw-   0        0        0     3727 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body_1.py
+-rw-rw-rw-   0        0        0     7110 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages.py
+-rw-rw-rw-   0        0        0    12189 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages_error.py
+-rw-rw-rw-   0        0        0    18472 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/canonical_version.py
+-rw-rw-rw-   0        0        0     3615 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_current_account.py
+-rw-rw-rw-   0        0        0     3735 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_privilege.py
+-rw-rw-rw-   0        0        0     5504 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_account.py
+-rw-rw-rw-   0        0        0     4973 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_canonical.py
+-rw-rw-rw-   0        0        0     4853 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_package.py
+-rw-rw-rw-   0        0        0     7008 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_version.py
+-rw-rw-rw-   0        0        0     5695 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies.py
+-rw-rw-rw-   0        0        0     4261 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies_list.py
+-rw-rw-rw-   0        0        0    11135 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail.py
+-rw-rw-rw-   0        0        0     5279 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail_dependency_of_package.py
+-rw-rw-rw-   0        0        0     4151 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/documents.py
+-rw-rw-rw-   0        0        0     4125 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error.py
+-rw-rw-rw-   0        0        0     5150 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response400.py
+-rw-rw-rw-   0        0        0     5198 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response401.py
+-rw-rw-rw-   0        0        0     9159 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response409.py
+-rw-rw-rw-   0        0        0     9152 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response412.py
+-rw-rw-rw-   0        0        0     6037 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response500.py
+-rw-rw-rw-   0        0        0     8824 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/failed_dependency_error.py
+-rw-rw-rw-   0        0        0     4246 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_account.py
+-rw-rw-rw-   0        0        0     3645 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_canonical_version.py
+-rw-rw-rw-   0        0        0     7652 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_current_account.py
+-rw-rw-rw-   0        0        0     4399 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_dependency_packages.py
+-rw-rw-rw-   0        0        0     9790 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_draft.py
+-rw-rw-rw-   0        0        0     4256 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_licenses.py
+-rw-rw-rw-   0        0        0     4308 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_pending_user.py
+-rw-rw-rw-   0        0        0     4239 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_ratings.py
+-rw-rw-rw-   0        0        0     4201 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_user.py
+-rw-rw-rw-   0        0        0     4286 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_validators.py
+-rw-rw-rw-   0        0        0    10246 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_package.py
+-rw-rw-rw-   0        0        0     4251 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_packages.py
+-rw-rw-rw-   0        0        0     3735 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/inline_response_200.py
+-rw-rw-rw-   0        0        0     5230 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/license.py
+-rw-rw-rw-   0        0        0     4598 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/like.py
+-rw-rw-rw-   0        0        0     5095 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/login.py
+-rw-rw-rw-   0        0        0     3651 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/logout.py
+-rw-rw-rw-   0        0        0     4919 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/new_draft.py
+-rw-rw-rw-   0        0        0     2986 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/operands.py
+-rw-rw-rw-   0        0        0     6127 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_detail_data.py
+-rw-rw-rw-   0        0        0     5293 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_images.py
+-rw-rw-rw-   0        0        0     4181 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/packages.py
+-rw-rw-rw-   0        0        0     5560 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_user.py
+-rw-rw-rw-   0        0        0     4212 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_users.py
+-rw-rw-rw-   0        0        0    10618 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication.py
+-rw-rw-rw-   0        0        0    14020 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_error.py
+-rw-rw-rw-   0        0        0    17540 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_validation_error.py
+-rw-rw-rw-   0        0        0     8618 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version.py
+-rw-rw-rw-   0        0        0     8540 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version_error.py
+-rw-rw-rw-   0        0        0     4303 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions.py
+-rw-rw-rw-   0        0        0     4368 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions_error.py
+-rw-rw-rw-   0        0        0     5025 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications.py
+-rw-rw-rw-   0        0        0     7275 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications_error.py
+-rw-rw-rw-   0        0        0     5218 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/rating.py
+-rw-rw-rw-   0        0        0    13040 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reject_acquisition_package.py
+-rw-rw-rw-   0        0        0     4502 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/remove_pending.py
+-rw-rw-rw-   0        0        0     3659 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_account_verification_link.py
+-rw-rw-rw-   0        0        0     5940 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_invite.py
+-rw-rw-rw-   0        0        0     3624 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reset_password.py
+-rw-rw-rw-   0        0        0    16618 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_result.py
+-rw-rw-rw-   0        0        0     5002 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_results.py
+-rw-rw-rw-   0        0        0     5133 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/session_data.py
+-rw-rw-rw-   0        0        0     4390 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/share_approval_list_error.py
+-rw-rw-rw-   0        0        0     9362 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_account.py
+-rw-rw-rw-   0        0        0     4385 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_accounts_list.py
+-rw-rw-rw-   0        0        0     9033 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_account.py
+-rw-rw-rw-   0        0        0     4935 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_draft.py
+-rw-rw-rw-   0        0        0     3569 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_license.py
+-rw-rw-rw-   0        0        0     6351 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_package.py
+-rw-rw-rw-   0        0        0     4537 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_publication.py
+-rw-rw-rw-   0        0        0     3780 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_version.py
+-rw-rw-rw-   0        0        0     4799 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/upload_media.py
+-rw-rw-rw-   0        0        0    12227 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/user.py
+-rw-rw-rw-   0        0        0     4121 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/users.py
+-rw-rw-rw-   0        0        0     8930 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator.py
+-rw-rw-rw-   0        0        0     6347 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_detail.py
+-rw-rw-rw-   0        0        0     6614 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_plan.py
+-rw-rw-rw-   0        0        0     9282 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_sets_in_badge.py
+-rw-rw-rw-   0        0        0    17690 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/version.py
+-rw-rw-rw-   0        0        0     4152 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/versions.py
+-rw-rw-rw-   0        0        0     9542 2023-04-24 05:51:06.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/rest.py
+-rw-rw-rw-   0        0        0     3319 2023-07-13 13:32:53.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/tests.py
+-rw-rw-rw-   0        0        0    11975 2023-07-06 12:33:23.000000 ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/transform_image.py
+-rw-rw-rw-   0        0        0     4612 2023-07-13 13:32:53.000000 ux-graj-0.0.2/blendedUx/blended_flask/functions.py
+-rw-rw-rw-   0        0        0      329 2023-05-03 09:50:10.000000 ux-graj-0.0.2/blendedUx/blended_flask/settings.py
+-rw-rw-rw-   0        0        0     3799 2023-07-13 13:32:53.000000 ux-graj-0.0.2/blendedUx/blended_flask/utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-13 15:21:26.752283 ux-graj-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2023-07-13 15:21:10.000000 ux-graj-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:21:26.744723 ux-graj-0.0.2/ux_graj.egg-info/
+-rw-rw-rw-   0        0        0     7387 2023-07-13 15:21:19.000000 ux-graj-0.0.2/ux_graj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10118 2023-07-13 15:21:19.000000 ux-graj-0.0.2/ux_graj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 15:21:19.000000 ux-graj-0.0.2/ux_graj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      212 2023-07-13 15:21:19.000000 ux-graj-0.0.2/ux_graj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-13 15:21:19.000000 ux-graj-0.0.2/ux_graj.egg-info/top_level.txt
```

### Comparing `ux-graj-0.0.1/LICENSE` & `ux-graj-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/PKG-INFO` & `ux-graj-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 Metadata-Version: 2.1
 Name: ux-graj
-Version: 0.0.1
+Version: 0.0.2
 Summary: A cross-platform design theme framework.
 Home-page: UNKNOWN
 Author: Gaurav Raj
 Author-email: <graj@cognam.com>
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Blended-Flask
+# Blended-Ux
 ---
-### Install Blended-Flask
+### Install Blended-Ux
 
-We recommend to make a python virtual environment to install Blended-Flask, with python version 3.11.3.
+We recommend to make a python virtual environment to install Blended-Ux, with python version 3.11.3.
 
 ```python
 python -m venv venv
 cd venv
 .\Scripts\activate
-pip install blended_flask
+pip install blendedux
 ```
 
 # Quickstart
 Eager to get started? Follow installation doc to install.
-Two ways to use Blended-Flask…………
+Two ways to use Blended-Ux…………
 
 - ####  With Blended-Theme
 
-We recommend using Python version 3.11.3 for Blended-Flask. Blended-Flask supports Python 3.11.3. Additionally, we recommend using a virtual environment to isolate your project dependencies from other projects and the system.
+We recommend using Python version 3.11.3 for Blended-Ux. Blended-Ux supports Python 3.11.3. Additionally, we recommend using a virtual environment to isolate your project dependencies from other projects and the system.
 
 ```python
-python -m venv Blended-Flask
-cd Blended-Flask
+python -m venv ux_env
+cd ux_env
 Scripts\activate
 ```
 You can install this package as usual with pip:
 ```python
-pip install blended_flask
+pip install blendedux
 ```
 **Create a file name app.py in the root directory and paste below line of code.**
 ```python
 
 from flask import Flask
-from blended_flask.bl_flask_app import Bl_Flask
-from blended_flask import *
+from blendedUx import *
+from blendedUx.blended_flask.bl_flask_app import Bl_Flask
+
 PACKAGE_DIR = "themes-directory"
 
 app = Bl_Flask(__name__, package_dir= PACKAGE_DIR)
 
 user_name = 'user_name'
 theme_name = 'theme_name'
 password = ''
@@ -89,15 +90,15 @@
 ```
 PACKAGE_DIR = "C:/Users/themes"
 user_name = 'blended'
 theme_name = 'base_theme'
 password = ''
 ```
 
-⇒           How to include blended theme in your Blended_Flask application……………..
+⇒           How to include blended theme in your Blended-Ux application……………..
 
 Create a templates directory in the root and create a home.html inside the templates directory and paste below line of code in the home.html and save.
 
 ```html
 {% extends theme.template.home|template %}
 	{% block title %}
 		<title>My Blended Site </title>
@@ -177,27 +178,27 @@
 
 
 
 - ####      Without Blended-Theme
 
 ##### Project Setup
 
-We recommend using Python version 3.11.3 for Blended-Flask. Blended-Flask supports Python 3.11.3. Additionally, we recommend using a virtual environment to isolate your project dependencies from other projects and the system.
+We recommend using Python version 3.11.3 for Blended-Ux. Blended-Ux supports Python 3.11.3. Additionally, we recommend using a virtual environment to isolate your project dependencies from other projects and the system.
 
 ```python
-python -m venv Blended-Flask
-cd Blended-Flask
+python -m venv ux_env
+cd ux_env
 Scripts\activate
 ```
 You can install this package as usual with pip:
 ```python
-pip install blended_flask
+pip install blendedux
 ```
 
-**A minimal application for Blended-Flask**
+**A minimal application for Blended-Ux**
 Note: You can define and access static files as done in Flask.
 
 ```python
 myproject/
 			templates/
 						greeting.html
 			static/
@@ -207,15 +208,15 @@
 			app.py
 ```
 Paste the below Code Snippets in `app.py`
 ```python
 import os
 from flask import Flask, flash
 from blendedUx import *
-from blended_flask.bl_flask_app import Bl_Flask
+from blendedUx.blended_flask.bl_flask_app import Bl_Flask
 
 app = Bl_Flask(__name__)
 
 @app.route('/')
 def home(**kwargs):
     """
     """
@@ -247,11 +248,10 @@
 To run the app server
 
 ```python
 cd myproject
 python app.py
 ```
 
-**Note**: As Flask uses Jinja under the hood to rendering the templates, similarly Blended-Flask uses Blended-Jinja for rendering the templates.
```

### Comparing `ux-graj-0.0.1/README.md` & `ux-graj-0.0.2/ux_graj.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,56 @@
-# Blended-Flask
+Metadata-Version: 2.1
+Name: ux-graj
+Version: 0.0.2
+Summary: A cross-platform design theme framework.
+Home-page: UNKNOWN
+Author: Gaurav Raj
+Author-email: <graj@cognam.com>
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Blended-Ux
 ---
-### Install Blended-Flask
+### Install Blended-Ux
 
-We recommend to make a python virtual environment to install Blended-Flask, with python version 3.11.3.
+We recommend to make a python virtual environment to install Blended-Ux, with python version 3.11.3.
 
 ```python
 python -m venv venv
 cd venv
 .\Scripts\activate
-pip install blended_flask
+pip install blendedux
 ```
 
 # Quickstart
 Eager to get started? Follow installation doc to install.
-Two ways to use Blended-Flask…………
+Two ways to use Blended-Ux…………
 
 - ####  With Blended-Theme
 
-We recommend using Python version 3.11.3 for Blended-Flask. Blended-Flask supports Python 3.11.3. Additionally, we recommend using a virtual environment to isolate your project dependencies from other projects and the system.
+We recommend using Python version 3.11.3 for Blended-Ux. Blended-Ux supports Python 3.11.3. Additionally, we recommend using a virtual environment to isolate your project dependencies from other projects and the system.
 
 ```python
-python -m venv Blended-Flask
-cd Blended-Flask
+python -m venv ux_env
+cd ux_env
 Scripts\activate
 ```
 You can install this package as usual with pip:
 ```python
-pip install blended_flask
+pip install blendedux
 ```
 **Create a file name app.py in the root directory and paste below line of code.**
 ```python
 
 from flask import Flask
-from blended_flask.bl_flask_app import Bl_Flask
-from blended_flask import *
+from blendedUx import *
+from blendedUx.blended_flask.bl_flask_app import Bl_Flask
+
 PACKAGE_DIR = "themes-directory"
 
 app = Bl_Flask(__name__, package_dir= PACKAGE_DIR)
 
 user_name = 'user_name'
 theme_name = 'theme_name'
 password = ''
@@ -77,15 +90,15 @@
 ```
 PACKAGE_DIR = "C:/Users/themes"
 user_name = 'blended'
 theme_name = 'base_theme'
 password = ''
 ```
 
-⇒           How to include blended theme in your Blended_Flask application……………..
+⇒           How to include blended theme in your Blended-Ux application……………..
 
 Create a templates directory in the root and create a home.html inside the templates directory and paste below line of code in the home.html and save.
 
 ```html
 {% extends theme.template.home|template %}
 	{% block title %}
 		<title>My Blended Site </title>
@@ -165,27 +178,27 @@
 
 
 
 - ####      Without Blended-Theme
 
 ##### Project Setup
 
-We recommend using Python version 3.11.3 for Blended-Flask. Blended-Flask supports Python 3.11.3. Additionally, we recommend using a virtual environment to isolate your project dependencies from other projects and the system.
+We recommend using Python version 3.11.3 for Blended-Ux. Blended-Ux supports Python 3.11.3. Additionally, we recommend using a virtual environment to isolate your project dependencies from other projects and the system.
 
 ```python
-python -m venv Blended-Flask
-cd Blended-Flask
+python -m venv ux_env
+cd ux_env
 Scripts\activate
 ```
 You can install this package as usual with pip:
 ```python
-pip install blended_flask
+pip install blendedux
 ```
 
-**A minimal application for Blended-Flask**
+**A minimal application for Blended-Ux**
 Note: You can define and access static files as done in Flask.
 
 ```python
 myproject/
 			templates/
 						greeting.html
 			static/
@@ -195,15 +208,15 @@
 			app.py
 ```
 Paste the below Code Snippets in `app.py`
 ```python
 import os
 from flask import Flask, flash
 from blendedUx import *
-from blended_flask.bl_flask_app import Bl_Flask
+from blendedUx.blended_flask.bl_flask_app import Bl_Flask
 
 app = Bl_Flask(__name__)
 
 @app.route('/')
 def home(**kwargs):
     """
     """
@@ -235,9 +248,10 @@
 To run the app server
 
 ```python
 cd myproject
 python app.py
 ```
 
-**Note**: As Flask uses Jinja under the hood to rendering the templates, similarly Blended-Flask uses Blended-Jinja for rendering the templates.
+
+
```

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/app.py` & `ux-graj-0.0.2/blendedUx/blended_flask/app.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/bl_flask_app.py` & `ux-graj-0.0.2/blendedUx/blended_flask/bl_flask_app.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/backend/backend.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/backend/backend.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/backend/intermediary.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/backend/intermediary.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/backend/settings.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/backend/settings.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/controller/controller.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/controller/controller.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/functions/functions.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/functions/functions.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/initializer.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/initializer.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/network/network.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/network/network.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/__init__.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/api_client.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/accounts_api.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/accounts_api.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/packages_api.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/packages_api.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/configuration.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/__init__.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invite_pending.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invite_pending.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invites_pending_list.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invites_pending_list.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/accounts.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/accounts.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response_data.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response_data.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/activationchallenge.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/activationchallenge.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/active_account.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/active_account.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_account.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_account.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_admin.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_admin.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_license.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_license.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_pending.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_pending.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_rating.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_rating.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/all_license_price.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/all_license_price.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/blended_package.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/blended_package.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body_1.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body_1.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages_error.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages_error.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/canonical_version.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/canonical_version.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_current_account.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_current_account.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_privilege.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_privilege.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_account.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_account.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_canonical.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_canonical.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_package.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_package.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_version.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_version.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies_list.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies_list.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail_dependency_of_package.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail_dependency_of_package.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/documents.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/documents.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response400.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response400.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response401.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response401.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response409.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response409.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response412.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response412.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response500.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response500.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/failed_dependency_error.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/failed_dependency_error.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_account.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_account.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_canonical_version.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_canonical_version.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_current_account.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_current_account.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_dependency_packages.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_dependency_packages.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_draft.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_draft.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_licenses.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_licenses.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_pending_user.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_pending_user.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_ratings.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_ratings.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_user.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_user.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_validators.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_validators.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_package.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_package.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_packages.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_packages.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/inline_response_200.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/inline_response_200.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/license.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/license.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/like.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/like.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/login.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/login.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/logout.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/logout.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/new_draft.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/new_draft.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/operands.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/operands.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_detail_data.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_detail_data.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_images.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_images.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/packages.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/packages.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_user.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_user.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_users.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_users.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_error.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_error.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_validation_error.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_validation_error.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version_error.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version_error.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions_error.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions_error.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications_error.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications_error.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/rating.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/rating.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reject_acquisition_package.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reject_acquisition_package.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/remove_pending.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/remove_pending.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_account_verification_link.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_account_verification_link.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_invite.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_invite.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reset_password.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reset_password.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_result.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_result.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_results.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_results.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/session_data.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/session_data.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/share_approval_list_error.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/share_approval_list_error.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_account.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_account.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_accounts_list.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_accounts_list.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_account.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_account.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_draft.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_draft.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_license.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_license.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_package.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_package.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_publication.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_publication.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_version.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_version.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/upload_media.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/upload_media.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/user.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/user.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/users.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/users.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_detail.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_detail.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_plan.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_plan.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_sets_in_badge.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_sets_in_badge.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/version.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/version.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/models/versions.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/versions.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/swagger_client/rest.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/tests.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/tests.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/blended_hostlib/transform_image.py` & `ux-graj-0.0.2/blendedUx/blended_flask/blended_hostlib/transform_image.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/functions.py` & `ux-graj-0.0.2/blendedUx/blended_flask/functions.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/blendedUx/blended_flask/utils.py` & `ux-graj-0.0.2/blendedUx/blended_flask/utils.py`

 * *Files identical despite different names*

### Comparing `ux-graj-0.0.1/setup.py` & `ux-graj-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text(encoding="utf-8")
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A cross-platform design theme framework.'
 
 
 
 # Setting up
 setup(
     name="ux-graj",
```

### Comparing `ux-graj-0.0.1/ux_graj.egg-info/PKG-INFO` & `ux-graj-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,44 @@
-Metadata-Version: 2.1
-Name: ux-graj
-Version: 0.0.1
-Summary: A cross-platform design theme framework.
-Home-page: UNKNOWN
-Author: Gaurav Raj
-Author-email: <graj@cognam.com>
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Blended-Flask
+# Blended-Ux
 ---
-### Install Blended-Flask
+### Install Blended-Ux
 
-We recommend to make a python virtual environment to install Blended-Flask, with python version 3.11.3.
+We recommend to make a python virtual environment to install Blended-Ux, with python version 3.11.3.
 
 ```python
 python -m venv venv
 cd venv
 .\Scripts\activate
-pip install blended_flask
+pip install blendedux
 ```
 
 # Quickstart
 Eager to get started? Follow installation doc to install.
-Two ways to use Blended-Flask…………
+Two ways to use Blended-Ux…………
 
 - ####  With Blended-Theme
 
-We recommend using Python version 3.11.3 for Blended-Flask. Blended-Flask supports Python 3.11.3. Additionally, we recommend using a virtual environment to isolate your project dependencies from other projects and the system.
+We recommend using Python version 3.11.3 for Blended-Ux. Blended-Ux supports Python 3.11.3. Additionally, we recommend using a virtual environment to isolate your project dependencies from other projects and the system.
 
 ```python
-python -m venv Blended-Flask
-cd Blended-Flask
+python -m venv ux_env
+cd ux_env
 Scripts\activate
 ```
 You can install this package as usual with pip:
 ```python
-pip install blended_flask
+pip install blendedux
 ```
 **Create a file name app.py in the root directory and paste below line of code.**
 ```python
 
 from flask import Flask
-from blended_flask.bl_flask_app import Bl_Flask
-from blended_flask import *
+from blendedUx import *
+from blendedUx.blended_flask.bl_flask_app import Bl_Flask
+
 PACKAGE_DIR = "themes-directory"
 
 app = Bl_Flask(__name__, package_dir= PACKAGE_DIR)
 
 user_name = 'user_name'
 theme_name = 'theme_name'
 password = ''
@@ -89,15 +78,15 @@
 ```
 PACKAGE_DIR = "C:/Users/themes"
 user_name = 'blended'
 theme_name = 'base_theme'
 password = ''
 ```
 
-⇒           How to include blended theme in your Blended_Flask application……………..
+⇒           How to include blended theme in your Blended-Ux application……………..
 
 Create a templates directory in the root and create a home.html inside the templates directory and paste below line of code in the home.html and save.
 
 ```html
 {% extends theme.template.home|template %}
 	{% block title %}
 		<title>My Blended Site </title>
@@ -177,27 +166,27 @@
 
 
 
 - ####      Without Blended-Theme
 
 ##### Project Setup
 
-We recommend using Python version 3.11.3 for Blended-Flask. Blended-Flask supports Python 3.11.3. Additionally, we recommend using a virtual environment to isolate your project dependencies from other projects and the system.
+We recommend using Python version 3.11.3 for Blended-Ux. Blended-Ux supports Python 3.11.3. Additionally, we recommend using a virtual environment to isolate your project dependencies from other projects and the system.
 
 ```python
-python -m venv Blended-Flask
-cd Blended-Flask
+python -m venv ux_env
+cd ux_env
 Scripts\activate
 ```
 You can install this package as usual with pip:
 ```python
-pip install blended_flask
+pip install blendedux
 ```
 
-**A minimal application for Blended-Flask**
+**A minimal application for Blended-Ux**
 Note: You can define and access static files as done in Flask.
 
 ```python
 myproject/
 			templates/
 						greeting.html
 			static/
@@ -207,15 +196,15 @@
 			app.py
 ```
 Paste the below Code Snippets in `app.py`
 ```python
 import os
 from flask import Flask, flash
 from blendedUx import *
-from blended_flask.bl_flask_app import Bl_Flask
+from blendedUx.blended_flask.bl_flask_app import Bl_Flask
 
 app = Bl_Flask(__name__)
 
 @app.route('/')
 def home(**kwargs):
     """
     """
@@ -247,11 +236,8 @@
 To run the app server
 
 ```python
 cd myproject
 python app.py
 ```
 
-**Note**: As Flask uses Jinja under the hood to rendering the templates, similarly Blended-Flask uses Blended-Jinja for rendering the templates.
-
-
```

### Comparing `ux-graj-0.0.1/ux_graj.egg-info/SOURCES.txt` & `ux-graj-0.0.2/ux_graj.egg-info/SOURCES.txt`

 * *Files identical despite different names*

