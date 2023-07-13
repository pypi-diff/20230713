# Comparing `tmp/crackerjack-0.3.6.tar.gz` & `tmp/crackerjack-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.3.6.tar", last modified: Sat Jul  8 10:46:01 2023, max compression
+gzip compressed data, was "crackerjack-0.3.7.tar", last modified: Thu Jul 13 14:04:55 2023, max compression
```

## Comparing `crackerjack-0.3.6.tar` & `crackerjack-0.3.7.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.3.6/LICENSE
--rw-r--r--   0        0        0     5917 2023-06-18 16:33:36.904528 crackerjack-0.3.6/README.md
--rw-r--r--   0        0        0        0 2023-07-08 10:08:28.778621 crackerjack-0.3.6/crackerjack/.crackerjack-config.yaml
--rw-r--r--   0        0        0      255 2023-07-08 10:08:28.722503 crackerjack-0.3.6/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2023-07-08 10:08:28.763421 crackerjack-0.3.6/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     2917 2023-07-08 10:08:28.745489 crackerjack-0.3.6/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0    15547 2023-06-18 10:35:54.994502 crackerjack-0.3.6/crackerjack/.pyanalyze-report.json
--rw-r--r--   0        0        0     8180 2023-06-18 10:35:54.997907 crackerjack-0.3.6/crackerjack/.pyanalyze-report.md
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.3.6/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.3.6/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.3.6/crackerjack/__init__.py
--rw-r--r--   0        0        0     1559 2023-07-07 13:10:39.683493 crackerjack-0.3.6/crackerjack/__main__.py
--rw-r--r--   0        0        0     6157 2023-07-08 10:44:25.772068 crackerjack-0.3.6/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     1659 2023-07-08 10:08:29.586215 crackerjack-0.3.6/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     2010 2023-07-08 10:46:01.423860 crackerjack-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     6910 1970-01-01 00:00:00.000000 crackerjack-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.3.7/LICENSE
+-rw-r--r--   0        0        0     5917 2023-06-18 16:33:36.904528 crackerjack-0.3.7/README.md
+-rw-r--r--   0        0        0      243 2023-07-13 14:00:32.056242 crackerjack-0.3.7/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2023-07-13 14:00:32.094427 crackerjack-0.3.7/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     2918 2023-07-13 14:00:32.078277 crackerjack-0.3.7/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    15547 2023-06-18 10:35:54.994502 crackerjack-0.3.7/crackerjack/.pyanalyze-report.json
+-rw-r--r--   0        0        0     8180 2023-06-18 10:35:54.997907 crackerjack-0.3.7/crackerjack/.pyanalyze-report.md
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.3.7/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.3.7/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.3.7/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1559 2023-07-07 13:10:39.683493 crackerjack-0.3.7/crackerjack/__main__.py
+-rw-r--r--   0        0        0     6120 2023-07-09 13:10:21.246677 crackerjack-0.3.7/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     1659 2023-07-13 14:00:32.992392 crackerjack-0.3.7/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     2010 2023-07-13 14:04:55.130236 crackerjack-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     6910 1970-01-01 00:00:00.000000 crackerjack-0.3.7/PKG-INFO
```

### Comparing `crackerjack-0.3.6/LICENSE` & `crackerjack-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.6/README.md` & `crackerjack-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.6/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.3.7/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.6/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.3.7/crackerjack/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,29 +13,29 @@
       - id: check-yaml
         name: check-yaml
       - id: check-toml
         name: check-toml
       - id: check-added-large-files
         name: check-added-large-files
   - repo: https://github.com/psf/black
-    rev: '23.3.0'
+    rev: '23.7.0'
     hooks:
       - id: black
         language_version: python3.11
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.277
+    rev: v0.0.278
     hooks:
       - id: ruff
   - repo: https://github.com/fredrikaverpil/creosote
-    rev: v2.6.2
+    rev: v2.6.3
     hooks:
       - id: creosote
         args: [--paths, "crackerjack", --exclude-deps, "pdm-bump", "tomli-w"]
   - repo: https://github.com/ikamensh/flynt/
-    rev: '0.78'
+    rev: '1.0.0'
     hooks:
       - id: flynt
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.5
     hooks:
       - id: codespell
         additional_dependencies:
@@ -69,33 +69,33 @@
           - autotyping>=23.3.0
           - libcst>=0.4.9
   - repo: https://github.com/dosisod/refurb
     rev: v1.17.0
     hooks:
       - id: refurb
   - repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.316
+    rev: v1.1.317
     hooks:
       - id: pyright
   #  - repo: https://github.com/pdoc3/pdoc
   #    rev: master
   #    hooks:
   #      - id: pdoc
   #        name: pdoc
   #        entry: pdoc --html -f -o docs module1 module2 module3
   #        language_version: python3.11
   #        require_serial: true
   #        types: [ python ]
   #        always_run: true
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.277
+    rev: v0.0.278
     hooks:
       - id: ruff
   - repo: https://github.com/psf/black
-    rev: '23.3.0'
+    rev: '23.7.0'
     hooks:
       - id: black
         language_version: python3.11
   - repo: https://github.com/pdm-project/pdm
     rev: 2.8.0a2 # a PDM release exposing the hook
     hooks:
       - id: pdm-export
```

### Comparing `crackerjack-0.3.6/crackerjack/.pyanalyze-report.json` & `crackerjack-0.3.7/crackerjack/.pyanalyze-report.json`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.6/crackerjack/.pyanalyze-report.md` & `crackerjack-0.3.7/crackerjack/.pyanalyze-report.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.6/crackerjack/__main__.py` & `crackerjack-0.3.7/crackerjack/__main__.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.6/crackerjack/crackerjack.py` & `crackerjack-0.3.7/crackerjack/crackerjack.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,14 @@
                 await file.unlink()
 
     async def copy_configs(self) -> None:
         config_files = (
             ".gitignore",
             ".pre-commit-config.yaml",
             ".libcst.codemod.yaml",
-            ".crackerjack-config.yaml",
             ".pyanalyze-report.json",
             ".pyanalyze-report.md",
         )
         for config in config_files:
             config_path = self.our_path.parent / config
             pkg_config_path = self.pkg_path / config
             await pkg_config_path.touch(exist_ok=True)
@@ -111,15 +110,15 @@
             run(["pdm", "config", "python.use_venv", "false"])
             run(["git", "init"])
             run(["git", "branch", "-m", "main"])
             run(["git", "add", "pyproject.toml"])
             run(["pdm", "add", "-d", "pre_commit"])
             run(["pre-commit", "install"])
             run(["git", "add", "pdm.lock"])
-            run(["git", "config advice.addIgnoredFile", "false"])
+            run(["git", "config", "advice.addIgnoredFile", "false"])
         await self.update_pyproject_configs()
 
     async def process(self, options: t.Any) -> None:
         imp_dir = self.pkg_path / "__pypackages__"
         sys.path.append(str(imp_dir))
         self.pkg_name = underscore(self.pkg_path.stem.lower())
         self.pkg_dir = self.pkg_path / self.pkg_name
```

### Comparing `crackerjack-0.3.6/crackerjack/pyproject.toml` & `crackerjack-0.3.7/crackerjack/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.3.6"
+version = "0.3.7"
 description = "Crackerjack code style"
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
```

### Comparing `crackerjack-0.3.6/pyproject.toml` & `crackerjack-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.3.6"
+version = "0.3.7"
 description = "Crackerjack code style"
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
```

### Comparing `crackerjack-0.3.6/PKG-INFO` & `crackerjack-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Crackerjack
-Version: 0.3.6
+Version: 0.3.7
 Summary: Crackerjack code style
 Keywords: black ruff mypy creosote refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
```

