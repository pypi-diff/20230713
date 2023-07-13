# Comparing `tmp/gitlabform-3.6.0.tar.gz` & `tmp/gitlabform-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlabform-3.6.0.tar", last modified: Fri May 19 08:44:55 2023, max compression
+gzip compressed data, was "gitlabform-3.6.1.tar", last modified: Thu Jul 13 08:00:12 2023, max compression
```

## Comparing `gitlabform-3.6.0.tar` & `gitlabform-3.6.1.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.935792 gitlabform-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-19 08:44:49.000000 gitlabform-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-19 08:44:55.935792 gitlabform-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-19 08:44:49.000000 gitlabform-3.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.927792 gitlabform-3.6.0/gitlabform/
--rw-r--r--   0 runner    (1001) docker     (123)    23870 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.927792 gitlabform-3.6.0/gitlabform/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/configuration/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/configuration/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/configuration/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/configuration/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/configuration/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.927792 gitlabform-3.6.0/gitlabform/gitlab/
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/commits.py
--rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/group_badges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/group_ldap_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/group_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/merge_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/project_badges.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/project_deploy_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/project_merge_requests_approvals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/project_protected_environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/resource_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/gitlab/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.927792 gitlabform-3.6.0/gitlabform/lists/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/lists/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/lists/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/lists/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.927792 gitlabform-3.6.0/gitlabform/processors/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/abstract_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/defining_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.927792 gitlabform-3.6.0/gitlabform/processors/group/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/group/group_badges_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/group/group_ldap_links_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/group/group_members_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/group/group_settings_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/group/group_variables_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/multiple_entities_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.931792 gitlabform-3.6.0/gitlabform/processors/project/
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/badges_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/branches_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/deploy_keys_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/files_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/hooks_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/integrations_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/members_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/merge_requests_approval_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/merge_requests_approvals.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/project_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/project_push_rules_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/project_settings_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/resource_groups_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/schedules_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/tags_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/project/variables_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.931792 gitlabform-3.6.0/gitlabform/processors/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/shared/protected_environments_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/single_entity_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.931792 gitlabform-3.6.0/gitlabform/processors/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14003 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/util/branch_protector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/processors/util/difference_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-19 08:44:49.000000 gitlabform-3.6.0/gitlabform/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.927792 gitlabform-3.6.0/gitlabform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-19 08:44:55.000000 gitlabform-3.6.0/gitlabform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-05-19 08:44:55.000000 gitlabform-3.6.0/gitlabform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 08:44:55.000000 gitlabform-3.6.0/gitlabform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-19 08:44:55.000000 gitlabform-3.6.0/gitlabform.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-19 08:44:55.000000 gitlabform-3.6.0/gitlabform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 08:44:55.000000 gitlabform-3.6.0/gitlabform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 08:44:55.935792 gitlabform-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-19 08:44:49.000000 gitlabform-3.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.931792 gitlabform-3.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.931792 gitlabform-3.6.0/tests/acceptance/
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.931792 gitlabform-3.6.0/tests/acceptance/standard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2738 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_archive_project.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5971 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_badges.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3293 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_branches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8047 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_deploy_keys.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_deploy_keys_all_projects.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10859 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1434 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_files_all.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1951 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_files_protected.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3059 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_files_templates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4136 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_group_badges.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_group_members_groups.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9639 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_group_members_users.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_group_settings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5622 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_group_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_inheritance_break.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10353 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_integrations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2324 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_members.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2071 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_members_add_group.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2231 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_members_enforce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_project_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_resource_groups.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1664 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_running.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7264 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_schedules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5045 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_tags.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_token_from_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5559 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/acceptance/standard/test_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.935792 gitlabform-3.6.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.935792 gitlabform-3.6.0/tests/unit/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/configuration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3042 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/configuration/test_case_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/configuration/test_inheritance_break_projects_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/configuration/test_inheritance_break_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/configuration/test_inheritance_break_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/configuration/test_projects_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/configuration/test_skip_groups_skip_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/configuration/test_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/configuration/test_yaml_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:55.935792 gitlabform-3.6.0/tests/unit/processors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/processors/test_abstract_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/processors/test_branch_protector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/processors/test_difference_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/test_access_levels.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-19 08:44:49.000000 gitlabform-3.6.0/tests/unit/test_non_empty_configs_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.483162 gitlabform-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-13 08:00:09.000000 gitlabform-3.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-13 08:00:12.483162 gitlabform-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-13 08:00:09.000000 gitlabform-3.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.467162 gitlabform-3.6.1/gitlabform/
+-rw-r--r--   0 runner    (1001) docker     (123)    23870 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.467162 gitlabform-3.6.1/gitlabform/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/configuration/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/configuration/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/configuration/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/configuration/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/configuration/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.471162 gitlabform-3.6.1/gitlabform/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/commits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/group_badges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/group_ldap_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/group_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/merge_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/project_badges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/project_deploy_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/project_merge_requests_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/project_protected_environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/resource_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.471162 gitlabform-3.6.1/gitlabform/lists/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/lists/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/lists/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/lists/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.471162 gitlabform-3.6.1/gitlabform/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/abstract_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/defining_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.475162 gitlabform-3.6.1/gitlabform/processors/group/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/group/group_badges_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/group/group_ldap_links_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/group/group_members_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/group/group_settings_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/group/group_variables_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/multiple_entities_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.475162 gitlabform-3.6.1/gitlabform/processors/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/badges_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/branches_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/deploy_keys_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/files_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/hooks_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/integrations_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/members_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/merge_requests_approval_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/merge_requests_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/project_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/project_push_rules_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/project_settings_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/resource_groups_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/schedules_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/tags_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/variables_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.479162 gitlabform-3.6.1/gitlabform/processors/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/shared/protected_environments_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/single_entity_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.479162 gitlabform-3.6.1/gitlabform/processors/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14003 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/util/branch_protector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/util/difference_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.467162 gitlabform-3.6.1/gitlabform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-13 08:00:12.000000 gitlabform-3.6.1/gitlabform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-07-13 08:00:12.000000 gitlabform-3.6.1/gitlabform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:00:12.000000 gitlabform-3.6.1/gitlabform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-13 08:00:12.000000 gitlabform-3.6.1/gitlabform.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-13 08:00:12.000000 gitlabform-3.6.1/gitlabform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 08:00:12.000000 gitlabform-3.6.1/gitlabform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-13 08:00:12.487162 gitlabform-3.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-13 08:00:09.000000 gitlabform-3.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.479162 gitlabform-3.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.479162 gitlabform-3.6.1/tests/acceptance/
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.483162 gitlabform-3.6.1/tests/acceptance/standard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2738 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_archive_project.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5971 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_badges.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3293 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_branches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8047 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_deploy_keys.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_deploy_keys_all_projects.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10859 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1434 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_files_all.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1951 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_files_protected.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3059 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_files_templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4136 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_group_badges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_group_members_groups.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9639 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_group_members_users.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_group_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5622 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_group_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_inheritance_break.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10353 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_integrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2324 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_members.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2071 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_members_add_group.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2231 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_members_enforce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_project_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_resource_groups.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1664 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_running.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7264 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_schedules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5045 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_tags.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_token_from_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5559 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.483162 gitlabform-3.6.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.483162 gitlabform-3.6.1/tests/unit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/configuration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3042 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/configuration/test_case_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/configuration/test_inheritance_break_projects_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/configuration/test_inheritance_break_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/configuration/test_inheritance_break_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/configuration/test_projects_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/configuration/test_skip_groups_skip_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/configuration/test_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/configuration/test_yaml_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.483162 gitlabform-3.6.1/tests/unit/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/processors/test_abstract_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/processors/test_branch_protector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/processors/test_difference_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/test_access_levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/test_non_empty_configs_provider.py
```

### Comparing `gitlabform-3.6.0/LICENSE` & `gitlabform-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/PKG-INFO` & `gitlabform-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabform
-Version: 3.6.0
+Version: 3.6.1
 Summary: 🏗 Specialized configuration as a code tool for GitLab projects, groups and more using hierarchical configuration written in YAML
 Home-page: https://gitlabform.github.io/gitlabform
 Author: Greg Dubicki and Contributors
 Keywords: cli,yaml,gitlab,configuration-as-code
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gitlabform Version: 3.6.0 Summary: ð Specialized
+Metadata-Version: 2.1 Name: gitlabform Version: 3.6.1 Summary: ð Specialized
 configuration as a code tool for GitLab projects, groups and more using
 hierarchical configuration written in YAML Home-page: https://
 gitlabform.github.io/gitlabform Author: Greg Dubicki and Contributors Keywords:
 cli,yaml,gitlab,configuration-as-code Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

### Comparing `gitlabform-3.6.0/README.md` & `gitlabform-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/__init__.py` & `gitlabform-3.6.1/gitlabform/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/configuration/common.py` & `gitlabform-3.6.1/gitlabform/configuration/common.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/configuration/core.py` & `gitlabform-3.6.1/gitlabform/configuration/core.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/configuration/groups.py` & `gitlabform-3.6.1/gitlabform/configuration/groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/configuration/projects.py` & `gitlabform-3.6.1/gitlabform/configuration/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/configuration/transform.py` & `gitlabform-3.6.1/gitlabform/configuration/transform.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/__init__.py` & `gitlabform-3.6.1/gitlabform/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/branches.py` & `gitlabform-3.6.1/gitlabform/gitlab/branches.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/commits.py` & `gitlabform-3.6.1/gitlabform/gitlab/commits.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/core.py` & `gitlabform-3.6.1/gitlabform/gitlab/core.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/group_badges.py` & `gitlabform-3.6.1/gitlabform/gitlab/group_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/group_ldap_links.py` & `gitlabform-3.6.1/gitlabform/gitlab/group_ldap_links.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/group_variables.py` & `gitlabform-3.6.1/gitlabform/gitlab/group_variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/groups.py` & `gitlabform-3.6.1/gitlabform/gitlab/groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/integrations.py` & `gitlabform-3.6.1/gitlabform/gitlab/integrations.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/members.py` & `gitlabform-3.6.1/gitlabform/gitlab/members.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/merge_requests.py` & `gitlabform-3.6.1/gitlabform/gitlab/merge_requests.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/pipelines.py` & `gitlabform-3.6.1/gitlabform/gitlab/pipelines.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/project_badges.py` & `gitlabform-3.6.1/gitlabform/gitlab/project_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/project_deploy_keys.py` & `gitlabform-3.6.1/gitlabform/gitlab/project_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/project_merge_requests_approvals.py` & `gitlabform-3.6.1/gitlabform/gitlab/project_merge_requests_approvals.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/project_protected_environments.py` & `gitlabform-3.6.1/gitlabform/gitlab/project_protected_environments.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/projects.py` & `gitlabform-3.6.1/gitlabform/gitlab/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/repositories.py` & `gitlabform-3.6.1/gitlabform/gitlab/repositories.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/resource_groups.py` & `gitlabform-3.6.1/gitlabform/gitlab/resource_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/schedules.py` & `gitlabform-3.6.1/gitlabform/gitlab/schedules.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/tags.py` & `gitlabform-3.6.1/gitlabform/gitlab/tags.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/users.py` & `gitlabform-3.6.1/gitlabform/gitlab/users.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/gitlab/variables.py` & `gitlabform-3.6.1/gitlabform/gitlab/variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/lists/__init__.py` & `gitlabform-3.6.1/gitlabform/lists/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/lists/filter.py` & `gitlabform-3.6.1/gitlabform/lists/filter.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/lists/groups.py` & `gitlabform-3.6.1/gitlabform/lists/groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/lists/projects.py` & `gitlabform-3.6.1/gitlabform/lists/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/output.py` & `gitlabform-3.6.1/gitlabform/output.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/__init__.py` & `gitlabform-3.6.1/gitlabform/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/abstract_processor.py` & `gitlabform-3.6.1/gitlabform/processors/abstract_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/defining_keys.py` & `gitlabform-3.6.1/gitlabform/processors/defining_keys.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/group/__init__.py` & `gitlabform-3.6.1/gitlabform/processors/group/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/group/group_badges_processor.py` & `gitlabform-3.6.1/gitlabform/processors/group/group_badges_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/group/group_ldap_links_processor.py` & `gitlabform-3.6.1/gitlabform/processors/group/group_ldap_links_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/group/group_members_processor.py` & `gitlabform-3.6.1/gitlabform/processors/group/group_members_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/group/group_variables_processor.py` & `gitlabform-3.6.1/gitlabform/processors/group/group_variables_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/multiple_entities_processor.py` & `gitlabform-3.6.1/gitlabform/processors/multiple_entities_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/project/__init__.py` & `gitlabform-3.6.1/gitlabform/processors/project/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/project/badges_processor.py` & `gitlabform-3.6.1/gitlabform/processors/project/badges_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/project/branches_processor.py` & `gitlabform-3.6.1/gitlabform/processors/project/branches_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/project/deploy_keys_processor.py` & `gitlabform-3.6.1/gitlabform/processors/project/deploy_keys_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/project/files_processor.py` & `gitlabform-3.6.1/gitlabform/processors/project/files_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/project/hooks_processor.py` & `gitlabform-3.6.1/gitlabform/processors/project/hooks_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/project/integrations_processor.py` & `gitlabform-3.6.1/gitlabform/processors/project/integrations_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/project/members_processor.py` & `gitlabform-3.6.1/gitlabform/processors/project/members_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/project/merge_requests_approval_rules.py` & `gitlabform-3.6.1/gitlabform/processors/project/merge_requests_approval_rules.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/project/merge_requests_approvals.py` & `gitlabform-3.6.1/gitlabform/processors/project/merge_requests_approvals.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/project/project_processor.py` & `gitlabform-3.6.1/gitlabform/processors/project/project_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/project/resource_groups_processor.py` & `gitlabform-3.6.1/gitlabform/processors/project/resource_groups_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/project/schedules_processor.py` & `gitlabform-3.6.1/gitlabform/processors/project/schedules_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/project/tags_processor.py` & `gitlabform-3.6.1/gitlabform/processors/project/tags_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/project/variables_processor.py` & `gitlabform-3.6.1/gitlabform/processors/project/variables_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/shared/protected_environments_processor.py` & `gitlabform-3.6.1/gitlabform/processors/shared/protected_environments_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/single_entity_processor.py` & `gitlabform-3.6.1/gitlabform/processors/single_entity_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/util/branch_protector.py` & `gitlabform-3.6.1/gitlabform/processors/util/branch_protector.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/util/decorators.py` & `gitlabform-3.6.1/gitlabform/processors/util/decorators.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform/processors/util/difference_logger.py` & `gitlabform-3.6.1/gitlabform/processors/util/difference_logger.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/gitlabform.egg-info/PKG-INFO` & `gitlabform-3.6.1/gitlabform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabform
-Version: 3.6.0
+Version: 3.6.1
 Summary: 🏗 Specialized configuration as a code tool for GitLab projects, groups and more using hierarchical configuration written in YAML
 Home-page: https://gitlabform.github.io/gitlabform
 Author: Greg Dubicki and Contributors
 Keywords: cli,yaml,gitlab,configuration-as-code
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gitlabform Version: 3.6.0 Summary: ð Specialized
+Metadata-Version: 2.1 Name: gitlabform Version: 3.6.1 Summary: ð Specialized
 configuration as a code tool for GitLab projects, groups and more using
 hierarchical configuration written in YAML Home-page: https://
 gitlabform.github.io/gitlabform Author: Greg Dubicki and Contributors Keywords:
 cli,yaml,gitlab,configuration-as-code Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

### Comparing `gitlabform-3.6.0/gitlabform.egg-info/SOURCES.txt` & `gitlabform-3.6.1/gitlabform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/setup.py` & `gitlabform-3.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,37 +41,37 @@
     ],
     packages=find_packages(),
     package_data={"": ["LICENSE", "version", "*.md", "config.yml"]},
     include_package_data=True,
     python_requires=">=3.7.0",
     install_requires=[
         "certifi",  # we want the latest root certs for security
-        "requests==2.28.2",
+        "requests==2.31.0",
         "types-requests==2.28.11.17",
         "Jinja2==3.1.2",
         "MarkupSafe==2.1.2",
         "ruamel.yaml==0.17.21",
         "luddite==1.0.2",
         "cli-ui==0.17.2",
-        "packaging==23.0",
+        "packaging==23.1",
         "mergedeep==1.3.4",
         "yamlpath==3.8.0",
         "ez-yaml==1.2.0",
     ],
     extras_require={
         "test": [
             "python-gitlab==3.13.0",
             "pytest==7.3.1",
             "xkcdpass==1.19.3",
             "pre-commit==2.21.0",  # not really for tests, but for development
-            "coverage==7.2.1",
+            "coverage==7.2.7",
             "pytest-cov==4.0.0",
-            "deepdiff==6.2.3",
+            "deepdiff==6.3.1",
             "pytest-rerunfailures==11.1.2",
-            "cryptography==40.0.1",
+            "cryptography==41.0.2",
             "mypy==1.1.1",
             "mypy-extensions==1.0.0",
         ],
         "docs": [
             "mkdocs",
             "mkdocs-material",
         ],
```

### Comparing `gitlabform-3.6.0/tests/acceptance/__init__.py` & `gitlabform-3.6.1/tests/acceptance/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/conftest.py` & `gitlabform-3.6.1/tests/acceptance/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import date, timedelta
 import os
 from typing import Callable, Optional, Generator, List
 
 import pytest
 from cryptography.hazmat.primitives import serialization as crypto_serialization
 from cryptography.hazmat.primitives.asymmetric import rsa
 from cryptography.hazmat.backends import default_backend as crypto_default_backend
@@ -239,19 +240,21 @@
     created_tokens: List[ProjectAccessToken] = []
 
     def _make_project_access_token(
         level: AccessLevel = AccessLevel.DEVELOPER, scopes: List[str] = ["api"]
     ) -> ProjectAccessToken:
         last_id = len(created_tokens) + 1
         token_name = f"{token_name_base}_{last_id}_bot"
+        expires_at = (date.today() + timedelta(days=30)).isoformat()
         token = project.access_tokens.create(
             {
                 "access_level": level,
                 "name": token_name,
                 "scopes": scopes,
+                "expires_at": expires_at,
             }
         )
         created_tokens.append(token)
         return token
 
     yield _make_project_access_token
 
@@ -268,19 +271,21 @@
     created_tokens: List[GroupAccessToken] = []
 
     def _make_group_access_token(
         level: AccessLevel = AccessLevel.DEVELOPER, scopes: List[str] = ["api"]
     ) -> GroupAccessToken:
         last_id = len(created_tokens) + 1
         token_name = f"{token_name_base}_{last_id}_bot"
+        expires_at = (date.today() + timedelta(days=30)).isoformat()
         token = group.access_tokens.create(
             {
                 "access_level": level,
                 "name": token_name,
                 "scopes": scopes,
+                "expires_at": expires_at,
             }
         )
         created_tokens.append(token)
         return token
 
     yield _make_group_access_token
```

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_archive_project.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_archive_project.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_badges.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_branches.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_branches.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_deploy_keys.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_deploy_keys_all_projects.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_deploy_keys_all_projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_files.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_files.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_files_all.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_files_all.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_files_protected.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_files_protected.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_files_templates.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_files_templates.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_group_badges.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_group_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_group_members_groups.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_group_members_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_group_members_users.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_group_members_users.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_group_settings.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_group_settings.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_group_variables.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_group_variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_inheritance_break.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_inheritance_break.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_integrations.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_integrations.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_members.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_members.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_members_add_group.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_members_add_group.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_members_enforce.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_members_enforce.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_project_settings.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_project_settings.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_resource_groups.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_resource_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_running.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_running.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_schedules.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_schedules.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_tags.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_tags.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_token_from_config.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_token_from_config.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/acceptance/standard/test_variables.py` & `gitlabform-3.6.1/tests/acceptance/standard/test_variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/unit/configuration/test_case_sensitivity.py` & `gitlabform-3.6.1/tests/unit/configuration/test_case_sensitivity.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/unit/configuration/test_inheritance_break_projects_and_groups.py` & `gitlabform-3.6.1/tests/unit/configuration/test_inheritance_break_projects_and_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/unit/configuration/test_inheritance_break_subgroups.py` & `gitlabform-3.6.1/tests/unit/configuration/test_inheritance_break_subgroups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/unit/configuration/test_inheritance_break_validation.py` & `gitlabform-3.6.1/tests/unit/configuration/test_inheritance_break_validation.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/unit/configuration/test_projects_and_groups.py` & `gitlabform-3.6.1/tests/unit/configuration/test_projects_and_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/unit/configuration/test_skip_groups_skip_projects.py` & `gitlabform-3.6.1/tests/unit/configuration/test_skip_groups_skip_projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/unit/configuration/test_subgroups.py` & `gitlabform-3.6.1/tests/unit/configuration/test_subgroups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/unit/configuration/test_yaml_version.py` & `gitlabform-3.6.1/tests/unit/configuration/test_yaml_version.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/unit/processors/test_abstract_processor.py` & `gitlabform-3.6.1/tests/unit/processors/test_abstract_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/unit/processors/test_branch_protector.py` & `gitlabform-3.6.1/tests/unit/processors/test_branch_protector.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/unit/processors/test_difference_logger.py` & `gitlabform-3.6.1/tests/unit/processors/test_difference_logger.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/unit/test_access_levels.py` & `gitlabform-3.6.1/tests/unit/test_access_levels.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.0/tests/unit/test_non_empty_configs_provider.py` & `gitlabform-3.6.1/tests/unit/test_non_empty_configs_provider.py`

 * *Files identical despite different names*

