# Comparing `tmp/iambic_core-0.9.6.tar.gz` & `tmp/iambic_core-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iambic_core-0.9.6.tar", max compression
+gzip compressed data, was "iambic_core-0.9.8.tar", max compression
```

## Comparing `iambic_core-0.9.6.tar` & `iambic_core-0.9.8.tar`

### file list

```diff
@@ -1,162 +1,162 @@
--rw-r--r--   0        0        0    11356 2023-06-15 22:09:36.885295 iambic_core-0.9.6/LICENSE.md
--rw-r--r--   0        0        0    15653 2023-06-15 22:09:36.885295 iambic_core-0.9.6/README.md
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.921296 iambic_core-0.9.6/iambic/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/config/__init__.py
--rw-r--r--   0        0        0    19724 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/config/dynamic_config.py
--rw-r--r--   0        0        0     3312 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/config/utils.py
--rw-r--r--   0        0        0    78470 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/config/wizard.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/__init__.py
--rw-r--r--   0        0        0     3010 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/aio_utils/__init__.py
--rw-r--r--   0        0        0      290 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/context.py
--rw-r--r--   0        0        0      609 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/exceptions.py
--rw-r--r--   0        0        0    15943 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/git.py
--rw-r--r--   0        0        0      758 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/iambic_enum.py
--rw-r--r--   0        0        0     4845 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/iambic_plugin.py
--rw-r--r--   0        0        0     1946 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/logger.py
--rw-r--r--   0        0        0    25633 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/models.py
--rw-r--r--   0        0        0     1782 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/noq_json.py
--rw-r--r--   0        0        0     5515 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/parser.py
--rw-r--r--   0        0        0    48281 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/template_generation.py
--rw-r--r--   0        0        0    33010 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/utils.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/github/__init__.py
--rw-r--r--   0        0        0      607 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/github/templates/iambic-detect.yml
--rw-r--r--   0        0        0      654 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/github/templates/iambic-enforce.yml
--rw-r--r--   0        0        0      658 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/github/templates/iambic-expire.yml
--rw-r--r--   0        0        0      656 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/github/templates/iambic-import.yml
--rw-r--r--   0        0        0     1042 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/github/utils.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/lambda/__init__.py
--rw-r--r--   0        0        0     4307 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/lambda/app.py
--rw-r--r--   0        0        0    14703 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/main.py
--rw-r--r--   0        0        0      664 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/output/__init__.py
--rw-r--r--   0        0        0     2799 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/output/filters.py
--rw-r--r--   0        0        0      480 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/output/markdown.py
--rw-r--r--   0        0        0    12556 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/output/models.py
--rw-r--r--   0        0        0     4736 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/output/templates/github_summary.jinja2
--rw-r--r--   0        0        0     1086 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/output/templates/text_file_summary.jinja2
--rw-r--r--   0        0        0     1082 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/output/templates/text_screen_summary.jinja2
--rw-r--r--   0        0        0     1040 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/output/text.py
--rw-r--r--   0        0        0     1240 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/README.md
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/__init__.py
--rw-r--r--   0        0        0       62 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
--rw-r--r--   0        0        0     1753 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
--rw-r--r--   0        0        0     2728 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
--rw-r--r--   0        0        0     2268 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml
--rw-r--r--   0        0        0     2712 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
--rw-r--r--   0        0        0     2102 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
--rw-r--r--   0        0        0    18133 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
--rw-r--r--   0        0        0     1721 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/event_bridge/models.py
--rw-r--r--   0        0        0    39712 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/handlers.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
--rw-r--r--   0        0        0    10334 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/group/models.py
--rw-r--r--   0        0        0    18144 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
--rw-r--r--   0        0        0    13681 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/group/utils.py
--rw-r--r--   0        0        0     1254 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/models.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
--rw-r--r--   0        0        0    16084 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/policy/models.py
--rw-r--r--   0        0        0    18077 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
--rw-r--r--   0        0        0    10706 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
--rw-r--r--   0        0        0       35 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
--rw-r--r--   0        0        0    16135 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/role/models.py
--rw-r--r--   0        0        0    22080 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
--rw-r--r--   0        0        0    24602 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/role/utils.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
--rw-r--r--   0        0        0    14064 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/user/models.py
--rw-r--r--   0        0        0    21076 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
--rw-r--r--   0        0        0    22644 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/user/utils.py
--rw-r--r--   0        0        0     5842 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iambic_plugin.py
--rw-r--r--   0        0        0     4968 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
--rw-r--r--   0        0        0    31619 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
--rw-r--r--   0        0        0    20296 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
--rw-r--r--   0        0        0    35636 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
--rw-r--r--   0        0        0    30478 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/models.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/organizations/scp/__init__.py
--rw-r--r--   0        0        0      101 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/organizations/scp/exceptions.py
--rw-r--r--   0        0        0    18860 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/organizations/scp/models.py
--rw-r--r--   0        0        0    11040 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/organizations/scp/template_generation.py
--rw-r--r--   0        0        0    19286 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/organizations/scp/utils.py
--rw-r--r--   0        0        0     1291 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/sqs/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/sqs/util.py
--rw-r--r--   0        0        0     3009 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/template_generation.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/tests/__init__.py
--rw-r--r--   0        0        0    11950 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
--rw-r--r--   0        0        0     3550 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/tests/test_models.py
--rw-r--r--   0        0        0    10209 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/utils.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
--rw-r--r--   0        0        0    14003 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/group/models.py
--rw-r--r--   0        0        0     3820 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
--rw-r--r--   0        0        0    14891 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/group/utils.py
--rw-r--r--   0        0        0     2283 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/handlers.py
--rw-r--r--   0        0        0     2033 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
--rw-r--r--   0        0        0     8515 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/models.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
--rw-r--r--   0        0        0     8798 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/user/models.py
--rw-r--r--   0        0        0     3783 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
--rw-r--r--   0        0        0     7179 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/user/utils.py
--rw-r--r--   0        0        0      258 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/utils.py
--rw-r--r--   0        0        0       82 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/example/README.md
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/example/__init__.py
--rw-r--r--   0        0        0      413 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/example/handlers.py
--rw-r--r--   0        0        0     1128 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/example/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/example/local_database/__init__.py
--rw-r--r--   0        0        0     1514 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/example/local_database/models.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/example/local_file/__init__.py
--rw-r--r--   0        0        0     3366 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/example/local_file/models.py
--rw-r--r--   0        0        0      284 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/github/README.md
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/github/__init__.py
--rw-r--r--   0        0        0    34737 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/github/github.py
--rw-r--r--   0        0        0    12212 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/github/github_app.py
--rw-r--r--   0        0        0     1349 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/github/handlers.py
--rw-r--r--   0        0        0     2015 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/github/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
--rw-r--r--   0        0        0     9806 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/group/models.py
--rw-r--r--   0        0        0     5383 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
--rw-r--r--   0        0        0    14801 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/group/utils.py
--rw-r--r--   0        0        0     2030 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/handlers.py
--rw-r--r--   0        0        0     5437 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
--rw-r--r--   0        0        0     4409 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/models.py
--rw-r--r--   0        0        0     1359 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
--rw-r--r--   0        0        0     7860 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
--rw-r--r--   0        0        0    14373 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
--rw-r--r--   0        0        0    11307 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
--rw-r--r--   0        0        0     3029 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
--rw-r--r--   0        0        0     3177 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/app/__init__.py
--rw-r--r--   0        0        0     9327 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/app/models.py
--rw-r--r--   0        0        0     3176 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/app/template_generation.py
--rw-r--r--   0        0        0    17906 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/app/utils.py
--rw-r--r--   0        0        0       91 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/group/__init__.py
--rw-r--r--   0        0        0    11442 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/group/models.py
--rw-r--r--   0        0        0     3606 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/group/template_generation.py
--rw-r--r--   0        0        0    20065 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/group/utils.py
--rw-r--r--   0        0        0     2502 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/handlers.py
--rw-r--r--   0        0        0     2890 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/iambic_plugin.py
--rw-r--r--   0        0        0     6720 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/models.py
--rw-r--r--   0        0        0     1290 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/user/__init__.py
--rw-r--r--   0        0        0     9587 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/user/models.py
--rw-r--r--   0        0        0     3495 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/user/template_generation.py
--rw-r--r--   0        0        0    13610 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/user/utils.py
--rw-r--r--   0        0        0     1536 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/utils.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/request_handler/__init__.py
--rw-r--r--   0        0        0     1002 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/request_handler/expire_resources.py
--rw-r--r--   0        0        0     4293 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/request_handler/git_apply.py
--rw-r--r--   0        0        0      994 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/request_handler/git_plan.py
--rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/vendor/__init__.py
--rw-r--r--   0        0        0      168 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
--rw-r--r--   0        0        0     1069 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/vendor/lambda_multiprocessing/LICENSE
--rw-r--r--   0        0        0      173 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/vendor/lambda_multiprocessing/__init__.py
--rw-r--r--   0        0        0    12636 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/vendor/lambda_multiprocessing/main.py
--rw-r--r--   0        0        0     2263 2023-06-15 22:09:36.937296 iambic_core-0.9.6/pyproject.toml
--rw-r--r--   0        0        0    17621 1970-01-01 00:00:00.000000 iambic_core-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-20 23:03:50.135947 iambic_core-0.9.8/LICENSE.md
+-rw-r--r--   0        0        0    15653 2023-06-20 23:03:50.135947 iambic_core-0.9.8/README.md
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/config/__init__.py
+-rw-r--r--   0        0        0    19724 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/config/dynamic_config.py
+-rw-r--r--   0        0        0     3312 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/config/utils.py
+-rw-r--r--   0        0        0    78470 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/config/wizard.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/core/__init__.py
+-rw-r--r--   0        0        0     3010 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/core/aio_utils/__init__.py
+-rw-r--r--   0        0        0      290 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/core/context.py
+-rw-r--r--   0        0        0      609 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/core/exceptions.py
+-rw-r--r--   0        0        0    15943 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/core/git.py
+-rw-r--r--   0        0        0      758 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/core/iambic_enum.py
+-rw-r--r--   0        0        0     4845 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/core/iambic_plugin.py
+-rw-r--r--   0        0        0     1946 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/core/logger.py
+-rw-r--r--   0        0        0    25633 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/core/models.py
+-rw-r--r--   0        0        0     1782 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/core/noq_json.py
+-rw-r--r--   0        0        0     5515 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/core/parser.py
+-rw-r--r--   0        0        0    48281 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/core/template_generation.py
+-rw-r--r--   0        0        0    33010 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/core/utils.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/github/__init__.py
+-rw-r--r--   0        0        0      607 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/github/templates/iambic-detect.yml
+-rw-r--r--   0        0        0      654 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/github/templates/iambic-enforce.yml
+-rw-r--r--   0        0        0      658 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/github/templates/iambic-expire.yml
+-rw-r--r--   0        0        0      656 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/github/templates/iambic-import.yml
+-rw-r--r--   0        0        0     1042 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/github/utils.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/lambda/__init__.py
+-rw-r--r--   0        0        0     4307 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/lambda/app.py
+-rw-r--r--   0        0        0    14703 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/main.py
+-rw-r--r--   0        0        0      664 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/output/__init__.py
+-rw-r--r--   0        0        0     2799 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/output/filters.py
+-rw-r--r--   0        0        0      480 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/output/markdown.py
+-rw-r--r--   0        0        0    12556 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/output/models.py
+-rw-r--r--   0        0        0     4736 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/output/templates/github_summary.jinja2
+-rw-r--r--   0        0        0     1086 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/output/templates/text_file_summary.jinja2
+-rw-r--r--   0        0        0     1082 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/output/templates/text_screen_summary.jinja2
+-rw-r--r--   0        0        0     1040 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/output/text.py
+-rw-r--r--   0        0        0     1240 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/plugins/README.md
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/plugins/__init__.py
+-rw-r--r--   0        0        0       62 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/plugins/v0_1_0/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
+-rw-r--r--   0        0        0     1753 2023-06-20 23:03:50.179947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
+-rw-r--r--   0        0        0     2728 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
+-rw-r--r--   0        0        0     2268 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml
+-rw-r--r--   0        0        0     2712 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
+-rw-r--r--   0        0        0     2102 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
+-rw-r--r--   0        0        0    18133 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
+-rw-r--r--   0        0        0     1721 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/event_bridge/models.py
+-rw-r--r--   0        0        0    39712 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/handlers.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
+-rw-r--r--   0        0        0    10334 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/group/models.py
+-rw-r--r--   0        0        0    18144 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
+-rw-r--r--   0        0        0    13681 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/group/utils.py
+-rw-r--r--   0        0        0     1254 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/models.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
+-rw-r--r--   0        0        0    16084 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/policy/models.py
+-rw-r--r--   0        0        0    18077 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
+-rw-r--r--   0        0        0    10706 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
+-rw-r--r--   0        0        0       35 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
+-rw-r--r--   0        0        0    16135 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/role/models.py
+-rw-r--r--   0        0        0    22080 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
+-rw-r--r--   0        0        0    24602 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/role/utils.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
+-rw-r--r--   0        0        0    14064 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/user/models.py
+-rw-r--r--   0        0        0    21076 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
+-rw-r--r--   0        0        0    22644 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/user/utils.py
+-rw-r--r--   0        0        0     5842 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iambic_plugin.py
+-rw-r--r--   0        0        0     4968 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
+-rw-r--r--   0        0        0    31619 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
+-rw-r--r--   0        0        0    20296 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
+-rw-r--r--   0        0        0    35636 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
+-rw-r--r--   0        0        0    30478 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/models.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/organizations/scp/__init__.py
+-rw-r--r--   0        0        0      101 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/organizations/scp/exceptions.py
+-rw-r--r--   0        0        0    18860 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/organizations/scp/models.py
+-rw-r--r--   0        0        0    11040 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/organizations/scp/template_generation.py
+-rw-r--r--   0        0        0    19286 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/organizations/scp/utils.py
+-rw-r--r--   0        0        0     1291 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/sqs/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/sqs/util.py
+-rw-r--r--   0        0        0     3009 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/template_generation.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/tests/__init__.py
+-rw-r--r--   0        0        0    11950 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
+-rw-r--r--   0        0        0     3550 2023-06-20 23:03:50.183947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/tests/test_models.py
+-rw-r--r--   0        0        0    10209 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/utils.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
+-rw-r--r--   0        0        0    14003 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/group/models.py
+-rw-r--r--   0        0        0     3820 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
+-rw-r--r--   0        0        0    14891 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/group/utils.py
+-rw-r--r--   0        0        0     2283 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/handlers.py
+-rw-r--r--   0        0        0     2033 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
+-rw-r--r--   0        0        0     8515 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/models.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
+-rw-r--r--   0        0        0     8798 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/user/models.py
+-rw-r--r--   0        0        0     3783 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
+-rw-r--r--   0        0        0     7179 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/user/utils.py
+-rw-r--r--   0        0        0      258 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/utils.py
+-rw-r--r--   0        0        0       82 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/example/README.md
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/example/__init__.py
+-rw-r--r--   0        0        0      413 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/example/handlers.py
+-rw-r--r--   0        0        0     1128 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/example/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/example/local_database/__init__.py
+-rw-r--r--   0        0        0     1514 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/example/local_database/models.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/example/local_file/__init__.py
+-rw-r--r--   0        0        0     3366 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/example/local_file/models.py
+-rw-r--r--   0        0        0      284 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/github/README.md
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/github/__init__.py
+-rw-r--r--   0        0        0    34737 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/github/github.py
+-rw-r--r--   0        0        0    12482 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/github/github_app.py
+-rw-r--r--   0        0        0     1349 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/github/handlers.py
+-rw-r--r--   0        0        0     2015 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/github/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
+-rw-r--r--   0        0        0     9806 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/group/models.py
+-rw-r--r--   0        0        0     5383 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
+-rw-r--r--   0        0        0    14801 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/group/utils.py
+-rw-r--r--   0        0        0     2030 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/handlers.py
+-rw-r--r--   0        0        0     5437 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
+-rw-r--r--   0        0        0     4409 2023-06-20 23:03:50.187947 iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/models.py
+-rw-r--r--   0        0        0     1359 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
+-rw-r--r--   0        0        0     7860 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
+-rw-r--r--   0        0        0    14373 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
+-rw-r--r--   0        0        0    11307 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
+-rw-r--r--   0        0        0     3029 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
+-rw-r--r--   0        0        0     3177 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/app/__init__.py
+-rw-r--r--   0        0        0     9327 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/app/models.py
+-rw-r--r--   0        0        0     3176 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/app/template_generation.py
+-rw-r--r--   0        0        0    17906 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/app/utils.py
+-rw-r--r--   0        0        0       91 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/group/__init__.py
+-rw-r--r--   0        0        0    11442 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/group/models.py
+-rw-r--r--   0        0        0     3606 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/group/template_generation.py
+-rw-r--r--   0        0        0    20065 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/group/utils.py
+-rw-r--r--   0        0        0     2502 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/handlers.py
+-rw-r--r--   0        0        0     2890 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/iambic_plugin.py
+-rw-r--r--   0        0        0     6720 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/models.py
+-rw-r--r--   0        0        0     1290 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/user/__init__.py
+-rw-r--r--   0        0        0     9587 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/user/models.py
+-rw-r--r--   0        0        0     3495 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/user/template_generation.py
+-rw-r--r--   0        0        0    13610 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/user/utils.py
+-rw-r--r--   0        0        0     1536 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/utils.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/request_handler/__init__.py
+-rw-r--r--   0        0        0     1002 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/request_handler/expire_resources.py
+-rw-r--r--   0        0        0     4293 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/request_handler/git_apply.py
+-rw-r--r--   0        0        0      994 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/request_handler/git_plan.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/vendor/__init__.py
+-rw-r--r--   0        0        0      168 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
+-rw-r--r--   0        0        0     1069 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/vendor/lambda_multiprocessing/LICENSE
+-rw-r--r--   0        0        0      173 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/vendor/lambda_multiprocessing/__init__.py
+-rw-r--r--   0        0        0    12636 2023-06-20 23:03:50.191947 iambic_core-0.9.8/iambic/vendor/lambda_multiprocessing/main.py
+-rw-r--r--   0        0        0     2263 2023-06-20 23:03:50.191947 iambic_core-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0    17621 1970-01-01 00:00:00.000000 iambic_core-0.9.8/PKG-INFO
```

### Comparing `iambic_core-0.9.6/LICENSE.md` & `iambic_core-0.9.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/README.md` & `iambic_core-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/config/dynamic_config.py` & `iambic_core-0.9.8/iambic/config/dynamic_config.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/config/utils.py` & `iambic_core-0.9.8/iambic/config/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/config/wizard.py` & `iambic_core-0.9.8/iambic/config/wizard.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/core/aio_utils/__init__.py` & `iambic_core-0.9.8/iambic/core/aio_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/core/exceptions.py` & `iambic_core-0.9.8/iambic/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/core/git.py` & `iambic_core-0.9.8/iambic/core/git.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/core/iambic_enum.py` & `iambic_core-0.9.8/iambic/core/iambic_enum.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/core/iambic_plugin.py` & `iambic_core-0.9.8/iambic/core/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/core/logger.py` & `iambic_core-0.9.8/iambic/core/logger.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/core/models.py` & `iambic_core-0.9.8/iambic/core/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/core/noq_json.py` & `iambic_core-0.9.8/iambic/core/noq_json.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/core/parser.py` & `iambic_core-0.9.8/iambic/core/parser.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/core/template_generation.py` & `iambic_core-0.9.8/iambic/core/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/core/utils.py` & `iambic_core-0.9.8/iambic/core/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/github/templates/iambic-detect.yml` & `iambic_core-0.9.8/iambic/github/templates/iambic-detect.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/github/templates/iambic-enforce.yml` & `iambic_core-0.9.8/iambic/github/templates/iambic-enforce.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/github/templates/iambic-expire.yml` & `iambic_core-0.9.8/iambic/github/templates/iambic-expire.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/github/templates/iambic-import.yml` & `iambic_core-0.9.8/iambic/github/templates/iambic-import.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/github/utils.py` & `iambic_core-0.9.8/iambic/github/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/lambda/app.py` & `iambic_core-0.9.8/iambic/lambda/app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/main.py` & `iambic_core-0.9.8/iambic/main.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/output/__init__.py` & `iambic_core-0.9.8/iambic/output/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/output/filters.py` & `iambic_core-0.9.8/iambic/output/filters.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/output/models.py` & `iambic_core-0.9.8/iambic/output/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/output/templates/github_summary.jinja2` & `iambic_core-0.9.8/iambic/output/templates/github_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/output/templates/text_file_summary.jinja2` & `iambic_core-0.9.8/iambic/output/templates/text_file_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/output/templates/text_screen_summary.jinja2` & `iambic_core-0.9.8/iambic/output/templates/text_screen_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/output/text.py` & `iambic_core-0.9.8/iambic/output/text.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/README.md` & `iambic_core-0.9.8/iambic/plugins/README.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/event_bridge/models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/event_bridge/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/handlers.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/group/models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/group/utils.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/policy/models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/policy/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/policy/utils.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/policy/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/role/models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/role/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/role/utils.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/role/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/user/models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/user/utils.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iam/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iambic_plugin.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/organizations/scp/models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/organizations/scp/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/organizations/scp/template_generation.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/organizations/scp/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/organizations/scp/utils.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/organizations/scp/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/pyproject.toml` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/template_generation.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/tests/test_models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/utils.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/aws/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/group/models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/group/utils.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/handlers.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/user/models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/user/utils.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/azure_ad/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/example/iambic_plugin.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/example/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/example/local_database/models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/example/local_database/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/example/local_file/models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/example/local_file/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/github/github.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/github/github.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/github/github_app.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/github/github_app.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,20 @@
 # FIXME struct logs is not showing up on lambda cloudwatch logs
 
 # FIXME exception during git-plan is unknown
 # /tmp/.iambic/repos/ already exists. This is unexpected.
 # This is due to lambda reusing the already running container
 
 
+# We typically ignore bot interactions; however, there are scenarios
+# in which we want other installed GitHub App to interact with the
+# integrations, we allow list such situations explicitly.
+ALLOWED_BOT_INTERACTIONS = ["iambic approve", "iambic apply"]
+
+
 def format_github_url(repository_url: str, github_token: str) -> str:
     parse_result = urlparse(repository_url)
     return parse_result._replace(
         netloc="x-access-token:{0}@{1}".format(github_token, parse_result.netloc)
     ).geturl()
 
 
@@ -233,15 +239,15 @@
             "command_lookup": command_lookup,
             "comment_body": comment_body,
         }
         log.error("handle_issue_comment: no op", **log_params)
         return HandleIssueCommentReturnCode.NO_MATCHING_BODY
 
     if comment_user_login.endswith("[bot]"):
-        if command_lookup != "iambic approve":
+        if command_lookup not in ALLOWED_BOT_INTERACTIONS:
             # return early unless it's the approve attempt
             # the approve handler require to walk the full config
             # to determine.
             return HandleIssueCommentReturnCode.UNDEFINED
 
     repo_name = webhook_payload["repository"]["full_name"]
     pull_number = webhook_payload["issue"]["number"]
```

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/github/handlers.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/github/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/github/iambic_plugin.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/github/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/group/models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/group/utils.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/handlers.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/pyproject.toml` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/app/models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/app/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/app/template_generation.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/app/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/app/utils.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/app/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/group/models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/group/template_generation.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/group/utils.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/handlers.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/iambic_plugin.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/pyproject.toml` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/user/models.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/user/template_generation.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/user/utils.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/utils.py` & `iambic_core-0.9.8/iambic/plugins/v0_1_0/okta/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/request_handler/expire_resources.py` & `iambic_core-0.9.8/iambic/request_handler/expire_resources.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/request_handler/git_apply.py` & `iambic_core-0.9.8/iambic/request_handler/git_apply.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/request_handler/git_plan.py` & `iambic_core-0.9.8/iambic/request_handler/git_plan.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/vendor/lambda_multiprocessing/LICENSE` & `iambic_core-0.9.8/iambic/vendor/lambda_multiprocessing/LICENSE`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/iambic/vendor/lambda_multiprocessing/main.py` & `iambic_core-0.9.8/iambic/vendor/lambda_multiprocessing/main.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.6/pyproject.toml` & `iambic_core-0.9.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 [tool.poetry]
 name = "iambic-core"
 packages = [
     { include="iambic", from="." },
 ]
-version = "0.9.6"
+version = "0.9.8"
 license = "Apache-2.0"
 description = "The python package used to generate, parse, and execute noqform yaml templates."
 authors = ["Noq Software <hello@noq.dev>"]
 readme = "README.md"
 exclude = ["build_util/*"]
 include = ["iambic/output/templates/*"]
```

### Comparing `iambic_core-0.9.6/PKG-INFO` & `iambic_core-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iambic-core
-Version: 0.9.6
+Version: 0.9.8
 Summary: The python package used to generate, parse, and execute noqform yaml templates.
 License: Apache-2.0
 Author: Noq Software
 Author-email: hello@noq.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

