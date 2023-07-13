# Comparing `tmp/renku-2.6.0rc1.tar.gz` & `tmp/renku-2.6.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renku-2.6.0rc1.tar", max compression
+gzip compressed data, was "renku-2.6.1rc1.tar", max compression
```

## Comparing `renku-2.6.0rc1.tar` & `renku-2.6.1rc1.tar`

### file list

```diff
@@ -1,679 +1,679 @@
--rw-r--r--   0        0        0      900 2023-06-22 14:43:37.012647 renku-2.6.0rc1/AUTHORS.rst
--rw-r--r--   0        0        0   182553 2023-06-22 14:43:37.012647 renku-2.6.0rc1/CHANGES.rst
--rw-r--r--   0        0        0    11358 2023-06-22 14:43:37.012647 renku-2.6.0rc1/LICENSE
--rw-r--r--   0        0        0    12889 2023-06-22 14:43:37.016647 renku-2.6.0rc1/README.rst
--rw-r--r--   0        0        0    10490 2023-06-22 14:44:47.313028 renku-2.6.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4391 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/__init__.py
--rw-r--r--   0        0        0      784 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/__init__.py
--rw-r--r--   0        0        0      209 2023-06-22 14:44:41.360996 renku-2.6.0rc1/renku/command/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      437 2023-06-22 14:44:41.360996 renku-2.6.0rc1/renku/command/__pycache__/options.cpython-39.pyc
--rw-r--r--   0        0        0     1057 2023-06-22 14:44:45.241017 renku-2.6.0rc1/renku/command/__pycache__/run.cpython-39.pyc
--rw-r--r--   0        0        0     1343 2023-06-22 14:44:41.360996 renku-2.6.0rc1/renku/command/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0      593 2023-06-22 14:44:41.360996 renku-2.6.0rc1/renku/command/__pycache__/version.cpython-39.pyc
--rw-r--r--   0        0        0     2096 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/checks/__init__.py
--rw-r--r--   0        0        0     4808 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/checks/activities.py
--rw-r--r--   0        0        0     8408 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/checks/datasets.py
--rw-r--r--   0        0        0     2797 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/checks/githooks.py
--rw-r--r--   0        0        0     1548 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/checks/migration.py
--rw-r--r--   0        0        0     2448 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/checks/project.py
--rw-r--r--   0        0        0     1572 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/checks/storage.py
--rw-r--r--   0        0        0     4124 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/checks/validate_shacl.py
--rw-r--r--   0        0        0     5025 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/checks/workflow.py
--rw-r--r--   0        0        0     3872 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/clone.py
--rw-r--r--   0        0        0      828 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/command_builder/__init__.py
--rw-r--r--   0        0        0      301 2023-06-22 14:44:42.069000 renku-2.6.0rc1/renku/command/command_builder/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    15431 2023-06-22 14:44:42.073000 renku-2.6.0rc1/renku/command/command_builder/__pycache__/command.cpython-39.pyc
--rw-r--r--   0        0        0    16678 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/command_builder/command.py
--rw-r--r--   0        0        0     1951 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/command_builder/communication.py
--rw-r--r--   0        0        0     5325 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/command_builder/database.py
--rw-r--r--   0        0        0     1701 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/command_builder/lock.py
--rw-r--r--   0        0        0     1481 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/command_builder/migration.py
--rw-r--r--   0        0        0     7694 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/command_builder/repo.py
--rw-r--r--   0        0        0     4803 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/config.py
--rw-r--r--   0        0        0     5640 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/dataset.py
--rw-r--r--   0        0        0     2835 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/doctor.py
--rw-r--r--   0        0        0      775 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/format/__init__.py
--rw-r--r--   0        0        0      220 2023-06-22 14:44:41.616998 renku-2.6.0rc1/renku/command/format/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5765 2023-06-22 14:44:41.620998 renku-2.6.0rc1/renku/command/format/__pycache__/dataset_files.cpython-39.pyc
--rw-r--r--   0        0        0     1508 2023-06-22 14:44:41.620998 renku-2.6.0rc1/renku/command/format/__pycache__/dataset_tags.cpython-39.pyc
--rw-r--r--   0        0        0     2884 2023-06-22 14:44:41.620998 renku-2.6.0rc1/renku/command/format/__pycache__/datasets.cpython-39.pyc
--rw-r--r--   0        0        0      817 2023-06-22 14:44:44.129011 renku-2.6.0rc1/renku/command/format/__pycache__/json.cpython-39.pyc
--rw-r--r--   0        0        0     1754 2023-06-22 14:44:45.265017 renku-2.6.0rc1/renku/command/format/__pycache__/session.cpython-39.pyc
--rw-r--r--   0        0        0     1929 2023-06-22 14:44:44.129011 renku-2.6.0rc1/renku/command/format/__pycache__/tabulate.cpython-39.pyc
--rw-r--r--   0        0        0     2416 2023-06-22 14:44:44.129011 renku-2.6.0rc1/renku/command/format/__pycache__/workflow.cpython-39.pyc
--rw-r--r--   0        0        0     2643 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/format/activity.py
--rw-r--r--   0        0        0     6230 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/format/dataset_files.py
--rw-r--r--   0        0        0     2098 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/format/dataset_tags.py
--rw-r--r--   0        0        0     3236 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/format/datasets.py
--rw-r--r--   0        0        0     1212 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/format/json.py
--rw-r--r--   0        0        0     2402 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/format/session.py
--rw-r--r--   0        0        0     2769 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/format/tabulate.py
--rw-r--r--   0        0        0     2728 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/format/workflow.py
--rw-r--r--   0        0        0     1012 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/gc.py
--rw-r--r--   0        0        0     1154 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/githooks.py
--rw-r--r--   0        0        0     9880 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/graph.py
--rw-r--r--   0        0        0     1081 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/group.py
--rw-r--r--   0        0        0     1203 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/init.py
--rw-r--r--   0        0        0     3124 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/log.py
--rw-r--r--   0        0        0     1241 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/login.py
--rw-r--r--   0        0        0     2822 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/mergetool.py
--rw-r--r--   0        0        0    10732 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/migrate.py
--rw-r--r--   0        0        0     9141 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/move.py
--rw-r--r--   0        0        0     1015 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/options.py
--rw-r--r--   0        0        0     1362 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/project.py
--rw-r--r--   0        0        0     4748 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/remove.py
--rw-r--r--   0        0        0     3146 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/rerun.py
--rw-r--r--   0        0        0    10987 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/rollback.py
--rw-r--r--   0        0        0     1600 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/run.py
--rw-r--r--   0        0        0     3375 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/save.py
--rw-r--r--   0        0        0      766 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/__init__.py
--rw-r--r--   0        0        0      211 2023-06-22 14:44:41.824999 renku-2.6.0rc1/renku/command/schema/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2040 2023-06-22 14:44:41.828999 renku-2.6.0rc1/renku/command/schema/__pycache__/agent.cpython-39.pyc
--rw-r--r--   0        0        0      977 2023-06-22 14:44:42.009000 renku-2.6.0rc1/renku/command/schema/__pycache__/annotation.cpython-39.pyc
--rw-r--r--   0        0        0     6652 2023-06-22 14:44:41.997000 renku-2.6.0rc1/renku/command/schema/__pycache__/calamus.cpython-39.pyc
--rw-r--r--   0        0        0     7584 2023-06-22 14:44:41.828999 renku-2.6.0rc1/renku/command/schema/__pycache__/dataset.cpython-39.pyc
--rw-r--r--   0        0        0     1345 2023-06-22 14:44:42.009000 renku-2.6.0rc1/renku/command/schema/__pycache__/entity.cpython-39.pyc
--rw-r--r--   0        0        0     5615 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/activity.py
--rw-r--r--   0        0        0     2478 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/agent.py
--rw-r--r--   0        0        0     1235 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/annotation.py
--rw-r--r--   0        0        0     8986 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/calamus.py
--rw-r--r--   0        0        0     3186 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/composite_plan.py
--rw-r--r--   0        0        0     8210 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/dataset.py
--rw-r--r--   0        0        0     1445 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/entity.py
--rw-r--r--   0        0        0     4016 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/parameter.py
--rw-r--r--   0        0        0     3427 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/plan.py
--rw-r--r--   0        0        0     3406 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/project.py
--rw-r--r--   0        0        0     3065 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/workflow_file.py
--rw-r--r--   0        0        0     2039 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/session.py
--rw-r--r--   0        0        0     1036 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/status.py
--rw-r--r--   0        0        0     3944 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/storage.py
--rw-r--r--   0        0        0     1919 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/template.py
--rw-r--r--   0        0        0     1254 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/update.py
--rw-r--r--   0        0        0     1726 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/util.py
--rw-r--r--   0        0        0     1088 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/version.py
--rw-r--r--   0        0        0      768 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/view_model/__init__.py
--rw-r--r--   0        0        0      217 2023-06-22 14:44:42.197001 renku-2.6.0rc1/renku/command/view_model/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    13290 2023-06-22 14:44:44.133011 renku-2.6.0rc1/renku/command/view_model/__pycache__/activity_graph.cpython-39.pyc
--rw-r--r--   0        0        0     1350 2023-06-22 14:44:44.177011 renku-2.6.0rc1/renku/command/view_model/__pycache__/agent.cpython-39.pyc
--rw-r--r--   0        0        0     8157 2023-06-22 14:44:44.177011 renku-2.6.0rc1/renku/command/view_model/__pycache__/composite_plan.cpython-39.pyc
--rw-r--r--   0        0        0     1848 2023-06-22 14:44:42.201001 renku-2.6.0rc1/renku/command/view_model/__pycache__/dataset.cpython-39.pyc
--rw-r--r--   0        0        0    11145 2023-06-22 14:44:45.193017 renku-2.6.0rc1/renku/command/view_model/__pycache__/log.cpython-39.pyc
--rw-r--r--   0        0        0     7823 2023-06-22 14:44:44.177011 renku-2.6.0rc1/renku/command/view_model/__pycache__/plan.cpython-39.pyc
--rw-r--r--   0        0        0    14258 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/view_model/activity_graph.py
--rw-r--r--   0        0        0     1657 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/view_model/agent.py
--rw-r--r--   0        0        0     8768 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/view_model/composite_plan.py
--rw-r--r--   0        0        0     2138 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/view_model/dataset.py
--rw-r--r--   0        0        0     7850 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/command/view_model/graph.py
--rw-r--r--   0        0        0    12497 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/command/view_model/log.py
--rw-r--r--   0        0        0     9377 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/command/view_model/plan.py
--rw-r--r--   0        0        0     3306 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/command/view_model/project.py
--rw-r--r--   0        0        0     5947 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/command/view_model/template.py
--rw-r--r--   0        0        0    15885 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/command/view_model/text_canvas.py
--rw-r--r--   0        0        0     4792 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/command/view_model/workflow_file.py
--rw-r--r--   0        0        0     4114 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/command/workflow.py
--rw-r--r--   0        0        0      745 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/__init__.py
--rw-r--r--   0        0        0      180 2023-06-22 14:44:41.360996 renku-2.6.0rc1/renku/core/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4501 2023-06-22 14:44:41.648998 renku-2.6.0rc1/renku/core/__pycache__/config.cpython-39.pyc
--rw-r--r--   0        0        0     1707 2023-06-22 14:44:41.368996 renku-2.6.0rc1/renku/core/__pycache__/constant.cpython-39.pyc
--rw-r--r--   0        0        0    34603 2023-06-22 14:44:41.364997 renku-2.6.0rc1/renku/core/__pycache__/errors.cpython-39.pyc
--rw-r--r--   0        0        0     4854 2023-06-22 14:44:44.181011 renku-2.6.0rc1/renku/core/__pycache__/git.cpython-39.pyc
--rw-r--r--   0        0        0     8039 2023-06-22 14:44:42.081000 renku-2.6.0rc1/renku/core/__pycache__/login.cpython-39.pyc
--rw-r--r--   0        0        0    14579 2023-06-22 14:44:42.037000 renku-2.6.0rc1/renku/core/__pycache__/storage.cpython-39.pyc
--rw-r--r--   0        0        0     6170 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/config.py
--rw-r--r--   0        0        0     2717 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/constant.py
--rw-r--r--   0        0        0      765 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/__init__.py
--rw-r--r--   0        0        0      208 2023-06-22 14:44:41.624998 renku-2.6.0rc1/renku/core/dataset/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2042 2023-06-22 14:44:42.169001 renku-2.6.0rc1/renku/core/dataset/__pycache__/context.cpython-39.pyc
--rw-r--r--   0        0        0    38317 2023-06-22 14:44:42.181001 renku-2.6.0rc1/renku/core/dataset/__pycache__/dataset.cpython-39.pyc
--rw-r--r--   0        0        0    15656 2023-06-22 14:44:42.169001 renku-2.6.0rc1/renku/core/dataset/__pycache__/dataset_add.cpython-39.pyc
--rw-r--r--   0        0        0     7431 2023-06-22 14:44:42.069000 renku-2.6.0rc1/renku/core/dataset/__pycache__/datasets_provenance.cpython-39.pyc
--rw-r--r--   0        0        0     3355 2023-06-22 14:44:42.033000 renku-2.6.0rc1/renku/core/dataset/__pycache__/pointer_file.cpython-39.pyc
--rw-r--r--   0        0        0     2737 2023-06-22 14:44:42.201001 renku-2.6.0rc1/renku/core/dataset/__pycache__/request_model.cpython-39.pyc
--rw-r--r--   0        0        0     5280 2023-06-22 14:44:42.205001 renku-2.6.0rc1/renku/core/dataset/__pycache__/tag.cpython-39.pyc
--rw-r--r--   0        0        0     2954 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/context.py
--rw-r--r--   0        0        0    50044 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/dataset.py
--rw-r--r--   0        0        0    21429 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/dataset_add.py
--rw-r--r--   0        0        0     9747 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/datasets_provenance.py
--rw-r--r--   0        0        0     4296 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/pointer_file.py
--rw-r--r--   0        0        0      760 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/__init__.py
--rw-r--r--   0        0        0      213 2023-06-22 14:44:41.624998 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    18159 2023-06-22 14:44:41.628998 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/api.cpython-39.pyc
--rw-r--r--   0        0        0     6734 2023-06-22 14:44:41.808999 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/azure.cpython-39.pyc
--rw-r--r--   0        0        0     1646 2023-06-22 14:44:41.812999 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/common.cpython-39.pyc
--rw-r--r--   0        0        0    19710 2023-06-22 14:44:42.025000 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/dataverse.cpython-39.pyc
--rw-r--r--   0        0        0     3221 2023-06-22 14:44:42.025000 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/dataverse_metadata_templates.cpython-39.pyc
--rw-r--r--   0        0        0     5087 2023-06-22 14:44:42.029000 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/doi.cpython-39.pyc
--rw-r--r--   0        0        0     5963 2023-06-22 14:44:42.029000 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/external.cpython-39.pyc
--rw-r--r--   0        0        0     5562 2023-06-22 14:44:41.628998 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/factory.cpython-39.pyc
--rw-r--r--   0        0        0     7710 2023-06-22 14:44:42.033000 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/git.cpython-39.pyc
--rw-r--r--   0        0        0    10821 2023-06-22 14:44:42.057000 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/local.cpython-39.pyc
--rw-r--r--   0        0        0     6644 2023-06-22 14:44:41.812999 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/models.cpython-39.pyc
--rw-r--r--   0        0        0     9573 2023-06-22 14:44:42.061000 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/olos.cpython-39.pyc
--rw-r--r--   0        0        0    17180 2023-06-22 14:44:42.069000 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/renku.cpython-39.pyc
--rw-r--r--   0        0        0     2538 2023-06-22 14:44:42.029000 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/repository.cpython-39.pyc
--rw-r--r--   0        0        0     6260 2023-06-22 14:44:42.161001 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/s3.cpython-39.pyc
--rw-r--r--   0        0        0     7131 2023-06-22 14:44:42.165001 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/web.cpython-39.pyc
--rw-r--r--   0        0        0    18001 2023-06-22 14:44:42.253001 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/zenodo.cpython-39.pyc
--rw-r--r--   0        0        0    16174 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/api.py
--rw-r--r--   0        0        0     6987 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/azure.py
--rw-r--r--   0        0        0     2225 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/common.py
--rw-r--r--   0        0        0    21202 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/dataverse.py
--rw-r--r--   0        0        0     3742 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/dataverse_metadata_templates.py
--rw-r--r--   0        0        0     4829 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/doi.py
--rw-r--r--   0        0        0     5623 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/external.py
--rw-r--r--   0        0        0     5764 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/factory.py
--rw-r--r--   0        0        0    10563 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/git.py
--rw-r--r--   0        0        0    14308 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/local.py
--rw-r--r--   0        0        0     6292 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/models.py
--rw-r--r--   0        0        0    10118 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/olos.py
--rw-r--r--   0        0        0    22167 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/renku.py
--rw-r--r--   0        0        0     2553 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/repository.py
--rw-r--r--   0        0        0     6413 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/s3.py
--rw-r--r--   0        0        0     9427 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/web.py
--rw-r--r--   0        0        0    18757 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/zenodo.py
--rw-r--r--   0        0        0     3973 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/request_model.py
--rw-r--r--   0        0        0     5361 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/tag.py
--rw-r--r--   0        0        0    25658 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/errors.py
--rw-r--r--   0        0        0     1115 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/gc.py
--rw-r--r--   0        0        0     7394 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/git.py
--rw-r--r--   0        0        0     2151 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/githooks.py
--rw-r--r--   0        0        0    16526 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/init.py
--rw-r--r--   0        0        0      775 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/interface/__init__.py
--rw-r--r--   0        0        0      207 2023-06-22 14:44:42.017000 renku-2.6.0rc1/renku/core/interface/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4269 2023-06-22 14:44:44.133011 renku-2.6.0rc1/renku/core/interface/__pycache__/activity_gateway.cpython-39.pyc
--rw-r--r--   0        0        0     1246 2023-06-22 14:44:44.181011 renku-2.6.0rc1/renku/core/interface/__pycache__/database_gateway.cpython-39.pyc
--rw-r--r--   0        0        0     2159 2023-06-22 14:44:42.081000 renku-2.6.0rc1/renku/core/interface/__pycache__/dataset_gateway.cpython-39.pyc
--rw-r--r--   0        0        0     2057 2023-06-22 14:44:44.121011 renku-2.6.0rc1/renku/core/interface/__pycache__/plan_gateway.cpython-39.pyc
--rw-r--r--   0        0        0      959 2023-06-22 14:44:44.121011 renku-2.6.0rc1/renku/core/interface/__pycache__/project_gateway.cpython-39.pyc
--rw-r--r--   0        0        0     4402 2023-06-22 14:44:42.017000 renku-2.6.0rc1/renku/core/interface/__pycache__/storage.cpython-39.pyc
--rw-r--r--   0        0        0     1579 2023-06-22 14:44:44.029011 renku-2.6.0rc1/renku/core/interface/__pycache__/workflow_file_parser.cpython-39.pyc
--rw-r--r--   0        0        0     3741 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/interface/activity_gateway.py
--rw-r--r--   0        0        0     1418 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/interface/database_gateway.py
--rw-r--r--   0        0        0     2095 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/interface/dataset_gateway.py
--rw-r--r--   0        0        0     1996 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/interface/plan_gateway.py
--rw-r--r--   0        0        0     1212 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/interface/project_gateway.py
--rw-r--r--   0        0        0     4226 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/interface/storage.py
--rw-r--r--   0        0        0     1780 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/interface/workflow_file_parser.py
--rw-r--r--   0        0        0    10639 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/login.py
--rw-r--r--   0        0        0      764 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/__init__.py
--rw-r--r--   0        0        0      196 2023-06-22 14:44:41.748998 renku-2.6.0rc1/renku/core/migration/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1122 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0003__0_pyld2.py
--rw-r--r--   0        0        0    15324 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0003__1_jsonld.py
--rw-r--r--   0        0        0     9570 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0003__2_initial.py
--rw-r--r--   0        0        0     1122 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0004__0_pyld2.py
--rw-r--r--   0        0        0     5318 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0004__submodules.py
--rw-r--r--   0        0        0     1548 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0005__1_pyld2.py
--rw-r--r--   0        0        0    16075 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0005__2_cwl.py
--rw-r--r--   0        0        0     1015 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0006__dataset_context.py
--rw-r--r--   0        0        0     1430 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0007__source_url.py
--rw-r--r--   0        0        0     1175 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0008__dataset_metadata.py
--rw-r--r--   0        0        0    30683 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0009__new_metadata_storage.py
--rw-r--r--   0        0        0    14077 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0010__metadata_fixes.py
--rw-r--r--   0        0        0    10163 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/migrate.py
--rw-r--r--   0        0        0      770 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/models/__init__.py
--rw-r--r--   0        0        0     5830 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/models/migration.py
--rw-r--r--   0        0        0     3861 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/models/refs.py
--rw-r--r--   0        0        0     5091 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/models/v10.py
--rw-r--r--   0        0        0    11828 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/models/v3.py
--rw-r--r--   0        0        0     2422 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/models/v7.py
--rw-r--r--   0        0        0     4587 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/models/v8.py
--rw-r--r--   0        0        0    74094 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/models/v9.py
--rw-r--r--   0        0        0     7945 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/utils/__init__.py
--rw-r--r--   0        0        0     6660 2023-06-22 14:44:41.748998 renku-2.6.0rc1/renku/core/migration/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     8121 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/utils/conversion.py
--rw-r--r--   0        0        0      824 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/plugin/__init__.py
--rw-r--r--   0        0        0      265 2023-06-22 14:44:41.632998 renku-2.6.0rc1/renku/core/plugin/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1033 2023-06-22 14:44:41.804999 renku-2.6.0rc1/renku/core/plugin/__pycache__/dataset_provider.cpython-39.pyc
--rw-r--r--   0        0        0     1049 2023-06-22 14:44:41.808999 renku-2.6.0rc1/renku/core/plugin/__pycache__/pluginmanager.cpython-39.pyc
--rw-r--r--   0        0        0     3246 2023-06-22 14:44:43.137006 renku-2.6.0rc1/renku/core/plugin/__pycache__/provider.cpython-39.pyc
--rw-r--r--   0        0        0     1467 2023-06-22 14:44:45.081016 renku-2.6.0rc1/renku/core/plugin/__pycache__/run.cpython-39.pyc
--rw-r--r--   0        0        0     1170 2023-06-22 14:44:45.265017 renku-2.6.0rc1/renku/core/plugin/__pycache__/session.cpython-39.pyc
--rw-r--r--   0        0        0     4177 2023-06-22 14:44:44.689014 renku-2.6.0rc1/renku/core/plugin/__pycache__/workflow.cpython-39.pyc
--rw-r--r--   0        0        0     2978 2023-06-22 14:44:44.141011 renku-2.6.0rc1/renku/core/plugin/__pycache__/workflow_file_parser.cpython-39.pyc
--rw-r--r--   0        0        0     1467 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/plugin/dataset_provider.py
--rw-r--r--   0        0        0     3046 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/plugin/implementations/__init__.py
--rw-r--r--   0        0        0     2540 2023-06-22 14:44:41.808999 renku-2.6.0rc1/renku/core/plugin/implementations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1790 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/plugin/pluginmanager.py
--rw-r--r--   0        0        0     3357 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/plugin/provider.py
--rw-r--r--   0        0        0     1839 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/plugin/run.py
--rw-r--r--   0        0        0     1515 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/plugin/session.py
--rw-r--r--   0        0        0     4195 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/plugin/workflow.py
--rw-r--r--   0        0        0     3065 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/plugin/workflow_file_parser.py
--rw-r--r--   0        0        0     3355 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/project.py
--rw-r--r--   0        0        0      770 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/session/__init__.py
--rw-r--r--   0        0        0      210 2023-06-22 14:44:42.253001 renku-2.6.0rc1/renku/core/session/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    16099 2023-06-22 14:44:42.257001 renku-2.6.0rc1/renku/core/session/__pycache__/docker.cpython-39.pyc
--rw-r--r--   0        0        0    16431 2023-06-22 14:44:42.453002 renku-2.6.0rc1/renku/core/session/__pycache__/renkulab.cpython-39.pyc
--rw-r--r--   0        0        0     1449 2023-06-22 14:44:42.457002 renku-2.6.0rc1/renku/core/session/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0        0        0    22065 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/session/docker.py
--rw-r--r--   0        0        0    21512 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/session/renkulab.py
--rw-r--r--   0        0        0    13503 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/session/session.py
--rw-r--r--   0        0        0     2206 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/session/utils.py
--rw-r--r--   0        0        0    19478 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/storage.py
--rw-r--r--   0        0        0      760 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/template/__init__.py
--rw-r--r--   0        0        0    22043 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/template/template.py
--rw-r--r--   0        0        0    14612 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/template/usecase.py
--rw-r--r--   0        0        0      756 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/__init__.py
--rw-r--r--   0        0        0      196 2023-06-22 14:44:41.372996 renku-2.6.0rc1/renku/core/util/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    11124 2023-06-22 14:44:41.644998 renku-2.6.0rc1/renku/core/util/__pycache__/communication.cpython-39.pyc
--rw-r--r--   0        0        0     6320 2023-06-22 14:44:44.181011 renku-2.6.0rc1/renku/core/util/__pycache__/contexts.cpython-39.pyc
--rw-r--r--   0        0        0     1801 2023-06-22 14:44:41.744999 renku-2.6.0rc1/renku/core/util/__pycache__/datetime8601.cpython-39.pyc
--rw-r--r--   0        0        0      933 2023-06-22 14:44:41.808999 renku-2.6.0rc1/renku/core/util/__pycache__/doi.cpython-39.pyc
--rw-r--r--   0        0        0    33652 2023-06-22 14:44:41.380997 renku-2.6.0rc1/renku/core/util/__pycache__/git.cpython-39.pyc
--rw-r--r--   0        0        0      669 2023-06-22 14:44:42.457002 renku-2.6.0rc1/renku/core/util/__pycache__/jwt.cpython-39.pyc
--rw-r--r--   0        0        0     6008 2023-06-22 14:44:41.748998 renku-2.6.0rc1/renku/core/util/__pycache__/metadata.cpython-39.pyc
--rw-r--r--   0        0        0    11013 2023-06-22 14:44:41.588998 renku-2.6.0rc1/renku/core/util/__pycache__/os.cpython-39.pyc
--rw-r--r--   0        0        0     6893 2023-06-22 14:44:42.245001 renku-2.6.0rc1/renku/core/util/__pycache__/requests.cpython-39.pyc
--rw-r--r--   0        0        0     5971 2023-06-22 14:44:42.489002 renku-2.6.0rc1/renku/core/util/__pycache__/ssh.cpython-39.pyc
--rw-r--r--   0        0        0     1736 2023-06-22 14:44:42.209001 renku-2.6.0rc1/renku/core/util/__pycache__/tabulate.cpython-39.pyc
--rw-r--r--   0        0        0     4943 2023-06-22 14:44:41.644998 renku-2.6.0rc1/renku/core/util/__pycache__/urls.cpython-39.pyc
--rw-r--r--   0        0        0     3737 2023-06-22 14:44:42.209001 renku-2.6.0rc1/renku/core/util/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0     2663 2023-06-22 14:44:41.752998 renku-2.6.0rc1/renku/core/util/__pycache__/yaml.cpython-39.pyc
--rw-r--r--   0        0        0    10282 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/communication.py
--rw-r--r--   0        0        0     6617 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/contexts.py
--rw-r--r--   0        0        0     2313 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/datetime8601.py
--rw-r--r--   0        0        0     1376 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/doi.py
--rw-r--r--   0        0        0    40689 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/git.py
--rw-r--r--   0        0        0     1244 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/jwt.py
--rw-r--r--   0        0        0     7036 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/metadata.py
--rw-r--r--   0        0        0    12140 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/os.py
--rw-r--r--   0        0        0     7626 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/requests.py
--rw-r--r--   0        0        0     1611 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/shacl.py
--rw-r--r--   0        0        0     6871 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/ssh.py
--rw-r--r--   0        0        0     2158 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/tabulate.py
--rw-r--r--   0        0        0     6228 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/urls.py
--rw-r--r--   0        0        0     3878 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/util.py
--rw-r--r--   0        0        0     2836 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/yaml.py
--rw-r--r--   0        0        0      773 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/__init__.py
--rw-r--r--   0        0        0      204 2023-06-22 14:44:42.489002 renku-2.6.0rc1/renku/core/workflow/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    18165 2023-06-22 14:44:44.189011 renku-2.6.0rc1/renku/core/workflow/__pycache__/activity.cpython-39.pyc
--rw-r--r--   0        0        0    14583 2023-06-22 14:44:45.249017 renku-2.6.0rc1/renku/core/workflow/__pycache__/execute.cpython-39.pyc
--rw-r--r--   0        0        0    26495 2023-06-22 14:44:44.129011 renku-2.6.0rc1/renku/core/workflow/__pycache__/plan.cpython-39.pyc
--rw-r--r--   0        0        0    23623 2023-06-22 14:44:44.197011 renku-2.6.0rc1/renku/core/workflow/__pycache__/plan_factory.cpython-39.pyc
--rw-r--r--   0        0        0    10263 2023-06-22 14:44:44.173011 renku-2.6.0rc1/renku/core/workflow/__pycache__/run.cpython-39.pyc
--rw-r--r--   0        0        0     1660 2023-06-22 14:44:44.197011 renku-2.6.0rc1/renku/core/workflow/__pycache__/types.cpython-39.pyc
--rw-r--r--   0        0        0     8676 2023-06-22 14:44:44.145011 renku-2.6.0rc1/renku/core/workflow/__pycache__/value_resolution.cpython-39.pyc
--rw-r--r--   0        0        0     4780 2023-06-22 14:44:45.245017 renku-2.6.0rc1/renku/core/workflow/__pycache__/workflow_file.cpython-39.pyc
--rw-r--r--   0        0        0    22713 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/activity.py
--rw-r--r--   0        0        0      773 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/converters/__init__.py
--rw-r--r--   0        0        0      215 2023-06-22 14:44:42.493003 renku-2.6.0rc1/renku/core/workflow/converters/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    11079 2023-06-22 14:44:42.493003 renku-2.6.0rc1/renku/core/workflow/converters/__pycache__/cwl.cpython-39.pyc
--rw-r--r--   0        0        0     4668 2023-06-22 14:44:44.025010 renku-2.6.0rc1/renku/core/workflow/converters/__pycache__/renku.cpython-39.pyc
--rw-r--r--   0        0        0    17937 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/converters/cwl.py
--rw-r--r--   0        0        0     5142 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/converters/renku.py
--rw-r--r--   0        0        0    18756 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/execute.py
--rw-r--r--   0        0        0      769 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/model/__init__.py
--rw-r--r--   0        0        0      206 2023-06-22 14:44:43.141006 renku-2.6.0rc1/renku/core/workflow/model/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4825 2023-06-22 14:44:43.141006 renku-2.6.0rc1/renku/core/workflow/model/__pycache__/concrete_execution_graph.cpython-39.pyc
--rw-r--r--   0        0        0    26172 2023-06-22 14:44:44.037011 renku-2.6.0rc1/renku/core/workflow/model/__pycache__/workflow_file.cpython-39.pyc
--rw-r--r--   0        0        0     6530 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/model/concrete_execution_graph.py
--rw-r--r--   0        0        0    37866 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/model/workflow_file.py
--rw-r--r--   0        0        0      775 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/parser/__init__.py
--rw-r--r--   0        0        0      213 2023-06-22 14:44:44.025010 renku-2.6.0rc1/renku/core/workflow/parser/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     8620 2023-06-22 14:44:44.029011 renku-2.6.0rc1/renku/core/workflow/parser/__pycache__/renku.cpython-39.pyc
--rw-r--r--   0        0        0    10631 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/parser/renku.py
--rw-r--r--   0        0        0    34209 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/plan.py
--rw-r--r--   0        0        0    33046 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/plan_factory.py
--rw-r--r--   0        0        0      772 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/providers/__init__.py
--rw-r--r--   0        0        0      213 2023-06-22 14:44:44.205011 renku-2.6.0rc1/renku/core/workflow/providers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4631 2023-06-22 14:44:44.205011 renku-2.6.0rc1/renku/core/workflow/providers/__pycache__/cwltool.cpython-39.pyc
--rw-r--r--   0        0        0     3918 2023-06-22 14:44:44.689014 renku-2.6.0rc1/renku/core/workflow/providers/__pycache__/local.cpython-39.pyc
--rw-r--r--   0        0        0    11194 2023-06-22 14:44:44.693014 renku-2.6.0rc1/renku/core/workflow/providers/__pycache__/toil.cpython-39.pyc
--rw-r--r--   0        0        0     5999 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/providers/cwltool.py
--rw-r--r--   0        0        0     4271 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/providers/local.py
--rw-r--r--   0        0        0    13372 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/core/workflow/providers/toil.py
--rw-r--r--   0        0        0    14384 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/core/workflow/run.py
--rw-r--r--   0        0        0     1681 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/core/workflow/types.py
--rw-r--r--   0        0        0     2869 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/core/workflow/update.py
--rw-r--r--   0        0        0     8335 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/core/workflow/value_resolution.py
--rw-r--r--   0        0        0     5089 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/core/workflow/workflow_file.py
--rw-r--r--   0        0        0      767 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/data/__init__.py
--rw-r--r--   0        0        0      114 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/data/defaults.ini
--rw-r--r--   0        0        0     3364 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/data/gitignore.default
--rwxr-xr-x   0        0        0     4474 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/data/pre-commit.sh
--rw-r--r--   0        0        0    48383 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/data/shacl_shape.json
--rw-r--r--   0        0        0      767 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/__init__.py
--rw-r--r--   0        0        0      210 2023-06-22 14:44:41.596998 renku-2.6.0rc1/renku/domain_model/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      388 2023-06-22 14:44:41.624998 renku-2.6.0rc1/renku/domain_model/__pycache__/constant.cpython-39.pyc
--rw-r--r--   0        0        0    26295 2023-06-22 14:44:41.656998 renku-2.6.0rc1/renku/domain_model/__pycache__/dataset.cpython-39.pyc
--rw-r--r--   0        0        0      988 2023-06-22 14:44:41.804999 renku-2.6.0rc1/renku/domain_model/__pycache__/dataset_provider.cpython-39.pyc
--rw-r--r--   0        0        0     2204 2023-06-22 14:44:44.197011 renku-2.6.0rc1/renku/domain_model/__pycache__/datastructures.cpython-39.pyc
--rw-r--r--   0        0        0     2539 2023-06-22 14:44:42.009000 renku-2.6.0rc1/renku/domain_model/__pycache__/entity.cpython-39.pyc
--rw-r--r--   0        0        0      575 2023-06-22 14:44:41.648998 renku-2.6.0rc1/renku/domain_model/__pycache__/enums.cpython-39.pyc
--rw-r--r--   0        0        0     6097 2023-06-22 14:44:44.017011 renku-2.6.0rc1/renku/domain_model/__pycache__/project.cpython-39.pyc
--rw-r--r--   0        0        0    12164 2023-06-22 14:44:41.600998 renku-2.6.0rc1/renku/domain_model/__pycache__/project_context.cpython-39.pyc
--rw-r--r--   0        0        0     7426 2023-06-22 14:44:42.449002 renku-2.6.0rc1/renku/domain_model/__pycache__/session.cpython-39.pyc
--rw-r--r--   0        0        0     1092 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/constant.py
--rw-r--r--   0        0        0    29611 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/dataset.py
--rw-r--r--   0        0        0     1267 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/dataset_provider.py
--rw-r--r--   0        0        0     2754 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/datastructures.py
--rw-r--r--   0        0        0     2499 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/entity.py
--rw-r--r--   0        0        0      971 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/enums.py
--rw-r--r--   0        0        0     5059 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/git.py
--rw-r--r--   0        0        0     8329 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/project.py
--rw-r--r--   0        0        0    11817 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/project_context.py
--rw-r--r--   0        0        0      829 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/provenance/__init__.py
--rw-r--r--   0        0        0      283 2023-06-22 14:44:42.005000 renku-2.6.0rc1/renku/domain_model/provenance/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    11882 2023-06-22 14:44:44.137011 renku-2.6.0rc1/renku/domain_model/provenance/__pycache__/activity.cpython-39.pyc
--rw-r--r--   0        0        0     4946 2023-06-22 14:44:42.005000 renku-2.6.0rc1/renku/domain_model/provenance/__pycache__/agent.cpython-39.pyc
--rw-r--r--   0        0        0     1092 2023-06-22 14:44:42.009000 renku-2.6.0rc1/renku/domain_model/provenance/__pycache__/annotation.cpython-39.pyc
--rw-r--r--   0        0        0     1363 2023-06-22 14:44:44.137011 renku-2.6.0rc1/renku/domain_model/provenance/__pycache__/parameter.cpython-39.pyc
--rw-r--r--   0        0        0    13200 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/provenance/activity.py
--rw-r--r--   0        0        0     5155 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/provenance/agent.py
--rw-r--r--   0        0        0     1268 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/provenance/annotation.py
--rw-r--r--   0        0        0     1530 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/provenance/parameter.py
--rw-r--r--   0        0        0     6871 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/session.py
--rw-r--r--   0        0        0     1471 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/sort.py
--rw-r--r--   0        0        0    27042 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/template.py
--rw-r--r--   0        0        0      782 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/workflow/__init__.py
--rw-r--r--   0        0        0      234 2023-06-22 14:44:43.137006 renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    13527 2023-06-22 14:44:43.657009 renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/composite_plan.cpython-39.pyc
--rw-r--r--   0        0        0    15243 2023-06-22 14:44:43.661008 renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/parameter.cpython-39.pyc
--rw-r--r--   0        0        0    15096 2023-06-22 14:44:43.665009 renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/plan.cpython-39.pyc
--rw-r--r--   0        0        0     1483 2023-06-22 14:44:43.137006 renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/provider.cpython-39.pyc
--rw-r--r--   0        0        0     4523 2023-06-22 14:44:44.141011 renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/workflow_file.cpython-39.pyc
--rw-r--r--   0        0        0    15917 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/workflow/composite_plan.py
--rw-r--r--   0        0        0     1531 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/workflow/converters/__init__.py
--rw-r--r--   0        0        0     1391 2023-06-22 14:44:44.025010 renku-2.6.0rc1/renku/domain_model/workflow/converters/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    18124 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/workflow/parameter.py
--rw-r--r--   0        0        0    16602 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/workflow/plan.py
--rw-r--r--   0        0        0     1639 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/workflow/provider.py
--rw-r--r--   0        0        0     4660 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/workflow/workflow_file.py
--rw-r--r--   0        0        0      780 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/infrastructure/__init__.py
--rw-r--r--   0        0        0      212 2023-06-22 14:44:41.380997 renku-2.6.0rc1/renku/infrastructure/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    34957 2023-06-22 14:44:43.797009 renku-2.6.0rc1/renku/infrastructure/__pycache__/database.cpython-39.pyc
--rw-r--r--   0        0        0     5073 2023-06-22 14:44:41.624998 renku-2.6.0rc1/renku/infrastructure/__pycache__/immutable.cpython-39.pyc
--rw-r--r--   0        0        0     2259 2023-06-22 14:44:41.752998 renku-2.6.0rc1/renku/infrastructure/__pycache__/persistent.cpython-39.pyc
--rw-r--r--   0        0        0    67803 2023-06-22 14:44:41.400997 renku-2.6.0rc1/renku/infrastructure/__pycache__/repository.cpython-39.pyc
--rw-r--r--   0        0        0    41333 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/infrastructure/database.py
--rw-r--r--   0        0        0      786 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/infrastructure/gateway/__init__.py
--rw-r--r--   0        0        0      226 2023-06-22 14:44:42.205001 renku-2.6.0rc1/renku/infrastructure/gateway/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3238 2023-06-22 14:44:42.205001 renku-2.6.0rc1/renku/infrastructure/gateway/__pycache__/dataset_gateway.cpython-39.pyc
--rw-r--r--   0        0        0    12730 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/infrastructure/gateway/activity_gateway.py
--rw-r--r--   0        0        0     5845 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/infrastructure/gateway/database_gateway.py
--rw-r--r--   0        0        0     3743 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/infrastructure/gateway/dataset_gateway.py
--rw-r--r--   0        0        0     3529 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/infrastructure/gateway/plan_gateway.py
--rw-r--r--   0        0        0     1711 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/infrastructure/gateway/project_gateway.py
--rw-r--r--   0        0        0    18006 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/infrastructure/git_merger.py
--rw-r--r--   0        0        0     4969 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/infrastructure/immutable.py
--rw-r--r--   0        0        0     2394 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/infrastructure/persistent.py
--rw-r--r--   0        0        0    72047 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/infrastructure/repository.py
--rw-r--r--   0        0        0      784 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/infrastructure/storage/__init__.py
--rw-r--r--   0        0        0      224 2023-06-22 14:44:42.021000 renku-2.6.0rc1/renku/infrastructure/storage/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1523 2023-06-22 14:44:42.021000 renku-2.6.0rc1/renku/infrastructure/storage/__pycache__/factory.cpython-39.pyc
--rw-r--r--   0        0        0     1989 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/infrastructure/storage/factory.py
--rw-r--r--   0        0        0     8859 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/infrastructure/storage/rclone.py
--rw-r--r--   0        0        0      913 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      553 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      637 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      523 2023-06-22 14:44:46.349023 renku-2.6.0rc1/renku/templates/.github/dependabot.yml
--rw-r--r--   0        0        0      396 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/.github/workflows/github-project.yml
--rw-r--r--   0        0        0     3940 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/.gitignore
--rw-r--r--   0        0        0       27 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/.dockerignore
--rw-r--r--   0        0        0     6018 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/.gitignore
--rw-r--r--   0        0        0      450 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/.gitlab-ci.yml
--rw-r--r--   0        0        0       37 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/.renku/renku.ini
--rw-r--r--   0        0        0      984 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/.renkulfsignore
--rw-r--r--   0        0        0     2087 2023-06-22 14:44:46.349023 renku-2.6.0rc1/renku/templates/R-minimal/Dockerfile
--rw-r--r--   0        0        0     1603 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/README.md
--rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/data/.gitkeep
--rw-r--r--   0        0        0      112 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/environment.yml
--rw-r--r--   0        0        0      360 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/install.R
--rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/notebooks/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/requirements.txt
--rw-r--r--   0        0        0     1439 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/workflows/my-workflow.yaml
--rw-r--r--   0        0        0      205 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/{{ __sanitized_project_name__ }}.Rproj
--rw-r--r--   0        0        0    14286 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal.png
--rw-r--r--   0        0        0     4846 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/README.md
--rw-r--r--   0        0        0       27 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/.dockerignore
--rw-r--r--   0        0        0     6018 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/.gitignore
--rw-r--r--   0        0        0      450 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/.gitlab-ci.yml
--rw-r--r--   0        0        0       37 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/.renku/renku.ini
--rw-r--r--   0        0        0      976 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/.renkulfsignore
--rw-r--r--   0        0        0     2077 2023-06-22 14:44:46.349023 renku-2.6.0rc1/renku/templates/bioc-minimal/Dockerfile
--rw-r--r--   0        0        0     1603 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/README.md
--rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/data/.gitkeep
--rw-r--r--   0        0        0      112 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/environment.yml
--rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/install.R
--rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/notebooks/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/requirements.txt
--rw-r--r--   0        0        0     1439 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/workflows/my-workflow.yaml
--rw-r--r--   0        0        0      205 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/{{ __sanitized_project_name__ }}.Rproj
--rw-r--r--   0        0        0    44589 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioconductor.png
--rw-r--r--   0        0        0       27 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/.dockerignore
--rw-r--r--   0        0        0     6018 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/.gitignore
--rw-r--r--   0        0        0      450 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/.gitlab-ci.yml
--rw-r--r--   0        0        0       50 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/.renku/renku.ini
--rw-r--r--   0        0        0      976 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/.renkulfsignore
--rw-r--r--   0        0        0     2469 2023-06-22 14:44:46.349023 renku-2.6.0rc1/renku/templates/julia-minimal/Dockerfile
--rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/Manifest.toml
--rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/Project.toml
--rw-r--r--   0        0        0     1842 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/README.md
--rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/data/.gitkeep
--rw-r--r--   0        0        0      112 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/environment.yml
--rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/notebooks/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/requirements.txt
--rw-r--r--   0        0        0     1439 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/workflows/my-workflow.yaml
--rw-r--r--   0        0        0    13782 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julialang.png
--rw-r--r--   0        0        0     1174 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/manifest.yaml
--rw-r--r--   0        0        0       17 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/minimal/.dockerignore
--rw-r--r--   0        0        0       77 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/minimal/.gitignore
--rw-r--r--   0        0        0      450 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/minimal/.gitlab-ci.yml
--rw-r--r--   0        0        0       33 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/minimal/.renku/renku.ini
--rw-r--r--   0        0        0      976 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/minimal/.renkulfsignore
--rw-r--r--   0        0        0     2414 2023-06-22 14:44:46.349023 renku-2.6.0rc1/renku/templates/minimal/Dockerfile
--rw-r--r--   0        0        0     1439 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/minimal/workflows/my-workflow.yaml
--rw-r--r--   0        0        0       27 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/python-minimal/.dockerignore
--rw-r--r--   0        0        0     5401 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/python-minimal/.gitignore
--rw-r--r--   0        0        0      450 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/python-minimal/.gitlab-ci.yml
--rw-r--r--   0        0        0       33 2023-06-22 14:44:46.345023 renku-2.6.0rc1/renku/templates/python-minimal/.renku/renku.ini
--rw-r--r--   0        0        0      976 2023-06-22 14:44:46.345023 renku-2.6.0rc1/renku/templates/python-minimal/.renkulfsignore
--rw-r--r--   0        0        0     2159 2023-06-22 14:44:46.349023 renku-2.6.0rc1/renku/templates/python-minimal/Dockerfile
--rw-r--r--   0        0        0     1597 2023-06-22 14:44:46.345023 renku-2.6.0rc1/renku/templates/python-minimal/README.md
--rw-r--r--   0        0        0        0 2023-06-22 14:44:46.345023 renku-2.6.0rc1/renku/templates/python-minimal/data/.gitkeep
--rw-r--r--   0        0        0      112 2023-06-22 14:44:46.345023 renku-2.6.0rc1/renku/templates/python-minimal/environment.yml
--rw-r--r--   0        0        0        0 2023-06-22 14:44:46.345023 renku-2.6.0rc1/renku/templates/python-minimal/notebooks/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-22 14:44:46.345023 renku-2.6.0rc1/renku/templates/python-minimal/requirements.txt
--rw-r--r--   0        0        0     1439 2023-06-22 14:44:46.345023 renku-2.6.0rc1/renku/templates/python-minimal/workflows/my-workflow.yaml
--rw-r--r--   0        0        0    25599 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/python-minimal.png
--rw-r--r--   0        0        0      763 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/__init__.py
--rw-r--r--   0        0        0      184 2023-06-22 14:44:41.212996 renku-2.6.0rc1/renku/ui/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1268 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/api/__init__.py
--rw-r--r--   0        0        0      763 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/api/graph/__init__.py
--rw-r--r--   0        0        0     2519 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/api/graph/rdf.py
--rw-r--r--   0        0        0      764 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/api/models/__init__.py
--rw-r--r--   0        0        0    16448 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/api/models/activity.py
--rw-r--r--   0        0        0     4648 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/api/models/dataset.py
--rw-r--r--   0        0        0    10361 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/api/models/parameter.py
--rw-r--r--   0        0        0     9227 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/api/models/plan.py
--rw-r--r--   0        0        0     3643 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/api/models/project.py
--rw-r--r--   0        0        0     2519 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/api/util.py
--rw-r--r--   0        0        0     9319 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/__init__.py
--rw-r--r--   0        0        0      922 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/__main__.py
--rw-r--r--   0        0        0     8150 2023-06-22 14:44:41.216996 renku-2.6.0rc1/renku/ui/cli/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2117 2023-06-22 14:44:41.600998 renku-2.6.0rc1/renku/ui/cli/__pycache__/clone.cpython-39.pyc
--rw-r--r--   0        0        0     7029 2023-06-22 14:44:41.604998 renku-2.6.0rc1/renku/ui/cli/__pycache__/config.cpython-39.pyc
--rw-r--r--   0        0        0    36275 2023-06-22 14:44:41.612998 renku-2.6.0rc1/renku/ui/cli/__pycache__/dataset.cpython-39.pyc
--rw-r--r--   0        0        0     1787 2023-06-22 14:44:45.157016 renku-2.6.0rc1/renku/ui/cli/__pycache__/doctor.cpython-39.pyc
--rw-r--r--   0        0        0      964 2023-06-22 14:44:45.157016 renku-2.6.0rc1/renku/ui/cli/__pycache__/env.cpython-39.pyc
--rw-r--r--   0        0        0     7957 2023-06-22 14:44:45.161017 renku-2.6.0rc1/renku/ui/cli/__pycache__/exception_handler.cpython-39.pyc
--rw-r--r--   0        0        0      645 2023-06-22 14:44:45.185017 renku-2.6.0rc1/renku/ui/cli/__pycache__/gc.cpython-39.pyc
--rw-r--r--   0        0        0     2168 2023-06-22 14:44:45.185017 renku-2.6.0rc1/renku/ui/cli/__pycache__/githooks.cpython-39.pyc
--rw-r--r--   0        0        0     4041 2023-06-22 14:44:45.185017 renku-2.6.0rc1/renku/ui/cli/__pycache__/graph.cpython-39.pyc
--rw-r--r--   0        0        0     9637 2023-06-22 14:44:45.189017 renku-2.6.0rc1/renku/ui/cli/__pycache__/init.cpython-39.pyc
--rw-r--r--   0        0        0     7264 2023-06-22 14:44:45.189017 renku-2.6.0rc1/renku/ui/cli/__pycache__/log.cpython-39.pyc
--rw-r--r--   0        0        0     4296 2023-06-22 14:44:45.201017 renku-2.6.0rc1/renku/ui/cli/__pycache__/login.cpython-39.pyc
--rw-r--r--   0        0        0     2066 2023-06-22 14:44:45.233017 renku-2.6.0rc1/renku/ui/cli/__pycache__/mergetool.cpython-39.pyc
--rw-r--r--   0        0        0     4585 2023-06-22 14:44:45.233017 renku-2.6.0rc1/renku/ui/cli/__pycache__/migrate.cpython-39.pyc
--rw-r--r--   0        0        0     2306 2023-06-22 14:44:45.233017 renku-2.6.0rc1/renku/ui/cli/__pycache__/move.cpython-39.pyc
--rw-r--r--   0        0        0     4028 2023-06-22 14:44:45.237017 renku-2.6.0rc1/renku/ui/cli/__pycache__/project.cpython-39.pyc
--rw-r--r--   0        0        0     1283 2023-06-22 14:44:45.237017 renku-2.6.0rc1/renku/ui/cli/__pycache__/remove.cpython-39.pyc
--rw-r--r--   0        0        0     3485 2023-06-22 14:44:45.237017 renku-2.6.0rc1/renku/ui/cli/__pycache__/rerun.cpython-39.pyc
--rw-r--r--   0        0        0     2761 2023-06-22 14:44:45.241017 renku-2.6.0rc1/renku/ui/cli/__pycache__/rollback.cpython-39.pyc
--rw-r--r--   0        0        0    23646 2023-06-22 14:44:45.241017 renku-2.6.0rc1/renku/ui/cli/__pycache__/run.cpython-39.pyc
--rw-r--r--   0        0        0     2890 2023-06-22 14:44:45.257017 renku-2.6.0rc1/renku/ui/cli/__pycache__/save.cpython-39.pyc
--rw-r--r--   0        0        0    10362 2023-06-22 14:44:45.261017 renku-2.6.0rc1/renku/ui/cli/__pycache__/service.cpython-39.pyc
--rw-r--r--   0        0        0    13046 2023-06-22 14:44:45.265017 renku-2.6.0rc1/renku/ui/cli/__pycache__/session.cpython-39.pyc
--rw-r--r--   0        0        0     3715 2023-06-22 14:44:45.269017 renku-2.6.0rc1/renku/ui/cli/__pycache__/status.cpython-39.pyc
--rw-r--r--   0        0        0     5061 2023-06-22 14:44:45.273017 renku-2.6.0rc1/renku/ui/cli/__pycache__/storage.cpython-39.pyc
--rw-r--r--   0        0        0    10944 2023-06-22 14:44:45.277017 renku-2.6.0rc1/renku/ui/cli/__pycache__/template.cpython-39.pyc
--rw-r--r--   0        0        0     5790 2023-06-22 14:44:45.277017 renku-2.6.0rc1/renku/ui/cli/__pycache__/update.cpython-39.pyc
--rw-r--r--   0        0        0    41570 2023-06-22 14:44:45.281017 renku-2.6.0rc1/renku/ui/cli/__pycache__/workflow.cpython-39.pyc
--rw-r--r--   0        0        0     2594 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/clone.py
--rw-r--r--   0        0        0     7953 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/config.py
--rw-r--r--   0        0        0    42787 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/dataset.py
--rw-r--r--   0        0        0     2333 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/doctor.py
--rw-r--r--   0        0        0     1587 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/env.py
--rw-r--r--   0        0        0     7931 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/exception_handler.py
--rw-r--r--   0        0        0     1139 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/gc.py
--rw-r--r--   0        0        0     2538 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/githooks.py
--rw-r--r--   0        0        0     4950 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/graph.py
--rw-r--r--   0        0        0    11113 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/init.py
--rw-r--r--   0        0        0     8581 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/log.py
--rw-r--r--   0        0        0     4845 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/login.py
--rw-r--r--   0        0        0     2499 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/mergetool.py
--rw-r--r--   0        0        0     5894 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/migrate.py
--rw-r--r--   0        0        0     2881 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/move.py
--rw-r--r--   0        0        0     5768 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/project.py
--rw-r--r--   0        0        0     1754 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/remove.py
--rw-r--r--   0        0        0     4227 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/rerun.py
--rw-r--r--   0        0        0     3249 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/rollback.py
--rw-r--r--   0        0        0    26417 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/run.py
--rw-r--r--   0        0        0     3510 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/save.py
--rw-r--r--   0        0        0    11927 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/service.py
--rw-r--r--   0        0        0    14738 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/session.py
--rw-r--r--   0        0        0     5489 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/status.py
--rw-r--r--   0        0        0     5604 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/storage.py
--rw-r--r--   0        0        0    13434 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/template.py
--rw-r--r--   0        0        0     6723 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/update.py
--rw-r--r--   0        0        0      760 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/utils/__init__.py
--rw-r--r--   0        0        0      203 2023-06-22 14:44:41.600998 renku-2.6.0rc1/renku/ui/cli/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5720 2023-06-22 14:44:45.201017 renku-2.6.0rc1/renku/ui/cli/utils/__pycache__/callback.cpython-39.pyc
--rw-r--r--   0        0        0     5071 2023-06-22 14:44:41.604998 renku-2.6.0rc1/renku/ui/cli/utils/__pycache__/click.cpython-39.pyc
--rw-r--r--   0        0        0      301 2023-06-22 14:44:41.604998 renku-2.6.0rc1/renku/ui/cli/utils/__pycache__/color.cpython-39.pyc
--rw-r--r--   0        0        0      998 2023-06-22 14:44:45.237017 renku-2.6.0rc1/renku/ui/cli/utils/__pycache__/plugins.cpython-39.pyc
--rw-r--r--   0        0        0     7369 2023-06-22 14:44:45.197017 renku-2.6.0rc1/renku/ui/cli/utils/__pycache__/terminal.cpython-39.pyc
--rw-r--r--   0        0        0     5409 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/utils/callback.py
--rw-r--r--   0        0        0     5473 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/utils/click.py
--rw-r--r--   0        0        0      842 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/utils/color.py
--rw-r--r--   0        0        0    14521 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/utils/curses.py
--rw-r--r--   0        0        0     1375 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/utils/plugins.py
--rw-r--r--   0        0        0     9917 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/utils/terminal.py
--rw-r--r--   0        0        0    47787 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/workflow.py
--rw-r--r--   0        0        0      843 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/.env-example
--rw-r--r--   0        0        0      756 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/__init__.py
--rw-r--r--   0        0        0      189 2023-06-22 14:44:45.161017 renku-2.6.0rc1/renku/ui/service/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2109 2023-06-22 14:44:45.161017 renku-2.6.0rc1/renku/ui/service/__pycache__/config.cpython-39.pyc
--rw-r--r--   0        0        0     1535 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/__init__.py
--rw-r--r--   0        0        0     2917 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/base.py
--rw-r--r--   0        0        0     1168 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/config.py
--rw-r--r--   0        0        0     3315 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/files.py
--rw-r--r--   0        0        0     2333 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/jobs.py
--rw-r--r--   0        0        0      769 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/models/__init__.py
--rw-r--r--   0        0        0     4356 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/models/file.py
--rw-r--r--   0        0        0     2298 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/models/job.py
--rw-r--r--   0        0        0     4043 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/models/project.py
--rw-r--r--   0        0        0     1127 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/models/user.py
--rw-r--r--   0        0        0     2558 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/projects.py
--rw-r--r--   0        0        0      774 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/serializers/__init__.py
--rw-r--r--   0        0        0     1821 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/serializers/file.py
--rw-r--r--   0        0        0     1711 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/serializers/job.py
--rw-r--r--   0        0        0     1812 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/serializers/project.py
--rw-r--r--   0        0        0     1227 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/serializers/user.py
--rw-r--r--   0        0        0     1657 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/users.py
--rw-r--r--   0        0        0     3091 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/config.py
--rw-r--r--   0        0        0      773 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/controllers/__init__.py
--rw-r--r--   0        0        0      777 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/controllers/api/__init__.py
--rw-r--r--   0        0        0     1085 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/controllers/api/abstract.py
--rw-r--r--   0        0        0    15665 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/controllers/api/mixins.py
--rw-r--r--   0        0        0     2647 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/controllers/cache_files_delete_chunks.py
--rw-r--r--   0        0        0     7478 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/controllers/cache_files_upload.py
--rw-r--r--   0        0        0     2239 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/controllers/cache_list_projects.py
--rw-r--r--   0        0        0     1927 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/controllers/cache_list_uploaded.py
--rw-r--r--   0        0        0     4823 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/cache_migrate_project.py
--rw-r--r--   0        0        0     4905 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/cache_migrations_check.py
--rw-r--r--   0        0        0     2350 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/cache_project_clone.py
--rw-r--r--   0        0        0     2649 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/config_set.py
--rw-r--r--   0        0        0     2333 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/config_show.py
--rw-r--r--   0        0        0     5682 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/datasets_add_file.py
--rw-r--r--   0        0        0     3916 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/datasets_create.py
--rw-r--r--   0        0        0     5359 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/datasets_edit.py
--rw-r--r--   0        0        0     2132 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/datasets_files_list.py
--rw-r--r--   0        0        0     3333 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/datasets_import.py
--rw-r--r--   0        0        0     2065 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/datasets_list.py
--rw-r--r--   0        0        0     2637 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/datasets_remove.py
--rw-r--r--   0        0        0     3290 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/datasets_unlink.py
--rw-r--r--   0        0        0     5370 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/graph_export.py
--rw-r--r--   0        0        0     3936 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/project_edit.py
--rw-r--r--   0        0        0     3180 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/project_lock_status.py
--rw-r--r--   0        0        0     2096 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/project_show.py
--rw-r--r--   0        0        0     8049 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/templates_create_project.py
--rw-r--r--   0        0        0     3103 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/templates_read_manifest.py
--rw-r--r--   0        0        0      773 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/utils/__init__.py
--rw-r--r--   0        0        0     1083 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/utils/datasets.py
--rw-r--r--   0        0        0     3233 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/utils/project_clone.py
--rw-r--r--   0        0        0     2664 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/utils/remote_project.py
--rw-r--r--   0        0        0     1641 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/version.py
--rw-r--r--   0        0        0     1389 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/versions_list.py
--rw-r--r--   0        0        0     2441 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/workflow_plans_export.py
--rw-r--r--   0        0        0     2257 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/workflow_plans_list.py
--rw-r--r--   0        0        0     2146 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/workflow_plans_show.py
--rw-r--r--   0        0        0     6275 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/entrypoint.py
--rw-r--r--   0        0        0    32144 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/errors.py
--rw-r--r--   0        0        0      774 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/gateways/__init__.py
--rw-r--r--   0        0        0     4083 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/gateways/gitlab_api_provider.py
--rw-r--r--   0        0        0      793 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/interfaces/__init__.py
--rw-r--r--   0        0        0     1272 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/interfaces/git_api_provider.py
--rw-r--r--   0        0        0      766 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/jobs/__init__.py
--rw-r--r--   0        0        0     3035 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/jobs/cleanup.py
--rw-r--r--   0        0        0      756 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/jobs/constants.py
--rw-r--r--   0        0        0     1186 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/jobs/contexts.py
--rw-r--r--   0        0        0     5288 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/jobs/datasets.py
--rw-r--r--   0        0        0     1829 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/jobs/delayed_ctrl.py
--rw-r--r--   0        0        0     2665 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/jobs/queues.py
--rw-r--r--   0        0        0     1269 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/logger.py
--rw-r--r--   0        0        0      644 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/logging.yaml
--rw-r--r--   0        0        0     2742 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/scheduler.py
--rw-r--r--   0        0        0      768 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/__init__.py
--rw-r--r--   0        0        0    14561 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/cache.py
--rw-r--r--   0        0        0     4843 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/common.py
--rw-r--r--   0        0        0     2228 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/config.py
--rw-r--r--   0        0        0     8503 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/datasets.py
--rw-r--r--   0        0        0     2195 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/graph.py
--rw-r--r--   0        0        0     5362 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/headers.py
--rw-r--r--   0        0        0     1961 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/jobs.py
--rw-r--r--   0        0        0     4510 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/project.py
--rw-r--r--   0        0        0      911 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/rpc.py
--rw-r--r--   0        0        0     5815 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/templates.py
--rw-r--r--   0        0        0      773 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/v1/__init__.py
--rw-r--r--   0        0        0     4212 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/v1/cache.py
--rw-r--r--   0        0        0     1880 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/v1/templates.py
--rw-r--r--   0        0        0     1171 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/version.py
--rw-r--r--   0        0        0     1365 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/versions_list.py
--rw-r--r--   0        0        0     6907 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/workflows.py
--rw-r--r--   0        0        0     2186 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/utils/__init__.py
--rw-r--r--   0        0        0     2220 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/utils/callback.py
--rw-r--r--   0        0        0     1323 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/utils/json_encoder.py
--rw-r--r--   0        0        0     1260 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/utils/squash.py
--rw-r--r--   0        0        0     1427 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/utils/timeout.py
--rw-r--r--   0        0        0     1761 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/__init__.py
--rw-r--r--   0        0        0     2438 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/api_versions.py
--rw-r--r--   0        0        0     4767 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/apispec.py
--rw-r--r--   0        0        0     7427 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/cache.py
--rw-r--r--   0        0        0     2957 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/config.py
--rw-r--r--   0        0        0     8187 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/datasets.py
--rw-r--r--   0        0        0     2961 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/decorators.py
--rw-r--r--   0        0        0    15114 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/error_handlers.py
--rw-r--r--   0        0        0     2084 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/graph.py
--rw-r--r--   0        0        0     3267 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/jobs.py
--rw-r--r--   0        0        0     3805 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/project.py
--rw-r--r--   0        0        0     3592 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/templates.py
--rw-r--r--   0        0        0      767 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/v1/__init__.py
--rw-r--r--   0        0        0     4775 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/v1/cache.py
--rw-r--r--   0        0        0     2634 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/v1/templates.py
--rw-r--r--   0        0        0     1702 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/version.py
--rw-r--r--   0        0        0     1676 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/versions_list.py
--rw-r--r--   0        0        0     3873 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/workflow_plans.py
--rw-r--r--   0        0        0     2890 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/worker.py
--rw-r--r--   0        0        0     1614 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/version.py
--rw-r--r--   0        0        0    17131 1970-01-01 00:00:00.000000 renku-2.6.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      900 2023-07-13 15:43:27.146978 renku-2.6.1rc1/AUTHORS.rst
+-rw-r--r--   0        0        0   182553 2023-07-13 15:43:27.150978 renku-2.6.1rc1/CHANGES.rst
+-rw-r--r--   0        0        0    11358 2023-07-13 15:43:27.150978 renku-2.6.1rc1/LICENSE
+-rw-r--r--   0        0        0    12889 2023-07-13 15:43:27.150978 renku-2.6.1rc1/README.rst
+-rw-r--r--   0        0        0    10498 2023-07-13 15:44:55.657385 renku-2.6.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     4391 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/__init__.py
+-rw-r--r--   0        0        0      784 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/__init__.py
+-rw-r--r--   0        0        0      209 2023-07-13 15:44:49.645221 renku-2.6.1rc1/renku/command/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      437 2023-07-13 15:44:49.645221 renku-2.6.1rc1/renku/command/__pycache__/options.cpython-39.pyc
+-rw-r--r--   0        0        0     1057 2023-07-13 15:44:53.981339 renku-2.6.1rc1/renku/command/__pycache__/run.cpython-39.pyc
+-rw-r--r--   0        0        0     1343 2023-07-13 15:44:49.645221 renku-2.6.1rc1/renku/command/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0      593 2023-07-13 15:44:49.645221 renku-2.6.1rc1/renku/command/__pycache__/version.cpython-39.pyc
+-rw-r--r--   0        0        0     2096 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/checks/__init__.py
+-rw-r--r--   0        0        0     4808 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/checks/activities.py
+-rw-r--r--   0        0        0     8408 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/checks/datasets.py
+-rw-r--r--   0        0        0     2797 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/checks/githooks.py
+-rw-r--r--   0        0        0     1548 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/checks/migration.py
+-rw-r--r--   0        0        0     2448 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/checks/project.py
+-rw-r--r--   0        0        0     1572 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/checks/storage.py
+-rw-r--r--   0        0        0     4124 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/checks/validate_shacl.py
+-rw-r--r--   0        0        0     5025 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/checks/workflow.py
+-rw-r--r--   0        0        0     3872 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/clone.py
+-rw-r--r--   0        0        0      828 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/command_builder/__init__.py
+-rw-r--r--   0        0        0      301 2023-07-13 15:44:50.361240 renku-2.6.1rc1/renku/command/command_builder/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    15431 2023-07-13 15:44:50.365240 renku-2.6.1rc1/renku/command/command_builder/__pycache__/command.cpython-39.pyc
+-rw-r--r--   0        0        0    16678 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/command_builder/command.py
+-rw-r--r--   0        0        0     1951 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/command_builder/communication.py
+-rw-r--r--   0        0        0     5325 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/command_builder/database.py
+-rw-r--r--   0        0        0     1701 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/command_builder/lock.py
+-rw-r--r--   0        0        0     1481 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/command_builder/migration.py
+-rw-r--r--   0        0        0     7694 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/command_builder/repo.py
+-rw-r--r--   0        0        0     4803 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/config.py
+-rw-r--r--   0        0        0     5640 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/dataset.py
+-rw-r--r--   0        0        0     2835 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/doctor.py
+-rw-r--r--   0        0        0      775 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/format/__init__.py
+-rw-r--r--   0        0        0      220 2023-07-13 15:44:49.905228 renku-2.6.1rc1/renku/command/format/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5765 2023-07-13 15:44:49.909228 renku-2.6.1rc1/renku/command/format/__pycache__/dataset_files.cpython-39.pyc
+-rw-r--r--   0        0        0     1508 2023-07-13 15:44:49.909228 renku-2.6.1rc1/renku/command/format/__pycache__/dataset_tags.cpython-39.pyc
+-rw-r--r--   0        0        0     2884 2023-07-13 15:44:49.909228 renku-2.6.1rc1/renku/command/format/__pycache__/datasets.cpython-39.pyc
+-rw-r--r--   0        0        0      817 2023-07-13 15:44:52.605301 renku-2.6.1rc1/renku/command/format/__pycache__/json.cpython-39.pyc
+-rw-r--r--   0        0        0     1754 2023-07-13 15:44:54.001340 renku-2.6.1rc1/renku/command/format/__pycache__/session.cpython-39.pyc
+-rw-r--r--   0        0        0     1929 2023-07-13 15:44:52.605301 renku-2.6.1rc1/renku/command/format/__pycache__/tabulate.cpython-39.pyc
+-rw-r--r--   0        0        0     2416 2023-07-13 15:44:52.605301 renku-2.6.1rc1/renku/command/format/__pycache__/workflow.cpython-39.pyc
+-rw-r--r--   0        0        0     2643 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/format/activity.py
+-rw-r--r--   0        0        0     6230 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/format/dataset_files.py
+-rw-r--r--   0        0        0     2098 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/format/dataset_tags.py
+-rw-r--r--   0        0        0     3236 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/format/datasets.py
+-rw-r--r--   0        0        0     1212 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/format/json.py
+-rw-r--r--   0        0        0     2402 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/format/session.py
+-rw-r--r--   0        0        0     2769 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/format/tabulate.py
+-rw-r--r--   0        0        0     2728 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/format/workflow.py
+-rw-r--r--   0        0        0     1012 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/gc.py
+-rw-r--r--   0        0        0     1154 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/githooks.py
+-rw-r--r--   0        0        0     9880 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/graph.py
+-rw-r--r--   0        0        0     1081 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/group.py
+-rw-r--r--   0        0        0     1203 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/init.py
+-rw-r--r--   0        0        0     3124 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/log.py
+-rw-r--r--   0        0        0     1241 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/login.py
+-rw-r--r--   0        0        0     2822 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/mergetool.py
+-rw-r--r--   0        0        0    10732 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/migrate.py
+-rw-r--r--   0        0        0     9141 2023-07-13 15:43:27.214980 renku-2.6.1rc1/renku/command/move.py
+-rw-r--r--   0        0        0     1015 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/options.py
+-rw-r--r--   0        0        0     1362 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/project.py
+-rw-r--r--   0        0        0     4748 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/remove.py
+-rw-r--r--   0        0        0     3146 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/rerun.py
+-rw-r--r--   0        0        0    10987 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/rollback.py
+-rw-r--r--   0        0        0     1600 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/run.py
+-rw-r--r--   0        0        0     3375 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/save.py
+-rw-r--r--   0        0        0      766 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/schema/__init__.py
+-rw-r--r--   0        0        0      211 2023-07-13 15:44:50.105234 renku-2.6.1rc1/renku/command/schema/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2040 2023-07-13 15:44:50.105234 renku-2.6.1rc1/renku/command/schema/__pycache__/agent.cpython-39.pyc
+-rw-r--r--   0        0        0      977 2023-07-13 15:44:50.305239 renku-2.6.1rc1/renku/command/schema/__pycache__/annotation.cpython-39.pyc
+-rw-r--r--   0        0        0     6652 2023-07-13 15:44:50.297239 renku-2.6.1rc1/renku/command/schema/__pycache__/calamus.cpython-39.pyc
+-rw-r--r--   0        0        0     7584 2023-07-13 15:44:50.105234 renku-2.6.1rc1/renku/command/schema/__pycache__/dataset.cpython-39.pyc
+-rw-r--r--   0        0        0     1345 2023-07-13 15:44:50.309239 renku-2.6.1rc1/renku/command/schema/__pycache__/entity.cpython-39.pyc
+-rw-r--r--   0        0        0     5615 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/schema/activity.py
+-rw-r--r--   0        0        0     2478 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/schema/agent.py
+-rw-r--r--   0        0        0     1235 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/schema/annotation.py
+-rw-r--r--   0        0        0     8986 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/schema/calamus.py
+-rw-r--r--   0        0        0     3186 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/schema/composite_plan.py
+-rw-r--r--   0        0        0     8210 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/schema/dataset.py
+-rw-r--r--   0        0        0     1445 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/schema/entity.py
+-rw-r--r--   0        0        0     4016 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/schema/parameter.py
+-rw-r--r--   0        0        0     3427 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/schema/plan.py
+-rw-r--r--   0        0        0     3406 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/schema/project.py
+-rw-r--r--   0        0        0     3065 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/schema/workflow_file.py
+-rw-r--r--   0        0        0     2039 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/session.py
+-rw-r--r--   0        0        0     1036 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/status.py
+-rw-r--r--   0        0        0     3944 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/storage.py
+-rw-r--r--   0        0        0     1919 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/template.py
+-rw-r--r--   0        0        0     1254 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/update.py
+-rw-r--r--   0        0        0     1726 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/util.py
+-rw-r--r--   0        0        0     1088 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/version.py
+-rw-r--r--   0        0        0      768 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/view_model/__init__.py
+-rw-r--r--   0        0        0      217 2023-07-13 15:44:50.509244 renku-2.6.1rc1/renku/command/view_model/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    13290 2023-07-13 15:44:52.609301 renku-2.6.1rc1/renku/command/view_model/__pycache__/activity_graph.cpython-39.pyc
+-rw-r--r--   0        0        0     1350 2023-07-13 15:44:52.649303 renku-2.6.1rc1/renku/command/view_model/__pycache__/agent.cpython-39.pyc
+-rw-r--r--   0        0        0     8157 2023-07-13 15:44:52.649303 renku-2.6.1rc1/renku/command/view_model/__pycache__/composite_plan.cpython-39.pyc
+-rw-r--r--   0        0        0     1848 2023-07-13 15:44:50.509244 renku-2.6.1rc1/renku/command/view_model/__pycache__/dataset.cpython-39.pyc
+-rw-r--r--   0        0        0    11145 2023-07-13 15:44:53.933338 renku-2.6.1rc1/renku/command/view_model/__pycache__/log.cpython-39.pyc
+-rw-r--r--   0        0        0     7823 2023-07-13 15:44:52.645302 renku-2.6.1rc1/renku/command/view_model/__pycache__/plan.cpython-39.pyc
+-rw-r--r--   0        0        0    14258 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/view_model/activity_graph.py
+-rw-r--r--   0        0        0     1657 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/view_model/agent.py
+-rw-r--r--   0        0        0     8768 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/view_model/composite_plan.py
+-rw-r--r--   0        0        0     2138 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/view_model/dataset.py
+-rw-r--r--   0        0        0     7850 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/view_model/graph.py
+-rw-r--r--   0        0        0    12497 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/view_model/log.py
+-rw-r--r--   0        0        0     9377 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/view_model/plan.py
+-rw-r--r--   0        0        0     3306 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/view_model/project.py
+-rw-r--r--   0        0        0     5947 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/view_model/template.py
+-rw-r--r--   0        0        0    15885 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/view_model/text_canvas.py
+-rw-r--r--   0        0        0     4792 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/view_model/workflow_file.py
+-rw-r--r--   0        0        0     4114 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/command/workflow.py
+-rw-r--r--   0        0        0      745 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/core/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-13 15:44:49.645221 renku-2.6.1rc1/renku/core/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4501 2023-07-13 15:44:49.933229 renku-2.6.1rc1/renku/core/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0        0        0     1707 2023-07-13 15:44:49.657221 renku-2.6.1rc1/renku/core/__pycache__/constant.cpython-39.pyc
+-rw-r--r--   0        0        0    34603 2023-07-13 15:44:49.653221 renku-2.6.1rc1/renku/core/__pycache__/errors.cpython-39.pyc
+-rw-r--r--   0        0        0     4854 2023-07-13 15:44:52.653303 renku-2.6.1rc1/renku/core/__pycache__/git.cpython-39.pyc
+-rw-r--r--   0        0        0     8039 2023-07-13 15:44:50.373241 renku-2.6.1rc1/renku/core/__pycache__/login.cpython-39.pyc
+-rw-r--r--   0        0        0    14579 2023-07-13 15:44:50.337240 renku-2.6.1rc1/renku/core/__pycache__/storage.cpython-39.pyc
+-rw-r--r--   0        0        0     6170 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/core/config.py
+-rw-r--r--   0        0        0     2717 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/core/constant.py
+-rw-r--r--   0        0        0      765 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/core/dataset/__init__.py
+-rw-r--r--   0        0        0      208 2023-07-13 15:44:49.913228 renku-2.6.1rc1/renku/core/dataset/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2042 2023-07-13 15:44:50.481244 renku-2.6.1rc1/renku/core/dataset/__pycache__/context.cpython-39.pyc
+-rw-r--r--   0        0        0    38317 2023-07-13 15:44:50.489244 renku-2.6.1rc1/renku/core/dataset/__pycache__/dataset.cpython-39.pyc
+-rw-r--r--   0        0        0    15656 2023-07-13 15:44:50.481244 renku-2.6.1rc1/renku/core/dataset/__pycache__/dataset_add.cpython-39.pyc
+-rw-r--r--   0        0        0     7431 2023-07-13 15:44:50.361240 renku-2.6.1rc1/renku/core/dataset/__pycache__/datasets_provenance.cpython-39.pyc
+-rw-r--r--   0        0        0     3355 2023-07-13 15:44:50.329239 renku-2.6.1rc1/renku/core/dataset/__pycache__/pointer_file.cpython-39.pyc
+-rw-r--r--   0        0        0     2737 2023-07-13 15:44:50.513244 renku-2.6.1rc1/renku/core/dataset/__pycache__/request_model.cpython-39.pyc
+-rw-r--r--   0        0        0     5280 2023-07-13 15:44:50.577246 renku-2.6.1rc1/renku/core/dataset/__pycache__/tag.cpython-39.pyc
+-rw-r--r--   0        0        0     2954 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/core/dataset/context.py
+-rw-r--r--   0        0        0    50044 2023-07-13 15:43:27.218980 renku-2.6.1rc1/renku/core/dataset/dataset.py
+-rw-r--r--   0        0        0    21429 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/dataset_add.py
+-rw-r--r--   0        0        0     9747 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/datasets_provenance.py
+-rw-r--r--   0        0        0     4296 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/pointer_file.py
+-rw-r--r--   0        0        0      760 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/providers/__init__.py
+-rw-r--r--   0        0        0      213 2023-07-13 15:44:49.913228 renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    18159 2023-07-13 15:44:49.917228 renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/api.cpython-39.pyc
+-rw-r--r--   0        0        0     6734 2023-07-13 15:44:50.089233 renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/azure.cpython-39.pyc
+-rw-r--r--   0        0        0     1646 2023-07-13 15:44:50.089233 renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0        0        0    19710 2023-07-13 15:44:50.325239 renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/dataverse.cpython-39.pyc
+-rw-r--r--   0        0        0     3221 2023-07-13 15:44:50.325239 renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/dataverse_metadata_templates.cpython-39.pyc
+-rw-r--r--   0        0        0     5087 2023-07-13 15:44:50.325239 renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/doi.cpython-39.pyc
+-rw-r--r--   0        0        0     5963 2023-07-13 15:44:50.329239 renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/external.cpython-39.pyc
+-rw-r--r--   0        0        0     5562 2023-07-13 15:44:49.913228 renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/factory.cpython-39.pyc
+-rw-r--r--   0        0        0     7710 2023-07-13 15:44:50.329239 renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/git.cpython-39.pyc
+-rw-r--r--   0        0        0    10821 2023-07-13 15:44:50.353240 renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/local.cpython-39.pyc
+-rw-r--r--   0        0        0     6644 2023-07-13 15:44:50.093233 renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0        0        0     9573 2023-07-13 15:44:50.353240 renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/olos.cpython-39.pyc
+-rw-r--r--   0        0        0    17180 2023-07-13 15:44:50.361240 renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/renku.cpython-39.pyc
+-rw-r--r--   0        0        0     2538 2023-07-13 15:44:50.325239 renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/repository.cpython-39.pyc
+-rw-r--r--   0        0        0     6260 2023-07-13 15:44:50.473243 renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/s3.cpython-39.pyc
+-rw-r--r--   0        0        0     7131 2023-07-13 15:44:50.473243 renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/web.cpython-39.pyc
+-rw-r--r--   0        0        0    18001 2023-07-13 15:44:50.621247 renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/zenodo.cpython-39.pyc
+-rw-r--r--   0        0        0    16174 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/providers/api.py
+-rw-r--r--   0        0        0     6987 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/providers/azure.py
+-rw-r--r--   0        0        0     2225 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/providers/common.py
+-rw-r--r--   0        0        0    21202 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/providers/dataverse.py
+-rw-r--r--   0        0        0     3742 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/providers/dataverse_metadata_templates.py
+-rw-r--r--   0        0        0     4829 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/providers/doi.py
+-rw-r--r--   0        0        0     5623 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/providers/external.py
+-rw-r--r--   0        0        0     5764 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/providers/factory.py
+-rw-r--r--   0        0        0    10563 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/providers/git.py
+-rw-r--r--   0        0        0    14308 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/providers/local.py
+-rw-r--r--   0        0        0     6292 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/providers/models.py
+-rw-r--r--   0        0        0    10118 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/providers/olos.py
+-rw-r--r--   0        0        0    22167 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/providers/renku.py
+-rw-r--r--   0        0        0     2553 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/providers/repository.py
+-rw-r--r--   0        0        0     6413 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/providers/s3.py
+-rw-r--r--   0        0        0     9427 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/providers/web.py
+-rw-r--r--   0        0        0    18757 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/providers/zenodo.py
+-rw-r--r--   0        0        0     3973 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/request_model.py
+-rw-r--r--   0        0        0     5361 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/dataset/tag.py
+-rw-r--r--   0        0        0    25658 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/errors.py
+-rw-r--r--   0        0        0     1115 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/gc.py
+-rw-r--r--   0        0        0     7394 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/git.py
+-rw-r--r--   0        0        0     2151 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/githooks.py
+-rw-r--r--   0        0        0    16526 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/init.py
+-rw-r--r--   0        0        0      775 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/interface/__init__.py
+-rw-r--r--   0        0        0      207 2023-07-13 15:44:50.317239 renku-2.6.1rc1/renku/core/interface/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4269 2023-07-13 15:44:52.609301 renku-2.6.1rc1/renku/core/interface/__pycache__/activity_gateway.cpython-39.pyc
+-rw-r--r--   0        0        0     1246 2023-07-13 15:44:52.653303 renku-2.6.1rc1/renku/core/interface/__pycache__/database_gateway.cpython-39.pyc
+-rw-r--r--   0        0        0     2159 2023-07-13 15:44:50.373241 renku-2.6.1rc1/renku/core/interface/__pycache__/dataset_gateway.cpython-39.pyc
+-rw-r--r--   0        0        0     2057 2023-07-13 15:44:52.597301 renku-2.6.1rc1/renku/core/interface/__pycache__/plan_gateway.cpython-39.pyc
+-rw-r--r--   0        0        0      959 2023-07-13 15:44:52.597301 renku-2.6.1rc1/renku/core/interface/__pycache__/project_gateway.cpython-39.pyc
+-rw-r--r--   0        0        0     4402 2023-07-13 15:44:50.317239 renku-2.6.1rc1/renku/core/interface/__pycache__/storage.cpython-39.pyc
+-rw-r--r--   0        0        0     1579 2023-07-13 15:44:52.501299 renku-2.6.1rc1/renku/core/interface/__pycache__/workflow_file_parser.cpython-39.pyc
+-rw-r--r--   0        0        0     3741 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/interface/activity_gateway.py
+-rw-r--r--   0        0        0     1418 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/interface/database_gateway.py
+-rw-r--r--   0        0        0     2095 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/interface/dataset_gateway.py
+-rw-r--r--   0        0        0     1996 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/interface/plan_gateway.py
+-rw-r--r--   0        0        0     1212 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/interface/project_gateway.py
+-rw-r--r--   0        0        0     4226 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/interface/storage.py
+-rw-r--r--   0        0        0     1780 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/interface/workflow_file_parser.py
+-rw-r--r--   0        0        0    10639 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/login.py
+-rw-r--r--   0        0        0      764 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/migration/__init__.py
+-rw-r--r--   0        0        0      196 2023-07-13 15:44:50.025231 renku-2.6.1rc1/renku/core/migration/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1122 2023-07-13 15:43:27.222980 renku-2.6.1rc1/renku/core/migration/m_0003__0_pyld2.py
+-rw-r--r--   0        0        0    15324 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/m_0003__1_jsonld.py
+-rw-r--r--   0        0        0     9570 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/m_0003__2_initial.py
+-rw-r--r--   0        0        0     1122 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/m_0004__0_pyld2.py
+-rw-r--r--   0        0        0     5318 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/m_0004__submodules.py
+-rw-r--r--   0        0        0     1548 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/m_0005__1_pyld2.py
+-rw-r--r--   0        0        0    16075 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/m_0005__2_cwl.py
+-rw-r--r--   0        0        0     1015 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/m_0006__dataset_context.py
+-rw-r--r--   0        0        0     1430 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/m_0007__source_url.py
+-rw-r--r--   0        0        0     1175 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/m_0008__dataset_metadata.py
+-rw-r--r--   0        0        0    30683 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/m_0009__new_metadata_storage.py
+-rw-r--r--   0        0        0    14077 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/m_0010__metadata_fixes.py
+-rw-r--r--   0        0        0    10163 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/migrate.py
+-rw-r--r--   0        0        0      770 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/models/__init__.py
+-rw-r--r--   0        0        0     5830 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/models/migration.py
+-rw-r--r--   0        0        0     3861 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/models/refs.py
+-rw-r--r--   0        0        0     5091 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/models/v10.py
+-rw-r--r--   0        0        0    11828 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/models/v3.py
+-rw-r--r--   0        0        0     2422 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/models/v7.py
+-rw-r--r--   0        0        0     4587 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/models/v8.py
+-rw-r--r--   0        0        0    74094 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/models/v9.py
+-rw-r--r--   0        0        0     7945 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/utils/__init__.py
+-rw-r--r--   0        0        0     6660 2023-07-13 15:44:50.029231 renku-2.6.1rc1/renku/core/migration/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     8121 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/migration/utils/conversion.py
+-rw-r--r--   0        0        0      824 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/plugin/__init__.py
+-rw-r--r--   0        0        0      265 2023-07-13 15:44:49.917228 renku-2.6.1rc1/renku/core/plugin/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1033 2023-07-13 15:44:50.085233 renku-2.6.1rc1/renku/core/plugin/__pycache__/dataset_provider.cpython-39.pyc
+-rw-r--r--   0        0        0     1049 2023-07-13 15:44:50.089233 renku-2.6.1rc1/renku/core/plugin/__pycache__/pluginmanager.cpython-39.pyc
+-rw-r--r--   0        0        0     3246 2023-07-13 15:44:51.625275 renku-2.6.1rc1/renku/core/plugin/__pycache__/provider.cpython-39.pyc
+-rw-r--r--   0        0        0     1467 2023-07-13 15:44:53.821334 renku-2.6.1rc1/renku/core/plugin/__pycache__/run.cpython-39.pyc
+-rw-r--r--   0        0        0     1170 2023-07-13 15:44:54.001340 renku-2.6.1rc1/renku/core/plugin/__pycache__/session.cpython-39.pyc
+-rw-r--r--   0        0        0     4177 2023-07-13 15:44:53.185317 renku-2.6.1rc1/renku/core/plugin/__pycache__/workflow.cpython-39.pyc
+-rw-r--r--   0        0        0     2978 2023-07-13 15:44:52.617302 renku-2.6.1rc1/renku/core/plugin/__pycache__/workflow_file_parser.cpython-39.pyc
+-rw-r--r--   0        0        0     1467 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/plugin/dataset_provider.py
+-rw-r--r--   0        0        0     3046 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/plugin/implementations/__init__.py
+-rw-r--r--   0        0        0     2540 2023-07-13 15:44:50.089233 renku-2.6.1rc1/renku/core/plugin/implementations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1790 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/plugin/pluginmanager.py
+-rw-r--r--   0        0        0     3357 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/plugin/provider.py
+-rw-r--r--   0        0        0     1839 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/plugin/run.py
+-rw-r--r--   0        0        0     1515 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/plugin/session.py
+-rw-r--r--   0        0        0     4195 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/plugin/workflow.py
+-rw-r--r--   0        0        0     3065 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/plugin/workflow_file_parser.py
+-rw-r--r--   0        0        0     3355 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/project.py
+-rw-r--r--   0        0        0      770 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/session/__init__.py
+-rw-r--r--   0        0        0      210 2023-07-13 15:44:50.621247 renku-2.6.1rc1/renku/core/session/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    16099 2023-07-13 15:44:50.625248 renku-2.6.1rc1/renku/core/session/__pycache__/docker.cpython-39.pyc
+-rw-r--r--   0        0        0    16431 2023-07-13 15:44:50.825253 renku-2.6.1rc1/renku/core/session/__pycache__/renkulab.cpython-39.pyc
+-rw-r--r--   0        0        0     1449 2023-07-13 15:44:50.881255 renku-2.6.1rc1/renku/core/session/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0        0        0    22065 2023-07-13 15:43:27.226980 renku-2.6.1rc1/renku/core/session/docker.py
+-rw-r--r--   0        0        0    21512 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/session/renkulab.py
+-rw-r--r--   0        0        0    13503 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/session/session.py
+-rw-r--r--   0        0        0     2206 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/session/utils.py
+-rw-r--r--   0        0        0    19478 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/storage.py
+-rw-r--r--   0        0        0      760 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/template/__init__.py
+-rw-r--r--   0        0        0    22043 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/template/template.py
+-rw-r--r--   0        0        0    14612 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/template/usecase.py
+-rw-r--r--   0        0        0      756 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/util/__init__.py
+-rw-r--r--   0        0        0      196 2023-07-13 15:44:49.657221 renku-2.6.1rc1/renku/core/util/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    11124 2023-07-13 15:44:49.929229 renku-2.6.1rc1/renku/core/util/__pycache__/communication.cpython-39.pyc
+-rw-r--r--   0        0        0     6320 2023-07-13 15:44:52.653303 renku-2.6.1rc1/renku/core/util/__pycache__/contexts.cpython-39.pyc
+-rw-r--r--   0        0        0     1801 2023-07-13 15:44:50.025231 renku-2.6.1rc1/renku/core/util/__pycache__/datetime8601.cpython-39.pyc
+-rw-r--r--   0        0        0      933 2023-07-13 15:44:50.085233 renku-2.6.1rc1/renku/core/util/__pycache__/doi.cpython-39.pyc
+-rw-r--r--   0        0        0    33652 2023-07-13 15:44:49.665222 renku-2.6.1rc1/renku/core/util/__pycache__/git.cpython-39.pyc
+-rw-r--r--   0        0        0      669 2023-07-13 15:44:50.881255 renku-2.6.1rc1/renku/core/util/__pycache__/jwt.cpython-39.pyc
+-rw-r--r--   0        0        0     6008 2023-07-13 15:44:50.025231 renku-2.6.1rc1/renku/core/util/__pycache__/metadata.cpython-39.pyc
+-rw-r--r--   0        0        0    11013 2023-07-13 15:44:49.881227 renku-2.6.1rc1/renku/core/util/__pycache__/os.cpython-39.pyc
+-rw-r--r--   0        0        0     6893 2023-07-13 15:44:50.617247 renku-2.6.1rc1/renku/core/util/__pycache__/requests.cpython-39.pyc
+-rw-r--r--   0        0        0     5971 2023-07-13 15:44:50.965257 renku-2.6.1rc1/renku/core/util/__pycache__/ssh.cpython-39.pyc
+-rw-r--r--   0        0        0     1736 2023-07-13 15:44:50.581246 renku-2.6.1rc1/renku/core/util/__pycache__/tabulate.cpython-39.pyc
+-rw-r--r--   0        0        0     4943 2023-07-13 15:44:49.929229 renku-2.6.1rc1/renku/core/util/__pycache__/urls.cpython-39.pyc
+-rw-r--r--   0        0        0     3737 2023-07-13 15:44:50.581246 renku-2.6.1rc1/renku/core/util/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0     2663 2023-07-13 15:44:50.029231 renku-2.6.1rc1/renku/core/util/__pycache__/yaml.cpython-39.pyc
+-rw-r--r--   0        0        0    10282 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/util/communication.py
+-rw-r--r--   0        0        0     6617 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/util/contexts.py
+-rw-r--r--   0        0        0     2313 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/util/datetime8601.py
+-rw-r--r--   0        0        0     1376 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/util/doi.py
+-rw-r--r--   0        0        0    40689 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/util/git.py
+-rw-r--r--   0        0        0     1244 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/util/jwt.py
+-rw-r--r--   0        0        0     7036 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/util/metadata.py
+-rw-r--r--   0        0        0    12140 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/util/os.py
+-rw-r--r--   0        0        0     7626 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/util/requests.py
+-rw-r--r--   0        0        0     1611 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/util/shacl.py
+-rw-r--r--   0        0        0     6871 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/util/ssh.py
+-rw-r--r--   0        0        0     2158 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/util/tabulate.py
+-rw-r--r--   0        0        0     6228 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/util/urls.py
+-rw-r--r--   0        0        0     3878 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/util/util.py
+-rw-r--r--   0        0        0     2836 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/util/yaml.py
+-rw-r--r--   0        0        0      773 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/workflow/__init__.py
+-rw-r--r--   0        0        0      204 2023-07-13 15:44:50.965257 renku-2.6.1rc1/renku/core/workflow/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    18165 2023-07-13 15:44:52.657303 renku-2.6.1rc1/renku/core/workflow/__pycache__/activity.cpython-39.pyc
+-rw-r--r--   0        0        0    14583 2023-07-13 15:44:53.985339 renku-2.6.1rc1/renku/core/workflow/__pycache__/execute.cpython-39.pyc
+-rw-r--r--   0        0        0    26495 2023-07-13 15:44:52.605301 renku-2.6.1rc1/renku/core/workflow/__pycache__/plan.cpython-39.pyc
+-rw-r--r--   0        0        0    23623 2023-07-13 15:44:52.669303 renku-2.6.1rc1/renku/core/workflow/__pycache__/plan_factory.cpython-39.pyc
+-rw-r--r--   0        0        0    10263 2023-07-13 15:44:52.645302 renku-2.6.1rc1/renku/core/workflow/__pycache__/run.cpython-39.pyc
+-rw-r--r--   0        0        0     1660 2023-07-13 15:44:52.669303 renku-2.6.1rc1/renku/core/workflow/__pycache__/types.cpython-39.pyc
+-rw-r--r--   0        0        0     8676 2023-07-13 15:44:52.621302 renku-2.6.1rc1/renku/core/workflow/__pycache__/value_resolution.cpython-39.pyc
+-rw-r--r--   0        0        0     4780 2023-07-13 15:44:53.981339 renku-2.6.1rc1/renku/core/workflow/__pycache__/workflow_file.cpython-39.pyc
+-rw-r--r--   0        0        0    22713 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/workflow/activity.py
+-rw-r--r--   0        0        0      773 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/workflow/converters/__init__.py
+-rw-r--r--   0        0        0      215 2023-07-13 15:44:50.965257 renku-2.6.1rc1/renku/core/workflow/converters/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    11079 2023-07-13 15:44:50.969257 renku-2.6.1rc1/renku/core/workflow/converters/__pycache__/cwl.cpython-39.pyc
+-rw-r--r--   0        0        0     4668 2023-07-13 15:44:52.497298 renku-2.6.1rc1/renku/core/workflow/converters/__pycache__/renku.cpython-39.pyc
+-rw-r--r--   0        0        0    17937 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/workflow/converters/cwl.py
+-rw-r--r--   0        0        0     5142 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/workflow/converters/renku.py
+-rw-r--r--   0        0        0    18756 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/workflow/execute.py
+-rw-r--r--   0        0        0      769 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/workflow/model/__init__.py
+-rw-r--r--   0        0        0      206 2023-07-13 15:44:51.629275 renku-2.6.1rc1/renku/core/workflow/model/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4825 2023-07-13 15:44:51.629275 renku-2.6.1rc1/renku/core/workflow/model/__pycache__/concrete_execution_graph.cpython-39.pyc
+-rw-r--r--   0        0        0    26172 2023-07-13 15:44:52.509299 renku-2.6.1rc1/renku/core/workflow/model/__pycache__/workflow_file.cpython-39.pyc
+-rw-r--r--   0        0        0     6530 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/workflow/model/concrete_execution_graph.py
+-rw-r--r--   0        0        0    37866 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/workflow/model/workflow_file.py
+-rw-r--r--   0        0        0      775 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/workflow/parser/__init__.py
+-rw-r--r--   0        0        0      213 2023-07-13 15:44:52.497298 renku-2.6.1rc1/renku/core/workflow/parser/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     8620 2023-07-13 15:44:52.501299 renku-2.6.1rc1/renku/core/workflow/parser/__pycache__/renku.cpython-39.pyc
+-rw-r--r--   0        0        0    10631 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/workflow/parser/renku.py
+-rw-r--r--   0        0        0    34209 2023-07-13 15:43:27.230980 renku-2.6.1rc1/renku/core/workflow/plan.py
+-rw-r--r--   0        0        0    33046 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/core/workflow/plan_factory.py
+-rw-r--r--   0        0        0      772 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/core/workflow/providers/__init__.py
+-rw-r--r--   0        0        0      213 2023-07-13 15:44:52.677303 renku-2.6.1rc1/renku/core/workflow/providers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4631 2023-07-13 15:44:52.677303 renku-2.6.1rc1/renku/core/workflow/providers/__pycache__/cwltool.cpython-39.pyc
+-rw-r--r--   0        0        0     3918 2023-07-13 15:44:53.189317 renku-2.6.1rc1/renku/core/workflow/providers/__pycache__/local.cpython-39.pyc
+-rw-r--r--   0        0        0    11194 2023-07-13 15:44:53.193318 renku-2.6.1rc1/renku/core/workflow/providers/__pycache__/toil.cpython-39.pyc
+-rw-r--r--   0        0        0     5999 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/core/workflow/providers/cwltool.py
+-rw-r--r--   0        0        0     4271 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/core/workflow/providers/local.py
+-rw-r--r--   0        0        0    13372 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/core/workflow/providers/toil.py
+-rw-r--r--   0        0        0    14384 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/core/workflow/run.py
+-rw-r--r--   0        0        0     1681 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/core/workflow/types.py
+-rw-r--r--   0        0        0     2869 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/core/workflow/update.py
+-rw-r--r--   0        0        0     8335 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/core/workflow/value_resolution.py
+-rw-r--r--   0        0        0     5089 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/core/workflow/workflow_file.py
+-rw-r--r--   0        0        0      767 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/data/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/data/defaults.ini
+-rw-r--r--   0        0        0     3364 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/data/gitignore.default
+-rwxr-xr-x   0        0        0     4474 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/data/pre-commit.sh
+-rw-r--r--   0        0        0    48383 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/data/shacl_shape.json
+-rw-r--r--   0        0        0      767 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/__init__.py
+-rw-r--r--   0        0        0      210 2023-07-13 15:44:49.885228 renku-2.6.1rc1/renku/domain_model/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      388 2023-07-13 15:44:49.909228 renku-2.6.1rc1/renku/domain_model/__pycache__/constant.cpython-39.pyc
+-rw-r--r--   0        0        0    26295 2023-07-13 15:44:49.941229 renku-2.6.1rc1/renku/domain_model/__pycache__/dataset.cpython-39.pyc
+-rw-r--r--   0        0        0      988 2023-07-13 15:44:50.085233 renku-2.6.1rc1/renku/domain_model/__pycache__/dataset_provider.cpython-39.pyc
+-rw-r--r--   0        0        0     2204 2023-07-13 15:44:52.669303 renku-2.6.1rc1/renku/domain_model/__pycache__/datastructures.cpython-39.pyc
+-rw-r--r--   0        0        0     2539 2023-07-13 15:44:50.309239 renku-2.6.1rc1/renku/domain_model/__pycache__/entity.cpython-39.pyc
+-rw-r--r--   0        0        0      575 2023-07-13 15:44:49.933229 renku-2.6.1rc1/renku/domain_model/__pycache__/enums.cpython-39.pyc
+-rw-r--r--   0        0        0     6097 2023-07-13 15:44:52.493298 renku-2.6.1rc1/renku/domain_model/__pycache__/project.cpython-39.pyc
+-rw-r--r--   0        0        0    12164 2023-07-13 15:44:49.885228 renku-2.6.1rc1/renku/domain_model/__pycache__/project_context.cpython-39.pyc
+-rw-r--r--   0        0        0     7426 2023-07-13 15:44:50.821253 renku-2.6.1rc1/renku/domain_model/__pycache__/session.cpython-39.pyc
+-rw-r--r--   0        0        0     1092 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/constant.py
+-rw-r--r--   0        0        0    29611 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/dataset.py
+-rw-r--r--   0        0        0     1267 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/dataset_provider.py
+-rw-r--r--   0        0        0     2754 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/datastructures.py
+-rw-r--r--   0        0        0     2499 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/entity.py
+-rw-r--r--   0        0        0      971 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/enums.py
+-rw-r--r--   0        0        0     5059 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/git.py
+-rw-r--r--   0        0        0     8329 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/project.py
+-rw-r--r--   0        0        0    11817 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/project_context.py
+-rw-r--r--   0        0        0      829 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/provenance/__init__.py
+-rw-r--r--   0        0        0      283 2023-07-13 15:44:50.305239 renku-2.6.1rc1/renku/domain_model/provenance/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    11882 2023-07-13 15:44:52.613302 renku-2.6.1rc1/renku/domain_model/provenance/__pycache__/activity.cpython-39.pyc
+-rw-r--r--   0        0        0     4946 2023-07-13 15:44:50.305239 renku-2.6.1rc1/renku/domain_model/provenance/__pycache__/agent.cpython-39.pyc
+-rw-r--r--   0        0        0     1092 2023-07-13 15:44:50.305239 renku-2.6.1rc1/renku/domain_model/provenance/__pycache__/annotation.cpython-39.pyc
+-rw-r--r--   0        0        0     1363 2023-07-13 15:44:52.613302 renku-2.6.1rc1/renku/domain_model/provenance/__pycache__/parameter.cpython-39.pyc
+-rw-r--r--   0        0        0    13200 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/provenance/activity.py
+-rw-r--r--   0        0        0     5155 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/provenance/agent.py
+-rw-r--r--   0        0        0     1268 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/provenance/annotation.py
+-rw-r--r--   0        0        0     1530 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/provenance/parameter.py
+-rw-r--r--   0        0        0     6871 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/session.py
+-rw-r--r--   0        0        0     1471 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/sort.py
+-rw-r--r--   0        0        0    27042 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/template.py
+-rw-r--r--   0        0        0      782 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/workflow/__init__.py
+-rw-r--r--   0        0        0      234 2023-07-13 15:44:51.625275 renku-2.6.1rc1/renku/domain_model/workflow/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    13527 2023-07-13 15:44:52.121288 renku-2.6.1rc1/renku/domain_model/workflow/__pycache__/composite_plan.cpython-39.pyc
+-rw-r--r--   0        0        0    15243 2023-07-13 15:44:52.125288 renku-2.6.1rc1/renku/domain_model/workflow/__pycache__/parameter.cpython-39.pyc
+-rw-r--r--   0        0        0    15096 2023-07-13 15:44:52.129288 renku-2.6.1rc1/renku/domain_model/workflow/__pycache__/plan.cpython-39.pyc
+-rw-r--r--   0        0        0     1483 2023-07-13 15:44:51.625275 renku-2.6.1rc1/renku/domain_model/workflow/__pycache__/provider.cpython-39.pyc
+-rw-r--r--   0        0        0     4523 2023-07-13 15:44:52.617302 renku-2.6.1rc1/renku/domain_model/workflow/__pycache__/workflow_file.cpython-39.pyc
+-rw-r--r--   0        0        0    15917 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/workflow/composite_plan.py
+-rw-r--r--   0        0        0     1531 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/workflow/converters/__init__.py
+-rw-r--r--   0        0        0     1391 2023-07-13 15:44:52.497298 renku-2.6.1rc1/renku/domain_model/workflow/converters/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    18124 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/workflow/parameter.py
+-rw-r--r--   0        0        0    16602 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/workflow/plan.py
+-rw-r--r--   0        0        0     1639 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/workflow/provider.py
+-rw-r--r--   0        0        0     4660 2023-07-13 15:43:27.234980 renku-2.6.1rc1/renku/domain_model/workflow/workflow_file.py
+-rw-r--r--   0        0        0      780 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/infrastructure/__init__.py
+-rw-r--r--   0        0        0      212 2023-07-13 15:44:49.665222 renku-2.6.1rc1/renku/infrastructure/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    34957 2023-07-13 15:44:52.261292 renku-2.6.1rc1/renku/infrastructure/__pycache__/database.cpython-39.pyc
+-rw-r--r--   0        0        0     5073 2023-07-13 15:44:49.909228 renku-2.6.1rc1/renku/infrastructure/__pycache__/immutable.cpython-39.pyc
+-rw-r--r--   0        0        0     2259 2023-07-13 15:44:50.029231 renku-2.6.1rc1/renku/infrastructure/__pycache__/persistent.cpython-39.pyc
+-rw-r--r--   0        0        0    67803 2023-07-13 15:44:49.689222 renku-2.6.1rc1/renku/infrastructure/__pycache__/repository.cpython-39.pyc
+-rw-r--r--   0        0        0    41333 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/infrastructure/database.py
+-rw-r--r--   0        0        0      786 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/infrastructure/gateway/__init__.py
+-rw-r--r--   0        0        0      226 2023-07-13 15:44:50.577246 renku-2.6.1rc1/renku/infrastructure/gateway/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3238 2023-07-13 15:44:50.577246 renku-2.6.1rc1/renku/infrastructure/gateway/__pycache__/dataset_gateway.cpython-39.pyc
+-rw-r--r--   0        0        0    12730 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/infrastructure/gateway/activity_gateway.py
+-rw-r--r--   0        0        0     5845 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/infrastructure/gateway/database_gateway.py
+-rw-r--r--   0        0        0     3743 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/infrastructure/gateway/dataset_gateway.py
+-rw-r--r--   0        0        0     3529 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/infrastructure/gateway/plan_gateway.py
+-rw-r--r--   0        0        0     1711 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/infrastructure/gateway/project_gateway.py
+-rw-r--r--   0        0        0    18006 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/infrastructure/git_merger.py
+-rw-r--r--   0        0        0     4969 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/infrastructure/immutable.py
+-rw-r--r--   0        0        0     2394 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/infrastructure/persistent.py
+-rw-r--r--   0        0        0    72047 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/infrastructure/repository.py
+-rw-r--r--   0        0        0      784 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/infrastructure/storage/__init__.py
+-rw-r--r--   0        0        0      224 2023-07-13 15:44:50.317239 renku-2.6.1rc1/renku/infrastructure/storage/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1523 2023-07-13 15:44:50.317239 renku-2.6.1rc1/renku/infrastructure/storage/__pycache__/factory.cpython-39.pyc
+-rw-r--r--   0        0        0     1989 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/infrastructure/storage/factory.py
+-rw-r--r--   0        0        0     8859 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/infrastructure/storage/rclone.py
+-rw-r--r--   0        0        0      913 2023-07-13 15:44:54.729359 renku-2.6.1rc1/renku/templates/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      553 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      637 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      523 2023-07-13 15:44:54.741360 renku-2.6.1rc1/renku/templates/.github/dependabot.yml
+-rw-r--r--   0        0        0      396 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/.github/workflows/github-project.yml
+-rw-r--r--   0        0        0     3940 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/.gitignore
+-rw-r--r--   0        0        0       27 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/R-minimal/.dockerignore
+-rw-r--r--   0        0        0     6018 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/R-minimal/.gitignore
+-rw-r--r--   0        0        0      450 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/R-minimal/.gitlab-ci.yml
+-rw-r--r--   0        0        0       37 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/R-minimal/.renku/renku.ini
+-rw-r--r--   0        0        0      984 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/R-minimal/.renkulfsignore
+-rw-r--r--   0        0        0     2087 2023-07-13 15:44:54.741360 renku-2.6.1rc1/renku/templates/R-minimal/Dockerfile
+-rw-r--r--   0        0        0     1603 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/R-minimal/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/R-minimal/data/.gitkeep
+-rw-r--r--   0        0        0      112 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/R-minimal/environment.yml
+-rw-r--r--   0        0        0      360 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/R-minimal/install.R
+-rw-r--r--   0        0        0        0 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/R-minimal/notebooks/.gitkeep
+-rw-r--r--   0        0        0        0 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/R-minimal/requirements.txt
+-rw-r--r--   0        0        0     1439 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/R-minimal/workflows/my-workflow.yaml
+-rw-r--r--   0        0        0      205 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/R-minimal/{{ __sanitized_project_name__ }}.Rproj
+-rw-r--r--   0        0        0    14286 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/R-minimal.png
+-rw-r--r--   0        0        0     4846 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/README.md
+-rw-r--r--   0        0        0       27 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/bioc-minimal/.dockerignore
+-rw-r--r--   0        0        0     6018 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/bioc-minimal/.gitignore
+-rw-r--r--   0        0        0      450 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/bioc-minimal/.gitlab-ci.yml
+-rw-r--r--   0        0        0       37 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/bioc-minimal/.renku/renku.ini
+-rw-r--r--   0        0        0      976 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/bioc-minimal/.renkulfsignore
+-rw-r--r--   0        0        0     2077 2023-07-13 15:44:54.741360 renku-2.6.1rc1/renku/templates/bioc-minimal/Dockerfile
+-rw-r--r--   0        0        0     1603 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/bioc-minimal/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/bioc-minimal/data/.gitkeep
+-rw-r--r--   0        0        0      112 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/bioc-minimal/environment.yml
+-rw-r--r--   0        0        0        0 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/bioc-minimal/install.R
+-rw-r--r--   0        0        0        0 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/bioc-minimal/notebooks/.gitkeep
+-rw-r--r--   0        0        0        0 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/bioc-minimal/requirements.txt
+-rw-r--r--   0        0        0     1439 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/bioc-minimal/workflows/my-workflow.yaml
+-rw-r--r--   0        0        0      205 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/bioc-minimal/{{ __sanitized_project_name__ }}.Rproj
+-rw-r--r--   0        0        0    44589 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/bioconductor.png
+-rw-r--r--   0        0        0       27 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/julia-minimal/.dockerignore
+-rw-r--r--   0        0        0     6018 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/julia-minimal/.gitignore
+-rw-r--r--   0        0        0      450 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/julia-minimal/.gitlab-ci.yml
+-rw-r--r--   0        0        0       50 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/julia-minimal/.renku/renku.ini
+-rw-r--r--   0        0        0      976 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/julia-minimal/.renkulfsignore
+-rw-r--r--   0        0        0     2469 2023-07-13 15:44:54.741360 renku-2.6.1rc1/renku/templates/julia-minimal/Dockerfile
+-rw-r--r--   0        0        0        0 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/julia-minimal/Manifest.toml
+-rw-r--r--   0        0        0        0 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/julia-minimal/Project.toml
+-rw-r--r--   0        0        0     1842 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/julia-minimal/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/julia-minimal/data/.gitkeep
+-rw-r--r--   0        0        0      112 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/julia-minimal/environment.yml
+-rw-r--r--   0        0        0        0 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/julia-minimal/notebooks/.gitkeep
+-rw-r--r--   0        0        0        0 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/julia-minimal/requirements.txt
+-rw-r--r--   0        0        0     1439 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/julia-minimal/workflows/my-workflow.yaml
+-rw-r--r--   0        0        0    13782 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/julialang.png
+-rw-r--r--   0        0        0     1174 2023-07-13 15:44:54.741360 renku-2.6.1rc1/renku/templates/manifest.yaml
+-rw-r--r--   0        0        0       17 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/minimal/.dockerignore
+-rw-r--r--   0        0        0       77 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/minimal/.gitignore
+-rw-r--r--   0        0        0      450 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/minimal/.gitlab-ci.yml
+-rw-r--r--   0        0        0       33 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/minimal/.renku/renku.ini
+-rw-r--r--   0        0        0      976 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/minimal/.renkulfsignore
+-rw-r--r--   0        0        0     2414 2023-07-13 15:44:54.741360 renku-2.6.1rc1/renku/templates/minimal/Dockerfile
+-rw-r--r--   0        0        0     1439 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/minimal/workflows/my-workflow.yaml
+-rw-r--r--   0        0        0       27 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/python-minimal/.dockerignore
+-rw-r--r--   0        0        0     5401 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/python-minimal/.gitignore
+-rw-r--r--   0        0        0      450 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/python-minimal/.gitlab-ci.yml
+-rw-r--r--   0        0        0       33 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/python-minimal/.renku/renku.ini
+-rw-r--r--   0        0        0      976 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/python-minimal/.renkulfsignore
+-rw-r--r--   0        0        0     2159 2023-07-13 15:44:54.741360 renku-2.6.1rc1/renku/templates/python-minimal/Dockerfile
+-rw-r--r--   0        0        0     1597 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/python-minimal/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/python-minimal/data/.gitkeep
+-rw-r--r--   0        0        0      112 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/python-minimal/environment.yml
+-rw-r--r--   0        0        0        0 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/python-minimal/notebooks/.gitkeep
+-rw-r--r--   0        0        0        0 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/python-minimal/requirements.txt
+-rw-r--r--   0        0        0     1439 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/python-minimal/workflows/my-workflow.yaml
+-rw-r--r--   0        0        0    25599 2023-07-13 15:44:54.733359 renku-2.6.1rc1/renku/templates/python-minimal.png
+-rw-r--r--   0        0        0      763 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/ui/__init__.py
+-rw-r--r--   0        0        0      184 2023-07-13 15:44:49.501217 renku-2.6.1rc1/renku/ui/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1268 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/ui/api/__init__.py
+-rw-r--r--   0        0        0      763 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/ui/api/graph/__init__.py
+-rw-r--r--   0        0        0     2519 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/ui/api/graph/rdf.py
+-rw-r--r--   0        0        0      764 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/ui/api/models/__init__.py
+-rw-r--r--   0        0        0    16448 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/ui/api/models/activity.py
+-rw-r--r--   0        0        0     4648 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/ui/api/models/dataset.py
+-rw-r--r--   0        0        0    10361 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/ui/api/models/parameter.py
+-rw-r--r--   0        0        0     9227 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/ui/api/models/plan.py
+-rw-r--r--   0        0        0     3643 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/ui/api/models/project.py
+-rw-r--r--   0        0        0     2519 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/ui/api/util.py
+-rw-r--r--   0        0        0     9319 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/ui/cli/__init__.py
+-rw-r--r--   0        0        0      922 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/ui/cli/__main__.py
+-rw-r--r--   0        0        0     8150 2023-07-13 15:44:49.501217 renku-2.6.1rc1/renku/ui/cli/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2117 2023-07-13 15:44:49.889227 renku-2.6.1rc1/renku/ui/cli/__pycache__/clone.cpython-39.pyc
+-rw-r--r--   0        0        0     7029 2023-07-13 15:44:49.893228 renku-2.6.1rc1/renku/ui/cli/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0        0        0    36275 2023-07-13 15:44:49.901228 renku-2.6.1rc1/renku/ui/cli/__pycache__/dataset.cpython-39.pyc
+-rw-r--r--   0        0        0     1787 2023-07-13 15:44:53.905337 renku-2.6.1rc1/renku/ui/cli/__pycache__/doctor.cpython-39.pyc
+-rw-r--r--   0        0        0      964 2023-07-13 15:44:53.909337 renku-2.6.1rc1/renku/ui/cli/__pycache__/env.cpython-39.pyc
+-rw-r--r--   0        0        0     7957 2023-07-13 15:44:53.909337 renku-2.6.1rc1/renku/ui/cli/__pycache__/exception_handler.cpython-39.pyc
+-rw-r--r--   0        0        0      645 2023-07-13 15:44:53.925337 renku-2.6.1rc1/renku/ui/cli/__pycache__/gc.cpython-39.pyc
+-rw-r--r--   0        0        0     2168 2023-07-13 15:44:53.925337 renku-2.6.1rc1/renku/ui/cli/__pycache__/githooks.cpython-39.pyc
+-rw-r--r--   0        0        0     4041 2023-07-13 15:44:53.925337 renku-2.6.1rc1/renku/ui/cli/__pycache__/graph.cpython-39.pyc
+-rw-r--r--   0        0        0     9637 2023-07-13 15:44:53.929338 renku-2.6.1rc1/renku/ui/cli/__pycache__/init.cpython-39.pyc
+-rw-r--r--   0        0        0     7264 2023-07-13 15:44:53.929338 renku-2.6.1rc1/renku/ui/cli/__pycache__/log.cpython-39.pyc
+-rw-r--r--   0        0        0     4296 2023-07-13 15:44:53.941338 renku-2.6.1rc1/renku/ui/cli/__pycache__/login.cpython-39.pyc
+-rw-r--r--   0        0        0     2066 2023-07-13 15:44:53.973339 renku-2.6.1rc1/renku/ui/cli/__pycache__/mergetool.cpython-39.pyc
+-rw-r--r--   0        0        0     4585 2023-07-13 15:44:53.973339 renku-2.6.1rc1/renku/ui/cli/__pycache__/migrate.cpython-39.pyc
+-rw-r--r--   0        0        0     2306 2023-07-13 15:44:53.973339 renku-2.6.1rc1/renku/ui/cli/__pycache__/move.cpython-39.pyc
+-rw-r--r--   0        0        0     4028 2023-07-13 15:44:53.977339 renku-2.6.1rc1/renku/ui/cli/__pycache__/project.cpython-39.pyc
+-rw-r--r--   0        0        0     1283 2023-07-13 15:44:53.977339 renku-2.6.1rc1/renku/ui/cli/__pycache__/remove.cpython-39.pyc
+-rw-r--r--   0        0        0     3485 2023-07-13 15:44:53.977339 renku-2.6.1rc1/renku/ui/cli/__pycache__/rerun.cpython-39.pyc
+-rw-r--r--   0        0        0     2761 2023-07-13 15:44:53.977339 renku-2.6.1rc1/renku/ui/cli/__pycache__/rollback.cpython-39.pyc
+-rw-r--r--   0        0        0    23646 2023-07-13 15:44:53.981339 renku-2.6.1rc1/renku/ui/cli/__pycache__/run.cpython-39.pyc
+-rw-r--r--   0        0        0     2890 2023-07-13 15:44:53.993339 renku-2.6.1rc1/renku/ui/cli/__pycache__/save.cpython-39.pyc
+-rw-r--r--   0        0        0    10362 2023-07-13 15:44:53.997339 renku-2.6.1rc1/renku/ui/cli/__pycache__/service.cpython-39.pyc
+-rw-r--r--   0        0        0    13046 2023-07-13 15:44:54.001340 renku-2.6.1rc1/renku/ui/cli/__pycache__/session.cpython-39.pyc
+-rw-r--r--   0        0        0     3715 2023-07-13 15:44:54.005340 renku-2.6.1rc1/renku/ui/cli/__pycache__/status.cpython-39.pyc
+-rw-r--r--   0        0        0     5061 2023-07-13 15:44:54.009340 renku-2.6.1rc1/renku/ui/cli/__pycache__/storage.cpython-39.pyc
+-rw-r--r--   0        0        0    10944 2023-07-13 15:44:54.009340 renku-2.6.1rc1/renku/ui/cli/__pycache__/template.cpython-39.pyc
+-rw-r--r--   0        0        0     5790 2023-07-13 15:44:54.013340 renku-2.6.1rc1/renku/ui/cli/__pycache__/update.cpython-39.pyc
+-rw-r--r--   0        0        0    41570 2023-07-13 15:44:54.017340 renku-2.6.1rc1/renku/ui/cli/__pycache__/workflow.cpython-39.pyc
+-rw-r--r--   0        0        0     2594 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/ui/cli/clone.py
+-rw-r--r--   0        0        0     7953 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/ui/cli/config.py
+-rw-r--r--   0        0        0    42787 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/ui/cli/dataset.py
+-rw-r--r--   0        0        0     2333 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/ui/cli/doctor.py
+-rw-r--r--   0        0        0     1587 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/ui/cli/env.py
+-rw-r--r--   0        0        0     7931 2023-07-13 15:43:27.238980 renku-2.6.1rc1/renku/ui/cli/exception_handler.py
+-rw-r--r--   0        0        0     1139 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/gc.py
+-rw-r--r--   0        0        0     2538 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/githooks.py
+-rw-r--r--   0        0        0     4950 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/graph.py
+-rw-r--r--   0        0        0    11113 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/init.py
+-rw-r--r--   0        0        0     8581 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/log.py
+-rw-r--r--   0        0        0     4845 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/login.py
+-rw-r--r--   0        0        0     2499 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/mergetool.py
+-rw-r--r--   0        0        0     5894 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/migrate.py
+-rw-r--r--   0        0        0     2881 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/move.py
+-rw-r--r--   0        0        0     5768 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/project.py
+-rw-r--r--   0        0        0     1754 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/remove.py
+-rw-r--r--   0        0        0     4227 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/rerun.py
+-rw-r--r--   0        0        0     3249 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/rollback.py
+-rw-r--r--   0        0        0    26417 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/run.py
+-rw-r--r--   0        0        0     3510 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/save.py
+-rw-r--r--   0        0        0    11927 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/service.py
+-rw-r--r--   0        0        0    14738 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/session.py
+-rw-r--r--   0        0        0     5489 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/status.py
+-rw-r--r--   0        0        0     5604 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/storage.py
+-rw-r--r--   0        0        0    13434 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/template.py
+-rw-r--r--   0        0        0     6723 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/update.py
+-rw-r--r--   0        0        0      760 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/utils/__init__.py
+-rw-r--r--   0        0        0      203 2023-07-13 15:44:49.889227 renku-2.6.1rc1/renku/ui/cli/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5720 2023-07-13 15:44:53.941338 renku-2.6.1rc1/renku/ui/cli/utils/__pycache__/callback.cpython-39.pyc
+-rw-r--r--   0        0        0     5071 2023-07-13 15:44:49.893228 renku-2.6.1rc1/renku/ui/cli/utils/__pycache__/click.cpython-39.pyc
+-rw-r--r--   0        0        0      301 2023-07-13 15:44:49.889227 renku-2.6.1rc1/renku/ui/cli/utils/__pycache__/color.cpython-39.pyc
+-rw-r--r--   0        0        0      998 2023-07-13 15:44:53.977339 renku-2.6.1rc1/renku/ui/cli/utils/__pycache__/plugins.cpython-39.pyc
+-rw-r--r--   0        0        0     7369 2023-07-13 15:44:53.937338 renku-2.6.1rc1/renku/ui/cli/utils/__pycache__/terminal.cpython-39.pyc
+-rw-r--r--   0        0        0     5409 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/utils/callback.py
+-rw-r--r--   0        0        0     5473 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/utils/click.py
+-rw-r--r--   0        0        0      842 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/utils/color.py
+-rw-r--r--   0        0        0    14521 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/utils/curses.py
+-rw-r--r--   0        0        0     1375 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/utils/plugins.py
+-rw-r--r--   0        0        0     9917 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/utils/terminal.py
+-rw-r--r--   0        0        0    47787 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/cli/workflow.py
+-rw-r--r--   0        0        0      843 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/service/.env-example
+-rw-r--r--   0        0        0      756 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/service/__init__.py
+-rw-r--r--   0        0        0      189 2023-07-13 15:44:53.909337 renku-2.6.1rc1/renku/ui/service/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2109 2023-07-13 15:44:53.909337 renku-2.6.1rc1/renku/ui/service/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0        0        0     1535 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/service/cache/__init__.py
+-rw-r--r--   0        0        0     2917 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/service/cache/base.py
+-rw-r--r--   0        0        0     1444 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/service/cache/config.py
+-rw-r--r--   0        0        0     3315 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/service/cache/files.py
+-rw-r--r--   0        0        0     2333 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/service/cache/jobs.py
+-rw-r--r--   0        0        0      769 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/service/cache/models/__init__.py
+-rw-r--r--   0        0        0     4356 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/service/cache/models/file.py
+-rw-r--r--   0        0        0     2298 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/service/cache/models/job.py
+-rw-r--r--   0        0        0     4043 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/service/cache/models/project.py
+-rw-r--r--   0        0        0     1127 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/service/cache/models/user.py
+-rw-r--r--   0        0        0     2558 2023-07-13 15:43:27.242980 renku-2.6.1rc1/renku/ui/service/cache/projects.py
+-rw-r--r--   0        0        0      774 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/cache/serializers/__init__.py
+-rw-r--r--   0        0        0     1821 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/cache/serializers/file.py
+-rw-r--r--   0        0        0     1711 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/cache/serializers/job.py
+-rw-r--r--   0        0        0     1812 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/cache/serializers/project.py
+-rw-r--r--   0        0        0     1227 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/cache/serializers/user.py
+-rw-r--r--   0        0        0     1657 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/cache/users.py
+-rw-r--r--   0        0        0     3091 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/config.py
+-rw-r--r--   0        0        0      773 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/__init__.py
+-rw-r--r--   0        0        0      777 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/api/__init__.py
+-rw-r--r--   0        0        0     1085 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/api/abstract.py
+-rw-r--r--   0        0        0    15838 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/api/mixins.py
+-rw-r--r--   0        0        0     2647 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/cache_files_delete_chunks.py
+-rw-r--r--   0        0        0     7478 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/cache_files_upload.py
+-rw-r--r--   0        0        0     2239 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/cache_list_projects.py
+-rw-r--r--   0        0        0     1927 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/cache_list_uploaded.py
+-rw-r--r--   0        0        0     4823 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/cache_migrate_project.py
+-rw-r--r--   0        0        0     4905 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/cache_migrations_check.py
+-rw-r--r--   0        0        0     2350 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/cache_project_clone.py
+-rw-r--r--   0        0        0     2649 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/config_set.py
+-rw-r--r--   0        0        0     2333 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/config_show.py
+-rw-r--r--   0        0        0     5682 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/datasets_add_file.py
+-rw-r--r--   0        0        0     3916 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/datasets_create.py
+-rw-r--r--   0        0        0     5359 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/datasets_edit.py
+-rw-r--r--   0        0        0     2132 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/datasets_files_list.py
+-rw-r--r--   0        0        0     3333 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/datasets_import.py
+-rw-r--r--   0        0        0     2065 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/datasets_list.py
+-rw-r--r--   0        0        0     2637 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/datasets_remove.py
+-rw-r--r--   0        0        0     3290 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/datasets_unlink.py
+-rw-r--r--   0        0        0     5370 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/graph_export.py
+-rw-r--r--   0        0        0     3936 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/project_edit.py
+-rw-r--r--   0        0        0     3180 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/project_lock_status.py
+-rw-r--r--   0        0        0     2096 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/project_show.py
+-rw-r--r--   0        0        0     8150 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/templates_create_project.py
+-rw-r--r--   0        0        0     3103 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/templates_read_manifest.py
+-rw-r--r--   0        0        0      773 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/utils/__init__.py
+-rw-r--r--   0        0        0     1083 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/utils/datasets.py
+-rw-r--r--   0        0        0     3233 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/utils/project_clone.py
+-rw-r--r--   0        0        0     2664 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/utils/remote_project.py
+-rw-r--r--   0        0        0     1641 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/version.py
+-rw-r--r--   0        0        0     1389 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/versions_list.py
+-rw-r--r--   0        0        0     2441 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/workflow_plans_export.py
+-rw-r--r--   0        0        0     2257 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/workflow_plans_list.py
+-rw-r--r--   0        0        0     2146 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/controllers/workflow_plans_show.py
+-rw-r--r--   0        0        0     6275 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/entrypoint.py
+-rw-r--r--   0        0        0    32144 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/errors.py
+-rw-r--r--   0        0        0      774 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/gateways/__init__.py
+-rw-r--r--   0        0        0     4083 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/gateways/gitlab_api_provider.py
+-rw-r--r--   0        0        0      793 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/interfaces/__init__.py
+-rw-r--r--   0        0        0     1272 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/interfaces/git_api_provider.py
+-rw-r--r--   0        0        0      766 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/jobs/__init__.py
+-rw-r--r--   0        0        0     3035 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/jobs/cleanup.py
+-rw-r--r--   0        0        0      756 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/jobs/constants.py
+-rw-r--r--   0        0        0     1186 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/jobs/contexts.py
+-rw-r--r--   0        0        0     5288 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/jobs/datasets.py
+-rw-r--r--   0        0        0     1829 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/jobs/delayed_ctrl.py
+-rw-r--r--   0        0        0     2665 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/jobs/queues.py
+-rw-r--r--   0        0        0     1269 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/logger.py
+-rw-r--r--   0        0        0      644 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/logging.yaml
+-rw-r--r--   0        0        0     2742 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/scheduler.py
+-rw-r--r--   0        0        0      768 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/serializers/__init__.py
+-rw-r--r--   0        0        0    14561 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/serializers/cache.py
+-rw-r--r--   0        0        0     4843 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/serializers/common.py
+-rw-r--r--   0        0        0     2228 2023-07-13 15:43:27.246981 renku-2.6.1rc1/renku/ui/service/serializers/config.py
+-rw-r--r--   0        0        0     8503 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/serializers/datasets.py
+-rw-r--r--   0        0        0     2195 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/serializers/graph.py
+-rw-r--r--   0        0        0     5362 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/serializers/headers.py
+-rw-r--r--   0        0        0     1961 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/serializers/jobs.py
+-rw-r--r--   0        0        0     4510 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/serializers/project.py
+-rw-r--r--   0        0        0      911 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/serializers/rpc.py
+-rw-r--r--   0        0        0     5815 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/serializers/templates.py
+-rw-r--r--   0        0        0      773 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/serializers/v1/__init__.py
+-rw-r--r--   0        0        0     4212 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/serializers/v1/cache.py
+-rw-r--r--   0        0        0     1880 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/serializers/v1/templates.py
+-rw-r--r--   0        0        0     1171 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/serializers/version.py
+-rw-r--r--   0        0        0     1365 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/serializers/versions_list.py
+-rw-r--r--   0        0        0     6907 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/serializers/workflows.py
+-rw-r--r--   0        0        0     2186 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/utils/__init__.py
+-rw-r--r--   0        0        0     2220 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/utils/callback.py
+-rw-r--r--   0        0        0     1323 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/utils/json_encoder.py
+-rw-r--r--   0        0        0     1260 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/utils/squash.py
+-rw-r--r--   0        0        0     1427 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/utils/timeout.py
+-rw-r--r--   0        0        0     1761 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/views/__init__.py
+-rw-r--r--   0        0        0     2438 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/views/api_versions.py
+-rw-r--r--   0        0        0     4767 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/views/apispec.py
+-rw-r--r--   0        0        0     7427 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/views/cache.py
+-rw-r--r--   0        0        0     2957 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/views/config.py
+-rw-r--r--   0        0        0     8187 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/views/datasets.py
+-rw-r--r--   0        0        0     2961 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/views/decorators.py
+-rw-r--r--   0        0        0    15114 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/views/error_handlers.py
+-rw-r--r--   0        0        0     2084 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/views/graph.py
+-rw-r--r--   0        0        0     3267 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/views/jobs.py
+-rw-r--r--   0        0        0     3805 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/views/project.py
+-rw-r--r--   0        0        0     3592 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/views/templates.py
+-rw-r--r--   0        0        0      767 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/views/v1/__init__.py
+-rw-r--r--   0        0        0     4775 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/views/v1/cache.py
+-rw-r--r--   0        0        0     2634 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/views/v1/templates.py
+-rw-r--r--   0        0        0     1702 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/views/version.py
+-rw-r--r--   0        0        0     1676 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/views/versions_list.py
+-rw-r--r--   0        0        0     3873 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/views/workflow_plans.py
+-rw-r--r--   0        0        0     2976 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/ui/service/worker.py
+-rw-r--r--   0        0        0     1614 2023-07-13 15:43:27.250980 renku-2.6.1rc1/renku/version.py
+-rw-r--r--   0        0        0    17139 1970-01-01 00:00:00.000000 renku-2.6.1rc1/PKG-INFO
```

### Comparing `renku-2.6.0rc1/AUTHORS.rst` & `renku-2.6.1rc1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/CHANGES.rst` & `renku-2.6.1rc1/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/LICENSE` & `renku-2.6.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/README.rst` & `renku-2.6.1rc1/README.rst`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/pyproject.toml` & `renku-2.6.1rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 [tool]
 
 [tool.poetry]
 name = "renku"
-version = "2.6.0rc1" # placeholder, see poetry-dynamic-versioning
+version = "2.6.1rc1" # placeholder, see poetry-dynamic-versioning
 description = "Python SDK and CLI for the Renku platform."
 license = "Apache License 2.0"
 keywords = ["Renku", "CLI"]
 classifiers = [
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
@@ -112,15 +112,15 @@
 circus = { version = "==0.18.0", optional = true }
 flask = { version = "==2.2.5", optional = true }
 gunicorn = { version = "*", optional = true }
 marshmallow = { version = ">=3.18.0,<3.20.0", optional = true }
 marshmallow-oneofschema = { version = ">=3.0.1,<4.0.0", optional = true }
 pillow = { version = ">=9.0.0,<9.6", optional = true }
 python-dotenv = { version = ">=0.19.0,<0.21.0", optional = true }
-redis = { version = ">=3.5.3,<4.6.0", optional = true }
+redis = { version = ">=3.5.3,<4.6.0,!=4.5.5", optional = true }
 rq = { version = "==1.15.0", optional = true }
 rq-scheduler = { version = "==0.13.1", optional = true }
 sentry-sdk = { version = ">=1.5.11,<1.26.0", extras = ["flask"],  optional = true }
 walrus = { version = ">=0.8.2,<0.10.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 black = "==23.1.0"
```

### Comparing `renku-2.6.0rc1/renku/__init__.py` & `renku-2.6.1rc1/renku/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/__init__.py` & `renku-2.6.1rc1/renku/command/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/__pycache__/run.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/__pycache__/run.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1600 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 4006 0000  a........^.d@...
+00000000: 610d 0d0a 0000 0000 9f1b b064 4006 0000  a..........d@...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6406 6407 8400 5a0a 650b  m.Z...d.d...Z.e.
 00000070: 6503 6502 650c 1900 1900 6408 9c02 6409  e.e.e.....d...d.
```

### Comparing `renku-2.6.0rc1/renku/command/__pycache__/util.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/__pycache__/util.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1726 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 be06 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 be06 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 9a00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6503 6a04 6403  Z.d.d.l.Z.e.j.d.
 00000050: 6404 6405 6406 8d03 5a05 6503 6a04 6407  d.d.d...Z.e.j.d.
 00000060: 6404 6408 6406 8d03 5a06 6503 6a04 6409  d.d.d...Z.e.j.d.
 00000070: 6404 640a 6406 8d03 5a07 640b 640c 8400  d.d.d...Z.d.d...
```

### Comparing `renku-2.6.0rc1/renku/command/__pycache__/version.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/__pycache__/version.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1088 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 4004 0000  a........^.d@...
+00000000: 610d 0d0a 0000 0000 9f1b b064 4004 0000  a..........d@...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6403 6404 8400  Z.d.d.l.Z.d.d...
 00000040: 5a02 6402 5300 2905 7a15 5665 7273 696f  Z.d.S.).z.Versio
 00000050: 6e69 6e67 2075 7469 6c69 7469 6573 2ee9  ning utilities..
 00000060: 0000 0000 4e63 0300 0000 0000 0000 0000  ....Nc..........
 00000070: 0000 0400 0000 0300 0000 4300 0000 7330  ..........C...s0
```

### Comparing `renku-2.6.0rc1/renku/command/checks/__init__.py` & `renku-2.6.1rc1/renku/command/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/checks/activities.py` & `renku-2.6.1rc1/renku/command/checks/activities.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/checks/datasets.py` & `renku-2.6.1rc1/renku/command/checks/datasets.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/checks/githooks.py` & `renku-2.6.1rc1/renku/command/checks/githooks.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/checks/migration.py` & `renku-2.6.1rc1/renku/command/checks/migration.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/checks/project.py` & `renku-2.6.1rc1/renku/command/checks/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/checks/storage.py` & `renku-2.6.1rc1/renku/command/checks/storage.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/checks/validate_shacl.py` & `renku-2.6.1rc1/renku/command/checks/validate_shacl.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/checks/workflow.py` & `renku-2.6.1rc1/renku/command/checks/workflow.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/clone.py` & `renku-2.6.1rc1/renku/command/clone.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/command_builder/__init__.py` & `renku-2.6.1rc1/renku/command/command_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/command_builder/__pycache__/command.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/command_builder/__pycache__/command.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 16678 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 2641 0000  a........^.d&A..
+00000000: 610d 0d0a 0000 0000 9f1b b064 2641 0000  a..........d&A..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 1601 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/command/command_builder/command.py` & `renku-2.6.1rc1/renku/command/command_builder/command.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/command_builder/communication.py` & `renku-2.6.1rc1/renku/command/command_builder/communication.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/command_builder/database.py` & `renku-2.6.1rc1/renku/command/command_builder/database.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/command_builder/lock.py` & `renku-2.6.1rc1/renku/command/command_builder/lock.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/command_builder/migration.py` & `renku-2.6.1rc1/renku/command/command_builder/migration.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/command_builder/repo.py` & `renku-2.6.1rc1/renku/command/command_builder/repo.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/config.py` & `renku-2.6.1rc1/renku/command/config.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/dataset.py` & `renku-2.6.1rc1/renku/command/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/doctor.py` & `renku-2.6.1rc1/renku/command/doctor.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/format/__init__.py` & `renku-2.6.1rc1/renku/command/format/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/format/__pycache__/dataset_files.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/format/__pycache__/dataset_files.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 6230 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 5618 0000  a........^.dV...
+00000000: 610d 0d0a 0000 0000 9f1b b064 5618 0000  a..........dV...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 b800 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6403  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 6d04 5a04 6d05 5a05 0100  l.m.Z.m.Z.m.Z...
 00000050: 6401 6404 6c06 6d07 5a07 6d08 5a08 6d09  d.d.l.m.Z.m.Z.m.
 00000060: 5a09 6d0a 5a0a 0100 6401 6405 6c0b 6d0c  Z.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6402 6406 9c01 6407 6408 8402  Z...d.d...d.d...
```

### Comparing `renku-2.6.0rc1/renku/command/format/__pycache__/dataset_tags.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/format/__pycache__/dataset_tags.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2098 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 3208 0000  a........^.d2...
+00000000: 610d 0d0a 0000 0000 9f1b b064 3208 0000  a..........d2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5000 0000 5500  .....@...sP...U.
 00000030: 6400 5a00 6401 6402 6c01 6d02 5a02 0100  d.Z.d.d.l.m.Z...
 00000040: 6401 6403 6c03 6d04 5a04 6d05 5a05 0100  d.d.l.m.Z.m.Z...
 00000050: 6404 6405 8400 5a06 6406 6407 8400 5a07  d.d...Z.d.d...Z.
 00000060: 6506 6507 6408 9c02 5a08 6505 6509 6504  e.e.d...Z.e.e.e.
 00000070: 6602 1900 650a 6409 3c00 640a 5300 290b  f...e.d.<.d.S.).
```

### Comparing `renku-2.6.0rc1/renku/command/format/__pycache__/datasets.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/format/__pycache__/datasets.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 3236 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 a40c 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 a40c 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000f 0000 0040 0000 0073 9200 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6403  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 6d04 5a04 0100 6401 6404  l.m.Z.m.Z...d.d.
 00000050: 6c05 6d06 5a06 0100 6402 6405 9c01 6406  l.m.Z...d.d...d.
 00000060: 6407 8402 5a07 6408 6409 8400 5a08 640a  d...Z.d.d...Z.d.
 00000070: 640b 8400 5a09 640c 640d 8400 5a0a 6507  d...Z.d.d...Z.e.
```

### Comparing `renku-2.6.0rc1/renku/command/format/__pycache__/json.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/format/__pycache__/json.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1212 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 bc04 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 bc04 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000060: 6503 6a06 8303 5a06 6502 6a07 6503 6a08  e.j...Z.e.j.e.j.
 00000070: 6506 6406 8d02 5a08 6402 5300 2907 7a1b  e.d...Z.d.S.).z.
```

### Comparing `renku-2.6.0rc1/renku/command/format/__pycache__/session.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/format/__pycache__/session.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2402 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 6209 0000  a........^.db...
+00000000: 610d 0d0a 0000 0000 9f1b b064 6209 0000  a..........db...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 8c00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6405 6406 9c01  d.l.m.Z...d.d...
 00000060: 6502 6507 1900 6503 6508 1900 6407 9c02  e.e...e.e...d...
 00000070: 6408 6409 8406 5a09 6405 6406 9c01 6502  d.d...Z.d.d...e.
```

### Comparing `renku-2.6.0rc1/renku/command/format/__pycache__/tabulate.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/format/__pycache__/tabulate.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2769 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 d10a 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 d10a 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 640d 6507 6408 9c01 6409  m.Z...d.e.d...d.
 00000060: 640a 8405 5a08 640b 640c 8400 5a09 6405  d...Z.d.d...Z.d.
 00000070: 5300 290e 7a20 5461 6275 6c61 7220 666f  S.).z Tabular fo
```

### Comparing `renku-2.6.0rc1/renku/command/format/__pycache__/workflow.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/format/__pycache__/workflow.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2728 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 a80a 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 a80a 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 9600 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6403  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 6d04 5a04 0100 6401 6404  l.m.Z.m.Z...d.d.
 00000050: 6c05 6d06 5a06 0100 6401 6405 6c07 6d08  l.m.Z...d.d.l.m.
 00000060: 5a08 0100 6402 6406 9c01 6407 6408 8402  Z...d.d...d.d...
 00000070: 5a09 6409 640a 8400 5a0a 640b 640c 8400  Z.d.d...Z.d.d...
```

### Comparing `renku-2.6.0rc1/renku/command/format/activity.py` & `renku-2.6.1rc1/renku/command/format/activity.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/format/dataset_files.py` & `renku-2.6.1rc1/renku/command/format/dataset_files.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/format/dataset_tags.py` & `renku-2.6.1rc1/renku/command/format/dataset_tags.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/format/datasets.py` & `renku-2.6.1rc1/renku/command/format/datasets.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/format/json.py` & `renku-2.6.1rc1/renku/command/format/json.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/format/session.py` & `renku-2.6.1rc1/renku/command/format/session.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/format/tabulate.py` & `renku-2.6.1rc1/renku/command/format/tabulate.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/format/workflow.py` & `renku-2.6.1rc1/renku/command/format/workflow.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/gc.py` & `renku-2.6.1rc1/renku/command/gc.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/githooks.py` & `renku-2.6.1rc1/renku/command/githooks.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/graph.py` & `renku-2.6.1rc1/renku/command/graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/group.py` & `renku-2.6.1rc1/renku/command/group.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/init.py` & `renku-2.6.1rc1/renku/command/init.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/log.py` & `renku-2.6.1rc1/renku/command/log.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/login.py` & `renku-2.6.1rc1/renku/command/login.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/mergetool.py` & `renku-2.6.1rc1/renku/command/mergetool.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/migrate.py` & `renku-2.6.1rc1/renku/command/migrate.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/move.py` & `renku-2.6.1rc1/renku/command/move.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/options.py` & `renku-2.6.1rc1/renku/command/options.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/project.py` & `renku-2.6.1rc1/renku/command/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/remove.py` & `renku-2.6.1rc1/renku/command/remove.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/rerun.py` & `renku-2.6.1rc1/renku/command/rerun.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/rollback.py` & `renku-2.6.1rc1/renku/command/rollback.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/run.py` & `renku-2.6.1rc1/renku/command/run.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/save.py` & `renku-2.6.1rc1/renku/command/save.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/schema/__init__.py` & `renku-2.6.1rc1/renku/command/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/schema/__pycache__/agent.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/schema/__pycache__/agent.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2478 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 ae09 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 ae09 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6401  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 6d08 5a08 6d09 5a09  d.l.m.Z.m.Z.m.Z.
 00000060: 6d0a 5a0a 0100 6401 6405 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 6d0d 5a0d 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
```

### Comparing `renku-2.6.0rc1/renku/command/schema/__pycache__/annotation.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/schema/__pycache__/annotation.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1235 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 d304 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 d304 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6401 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6504 8303  ..G.d.d...d.e...
 00000070: 5a0a 6407 5300 2908 7a1a 416e 6e6f 7461  Z.d.S.).z.Annota
```

### Comparing `renku-2.6.0rc1/renku/command/schema/__pycache__/calamus.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/schema/__pycache__/calamus.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 8986 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 1a23 0000  a........^.d.#..
+00000000: 610d 0d0a 0000 0000 9f1b b064 1a23 0000  a..........d.#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 0c01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6401 6406 6c0c 6d0d 5a0d 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.6.0rc1/renku/command/schema/__pycache__/dataset.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/schema/__pycache__/dataset.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 8210 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 1220 0000  a........^.d. ..
+00000000: 610d 0d0a 0000 0000 9f1b b064 1220 0000  a..........d. ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/command/schema/__pycache__/entity.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/schema/__pycache__/entity.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1445 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 a505 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 a505 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6401  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c07 6d08 5a08 6d09 5a09 0100 4700  d.l.m.Z.m.Z...G.
 00000060: 6404 6405 8400 6405 6502 8303 5a0a 4700  d.d...d.e...Z.G.
 00000070: 6406 6407 8400 6407 650a 8303 5a0b 6408  d.d...d.e...Z.d.
```

### Comparing `renku-2.6.0rc1/renku/command/schema/activity.py` & `renku-2.6.1rc1/renku/command/schema/activity.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/schema/agent.py` & `renku-2.6.1rc1/renku/command/schema/agent.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/schema/annotation.py` & `renku-2.6.1rc1/renku/command/schema/annotation.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/schema/calamus.py` & `renku-2.6.1rc1/renku/command/schema/calamus.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/schema/composite_plan.py` & `renku-2.6.1rc1/renku/command/schema/composite_plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/schema/dataset.py` & `renku-2.6.1rc1/renku/command/schema/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/schema/entity.py` & `renku-2.6.1rc1/renku/command/schema/entity.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/schema/parameter.py` & `renku-2.6.1rc1/renku/command/schema/parameter.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/schema/plan.py` & `renku-2.6.1rc1/renku/command/schema/plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/schema/project.py` & `renku-2.6.1rc1/renku/command/schema/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/schema/workflow_file.py` & `renku-2.6.1rc1/renku/command/schema/workflow_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/session.py` & `renku-2.6.1rc1/renku/command/session.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/status.py` & `renku-2.6.1rc1/renku/command/status.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/storage.py` & `renku-2.6.1rc1/renku/command/storage.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/template.py` & `renku-2.6.1rc1/renku/command/template.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/update.py` & `renku-2.6.1rc1/renku/command/update.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/util.py` & `renku-2.6.1rc1/renku/command/util.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/version.py` & `renku-2.6.1rc1/renku/command/version.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/view_model/__init__.py` & `renku-2.6.1rc1/renku/command/view_model/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/view_model/__pycache__/activity_graph.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/view_model/__pycache__/activity_graph.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 14258 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 b237 0000  a........^.d.7..
+00000000: 610d 0d0a 0000 0000 9f1b b064 b237 0000  a..........d.7..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 0100 6401 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6401 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 0100 6401 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/command/view_model/__pycache__/agent.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/view_model/__pycache__/agent.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1657 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 7906 0000  a........^.dy...
+00000000: 610d 0d0a 0000 0000 9f1b b064 7906 0000  a..........dy...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000050: 8400 6405 8302 5a05 6406 5300 2907 7a11  ..d...Z.d.S.).z.
 00000060: 4167 656e 7420 7669 6577 206d 6f64 656c  Agent view model
 00000070: 2ee9 0000 0000 2901 da08 4f70 7469 6f6e  ......)...Option
@@ -55,15 +55,15 @@
 00000360: 6d5f 7065 7273 6f6e 2901 7208 0000 0063  m_person).r....c
 00000370: 0100 0000 0000 0000 0000 0000 0300 0000  ................
 00000380: 0300 0000 4300 0000 7342 0000 0064 0104  ....C...sB...d..
 00000390: 007d 017d 027c 006a 0072 1c64 027c 006a  .}.}.|.j.r.d.|.j
 000003a0: 009b 0064 039d 037d 017c 006a 0172 3064  ...d...}.|.j.r0d
 000003b0: 047c 006a 019b 0064 059d 037d 027c 006a  .|.j...d...}.|.j
 000003c0: 029b 007c 019b 007c 029b 009d 0353 0029  ...|...|.....S.)
-000003d0: 064e da00 7a02 203c da01 3e7a 0220 5bda  .N..z. <..>z. [.
+000003d0: 064e da00 7a02 203c da01 3e7a 0220 5bfa  .N..z. <..>z. [.
 000003e0: 015d 2903 7206 0000 0072 0700 0000 7205  .]).r....r....r.
 000003f0: 0000 0029 0372 0a00 0000 7206 0000 0072  ...).r....r....r
 00000400: 0700 0000 720b 0000 0072 0b00 0000 720c  ....r....r....r.
 00000410: 0000 00da 075f 5f73 7472 5f5f 2b00 0000  .....__str__+...
 00000420: 730c 0000 0000 0108 0206 010e 0206 010e  s...............
 00000430: 027a 1750 6572 736f 6e56 6965 774d 6f64  .z.PersonViewMod
 00000440: 656c 2e5f 5f73 7472 5f5f 290b da08 5f5f  el.__str__)...__
```

### Comparing `renku-2.6.0rc1/renku/command/view_model/__pycache__/composite_plan.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/view_model/__pycache__/composite_plan.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 8768 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 4022 0000  a........^.d@"..
+00000000: 610d 0d0a 0000 0000 9f1b b064 4022 0000  a..........d@"..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 3001 0000 5500  .....@...s0...U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6403  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d02 5a02 6d03 5a03 0100 6401 6404  l.m.Z.m.Z...d.d.
 00000050: 6c04 6d05 5a05 6d06 5a06 6d07 5a07 6d08  l.m.Z.m.Z.m.Z.m.
 00000060: 5a08 6d09 5a09 6d0a 5a0a 0100 6401 6405  Z.m.Z.m.Z...d.d.
 00000070: 6c0b 6d0c 5a0c 0100 6401 6406 6c0d 6d0e  l.m.Z...d.d.l.m.
```

### Comparing `renku-2.6.0rc1/renku/command/view_model/__pycache__/dataset.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/view_model/__pycache__/dataset.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2138 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 5a08 0000  a........^.dZ...
+00000000: 610d 0d0a 0000 0000 9f1b b064 5a08 0000  a..........dZ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 4700  d.l.m.Z.m.Z...G.
 00000050: 6404 6405 8400 6405 8302 5a06 4700 6406  d.d...d...Z.G.d.
 00000060: 6407 8400 6407 8302 5a07 6408 5300 2909  d...d...Z.d.S.).
 00000070: 7a1f 4461 7461 7365 742f 4461 7461 7365  z.Dataset/Datase
```

### Comparing `renku-2.6.0rc1/renku/command/view_model/__pycache__/log.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/view_model/__pycache__/log.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 12497 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 d130 0000  a........^.d.0..
+00000000: 610d 0d0a 0000 0000 9f1b b064 d130 0000  a..........d.0..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 1c01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d04 5a04 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6401 6406 6c0e  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/command/view_model/__pycache__/plan.cpython-39.pyc` & `renku-2.6.1rc1/renku/command/view_model/__pycache__/plan.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 9377 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 a124 0000  a........^.d.$..
+00000000: 610d 0d0a 0000 0000 9f1b b064 a124 0000  a..........d.$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 e400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6404 6c04 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6401 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 0100 6401  m.Z.m.Z.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 6401 6407 6c0d  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/command/view_model/activity_graph.py` & `renku-2.6.1rc1/renku/command/view_model/activity_graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/view_model/agent.py` & `renku-2.6.1rc1/renku/command/view_model/agent.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/view_model/composite_plan.py` & `renku-2.6.1rc1/renku/command/view_model/composite_plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/view_model/dataset.py` & `renku-2.6.1rc1/renku/command/view_model/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/view_model/graph.py` & `renku-2.6.1rc1/renku/command/view_model/graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/view_model/log.py` & `renku-2.6.1rc1/renku/command/view_model/log.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/view_model/plan.py` & `renku-2.6.1rc1/renku/command/view_model/plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/view_model/project.py` & `renku-2.6.1rc1/renku/command/view_model/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/view_model/template.py` & `renku-2.6.1rc1/renku/command/view_model/template.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/view_model/text_canvas.py` & `renku-2.6.1rc1/renku/command/view_model/text_canvas.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/view_model/workflow_file.py` & `renku-2.6.1rc1/renku/command/view_model/workflow_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/command/workflow.py` & `renku-2.6.1rc1/renku/command/workflow.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/__init__.py` & `renku-2.6.1rc1/renku/core/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/__pycache__/config.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/__pycache__/config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 6170 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 1a18 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 1a18 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6401 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6407 6408 8400 5a0b 6409 640a 8400  ..d.d...Z.d.d...
```

### Comparing `renku-2.6.0rc1/renku/core/__pycache__/constant.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/__pycache__/constant.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2717 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 9d0a 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 9d0a 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 d200 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6403  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 0100 6401 6404 6c04 6d05  l.m.Z...d.d.l.m.
 00000050: 5a05 0100 6405 5a06 6406 5a07 6407 5a08  Z...d.Z.d.Z.d.Z.
 00000060: 6408 5a09 6409 5a0a 6501 6a0b a00c 6507  d.Z.d.Z.e.j...e.
 00000070: 650a a102 5a0d 640a 5a0e 640b 5a0f 6510  e...Z.d.Z.d.Z.e.
```

### Comparing `renku-2.6.0rc1/renku/core/__pycache__/errors.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/__pycache__/errors.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 25658 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 3a64 0000  a........^.d:d..
+00000000: 610d 0d0a 0000 0000 9f1b b064 3a64 0000  a..........d:d..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5c06 0000 6400  .....@...s\...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6401 6404 6c07 5a07 6401 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6401 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 4700 6407 6408 8400 6408 650c 8303  ..G.d.d...d.e...
```

### Comparing `renku-2.6.0rc1/renku/core/__pycache__/git.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/__pycache__/git.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 7394 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 e21c 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 e21c 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 fc00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 0100 6401 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/__pycache__/login.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/__pycache__/login.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 10639 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 8f29 0000  a........^.d.)..
+00000000: 610d 0d0a 0000 0000 9f1b b064 8f29 0000  a..........d.)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 b201 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000060: 6d08 5a08 0100 6401 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6405 6c0b 6d0c 5a0c 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.6.0rc1/renku/core/__pycache__/storage.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/__pycache__/storage.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 19478 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 164c 0000  a........^.d.L..
+00000000: 610d 0d0a 0000 0000 9f1b b064 164c 0000  a..........d.L..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 2203 0000 6400  .....@...s"...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a06 6401 6403 6c07 6d08 5a08 0100 6401  Z.d.d.l.m.Z...d.
 00000070: 6404 6c09 6d0a 5a0a 0100 6401 6405 6c0b  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/core/config.py` & `renku-2.6.1rc1/renku/core/config.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/constant.py` & `renku-2.6.1rc1/renku/core/constant.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/__init__.py` & `renku-2.6.1rc1/renku/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/__pycache__/context.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/__pycache__/context.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2954 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 8a0b 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 8a0b 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6407 6c0b 6d0c 5a0c 0100 6401 6408 6c0d  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/__pycache__/dataset.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/__pycache__/dataset.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 50044 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 7cc3 0000  a........^.d|...
+00000000: 610d 0d0a 0000 0000 9f1b b064 7cc3 0000  a..........d|...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0013 0000 0040 0000 0073 1807 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/__pycache__/dataset_add.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/__pycache__/dataset_add.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 21429 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 b553 0000  a........^.d.S..
+00000000: 610d 0d0a 0000 0000 9f1b b064 b553 0000  a..........d.S..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0011 0000 0040 0000 0073 6403 0000 6400  .....@...sd...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 6401 6402 6c04 5a04 6401 6402 6c05  Z.d.d.l.Z.d.d.l.
 00000050: 5a05 6401 6403 6c06 6d07 5a07 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/__pycache__/datasets_provenance.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/__pycache__/datasets_provenance.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 9747 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 1326 0000  a........^.d.&..
+00000000: 610d 0d0a 0000 0000 9f1b b064 1326 0000  a..........d.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 0100 6401 6405 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/__pycache__/pointer_file.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/__pycache__/pointer_file.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 4296 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 c810 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 c810 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2001 0000 6400  .....@...s ...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 6d08 5a08  d.l.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6401 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/__pycache__/request_model.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/__pycache__/request_model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 3973 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 850f 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 850f 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 0100 6401 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/__pycache__/tag.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/__pycache__/tag.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 5361 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 f114 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 f114 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 de00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6401  m.Z.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6401 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6407 6c0c 6d0d 5a0d 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/context.py` & `renku-2.6.1rc1/renku/core/dataset/context.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/dataset.py` & `renku-2.6.1rc1/renku/core/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/dataset_add.py` & `renku-2.6.1rc1/renku/core/dataset/dataset_add.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/datasets_provenance.py` & `renku-2.6.1rc1/renku/core/dataset/datasets_provenance.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/pointer_file.py` & `renku-2.6.1rc1/renku/core/dataset/pointer_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/__init__.py` & `renku-2.6.1rc1/renku/core/dataset/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/api.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/api.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 16174 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 2e3f 0000  a........^.d.?..
+00000000: 610d 0d0a 0000 0000 9f1b b064 2e3f 0000  a..........d.?..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 c201 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6401 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/azure.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/azure.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 6987 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 4b1b 0000  a........^.dK...
+00000000: 610d 0d0a 0000 0000 9f1b b064 4b1b 0000  a..........dK...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 1401 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6405 6c0a 6d0b 5a0b 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  d.l.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/common.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/common.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2225 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 b108 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 b108 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 8200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6401 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6401 6408 6c0d  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/dataverse.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/dataverse.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 21202 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 d252 0000  a........^.d.R..
+00000000: 610d 0d0a 0000 0000 9f1b b064 d252 0000  a..........d.R..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 de01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 0100 6401 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/dataverse_metadata_templates.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/dataverse_metadata_templates.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 3742 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 9e0e 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 9e0e 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 1800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 5300 2906 7a1d 4461 7461 7665  Z.d.S.).z.Datave
 00000050: 7273 6520 6d65 7461 6461 7461 2074 656d  rse metadata tem
 00000060: 706c 6174 6573 2e61 e007 0000 0a7b 0a20  plates.a.....{. 
 00000070: 2020 2022 6461 7461 7365 7456 6572 7369     "datasetVersi
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/doi.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/doi.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 4829 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 dd12 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 dd12 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6401 6406 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6407 5a0e 4700  m.Z.m.Z...d.Z.G.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/external.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/external.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 5623 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 f715 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 f715 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0173 1001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6404 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6401  m.Z.m.Z.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 0100 6401 6407 6c0e  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/factory.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/factory.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 5764 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 8416 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 8416 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6401 6403 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6404 6c07 6d08 5a08 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 6d0e 5a0e 0100 6401 6406 6c0f  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/git.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/git.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 10563 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 4329 0000  a........^.dC)..
+00000000: 610d 0d0a 0000 0000 9f1b b064 4329 0000  a..........dC)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 3001 0000 6400  .....@...s0...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/local.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/local.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 14308 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 e437 0000  a........^.d.7..
+00000000: 610d 0d0a 0000 0000 9f1b b064 e437 0000  a..........d.7..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 2e01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6401 6405 6c0c 6d0d 5a0d 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/models.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/models.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 6292 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 9418 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 9418 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3601 0000 6400  .....@...s6...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6401 6404 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6401  m.Z.m.Z.m.Z...d.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/olos.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/olos.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 10118 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 8627 0000  a........^.d.'..
+00000000: 610d 0d0a 0000 0000 9f1b b064 8627 0000  a..........d.'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 f000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 6d08 5a08  d.l.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6405 6c02 6d09 5a0a 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 6d0d 5a0d 0100 6401  d.l.m.Z.m.Z...d.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/renku.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/renku.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 22167 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 9756 0000  a........^.d.V..
+00000000: 610d 0d0a 0000 0000 9f1b b064 9756 0000  a..........d.V..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2c01 0000 6400  .....@...s,...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 0100 6401  m.Z.m.Z.m.Z...d.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/repository.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/repository.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2553 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 f909 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 f909 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 6401  d.l.m.Z.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6506 7258 6401  d.l.m.Z...e.rXd.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6401 6407 6c0c  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/s3.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/s3.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 6413 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 0d19 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 0d19 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 0e01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6405 6c0a 6d0b 5a0b 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  d.l.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/web.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/web.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 9427 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 d324 0000  a........^.d.$..
+00000000: 610d 0d0a 0000 0000 9f1b b064 d324 0000  a..........d.$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 5c01 0000 6400  .....@...s\...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0a 5a0a 6d0b 5a0b 0100 6401 6405 6c0c  m.Z.m.Z...d.d.l.
 00000070: 6d0d 5a0d 0100 6401 6406 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/zenodo.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/dataset/providers/__pycache__/zenodo.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 18757 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 4549 0000  a........^.dEI..
+00000000: 610d 0d0a 0000 0000 9f1b b064 4549 0000  a..........dEI..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 8801 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6401 6405 6c0d  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/api.py` & `renku-2.6.1rc1/renku/core/dataset/providers/api.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/azure.py` & `renku-2.6.1rc1/renku/core/dataset/providers/azure.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/common.py` & `renku-2.6.1rc1/renku/core/dataset/providers/common.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/dataverse.py` & `renku-2.6.1rc1/renku/core/dataset/providers/dataverse.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/dataverse_metadata_templates.py` & `renku-2.6.1rc1/renku/core/dataset/providers/dataverse_metadata_templates.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/doi.py` & `renku-2.6.1rc1/renku/core/dataset/providers/doi.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/external.py` & `renku-2.6.1rc1/renku/core/dataset/providers/external.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/factory.py` & `renku-2.6.1rc1/renku/core/dataset/providers/factory.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/git.py` & `renku-2.6.1rc1/renku/core/dataset/providers/git.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/local.py` & `renku-2.6.1rc1/renku/core/dataset/providers/local.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/models.py` & `renku-2.6.1rc1/renku/core/dataset/providers/models.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/olos.py` & `renku-2.6.1rc1/renku/core/dataset/providers/olos.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/renku.py` & `renku-2.6.1rc1/renku/core/dataset/providers/renku.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/repository.py` & `renku-2.6.1rc1/renku/core/dataset/providers/repository.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/s3.py` & `renku-2.6.1rc1/renku/core/dataset/providers/s3.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/web.py` & `renku-2.6.1rc1/renku/core/dataset/providers/web.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/providers/zenodo.py` & `renku-2.6.1rc1/renku/core/dataset/providers/zenodo.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/request_model.py` & `renku-2.6.1rc1/renku/core/dataset/request_model.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/dataset/tag.py` & `renku-2.6.1rc1/renku/core/dataset/tag.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/errors.py` & `renku-2.6.1rc1/renku/core/errors.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/gc.py` & `renku-2.6.1rc1/renku/core/gc.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/git.py` & `renku-2.6.1rc1/renku/core/git.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/githooks.py` & `renku-2.6.1rc1/renku/core/githooks.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/init.py` & `renku-2.6.1rc1/renku/core/init.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/interface/__init__.py` & `renku-2.6.1rc1/renku/core/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/interface/__pycache__/activity_gateway.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/interface/__pycache__/activity_gateway.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 3741 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 9d0e 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 9d0e 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0a 5a0a 0100 6401 6405 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 6d0d 5a0d 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
```

### Comparing `renku-2.6.0rc1/renku/core/interface/__pycache__/database_gateway.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/interface/__pycache__/database_gateway.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1418 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 8a05 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 8a05 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6504  d.l.m.Z.m.Z...e.
 00000050: 7230 6401 6404 6c06 6d07 5a07 0100 4700  r0d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 6502 8303 5a08 6407  d.d...d.e...Z.d.
 00000070: 5300 2908 7a21 5265 6e6b 7520 6461 7461  S.).z!Renku data
```

### Comparing `renku-2.6.0rc1/renku/core/interface/__pycache__/dataset_gateway.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/interface/__pycache__/dataset_gateway.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2095 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 2f08 0000  a........^.d/...
+00000000: 610d 0d0a 0000 0000 9f1b b064 2f08 0000  a..........d/...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6504 7238 6401 6404 6c07 6d08 5a08  ..e.r8d.d.l.m.Z.
 00000060: 6d09 5a09 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000070: 6502 8303 5a0a 6407 5300 2908 7a20 5265  e...Z.d.S.).z Re
```

### Comparing `renku-2.6.0rc1/renku/core/interface/__pycache__/plan_gateway.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/interface/__pycache__/plan_gateway.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1996 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 cc07 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 cc07 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6401 6404 6c07 6d08 5a08 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 6502 8303 5a09 6407  d.d...d.e...Z.d.
 00000070: 5300 2908 7a1d 5265 6e6b 7520 706c 616e  S.).z.Renku plan
```

### Comparing `renku-2.6.0rc1/renku/core/interface/__pycache__/project_gateway.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/interface/__pycache__/project_gateway.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1212 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 bc04 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 bc04 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6504 722c 6401  d.l.m.Z...e.r,d.
 00000050: 6404 6c05 6d06 5a06 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000060: 8400 6406 6502 8303 5a07 6407 5300 2908  ..d.e...Z.d.S.).
 00000070: 7a20 5265 6e6b 7520 7072 6f6a 6563 7420  z Renku project
```

### Comparing `renku-2.6.0rc1/renku/core/interface/__pycache__/storage.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/interface/__pycache__/storage.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 4226 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 8210 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 8210 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6507  m.Z.m.Z.m.Z...e.
 00000070: 7254 6401 6406 6c0c 6d0d 5a0d 6d0e 5a0e  rTd.d.l.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/interface/__pycache__/workflow_file_parser.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/interface/__pycache__/workflow_file_parser.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1780 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 f406 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 f406 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 6600 0000 6400  .....@...sf...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6401  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6509  m.Z.m.Z.m.Z...e.
 00000070: 7250 6401 6406 6c0c 6d0d 5a0d 0100 4700  rPd.d.l.m.Z...G.
```

### Comparing `renku-2.6.0rc1/renku/core/interface/activity_gateway.py` & `renku-2.6.1rc1/renku/core/interface/activity_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/interface/database_gateway.py` & `renku-2.6.1rc1/renku/core/interface/database_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/interface/dataset_gateway.py` & `renku-2.6.1rc1/renku/core/interface/dataset_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/interface/plan_gateway.py` & `renku-2.6.1rc1/renku/core/interface/plan_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/interface/project_gateway.py` & `renku-2.6.1rc1/renku/core/interface/project_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/interface/storage.py` & `renku-2.6.1rc1/renku/core/interface/storage.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/interface/workflow_file_parser.py` & `renku-2.6.1rc1/renku/core/interface/workflow_file_parser.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/login.py` & `renku-2.6.1rc1/renku/core/login.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/__init__.py` & `renku-2.6.1rc1/renku/core/migration/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/m_0003__0_pyld2.py` & `renku-2.6.1rc1/renku/core/migration/m_0003__0_pyld2.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/m_0003__1_jsonld.py` & `renku-2.6.1rc1/renku/core/migration/m_0003__1_jsonld.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/m_0003__2_initial.py` & `renku-2.6.1rc1/renku/core/migration/m_0003__2_initial.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/m_0004__0_pyld2.py` & `renku-2.6.1rc1/renku/core/migration/m_0004__0_pyld2.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/m_0004__submodules.py` & `renku-2.6.1rc1/renku/core/migration/m_0004__submodules.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/m_0005__1_pyld2.py` & `renku-2.6.1rc1/renku/core/migration/m_0005__1_pyld2.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/m_0005__2_cwl.py` & `renku-2.6.1rc1/renku/core/migration/m_0005__2_cwl.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/m_0006__dataset_context.py` & `renku-2.6.1rc1/renku/core/migration/m_0006__dataset_context.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/m_0007__source_url.py` & `renku-2.6.1rc1/renku/core/migration/m_0007__source_url.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/m_0008__dataset_metadata.py` & `renku-2.6.1rc1/renku/core/migration/m_0008__dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/m_0009__new_metadata_storage.py` & `renku-2.6.1rc1/renku/core/migration/m_0009__new_metadata_storage.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/m_0010__metadata_fixes.py` & `renku-2.6.1rc1/renku/core/migration/m_0010__metadata_fixes.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/migrate.py` & `renku-2.6.1rc1/renku/core/migration/migrate.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/models/__init__.py` & `renku-2.6.1rc1/renku/core/migration/models/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/models/migration.py` & `renku-2.6.1rc1/renku/core/migration/models/migration.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/models/refs.py` & `renku-2.6.1rc1/renku/core/migration/models/refs.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/models/v10.py` & `renku-2.6.1rc1/renku/core/migration/models/v10.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/models/v3.py` & `renku-2.6.1rc1/renku/core/migration/models/v3.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/models/v7.py` & `renku-2.6.1rc1/renku/core/migration/models/v7.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/models/v8.py` & `renku-2.6.1rc1/renku/core/migration/models/v8.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/models/v9.py` & `renku-2.6.1rc1/renku/core/migration/models/v9.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/utils/__init__.py` & `renku-2.6.1rc1/renku/core/migration/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/migration/utils/__pycache__/__init__.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/migration/utils/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 7945 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 091f 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 091f 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 0c01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000060: 0100 6401 6404 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6401 6405 6c0d  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/core/migration/utils/conversion.py` & `renku-2.6.1rc1/renku/core/migration/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/plugin/__init__.py` & `renku-2.6.1rc1/renku/core/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/plugin/__pycache__/dataset_provider.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/plugin/__pycache__/dataset_provider.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1467 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 bb05 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 bb05 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6401 6403 6c05 5a05 6502  m.Z...d.d.l.Z.e.
 00000050: 7230 6401 6404 6c06 6d07 5a07 0100 6505  r0d.d.l.m.Z...e.
 00000060: a008 6405 a101 5a09 6509 6406 6407 9c01  ..d...Z.e.d.d...
 00000070: 6408 6409 8404 8301 5a0a 640a 6407 9c01  d.d.....Z.d.d...
```

### Comparing `renku-2.6.0rc1/renku/core/plugin/__pycache__/pluginmanager.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/plugin/__pycache__/pluginmanager.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1790 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 fe06 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 fe06 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6502 6403 8301 6404 6405  d.l.Z.e.d...d.d.
 00000050: 8400 8301 5a04 6403 5300 2906 7a14 706c  ....Z.d.S.).z.pl
 00000060: 7567 6779 2050 6c75 6769 6e20 7365 7475  uggy Plugin setu
 00000070: 702e e900 0000 0029 01da 096c 7275 5f63  p......)...lru_c
```

### Comparing `renku-2.6.0rc1/renku/core/plugin/__pycache__/provider.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/plugin/__pycache__/provider.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 3357 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 1d0d 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 1d0d 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 de00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6504 7238 6401  m.Z.m.Z...e.r8d.
 00000060: 6404 6c09 5a0a 6401 6404 6c0b 5a0b 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6405 6c0c 6d0d 5a0d 0100 6401 6406 6c0e  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/core/plugin/__pycache__/run.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/plugin/__pycache__/run.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1839 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 2f07 0000  a........^.d/...
+00000000: 610d 0d0a 0000 0000 9f1b b064 2f07 0000  a..........d/...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 5a00 6401 6402 6c01 5a01 6501 a002 6403  Z.d.d.l.Z.e...d.
 00000040: a101 5a03 6503 6404 6405 8400 8301 5a04  ..Z.e.d.d.....Z.
 00000050: 6503 6406 6407 8400 8301 5a05 6503 6408  e.d.d.....Z.e.d.
 00000060: 6409 8400 8301 5a06 6402 5300 290a 7a29  d.....Z.d.S.).z)
 00000070: 506c 7567 696e 2068 6f6f 6b73 2066 6f72  Plugin hooks for
```

### Comparing `renku-2.6.0rc1/renku/core/plugin/__pycache__/session.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/plugin/__pycache__/session.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1515 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 eb05 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 eb05 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 5a04 6401 6404 6c05  ..d.d.l.Z.d.d.l.
 00000050: 6d06 5a06 0100 6504 a007 6405 a101 5a08  m.Z...e...d...Z.
 00000060: 6508 6503 6506 6509 6602 1900 6406 9c01  e.e.e.e.f...d...
 00000070: 6407 6408 8404 8301 5a0a 6502 6506 1900  d.d.....Z.e.e...
```

### Comparing `renku-2.6.0rc1/renku/core/plugin/__pycache__/workflow.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/plugin/__pycache__/workflow.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 4195 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 6310 0000  a........^.dc...
+00000000: 610d 0d0a 0000 0000 9f1b b064 6310 0000  a..........dc...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 de00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6401 6404 6c08 5a08 6401  m.Z...d.d.l.Z.d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6401 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/plugin/__pycache__/workflow_file_parser.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/plugin/__pycache__/workflow_file_parser.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 3065 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 f90b 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 f90b 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6401 6404 6c08 5a08 6401  m.Z...d.d.l.Z.d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6401 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6504 7258 6401 6407 6c0d  m.Z...e.rXd.d.l.
```

### Comparing `renku-2.6.0rc1/renku/core/plugin/dataset_provider.py` & `renku-2.6.1rc1/renku/core/plugin/dataset_provider.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/plugin/implementations/__init__.py` & `renku-2.6.1rc1/renku/core/plugin/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/plugin/implementations/__pycache__/__init__.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/plugin/implementations/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 3046 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 e60b 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 e60b 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 ca01 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 6d02 5a02 6d03  d.Z.d.d.l.m.Z.m.
 00000040: 5a03 6d04 5a04 0100 6401 6403 6c05 6d06  Z.m.Z...d.d.l.m.
 00000050: 5a06 0100 6401 6404 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
 00000060: 6401 6405 6c09 6d0a 5a0a 0100 6401 6406  d.d.l.m.Z...d.d.
 00000070: 6c0b 6d0c 5a0c 0100 6401 6407 6c0d 6d0e  l.m.Z...d.d.l.m.
```

### Comparing `renku-2.6.0rc1/renku/core/plugin/pluginmanager.py` & `renku-2.6.1rc1/renku/core/plugin/pluginmanager.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/plugin/provider.py` & `renku-2.6.1rc1/renku/core/plugin/provider.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/plugin/run.py` & `renku-2.6.1rc1/renku/core/plugin/run.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/plugin/session.py` & `renku-2.6.1rc1/renku/core/plugin/session.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/plugin/workflow.py` & `renku-2.6.1rc1/renku/core/plugin/workflow.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/plugin/workflow_file_parser.py` & `renku-2.6.1rc1/renku/core/plugin/workflow_file_parser.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/project.py` & `renku-2.6.1rc1/renku/core/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/session/__init__.py` & `renku-2.6.1rc1/renku/core/session/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/session/__pycache__/docker.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/session/__pycache__/docker.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 22065 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 3156 0000  a........^.d1V..
+00000000: 610d 0d0a 0000 0000 9f1b b064 3156 0000  a..........d1V..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 0001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/session/__pycache__/renkulab.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/session/__pycache__/renkulab.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 21512 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 0854 0000  a........^.d.T..
+00000000: 610d 0d0a 0000 0000 9f1b b064 0854 0000  a..........d.T..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6401 6406 6c0a 6d0b 5a0b 6d0c 5a0c  ..d.d.l.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/session/__pycache__/utils.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/session/__pycache__/utils.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2206 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 9e08 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 9e08 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6401 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 650b 6407 9c01 6408 6409 8404 5a0c  ..e.d...d.d...Z.
```

### Comparing `renku-2.6.0rc1/renku/core/session/docker.py` & `renku-2.6.1rc1/renku/core/session/docker.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/session/renkulab.py` & `renku-2.6.1rc1/renku/core/session/renkulab.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/session/session.py` & `renku-2.6.1rc1/renku/core/session/session.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/session/utils.py` & `renku-2.6.1rc1/renku/core/session/utils.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/storage.py` & `renku-2.6.1rc1/renku/core/storage.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/template/__init__.py` & `renku-2.6.1rc1/renku/core/template/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/template/template.py` & `renku-2.6.1rc1/renku/core/template/template.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/template/usecase.py` & `renku-2.6.1rc1/renku/core/template/usecase.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/util/__init__.py` & `renku-2.6.1rc1/renku/core/util/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/util/__pycache__/communication.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/util/__pycache__/communication.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 10282 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 2a28 0000  a........^.d*(..
+00000000: 610d 0d0a 0000 0000 9f1b b064 2a28 0000  a..........d*(..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5201 0000 6400  .....@...sR...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000060: 8400 6406 8302 5a08 6407 6408 8400 5a09  ..d...Z.d.d...Z.
 00000070: 6409 640a 8400 5a0a 4700 640b 640c 8400  d.d...Z.G.d.d...
```

### Comparing `renku-2.6.0rc1/renku/core/util/__pycache__/contexts.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/util/__pycache__/contexts.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 6617 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 d919 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 d919 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 5601 0000 6400  .....@...sV...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 0100 6401 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/util/__pycache__/datetime8601.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/util/__pycache__/datetime8601.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2313 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 0909 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 0909 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d02 5a02 6d03 5a03 0100 6401 6404 6c04  m.Z.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6405 5a06 6501 a007 6506  m.Z...d.Z.e...e.
 00000060: a101 6a08 5a09 6406 6407 8400 5a0a 6408  ..j.Z.d.d...Z.d.
 00000070: 6409 8400 5a0b 6505 6502 1900 640a 9c01  d...Z.e.e...d...
```

### Comparing `renku-2.6.0rc1/renku/core/util/__pycache__/doi.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/util/__pycache__/doi.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1376 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 6005 0000  a........^.d`...
+00000000: 610d 0d0a 0000 0000 9f1b b064 6005 0000  a..........d`...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6501 6a03 6403 6501 6a04 6404 8d02  Z.e.j.d.e.j.d...
 00000050: 5a05 6405 6406 8400 5a06 6407 6408 8400  Z.d.d...Z.d.d...
 00000060: 5a07 6508 6409 9c01 640a 640b 8404 5a09  Z.e.d...d.d...Z.
 00000070: 6402 5300 290c 7a23 4865 6c70 6572 2075  d.S.).z#Helper u
```

### Comparing `renku-2.6.0rc1/renku/core/util/__pycache__/git.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/util/__pycache__/git.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 40689 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 f19e 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 f19e 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 5c04 0000 5500  .....@...s\...U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6402  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 5a02 6401 6402 6c03 5a03 6401 6402  l.Z.d.d.l.Z.d.d.
 00000050: 6c04 5a04 6401 6402 6c05 5a05 6401 6402  l.Z.d.d.l.Z.d.d.
 00000060: 6c06 5a06 6401 6402 6c07 5a07 6401 6402  l.Z.d.d.l.Z.d.d.
 00000070: 6c08 5a08 6401 6403 6c09 6d0a 5a0a 0100  l.Z.d.d.l.m.Z...
@@ -627,17 +627,17 @@
 00002720: 2020 2020 2020 2020 7061 7468 2855 6e69          path(Uni
 00002730: 6f6e 5b50 6174 682c 2073 7472 5d29 3a20  on[Path, str]): 
 00002740: 5468 6520 7061 7468 2074 6f20 6368 6563  The path to chec
 00002750: 6b2e 0a0a 2020 2020 5265 7475 726e 733a  k...    Returns:
 00002760: 0a20 2020 2020 2020 2062 6f6f 6c3a 2054  .        bool: T
 00002770: 7275 6520 6966 2074 6865 2070 6174 6820  rue if the path 
 00002780: 6973 2073 6166 6520 656c 7365 2046 616c  is safe else Fal
-00002790: 7365 2e0a 2020 2020 3e02 0000 007a 0a2e  se..    >....z..
-000027a0: 6769 7469 676e 6f72 657a 0e2e 6769 7461  gitignorez..gita
-000027b0: 7474 7269 6275 7465 7346 7a06 2e72 656e  ttributesFz..ren
+00002790: 7365 2e0a 2020 2020 3e02 0000 007a 0e2e  se..    >....z..
+000027a0: 6769 7461 7474 7269 6275 7465 737a 0a2e  gitattributesz..
+000027b0: 6769 7469 676e 6f72 6546 7a06 2e72 656e  gitignoreFz..ren
 000027c0: 6b75 5429 02da 0373 7472 725b 0000 00a9  kuT)...strr[....
 000027d0: 0172 3700 0000 722e 0000 0072 2e00 0000  .r7...r....r....
 000027e0: 722f 0000 00da 0c69 735f 7061 7468 5f73  r/.....is_path_s
 000027f0: 6166 655d 0100 0073 0c00 0000 0009 0803  afe]...s........
 00002800: 0801 0403 0a01 0402 7293 0000 0046 7214  ........r....Fr.
 00002810: 0000 0029 0672 3100 0000 7237 0000 00da  ...).r1...r7....
 00002820: 0872 6576 6973 696f 6eda 0c62 7970 6173  .revision..bypas
```

### Comparing `renku-2.6.0rc1/renku/core/util/__pycache__/jwt.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/util/__pycache__/jwt.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1244 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 dc04 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 dc04 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 6d02 5a02  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c03 5a03 6504 6505 6404  ..d.d.l.Z.e.e.d.
 00000050: 9c02 6405 6406 8404 5a06 6403 5300 2907  ..d.d...Z.d.S.).
 00000060: 7a0e 4a57 5420 7574 696c 6974 6965 732e  z.JWT utilities.
 00000070: e900 0000 0029 02da 0864 6174 6574 696d  .....)...datetim
```

### Comparing `renku-2.6.0rc1/renku/core/util/__pycache__/metadata.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/util/__pycache__/metadata.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 7036 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 7c1b 0000  a........^.d|...
+00000000: 610d 0d0a 0000 0000 9f1b b064 7c1b 0000  a..........d|...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 1e02 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6401 6405 6c0d  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/core/util/__pycache__/os.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/util/__pycache__/os.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 12140 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 6c2f 0000  a........^.dl/..
+00000000: 610d 0d0a 0000 0000 9f1b b064 6c2f 0000  a..........dl/..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0015 0000 0040 0000 0073 5a03 0000 6400  .....@...sZ...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a06 6401 6402 6c07 5a07 6401 6402 6c08  Z.d.d.l.Z.d.d.l.
 00000070: 5a08 6401 6403 6c09 6d0a 5a0a 0100 6401  Z.d.d.l.m.Z...d.
```

### Comparing `renku-2.6.0rc1/renku/core/util/__pycache__/requests.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/util/__pycache__/requests.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 7626 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 ca1d 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 ca1d 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 5801 0000 6400  .....@...sX...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c08 6d09 5a09 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6402 6c0a 5a0a 6401 6402 6c0b 5a0b 6401  d.l.Z.d.d.l.Z.d.
```

### Comparing `renku-2.6.0rc1/renku/core/util/__pycache__/ssh.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/util/__pycache__/ssh.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 6871 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 d71a 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 d71a 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ac00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 6401 6403 6c04 6d05 5a05 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 6d08 5a08 6d09 5a09  d.l.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6405 6c0a 6d0b 5a0c 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c0d 6d0e 5a0e 0100 6401 6407 6c0f  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/core/util/__pycache__/tabulate.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/util/__pycache__/tabulate.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2158 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 6e08 0000  a........^.dn...
+00000000: 610d 0d0a 0000 0000 9f1b b064 6e08 0000  a..........dn...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 0100 640c 6405 6406  d.l.m.Z...d.d.d.
 00000050: 8401 5a04 640d 6408 6409 8401 5a05 640a  ..Z.d.d.d...Z.d.
 00000060: 640b 8400 5a06 6404 5300 290e 7a1e 5072  d...Z.d.S.).z.Pr
 00000070: 696e 7420 6120 636f 6c6c 6563 7469 6f6e  int a collection
```

### Comparing `renku-2.6.0rc1/renku/core/util/__pycache__/urls.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/util/__pycache__/urls.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 6228 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 5418 0000  a........^.dT...
+00000000: 610d 0d0a 0000 0000 9f1b b064 5418 0000  a..........dT...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 4601 0000 6400  .....@...sF...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6401 6405 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/util/__pycache__/util.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/util/__pycache__/util.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 3878 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 260f 0000  a........^.d&...
+00000000: 610d 0d0a 0000 0000 9f1b b064 260f 0000  a..........d&...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 f200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 6401 6402 6c04 5a04 6401 6403 6c05  Z.d.d.l.Z.d.d.l.
 00000050: 6d06 5a06 0100 6401 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 0100 6401 6402 6c0e 5a0e 6401  m.Z...d.d.l.Z.d.
```

### Comparing `renku-2.6.0rc1/renku/core/util/__pycache__/yaml.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/util/__pycache__/yaml.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2836 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 140b 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 140b 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 5a05 7a1c 6401 6405 6c05 6d06 5a07 0100  Z.z.d.d.l.m.Z...
 00000060: 6401 6406 6c05 6d08 5a09 0100 5700 6e22  d.d.l.m.Z...W.n"
 00000070: 0400 650a 7962 0100 0100 0100 6401 6407  ..e.yb......d.d.
```

### Comparing `renku-2.6.0rc1/renku/core/util/communication.py` & `renku-2.6.1rc1/renku/core/util/communication.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/util/contexts.py` & `renku-2.6.1rc1/renku/core/util/contexts.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/util/datetime8601.py` & `renku-2.6.1rc1/renku/core/util/datetime8601.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/util/doi.py` & `renku-2.6.1rc1/renku/core/util/doi.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/util/git.py` & `renku-2.6.1rc1/renku/core/util/git.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/util/jwt.py` & `renku-2.6.1rc1/renku/core/util/jwt.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/util/metadata.py` & `renku-2.6.1rc1/renku/core/util/metadata.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/util/os.py` & `renku-2.6.1rc1/renku/core/util/os.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/util/requests.py` & `renku-2.6.1rc1/renku/core/util/requests.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/util/shacl.py` & `renku-2.6.1rc1/renku/core/util/shacl.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/util/ssh.py` & `renku-2.6.1rc1/renku/core/util/ssh.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/util/tabulate.py` & `renku-2.6.1rc1/renku/core/util/tabulate.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/util/urls.py` & `renku-2.6.1rc1/renku/core/util/urls.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/util/util.py` & `renku-2.6.1rc1/renku/core/util/util.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/util/yaml.py` & `renku-2.6.1rc1/renku/core/util/yaml.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/__init__.py` & `renku-2.6.1rc1/renku/core/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/__pycache__/activity.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/workflow/__pycache__/activity.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 22713 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 b958 0000  a........^.d.X..
+00000000: 610d 0d0a 0000 0000 9f1b b064 b958 0000  a..........d.X..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 4402 0000 6400  .....@...sD...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/workflow/__pycache__/execute.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/workflow/__pycache__/execute.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 18756 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 4449 0000  a........^.dDI..
+00000000: 610d 0d0a 0000 0000 9f1b b064 4449 0000  a..........dDI..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 8402 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6401  m.Z.m.Z.m.Z...d.
@@ -230,15 +230,15 @@
 00000e50: a101 a101 0100 7114 6408 7d06 7c06 6409  ......q.d.}.|.d.
 00000e60: a009 7c01 a101 3700 7d06 740a 6a0b 7c06  ..|...7.}.t.j.|.
 00000e70: 6700 640a 8d02 8201 6401 5300 290b 7a43  g.d.....d.S.).zC
 00000e80: 4368 6563 6b20 666f 7220 6379 636c 6573  Check for cycles
 00000e90: 2069 6e20 7468 6520 6772 6170 6820 616e   in the graph an
 00000ea0: 6420 7261 6973 6573 2061 6e20 6572 726f  d raises an erro
 00000eb0: 7220 6966 2074 6865 7265 2061 7265 2061  r if there are a
-00000ec0: 6e79 2e4e da01 5bda 015d da07 436f 6d6d  ny.N..[..]..Comm
+00000ec0: 6e79 2e4e da01 5bfa 015d da07 436f 6d6d  ny.N..[..]..Comm
 00000ed0: 616e 64da 007a 023a 207a 0420 2d3e 207a  and..z.: z. -> z
 00000ee0: 4c43 6972 6375 6c61 7220 776f 726b 666c  LCircular workfl
 00000ef0: 6f77 7320 6172 6520 6e6f 7420 7375 7070  ows are not supp
 00000f00: 6f72 7465 6420 696e 2052 656e 6b75 2e20  orted in Renku. 
 00000f10: 506c 6561 7365 2072 656d 6f76 6520 7468  Please remove th
 00000f20: 6573 6520 6379 636c 6573 3a0a 097a 020a  ese cycles:..z..
 00000f30: 0929 02da 076d 6573 7361 6765 da06 6379  .)...message..cy
```

### Comparing `renku-2.6.0rc1/renku/core/workflow/__pycache__/plan.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/workflow/__pycache__/plan.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 34209 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 a185 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 a185 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0016 0000 0040 0000 0073 2406 0000 6400  .....@...s$...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d03 5a03 6d04 5a04  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6401 6404 6c05 6d06 5a06 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6405 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/workflow/__pycache__/plan_factory.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/workflow/__pycache__/plan_factory.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 33046 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 1681 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 1681 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 ee01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000070: 6d09 5a09 0100 6401 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/workflow/__pycache__/run.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/workflow/__pycache__/run.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 14384 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 3038 0000  a........^.d08..
+00000000: 610d 0d0a 0000 0000 9f1b b064 3038 0000  a..........d08..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 ee01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6401 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6407 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/workflow/__pycache__/types.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/workflow/__pycache__/types.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1681 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 9106 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 9106 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 4700 6405 6406  m.Z.m.Z...G.d.d.
 00000060: 8400 6406 8302 5a08 4700 6407 6408 8400  ..d...Z.G.d.d...
 00000070: 6408 6508 8303 5a09 4700 6409 640a 8400  d.e...Z.G.d.d...
```

### Comparing `renku-2.6.0rc1/renku/core/workflow/__pycache__/value_resolution.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/workflow/__pycache__/value_resolution.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 8335 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 8f20 0000  a........^.d. ..
+00000000: 610d 0d0a 0000 0000 9f1b b064 8f20 0000  a..........d. ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 e800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6401 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/workflow/__pycache__/workflow_file.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/workflow/__pycache__/workflow_file.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 5089 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 e113 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 e113 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0173 3401 0000 6400  .....@...s4...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6404 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 0100 6401 6403 6c0a 5a0b 6401  m.Z...d.d.l.Z.d.
 00000070: 6406 6c0c 6d0d 5a0d 0100 6401 6407 6c0e  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/core/workflow/activity.py` & `renku-2.6.1rc1/renku/core/workflow/activity.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/converters/__init__.py` & `renku-2.6.1rc1/renku/core/workflow/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/converters/__pycache__/cwl.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/workflow/converters/__pycache__/cwl.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 17937 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 1146 0000  a........^.d.F..
+00000000: 610d 0d0a 0000 0000 9f1b b064 1146 0000  a..........d.F..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2601 0000 6400  .....@...s&...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6401 6405 6c0e  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/core/workflow/converters/__pycache__/renku.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/workflow/converters/__pycache__/renku.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 5142 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 1614 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 1614 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6401 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/workflow/converters/cwl.py` & `renku-2.6.1rc1/renku/core/workflow/converters/cwl.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/converters/renku.py` & `renku-2.6.1rc1/renku/core/workflow/converters/renku.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/execute.py` & `renku-2.6.1rc1/renku/core/workflow/execute.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/model/__init__.py` & `renku-2.6.1rc1/renku/core/workflow/model/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/model/__pycache__/concrete_execution_graph.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/workflow/model/__pycache__/concrete_execution_graph.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 6530 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 8219 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 8219 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6405 6c0a 5a0b 6401 6406 6c0c  ..d.d.l.Z.d.d.l.
 00000070: 6d0d 5a0d 0100 6401 6407 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/workflow/model/__pycache__/workflow_file.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/workflow/model/__pycache__/workflow_file.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 37866 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 ea93 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 ea93 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0173 1802 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6404 6c04 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6401 6405 6c05 6d06 5a06 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6406 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/core/workflow/model/concrete_execution_graph.py` & `renku-2.6.1rc1/renku/core/workflow/model/concrete_execution_graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/model/workflow_file.py` & `renku-2.6.1rc1/renku/core/workflow/model/workflow_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/parser/__init__.py` & `renku-2.6.1rc1/renku/core/workflow/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/parser/__pycache__/renku.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/workflow/parser/__pycache__/renku.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 10631 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 8729 0000  a........^.d.)..
+00000000: 610d 0d0a 0000 0000 9f1b b064 8729 0000  a..........d.)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0173 3e01 0000 6400  .....@...s>...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6401 6405 6c0e 6d0f 5a0f 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.6.0rc1/renku/core/workflow/parser/renku.py` & `renku-2.6.1rc1/renku/core/workflow/parser/renku.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/plan.py` & `renku-2.6.1rc1/renku/core/workflow/plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/plan_factory.py` & `renku-2.6.1rc1/renku/core/workflow/plan_factory.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/providers/__init__.py` & `renku-2.6.1rc1/renku/core/workflow/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/providers/__pycache__/cwltool.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/workflow/providers/__pycache__/cwltool.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 5999 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 6f17 0000  a........^.do...
+00000000: 610d 0d0a 0000 0000 9f1b b064 6f17 0000  a..........do...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 0100 6401  d.l.m.Z.m.Z...d.
 00000070: 6405 6c0a 6d0b 5a0b 0100 6401 6406 6c0c  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/core/workflow/providers/__pycache__/local.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/workflow/providers/__pycache__/local.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 4271 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 af10 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 af10 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 0601 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 0100 6401 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 0100 6401  m.Z.m.Z.m.Z...d.
```

### Comparing `renku-2.6.0rc1/renku/core/workflow/providers/__pycache__/toil.cpython-39.pyc` & `renku-2.6.1rc1/renku/core/workflow/providers/__pycache__/toil.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 13372 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 3c34 0000  a........^.d<4..
+00000000: 610d 0d0a 0000 0000 9f1b b064 3c34 0000  a..........d<4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 0a02 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 0100 6401 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6405 6c0a 6d0b 5a0b 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.6.0rc1/renku/core/workflow/providers/cwltool.py` & `renku-2.6.1rc1/renku/core/workflow/providers/cwltool.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/providers/local.py` & `renku-2.6.1rc1/renku/core/workflow/providers/local.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/providers/toil.py` & `renku-2.6.1rc1/renku/core/workflow/providers/toil.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/run.py` & `renku-2.6.1rc1/renku/core/workflow/run.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/types.py` & `renku-2.6.1rc1/renku/core/workflow/types.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/update.py` & `renku-2.6.1rc1/renku/core/workflow/update.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/value_resolution.py` & `renku-2.6.1rc1/renku/core/workflow/value_resolution.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/core/workflow/workflow_file.py` & `renku-2.6.1rc1/renku/core/workflow/workflow_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/data/__init__.py` & `renku-2.6.1rc1/renku/data/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/data/gitignore.default` & `renku-2.6.1rc1/renku/data/gitignore.default`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/data/pre-commit.sh` & `renku-2.6.1rc1/renku/data/pre-commit.sh`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/data/shacl_shape.json` & `renku-2.6.1rc1/renku/data/shacl_shape.json`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/__init__.py` & `renku-2.6.1rc1/renku/domain_model/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/__pycache__/dataset.cpython-39.pyc` & `renku-2.6.1rc1/renku/domain_model/__pycache__/dataset.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 29611 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 ab73 0000  a........^.d.s..
+00000000: 610d 0d0a 0000 0000 9f1b b064 ab73 0000  a..........d.s..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 4e02 0000 6400  .....@...sN...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/domain_model/__pycache__/dataset_provider.cpython-39.pyc` & `renku-2.6.1rc1/renku/domain_model/__pycache__/dataset_provider.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1267 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 f304 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 f304 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6503 722c 6401  m.Z.m.Z...e.r,d.
 00000050: 6404 6c05 6d06 5a06 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000060: 8400 6406 6501 6a07 8303 5a08 6402 5300  ..d.e.j...Z.d.S.
 00000070: 2907 7a12 4461 7461 7365 7420 7072 6f76  ).z.Dataset prov
```

### Comparing `renku-2.6.0rc1/renku/domain_model/__pycache__/datastructures.cpython-39.pyc` & `renku-2.6.1rc1/renku/domain_model/__pycache__/datastructures.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2754 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 c20a 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 c20a 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
 00000070: 650a 8303 5a0b 6402 5300 2908 7a32 4261  e...Z.d.S.).z2Ba
```

### Comparing `renku-2.6.0rc1/renku/domain_model/__pycache__/entity.cpython-39.pyc` & `renku-2.6.1rc1/renku/domain_model/__pycache__/entity.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2499 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 c309 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 c309 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6405 6c0a 6d0b 5a0b 0100 6401 6406 6c0c  d.l.m.Z...d.d.l.
 00000070: 6d0d 5a0d 0100 4700 6407 6408 8400 6408  m.Z...G.d.d...d.
```

### Comparing `renku-2.6.0rc1/renku/domain_model/__pycache__/enums.cpython-39.pyc` & `renku-2.6.1rc1/renku/domain_model/__pycache__/enums.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 971 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 cb03 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 cb03 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2400 0000 6400  .....@...s$...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 4700  Z.d.d.l.m.Z...G.
 00000040: 6403 6404 8400 6404 6502 8303 5a03 6405  d.d...d.e...Z.d.
 00000050: 5300 2906 7a14 456e 756d 7320 7573 6564  S.).z.Enums used
 00000060: 2069 6e20 7265 6e6b 752e e900 0000 0029   in renku......)
 00000070: 01da 0445 6e75 6d63 0000 0000 0000 0000  ...Enumc........
```

### Comparing `renku-2.6.0rc1/renku/domain_model/__pycache__/project.cpython-39.pyc` & `renku-2.6.1rc1/renku/domain_model/__pycache__/project.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 8329 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 8920 0000  a........^.d. ..
+00000000: 610d 0d0a 0000 0000 9f1b b064 8920 0000  a..........d. ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 fc00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d03 5a03 0100 6401 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 0100 6401 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6406 6c0c 5a0c 6401 6407 6c0d  ..d.d.l.Z.d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/domain_model/__pycache__/project_context.cpython-39.pyc` & `renku-2.6.1rc1/renku/domain_model/__pycache__/project_context.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 11817 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 292e 0000  a........^.d)...
+00000000: 610d 0d0a 0000 0000 9f1b b064 292e 0000  a..........d)...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1601 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6402  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 5a02 6401 6402 6c03 5a03 6401 6403  l.Z.d.d.l.Z.d.d.
 00000050: 6c04 6d05 5a05 0100 6401 6404 6c06 6d07  l.m.Z...d.d.l.m.
 00000060: 5a07 0100 6401 6405 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000070: 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e  Z.m.Z.m.Z.m.Z.m.
```

### Comparing `renku-2.6.0rc1/renku/domain_model/__pycache__/session.cpython-39.pyc` & `renku-2.6.1rc1/renku/domain_model/__pycache__/session.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 6871 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 d71a 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 d71a 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 b800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6401  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6401 6406 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6401 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/domain_model/constant.py` & `renku-2.6.1rc1/renku/domain_model/constant.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/dataset.py` & `renku-2.6.1rc1/renku/domain_model/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/dataset_provider.py` & `renku-2.6.1rc1/renku/domain_model/dataset_provider.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/datastructures.py` & `renku-2.6.1rc1/renku/domain_model/datastructures.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/entity.py` & `renku-2.6.1rc1/renku/domain_model/entity.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/enums.py` & `renku-2.6.1rc1/renku/domain_model/enums.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/git.py` & `renku-2.6.1rc1/renku/domain_model/git.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/project.py` & `renku-2.6.1rc1/renku/domain_model/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/project_context.py` & `renku-2.6.1rc1/renku/domain_model/project_context.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/provenance/__init__.py` & `renku-2.6.1rc1/renku/domain_model/provenance/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/provenance/__pycache__/activity.cpython-39.pyc` & `renku-2.6.1rc1/renku/domain_model/provenance/__pycache__/activity.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 13200 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 9033 0000  a........^.d.3..
+00000000: 610d 0d0a 0000 0000 9f1b b064 9033 0000  a..........d.3..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8201 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 0100 6401 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 0100 6401 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6406 6c0c 5a0c 6401 6407 6c0d  ..d.d.l.Z.d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/domain_model/provenance/__pycache__/agent.cpython-39.pyc` & `renku-2.6.1rc1/renku/domain_model/provenance/__pycache__/agent.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 5155 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 2314 0000  a........^.d#...
+00000000: 610d 0d0a 0000 0000 9f1b b064 2314 0000  a..........d#...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6401 6404 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6401 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 4700 6407 6408  m.Z.m.Z...G.d.d.
```

### Comparing `renku-2.6.0rc1/renku/domain_model/provenance/__pycache__/annotation.cpython-39.pyc` & `renku-2.6.1rc1/renku/domain_model/provenance/__pycache__/annotation.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1268 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 f404 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 f404 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000050: 8302 5a04 6402 5300 2906 7a27 5265 7072  ..Z.d.S.).z'Repr
 00000060: 6573 656e 7420 616e 2061 6e6e 6f74 6174  esent an annotat
 00000070: 696f 6e20 666f 7220 6120 776f 726b 666c  ion for a workfl
```

### Comparing `renku-2.6.0rc1/renku/domain_model/provenance/__pycache__/parameter.cpython-39.pyc` & `renku-2.6.1rc1/renku/domain_model/provenance/__pycache__/parameter.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1530 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 fa05 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 fa05 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000060: 8302 5a07 6407 5300 2908 7a34 436c 6173  ..Z.d.S.).z4Clas
 00000070: 7365 7320 666f 7220 7472 6163 6b69 6e67  ses for tracking
```

### Comparing `renku-2.6.0rc1/renku/domain_model/provenance/activity.py` & `renku-2.6.1rc1/renku/domain_model/provenance/activity.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/provenance/agent.py` & `renku-2.6.1rc1/renku/domain_model/provenance/agent.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/provenance/annotation.py` & `renku-2.6.1rc1/renku/domain_model/provenance/annotation.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/provenance/parameter.py` & `renku-2.6.1rc1/renku/domain_model/provenance/parameter.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/session.py` & `renku-2.6.1rc1/renku/domain_model/session.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/sort.py` & `renku-2.6.1rc1/renku/domain_model/sort.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/template.py` & `renku-2.6.1rc1/renku/domain_model/template.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/workflow/__init__.py` & `renku-2.6.1rc1/renku/domain_model/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/composite_plan.cpython-39.pyc` & `renku-2.6.1rc1/renku/domain_model/workflow/__pycache__/composite_plan.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 15917 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 2d3e 0000  a........^.d->..
+00000000: 610d 0d0a 0000 0000 9f1b b064 2d3e 0000  a..........d->..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6401 6406 6c0e  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/parameter.cpython-39.pyc` & `renku-2.6.1rc1/renku/domain_model/workflow/__pycache__/parameter.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 18124 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 cc46 0000  a........^.d.F..
+00000000: 610d 0d0a 0000 0000 9f1b b064 cc46 0000  a..........d.F..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2601 0000 6400  .....@...s&...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 0100 6401 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 0100 6401  m.Z.m.Z.m.Z...d.
```

### Comparing `renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/plan.cpython-39.pyc` & `renku-2.6.1rc1/renku/domain_model/workflow/__pycache__/plan.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 16602 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 da40 0000  a........^.d.@..
+00000000: 610d 0d0a 0000 0000 9f1b b064 da40 0000  a..........d.@..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 3201 0000 6400  .....@...s2...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/provider.cpython-39.pyc` & `renku-2.6.1rc1/renku/domain_model/workflow/__pycache__/provider.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1639 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 6706 0000  a........^.dg...
+00000000: 610d 0d0a 0000 0000 9f1b b064 6706 0000  a..........dg...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 6600 0000 6400  .....@...sf...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6401  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6509 7250 6401 6406 6c0d 5a0e 4700  ..e.rPd.d.l.Z.G.
```

### Comparing `renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/workflow_file.cpython-39.pyc` & `renku-2.6.1rc1/renku/domain_model/workflow/__pycache__/workflow_file.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 4660 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 3412 0000  a........^.d4...
+00000000: 610d 0d0a 0000 0000 9f1b b064 3412 0000  a..........d4...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 8000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a04 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 0100 6401  m.Z.m.Z.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 6401 6407 6c0d  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/domain_model/workflow/composite_plan.py` & `renku-2.6.1rc1/renku/domain_model/workflow/composite_plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/workflow/converters/__init__.py` & `renku-2.6.1rc1/renku/domain_model/workflow/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/workflow/converters/__pycache__/__init__.cpython-39.pyc` & `renku-2.6.1rc1/renku/domain_model/workflow/converters/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1531 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 fb05 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 fb05 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 6200 0000 6400  .....@...sb...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6401  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6401  m.Z.m.Z.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 0100 4700 6407 6408  d.l.m.Z...G.d.d.
```

### Comparing `renku-2.6.0rc1/renku/domain_model/workflow/parameter.py` & `renku-2.6.1rc1/renku/domain_model/workflow/parameter.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/workflow/plan.py` & `renku-2.6.1rc1/renku/domain_model/workflow/plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/workflow/provider.py` & `renku-2.6.1rc1/renku/domain_model/workflow/provider.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/domain_model/workflow/workflow_file.py` & `renku-2.6.1rc1/renku/domain_model/workflow/workflow_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/infrastructure/__init__.py` & `renku-2.6.1rc1/renku/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/infrastructure/__pycache__/database.cpython-39.pyc` & `renku-2.6.1rc1/renku/infrastructure/__pycache__/database.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 41333 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 75a1 0000  a........^.du...
+00000000: 610d 0d0a 0000 0000 9f1b b064 75a1 0000  a..........du...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2602 0000 6400  .....@...s&...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 0100 6401 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6405 6c0a 6d0b 5a0b 6d0c 5a0c  ..d.d.l.m.Z.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/infrastructure/__pycache__/immutable.cpython-39.pyc` & `renku-2.6.1rc1/renku/infrastructure/__pycache__/immutable.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 4969 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 6913 0000  a........^.di...
+00000000: 610d 0d0a 0000 0000 9f1b b064 6913 0000  a..........di...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 4700 6404 6405 8400 6405 8302 5a06  ..G.d.d...d...Z.
 00000060: 4700 6406 6407 8400 6407 6506 8303 5a07  G.d.d...d.e...Z.
 00000070: 4700 6408 6409 8400 6409 8302 5a08 6402  G.d.d...d...Z.d.
```

### Comparing `renku-2.6.0rc1/renku/infrastructure/__pycache__/persistent.cpython-39.pyc` & `renku-2.6.1rc1/renku/infrastructure/__pycache__/persistent.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2394 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 5a09 0000  a........^.dZ...
+00000000: 610d 0d0a 0000 0000 9f1b b064 5a09 0000  a..........dZ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 5a00 6401 6402 6c01 5a01 4700 6403 6404  Z.d.d.l.Z.G.d.d.
 00000040: 8400 6404 6501 6a02 8303 5a02 6402 5300  ..d.e.j...Z.d.S.
 00000050: 2905 7a1c 4261 7365 2052 656e 6b75 2070  ).z.Base Renku p
 00000060: 6572 7369 7374 656e 7420 636c 6173 732e  ersistent class.
 00000070: e900 0000 004e 6300 0000 0000 0000 0000  .....Nc.........
```

### Comparing `renku-2.6.0rc1/renku/infrastructure/__pycache__/repository.cpython-39.pyc` & `renku-2.6.1rc1/renku/infrastructure/__pycache__/repository.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 72047 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 6f19 0100  a........^.do...
+00000000: 610d 0d0a 0000 0000 9f1b b064 6f19 0100  a..........do...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 fc02 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a06 6401 6402 6c07 5a07 6401 6403 6c08  Z.d.d.l.Z.d.d.l.
 00000070: 6d09 5a09 0100 6401 6404 6c0a 6d0a 5a0a  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/infrastructure/database.py` & `renku-2.6.1rc1/renku/infrastructure/database.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/infrastructure/gateway/__init__.py` & `renku-2.6.1rc1/renku/infrastructure/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/infrastructure/gateway/__pycache__/dataset_gateway.cpython-39.pyc` & `renku-2.6.1rc1/renku/infrastructure/gateway/__pycache__/dataset_gateway.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 3743 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 9f0e 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 9f0e 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 5a04 6401 6404 6c05  ..d.d.l.Z.d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6401 6407 6c0c 6d0d 5a0d 0100 4700  ..d.d.l.m.Z...G.
```

### Comparing `renku-2.6.0rc1/renku/infrastructure/gateway/activity_gateway.py` & `renku-2.6.1rc1/renku/infrastructure/gateway/activity_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/infrastructure/gateway/database_gateway.py` & `renku-2.6.1rc1/renku/infrastructure/gateway/database_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/infrastructure/gateway/dataset_gateway.py` & `renku-2.6.1rc1/renku/infrastructure/gateway/dataset_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/infrastructure/gateway/plan_gateway.py` & `renku-2.6.1rc1/renku/infrastructure/gateway/plan_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/infrastructure/gateway/project_gateway.py` & `renku-2.6.1rc1/renku/infrastructure/gateway/project_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/infrastructure/git_merger.py` & `renku-2.6.1rc1/renku/infrastructure/git_merger.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/infrastructure/immutable.py` & `renku-2.6.1rc1/renku/infrastructure/immutable.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/infrastructure/persistent.py` & `renku-2.6.1rc1/renku/infrastructure/persistent.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/infrastructure/repository.py` & `renku-2.6.1rc1/renku/infrastructure/repository.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/infrastructure/storage/__init__.py` & `renku-2.6.1rc1/renku/infrastructure/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/infrastructure/storage/__pycache__/factory.cpython-39.pyc` & `renku-2.6.1rc1/renku/infrastructure/storage/__pycache__/factory.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1989 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 c507 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 c507 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6502 7238 6401 6404 6c07 6d08 5a08  ..e.r8d.d.l.m.Z.
 00000060: 6d09 5a09 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000070: 6506 8303 5a0a 6407 5300 2908 7a1f 5374  e...Z.d.S.).z.St
```

### Comparing `renku-2.6.0rc1/renku/infrastructure/storage/factory.py` & `renku-2.6.1rc1/renku/infrastructure/storage/factory.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/infrastructure/storage/rclone.py` & `renku-2.6.1rc1/renku/infrastructure/storage/rclone.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/.github/ISSUE_TEMPLATE/bug_report.md` & `renku-2.6.1rc1/renku/templates/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/.github/ISSUE_TEMPLATE/config.yml` & `renku-2.6.1rc1/renku/templates/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/.github/ISSUE_TEMPLATE/feature_request.md` & `renku-2.6.1rc1/renku/templates/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/.github/dependabot.yml` & `renku-2.6.1rc1/renku/templates/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/.gitignore` & `renku-2.6.1rc1/renku/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/R-minimal/.gitignore` & `renku-2.6.1rc1/renku/templates/R-minimal/.gitignore`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/R-minimal/.renkulfsignore` & `renku-2.6.1rc1/renku/templates/R-minimal/.renkulfsignore`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/R-minimal/Dockerfile` & `renku-2.6.1rc1/renku/templates/R-minimal/Dockerfile`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/R-minimal/README.md` & `renku-2.6.1rc1/renku/templates/R-minimal/README.md`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/R-minimal/workflows/my-workflow.yaml` & `renku-2.6.1rc1/renku/templates/R-minimal/workflows/my-workflow.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/R-minimal.png` & `renku-2.6.1rc1/renku/templates/R-minimal.png`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/README.md` & `renku-2.6.1rc1/renku/templates/README.md`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/bioc-minimal/.gitignore` & `renku-2.6.1rc1/renku/templates/bioc-minimal/.gitignore`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/bioc-minimal/.renkulfsignore` & `renku-2.6.1rc1/renku/templates/bioc-minimal/.renkulfsignore`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/bioc-minimal/Dockerfile` & `renku-2.6.1rc1/renku/templates/bioc-minimal/Dockerfile`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/bioc-minimal/README.md` & `renku-2.6.1rc1/renku/templates/bioc-minimal/README.md`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/bioc-minimal/workflows/my-workflow.yaml` & `renku-2.6.1rc1/renku/templates/bioc-minimal/workflows/my-workflow.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/bioconductor.png` & `renku-2.6.1rc1/renku/templates/bioconductor.png`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/julia-minimal/.gitignore` & `renku-2.6.1rc1/renku/templates/julia-minimal/.gitignore`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/julia-minimal/.renkulfsignore` & `renku-2.6.1rc1/renku/templates/julia-minimal/.renkulfsignore`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/julia-minimal/Dockerfile` & `renku-2.6.1rc1/renku/templates/julia-minimal/Dockerfile`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/julia-minimal/README.md` & `renku-2.6.1rc1/renku/templates/julia-minimal/README.md`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/julia-minimal/workflows/my-workflow.yaml` & `renku-2.6.1rc1/renku/templates/julia-minimal/workflows/my-workflow.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/julialang.png` & `renku-2.6.1rc1/renku/templates/julialang.png`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/manifest.yaml` & `renku-2.6.1rc1/renku/templates/manifest.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/minimal/.renkulfsignore` & `renku-2.6.1rc1/renku/templates/minimal/.renkulfsignore`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/minimal/Dockerfile` & `renku-2.6.1rc1/renku/templates/minimal/Dockerfile`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/minimal/workflows/my-workflow.yaml` & `renku-2.6.1rc1/renku/templates/minimal/workflows/my-workflow.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/python-minimal/.gitignore` & `renku-2.6.1rc1/renku/templates/python-minimal/.gitignore`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/python-minimal/.renkulfsignore` & `renku-2.6.1rc1/renku/templates/python-minimal/.renkulfsignore`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/python-minimal/Dockerfile` & `renku-2.6.1rc1/renku/templates/python-minimal/Dockerfile`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/python-minimal/README.md` & `renku-2.6.1rc1/renku/templates/python-minimal/README.md`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/python-minimal/workflows/my-workflow.yaml` & `renku-2.6.1rc1/renku/templates/python-minimal/workflows/my-workflow.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/templates/python-minimal.png` & `renku-2.6.1rc1/renku/templates/python-minimal.png`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/__init__.py` & `renku-2.6.1rc1/renku/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/api/__init__.py` & `renku-2.6.1rc1/renku/ui/api/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/api/graph/__init__.py` & `renku-2.6.1rc1/renku/ui/api/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/api/graph/rdf.py` & `renku-2.6.1rc1/renku/ui/api/graph/rdf.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/api/models/__init__.py` & `renku-2.6.1rc1/renku/ui/api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/api/models/activity.py` & `renku-2.6.1rc1/renku/ui/api/models/activity.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/api/models/dataset.py` & `renku-2.6.1rc1/renku/ui/api/models/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/api/models/parameter.py` & `renku-2.6.1rc1/renku/ui/api/models/parameter.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/api/models/plan.py` & `renku-2.6.1rc1/renku/ui/api/models/plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/api/models/project.py` & `renku-2.6.1rc1/renku/ui/api/models/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/api/util.py` & `renku-2.6.1rc1/renku/ui/api/util.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/__init__.py` & `renku-2.6.1rc1/renku/ui/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/__main__.py` & `renku-2.6.1rc1/renku/ui/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/__init__.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 9319 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 6724 0000  a........^.dg$..
+00000000: 610d 0d0a 0000 0000 9f1b b064 6724 0000  a..........dg$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 5404 0000 6400  .....@...sT...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6402 6c06 5a06 6401  m.Z...d.d.l.Z.d.
 00000060: 6402 6c07 5a07 6401 6404 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6401 6405 6c0a 6d0b 5a0b 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/clone.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/clone.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2594 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 220a 0000  a........^.d"...
+00000000: 610d 0d0a 0000 0000 9f1b b064 220a 0000  a..........d"...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 0200  m.....m.....m...
 00000050: 0100 6d06 5a06 0100 6501 a007 a100 6501  ..m.Z...e.....e.
 00000060: 6a08 6403 6404 6405 6406 6407 8d04 6501  j.d.d.d.d.d...e.
 00000070: a009 6408 a101 6501 6a09 6409 6406 6402  ..d...e.j.d.d.d.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/config.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 7953 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 111f 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 111f 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 1c01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 0200  m.....m.....m...
 00000050: 0100 6d06 5a06 0100 6401 6403 6c07 6d08  ..m.Z...d.d.l.m.
 00000060: 5a08 0100 6501 a009 a100 6404 6405 8400  Z...e.....d.d...
 00000070: 8301 5a0a 650a a00b a100 6501 6a0c 6406  ..Z.e.....e.j.d.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/dataset.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/dataset.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 42787 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 23a7 0000  a........^.d#...
+00000000: 610d 0d0a 0000 0000 9f1b b064 23a7 0000  a..........d#...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0015 0000 0040 0000 0073 fc07 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 6d08 5a08  d.l.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6402 6c09 5a09 6401 6405 6c0a  ..d.d.l.Z.d.d.l.
 00000070: 6d0b 5a0b 0100 6401 6402 6c0c 6d0d 0200  m.Z...d.d.l.m...
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/doctor.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/doctor.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2333 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 1d09 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 1d09 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6502  Z.d.d.l.m.Z...e.
 00000050: a005 a100 6502 6a06 6502 6a07 6404 6405  ....e.j.e.j.d.d.
 00000060: 6406 6407 8d03 6502 6a07 6408 6409 6405  d.d...e.j.d.d.d.
 00000070: 640a 6407 8d04 640b 640c 8400 8301 8301  d.d...d.d.......
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/env.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/env.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1587 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 3306 0000  a........^.d3...
+00000000: 610d 0d0a 0000 0000 9f1b b064 3306 0000  a..........d3...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 5a00 6401 6402 6c01 5a01 6501 a002 a100  Z.d.d.l.Z.e.....
 00000040: 6501 6a03 6403 6404 6405 6406 6407 8d04  e.j.d.d.d.d.d...
 00000050: 6501 6a04 6408 6409 8400 8301 8301 8301  e.j.d.d.........
 00000060: 5a05 6402 5300 290a 7a23 5265 6e6b 7520  Z.d.S.).z#Renku 
 00000070: 656e 7669 726f 6e6d 656e 7420 7265 6c61  environment rela
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/exception_handler.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/exception_handler.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 7931 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 fb1e 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 fb1e 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 2e01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a06 6401 6403 6c07 6d08 5a08 0100 6401  Z.d.d.l.m.Z...d.
 00000070: 6402 6c09 5a09 6401 6402 6c0a 6d0b 0200  d.l.Z.d.d.l.m...
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/gc.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/gc.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1139 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 7304 0000  a........^.ds...
+00000000: 610d 0d0a 0000 0000 9f1b b064 7304 0000  a..........ds...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 5a00 6401 6402 6c01 5a01 6501 a002 a100  Z.d.d.l.Z.e.....
 00000040: 6403 6404 8400 8301 5a03 6402 5300 2905  d.d.....Z.d.S.).
 00000050: 7adf 4672 6565 2075 7020 6469 736b 2073  z.Free up disk s
 00000060: 7061 6365 2062 7920 7265 6d6f 7669 6e67  pace by removing
 00000070: 2074 656d 706f 7261 7279 2066 696c 6573   temporary files
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/githooks.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/githooks.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2538 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 ea09 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 ea09 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 8200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6402 6c04 5a04 6401  m.Z...d.d.l.Z.d.
 00000050: 6402 6c05 6d06 0200 0100 6d07 0200 0100  d.l.m.....m.....
 00000060: 6d08 0200 0100 6d09 5a09 0100 6504 a00a  m.....m.Z...e...
 00000070: a100 6404 6405 8400 8301 5a0b 650b a00c  ..d.d.....Z.e...
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/graph.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/graph.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 4950 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 5613 0000  a........^.dV...
+00000000: 610d 0d0a 0000 0000 9f1b b064 5613 0000  a..........dV...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6404 6404 6405 6406 6407  m.Z...d.d.d.d.d.
 00000050: 6408 6409 640a 9c07 5a04 6501 a005 a100  d.d.d...Z.e.....
 00000060: 640b 640c 8400 8301 5a06 6506 a007 a100  d.d.....Z.e.....
 00000070: 6501 6a08 640d 6503 6509 6504 a00a a100  e.j.d.e.e.e.....
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/init.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/init.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 11113 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 692b 0000  a........^.di+..
+00000000: 610d 0d0a 0000 0000 9f1b b064 692b 0000  a..........di+..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0013 0000 0040 0000 0073 a001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6402 6c05 5a05 6401 6404 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6401 6405 6c08 6d09 5a09 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6700 6407 a201  d.l.m.Z...g.d...
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/log.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/log.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 8581 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 8521 0000  a........^.d.!..
+00000000: 610d 0d0a 0000 0000 9f1b b064 8521 0000  a..........d.!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 2e01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 0200  m.....m.....m...
 00000050: 0100 6d06 5a06 0100 6401 6403 6c07 6d08  ..m.Z...d.d.l.m.
 00000060: 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c  Z.m.Z.m.Z.m.Z.m.
 00000070: 5a0c 0100 6401 6404 6c0d 6d0e 5a0e 6d0f  Z...d.d.l.m.Z.m.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/login.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/login.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 4845 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 ed12 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 ed12 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 ce00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 0200  m.....m.....m...
 00000050: 0100 6d06 5a06 0100 6401 6403 6c07 6d08  ..m.Z...d.d.l.m.
 00000060: 5a08 0100 6501 a009 a100 6501 6a0a 6404  Z...e.....e.j.d.
 00000070: 6405 6402 6406 8d03 6501 6a0b 6407 6408  d.d.d...e.j.d.d.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/mergetool.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/mergetool.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2499 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 c309 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 c309 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6501 a004 a100 6404 6405  m.Z...e.....d.d.
 00000050: 8400 8301 5a05 6505 6a06 6406 6407 8d01  ....Z.e.j.d.d...
 00000060: 6501 6a07 6408 6501 6a08 6406 6409 8d01  e.j.d.e.j.d.d...
 00000070: 640a 8d02 6501 6a07 640b 6501 6a08 6406  d...e.j.d.e.j.d.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/migrate.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/migrate.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 5894 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 0617 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 0617 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 2a01 0000 6400  .....@...s*...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6402 6c05 5a05 6401 6402 6c06 6d07 0200  d.l.Z.d.d.l.m...
 00000060: 0100 6d08 0200 0100 6d09 0200 0100 6d0a  ..m.....m.....m.
 00000070: 5a0a 0100 6401 6404 6c0b 6d0c 5a0c 6d0d  Z...d.d.l.m.Z.m.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/move.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/move.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 2881 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 410b 0000  a........^.dA...
+00000000: 610d 0d0a 0000 0000 9f1b b064 410b 0000  a..........dA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6501 6a04 6404 6405 8d01  m.Z...e.j.d.d...
 00000050: 6501 6a05 6406 6501 6a06 6407 6408 8d01  e.j.d.e.j.d.d...
 00000060: 6409 640a 8d03 6501 6a05 640b 6501 a006  d.d...e.j.d.e...
 00000070: a100 640c 640a 8d03 6501 6a07 640d 640e  ..d.d...e.j.d.d.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/project.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/project.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 5768 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 8816 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 8816 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000e 0000 0040 0000 0073 2801 0000 6400  .....@...s(...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6402 6c04 5a04 6401  m.Z...d.d.l.Z.d.
 00000050: 6402 6c05 6d06 0200 0100 6d07 0200 0100  d.l.m.....m.....
 00000060: 6d08 0200 0100 6d09 5a09 0100 6401 6404  m.....m.Z...d.d.
 00000070: 6c0a 6d0b 5a0b 0100 6401 6405 6c0c 6d0d  l.m.Z...d.d.l.m.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/remove.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/remove.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1754 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 da06 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 da06 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6501 6a04 6404 6405 8d01  m.Z...e.j.d.d...
 00000050: 6501 6a05 6406 6501 6a06 6407 6408 8d01  e.j.d.e.j.d.d...
 00000060: 6409 6407 640a 8d04 640b 640c 8400 8301  d.d.d...d.d.....
 00000070: 8301 5a07 6402 5300 290d 6121 0200 0052  ..Z.d.S.).a!...R
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/rerun.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/rerun.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 4227 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 8310 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 8310 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000f 0000 0040 0000 0073 e800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6501 a00a a100  d.l.m.Z...e.....
 00000070: 6501 6a0b 6407 6408 6409 640a 640b 640c  e.j.d.d.d.d.d.d.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/rollback.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/rollback.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 3249 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 b10c 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 b10c 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6501 a004 a100 6501 6a05  m.Z...e.....e.j.
 00000050: 6404 6405 8400 8301 8301 5a06 6402 5300  d.d.......Z.d.S.
 00000060: 2906 75f8 0700 0052 6f6c 6c62 6163 6b20  ).u....Rollback 
 00000070: 7072 6f6a 6563 7420 746f 2061 2070 7265  project to a pre
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/run.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/run.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 26417 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 3167 0000  a........^.d1g..
+00000000: 610d 0d0a 0000 0000 9f1b b064 3167 0000  a..........d1g..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0019 0000 0040 0000 0073 0e02 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6402 6c04 5a04 6401  m.Z...d.d.l.Z.d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6401 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6407 6c0b 6d0c 5a0c 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/save.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/save.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 3510 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 b60d 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 b60d 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 8c00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 0200  m.....m.....m...
 00000050: 0100 6d06 5a06 0100 6401 6403 6c07 6d08  ..m.Z...d.d.l.m.
 00000060: 5a08 0100 6501 6a09 6404 6405 8d01 6501  Z...e.j.d.d...e.
 00000070: 6a0a 6406 6407 6402 6408 6409 8d04 6501  j.d.d.d.d.d...e.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/service.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/service.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 11927 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 972e 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 972e 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 8002 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a06 6401 6403 6c07 6d07 5a07 0100 6401  Z.d.d.l.m.Z...d.
 00000070: 6404 6c08 6d09 5a09 0100 6401 6402 6c0a  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/session.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/session.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 14738 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 9239 0000  a........^.d.9..
+00000000: 610d 0d0a 0000 0000 9f1b b064 9239 0000  a..........d.9..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000e 0000 0040 0000 0073 d602 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6407 6c0b 6d0c 5a0c 0100 6401 6408 6c0d  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/status.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/status.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 5489 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 7115 0000  a........^.dq...
+00000000: 610d 0d0a 0000 0000 9f1b b064 7115 0000  a..........dq...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 0200  m.....m.....m...
 00000050: 0100 6d06 5a06 0100 6401 6403 6c07 6d08  ..m.Z...d.d.l.m.
 00000060: 5a08 0100 6501 a009 a100 6501 6a0a 6501  Z...e.....e.j.e.
 00000070: 6a0b 6404 6405 6406 6407 6408 8d04 6501  j.d.d.d.d.d...e.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/storage.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/storage.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 5604 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 e415 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 e415 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 4801 0000 6400  .....@...sH...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 6d04 0200 0100 6d05  Z.d.d.l.m.....m.
 00000050: 0200 0100 6d06 0200 0100 6d07 5a07 0100  ....m.....m.Z...
 00000060: 6401 6403 6c08 6d09 5a09 0100 6401 6404  d.d.l.m.Z...d.d.
 00000070: 6c0a 6d0b 5a0b 0100 6502 a00c a100 6405  l.m.Z...e.....d.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/template.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/template.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 13434 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 7a34 0000  a........^.dz4..
+00000000: 610d 0d0a 0000 0000 9f1b b064 7a34 0000  a..........dz4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 7402 0000 6400  .....@...st...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 6401 6402 6c08  m.Z.m.Z...d.d.l.
 00000060: 5a08 6401 6402 6c09 6d0a 0200 0100 6d0b  Z.d.d.l.m.....m.
 00000070: 0200 0100 6d0c 0200 0100 6d0d 5a0d 0100  ....m.....m.Z...
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/update.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/update.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 6723 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 431a 0000  a........^.dC...
+00000000: 610d 0d0a 0000 0000 9f1b b064 431a 0000  a..........dC...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000e 0000 0040 0000 0073 fc00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6401 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6501 a00c a100 6501 6a0d  m.Z...e.....e.j.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/__pycache__/workflow.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/__pycache__/workflow.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 47787 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 abba 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 abba 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0016 0000 0040 0000 0073 6607 0000 6400  .....@...sf...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6402 6c07 5a07 6401 6404 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6401 6402 6c0a 6d0b 0200 0100 6d0c  ..d.d.l.m.....m.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/clone.py` & `renku-2.6.1rc1/renku/ui/cli/clone.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/config.py` & `renku-2.6.1rc1/renku/ui/cli/config.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/dataset.py` & `renku-2.6.1rc1/renku/ui/cli/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/doctor.py` & `renku-2.6.1rc1/renku/ui/cli/doctor.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/env.py` & `renku-2.6.1rc1/renku/ui/cli/env.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/exception_handler.py` & `renku-2.6.1rc1/renku/ui/cli/exception_handler.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/gc.py` & `renku-2.6.1rc1/renku/ui/cli/gc.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/githooks.py` & `renku-2.6.1rc1/renku/ui/cli/githooks.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/graph.py` & `renku-2.6.1rc1/renku/ui/cli/graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/init.py` & `renku-2.6.1rc1/renku/ui/cli/init.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/log.py` & `renku-2.6.1rc1/renku/ui/cli/log.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/login.py` & `renku-2.6.1rc1/renku/ui/cli/login.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/mergetool.py` & `renku-2.6.1rc1/renku/ui/cli/mergetool.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/migrate.py` & `renku-2.6.1rc1/renku/ui/cli/migrate.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/move.py` & `renku-2.6.1rc1/renku/ui/cli/move.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/project.py` & `renku-2.6.1rc1/renku/ui/cli/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/remove.py` & `renku-2.6.1rc1/renku/ui/cli/remove.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/rerun.py` & `renku-2.6.1rc1/renku/ui/cli/rerun.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/rollback.py` & `renku-2.6.1rc1/renku/ui/cli/rollback.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/run.py` & `renku-2.6.1rc1/renku/ui/cli/run.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/save.py` & `renku-2.6.1rc1/renku/ui/cli/save.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/service.py` & `renku-2.6.1rc1/renku/ui/cli/service.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/session.py` & `renku-2.6.1rc1/renku/ui/cli/session.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/status.py` & `renku-2.6.1rc1/renku/ui/cli/status.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/storage.py` & `renku-2.6.1rc1/renku/ui/cli/storage.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/template.py` & `renku-2.6.1rc1/renku/ui/cli/template.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/update.py` & `renku-2.6.1rc1/renku/ui/cli/update.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/utils/__init__.py` & `renku-2.6.1rc1/renku/ui/cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/utils/__pycache__/callback.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/utils/__pycache__/callback.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 5409 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 2115 0000  a........^.d!...
+00000000: 610d 0d0a 0000 0000 9f1b b064 2115 0000  a..........d!...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6402 6c04 5a04 6401  m.Z...d.d.l.Z.d.
 00000050: 6404 6c05 6d05 5a05 0100 6401 6405 6c06  d.l.m.Z...d.d.l.
 00000060: 6d06 5a06 0100 6401 6402 6c07 6d08 0200  m.Z...d.d.l.m...
 00000070: 0100 6d09 0200 0100 6d0a 0200 0100 6d0b  ..m.....m.....m.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/utils/__pycache__/click.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/utils/__pycache__/click.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 5473 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 6115 0000  a........^.da...
+00000000: 610d 0d0a 0000 0000 9f1b b064 6115 0000  a..........da...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 aa00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 5a04 6502 722c 6401  ..d.d.l.Z.e.r,d.
 00000050: 6404 6c05 6d06 5a06 0100 6503 6507 1900  d.l.m.Z...e.e...
 00000060: 6405 9c01 6406 6407 8404 5a08 6503 6507  d...d.d...Z.e.e.
 00000070: 1900 6405 9c01 6408 6409 8404 5a09 6503  ..d...d.d...Z.e.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/utils/__pycache__/plugins.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/utils/__pycache__/plugins.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 1375 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 5f05 0000  a........^.d_...
+00000000: 610d 0d0a 0000 0000 9f1b b064 5f05 0000  a..........d_...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 5a00 6401 6402 8400 5a01 6403 6404 8400  Z.d.d...Z.d.d...
 00000040: 5a02 6405 6406 8400 5a03 6407 5300 2908  Z.d.d...Z.d.S.).
 00000050: 7a1e 5574 696c 6974 7920 6675 6e63 7469  z.Utility functi
 00000060: 6f6e 7320 666f 7220 706c 7567 696e 732e  ons for plugins.
 00000070: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/utils/__pycache__/terminal.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/cli/utils/__pycache__/terminal.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 9917 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 bd26 0000  a........^.d.&..
+00000000: 610d 0d0a 0000 0000 9f1b b064 bd26 0000  a..........d.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 6e01 0000 6400  .....@...sn...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6402 6c07 5a07 6401 6404 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6506 7270 6401 6405 6c0a 6d0b 5a0b  ..e.rpd.d.l.m.Z.
```

### Comparing `renku-2.6.0rc1/renku/ui/cli/utils/callback.py` & `renku-2.6.1rc1/renku/ui/cli/utils/callback.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/utils/click.py` & `renku-2.6.1rc1/renku/ui/cli/utils/click.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/utils/color.py` & `renku-2.6.1rc1/renku/ui/cli/utils/color.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/utils/curses.py` & `renku-2.6.1rc1/renku/ui/cli/utils/curses.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/utils/plugins.py` & `renku-2.6.1rc1/renku/ui/cli/utils/plugins.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/utils/terminal.py` & `renku-2.6.1rc1/renku/ui/cli/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/cli/workflow.py` & `renku-2.6.1rc1/renku/ui/cli/workflow.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/.env-example` & `renku-2.6.1rc1/renku/ui/service/.env-example`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/__init__.py` & `renku-2.6.1rc1/renku/ui/service/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/__pycache__/config.cpython-39.pyc` & `renku-2.6.1rc1/renku/ui/service/__pycache__/config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 14:43:37 2023 UTC, .py size: 3091 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 195e 9464 130c 0000  a........^.d....
+00000000: 610d 0d0a 0000 0000 9f1b b064 130c 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 ca01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 7a0c  Z.d.d.l.m.Z...z.
 00000050: 6401 6402 6c05 5a05 5700 6e1e 0400 6506  d.d.l.Z.W.n...e.
 00000060: 794a 0100 0100 0100 6401 6402 6c07 6d08  yJ......d.d.l.m.
 00000070: 5a05 0100 5900 6e02 3000 6401 5a09 6404  Z...Y.n.0.d.Z.d.
```

### Comparing `renku-2.6.0rc1/renku/ui/service/cache/__init__.py` & `renku-2.6.1rc1/renku/ui/service/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/cache/base.py` & `renku-2.6.1rc1/renku/ui/service/cache/base.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/cache/files.py` & `renku-2.6.1rc1/renku/ui/service/cache/files.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/cache/jobs.py` & `renku-2.6.1rc1/renku/ui/service/cache/jobs.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/cache/models/__init__.py` & `renku-2.6.1rc1/renku/ui/service/cache/models/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/cache/models/file.py` & `renku-2.6.1rc1/renku/ui/service/cache/models/file.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/cache/models/job.py` & `renku-2.6.1rc1/renku/ui/service/cache/models/job.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/cache/models/project.py` & `renku-2.6.1rc1/renku/ui/service/cache/models/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/cache/models/user.py` & `renku-2.6.1rc1/renku/ui/service/cache/models/user.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/cache/projects.py` & `renku-2.6.1rc1/renku/ui/service/cache/projects.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/cache/serializers/__init__.py` & `renku-2.6.1rc1/renku/ui/service/cache/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/cache/serializers/file.py` & `renku-2.6.1rc1/renku/ui/service/cache/serializers/file.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/cache/serializers/job.py` & `renku-2.6.1rc1/renku/ui/service/cache/serializers/job.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/cache/serializers/project.py` & `renku-2.6.1rc1/renku/ui/service/cache/serializers/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/cache/serializers/user.py` & `renku-2.6.1rc1/renku/ui/service/cache/serializers/user.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/cache/users.py` & `renku-2.6.1rc1/renku/ui/service/cache/users.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/config.py` & `renku-2.6.1rc1/renku/ui/service/config.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/__init__.py` & `renku-2.6.1rc1/renku/ui/service/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/api/__init__.py` & `renku-2.6.1rc1/renku/ui/service/controllers/api/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/api/abstract.py` & `renku-2.6.1rc1/renku/ui/service/controllers/api/abstract.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/api/mixins.py` & `renku-2.6.1rc1/renku/ui/service/controllers/api/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,19 @@
             return self.remote()
 
         elif "git_url" in self.context and "user_id" in self.user_data:
             try:
                 project = Project.get(
                     (Project.user_id == self.user_data["user_id"]) & (Project.git_url == self.context["git_url"])
                 )
+
+                if not project.abs_path.exists():
+                    project.delete()
+                    raise ValueError("Project found in redis but missing on disk.")
+
             except ValueError:
                 from renku.ui.service.controllers.cache_project_clone import ProjectCloneCtrl
 
                 clone_context = {
                     "git_url": self.request_data["git_url"],
                 }
```

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/cache_files_delete_chunks.py` & `renku-2.6.1rc1/renku/ui/service/controllers/cache_files_delete_chunks.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/cache_files_upload.py` & `renku-2.6.1rc1/renku/ui/service/controllers/cache_files_upload.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/cache_list_projects.py` & `renku-2.6.1rc1/renku/ui/service/controllers/cache_list_projects.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/cache_list_uploaded.py` & `renku-2.6.1rc1/renku/ui/service/controllers/cache_list_uploaded.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/cache_migrate_project.py` & `renku-2.6.1rc1/renku/ui/service/controllers/cache_migrate_project.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/cache_migrations_check.py` & `renku-2.6.1rc1/renku/ui/service/controllers/cache_migrations_check.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/cache_project_clone.py` & `renku-2.6.1rc1/renku/ui/service/controllers/cache_project_clone.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/config_set.py` & `renku-2.6.1rc1/renku/ui/service/controllers/config_set.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/config_show.py` & `renku-2.6.1rc1/renku/ui/service/controllers/config_show.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/datasets_add_file.py` & `renku-2.6.1rc1/renku/ui/service/controllers/datasets_add_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/datasets_create.py` & `renku-2.6.1rc1/renku/ui/service/controllers/datasets_create.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/datasets_edit.py` & `renku-2.6.1rc1/renku/ui/service/controllers/datasets_edit.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/datasets_files_list.py` & `renku-2.6.1rc1/renku/ui/service/controllers/datasets_files_list.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/datasets_import.py` & `renku-2.6.1rc1/renku/ui/service/controllers/datasets_import.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/datasets_list.py` & `renku-2.6.1rc1/renku/ui/service/controllers/datasets_list.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/datasets_remove.py` & `renku-2.6.1rc1/renku/ui/service/controllers/datasets_remove.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/datasets_unlink.py` & `renku-2.6.1rc1/renku/ui/service/controllers/datasets_unlink.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/graph_export.py` & `renku-2.6.1rc1/renku/ui/service/controllers/graph_export.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/project_edit.py` & `renku-2.6.1rc1/renku/ui/service/controllers/project_edit.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/project_lock_status.py` & `renku-2.6.1rc1/renku/ui/service/controllers/project_lock_status.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/project_show.py` & `renku-2.6.1rc1/renku/ui/service/controllers/project_show.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/templates_create_project.py` & `renku-2.6.1rc1/renku/ui/service/controllers/templates_create_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,17 +126,18 @@
         except errors.InvalidTemplateError as e:
             raise UserTemplateInvalidError(error_message=f"the template '{identifier}' is invalid") from e
 
         repository = Repository(templates_source.path)
         self.template_version = repository.head.commit.hexsha
 
         # Verify missing parameters
-        template_parameters = {p.name for p in self.template.parameters}
+        template_parameters = {p.name: p for p in self.template.parameters}
         provided_parameters = {p["key"]: p["value"] for p in self.ctx["parameters"]}
-        missing_keys = list(template_parameters - provided_parameters.keys())
+        missing_keys = list(template_parameters.keys() - provided_parameters.keys())
+        missing_keys = [k for k in missing_keys if not template_parameters[k].has_default]
         if len(missing_keys) > 0:
             raise UserProjectCreationError(error_message=f"the template requires a value for '${missing_keys[0]}'")
 
         return provided_parameters
 
     def new_project_push(self, project_path):
         """Push new project to the remote."""
```

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/templates_read_manifest.py` & `renku-2.6.1rc1/renku/ui/service/controllers/templates_read_manifest.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/utils/__init__.py` & `renku-2.6.1rc1/renku/ui/service/controllers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/utils/datasets.py` & `renku-2.6.1rc1/renku/ui/service/controllers/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/utils/project_clone.py` & `renku-2.6.1rc1/renku/ui/service/controllers/utils/project_clone.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/utils/remote_project.py` & `renku-2.6.1rc1/renku/ui/service/controllers/utils/remote_project.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/version.py` & `renku-2.6.1rc1/renku/ui/service/controllers/version.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/versions_list.py` & `renku-2.6.1rc1/renku/ui/service/controllers/versions_list.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/workflow_plans_export.py` & `renku-2.6.1rc1/renku/ui/service/controllers/workflow_plans_export.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/workflow_plans_list.py` & `renku-2.6.1rc1/renku/ui/service/controllers/workflow_plans_list.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/controllers/workflow_plans_show.py` & `renku-2.6.1rc1/renku/ui/service/controllers/workflow_plans_show.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/entrypoint.py` & `renku-2.6.1rc1/renku/ui/service/entrypoint.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/errors.py` & `renku-2.6.1rc1/renku/ui/service/errors.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/gateways/__init__.py` & `renku-2.6.1rc1/renku/ui/service/gateways/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/gateways/gitlab_api_provider.py` & `renku-2.6.1rc1/renku/ui/service/gateways/gitlab_api_provider.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/interfaces/__init__.py` & `renku-2.6.1rc1/renku/ui/service/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/interfaces/git_api_provider.py` & `renku-2.6.1rc1/renku/ui/service/interfaces/git_api_provider.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/jobs/__init__.py` & `renku-2.6.1rc1/renku/ui/service/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/jobs/cleanup.py` & `renku-2.6.1rc1/renku/ui/service/jobs/cleanup.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/jobs/constants.py` & `renku-2.6.1rc1/renku/ui/service/jobs/constants.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/jobs/contexts.py` & `renku-2.6.1rc1/renku/ui/service/jobs/contexts.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/jobs/datasets.py` & `renku-2.6.1rc1/renku/ui/service/jobs/datasets.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/jobs/delayed_ctrl.py` & `renku-2.6.1rc1/renku/ui/service/jobs/delayed_ctrl.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/jobs/queues.py` & `renku-2.6.1rc1/renku/ui/service/jobs/queues.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/logger.py` & `renku-2.6.1rc1/renku/ui/service/logger.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/logging.yaml` & `renku-2.6.1rc1/renku/ui/service/logging.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/scheduler.py` & `renku-2.6.1rc1/renku/ui/service/scheduler.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/serializers/__init__.py` & `renku-2.6.1rc1/renku/ui/service/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/serializers/cache.py` & `renku-2.6.1rc1/renku/ui/service/serializers/cache.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/serializers/common.py` & `renku-2.6.1rc1/renku/ui/service/serializers/common.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/serializers/config.py` & `renku-2.6.1rc1/renku/ui/service/serializers/config.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/serializers/datasets.py` & `renku-2.6.1rc1/renku/ui/service/serializers/datasets.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/serializers/graph.py` & `renku-2.6.1rc1/renku/ui/service/serializers/graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/serializers/headers.py` & `renku-2.6.1rc1/renku/ui/service/serializers/headers.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/serializers/jobs.py` & `renku-2.6.1rc1/renku/ui/service/serializers/jobs.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/serializers/project.py` & `renku-2.6.1rc1/renku/ui/service/serializers/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/serializers/rpc.py` & `renku-2.6.1rc1/renku/ui/service/serializers/rpc.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/serializers/templates.py` & `renku-2.6.1rc1/renku/ui/service/serializers/templates.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/serializers/v1/__init__.py` & `renku-2.6.1rc1/renku/ui/service/serializers/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/serializers/v1/cache.py` & `renku-2.6.1rc1/renku/ui/service/serializers/v1/cache.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/serializers/v1/templates.py` & `renku-2.6.1rc1/renku/ui/service/serializers/v1/templates.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/serializers/version.py` & `renku-2.6.1rc1/renku/ui/service/serializers/version.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/serializers/versions_list.py` & `renku-2.6.1rc1/renku/ui/service/serializers/versions_list.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/serializers/workflows.py` & `renku-2.6.1rc1/renku/ui/service/serializers/workflows.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/utils/__init__.py` & `renku-2.6.1rc1/renku/ui/service/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/utils/callback.py` & `renku-2.6.1rc1/renku/ui/service/utils/callback.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/utils/json_encoder.py` & `renku-2.6.1rc1/renku/ui/service/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/utils/squash.py` & `renku-2.6.1rc1/renku/ui/service/utils/squash.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/utils/timeout.py` & `renku-2.6.1rc1/renku/ui/service/utils/timeout.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/views/__init__.py` & `renku-2.6.1rc1/renku/ui/service/views/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/views/api_versions.py` & `renku-2.6.1rc1/renku/ui/service/views/api_versions.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/views/apispec.py` & `renku-2.6.1rc1/renku/ui/service/views/apispec.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/views/cache.py` & `renku-2.6.1rc1/renku/ui/service/views/cache.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/views/config.py` & `renku-2.6.1rc1/renku/ui/service/views/config.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/views/datasets.py` & `renku-2.6.1rc1/renku/ui/service/views/datasets.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/views/decorators.py` & `renku-2.6.1rc1/renku/ui/service/views/decorators.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/views/error_handlers.py` & `renku-2.6.1rc1/renku/ui/service/views/error_handlers.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/views/graph.py` & `renku-2.6.1rc1/renku/ui/service/views/graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/views/jobs.py` & `renku-2.6.1rc1/renku/ui/service/views/jobs.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/views/project.py` & `renku-2.6.1rc1/renku/ui/service/views/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/views/templates.py` & `renku-2.6.1rc1/renku/ui/service/views/templates.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/views/v1/__init__.py` & `renku-2.6.1rc1/renku/ui/service/views/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/views/v1/cache.py` & `renku-2.6.1rc1/renku/ui/service/views/v1/cache.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/views/v1/templates.py` & `renku-2.6.1rc1/renku/ui/service/views/v1/templates.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/views/version.py` & `renku-2.6.1rc1/renku/ui/service/views/version.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/views/versions_list.py` & `renku-2.6.1rc1/renku/ui/service/views/versions_list.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/views/workflow_plans.py` & `renku-2.6.1rc1/renku/ui/service/views/workflow_plans.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/renku/ui/service/worker.py` & `renku-2.6.1rc1/renku/ui/service/worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from contextlib import contextmanager
 
 import sentry_sdk
 from rq import Worker
 from sentry_sdk.integrations.rq import RqIntegration
 
 from renku.core.errors import ConfigurationError, UsageError
+from renku.ui.service.cache.config import REDIS_NAMESPACE
 from renku.ui.service.config import SENTRY_ENABLED, SENTRY_SAMPLERATE
 from renku.ui.service.jobs.queues import QUEUES, WorkerQueues
 from renku.ui.service.logger import DEPLOYMENT_LOG_LEVEL, worker_log
 
 if SENTRY_ENABLED:
     sentry_sdk.init(
         dsn=os.getenv("SENTRY_DSN"),
@@ -59,27 +60,27 @@
         if queue and queue not in QUEUES:
             err_msg = "Invalid queue name: {}\n\nValid queue names: \n{}".format(queue, "\n".join(QUEUES))
             raise UsageError(err_msg)
 
 
 def start_worker(queue_list):
     """Start worker."""
-    q = [q.strip() for q in queue_list if q.strip()]
+    q = [f"{REDIS_NAMESPACE}.{q.strip()}" for q in queue_list if q.strip()]
     check_queues(q)
 
-    worker_log.info(f"working on queues: {queue_list}")
+    worker_log.info(f"working on queues: {q}")
 
-    with worker(queue_list) as rq_worker:
+    with worker(q) as rq_worker:
         worker_log.info("running worker")
         rq_worker.work(logging_level=DEPLOYMENT_LOG_LEVEL)
 
 
 if __name__ == "__main__":
     queues = os.getenv("RENKU_SVC_WORKER_QUEUES")
     worker_log.info(f"working on queues: {queues}")
 
     if not queues:
         raise ConfigurationError(
             "Worker queues not specified. Please, set RENKU_SVC_WORKER_QUEUES environment variable."
         )
 
-    start_worker([queue_name.strip() for queue_name in queues.strip().split(",")])
+    start_worker([f"{REDIS_NAMESPACE}.{queue_name.strip()}" for queue_name in queues.strip().split(",")])
```

### Comparing `renku-2.6.0rc1/renku/version.py` & `renku-2.6.1rc1/renku/version.py`

 * *Files identical despite different names*

### Comparing `renku-2.6.0rc1/PKG-INFO` & `renku-2.6.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renku
-Version: 2.6.0rc1
+Version: 2.6.1rc1
 Summary: Python SDK and CLI for the Renku platform.
 Home-page: https://github.com/swissdatasciencecenter/renku-python
 License: Apache-2.0
 Keywords: Renku,CLI
 Author: Swiss Data Science Center
 Author-email: contact@datascience.ch
 Requires-Python: >=3.8.1,<3.12
@@ -69,15 +69,15 @@
 Requires-Dist: pyshacl (>=0.17.2,<0.19.2)
 Requires-Dist: python-dateutil (>=2.6.1,<2.8.3)
 Requires-Dist: python-dotenv (>=0.19.0,<0.21.0) ; extra == "service"
 Requires-Dist: python-editor (==1.0.4)
 Requires-Dist: python-gitlab (>=2.10.1,<3.8.2)
 Requires-Dist: pyyaml (>=5.4,<6.1.0)
 Requires-Dist: rdflib (>=6.0.0,<7.0)
-Requires-Dist: redis (>=3.5.3,<4.6.0) ; extra == "service"
+Requires-Dist: redis (>=3.5.3,<4.6.0,!=4.5.5) ; extra == "service"
 Requires-Dist: requests (>=2.23.0,<2.31.1)
 Requires-Dist: rich (>=9.3.0,<13.4.0)
 Requires-Dist: rq (==1.15.0) ; extra == "service"
 Requires-Dist: rq-scheduler (==0.13.1) ; extra == "service"
 Requires-Dist: sentry-sdk[flask] (>=1.5.11,<1.26.0) ; extra == "service"
 Requires-Dist: shellingham (==1.5.0.post1)
 Requires-Dist: tabulate (>=0.7.7,<0.9.1)
```

