# Comparing `tmp/kiara_plugin.service-0.4.3.tar.gz` & `tmp/kiara_plugin.service-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.service-0.4.3.tar", last modified: Thu Jun 29 10:13:28 2023, max compression
+gzip compressed data, was "kiara_plugin.service-0.4.4.tar", last modified: Thu Jul 13 10:57:10 2023, max compression
```

## Comparing `kiara_plugin.service-0.4.3.tar` & `kiara_plugin.service-0.4.4.tar`

### file list

```diff
@@ -1,135 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.276420 kiara_plugin.service-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.260420 kiara_plugin.service-0.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.264420 kiara_plugin.service-0.4.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.268420 kiara_plugin.service-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-29 10:13:28.276420 kiara_plugin.service-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.260420 kiara_plugin.service-0.4.3/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.268420 kiara_plugin.service-0.4.3/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/ci/conda/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.268420 kiara_plugin.service-0.4.3/ci/conda/kiara_plugin.service/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/ci/conda/kiara_plugin.service/meta.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.268420 kiara_plugin.service-0.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.268420 kiara_plugin.service-0.4.3/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.260420 kiara_plugin.service-0.4.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.268420 kiara_plugin.service-0.4.3/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.268420 kiara_plugin.service-0.4.3/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.268420 kiara_plugin.service-0.4.3/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/examples/jobs/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.268420 kiara_plugin.service-0.4.3/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/examples/pipelines/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/examples/pipelines/example_pipeline_service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.260420 kiara_plugin.service-0.4.3/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.268420 kiara_plugin.service-0.4.3/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-29 10:13:28.276420 kiara_plugin.service-0.4.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.264420 kiara_plugin.service-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.264420 kiara_plugin.service-0.4.3/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.268420 kiara_plugin.service-0.4.3/src/kiara_plugin/service/
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.268420 kiara_plugin.service-0.4.3/src/kiara_plugin/service/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.268420 kiara_plugin.service-0.4.3/src/kiara_plugin/service/interfaces/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/interfaces/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.272420 kiara_plugin.service-0.4.3/src/kiara_plugin/service/interfaces/cli/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/interfaces/cli/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/interfaces/cli/service/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.272420 kiara_plugin.service-0.4.3/src/kiara_plugin/service/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.272420 kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.272420 kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/controllers/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/controllers/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/controllers/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/controllers/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/controllers/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/controllers/values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/controllers/workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.272420 kiara_plugin.service-0.4.3/src/kiara_plugin/service/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.272420 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.272420 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/static/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/static/input.css
--rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/static/main.css
--rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/static/simple.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.272420 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.272420 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/jobs/job_finished.html
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/jobs/job_monitor.html
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/macros.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.272420 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/operations/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/operations/operation_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/operations/operations.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.272420 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/values/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/values/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.276420 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/values/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/values/inputs/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/values/inputs/boolean.html
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/values/inputs/generic-scalar.html
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/values/inputs/generic.html
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/values/inputs/table.html
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/values/value_inputs_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/values/value_select.html
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/values/value_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/values/values.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.268420 kiara_plugin.service-0.4.3/src/kiara_plugin.service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-29 10:13:28.000000 kiara_plugin.service-0.4.3/src/kiara_plugin.service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-06-29 10:13:28.000000 kiara_plugin.service-0.4.3/src/kiara_plugin.service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 10:13:28.000000 kiara_plugin.service-0.4.3/src/kiara_plugin.service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-29 10:13:28.000000 kiara_plugin.service-0.4.3/src/kiara_plugin.service.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 10:12:59.000000 kiara_plugin.service-0.4.3/src/kiara_plugin.service.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-29 10:13:28.000000 kiara_plugin.service-0.4.3/src/kiara_plugin.service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 10:13:28.000000 kiara_plugin.service-0.4.3/src/kiara_plugin.service.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/tailwind.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.276420 kiara_plugin.service-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:13:28.276420 kiara_plugin.service-0.4.3/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      227 2023-06-29 10:12:45.000000 kiara_plugin.service-0.4.3/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.673514 kiara_plugin.service-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.661514 kiara_plugin.service-0.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-13 10:57:10.673514 kiara_plugin.service-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.661514 kiara_plugin.service-0.4.4/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/ci/conda/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/ci/conda/kiara_plugin.service/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/ci/conda/kiara_plugin.service/meta.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.661514 kiara_plugin.service-0.4.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/examples/jobs/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/examples/pipelines/example_pipeline_service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   171640 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/kiara_import.profile
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.661514 kiara_plugin.service-0.4.4/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.665514 kiara_plugin.service-0.4.4/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-13 10:57:10.673514 kiara_plugin.service-0.4.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.661514 kiara_plugin.service-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.661514 kiara_plugin.service-0.4.4/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/interfaces/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/interfaces/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/interfaces/cli/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/interfaces/cli/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/interfaces/cli/service/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/context_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/static/input.css
+-rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/static/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/static/simple.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.673514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/jobs/job_finished.html
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/jobs/job_monitor.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/macros.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.673514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/operations/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/operations/operation_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/operations/operations.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.673514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.673514 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/inputs/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/inputs/boolean.html
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/inputs/generic-scalar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/inputs/generic.html
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/inputs/table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/value_inputs_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/value_select.html
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/value_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/values.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.669514 kiara_plugin.service-0.4.4/src/kiara_plugin.service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-13 10:57:10.000000 kiara_plugin.service-0.4.4/src/kiara_plugin.service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-13 10:57:10.000000 kiara_plugin.service-0.4.4/src/kiara_plugin.service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:57:10.000000 kiara_plugin.service-0.4.4/src/kiara_plugin.service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-13 10:57:10.000000 kiara_plugin.service-0.4.4/src/kiara_plugin.service.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:56:43.000000 kiara_plugin.service-0.4.4/src/kiara_plugin.service.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-13 10:57:10.000000 kiara_plugin.service-0.4.4/src/kiara_plugin.service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 10:57:10.000000 kiara_plugin.service-0.4.4/src/kiara_plugin.service.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/tailwind.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.673514 kiara_plugin.service-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:10.673514 kiara_plugin.service-0.4.4/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/tests/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      227 2023-07-13 10:56:31.000000 kiara_plugin.service-0.4.4/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.service-0.4.3/.cruft.json` & `kiara_plugin.service-0.4.4/.cruft.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.service-0.4.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.service-0.4.4/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/.github/workflows/build-darwin.yaml` & `kiara_plugin.service-0.4.4/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/.github/workflows/build-linux.yaml` & `kiara_plugin.service-0.4.4/.github/workflows/build-linux.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/.github/workflows/build-windows.yaml` & `kiara_plugin.service-0.4.4/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/.gitignore` & `kiara_plugin.service-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/.pre-commit-config.yaml` & `kiara_plugin.service-0.4.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/LICENSE` & `kiara_plugin.service-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/Makefile` & `kiara_plugin.service-0.4.4/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/PKG-INFO` & `kiara_plugin.service-0.4.4/src/kiara_plugin.service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kiara_plugin.service
-Version: 0.4.3
+Name: kiara-plugin.service
+Version: 0.4.4
 Summary: A plugin to create, run and manage a service for kiara functionality.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.service
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.service
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.service
 Keywords: kiara
```

### Comparing `kiara_plugin.service-0.4.3/README.md` & `kiara_plugin.service-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/ci/conda/kiara_plugin.service/meta.yaml.template` & `kiara_plugin.service-0.4.4/ci/conda/kiara_plugin.service/meta.yaml.template`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/docs/development.md` & `kiara_plugin.service-0.4.4/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/docs/index.md` & `kiara_plugin.service-0.4.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.service-0.4.4/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.service-0.4.4/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/examples/pipelines/example_pipeline_service.yaml` & `kiara_plugin.service-0.4.4/examples/pipelines/example_pipeline_service.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/mkdocs.yml` & `kiara_plugin.service-0.4.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/pyproject.toml` & `kiara_plugin.service-0.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 dependencies = [
-    "kiara>=0.4.44",
+    "kiara>=0.4.47",
     "kiara_plugin.core_types>=0.4.20",
     "uvicorn>=0.22.0",
     "starlite==1.39.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
```

### Comparing `kiara_plugin.service-0.4.3/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.service-0.4.4/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/scripts/documentation/gen_info_pages.py` & `kiara_plugin.service-0.4.4/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/scripts/documentation/gen_module_doc.py` & `kiara_plugin.service-0.4.4/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/setup.cfg` & `kiara_plugin.service-0.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/setup.py` & `kiara_plugin.service-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/__init__.py` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/defaults.py` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/defaults.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/interfaces/cli/service/commands.py` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/interfaces/cli/service/commands.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/models.py` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/modules/__init__.py` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/__init__.py` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/controllers/__init__.py` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/controllers/jobs.py` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/jobs.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/controllers/modules.py` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/modules.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         self, kiara_api: KiaraAPI, data: ModuleMatcher
     ) -> Dict[str, ModuleTypeInfo]:
 
         filters = data.filters
         python_package = data.python_package
 
         module_types = kiara_api.retrieve_module_types_info(
-            *filters, python_package=python_package
+            filter=filters, python_package=python_package
         )
         return module_types.item_infos  # type: ignore
 
     @get(path="/type_names", api_func=KiaraAPI.list_module_type_names)
     async def list_module_type_names(self, kiara_api: KiaraAPI) -> List[str]:
         """List the ids of all available operations."""
```

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/controllers/operations.py` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/operations.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/controllers/pipeline.py` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     @get(path="/structure/{pipeline:str}", api_func=get_pipeline_config)
     async def get_pipeline_structure(
         self, kiara_api: KiaraAPI, pipeline: str
     ) -> PipelineStructureInfo:
 
         print(f"PIPELINE: {pipeline}")
         pipeline_config = get_pipeline_config(pipeline=pipeline)
+        print(pipeline_config)
         info = PipelineStructureInfo.create_from_instance(
             kiara=kiara_api.context, instance=pipeline_config.structure
         )
         return info
 
     @get(path="/list", api_func=get_pipeline_config)
     async def list_pipelines(self, kiara_api: KiaraAPI) -> List[str]:
```

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/controllers/render.py` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/render.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,20 +49,29 @@
             target_format: the render format
             data: (optional) target & data type specific render configuration
 
         Returns:
             the render result
         """
 
-        # filters = ["select_columns", "drop_columns"]
-        filters: List[str] = []
-        v = kiara_api.get_value(value)
-        result = kiara_api.render_value(
-            value=v, target_format=target_format, filters=filters, render_config=data
-        )
+        try:
+            # filters = ["select_columns", "drop_columns"]
+            filters: List[str] = []
+            v = kiara_api.get_value(value)
+            result = kiara_api.render_value(
+                value=v,
+                target_format=target_format,
+                filters=filters,
+                render_config=data,
+            )
+        except Exception as e:
+            import traceback
+
+            traceback.print_exc()
+            raise e
         return result
 
     @post(
         path="/value_info/{value:str}/{target_format:str}",
         summary="Render value info as HTML",
     )
     async def render_operation_info(
```

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/controllers/values.py` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/values.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         matcher_data = data.dict()
 
         result = kiara_api.list_aliases(**matcher_data)
         return result  # type: ignore
 
     @post(path="/aliases_info", api_func=KiaraAPI.retrieve_aliases_info)
     async def list_aliases_info(
-        self, kiara_api: KiaraAPI, data: ValueMatcher
+        self, kiara_api: KiaraAPI, data: Union[ValueMatcher, None]
     ) -> Dict[str, ValueInfo]:
 
         if data is None:
             matcher_data = {}
         else:
             matcher_data = data.dict()
```

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/controllers/workflows.py` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/controllers/workflows.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/openapi/service.py` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/openapi/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,18 @@
 
 from kiara.context import Kiara
 from kiara.interfaces.python_api import KiaraAPI
 from kiara.models import KiaraModel
 from kiara.registries.templates import TemplateRegistry
 from kiara.utils import is_debug, is_develop
 from kiara_plugin.service.defaults import KIARA_SERVICE_RESOURCES_FOLDER
+from kiara_plugin.service.openapi.controllers.context_info import (
+    DataTypeControllerJson,
+    KiaraContextControllerJson,
+)
 from kiara_plugin.service.openapi.controllers.jobs import JobControllerJson
 from kiara_plugin.service.openapi.controllers.modules import ModuleControllerJson
 from kiara_plugin.service.openapi.controllers.operations import (
     OperationControllerJson,
 )
 from kiara_plugin.service.openapi.controllers.pipeline import PipelineControllerJson
 from kiara_plugin.service.openapi.controllers.render import RenderControllerJson
@@ -164,41 +168,49 @@
     def app(self) -> Starlite:
         if self._app is not None:
             return self._app
 
         from starlite import Router
 
         value_router = Router(path="/data", route_handlers=[ValueControllerJson])
-        module_router = Router(path="/modules", route_handlers=[ModuleControllerJson])
         operation_router = Router(
             path="/operations", route_handlers=[OperationControllerJson]
         )
         job_router = Router(path="/jobs", route_handlers=[JobControllerJson])
+        module_router = Router(path="/modules", route_handlers=[ModuleControllerJson])
+        data_type_router = Router(
+            path="/data-types", route_handlers=[DataTypeControllerJson]
+        )
         render_router = Router(path="/render", route_handlers=[RenderControllerJson])
         workflow_router = Router(
             path="/workflows", route_handlers=[WorkflowControllerJson]
         )
         pipeline_router = Router(
             path="/pipelines", route_handlers=[PipelineControllerJson]
         )
+        context_router = Router(
+            path="/context", route_handlers=[KiaraContextControllerJson]
+        )
 
         # info_router_html = Router(
         #     path="/html/info", route_handlers=[OperationControllerHtml]
         # )
         # Router(path="/html/values", route_handlers=[ValueControllerHtmx])
         # Router(path="/html/operations", route_handlers=[OperationControllerHtmx])
 
         route_handlers: List[ControllerRouterHandler] = []
         route_handlers.append(value_router)
         route_handlers.append(module_router)
+        route_handlers.append(data_type_router)
         route_handlers.append(operation_router)
         route_handlers.append(job_router)
         route_handlers.append(render_router)
         route_handlers.append(workflow_router)
         route_handlers.append(pipeline_router)
+        route_handlers.append(context_router)
 
         # route_handlers.append(value_router_htmx)
         # route_handlers.append(operation_router_htmx)
 
         static_dir = self._resources_base / "static"
 
         static_file_config = [
```

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/static/favicon.ico` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/static/main.css` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/static/main.css`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/static/simple.css` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/static/simple.css`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/jobs/job_finished.html` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/jobs/job_finished.html`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/macros.html` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/macros.html`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html` & `kiara_plugin.service-0.4.4/src/kiara_plugin/service/resources/templates/values/inputs/base_scalar.html`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin.service.egg-info/PKG-INFO` & `kiara_plugin.service-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kiara-plugin.service
-Version: 0.4.3
+Name: kiara_plugin.service
+Version: 0.4.4
 Summary: A plugin to create, run and manage a service for kiara functionality.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.service
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.service
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.service
 Keywords: kiara
```

### Comparing `kiara_plugin.service-0.4.3/src/kiara_plugin.service.egg-info/SOURCES.txt` & `kiara_plugin.service-0.4.4/src/kiara_plugin.service.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 AUTHORS.md
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 commitlint.config.js
+kiara_import.profile
 mkdocs.yml
 pyproject.toml
 setup.cfg
 setup.py
 tailwind.config.js
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/suggest-a-module.md
@@ -54,14 +55,15 @@
 src/kiara_plugin/service/interfaces/cli/__init__.py
 src/kiara_plugin/service/interfaces/cli/service/__init__.py
 src/kiara_plugin/service/interfaces/cli/service/commands.py
 src/kiara_plugin/service/modules/__init__.py
 src/kiara_plugin/service/openapi/__init__.py
 src/kiara_plugin/service/openapi/service.py
 src/kiara_plugin/service/openapi/controllers/__init__.py
+src/kiara_plugin/service/openapi/controllers/context_info.py
 src/kiara_plugin/service/openapi/controllers/jobs.py
 src/kiara_plugin/service/openapi/controllers/modules.py
 src/kiara_plugin/service/openapi/controllers/operations.py
 src/kiara_plugin/service/openapi/controllers/pipeline.py
 src/kiara_plugin/service/openapi/controllers/render.py
 src/kiara_plugin/service/openapi/controllers/values.py
 src/kiara_plugin/service/openapi/controllers/workflows.py
```

### Comparing `kiara_plugin.service-0.4.3/tests/conftest.py` & `kiara_plugin.service-0.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.service-0.4.3/tests/test_job_descs.py` & `kiara_plugin.service-0.4.4/tests/test_job_descs.py`

 * *Files identical despite different names*

