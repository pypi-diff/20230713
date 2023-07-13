# Comparing `tmp/conan-2.0.7.tar.gz` & `tmp/conan-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/conan-2.0.7.tar", last modified: Wed Jun 21 11:09:16 2023, max compression
+gzip compressed data, was "dist/conan-2.0.8.tar", last modified: Thu Jul 13 11:36:25 2023, max compression
```

## Comparing `conan-2.0.7.tar` & `conan-2.0.8.tar`

### file list

```diff
@@ -1,349 +1,350 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.930812 conan-2.0.7/
--rw-r--r--   0 root         (0) root         (0)     1084 2023-06-21 11:09:09.000000 conan-2.0.7/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-21 11:09:09.000000 conan-2.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8328 2023-06-21 11:09:16.931813 conan-2.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6045 2023-06-21 11:09:09.000000 conan-2.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.895809 conan-2.0.7/conan/
--rw-r--r--   0 root         (0) root         (0)      152 2023-06-21 11:09:09.000000 conan-2.0.7/conan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.897809 conan-2.0.7/conan/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-2.0.7/conan/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2360 2023-06-21 11:09:09.000000 conan-2.0.7/conan/api/conan_api.py
--rw-r--r--   0 root         (0) root         (0)     9995 2023-06-21 11:09:09.000000 conan-2.0.7/conan/api/model.py
--rw-r--r--   0 root         (0) root         (0)     8089 2023-06-21 11:09:09.000000 conan-2.0.7/conan/api/output.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.898809 conan-2.0.7/conan/api/subapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-2.0.7/conan/api/subapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4888 2023-06-21 11:09:09.000000 conan-2.0.7/conan/api/subapi/cache.py
--rw-r--r--   0 root         (0) root         (0)     1101 2023-06-21 11:09:09.000000 conan-2.0.7/conan/api/subapi/config.py
--rw-r--r--   0 root         (0) root         (0)     2897 2023-06-21 11:09:09.000000 conan-2.0.7/conan/api/subapi/download.py
--rw-r--r--   0 root         (0) root         (0)     2309 2023-06-21 11:09:09.000000 conan-2.0.7/conan/api/subapi/export.py
--rw-r--r--   0 root         (0) root         (0)    10725 2023-06-21 11:09:09.000000 conan-2.0.7/conan/api/subapi/graph.py
--rw-r--r--   0 root         (0) root         (0)     3101 2023-06-21 11:09:09.000000 conan-2.0.7/conan/api/subapi/install.py
--rw-r--r--   0 root         (0) root         (0)     7275 2023-06-21 11:09:09.000000 conan-2.0.7/conan/api/subapi/list.py
--rw-r--r--   0 root         (0) root         (0)     5110 2023-06-21 11:09:09.000000 conan-2.0.7/conan/api/subapi/local.py
--rw-r--r--   0 root         (0) root         (0)     4386 2023-06-21 11:09:09.000000 conan-2.0.7/conan/api/subapi/lockfile.py
--rw-r--r--   0 root         (0) root         (0)     4864 2023-06-21 11:09:09.000000 conan-2.0.7/conan/api/subapi/new.py
--rw-r--r--   0 root         (0) root         (0)     4426 2023-06-21 11:09:09.000000 conan-2.0.7/conan/api/subapi/profiles.py
--rw-r--r--   0 root         (0) root         (0)     4478 2023-06-21 11:09:09.000000 conan-2.0.7/conan/api/subapi/remotes.py
--rw-r--r--   0 root         (0) root         (0)     2212 2023-06-21 11:09:09.000000 conan-2.0.7/conan/api/subapi/remove.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-06-21 11:09:09.000000 conan-2.0.7/conan/api/subapi/search.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-06-21 11:09:09.000000 conan-2.0.7/conan/api/subapi/upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.899809 conan-2.0.7/conan/cli/
--rw-r--r--   0 root         (0) root         (0)      397 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7582 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/args.py
--rw-r--r--   0 root         (0) root         (0)    10968 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/cli.py
--rw-r--r--   0 root         (0) root         (0)     6240 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.902810 conan-2.0.7/conan/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3311 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/build.py
--rw-r--r--   0 root         (0) root         (0)     4648 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/cache.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/config.py
--rw-r--r--   0 root         (0) root         (0)     8291 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/create.py
--rw-r--r--   0 root         (0) root         (0)     4355 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/download.py
--rw-r--r--   0 root         (0) root         (0)     2708 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/editable.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/export.py
--rw-r--r--   0 root         (0) root         (0)     5587 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/export_pkg.py
--rw-r--r--   0 root         (0) root         (0)     8879 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/graph.py
--rw-r--r--   0 root         (0) root         (0)     2233 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/inspect.py
--rw-r--r--   0 root         (0) root         (0)     5003 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/install.py
--rw-r--r--   0 root         (0) root         (0)     6454 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/list.py
--rw-r--r--   0 root         (0) root         (0)     5485 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/lock.py
--rw-r--r--   0 root         (0) root         (0)     4239 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/new.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/profile.py
--rw-r--r--   0 root         (0) root         (0)    11410 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/remote.py
--rw-r--r--   0 root         (0) root         (0)     4862 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/remove.py
--rw-r--r--   0 root         (0) root         (0)     1754 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/search.py
--rw-r--r--   0 root         (0) root         (0)      648 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/source.py
--rw-r--r--   0 root         (0) root         (0)     3884 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/test.py
--rw-r--r--   0 root         (0) root         (0)     5977 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/upload.py
--rw-r--r--   0 root         (0) root         (0)      653 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)      490 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/exit_codes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.902810 conan-2.0.7/conan/cli/formatters/
--rw-r--r--   0 root         (0) root         (0)      158 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/formatters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.903810 conan-2.0.7/conan/cli/formatters/graph/
--rw-r--r--   0 root         (0) root         (0)      110 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/formatters/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5593 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/formatters/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)     1703 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/formatters/graph/graph_info_text.py
--rw-r--r--   0 root         (0) root         (0)      144 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/formatters/graph/info_graph_dot.py
--rw-r--r--   0 root         (0) root         (0)     7359 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/formatters/graph/info_graph_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.903810 conan-2.0.7/conan/cli/formatters/list/
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/formatters/list/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4612 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/formatters/list/binary_html_table.py
--rw-r--r--   0 root         (0) root         (0)      939 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/formatters/list/list.py
--rw-r--r--   0 root         (0) root         (0)    12834 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/formatters/list/search_table_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.903810 conan-2.0.7/conan/cli/printers/
--rw-r--r--   0 root         (0) root         (0)      331 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/printers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5660 2023-06-21 11:09:09.000000 conan-2.0.7/conan/cli/printers/graph.py
--rw-r--r--   0 root         (0) root         (0)      139 2023-06-21 11:09:09.000000 conan-2.0.7/conan/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.904810 conan-2.0.7/conan/internal/
--rw-r--r--   0 root         (0) root         (0)      419 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.904810 conan-2.0.7/conan/internal/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.906810 conan-2.0.7/conan/internal/api/new/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/api/new/__init__.py
--rw-r--r--   0 root         (0) root         (0)      293 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/api/new/alias_new.py
--rw-r--r--   0 root         (0) root         (0)     2716 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/api/new/autoools_exe.py
--rw-r--r--   0 root         (0) root         (0)     3781 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/api/new/autotools_lib.py
--rw-r--r--   0 root         (0) root         (0)     2843 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/api/new/basic.py
--rw-r--r--   0 root         (0) root         (0)     2066 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/api/new/bazel_exe.py
--rw-r--r--   0 root         (0) root         (0)     3596 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/api/new/bazel_lib.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/api/new/cmake_exe.py
--rw-r--r--   0 root         (0) root         (0)     8187 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/api/new/cmake_lib.py
--rw-r--r--   0 root         (0) root         (0)     2334 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/api/new/meson_exe.py
--rw-r--r--   0 root         (0) root         (0)     2740 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/api/new/meson_lib.py
--rw-r--r--   0 root         (0) root         (0)     2207 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/api/new/msbuild_exe.py
--rw-r--r--   0 root         (0) root         (0)    12247 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/api/new/msbuild_lib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.906810 conan-2.0.7/conan/internal/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9923 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/cache/cache.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/cache/conan_reference_layout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.907810 conan-2.0.7/conan/internal/cache/db/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/cache/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3170 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/cache/db/cache_database.py
--rw-r--r--   0 root         (0) root         (0)     7953 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/cache/db/packages_table.py
--rw-r--r--   0 root         (0) root         (0)     4791 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/cache/db/recipes_table.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/cache/db/table.py
--rw-r--r--   0 root         (0) root         (0)     2617 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/conan_app.py
--rw-r--r--   0 root         (0) root         (0)     3522 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/deploy.py
--rw-r--r--   0 root         (0) root         (0)     2468 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/integrity_check.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-06-21 11:09:09.000000 conan-2.0.7/conan/internal/upload_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.907810 conan-2.0.7/conan/tools/
--rw-r--r--   0 root         (0) root         (0)      384 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.907810 conan-2.0.7/conan/tools/android/
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/android/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1138 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/android/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.908810 conan-2.0.7/conan/tools/apple/
--rw-r--r--   0 root         (0) root         (0)      534 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/apple/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11200 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/apple/apple.py
--rw-r--r--   0 root         (0) root         (0)     2167 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/apple/xcodebuild.py
--rw-r--r--   0 root         (0) root         (0)    16379 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/apple/xcodedeps.py
--rw-r--r--   0 root         (0) root         (0)     5683 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/apple/xcodetoolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.908810 conan-2.0.7/conan/tools/build/
--rw-r--r--   0 root         (0) root         (0)     4142 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/build/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11103 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/build/cppstd.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/build/cpu.py
--rw-r--r--   0 root         (0) root         (0)     2043 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/build/cross_building.py
--rw-r--r--   0 root         (0) root         (0)    15391 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/build/flags.py
--rw-r--r--   0 root         (0) root         (0)      563 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/build/stdcpp_library.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.909810 conan-2.0.7/conan/tools/cmake/
--rw-r--r--   0 root         (0) root         (0)      217 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/cmake/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11124 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/cmake/cmake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.909810 conan-2.0.7/conan/tools/cmake/cmakedeps/
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/cmake/cmakedeps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8168 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/cmake/cmakedeps/cmakedeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.910811 conan-2.0.7/conan/tools/cmake/cmakedeps/templates/
--rw-r--r--   0 root         (0) root         (0)     3944 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/cmake/cmakedeps/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4451 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/cmake/cmakedeps/templates/config.py
--rw-r--r--   0 root         (0) root         (0)     1613 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/cmake/cmakedeps/templates/config_version.py
--rw-r--r--   0 root         (0) root         (0)     5704 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/cmake/cmakedeps/templates/macros.py
--rw-r--r--   0 root         (0) root         (0)    14925 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/cmake/cmakedeps/templates/target_configuration.py
--rw-r--r--   0 root         (0) root         (0)    19857 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/cmake/cmakedeps/templates/target_data.py
--rw-r--r--   0 root         (0) root         (0)     3916 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/cmake/cmakedeps/templates/targets.py
--rw-r--r--   0 root         (0) root         (0)     4044 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/cmake/layout.py
--rw-r--r--   0 root         (0) root         (0)    14422 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/cmake/presets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.910811 conan-2.0.7/conan/tools/cmake/toolchain/
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/cmake/toolchain/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35960 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/cmake/toolchain/blocks.py
--rw-r--r--   0 root         (0) root         (0)    11204 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/cmake/toolchain/toolchain.py
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/cmake/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.911810 conan-2.0.7/conan/tools/env/
--rw-r--r--   0 root         (0) root         (0)      168 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/env/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25388 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/env/environment.py
--rw-r--r--   0 root         (0) root         (0)     3233 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/env/virtualbuildenv.py
--rw-r--r--   0 root         (0) root         (0)     3394 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/env/virtualrunenv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.912811 conan-2.0.7/conan/tools/files/
--rw-r--r--   0 root         (0) root         (0)      519 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/files/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1467 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/files/conandata.py
--rw-r--r--   0 root         (0) root         (0)     6009 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/files/copy_pattern.py
--rw-r--r--   0 root         (0) root         (0)    23768 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/files/files.py
--rw-r--r--   0 root         (0) root         (0)     4177 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/files/packager.py
--rw-r--r--   0 root         (0) root         (0)     5823 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/files/patches.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.912811 conan-2.0.7/conan/tools/files/symlinks/
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/files/symlinks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2456 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/files/symlinks/symlinks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.913811 conan-2.0.7/conan/tools/gnu/
--rw-r--r--   0 root         (0) root         (0)      274 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/gnu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6234 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/gnu/autotools.py
--rw-r--r--   0 root         (0) root         (0)     2962 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/gnu/autotoolsdeps.py
--rw-r--r--   0 root         (0) root         (0)    13227 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/gnu/autotoolstoolchain.py
--rw-r--r--   0 root         (0) root         (0)     3556 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/gnu/get_gnu_triplet.py
--rw-r--r--   0 root         (0) root         (0)     3596 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/gnu/gnudeps_flags.py
--rw-r--r--   0 root         (0) root         (0)     4028 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/gnu/pkgconfig.py
--rw-r--r--   0 root         (0) root         (0)    18557 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/gnu/pkgconfigdeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.914811 conan-2.0.7/conan/tools/google/
--rw-r--r--   0 root         (0) root         (0)      201 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/google/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1806 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/google/bazel.py
--rw-r--r--   0 root         (0) root         (0)    10955 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/google/bazeldeps.py
--rw-r--r--   0 root         (0) root         (0)      585 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/google/layout.py
--rw-r--r--   0 root         (0) root         (0)      857 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/google/toolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.914811 conan-2.0.7/conan/tools/intel/
--rw-r--r--   0 root         (0) root         (0)       47 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/intel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6498 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/intel/intel_cc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.914811 conan-2.0.7/conan/tools/layout/
--rw-r--r--   0 root         (0) root         (0)      605 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/layout/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.914811 conan-2.0.7/conan/tools/meson/
--rw-r--r--   0 root         (0) root         (0)       98 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/meson/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4073 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/meson/helpers.py
--rw-r--r--   0 root         (0) root         (0)     4954 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/meson/meson.py
--rw-r--r--   0 root         (0) root         (0)    22060 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/meson/toolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.915811 conan-2.0.7/conan/tools/microsoft/
--rw-r--r--   0 root         (0) root         (0)      558 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/microsoft/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1335 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/microsoft/layout.py
--rw-r--r--   0 root         (0) root         (0)     3312 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/microsoft/msbuild.py
--rw-r--r--   0 root         (0) root         (0)    19214 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/microsoft/msbuilddeps.py
--rw-r--r--   0 root         (0) root         (0)     2965 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/microsoft/nmakedeps.py
--rw-r--r--   0 root         (0) root         (0)     4989 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/microsoft/nmaketoolchain.py
--rw-r--r--   0 root         (0) root         (0)      593 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/microsoft/subsystems.py
--rw-r--r--   0 root         (0) root         (0)    10843 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/microsoft/toolchain.py
--rw-r--r--   0 root         (0) root         (0)    13069 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/microsoft/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.916811 conan-2.0.7/conan/tools/premake/
--rw-r--r--   0 root         (0) root         (0)      103 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/premake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/premake/premake.py
--rw-r--r--   0 root         (0) root         (0)    10534 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/premake/premakedeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.916811 conan-2.0.7/conan/tools/qbs/
--rw-r--r--   0 root         (0) root         (0)      152 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/qbs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2901 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/qbs/qbs.py
--rw-r--r--   0 root         (0) root         (0)     9873 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/qbs/qbsprofile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.916811 conan-2.0.7/conan/tools/scm/
--rw-r--r--   0 root         (0) root         (0)       77 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/scm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8718 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/scm/git.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.917811 conan-2.0.7/conan/tools/system/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/system/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16285 2023-06-21 11:09:09.000000 conan-2.0.7/conan/tools/system/package_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.896809 conan-2.0.7/conan.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8328 2023-06-21 11:09:16.000000 conan-2.0.7/conan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9036 2023-06-21 11:09:16.000000 conan-2.0.7/conan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 11:09:16.000000 conan-2.0.7/conan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-06-21 11:09:16.000000 conan-2.0.7/conan.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      469 2023-06-21 11:09:16.000000 conan-2.0.7/conan.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 11:09:16.000000 conan-2.0.7/conan.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.918811 conan-2.0.7/conans/
--rw-r--r--   0 root         (0) root         (0)      201 2023-06-21 11:09:09.000000 conan-2.0.7/conans/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.919811 conan-2.0.7/conans/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.920812 conan-2.0.7/conans/client/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10525 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/cache/cache.py
--rw-r--r--   0 root         (0) root         (0)     2033 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/cache/editable.py
--rw-r--r--   0 root         (0) root         (0)     6569 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/cache/remote_registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.920812 conan-2.0.7/conans/client/cmd/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/cmd/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7671 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/cmd/export.py
--rw-r--r--   0 root         (0) root         (0)    12762 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/cmd/uploader.py
--rw-r--r--   0 root         (0) root         (0)      968 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/cmd/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.921811 conan-2.0.7/conans/client/conanfile/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/conanfile/__init__.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/conanfile/build.py
--rw-r--r--   0 root         (0) root         (0)     2208 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/conanfile/configure.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/conanfile/package.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.921811 conan-2.0.7/conans/client/conf/
--rw-r--r--   0 root         (0) root         (0)     6356 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9195 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/conf/config_installer.py
--rw-r--r--   0 root         (0) root         (0)    14019 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/conf/detect.py
--rw-r--r--   0 root         (0) root         (0)     5473 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/conf/detect_vs.py
--rw-r--r--   0 root         (0) root         (0)     1363 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/conf/required_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.922812 conan-2.0.7/conans/client/downloaders/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/downloaders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9512 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/downloaders/caching_file_downloader.py
--rw-r--r--   0 root         (0) root         (0)     4228 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/downloaders/download_cache.py
--rw-r--r--   0 root         (0) root         (0)     6723 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/downloaders/file_downloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.922812 conan-2.0.7/conans/client/generators/
--rw-r--r--   0 root         (0) root         (0)     9708 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/generators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.924812 conan-2.0.7/conans/client/graph/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4837 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/graph/build_mode.py
--rw-r--r--   0 root         (0) root         (0)     4571 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/graph/compatibility.py
--rw-r--r--   0 root         (0) root         (0)     3832 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/graph/compute_pid.py
--rw-r--r--   0 root         (0) root         (0)    14948 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)    16759 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/graph/graph_binaries.py
--rw-r--r--   0 root         (0) root         (0)    17797 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/graph/graph_builder.py
--rw-r--r--   0 root         (0) root         (0)     2668 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/graph/graph_error.py
--rw-r--r--   0 root         (0) root         (0)    12486 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/graph/install_graph.py
--rw-r--r--   0 root         (0) root         (0)     4163 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/graph/profile_node_definer.py
--rw-r--r--   0 root         (0) root         (0)     1529 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/graph/provides.py
--rw-r--r--   0 root         (0) root         (0)     6594 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/graph/proxy.py
--rw-r--r--   0 root         (0) root         (0)     5806 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/graph/python_requires.py
--rw-r--r--   0 root         (0) root         (0)     4692 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/graph/range_resolver.py
--rw-r--r--   0 root         (0) root         (0)     2595 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/hook_manager.py
--rw-r--r--   0 root         (0) root         (0)    21259 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/installer.py
--rw-r--r--   0 root         (0) root         (0)    15815 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/loader.py
--rw-r--r--   0 root         (0) root         (0)     1829 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/loader_txt.py
--rw-r--r--   0 root         (0) root         (0)     1860 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/migrations.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/pkg_sign.py
--rw-r--r--   0 root         (0) root         (0)    16848 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/profile_loader.py
--rw-r--r--   0 root         (0) root         (0)    13519 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/remote_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.925812 conan-2.0.7/conans/client/rest/
--rw-r--r--   0 root         (0) root         (0)      838 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5987 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/rest/auth_manager.py
--rw-r--r--   0 root         (0) root         (0)     6132 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/rest/client_routes.py
--rw-r--r--   0 root         (0) root         (0)     6894 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/rest/conan_requester.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/rest/file_uploader.py
--rw-r--r--   0 root         (0) root         (0)     5488 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/rest/rest_client.py
--rw-r--r--   0 root         (0) root         (0)    10011 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/rest/rest_client_common.py
--rw-r--r--   0 root         (0) root         (0)    14018 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/rest/rest_client_v2.py
--rw-r--r--   0 root         (0) root         (0)     3606 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.925812 conan-2.0.7/conans/client/store/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/store/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4305 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/store/localdb.py
--rw-r--r--   0 root         (0) root         (0)     8798 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/subsystems.py
--rw-r--r--   0 root         (0) root         (0)     5457 2023-06-21 11:09:09.000000 conan-2.0.7/conans/client/userio.py
--rwxr-xr-x   0 root         (0) root         (0)      118 2023-06-21 11:09:09.000000 conan-2.0.7/conans/conan.py
--rw-r--r--   0 root         (0) root         (0)      699 2023-06-21 11:09:09.000000 conan-2.0.7/conans/conan_server.py
--rw-r--r--   0 root         (0) root         (0)     7817 2023-06-21 11:09:09.000000 conan-2.0.7/conans/errors.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-06-21 11:09:09.000000 conan-2.0.7/conans/migrations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.927812 conan-2.0.7/conans/model/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-2.0.7/conans/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20745 2023-06-21 11:09:09.000000 conan-2.0.7/conans/model/build_info.py
--rw-r--r--   0 root         (0) root         (0)    12420 2023-06-21 11:09:09.000000 conan-2.0.7/conans/model/conan_file.py
--rw-r--r--   0 root         (0) root         (0)     2775 2023-06-21 11:09:09.000000 conan-2.0.7/conans/model/conanfile_interface.py
--rw-r--r--   0 root         (0) root         (0)    29771 2023-06-21 11:09:09.000000 conan-2.0.7/conans/model/conf.py
--rw-r--r--   0 root         (0) root         (0)     5901 2023-06-21 11:09:09.000000 conan-2.0.7/conans/model/dependencies.py
--rw-r--r--   0 root         (0) root         (0)    10886 2023-06-21 11:09:09.000000 conan-2.0.7/conans/model/graph_lock.py
--rw-r--r--   0 root         (0) root         (0)    13067 2023-06-21 11:09:09.000000 conan-2.0.7/conans/model/info.py
--rw-r--r--   0 root         (0) root         (0)     5247 2023-06-21 11:09:09.000000 conan-2.0.7/conans/model/layout.py
--rw-r--r--   0 root         (0) root         (0)     4883 2023-06-21 11:09:09.000000 conan-2.0.7/conans/model/manifest.py
--rw-r--r--   0 root         (0) root         (0)    17174 2023-06-21 11:09:09.000000 conan-2.0.7/conans/model/options.py
--rw-r--r--   0 root         (0) root         (0)     3861 2023-06-21 11:09:09.000000 conan-2.0.7/conans/model/package_ref.py
--rw-r--r--   0 root         (0) root         (0)     2320 2023-06-21 11:09:09.000000 conan-2.0.7/conans/model/pkg_type.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-06-21 11:09:09.000000 conan-2.0.7/conans/model/profile.py
--rw-r--r--   0 root         (0) root         (0)     7612 2023-06-21 11:09:09.000000 conan-2.0.7/conans/model/recipe_ref.py
--rw-r--r--   0 root         (0) root         (0)    24646 2023-06-21 11:09:09.000000 conan-2.0.7/conans/model/requires.py
--rw-r--r--   0 root         (0) root         (0)     2171 2023-06-21 11:09:09.000000 conan-2.0.7/conans/model/rest_routes.py
--rw-r--r--   0 root         (0) root         (0)    13368 2023-06-21 11:09:09.000000 conan-2.0.7/conans/model/settings.py
--rw-r--r--   0 root         (0) root         (0)     6038 2023-06-21 11:09:09.000000 conan-2.0.7/conans/model/version.py
--rw-r--r--   0 root         (0) root         (0)     4350 2023-06-21 11:09:09.000000 conan-2.0.7/conans/model/version_range.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.927812 conan-2.0.7/conans/paths/
--rw-r--r--   0 root         (0) root         (0)     2184 2023-06-21 11:09:09.000000 conan-2.0.7/conans/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2883 2023-06-21 11:09:09.000000 conan-2.0.7/conans/pylint_plugin.py
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-21 11:09:09.000000 conan-2.0.7/conans/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-21 11:09:09.000000 conan-2.0.7/conans/requirements_dev.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-21 11:09:09.000000 conan-2.0.7/conans/requirements_server.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.928812 conan-2.0.7/conans/search/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-2.0.7/conans/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3814 2023-06-21 11:09:09.000000 conan-2.0.7/conans/search/query_parse.py
--rw-r--r--   0 root         (0) root         (0)     4474 2023-06-21 11:09:09.000000 conan-2.0.7/conans/search/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.928812 conan-2.0.7/conans/test/
--rw-r--r--   0 root         (0) root         (0)      203 2023-06-21 11:09:09.000000 conan-2.0.7/conans/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13174 2023-06-21 11:09:09.000000 conan-2.0.7/conans/test/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.929812 conan-2.0.7/conans/test/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-2.0.7/conans/test/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4868 2023-06-21 11:09:09.000000 conan-2.0.7/conans/test/utils/artifactory.py
--rw-r--r--   0 root         (0) root         (0)     4852 2023-06-21 11:09:09.000000 conan-2.0.7/conans/test/utils/mocks.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-06-21 11:09:09.000000 conan-2.0.7/conans/test/utils/profiles.py
--rw-r--r--   0 root         (0) root         (0)     2038 2023-06-21 11:09:09.000000 conan-2.0.7/conans/test/utils/scm.py
--rw-r--r--   0 root         (0) root         (0)     3858 2023-06-21 11:09:09.000000 conan-2.0.7/conans/test/utils/server_launcher.py
--rw-r--r--   0 root         (0) root         (0)     3071 2023-06-21 11:09:09.000000 conan-2.0.7/conans/test/utils/test_files.py
--rw-r--r--   0 root         (0) root         (0)    35487 2023-06-21 11:09:09.000000 conan-2.0.7/conans/test/utils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 11:09:16.930812 conan-2.0.7/conans/util/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 11:09:09.000000 conan-2.0.7/conans/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-06-21 11:09:09.000000 conan-2.0.7/conans/util/config_parser.py
--rw-r--r--   0 root         (0) root         (0)     1516 2023-06-21 11:09:09.000000 conan-2.0.7/conans/util/dates.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-06-21 11:09:09.000000 conan-2.0.7/conans/util/encrypt.py
--rw-r--r--   0 root         (0) root         (0)     1437 2023-06-21 11:09:09.000000 conan-2.0.7/conans/util/env.py
--rw-r--r--   0 root         (0) root         (0)    12086 2023-06-21 11:09:09.000000 conan-2.0.7/conans/util/files.py
--rw-r--r--   0 root         (0) root         (0)     3657 2023-06-21 11:09:09.000000 conan-2.0.7/conans/util/locks.py
--rw-r--r--   0 root         (0) root         (0)     3688 2023-06-21 11:09:09.000000 conan-2.0.7/conans/util/runners.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-06-21 11:09:09.000000 conan-2.0.7/conans/util/sha.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-06-21 11:09:09.000000 conan-2.0.7/conans/util/thread.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-06-21 11:09:09.000000 conan-2.0.7/conans/util/windows.py
--rw-r--r--   0 root         (0) root         (0)      101 2023-06-21 11:09:16.931813 conan-2.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5058 2023-06-21 11:09:09.000000 conan-2.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.912234 conan-2.0.8/
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-07-13 11:36:17.000000 conan-2.0.8/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-13 11:36:17.000000 conan-2.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8328 2023-07-13 11:36:25.912234 conan-2.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6045 2023-07-13 11:36:17.000000 conan-2.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.873231 conan-2.0.8/conan/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-07-13 11:36:17.000000 conan-2.0.8/conan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.875232 conan-2.0.8/conan/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 11:36:17.000000 conan-2.0.8/conan/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2360 2023-07-13 11:36:17.000000 conan-2.0.8/conan/api/conan_api.py
+-rw-r--r--   0 root         (0) root         (0)     9995 2023-07-13 11:36:17.000000 conan-2.0.8/conan/api/model.py
+-rw-r--r--   0 root         (0) root         (0)     8089 2023-07-13 11:36:17.000000 conan-2.0.8/conan/api/output.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.877232 conan-2.0.8/conan/api/subapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 11:36:17.000000 conan-2.0.8/conan/api/subapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4894 2023-07-13 11:36:17.000000 conan-2.0.8/conan/api/subapi/cache.py
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-07-13 11:36:17.000000 conan-2.0.8/conan/api/subapi/config.py
+-rw-r--r--   0 root         (0) root         (0)     2530 2023-07-13 11:36:17.000000 conan-2.0.8/conan/api/subapi/download.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-07-13 11:36:17.000000 conan-2.0.8/conan/api/subapi/export.py
+-rw-r--r--   0 root         (0) root         (0)    10725 2023-07-13 11:36:17.000000 conan-2.0.8/conan/api/subapi/graph.py
+-rw-r--r--   0 root         (0) root         (0)     3101 2023-07-13 11:36:17.000000 conan-2.0.8/conan/api/subapi/install.py
+-rw-r--r--   0 root         (0) root         (0)     7275 2023-07-13 11:36:17.000000 conan-2.0.8/conan/api/subapi/list.py
+-rw-r--r--   0 root         (0) root         (0)     5110 2023-07-13 11:36:17.000000 conan-2.0.8/conan/api/subapi/local.py
+-rw-r--r--   0 root         (0) root         (0)     4386 2023-07-13 11:36:17.000000 conan-2.0.8/conan/api/subapi/lockfile.py
+-rw-r--r--   0 root         (0) root         (0)     4864 2023-07-13 11:36:17.000000 conan-2.0.8/conan/api/subapi/new.py
+-rw-r--r--   0 root         (0) root         (0)     4426 2023-07-13 11:36:17.000000 conan-2.0.8/conan/api/subapi/profiles.py
+-rw-r--r--   0 root         (0) root         (0)     4478 2023-07-13 11:36:17.000000 conan-2.0.8/conan/api/subapi/remotes.py
+-rw-r--r--   0 root         (0) root         (0)     2215 2023-07-13 11:36:17.000000 conan-2.0.8/conan/api/subapi/remove.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-07-13 11:36:17.000000 conan-2.0.8/conan/api/subapi/search.py
+-rw-r--r--   0 root         (0) root         (0)     4468 2023-07-13 11:36:17.000000 conan-2.0.8/conan/api/subapi/upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.877232 conan-2.0.8/conan/cli/
+-rw-r--r--   0 root         (0) root         (0)      397 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7582 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/args.py
+-rw-r--r--   0 root         (0) root         (0)    10968 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     6240 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.881232 conan-2.0.8/conan/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3311 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/build.py
+-rw-r--r--   0 root         (0) root         (0)     4728 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/cache.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/config.py
+-rw-r--r--   0 root         (0) root         (0)     8291 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/create.py
+-rw-r--r--   0 root         (0) root         (0)     4355 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/download.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/editable.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/export.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/export_pkg.py
+-rw-r--r--   0 root         (0) root         (0)     8879 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/graph.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/inspect.py
+-rw-r--r--   0 root         (0) root         (0)     5003 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/install.py
+-rw-r--r--   0 root         (0) root         (0)     6454 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/list.py
+-rw-r--r--   0 root         (0) root         (0)     5485 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/lock.py
+-rw-r--r--   0 root         (0) root         (0)     4239 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/new.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/profile.py
+-rw-r--r--   0 root         (0) root         (0)    11410 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/remote.py
+-rw-r--r--   0 root         (0) root         (0)     4862 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/remove.py
+-rw-r--r--   0 root         (0) root         (0)     1754 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/search.py
+-rw-r--r--   0 root         (0) root         (0)      648 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/source.py
+-rw-r--r--   0 root         (0) root         (0)     3884 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/test.py
+-rw-r--r--   0 root         (0) root         (0)     6293 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/upload.py
+-rw-r--r--   0 root         (0) root         (0)      653 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/exit_codes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.881232 conan-2.0.8/conan/cli/formatters/
+-rw-r--r--   0 root         (0) root         (0)      158 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/formatters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.882232 conan-2.0.8/conan/cli/formatters/graph/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/formatters/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5376 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/formatters/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1703 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/formatters/graph/graph_info_text.py
+-rw-r--r--   0 root         (0) root         (0)      144 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/formatters/graph/info_graph_dot.py
+-rw-r--r--   0 root         (0) root         (0)     8452 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/formatters/graph/info_graph_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.883232 conan-2.0.8/conan/cli/formatters/list/
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/formatters/list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4612 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/formatters/list/binary_html_table.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/formatters/list/list.py
+-rw-r--r--   0 root         (0) root         (0)    12834 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/formatters/list/search_table_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.883232 conan-2.0.8/conan/cli/printers/
+-rw-r--r--   0 root         (0) root         (0)      331 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/printers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5660 2023-07-13 11:36:17.000000 conan-2.0.8/conan/cli/printers/graph.py
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-13 11:36:17.000000 conan-2.0.8/conan/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.884232 conan-2.0.8/conan/internal/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.884232 conan-2.0.8/conan/internal/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.885232 conan-2.0.8/conan/internal/api/new/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/api/new/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      293 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/api/new/alias_new.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/api/new/autoools_exe.py
+-rw-r--r--   0 root         (0) root         (0)     3810 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/api/new/autotools_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2916 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/api/new/basic.py
+-rw-r--r--   0 root         (0) root         (0)     2066 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/api/new/bazel_exe.py
+-rw-r--r--   0 root         (0) root         (0)     3625 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/api/new/bazel_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/api/new/cmake_exe.py
+-rw-r--r--   0 root         (0) root         (0)     8212 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/api/new/cmake_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/api/new/meson_exe.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/api/new/meson_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/api/new/msbuild_exe.py
+-rw-r--r--   0 root         (0) root         (0)    12247 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/api/new/msbuild_lib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.886232 conan-2.0.8/conan/internal/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10041 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/cache/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/cache/conan_reference_layout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.887232 conan-2.0.8/conan/internal/cache/db/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/cache/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3305 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/cache/db/cache_database.py
+-rw-r--r--   0 root         (0) root         (0)     7953 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/cache/db/packages_table.py
+-rw-r--r--   0 root         (0) root         (0)     4791 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/cache/db/recipes_table.py
+-rw-r--r--   0 root         (0) root         (0)     2414 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/cache/db/table.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/conan_app.py
+-rw-r--r--   0 root         (0) root         (0)     3522 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/deploy.py
+-rw-r--r--   0 root         (0) root         (0)     2471 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/integrity_check.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-07-13 11:36:17.000000 conan-2.0.8/conan/internal/upload_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.887232 conan-2.0.8/conan/tools/
+-rw-r--r--   0 root         (0) root         (0)      494 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.887232 conan-2.0.8/conan/tools/android/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/android/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/android/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.888232 conan-2.0.8/conan/tools/apple/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/apple/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11538 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/apple/apple.py
+-rw-r--r--   0 root         (0) root         (0)     2167 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/apple/xcodebuild.py
+-rw-r--r--   0 root         (0) root         (0)    16434 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/apple/xcodedeps.py
+-rw-r--r--   0 root         (0) root         (0)     5763 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/apple/xcodetoolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.889232 conan-2.0.8/conan/tools/build/
+-rw-r--r--   0 root         (0) root         (0)     4142 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/build/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11103 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/build/cppstd.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/build/cpu.py
+-rw-r--r--   0 root         (0) root         (0)     2043 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/build/cross_building.py
+-rw-r--r--   0 root         (0) root         (0)    15391 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/build/flags.py
+-rw-r--r--   0 root         (0) root         (0)      563 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/build/stdcpp_library.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.889232 conan-2.0.8/conan/tools/cmake/
+-rw-r--r--   0 root         (0) root         (0)      217 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/cmake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11276 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/cmake/cmake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.890232 conan-2.0.8/conan/tools/cmake/cmakedeps/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/cmake/cmakedeps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8168 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/cmake/cmakedeps/cmakedeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.890232 conan-2.0.8/conan/tools/cmake/cmakedeps/templates/
+-rw-r--r--   0 root         (0) root         (0)     3944 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/cmake/cmakedeps/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4451 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/cmake/cmakedeps/templates/config.py
+-rw-r--r--   0 root         (0) root         (0)     3929 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/cmake/cmakedeps/templates/config_version.py
+-rw-r--r--   0 root         (0) root         (0)     5956 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/cmake/cmakedeps/templates/macros.py
+-rw-r--r--   0 root         (0) root         (0)    14925 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/cmake/cmakedeps/templates/target_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    19857 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/cmake/cmakedeps/templates/target_data.py
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/cmake/cmakedeps/templates/targets.py
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/cmake/layout.py
+-rw-r--r--   0 root         (0) root         (0)    14402 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/cmake/presets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.891233 conan-2.0.8/conan/tools/cmake/toolchain/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/cmake/toolchain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36083 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/cmake/toolchain/blocks.py
+-rw-r--r--   0 root         (0) root         (0)    11204 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/cmake/toolchain/toolchain.py
+-rw-r--r--   0 root         (0) root         (0)      171 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/cmake/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.891233 conan-2.0.8/conan/tools/env/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25388 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/env/environment.py
+-rw-r--r--   0 root         (0) root         (0)     3233 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/env/virtualbuildenv.py
+-rw-r--r--   0 root         (0) root         (0)     3394 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/env/virtualrunenv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.892233 conan-2.0.8/conan/tools/files/
+-rw-r--r--   0 root         (0) root         (0)      535 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/files/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/files/conandata.py
+-rw-r--r--   0 root         (0) root         (0)     6009 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/files/copy_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    23768 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/files/files.py
+-rw-r--r--   0 root         (0) root         (0)     4177 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/files/packager.py
+-rw-r--r--   0 root         (0) root         (0)     6014 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/files/patches.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.892233 conan-2.0.8/conan/tools/files/symlinks/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/files/symlinks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/files/symlinks/symlinks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.893233 conan-2.0.8/conan/tools/gnu/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/gnu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6234 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/gnu/autotools.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/gnu/autotoolsdeps.py
+-rw-r--r--   0 root         (0) root         (0)    13227 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/gnu/autotoolstoolchain.py
+-rw-r--r--   0 root         (0) root         (0)     3556 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/gnu/get_gnu_triplet.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/gnu/gnudeps_flags.py
+-rw-r--r--   0 root         (0) root         (0)     4191 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/gnu/pkgconfig.py
+-rw-r--r--   0 root         (0) root         (0)    18031 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/gnu/pkgconfigdeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.894233 conan-2.0.8/conan/tools/google/
+-rw-r--r--   0 root         (0) root         (0)      201 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/google/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/google/bazel.py
+-rw-r--r--   0 root         (0) root         (0)    10955 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/google/bazeldeps.py
+-rw-r--r--   0 root         (0) root         (0)      585 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/google/layout.py
+-rw-r--r--   0 root         (0) root         (0)      857 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/google/toolchain.py
+-rw-r--r--   0 root         (0) root         (0)      611 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.894233 conan-2.0.8/conan/tools/intel/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/intel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6498 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/intel/intel_cc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.895233 conan-2.0.8/conan/tools/layout/
+-rw-r--r--   0 root         (0) root         (0)      605 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/layout/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.895233 conan-2.0.8/conan/tools/meson/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/meson/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4073 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/meson/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     4954 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/meson/meson.py
+-rw-r--r--   0 root         (0) root         (0)    22060 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/meson/toolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.896233 conan-2.0.8/conan/tools/microsoft/
+-rw-r--r--   0 root         (0) root         (0)      558 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/microsoft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/microsoft/layout.py
+-rw-r--r--   0 root         (0) root         (0)     3312 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/microsoft/msbuild.py
+-rw-r--r--   0 root         (0) root         (0)    19214 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/microsoft/msbuilddeps.py
+-rw-r--r--   0 root         (0) root         (0)     2965 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/microsoft/nmakedeps.py
+-rw-r--r--   0 root         (0) root         (0)     4989 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/microsoft/nmaketoolchain.py
+-rw-r--r--   0 root         (0) root         (0)      593 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/microsoft/subsystems.py
+-rw-r--r--   0 root         (0) root         (0)    10843 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/microsoft/toolchain.py
+-rw-r--r--   0 root         (0) root         (0)    13069 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/microsoft/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.897233 conan-2.0.8/conan/tools/premake/
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/premake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/premake/premake.py
+-rw-r--r--   0 root         (0) root         (0)    10534 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/premake/premakedeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.897233 conan-2.0.8/conan/tools/qbs/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/qbs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/qbs/qbs.py
+-rw-r--r--   0 root         (0) root         (0)     9873 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/qbs/qbsprofile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.897233 conan-2.0.8/conan/tools/scm/
+-rw-r--r--   0 root         (0) root         (0)       77 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/scm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8718 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/scm/git.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.897233 conan-2.0.8/conan/tools/system/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/system/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16285 2023-07-13 11:36:17.000000 conan-2.0.8/conan/tools/system/package_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.874231 conan-2.0.8/conan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8328 2023-07-13 11:36:25.000000 conan-2.0.8/conan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9059 2023-07-13 11:36:25.000000 conan-2.0.8/conan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 11:36:25.000000 conan-2.0.8/conan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-13 11:36:25.000000 conan-2.0.8/conan.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      469 2023-07-13 11:36:25.000000 conan-2.0.8/conan.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 11:36:25.000000 conan-2.0.8/conan.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.899233 conan-2.0.8/conans/
+-rw-r--r--   0 root         (0) root         (0)      201 2023-07-13 11:36:17.000000 conan-2.0.8/conans/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.900233 conan-2.0.8/conans/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.901233 conan-2.0.8/conans/client/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10493 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/cache/cache.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/cache/editable.py
+-rw-r--r--   0 root         (0) root         (0)     6569 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/cache/remote_registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.901233 conan-2.0.8/conans/client/cmd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/cmd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7736 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/cmd/export.py
+-rw-r--r--   0 root         (0) root         (0)    12768 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/cmd/uploader.py
+-rw-r--r--   0 root         (0) root         (0)      968 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/cmd/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.902233 conan-2.0.8/conans/client/conanfile/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/conanfile/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/conanfile/build.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/conanfile/configure.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/conanfile/package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.902233 conan-2.0.8/conans/client/conf/
+-rw-r--r--   0 root         (0) root         (0)     6364 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/conf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9195 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/conf/config_installer.py
+-rw-r--r--   0 root         (0) root         (0)    14019 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/conf/detect.py
+-rw-r--r--   0 root         (0) root         (0)     5473 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/conf/detect_vs.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/conf/required_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.903233 conan-2.0.8/conans/client/downloaders/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/downloaders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9589 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/downloaders/caching_file_downloader.py
+-rw-r--r--   0 root         (0) root         (0)     4257 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/downloaders/download_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6723 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/downloaders/file_downloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.903233 conan-2.0.8/conans/client/generators/
+-rw-r--r--   0 root         (0) root         (0)     9706 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/generators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.905233 conan-2.0.8/conans/client/graph/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4837 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/graph/build_mode.py
+-rw-r--r--   0 root         (0) root         (0)     4571 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/graph/compatibility.py
+-rw-r--r--   0 root         (0) root         (0)     3922 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/graph/compute_pid.py
+-rw-r--r--   0 root         (0) root         (0)    14948 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)    16759 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/graph/graph_binaries.py
+-rw-r--r--   0 root         (0) root         (0)    17797 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/graph/graph_builder.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/graph/graph_error.py
+-rw-r--r--   0 root         (0) root         (0)    12990 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/graph/install_graph.py
+-rw-r--r--   0 root         (0) root         (0)     4163 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/graph/profile_node_definer.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/graph/provides.py
+-rw-r--r--   0 root         (0) root         (0)     6600 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/graph/proxy.py
+-rw-r--r--   0 root         (0) root         (0)     5806 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/graph/python_requires.py
+-rw-r--r--   0 root         (0) root         (0)     4692 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/graph/range_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/hook_manager.py
+-rw-r--r--   0 root         (0) root         (0)    21384 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/installer.py
+-rw-r--r--   0 root         (0) root         (0)    15815 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/loader.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/loader_txt.py
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/migrations.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/pkg_sign.py
+-rw-r--r--   0 root         (0) root         (0)    16848 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/profile_loader.py
+-rw-r--r--   0 root         (0) root         (0)    13267 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/remote_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.906233 conan-2.0.8/conans/client/rest/
+-rw-r--r--   0 root         (0) root         (0)      838 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5987 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/rest/auth_manager.py
+-rw-r--r--   0 root         (0) root         (0)     6132 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/rest/client_routes.py
+-rw-r--r--   0 root         (0) root         (0)     6894 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/rest/conan_requester.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/rest/file_uploader.py
+-rw-r--r--   0 root         (0) root         (0)     5488 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/rest/rest_client.py
+-rw-r--r--   0 root         (0) root         (0)    10011 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/rest/rest_client_common.py
+-rw-r--r--   0 root         (0) root         (0)    14916 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/rest/rest_client_v2.py
+-rw-r--r--   0 root         (0) root         (0)     3658 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.906233 conan-2.0.8/conans/client/store/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/store/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4305 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/store/localdb.py
+-rw-r--r--   0 root         (0) root         (0)     8798 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/subsystems.py
+-rw-r--r--   0 root         (0) root         (0)     5457 2023-07-13 11:36:17.000000 conan-2.0.8/conans/client/userio.py
+-rwxr-xr-x   0 root         (0) root         (0)      118 2023-07-13 11:36:17.000000 conan-2.0.8/conans/conan.py
+-rw-r--r--   0 root         (0) root         (0)      699 2023-07-13 11:36:17.000000 conan-2.0.8/conans/conan_server.py
+-rw-r--r--   0 root         (0) root         (0)     7817 2023-07-13 11:36:17.000000 conan-2.0.8/conans/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-07-13 11:36:17.000000 conan-2.0.8/conans/migrations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.909234 conan-2.0.8/conans/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 11:36:17.000000 conan-2.0.8/conans/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20216 2023-07-13 11:36:17.000000 conan-2.0.8/conans/model/build_info.py
+-rw-r--r--   0 root         (0) root         (0)    12428 2023-07-13 11:36:17.000000 conan-2.0.8/conans/model/conan_file.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2023-07-13 11:36:17.000000 conan-2.0.8/conans/model/conanfile_interface.py
+-rw-r--r--   0 root         (0) root         (0)    29837 2023-07-13 11:36:17.000000 conan-2.0.8/conans/model/conf.py
+-rw-r--r--   0 root         (0) root         (0)     5901 2023-07-13 11:36:17.000000 conan-2.0.8/conans/model/dependencies.py
+-rw-r--r--   0 root         (0) root         (0)    10886 2023-07-13 11:36:17.000000 conan-2.0.8/conans/model/graph_lock.py
+-rw-r--r--   0 root         (0) root         (0)    13067 2023-07-13 11:36:17.000000 conan-2.0.8/conans/model/info.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2023-07-13 11:36:17.000000 conan-2.0.8/conans/model/layout.py
+-rw-r--r--   0 root         (0) root         (0)     4883 2023-07-13 11:36:17.000000 conan-2.0.8/conans/model/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    17047 2023-07-13 11:36:17.000000 conan-2.0.8/conans/model/options.py
+-rw-r--r--   0 root         (0) root         (0)     3861 2023-07-13 11:36:17.000000 conan-2.0.8/conans/model/package_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2023-07-13 11:36:17.000000 conan-2.0.8/conans/model/pkg_type.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-07-13 11:36:17.000000 conan-2.0.8/conans/model/profile.py
+-rw-r--r--   0 root         (0) root         (0)     7612 2023-07-13 11:36:17.000000 conan-2.0.8/conans/model/recipe_ref.py
+-rw-r--r--   0 root         (0) root         (0)    23782 2023-07-13 11:36:17.000000 conan-2.0.8/conans/model/requires.py
+-rw-r--r--   0 root         (0) root         (0)     2171 2023-07-13 11:36:17.000000 conan-2.0.8/conans/model/rest_routes.py
+-rw-r--r--   0 root         (0) root         (0)    13368 2023-07-13 11:36:17.000000 conan-2.0.8/conans/model/settings.py
+-rw-r--r--   0 root         (0) root         (0)     5991 2023-07-13 11:36:17.000000 conan-2.0.8/conans/model/version.py
+-rw-r--r--   0 root         (0) root         (0)     4350 2023-07-13 11:36:17.000000 conan-2.0.8/conans/model/version_range.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.909234 conan-2.0.8/conans/paths/
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-07-13 11:36:17.000000 conan-2.0.8/conans/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2023-07-13 11:36:17.000000 conan-2.0.8/conans/pylint_plugin.py
+-rw-r--r--   0 root         (0) root         (0)      251 2023-07-13 11:36:17.000000 conan-2.0.8/conans/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      146 2023-07-13 11:36:17.000000 conan-2.0.8/conans/requirements_dev.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-13 11:36:17.000000 conan-2.0.8/conans/requirements_server.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.909234 conan-2.0.8/conans/search/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 11:36:17.000000 conan-2.0.8/conans/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3814 2023-07-13 11:36:17.000000 conan-2.0.8/conans/search/query_parse.py
+-rw-r--r--   0 root         (0) root         (0)     4474 2023-07-13 11:36:17.000000 conan-2.0.8/conans/search/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.910234 conan-2.0.8/conans/test/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-07-13 11:36:17.000000 conan-2.0.8/conans/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13174 2023-07-13 11:36:17.000000 conan-2.0.8/conans/test/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.911234 conan-2.0.8/conans/test/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 11:36:17.000000 conan-2.0.8/conans/test/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4868 2023-07-13 11:36:17.000000 conan-2.0.8/conans/test/utils/artifactory.py
+-rw-r--r--   0 root         (0) root         (0)     5129 2023-07-13 11:36:17.000000 conan-2.0.8/conans/test/utils/mocks.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-07-13 11:36:17.000000 conan-2.0.8/conans/test/utils/profiles.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-07-13 11:36:17.000000 conan-2.0.8/conans/test/utils/scm.py
+-rw-r--r--   0 root         (0) root         (0)     3858 2023-07-13 11:36:17.000000 conan-2.0.8/conans/test/utils/server_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-07-13 11:36:17.000000 conan-2.0.8/conans/test/utils/test_files.py
+-rw-r--r--   0 root         (0) root         (0)    35637 2023-07-13 11:36:17.000000 conan-2.0.8/conans/test/utils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 11:36:25.912234 conan-2.0.8/conans/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 11:36:17.000000 conan-2.0.8/conans/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-07-13 11:36:17.000000 conan-2.0.8/conans/util/config_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-07-13 11:36:17.000000 conan-2.0.8/conans/util/dates.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-07-13 11:36:17.000000 conan-2.0.8/conans/util/encrypt.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-07-13 11:36:17.000000 conan-2.0.8/conans/util/env.py
+-rw-r--r--   0 root         (0) root         (0)    12086 2023-07-13 11:36:17.000000 conan-2.0.8/conans/util/files.py
+-rw-r--r--   0 root         (0) root         (0)     3657 2023-07-13 11:36:17.000000 conan-2.0.8/conans/util/locks.py
+-rw-r--r--   0 root         (0) root         (0)     3688 2023-07-13 11:36:17.000000 conan-2.0.8/conans/util/runners.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-07-13 11:36:17.000000 conan-2.0.8/conans/util/sha.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-07-13 11:36:17.000000 conan-2.0.8/conans/util/thread.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-07-13 11:36:17.000000 conan-2.0.8/conans/util/windows.py
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-13 11:36:25.913234 conan-2.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     5058 2023-07-13 11:36:17.000000 conan-2.0.8/setup.py
```

### Comparing `conan-2.0.7/LICENSE.md` & `conan-2.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/PKG-INFO` & `conan-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan
-Version: 2.0.7
+Version: 2.0.8
 Summary: Conan C/C++ package manager
 Home-page: https://conan.io
 Author: JFrog LTD
 Author-email: luism@jfrog.com
 License: MIT
 Project-URL: Documentation, https://docs.conan.io
 Project-URL: Source, https://github.com/conan-io/conan
```

### Comparing `conan-2.0.7/README.md` & `conan-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/api/conan_api.py` & `conan-2.0.8/conan/api/conan_api.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/api/model.py` & `conan-2.0.8/conan/api/model.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/api/output.py` & `conan-2.0.8/conan/api/output.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/api/subapi/cache.py` & `conan-2.0.8/conan/api/subapi/cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         ref.revision = None if ref.revision == "latest" else ref.revision
         ref_layout = app.cache.recipe_layout(ref)
         return ref_layout.export()
 
     def recipe_metadata_path(self, ref: RecipeReference):
         app = ConanApp(self.conan_api.cache_folder)
         ref = _resolve_latest_ref(app, ref)
-        ref_layout = app.cache.ref_layout(ref)
+        ref_layout = app.cache.recipe_layout(ref)
         return ref_layout.metadata()
 
     def export_source_path(self, ref: RecipeReference):
         app = ConanApp(self.conan_api.cache_folder)
         ref.revision = None if ref.revision == "latest" else ref.revision
         ref_layout = app.cache.recipe_layout(ref)
         return ref_layout.export_sources()
@@ -83,15 +83,15 @@
                     folder = os.path.join(builds_folder, subdir)
                     manifest = os.path.join(folder, "p", "conanmanifest.txt")
                     info = os.path.join(folder, "p", "conaninfo.txt")
                     if not os.path.exists(manifest) or not os.path.exists(info):
                         rmdir(folder)
 
         for ref, ref_bundle in package_list.refs():
-            ref_layout = app.cache.ref_layout(ref)
+            ref_layout = app.cache.recipe_layout(ref)
             if source:
                 rmdir(ref_layout.source())
             if download:
                 rmdir(ref_layout.download_export())
             for pref, _ in package_list.prefs(ref, ref_bundle):
                 pref_layout = app.cache.pkg_layout(pref)
                 if build:
```

### Comparing `conan-2.0.7/conan/api/subapi/config.py` & `conan-2.0.8/conan/api/subapi/config.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/api/subapi/export.py` & `conan-2.0.8/conan/api/subapi/export.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/api/subapi/graph.py` & `conan-2.0.8/conan/api/subapi/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/api/subapi/install.py` & `conan-2.0.8/conan/api/subapi/install.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/api/subapi/list.py` & `conan-2.0.8/conan/api/subapi/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/api/subapi/local.py` & `conan-2.0.8/conan/api/subapi/local.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/api/subapi/lockfile.py` & `conan-2.0.8/conan/api/subapi/lockfile.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/api/subapi/new.py` & `conan-2.0.8/conan/api/subapi/new.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/api/subapi/profiles.py` & `conan-2.0.8/conan/api/subapi/profiles.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/api/subapi/remotes.py` & `conan-2.0.8/conan/api/subapi/remotes.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/api/subapi/remove.py` & `conan-2.0.8/conan/api/subapi/remove.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         assert ref.revision, "Recipe revision cannot be None to remove a recipe"
         """Removes the recipe (or recipe revision if present) and all the packages (with all prev)"""
         app = ConanApp(self.conan_api.cache_folder)
         if remote:
             app.remote_manager.remove_recipe(ref, remote)
         else:
             self.all_recipe_packages(ref)
-            recipe_layout = app.cache.ref_layout(ref)
+            recipe_layout = app.cache.recipe_layout(ref)
             app.cache.remove_recipe_layout(recipe_layout)
 
     def all_recipe_packages(self, ref: RecipeReference, remote: Remote = None):
         assert ref.revision, "Recipe revision cannot be None to remove a recipe"
         """Removes all the packages from the provided reference"""
         app = ConanApp(self.conan_api.cache_folder)
         if remote:
```

### Comparing `conan-2.0.7/conan/api/subapi/search.py` & `conan-2.0.8/conan/api/subapi/search.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/api/subapi/upload.py` & `conan-2.0.8/conan/api/subapi/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         self.conan_api = conan_api
 
     def check_upstream(self, package_list, remote, force=False):
         """Check if the artifacts are already in the specified remote, skipping them from
         the package_list in that case"""
         app = ConanApp(self.conan_api.cache_folder)
         for ref, bundle in package_list.refs():
-            layout = app.cache.ref_layout(ref)
+            layout = app.cache.recipe_layout(ref)
             conanfile_path = layout.conanfile()
             conanfile = app.loader.load_basic(conanfile_path)
             if conanfile.upload_policy == "skip":
                 ConanOutput().info(f"{ref}: Skipping upload of binaries, "
                                    "because upload_policy='skip'")
                 bundle["packages"] = {}
```

### Comparing `conan-2.0.7/conan/cli/args.py` & `conan-2.0.8/conan/cli/args.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/cli.py` & `conan-2.0.8/conan/cli/cli.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/command.py` & `conan-2.0.8/conan/cli/command.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/commands/build.py` & `conan-2.0.8/conan/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/commands/cache.py` & `conan-2.0.8/conan/cli/commands/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 @conan_subcommand(formatters={"text": cli_out_write})
 def cache_path(conan_api: ConanAPI, parser, subparser, *args):
     """
     Show the path to the Conan cache for a given reference.
     """
     subparser.add_argument("reference", help="Recipe reference or Package reference")
     subparser.add_argument("--folder", choices=['export_source', 'source', 'build', 'metadata'],
-                           help="Path to show. The 'build'"
-                                " requires a package reference. If not specified it shows 'exports'"
-                                " path ")
+                           help="Path to show. The 'build' requires a package reference. "
+                                "If the argument is not passed, it shows 'exports' path for recipe references "
+                                "and 'package' folder for package references.")
 
     args = parser.parse_args(*args)
     try:
         pref = PkgReference.loads(args.reference)
     except ConanException:
         pref = None
```

### Comparing `conan-2.0.7/conan/cli/commands/config.py` & `conan-2.0.8/conan/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/commands/create.py` & `conan-2.0.8/conan/cli/commands/create.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/commands/download.py` & `conan-2.0.8/conan/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/commands/editable.py` & `conan-2.0.8/conan/cli/commands/editable.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/commands/export.py` & `conan-2.0.8/conan/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/commands/export_pkg.py` & `conan-2.0.8/conan/cli/commands/export_pkg.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/commands/graph.py` & `conan-2.0.8/conan/cli/commands/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/commands/inspect.py` & `conan-2.0.8/conan/cli/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/commands/install.py` & `conan-2.0.8/conan/cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/commands/list.py` & `conan-2.0.8/conan/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/commands/lock.py` & `conan-2.0.8/conan/cli/commands/lock.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/commands/new.py` & `conan-2.0.8/conan/cli/commands/new.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/commands/profile.py` & `conan-2.0.8/conan/cli/commands/profile.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/commands/remote.py` & `conan-2.0.8/conan/cli/commands/remote.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/commands/remove.py` & `conan-2.0.8/conan/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/commands/search.py` & `conan-2.0.8/conan/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/commands/source.py` & `conan-2.0.8/conan/cli/commands/source.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/commands/test.py` & `conan-2.0.8/conan/cli/commands/test.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/commands/upload.py` & `conan-2.0.8/conan/cli/commands/upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from conan.api.conan_api import ConanAPI
 from conan.api.model import ListPattern, MultiPackagesList
-from conan.api.output import cli_out_write
+from conan.api.output import cli_out_write, ConanOutput
 from conan.cli import make_abs_path
 from conan.cli.command import conan_command, OnceArgument
 from conan.cli.commands.list import print_list_json, print_serial
 from conans.client.userio import UserInput
 from conan.errors import ConanException
 
 
@@ -77,32 +77,36 @@
         listfile = make_abs_path(args.list)
         multi_package_list = MultiPackagesList.load(listfile)
         package_list = multi_package_list["Local Cache"]
     else:
         ref_pattern = ListPattern(args.pattern, package_id="*", only_recipe=args.only_recipe)
         package_list = conan_api.list.select(ref_pattern, package_query=args.package_query)
 
-    if not package_list.recipes:
+    if package_list.recipes:
+        if args.check:
+            conan_api.cache.check_integrity(package_list)
+        # Check if the recipes/packages are in the remote
+        conan_api.upload.check_upstream(package_list, remote, args.force)
+
+        # If only if search with "*" we ask for confirmation
+        if not args.list and not args.confirm and "*" in args.pattern:
+            _ask_confirm_upload(conan_api, package_list)
+
+        conan_api.upload.prepare(package_list, enabled_remotes, args.metadata)
+
+        if not args.dry_run:
+            conan_api.upload.upload(package_list, remote)
+            conan_api.upload.upload_backup_sources(package_list)
+    elif args.list:
+        # Don't error on no recipes for automated workflows using list,
+        # but warn to tell the user that no packages were uploaded
+        ConanOutput().warning(f"No packages were uploaded because the package list is empty.")
+    else:
         raise ConanException("No recipes found matching pattern '{}'".format(args.pattern))
 
-    if args.check:
-        conan_api.cache.check_integrity(package_list)
-    # Check if the recipes/packages are in the remote
-    conan_api.upload.check_upstream(package_list, remote, args.force)
-
-    # If only if search with "*" we ask for confirmation
-    if not args.list and not args.confirm and "*" in args.pattern:
-        _ask_confirm_upload(conan_api, package_list)
-
-    conan_api.upload.prepare(package_list, enabled_remotes, args.metadata)
-
-    if not args.dry_run:
-        conan_api.upload.upload(package_list, remote)
-        conan_api.upload.upload_backup_sources(package_list)
-
     pkglist = MultiPackagesList()
     pkglist.add(remote.name, package_list)
     return {
         "results": pkglist.serialize(),
         "conan_api": conan_api
     }
```

### Comparing `conan-2.0.7/conan/cli/commands/version.py` & `conan-2.0.8/conan/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/formatters/graph/graph.py` & `conan-2.0.8/conan/cli/formatters/graph/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,28 +101,22 @@
     serial = graph.serialize()
     # TODO: This is not used, it is necessary to update the renderings to use the serialized graph
     #  instead of the native graph
     serial = filter_graph(serial, package_filter)
     template_folder = os.path.join(conan_api.cache_folder, "templates")
     user_template = os.path.join(template_folder, "graph.html")
     template = load(user_template) if os.path.isfile(user_template) else graph_info_html
+    error = {
+        "type": "unknown",
+        "context": graph.error,
+        "should_highlight_node": lambda node: False
+    }
     if isinstance(graph.error, GraphConflictError):
-        error = {
-            "label": graph.error.require.ref,
-            "type": "conflict",
-            "from": graph.error.node.id or graph.error.base_previous.id,
-            "prev_node": graph.error.prev_node,
-            "should_highlight_node": lambda node: node.id == graph.error.node.id
-        }
-    else:
-        error = {
-            "type": "unknown",
-            "error:": graph.error,
-            "should_highlight_node": lambda node: False
-        }
+        error["type"] = "conflict"
+        error["should_highlight_node"] = lambda node: node.id == graph.error.node.id
     cli_out_write(_render_graph(graph, error, template, template_folder))
     if graph.error:
         raise graph.error
 
 
 def format_graph_dot(result):
     graph = result["graph"]
```

### Comparing `conan-2.0.7/conan/cli/formatters/graph/graph_info_text.py` & `conan-2.0.8/conan/cli/formatters/graph/graph_info_text.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/formatters/graph/info_graph_html.py` & `conan-2.0.8/conan/cli/formatters/graph/info_graph_html.py`

 * *Files 21% similar despite different names*

```diff
@@ -75,40 +75,61 @@
             var edges = [
                 {%- for src, dst in graph.edges %}
                     { from: {{ src.id }}, to: {{ dst.id }} }{%- if not loop.last %},{% endif %}
                 {%- endfor %}
             ]
 
             {% if error is not none and error["type"] == "conflict" %}
-                // Add some helpful visualizations for conflicts
+                // Add error conflict node
                 nodes.push({
                     id: "{{ error["type"] }}",
-                    label: "{{ error["label"] }}",
+                    label: "{{ error["context"].require.ref }}",
                     shape: "circle",
                     font: { color: "white" },
                     color: "red",
-                    fulllabel: '<h3>{{ error["label"] }}</h3><p>This node creates a conflict in the dependency graph with {{ error["prev_node"]["ref"] }}</p>',
+                    fulllabel: '<h3>{{ error["context"].require.ref }}</h3><p>This node creates a conflict in the dependency graph</p>',
                     shapeProperties: { borderDashes: [5, 5] }
                 })
 
-                {% if error["from"] is not none %}
-                    edges.push({from: {{ error["from"] }}, to: "{{ error["type"] }}", color: "red", dashes: true, title: "Conflict"})
+                {% if error["context"].node.id is not none %}
+                    // Add edge from node that introduces the conflict to the new error node
+                    edges.push({from: {{ error["context"].node.id }},
+                                to: "{{ error["type"] }}",
+                                color: "red",
+                                dashes: true,
+                                title: "Conflict",
+                                physics: false,
+                                color: "red",
+                                arrows: "to;from"})
                 {% endif %}
-                edges.push({from: {{ error["from"] }},
-                            to: "{{ error["type"] }}",
-                            dashes: true,
-                            title: "Conflict",
-                            physics: false,
-                            color: "red",
-                            arrows: "to;from"})
-
-                edges.push({from: {{ error["prev_node"].id }},
-                            to: "{{ error["type"] }}",
-                            color: "red",
-                            title: "Problematic require"})
+
+                {% if error["context"].prev_node is none and error["context"].base_previous.id is not none %}
+                    // Add edge from base node to the new error node
+                    edges.push({from: {{ error["context"].base_previous.id }},
+                                to: "{{ error["type"] }}",
+                                color: "red",
+                                dashes: true,
+                                title: "Conflict",
+                                physics: false,
+                                color: "red",
+                                arrows: "to;from"})
+                {% endif %}
+
+                {% if error["context"].prev_node is not none and error["context"].prev_node.id is not none %}
+                    // Add edge from previous node that already had conflicting dependency
+                    edges.push({from: {{ error["context"].prev_node.id }},
+                                to: "{{ error["type"] }}",
+                                color: "red",
+                                dashes: true,
+                                title: "Conflict",
+                                physics: false,
+                                color: "red",
+                                arrows: "to;from"})
+                {% endif %}
+
             {% endif %}
 
             var nodes = new vis.DataSet(nodes);
             var edges = new vis.DataSet(edges);
 
             var container = document.getElementById('mynetwork');
             var controls = document.getElementById('controls');
```

### Comparing `conan-2.0.7/conan/cli/formatters/list/binary_html_table.py` & `conan-2.0.8/conan/cli/formatters/list/binary_html_table.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/formatters/list/list.py` & `conan-2.0.8/conan/cli/formatters/list/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/formatters/list/search_table_html.py` & `conan-2.0.8/conan/cli/formatters/list/search_table_html.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/cli/printers/graph.py` & `conan-2.0.8/conan/cli/printers/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/internal/api/new/autoools_exe.py` & `conan-2.0.8/conan/internal/api/new/autoools_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/internal/api/new/autotools_lib.py` & `conan-2.0.8/conan/internal/api/new/autotools_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from conan.tools.layout import basic_layout
 from conan.tools.apple import fix_apple_shared_install_name
 
 
 class {{package_name}}Conan(ConanFile):
     name = "{{name}}"
     version = "{{version}}"
+    package_type = "library"
 
     # Optional metadata
     license = "<Put the package license here>"
     author = "<Put your name here> <And your email here>"
     url = "<Package recipe repository url here, for issues about the package>"
     description = "<Description of {package_name} here>"
     topics = ("<Put some tag here>", "<here>", "<and here>")
```

### Comparing `conan-2.0.7/conan/internal/api/new/basic.py` & `conan-2.0.8/conan/internal/api/new/basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
 _conanfile = '''\
 from conan import ConanFile
 
 class BasicConanfile(ConanFile):
 ''' + _conanfile_header + '''\
 
+    # Check the documentation for the rest of the available attributes
+
+
     # The requirements method allows you to define the dependencies of your recipe
     def requirements(self):
         # Each call to self.requires() will add the corresponding requirement
         # to the current list of requirements
         {% if requires is defined -%}
         {% for require in requires -%}
         self.requires("{{ require }}")
```

### Comparing `conan-2.0.7/conan/internal/api/new/bazel_exe.py` & `conan-2.0.8/conan/internal/api/new/bazel_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/internal/api/new/bazel_lib.py` & `conan-2.0.8/conan/internal/api/new/bazel_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from conan import ConanFile
 from conan.tools.google import Bazel, bazel_layout
 from conan.tools.files import copy
 
 class {{package_name}}Recipe(ConanFile):
     name = "{{name}}"
     version = "{{version}}"
+    package_type = "library"
 
     # Binary configuration
     settings = "os", "compiler", "build_type", "arch"
     options = {"shared": [True, False], "fPIC": [True, False]}
     default_options = {"shared": False, "fPIC": True}
 
     # Sources are located in the same place as this recipe, copy them to the recipe
```

### Comparing `conan-2.0.7/conan/internal/api/new/cmake_exe.py` & `conan-2.0.8/conan/internal/api/new/cmake_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/internal/api/new/cmake_lib.py` & `conan-2.0.8/conan/internal/api/new/cmake_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 conanfile_sources_v2 = '''from conan import ConanFile
 from conan.tools.cmake import CMakeToolchain, CMake, cmake_layout, CMakeDeps
 
 
 class {{package_name}}Recipe(ConanFile):
     name = "{{name}}"
     version = "{{version}}"
+    package_type = "library"
 
     # Optional metadata
     license = "<Put the package license here>"
     author = "<Put your name here> <And your email here>"
     url = "<Package recipe repository url here, for issues about the package>"
     description = "<Description of {{ name }} package here>"
     topics = ("<Put some tag here>", "<here>", "<and here>")
@@ -282,15 +283,15 @@
 
 test_main = """#include "{{name}}.h"
 #include <vector>
 #include <string>
 
 int main() {
     {{package_name}}();
-    
+
     std::vector<std::string> vec;
     vec.push_back("test_package");
 
     {{package_name}}_print_vector(vec);
 }
 """
```

### Comparing `conan-2.0.7/conan/internal/api/new/meson_exe.py` & `conan-2.0.8/conan/internal/api/new/meson_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/internal/api/new/meson_lib.py` & `conan-2.0.8/conan/internal/api/new/meson_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from conan.tools.meson import MesonToolchain, Meson
 from conan.tools.layout import basic_layout
 from conan.tools.files import copy
 
 class {{package_name}}Conan(ConanFile):
     name = "{{name}}"
     version = "{{version}}"
+    package_type = "library"
 
     # Binary configuration
     settings = "os", "compiler", "build_type", "arch"
     options = {"shared": [True, False], "fPIC": [True, False]}
     default_options = {"shared": False, "fPIC": True}
 
     # Sources are located in the same place as this recipe, copy them to the recipe
```

### Comparing `conan-2.0.7/conan/internal/api/new/msbuild_exe.py` & `conan-2.0.8/conan/internal/api/new/msbuild_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/internal/api/new/msbuild_lib.py` & `conan-2.0.8/conan/internal/api/new/msbuild_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/internal/cache/cache.py` & `conan-2.0.8/conan/internal/cache/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,27 +13,29 @@
 from conans.util.dates import revision_timestamp_now
 from conans.util.files import rmdir, renamedir
 
 
 class DataCache:
 
     def __init__(self, base_folder, db_filename):
-        self._base_folder = os.path.realpath(base_folder)
+        self._base_folder = os.path.abspath(base_folder)
         self._db = CacheDatabase(filename=db_filename)
 
     def _create_path(self, relative_path, remove_contents=True):
         path = self._full_path(relative_path)
         if os.path.exists(path) and remove_contents:
             self._remove_path(relative_path)
         os.makedirs(path, exist_ok=True)
 
     def _remove_path(self, relative_path):
         rmdir(self._full_path(relative_path))
 
     def _full_path(self, relative_path):
+        # This one is used only for rmdir and mkdir operations, not returned to user
+        # or stored in DB
         path = os.path.realpath(os.path.join(self._base_folder, relative_path))
         return path
 
     @property
     def base_folder(self):
         return self._base_folder
 
@@ -74,75 +76,75 @@
     def create_export_recipe_layout(self, ref: RecipeReference):
         # This is a temporary layout while exporting a new recipe, because the revision is not
         # computed yet, until it is. The entry is not added to DB, just a temp folder is created
         assert ref.revision is None, "Recipe revision should be None"
         assert ref.timestamp is None
         reference_path = self._get_tmp_path(ref)
         self._create_path(reference_path)
-        return RecipeLayout(ref, os.path.join(self.base_folder, reference_path))
+        return RecipeLayout(ref, os.path.join(self._base_folder, reference_path))
 
     def create_build_pkg_layout(self, pref: PkgReference):
         # Temporary layout to build a new package, when we don't know the package revision yet
         assert pref.ref.revision, "Recipe revision must be known to get or create the package layout"
         assert pref.package_id, "Package id must be known to get or create the package layout"
         assert pref.revision is None, "Package revision should be None"
         assert pref.timestamp is None
         package_path = self._get_tmp_path_pref(pref)
         self._create_path(package_path)
-        return PackageLayout(pref, os.path.join(self.base_folder, package_path))
+        return PackageLayout(pref, os.path.join(self._base_folder, package_path))
 
     def get_recipe_layout(self, ref: RecipeReference):
         """ the revision must exists, the folder must exist
         """
         if ref.revision is None:  # Latest one
             ref_data = self._db.get_latest_recipe(ref)
         else:
             ref_data = self._db.get_recipe(ref)
         ref_path = ref_data.get("path")
         ref = ref_data.get("ref")  # new revision with timestamp
-        return RecipeLayout(ref, os.path.join(self.base_folder, ref_path))
+        return RecipeLayout(ref, os.path.join(self._base_folder, ref_path))
 
     def get_recipe_revisions_references(self, ref: RecipeReference):
         return self._db.get_recipe_revisions_references(ref)
 
     def get_package_layout(self, pref: PkgReference):
         """ the revision must exists, the folder must exist
         """
         assert pref.ref.revision, "Recipe revision must be known to get the package layout"
         assert pref.package_id, "Package id must be known to get the package layout"
         assert pref.revision, "Package revision must be known to get the package layout"
         pref_data = self._db.try_get_package(pref)
         pref_path = pref_data.get("path")
-        return PackageLayout(pref, os.path.join(self.base_folder, pref_path))
+        return PackageLayout(pref, os.path.join(self._base_folder, pref_path))
 
     def get_or_create_ref_layout(self, ref: RecipeReference):
         """ called by RemoteManager.get_recipe()
         """
         try:
             return self.get_recipe_layout(ref)
         except ConanReferenceDoesNotExistInDB:
             assert ref.revision, "Recipe revision must be known to create the package layout"
             reference_path = self._get_path(ref)
             self._db.create_recipe(reference_path, ref)
             self._create_path(reference_path, remove_contents=False)
-            return RecipeLayout(ref, os.path.join(self.base_folder, reference_path))
+            return RecipeLayout(ref, os.path.join(self._base_folder, reference_path))
 
     def get_or_create_pkg_layout(self, pref: PkgReference):
         """ called by RemoteManager.get_package() and  BinaryInstaller
         """
         try:
             return self.get_package_layout(pref)
         except ConanReferenceDoesNotExistInDB:
             assert pref.ref.revision, "Recipe revision must be known to create the package layout"
             assert pref.package_id, "Package id must be known to create the package layout"
             assert pref.revision, "Package revision should be known to create the package layout"
             package_path = self._get_path_pref(pref)
             self._db.create_package(package_path, pref, None)
             self._create_path(package_path, remove_contents=False)
-            return PackageLayout(pref, os.path.join(self.base_folder, package_path))
+            return PackageLayout(pref, os.path.join(self._base_folder, package_path))
 
     def update_recipe_timestamp(self, ref: RecipeReference):
         assert ref.revision
         assert ref.timestamp
         self._db.update_recipe_timestamp(ref)
 
     def list_references(self):
@@ -174,15 +176,15 @@
 
     def assign_prev(self, layout: PackageLayout):
         pref = layout.reference
 
         build_id = layout.build_id
         pref.timestamp = revision_timestamp_now()
         # Wait until it finish to really update the DB
-        relpath = os.path.relpath(layout.base_folder, self.base_folder)
+        relpath = os.path.relpath(layout.base_folder, self._base_folder)
         try:
             self._db.create_package(relpath, pref, build_id)
         except ConanReferenceAlreadyExistsInDB:
             # TODO: Optimize this into 1 single UPSERT operation
             # This was exported before, making it latest again, update timestamp
             pkg_layout = self.get_package_layout(pref)
             pkg_layout.remove()
@@ -207,15 +209,15 @@
             # If there source folder exists, export and export_sources
             # folders are already copied so we can remove the tmp ones
             rmdir(self._full_path(layout.base_folder))
         else:
             # Destination folder is empty, move all the tmp contents
             renamedir(self._full_path(layout.base_folder), new_path_absolute)
 
-        layout._base_folder = os.path.join(self.base_folder, new_path_relative)
+        layout._base_folder = os.path.join(self._base_folder, new_path_relative)
 
         # Wait until it finish to really update the DB
         try:
             self._db.create_recipe(new_path_relative, ref)
         except ConanReferenceAlreadyExistsInDB:
             # This was exported before, making it latest again, update timestamp
             ref = layout.reference
```

### Comparing `conan-2.0.7/conan/internal/cache/conan_reference_layout.py` & `conan-2.0.8/conan/internal/cache/conan_reference_layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/internal/cache/db/cache_database.py` & `conan-2.0.8/conan/internal/cache/db/cache_database.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,25 @@
+import os
+
 from conan.internal.cache.db.packages_table import PackagesDBTable
 from conan.internal.cache.db.recipes_table import RecipesDBTable
 from conans.model.package_ref import PkgReference
 from conans.model.recipe_ref import RecipeReference
 
 CONNECTION_TIMEOUT_SECONDS = 1  # Time a connection will wait when the database is locked
 
 
 class CacheDatabase:
 
     def __init__(self, filename):
         self._recipes = RecipesDBTable(filename)
         self._packages = PackagesDBTable(filename)
+        if not os.path.isfile(filename):
+            self._recipes.create_table()
+            self._packages.create_table()
 
     def exists_prev(self, ref):
         # TODO: This logic could be done directly against DB
         matching_prevs = self.get_package_revisions_references(ref)
         return len(matching_prevs) > 0
 
     def get_latest_package_reference(self, ref):
```

### Comparing `conan-2.0.7/conan/internal/cache/db/packages_table.py` & `conan-2.0.8/conan/internal/cache/db/packages_table.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/internal/cache/db/recipes_table.py` & `conan-2.0.8/conan/internal/cache/db/recipes_table.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/internal/cache/db/table.py` & `conan-2.0.8/conan/internal/cache/db/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,21 +12,20 @@
     unique_together: tuple = None
 
     def __init__(self, filename):
         self.filename = filename
         column_names: List[str] = [it[0] for it in self.columns_description]
         self.row_type = namedtuple('_', column_names)
         self.columns = self.row_type(*column_names)
-        self.create_table()
 
     @contextmanager
     def db_connection(self):
+        connection = sqlite3.connect(self.filename, isolation_level=None,
+                                     timeout=1, check_same_thread=False)
         try:
-            connection = sqlite3.connect(self.filename, isolation_level=None,
-                                        timeout=1, check_same_thread=False)
             yield connection
         finally:
             connection.close()
 
     def create_table(self):
         def field(name, typename, nullable=False, check_constraints: Optional[List] = None,
                   unique=False):
```

### Comparing `conan-2.0.7/conan/internal/conan_app.py` & `conan-2.0.8/conan/internal/conan_app.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/internal/deploy.py` & `conan-2.0.8/conan/internal/deploy.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/internal/integrity_check.py` & `conan-2.0.8/conan/internal/integrity_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             corrupted = self._recipe_corrupted(ref) or corrupted
             for pref, prev_bundle in upload_data.prefs(ref, recipe_bundle):
                 corrupted = self._package_corrupted(pref) or corrupted
         if corrupted:
             raise ConanException("There are corrupted artifacts, check the error logs")
 
     def _recipe_corrupted(self, ref: RecipeReference):
-        layout = self._app.cache.ref_layout(ref)
+        layout = self._app.cache.recipe_layout(ref)
         output = ConanOutput()
         read_manifest, expected_manifest = layout.recipe_manifests()
 
         if read_manifest != expected_manifest:
             output.error(f"{ref}: Manifest mismatch")
             output.error(f"Folder: {layout.export()}")
             diff = read_manifest.difference(expected_manifest)
```

### Comparing `conan-2.0.7/conan/internal/upload_metadata.py` & `conan-2.0.8/conan/internal/upload_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             result[path] = abs_path
     return result
 
 
 def gather_metadata(package_list, cache, metadata):
     for rref, recipe_bundle in package_list.refs():
         if metadata or recipe_bundle["upload"]:
-            metadata_folder = cache.ref_layout(rref).metadata()
+            metadata_folder = cache.recipe_layout(rref).metadata()
             files = _metadata_files(metadata_folder, metadata)
             if files:
                 ConanOutput(scope=str(rref)).info(f"Recipe metadata: {len(files)} files")
                 recipe_bundle.setdefault("files", {}).update(files)
                 recipe_bundle["upload"] = True
 
         for pref, pkg_bundle in package_list.prefs(rref, recipe_bundle):
```

### Comparing `conan-2.0.7/conan/tools/android/utils.py` & `conan-2.0.8/conan/tools/android/utils.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/apple/__init__.py` & `conan-2.0.8/conan/tools/apple/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/apple/apple.py` & `conan-2.0.8/conan/tools/apple/apple.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,17 +171,27 @@
         return self.find('strip')
 
     @property
     def libtool(self):
         """path to libtool"""
         return self.find('libtool')
 
+    @property
+    def otool(self):
+        """path to otool"""
+        return self.find('otool')
+
+    @property
+    def install_name_tool(self):
+        """path to install_name_tool"""
+        return self.find('install_name_tool')
 
-def _get_dylib_install_name(path_to_dylib):
-    command = "otool -D {}".format(path_to_dylib)
+
+def _get_dylib_install_name(otool, path_to_dylib):
+    command = f"{otool} -D {path_to_dylib}"
     output =  iter(check_output_runner(command).splitlines())
     # Note: if otool return multiple entries for different architectures
     # assume they are the same and pick the first one.
     for line in output:
         if ":" in line:
             return next(output)
     raise ConanException(f"Unable to extract install_name for {path_to_dylib}")
@@ -190,44 +200,51 @@
 def fix_apple_shared_install_name(conanfile):
     """
     Search for all the *dylib* files in the conanfile's *package_folder* and fix
     both the ``LC_ID_DYLIB`` and ``LC_LOAD_DYLIB`` fields on those files using the
     *install_name_tool* utility available in macOS to set ``@rpath``.
     """
 
+    if not is_apple_os(conanfile):
+        return
+
+    xcrun = XCRun(conanfile)
+    otool = xcrun.otool
+    install_name_tool = xcrun.install_name_tool
+
     def _darwin_is_binary(file, binary_type):
         if binary_type not in ("DYLIB", "EXECUTE") or os.path.islink(file) or os.path.isdir(file):
             return False
-        check_file = f"otool -hv {file}"
+        check_file = f"{otool} -hv {file}"
         return binary_type in check_output_runner(check_file)
 
     def _darwin_collect_binaries(folder, binary_type):
         return [os.path.join(folder, f) for f in os.listdir(folder) if _darwin_is_binary(os.path.join(folder, f), binary_type)]
 
     def _fix_install_name(dylib_path, new_name):
-        command = f"install_name_tool {dylib_path} -id {new_name}"
+        command = f"{install_name_tool} {dylib_path} -id {new_name}"
         conanfile.run(command)
 
     def _fix_dep_name(dylib_path, old_name, new_name):
-        command = f"install_name_tool {dylib_path} -change {old_name} {new_name}"
+        command = f"{install_name_tool} {dylib_path} -change {old_name} {new_name}"
         conanfile.run(command)
 
     def _get_rpath_entries(binary_file):
         entries = []
-        command = "otool -l {}".format(binary_file)
+        command = f"{otool} -l {binary_file}"
         otool_output = check_output_runner(command).splitlines()
         for count, text in enumerate(otool_output):
             pass
             if "LC_RPATH" in text:
                 rpath_entry = otool_output[count+2].split("path ")[1].split(" ")[0]
                 entries.append(rpath_entry)
         return entries
 
     def _get_shared_dependencies(binary_file):
-        command = "otool -L {}".format(binary_file)
+        command = f"{otool} -L {binary_file}"
         all_shared = check_output_runner(command).strip().split(":")[1].strip()
         ret = [s.split("(")[0].strip() for s in all_shared.splitlines()]
         return ret
 
     def _fix_dylib_files(conanfile):
         substitutions = {}
         libdirs = getattr(conanfile.cpp.package, "libdirs")
@@ -235,15 +252,15 @@
             full_folder = os.path.join(conanfile.package_folder, libdir)
             if not os.path.exists(full_folder):
                 raise ConanException(f"Trying to locate shared libraries, but `{libdir}` "
                                      f" not found inside package folder {conanfile.package_folder}")
             shared_libs = _darwin_collect_binaries(full_folder, "DYLIB")
             # fix LC_ID_DYLIB in first pass
             for shared_lib in shared_libs:
-                install_name = _get_dylib_install_name(shared_lib)
+                install_name = _get_dylib_install_name(otool, shared_lib)
                 #TODO: we probably only want to fix the install the name if
                 # it starts with `/`.
                 rpath_name = f"@rpath/{os.path.basename(install_name)}"
                 _fix_install_name(shared_lib, rpath_name)
                 substitutions[install_name] = rpath_name
 
             # fix dependencies in second pass
@@ -278,17 +295,16 @@
                 # existing duplicates
                 libdirs = getattr(conanfile.cpp.package, "libdirs")
                 libdirs = [os.path.join(conanfile.package_folder, dir) for dir in libdirs]
                 rel_paths = [f"@executable_path/{os.path.relpath(dir, full_folder)}" for dir in libdirs]
                 existing_rpaths = _get_rpath_entries(executable)
                 rpaths_to_add = list(set(rel_paths) - set(existing_rpaths))
                 for entry in rpaths_to_add:
-                    command = f"install_name_tool {executable} -add_rpath {entry}"
+                    command = f"{install_name_tool} {executable} -add_rpath {entry}"
                     conanfile.run(command)
 
-    if is_apple_os(conanfile):
-        substitutions = _fix_dylib_files(conanfile)
+    substitutions = _fix_dylib_files(conanfile)
 
-        # Only "fix" executables if dylib files were patched, otherwise
-        # there is nothing to do.
-        if substitutions:
-            _fix_executables(conanfile, substitutions)
+    # Only "fix" executables if dylib files were patched, otherwise
+    # there is nothing to do.
+    if substitutions:
+        _fix_executables(conanfile, substitutions)
```

### Comparing `conan-2.0.7/conan/tools/apple/xcodebuild.py` & `conan-2.0.8/conan/tools/apple/xcodebuild.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/apple/xcodedeps.py` & `conan-2.0.8/conan/tools/apple/xcodedeps.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,34 +20,34 @@
 
 
 def _format_name(name):
     name = name.replace(".", "_").replace("-", "_")
     return name.lower()
 
 
-def _xcconfig_settings_filename(settings):
+def _xcconfig_settings_filename(settings, configuration):
     arch = settings.get_safe("arch")
     architecture = _to_apple_arch(arch) or arch
-    props = [("configuration", settings.get_safe("build_type")),
+    props = [("configuration", configuration),
              ("architecture", architecture),
              ("sdk name", settings.get_safe("os.sdk")),
              ("sdk version", settings.get_safe("os.sdk_version"))]
     name = "".join("_{}".format(v) for _, v in props if v is not None and v)
     return _format_name(name)
 
 
-def _xcconfig_conditional(settings):
+def _xcconfig_conditional(settings, configuration):
     sdk_condition = "*"
     arch = settings.get_safe("arch")
     architecture = _to_apple_arch(arch) or arch
     sdk = settings.get_safe("os.sdk") if settings.get_safe("os") != "Macos" else "macosx"
     if sdk:
         sdk_condition = "{}{}".format(sdk, settings.get_safe("os.sdk_version") or "*")
 
-    return "[config={}][arch={}][sdk={}]".format(settings.get_safe("build_type"), architecture, sdk_condition)
+    return "[config={}][arch={}][sdk={}]".format(configuration, architecture, sdk_condition)
 
 
 def _add_includes_to_file_or_create(filename, template, files_to_include):
     if os.path.isfile(filename):
         content = load(filename)
     else:
         content = template
@@ -61,15 +61,15 @@
 
 class XcodeDeps(object):
     general_name = "conandeps.xcconfig"
 
     _conf_xconfig = textwrap.dedent("""\
         PACKAGE_ROOT_{{pkg_name}}{{condition}} = {{root}}
         // Compiler options for {{pkg_name}}::{{comp_name}}
-        HEADER_SEARCH_PATHS_{{pkg_name}}_{{comp_name}}{{condition}} = {{include_dirs}}
+        SYSTEM_HEADER_SEARCH_PATHS_{{pkg_name}}_{{comp_name}}{{condition}} = {{include_dirs}}
         GCC_PREPROCESSOR_DEFINITIONS_{{pkg_name}}_{{comp_name}}{{condition}} = {{definitions}}
         OTHER_CFLAGS_{{pkg_name}}_{{comp_name}}{{condition}} = {{c_compiler_flags}}
         OTHER_CPLUSPLUSFLAGS_{{pkg_name}}_{{comp_name}}{{condition}} = {{cxx_compiler_flags}}
         FRAMEWORK_SEARCH_PATHS_{{pkg_name}}_{{comp_name}}{{condition}} = {{frameworkdirs}}
 
         // Link options for {{pkg_name}}::{{comp_name}}
         LIBRARY_SEARCH_PATHS_{{pkg_name}}_{{comp_name}}{{condition}} = {{lib_dirs}}
@@ -80,15 +80,15 @@
         // Conan XcodeDeps generated file for {{pkg_name}}::{{comp_name}}
         // Includes all configurations for each dependency
         {% for include in deps_includes %}
         #include "{{include}}"
         {% endfor %}
         #include "{{dep_xconfig_filename}}"
 
-        HEADER_SEARCH_PATHS = $(inherited) $(HEADER_SEARCH_PATHS_{{pkg_name}}_{{comp_name}})
+        SYSTEM_HEADER_SEARCH_PATHS = $(inherited) $(SYSTEM_HEADER_SEARCH_PATHS_{{pkg_name}}_{{comp_name}})
         GCC_PREPROCESSOR_DEFINITIONS = $(inherited) $(GCC_PREPROCESSOR_DEFINITIONS_{{pkg_name}}_{{comp_name}})
         OTHER_CFLAGS = $(inherited) $(OTHER_CFLAGS_{{pkg_name}}_{{comp_name}})
         OTHER_CPLUSPLUSFLAGS = $(inherited) $(OTHER_CPLUSPLUSFLAGS_{{pkg_name}}_{{comp_name}})
         FRAMEWORK_SEARCH_PATHS = $(inherited) $(FRAMEWORK_SEARCH_PATHS_{{pkg_name}}_{{comp_name}})
 
         // Link options for {{pkg_name}}_{{comp_name}}
         LIBRARY_SEARCH_PATHS = $(inherited) $(LIBRARY_SEARCH_PATHS_{{pkg_name}}_{{comp_name}})
@@ -145,15 +145,15 @@
             'frameworkdirs': " ".join('"{}"'.format(p) for p in _merged_vars("frameworkdirs")),
             'frameworks': " ".join("-framework {}".format(framework) for framework in _merged_vars("frameworks")),
             'definitions': " ".join('"{}"'.format(p.replace('"', '\\"')) for p in _merged_vars("defines")),
             'c_compiler_flags': " ".join('"{}"'.format(p.replace('"', '\\"')) for p in _merged_vars("cflags")),
             'cxx_compiler_flags': " ".join('"{}"'.format(p.replace('"', '\\"')) for p in _merged_vars("cxxflags")),
             'linker_flags': " ".join('"{}"'.format(p.replace('"', '\\"')) for p in _merged_vars("sharedlinkflags")),
             'exe_flags': " ".join('"{}"'.format(p.replace('"', '\\"')) for p in _merged_vars("exelinkflags")),
-            'condition': _xcconfig_conditional(self._conanfile.settings)
+            'condition': _xcconfig_conditional(self._conanfile.settings, self.configuration)
         }
 
         if not require.headers:
             fields["include_dirs"] = ""
 
         if not require.libs:
             fields["lib_dirs"] = ""
@@ -227,15 +227,15 @@
         return _add_includes_to_file_or_create(GLOBAL_XCCONFIG_FILENAME,
                                                GLOBAL_XCCONFIG_TEMPLATE,
                                                [self.general_name])
 
     def get_content_for_component(self, require, pkg_name, component_name, package_folder, transitive_internal, transitive_external):
         result = {}
 
-        conf_name = _xcconfig_settings_filename(self._conanfile.settings)
+        conf_name = _xcconfig_settings_filename(self._conanfile.settings, self.configuration)
 
         props_name = "conan_{}_{}{}.xcconfig".format(pkg_name, component_name, conf_name)
         result[props_name] = self._conf_xconfig_file(require, pkg_name, component_name, package_folder, transitive_internal)
 
         # The entry point for each package
         file_dep_name = "conan_{}_{}.xcconfig".format(pkg_name, component_name)
         dep_content = self._dep_xconfig_file(pkg_name, component_name, file_dep_name, props_name, transitive_external)
```

### Comparing `conan-2.0.7/conan/tools/apple/xcodetoolchain.py` & `conan-2.0.8/conan/tools/apple/xcodetoolchain.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,29 +60,29 @@
         cppstd = cppstd_flag(self._conanfile.settings)
         if cppstd.startswith("-std="):
             return cppstd[5:]
         return cppstd
 
     @property
     def _macosx_deployment_target(self):
-        return 'MACOSX_DEPLOYMENT_TARGET{}={}'.format(_xcconfig_conditional(self._conanfile.settings),
+        return 'MACOSX_DEPLOYMENT_TARGET{}={}'.format(_xcconfig_conditional(self._conanfile.settings, self.configuration),
                                                       self.os_version) if self.os_version else ""
 
     @property
     def _clang_cxx_library(self):
-        return 'CLANG_CXX_LIBRARY{}={}'.format(_xcconfig_conditional(self._conanfile.settings),
+        return 'CLANG_CXX_LIBRARY{}={}'.format(_xcconfig_conditional(self._conanfile.settings, self.configuration),
                                                self.libcxx) if self.libcxx else ""
 
     @property
     def _clang_cxx_language_standard(self):
-        return 'CLANG_CXX_LANGUAGE_STANDARD{}={}'.format(_xcconfig_conditional(self._conanfile.settings),
+        return 'CLANG_CXX_LANGUAGE_STANDARD{}={}'.format(_xcconfig_conditional(self._conanfile.settings, self.configuration),
                                                          self._cppstd) if self._cppstd else ""
     @property
     def _vars_xconfig_filename(self):
-        return "conantoolchain{}{}".format(_xcconfig_settings_filename(self._conanfile.settings),
+        return "conantoolchain{}{}".format(_xcconfig_settings_filename(self._conanfile.settings, self.configuration),
                                                                        self.extension)
 
     @property
     def _vars_xconfig_content(self):
         ret = self._vars_xconfig.format(macosx_deployment_target=self._macosx_deployment_target,
                                         clang_cxx_library=self._clang_cxx_library,
                                         clang_cxx_language_standard=self._clang_cxx_language_standard)
```

### Comparing `conan-2.0.7/conan/tools/build/__init__.py` & `conan-2.0.8/conan/tools/build/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/build/cppstd.py` & `conan-2.0.8/conan/tools/build/cppstd.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/build/cpu.py` & `conan-2.0.8/conan/tools/build/cpu.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/build/cross_building.py` & `conan-2.0.8/conan/tools/build/cross_building.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/build/flags.py` & `conan-2.0.8/conan/tools/build/flags.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/build/stdcpp_library.py` & `conan-2.0.8/conan/tools/build/stdcpp_library.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/cmake/cmake.py` & `conan-2.0.8/conan/tools/cmake/cmake.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,14 +184,19 @@
 
         pkg_folder = '"{}"'.format(self._conanfile.package_folder.replace("\\", "/"))
         build_folder = '"{}"'.format(self._conanfile.build_folder)
         arg_list = ["--install", build_folder, build_config, "--prefix", pkg_folder]
         if component:
             arg_list.extend(["--component", component])
         arg_list.extend(self._compilation_verbosity_arg)
+
+        do_strip = self._conanfile.conf.get("tools.cmake:install_strip", check_type=bool)
+        if do_strip:
+            arg_list.append("--strip")
+
         arg_list = " ".join(filter(None, arg_list))
         command = "%s %s" % (self._cmake_program, arg_list)
         self._conanfile.run(command)
 
     def test(self, build_type=None, target=None, cli_args=None, build_tool_args=None, env=""):
         """
         Equivalent to running cmake --build . --target=RUN_TESTS.
```

### Comparing `conan-2.0.7/conan/tools/cmake/cmakedeps/cmakedeps.py` & `conan-2.0.8/conan/tools/cmake/cmakedeps/cmakedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/cmake/cmakedeps/templates/__init__.py` & `conan-2.0.8/conan/tools/cmake/cmakedeps/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/cmake/cmakedeps/templates/config.py` & `conan-2.0.8/conan/tools/cmake/cmakedeps/templates/config.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/cmake/cmakedeps/templates/macros.py` & `conan-2.0.8/conan/tools/cmake/cmakedeps/templates/macros.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,17 +54,20 @@
 
                    # Create a micro-target for each lib/a found
                    # Allow only some characters for the target name
                    string(REGEX REPLACE "[^A-Za-z0-9.+_-]" "_" _LIBRARY_NAME ${_LIBRARY_NAME})
                    set(_LIB_NAME CONAN_LIB::${package_name}_${_LIBRARY_NAME}${config_suffix})
 
                    if(is_host_windows AND library_type STREQUAL "SHARED")
+                     # Store and reset the variable, so it doesn't leak
+                     set(_OLD_CMAKE_FIND_LIBRARY_SUFFIXES ${CMAKE_FIND_LIBRARY_SUFFIXES})
                      set(CMAKE_FIND_LIBRARY_SUFFIXES .dll ${CMAKE_FIND_LIBRARY_SUFFIXES})
                      find_library(CONAN_SHARED_FOUND_LIBRARY NAMES ${_LIBRARY_NAME} PATHS ${package_bindir}
                                   NO_DEFAULT_PATH NO_CMAKE_FIND_ROOT_PATH)
+                     set(CMAKE_FIND_LIBRARY_SUFFIXES ${_OLD_CMAKE_FIND_LIBRARY_SUFFIXES})
                      if(NOT CONAN_SHARED_FOUND_LIBRARY)
                        message(STATUS "Cannot locate shared library: ${_LIBRARY_NAME}")
                        message(DEBUG "DLL library not found, creating UNKNOWN IMPORTED target")
                        if(NOT TARGET ${_LIB_NAME})
                           add_library(${_LIB_NAME} UNKNOWN IMPORTED)
                        endif()
                        set_target_properties(${_LIB_NAME} PROPERTIES IMPORTED_LOCATION${config_suffix} ${CONAN_FOUND_LIBRARY})
```

### Comparing `conan-2.0.7/conan/tools/cmake/cmakedeps/templates/target_configuration.py` & `conan-2.0.8/conan/tools/cmake/cmakedeps/templates/target_configuration.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/cmake/cmakedeps/templates/target_data.py` & `conan-2.0.8/conan/tools/cmake/cmakedeps/templates/target_data.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/cmake/cmakedeps/templates/targets.py` & `conan-2.0.8/conan/tools/cmake/cmakedeps/templates/targets.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/cmake/layout.py` & `conan-2.0.8/conan/tools/cmake/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/cmake/presets.py` & `conan-2.0.8/conan/tools/cmake/presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,19 +24,19 @@
     @staticmethod
     def generate(conanfile, toolchain_file, generator, cache_variables, preset_prefix):
         cache_variables = cache_variables or {}
         if platform.system() == "Windows" and generator == "MinGW Makefiles":
             if "CMAKE_SH" not in cache_variables:
                 cache_variables["CMAKE_SH"] = "CMAKE_SH-NOTFOUND"
 
-            cmake_make_program = conanfile.conf.get("tools.gnu:make_program",
-                                                    default=cache_variables.get("CMAKE_MAKE_PROGRAM"))
-            if cmake_make_program:
-                cmake_make_program = cmake_make_program.replace("\\", "/")
-                cache_variables["CMAKE_MAKE_PROGRAM"] = cmake_make_program
+        cmake_make_program = conanfile.conf.get("tools.gnu:make_program",
+                                                default=cache_variables.get("CMAKE_MAKE_PROGRAM"))
+        if cmake_make_program:
+            cmake_make_program = cmake_make_program.replace("\\", "/")
+            cache_variables["CMAKE_MAKE_PROGRAM"] = cmake_make_program
 
         if "CMAKE_POLICY_DEFAULT_CMP0091" not in cache_variables:
             cache_variables["CMAKE_POLICY_DEFAULT_CMP0091"] = "NEW"
 
         if "BUILD_TESTING" not in cache_variables:
             if conanfile.conf.get("tools.build:skip_test", check_type=bool):
                 cache_variables["BUILD_TESTING"] = "OFF"
```

### Comparing `conan-2.0.7/conan/tools/cmake/toolchain/blocks.py` & `conan-2.0.8/conan/tools/cmake/toolchain/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -729,27 +729,29 @@
                     (arch_build == "ppc64") and (arch_host == "ppc32")):
                 return cmake_system_name_map.get(os_host, os_host)
 
     def _is_apple_cross_building(self):
         os_host = self._conanfile.settings.get_safe("os")
         arch_host = self._conanfile.settings.get_safe("arch")
         arch_build = self._conanfile.settings_build.get_safe("arch")
+        os_build = self._conanfile.settings_build.get_safe("os")
         return os_host in ('iOS', 'watchOS', 'tvOS') or (
-                os_host == 'Macos' and arch_host != arch_build)
+                os_host == 'Macos' and (arch_host != arch_build or os_build != os_host))
 
     def _get_cross_build(self):
         user_toolchain = self._conanfile.conf.get("tools.cmake.cmaketoolchain:user_toolchain")
         if user_toolchain is not None:
             return None, None, None  # Will be provided by user_toolchain
 
         system_name = self._conanfile.conf.get("tools.cmake.cmaketoolchain:system_name")
         system_version = self._conanfile.conf.get("tools.cmake.cmaketoolchain:system_version")
         system_processor = self._conanfile.conf.get("tools.cmake.cmaketoolchain:system_processor")
 
         assert hasattr(self._conanfile, "settings_build")
+        # TODO: Remove unused if
         if hasattr(self._conanfile, "settings_build"):
             os_host = self._conanfile.settings.get_safe("os")
             arch_host = self._conanfile.settings.get_safe("arch")
             if system_name is None:  # Try to deduce
                 _system_version = None
                 _system_processor = None
                 if self._is_apple_cross_building():
```

### Comparing `conan-2.0.7/conan/tools/cmake/toolchain/toolchain.py` & `conan-2.0.8/conan/tools/cmake/toolchain/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/env/environment.py` & `conan-2.0.8/conan/tools/env/environment.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/env/virtualbuildenv.py` & `conan-2.0.8/conan/tools/env/virtualbuildenv.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/env/virtualrunenv.py` & `conan-2.0.8/conan/tools/env/virtualrunenv.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/files/__init__.py` & `conan-2.0.8/conan/tools/files/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,8 +2,8 @@
     rename, chdir, unzip, replace_in_file, collect_libs, check_md5, check_sha1, check_sha256, \
     move_folder_contents
 
 from conan.tools.files.patches import patch, apply_conandata_patches, export_conandata_patches
 from conan.tools.files.packager import AutoPackager
 from conan.tools.files.symlinks import symlinks
 from conan.tools.files.copy_pattern import copy
-from conan.tools.files.conandata import update_conandata
+from conan.tools.files.conandata import update_conandata, trim_conandata
```

### Comparing `conan-2.0.7/conan/tools/files/conandata.py` & `conan-2.0.8/conan/tools/files/conandata.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,7 +35,35 @@
             else:
                 d[k] = v
         return d
 
     recursive_dict_update(conandata, data)
     new_content = yaml.safe_dump(conandata)
     save(path, new_content)
+
+
+def trim_conandata(conanfile):
+    """
+    Tool to modify the ``conandata.yml`` once it is exported, to limit it to the current version
+    only
+    """
+    if not hasattr(conanfile, "export_folder") or conanfile.export_folder is None:
+        raise ConanException("The 'trim_conandata()' can only be used in the 'export()' method")
+    path = os.path.join(conanfile.export_folder, "conandata.yml")
+    if not os.path.exists(path):
+        raise ConanException("conandata.yml file doesn't exist")
+
+    conandata = load(path)
+    conandata = yaml.safe_load(conandata)
+
+    version = str(conanfile.version)
+    result = {}
+    for k, v in conandata.items():
+        if not isinstance(v, dict):
+            result[k] = v
+            continue  # to allow user extra conandata, common to all versions
+        version_data = v.get(version)
+        if version_data is not None:
+            result[k] = {version: version_data}
+
+    new_conandata_yml = yaml.safe_dump(result, default_flow_style=False)
+    save(path, new_conandata_yml)
```

### Comparing `conan-2.0.7/conan/tools/files/copy_pattern.py` & `conan-2.0.8/conan/tools/files/copy_pattern.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/files/files.py` & `conan-2.0.8/conan/tools/files/files.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/files/packager.py` & `conan-2.0.8/conan/tools/files/packager.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/files/patches.py` & `conan-2.0.8/conan/tools/files/patches.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     :param patch_string: Patch string that should be applied.
     :param strip: Number of folders to be stripped from the path.
     :param output: Stream object.
     :param fuzz: Should accept fuzzy patches.
     :param kwargs: Extra parameters that can be added and will contribute to output information
     """
 
-    patch_type = kwargs.get('patch_type')
+    patch_type = kwargs.get('patch_type') or ("file" if patch_file else "string")
     patch_description = kwargs.get('patch_description')
 
     if patch_type or patch_description:
         patch_type_str = ' ({})'.format(patch_type) if patch_type else ''
         patch_description_str = ': {}'.format(patch_description) if patch_description else ''
         conanfile.output.info('Apply patch{}{}'.format(patch_type_str, patch_description_str))
 
@@ -92,16 +92,19 @@
         entries = patches
     else:
         raise ConanException("conandata.yml 'patches' should be a list or a dict {version: list}")
     for it in entries:
         if "patch_file" in it:
             # The patch files are located in the root src
             entry = it.copy()
-            patch_file = os.path.join(conanfile.export_sources_folder, entry.pop("patch_file"))
-            patch(conanfile, patch_file=patch_file, **entry)
+            patch_file = entry.pop("patch_file")
+            patch_file_path = os.path.join(conanfile.export_sources_folder, patch_file)
+            if not "patch_description" in entry:
+                entry["patch_description"] = patch_file
+            patch(conanfile, patch_file=patch_file_path, **entry)
         elif "patch_string" in it:
             patch(conanfile, **it)
         else:
             raise ConanException("The 'conandata.yml' file needs a 'patch_file' or 'patch_string'"
                                  " entry for every patch to be applied")
```

### Comparing `conan-2.0.7/conan/tools/files/symlinks/symlinks.py` & `conan-2.0.8/conan/tools/files/symlinks/symlinks.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/gnu/autotools.py` & `conan-2.0.8/conan/tools/gnu/autotools.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/gnu/autotoolsdeps.py` & `conan-2.0.8/conan/tools/gnu/autotoolsdeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/gnu/autotoolstoolchain.py` & `conan-2.0.8/conan/tools/gnu/autotoolstoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/gnu/get_gnu_triplet.py` & `conan-2.0.8/conan/tools/gnu/get_gnu_triplet.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/gnu/gnudeps_flags.py` & `conan-2.0.8/conan/tools/gnu/gnudeps_flags.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/gnu/pkgconfig.py` & `conan-2.0.8/conan/tools/gnu/pkgconfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from io import StringIO
+
 from conan.tools.build import cmd_args_to_string
 from conan.tools.env import Environment
 from conan.errors import ConanException
-from conans.util.runners import check_output_runner
 
 
 class PkgConfig:
 
     def __init__(self, conanfile, library, pkg_config_path=None):
         """
 
@@ -19,19 +20,24 @@
         self._info = {}
         self._pkg_config_path = pkg_config_path
         self._variables = None
 
     def _parse_output(self, option):
         executable = self._conanfile.conf.get("tools.gnu:pkg_config", default="pkg-config")
         command = cmd_args_to_string([executable, '--' + option, self._library, '--print-errors'])
+
         env = Environment()
         if self._pkg_config_path:
             env.prepend_path("PKG_CONFIG_PATH", self._pkg_config_path)
         with env.vars(self._conanfile).apply():
-            return check_output_runner(command).strip()
+            # This way we get the environment from ConanFile, from profile (default buildenv)
+            output = StringIO()
+            self._conanfile.run(command, stdout=output)
+        value = output.getvalue().strip()
+        return value
 
     def _get_option(self, option):
         if option not in self._info:
             self._info[option] = self._parse_output(option)
         return self._info[option]
 
     @property
```

### Comparing `conan-2.0.7/conan/tools/gnu/pkgconfigdeps.py` & `conan-2.0.8/conan/tools/gnu/pkgconfigdeps.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
+import re
 import textwrap
 from collections import namedtuple
 
 from jinja2 import Template, StrictUndefined
 
+from conan.errors import ConanException
 from conan.internal import check_duplicated_generator
 from conan.tools.gnu.gnudeps_flags import GnuDepsFlags
-from conan.errors import ConanException
 from conans.model.dependencies import get_transitive_requires
 from conans.util.files import save
 
 
 def _get_name_with_namespace(namespace, name):
     """
     Build a name with a namespace, e.g., openssl-crypto
@@ -71,99 +72,49 @@
     :return: `str` with the suffix
     """
     if not build_context_suffix or not req.is_build_context:
         return ""
     return build_context_suffix.get(req.ref.name, "")
 
 
-def _get_formatted_dirs(folders, prefix_path_):
-    ret = []
+def _get_formatted_dirs(folder_name, folders, prefix_path_):
+    ret = {}
     for i, directory in enumerate(folders):
         directory = os.path.normpath(directory).replace("\\", "/")
         prefix = ""
         if not os.path.isabs(directory):
             prefix = "${prefix}/"
         elif directory.startswith(prefix_path_):
             prefix = "${prefix}/"
             directory = os.path.relpath(directory, prefix_path_).replace("\\", "/")
-        ret.append("%s%s" % (prefix, directory))
+        suffix = str(i) if i else ""
+        var_name = f"{folder_name}{suffix}"
+        ret[var_name] = f"{prefix}{directory}"
     return ret
 
 
 _PCInfo = namedtuple("PCInfo", ['name', 'requires', 'description', 'cpp_info', 'aliases'])
 
 
 class _PCContentGenerator:
 
     template = textwrap.dedent("""\
-        {%- macro get_libs(libdirs, cpp_info, gnudeps_flags) -%}
-        {%- for _ in libdirs -%}
-        {{ '-L"${libdir%s}"' % (loop.index0 or "") + " " }}
-        {%- endfor -%}
-        {%- for sys_lib in (cpp_info.libs + cpp_info.system_libs) -%}
-        {{ "-l%s" % sys_lib + " " }}
-        {%- endfor -%}
-        {%- for shared_flag in (cpp_info.sharedlinkflags + cpp_info.exelinkflags) -%}
-        {{  shared_flag + " " }}
-        {%- endfor -%}
-        {%- for framework in (gnudeps_flags.frameworks + gnudeps_flags.framework_paths) -%}
-        {{ framework + " " }}
-        {%- endfor -%}
-        {%- endmacro -%}
-
-        {%- macro get_cflags(includedirs, cxxflags, cflags, defines) -%}
-        {%- for _ in includedirs -%}
-        {{ '-I"${includedir%s}"' % (loop.index0 or "") + " " }}
-        {%- endfor -%}
-        {%- for cxxflag in cxxflags -%}
-        {{ cxxflag + " " }}
-        {%- endfor -%}
-        {%- for cflag in cflags-%}
-        {{ cflag + " " }}
-        {%- endfor -%}
-        {%- for define in defines-%}
-        {{  "-D%s" % define + " " }}
-        {%- endfor -%}
-        {%- endmacro -%}
-
-        prefix={{ prefix_path }}
-        {% for path in libdirs %}
-        {{ "libdir{}={}".format((loop.index0 or ""), path) }}
-        {% endfor %}
-        {% for path in includedirs %}
-        {{ "includedir%s=%s" % ((loop.index0 or ""), path) }}
-        {% endfor %}
-        {% for path in bindirs %}
-        {{ "bindir{}={}".format((loop.index0 or ""), path) }}
+        {% for k, v in pc_variables.items() %}
+        {{ "{}={}".format(k, v) }}
         {% endfor %}
-        {% if pkg_config_custom_content %}
-        # Custom PC content
-        {{ pkg_config_custom_content }}
-        {% endif %}
 
         Name: {{ name }}
         Description: {{ description }}
         Version: {{ version }}
-        Libs: {{ get_libs(libdirs, cpp_info, gnudeps_flags) }}
-        Cflags: {{ get_cflags(includedirs, cxxflags, cflags, defines) }}
-        {% if requires|length %}
-        Requires: {{ requires|join(' ') }}
+        {% if libflags %}
+        Libs: {{ libflags }}
         {% endif %}
-    """)
-
-    shortened_template = textwrap.dedent("""\
-        prefix={{ prefix_path }}
-        {% if pkg_config_custom_content %}
-        # Custom PC content
-        {{ pkg_config_custom_content }}
+        {% if cflags %}
+        Cflags: {{ cflags }}
         {% endif %}
-
-        Name: {{ name }}
-        Description: {{ description }}
-        Version: {{ version }}
         {% if requires|length %}
         Requires: {{ requires|join(' ') }}
         {% endif %}
     """)
 
     def __init__(self, conanfile, dep):
         self._conanfile = conanfile
@@ -171,58 +122,82 @@
 
     def _get_prefix_path(self):
         # If editable, package_folder can be None
         root_folder = self._dep.recipe_folder if self._dep.package_folder is None \
             else self._dep.package_folder
         return root_folder.replace("\\", "/")
 
-    def content(self, info):
-        assert isinstance(info, _PCInfo) and info.cpp_info is not None
-
+    def _get_pc_variables(self, cpp_info):
+        """
+        Get all the freeform variables defined by Conan and
+        users (through ``pkg_config_custom_content``). This last ones will override the
+        Conan defined variables.
+        """
         prefix_path = self._get_prefix_path()
-        version = info.cpp_info.get_property("component_version") or self._dep.ref.version
-        libdirs = _get_formatted_dirs(info.cpp_info.libdirs, prefix_path)
-        includedirs = _get_formatted_dirs(info.cpp_info.includedirs, prefix_path)
-        bindirs = _get_formatted_dirs(info.cpp_info.bindirs, prefix_path)
-        custom_content = info.cpp_info.get_property("pkg_config_custom_content")
+        pc_variables = {"prefix": prefix_path}
+        if cpp_info is None:
+            return pc_variables
+        # Already formatted directories
+        pc_variables.update(_get_formatted_dirs("libdir", cpp_info.libdirs, prefix_path))
+        pc_variables.update(_get_formatted_dirs("includedir", cpp_info.includedirs, prefix_path))
+        pc_variables.update(_get_formatted_dirs("bindir", cpp_info.bindirs, prefix_path))
+        # Get the custom content introduced by user and sanitize it
+        custom_content = cpp_info.get_property("pkg_config_custom_content")
+        if isinstance(custom_content, dict):
+            pc_variables.update(custom_content)
+        elif custom_content:  # Legacy: custom content is string
+            pc_variable_pattern = re.compile("^(.*)=(.*)")
+            for line in custom_content.splitlines():
+                match = pc_variable_pattern.match(line)
+                if match:
+                    key, value = match.group(1).strip(), match.group(2).strip()
+                    pc_variables[key] = value
+        return pc_variables
+
+    def _get_lib_flags(self, libdirvars, cpp_info):
+        gnudeps_flags = GnuDepsFlags(self._conanfile, cpp_info)
+        libdirsflags = ['-L"${%s}"' % d for d in libdirvars]
+        system_libs = ["-l%s" % l for l in (cpp_info.libs + cpp_info.system_libs)]
+        shared_flags = cpp_info.sharedlinkflags + cpp_info.exelinkflags
+        framework_flags = gnudeps_flags.frameworks + gnudeps_flags.framework_paths
+        return " ".join(libdirsflags + system_libs + shared_flags + framework_flags)
+
+    def _get_cflags(self, includedirvars, cpp_info):
+        includedirsflags = ['-I"${%s}"' % d for d in includedirvars]
+        cxxflags = [var.replace('"', '\\"') for var in cpp_info.cxxflags]
+        cflags = [var.replace('"', '\\"') for var in cpp_info.cflags]
+        defines = ["-D%s" % var.replace('"', '\\"') for var in cpp_info.defines]
+        return " ".join(includedirsflags + cxxflags + cflags + defines)
 
+    def _get_context(self, info):
+        pc_variables = self._get_pc_variables(info.cpp_info)
         context = {
-            "prefix_path": prefix_path,
-            "libdirs": libdirs,
-            "includedirs": includedirs,
-            "bindirs": bindirs,
-            "pkg_config_custom_content": custom_content,
             "name": info.name,
             "description": info.description,
-            "version": version,
+            "version": self._dep.ref.version,
             "requires": info.requires,
-            "cpp_info": info.cpp_info,
-            "cxxflags": [var.replace('"', '\\"') for var in info.cpp_info.cxxflags],
-            "cflags": [var.replace('"', '\\"') for var in info.cpp_info.cflags],
-            "defines": [var.replace('"', '\\"') for var in info.cpp_info.defines],
-            "gnudeps_flags": GnuDepsFlags(self._conanfile, info.cpp_info)
+            "pc_variables": pc_variables,
+            "cflags": "",
+            "libflags": ""
         }
-        template = Template(self.template, trim_blocks=True, lstrip_blocks=True,
-                            undefined=StrictUndefined)
-        return template.render(context)
+        if info.cpp_info is not None:
+            context.update({
+                "version": info.cpp_info.get_property("component_version") or self._dep.ref.version,
+                "cflags": self._get_cflags([d for d in pc_variables if d.startswith("includedir")],
+                                           info.cpp_info),
+                "libflags": self._get_lib_flags([d for d in pc_variables if d.startswith("libdir")],
+                                                info.cpp_info)
+            })
+        return context
 
-    def shortened_content(self, info):
+    def content(self, info):
         assert isinstance(info, _PCInfo)
-        custom_content = info.cpp_info.get_property("pkg_config_custom_content") if info.cpp_info \
-            else None
-        context = {
-            "prefix_path": self._get_prefix_path(),
-            "pkg_config_custom_content": custom_content,
-            "name": info.name,
-            "description": info.description,
-            "version": self._dep.ref.version,
-            "requires": info.requires
-        }
-        template = Template(self.shortened_template, trim_blocks=True,
-                            lstrip_blocks=True, undefined=StrictUndefined)
+        context = self._get_context(info)
+        template = Template(self.template, trim_blocks=True, lstrip_blocks=True,
+                            undefined=StrictUndefined)
         return template.render(context)
 
 
 class _PCGenerator:
 
     def __init__(self, conanfile, dep, build_context_suffix=None):
         self._conanfile = conanfile
@@ -336,15 +311,15 @@
 
         * Apart from those PC files, if there are any aliases declared, they will be created too.
         """
         def _update_pc_files(info):
             pc_files[f"{info.name}.pc"] = self._content_generator.content(info)
             for alias in info.aliases:
                 alias_info = _PCInfo(alias, [info.name], f"Alias {alias} for {info.name}", None, [])
-                pc_files[f"{alias}.pc"] = self._content_generator.shortened_content(alias_info)
+                pc_files[f"{alias}.pc"] = self._content_generator.content(alias_info)
 
         pc_files = {}
         # If the package has no components, then we have to calculate only the root pc file
         if not self._dep.cpp_info.has_components:
             package_info = self.package_info
             _update_pc_files(package_info)
             return pc_files
@@ -361,19 +336,19 @@
         # if it does not already exist in components one
         # Issue related: https://github.com/conan-io/conan/issues/10341
         pkg_name = _get_package_name(self._dep, self._build_context_suffix)
         if f"{pkg_name}.pc" not in pc_files:
             package_info = _PCInfo(pkg_name, pkg_requires, f"Conan package: {pkg_name}",
                                    self._dep.cpp_info, _get_package_aliases(self._dep))
             # It'll be enough creating a shortened PC file. This file will be like an alias
-            pc_files[f"{package_info.name}.pc"] = self._content_generator.shortened_content(package_info)
+            pc_files[f"{package_info.name}.pc"] = self._content_generator.content(package_info)
             for alias in package_info.aliases:
                 alias_info = _PCInfo(alias, [package_info.name],
                                      f"Alias {alias} for {package_info.name}", None, [])
-                pc_files[f"{alias}.pc"] = self._content_generator.shortened_content(alias_info)
+                pc_files[f"{alias}.pc"] = self._content_generator.content(alias_info)
 
         return pc_files
 
 
 class PkgConfigDeps:
 
     def __init__(self, conanfile):
```

### Comparing `conan-2.0.7/conan/tools/google/bazel.py` & `conan-2.0.8/conan/tools/google/bazel.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/google/bazeldeps.py` & `conan-2.0.8/conan/tools/google/bazeldeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/google/layout.py` & `conan-2.0.8/conan/tools/google/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/google/toolchain.py` & `conan-2.0.8/conan/tools/google/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/intel/intel_cc.py` & `conan-2.0.8/conan/tools/intel/intel_cc.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/layout/__init__.py` & `conan-2.0.8/conan/tools/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/meson/helpers.py` & `conan-2.0.8/conan/tools/meson/helpers.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/meson/meson.py` & `conan-2.0.8/conan/tools/meson/meson.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/meson/toolchain.py` & `conan-2.0.8/conan/tools/meson/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/microsoft/__init__.py` & `conan-2.0.8/conan/tools/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/microsoft/layout.py` & `conan-2.0.8/conan/tools/microsoft/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/microsoft/msbuild.py` & `conan-2.0.8/conan/tools/microsoft/msbuild.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/microsoft/msbuilddeps.py` & `conan-2.0.8/conan/tools/microsoft/msbuilddeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/microsoft/nmakedeps.py` & `conan-2.0.8/conan/tools/microsoft/nmakedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/microsoft/nmaketoolchain.py` & `conan-2.0.8/conan/tools/microsoft/nmaketoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/microsoft/subsystems.py` & `conan-2.0.8/conan/tools/microsoft/subsystems.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/microsoft/toolchain.py` & `conan-2.0.8/conan/tools/microsoft/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/microsoft/visual.py` & `conan-2.0.8/conan/tools/microsoft/visual.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/premake/premake.py` & `conan-2.0.8/conan/tools/premake/premake.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/premake/premakedeps.py` & `conan-2.0.8/conan/tools/premake/premakedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/qbs/qbs.py` & `conan-2.0.8/conan/tools/qbs/qbs.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/qbs/qbsprofile.py` & `conan-2.0.8/conan/tools/qbs/qbsprofile.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/scm/git.py` & `conan-2.0.8/conan/tools/scm/git.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan/tools/system/package_manager.py` & `conan-2.0.8/conan/tools/system/package_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conan.egg-info/PKG-INFO` & `conan-2.0.8/conan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan
-Version: 2.0.7
+Version: 2.0.8
 Summary: Conan C/C++ package manager
 Home-page: https://conan.io
 Author: JFrog LTD
 Author-email: luism@jfrog.com
 License: MIT
 Project-URL: Documentation, https://docs.conan.io
 Project-URL: Source, https://github.com/conan-io/conan
```

### Comparing `conan-2.0.7/conan.egg-info/SOURCES.txt` & `conan-2.0.8/conan.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 conan/internal/cache/conan_reference_layout.py
 conan/internal/cache/db/__init__.py
 conan/internal/cache/db/cache_database.py
 conan/internal/cache/db/packages_table.py
 conan/internal/cache/db/recipes_table.py
 conan/internal/cache/db/table.py
 conan/tools/__init__.py
+conan/tools/helpers.py
 conan/tools/android/__init__.py
 conan/tools/android/utils.py
 conan/tools/apple/__init__.py
 conan/tools/apple/apple.py
 conan/tools/apple/xcodebuild.py
 conan/tools/apple/xcodedeps.py
 conan/tools/apple/xcodetoolchain.py
```

### Comparing `conan-2.0.7/conans/client/cache/cache.py` & `conan-2.0.8/conans/client/cache/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,16 +74,14 @@
     def assign_prev(self, layout: PackageLayout):
         return self._data_cache.assign_prev(layout)
 
     # Recipe methods
     def recipe_layout(self, ref: RecipeReference):
         return self._data_cache.get_recipe_layout(ref)
 
-    ref_layout = recipe_layout
-
     def get_latest_recipe_reference(self, ref):
         # TODO: We keep this for testing only, to be removed
         assert ref.revision is None
         return self._data_cache.get_recipe_layout(ref).reference
 
     def get_recipe_revisions_references(self, ref):
         # For listing multiple revisions only
```

### Comparing `conan-2.0.7/conans/client/cache/editable.py` & `conan-2.0.8/conans/client/cache/editable.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/cache/remote_registry.py` & `conan-2.0.8/conans/client/cache/remote_registry.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/cmd/export.py` & `conan-2.0.8/conans/client/cmd/export.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,17 @@
     scoped_output.info(f"Exporting package recipe: {conanfile_path}")
 
     export_folder = recipe_layout.export()
     export_src_folder = recipe_layout.export_sources()
     # TODO: cache2.0 move this creation to other place
     mkdir(export_folder)
     mkdir(export_src_folder)
-    conanfile.folders.set_base_recipe_metadata(recipe_layout.metadata())
+    recipe_metadata = recipe_layout.metadata()
+    mkdir(recipe_metadata)
+    conanfile.folders.set_base_recipe_metadata(recipe_metadata)
     export_recipe(conanfile, export_folder)
     export_source(conanfile, export_src_folder)
     shutil.copy2(conanfile_path, recipe_layout.conanfile())
 
     # Execute post-export hook before computing the digest
     hook_manager.execute("post_export", conanfile=conanfile)
     conanfile.folders.set_base_export(None)
```

### Comparing `conan-2.0.7/conans/client/cmd/uploader.py` & `conan-2.0.8/conans/client/cmd/uploader.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     def __init__(self, app: ConanApp):
         self._app = app
         self._output = ConanOutput()
 
     def prepare(self, upload_bundle, enabled_remotes):
         self._output.info("Preparing artifacts to upload")
         for ref, bundle in upload_bundle.refs():
-            layout = self._app.cache.ref_layout(ref)
+            layout = self._app.cache.recipe_layout(ref)
             conanfile_path = layout.conanfile()
             conanfile = self._app.loader.load_basic(conanfile_path)
 
             if bundle.get("upload"):
                 self._prepare_recipe(ref, bundle, conanfile, enabled_remotes)
             for pref, prev_bundle in upload_bundle.prefs(ref, bundle):
                 if prev_bundle.get("upload"):
@@ -93,15 +93,15 @@
 
     def _prepare_recipe(self, ref, ref_bundle, conanfile, remotes):
         """ do a bunch of things that are necessary before actually executing the upload:
         - retrieve exports_sources to complete the recipe if necessary
         - compress the artifacts in conan_export.tgz and conan_export_sources.tgz
         """
         try:
-            recipe_layout = self._app.cache.ref_layout(ref)
+            recipe_layout = self._app.cache.recipe_layout(ref)
             retrieve_exports_sources(self._app.remote_manager, recipe_layout, conanfile, ref,
                                      remotes)
             cache_files = self._compress_recipe_files(recipe_layout, ref)
             ref_bundle["files"] = cache_files
         except Exception as e:
             raise ConanException(f"{ref} Error while compressing: {e}")
```

### Comparing `conan-2.0.7/conans/client/cmd/user.py` & `conan-2.0.8/conans/client/cmd/user.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/conanfile/build.py` & `conan-2.0.8/conans/client/conanfile/build.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from conans.errors import conanfile_exception_formatter
 from conans.util.files import chdir, mkdir
 
 
 def run_build_method(conanfile, hook_manager):
     mkdir(conanfile.build_folder)
+    mkdir(conanfile.package_metadata_folder)
     with chdir(conanfile.build_folder):
         hook_manager.execute("pre_build", conanfile=conanfile)
         if hasattr(conanfile, "build"):
             conanfile.output.highlight("Calling build()")
             with conanfile_exception_formatter(conanfile, "build"):
                 try:
                     conanfile.build()
```

### Comparing `conan-2.0.7/conans/client/conanfile/configure.py` & `conan-2.0.8/conans/client/conanfile/configure.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 from conans.errors import conanfile_exception_formatter
 from conans.model.pkg_type import PackageType
 from conans.model.requires import BuildRequirements, TestRequirements, ToolRequirements
-from conans.util.env import no_op
+from conan.tools import default_config_options, default_configure
 
 
 def run_configure_method(conanfile, down_options, profile_options, ref):
     """ Run all the config-related functions for the given conanfile object """
 
-    # Avoid extra time manipulating the sys.path for python
-    with no_op():  # TODO: Remove this in a later refactor
-        if hasattr(conanfile, "config_options"):
-            with conanfile_exception_formatter(conanfile, "config_options"):
-                conanfile.config_options()
-
-        # Assign only the current package options values, but none of the dependencies
-        is_consumer = conanfile._conan_is_consumer
-        conanfile.options.apply_downstream(down_options, profile_options, ref, is_consumer)
-
-        if hasattr(conanfile, "configure"):
-            with conanfile_exception_formatter(conanfile, "configure"):
-                conanfile.configure()
-
-        self_options, up_options = conanfile.options.get_upstream_options(down_options, ref,
-                                                                          is_consumer)
-        # self_options are the minimum to reproduce state, as defined from downstream (not profile)
-        conanfile.self_options = self_options
-        # up_options are the minimal options that should be propagated to dependencies
-        conanfile.up_options = up_options
-
-        PackageType.compute_package_type(conanfile)
-
-        conanfile.build_requires = BuildRequirements(conanfile.requires)
-        conanfile.test_requires = TestRequirements(conanfile.requires)
-        conanfile.tool_requires = ToolRequirements(conanfile.requires)
-
-        if hasattr(conanfile, "requirements"):
-            with conanfile_exception_formatter(conanfile, "requirements"):
-                conanfile.requirements()
-
-        # TODO: Maybe this could be integrated in one single requirements() method
-        if hasattr(conanfile, "build_requirements"):
-            with conanfile_exception_formatter(conanfile, "build_requirements"):
-                conanfile.build_requirements()
+    if hasattr(conanfile, "config_options"):
+        with conanfile_exception_formatter(conanfile, "config_options"):
+            conanfile.config_options()
+    else:
+        default_config_options(conanfile)
+
+    # Assign only the current package options values, but none of the dependencies
+    is_consumer = conanfile._conan_is_consumer
+    conanfile.options.apply_downstream(down_options, profile_options, ref, is_consumer)
+
+    if hasattr(conanfile, "configure"):
+        with conanfile_exception_formatter(conanfile, "configure"):
+            conanfile.configure()
+    else:
+        default_configure(conanfile)
+
+    self_options, up_options = conanfile.options.get_upstream_options(down_options, ref,
+                                                                      is_consumer)
+    # self_options are the minimum to reproduce state, as defined from downstream (not profile)
+    conanfile.self_options = self_options
+    # up_options are the minimal options that should be propagated to dependencies
+    conanfile.up_options = up_options
+
+    PackageType.compute_package_type(conanfile)
+
+    conanfile.build_requires = BuildRequirements(conanfile.requires)
+    conanfile.test_requires = TestRequirements(conanfile.requires)
+    conanfile.tool_requires = ToolRequirements(conanfile.requires)
+
+    if hasattr(conanfile, "requirements"):
+        with conanfile_exception_formatter(conanfile, "requirements"):
+            conanfile.requirements()
+
+    if hasattr(conanfile, "build_requirements"):
+        with conanfile_exception_formatter(conanfile, "build_requirements"):
+            conanfile.build_requirements()
```

### Comparing `conan-2.0.7/conans/client/conanfile/package.py` & `conan-2.0.8/conans/client/conanfile/package.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/conf/__init__.py` & `conan-2.0.8/conans/client/conf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     gcc:
         version: ["4.1", "4.4", "4.5", "4.6", "4.7", "4.8", "4.9",
                     "5", "5.1", "5.2", "5.3", "5.4", "5.5",
                     "6", "6.1", "6.2", "6.3", "6.4", "6.5",
                     "7", "7.1", "7.2", "7.3", "7.4", "7.5",
                     "8", "8.1", "8.2", "8.3", "8.4", "8.5",
                     "9", "9.1", "9.2", "9.3", "9.4", "9.5",
-                    "10", "10.1", "10.2", "10.3", "10.4",
+                    "10", "10.1", "10.2", "10.3", "10.4", "10.5",
                     "11", "11.1", "11.2", "11.3",
                     "12", "12.1", "12.2", "12.3",
                     "13", "13.1"]
         libcxx: [libstdc++, libstdc++11]
         threads: [null, posix, win32]  # Windows MinGW
         exception: [null, dwarf2, sjlj, seh]  # Windows MinGW
         cppstd: [null, 98, gnu98, 11, gnu11, 14, gnu14, 17, gnu17, 20, gnu20, 23, gnu23]
```

### Comparing `conan-2.0.7/conans/client/conf/config_installer.py` & `conan-2.0.8/conans/client/conf/config_installer.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/conf/detect.py` & `conan-2.0.8/conans/client/conf/detect.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/conf/detect_vs.py` & `conan-2.0.8/conans/client/conf/detect_vs.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/conf/required_version.py` & `conan-2.0.8/conans/client/conf/required_version.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/downloaders/caching_file_downloader.py` & `conan-2.0.8/conans/client/downloaders/caching_file_downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,18 +154,18 @@
     """
     def __init__(self, requester, config, scope=None):
         self._download_cache = config.get("core.download:download_cache")
         if self._download_cache and not os.path.isabs(self._download_cache):
             raise ConanException("core.download:download_cache must be an absolute path")
         self._file_downloader = FileDownloader(requester, scope=scope)
 
-    def download(self, url, file_path, auth, verify_ssl, retry, retry_wait):
-        if not self._download_cache:
+    def download(self, url, file_path, auth, verify_ssl, retry, retry_wait, metadata=False):
+        if not self._download_cache or metadata:  # Metadata not cached and can be overwritten
             self._file_downloader.download(url, file_path, retry=retry, retry_wait=retry_wait,
-                                           verify_ssl=verify_ssl, auth=auth, overwrite=False)
+                                           verify_ssl=verify_ssl, auth=auth, overwrite=metadata)
             return
 
         download_cache = DownloadCache(self._download_cache)
         cached_path, h = download_cache.cached_path(url)
         with download_cache.lock(h):
             remove_if_dirty(cached_path)
```

### Comparing `conan-2.0.7/conans/client/downloaders/download_cache.py` & `conan-2.0.8/conans/client/downloaders/download_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,20 @@
 
         if not os.path.exists(path_backups):
             return []
 
         if excluded_urls is None:
             excluded_urls = []
 
-        all_refs = {str(k) for k, ref in package_list.refs()
-                    if ref.get("upload") or any(should_upload_sources(p)
-                                                for p in ref["packages"].values())}
+        all_refs = set()
+        for k, ref in package_list.refs():
+            packages = ref.get("packages", {}).values()
+            if ref.get("upload") or any(should_upload_sources(p) for p in packages):
+                all_refs.add(str(k))
+
         for f in os.listdir(path_backups):
             if f.endswith(".json"):
                 f = os.path.join(path_backups, f)
                 content = json.loads(load(f))
                 refs = content["references"]
                 # unknown entries are not uploaded at this moment, the flow is not expected.
                 for ref, urls in refs.items():
```

### Comparing `conan-2.0.7/conans/client/downloaders/file_downloader.py` & `conan-2.0.8/conans/client/downloaders/file_downloader.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/generators/__init__.py` & `conan-2.0.8/conans/client/generators/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     for f in os.listdir(path):
         if not f.endswith(".py") or f.startswith("_"):
             continue
         full_path = os.path.join(path, f)
         mod, _ = load_python_file(full_path)
         for name, value in inspect.getmembers(mod):
             if inspect.isclass(value) and not name.startswith("_"):
-                result = {name: value}
+                result[name] = value
     return result
 
 
 def write_generators(conanfile, app):
     new_gen_folder = conanfile.generators_folder
     _receive_conf(conanfile)
```

### Comparing `conan-2.0.7/conans/client/graph/build_mode.py` & `conan-2.0.8/conans/client/graph/build_mode.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/graph/compatibility.py` & `conan-2.0.8/conans/client/graph/compatibility.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/graph/compute_pid.py` & `conan-2.0.8/conans/client/graph/compute_pid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import OrderedDict
 
 from conans.errors import conanfile_exception_formatter, ConanInvalidConfiguration, \
     conanfile_remove_attr, ConanException
 from conans.model.info import ConanInfo, RequirementsInfo, RequirementInfo, PythonRequiresInfo
+from conan.tools import default_package_id
 
 
 def compute_package_id(node, new_config):
     """
     Compute the binary package ID of this node
     """
     conanfile = node.conanfile
@@ -77,9 +78,10 @@
                     conanfile.info.invalid = str(e)
 
     # Once we are done, call package_id() to narrow and change possible values
     if hasattr(conanfile, "package_id"):
         with conanfile_exception_formatter(conanfile, "package_id"):
             with conanfile_remove_attr(conanfile, ['cpp_info', 'settings', 'options'], "package_id"):
                 conanfile.package_id()
-
+    else:
+        default_package_id(conanfile)
     conanfile.info.validate()
```

### Comparing `conan-2.0.7/conans/client/graph/graph.py` & `conan-2.0.8/conans/client/graph/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/graph/graph_binaries.py` & `conan-2.0.8/conans/client/graph/graph_binaries.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/graph/graph_builder.py` & `conan-2.0.8/conans/client/graph/graph_builder.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/graph/graph_error.py` & `conan-2.0.8/conans/client/graph/graph_error.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/graph/install_graph.py` & `conan-2.0.8/conans/client/graph/install_graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,16 +181,18 @@
 class InstallGraph:
     """ A graph containing the package references in order to be built/downloaded
     """
 
     def __init__(self, deps_graph=None):
         self._nodes = {}  # ref with rev: _InstallGraphNode
 
+        self._is_test_package = False
         if deps_graph is not None:
             self._initialize_deps_graph(deps_graph)
+            self._is_test_package = deps_graph.root.conanfile.tested_reference_str is not None
 
     @staticmethod
     def load(filename):
         data = json.loads(load(filename))
         filename = os.path.basename(filename)
         filename = os.path.splitext(filename)[0]
         install_graph = InstallGraph.deserialize(data, filename)
@@ -274,16 +276,15 @@
                 else:
                     binary, reason = "Invalid", node.conanfile.info.invalid
                 msg.append("{}: {}: {}".format(node.conanfile, binary, reason))
             raise ConanInvalidConfiguration("\n".join(msg))
         if missing:
             self._raise_missing(missing)
 
-    @staticmethod
-    def _raise_missing(missing):
+    def _raise_missing(self, missing):
         # TODO: Remove out argument
         # TODO: A bit dirty access to .pref
         missing_prefs = set(n.nodes[0].pref for n in missing)  # avoid duplicated
         missing_prefs_str = list(sorted([str(pref) for pref in missing_prefs]))
         out = ConanOutput()
         for pref_str in missing_prefs_str:
             out.error("Missing binary: %s" % pref_str)
@@ -295,19 +296,26 @@
         package_id = node.package_id
         ref, conanfile = node.ref, node.conanfile
 
         msg = f"Can't find a '{ref}' package binary '{package_id}' for the configuration:\n"\
               f"{conanfile.info.dumps()}"
         conanfile.output.warning(msg)
         missing_pkgs = "', '".join(list(sorted([str(pref.ref) for pref in missing_prefs])))
-        if len(missing_prefs) >= 5:
-            build_str = "--build=missing"
+        if self._is_test_package:
+            build_msg = "'conan test' tested packages must exist, and '--build' argument " \
+                        "is used only for the 'test_package' dependencies, not for the tested " \
+                        "dependencies"
         else:
-            build_str = " ".join(list(sorted(["--build=%s" % str(pref.ref) for pref in missing_prefs])))
+            if len(missing_prefs) >= 5:
+                build_str = "--build=missing"
+            else:
+                build_str = " ".join(list(sorted(["--build=%s" % str(pref.ref)
+                                                  for pref in missing_prefs])))
+            build_msg = f"or try to build locally from sources using the '{build_str}' argument"
 
         raise ConanException(textwrap.dedent(f'''\
            Missing prebuilt package for '{missing_pkgs}'
            Check the available packages using 'conan list {ref}:* -r=remote'
-           or try to build locally from sources using the '{build_str}' argument
+           {build_msg}
 
            More Info at 'https://docs.conan.io/2/knowledge/faq.html#error-missing-prebuilt-package'
            '''))
```

### Comparing `conan-2.0.7/conans/client/graph/profile_node_definer.py` & `conan-2.0.8/conans/client/graph/profile_node_definer.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/graph/provides.py` & `conan-2.0.8/conans/client/graph/provides.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/graph/proxy.py` & `conan-2.0.8/conans/client/graph/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         try:
             recipe_layout = self._cache.recipe_layout(reference)
             ref = recipe_layout.reference  # latest revision if it was not defined
         except ConanException:
             # NOT in disk, must be retrieved from remotes
             # we will only check all servers for latest revision if we did a --update
             remote, new_ref = self._download_recipe(reference, remotes, output, update, check_update)
-            recipe_layout = self._cache.ref_layout(new_ref)
+            recipe_layout = self._cache.recipe_layout(new_ref)
             status = RECIPE_DOWNLOADED
             conanfile_path = recipe_layout.conanfile()
             return conanfile_path, status, remote, new_ref
 
         # TODO: cache2.0: check with new --update flows
         conanfile_path = recipe_layout.conanfile()
 
@@ -70,15 +70,15 @@
         cache_time = ref.timestamp
         if remote_ref.revision != ref.revision:
             if cache_time < remote_ref.timestamp:
                 # the remote one is newer
                 if update:
                     output.info("Retrieving from remote '%s'..." % remote.name)
                     self._download(remote_ref, remote)
-                    new_recipe_layout = self._cache.ref_layout(remote_ref)
+                    new_recipe_layout = self._cache.recipe_layout(remote_ref)
                     new_conanfile_path = new_recipe_layout.conanfile()
                     status = RECIPE_UPDATED
                     return new_conanfile_path, status, remote, remote_ref
                 else:
                     status = RECIPE_UPDATEABLE
             else:
                 status = RECIPE_NEWER
```

### Comparing `conan-2.0.7/conans/client/graph/python_requires.py` & `conan-2.0.8/conans/client/graph/python_requires.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/graph/range_resolver.py` & `conan-2.0.8/conans/client/graph/range_resolver.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/hook_manager.py` & `conan-2.0.8/conans/client/hook_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/installer.py` & `conan-2.0.8/conans/client/installer.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         return prev
 
     def build_package(self, node, package_layout):
         conanfile = node.conanfile
         pref = node.pref
 
         # TODO: cache2.0 fix this
-        recipe_layout = self._cache.ref_layout(pref.ref)
+        recipe_layout = self._cache.recipe_layout(pref.ref)
 
         base_source = recipe_layout.source()
         base_package = package_layout.package()
 
         base_build, skip_build = self._get_build_folder(conanfile, package_layout)
 
         # PREPARE SOURCES
@@ -151,15 +151,15 @@
                     # In local cache, install folder always is build_folder
                     self._build(conanfile, pref)
                     clean_dirty(base_build)
 
                 prev = self._package(conanfile, pref)
                 assert prev
                 node.prev = prev
-            except ConanException as exc:
+            except ConanException as exc:  # TODO: Remove this? unnecessary?
                 raise exc
 
         return node.pref
 
 
 class BinaryInstaller:
     """ main responsible of retrieving binary packages or building them from source
@@ -176,15 +176,15 @@
         conanfile = node.conanfile
         download_source = conanfile.conf.get("tools.build:download_source", check_type=bool)
 
         if not download_source and node.binary != BINARY_BUILD:
             return
 
         conanfile = node.conanfile
-        recipe_layout = self._cache.ref_layout(node.ref)
+        recipe_layout = self._cache.recipe_layout(node.ref)
         export_source_folder = recipe_layout.export_sources()
         source_folder = recipe_layout.source()
 
         retrieve_exports_sources(self._remote_manager, recipe_layout, conanfile, node.ref, remotes)
 
         conanfile.folders.set_base_source(source_folder)
         conanfile.folders.set_base_export_sources(source_folder)
@@ -245,15 +245,15 @@
         handled_count = 1
 
         self._download_bulk(install_order)
         for level in install_order:
             for install_reference in level:
                 for package in install_reference.packages.values():
                     self._install_source(package.nodes[0], remotes)
-                    self._handle_package(package, install_reference, None, handled_count, package_count)
+                    self._handle_package(package, install_reference, handled_count, package_count)
                     handled_count += 1
 
         MockInfoProperty.message()
 
     def _download_bulk(self, install_order):
         """ executes the download of packages (both download and update), only once for a given
         PREF
@@ -281,17 +281,17 @@
             for node in downloads:
                 self._download_pkg(node)
 
     def _download_pkg(self, package):
         node = package.nodes[0]
         assert node.pref.revision is not None
         assert node.pref.timestamp is not None
-        self._remote_manager.get_package(node.conanfile, node.pref, node.binary_remote)
+        self._remote_manager.get_package(node.pref, node.binary_remote)
 
-    def _handle_package(self, package, install_reference, remotes, handled_count, total_count):
+    def _handle_package(self, package, install_reference, handled_count, total_count):
         if package.binary == BINARY_SYSTEM_TOOL:
             return
 
         if package.binary in (BINARY_EDITABLE, BINARY_EDITABLE_BUILD):
             self._handle_node_editable(package)
             return
 
@@ -322,20 +322,22 @@
             node = package.nodes[0]
             pref = node.pref
             assert node.prev, "PREV for %s is None" % str(pref)
             node.conanfile.output.success(f'Already installed! ({handled_count} of {total_count})')
 
         # Make sure that all nodes with same pref compute package_info()
         pkg_folder = package_layout.package()
+        pkg_metadata = package_layout.metadata()
         assert os.path.isdir(pkg_folder), "Pkg '%s' folder must exist: %s" % (str(pref), pkg_folder)
         for n in package.nodes:
             n.prev = pref.revision  # Make sure the prev is assigned
             conanfile = n.conanfile
             # Call the info method
             conanfile.folders.set_base_package(pkg_folder)
+            conanfile.folders.set_base_pkg_metadata(pkg_metadata)
             self._call_package_info(conanfile, pkg_folder, is_editable=False)
 
     def _handle_node_editable(self, install_node):
         # It will only run generation
         node = install_node.nodes[0]
         conanfile = node.conanfile
         ref = node.ref
```

### Comparing `conan-2.0.7/conans/client/loader.py` & `conan-2.0.8/conans/client/loader.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/loader_txt.py` & `conan-2.0.8/conans/client/loader_txt.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/migrations.py` & `conan-2.0.8/conans/client/migrations.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/pkg_sign.py` & `conan-2.0.8/conans/client/pkg_sign.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             mkdir(metadata_sign)
             self._plugin_sign_function(ref, artifacts_folder=folder, signature_folder=metadata_sign)
             for f in os.listdir(metadata_sign):
                 files[f"{METADATA}/sign/{f}"] = os.path.join(metadata_sign, f)
 
         for rref, recipe_bundle in upload_data.refs():
             if recipe_bundle["upload"]:
-                _sign(rref, recipe_bundle["files"], self._cache.ref_layout(rref).download_export())
+                _sign(rref, recipe_bundle["files"], self._cache.recipe_layout(rref).download_export())
             for pref, pkg_bundle in upload_data.prefs(rref, recipe_bundle):
                 if pkg_bundle["upload"]:
                     _sign(pref, pkg_bundle["files"], self._cache.pkg_layout(pref).download_package())
 
     def verify(self, ref, folder):
         if self._plugin_verify_function is None:
             return
```

### Comparing `conan-2.0.7/conans/client/profile_loader.py` & `conan-2.0.8/conans/client/profile_loader.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/remote_manager.py` & `conan-2.0.8/conans/client/remote_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,20 +36,14 @@
 
     def upload_package(self, pref, files_to_upload, remote):
         assert pref.ref.revision, "upload_package requires RREV"
         assert pref.revision, "upload_package requires PREV"
         self._call_remote(remote, "upload_package", pref, files_to_upload)
 
     def get_recipe(self, ref, remote, metadata=None):
-        """
-        Read the conans from remotes
-        Will iterate the remotes to find the conans unless remote was specified
-
-        returns (dict relative_filepath:abs_path , remote_name)"""
-
         assert ref.revision, "get_recipe without revision specified"
 
         layout = self._cache.get_or_create_ref_layout(ref)
         layout.export_remove()
 
         download_export = layout.download_export()
         try:
@@ -86,21 +80,20 @@
     def get_recipe_metadata(self, ref, remote, metadata):
         """
         Get only the metadata for a locally existing recipe in Cache
         """
         assert ref.revision, "get_recipe without revision specified"
         output = ConanOutput(scope=str(ref))
         output.info("Retrieving recipe metadata from remote '%s' " % remote.name)
-        layout = self._cache.ref_layout(ref)
+        layout = self._cache.recipe_layout(ref)
         download_export = layout.download_export()
         try:
             self._call_remote(remote, "get_recipe", ref, download_export, metadata,
                               only_metadata=True)
         except BaseException:  # So KeyboardInterrupt also cleans things
-
             output.error(f"Error downloading metadata from remote '{remote.name}'")
             raise
 
     def get_recipe_sources(self, ref, layout, remote):
         assert ref.revision, "get_recipe_sources requires RREV"
 
         download_folder = layout.download_export()
@@ -109,24 +102,24 @@
         if not zipped_files:
             mkdir(export_sources_folder)  # create the folder even if no source files
             return
 
         tgz_file = zipped_files[EXPORT_SOURCES_TGZ_NAME]
         uncompress_file(tgz_file, export_sources_folder, scope=str(ref))
 
-    def get_package(self, conanfile, pref, remote, metadata=None):
-        conanfile.output.info("Retrieving package %s from remote '%s' " % (pref.package_id,
-                                                                           remote.name))
+    def get_package(self, pref, remote, metadata=None):
+        output = ConanOutput(scope=str(pref.ref))
+        output.info("Retrieving package %s from remote '%s' " % (pref.package_id, remote.name))
 
         assert pref.revision is not None
 
         pkg_layout = self._cache.get_or_create_pkg_layout(pref)
         pkg_layout.package_remove()  # Remove first the destination folder
         with pkg_layout.set_dirty_context_manager():
-            self._get_package(pkg_layout, pref, remote, conanfile.output, metadata)
+            self._get_package(pkg_layout, pref, remote, output, metadata)
 
     def get_package_metadata(self, pref, remote, metadata):
         """
         only download the metadata, not the packge itself
         """
         output = ConanOutput(scope=str(pref.ref))
         output.info("Retrieving package metadata %s from remote '%s' "
```

### Comparing `conan-2.0.7/conans/client/rest/__init__.py` & `conan-2.0.8/conans/client/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/rest/auth_manager.py` & `conan-2.0.8/conans/client/rest/auth_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/rest/client_routes.py` & `conan-2.0.8/conans/client/rest/client_routes.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/rest/conan_requester.py` & `conan-2.0.8/conans/client/rest/conan_requester.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/rest/file_uploader.py` & `conan-2.0.8/conans/client/rest/file_uploader.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/rest/rest_client.py` & `conan-2.0.8/conans/client/rest/rest_client.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/rest/rest_client_common.py` & `conan-2.0.8/conans/client/rest/rest_client_common.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/rest/rest_client_v2.py` & `conan-2.0.8/conans/client/rest/rest_client_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,33 +35,36 @@
         # and make sure the paths like metadata/sign/signature are normalized to /
         data["files"] = list(d.replace("\\", "/") for d in data["files"].keys())
         return data
 
     def get_recipe(self, ref, dest_folder, metadata, only_metadata):
         url = self.router.recipe_snapshot(ref)
         data = self._get_file_list_json(url)
-        files = data["files"]
-        accepted_files = ["conanfile.py", "conan_export.tgz", "conanmanifest.txt", "metadata/sign"]
-        if only_metadata:
-            accepted_files = []
-        metadata = metadata or []
-        metadata = [f"metadata/{m}" for m in metadata]
-        files = [f for f in files if any(f.startswith(m) for m in accepted_files)
-                 or any(fnmatch.fnmatch(f, m) for m in metadata)]
+        server_files = data["files"]
+        result = {}
 
-        # If we didn't indicated reference, server got the latest, use absolute now, it's safer
-        urls = {fn: self.router.recipe_file(ref, fn) for fn in files}
-        self._download_and_save_files(urls, dest_folder, files, parallel=True)
-        ret = {fn: os.path.join(dest_folder, fn) for fn in files}
-        return ret
+        if not only_metadata:
+            accepted_files = ["conanfile.py", "conan_export.tgz", "conanmanifest.txt",
+                              "metadata/sign"]
+            files = [f for f in server_files if any(f.startswith(m) for m in accepted_files)]
+            # If we didn't indicated reference, server got the latest, use absolute now, it's safer
+            urls = {fn: self.router.recipe_file(ref, fn) for fn in files}
+            self._download_and_save_files(urls, dest_folder, files, parallel=True)
+            result.update({fn: os.path.join(dest_folder, fn) for fn in files})
+        if metadata:
+            metadata = [f"metadata/{m}" for m in metadata]
+            files = [f for f in server_files if any(fnmatch.fnmatch(f, m) for m in metadata)]
+            urls = {fn: self.router.recipe_file(ref, fn) for fn in files}
+            self._download_and_save_files(urls, dest_folder, files, parallel=True, metadata=True)
+            result.update({fn: os.path.join(dest_folder, fn) for fn in files})
+        return result
 
     def get_recipe_sources(self, ref, dest_folder):
         # If revision not specified, check latest
-        if not ref.revision:
-            ref, _ = self.get_latest_recipe_reference(ref)
+        assert ref.revision, f"get_recipe_sources() called without revision {ref}"
         url = self.router.recipe_snapshot(ref)
         data = self._get_file_list_json(url)
         files = data["files"]
         if EXPORT_SOURCES_TGZ_NAME not in files:
             return None
         files = [EXPORT_SOURCES_TGZ_NAME, ]
 
@@ -70,29 +73,34 @@
         self._download_and_save_files(urls, dest_folder, files, scope=str(ref))
         ret = {fn: os.path.join(dest_folder, fn) for fn in files}
         return ret
 
     def get_package(self, pref, dest_folder, metadata, only_metadata):
         url = self.router.package_snapshot(pref)
         data = self._get_file_list_json(url)
-        files = data["files"]
+        server_files = data["files"]
+        result = {}
         # Download only known files, but not metadata (except sign)
-        accepted_files = ["conaninfo.txt", "conan_package.tgz", "conanmanifest.txt", "metadata/sign"]
-        if only_metadata:
-            accepted_files = []
-        metadata = metadata or []
-        metadata = [f"metadata/{m}" for m in metadata]
-        files = [f for f in files if any(f.startswith(m) for m in accepted_files)
-                 or any(fnmatch.fnmatch(f, m) for m in metadata)]
-
-        # If we didn't indicated reference, server got the latest, use absolute now, it's safer
-        urls = {fn: self.router.package_file(pref, fn) for fn in files}
-        self._download_and_save_files(urls, dest_folder, files, scope=str(pref.ref))
-        ret = {fn: os.path.join(dest_folder, fn) for fn in files}
-        return ret
+        if not only_metadata:  # Retrieve package first, then metadata
+            accepted_files = ["conaninfo.txt", "conan_package.tgz", "conanmanifest.txt",
+                              "metadata/sign"]
+            files = [f for f in server_files if any(f.startswith(m) for m in accepted_files)]
+            # If we didn't indicated reference, server got the latest, use absolute now, it's safer
+            urls = {fn: self.router.package_file(pref, fn) for fn in files}
+            self._download_and_save_files(urls, dest_folder, files, scope=str(pref.ref))
+            result.update({fn: os.path.join(dest_folder, fn) for fn in files})
+
+        if metadata:
+            metadata = [f"metadata/{m}" for m in metadata]
+            files = [f for f in server_files if any(fnmatch.fnmatch(f, m) for m in metadata)]
+            urls = {fn: self.router.package_file(pref, fn) for fn in files}
+            self._download_and_save_files(urls, dest_folder, files, scope=str(pref.ref),
+                                          metadata=True)
+            result.update({fn: os.path.join(dest_folder, fn) for fn in files})
+        return result
 
     @staticmethod
     def _is_dir(path, files):
         if path == ".":
             return True
         for the_file in files["files"]:
             if path == the_file:
@@ -142,36 +150,38 @@
                 output.error("\nError uploading file: %s, '%s'" % (filename, exc))
                 failed.append(filename)
 
         if failed:
             raise ConanException("Execute upload again to retry upload the failed files: %s"
                                  % ", ".join(failed))
 
-    def _download_and_save_files(self, urls, dest_folder, files, parallel=False, scope=None):
+    def _download_and_save_files(self, urls, dest_folder, files, parallel=False, scope=None,
+                                 metadata=False):
         # Take advantage of filenames ordering, so that conan_package.tgz and conan_export.tgz
         # can be < conanfile, conaninfo, and sent always the last, so smaller files go first
         retry = self._config.get("core.download:retry", check_type=int, default=2)
         retry_wait = self._config.get("core.download:retry_wait", check_type=int, default=0)
         downloader = ConanInternalCacheDownloader(self.requester, self._config, scope=scope)
         threads = []
 
         for filename in sorted(files, reverse=True):
             resource_url = urls[filename]
             abs_path = os.path.join(dest_folder, filename)
             os.makedirs(os.path.dirname(abs_path), exist_ok=True)  # filename in subfolder must exist
             if parallel:
                 kwargs = {"url": resource_url, "file_path": abs_path, "retry": retry,
                           "retry_wait": retry_wait, "verify_ssl": self.verify_ssl,
-                          "auth": self.auth}
+                          "auth": self.auth, "metadata": metadata}
                 thread = ExceptionThread(target=downloader.download, kwargs=kwargs)
                 threads.append(thread)
                 thread.start()
             else:
                 downloader.download(url=resource_url, file_path=abs_path, auth=self.auth,
-                                    verify_ssl=self.verify_ssl, retry=retry, retry_wait=retry_wait)
+                                    verify_ssl=self.verify_ssl, retry=retry, retry_wait=retry_wait,
+                                    metadata=metadata)
         for t in threads:
             t.join()
         for t in threads:  # Need to join all before raising errors
             t.raise_errors()
 
     def remove_all_packages(self, ref):
         """ Remove all packages from the specified reference"""
```

### Comparing `conan-2.0.7/conans/client/source.py` & `conan-2.0.8/conans/client/source.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         conanfile.output.warning("This can take a while for big packages")
         rmdir(conanfile.folders.base_source)
         clean_dirty(conanfile.folders.base_source)
 
     if not os.path.exists(conanfile.folders.base_source):  # No source folder, need to get it
         with set_dirty_context_manager(conanfile.folders.base_source):
             mkdir(conanfile.source_folder)
+            mkdir(conanfile.recipe_metadata_folder)
 
             # First of all get the exported scm sources (if auto) or clone (if fixed)
             # Now move the export-sources to the right location
             merge_directories(export_source_folder, conanfile.folders.base_source)
 
             run_source_method(conanfile, hook_manager)
```

### Comparing `conan-2.0.7/conans/client/store/localdb.py` & `conan-2.0.8/conans/client/store/localdb.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/subsystems.py` & `conan-2.0.8/conans/client/subsystems.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/client/userio.py` & `conan-2.0.8/conans/client/userio.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/conan_server.py` & `conan-2.0.8/conans/conan_server.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/errors.py` & `conan-2.0.8/conans/errors.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/migrations.py` & `conan-2.0.8/conans/migrations.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/model/build_info.py` & `conan-2.0.8/conans/model/build_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -113,38 +113,16 @@
             "requires": self._requires,
             "properties": self._properties
         }
 
     @staticmethod
     def deserialize(contents):
         result = _Component()
-        # TODO: Refactor to avoid this repetition
-        fields = [
-            "includedirs",
-            "srcdirs",
-            "libdirs",
-            "resdirs",
-            "bindirs",
-            "builddirs",
-            "frameworkdirs",
-            "system_libs",
-            "frameworks",
-            "libs",
-            "defines",
-            "cflags",
-            "cxxflags",
-            "sharedlinkflags",
-            "exelinkflags",
-            "objects",
-            "sysroot",
-            "requires",
-            "properties"
-        ]
-        for f in fields:
-            setattr(result, f"_{f}", contents[f])
+        for field, value in contents.items():
+            setattr(result, f"_{field}", value)
         return result
 
     @property
     def includedirs(self):
         if self._includedirs is None:
             self._includedirs = []
         return self._includedirs
```

### Comparing `conan-2.0.7/conans/model/conan_file.py` & `conan-2.0.8/conans/model/conan_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,16 +274,16 @@
         return self.folders.build_folder
 
     @property
     def recipe_metadata_folder(self):
         return self.folders.recipe_metadata_folder
 
     @property
-    def pkg_metadata_folder(self):
-        return self.folders.pkg_metadata_folder
+    def package_metadata_folder(self):
+        return self.folders.package_metadata_folder
 
     @property
     def build_path(self) -> Path:
         assert self.build_folder is not None, "`build_folder` is `None`"
         return Path(self.build_folder)
 
     @property
```

### Comparing `conan-2.0.7/conans/model/conanfile_interface.py` & `conan-2.0.8/conans/model/conanfile_interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,18 +28,26 @@
         return self._conanfile.options
 
     @property
     def recipe_folder(self):
         return self._conanfile.recipe_folder
 
     @property
+    def recipe_metadata_folder(self):
+        return self._conanfile.recipe_metadata_folder
+
+    @property
     def package_folder(self):
         return self._conanfile.package_folder
 
     @property
+    def package_metadata_folder(self):
+        return self._conanfile.package_metadata_folder
+
+    @property
     def package_path(self) -> Path:
         assert self.package_folder is not None, "`package_folder` is `None`"
         return Path(self.package_folder)
 
     @property
     def ref(self):
         return self._conanfile.ref
```

### Comparing `conan-2.0.7/conans/model/conf.py` & `conan-2.0.8/conans/model/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     "tools.cmake.cmaketoolchain:user_toolchain": "Inject existing user toolchains at the beginning of conan_toolchain.cmake",
     "tools.cmake.cmaketoolchain:system_name": "Define CMAKE_SYSTEM_NAME in CMakeToolchain",
     "tools.cmake.cmaketoolchain:system_version": "Define CMAKE_SYSTEM_VERSION in CMakeToolchain",
     "tools.cmake.cmaketoolchain:system_processor": "Define CMAKE_SYSTEM_PROCESSOR in CMakeToolchain",
     "tools.cmake.cmaketoolchain:toolset_arch": "Toolset architecture to be used as part of CMAKE_GENERATOR_TOOLSET in CMakeToolchain",
     "tools.cmake.cmake_layout:build_folder_vars": "Settings and Options that will produce a different build folder and different CMake presets names",
     "tools.cmake:cmake_program": "Path to CMake executable",
+    "tools.cmake:install_strip": "Add --strip to cmake.instal()",
     "tools.files.download:retry": "Number of retries in case of failure when downloading",
     "tools.files.download:retry_wait": "Seconds to wait between download attempts",
     "tools.gnu:make_program": "Indicate path to make program",
     "tools.gnu:define_libcxx11_abi": "Force definition of GLIBCXX_USE_CXX11_ABI=1 for libstdc++11",
     "tools.gnu:pkg_config": "Path to pkg-config executable used by PkgConfig build helper",
     "tools.gnu:host_triplet": "Custom host triplet to pass to Autotools scripts",
     "tools.google.bazel:configs": "Define Bazel config file",
```

### Comparing `conan-2.0.7/conans/model/dependencies.py` & `conan-2.0.8/conans/model/dependencies.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/model/graph_lock.py` & `conan-2.0.8/conans/model/graph_lock.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/model/info.py` & `conan-2.0.8/conans/model/info.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/model/layout.py` & `conan-2.0.8/conans/model/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     def recipe_metadata_folder(self):
         return self._base_recipe_metadata
 
     def set_base_recipe_metadata(self, folder):
         self._base_recipe_metadata = folder
 
     @property
-    def pkg_metadata_folder(self):
+    def package_metadata_folder(self):
         return self._base_pkg_metadata
 
     def set_base_pkg_metadata(self, folder):
         self._base_pkg_metadata = folder
 
     @property
     def base_build(self):
```

### Comparing `conan-2.0.7/conans/model/manifest.py` & `conan-2.0.8/conans/model/manifest.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/model/options.py` & `conan-2.0.8/conans/model/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,48 +131,41 @@
     def __contains__(self, option):
         return str(option) in self._data
 
     def get_safe(self, field, default=None):
         return self._data.get(field, default)
 
     def rm_safe(self, field):
-        try:
-            delattr(self, field)
-        except ConanException:
-            pass
+        # This should never raise any exception, in any case
+        self._data.pop(field, None)
 
     def validate(self):
         for child in self._data.values():
             child.validate()
 
     def copy_conaninfo_options(self):
         # To generate a copy without validation, for package_id info.options value
         result = _PackageOptions()
         for k, v in self._data.items():
             result._data[k] = v.copy_conaninfo_option()
         return result
 
-    @property
-    def fields(self):
-        return sorted(list(self._data.keys()))
-
     def _ensure_exists(self, field):
         if self._constrained and field not in self._data:
             raise ConanException(option_not_exist_msg(field, list(self._data.keys())))
 
     def __getattr__(self, field):
         assert field[0] != "_", "ERROR %s" % field
         try:
             return self._data[field]
         except KeyError:
             raise ConanException(option_not_exist_msg(field, list(self._data.keys())))
 
     def __delattr__(self, field):
         assert field[0] != "_", "ERROR %s" % field
-        current_value = self._data.get(field)
         # It is always possible to remove an option, even if it is frozen (freeze=True),
         # and it got a value, because it is the only way an option could be removed
         # conditionally to other option value (like fPIC if shared)
         self._ensure_exists(field)
         del self._data[field]
 
     def __setattr__(self, field, value):
```

### Comparing `conan-2.0.7/conans/model/package_ref.py` & `conan-2.0.8/conans/model/package_ref.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/model/pkg_type.py` & `conan-2.0.8/conans/model/pkg_type.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/model/profile.py` & `conan-2.0.8/conans/model/profile.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/model/recipe_ref.py` & `conan-2.0.8/conans/model/recipe_ref.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/model/requires.py` & `conan-2.0.8/conans/model/requires.py`

 * *Files 4% similar despite different names*

```diff
@@ -272,28 +272,15 @@
             if dep_pkg_type is PackageType.SHARED or require.run:
                 downstream_require = Requirement(require.ref, headers=False, libs=False, build=True,
                                                  run=True, visible=False, direct=False)
                 return downstream_require
             return
 
         # Regular and test requires
-        if dep_pkg_type is PackageType.SHARED:
-            if pkg_type is PackageType.SHARED:
-                downstream_require = Requirement(require.ref, headers=False, libs=False, run=require.run)
-            elif pkg_type is PackageType.STATIC:
-                downstream_require = Requirement(require.ref, headers=False, libs=require.libs, run=require.run)
-            elif pkg_type is PackageType.APP:
-                downstream_require = Requirement(require.ref, headers=False, libs=False, run=require.run)
-            elif pkg_type is PackageType.HEADER:
-                downstream_require = Requirement(require.ref, headers=require.headers, libs=require.libs, run=require.run)
-            else:
-                assert pkg_type == PackageType.UNKNOWN
-                # TODO: This is undertested, changing it did not break tests
-                downstream_require = require.copy_requirement()
-        elif dep_pkg_type is PackageType.STATIC:
+        if dep_pkg_type is PackageType.SHARED or dep_pkg_type is PackageType.STATIC:
             if pkg_type is PackageType.SHARED:
                 downstream_require = Requirement(require.ref, headers=False, libs=False, run=require.run)
             elif pkg_type is PackageType.STATIC:
                 downstream_require = Requirement(require.ref, headers=False, libs=require.libs, run=require.run)
             elif pkg_type is PackageType.APP:
                 downstream_require = Requirement(require.ref, headers=False, libs=False, run=require.run)
             elif pkg_type is PackageType.HEADER:
```

### Comparing `conan-2.0.7/conans/model/rest_routes.py` & `conan-2.0.8/conans/model/rest_routes.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/model/settings.py` & `conan-2.0.8/conans/model/settings.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/model/version.py` & `conan-2.0.8/conans/model/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         items = value.rsplit("-", 1)  # split for pre-release
         if len(items) == 2:
             value, pre = items
             self._pre = Version(pre)  # This is a nested version by itself
         else:
             value = items[0]
             self._pre = None
+
         items = value.split(".")
         items = [_VersionItem(item) for item in items]
         self._items = tuple(items)
         while items and items[-1].value == 0:
             del items[-1]
         self._nonzero_items = tuple(items)
 
@@ -95,28 +96,26 @@
         try:
             items.append(self._items[index]+1)
         except TypeError:
             raise ConanException(f"Cannot bump '{self._value} version index {index}, not an int")
         items.extend([0] * (len(items) - index - 1))
         v = ".".join(str(i) for i in items)
         # prerelease and build are dropped while bumping digits
-        result = Version(v)
-        return result
+        return Version(v)
 
     def upper_bound(self, index):
         items = list(self._items[:index])
         try:
             items.append(self._items[index] + 1)
         except TypeError:
             raise ConanException(f"Cannot bump '{self._value} version index {index}, not an int")
         items.extend([0] * (len(items) - index - 1))
         v = ".".join(str(i) for i in items)
         v += "-"  # Exclude prereleases
-        result = Version(v)
-        return result
+        return Version(v)
 
     @property
     def pre(self):
         return self._pre
 
     @property
     def build(self):
```

### Comparing `conan-2.0.7/conans/model/version_range.py` & `conan-2.0.8/conans/model/version_range.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/paths/__init__.py` & `conan-2.0.8/conans/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/pylint_plugin.py` & `conan-2.0.8/conans/pylint_plugin.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/search/query_parse.py` & `conan-2.0.8/conans/search/query_parse.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/search/search.py` & `conan-2.0.8/conans/search/search.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/test/conftest.py` & `conan-2.0.8/conans/test/conftest.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/test/utils/artifactory.py` & `conan-2.0.8/conans/test/utils/artifactory.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/test/utils/mocks.py` & `conan-2.0.8/conans/test/utils/mocks.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,14 +58,17 @@
 
     def __getattr__(self, name):
         try:
             return self.values[name]
         except KeyError:
             raise ConanException("'%s' value not defined" % name)
 
+    def rm_safe(self, name):
+        self.values.pop(name, None)
+
 
 class MockCppInfo(object):
     def __init__(self):
         self.bin_paths = []
         self.lib_paths = []
         self.include_paths = []
         self.libs = []
@@ -77,26 +80,33 @@
 
 
 class MockConanfile(ConanFile):
 
     def __init__(self, settings, options=None, runner=None):
         self.display_name = ""
         self._conan_node = None
+        self.package_type = "unknown"
         self.folders = Folders()
         self.settings = settings
         self.settings_build = settings
         self.runner = runner
         self.options = options or MockOptions({})
         self.generators = []
         self.conf = Conf()
 
         class MockConanInfo:
-            pass
+            settings = None
+            options = None
+
+            def clear(self):
+                self.settings = {}
+                self.options = {}
         self.info = MockConanInfo()
         self.info.settings = settings  # Incomplete, only settings for Cppstd Min/Max tests
+        self.info.options = options
 
     def run(self, *args, **kwargs):
         if self.runner:
             kwargs["output"] = None
             self.runner(*args, **kwargs)
```

### Comparing `conan-2.0.7/conans/test/utils/profiles.py` & `conan-2.0.8/conans/test/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/test/utils/scm.py` & `conan-2.0.8/conans/test/utils/scm.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/test/utils/server_launcher.py` & `conan-2.0.8/conans/test/utils/server_launcher.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/test/utils/test_files.py` & `conan-2.0.8/conans/test/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/test/utils/tools.py` & `conan-2.0.8/conans/test/utils/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -653,15 +653,15 @@
         # Let's make it easier for all the test clients
         latest_prev = self.cache.get_latest_package_reference(pref)
         pkg_layout = self.cache.pkg_layout(latest_prev)
         return pkg_layout
 
     def get_latest_ref_layout(self, ref) -> RecipeLayout:
         """Get the latest RecipeLayout given a file reference"""
-        ref_layout = self.cache.ref_layout(ref)
+        ref_layout = self.cache.recipe_layout(ref)
         return ref_layout
 
     def get_default_host_profile(self):
         api = ConanAPI(cache_folder=self.cache_folder)
         return api.profiles.get_profile([api.profiles.get_default_host()])
 
     def get_default_build_profile(self):
@@ -761,23 +761,27 @@
         return package_id
 
     def created_package_reference(self, ref):
         pref = re.search(r"{}: Full package reference: (\S+)".format(str(ref)),
                                str(self.out)).group(1)
         return PkgReference.loads(pref)
 
-    def created_package_folder(self, ref):
-        pref = self.created_package_reference(ref)
-        prev = self.cache.get_latest_package_reference(pref)
-        pkg_folder = self.cache.pkg_layout(prev).package()
-        return pkg_folder
-
     def exported_recipe_revision(self):
         return re.search(r": Exported: .*#(\S+)", str(self.out)).group(1)
 
+    def exported_layout(self):
+        m = re.search(r": Exported: (\S+)", str(self.out)).group(1)
+        ref = RecipeReference.loads(m)
+        return self.cache.recipe_layout(ref)
+
+    def created_layout(self):
+        pref = re.search(r"(?s:.*)Full package reference: (\S+)", str(self.out)).group(1)
+        pref = PkgReference.loads(pref)
+        return self.cache.pkg_layout(pref)
+
 
 class TurboTestClient(TestClient):
 
     def __init__(self, *args, **kwargs):
         super(TurboTestClient, self).__init__(*args, **kwargs)
 
     def create(self, ref, conanfile=GenConanfile(), args=None, assert_error=False):
```

### Comparing `conan-2.0.7/conans/util/config_parser.py` & `conan-2.0.8/conans/util/config_parser.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/util/dates.py` & `conan-2.0.8/conans/util/dates.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/util/encrypt.py` & `conan-2.0.8/conans/util/encrypt.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/util/env.py` & `conan-2.0.8/conans/util/env.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,19 +21,14 @@
     try:
         yield
     finally:
         os.environ.clear()
         os.environ.update(old_env)
 
 
-@contextmanager
-def no_op():
-    yield
-
-
 def get_env(env_key, default=None, environment=None):
     """Get the env variable associated with env_key"""
     if environment is None:
         environment = os.environ
 
     env_var = environment.get(env_key, default)
     if env_var != default:
```

### Comparing `conan-2.0.7/conans/util/files.py` & `conan-2.0.8/conans/util/files.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/util/locks.py` & `conan-2.0.8/conans/util/locks.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/util/runners.py` & `conan-2.0.8/conans/util/runners.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/util/sha.py` & `conan-2.0.8/conans/util/sha.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/conans/util/windows.py` & `conan-2.0.8/conans/util/windows.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.7/setup.py` & `conan-2.0.8/setup.py`

 * *Files identical despite different names*

