# Comparing `tmp/app_model-0.2.0.tar.gz` & `tmp/app_model-0.2.0rc1.tar.gz`

## Comparing `app_model-0.2.0.tar` & `app_model-0.2.0rc1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 app_model-0.2.0/.github_changelog_generator
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 app_model-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 app_model-0.2.0/.readthedocs.yaml
--rw-r--r--   0        0        0    12104 2020-02-02 00:00:00.000000 app_model-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 app_model-0.2.0/codecov.yml
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 app_model-0.2.0/mkdocs.yml
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 app_model-0.2.0/setup.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 app_model-0.2.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 app_model-0.2.0/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 app_model-0.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 app_model-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 app_model-0.2.0/.github/workflows/cron.yml
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 app_model-0.2.0/demo/keybinding_helper.py
--rw-r--r--   0        0        0     8203 2020-02-02 00:00:00.000000 app_model-0.2.0/demo/model_app.py
--rw-r--r--   0        0        0     8316 2020-02-02 00:00:00.000000 app_model-0.2.0/demo/qapplication.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 app_model-0.2.0/demo/multi_file/__init__.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 app_model-0.2.0/demo/multi_file/__main__.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 app_model-0.2.0/demo/multi_file/actions.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 app_model-0.2.0/demo/multi_file/app.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 app_model-0.2.0/demo/multi_file/constants.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 app_model-0.2.0/demo/multi_file/functions.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 app_model-0.2.0/docs/_macros.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 app_model-0.2.0/docs/application.md
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 app_model-0.2.0/docs/expressions.md
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 app_model-0.2.0/docs/index.md
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 app_model-0.2.0/docs/keybindings.md
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 app_model-0.2.0/docs/registries.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 app_model-0.2.0/docs/types.md
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/__init__.py
--rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/_app.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/_pydantic_compat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/py.typed
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/backends/__init__.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/backends/qt/__init__.py
--rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/backends/qt/_qaction.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/backends/qt/_qkeybindingedit.py
--rw-r--r--   0        0        0    16388 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/backends/qt/_qkeymap.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/backends/qt/_qmainwindow.py
--rw-r--r--   0        0        0    12837 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/backends/qt/_qmenu.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/backends/qt/_util.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/expressions/__init__.py
--rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/expressions/_context.py
--rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/expressions/_context_keys.py
--rw-r--r--   0        0        0    19577 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/expressions/_expressions.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/registries/__init__.py
--rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/registries/_commands_reg.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/registries/_keybindings_reg.py
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/registries/_menus_reg.py
--rw-r--r--   0        0        0     8764 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/registries/_register.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/types/__init__.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/types/_action.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/types/_base.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/types/_command_rule.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/types/_constants.py
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/types/_icon.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/types/_keybinding_rule.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/types/_menu_rule.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/types/_utils.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/types/_keys/__init__.py
--rw-r--r--   0        0        0    34077 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/types/_keys/_key_codes.py
--rw-r--r--   0        0        0     9966 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/types/_keys/_keybindings.py
--rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 app_model-0.2.0/src/app_model/types/_keys/_standard_bindings.py
--rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 app_model-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 app_model-0.2.0/tests/test_actions.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 app_model-0.2.0/tests/test_app.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 app_model-0.2.0/tests/test_command_registry.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 app_model-0.2.0/tests/test_key_codes.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 app_model-0.2.0/tests/test_keybindings.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 app_model-0.2.0/tests/test_registries.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 app_model-0.2.0/tests/test_types.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 app_model-0.2.0/tests/fixtures/fake_module.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 app_model-0.2.0/tests/test_context/test_context.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 app_model-0.2.0/tests/test_context/test_context_keys.py
--rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 app_model-0.2.0/tests/test_context/test_expressions.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 app_model-0.2.0/tests/test_qt/__init__.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 app_model-0.2.0/tests/test_qt/test_demos.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 app_model-0.2.0/tests/test_qt/test_qactions.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 app_model-0.2.0/tests/test_qt/test_qkeybindingedit.py
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 app_model-0.2.0/tests/test_qt/test_qkeymap.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 app_model-0.2.0/tests/test_qt/test_qmainwindow.py
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 app_model-0.2.0/tests/test_qt/test_qmenu.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 app_model-0.2.0/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 app_model-0.2.0/LICENSE
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 app_model-0.2.0/README.md
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 app_model-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 app_model-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/.github_changelog_generator
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/.readthedocs.yaml
+-rw-r--r--   0        0        0    11612 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/codecov.yml
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/mkdocs.yml
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/setup.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/.github/dependabot.yml
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/.github/workflows/cron.yml
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/demo/keybinding_helper.py
+-rw-r--r--   0        0        0     8203 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/demo/model_app.py
+-rw-r--r--   0        0        0     8316 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/demo/qapplication.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/demo/multi_file/__init__.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/demo/multi_file/__main__.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/demo/multi_file/actions.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/demo/multi_file/app.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/demo/multi_file/constants.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/demo/multi_file/functions.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/docs/_macros.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/docs/application.md
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/docs/expressions.md
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/docs/index.md
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/docs/keybindings.md
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/docs/registries.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/docs/types.md
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/__init__.py
+-rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/_app.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/_pydantic_compat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/py.typed
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/backends/__init__.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/backends/qt/__init__.py
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/backends/qt/_qaction.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/backends/qt/_qkeybindingedit.py
+-rw-r--r--   0        0        0    16388 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/backends/qt/_qkeymap.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/backends/qt/_qmainwindow.py
+-rw-r--r--   0        0        0    12837 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/backends/qt/_qmenu.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/backends/qt/_util.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/expressions/__init__.py
+-rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/expressions/_context.py
+-rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/expressions/_context_keys.py
+-rw-r--r--   0        0        0    19395 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/expressions/_expressions.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/registries/__init__.py
+-rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/registries/_commands_reg.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/registries/_keybindings_reg.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/registries/_menus_reg.py
+-rw-r--r--   0        0        0     8777 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/registries/_register.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/__init__.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_action.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_base.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_command_rule.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_constants.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_icon.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_keybinding_rule.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_menu_rule.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_utils.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_keys/__init__.py
+-rw-r--r--   0        0        0    33936 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_keys/_key_codes.py
+-rw-r--r--   0        0        0     9966 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_keys/_keybindings.py
+-rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/src/app_model/types/_keys/_standard_bindings.py
+-rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/conftest.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_actions.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_app.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_command_registry.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_key_codes.py
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_keybindings.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_registries.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_types.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/fixtures/fake_module.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_context/test_context.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_context/test_context_keys.py
+-rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_context/test_expressions.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_qt/__init__.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_qt/test_demos.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_qt/test_qactions.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_qt/test_qkeybindingedit.py
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_qt/test_qkeymap.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_qt/test_qmainwindow.py
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/tests/test_qt/test_qmenu.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/LICENSE
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/README.md
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 app_model-0.2.0rc1/PKG-INFO
```

### Comparing `app_model-0.2.0/.pre-commit-config.yaml` & `app_model-0.2.0rc1/.pre-commit-config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -3,53 +3,53 @@
   autofix_commit_msg: "style: [pre-commit.ci] auto fixes [...]"
   autoupdate_commit_msg: "ci: [pre-commit.ci] autoupdate"
 
 default_install_hook_types: [pre-commit, commit-msg]
 
 repos:
   - repo: https://github.com/compilerla/conventional-pre-commit
-    rev: v2.3.0
+    rev: v2.2.0
     hooks:
       - id: conventional-pre-commit
         stages: [commit-msg]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-docstring-first
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/psf/black
-    rev: 23.7.0
+    rev: 23.3.0
     hooks:
       - id: black
 
-  - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.0.278
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: v0.0.263
     hooks:
       - id: ruff
         args: ["--fix"]
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.13
+    rev: v0.12.2
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.4.1
+    rev: v1.2.0
     hooks:
       - id: mypy
         files: "^src/"
         additional_dependencies:
           - pydantic
           - in-n-out
 
   # manual hooks
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.5
+    rev: v2.2.4
     hooks:
       - id: codespell
         exclude: CHANGELOG.md
         stages:
           - "manual"
```

### Comparing `app_model-0.2.0/CHANGELOG.md` & `app_model-0.2.0rc1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,18 @@
 # Changelog
 
-## [v0.2.0](https://github.com/pyapp-kit/app-model/tree/v0.2.0) (2023-07-13)
+## [0.2.0](https://github.com/pyapp-kit/app-model/tree/0.2.0) (2023-05-30)
 
-[Full Changelog](https://github.com/pyapp-kit/app-model/compare/v0.1.4...v0.2.0)
+[Full Changelog](https://github.com/pyapp-kit/app-model/compare/v0.1.4...0.2.0)
 
-**Implemented enhancements:**
-
-- feat: map win and cmd to meta [\#113](https://github.com/pyapp-kit/app-model/pull/113) ([tlambert03](https://github.com/tlambert03))
-- feat: support pydantic v2 [\#98](https://github.com/pyapp-kit/app-model/pull/98) ([tlambert03](https://github.com/tlambert03))
-
-**Fixed bugs:**
+**Merged pull requests:**
 
-- fix: Amend preferences `StandardKeyBinding` [\#104](https://github.com/pyapp-kit/app-model/pull/104) ([lucyleeow](https://github.com/lucyleeow))
 - fix: fix menu titles in QtModelMenuBar [\#102](https://github.com/pyapp-kit/app-model/pull/102) ([tlambert03](https://github.com/tlambert03))
-
-**Tests & CI:**
-
-- ci: test pydantic1 [\#115](https://github.com/pyapp-kit/app-model/pull/115) ([tlambert03](https://github.com/tlambert03))
-
-**Documentation:**
-
-- docs: Move `_expressions.py` docstring to be included in documentation [\#107](https://github.com/pyapp-kit/app-model/pull/107) ([lucyleeow](https://github.com/lucyleeow))
+- ci: \[pre-commit.ci\] autoupdate [\#99](https://github.com/pyapp-kit/app-model/pull/99) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
+- feat: support pydantic v2 [\#98](https://github.com/pyapp-kit/app-model/pull/98) ([tlambert03](https://github.com/tlambert03))
 
 ## [v0.1.4](https://github.com/pyapp-kit/app-model/tree/v0.1.4) (2023-04-06)
 
 [Full Changelog](https://github.com/pyapp-kit/app-model/compare/v0.1.3...v0.1.4)
 
 **Merged pull requests:**
```

### Comparing `app_model-0.2.0/mkdocs.yml` & `app_model-0.2.0rc1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/setup.py` & `app_model-0.2.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/.github/workflows/ci.yml` & `app_model-0.2.0rc1/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,16 @@
         run: |
           python -m pip install -U pip
           python -m pip install -e .[test]
 
       - name: Test
         run: pytest -s --color=yes
 
-  test-pydantic1:
-    name: pydantic1 (py${{ matrix.python-version }})
+  test-pydantic2:
+    name: pydantic2 (py${{ matrix.python-version }})
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.8", "3.10", "3.11"]
 
     steps:
@@ -66,15 +66,15 @@
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install -e .[test]
-          pip install 'pydantic<2'
+          pip install -U --pre pydantic
 
       - name: Test
         run: pytest --color=yes --cov=app_model --cov-report=xml
 
       - name: Coverage
         uses: codecov/codecov-action@v3
```

### Comparing `app_model-0.2.0/.github/workflows/cron.yml` & `app_model-0.2.0rc1/.github/workflows/cron.yml`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/demo/model_app.py` & `app_model-0.2.0rc1/demo/model_app.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/demo/qapplication.py` & `app_model-0.2.0rc1/demo/qapplication.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/demo/multi_file/actions.py` & `app_model-0.2.0rc1/demo/multi_file/actions.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/demo/multi_file/app.py` & `app_model-0.2.0rc1/demo/multi_file/app.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/docs/index.md` & `app_model-0.2.0rc1/docs/index.md`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/docs/types.md` & `app_model-0.2.0rc1/docs/types.md`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/_app.py` & `app_model-0.2.0rc1/src/app_model/_app.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/_pydantic_compat.py` & `app_model-0.2.0rc1/src/app_model/_pydantic_compat.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,28 +14,28 @@
     def decorator(func: C) -> C:
         return func
 
     return decorator
 
 
 if PYDANTIC2:
-    from pydantic import field_validator
+    from pydantic import field_validator  # type: ignore
     from pydantic import model_validator as model_validator  # type: ignore # noqa
 
     def validator(*args: Any, **kwargs: Any) -> Callable[[Callable], Callable]:
-        return field_validator(*args, **kwargs)
+        return field_validator(*args, **kwargs)  # type: ignore
 
     def asdict(obj: BaseModel, *args: Any, **kwargs: Any) -> dict:
-        return obj.model_dump(*args, **kwargs)
+        return obj.model_dump(*args, **kwargs)  # type: ignore
 
     def asjson(obj: BaseModel, *args: Any, **kwargs: Any) -> str:
-        return obj.model_dump_json(*args, **kwargs)
+        return obj.model_dump_json(*args, **kwargs)  # type: ignore
 
 else:
-    from pydantic import validator as validator
+    from pydantic import validator as validator  # type: ignore # noqa
 
     def asdict(obj: BaseModel, *args: Any, **kwargs: Any) -> dict:
         return obj.dict(*args, **kwargs)
 
     def asjson(obj: BaseModel, *args: Any, **kwargs: Any) -> str:
         return obj.json(*args, **kwargs)
```

### Comparing `app_model-0.2.0/src/app_model/backends/qt/__init__.py` & `app_model-0.2.0rc1/src/app_model/backends/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/backends/qt/_qaction.py` & `app_model-0.2.0rc1/src/app_model/backends/qt/_qaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,11 @@
 from __future__ import annotations
 
 import contextlib
-from typing import (
-    TYPE_CHECKING,
-    ClassVar,
-    Dict,
-    Mapping,
-    Optional,
-    Tuple,
-    Type,
-    Union,
-    cast,
-)
+from typing import TYPE_CHECKING, Dict, Mapping, Optional, Tuple, Type, Union, cast
 
 from qtpy.QtWidgets import QAction
 
 from app_model import Application
 from app_model.expressions import Expr
 from app_model.types import ToggleRule
 
@@ -122,15 +112,15 @@
 class QMenuItemAction(QCommandRuleAction):
     """QAction for a MenuItem.
 
     Mostly the same as a CommandRuleAction, but aware of the `menu_item.when` clause
     to toggle visibility.
     """
 
-    _cache: ClassVar[Dict[Tuple[int, int], QMenuItemAction]] = {}
+    _cache: Dict[Tuple[int, int], QMenuItemAction] = {}
 
     def __new__(
         cls: Type[QMenuItemAction],
         menu_item: MenuItem,
         app: Union[str, Application],
         parent: Optional[QObject] = None,
         *,
```

### Comparing `app_model-0.2.0/src/app_model/backends/qt/_qkeybindingedit.py` & `app_model-0.2.0rc1/src/app_model/backends/qt/_qkeybindingedit.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/backends/qt/_qkeymap.py` & `app_model-0.2.0rc1/src/app_model/backends/qt/_qkeymap.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/backends/qt/_qmainwindow.py` & `app_model-0.2.0rc1/src/app_model/backends/qt/_qmainwindow.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/backends/qt/_qmenu.py` & `app_model-0.2.0rc1/src/app_model/backends/qt/_qmenu.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/expressions/__init__.py` & `app_model-0.2.0rc1/src/app_model/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/expressions/_context.py` & `app_model-0.2.0rc1/src/app_model/expressions/_context.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/expressions/_context_keys.py` & `app_model-0.2.0rc1/src/app_model/expressions/_context_keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import contextlib
 from types import MappingProxyType
 from typing import (
     Any,
     Callable,
-    ClassVar,
     Dict,
     Generic,
     List,
     Literal,
     MutableMapping,
     NamedTuple,
     Optional,
@@ -83,15 +82,15 @@
     >>> expr.eval({'some_key': 3})  # False
     >>> expr.eval({'some_key': 6})  # True
     """
 
     # This will catalog all ContextKeys that get instantiated, which provides
     # an easy way to organize documentation.
     # ContextKey.info() returns a list with info for all ContextKeys
-    _info: ClassVar[List[ContextKeyInfo]] = []
+    _info: List[ContextKeyInfo] = []
     MISSING = MISSING
 
     def __init__(
         self,
         default_value: Union[T, __missing] = MISSING,
         description: Optional[str] = None,
         getter: Optional[Callable[[A], T]] = None,
```

### Comparing `app_model-0.2.0/src/app_model/expressions/_expressions.py` & `app_model-0.2.0rc1/src/app_model/expressions/_expressions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,32 @@
-"""Provides the  :class:`Expr` and its subclasses."""
+"""Provides the  :class:`Expr` and its subclasses.
+
+`Expr` is a subclass of `ast.AST` that provides rich dunder methods that
+facilitate joining and comparing typed expressions.  It only implements a
+subset of ast Expressions (for safety of evaluation), but provides more
+than ast.literal_eval.
+
+Expressions that are supported:
+- Names: 'myvar' (these must be evaluated along with some context)
+- Constants: '1'
+- Comparisons: 'myvar > 1'
+- Boolean Operators: 'myvar and yourvar'
+- Binary Operators: 'myvar + 42'
+- Unary Operators: 'not myvar'
+
+Things that are *NOT* supported:
+- attribute access: 'my.attr'
+- calls: 'f(x)'
+- containers (lists, tuples, sets, dicts)
+- indexing or slicing
+- joined strings (f-strings)
+- named expressions (walrus operator)
+- comprehensions (list, set, dict, generator)
+- statements & assignments (e.g. 'a = b')
+"""
 from __future__ import annotations
 
 import ast
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
@@ -91,38 +115,14 @@
         return expr
     return parse_expression(expr).eval(context or {})
 
 
 class Expr(ast.AST, Generic[T]):
     """Base Expression class providing dunder and convenience methods.
 
-    This is a subclass of `ast.AST` that provides rich dunder methods that
-    facilitate joining and comparing typed expressions.  It only implements a
-    subset of ast Expressions (for safety of evaluation), but provides more
-    than `ast.literal_eval`.
-
-    Expressions that are supported:
-    - Names: 'myvar' (these must be evaluated along with some context)
-    - Constants: '1'
-    - Comparisons: 'myvar > 1'
-    - Boolean Operators: 'myvar & yourvar' (bitwise `&` and `|` are overloaded
-      here to mean boolean `and` and `or`)
-    - Binary Operators: 'myvar + 42' (includes `//`, `@`, `^`)
-    - Unary Operators: 'not myvar'
-
-    Things that are *NOT* supported:
-    - attribute access: 'my.attr'
-    - calls: 'f(x)'
-    - containers (lists, tuples, sets, dicts)
-    - indexing or slicing
-    - joined strings (f-strings)
-    - named expressions (walrus operator)
-    - comprehensions (list, set, dict, generator)
-    - statements & assignments (e.g. 'a = b')
-
     This class is not meant to be instantiated directly. Instead, use
     [`parse_expression`][app_model.expressions._expressions.parse_expression], or the
     [`Expr.parse`][app_model.expressions.Expr.parse] classmethod to create an expression
     instance.
 
     Once created, an expression can be joined with other expressions, or
     constants.
```

### Comparing `app_model-0.2.0/src/app_model/registries/_commands_reg.py` & `app_model-0.2.0rc1/src/app_model/registries/_commands_reg.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/registries/_keybindings_reg.py` & `app_model-0.2.0rc1/src/app_model/registries/_keybindings_reg.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/registries/_menus_reg.py` & `app_model-0.2.0rc1/src/app_model/registries/_menus_reg.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/registries/_register.py` & `app_model-0.2.0rc1/src/app_model/registries/_register.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,39 +26,39 @@
 
 @overload
 def register_action(
     app: Union[Application, str],
     id_or_action: str,
     title: str,
     *,
-    callback: Literal[None] = ...,
-    category: Optional[str] = ...,
-    tooltip: Optional[str] = ...,
-    icon: Optional[IconOrDict] = ...,
-    enablement: Optional[expressions.Expr] = ...,
-    menus: Optional[List[MenuRuleOrDict]] = ...,
-    keybindings: Optional[List[KeyBindingRuleOrDict]] = ...,
+    callback: Literal[None] = None,
+    category: Optional[str] = None,
+    tooltip: Optional[str] = None,
+    icon: Optional[IconOrDict] = None,
+    enablement: Optional[expressions.Expr] = None,
+    menus: Optional[List[MenuRuleOrDict]] = None,
+    keybindings: Optional[List[KeyBindingRuleOrDict]] = None,
     palette: bool = True,
 ) -> CommandDecorator:
     ...
 
 
 @overload
 def register_action(
     app: Union[Application, str],
     id_or_action: str,
     title: str,
     *,
     callback: CommandCallable,
-    category: Optional[str] = ...,
-    tooltip: Optional[str] = ...,
-    icon: Optional[IconOrDict] = ...,
-    enablement: Optional[expressions.Expr] = ...,
-    menus: Optional[List[MenuRuleOrDict]] = ...,
-    keybindings: Optional[List[KeyBindingRuleOrDict]] = ...,
+    category: Optional[str] = None,
+    tooltip: Optional[str] = None,
+    icon: Optional[IconOrDict] = None,
+    enablement: Optional[expressions.Expr] = None,
+    menus: Optional[List[MenuRuleOrDict]] = None,
+    keybindings: Optional[List[KeyBindingRuleOrDict]] = None,
     palette: bool = True,
 ) -> DisposeCallable:
     ...
 
 
 def register_action(
     app: Union[Application, str],
```

### Comparing `app_model-0.2.0/src/app_model/types/__init__.py` & `app_model-0.2.0rc1/src/app_model/types/__init__.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/types/_action.py` & `app_model-0.2.0rc1/src/app_model/types/_action.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/types/_command_rule.py` & `app_model-0.2.0rc1/src/app_model/types/_command_rule.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/types/_constants.py` & `app_model-0.2.0rc1/src/app_model/types/_constants.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/types/_icon.py` & `app_model-0.2.0rc1/src/app_model/types/_icon.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/types/_keybinding_rule.py` & `app_model-0.2.0rc1/src/app_model/types/_keybinding_rule.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/types/_menu_rule.py` & `app_model-0.2.0rc1/src/app_model/types/_menu_rule.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/types/_utils.py` & `app_model-0.2.0rc1/src/app_model/types/_utils.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/types/_keys/_key_codes.py` & `app_model-0.2.0rc1/src/app_model/types/_keys/_key_codes.py`

 * *Files 1% similar despite different names*

```diff
@@ -553,19 +553,15 @@
         _KM(ScanCode.MetaRight, 'MetaRight', KeyCode.Meta, _, 0, 'VK_RWIN'),
     ]
 
     SCANCODE_TO_STRING: Dict[ScanCode, str] = {}
     SCANCODE_FROM_LOWERCASE_STRING: Dict[str, ScanCode] = {}
 
     KEYCODE_TO_STRING: Dict[KeyCode, str] = {}
-    KEYCODE_FROM_LOWERCASE_STRING: Dict[str, KeyCode] = {
-        # two special cases for assigning os-specific strings to the meta key
-        'win': KeyCode.Meta,
-        'cmd': KeyCode.Meta,
-    }
+    KEYCODE_FROM_LOWERCASE_STRING: Dict[str, KeyCode] = {}
 
     seen_scancodes: Set[ScanCode] = set()
     seen_keycodes: Set[KeyCode] = set()
     for i, km in enumerate(_MAPPINGS):
         if km.scancode not in seen_scancodes:
             seen_scancodes.add(km.scancode)
             SCANCODE_TO_STRING[km.scancode] = km.scanstr
```

### Comparing `app_model-0.2.0/src/app_model/types/_keys/_keybindings.py` & `app_model-0.2.0rc1/src/app_model/types/_keys/_keybindings.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/src/app_model/types/_keys/_standard_bindings.py` & `app_model-0.2.0rc1/src/app_model/types/_keys/_standard_bindings.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     SK(StandardKeyBinding.MoveToPreviousWord, KeyMod.CtrlCmd | KeyCode.LeftArrow, _, KeyMod.Alt | KeyCode.LeftArrow),
     SK(StandardKeyBinding.MoveToStartOfDocument, KeyMod.CtrlCmd | KeyCode.Home, _, KeyCode.Home),
     SK(StandardKeyBinding.MoveToStartOfLine, KeyCode.Home, _, KeyMod.CtrlCmd | KeyCode.LeftArrow),
     SK(StandardKeyBinding.New, KeyMod.CtrlCmd | KeyCode.KeyN),
     SK(StandardKeyBinding.NextChild, KeyMod.CtrlCmd | KeyCode.Tab, _, KeyMod.CtrlCmd | KeyMod.Shift | KeyCode.BracketRight),
     SK(StandardKeyBinding.Open, KeyMod.CtrlCmd | KeyCode.KeyO),
     SK(StandardKeyBinding.Paste, KeyMod.CtrlCmd | KeyCode.KeyV),
-    SK(StandardKeyBinding.Preferences, KeyMod.CtrlCmd | KeyCode.Comma),
+    SK(StandardKeyBinding.Preferences, _, _, KeyMod.CtrlCmd, KeyCode.Comma),
     SK(StandardKeyBinding.PreviousChild, KeyMod.CtrlCmd | KeyMod.Shift | KeyCode.Tab, _, KeyMod.CtrlCmd | KeyMod.Shift | KeyCode.BracketLeft),
     SK(StandardKeyBinding.Print, KeyMod.CtrlCmd | KeyCode.KeyP),
     SK(StandardKeyBinding.Quit, KeyMod.CtrlCmd | KeyCode.KeyQ),
     SK(StandardKeyBinding.Redo, KeyMod.CtrlCmd | KeyMod.Shift | KeyCode.KeyZ, KeyMod.CtrlCmd | KeyCode.KeyY),
     SK(StandardKeyBinding.Refresh, KeyMod.CtrlCmd | KeyCode.KeyR),
     SK(StandardKeyBinding.Replace, KeyMod.CtrlCmd | KeyCode.KeyH),
     SK(StandardKeyBinding.Save, KeyMod.CtrlCmd | KeyCode.KeyS),
```

### Comparing `app_model-0.2.0/tests/conftest.py` & `app_model-0.2.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/tests/test_actions.py` & `app_model-0.2.0rc1/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/tests/test_app.py` & `app_model-0.2.0rc1/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/tests/test_command_registry.py` & `app_model-0.2.0rc1/tests/test_command_registry.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/tests/test_key_codes.py` & `app_model-0.2.0rc1/tests/test_key_codes.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/tests/test_keybindings.py` & `app_model-0.2.0rc1/tests/test_keybindings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import sys
-from typing import ClassVar
 
 import pytest
 from pydantic import BaseModel
 
 from app_model._pydantic_compat import PYDANTIC2, asjson
 from app_model.types import (
     KeyBinding,
@@ -103,15 +102,15 @@
 def test_in_model():
     class M(BaseModel):
         key: KeyBinding
 
         if not PYDANTIC2:
 
             class Config:
-                json_encoders: ClassVar[dict] = {KeyBinding: str}
+                json_encoders = {KeyBinding: str}
 
     m = M(key="Shift+A B")
     # pydantic v1 and v2 have slightly different json outputs
     assert asjson(m).replace('": "', '":"') == '{"key":"Shift+A B"}'
 
 
 def test_standard_keybindings():
```

### Comparing `app_model-0.2.0/tests/test_registries.py` & `app_model-0.2.0rc1/tests/test_registries.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/tests/test_types.py` & `app_model-0.2.0rc1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/tests/test_context/test_context.py` & `app_model-0.2.0rc1/tests/test_context/test_context.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/tests/test_context/test_context_keys.py` & `app_model-0.2.0rc1/tests/test_context/test_context_keys.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/tests/test_context/test_expressions.py` & `app_model-0.2.0rc1/tests/test_context/test_expressions.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/tests/test_qt/test_qactions.py` & `app_model-0.2.0rc1/tests/test_qt/test_qactions.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/tests/test_qt/test_qkeymap.py` & `app_model-0.2.0rc1/tests/test_qt/test_qkeymap.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/tests/test_qt/test_qmainwindow.py` & `app_model-0.2.0rc1/tests/test_qt/test_qmainwindow.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/tests/test_qt/test_qmenu.py` & `app_model-0.2.0rc1/tests/test_qt/test_qmenu.py`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/.gitignore` & `app_model-0.2.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/LICENSE` & `app_model-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/README.md` & `app_model-0.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/pyproject.toml` & `app_model-0.2.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `app_model-0.2.0/PKG-INFO` & `app_model-0.2.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app-model
-Version: 0.2.0
+Version: 0.2.0rc1
 Summary: Generic application schema implemented in python
 Project-URL: homepage, https://github.com/pyapp-kit/app-model
 Project-URL: repository, https://github.com/pyapp-kit/app-model
 Author: Talley Lambert
 Author-email: talley.lambert@gmail.com
 License: BSD 3-Clause License
 License-File: LICENSE
```

