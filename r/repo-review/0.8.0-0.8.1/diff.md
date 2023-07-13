# Comparing `tmp/repo_review-0.8.0.tar.gz` & `tmp/repo_review-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu Jun 29 13:59:05 2023, max compression
+gzip compressed data, last modified: Thu Jul 13 17:42:45 2023, max compression
```

## Comparing `repo_review-0.8.0.tar` & `repo_review-0.8.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      125 2023-06-29 13:59:05.000000 repo_review-0.8.0/.git_archival.txt
--rw-r--r--   0        0        0       32 2023-06-29 13:59:05.000000 repo_review-0.8.0/.gitattributes
--rw-r--r--   0        0        0     2061 2023-06-29 13:59:05.000000 repo_review-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      187 2023-06-29 13:59:05.000000 repo_review-0.8.0/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      400 2023-06-29 13:59:05.000000 repo_review-0.8.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1216 2023-06-29 13:59:05.000000 repo_review-0.8.0/action.yml
--rw-r--r--   0        0        0     3242 2023-06-29 13:59:05.000000 repo_review-0.8.0/noxfile.py
--rw-r--r--   0        0        0      359 2023-06-29 13:59:05.000000 repo_review-0.8.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     2527 2023-06-29 13:59:05.000000 repo_review-0.8.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2023-06-29 13:59:05.000000 repo_review-0.8.0/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2023-06-29 13:59:05.000000 repo_review-0.8.0/.github/matchers/pylint.json
--rw-r--r--   0        0        0      669 2023-06-29 13:59:05.000000 repo_review-0.8.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0     2356 2023-06-29 13:59:05.000000 repo_review-0.8.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0        0 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/.nojekyll
--rw-r--r--   0        0        0      217 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/changelog.md
--rw-r--r--   0        0        0     5910 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/checks.md
--rw-r--r--   0        0        0      990 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/cli.md
--rw-r--r--   0        0        0     1009 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/conf.py
--rw-r--r--   0        0        0     1236 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/families.md
--rw-r--r--   0        0        0     2243 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/fixtures.md
--rw-r--r--   0        0        0     1919 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/index.html
--rw-r--r--   0        0        0      253 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/index.md
--rw-r--r--   0        0        0     2248 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/intro.md
--rw-r--r--   0        0        0     2746 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/plugins.md
--rw-r--r--   0        0        0     2801 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/programmatic.md
--rw-r--r--   0        0        0    10215 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/webapp.js
--rw-r--r--   0        0        0     1770 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/webapp.md
--rw-r--r--   0        0        0     1033 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/api/repo_review.rst
--rw-r--r--   0        0        0      230 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/__init__.py
--rw-r--r--   0        0        0     7626 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/__main__.py
--rw-r--r--   0        0        0      160 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/_version.py
--rw-r--r--   0        0        0      118 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/_version.pyi
--rw-r--r--   0        0        0     3576 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/checks.py
--rw-r--r--   0        0        0     1591 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/families.py
--rw-r--r--   0        0        0     3607 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/fixtures.py
--rw-r--r--   0        0        0     6010 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/ghpath.py
--rw-r--r--   0        0        0     2315 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/html.py
--rw-r--r--   0        0        0     7410 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/processor.py
--rw-r--r--   0        0        0        0 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/py.typed
--rw-r--r--   0        0        0        0 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/_compat/__init__.py
--rw-r--r--   0        0        0      233 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/_compat/tomllib.py
--rw-r--r--   0        0        0      246 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/_compat/typing.py
--rw-r--r--   0        0        0        0 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/_compat/importlib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/_compat/importlib/resources/__init__.py
--rw-r--r--   0        0        0      256 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/_compat/importlib/resources/abc.py
--rw-r--r--   0        0        0     4393 2023-06-29 13:59:05.000000 repo_review-0.8.0/tests/test_checks.py
--rw-r--r--   0        0        0      904 2023-06-29 13:59:05.000000 repo_review-0.8.0/tests/test_cmd.py
--rw-r--r--   0        0        0     2460 2023-06-29 13:59:05.000000 repo_review-0.8.0/tests/test_fixtures.py
--rw-r--r--   0        0        0      598 2023-06-29 13:59:05.000000 repo_review-0.8.0/tests/test_package.py
--rw-r--r--   0        0        0     2185 2023-06-29 13:59:05.000000 repo_review-0.8.0/tests/test_self.py
--rw-r--r--   0        0        0     3981 2023-06-29 13:59:05.000000 repo_review-0.8.0/tests/test_utilities/pyproject.py
--rw-r--r--   0        0        0      333 2023-06-29 13:59:05.000000 repo_review-0.8.0/tests/test_utilities/pyproject.toml
--rw-r--r--   0        0        0     2086 2023-06-29 13:59:05.000000 repo_review-0.8.0/.gitignore
--rw-r--r--   0        0        0     1525 2023-06-29 13:59:05.000000 repo_review-0.8.0/LICENSE
--rw-r--r--   0        0        0     6123 2023-06-29 13:59:05.000000 repo_review-0.8.0/README.md
--rw-r--r--   0        0        0     5262 2023-06-29 13:59:05.000000 repo_review-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     8397 2023-06-29 13:59:05.000000 repo_review-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-07-13 17:42:45.000000 repo_review-0.8.1/.git_archival.txt
+-rw-r--r--   0        0        0       32 2023-07-13 17:42:45.000000 repo_review-0.8.1/.gitattributes
+-rw-r--r--   0        0        0     2045 2023-07-13 17:42:45.000000 repo_review-0.8.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      187 2023-07-13 17:42:45.000000 repo_review-0.8.1/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      400 2023-07-13 17:42:45.000000 repo_review-0.8.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1216 2023-07-13 17:42:45.000000 repo_review-0.8.1/action.yml
+-rw-r--r--   0        0        0     3242 2023-07-13 17:42:45.000000 repo_review-0.8.1/noxfile.py
+-rw-r--r--   0        0        0      359 2023-07-13 17:42:45.000000 repo_review-0.8.1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     2527 2023-07-13 17:42:45.000000 repo_review-0.8.1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2023-07-13 17:42:45.000000 repo_review-0.8.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2023-07-13 17:42:45.000000 repo_review-0.8.1/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      669 2023-07-13 17:42:45.000000 repo_review-0.8.1/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     2356 2023-07-13 17:42:45.000000 repo_review-0.8.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        0 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/.nojekyll
+-rw-r--r--   0        0        0      217 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/changelog.md
+-rw-r--r--   0        0        0     5910 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/checks.md
+-rw-r--r--   0        0        0      990 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/cli.md
+-rw-r--r--   0        0        0     1009 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/conf.py
+-rw-r--r--   0        0        0     1236 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/families.md
+-rw-r--r--   0        0        0     2243 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/fixtures.md
+-rw-r--r--   0        0        0     1915 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/index.html
+-rw-r--r--   0        0        0      253 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/index.md
+-rw-r--r--   0        0        0     2248 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/intro.md
+-rw-r--r--   0        0        0     2746 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/plugins.md
+-rw-r--r--   0        0        0     2821 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/programmatic.md
+-rw-r--r--   0        0        0    10563 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/webapp.js
+-rw-r--r--   0        0        0     1770 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/webapp.md
+-rw-r--r--   0        0        0     1033 2023-07-13 17:42:45.000000 repo_review-0.8.1/docs/api/repo_review.rst
+-rw-r--r--   0        0        0      230 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/__init__.py
+-rw-r--r--   0        0        0     7626 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/__main__.py
+-rw-r--r--   0        0        0      160 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/_version.py
+-rw-r--r--   0        0        0      118 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/_version.pyi
+-rw-r--r--   0        0        0     3576 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/checks.py
+-rw-r--r--   0        0        0     1591 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/families.py
+-rw-r--r--   0        0        0     3607 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/fixtures.py
+-rw-r--r--   0        0        0     6010 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/ghpath.py
+-rw-r--r--   0        0        0     2315 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/html.py
+-rw-r--r--   0        0        0     7393 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/processor.py
+-rw-r--r--   0        0        0        0 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/py.typed
+-rw-r--r--   0        0        0        0 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0      246 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/_compat/typing.py
+-rw-r--r--   0        0        0        0 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2023-07-13 17:42:45.000000 repo_review-0.8.1/src/repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0     4393 2023-07-13 17:42:45.000000 repo_review-0.8.1/tests/test_checks.py
+-rw-r--r--   0        0        0      904 2023-07-13 17:42:45.000000 repo_review-0.8.1/tests/test_cmd.py
+-rw-r--r--   0        0        0     2429 2023-07-13 17:42:45.000000 repo_review-0.8.1/tests/test_fixtures.py
+-rw-r--r--   0        0        0      598 2023-07-13 17:42:45.000000 repo_review-0.8.1/tests/test_package.py
+-rw-r--r--   0        0        0     2185 2023-07-13 17:42:45.000000 repo_review-0.8.1/tests/test_self.py
+-rw-r--r--   0        0        0     4029 2023-07-13 17:42:45.000000 repo_review-0.8.1/tests/test_utilities/pyproject.py
+-rw-r--r--   0        0        0      333 2023-07-13 17:42:45.000000 repo_review-0.8.1/tests/test_utilities/pyproject.toml
+-rw-r--r--   0        0        0     2086 2023-07-13 17:42:45.000000 repo_review-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1525 2023-07-13 17:42:45.000000 repo_review-0.8.1/LICENSE
+-rw-r--r--   0        0        0     6123 2023-07-13 17:42:45.000000 repo_review-0.8.1/README.md
+-rw-r--r--   0        0        0     5359 2023-07-13 17:42:45.000000 repo_review-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     8397 2023-07-13 17:42:45.000000 repo_review-0.8.1/PKG-INFO
```

### Comparing `repo_review-0.8.0/.pre-commit-config.yaml` & `repo_review-0.8.1/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 ci:
   autoupdate_commit_msg: "chore(deps): update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black-jupyter
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: 1.13.0
+    rev: 1.15.0
     hooks:
       - id: blacken-docs
-        additional_dependencies: [black==23.1.0]
+        additional_dependencies: [black==23.7.0]
 
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.270"
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: "v0.0.277"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.9-for-vscode"
+    rev: "v3.0.0"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
@@ -44,35 +44,35 @@
     rev: v1.10.0
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.3.0
+    rev: v1.4.1
     hooks:
       - id: mypy
         files: (src|web|tests)
         args: []
         additional_dependencies:
-          - click
+          - click==8.1.3
           - markdown-it-py
           - pytest
           - rich
           - tomli
           - types-PyYAML
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.4
+    rev: v2.2.5
     hooks:
       - id: codespell
         args: ["-Lhist,absense"]
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: v0.9.0.2
+    rev: v0.9.0.5
     hooks:
       - id: shellcheck
 
   - repo: local
     hooks:
       - id: disallow-caps
         name: Disallow improper capitalization
```

### Comparing `repo_review-0.8.0/action.yml` & `repo_review-0.8.1/action.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/noxfile.py` & `repo_review-0.8.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/.github/CONTRIBUTING.md` & `repo_review-0.8.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/.github/matchers/pylint.json` & `repo_review-0.8.1/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/.github/workflows/cd.yml` & `repo_review-0.8.1/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/.github/workflows/ci.yml` & `repo_review-0.8.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/docs/checks.md` & `repo_review-0.8.1/docs/checks.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/docs/cli.md` & `repo_review-0.8.1/docs/cli.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/docs/conf.py` & `repo_review-0.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/docs/families.md` & `repo_review-0.8.1/docs/families.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/docs/fixtures.md` & `repo_review-0.8.1/docs/fixtures.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/docs/index.html` & `repo_review-0.8.1/docs/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -59,13 +59,13 @@
   <body>
     <div id="root">Loading...</div>
     <script type="text/babel">
       const root = ReactDOM.createRoot(document.getElementById("root"));
       root.render(
         <App
           header={true}
-          deps={["sp-repo-review==2023.06.17", "repo-review>=0.7,<=0.9"]}
+          deps={["sp-repo-review==2023.06.29", "repo-review==0.8.0"]}
         />,
       );
     </script>
   </body>
 </html>
```

### Comparing `repo_review-0.8.0/docs/intro.md` & `repo_review-0.8.1/docs/intro.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/docs/plugins.md` & `repo_review-0.8.1/docs/plugins.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/docs/programmatic.md` & `repo_review-0.8.1/docs/programmatic.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,50 +25,58 @@
 A common requirement is getting the "nice" family name given the short name.
 There's a tiny helper for this, {func}`repo_review.families.get_family_name`:
 
 ```python
 family_name = get_family_name(families, family)
 ```
 
-.. versionadded:: 0.8
+```{versionadded} 0.8
+
+```
 
 ## Listing all possible checks
 
 You can also get a list of checks:
 
 ```python
 collected = repo_review.processor.collect_all()
 ```
 
 This returns a {class}`~repo_review.processor.CollectionReturn`. You can access the `.checks`,
 `.families`, and `.fixtures`, all are dicts.
 
-.. versionadded:: 0.8
+```{versionadded} 0.8
+
+```
 
 ### Getting the check properties
 
 A common requirement is getting the url from the
 {class}`~repo_review.checks.Check`. While a
 {class}`~repo_review.processor.Result` already has the URL fully rendered,
 checks do not; they are directly returned by plugins. There's a tiny helper
 for this, {func}`repo_review.checks.get_check_url`:
 
 ```python
 url = get_check_url(name, check)
 ```
 
-.. versionadded:: 0.8
+```{versionadded} 0.8
+
+```
 
 You can also use a helper to get `__doc__` with the correct substitution, as well:
 
 ```python
 doc = get_check_description(name, check)
 ```
 
-.. versionadded:: 0.8
+```{versionadded} 0.8
+
+```
 
 ### Example: cog
 
 Here's an example of using this to fill out a README with [`cog`][], formatting all possible checks in markdown:
 
 ```md
 <!-- [[[cog
```

### Comparing `repo_review-0.8.0/docs/webapp.js` & `repo_review-0.8.1/docs/webapp.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -312,35 +312,35 @@
             progress: true,
         });
         const state = this.state;
         this.pyodide_promise.then((pyodide) => {
             var families_checks;
             try {
                 families_checks = pyodide.runPython(`
-            from pyodide.http import open_url
-            from repo_review.processor import process
-            from repo_review.ghpath import GHPath
-
-            GHPath.open_url = staticmethod(open_url)
-
-            package = GHPath(repo="${state.repo}", branch="${state.branch}")
-            process(package)
-        `);
+          from pyodide.http import open_url
+          from repo_review.processor import process
+          from repo_review.ghpath import GHPath
+
+          GHPath.open_url = staticmethod(open_url)
+
+          package = GHPath(repo="${state.repo}", branch="${state.branch}")
+          process(package)
+          `);
             } catch (e) {
                 if (e.message.includes("KeyError: 'tree'")) {
                     this.setState({
                         msg: DEFAULT_MSG,
                         progress: false,
                         err_msg: "Invalid repository or branch. Please try again.",
                     });
                     return;
                 }
                 this.setState({
                     progress: false,
-                    err_msg: e.message,
+                    err_msg: `<pre><code>${e.message}</code><pre>`,
                 });
                 return;
             }
 
             const families_dict = families_checks.get(0);
             const results_list = families_checks.get(1);
 
@@ -406,14 +406,20 @@
             MaterialUI.TextField id = "repo-select"
             label = "Org/Repo"
             helperText = "e.g. scikit-hep/hist"
             variant = "outlined"
             autoFocus = {
                 true
             }
+            onKeyDown = {
+                (e) => {
+                    if (event.keyCode === 13)
+                        document.getElementById("branch-select").focus();
+                }
+            }
             onInput = {
                 (e) => this.setState({
                     repo: e.target.value
                 })
             }
             defaultValue = {
                 urlParams.get("repo")
@@ -427,14 +433,19 @@
             MaterialUI.Autocomplete disablePortal id = "branch-select"
             options = {
                 common_branches
             }
             freeSolo = {
                 true
             }
+            onKeyDown = {
+                (e) => {
+                    if (event.keyCode === 13) this.handleCompute();
+                }
+            }
             onInputChange = {
                 (e, value) => this.setState({
                     branch: value
                 })
             }
             defaultValue = {
                 urlParams.get("branch")
@@ -488,21 +499,21 @@
             /MaterialUI.Typography> {
                 this.state.progress && < MaterialUI.LinearProgress / >
             } {
                 this.state.err_msg && ( <
                     MaterialUI.Typography variant = "body1"
                     component = "div"
                     color = "error" >
-                    {
-                        " "
-                    } {
-                        this.state.err_msg
-                    } {
-                        " "
-                    } <
+                    <
+                    span dangerouslySetInnerHTML = {
+                        {
+                            __html: this.state.err_msg
+                        }
+                    }
+                    /> <
                     /MaterialUI.Typography>
                 )
             } <
             /MaterialUI.Box> <
             Results results = {
                 this.state.results
             }
```

### Comparing `repo_review-0.8.0/docs/webapp.md` & `repo_review-0.8.1/docs/webapp.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/docs/api/repo_review.rst` & `repo_review-0.8.1/docs/api/repo_review.rst`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/src/repo_review/__main__.py` & `repo_review-0.8.1/src/repo_review/__main__.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/src/repo_review/checks.py` & `repo_review-0.8.1/src/repo_review/checks.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/src/repo_review/families.py` & `repo_review-0.8.1/src/repo_review/families.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/src/repo_review/fixtures.py` & `repo_review-0.8.1/src/repo_review/fixtures.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/src/repo_review/ghpath.py` & `repo_review-0.8.1/src/repo_review/ghpath.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/src/repo_review/html.py` & `repo_review-0.8.1/src/repo_review/html.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/src/repo_review/processor.py` & `repo_review-0.8.1/src/repo_review/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     }
     # Keep track of which checks have been completed
     completed: dict[str, str | None] = {}
 
     # Run all the checks in topological order based on their dependencies
     ts = graphlib.TopologicalSorter(graph)
     for name in ts.static_order():
-        if all(completed.get(n, "") == "" for n in graph[name]):  # noqa: PLC1901
+        if all(completed.get(n, "") == "" for n in graph[name]):
             result = apply_fixtures(fixtures, tasks[name].check)
             if isinstance(result, bool):
                 completed[name] = "" if result else tasks[name].check.__doc__
             else:
                 completed[name] = result
         else:
             completed[name] = None
```

### Comparing `repo_review-0.8.0/tests/test_checks.py` & `repo_review-0.8.1/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/tests/test_cmd.py` & `repo_review-0.8.1/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/tests/test_fixtures.py` & `repo_review-0.8.1/tests/test_fixtures.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             "nothing": nothing,
             "not_simple": not_simple,
         },
     )
 
     assert apply_fixtures(fixtures, nothing) == 42
     assert apply_fixtures(fixtures, simple) == "."
-    assert apply_fixtures(fixtures, lambda package: package) == Path(".")  # type: ignore[no-any-return]
+    assert apply_fixtures(fixtures, lambda package: package) == Path(".")
     assert apply_fixtures(fixtures, not_simple) == ". ."
 
 
 @pytest.mark.parametrize("some_bool", [True, False])
 def test_process_checks(monkeypatch: pytest.MonkeyPatch, some_bool: bool) -> None:
     ep = importlib.metadata.EntryPoint(name="x", group="y", value="test_module:f")
     sys.modules["test_module"] = ModuleType("test_module")
```

### Comparing `repo_review-0.8.0/tests/test_package.py` & `repo_review-0.8.1/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/tests/test_self.py` & `repo_review-0.8.1/tests/test_self.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/tests/test_utilities/pyproject.py` & `repo_review-0.8.1/tests/test_utilities/pyproject.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 class PyProject:
     family = "pyproject"
 
 
 class PP002(PyProject):
     "Has a proper build-system table"
 
-    requires = {"PY001"}
+    requires = frozenset(("PY001",))
     url = "https://packaging.python.org/en/latest/specifications/declaring-build-dependencies"
 
     @staticmethod
     def check(pyproject: dict[str, Any]) -> bool:
         """
         Must have `build-system.requires` *and* `build-system.backend`. Both
         should be present in all modern packages.
@@ -86,15 +86,15 @@
             case _:
                 return False
 
 
 class PP003(PyProject):
     "Does not list wheel as a build-dep"
 
-    requires = {"PY001"}
+    requires = frozenset(("PY001",))
 
     @staticmethod
     def check(pyproject: dict[str, Any]) -> bool:
         """
         Do not include `"wheel"` in your `build-system.requires`, setuptools
         does this via PEP 517 already. Setuptools will also only require this
         for actual wheel builds, and might have version limits.
@@ -106,15 +106,15 @@
             case _:
                 return False
 
 
 class PP301(PyProject):
     "Has pytest in pyproject"
 
-    requires = {"PY001"}
+    requires = frozenset(("PY001",))
 
     @staticmethod
     def check(pyproject: dict[str, Any]) -> bool:
         """
         Must have a pytest configuration section in pyproject.toml. If you must
         have it somewhere else (such as to support `pytest<6`), ignore this
         check.
@@ -125,15 +125,15 @@
                 return True
             case _:
                 return False
 
 
 class PP302(PyProject):
     "Sets a minimum pytest to at least 6"
-    requires = {"PP301"}
+    requires = frozenset(("PP301",))
 
     @staticmethod
     def check(pyproject: dict[str, Any]) -> bool:
         """
         Must have a `minversion=`, and must be at least 6 (first version to
         support `pyproject.toml` configuration).
         """
```

### Comparing `repo_review-0.8.0/.gitignore` & `repo_review-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/LICENSE` & `repo_review-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/README.md` & `repo_review-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.8.0/pyproject.toml` & `repo_review-0.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -178,7 +178,10 @@
 "typing.assert_never".msg = "Use repo_review._compat.typing.assert_never instead."
 "importlib.abc".msg = "Use repo_review._compat.importlib.resources.abc instead."
 "importlib.resources.abc".msg = "Use repo_review._compat.importlib.resources.abc instead."
 
 [tool.ruff.per-file-ignores]
 "src/repo_review/_compat/**.py" = ["TID251"]
 "src/**/__main__.py" = ["T20"]
+
+[tool.repo-review]
+ignore = ["PC190"]  # Remove after first July 2023 release of sp-repo-review
```

### Comparing `repo_review-0.8.0/PKG-INFO` & `repo_review-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo_review
-Version: 0.8.0
+Version: 0.8.1
 Summary: Framework that can run checks on repos
 Project-URL: Changelog, https://github.com/scientific-python/repo-review/releases
 Project-URL: Demo, https://scientific-python.github.io/repo-review
 Project-URL: Documentation, https://repo-review.readthedocs.io
 Project-URL: Homepage, https://repo-review.readthedocs.io
 Project-URL: Source, https://github.com/scientific-python/repo-review
 Author-email: Henry Schreiner <henryfs@princeton.edu>
```

