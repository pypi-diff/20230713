# Comparing `tmp/orchestrator_core-1.2.2rc2.tar.gz` & `tmp/orchestrator_core-1.2.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchestrator_core-1.2.2rc2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "orchestrator_core-1.2.2rc3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `orchestrator_core-1.2.2rc2.tar` & `orchestrator_core-1.2.2rc3.tar`

### file list

```diff
@@ -1,403 +1,405 @@
--rw-r--r--   0        0        0      342 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/.bumpversion.cfg
--rw-r--r--   0        0        0       33 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/.coveragerc
--rw-r--r--   0        0        0     2620 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/.github/workflows/README.md
--rw-r--r--   0        0        0     1851 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/.github/workflows/build-push-container.yml
--rw-r--r--   0        0        0      291 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/.github/workflows/changelog.yml
--rw-r--r--   0        0        0     2341 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      371 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/.github/workflows/gh-pages.yml
--rw-r--r--   0        0        0      550 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0     1138 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/.github/workflows/run-linting-tests.yml
--rw-r--r--   0        0        0     2113 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/.github/workflows/run-unit-tests.yml
--rw-r--r--   0        0        0     1985 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0     1809 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/.gitignore
--rw-r--r--   0        0        0     1592 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1150 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/.stignore
--rw-r--r--   0        0        0    30087 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/CHANGELOG.md
--rw-r--r--   0        0        0      333 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/Dockerfile
--rw-r--r--   0        0        0    11409 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/LICENSE
--rw-r--r--   0        0        0      150 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/NOTICE
--rw-r--r--   0        0        0     4965 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/README.md
--rw-r--r--   0        0        0       76 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/codecov.yml
--rw-r--r--   0        0        0       45 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/docs/architecture/application/api.md
--rw-r--r--   0        0        0    16572 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/docs/architecture/application/cli.md
--rw-r--r--   0        0        0    10741 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/docs/architecture/application/domainmodels.md
--rw-r--r--   0        0        0    13931 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/docs/architecture/application/forms.md
--rw-r--r--   0        0        0    48867 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/docs/architecture/application/openapi.json
--rw-r--r--   0        0        0     1565 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/docs/architecture/application/python.md
--rw-r--r--   0        0        0     5585 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/docs/architecture/application/scaling.md
--rw-r--r--   0        0        0     5514 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/docs/architecture/application/tasks.md
--rw-r--r--   0        0        0     2371 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/docs/architecture/application/websockets.md
--rw-r--r--   0        0        0    11465 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/docs/architecture/application/workflow.md
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/docs/architecture/orchestration/philosophy.md
--rw-r--r--   0        0        0      668 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/context.md
--rw-r--r--   0        0        0      802 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/introduction.md
--rw-r--r--   0        0        0     1671 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/ip_static.md
--rw-r--r--   0        0        0    84576 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/ip_static.png
--rw-r--r--   0        0        0     1310 2023-07-03 19:39:26.413062 orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/l2_point_to_point.md
--rw-r--r--   0        0        0    55937 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/l2_point_to_point.png
--rw-r--r--   0        0        0      854 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/l2_vpn.md
--rw-r--r--   0        0        0    29551 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/l2_vpn.png
--rw-r--r--   0        0        0     1397 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/modelling.md
--rw-r--r--   0        0        0     1137 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/node.md
--rw-r--r--   0        0        0    23110 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/node.png
--rw-r--r--   0        0        0     1147 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/port.md
--rw-r--r--   0        0        0    37248 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/port.png
--rw-r--r--   0        0        0     1694 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/product_block_graph.md
--rw-r--r--   0        0        0    78824 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/product_block_graph.png
--rw-r--r--   0        0        0      989 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/standards.md
--rw-r--r--   0        0        0     1114 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/terminology.md
--rw-r--r--   0        0        0     2080 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/architecture/tldr.md
--rw-r--r--   0        0        0     1694 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/contributing/guidelines.md
--rw-r--r--   0        0        0    10000 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/contributing/testing.md
--rw-r--r--   0        0        0      452 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/css/custom.css
--rw-r--r--   0        0        0     2165 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/css/termynal.css
--rw-r--r--   0        0        0     2135 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/getting-started/base.md
--rw-r--r--   0        0        0      928 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/getting-started/development.md
--rw-r--r--   0        0        0     2367 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/index.md
--rw-r--r--   0        0        0     3897 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/js/termynal.js
--rw-r--r--   0        0        0     8925 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/advanced/circuit-workflow.md
--rw-r--r--   0        0        0      254 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/advanced/database-migration.md
--rw-r--r--   0        0        0     3776 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/advanced/docker-installation.md
--rw-r--r--   0        0        0     2563 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/advanced/domain-models.md
--rw-r--r--   0        0        0     4126 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/advanced/node-workflow.md
--rw-r--r--   0        0        0     3079 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/advanced/overview.md
--rw-r--r--   0        0        0     1750 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/advanced/scenario.md
--rw-r--r--   0        0        0     4369 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/advanced/workflow-introduction.md
--rw-r--r--   0        0        0     5605 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/beginner/create-user-group.md
--rw-r--r--   0        0        0     4438 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/beginner/create-user.md
--rw-r--r--   0        0        0     7471 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/beginner/database-migration.md
--rw-r--r--   0        0        0     3700 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/beginner/debian.md
--rw-r--r--   0        0        0     3063 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/beginner/docker.md
--rw-r--r--   0        0        0     6106 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/beginner/domain-models.md
--rw-r--r--   0        0        0     1952 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/beginner/explore.md
--rw-r--r--   0        0        0     3996 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/beginner/input-forms.md
--rw-r--r--   0        0        0     3595 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/beginner/macos.md
--rw-r--r--   0        0        0     3411 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/beginner/modify-user-group.md
--rw-r--r--   0        0        0     2143 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/beginner/modify-user.md
--rw-r--r--   0        0        0     2885 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/beginner/overview.md
--rw-r--r--   0        0        0     4547 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/beginner/register-workflows.md
--rw-r--r--   0        0        0      786 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/beginner/scenario.md
--rw-r--r--   0        0        0     1013 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/beginner/start-applications.md
--rw-r--r--   0        0        0     2988 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/beginner/terminate-user-group.md
--rw-r--r--   0        0        0     1332 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/beginner/terminate-user.md
--rw-r--r--   0        0        0     3637 2023-07-03 19:39:26.417062 orchestrator_core-1.2.2rc2/docs/workshops/beginner/workflow-introduction.md
--rw-r--r--   0        0        0    46296 2023-07-03 19:39:26.421062 orchestrator_core-1.2.2rc2/docs/workshops/images/metadata_products.png
--rw-r--r--   0        0        0   983304 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/docs/workshops/images/netbox_devices_active.png
--rw-r--r--   0        0        0      771 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/examples/basic/basic_orchestrator.py
--rw-r--r--   0        0        0     4990 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/mkdocs.yml
--rw-r--r--   0        0        0     1262 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/mutmut_config.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/orchestrator/.stignore
--rw-r--r--   0        0        0     1098 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/orchestrator/__init__.py
--rw-r--r--   0        0        0      571 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/orchestrator/api/__init__.py
--rw-r--r--   0        0        0      571 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/__init__.py
--rw-r--r--   0        0        0     2967 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/api.py
--rw-r--r--   0        0        0      571 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/__init__.py
--rw-r--r--   0        0        0     2855 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/fixed_input.py
--rw-r--r--   0        0        0     1236 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/health.py
--rw-r--r--   0        0        0    12981 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/processes.py
--rw-r--r--   0        0        0     2703 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/product_blocks.py
--rw-r--r--   0        0        0     3331 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/products.py
--rw-r--r--   0        0        0     2552 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/resource_types.py
--rw-r--r--   0        0        0     5801 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/settings.py
--rw-r--r--   0        0        0     2866 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
--rw-r--r--   0        0        0    11648 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/subscriptions.py
--rw-r--r--   0        0        0      961 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/translations.py
--rw-r--r--   0        0        0     1833 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/user.py
--rw-r--r--   0        0        0     1961 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/workflows.py
--rw-r--r--   0        0        0     1543 2023-07-03 19:39:26.425062 orchestrator_core-1.2.2rc2/orchestrator/api/error_handling.py
--rw-r--r--   0        0        0    11719 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/api/helpers.py
--rw-r--r--   0        0        0     5617 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/api/models.py
--rw-r--r--   0        0        0     7557 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/app.py
--rw-r--r--   0        0        0      571 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/__init__.py
--rw-r--r--   0        0        0    13845 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/database.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/domain_gen_helpers/__init__.py
--rw-r--r--   0        0        0     6837 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
--rw-r--r--   0        0        0     1953 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/domain_gen_helpers/helpers.py
--rw-r--r--   0        0        0    10635 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
--rw-r--r--   0        0        0     9409 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/domain_gen_helpers/product_helpers.py
--rw-r--r--   0        0        0    24055 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
--rw-r--r--   0        0        0     1435 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/domain_gen_helpers/types.py
--rw-r--r--   0        0        0     2371 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generate.md
--rw-r--r--   0        0        0     5168 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generate.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/__init__.py
--rw-r--r--   0        0        0     1744 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/fixed_input.py
--rw-r--r--   0        0        0     2626 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/helpers.py
--rw-r--r--   0        0        0     2607 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/migration.py
--rw-r--r--   0        0        0     2152 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/product.py
--rw-r--r--   0        0        0     5793 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/product_block.py
--rw-r--r--   0        0        0     1400 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/settings.py
--rw-r--r--   0        0        0     1794 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/translations.py
--rw-r--r--   0        0        0     4234 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/unittest.py
--rw-r--r--   0        0        0     1957 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/validations.py
--rw-r--r--   0        0        0     6535 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/workflow.py
--rw-r--r--   0        0        0      779 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/products/workshop/circuit.yaml
--rw-r--r--   0        0        0      557 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/products/workshop/node.yaml
--rw-r--r--   0        0        0      553 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/products/workshop/user.yaml
--rw-r--r--   0        0        0      380 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/products/workshop/user_group.yaml
--rw-r--r--   0        0        0      289 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/constrained_int_definitions.j2
--rw-r--r--   0        0        0     4196 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/create_product.j2
--rw-r--r--   0        0        0      337 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/list_definitions.j2
--rw-r--r--   0        0        0      520 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/macros.j2
--rw-r--r--   0        0        0     4405 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/modify_product.j2
--rw-r--r--   0        0        0     2639 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/new_product_migration.j2
--rw-r--r--   0        0        0     1675 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/product.j2
--rw-r--r--   0        0        0     2275 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/product_block.j2
--rw-r--r--   0        0        0      514 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/shared_forms.j2
--rw-r--r--   0        0        0     2808 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/terminate_product.j2
--rw-r--r--   0        0        0     1764 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/test_create_workflow.j2
--rw-r--r--   0        0        0     1689 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/test_modify_workflow.j2
--rw-r--r--   0        0        0     1860 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/test_product_type.j2
--rw-r--r--   0        0        0     1518 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/test_terminate_workflow.j2
--rw-r--r--   0        0        0      984 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/test_validate_workflow.j2
--rw-r--r--   0        0        0     2391 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/validate_product.j2
--rw-r--r--   0        0        0      571 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/helpers/__init__.py
--rw-r--r--   0        0        0     1165 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/helpers/input_helpers.py
--rw-r--r--   0        0        0      830 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/helpers/print_helpers.py
--rw-r--r--   0        0        0      983 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/main.py
--rwxr-xr-x   0        0        0    20258 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/migrate_domain_models.py
--rwxr-xr-x   0        0        0     8929 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/migrate_workflows.py
--rw-r--r--   0        0        0     4093 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/migration_helpers.py
--rw-r--r--   0        0        0     1896 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/cli/scheduler.py
--rw-r--r--   0        0        0      571 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/config/__init__.py
--rw-r--r--   0        0        0      770 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/config/assignee.py
--rw-r--r--   0        0        0     2981 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/db/__init__.py
--rw-r--r--   0        0        0    10201 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/db/database.py
--rw-r--r--   0        0        0      303 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/db/filters/__init__.py
--rw-r--r--   0        0        0     3618 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/db/filters/filters.py
--rw-r--r--   0        0        0      774 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/db/filters/generic_filters/__init__.py
--rw-r--r--   0        0        0      992 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/db/filters/generic_filters/bool_filter.py
--rw-r--r--   0        0        0      952 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/db/filters/generic_filters/is_like_filter.py
--rw-r--r--   0        0        0     2542 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/db/filters/generic_filters/range_filter.py
--rw-r--r--   0        0        0      993 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/db/filters/generic_filters/values_in_column_filter.py
--rw-r--r--   0        0        0     3592 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/db/filters/process.py
--rw-r--r--   0        0        0     1251 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/db/filters/product.py
--rw-r--r--   0        0        0     3203 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/db/filters/subscription.py
--rw-r--r--   0        0        0    23604 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/db/models.py
--rw-r--r--   0        0        0      104 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/db/range/__init__.py
--rw-r--r--   0        0        0     1433 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/db/range/range.py
--rw-r--r--   0        0        0      419 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/db/sorting/__init__.py
--rw-r--r--   0        0        0      603 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/db/sorting/process.py
--rw-r--r--   0        0        0      418 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/db/sorting/product.py
--rw-r--r--   0        0        0     4367 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/db/sorting/sorting.py
--rw-r--r--   0        0        0      606 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/db/sorting/subscription.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.429062 orchestrator_core-1.2.2rc2/orchestrator/devtools/__init__.py
--rw-r--r--   0        0        0    16814 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/devtools/populator.py
--rw-r--r--   0        0        0     2513 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/distlock/__init__.py
--rw-r--r--   0        0        0     2533 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/distlock/distlock_manager.py
--rw-r--r--   0        0        0      571 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/distlock/managers/__init__.py
--rw-r--r--   0        0        0     3062 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/distlock/managers/memory_distlock_manager.py
--rw-r--r--   0        0        0     3298 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/distlock/managers/redis_distlock_manager.py
--rw-r--r--   0        0        0      924 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/domain/__init__.py
--rw-r--r--   0        0        0    62898 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/domain/base.py
--rw-r--r--   0        0        0     2694 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/domain/lifecycle.py
--rw-r--r--   0        0        0     2908 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/exception_handlers.py
--rw-r--r--   0        0        0     5418 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/forms/__init__.py
--rw-r--r--   0        0        0     2145 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/forms/network_type_validators.py
--rw-r--r--   0        0        0    11483 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/forms/validators.py
--rw-r--r--   0        0        0     5373 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/extensions/__init__.py
--rw-r--r--   0        0        0     4311 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/extensions/deprecation_checker_extension.py
--rw-r--r--   0        0        0     1777 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/extensions/error_collector_extension.py
--rw-r--r--   0        0        0     2334 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/pagination.py
--rw-r--r--   0        0        0      420 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/resolvers/__init__.py
--rw-r--r--   0        0        0     3674 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/resolvers/process.py
--rw-r--r--   0        0        0     2154 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/resolvers/product.py
--rw-r--r--   0        0        0     3727 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/resolvers/settings.py
--rw-r--r--   0        0        0     2907 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/resolvers/subscription.py
--rw-r--r--   0        0        0      203 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/schemas/errors.py
--rw-r--r--   0        0        0      513 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/schemas/fixed_input.py
--rw-r--r--   0        0        0     3674 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/schemas/process.py
--rw-r--r--   0        0        0     1776 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/schemas/product.py
--rw-r--r--   0        0        0      530 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/schemas/product_block.py
--rw-r--r--   0        0        0      305 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/schemas/resource_type.py
--rw-r--r--   0        0        0      980 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/schemas/settings.py
--rw-r--r--   0        0        0     7736 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/schemas/subscription.py
--rw-r--r--   0        0        0      172 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/schemas/workflow.py
--rw-r--r--   0        0        0     1789 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/types.py
--rw-r--r--   0        0        0      114 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/utils/__init__.py
--rw-r--r--   0        0        0     1071 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/utils/create_resolver_error_handler.py
--rw-r--r--   0        0        0      990 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/graphql/utils/get_selected_fields.py
--rw-r--r--   0        0        0       39 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/migrations/README
--rw-r--r--   0        0        0      873 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/migrations/alembic.ini
--rwxr-xr-x   0        0        0     3365 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/migrations/env.py
--rw-r--r--   0        0        0    40411 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/migrations/helpers.py
--rw-r--r--   0        0        0      510 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/migrations/script.py.mako
--rw-r--r--   0        0        0      905 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/migrations/templates/alembic.ini.j2
--rwxr-xr-x   0        0        0     2821 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/migrations/templates/env.py.j2
--rw-r--r--   0        0        0       98 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/migrations/templates/helpers.py.j2
--rw-r--r--   0        0        0     2641 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
--rw-r--r--   0        0        0     1266 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
--rw-r--r--   0        0        0    38591 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
--rw-r--r--   0        0        0      951 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
--rw-r--r--   0        0        0     1213 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
--rw-r--r--   0        0        0     1556 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
--rw-r--r--   0        0        0     5105 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
--rw-r--r--   0        0        0     7723 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
--rw-r--r--   0        0        0      989 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/py.typed
--rw-r--r--   0        0        0     1090 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/schedules/__init__.py
--rw-r--r--   0        0        0      832 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/schedules/resume_workflows.py
--rw-r--r--   0        0        0     1535 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/schedules/scheduling.py
--rw-r--r--   0        0        0      821 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/schedules/task_vacuum.py
--rw-r--r--   0        0        0     1053 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/schedules/validate_products.py
--rw-r--r--   0        0        0     2131 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/schedules/validate_subscriptions.py
--rw-r--r--   0        0        0     2631 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/schemas/__init__.py
--rw-r--r--   0        0        0      886 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/schemas/base.py
--rw-r--r--   0        0        0     1293 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/schemas/engine_settings.py
--rw-r--r--   0        0        0     1346 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/schemas/fixed_input.py
--rw-r--r--   0        0        0      842 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/schemas/problem_detail.py
--rw-r--r--   0        0        0     3404 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/schemas/process.py
--rw-r--r--   0        0        0     1670 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/schemas/product.py
--rw-r--r--   0        0        0     1735 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/schemas/product_block.py
--rw-r--r--   0        0        0      951 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/schemas/resource_type.py
--rw-r--r--   0        0        0     3180 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/schemas/subscription.py
--rw-r--r--   0        0        0     1013 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/schemas/subscription_descriptions.py
--rw-r--r--   0        0        0     1803 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/schemas/workflow.py
--rw-r--r--   0        0        0     1797 2023-07-03 19:39:26.433062 orchestrator_core-1.2.2rc2/orchestrator/security.py
--rw-r--r--   0        0        0      571 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/services/__init__.py
--rw-r--r--   0        0        0     3586 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/services/celery.py
--rw-r--r--   0        0        0    22606 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/services/processes.py
--rw-r--r--   0        0        0     1525 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/services/products.py
--rw-r--r--   0        0        0     3927 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/services/settings.py
--rw-r--r--   0        0        0    24397 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/services/subscriptions.py
--rw-r--r--   0        0        0     5716 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/services/tasks.py
--rw-r--r--   0        0        0     1719 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/services/translations.py
--rw-r--r--   0        0        0     3190 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/settings.py
--rw-r--r--   0        0        0      766 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/targets.py
--rw-r--r--   0        0        0     9427 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/types.py
--rw-r--r--   0        0        0      571 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/utils/__init__.py
--rw-r--r--   0        0        0     5593 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/utils/crypt.py
--rw-r--r--   0        0        0     1477 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/utils/datetime.py
--rw-r--r--   0        0        0     6206 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/utils/docs.py
--rw-r--r--   0        0        0     4315 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/utils/errors.py
--rw-r--r--   0        0        0     8079 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/utils/functional.py
--rw-r--r--   0        0        0     2751 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/utils/helpers.py
--rw-r--r--   0        0        0     8489 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/utils/json.py
--rw-r--r--   0        0        0     3340 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/utils/redis.py
--rw-r--r--   0        0        0     2972 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/utils/show_process.py
--rw-r--r--   0        0        0     2395 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/utils/speed.py
--rw-r--r--   0        0        0    13057 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/utils/state.py
--rw-r--r--   0        0        0     1077 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/utils/strings.py
--rw-r--r--   0        0        0     7240 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/utils/vlans.py
--rw-r--r--   0        0        0     1318 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/version.py
--rw-r--r--   0        0        0     4476 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/websocket/__init__.py
--rw-r--r--   0        0        0     3535 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/websocket/managers/broadcast_websocket_manager.py
--rw-r--r--   0        0        0     3312 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/websocket/managers/memory_websocket_manager.py
--rw-r--r--   0        0        0     2900 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/websocket/websocket_manager.py
--rw-r--r--   0        0        0    33502 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/workflow.py
--rw-r--r--   0        0        0     4085 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2135 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/workflows/modify_note.py
--rw-r--r--   0        0        0      909 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/workflows/removed_workflow.py
--rw-r--r--   0        0        0     9185 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/workflows/steps.py
--rw-r--r--   0        0        0      571 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     1510 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/workflows/tasks/cleanup_tasks_log.py
--rw-r--r--   0        0        0     2120 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/workflows/tasks/resume_workflows.py
--rw-r--r--   0        0        0     8375 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/workflows/tasks/validate_products.py
--rw-r--r--   0        0        0      684 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/workflows/translations/en-GB.json
--rw-r--r--   0        0        0    12830 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/orchestrator/workflows/utils.py
--rw-r--r--   0        0        0     4873 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/pyproject.toml
--rw-r--r--   0        0        0     1940 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/setup.cfg
--rw-r--r--   0        0        0      665 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/setup.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/acceptance_tests/__init__.py
--rw-r--r--   0        0        0     3199 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/acceptance_tests/conftest.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
--rw-r--r--   0        0        0     1855 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
--rw-r--r--   0        0        0     1544 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/main.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
--rw-r--r--   0        0        0     1608 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
--rw-r--r--   0        0        0     1210 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2828 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
--rw-r--r--   0        0        0      588 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/acceptance_tests/test_test_product.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/unit_tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/unit_tests/api/__init__.py
--rw-r--r--   0        0        0     5159 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/unit_tests/api/test_caching.py
--rw-r--r--   0        0        0     1578 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/unit_tests/api/test_fixed_inputs.py
--rw-r--r--   0        0        0     1192 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/unit_tests/api/test_health.py
--rw-r--r--   0        0        0     3049 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/unit_tests/api/test_helpers.py
--rw-r--r--   0        0        0     1747 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/unit_tests/api/test_models.py
--rw-r--r--   0        0        0    19964 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/unit_tests/api/test_processes.py
--rw-r--r--   0        0        0    15454 2023-07-03 19:39:26.437062 orchestrator_core-1.2.2rc2/test/unit_tests/api/test_processes_ws.py
--rw-r--r--   0        0        0     3742 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/api/test_product_blocks.py
--rw-r--r--   0        0        0     7942 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/api/test_products.py
--rw-r--r--   0        0        0     2486 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/api/test_resource_types.py
--rw-r--r--   0        0        0     1772 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/api/test_settings.py
--rw-r--r--   0        0        0     2985 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/api/test_subscription_customer_descriptions.py
--rw-r--r--   0        0        0    37706 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/api/test_subscriptions.py
--rw-r--r--   0        0        0     2367 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/api/test_workflows.py
--rw-r--r--   0        0        0    25724 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
--rw-r--r--   0        0        0    27170 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
--rw-r--r--   0        0        0      511 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/config.py
--rw-r--r--   0        0        0    22634 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/conftest.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/domain/__init__.py
--rw-r--r--   0        0        0    50537 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/domain/test_base.py
--rw-r--r--   0        0        0     8092 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/domain/test_base_with_list_union.py
--rw-r--r--   0        0        0     4493 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/domain/test_base_with_union.py
--rw-r--r--   0        0        0     2845 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/__init__.py
--rw-r--r--   0        0        0     7530 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/processes.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_blocks/__init__.py
--rw-r--r--   0        0        0     1683 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
--rw-r--r--   0        0        0     2569 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
--rw-r--r--   0        0        0     1609 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
--rw-r--r--   0        0        0     2642 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
--rw-r--r--   0        0        0     2590 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
--rw-r--r--   0        0        0     1232 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
--rw-r--r--   0        0        0     1055 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/__init__.py
--rw-r--r--   0        0        0     2372 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
--rw-r--r--   0        0        0     2262 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
--rw-r--r--   0        0        0     4191 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
--rw-r--r--   0        0        0     3240 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_one.py
--rw-r--r--   0        0        0     2341 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
--rw-r--r--   0        0        0     2977 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
--rw-r--r--   0        0        0     2298 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
--rw-r--r--   0        0        0     2282 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
--rw-r--r--   0        0        0     1671 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
--rw-r--r--   0        0        0     1898 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_union.py
--rw-r--r--   0        0        0      527 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/resource_types.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/forms/__init__.py
--rw-r--r--   0        0        0     1462 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/forms/shared.py
--rw-r--r--   0        0        0    25426 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/forms/test_generic_validators.py
--rw-r--r--   0        0        0     7644 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/forms/test_network_validators.py
--rw-r--r--   0        0        0     6626 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/forms/test_post_process.py
--rw-r--r--   0        0        0    11107 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/graphql/test_processes.py
--rw-r--r--   0        0        0     7301 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/graphql/test_product.py
--rw-r--r--   0        0        0     5174 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/graphql/test_settings.py
--rw-r--r--   0        0        0    23655 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/graphql/test_subscriptions.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/schedules/__init__.py
--rw-r--r--   0        0        0      807 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/schedules/test_scheduling.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/services/__init__.py
--rw-r--r--   0        0        0    26695 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/services/test_processes.py
--rw-r--r--   0        0        0     1083 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/services/test_products.py
--rw-r--r--   0        0        0     5830 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/services/test_subscriptions.py
--rw-r--r--   0        0        0     2100 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/services/test_translations.py
--rw-r--r--   0        0        0     7353 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/test_db.py
--rw-r--r--   0        0        0      385 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/test_types.py
--rw-r--r--   0        0        0    12029 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/test_workflow.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/utils/__init__.py
--rw-r--r--   0        0        0      163 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/utils/test_datetime.py
--rw-r--r--   0        0        0     1891 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/utils/test_errors.py
--rw-r--r--   0        0        0     3517 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/utils/test_functional.py
--rw-r--r--   0        0        0     3052 2023-07-03 19:39:26.441062 orchestrator_core-1.2.2rc2/test/unit_tests/utils/test_json.py
--rw-r--r--   0        0        0     1144 2023-07-03 19:39:26.445062 orchestrator_core-1.2.2rc2/test/unit_tests/utils/test_speed.py
--rw-r--r--   0        0        0    11501 2023-07-03 19:39:26.445062 orchestrator_core-1.2.2rc2/test/unit_tests/utils/test_state.py
--rw-r--r--   0        0        0      192 2023-07-03 19:39:26.445062 orchestrator_core-1.2.2rc2/test/unit_tests/utils/test_strings.py
--rw-r--r--   0        0        0     8339 2023-07-03 19:39:26.445062 orchestrator_core-1.2.2rc2/test/unit_tests/utils/test_vlans.py
--rw-r--r--   0        0        0    12493 2023-07-03 19:39:26.445062 orchestrator_core-1.2.2rc2/test/unit_tests/workflows/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.445062 orchestrator_core-1.2.2rc2/test/unit_tests/workflows/conftest.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.445062 orchestrator_core-1.2.2rc2/test/unit_tests/workflows/shared/__init__.py
--rw-r--r--   0        0        0     2091 2023-07-03 19:39:26.445062 orchestrator_core-1.2.2rc2/test/unit_tests/workflows/shared/test_validate_subscriptions.py
--rw-r--r--   0        0        0        0 2023-07-03 19:39:26.445062 orchestrator_core-1.2.2rc2/test/unit_tests/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     2039 2023-07-03 19:39:26.445062 orchestrator_core-1.2.2rc2/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
--rw-r--r--   0        0        0     2584 2023-07-03 19:39:26.445062 orchestrator_core-1.2.2rc2/test/unit_tests/workflows/tasks/test_resume_workflows.py
--rw-r--r--   0        0        0      288 2023-07-03 19:39:26.445062 orchestrator_core-1.2.2rc2/test/unit_tests/workflows/tasks/test_validate_products.py
--rw-r--r--   0        0        0     3390 2023-07-03 19:39:26.445062 orchestrator_core-1.2.2rc2/test/unit_tests/workflows/test_config_db_code.py
--rw-r--r--   0        0        0     1877 2023-07-03 19:39:26.445062 orchestrator_core-1.2.2rc2/test/unit_tests/workflows/test_generic_workflow_steps.py
--rw-r--r--   0        0        0      987 2023-07-03 19:39:26.445062 orchestrator_core-1.2.2rc2/test/unit_tests/workflows/test_modify_note.py
--rw-r--r--   0        0        0     4353 1970-01-01 00:00:00.000000 orchestrator_core-1.2.2rc2/PKG-INFO
+-rw-r--r--   0        0        0      342 2023-07-05 09:25:09.948931 orchestrator_core-1.2.2rc3/.bumpversion.cfg
+-rw-r--r--   0        0        0       33 2023-07-05 09:25:09.948931 orchestrator_core-1.2.2rc3/.coveragerc
+-rw-r--r--   0        0        0     2620 2023-07-05 09:25:09.948931 orchestrator_core-1.2.2rc3/.github/workflows/README.md
+-rw-r--r--   0        0        0     1851 2023-07-05 09:25:09.948931 orchestrator_core-1.2.2rc3/.github/workflows/build-push-container.yml
+-rw-r--r--   0        0        0      291 2023-07-05 09:25:09.948931 orchestrator_core-1.2.2rc3/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0     2341 2023-07-05 09:25:09.948931 orchestrator_core-1.2.2rc3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      371 2023-07-05 09:25:09.948931 orchestrator_core-1.2.2rc3/.github/workflows/gh-pages.yml
+-rw-r--r--   0        0        0      550 2023-07-05 09:25:09.948931 orchestrator_core-1.2.2rc3/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0     1138 2023-07-05 09:25:09.948931 orchestrator_core-1.2.2rc3/.github/workflows/run-linting-tests.yml
+-rw-r--r--   0        0        0     2113 2023-07-05 09:25:09.948931 orchestrator_core-1.2.2rc3/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0        0        0     1985 2023-07-05 09:25:09.948931 orchestrator_core-1.2.2rc3/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0     1809 2023-07-05 09:25:09.948931 orchestrator_core-1.2.2rc3/.gitignore
+-rw-r--r--   0        0        0     1815 2023-07-05 09:25:09.948931 orchestrator_core-1.2.2rc3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1150 2023-07-05 09:25:09.948931 orchestrator_core-1.2.2rc3/.stignore
+-rw-r--r--   0        0        0    30087 2023-07-05 09:25:09.948931 orchestrator_core-1.2.2rc3/CHANGELOG.md
+-rw-r--r--   0        0        0      333 2023-07-05 09:25:09.948931 orchestrator_core-1.2.2rc3/Dockerfile
+-rw-r--r--   0        0        0    11409 2023-07-05 09:25:09.948931 orchestrator_core-1.2.2rc3/LICENSE
+-rw-r--r--   0        0        0      150 2023-07-05 09:25:09.948931 orchestrator_core-1.2.2rc3/NOTICE
+-rw-r--r--   0        0        0     4965 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/README.md
+-rw-r--r--   0        0        0       76 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/codecov.yml
+-rw-r--r--   0        0        0       45 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/application/api.md
+-rw-r--r--   0        0        0    16572 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/application/cli.md
+-rw-r--r--   0        0        0    10741 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/application/domainmodels.md
+-rw-r--r--   0        0        0    13931 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/application/forms.md
+-rw-r--r--   0        0        0    48867 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/application/openapi.json
+-rw-r--r--   0        0        0     1565 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/application/python.md
+-rw-r--r--   0        0        0     5585 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/application/scaling.md
+-rw-r--r--   0        0        0     5514 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/application/tasks.md
+-rw-r--r--   0        0        0     2371 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/application/websockets.md
+-rw-r--r--   0        0        0    11465 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/application/workflow.md
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/orchestration/philosophy.md
+-rw-r--r--   0        0        0      668 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/context.md
+-rw-r--r--   0        0        0      802 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/introduction.md
+-rw-r--r--   0        0        0     1671 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/ip_static.md
+-rw-r--r--   0        0        0    84576 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/ip_static.png
+-rw-r--r--   0        0        0     1310 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/l2_point_to_point.md
+-rw-r--r--   0        0        0    55937 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/l2_point_to_point.png
+-rw-r--r--   0        0        0      854 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/l2_vpn.md
+-rw-r--r--   0        0        0    29551 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/l2_vpn.png
+-rw-r--r--   0        0        0     1397 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/modelling.md
+-rw-r--r--   0        0        0     1137 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/node.md
+-rw-r--r--   0        0        0    23110 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/node.png
+-rw-r--r--   0        0        0     1147 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/port.md
+-rw-r--r--   0        0        0    37248 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/port.png
+-rw-r--r--   0        0        0     1694 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/product_block_graph.md
+-rw-r--r--   0        0        0    78824 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/product_block_graph.png
+-rw-r--r--   0        0        0      989 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/standards.md
+-rw-r--r--   0        0        0     1114 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/terminology.md
+-rw-r--r--   0        0        0     2080 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/architecture/tldr.md
+-rw-r--r--   0        0        0     1694 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/contributing/guidelines.md
+-rw-r--r--   0        0        0    10000 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/contributing/testing.md
+-rw-r--r--   0        0        0      452 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/css/custom.css
+-rw-r--r--   0        0        0     2165 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/css/termynal.css
+-rw-r--r--   0        0        0     2135 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/getting-started/base.md
+-rw-r--r--   0        0        0      928 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/getting-started/development.md
+-rw-r--r--   0        0        0     2367 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/index.md
+-rw-r--r--   0        0        0     3897 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/js/termynal.js
+-rw-r--r--   0        0        0     8925 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/workshops/advanced/circuit-workflow.md
+-rw-r--r--   0        0        0      254 2023-07-05 09:25:09.952931 orchestrator_core-1.2.2rc3/docs/workshops/advanced/database-migration.md
+-rw-r--r--   0        0        0     3776 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/advanced/docker-installation.md
+-rw-r--r--   0        0        0     2563 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/advanced/domain-models.md
+-rw-r--r--   0        0        0     4126 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/advanced/node-workflow.md
+-rw-r--r--   0        0        0     3079 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/advanced/overview.md
+-rw-r--r--   0        0        0     1750 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/advanced/scenario.md
+-rw-r--r--   0        0        0     4369 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/advanced/workflow-introduction.md
+-rw-r--r--   0        0        0     5605 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/beginner/create-user-group.md
+-rw-r--r--   0        0        0     4438 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/beginner/create-user.md
+-rw-r--r--   0        0        0     7471 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/beginner/database-migration.md
+-rw-r--r--   0        0        0     3700 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/beginner/debian.md
+-rw-r--r--   0        0        0     3063 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/beginner/docker.md
+-rw-r--r--   0        0        0     6106 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/beginner/domain-models.md
+-rw-r--r--   0        0        0     1952 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/beginner/explore.md
+-rw-r--r--   0        0        0     3996 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/beginner/input-forms.md
+-rw-r--r--   0        0        0     3595 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/beginner/macos.md
+-rw-r--r--   0        0        0     3411 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/beginner/modify-user-group.md
+-rw-r--r--   0        0        0     2143 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/beginner/modify-user.md
+-rw-r--r--   0        0        0     2885 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/beginner/overview.md
+-rw-r--r--   0        0        0     4547 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/beginner/register-workflows.md
+-rw-r--r--   0        0        0      786 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/beginner/scenario.md
+-rw-r--r--   0        0        0     1013 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/beginner/start-applications.md
+-rw-r--r--   0        0        0     2988 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/beginner/terminate-user-group.md
+-rw-r--r--   0        0        0     1332 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/beginner/terminate-user.md
+-rw-r--r--   0        0        0     3637 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/beginner/workflow-introduction.md
+-rw-r--r--   0        0        0    46296 2023-07-05 09:25:09.956931 orchestrator_core-1.2.2rc3/docs/workshops/images/metadata_products.png
+-rw-r--r--   0        0        0   983304 2023-07-05 09:25:09.960932 orchestrator_core-1.2.2rc3/docs/workshops/images/netbox_devices_active.png
+-rw-r--r--   0        0        0      771 2023-07-05 09:25:09.960932 orchestrator_core-1.2.2rc3/examples/basic/basic_orchestrator.py
+-rw-r--r--   0        0        0     4990 2023-07-05 09:25:09.960932 orchestrator_core-1.2.2rc3/mkdocs.yml
+-rw-r--r--   0        0        0     1262 2023-07-05 09:25:09.960932 orchestrator_core-1.2.2rc3/mutmut_config.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.960932 orchestrator_core-1.2.2rc3/orchestrator/.stignore
+-rw-r--r--   0        0        0     1098 2023-07-05 09:25:09.960932 orchestrator_core-1.2.2rc3/orchestrator/__init__.py
+-rw-r--r--   0        0        0      571 2023-07-05 09:25:09.960932 orchestrator_core-1.2.2rc3/orchestrator/api/__init__.py
+-rw-r--r--   0        0        0      571 2023-07-05 09:25:09.960932 orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/__init__.py
+-rw-r--r--   0        0        0     2967 2023-07-05 09:25:09.960932 orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/api.py
+-rw-r--r--   0        0        0      571 2023-07-05 09:25:09.960932 orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/__init__.py
+-rw-r--r--   0        0        0     2855 2023-07-05 09:25:09.960932 orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/fixed_input.py
+-rw-r--r--   0        0        0     1236 2023-07-05 09:25:09.960932 orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/health.py
+-rw-r--r--   0        0        0    12981 2023-07-05 09:25:09.960932 orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/processes.py
+-rw-r--r--   0        0        0     2703 2023-07-05 09:25:09.960932 orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/product_blocks.py
+-rw-r--r--   0        0        0     3331 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/products.py
+-rw-r--r--   0        0        0     2552 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/resource_types.py
+-rw-r--r--   0        0        0     5801 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/settings.py
+-rw-r--r--   0        0        0     2866 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    11648 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/subscriptions.py
+-rw-r--r--   0        0        0      961 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/translations.py
+-rw-r--r--   0        0        0     1833 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/user.py
+-rw-r--r--   0        0        0     1961 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/workflows.py
+-rw-r--r--   0        0        0     1543 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/api/error_handling.py
+-rw-r--r--   0        0        0    11719 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/api/helpers.py
+-rw-r--r--   0        0        0     5617 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/api/models.py
+-rw-r--r--   0        0        0     7557 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/app.py
+-rw-r--r--   0        0        0      571 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/__init__.py
+-rw-r--r--   0        0        0    13845 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/database.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/domain_gen_helpers/__init__.py
+-rw-r--r--   0        0        0     6837 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
+-rw-r--r--   0        0        0     1953 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/domain_gen_helpers/helpers.py
+-rw-r--r--   0        0        0    10635 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
+-rw-r--r--   0        0        0     9409 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/domain_gen_helpers/product_helpers.py
+-rw-r--r--   0        0        0    24055 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
+-rw-r--r--   0        0        0     1435 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/domain_gen_helpers/types.py
+-rw-r--r--   0        0        0     2371 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generate.md
+-rw-r--r--   0        0        0     5168 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generate.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/__init__.py
+-rw-r--r--   0        0        0     1744 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/fixed_input.py
+-rw-r--r--   0        0        0     2626 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/helpers.py
+-rw-r--r--   0        0        0     2607 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/migration.py
+-rw-r--r--   0        0        0     2152 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/product.py
+-rw-r--r--   0        0        0     5793 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/product_block.py
+-rw-r--r--   0        0        0     1400 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/settings.py
+-rw-r--r--   0        0        0     1794 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/translations.py
+-rw-r--r--   0        0        0     4234 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/unittest.py
+-rw-r--r--   0        0        0     1957 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/validations.py
+-rw-r--r--   0        0        0     6535 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/workflow.py
+-rw-r--r--   0        0        0      779 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/products/workshop/circuit.yaml
+-rw-r--r--   0        0        0      557 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/products/workshop/node.yaml
+-rw-r--r--   0        0        0      553 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/products/workshop/user.yaml
+-rw-r--r--   0        0        0      380 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/products/workshop/user_group.yaml
+-rw-r--r--   0        0        0      289 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/constrained_int_definitions.j2
+-rw-r--r--   0        0        0     4196 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/create_product.j2
+-rw-r--r--   0        0        0      337 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/list_definitions.j2
+-rw-r--r--   0        0        0      520 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/macros.j2
+-rw-r--r--   0        0        0     4405 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/modify_product.j2
+-rw-r--r--   0        0        0     2639 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/new_product_migration.j2
+-rw-r--r--   0        0        0     1675 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/product.j2
+-rw-r--r--   0        0        0     2275 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/product_block.j2
+-rw-r--r--   0        0        0      514 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/shared_forms.j2
+-rw-r--r--   0        0        0     2808 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/terminate_product.j2
+-rw-r--r--   0        0        0     1764 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/test_create_workflow.j2
+-rw-r--r--   0        0        0     1689 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/test_modify_workflow.j2
+-rw-r--r--   0        0        0     1860 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/test_product_type.j2
+-rw-r--r--   0        0        0     1518 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/test_terminate_workflow.j2
+-rw-r--r--   0        0        0      984 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/test_validate_workflow.j2
+-rw-r--r--   0        0        0     2391 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/validate_product.j2
+-rw-r--r--   0        0        0      571 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/helpers/__init__.py
+-rw-r--r--   0        0        0     1165 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/helpers/input_helpers.py
+-rw-r--r--   0        0        0      830 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/helpers/print_helpers.py
+-rw-r--r--   0        0        0      983 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/main.py
+-rwxr-xr-x   0        0        0    20258 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/migrate_domain_models.py
+-rwxr-xr-x   0        0        0     8929 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/migrate_workflows.py
+-rw-r--r--   0        0        0     4093 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/migration_helpers.py
+-rw-r--r--   0        0        0     1896 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/cli/scheduler.py
+-rw-r--r--   0        0        0      571 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/config/__init__.py
+-rw-r--r--   0        0        0      770 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/config/assignee.py
+-rw-r--r--   0        0        0     2981 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/db/__init__.py
+-rw-r--r--   0        0        0    10201 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/db/database.py
+-rw-r--r--   0        0        0      303 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/db/filters/__init__.py
+-rw-r--r--   0        0        0     3618 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/db/filters/filters.py
+-rw-r--r--   0        0        0      774 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/db/filters/generic_filters/__init__.py
+-rw-r--r--   0        0        0      992 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/db/filters/generic_filters/bool_filter.py
+-rw-r--r--   0        0        0      952 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/db/filters/generic_filters/is_like_filter.py
+-rw-r--r--   0        0        0     2542 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/db/filters/generic_filters/range_filter.py
+-rw-r--r--   0        0        0      993 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/db/filters/generic_filters/values_in_column_filter.py
+-rw-r--r--   0        0        0     3592 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/db/filters/process.py
+-rw-r--r--   0        0        0     1251 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/db/filters/product.py
+-rw-r--r--   0        0        0     3203 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/db/filters/subscription.py
+-rw-r--r--   0        0        0    23604 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/db/models.py
+-rw-r--r--   0        0        0      104 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/db/range/__init__.py
+-rw-r--r--   0        0        0     1433 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/db/range/range.py
+-rw-r--r--   0        0        0      419 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/db/sorting/__init__.py
+-rw-r--r--   0        0        0      603 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/db/sorting/process.py
+-rw-r--r--   0        0        0      418 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/db/sorting/product.py
+-rw-r--r--   0        0        0     4367 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/db/sorting/sorting.py
+-rw-r--r--   0        0        0      606 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/db/sorting/subscription.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/devtools/__init__.py
+-rw-r--r--   0        0        0    16814 2023-07-05 09:25:09.964932 orchestrator_core-1.2.2rc3/orchestrator/devtools/populator.py
+-rw-r--r--   0        0        0     2513 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/distlock/__init__.py
+-rw-r--r--   0        0        0     2533 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/distlock/distlock_manager.py
+-rw-r--r--   0        0        0      571 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/distlock/managers/__init__.py
+-rw-r--r--   0        0        0     3062 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/distlock/managers/memory_distlock_manager.py
+-rw-r--r--   0        0        0     3298 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/distlock/managers/redis_distlock_manager.py
+-rw-r--r--   0        0        0      924 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/domain/__init__.py
+-rw-r--r--   0        0        0    62898 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/domain/base.py
+-rw-r--r--   0        0        0     2694 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/domain/lifecycle.py
+-rw-r--r--   0        0        0     2908 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/exception_handlers.py
+-rw-r--r--   0        0        0     5418 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/forms/__init__.py
+-rw-r--r--   0        0        0     2145 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/forms/network_type_validators.py
+-rw-r--r--   0        0        0    11483 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/forms/validators.py
+-rw-r--r--   0        0        0     5361 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/extensions/__init__.py
+-rw-r--r--   0        0        0     4311 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/extensions/deprecation_checker_extension.py
+-rw-r--r--   0        0        0     1777 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/extensions/error_collector_extension.py
+-rw-r--r--   0        0        0     2334 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/pagination.py
+-rw-r--r--   0        0        0      420 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/resolvers/__init__.py
+-rw-r--r--   0        0        0     3674 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/resolvers/process.py
+-rw-r--r--   0        0        0     2154 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/resolvers/product.py
+-rw-r--r--   0        0        0     3715 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/resolvers/settings.py
+-rw-r--r--   0        0        0     2907 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/resolvers/subscription.py
+-rw-r--r--   0        0        0      203 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/schemas/errors.py
+-rw-r--r--   0        0        0      513 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/schemas/fixed_input.py
+-rw-r--r--   0        0        0     3662 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/schemas/process.py
+-rw-r--r--   0        0        0     1764 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/schemas/product.py
+-rw-r--r--   0        0        0      530 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/schemas/product_block.py
+-rw-r--r--   0        0        0      305 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/schemas/resource_type.py
+-rw-r--r--   0        0        0      980 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/schemas/settings.py
+-rw-r--r--   0        0        0     7724 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/schemas/subscription.py
+-rw-r--r--   0        0        0      172 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/schemas/workflow.py
+-rw-r--r--   0        0        0     1789 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/types.py
+-rw-r--r--   0        0        0      114 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/utils/__init__.py
+-rw-r--r--   0        0        0     1071 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/utils/create_resolver_error_handler.py
+-rw-r--r--   0        0        0      990 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/graphql/utils/get_selected_fields.py
+-rw-r--r--   0        0        0       39 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/migrations/README
+-rw-r--r--   0        0        0      873 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/migrations/alembic.ini
+-rwxr-xr-x   0        0        0     3365 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/migrations/env.py
+-rw-r--r--   0        0        0    40411 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/migrations/helpers.py
+-rw-r--r--   0        0        0      510 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/migrations/script.py.mako
+-rw-r--r--   0        0        0      905 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/migrations/templates/alembic.ini.j2
+-rwxr-xr-x   0        0        0     2821 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/migrations/templates/env.py.j2
+-rw-r--r--   0        0        0       98 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/migrations/templates/helpers.py.j2
+-rw-r--r--   0        0        0     2641 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
+-rw-r--r--   0        0        0     1266 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
+-rw-r--r--   0        0        0    38591 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
+-rw-r--r--   0        0        0      951 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
+-rw-r--r--   0        0        0     1213 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
+-rw-r--r--   0        0        0     1556 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
+-rw-r--r--   0        0        0     5105 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
+-rw-r--r--   0        0        0     7723 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
+-rw-r--r--   0        0        0      989 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py
+-rw-r--r--   0        0        0      556 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py
+-rw-r--r--   0        0        0      755 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/py.typed
+-rw-r--r--   0        0        0     1090 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/schedules/__init__.py
+-rw-r--r--   0        0        0      832 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/schedules/resume_workflows.py
+-rw-r--r--   0        0        0     1535 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/schedules/scheduling.py
+-rw-r--r--   0        0        0      821 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/schedules/task_vacuum.py
+-rw-r--r--   0        0        0     1053 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/schedules/validate_products.py
+-rw-r--r--   0        0        0     2131 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/schedules/validate_subscriptions.py
+-rw-r--r--   0        0        0     2631 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/schemas/__init__.py
+-rw-r--r--   0        0        0      886 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/schemas/base.py
+-rw-r--r--   0        0        0     1293 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/schemas/engine_settings.py
+-rw-r--r--   0        0        0     1346 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/schemas/fixed_input.py
+-rw-r--r--   0        0        0      842 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/schemas/problem_detail.py
+-rw-r--r--   0        0        0     3404 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/schemas/process.py
+-rw-r--r--   0        0        0     1670 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/schemas/product.py
+-rw-r--r--   0        0        0     1735 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/schemas/product_block.py
+-rw-r--r--   0        0        0      951 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/schemas/resource_type.py
+-rw-r--r--   0        0        0     3180 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/schemas/subscription.py
+-rw-r--r--   0        0        0     1013 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/schemas/subscription_descriptions.py
+-rw-r--r--   0        0        0     1803 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/schemas/workflow.py
+-rw-r--r--   0        0        0     1863 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/security.py
+-rw-r--r--   0        0        0      571 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/services/__init__.py
+-rw-r--r--   0        0        0     3586 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/services/celery.py
+-rw-r--r--   0        0        0    22606 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/services/processes.py
+-rw-r--r--   0        0        0     1525 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/services/products.py
+-rw-r--r--   0        0        0     3927 2023-07-05 09:25:09.968932 orchestrator_core-1.2.2rc3/orchestrator/services/settings.py
+-rw-r--r--   0        0        0    24397 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/services/subscriptions.py
+-rw-r--r--   0        0        0     5716 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/services/tasks.py
+-rw-r--r--   0        0        0     1719 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/services/translations.py
+-rw-r--r--   0        0        0     3403 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/settings.py
+-rw-r--r--   0        0        0      766 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/targets.py
+-rw-r--r--   0        0        0     9427 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/types.py
+-rw-r--r--   0        0        0      571 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/utils/__init__.py
+-rw-r--r--   0        0        0     5593 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/utils/crypt.py
+-rw-r--r--   0        0        0     1477 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/utils/datetime.py
+-rw-r--r--   0        0        0     6206 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/utils/docs.py
+-rw-r--r--   0        0        0     4315 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/utils/errors.py
+-rw-r--r--   0        0        0     8079 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/utils/functional.py
+-rw-r--r--   0        0        0     2751 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/utils/helpers.py
+-rw-r--r--   0        0        0     8489 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/utils/json.py
+-rw-r--r--   0        0        0     3340 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/utils/redis.py
+-rw-r--r--   0        0        0     2972 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/utils/show_process.py
+-rw-r--r--   0        0        0     2395 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/utils/speed.py
+-rw-r--r--   0        0        0    13057 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/utils/state.py
+-rw-r--r--   0        0        0     1077 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/utils/strings.py
+-rw-r--r--   0        0        0     7240 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/utils/vlans.py
+-rw-r--r--   0        0        0     1318 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/version.py
+-rw-r--r--   0        0        0     4476 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/websocket/__init__.py
+-rw-r--r--   0        0        0     3535 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/websocket/managers/broadcast_websocket_manager.py
+-rw-r--r--   0        0        0     3312 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/websocket/managers/memory_websocket_manager.py
+-rw-r--r--   0        0        0     2900 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/websocket/websocket_manager.py
+-rw-r--r--   0        0        0    33502 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/workflow.py
+-rw-r--r--   0        0        0     4085 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2135 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/workflows/modify_note.py
+-rw-r--r--   0        0        0      909 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/workflows/removed_workflow.py
+-rw-r--r--   0        0        0     9185 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/workflows/steps.py
+-rw-r--r--   0        0        0      571 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     1510 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/workflows/tasks/cleanup_tasks_log.py
+-rw-r--r--   0        0        0     2120 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/workflows/tasks/resume_workflows.py
+-rw-r--r--   0        0        0     8375 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/workflows/tasks/validate_products.py
+-rw-r--r--   0        0        0      684 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/workflows/translations/en-GB.json
+-rw-r--r--   0        0        0    12830 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/orchestrator/workflows/utils.py
+-rw-r--r--   0        0        0     4880 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/pyproject.toml
+-rw-r--r--   0        0        0     1940 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/setup.cfg
+-rw-r--r--   0        0        0      665 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/setup.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/acceptance_tests/__init__.py
+-rw-r--r--   0        0        0     3199 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/acceptance_tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
+-rw-r--r--   0        0        0     1855 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
+-rw-r--r--   0        0        0     1544 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/acceptance_tests/fixtures/test_orchestrator/main.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1608 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
+-rw-r--r--   0        0        0     1210 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2828 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
+-rw-r--r--   0        0        0      588 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/acceptance_tests/test_test_product.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/api/__init__.py
+-rw-r--r--   0        0        0     5159 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/api/test_caching.py
+-rw-r--r--   0        0        0     1578 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/api/test_fixed_inputs.py
+-rw-r--r--   0        0        0     1192 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/api/test_health.py
+-rw-r--r--   0        0        0     3049 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/api/test_helpers.py
+-rw-r--r--   0        0        0     1747 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/api/test_models.py
+-rw-r--r--   0        0        0    19964 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/api/test_processes.py
+-rw-r--r--   0        0        0    15454 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/api/test_processes_ws.py
+-rw-r--r--   0        0        0     3742 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/api/test_product_blocks.py
+-rw-r--r--   0        0        0     7942 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/api/test_products.py
+-rw-r--r--   0        0        0     2486 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/api/test_resource_types.py
+-rw-r--r--   0        0        0     1772 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/api/test_settings.py
+-rw-r--r--   0        0        0     2985 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/api/test_subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    37706 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/api/test_subscriptions.py
+-rw-r--r--   0        0        0     2367 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/api/test_workflows.py
+-rw-r--r--   0        0        0    25724 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
+-rw-r--r--   0        0        0    27170 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
+-rw-r--r--   0        0        0      511 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/config.py
+-rw-r--r--   0        0        0    22634 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.972932 orchestrator_core-1.2.2rc3/test/unit_tests/domain/__init__.py
+-rw-r--r--   0        0        0    50537 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/domain/test_base.py
+-rw-r--r--   0        0        0     8092 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/domain/test_base_with_list_union.py
+-rw-r--r--   0        0        0     4493 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/domain/test_base_with_union.py
+-rw-r--r--   0        0        0     2845 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     7530 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/processes.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1683 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
+-rw-r--r--   0        0        0     2569 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
+-rw-r--r--   0        0        0     1609 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
+-rw-r--r--   0        0        0     2642 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
+-rw-r--r--   0        0        0     2590 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
+-rw-r--r--   0        0        0     1232 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
+-rw-r--r--   0        0        0     1055 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/__init__.py
+-rw-r--r--   0        0        0     2372 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
+-rw-r--r--   0        0        0     2262 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
+-rw-r--r--   0        0        0     4191 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
+-rw-r--r--   0        0        0     3240 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/product_type_one.py
+-rw-r--r--   0        0        0     2341 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
+-rw-r--r--   0        0        0     2977 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
+-rw-r--r--   0        0        0     2298 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
+-rw-r--r--   0        0        0     2282 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
+-rw-r--r--   0        0        0     1671 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
+-rw-r--r--   0        0        0     1898 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/product_type_union.py
+-rw-r--r--   0        0        0      527 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/resource_types.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/forms/__init__.py
+-rw-r--r--   0        0        0     1462 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/forms/shared.py
+-rw-r--r--   0        0        0    25426 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/forms/test_generic_validators.py
+-rw-r--r--   0        0        0     7644 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/forms/test_network_validators.py
+-rw-r--r--   0        0        0     6626 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/forms/test_post_process.py
+-rw-r--r--   0        0        0    11107 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/graphql/test_processes.py
+-rw-r--r--   0        0        0     7301 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/graphql/test_product.py
+-rw-r--r--   0        0        0     5174 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/graphql/test_settings.py
+-rw-r--r--   0        0        0    23655 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/graphql/test_subscriptions.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/schedules/__init__.py
+-rw-r--r--   0        0        0      807 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/schedules/test_scheduling.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/services/__init__.py
+-rw-r--r--   0        0        0    26695 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/services/test_processes.py
+-rw-r--r--   0        0        0     1083 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/services/test_products.py
+-rw-r--r--   0        0        0     5830 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/services/test_subscriptions.py
+-rw-r--r--   0        0        0     2100 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/services/test_translations.py
+-rw-r--r--   0        0        0     7353 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/test_db.py
+-rw-r--r--   0        0        0      385 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/test_types.py
+-rw-r--r--   0        0        0    12029 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/test_workflow.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/utils/__init__.py
+-rw-r--r--   0        0        0      163 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/utils/test_datetime.py
+-rw-r--r--   0        0        0     1891 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/utils/test_errors.py
+-rw-r--r--   0        0        0     3517 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/utils/test_functional.py
+-rw-r--r--   0        0        0     3052 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/utils/test_json.py
+-rw-r--r--   0        0        0     1144 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/utils/test_speed.py
+-rw-r--r--   0        0        0    11501 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/utils/test_state.py
+-rw-r--r--   0        0        0      192 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/utils/test_strings.py
+-rw-r--r--   0        0        0     8339 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/utils/test_vlans.py
+-rw-r--r--   0        0        0    12493 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/workflows/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/workflows/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/workflows/shared/__init__.py
+-rw-r--r--   0        0        0     2091 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/workflows/shared/test_validate_subscriptions.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     2039 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
+-rw-r--r--   0        0        0     2584 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/workflows/tasks/test_resume_workflows.py
+-rw-r--r--   0        0        0      288 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/workflows/tasks/test_validate_products.py
+-rw-r--r--   0        0        0     3390 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/workflows/test_config_db_code.py
+-rw-r--r--   0        0        0     1877 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/workflows/test_generic_workflow_steps.py
+-rw-r--r--   0        0        0      987 2023-07-05 09:25:09.976932 orchestrator_core-1.2.2rc3/test/unit_tests/workflows/test_modify_note.py
+-rw-r--r--   0        0        0     4360 1970-01-01 00:00:00.000000 orchestrator_core-1.2.2rc3/PKG-INFO
```

### Comparing `orchestrator_core-1.2.2rc2/.github/workflows/README.md` & `orchestrator_core-1.2.2rc3/.github/workflows/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/.github/workflows/build-push-container.yml` & `orchestrator_core-1.2.2rc3/.github/workflows/build-push-container.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/.github/workflows/codeql-analysis.yml` & `orchestrator_core-1.2.2rc3/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/.github/workflows/publish-package.yml` & `orchestrator_core-1.2.2rc3/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/.github/workflows/run-linting-tests.yml` & `orchestrator_core-1.2.2rc3/.github/workflows/run-linting-tests.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/.github/workflows/run-unit-tests.yml` & `orchestrator_core-1.2.2rc3/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/.github/workflows/scheduled-build.yml` & `orchestrator_core-1.2.2rc3/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/.gitignore` & `orchestrator_core-1.2.2rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/.pre-commit-config.yaml` & `orchestrator_core-1.2.2rc3/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -2,35 +2,42 @@
   python: python3
 repos:
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/asottile/blacken-docs
-    rev: 1.13.0
+    rev: 1.14.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==23.1.0]
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    # Ruff version.
+    rev: v0.0.275
+    hooks:
+      - id: ruff
+        args: [ --fix, --exit-non-zero-on-fix, --show-fixes ]
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: trailing-whitespace
+        exclude: .bumpversion.cfg
       - id: end-of-file-fixer
       - id: check-docstring-first
       - id: check-json
       - id: check-yaml
       - id: debug-statements
       - id: requirements-txt-fixer
       - id: detect-private-key
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.4.1
     hooks:
       - id: mypy
         additional_dependencies:
-          - pydantic
+          - pydantic<2.0.0
           - types-toml
           - types-pytz
           - types-python-dateutil
           - types-requests
           - types-Deprecated
           - types-redis
           - types-orjson
@@ -45,14 +52,14 @@
     rev: v1.10.0
     hooks:
       - id: python-check-blanket-noqa
       - id: python-use-type-annotations
       - id: python-check-mock-methods
       - id: rst-backticks
   - repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: v0.9.0.2
+    rev: v0.9.0.5
     hooks:
       - id: shellcheck
   - repo: https://github.com/andreoliwa/nitpick
-    rev: v0.33.1
+    rev: v0.33.2
     hooks:
       - id: nitpick-check
```

### Comparing `orchestrator_core-1.2.2rc2/.stignore` & `orchestrator_core-1.2.2rc3/.stignore`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/CHANGELOG.md` & `orchestrator_core-1.2.2rc3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/LICENSE` & `orchestrator_core-1.2.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/README.md` & `orchestrator_core-1.2.2rc3/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/application/cli.md` & `orchestrator_core-1.2.2rc3/docs/architecture/application/cli.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/application/domainmodels.md` & `orchestrator_core-1.2.2rc3/docs/architecture/application/domainmodels.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/application/forms.md` & `orchestrator_core-1.2.2rc3/docs/architecture/application/forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/application/openapi.json` & `orchestrator_core-1.2.2rc3/docs/architecture/application/openapi.json`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/application/python.md` & `orchestrator_core-1.2.2rc3/docs/architecture/application/python.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/application/scaling.md` & `orchestrator_core-1.2.2rc3/docs/architecture/application/scaling.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/application/tasks.md` & `orchestrator_core-1.2.2rc3/docs/architecture/application/tasks.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/application/websockets.md` & `orchestrator_core-1.2.2rc3/docs/architecture/application/websockets.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/application/workflow.md` & `orchestrator_core-1.2.2rc3/docs/architecture/application/workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/context.md` & `orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/context.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/introduction.md` & `orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/ip_static.md` & `orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/ip_static.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/ip_static.png` & `orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/ip_static.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/l2_point_to_point.md` & `orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/l2_point_to_point.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/l2_point_to_point.png` & `orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/l2_point_to_point.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/l2_vpn.md` & `orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/l2_vpn.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/l2_vpn.png` & `orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/l2_vpn.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/modelling.md` & `orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/modelling.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/node.md` & `orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/node.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/node.png` & `orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/node.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/port.md` & `orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/port.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/port.png` & `orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/port.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/product_block_graph.md` & `orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/product_block_graph.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/product_block_graph.png` & `orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/product_block_graph.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/standards.md` & `orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/standards.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/product_modelling/terminology.md` & `orchestrator_core-1.2.2rc3/docs/architecture/product_modelling/terminology.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/architecture/tldr.md` & `orchestrator_core-1.2.2rc3/docs/architecture/tldr.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/contributing/guidelines.md` & `orchestrator_core-1.2.2rc3/docs/contributing/guidelines.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/contributing/testing.md` & `orchestrator_core-1.2.2rc3/docs/contributing/testing.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/css/termynal.css` & `orchestrator_core-1.2.2rc3/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/getting-started/base.md` & `orchestrator_core-1.2.2rc3/docs/getting-started/base.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/getting-started/development.md` & `orchestrator_core-1.2.2rc3/docs/getting-started/development.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/index.md` & `orchestrator_core-1.2.2rc3/docs/index.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/js/custom.js` & `orchestrator_core-1.2.2rc3/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/js/termynal.js` & `orchestrator_core-1.2.2rc3/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/advanced/circuit-workflow.md` & `orchestrator_core-1.2.2rc3/docs/workshops/advanced/circuit-workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/advanced/docker-installation.md` & `orchestrator_core-1.2.2rc3/docs/workshops/advanced/docker-installation.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/advanced/domain-models.md` & `orchestrator_core-1.2.2rc3/docs/workshops/advanced/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/advanced/node-workflow.md` & `orchestrator_core-1.2.2rc3/docs/workshops/advanced/node-workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/advanced/overview.md` & `orchestrator_core-1.2.2rc3/docs/workshops/advanced/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/advanced/scenario.md` & `orchestrator_core-1.2.2rc3/docs/workshops/advanced/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/advanced/workflow-introduction.md` & `orchestrator_core-1.2.2rc3/docs/workshops/advanced/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/beginner/create-user-group.md` & `orchestrator_core-1.2.2rc3/docs/workshops/beginner/create-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/beginner/create-user.md` & `orchestrator_core-1.2.2rc3/docs/workshops/beginner/create-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/beginner/database-migration.md` & `orchestrator_core-1.2.2rc3/docs/workshops/beginner/database-migration.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/beginner/debian.md` & `orchestrator_core-1.2.2rc3/docs/workshops/beginner/debian.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/beginner/docker.md` & `orchestrator_core-1.2.2rc3/docs/workshops/beginner/docker.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/beginner/domain-models.md` & `orchestrator_core-1.2.2rc3/docs/workshops/beginner/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/beginner/explore.md` & `orchestrator_core-1.2.2rc3/docs/workshops/beginner/explore.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/beginner/input-forms.md` & `orchestrator_core-1.2.2rc3/docs/workshops/beginner/input-forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/beginner/macos.md` & `orchestrator_core-1.2.2rc3/docs/workshops/beginner/macos.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/beginner/modify-user-group.md` & `orchestrator_core-1.2.2rc3/docs/workshops/beginner/modify-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/beginner/modify-user.md` & `orchestrator_core-1.2.2rc3/docs/workshops/beginner/modify-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/beginner/overview.md` & `orchestrator_core-1.2.2rc3/docs/workshops/beginner/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/beginner/register-workflows.md` & `orchestrator_core-1.2.2rc3/docs/workshops/beginner/register-workflows.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/beginner/scenario.md` & `orchestrator_core-1.2.2rc3/docs/workshops/beginner/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/beginner/start-applications.md` & `orchestrator_core-1.2.2rc3/docs/workshops/beginner/start-applications.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/beginner/terminate-user-group.md` & `orchestrator_core-1.2.2rc3/docs/workshops/beginner/terminate-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/beginner/terminate-user.md` & `orchestrator_core-1.2.2rc3/docs/workshops/beginner/terminate-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/beginner/workflow-introduction.md` & `orchestrator_core-1.2.2rc3/docs/workshops/beginner/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/images/metadata_products.png` & `orchestrator_core-1.2.2rc3/docs/workshops/images/metadata_products.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/docs/workshops/images/netbox_devices_active.png` & `orchestrator_core-1.2.2rc3/docs/workshops/images/netbox_devices_active.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/examples/basic/basic_orchestrator.py` & `orchestrator_core-1.2.2rc3/examples/basic/basic_orchestrator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/mkdocs.yml` & `orchestrator_core-1.2.2rc3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/mutmut_config.py` & `orchestrator_core-1.2.2rc3/mutmut_config.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This is the orchestrator workflow engine."""
 
-__version__ = "1.2.2rc2"
+__version__ = "1.2.2rc3"
 
 from orchestrator.app import OrchestratorCore
 from orchestrator.settings import app_settings, oauth2_settings
 from orchestrator.workflow import begin, conditional, done, focussteps, inputstep, retrystep, step, steplens, workflow
 
 __all__ = [
     "OrchestratorCore",
```

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/api/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/api/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/api.py` & `orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/api.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/fixed_input.py` & `orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/health.py` & `orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/processes.py` & `orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/processes.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 import structlog
 from fastapi import Request
 from fastapi.param_functions import Body, Depends, Header
 from fastapi.routing import APIRouter
 from fastapi.websockets import WebSocket
 from fastapi_etag.dependency import CacheHit
 from more_itertools import chunked
-from oauth2_lib.fastapi import OIDCUserModel
 from sqlalchemy.orm import contains_eager, defer, joinedload
 from sqlalchemy.sql import expression
 from sqlalchemy.sql.functions import count
 from starlette.responses import Response
 
+from oauth2_lib.fastapi import OIDCUserModel
 from orchestrator.api.error_handling import raise_status
 from orchestrator.api.helpers import VALID_SORT_KEYS, enrich_process
 from orchestrator.config.assignee import Assignee
 from orchestrator.db import EngineSettingsTable, ProcessSubscriptionTable, ProcessTable, SubscriptionTable, db
 from orchestrator.db.filters import Filter
 from orchestrator.db.filters.process import filter_processes
 from orchestrator.schemas import (
```

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/product_blocks.py` & `orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/products.py` & `orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/resource_types.py` & `orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/settings.py` & `orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/settings.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 from http import HTTPStatus
 from typing import Optional, Union
 
 import structlog
 from fastapi import Query, WebSocket
 from fastapi.param_functions import Depends
 from fastapi.routing import APIRouter
-from oauth2_lib.fastapi import OIDCUserModel
 from redis.asyncio import Redis as AIORedis
 
+from oauth2_lib.fastapi import OIDCUserModel
 from orchestrator.api.error_handling import raise_status
 from orchestrator.db import EngineSettingsTable
 from orchestrator.schemas import EngineSettingsBaseSchema, EngineSettingsSchema, GlobalStatusEnum, WorkerStatus
 from orchestrator.security import oidc_user
 from orchestrator.services import settings
 from orchestrator.services.processes import SYSTEM_USER, ThreadPoolWorkerStatus
 from orchestrator.settings import ExecutorType, app_settings
```

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py` & `orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/subscriptions.py` & `orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/subscriptions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 from typing import Any, Dict, List, Optional, Union
 from uuid import UUID
 
 import structlog
 from fastapi import Depends
 from fastapi.param_functions import Body
 from fastapi.routing import APIRouter
-from oauth2_lib.fastapi import OIDCUserModel
 from sqlalchemy import select
 from sqlalchemy.orm import contains_eager, defer, joinedload
 from starlette.exceptions import HTTPException
 from starlette.requests import Request
 from starlette.responses import Response
 
+from oauth2_lib.fastapi import OIDCUserModel
 from orchestrator.api.error_handling import raise_status
 from orchestrator.api.helpers import _query_with_filters
 from orchestrator.db import (
     ProcessStepTable,
     ProcessSubscriptionTable,
     ProcessTable,
     SubscriptionInstanceTable,
```

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/translations.py` & `orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/user.py` & `orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/api/api_v1/endpoints/workflows.py` & `orchestrator_core-1.2.2rc3/orchestrator/api/api_v1/endpoints/workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/api/error_handling.py` & `orchestrator_core-1.2.2rc3/orchestrator/api/error_handling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/api/helpers.py` & `orchestrator_core-1.2.2rc3/orchestrator/api/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/api/models.py` & `orchestrator_core-1.2.2rc3/orchestrator/api/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/app.py` & `orchestrator_core-1.2.2rc3/orchestrator/app.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/database.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/domain_gen_helpers/helpers.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/domain_gen_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/domain_gen_helpers/product_block_helpers.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/domain_gen_helpers/product_block_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/domain_gen_helpers/product_helpers.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/domain_gen_helpers/product_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/domain_gen_helpers/types.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/domain_gen_helpers/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generate.md` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generate.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generate.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generate.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/fixed_input.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/helpers.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/migration.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/product.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/product_block.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/settings.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/translations.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/unittest.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/unittest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/validations.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/validations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/generator/workflow.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/generator/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/products/workshop/circuit.yaml` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/products/workshop/circuit.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/products/workshop/node.yaml` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/products/workshop/node.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/products/workshop/user.yaml` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/products/workshop/user.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/create_product.j2` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/create_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/macros.j2` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/macros.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/modify_product.j2` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/modify_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/new_product_migration.j2` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/new_product_migration.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/product.j2` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/product_block.j2` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/product_block.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/shared_forms.j2` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/shared_forms.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/terminate_product.j2` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/terminate_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/test_create_workflow.j2` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/test_create_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/test_modify_workflow.j2` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/test_modify_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/test_product_type.j2` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/test_product_type.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/test_terminate_workflow.j2` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/test_terminate_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/test_validate_workflow.j2` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/test_validate_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/generator/templates/validate_product.j2` & `orchestrator_core-1.2.2rc3/orchestrator/cli/generator/templates/validate_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/helpers/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/helpers/input_helpers.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/helpers/input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/helpers/print_helpers.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/helpers/print_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/main.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/migrate_domain_models.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/migrate_domain_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/migrate_workflows.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/migrate_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/migration_helpers.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/migration_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/cli/scheduler.py` & `orchestrator_core-1.2.2rc3/orchestrator/cli/scheduler.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/config/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/config/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/config/assignee.py` & `orchestrator_core-1.2.2rc3/orchestrator/config/assignee.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/db/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/db/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/db/database.py` & `orchestrator_core-1.2.2rc3/orchestrator/db/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/db/filters/filters.py` & `orchestrator_core-1.2.2rc3/orchestrator/db/filters/filters.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/db/filters/generic_filters/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/db/filters/generic_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/db/filters/generic_filters/bool_filter.py` & `orchestrator_core-1.2.2rc3/orchestrator/db/filters/generic_filters/bool_filter.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/db/filters/generic_filters/is_like_filter.py` & `orchestrator_core-1.2.2rc3/orchestrator/db/filters/generic_filters/is_like_filter.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/db/filters/generic_filters/range_filter.py` & `orchestrator_core-1.2.2rc3/orchestrator/db/filters/generic_filters/range_filter.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/db/filters/generic_filters/values_in_column_filter.py` & `orchestrator_core-1.2.2rc3/orchestrator/db/filters/generic_filters/values_in_column_filter.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/db/filters/process.py` & `orchestrator_core-1.2.2rc3/orchestrator/db/filters/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/db/filters/product.py` & `orchestrator_core-1.2.2rc3/orchestrator/db/filters/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/db/filters/subscription.py` & `orchestrator_core-1.2.2rc3/orchestrator/db/filters/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/db/models.py` & `orchestrator_core-1.2.2rc3/orchestrator/db/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/db/range/range.py` & `orchestrator_core-1.2.2rc3/orchestrator/db/range/range.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/db/sorting/process.py` & `orchestrator_core-1.2.2rc3/orchestrator/db/sorting/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/db/sorting/sorting.py` & `orchestrator_core-1.2.2rc3/orchestrator/db/sorting/sorting.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/db/sorting/subscription.py` & `orchestrator_core-1.2.2rc3/orchestrator/db/sorting/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/devtools/populator.py` & `orchestrator_core-1.2.2rc3/orchestrator/devtools/populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/distlock/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/distlock/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/distlock/distlock_manager.py` & `orchestrator_core-1.2.2rc3/orchestrator/distlock/distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/distlock/managers/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/distlock/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/distlock/managers/memory_distlock_manager.py` & `orchestrator_core-1.2.2rc3/orchestrator/distlock/managers/memory_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/distlock/managers/redis_distlock_manager.py` & `orchestrator_core-1.2.2rc3/orchestrator/distlock/managers/redis_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/domain/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/domain/base.py` & `orchestrator_core-1.2.2rc3/orchestrator/domain/base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/domain/lifecycle.py` & `orchestrator_core-1.2.2rc3/orchestrator/domain/lifecycle.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/exception_handlers.py` & `orchestrator_core-1.2.2rc3/orchestrator/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/forms/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/forms/network_type_validators.py` & `orchestrator_core-1.2.2rc3/orchestrator/forms/network_type_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/forms/validators.py` & `orchestrator_core-1.2.2rc3/orchestrator/forms/validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/graphql/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/graphql/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 import strawberry
 import structlog
 from fastapi import Depends
 from fastapi.routing import APIRouter
 from graphql import GraphQLError, GraphQLFormattedError
 from graphql.error.graphql_error import format_error
 from httpx import HTTPStatusError
-from oauth2_lib.graphql_authentication import authenticated_field
 from starlette.requests import Request
 from strawberry.fastapi import GraphQLRouter
 from strawberry.http import GraphQLHTTPResponse
 from strawberry.tools import merge_types
 from strawberry.types import ExecutionContext, ExecutionResult
 from strawberry.utils.logging import StrawberryLogger
 
+from oauth2_lib.strawberry import authenticated_field
 from orchestrator.graphql.extensions.deprecation_checker_extension import make_deprecation_checker_extension
 from orchestrator.graphql.extensions.error_collector_extension import ErrorCollectorExtension
 from orchestrator.graphql.pagination import Connection
 from orchestrator.graphql.resolvers import (
     SettingsMutation,
     resolve_processes,
     resolve_products,
```

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/graphql/extensions/deprecation_checker_extension.py` & `orchestrator_core-1.2.2rc3/orchestrator/graphql/extensions/deprecation_checker_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/graphql/extensions/error_collector_extension.py` & `orchestrator_core-1.2.2rc3/orchestrator/graphql/extensions/error_collector_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/graphql/pagination.py` & `orchestrator_core-1.2.2rc3/orchestrator/graphql/pagination.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/graphql/resolvers/process.py` & `orchestrator_core-1.2.2rc3/orchestrator/graphql/resolvers/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/graphql/resolvers/product.py` & `orchestrator_core-1.2.2rc3/orchestrator/graphql/resolvers/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/graphql/resolvers/settings.py` & `orchestrator_core-1.2.2rc3/orchestrator/graphql/resolvers/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union
 
 import strawberry
 import structlog
-from oauth2_lib.graphql_authentication import authenticated_mutation_field
 from redis.asyncio import Redis as AIORedis
 
+from oauth2_lib.strawberry import authenticated_mutation_field
 from orchestrator.api.api_v1.endpoints.settings import generate_engine_status_response
 from orchestrator.db import EngineSettingsTable
 from orchestrator.graphql.schemas.errors import Error
 from orchestrator.graphql.schemas.settings import (
     CACHE_FLUSH_OPTIONS,
     CacheClearResponse,
     CacheClearSuccess,
```

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/graphql/resolvers/subscription.py` & `orchestrator_core-1.2.2rc3/orchestrator/graphql/resolvers/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/graphql/schemas/fixed_input.py` & `orchestrator_core-1.2.2rc3/orchestrator/graphql/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/graphql/schemas/process.py` & `orchestrator_core-1.2.2rc3/orchestrator/graphql/schemas/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from datetime import datetime
 from typing import TYPE_CHECKING, Annotated, Any, Dict, List, Optional, Union
 from uuid import UUID
 
 import strawberry
-from oauth2_lib.graphql_authentication import authenticated_field
 from sqlalchemy.orm import load_only
 from strawberry.scalars import JSON
 
+from oauth2_lib.strawberry import authenticated_field
 from orchestrator.config.assignee import Assignee
 from orchestrator.db import ProcessTable
 from orchestrator.graphql.pagination import EMPTY_PAGE, Connection
 from orchestrator.graphql.types import CustomInfo, GraphqlFilter, GraphqlSort
 from orchestrator.schemas.base import OrchestratorBaseModel
 from orchestrator.schemas.process import ProcessForm, ProcessStepSchema
 from orchestrator.workflow import ProcessStatus
```

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/graphql/schemas/product.py` & `orchestrator_core-1.2.2rc3/orchestrator/graphql/schemas/product.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TYPE_CHECKING, Annotated, Union
 
 import strawberry
-from oauth2_lib.graphql_authentication import authenticated_field
 
+from oauth2_lib.strawberry import authenticated_field
 from orchestrator.graphql.pagination import Connection
 from orchestrator.graphql.schemas.fixed_input import FixedInput
 from orchestrator.graphql.schemas.product_block import ProductBlock
 from orchestrator.graphql.schemas.workflow import Workflow
 from orchestrator.graphql.types import CustomInfo, GraphqlFilter, GraphqlSort
 from orchestrator.schemas.product import ProductSchema
```

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/graphql/schemas/product_block.py` & `orchestrator_core-1.2.2rc3/orchestrator/graphql/schemas/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/graphql/schemas/settings.py` & `orchestrator_core-1.2.2rc3/orchestrator/graphql/schemas/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/graphql/schemas/subscription.py` & `orchestrator_core-1.2.2rc3/orchestrator/graphql/schemas/subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from datetime import datetime
 from itertools import count
 from typing import Annotated, Any, Generator, List, Optional, Union
 from uuid import UUID
 
 import strawberry
-from oauth2_lib.graphql_authentication import authenticated_field
 from strawberry.scalars import JSON
 
+from oauth2_lib.strawberry import authenticated_field
 from orchestrator.db.models import SubscriptionTable
 from orchestrator.domain.base import SubscriptionModel
 from orchestrator.graphql.pagination import EMPTY_PAGE, Connection
 from orchestrator.graphql.resolvers.process import resolve_processes
 from orchestrator.graphql.schemas.process import ProcessType
 from orchestrator.graphql.types import CustomInfo, GraphqlFilter, GraphqlSort
 from orchestrator.schemas.base import OrchestratorBaseModel
```

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/graphql/types.py` & `orchestrator_core-1.2.2rc3/orchestrator/graphql/types.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 # limitations under the License.
 
 # Map some Orchestrator types to scalars
 from typing import Callable
 
 import strawberry
 from graphql import GraphQLError
-from oauth2_lib.fastapi import OIDCUserModel
 from strawberry.fastapi import BaseContext
 from strawberry.types import Info
 from strawberry.types.info import RootValueType
 
+from oauth2_lib.fastapi import OIDCUserModel
 from orchestrator.db.filters import Filter
 from orchestrator.db.sorting import Sort, SortOrder
 
 
 class CustomContext(BaseContext):
     def __init__(self, get_current_user: Callable[[], OIDCUserModel], get_opa_decision: Callable[[str], bool]):
         self.errors: list[GraphQLError] = []
```

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/graphql/utils/create_resolver_error_handler.py` & `orchestrator_core-1.2.2rc3/orchestrator/graphql/utils/create_resolver_error_handler.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/graphql/utils/get_selected_fields.py` & `orchestrator_core-1.2.2rc3/orchestrator/graphql/utils/get_selected_fields.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/migrations/alembic.ini` & `orchestrator_core-1.2.2rc3/orchestrator/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/migrations/env.py` & `orchestrator_core-1.2.2rc3/orchestrator/migrations/env.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/migrations/helpers.py` & `orchestrator_core-1.2.2rc3/orchestrator/migrations/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/migrations/templates/alembic.ini.j2` & `orchestrator_core-1.2.2rc3/orchestrator/migrations/templates/alembic.ini.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/migrations/templates/env.py.j2` & `orchestrator_core-1.2.2rc3/orchestrator/migrations/templates/env.py.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py` & `orchestrator_core-1.2.2rc3/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py` & `orchestrator_core-1.2.2rc3/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py` & `orchestrator_core-1.2.2rc3/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py` & `orchestrator_core-1.2.2rc3/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py` & `orchestrator_core-1.2.2rc3/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py` & `orchestrator_core-1.2.2rc3/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py` & `orchestrator_core-1.2.2rc3/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py` & `orchestrator_core-1.2.2rc3/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py` & `orchestrator_core-1.2.2rc3/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/schedules/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/schedules/resume_workflows.py` & `orchestrator_core-1.2.2rc3/orchestrator/schedules/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/schedules/scheduling.py` & `orchestrator_core-1.2.2rc3/orchestrator/schedules/scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/schedules/task_vacuum.py` & `orchestrator_core-1.2.2rc3/orchestrator/schedules/task_vacuum.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/schedules/validate_products.py` & `orchestrator_core-1.2.2rc3/orchestrator/schedules/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/schedules/validate_subscriptions.py` & `orchestrator_core-1.2.2rc3/orchestrator/schedules/validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/schemas/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/schemas/base.py` & `orchestrator_core-1.2.2rc3/orchestrator/schemas/base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/schemas/engine_settings.py` & `orchestrator_core-1.2.2rc3/orchestrator/schemas/engine_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/schemas/fixed_input.py` & `orchestrator_core-1.2.2rc3/orchestrator/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/schemas/problem_detail.py` & `orchestrator_core-1.2.2rc3/orchestrator/schemas/problem_detail.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/schemas/process.py` & `orchestrator_core-1.2.2rc3/orchestrator/schemas/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/schemas/product.py` & `orchestrator_core-1.2.2rc3/orchestrator/schemas/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/schemas/product_block.py` & `orchestrator_core-1.2.2rc3/orchestrator/schemas/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/schemas/resource_type.py` & `orchestrator_core-1.2.2rc3/orchestrator/schemas/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/schemas/subscription.py` & `orchestrator_core-1.2.2rc3/orchestrator/schemas/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/schemas/subscription_descriptions.py` & `orchestrator_core-1.2.2rc3/orchestrator/schemas/subscription_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/schemas/workflow.py` & `orchestrator_core-1.2.2rc3/orchestrator/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/security.py` & `orchestrator_core-1.2.2rc3/orchestrator/security.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from authlib.integrations.starlette_client import OAuth
-from oauth2_lib.fastapi import OIDCUser, opa_decision, opa_graphql_decision
 
 from nwastdlib.url import URL
+from oauth2_lib.fastapi import OIDCUser, opa_decision, opa_graphql_decision
+from oauth2_lib.settings import oauth2lib_settings
 from orchestrator.settings import oauth2_settings
 
 oauth_client_credentials = OAuth()
 
 well_known_endpoint = URL(oauth2_settings.OIDC_CONF_WELL_KNOWN_URL)
 
 oauth_client_credentials.register(
@@ -29,21 +30,23 @@
     request_token_params={"grant_type": "client_credentials"},
 )
 
 oidc_user = OIDCUser(
     oauth2_settings.OIDC_CONF_WELL_KNOWN_URL,
     oauth2_settings.OAUTH2_RESOURCE_SERVER_ID,
     oauth2_settings.OAUTH2_RESOURCE_SERVER_SECRET,
-    enabled=oauth2_settings.OAUTH2_ACTIVE,
+    enabled=oauth2lib_settings.OAUTH2_ACTIVE,
 )
 
-opa_security_default = opa_decision(oauth2_settings.OPA_URL, oidc_user, enabled=oauth2_settings.OAUTH2_ACTIVE)
+opa_security_default = opa_decision(oauth2_settings.OPA_URL, oidc_user, enabled=oauth2lib_settings.OAUTH2_ACTIVE)
 
 
-opa_security_graphql = opa_graphql_decision(oauth2_settings.OPA_URL, oidc_user, enabled=oauth2_settings.OAUTH2_ACTIVE)
+opa_security_graphql = opa_graphql_decision(
+    oauth2_settings.OPA_URL, oidc_user, enabled=oauth2lib_settings.OAUTH2_ACTIVE
+)
 
 
 def get_oidc_user() -> OIDCUser:
     return oidc_user
 
 
 def get_opa_security_graphql():  # type: ignore
```

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/services/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/services/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/services/celery.py` & `orchestrator_core-1.2.2rc3/orchestrator/services/celery.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/services/processes.py` & `orchestrator_core-1.2.2rc3/orchestrator/services/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/services/products.py` & `orchestrator_core-1.2.2rc3/orchestrator/services/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/services/settings.py` & `orchestrator_core-1.2.2rc3/orchestrator/services/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/services/subscriptions.py` & `orchestrator_core-1.2.2rc3/orchestrator/services/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/services/tasks.py` & `orchestrator_core-1.2.2rc3/orchestrator/services/tasks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/services/translations.py` & `orchestrator_core-1.2.2rc3/orchestrator/services/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/settings.py` & `orchestrator_core-1.2.2rc3/orchestrator/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import secrets
 import string
 from pathlib import Path
 from typing import List, Optional
 
 from pydantic import BaseSettings, PostgresDsn, RedisDsn
 
+from oauth2_lib.settings import oauth2lib_settings
 from orchestrator.types import strEnum
 
 
 class ExecutorType(strEnum):
     WORKER = "celery"
     THREADPOOL = "threadpool"
 
@@ -72,17 +73,20 @@
     DEFAULT_PRODUCT_WORKFLOWS: List[str] = ["modify_note"]
     SKIP_MODEL_FOR_MIGRATION_DB_DIFF: List[str] = []
     SERVE_GRAPHQL_UI: bool = True
     FEDEREATION_ENABLED: bool = False
 
 
 class Oauth2Settings(BaseSettings):
-    OAUTH2_ACTIVE: bool = False
     OAUTH2_RESOURCE_SERVER_ID: str = ""
     OAUTH2_RESOURCE_SERVER_SECRET: str = ""
     OAUTH2_TOKEN_URL: str = ""
     OIDC_CONF_WELL_KNOWN_URL: str = ""
     OPA_URL: str = "http://127.0.0.1:8181/v1/data/automation/authorization/allow"
 
 
 app_settings = AppSettings()
 oauth2_settings = Oauth2Settings()
+
+# Set oauth2lib_settings variables to the same (default) value of settings
+oauth2lib_settings.SERVICE_NAME = app_settings.SERVICE_NAME
+oauth2lib_settings.ENVIRONMENT = app_settings.ENVIRONMENT
```

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/targets.py` & `orchestrator_core-1.2.2rc3/orchestrator/targets.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/types.py` & `orchestrator_core-1.2.2rc3/orchestrator/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/utils/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/utils/crypt.py` & `orchestrator_core-1.2.2rc3/orchestrator/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/utils/datetime.py` & `orchestrator_core-1.2.2rc3/orchestrator/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/utils/docs.py` & `orchestrator_core-1.2.2rc3/orchestrator/utils/docs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/utils/errors.py` & `orchestrator_core-1.2.2rc3/orchestrator/utils/errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/utils/functional.py` & `orchestrator_core-1.2.2rc3/orchestrator/utils/functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/utils/helpers.py` & `orchestrator_core-1.2.2rc3/orchestrator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/utils/json.py` & `orchestrator_core-1.2.2rc3/orchestrator/utils/json.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/utils/redis.py` & `orchestrator_core-1.2.2rc3/orchestrator/utils/redis.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/utils/show_process.py` & `orchestrator_core-1.2.2rc3/orchestrator/utils/show_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/utils/speed.py` & `orchestrator_core-1.2.2rc3/orchestrator/utils/speed.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/utils/state.py` & `orchestrator_core-1.2.2rc3/orchestrator/utils/state.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/utils/strings.py` & `orchestrator_core-1.2.2rc3/orchestrator/utils/strings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/utils/vlans.py` & `orchestrator_core-1.2.2rc3/orchestrator/utils/vlans.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/version.py` & `orchestrator_core-1.2.2rc3/orchestrator/version.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/websocket/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/websocket/managers/broadcast_websocket_manager.py` & `orchestrator_core-1.2.2rc3/orchestrator/websocket/managers/broadcast_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/websocket/managers/memory_websocket_manager.py` & `orchestrator_core-1.2.2rc3/orchestrator/websocket/managers/memory_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/websocket/websocket_manager.py` & `orchestrator_core-1.2.2rc3/orchestrator/websocket/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/workflow.py` & `orchestrator_core-1.2.2rc3/orchestrator/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/workflows/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/workflows/modify_note.py` & `orchestrator_core-1.2.2rc3/orchestrator/workflows/modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/workflows/removed_workflow.py` & `orchestrator_core-1.2.2rc3/orchestrator/workflows/removed_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/workflows/steps.py` & `orchestrator_core-1.2.2rc3/orchestrator/workflows/steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/workflows/tasks/__init__.py` & `orchestrator_core-1.2.2rc3/orchestrator/workflows/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/workflows/tasks/cleanup_tasks_log.py` & `orchestrator_core-1.2.2rc3/orchestrator/workflows/tasks/cleanup_tasks_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/workflows/tasks/resume_workflows.py` & `orchestrator_core-1.2.2rc3/orchestrator/workflows/tasks/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/workflows/tasks/validate_products.py` & `orchestrator_core-1.2.2rc3/orchestrator/workflows/tasks/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/workflows/translations/en-GB.json` & `orchestrator_core-1.2.2rc3/orchestrator/workflows/translations/en-GB.json`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/orchestrator/workflows/utils.py` & `orchestrator_core-1.2.2rc3/orchestrator/workflows/utils.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/pyproject.toml` & `orchestrator_core-1.2.2rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -46,28 +46,28 @@
     "fastapi~=0.99.1",
     "fastapi-etag==0.4.0",
     "more-itertools~=9.0.0",
     "itsdangerous",
     "Jinja2==3.1.2",
     "orjson==3.9.1",
     "psycopg2-binary==2.9.5",
-    "pydantic[email]==1.10.9",
+    "pydantic[email]==1.10.9,<2.0.0",
     "python-dateutil==2.8.2",
     "python-rapidjson==1.9",
     "pytz==2023.3",
     "redis>=4.5.5,<4.6",
     "schedule==1.1.0",
     "sentry-sdk[fastapi]==1.25.1",
     "SQLAlchemy==1.4.48",
     "SQLAlchemy-Utils==0.40.0",
     "structlog",
     "typer==0.7.0",
     "uvicorn[standard]~=0.20.0",
     "nwa-stdlib~=1.4.8",
-    "oauth2-lib~=1.3.1",
+    "oauth2-lib==1.3.2",
     "tabulate==0.9.0",
     "strawberry-graphql==0.171.1"
 ]
 description-file = "README.md"
 requires-python = ">=3.9,<3.12"
 
 [project.urls]
@@ -201,23 +201,23 @@
     "I",
     "N",
     "RET",
     "S",
     "T",
     "W",
 ]
-target-version = "py310"
+target-version = "py39"
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.per-file-ignores]
 "orchestrator/api/*" = ["B008"]
 "orchestrator/cli/*" = ["B008"]
 "test/*" = ["S101", "B033", "N816", "N802"]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.ruff.isort]
 known-third-party = ["pynso", "pydantic"]
-known-first-party = ["migrations", "test", "nwastdlib", "oauth2-lib"]
+known-first-party = ["migrations", "test", "nwastdlib", "oauth2_lib"]
```

### Comparing `orchestrator_core-1.2.2rc2/setup.cfg` & `orchestrator_core-1.2.2rc3/setup.cfg`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/setup.py` & `orchestrator_core-1.2.2rc3/setup.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/acceptance_tests/conftest.py` & `orchestrator_core-1.2.2rc3/test/acceptance_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py` & `orchestrator_core-1.2.2rc3/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/main.py` & `orchestrator_core-1.2.2rc3/test/acceptance_tests/fixtures/test_orchestrator/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py` & `orchestrator_core-1.2.2rc3/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py` & `orchestrator_core-1.2.2rc3/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py` & `orchestrator_core-1.2.2rc3/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/acceptance_tests/test_test_product.py` & `orchestrator_core-1.2.2rc3/test/acceptance_tests/test_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/api/test_caching.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/api/test_caching.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/api/test_fixed_inputs.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/api/test_fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/api/test_health.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/api/test_health.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/api/test_helpers.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/api/test_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/api/test_models.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/api/test_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/api/test_processes.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/api/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/api/test_processes_ws.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/api/test_processes_ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/api/test_product_blocks.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/api/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/api/test_products.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/api/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/api/test_resource_types.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/api/test_resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/api/test_settings.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/api/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/api/test_subscription_customer_descriptions.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/api/test_subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/api/test_subscriptions.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/api/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/api/test_workflows.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/cli/test_migrate_domain_models_with_instances.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/cli/test_migrate_domain_models_with_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/cli/test_migrate_domain_models_without_instances.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/cli/test_migrate_domain_models_without_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/conftest.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/domain/test_base.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/domain/test_base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/domain/test_base_with_list_union.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/domain/test_base_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/domain/test_base_with_union.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/domain/test_base_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/__init__.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/processes.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/product_type_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_one.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/product_type_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_union.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/product_types/product_type_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/fixtures/products/resource_types.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/fixtures/products/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/forms/shared.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/forms/shared.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/forms/test_generic_validators.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/forms/test_generic_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/forms/test_network_validators.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/forms/test_network_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/forms/test_post_process.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/forms/test_post_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/graphql/test_processes.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/graphql/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/graphql/test_product.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/graphql/test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/graphql/test_settings.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/graphql/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/graphql/test_subscriptions.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/graphql/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/schedules/test_scheduling.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/schedules/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/services/test_processes.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/services/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/services/test_products.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/services/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/services/test_subscriptions.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/services/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/services/test_translations.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/services/test_translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/test_db.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/test_db.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/test_workflow.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/utils/test_errors.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/utils/test_errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/utils/test_functional.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/utils/test_functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/utils/test_json.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/utils/test_speed.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/utils/test_speed.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/utils/test_state.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/utils/test_state.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/utils/test_vlans.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/utils/test_vlans.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/workflows/__init__.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/workflows/shared/test_validate_subscriptions.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/workflows/shared/test_validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/workflows/tasks/test_clean_up_task_log.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/workflows/tasks/test_clean_up_task_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/workflows/tasks/test_resume_workflows.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/workflows/tasks/test_resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/workflows/test_config_db_code.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/workflows/test_config_db_code.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/workflows/test_generic_workflow_steps.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/workflows/test_generic_workflow_steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/test/unit_tests/workflows/test_modify_note.py` & `orchestrator_core-1.2.2rc3/test/unit_tests/workflows/test_modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.2.2rc2/PKG-INFO` & `orchestrator_core-1.2.2rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestrator-core
-Version: 1.2.2rc2
+Version: 1.2.2rc3
 Summary: Open source orchestration software for NREN's
 Requires-Python: >=3.9,<3.12
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
@@ -36,28 +36,28 @@
 Requires-Dist: fastapi~=0.99.1
 Requires-Dist: fastapi-etag==0.4.0
 Requires-Dist: more-itertools~=9.0.0
 Requires-Dist: itsdangerous
 Requires-Dist: Jinja2==3.1.2
 Requires-Dist: orjson==3.9.1
 Requires-Dist: psycopg2-binary==2.9.5
-Requires-Dist: pydantic[email]==1.10.9
+Requires-Dist: pydantic[email]==1.10.9,<2.0.0
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: python-rapidjson==1.9
 Requires-Dist: pytz==2023.3
 Requires-Dist: redis>=4.5.5,<4.6
 Requires-Dist: schedule==1.1.0
 Requires-Dist: sentry-sdk[fastapi]==1.25.1
 Requires-Dist: SQLAlchemy==1.4.48
 Requires-Dist: SQLAlchemy-Utils==0.40.0
 Requires-Dist: structlog
 Requires-Dist: typer==0.7.0
 Requires-Dist: uvicorn[standard]~=0.20.0
 Requires-Dist: nwa-stdlib~=1.4.8
-Requires-Dist: oauth2-lib~=1.3.1
+Requires-Dist: oauth2-lib==1.3.2
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: strawberry-graphql==0.171.1
 Requires-Dist: celery~=5.2.7 ; extra == "celery"
 Requires-Dist: toml ; extra == "dev"
 Requires-Dist: bumpversion ; extra == "dev"
 Requires-Dist: mypy_extensions ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
```

