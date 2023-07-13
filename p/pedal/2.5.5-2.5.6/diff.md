# Comparing `tmp/pedal-2.5.5.tar.gz` & `tmp/pedal-2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pedal-2.5.5.tar", last modified: Mon Jul 10 15:56:43 2023, max compression
+gzip compressed data, was "pedal-2.5.6.tar", last modified: Thu Jul 13 16:32:24 2023, max compression
```

## Comparing `pedal-2.5.5.tar` & `pedal-2.5.6.tar`

### file list

```diff
@@ -1,156 +1,158 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:43.306038 pedal-2.5.5/
--rw-rw-rw-   0        0        0     1103 2020-10-17 16:15:21.000000 pedal-2.5.5/LICENSE
--rw-rw-rw-   0        0        0     2981 2023-07-10 15:56:43.307035 pedal-2.5.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:43.082080 pedal-2.5.5/Pedal.egg-info/
--rw-rw-rw-   0        0        0     2981 2023-07-10 15:56:42.000000 pedal-2.5.5/Pedal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3759 2023-07-10 15:56:42.000000 pedal-2.5.5/Pedal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 15:56:42.000000 pedal-2.5.5/Pedal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-10 15:56:42.000000 pedal-2.5.5/Pedal.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-10 15:56:42.000000 pedal-2.5.5/Pedal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-10 15:56:42.000000 pedal-2.5.5/Pedal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1958 2023-06-14 16:24:47.000000 pedal-2.5.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:43.078113 pedal-2.5.5/pedal/
--rw-rw-rw-   0        0        0      995 2023-07-04 14:03:45.000000 pedal-2.5.5/pedal/__init__.py
--rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:43.101078 pedal-2.5.5/pedal/assertions/
--rw-rw-rw-   0        0        0      549 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/assertions/__init__.py
--rw-rw-rw-   0        0        0     8710 2022-09-25 02:42:31.000000 pedal-2.5.5/pedal/assertions/classes.py
--rw-rw-rw-   0        0        0    13562 2023-06-23 17:14:33.000000 pedal-2.5.5/pedal/assertions/commands.py
--rw-rw-rw-   0        0        0       73 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/assertions/constants.py
--rw-rw-rw-   0        0        0    20355 2023-05-27 15:44:30.000000 pedal-2.5.5/pedal/assertions/feedbacks.py
--rw-rw-rw-   0        0        0     8307 2021-12-05 16:26:04.000000 pedal-2.5.5/pedal/assertions/functions.py
--rw-rw-rw-   0        0        0     4153 2023-06-23 17:06:54.000000 pedal-2.5.5/pedal/assertions/organizers.py
--rw-rw-rw-   0        0        0    33752 2023-05-22 19:35:19.000000 pedal-2.5.5/pedal/assertions/runtime.py
--rw-rw-rw-   0        0        0     3316 2023-06-23 17:04:45.000000 pedal-2.5.5/pedal/assertions/setup.py
--rw-rw-rw-   0        0        0    30229 2023-05-26 20:52:09.000000 pedal-2.5.5/pedal/assertions/static.py
--rw-rw-rw-   0        0        0     6471 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/assertions/unittest.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:43.113078 pedal-2.5.5/pedal/cait/
--rw-rw-rw-   0        0        0      445 2020-10-17 20:34:56.000000 pedal-2.5.5/pedal/cait/__init__.py
--rw-rw-rw-   0        0        0     2255 2023-05-27 15:47:12.000000 pedal-2.5.5/pedal/cait/ast_helpers.py
--rw-rw-rw-   0        0        0    11275 2023-06-23 17:10:06.000000 pedal-2.5.5/pedal/cait/ast_map.py
--rw-rw-rw-   0        0        0    10523 2023-06-23 17:10:21.000000 pedal-2.5.5/pedal/cait/cait_api.py
--rw-rw-rw-   0        0        0    23405 2023-07-06 23:15:07.000000 pedal-2.5.5/pedal/cait/cait_node.py
--rw-rw-rw-   0        0        0       59 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/cait/constants.py
--rw-rw-rw-   0        0        0     4693 2021-06-28 19:26:48.000000 pedal-2.5.5/pedal/cait/find_node.py
--rw-rw-rw-   0        0        0    34016 2021-03-12 21:12:46.000000 pedal-2.5.5/pedal/cait/stretchy_tree_matching.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:43.124097 pedal-2.5.5/pedal/command_line/
--rw-rw-rw-   0        0        0       94 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/command_line/__init__.py
--rw-rw-rw-   0        0        0     8175 2023-06-30 18:05:29.000000 pedal-2.5.5/pedal/command_line/command_line.py
--rw-rw-rw-   0        0        0     7301 2023-05-27 15:42:09.000000 pedal-2.5.5/pedal/command_line/mocks.py
--rw-rw-rw-   0        0        0    24755 2023-06-28 02:41:46.000000 pedal-2.5.5/pedal/command_line/modes.py
--rw-rw-rw-   0        0        0     3323 2022-03-26 13:30:52.000000 pedal-2.5.5/pedal/command_line/report.py
--rw-rw-rw-   0        0        0     3549 2023-06-23 17:18:14.000000 pedal-2.5.5/pedal/command_line/verify.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:43.149033 pedal-2.5.5/pedal/core/
--rw-rw-rw-   0        0        0      107 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/core/__init__.py
--rw-rw-rw-   0        0        0     9411 2023-06-23 17:10:49.000000 pedal-2.5.5/pedal/core/commands.py
--rw-rw-rw-   0        0        0     2687 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/core/environment.py
--rw-rw-rw-   0        0        0      707 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/core/errors.py
--rw-rw-rw-   0        0        0    21596 2023-07-06 13:54:34.000000 pedal-2.5.5/pedal/core/feedback.py
--rw-rw-rw-   0        0        0     4173 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/core/feedback_category.py
--rw-rw-rw-   0        0        0     7614 2023-06-14 16:05:08.000000 pedal-2.5.5/pedal/core/final_feedback.py
--rw-rw-rw-   0        0        0     8147 2023-06-29 16:44:20.000000 pedal-2.5.5/pedal/core/formatting.py
--rw-rw-rw-   0        0        0     1962 2023-05-26 21:48:15.000000 pedal-2.5.5/pedal/core/location.py
--rw-rw-rw-   0        0        0    13916 2023-07-04 14:06:42.000000 pedal-2.5.5/pedal/core/report.py
--rw-rw-rw-   0        0        0      822 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/core/resolver.py
--rw-rw-rw-   0        0        0     3985 2022-11-17 14:35:11.000000 pedal-2.5.5/pedal/core/scoring.py
--rw-rw-rw-   0        0        0     6266 2021-02-02 16:05:08.000000 pedal-2.5.5/pedal/core/submission.py
--rw-rw-rw-   0        0        0      405 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/core/tag.py
--rw-rw-rw-   0        0        0     2286 2023-01-17 16:07:35.000000 pedal-2.5.5/pedal/core/tool.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:43.165035 pedal-2.5.5/pedal/environments/
--rw-rw-rw-   0        0        0      670 2023-06-14 15:19:32.000000 pedal-2.5.5/pedal/environments/__init__.py
--rw-rw-rw-   0        0        0     3065 2023-06-28 02:43:06.000000 pedal-2.5.5/pedal/environments/blockpy.py
--rw-rw-rw-   0        0        0     9910 2023-06-23 17:16:42.000000 pedal-2.5.5/pedal/environments/gradescope.py
--rw-rw-rw-   0        0        0    15874 2021-01-26 15:29:49.000000 pedal-2.5.5/pedal/environments/jupyter.py
--rw-rw-rw-   0        0        0    10369 2023-05-26 21:13:02.000000 pedal-2.5.5/pedal/environments/nbgrader.py
--rw-rw-rw-   0        0        0      369 2023-06-08 11:46:52.000000 pedal-2.5.5/pedal/environments/none.py
--rw-rw-rw-   0        0        0      766 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/environments/sandbox.py
--rw-rw-rw-   0        0        0     3572 2023-06-28 02:44:25.000000 pedal-2.5.5/pedal/environments/standard.py
--rw-rw-rw-   0        0        0     5528 2023-07-10 15:54:11.000000 pedal-2.5.5/pedal/environments/terminal.py
--rw-rw-rw-   0        0        0     6673 2023-06-23 16:04:44.000000 pedal-2.5.5/pedal/environments/vpl.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:43.172038 pedal-2.5.5/pedal/extensions/
--rw-rw-rw-   0        0        0        0 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/extensions/__init__.py
--rw-rw-rw-   0        0        0    13908 2022-07-24 19:32:33.000000 pedal-2.5.5/pedal/extensions/microbit.py
--rw-rw-rw-   0        0        0    11604 2022-11-26 00:03:07.000000 pedal-2.5.5/pedal/extensions/plotting.py
--rw-rw-rw-   0        0        0       81 2022-07-17 15:14:06.000000 pedal-2.5.5/pedal/extensions/turtles.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:43.185068 pedal-2.5.5/pedal/questions/
--rw-rw-rw-   0        0        0      669 2021-12-05 16:49:53.000000 pedal-2.5.5/pedal/questions/__init__.py
--rw-rw-rw-   0        0        0       66 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/questions/constants.py
--rw-rw-rw-   0        0        0      624 2021-09-15 19:16:10.000000 pedal-2.5.5/pedal/questions/feedbacks.py
--rw-rw-rw-   0        0        0     6043 2023-05-27 15:45:43.000000 pedal-2.5.5/pedal/questions/graders.py
--rw-rw-rw-   0        0        0     3477 2023-05-26 21:13:56.000000 pedal-2.5.5/pedal/questions/loader.py
--rw-rw-rw-   0        0        0     2808 2021-12-05 15:58:25.000000 pedal-2.5.5/pedal/questions/pool.py
--rw-rw-rw-   0        0        0     3784 2021-09-16 06:51:15.000000 pedal-2.5.5/pedal/questions/questions.py
--rw-rw-rw-   0        0        0     1660 2022-11-11 17:53:28.000000 pedal-2.5.5/pedal/questions/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:43.197036 pedal-2.5.5/pedal/resolvers/
--rw-rw-rw-   0        0        0     1043 2023-05-18 18:14:56.000000 pedal-2.5.5/pedal/resolvers/__init__.py
--rw-rw-rw-   0        0        0      650 2023-05-27 15:45:59.000000 pedal-2.5.5/pedal/resolvers/core.py
--rw-rw-rw-   0        0        0     1983 2023-06-20 18:25:54.000000 pedal-2.5.5/pedal/resolvers/export.py
--rw-rw-rw-   0        0        0     1823 2023-06-23 17:14:54.000000 pedal-2.5.5/pedal/resolvers/full.py
--rw-rw-rw-   0        0        0     1545 2023-05-26 21:21:46.000000 pedal-2.5.5/pedal/resolvers/sectional.py
--rw-rw-rw-   0        0        0      268 2021-01-26 15:52:26.000000 pedal-2.5.5/pedal/resolvers/silent.py
--rw-rw-rw-   0        0        0     4798 2023-05-26 21:21:54.000000 pedal-2.5.5/pedal/resolvers/simple.py
--rw-rw-rw-   0        0        0     1124 2023-05-26 21:34:10.000000 pedal-2.5.5/pedal/resolvers/statistics.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:43.217039 pedal-2.5.5/pedal/sandbox/
--rw-rw-rw-   0        0        0      662 2023-05-13 15:07:02.000000 pedal-2.5.5/pedal/sandbox/__init__.py
--rw-rw-rw-   0        0        0    18299 2023-06-28 02:55:07.000000 pedal-2.5.5/pedal/sandbox/commands.py
--rw-rw-rw-   0        0        0       72 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/sandbox/constants.py
--rw-rw-rw-   0        0        0     9807 2023-05-26 21:45:59.000000 pedal-2.5.5/pedal/sandbox/data.py
--rw-rw-rw-   0        0        0     1048 2021-02-24 17:20:18.000000 pedal-2.5.5/pedal/sandbox/exceptions.py
--rw-rw-rw-   0        0        0    10503 2023-06-29 17:39:28.000000 pedal-2.5.5/pedal/sandbox/feedbacks.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:43.227037 pedal-2.5.5/pedal/sandbox/library/
--rw-rw-rw-   0        0        0      222 2022-07-17 15:26:46.000000 pedal-2.5.5/pedal/sandbox/library/__init__.py
--rw-rw-rw-   0        0        0     5032 2023-05-27 15:46:08.000000 pedal-2.5.5/pedal/sandbox/library/designer.py
--rw-rw-rw-   0        0        0     5733 2022-07-17 15:20:41.000000 pedal-2.5.5/pedal/sandbox/library/matplotlib.py
--rw-rw-rw-   0        0        0     6973 2022-08-08 01:23:51.000000 pedal-2.5.5/pedal/sandbox/library/microbit.py
--rw-rw-rw-   0        0        0     3404 2023-05-27 15:46:26.000000 pedal-2.5.5/pedal/sandbox/library/turtles.py
--rw-rw-rw-   0        0        0    10132 2023-06-20 15:21:24.000000 pedal-2.5.5/pedal/sandbox/mocked.py
--rw-rw-rw-   0        0        0    14839 2022-11-25 23:20:23.000000 pedal-2.5.5/pedal/sandbox/result.py
--rw-rw-rw-   0        0        0    38840 2023-05-22 14:40:28.000000 pedal-2.5.5/pedal/sandbox/sandbox.py
--rw-rw-rw-   0        0        0     5048 2023-05-27 15:46:22.000000 pedal-2.5.5/pedal/sandbox/timeout.py
--rw-rw-rw-   0        0        0     5577 2021-10-28 00:27:49.000000 pedal-2.5.5/pedal/sandbox/tracer.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:43.238038 pedal-2.5.5/pedal/source/
--rw-rw-rw-   0        0        0      914 2023-05-27 15:44:56.000000 pedal-2.5.5/pedal/source/__init__.py
--rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/source/constants.py
--rw-rw-rw-   0        0        0     6539 2023-06-29 16:45:23.000000 pedal-2.5.5/pedal/source/feedbacks.py
--rw-rw-rw-   0        0        0     4609 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/source/sections.py
--rw-rw-rw-   0        0        0     7716 2023-06-10 14:14:43.000000 pedal-2.5.5/pedal/source/source.py
--rw-rw-rw-   0        0        0      484 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/source/substitutions.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:43.258038 pedal-2.5.5/pedal/tifa/
--rw-rw-rw-   0        0        0     3046 2023-05-27 15:47:23.000000 pedal-2.5.5/pedal/tifa/__init__.py
--rw-rw-rw-   0        0        0     2449 2023-06-23 17:11:58.000000 pedal-2.5.5/pedal/tifa/commands.py
--rw-rw-rw-   0        0        0       91 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/tifa/constants.py
--rw-rw-rw-   0        0        0     2833 2022-10-07 13:52:35.000000 pedal-2.5.5/pedal/tifa/contexts.py
--rw-rw-rw-   0        0        0    23656 2023-05-22 16:40:08.000000 pedal-2.5.5/pedal/tifa/feedbacks.py
--rw-rw-rw-   0        0        0     1171 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/tifa/identifier.py
--rw-rw-rw-   0        0        0      908 2022-06-07 19:06:45.000000 pedal-2.5.5/pedal/tifa/settings.py
--rw-rw-rw-   0        0        0     3649 2022-07-17 15:33:15.000000 pedal-2.5.5/pedal/tifa/state.py
--rw-rw-rw-   0        0        0    24283 2023-06-23 17:17:23.000000 pedal-2.5.5/pedal/tifa/tifa_core.py
--rw-rw-rw-   0        0        0    42742 2023-06-23 17:17:45.000000 pedal-2.5.5/pedal/tifa/tifa_visitor.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:43.269039 pedal-2.5.5/pedal/types/
--rw-rw-rw-   0        0        0       86 2022-06-09 18:41:53.000000 pedal-2.5.5/pedal/types/__init__.py
--rw-rw-rw-   0        0        0     9162 2023-05-27 15:45:10.000000 pedal-2.5.5/pedal/types/builtin.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:43.281038 pedal-2.5.5/pedal/types/library/
--rw-rw-rw-   0        0        0      192 2022-07-26 18:00:27.000000 pedal-2.5.5/pedal/types/library/__init__.py
--rw-rw-rw-   0        0        0      792 2022-11-28 05:46:58.000000 pedal-2.5.5/pedal/types/library/cs1_curriculum.py
--rw-rw-rw-   0        0        0     3499 2022-11-28 05:49:16.000000 pedal-2.5.5/pedal/types/library/designer.py
--rw-rw-rw-   0        0        0      792 2022-11-28 05:51:17.000000 pedal-2.5.5/pedal/types/library/matplotlib.py
--rw-rw-rw-   0        0        0     1615 2022-11-28 05:51:25.000000 pedal-2.5.5/pedal/types/library/microbit.py
--rw-rw-rw-   0        0        0      441 2022-11-28 05:52:06.000000 pedal-2.5.5/pedal/types/library/turtles.py
--rw-rw-rw-   0        0        0    51452 2023-06-23 17:23:01.000000 pedal-2.5.5/pedal/types/new_types.py
--rw-rw-rw-   0        0        0    15022 2023-06-23 16:26:55.000000 pedal-2.5.5/pedal/types/normalize.py
--rw-rw-rw-   0        0        0     8465 2022-10-21 18:56:52.000000 pedal-2.5.5/pedal/types/operations.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:56:43.305040 pedal-2.5.5/pedal/utilities/
--rw-rw-rw-   0        0        0      524 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/utilities/__init__.py
--rw-rw-rw-   0        0        0     6352 2022-09-19 04:45:01.000000 pedal-2.5.5/pedal/utilities/ast_tools.py
--rw-rw-rw-   0        0        0     6559 2023-06-23 17:07:40.000000 pedal-2.5.5/pedal/utilities/comparisons.py
--rw-rw-rw-   0        0        0      679 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/utilities/dictionaries.py
--rw-rw-rw-   0        0        0    10068 2023-06-30 15:15:29.000000 pedal-2.5.5/pedal/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1504 2021-02-04 17:26:41.000000 pedal-2.5.5/pedal/utilities/files.py
--rw-rw-rw-   0        0        0     1302 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/utilities/operators.py
--rw-rw-rw-   0        0        0     8215 2023-06-27 13:50:07.000000 pedal-2.5.5/pedal/utilities/progsnap.py
--rw-rw-rw-   0        0        0     1456 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/utilities/sorting.py
--rw-rw-rw-   0        0        0      449 2023-06-08 22:09:02.000000 pedal-2.5.5/pedal/utilities/system.py
--rw-rw-rw-   0        0        0     2457 2023-06-10 15:07:25.000000 pedal-2.5.5/pedal/utilities/text.py
--rw-rw-rw-   0        0        0      769 2020-10-17 16:15:22.000000 pedal-2.5.5/pedal/utilities/types.py
--rw-rw-rw-   0        0        0      121 2023-07-10 15:56:43.308038 pedal-2.5.5/setup.cfg
--rw-rw-rw-   0        0        0     1196 2023-07-10 15:56:28.000000 pedal-2.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:32:24.239469 pedal-2.5.6/
+-rw-rw-rw-   0        0        0     1103 2020-10-17 16:15:21.000000 pedal-2.5.6/LICENSE
+-rw-rw-rw-   0        0        0     2981 2023-07-13 16:32:24.239469 pedal-2.5.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-13 16:32:24.022467 pedal-2.5.6/Pedal.egg-info/
+-rw-rw-rw-   0        0        0     2981 2023-07-13 16:32:23.000000 pedal-2.5.6/Pedal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3826 2023-07-13 16:32:23.000000 pedal-2.5.6/Pedal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 16:32:23.000000 pedal-2.5.6/Pedal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-13 16:32:23.000000 pedal-2.5.6/Pedal.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-07-13 16:32:23.000000 pedal-2.5.6/Pedal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 16:32:23.000000 pedal-2.5.6/Pedal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1958 2023-06-14 16:24:47.000000 pedal-2.5.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-13 16:32:24.016465 pedal-2.5.6/pedal/
+-rw-rw-rw-   0        0        0      995 2023-07-04 14:03:45.000000 pedal-2.5.6/pedal/__init__.py
+-rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:32:24.044470 pedal-2.5.6/pedal/assertions/
+-rw-rw-rw-   0        0        0      665 2023-07-13 16:16:08.000000 pedal-2.5.6/pedal/assertions/__init__.py
+-rw-rw-rw-   0        0        0     8710 2022-09-25 02:42:31.000000 pedal-2.5.6/pedal/assertions/classes.py
+-rw-rw-rw-   0        0        0    13562 2023-06-23 17:14:33.000000 pedal-2.5.6/pedal/assertions/commands.py
+-rw-rw-rw-   0        0        0       73 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/assertions/constants.py
+-rw-rw-rw-   0        0        0    20355 2023-05-27 15:44:30.000000 pedal-2.5.6/pedal/assertions/feedbacks.py
+-rw-rw-rw-   0        0        0     8307 2021-12-05 16:26:04.000000 pedal-2.5.6/pedal/assertions/functions.py
+-rw-rw-rw-   0        0        0     4153 2023-06-23 17:06:54.000000 pedal-2.5.6/pedal/assertions/organizers.py
+-rw-rw-rw-   0        0        0      702 2023-07-13 15:41:54.000000 pedal-2.5.6/pedal/assertions/positive.py
+-rw-rw-rw-   0        0        0    33752 2023-05-22 19:35:19.000000 pedal-2.5.6/pedal/assertions/runtime.py
+-rw-rw-rw-   0        0        0     3316 2023-06-23 17:04:45.000000 pedal-2.5.6/pedal/assertions/setup.py
+-rw-rw-rw-   0        0        0    38421 2023-07-13 16:18:58.000000 pedal-2.5.6/pedal/assertions/static.py
+-rw-rw-rw-   0        0        0     6127 2023-07-13 16:14:45.000000 pedal-2.5.6/pedal/assertions/testing_libraries.py
+-rw-rw-rw-   0        0        0     6471 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/assertions/unittest.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:32:24.059467 pedal-2.5.6/pedal/cait/
+-rw-rw-rw-   0        0        0      445 2020-10-17 20:34:56.000000 pedal-2.5.6/pedal/cait/__init__.py
+-rw-rw-rw-   0        0        0     2255 2023-05-27 15:47:12.000000 pedal-2.5.6/pedal/cait/ast_helpers.py
+-rw-rw-rw-   0        0        0    11275 2023-06-23 17:10:06.000000 pedal-2.5.6/pedal/cait/ast_map.py
+-rw-rw-rw-   0        0        0    10523 2023-06-23 17:10:21.000000 pedal-2.5.6/pedal/cait/cait_api.py
+-rw-rw-rw-   0        0        0    23405 2023-07-06 23:15:07.000000 pedal-2.5.6/pedal/cait/cait_node.py
+-rw-rw-rw-   0        0        0       59 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/cait/constants.py
+-rw-rw-rw-   0        0        0     4693 2021-06-28 19:26:48.000000 pedal-2.5.6/pedal/cait/find_node.py
+-rw-rw-rw-   0        0        0    34016 2021-03-12 21:12:46.000000 pedal-2.5.6/pedal/cait/stretchy_tree_matching.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:32:24.070471 pedal-2.5.6/pedal/command_line/
+-rw-rw-rw-   0        0        0       94 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/command_line/__init__.py
+-rw-rw-rw-   0        0        0     8175 2023-06-30 18:05:29.000000 pedal-2.5.6/pedal/command_line/command_line.py
+-rw-rw-rw-   0        0        0     7301 2023-05-27 15:42:09.000000 pedal-2.5.6/pedal/command_line/mocks.py
+-rw-rw-rw-   0        0        0    24755 2023-07-13 13:42:53.000000 pedal-2.5.6/pedal/command_line/modes.py
+-rw-rw-rw-   0        0        0     3323 2022-03-26 13:30:52.000000 pedal-2.5.6/pedal/command_line/report.py
+-rw-rw-rw-   0        0        0     3549 2023-06-23 17:18:14.000000 pedal-2.5.6/pedal/command_line/verify.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:32:24.094466 pedal-2.5.6/pedal/core/
+-rw-rw-rw-   0        0        0      107 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/core/__init__.py
+-rw-rw-rw-   0        0        0     9411 2023-06-23 17:10:49.000000 pedal-2.5.6/pedal/core/commands.py
+-rw-rw-rw-   0        0        0     2687 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/core/environment.py
+-rw-rw-rw-   0        0        0      707 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/core/errors.py
+-rw-rw-rw-   0        0        0    21596 2023-07-06 13:54:34.000000 pedal-2.5.6/pedal/core/feedback.py
+-rw-rw-rw-   0        0        0     4173 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/core/feedback_category.py
+-rw-rw-rw-   0        0        0     7614 2023-06-14 16:05:08.000000 pedal-2.5.6/pedal/core/final_feedback.py
+-rw-rw-rw-   0        0        0     8147 2023-06-29 16:44:20.000000 pedal-2.5.6/pedal/core/formatting.py
+-rw-rw-rw-   0        0        0     1962 2023-05-26 21:48:15.000000 pedal-2.5.6/pedal/core/location.py
+-rw-rw-rw-   0        0        0    13916 2023-07-04 14:06:42.000000 pedal-2.5.6/pedal/core/report.py
+-rw-rw-rw-   0        0        0      822 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/core/resolver.py
+-rw-rw-rw-   0        0        0     3985 2022-11-17 14:35:11.000000 pedal-2.5.6/pedal/core/scoring.py
+-rw-rw-rw-   0        0        0     6266 2021-02-02 16:05:08.000000 pedal-2.5.6/pedal/core/submission.py
+-rw-rw-rw-   0        0        0      405 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/core/tag.py
+-rw-rw-rw-   0        0        0     2286 2023-01-17 16:07:35.000000 pedal-2.5.6/pedal/core/tool.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:32:24.111467 pedal-2.5.6/pedal/environments/
+-rw-rw-rw-   0        0        0      670 2023-06-14 15:19:32.000000 pedal-2.5.6/pedal/environments/__init__.py
+-rw-rw-rw-   0        0        0     3065 2023-06-28 02:43:06.000000 pedal-2.5.6/pedal/environments/blockpy.py
+-rw-rw-rw-   0        0        0     9910 2023-06-23 17:16:42.000000 pedal-2.5.6/pedal/environments/gradescope.py
+-rw-rw-rw-   0        0        0    15874 2021-01-26 15:29:49.000000 pedal-2.5.6/pedal/environments/jupyter.py
+-rw-rw-rw-   0        0        0    10369 2023-05-26 21:13:02.000000 pedal-2.5.6/pedal/environments/nbgrader.py
+-rw-rw-rw-   0        0        0      369 2023-06-08 11:46:52.000000 pedal-2.5.6/pedal/environments/none.py
+-rw-rw-rw-   0        0        0      766 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/environments/sandbox.py
+-rw-rw-rw-   0        0        0     3572 2023-06-28 02:44:25.000000 pedal-2.5.6/pedal/environments/standard.py
+-rw-rw-rw-   0        0        0     5528 2023-07-10 15:54:11.000000 pedal-2.5.6/pedal/environments/terminal.py
+-rw-rw-rw-   0        0        0     6673 2023-06-23 16:04:44.000000 pedal-2.5.6/pedal/environments/vpl.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:32:24.116467 pedal-2.5.6/pedal/extensions/
+-rw-rw-rw-   0        0        0        0 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/extensions/__init__.py
+-rw-rw-rw-   0        0        0    13908 2022-07-24 19:32:33.000000 pedal-2.5.6/pedal/extensions/microbit.py
+-rw-rw-rw-   0        0        0    11604 2022-11-26 00:03:07.000000 pedal-2.5.6/pedal/extensions/plotting.py
+-rw-rw-rw-   0        0        0       81 2022-07-17 15:14:06.000000 pedal-2.5.6/pedal/extensions/turtles.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:32:24.131466 pedal-2.5.6/pedal/questions/
+-rw-rw-rw-   0        0        0      669 2021-12-05 16:49:53.000000 pedal-2.5.6/pedal/questions/__init__.py
+-rw-rw-rw-   0        0        0       66 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/questions/constants.py
+-rw-rw-rw-   0        0        0      624 2021-09-15 19:16:10.000000 pedal-2.5.6/pedal/questions/feedbacks.py
+-rw-rw-rw-   0        0        0     6043 2023-05-27 15:45:43.000000 pedal-2.5.6/pedal/questions/graders.py
+-rw-rw-rw-   0        0        0     3477 2023-05-26 21:13:56.000000 pedal-2.5.6/pedal/questions/loader.py
+-rw-rw-rw-   0        0        0     2808 2021-12-05 15:58:25.000000 pedal-2.5.6/pedal/questions/pool.py
+-rw-rw-rw-   0        0        0     3784 2021-09-16 06:51:15.000000 pedal-2.5.6/pedal/questions/questions.py
+-rw-rw-rw-   0        0        0     1660 2022-11-11 17:53:28.000000 pedal-2.5.6/pedal/questions/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:32:24.144466 pedal-2.5.6/pedal/resolvers/
+-rw-rw-rw-   0        0        0     1043 2023-05-18 18:14:56.000000 pedal-2.5.6/pedal/resolvers/__init__.py
+-rw-rw-rw-   0        0        0      650 2023-05-27 15:45:59.000000 pedal-2.5.6/pedal/resolvers/core.py
+-rw-rw-rw-   0        0        0     1983 2023-06-20 18:25:54.000000 pedal-2.5.6/pedal/resolvers/export.py
+-rw-rw-rw-   0        0        0     1823 2023-06-23 17:14:54.000000 pedal-2.5.6/pedal/resolvers/full.py
+-rw-rw-rw-   0        0        0     1545 2023-05-26 21:21:46.000000 pedal-2.5.6/pedal/resolvers/sectional.py
+-rw-rw-rw-   0        0        0      268 2021-01-26 15:52:26.000000 pedal-2.5.6/pedal/resolvers/silent.py
+-rw-rw-rw-   0        0        0     4798 2023-05-26 21:21:54.000000 pedal-2.5.6/pedal/resolvers/simple.py
+-rw-rw-rw-   0        0        0     1124 2023-05-26 21:34:10.000000 pedal-2.5.6/pedal/resolvers/statistics.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:32:24.160466 pedal-2.5.6/pedal/sandbox/
+-rw-rw-rw-   0        0        0      662 2023-05-13 15:07:02.000000 pedal-2.5.6/pedal/sandbox/__init__.py
+-rw-rw-rw-   0        0        0    18299 2023-06-28 02:55:07.000000 pedal-2.5.6/pedal/sandbox/commands.py
+-rw-rw-rw-   0        0        0       72 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/sandbox/constants.py
+-rw-rw-rw-   0        0        0     9807 2023-05-26 21:45:59.000000 pedal-2.5.6/pedal/sandbox/data.py
+-rw-rw-rw-   0        0        0     1048 2021-02-24 17:20:18.000000 pedal-2.5.6/pedal/sandbox/exceptions.py
+-rw-rw-rw-   0        0        0    10503 2023-06-29 17:39:28.000000 pedal-2.5.6/pedal/sandbox/feedbacks.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:32:24.167469 pedal-2.5.6/pedal/sandbox/library/
+-rw-rw-rw-   0        0        0      222 2022-07-17 15:26:46.000000 pedal-2.5.6/pedal/sandbox/library/__init__.py
+-rw-rw-rw-   0        0        0     5032 2023-05-27 15:46:08.000000 pedal-2.5.6/pedal/sandbox/library/designer.py
+-rw-rw-rw-   0        0        0     5733 2022-07-17 15:20:41.000000 pedal-2.5.6/pedal/sandbox/library/matplotlib.py
+-rw-rw-rw-   0        0        0     6973 2022-08-08 01:23:51.000000 pedal-2.5.6/pedal/sandbox/library/microbit.py
+-rw-rw-rw-   0        0        0     3404 2023-05-27 15:46:26.000000 pedal-2.5.6/pedal/sandbox/library/turtles.py
+-rw-rw-rw-   0        0        0    10132 2023-06-20 15:21:24.000000 pedal-2.5.6/pedal/sandbox/mocked.py
+-rw-rw-rw-   0        0        0    14839 2022-11-25 23:20:23.000000 pedal-2.5.6/pedal/sandbox/result.py
+-rw-rw-rw-   0        0        0    38840 2023-05-22 14:40:28.000000 pedal-2.5.6/pedal/sandbox/sandbox.py
+-rw-rw-rw-   0        0        0     5048 2023-05-27 15:46:22.000000 pedal-2.5.6/pedal/sandbox/timeout.py
+-rw-rw-rw-   0        0        0     5577 2021-10-28 00:27:49.000000 pedal-2.5.6/pedal/sandbox/tracer.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:32:24.176466 pedal-2.5.6/pedal/source/
+-rw-rw-rw-   0        0        0      914 2023-05-27 15:44:56.000000 pedal-2.5.6/pedal/source/__init__.py
+-rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/source/constants.py
+-rw-rw-rw-   0        0        0     6539 2023-06-29 16:45:23.000000 pedal-2.5.6/pedal/source/feedbacks.py
+-rw-rw-rw-   0        0        0     4609 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/source/sections.py
+-rw-rw-rw-   0        0        0     7716 2023-06-10 14:14:43.000000 pedal-2.5.6/pedal/source/source.py
+-rw-rw-rw-   0        0        0      484 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/source/substitutions.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:32:24.194468 pedal-2.5.6/pedal/tifa/
+-rw-rw-rw-   0        0        0     3046 2023-05-27 15:47:23.000000 pedal-2.5.6/pedal/tifa/__init__.py
+-rw-rw-rw-   0        0        0     2449 2023-06-23 17:11:58.000000 pedal-2.5.6/pedal/tifa/commands.py
+-rw-rw-rw-   0        0        0       91 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/tifa/constants.py
+-rw-rw-rw-   0        0        0     2833 2022-10-07 13:52:35.000000 pedal-2.5.6/pedal/tifa/contexts.py
+-rw-rw-rw-   0        0        0    23656 2023-05-22 16:40:08.000000 pedal-2.5.6/pedal/tifa/feedbacks.py
+-rw-rw-rw-   0        0        0     1171 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/tifa/identifier.py
+-rw-rw-rw-   0        0        0      908 2022-06-07 19:06:45.000000 pedal-2.5.6/pedal/tifa/settings.py
+-rw-rw-rw-   0        0        0     3649 2022-07-17 15:33:15.000000 pedal-2.5.6/pedal/tifa/state.py
+-rw-rw-rw-   0        0        0    24283 2023-06-23 17:17:23.000000 pedal-2.5.6/pedal/tifa/tifa_core.py
+-rw-rw-rw-   0        0        0    42742 2023-06-23 17:17:45.000000 pedal-2.5.6/pedal/tifa/tifa_visitor.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:32:24.204519 pedal-2.5.6/pedal/types/
+-rw-rw-rw-   0        0        0       86 2022-06-09 18:41:53.000000 pedal-2.5.6/pedal/types/__init__.py
+-rw-rw-rw-   0        0        0     9162 2023-05-27 15:45:10.000000 pedal-2.5.6/pedal/types/builtin.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:32:24.215467 pedal-2.5.6/pedal/types/library/
+-rw-rw-rw-   0        0        0      192 2022-07-26 18:00:27.000000 pedal-2.5.6/pedal/types/library/__init__.py
+-rw-rw-rw-   0        0        0      792 2022-11-28 05:46:58.000000 pedal-2.5.6/pedal/types/library/cs1_curriculum.py
+-rw-rw-rw-   0        0        0     3499 2022-11-28 05:49:16.000000 pedal-2.5.6/pedal/types/library/designer.py
+-rw-rw-rw-   0        0        0      792 2022-11-28 05:51:17.000000 pedal-2.5.6/pedal/types/library/matplotlib.py
+-rw-rw-rw-   0        0        0     1615 2022-11-28 05:51:25.000000 pedal-2.5.6/pedal/types/library/microbit.py
+-rw-rw-rw-   0        0        0      441 2022-11-28 05:52:06.000000 pedal-2.5.6/pedal/types/library/turtles.py
+-rw-rw-rw-   0        0        0    51452 2023-06-23 17:23:01.000000 pedal-2.5.6/pedal/types/new_types.py
+-rw-rw-rw-   0        0        0    15022 2023-06-23 16:26:55.000000 pedal-2.5.6/pedal/types/normalize.py
+-rw-rw-rw-   0        0        0     8465 2022-10-21 18:56:52.000000 pedal-2.5.6/pedal/types/operations.py
+drwxrwxrwx   0        0        0        0 2023-07-13 16:32:24.238468 pedal-2.5.6/pedal/utilities/
+-rw-rw-rw-   0        0        0      524 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6352 2022-09-19 04:45:01.000000 pedal-2.5.6/pedal/utilities/ast_tools.py
+-rw-rw-rw-   0        0        0     6559 2023-06-23 17:07:40.000000 pedal-2.5.6/pedal/utilities/comparisons.py
+-rw-rw-rw-   0        0        0      679 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/utilities/dictionaries.py
+-rw-rw-rw-   0        0        0    10068 2023-06-30 15:15:29.000000 pedal-2.5.6/pedal/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1504 2021-02-04 17:26:41.000000 pedal-2.5.6/pedal/utilities/files.py
+-rw-rw-rw-   0        0        0     1302 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/utilities/operators.py
+-rw-rw-rw-   0        0        0     8215 2023-06-27 13:50:07.000000 pedal-2.5.6/pedal/utilities/progsnap.py
+-rw-rw-rw-   0        0        0     1456 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/utilities/sorting.py
+-rw-rw-rw-   0        0        0      449 2023-06-08 22:09:02.000000 pedal-2.5.6/pedal/utilities/system.py
+-rw-rw-rw-   0        0        0     2457 2023-06-10 15:07:25.000000 pedal-2.5.6/pedal/utilities/text.py
+-rw-rw-rw-   0        0        0      769 2020-10-17 16:15:22.000000 pedal-2.5.6/pedal/utilities/types.py
+-rw-rw-rw-   0        0        0      121 2023-07-13 16:32:24.240502 pedal-2.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     1196 2023-07-13 16:30:38.000000 pedal-2.5.6/setup.py
```

### Comparing `pedal-2.5.5/LICENSE` & `pedal-2.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/PKG-INFO` & `pedal-2.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pedal
-Version: 2.5.5
+Version: 2.5.6
 Summary: Tools to provide feedback on student code.
 Home-page: https://pedal-edu.github.io/pedal
 Author: acbart,lukesg08
 Author-email: acbart@udel.edu
 License: Creative Commons Attribution-Noncommercial-Share Alike license
 Description: Pedal
         =====
```

### Comparing `pedal-2.5.5/Pedal.egg-info/PKG-INFO` & `pedal-2.5.6/Pedal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pedal
-Version: 2.5.5
+Version: 2.5.6
 Summary: Tools to provide feedback on student code.
 Home-page: https://pedal-edu.github.io/pedal
 Author: acbart,lukesg08
 Author-email: acbart@udel.edu
 License: Creative Commons Attribution-Noncommercial-Share Alike license
 Description: Pedal
         =====
```

### Comparing `pedal-2.5.5/Pedal.egg-info/SOURCES.txt` & `pedal-2.5.6/Pedal.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,19 @@
 pedal/assertions/__init__.py
 pedal/assertions/classes.py
 pedal/assertions/commands.py
 pedal/assertions/constants.py
 pedal/assertions/feedbacks.py
 pedal/assertions/functions.py
 pedal/assertions/organizers.py
+pedal/assertions/positive.py
 pedal/assertions/runtime.py
 pedal/assertions/setup.py
 pedal/assertions/static.py
+pedal/assertions/testing_libraries.py
 pedal/assertions/unittest.py
 pedal/cait/__init__.py
 pedal/cait/ast_helpers.py
 pedal/cait/ast_map.py
 pedal/cait/cait_api.py
 pedal/cait/cait_node.py
 pedal/cait/constants.py
```

### Comparing `pedal-2.5.5/README.rst` & `pedal-2.5.6/README.rst`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/__init__.py` & `pedal-2.5.6/pedal/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/assertions/__init__.py` & `pedal-2.5.6/pedal/assertions/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 The assertions module contains classic unittest-style assert statements.
 """
 
 from pedal.assertions.setup import _setup_assertions, resolve_all
 from pedal.assertions.constants import TOOL_NAME
 from pedal.core.report import Report, MAIN_REPORT
 from pedal.assertions.commands import *
+from pedal.assertions.positive import close_output, correct_output
+from pedal.assertions.testing_libraries import *
 
 
 def reset(report=MAIN_REPORT):
     """
     Resets (or initializes) the information about assertions.
 
     Args:
```

### Comparing `pedal-2.5.5/pedal/assertions/classes.py` & `pedal-2.5.6/pedal/assertions/classes.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/assertions/commands.py` & `pedal-2.5.6/pedal/assertions/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/assertions/feedbacks.py` & `pedal-2.5.6/pedal/assertions/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/assertions/functions.py` & `pedal-2.5.6/pedal/assertions/functions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/assertions/organizers.py` & `pedal-2.5.6/pedal/assertions/organizers.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/assertions/runtime.py` & `pedal-2.5.6/pedal/assertions/runtime.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/assertions/setup.py` & `pedal-2.5.6/pedal/assertions/setup.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/assertions/static.py` & `pedal-2.5.6/pedal/assertions/static.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 
 from pedal.assertions.classes import (missing_dataclass, dataclass_not_available,
                                       missing_field_type, too_few_fields, too_many_fields,
                                       duplicate_dataclass_definition, invalid_field_type,
                                       wrong_fields_type, name_is_not_a_dataclass, missing_dataclass_annotation,
                                       unknown_field, wrong_field_order)
 from pedal.assertions.functions import *
-from pedal.cait.cait_api import parse_program
+from pedal.cait.cait_api import parse_program, find_match, find_matches
 from pedal.assertions.feedbacks import AssertionFeedback
 from pedal.cait.find_node import find_operation, find_function_calls, find_function_definition
-from pedal.core.feedback import CompositeFeedbackFunction
+from pedal.core.feedback import CompositeFeedbackFunction, Feedback, FeedbackResponse
 from pedal.core.location import Location
 from pedal.core.report import MAIN_REPORT
-from pedal.core.commands import compliment as core_compliment, give_partial
+from pedal.core.commands import compliment as core_compliment, give_partial, explain, gently
 from pedal.tifa.commands import tifa_type_check
 from pedal.types.normalize import normalize_type
 from pedal.types.new_types import is_subtype
 from pedal.utilities.ast_tools import AST_NODE_NAMES
 
 
 class EnsureAssertionFeedback(AssertionFeedback):
@@ -695,7 +695,210 @@
         super().__init__(fields=fields, **kwargs)
 
     def condition(self):
         """ Traverse the AST to find matches. """
         code = self.fields['code']
         ast = self.fields['root']
         return ast.find_match(code)
+
+
+class prevent_printing_functions(AssertionFeedback):
+    """
+    Detects if the user has defined a function with a print statement inside.
+
+    Args:
+        exceptions: A set of function names (or a single string) of functions to allow to print (e.g., `'main'`).
+    """
+    title = "Do Not Print in Function"
+    message_template = ("The function {name} is printing on line {location.line:line}."
+                        " However, that function is not supposed to print.")
+
+    def __init__(self, exceptions=None, root=None, **kwargs):
+        report = kwargs.get('report', MAIN_REPORT)
+        root = root or parse_program(report=report)
+        fields = {'root': root, 'exceptions': exceptions}
+        super().__init__(fields=fields, **kwargs)
+
+    def condition(self, *args, **kwargs):
+        exceptions = self.fields['exceptions']
+        if exceptions is None:
+            exceptions = set()
+        elif isinstance(exceptions, str):
+            exceptions = {exceptions}
+        root = self.fields['root']
+        defs = root.find_all("FunctionDef")
+        for a_def in defs:
+            name = a_def._name
+            if name in exceptions:
+                continue
+            for call in find_function_calls("print", root=a_def, report=self.report):
+                location = call.locate()
+                self.fields['name'] = name
+                self.update_location(location)
+                return True
+        return False
+
+
+class ensure_functions_return(AssertionFeedback):
+    """
+    Detects if the user has defined a function with a print statement inside.
+
+    Args:
+        exceptions: A set of function names (or a single string) of functions to allow to print (e.g., `'main'`).
+    """
+    title = "Must Return in Function"
+    message_template = ("The function {name} is not returning."
+                        " However, that function is supposed to have a return statement.")
+
+    def __init__(self, exceptions=None, root=None, **kwargs):
+        report = kwargs.get('report', MAIN_REPORT)
+        root = root or parse_program(report=report)
+        fields = {'root': root, 'exceptions': exceptions}
+        super().__init__(fields=fields, **kwargs)
+
+    def condition(self, *args, **kwargs):
+        exceptions = self.fields['exceptions']
+        if exceptions is None:
+            exceptions = set()
+        elif isinstance(exceptions, str):
+            exceptions = {exceptions}
+        root = self.fields['root']
+        defs = root.find_all("FunctionDef")
+        for a_def in defs:
+            name = a_def._name
+            if name in exceptions:
+                continue
+            if not a_def.find_match("return"):
+                self.fields['name'] = name
+                return True
+        return False
+
+
+class only_printing_variables(AssertionFeedback):
+    """
+    Determines whether the user is only printing variables, as opposed to
+    literal values.
+
+    """
+    title="Print Variables, Not Values"
+    message_template=("You printed something other than a variable on"
+                      " line {location.line:line}. Although that is not a"
+                      " normally an issue, we want you to practice printing"
+                      " variables in this problem.")
+
+    def __init__(self, root=None, **kwargs):
+        fields = kwargs.setdefault('fields', {})
+        report = kwargs.setdefault('report', MAIN_REPORT)
+        fields['root'] = root or parse_program(report=report)
+        super().__init__(**kwargs)
+
+    def condition(self):
+        """ Uses find_all to detect matches, ignoring named values. """
+        print_calls = find_function_calls('print', root=self.fields['root'],
+                                          report=self.report)
+        for print_call in print_calls:
+            for arg in print_call.args:
+                if arg.ast_name != "Name":
+                    self.update_location(print_call.lineno)
+                    return True
+                elif arg.id in ("True", "False", "None"):
+                    self.update_location(print_call.lineno)
+                    return True
+        return False
+
+
+ADVANCED_ITERATION_FUNCTIONS = [
+    "sum", "map", "filter", "reduce",
+    "len", "max", "min", "max",
+    "sorted", "all", "any",
+    "getattr", "setattr",
+    "eval", "exec", "iter", "next"
+]
+
+
+@CompositeFeedbackFunction()
+def prevent_advanced_iteration(allow_while=False, allow_for=False,
+                               allow_function=None, **kwargs):
+    """ Prevents the student from using certain advanced iteration functions
+    and constructs. Does not currently support blocking recursion. """
+    if isinstance(allow_function, str):
+        allow_function = {allow_function}
+    elif allow_function is None:
+        allow_function = set()
+    if not allow_while:
+        prevent_ast("While")
+    if not allow_for:
+        prevent_ast("For")
+    for function_name in ADVANCED_ITERATION_FUNCTIONS:
+        if function_name not in allow_function:
+            prevent_function_call(function_name, **kwargs)
+
+
+class open_without_arguments(FeedbackResponse):
+    """
+    Detects if the user has called the `open` function without any arguments.
+    """
+    muted = False
+    title = "Opened Without Arguments"
+    message_template = ("You have called the `open` function "
+                        "without any arguments. It needs a filename.")
+    category = Feedback.CATEGORIES.INSTRUCTOR
+
+
+@CompositeFeedbackFunction(open_without_arguments, ensure_literal)
+def files_not_handled_correctly(*filenames, muted=False):
+    """
+    Statically detect if files have been opened and closed correctly.
+    This is only useful in the case of very simplistic file handling.
+
+    TODO: This could be vastly improved with line numbers and other information.
+    """
+    if filenames and isinstance(filenames[0], int):
+        num_filenames = filenames[0]
+        actual_filenames = False
+    else:
+        num_filenames = len(filenames)
+        actual_filenames = True
+    ast = parse_program()
+    calls = ast.find_all("Call")
+    called_open = []
+    closed = []
+    for a_call in calls:
+        if a_call.func.ast_name == 'Name':
+            if a_call.func.id == 'open':
+                if not a_call.args:
+                    open_without_arguments(muted)
+                    return True
+                called_open.append(a_call)
+            elif a_call.func.id == 'close':
+                explain("You have attempted to call `close` as a "
+                        "function, but it is actually a method of the "
+                        "file object.", label="used_close_as_function", title="Close Is a Method", priority='syntax')
+                return True
+        elif a_call.func.ast_name == 'Attribute':
+            if a_call.func.attr == 'open':
+                # TODO: Make these feedback functions
+                explain("You have attempted to call `open` as a "
+                        "method, but it is actually a built-in function.", label="used_open_as_method",
+                        title="Open Is a Function")
+                return True
+            elif a_call.func.attr == 'close':
+                closed.append(a_call)
+    if len(called_open) < num_filenames:
+        explain("You have not opened all the files you were supposed to.", label="unopened_files", title="Unopened Files")
+        return True
+    elif len(called_open) > num_filenames:
+        explain("You have opened more files than you were supposed to.", label="extra_open_files", title="Extra Opened Files")
+        return True
+    withs = ast.find_all("With")
+    if len(withs) + len(closed) < num_filenames:
+        explain("You have not closed all the files you were supposed to.", label="unclosed_files", title="Unclosed Files")
+        return True
+    elif len(withs) + len(closed) > num_filenames:
+        explain("You have closed more files than you were supposed to.", label="extra_closed_files", title="Extra Closed Files")
+        return True
+    if actual_filenames:
+        for filename in filenames:
+            ensured = ensure_literal(filename)
+            if ensured:
+                return ensured
+    return False
```

### Comparing `pedal-2.5.5/pedal/assertions/unittest.py` & `pedal-2.5.6/pedal/assertions/unittest.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/cait/ast_helpers.py` & `pedal-2.5.6/pedal/cait/ast_helpers.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/cait/ast_map.py` & `pedal-2.5.6/pedal/cait/ast_map.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/cait/cait_api.py` & `pedal-2.5.6/pedal/cait/cait_api.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/cait/cait_node.py` & `pedal-2.5.6/pedal/cait/cait_node.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/cait/find_node.py` & `pedal-2.5.6/pedal/cait/find_node.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/cait/stretchy_tree_matching.py` & `pedal-2.5.6/pedal/cait/stretchy_tree_matching.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/command_line/command_line.py` & `pedal-2.5.6/pedal/command_line/command_line.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/command_line/mocks.py` & `pedal-2.5.6/pedal/command_line/mocks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/command_line/modes.py` & `pedal-2.5.6/pedal/command_line/modes.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/command_line/report.py` & `pedal-2.5.6/pedal/command_line/report.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/command_line/verify.py` & `pedal-2.5.6/pedal/command_line/verify.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/core/commands.py` & `pedal-2.5.6/pedal/core/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/core/environment.py` & `pedal-2.5.6/pedal/core/environment.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/core/errors.py` & `pedal-2.5.6/pedal/core/errors.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/core/feedback.py` & `pedal-2.5.6/pedal/core/feedback.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/core/feedback_category.py` & `pedal-2.5.6/pedal/core/feedback_category.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/core/final_feedback.py` & `pedal-2.5.6/pedal/core/final_feedback.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/core/formatting.py` & `pedal-2.5.6/pedal/core/formatting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/core/location.py` & `pedal-2.5.6/pedal/core/location.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/core/report.py` & `pedal-2.5.6/pedal/core/report.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/core/resolver.py` & `pedal-2.5.6/pedal/core/resolver.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/core/scoring.py` & `pedal-2.5.6/pedal/core/scoring.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/core/submission.py` & `pedal-2.5.6/pedal/core/submission.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/core/tool.py` & `pedal-2.5.6/pedal/core/tool.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/environments/__init__.py` & `pedal-2.5.6/pedal/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/environments/blockpy.py` & `pedal-2.5.6/pedal/environments/blockpy.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/environments/gradescope.py` & `pedal-2.5.6/pedal/environments/gradescope.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/environments/jupyter.py` & `pedal-2.5.6/pedal/environments/jupyter.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/environments/nbgrader.py` & `pedal-2.5.6/pedal/environments/nbgrader.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/environments/sandbox.py` & `pedal-2.5.6/pedal/environments/sandbox.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/environments/standard.py` & `pedal-2.5.6/pedal/environments/standard.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/environments/terminal.py` & `pedal-2.5.6/pedal/environments/terminal.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/environments/vpl.py` & `pedal-2.5.6/pedal/environments/vpl.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/extensions/microbit.py` & `pedal-2.5.6/pedal/extensions/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/extensions/plotting.py` & `pedal-2.5.6/pedal/extensions/plotting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/questions/__init__.py` & `pedal-2.5.6/pedal/questions/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/questions/feedbacks.py` & `pedal-2.5.6/pedal/questions/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/questions/graders.py` & `pedal-2.5.6/pedal/questions/graders.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/questions/loader.py` & `pedal-2.5.6/pedal/questions/loader.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/questions/pool.py` & `pedal-2.5.6/pedal/questions/pool.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/questions/questions.py` & `pedal-2.5.6/pedal/questions/questions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/questions/setup.py` & `pedal-2.5.6/pedal/questions/setup.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/resolvers/__init__.py` & `pedal-2.5.6/pedal/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/resolvers/core.py` & `pedal-2.5.6/pedal/resolvers/core.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/resolvers/export.py` & `pedal-2.5.6/pedal/resolvers/export.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/resolvers/full.py` & `pedal-2.5.6/pedal/resolvers/full.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/resolvers/sectional.py` & `pedal-2.5.6/pedal/resolvers/sectional.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/resolvers/simple.py` & `pedal-2.5.6/pedal/resolvers/simple.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/resolvers/statistics.py` & `pedal-2.5.6/pedal/resolvers/statistics.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/sandbox/__init__.py` & `pedal-2.5.6/pedal/sandbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/sandbox/commands.py` & `pedal-2.5.6/pedal/sandbox/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/sandbox/data.py` & `pedal-2.5.6/pedal/sandbox/data.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/sandbox/exceptions.py` & `pedal-2.5.6/pedal/sandbox/exceptions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/sandbox/feedbacks.py` & `pedal-2.5.6/pedal/sandbox/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/sandbox/library/designer.py` & `pedal-2.5.6/pedal/sandbox/library/designer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/sandbox/library/matplotlib.py` & `pedal-2.5.6/pedal/sandbox/library/matplotlib.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/sandbox/library/microbit.py` & `pedal-2.5.6/pedal/sandbox/library/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/sandbox/library/turtles.py` & `pedal-2.5.6/pedal/sandbox/library/turtles.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/sandbox/mocked.py` & `pedal-2.5.6/pedal/sandbox/mocked.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/sandbox/result.py` & `pedal-2.5.6/pedal/sandbox/result.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/sandbox/sandbox.py` & `pedal-2.5.6/pedal/sandbox/sandbox.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/sandbox/timeout.py` & `pedal-2.5.6/pedal/sandbox/timeout.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/sandbox/tracer.py` & `pedal-2.5.6/pedal/sandbox/tracer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/source/__init__.py` & `pedal-2.5.6/pedal/source/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/source/feedbacks.py` & `pedal-2.5.6/pedal/source/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/source/sections.py` & `pedal-2.5.6/pedal/source/sections.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/source/source.py` & `pedal-2.5.6/pedal/source/source.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/tifa/__init__.py` & `pedal-2.5.6/pedal/tifa/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/tifa/commands.py` & `pedal-2.5.6/pedal/tifa/commands.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/tifa/contexts.py` & `pedal-2.5.6/pedal/tifa/contexts.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/tifa/feedbacks.py` & `pedal-2.5.6/pedal/tifa/feedbacks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/tifa/identifier.py` & `pedal-2.5.6/pedal/tifa/identifier.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/tifa/settings.py` & `pedal-2.5.6/pedal/tifa/settings.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/tifa/state.py` & `pedal-2.5.6/pedal/tifa/state.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/tifa/tifa_core.py` & `pedal-2.5.6/pedal/tifa/tifa_core.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/tifa/tifa_visitor.py` & `pedal-2.5.6/pedal/tifa/tifa_visitor.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/types/builtin.py` & `pedal-2.5.6/pedal/types/builtin.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/types/library/cs1_curriculum.py` & `pedal-2.5.6/pedal/types/library/cs1_curriculum.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/types/library/designer.py` & `pedal-2.5.6/pedal/types/library/designer.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/types/library/matplotlib.py` & `pedal-2.5.6/pedal/types/library/matplotlib.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/types/library/microbit.py` & `pedal-2.5.6/pedal/types/library/microbit.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/types/new_types.py` & `pedal-2.5.6/pedal/types/new_types.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/types/normalize.py` & `pedal-2.5.6/pedal/types/normalize.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/types/operations.py` & `pedal-2.5.6/pedal/types/operations.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/utilities/__init__.py` & `pedal-2.5.6/pedal/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/utilities/ast_tools.py` & `pedal-2.5.6/pedal/utilities/ast_tools.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/utilities/comparisons.py` & `pedal-2.5.6/pedal/utilities/comparisons.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/utilities/dictionaries.py` & `pedal-2.5.6/pedal/utilities/dictionaries.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/utilities/exceptions.py` & `pedal-2.5.6/pedal/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/utilities/files.py` & `pedal-2.5.6/pedal/utilities/files.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/utilities/operators.py` & `pedal-2.5.6/pedal/utilities/operators.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/utilities/progsnap.py` & `pedal-2.5.6/pedal/utilities/progsnap.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/utilities/sorting.py` & `pedal-2.5.6/pedal/utilities/sorting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/utilities/text.py` & `pedal-2.5.6/pedal/utilities/text.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/pedal/utilities/types.py` & `pedal-2.5.6/pedal/utilities/types.py`

 * *Files identical despite different names*

### Comparing `pedal-2.5.5/setup.py` & `pedal-2.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='pedal',
-    version='2.5.5',
+    version='2.5.6',
     python_requires='>=3.7',
     author='acbart,lukesg08',
     author_email='acbart@udel.edu',
     description='Tools to provide feedback on student code.',
     keywords='feedback education teaching program analysis tifa cait sandbox pedal grading grader grade',
     packages=['pedal', 'pedal.core', 'pedal.utilities', 'pedal.environments',
               'pedal.resolvers', 'pedal.command_line',
```

