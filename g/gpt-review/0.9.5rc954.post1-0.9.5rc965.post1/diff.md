# Comparing `tmp/gpt_review-0.9.5rc954.post1.tar.gz` & `tmp/gpt_review-0.9.5rc965.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_review-0.9.5rc954.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gpt_review-0.9.5rc965.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gpt_review-0.9.5rc954.post1.tar` & `gpt_review-0.9.5rc965.post1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0      336 2023-07-04 21:59:50.182143 gpt_review-0.9.5rc954.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-07-04 21:59:50.182143 gpt_review-0.9.5rc954.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-07-04 21:59:50.182143 gpt_review-0.9.5rc954.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      766 2023-07-04 21:59:50.182143 gpt_review-0.9.5rc954.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1977 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4301 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      671 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/.github/workflows/schedule-action-update.yml
--rw-r--r--   0        0        0      314 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1776 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     2041 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/.pypirc
--rw-r--r--   0        0        0       96 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/.vscode/extensions.json
--rw-r--r--   0        0        0      530 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/.vscode/launch.json
--rw-r--r--   0        0        0     1125 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/.vscode/settings.json
--rw-r--r--   0        0        0      905 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/.vscode/tasks.json
--rw-r--r--   0        0        0     1070 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/LICENSE
--rw-r--r--   0        0        0     3556 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/README.md
--rw-r--r--   0        0        0     2757 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/SECURITY.md
--rw-r--r--   0        0        0     2307 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/action.yml
--rw-r--r--   0        0        0      308 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/azure.yaml.template
--rw-r--r--   0        0        0      218 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/config.summary.template.yml
--rw-r--r--   0        0        0      362 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/prompt.template.yml
--rw-r--r--   0        0        0     8725 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-04 22:00:21.702432 gpt_review-0.9.5rc954.post1/src/gpt/__init__.py
--rw-r--r--   0        0        0      170 2023-07-04 21:59:50.186143 gpt_review-0.9.5rc954.post1/src/gpt/__main__.py
--rw-r--r--   0        0        0      366 2023-07-04 22:00:21.702432 gpt_review-0.9.5rc954.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0      170 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/src/gpt_review/__main__.py
--rw-r--r--   0        0        0     9452 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     3520 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/src/gpt_review/_git.py
--rw-r--r--   0        0        0     1453 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0     6437 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/src/gpt_review/_llama_index.py
--rw-r--r--   0        0        0     4315 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/src/gpt_review/_openai.py
--rw-r--r--   0        0        0     8692 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/src/gpt_review/_review.py
--rw-r--r--   0        0        0      980 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0     3349 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/src/gpt_review/context.py
--rw-r--r--   0        0        0      924 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0       33 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/src/gpt_review/prompts/__init__.py
--rw-r--r--   0        0        0     1246 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/src/gpt_review/prompts/_prompt.py
--rw-r--r--   0        0        0      362 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/src/gpt_review/prompts/prompt_bug.yaml
--rw-r--r--   0        0        0      327 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/src/gpt_review/prompts/prompt_coverage.yaml
--rw-r--r--   0        0        0      349 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/src/gpt_review/prompts/prompt_summary.yaml
--rw-r--r--   0        0        0        1 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/src/gpt_review/repositories/__init__.py
--rw-r--r--   0        0        0      779 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/src/gpt_review/repositories/_repository.py
--rw-r--r--   0        0        0     6368 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/src/gpt_review/repositories/github.py
--rw-r--r--   0        0        0      863 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/src/gpt_review/utils.py
--rw-r--r--   0        0        0      218 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/tests/config.summary.test.yml
--rw-r--r--   0        0        0     5573 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/tests/conftest.py
--rw-r--r--   0        0        0      639 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/tests/mock.diff
--rw-r--r--   0        0        0      375 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/tests/test_context.py
--rw-r--r--   0        0        0      716 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/tests/test_git.py
--rw-r--r--   0        0        0     1452 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/tests/test_github.py
--rw-r--r--   0        0        0     5427 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0      684 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/tests/test_llama_index.py
--rw-r--r--   0        0        0     1449 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/tests/test_openai.py
--rw-r--r--   0        0        0     1015 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/tests/test_report.py
--rw-r--r--   0        0        0      807 2023-07-04 21:59:50.190143 gpt_review-0.9.5rc954.post1/tests/test_review.py
--rw-r--r--   0        0        0     5944 1970-01-01 00:00:00.000000 gpt_review-0.9.5rc954.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      766 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1977 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4301 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      671 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/.github/workflows/schedule-action-update.yml
+-rw-r--r--   0        0        0      314 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1888 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     2041 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/.pypirc
+-rw-r--r--   0        0        0       96 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/.vscode/extensions.json
+-rw-r--r--   0        0        0      530 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/.vscode/launch.json
+-rw-r--r--   0        0        0     1125 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/.vscode/settings.json
+-rw-r--r--   0        0        0      905 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/.vscode/tasks.json
+-rw-r--r--   0        0        0     1070 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/LICENSE
+-rw-r--r--   0        0        0     3556 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/README.md
+-rw-r--r--   0        0        0     2757 2023-07-13 02:33:18.670400 gpt_review-0.9.5rc965.post1/SECURITY.md
+-rw-r--r--   0        0        0     2307 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/action.yml
+-rw-r--r--   0        0        0      308 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/azure.yaml.template
+-rw-r--r--   0        0        0      218 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/config.summary.template.yml
+-rw-r--r--   0        0        0      362 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/prompt.template.yml
+-rw-r--r--   0        0        0     8725 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 02:33:35.914740 gpt_review-0.9.5rc965.post1/src/gpt/__init__.py
+-rw-r--r--   0        0        0      170 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt/__main__.py
+-rw-r--r--   0        0        0      366 2023-07-13 02:33:35.918741 gpt_review-0.9.5rc965.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0      170 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt_review/__main__.py
+-rw-r--r--   0        0        0     9452 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     3520 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt_review/_git.py
+-rw-r--r--   0        0        0     1453 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0     6437 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt_review/_llama_index.py
+-rw-r--r--   0        0        0     4315 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt_review/_openai.py
+-rw-r--r--   0        0        0     8692 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt_review/_review.py
+-rw-r--r--   0        0        0      980 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0     3349 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt_review/context.py
+-rw-r--r--   0        0        0      924 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0       33 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt_review/prompts/__init__.py
+-rw-r--r--   0        0        0     1246 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt_review/prompts/_prompt.py
+-rw-r--r--   0        0        0      362 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt_review/prompts/prompt_bug.yaml
+-rw-r--r--   0        0        0      327 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt_review/prompts/prompt_coverage.yaml
+-rw-r--r--   0        0        0      349 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt_review/prompts/prompt_summary.yaml
+-rw-r--r--   0        0        0        1 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt_review/repositories/__init__.py
+-rw-r--r--   0        0        0      779 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt_review/repositories/_repository.py
+-rw-r--r--   0        0        0     6368 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt_review/repositories/github.py
+-rw-r--r--   0        0        0      863 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/src/gpt_review/utils.py
+-rw-r--r--   0        0        0      218 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/tests/config.summary.test.yml
+-rw-r--r--   0        0        0     5573 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/tests/conftest.py
+-rw-r--r--   0        0        0      639 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/tests/mock.diff
+-rw-r--r--   0        0        0      375 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/tests/test_context.py
+-rw-r--r--   0        0        0      716 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/tests/test_git.py
+-rw-r--r--   0        0        0     1452 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/tests/test_github.py
+-rw-r--r--   0        0        0     5427 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0      684 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/tests/test_llama_index.py
+-rw-r--r--   0        0        0     1449 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/tests/test_openai.py
+-rw-r--r--   0        0        0     1015 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/tests/test_report.py
+-rw-r--r--   0        0        0      807 2023-07-13 02:33:18.674400 gpt_review-0.9.5rc965.post1/tests/test_review.py
+-rw-r--r--   0        0        0     5944 1970-01-01 00:00:00.000000 gpt_review-0.9.5rc965.post1/PKG-INFO
```

### Comparing `gpt_review-0.9.5rc954.post1/.devcontainer/devcontainer.json` & `gpt_review-0.9.5rc965.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt_review-0.9.5rc965.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/.github/dependabot.yml` & `gpt_review-0.9.5rc965.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/.github/pull_request_template.md` & `gpt_review-0.9.5rc965.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/.github/workflows/codeql.yml` & `gpt_review-0.9.5rc965.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/.github/workflows/dependency-review.yml` & `gpt_review-0.9.5rc965.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt_review-0.9.5rc965.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/.github/workflows/python.yml` & `gpt_review-0.9.5rc965.post1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/.github/workflows/schedule-action-update.yml` & `gpt_review-0.9.5rc965.post1/.github/workflows/schedule-action-update.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/.github/workflows/test-action.yml` & `gpt_review-0.9.5rc965.post1/.github/workflows/test-action.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,62 @@
-on: [pull_request_target]
+# Disable
+# on: [pull_request_target]
 
-jobs:
-  add_pr_comment:
-    permissions: write-all
-    runs-on: ubuntu-latest
-    name: OpenAI PR Comment
-    env:
-      GIT_COMMIT_HASH: ${{ github.event.pull_request.head.sha }}
-      GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-      PR_NUMBER: ${{ github.event.pull_request.number }}
-      PR_TITLE: ${{ github.event.pull_request.title }}
-      REPOSITORY_NAME: ${{ github.repository }}
-      AZURE_OPENAI_API: ${{ secrets.AZURE_OPENAI_API }}
-      AZURE_OPENAI_API_KEY: ${{ secrets.AZURE_OPENAI_API_KEY }}
-      LINK: "https://github.com/${{ github.repository }}/pull/${{ github.event.pull_request.number }}"
-      FILE_SUMMARY: false
-      TEST_SUMMARY: false
-      BUG_SUMMARY: false
-      RISK_SUMMARY: false
-      RISK_BREAKING: false
-
-    steps:
-      - uses: actions/checkout@v3
-        with:
-          ref: ${{ github.event.pull_request.head.sha }}
-
-      - name: Set up Python 3.11
-        uses: actions/setup-python@v4
-        with:
-          python-version: 3.11
-
-      - uses: Azure/login@v1.4.6
-        with:
-          creds: ${{ secrets.AZURE_CREDENTIALS }}
-
-      - run: |
-          sudo apt-get update
-          python3 -m venv .env
-          source .env/bin/activate
-          python -m pip install --upgrade pip
-          python -m pip install gpt-review\
-
-      - run: |
-          source .env/bin/activate
-
-          gpt github review \
-            --access-token $GITHUB_TOKEN \
-            --pull-request $PR_NUMBER \
-            --repository $REPOSITORY_NAME
-        continue-on-error: true
-
-      - run: |
-          source .env/bin/activate
-
-          pip install -e .
-
-          gpt github review \
-            --access-token $GITHUB_TOKEN \
-            --pull-request $PR_NUMBER \
-            --repository $REPOSITORY_NAME
+# jobs:
+#   add_pr_comment:
+#     permissions: write-all
+#     runs-on: ubuntu-latest
+#     name: OpenAI PR Comment
+#     env:
+#       GIT_COMMIT_HASH: ${{ github.event.pull_request.head.sha }}
+#       GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+#       PR_NUMBER: ${{ github.event.pull_request.number }}
+#       PR_TITLE: ${{ github.event.pull_request.title }}
+#       REPOSITORY_NAME: ${{ github.repository }}
+#       AZURE_OPENAI_API: ${{ secrets.AZURE_OPENAI_API }}
+#       AZURE_OPENAI_API_KEY: ${{ secrets.AZURE_OPENAI_API_KEY }}
+#       LINK: "https://github.com/${{ github.repository }}/pull/${{ github.event.pull_request.number }}"
+#       FILE_SUMMARY: false
+#       TEST_SUMMARY: false
+#       BUG_SUMMARY: false
+#       RISK_SUMMARY: false
+#       RISK_BREAKING: false
+
+#     steps:
+#       - uses: actions/checkout@v3
+#         with:
+#           ref: ${{ github.event.pull_request.head.sha }}
+
+#       - name: Set up Python 3.11
+#         uses: actions/setup-python@v4
+#         with:
+#           python-version: 3.11
+
+#       - uses: Azure/login@v1.4.6
+#         with:
+#           creds: ${{ secrets.AZURE_CREDENTIALS }}
+
+#       - run: |
+#           sudo apt-get update
+#           python3 -m venv .env
+#           source .env/bin/activate
+#           python -m pip install --upgrade pip
+#           python -m pip install gpt-review\
+
+#       - run: |
+#           source .env/bin/activate
+
+#           gpt github review \
+#             --access-token $GITHUB_TOKEN \
+#             --pull-request $PR_NUMBER \
+#             --repository $REPOSITORY_NAME
+#         continue-on-error: true
+
+#       - run: |
+#           source .env/bin/activate
+
+#           pip install -e .
+
+#           gpt github review \
+#             --access-token $GITHUB_TOKEN \
+#             --pull-request $PR_NUMBER \
+#             --repository $REPOSITORY_NAME
```

### Comparing `gpt_review-0.9.5rc954.post1/.gitignore` & `gpt_review-0.9.5rc965.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/.vscode/launch.json` & `gpt_review-0.9.5rc965.post1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/.vscode/settings.json` & `gpt_review-0.9.5rc965.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/.vscode/tasks.json` & `gpt_review-0.9.5rc965.post1/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/LICENSE` & `gpt_review-0.9.5rc965.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/README.md` & `gpt_review-0.9.5rc965.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/SECURITY.md` & `gpt_review-0.9.5rc965.post1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/action.yml` & `gpt_review-0.9.5rc965.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/pyproject.toml` & `gpt_review-0.9.5rc965.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/src/gpt_review/_ask.py` & `gpt_review-0.9.5rc965.post1/src/gpt_review/_ask.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/src/gpt_review/_git.py` & `gpt_review-0.9.5rc965.post1/src/gpt_review/_git.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/src/gpt_review/_gpt_cli.py` & `gpt_review-0.9.5rc965.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/src/gpt_review/_llama_index.py` & `gpt_review-0.9.5rc965.post1/src/gpt_review/_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/src/gpt_review/_openai.py` & `gpt_review-0.9.5rc965.post1/src/gpt_review/_openai.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/src/gpt_review/_review.py` & `gpt_review-0.9.5rc965.post1/src/gpt_review/_review.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/src/gpt_review/constants.py` & `gpt_review-0.9.5rc965.post1/src/gpt_review/constants.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/src/gpt_review/context.py` & `gpt_review-0.9.5rc965.post1/src/gpt_review/context.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/src/gpt_review/main.py` & `gpt_review-0.9.5rc965.post1/src/gpt_review/main.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/src/gpt_review/prompts/_prompt.py` & `gpt_review-0.9.5rc965.post1/src/gpt_review/prompts/_prompt.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/src/gpt_review/repositories/_repository.py` & `gpt_review-0.9.5rc965.post1/src/gpt_review/repositories/_repository.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/src/gpt_review/repositories/github.py` & `gpt_review-0.9.5rc965.post1/src/gpt_review/repositories/github.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/src/gpt_review/utils.py` & `gpt_review-0.9.5rc965.post1/src/gpt_review/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/tests/conftest.py` & `gpt_review-0.9.5rc965.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/tests/mock.diff` & `gpt_review-0.9.5rc965.post1/tests/mock.diff`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/tests/test_git.py` & `gpt_review-0.9.5rc965.post1/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/tests/test_github.py` & `gpt_review-0.9.5rc965.post1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/tests/test_gpt_cli.py` & `gpt_review-0.9.5rc965.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/tests/test_llama_index.py` & `gpt_review-0.9.5rc965.post1/tests/test_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/tests/test_openai.py` & `gpt_review-0.9.5rc965.post1/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/tests/test_report.py` & `gpt_review-0.9.5rc965.post1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/tests/test_review.py` & `gpt_review-0.9.5rc965.post1/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.5rc954.post1/PKG-INFO` & `gpt_review-0.9.5rc965.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.9.5rc954.post1
+Version: 0.9.5rc965.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gpt-review Version: 0.9.5rc954.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.9.5rc965.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.8.1 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

