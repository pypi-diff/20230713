# Comparing `tmp/jupyterlab_commands-0.3.4.tar.gz` & `tmp/jupyterlab_commands-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_commands-0.3.4.tar", last modified: Mon Apr 11 19:07:55 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jupyterlab_commands-0.3.4.tar` & `jupyterlab_commands-0.4.0.tar`

### file list

```diff
@@ -1,54 +1,38 @@
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-04-11 19:07:55.123019 jupyterlab_commands-0.3.4/
--rw-r--r--   0 timkpaine   (501) staff       (20)     3352 2021-01-02 20:27:13.000000 jupyterlab_commands-0.3.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 timkpaine   (501) staff       (20)     1954 2019-08-15 22:58:05.000000 jupyterlab_commands-0.3.4/CONTRIBUTING.md
--rw-r--r--   0 timkpaine   (501) staff       (20)    11362 2019-08-15 22:58:05.000000 jupyterlab_commands-0.3.4/LICENSE
--rw-r--r--   0 timkpaine   (501) staff       (20)      613 2022-04-11 19:07:13.000000 jupyterlab_commands-0.3.4/MANIFEST.in
--rw-r--r--   0 timkpaine   (501) staff       (20)     2230 2022-04-11 19:07:13.000000 jupyterlab_commands-0.3.4/Makefile
--rw-r--r--   0 timkpaine   (501) staff       (20)     3426 2022-04-11 19:07:55.123189 jupyterlab_commands-0.3.4/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)     2581 2021-02-01 03:31:52.000000 jupyterlab_commands-0.3.4/README.md
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-04-11 19:07:55.106495 jupyterlab_commands-0.3.4/js/
--rw-r--r--   0 timkpaine   (501) staff       (20)     6148 2021-11-30 03:27:21.000000 jupyterlab_commands-0.3.4/js/.DS_Store
--rw-r--r--   0 timkpaine   (501) staff       (20)     1345 2022-04-03 01:58:53.000000 jupyterlab_commands-0.3.4/js/.eslintrc.js
--rw-r--r--   0 timkpaine   (501) staff       (20)      154 2021-11-30 03:49:42.000000 jupyterlab_commands-0.3.4/js/babel.config.js
--rw-r--r--   0 timkpaine   (501) staff       (20)      520 2021-11-30 04:15:13.000000 jupyterlab_commands-0.3.4/js/jest.config.js
--rw-r--r--   0 timkpaine   (501) staff       (20)     2201 2022-04-11 19:07:13.000000 jupyterlab_commands-0.3.4/js/package.json
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-04-11 19:07:55.110646 jupyterlab_commands-0.3.4/js/src/
--rw-r--r--   0 timkpaine   (501) staff       (20)     2645 2021-11-30 04:15:13.000000 jupyterlab_commands-0.3.4/js/src/index.js
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-04-11 19:07:55.111395 jupyterlab_commands-0.3.4/js/style/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2021-11-30 03:49:42.000000 jupyterlab_commands-0.3.4/js/style/index.css
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-04-11 19:07:55.114627 jupyterlab_commands-0.3.4/js/tests/
--rw-r--r--   0 timkpaine   (501) staff       (20)      171 2021-11-30 04:15:13.000000 jupyterlab_commands-0.3.4/js/tests/activate.test.js
--rw-r--r--   0 timkpaine   (501) staff       (20)      177 2021-11-30 04:15:13.000000 jupyterlab_commands-0.3.4/js/tests/assetsTransformer.js
--rw-r--r--   0 timkpaine   (501) staff       (20)      174 2021-11-30 04:15:13.000000 jupyterlab_commands-0.3.4/js/tests/export.test.js
--rw-r--r--   0 timkpaine   (501) staff       (20)       35 2021-11-30 03:49:42.000000 jupyterlab_commands-0.3.4/js/tests/fileMock.js
--rw-r--r--   0 timkpaine   (501) staff       (20)       21 2021-11-30 03:49:42.000000 jupyterlab_commands-0.3.4/js/tests/styleMock.js
--rw-r--r--   0 timkpaine   (501) staff       (20)   437555 2022-04-03 02:14:27.000000 jupyterlab_commands-0.3.4/js/yarn.lock
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-04-11 19:07:55.115857 jupyterlab_commands-0.3.4/jupyterlab_commands/
--rw-r--r--   0 timkpaine   (501) staff       (20)      146 2021-01-02 20:27:13.000000 jupyterlab_commands-0.3.4/jupyterlab_commands/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)       22 2022-04-11 19:07:13.000000 jupyterlab_commands-0.3.4/jupyterlab_commands/_version.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-04-11 19:07:55.118237 jupyterlab_commands-0.3.4/jupyterlab_commands/extension/
--rw-r--r--   0 timkpaine   (501) staff       (20)       93 2022-04-03 01:58:53.000000 jupyterlab_commands-0.3.4/jupyterlab_commands/extension/jupyterlab_commands.json
--rw-r--r--   0 timkpaine   (501) staff       (20)     2068 2021-01-02 20:27:13.000000 jupyterlab_commands-0.3.4/jupyterlab_commands/extension.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-04-11 19:07:55.118868 jupyterlab_commands-0.3.4/jupyterlab_commands/labextension/
--rw-r--r--   0 timkpaine   (501) staff       (20)     2317 2022-04-11 19:07:39.000000 jupyterlab_commands-0.3.4/jupyterlab_commands/labextension/package.json
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-04-11 19:07:55.121012 jupyterlab_commands-0.3.4/jupyterlab_commands/labextension/static/
--rw-r--r--   0 timkpaine   (501) staff       (20)     4771 2022-04-11 19:07:39.000000 jupyterlab_commands-0.3.4/jupyterlab_commands/labextension/static/568.ae9692e317badeae2b0e.js
--rw-r--r--   0 timkpaine   (501) staff       (20)     2144 2022-04-11 19:07:39.000000 jupyterlab_commands-0.3.4/jupyterlab_commands/labextension/static/873.af0a6b8becacd1ba8457.js
--rw-r--r--   0 timkpaine   (501) staff       (20)     6894 2022-04-11 19:07:39.000000 jupyterlab_commands-0.3.4/jupyterlab_commands/labextension/static/remoteEntry.89ac62f95e2ea8afb0ea.js
--rw-r--r--   0 timkpaine   (501) staff       (20)      118 2022-04-11 19:07:37.000000 jupyterlab_commands-0.3.4/jupyterlab_commands/labextension/static/style.js
--rw-r--r--   0 timkpaine   (501) staff       (20)    19725 2022-04-11 19:07:39.000000 jupyterlab_commands-0.3.4/jupyterlab_commands/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-04-11 19:07:55.122630 jupyterlab_commands-0.3.4/jupyterlab_commands/tests/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2019-08-15 02:41:38.000000 jupyterlab_commands-0.3.4/jupyterlab_commands/tests/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-02-25 20:56:20.000000 jupyterlab_commands-0.3.4/jupyterlab_commands/tests/test_all.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      329 2022-04-03 01:58:53.000000 jupyterlab_commands-0.3.4/jupyterlab_commands/tests/test_extension.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      254 2022-04-03 01:58:53.000000 jupyterlab_commands-0.3.4/jupyterlab_commands/tests/test_init.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-04-11 19:07:55.117916 jupyterlab_commands-0.3.4/jupyterlab_commands.egg-info/
--rw-r--r--   0 timkpaine   (501) staff       (20)     3426 2022-04-11 19:07:53.000000 jupyterlab_commands-0.3.4/jupyterlab_commands.egg-info/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)     1300 2022-04-11 19:07:55.000000 jupyterlab_commands-0.3.4/jupyterlab_commands.egg-info/SOURCES.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2022-04-11 19:07:53.000000 jupyterlab_commands-0.3.4/jupyterlab_commands.egg-info/dependency_links.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2022-04-11 19:07:48.000000 jupyterlab_commands-0.3.4/jupyterlab_commands.egg-info/not-zip-safe
--rw-r--r--   0 timkpaine   (501) staff       (20)      428 2022-04-11 19:07:53.000000 jupyterlab_commands-0.3.4/jupyterlab_commands.egg-info/requires.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       20 2022-04-11 19:07:53.000000 jupyterlab_commands-0.3.4/jupyterlab_commands.egg-info/top_level.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)      134 2022-04-11 19:07:13.000000 jupyterlab_commands-0.3.4/pyproject.toml
--rw-r--r--   0 timkpaine   (501) staff       (20)      936 2022-04-11 19:07:55.123953 jupyterlab_commands-0.3.4/setup.cfg
--rw-r--r--   0 timkpaine   (501) staff       (20)     2821 2022-04-11 19:07:13.000000 jupyterlab_commands-0.3.4/setup.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/.bumpversion.cfg
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/.gitattributes
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/MANIFEST.in
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/Makefile
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/setup.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/js/.eslintrc.js
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/js/babel.config.js
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/js/jest.config.js
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/js/package.json
+-rw-r--r--   0        0        0   357789 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/js/yarn.lock
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/js/src/index.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/js/style/index.css
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/js/tests/activate.test.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/js/tests/assetsTransformer.js
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/js/tests/export.test.js
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/js/tests/fileMock.js
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/js/tests/setup.js
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/js/tests/styleMock.js
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/jupyterlab_commands/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/jupyterlab_commands/_version.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/jupyterlab_commands/extension.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/jupyterlab_commands/extension/jupyterlab_commands.json
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/jupyterlab_commands/labextension/package.json
+-rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/jupyterlab_commands/labextension/static/568.6fa7c06d94b5d4c0a342.js
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/jupyterlab_commands/labextension/static/873.af0a6b8becacd1ba8457.js
+-rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/jupyterlab_commands/labextension/static/remoteEntry.94043ea2257c211ef483.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/jupyterlab_commands/labextension/static/style.js
+-rw-r--r--   0        0        0    19725 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/jupyterlab_commands/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/jupyterlab_commands/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/jupyterlab_commands/tests/test_all.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/jupyterlab_commands/tests/test_extension.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/jupyterlab_commands/tests/test_init.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/.gitignore
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/README.md
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    16933 2020-02-02 00:00:00.000000 jupyterlab_commands-0.4.0/PKG-INFO
```

### Comparing `jupyterlab_commands-0.3.4/CONTRIBUTING.md` & `jupyterlab_commands-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_commands-0.3.4/LICENSE` & `jupyterlab_commands-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_commands-0.3.4/Makefile` & `jupyterlab_commands-0.4.0/Makefile`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,99 @@
+###############
+# Build Tools #
+###############
+build:  ## build python/javascript
+	python -m build .
+
+develop:  ## install to site-packages in editable mode
+	python -m pip install --upgrade build pip setuptools twine wheel
+	cd js; yarn
+	python -m pip install -e .[develop]
+
+install:  ## install to site-packages
+	python -m pip install .
+
+###########
+# Testing #
+###########
 testpy: ## Clean and Make unit tests
-	python -m pytest -v jupyterlab_commands/tests --cov=jupyterlab_commands --junitxml=python_junit.xml --cov-report=xml --cov-branch
+	python -m pytest -v jupyterlab_commands/tests --junitxml=junit.xml --cov=jupyterlab_commands --cov-report xml --cov-branch --cov-fail-under=20 --cov-report term-missing
 
 testjs: ## Clean and Make js tests
 	cd js; yarn test
 
 test: tests
 tests: testpy testjs ## run the tests
 
+###########
+# Linting #
+###########
 lintpy:  ## Black/flake8 python
-	python -m black --check jupyterlab_commands setup.py docs/conf.py
-	python -m flake8 jupyterlab_commands setup.py docs/conf.py
+	python -m ruff jupyterlab_commands setup.py
+	python -m black --check jupyterlab_commands setup.py
 
 lintjs:  ## ESlint javascript
 	cd js; yarn lint
 
 lint: lintpy lintjs  ## run linter
 
 fixpy:  ## Black python
-	python -m black jupyterlab_commands/ setup.py docs/conf.py
+	python -m ruff jupyterlab_commands setup.py --fix
+	python -m black jupyterlab_commands/ setup.py
 
 fixjs:  ## ESlint Autofix JS
 	cd js; yarn fix
 
 fix: fixpy fixjs  ## run black/tslint fix
+format: fix
 
+#################
+# Other Checks #
+#################
 check: checks
-checks:  ## run lint and other checks
-	check-manifest -v
 
-build:  ## build python/javascript
-	python -m build .
+checks: check-manifest  ## run security, packaging, and other checks
 
-develop:  ## install to site-packages in editable mode
-	python -m pip install --upgrade build pip setuptools twine wheel
-	cd js; yarn
-	python -m pip install -e .[develop]
+check-manifest:  ## run manifest checker for sdist
+	check-manifest -v
 
-install:  ## install to site-packages
-	python -m pip install .
+semgrep:  ## run semgrep
+	semgrep ci --config auto
 
+################
+# Distribution #
+################
 dist: clean build  ## create dists
 	python -m twine check dist/*
 
 publishpy:  ## dist to pypi
 	python -m twine upload dist/* --skip-existing
 
 publishjs:  ## dist to npm
 	cd js; npm publish || echo "can't publish - might already exist"
 
 publish: dist publishpy publishjs  ## dist to pypi and npm
 
-docs:  ## make documentation
-	make -C ./docs html
-	open ./docs/_build/html/index.html
-
+############
+# Cleaning #
+############
 clean: ## clean the repository
 	find . -name "__pycache__" | xargs  rm -rf
 	find . -name "*.pyc" | xargs rm -rf
 	find . -name ".ipynb_checkpoints" | xargs  rm -rf
-	rm -rf .coverage coverage *.xml build dist *.egg-info lib node_modules .pytest_cache *.egg-info .autoversion .mypy_cache
+	rm -rf .coverage coverage *.xml build dist *.egg-info lib node_modules .pytest_cache *.egg-info
 	rm -rf jupyterlab_commands/labextension
 	cd js && yarn clean
-	# make -C ./docs clean
 	git clean -fd
 
+###########
+# Helpers #
+###########
 # Thanks to Francoise at marmelab.com for this
 .DEFAULT_GOAL := help
 help:
 	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
 
 print-%:
 	@echo '$*=$($*)'
 
-.PHONY: testjs testpy tests test lintpy lintjs lint fixpy fixjs fix checks check build develop install labextension dist publishpy publishjs publish docs clean
+.PHONY: testjs testpy tests test lintpy lintjs lint fixpy fixjs fix format checks check check-manifest semgrep build develop install labextension dist publishpy publishjs publish docs clean
```

### Comparing `jupyterlab_commands-0.3.4/PKG-INFO` & `jupyterlab_commands-0.4.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,17 @@
-Metadata-Version: 2.1
-Name: jupyterlab_commands
-Version: 0.3.4
-Summary: Arbitrary python commands for notebooks in JupyterLab
-Home-page: https://github.com/timkpaine/jupyterlab_commands
-Author: Tim Paine
-Author-email: t.paine154@gmail.com
-License: Apache 2.0
-Keywords: Jupyter,Jupyterlab
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Framework :: Jupyter
-Classifier: Framework :: Jupyter :: JupyterLab
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: develop
-License-File: LICENSE
-
 # jupyterlab_commands
 
 Support for arbitrary python commands in the command palette. 
 
 [![Build Status](https://github.com/timkpaine/jupyterlab_commands/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/timkpaine/jupyterlab_commands/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/timkpaine/jupyterlab_commands/branch/main/graph/badge.svg?token=wWAQ6QqP6M)](https://codecov.io/gh/timkpaine/jupyterlab_commands)
 [![PyPI](https://img.shields.io/pypi/l/jupyterlab_commands.svg)](https://pypi.python.org/pypi/jupyterlab_commands)
 [![PyPI](https://img.shields.io/pypi/v/jupyterlab_commands.svg)](https://pypi.python.org/pypi/jupyterlab_commands)
 [![npm](https://img.shields.io/npm/v/jupyterlab_commands.svg)](https://www.npmjs.com/package/jupyterlab_commands)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/timkpaine/jupyterlab_commands/main?urlpath=lab)
 
 ## About
 
 This code lets you inject arbitrary commands into the JLab frontend. There are a variety of reasons why one might want to execute python commands outside of a notebook and a console:
 
 - a predefined NBConvert function that you dont want included in the converted result
 - interacting with VCS without including that interaction in the notebook
@@ -47,22 +22,22 @@
 pip install jupyterlab_commands
 jupyter labextension install jupyterlab_commands
 jupyter serverextension enable --py jupyterlab_commands
 ```
 
 ## Example 
 
-#### jupyter_notebook_config.py
+#### jupyter_lab_config.py
 
 ```python
 def convertMe(request, *args, **kwargs):
     import subprocess, tornado, os, os.path, json
     data = json.loads(tornado.escape.json_decode(request.body))
     path = os.path.join(os.getcwd(), data['path'])
-    subprocess.run(["jupyter", "nbconvert", path, '--template', '/Users/theocean154/.jupyter/test.tpl', '--to', 'html'])
+    subprocess.run(["jupyter", "nbconvert", path, '--to', 'html'])
     return {'body': 'ok'}
 
 c.JupyterLabCommands.commands = {'sample_command': convertMe}
 ```
 
 #### command palette
 
@@ -90,9 +65,7 @@
 ## Adding commands
 
 install the server extension, and add the following to `jupyter_notebook_config.py`
 
 ```python3
 c.JupyterLabCommands.commands = {'command display name': python_function, ...}
 ```
-
-
```

### Comparing `jupyterlab_commands-0.3.4/js/.eslintrc.js` & `jupyterlab_commands-0.4.0/js/.eslintrc.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text*

 * *Files 0% similar despite different names*

```diff
@@ -78,8 +78,8 @@
 000004d0: 6f6c 7665 6422 3a20 226f 6666 222c 0a20  olved": "off",. 
 000004e0: 2020 2022 696d 706f 7274 2f70 7265 6665     "import/prefe
 000004f0: 722d 6465 6661 756c 742d 6578 706f 7274  r-default-export
 00000500: 223a 2022 6f66 6622 2c0a 2020 2020 2269  ": "off",.    "i
 00000510: 6d70 6f72 742f 6e6f 2d65 7874 7261 6e65  mport/no-extrane
 00000520: 6f75 732d 6465 7065 6e64 656e 6369 6573  ous-dependencies
 00000530: 223a 2022 6f66 6622 2c0a 2020 7d2c 0a7d  ": "off",.  },.}
-00000540: 3b                                       ;
+00000540: 3b0a                                     ;.
```

### Comparing `jupyterlab_commands-0.3.4/js/package.json` & `jupyterlab_commands-0.4.0/jupyterlab_commands/labextension/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9121874999999999%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.2', '@jupyterlab/apputils': '^4.1.2', "*

 * *                   "'@jupyterlab/coreutils': '^6.0.2', '@jupyterlab/docmanager': '^4.0.2', "*

 * *                   "'@jupyterlab/filebrowser': '^4.0.2', '@jupyterlab/launcher': '^4.0.2', "*

 * *                   "'@lumino/widgets': '^2.2.0'}",*

 * * "'devDependencies'": "{'@babel/cli': '^7.22.6', '@babel/core': '^7.22.8', '@babel/eslint-parser': "*

 * *                      "'^7.22.7', '@babel/preset-env': '^7.22.7', '@jupyterlab/b […]*

```diff
@@ -1,49 +1,56 @@
 {
     "author": "Tim Paine",
     "dependencies": {
-        "@jupyterlab/application": "^3.2.0",
-        "@jupyterlab/apputils": "^3.2.0",
-        "@jupyterlab/coreutils": "^5.2.0",
-        "@jupyterlab/docmanager": "^3.3.2",
-        "@jupyterlab/filebrowser": "^3.3.2",
-        "@jupyterlab/launcher": "^3.3.2",
-        "@lumino/widgets": "^1.31.1",
+        "@jupyterlab/application": "^4.0.2",
+        "@jupyterlab/apputils": "^4.1.2",
+        "@jupyterlab/coreutils": "^6.0.2",
+        "@jupyterlab/docmanager": "^4.0.2",
+        "@jupyterlab/filebrowser": "^4.0.2",
+        "@jupyterlab/launcher": "^4.0.2",
+        "@lumino/widgets": "^2.2.0",
         "requests-helper": "^0.1.5"
     },
     "description": "Arbitrary python commands for notebooks in JupyterLab.",
     "devDependencies": {
-        "@babel/cli": "^7.17.6",
-        "@babel/core": "^7.17.8",
-        "@babel/eslint-parser": "^7.17.0",
-        "@babel/preset-env": "^7.16.11",
-        "@jupyterlab/builder": "^3.3.2",
+        "@babel/cli": "^7.22.6",
+        "@babel/core": "^7.22.8",
+        "@babel/eslint-parser": "^7.22.7",
+        "@babel/preset-env": "^7.22.7",
+        "@jupyterlab/builder": "^4.0.2",
         "babel-eslint": "^10.1.0",
-        "babel-jest": "^27.5.1",
-        "eslint": "^8.8.0",
+        "babel-jest": "^29.6.1",
+        "eslint": "^8.44.0",
         "eslint-config-airbnb": "^19.0.4",
         "eslint-config-airbnb-base": "^15.0.0",
-        "eslint-config-prettier": "^8.5.0",
-        "eslint-plugin-import": "^2.25.4",
-        "eslint-plugin-jest": "^26.1.0",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-import": "^2.27.5",
+        "eslint-plugin-jest": "^27.2.2",
         "eslint-plugin-json": "^3.0.0",
-        "eslint-plugin-prettier": "^4.0.0",
+        "eslint-plugin-prettier": "^5.0.0",
         "isomorphic-fetch": "^3.0.0",
-        "jest": "^27.5.1",
+        "jest": "^29.6.1",
+        "jest-environment-jsdom": "^29.6.1",
+        "jest-junit": "^16.0.0",
         "jest-raw-loader": "^1.0.1",
-        "jest-transform-css": "^3.0.0",
-        "mkdirp": "^1.0.4",
+        "jest-transform-css": "^6.0.1",
+        "mkdirp": "^3.0.1",
         "npm-run-all": "^4.1.5",
-        "rimraf": "^3.0.2"
+        "prettier": "^3.0.0",
+        "rimraf": "^5.0.1"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.css"
     ],
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.94043ea2257c211ef483.js"
+        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_commands"
                 },
                 "managers": [
                     "pip"
@@ -67,9 +74,9 @@
         "build:lab": "jupyter labextension build .",
         "clean": "rimraf lib ../jupyterlab_commands/labextension",
         "fix": "yarn lint --fix",
         "lint": "eslint -c .eslintrc.js --ext .js src/ tests/",
         "prepublishOnly": "npm run build",
         "test": "jest --coverage --collectCoverageFrom=src/*.{js}"
     },
-    "version": "0.3.4"
+    "version": "0.4.0"
 }
```

### Comparing `jupyterlab_commands-0.3.4/js/src/index.js` & `jupyterlab_commands-0.4.0/js/src/index.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -36,46 +36,58 @@
                 execute: async () => {
                     const result = await showDialog({
                         buttons: [Dialog.cancelButton(), Dialog.okButton({
                             label: "Ok"
                         })],
                         title: `Execute ${command}?`,
                     });
+
                     if (result.button.label === "Cancel") {
                         return;
                     }
 
-                    const folder = browser.defaultBrowser.model.path || "";
+                    let ok = false;
+                    let body = "An unexpected error occurred";
 
-                    if (!app.shell.currentWidget) {
-                        // need a current widget
-                        return;
-                    }
+                    try {
+                        // Try to execute command, and show dialog with info when done
+                        const folder = browser.tracker.currentWidget.model.path || "";
+
+                        if (!app.shell.currentWidget) {
+                            // need a current widget
+                            return;
+                        }
 
-                    const context = docManager.contextForWidget(app.shell.currentWidget);
+                        const context = docManager.contextForWidget(app.shell.currentWidget);
 
-                    let path = "";
-                    let model = {};
-                    if (context) {
-                        path = context.path;
-                        model = context.model.toJSON();
-                    }
+                        let path = "";
+                        let model = {};
+                        if (context) {
+                            path = context.path;
+                            model = context.model.toJSON();
+                        }
 
-                    // eslint-disable-next-line no-shadow
-                    const res = await request("post", `${PageConfig.getBaseUrl()}commands/run?command=${encodeURI(command)}`, {}, JSON.stringify({
-                        folder,
-                        path,
-                        model
-                    }));
-                    if (res.ok) {
-                        const resp = res.json();
-                        let body = "";
-                        if (resp) {
-                            body = resp.body;
+                        // eslint-disable-next-line no-shadow
+                        const res = await request("post", `${PageConfig.getBaseUrl()}commands/run?command=${encodeURI(command)}`, {}, JSON.stringify({
+                            folder,
+                            path,
+                            model
+                        }));
+                        if (res.ok) {
+                            const resp = res.json();
+                            body = "No output returned.";
+                            if (resp) {
+                                body = resp.body;
+                            }
+                            ok = true;
                         }
+                    } catch (e) {
+                        body = e.toString();
+                    }
+                    if (ok) {
                         await showDialog({
                             body,
                             buttons: [Dialog.okButton({
                                 label: "Ok"
                             })],
                             title: `Execute ${command} succeeded`,
                         });
```

### Comparing `jupyterlab_commands-0.3.4/jupyterlab_commands/extension.py` & `jupyterlab_commands-0.4.0/jupyterlab_commands/extension.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import tornado.web
-from notebook.base.handlers import IPythonHandler
-from notebook.utils import url_path_join
+from jupyter_server.base.handlers import JupyterHandler
+from jupyter_server.utils import url_path_join
 
 
-class CommandsHandler(IPythonHandler):
+class CommandsHandler(JupyterHandler):
     def initialize(self, commands=None):
         self.commands = commands
 
     @tornado.web.authenticated
     def get(self):
         command = self.get_argument("command", "")
         if command in self.commands:
@@ -23,15 +23,15 @@
         if command in self.commands:
             res = self.commands[command](self.request)
             self.finish(res)
         else:
             self.finish("{}")
 
 
-class CommandsListHandler(IPythonHandler):
+class CommandsListHandler(JupyterHandler):
     def initialize(self, commands=None):
         self.commands = commands
 
     @tornado.web.authenticated
     def get(self):
         self.finish(json.dumps(list(self.commands.keys())))
 
@@ -45,20 +45,20 @@
     """
     web_app = nb_server_app.web_app
     commands = nb_server_app.config.get("JupyterLabCommands", {}).get("commands", {})
 
     base_url = web_app.settings["base_url"]
 
     host_pattern = ".*$"
-    print(
+    nb_server_app.log.info(
         "Installing jupyterlab_commands handler on path %s"
         % url_path_join(base_url, "commands")
     )
 
-    print("Available commands: %s" % ",".join(k for k in commands))
+    nb_server_app.log.info("Available commands: %s" % ",".join(k for k in commands))
     web_app.add_handlers(
         host_pattern,
         [
             (
                 url_path_join(base_url, "commands/get"),
                 CommandsListHandler,
                 {"commands": commands},
```

### Comparing `jupyterlab_commands-0.3.4/jupyterlab_commands/labextension/package.json` & `jupyterlab_commands-0.4.0/js/package.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9121874999999999%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.2', '@jupyterlab/apputils': '^4.1.2', "*

 * *                   "'@jupyterlab/coreutils': '^6.0.2', '@jupyterlab/docmanager': '^4.0.2', "*

 * *                   "'@jupyterlab/filebrowser': '^4.0.2', '@jupyterlab/launcher': '^4.0.2', "*

 * *                   "'@lumino/widgets': '^2.2.0'}",*

 * * "'devDependencies'": "{'@babel/cli': '^7.22.6', '@babel/core': '^7.22.8', '@babel/eslint-parser': "*

 * *                      "'^7.22.7', '@babel/preset-env': '^7.22.7', '@jupyterlab/b […]*

```diff
@@ -1,53 +1,52 @@
 {
     "author": "Tim Paine",
     "dependencies": {
-        "@jupyterlab/application": "^3.2.0",
-        "@jupyterlab/apputils": "^3.2.0",
-        "@jupyterlab/coreutils": "^5.2.0",
-        "@jupyterlab/docmanager": "^3.3.2",
-        "@jupyterlab/filebrowser": "^3.3.2",
-        "@jupyterlab/launcher": "^3.3.2",
-        "@lumino/widgets": "^1.31.1",
+        "@jupyterlab/application": "^4.0.2",
+        "@jupyterlab/apputils": "^4.1.2",
+        "@jupyterlab/coreutils": "^6.0.2",
+        "@jupyterlab/docmanager": "^4.0.2",
+        "@jupyterlab/filebrowser": "^4.0.2",
+        "@jupyterlab/launcher": "^4.0.2",
+        "@lumino/widgets": "^2.2.0",
         "requests-helper": "^0.1.5"
     },
     "description": "Arbitrary python commands for notebooks in JupyterLab.",
     "devDependencies": {
-        "@babel/cli": "^7.17.6",
-        "@babel/core": "^7.17.8",
-        "@babel/eslint-parser": "^7.17.0",
-        "@babel/preset-env": "^7.16.11",
-        "@jupyterlab/builder": "^3.3.2",
+        "@babel/cli": "^7.22.6",
+        "@babel/core": "^7.22.8",
+        "@babel/eslint-parser": "^7.22.7",
+        "@babel/preset-env": "^7.22.7",
+        "@jupyterlab/builder": "^4.0.2",
         "babel-eslint": "^10.1.0",
-        "babel-jest": "^27.5.1",
-        "eslint": "^8.8.0",
+        "babel-jest": "^29.6.1",
+        "eslint": "^8.44.0",
         "eslint-config-airbnb": "^19.0.4",
         "eslint-config-airbnb-base": "^15.0.0",
-        "eslint-config-prettier": "^8.5.0",
-        "eslint-plugin-import": "^2.25.4",
-        "eslint-plugin-jest": "^26.1.0",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-import": "^2.27.5",
+        "eslint-plugin-jest": "^27.2.2",
         "eslint-plugin-json": "^3.0.0",
-        "eslint-plugin-prettier": "^4.0.0",
+        "eslint-plugin-prettier": "^5.0.0",
         "isomorphic-fetch": "^3.0.0",
-        "jest": "^27.5.1",
+        "jest": "^29.6.1",
+        "jest-environment-jsdom": "^29.6.1",
+        "jest-junit": "^16.0.0",
         "jest-raw-loader": "^1.0.1",
-        "jest-transform-css": "^3.0.0",
-        "mkdirp": "^1.0.4",
+        "jest-transform-css": "^6.0.1",
+        "mkdirp": "^3.0.1",
         "npm-run-all": "^4.1.5",
-        "rimraf": "^3.0.2"
+        "prettier": "^3.0.0",
+        "rimraf": "^5.0.1"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.css"
     ],
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.89ac62f95e2ea8afb0ea.js"
-        },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_commands"
                 },
                 "managers": [
                     "pip"
@@ -71,9 +70,9 @@
         "build:lab": "jupyter labextension build .",
         "clean": "rimraf lib ../jupyterlab_commands/labextension",
         "fix": "yarn lint --fix",
         "lint": "eslint -c .eslintrc.js --ext .js src/ tests/",
         "prepublishOnly": "npm run build",
         "test": "jest --coverage --collectCoverageFrom=src/*.{js}"
     },
-    "version": "0.3.4"
+    "version": "0.4.0"
 }
```

### Comparing `jupyterlab_commands-0.3.4/jupyterlab_commands/labextension/static/568.ae9692e317badeae2b0e.js` & `jupyterlab_commands-0.4.0/jupyterlab_commands/labextension/static/568.6fa7c06d94b5d4c0a342.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,247 +1,272 @@
 "use strict";
 (self.webpackChunkjupyterlab_commands = self.webpackChunkjupyterlab_commands || []).push([
     [568], {
         568: (e, t, n) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
-            }), t._activate = l, t.default = void 0;
-            var a = n(149),
-                o = n(626),
-                r = n(859),
-                i = n(998),
-                c = n(672),
+            }), t._activate = u, t.default = void 0;
+            var o = n(350),
+                a = n(993),
+                r = n(554),
+                c = n(164),
+                i = n(262),
                 s = n(760);
-            async function l(e, t, n, r) {
-                const i = await (0, s.request)("get", `${o.PageConfig.getBaseUrl()}commands/get`);
-                i.ok && i.json().map((i => (e.commands.addCommand(i, {
+            async function u(e, t, n, r) {
+                const c = await (0, s.request)("get", `${a.PageConfig.getBaseUrl()}commands/get`);
+                c.ok && c.json().map((c => (e.commands.addCommand(c, {
                     execute: async () => {
-                        if ("Cancel" === (await (0, a.showDialog)({
-                                buttons: [a.Dialog.cancelButton(), a.Dialog.okButton({
+                        if ("Cancel" === (await (0, o.showDialog)({
+                                buttons: [o.Dialog.cancelButton(), o.Dialog.okButton({
                                     label: "Ok"
                                 })],
-                                title: `Execute ${i}?`
+                                title: `Execute ${c}?`
                             })).button.label) return;
-                        const n = r.defaultBrowser.model.path || "";
-                        if (!e.shell.currentWidget) return;
-                        const c = t.contextForWidget(e.shell.currentWidget);
-                        let l = "",
-                            u = {};
-                        c && (l = c.path, u = c.model.toJSON());
-                        const d = await (0, s.request)("post", `${o.PageConfig.getBaseUrl()}commands/run?command=${encodeURI(i)}`, {}, JSON.stringify({
-                            folder: n,
-                            path: l,
-                            model: u
-                        }));
-                        if (d.ok) {
-                            const e = d.json();
-                            let t = "";
-                            e && (t = e.body), await (0, a.showDialog)({
-                                body: t,
-                                buttons: [a.Dialog.okButton({
-                                    label: "Ok"
-                                })],
-                                title: `Execute ${i} succeeded`
-                            })
-                        } else await (0, a.showDialog)({
-                            buttons: [a.Dialog.okButton({
+                        let n = !1,
+                            i = "An unexpected error occurred";
+                        try {
+                            const o = r.tracker.currentWidget.model.path || "";
+                            if (!e.shell.currentWidget) return;
+                            const u = t.contextForWidget(e.shell.currentWidget);
+                            let l = "",
+                                d = {};
+                            u && (l = u.path, d = u.model.toJSON());
+                            const p = await (0, s.request)("post", `${a.PageConfig.getBaseUrl()}commands/run?command=${encodeURI(c)}`, {}, JSON.stringify({
+                                folder: o,
+                                path: l,
+                                model: d
+                            }));
+                            if (p.ok) {
+                                const e = p.json();
+                                i = "No output returned.", e && (i = e.body), n = !0
+                            }
+                        } catch (e) {
+                            i = e.toString()
+                        }
+                        n ? await (0, o.showDialog)({
+                            body: i,
+                            buttons: [o.Dialog.okButton({
                                 label: "Ok"
                             })],
-                            title: `Execute ${i} failed`
+                            title: `Execute ${c} succeeded`
+                        }) : await (0, o.showDialog)({
+                            buttons: [o.Dialog.okButton({
+                                label: "Ok"
+                            })],
+                            title: `Execute ${c} failed`
                         })
                     },
                     isEnabled: () => !0,
-                    label: i
+                    label: c
                 }), n.addItem({
-                    command: i,
+                    command: c,
                     category: "Custom Commands"
-                }), i))), console.log("JupyterLab extension jupyterlab_commands is activated!")
+                }), c))), console.log("JupyterLab extension jupyterlab_commands is activated!")
             }
             n(549);
-            var u = {
-                activate: l,
+            var l = {
+                activate: u,
                 autoStart: !0,
                 id: "jupyterlab_commands",
-                optional: [c.ILauncher],
-                requires: [r.IDocumentManager, a.ICommandPalette, i.IFileBrowserFactory]
+                optional: [i.ILauncher],
+                requires: [r.IDocumentManager, o.ICommandPalette, c.IFileBrowserFactory]
             };
-            t.default = u
+            t.default = l
         },
         408: (e, t, n) => {
             n.d(t, {
-                Z: () => r
+                Z: () => i
             });
-            var a = n(645),
-                o = n.n(a)()((function(e) {
-                    return e[1]
-                }));
-            o.push([e.id, "", ""]);
-            const r = o
+            var o = n(81),
+                a = n.n(o),
+                r = n(645),
+                c = n.n(r)()(a());
+            c.push([e.id, "", ""]);
+            const i = c
         },
         645: e => {
             e.exports = function(e) {
                 var t = [];
                 return t.toString = function() {
                     return this.map((function(t) {
-                        var n = e(t);
-                        return t[2] ? "@media ".concat(t[2], " {").concat(n, "}") : n
+                        var n = "",
+                            o = void 0 !== t[5];
+                        return t[4] && (n += "@supports (".concat(t[4], ") {")), t[2] && (n += "@media ".concat(t[2], " {")), o && (n += "@layer".concat(t[5].length > 0 ? " ".concat(t[5]) : "", " {")), n += e(t), o && (n += "}"), t[2] && (n += "}"), t[4] && (n += "}"), n
                     })).join("")
-                }, t.i = function(e, n, a) {
+                }, t.i = function(e, n, o, a, r) {
                     "string" == typeof e && (e = [
-                        [null, e, ""]
+                        [null, e, void 0]
                     ]);
-                    var o = {};
-                    if (a)
-                        for (var r = 0; r < this.length; r++) {
-                            var i = this[r][0];
-                            null != i && (o[i] = !0)
+                    var c = {};
+                    if (o)
+                        for (var i = 0; i < this.length; i++) {
+                            var s = this[i][0];
+                            null != s && (c[s] = !0)
                         }
-                    for (var c = 0; c < e.length; c++) {
-                        var s = [].concat(e[c]);
-                        a && o[s[0]] || (n && (s[2] ? s[2] = "".concat(n, " and ").concat(s[2]) : s[2] = n), t.push(s))
+                    for (var u = 0; u < e.length; u++) {
+                        var l = [].concat(e[u]);
+                        o && c[l[0]] || (void 0 !== r && (void 0 === l[5] || (l[1] = "@layer".concat(l[5].length > 0 ? " ".concat(l[5]) : "", " {").concat(l[1], "}")), l[5] = r), n && (l[2] ? (l[1] = "@media ".concat(l[2], " {").concat(l[1], "}"), l[2] = n) : l[2] = n), a && (l[4] ? (l[1] = "@supports (".concat(l[4], ") {").concat(l[1], "}"), l[4] = a) : l[4] = "".concat(a)), t.push(l))
                     }
                 }, t
             }
         },
+        81: e => {
+            e.exports = function(e) {
+                return e[1]
+            }
+        },
         549: (e, t, n) => {
             n.r(t), n.d(t, {
-                default: () => i
-            });
-            var a = n(379),
-                o = n.n(a),
-                r = n(408);
-            o()(r.Z, {
-                insert: "head",
-                singleton: !1
+                default: () => g
             });
-            const i = r.Z.locals || {}
+            var o = n(379),
+                a = n.n(o),
+                r = n(795),
+                c = n.n(r),
+                i = n(569),
+                s = n.n(i),
+                u = n(565),
+                l = n.n(u),
+                d = n(216),
+                p = n.n(d),
+                f = n(589),
+                m = n.n(f),
+                v = n(408),
+                h = {};
+            h.styleTagTransform = m(), h.setAttributes = l(), h.insert = s().bind(null, "head"), h.domAPI = c(), h.insertStyleElement = p(), a()(v.Z, h);
+            const g = v.Z && v.Z.locals ? v.Z.locals : void 0
         },
-        379: (e, t, n) => {
-            var a, o = function() {
-                    var e = {};
-                    return function(t) {
-                        if (void 0 === e[t]) {
-                            var n = document.querySelector(t);
-                            if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
-                                n = n.contentDocument.head
-                            } catch (e) {
-                                n = null
-                            }
-                            e[t] = n
-                        }
-                        return e[t]
-                    }
-                }(),
-                r = [];
+        379: e => {
+            var t = [];
 
-            function i(e) {
-                for (var t = -1, n = 0; n < r.length; n++)
-                    if (r[n].identifier === e) {
-                        t = n;
+            function n(e) {
+                for (var n = -1, o = 0; o < t.length; o++)
+                    if (t[o].identifier === e) {
+                        n = o;
                         break
-                    } return t
+                    } return n
             }
 
-            function c(e, t) {
-                for (var n = {}, a = [], o = 0; o < e.length; o++) {
-                    var c = e[o],
-                        s = t.base ? c[0] + t.base : c[0],
-                        l = n[s] || 0,
-                        u = "".concat(s, " ").concat(l);
-                    n[s] = l + 1;
-                    var d = i(u),
+            function o(e, o) {
+                for (var r = {}, c = [], i = 0; i < e.length; i++) {
+                    var s = e[i],
+                        u = o.base ? s[0] + o.base : s[0],
+                        l = r[u] || 0,
+                        d = "".concat(u, " ").concat(l);
+                    r[u] = l + 1;
+                    var p = n(d),
                         f = {
-                            css: c[1],
-                            media: c[2],
-                            sourceMap: c[3]
-                        }; - 1 !== d ? (r[d].references++, r[d].updater(f)) : r.push({
-                        identifier: u,
-                        updater: h(f, t),
-                        references: 1
-                    }), a.push(u)
+                            css: s[1],
+                            media: s[2],
+                            sourceMap: s[3],
+                            supports: s[4],
+                            layer: s[5]
+                        };
+                    if (-1 !== p) t[p].references++, t[p].updater(f);
+                    else {
+                        var m = a(f, o);
+                        o.byIndex = i, t.splice(i, 0, {
+                            identifier: d,
+                            updater: m,
+                            references: 1
+                        })
+                    }
+                    c.push(d)
                 }
-                return a
+                return c
             }
 
-            function s(e) {
-                var t = document.createElement("style"),
-                    a = e.attributes || {};
-                if (void 0 === a.nonce) {
-                    var r = n.nc;
-                    r && (a.nonce = r)
-                }
-                if (Object.keys(a).forEach((function(e) {
-                        t.setAttribute(e, a[e])
-                    })), "function" == typeof e.insert) e.insert(t);
-                else {
-                    var i = o(e.insert || "head");
-                    if (!i) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
-                    i.appendChild(t)
-                }
-                return t
+            function a(e, t) {
+                var n = t.domAPI(t);
+                return n.update(e),
+                    function(t) {
+                        if (t) {
+                            if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap && t.supports === e.supports && t.layer === e.layer) return;
+                            n.update(e = t)
+                        } else n.remove()
+                    }
             }
-            var l, u = (l = [], function(e, t) {
-                return l[e] = t, l.filter(Boolean).join("\n")
-            });
-
-            function d(e, t, n, a) {
-                var o = n ? "" : a.media ? "@media ".concat(a.media, " {").concat(a.css, "}") : a.css;
-                if (e.styleSheet) e.styleSheet.cssText = u(t, o);
-                else {
-                    var r = document.createTextNode(o),
-                        i = e.childNodes;
-                    i[t] && e.removeChild(i[t]), i.length ? e.insertBefore(r, i[t]) : e.appendChild(r)
+            e.exports = function(e, a) {
+                var r = o(e = e || [], a = a || {});
+                return function(e) {
+                    e = e || [];
+                    for (var c = 0; c < r.length; c++) {
+                        var i = n(r[c]);
+                        t[i].references--
+                    }
+                    for (var s = o(e, a), u = 0; u < r.length; u++) {
+                        var l = n(r[u]);
+                        0 === t[l].references && (t[l].updater(), t.splice(l, 1))
+                    }
+                    r = s
                 }
             }
-
-            function f(e, t, n) {
-                var a = n.css,
-                    o = n.media,
-                    r = n.sourceMap;
-                if (o ? e.setAttribute("media", o) : e.removeAttribute("media"), r && "undefined" != typeof btoa && (a += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(r)))), " */")), e.styleSheet) e.styleSheet.cssText = a;
-                else {
-                    for (; e.firstChild;) e.removeChild(e.firstChild);
-                    e.appendChild(document.createTextNode(a))
-                }
+        },
+        569: e => {
+            var t = {};
+            e.exports = function(e, n) {
+                var o = function(e) {
+                    if (void 0 === t[e]) {
+                        var n = document.querySelector(e);
+                        if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
+                            n = n.contentDocument.head
+                        } catch (e) {
+                            n = null
+                        }
+                        t[e] = n
+                    }
+                    return t[e]
+                }(e);
+                if (!o) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
+                o.appendChild(n)
             }
-            var m = null,
-                p = 0;
-
-            function h(e, t) {
-                var n, a, o;
-                if (t.singleton) {
-                    var r = p++;
-                    n = m || (m = s(t)), a = d.bind(null, n, r, !1), o = d.bind(null, n, r, !0)
-                } else n = s(t), a = f.bind(null, n, t), o = function() {
-                    ! function(e) {
-                        if (null === e.parentNode) return !1;
-                        e.parentNode.removeChild(e)
-                    }(n)
+        },
+        216: e => {
+            e.exports = function(e) {
+                var t = document.createElement("style");
+                return e.setAttributes(t, e.attributes), e.insert(t, e.options), t
+            }
+        },
+        565: (e, t, n) => {
+            e.exports = function(e) {
+                var t = n.nc;
+                t && e.setAttribute("nonce", t)
+            }
+        },
+        795: e => {
+            e.exports = function(e) {
+                if ("undefined" == typeof document) return {
+                    update: function() {},
+                    remove: function() {}
                 };
-                return a(e),
-                    function(t) {
-                        if (t) {
-                            if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap) return;
-                            a(e = t)
-                        } else o()
+                var t = e.insertStyleElement(e);
+                return {
+                    update: function(n) {
+                        ! function(e, t, n) {
+                            var o = "";
+                            n.supports && (o += "@supports (".concat(n.supports, ") {")), n.media && (o += "@media ".concat(n.media, " {"));
+                            var a = void 0 !== n.layer;
+                            a && (o += "@layer".concat(n.layer.length > 0 ? " ".concat(n.layer) : "", " {")), o += n.css, a && (o += "}"), n.media && (o += "}"), n.supports && (o += "}");
+                            var r = n.sourceMap;
+                            r && "undefined" != typeof btoa && (o += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(r)))), " */")), t.styleTagTransform(o, e, t.options)
+                        }(t, e, n)
+                    },
+                    remove: function() {
+                        ! function(e) {
+                            if (null === e.parentNode) return !1;
+                            e.parentNode.removeChild(e)
+                        }(t)
                     }
+                }
             }
+        },
+        589: e => {
             e.exports = function(e, t) {
-                (t = t || {}).singleton || "boolean" == typeof t.singleton || (t.singleton = (void 0 === a && (a = Boolean(window && document && document.all && !window.atob)), a));
-                var n = c(e = e || [], t);
-                return function(e) {
-                    if (e = e || [], "[object Array]" === Object.prototype.toString.call(e)) {
-                        for (var a = 0; a < n.length; a++) {
-                            var o = i(n[a]);
-                            r[o].references--
-                        }
-                        for (var s = c(e, t), l = 0; l < n.length; l++) {
-                            var u = i(n[l]);
-                            0 === r[u].references && (r[u].updater(), r.splice(u, 1))
-                        }
-                        n = s
-                    }
+                if (t.styleSheet) t.styleSheet.cssText = e;
+                else {
+                    for (; t.firstChild;) t.removeChild(t.firstChild);
+                    t.appendChild(document.createTextNode(e))
                 }
             }
         }
     }
 ]);
```

### Comparing `jupyterlab_commands-0.3.4/jupyterlab_commands/labextension/static/873.af0a6b8becacd1ba8457.js` & `jupyterlab_commands-0.4.0/jupyterlab_commands/labextension/static/873.af0a6b8becacd1ba8457.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_commands-0.3.4/jupyterlab_commands/labextension/static/remoteEntry.89ac62f95e2ea8afb0ea.js` & `jupyterlab_commands-0.4.0/jupyterlab_commands/labextension/static/remoteEntry.94043ea2257c211ef483.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,282 +1,285 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, d, s, f, p, c, h, v, b, m, g = {
-            305: (e, r, t) => {
+    var e, r, t, n, o, a, i, u, l, s, f, d, c, p, h, v, m, b, g, y = {
+            822: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(568))),
                         "./extension": () => t.e(568).then((() => () => t(568)))
                     },
-                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    o = (e, r) => {
+                    a = (e, r) => {
                         if (t.S) {
-                            var n = t.S.default,
-                                a = "default";
-                            if (n && n !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
-                            return t.S[a] = e, t.I(a, r)
+                            var n = "default",
+                                o = t.S[n];
+                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                            return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => a,
-                    init: () => o
+                    get: () => o,
+                    init: () => a
                 })
             }
         },
-        y = {};
+        w = {};
 
-    function w(e) {
-        var r = y[e];
+    function j(e) {
+        var r = w[e];
         if (void 0 !== r) return r.exports;
-        var t = y[e] = {
+        var t = w[e] = {
             id: e,
             exports: {}
         };
-        return g[e](t, t.exports, w), t.exports
+        return y[e](t, t.exports, j), t.exports
     }
-    w.m = g, w.c = y, w.n = e => {
+    j.m = y, j.c = w, j.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return w.d(r, {
+        return j.d(r, {
             a: r
         }), r
-    }, w.d = (e, r) => {
-        for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
+    }, j.d = (e, r) => {
+        for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        568: "ae9692e317badeae2b0e",
+    }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
+        568: "6fa7c06d94b5d4c0a342",
         873: "af0a6b8becacd1ba8457"
     } [e] + ".js?v=" + {
-        568: "ae9692e317badeae2b0e",
+        568: "6fa7c06d94b5d4c0a342",
         873: "af0a6b8becacd1ba8457"
-    } [e], w.g = function() {
+    } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyterlab_commands:", w.l = (t, n, a, o) => {
+    }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyterlab_commands:", j.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
-            if (void 0 !== a)
-                for (var l = document.getElementsByTagName("script"), d = 0; d < l.length; d++) {
-                    var s = l[d];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
-                        i = s;
+            if (void 0 !== o)
+                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
+                    var f = l[s];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
+                        i = f;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var f = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
-                    var a = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            var d = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(c);
+                    var o = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(f.bind(null, void 0, {
+                c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, w.r = e => {
+    }, j.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        w.S = {};
+        j.S = {};
         var e = {},
             r = {};
-        w.I = (t, n) => {
+        j.I = (t, n) => {
             n || (n = []);
-            var a = r[t];
-            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
-                if (n.push(a), e[t]) return e[t];
-                w.o(w.S, t) || (w.S[t] = {});
-                var o = w.S[t],
+            var o = r[t];
+            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
+                if (n.push(o), e[t]) return e[t];
+                j.o(j.S, t) || (j.S[t] = {});
+                var a = j.S[t],
                     i = "jupyterlab_commands",
                     u = (e, r, t, n) => {
-                        var a = o[e] = o[e] || {},
-                            u = a[r];
-                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (a[r] = {
+                        var o = a[e] = a[e] || {},
+                            u = o[r];
+                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("jupyterlab_commands", "0.3.4", (() => w.e(568).then((() => () => w(568))))), u("requests-helper", "0.1.5", (() => w.e(873).then((() => () => w(873)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("jupyterlab_commands", "0.4.0", (() => j.e(568).then((() => () => j(568))))), u("requests-helper", "0.1.5", (() => j.e(873).then((() => () => j(873)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        w.g.importScripts && (e = w.g.location + "");
-        var r = w.g.document;
+        j.g.importScripts && (e = j.g.location + "");
+        var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            t.length && (e = t[t.length - 1].src)
+            if (t.length)
+                for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), w.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), j.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var a = e[n],
-                o = (typeof a)[0];
-            if (n >= r.length) return "u" == o;
+            var o = e[n],
+                a = (typeof o)[0];
+            if (n >= r.length) return "u" == a;
             var i = r[n],
                 u = (typeof i)[0];
-            if (o != u) return "o" == o && "n" == u || "s" == u || "u" == o;
-            if ("o" != o && "u" != o && a != i) return a < i;
+            if (a != u) return "o" == a && "n" == u || "s" == u || "u" == a;
+            if ("o" != a && "u" != a && o != i) return o < i;
             n++
         }
-    }, a = e => {
+    }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(u = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
+            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var i = [];
-        for (o = 1; o < e.length; o++) {
-            var u = e[o];
-            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : a(u))
+        for (a = 1; a < e.length; a++) {
+            var u = e[a];
+            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
         return l();
 
         function l() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, o = (e, r) => {
+    }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                a = n < 0;
-            a && (n = -n - 1);
+                o = n < 0;
+            o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var d, s, f = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(d = r[i]))[0])) return !l || ("u" == f ? u > n && !a : "" == f != a);
-                if ("u" == s) {
-                    if (!l || "u" != f) return !1
+                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+                if ("u" == f) {
+                    if (!l || "u" != d) return !1
                 } else if (l)
-                    if (f == s)
+                    if (d == f)
                         if (u <= n) {
-                            if (d != e[u]) return !1
+                            if (s != e[u]) return !1
                         } else {
-                            if (a ? d > e[u] : d < e[u]) return !1;
-                            d != e[u] && (l = !1)
+                            if (o ? s > e[u] : s < e[u]) return !1;
+                            s != e[u] && (l = !1)
                         }
-                else if ("s" != f && "n" != f) {
-                    if (a || u <= n) return !1;
+                else if ("s" != d && "n" != d) {
+                    if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || s < f != a) return !1;
+                    if (u <= n || f < d != o) return !1;
                     l = !1
-                } else "s" != f && "n" != f && (l = !1, u--)
+                } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var c = [],
+            p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
-        return !!c()
+        return !!p()
     }, i = (e, r) => {
-        var t = w.S[e];
-        if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = j.S[e];
+        if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", d = (e, r, t, n) => {
-        var a = u(e, t);
-        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(l(e, t, a, n)), f(e[t][a])
-    }, s = (e, r, t) => {
-        var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
-    }, f = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, a) {
-        var o = w.I(r);
-        return o && o.then ? o.then(e.bind(e, r, w.S[r], t, n, a)) : e(r, w.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), h = p(((e, r, t, n, a) => {
-        var o = r && w.o(r, t) && s(r, t, n);
-        return o ? f(o) : a()
-    })), v = {}, b = {
-        149: () => c("default", "@jupyterlab/apputils", [1, 3, 3, 2]),
-        626: () => c("default", "@jupyterlab/coreutils", [1, 5, 3, 2]),
-        672: () => c("default", "@jupyterlab/launcher", [1, 3, 3, 2]),
-        760: () => h("default", "requests-helper", [2, 0, 1, 5], (() => w.e(873).then((() => () => w(873))))),
-        859: () => c("default", "@jupyterlab/docmanager", [1, 3, 3, 2]),
-        998: () => c("default", "@jupyterlab/filebrowser", [1, 3, 3, 2])
-    }, m = {
-        568: [149, 626, 672, 760, 859, 998]
-    }, w.f.consumes = (e, r) => {
-        w.o(m, e) && m[e].forEach((e => {
-            if (w.o(v, e)) return r.push(v[e]);
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
+        var o = u(e, t);
+        return a(n, o) || d(l(e, t, o, n)), c(e[t][o])
+    }, f = (e, r, t) => {
+        var o = e[r];
+        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
+    }, d = e => {
+        "undefined" != typeof console && console.warn && console.warn(e)
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
+        var a = j.I(r);
+        return a && a.then ? a.then(e.bind(e, r, j.S[r], t, n, o)) : e(r, j.S[r], t, n, o)
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), v = p(((e, r, t, n, o) => {
+        var a = r && j.o(r, t) && f(r, t, n);
+        return a ? c(a) : o()
+    })), m = {}, b = {
+        164: () => h("default", "@jupyterlab/filebrowser", [1, 4, 0, 2]),
+        262: () => h("default", "@jupyterlab/launcher", [1, 4, 0, 2]),
+        350: () => h("default", "@jupyterlab/apputils", [1, 4, 1, 2]),
+        554: () => h("default", "@jupyterlab/docmanager", [1, 4, 0, 2]),
+        760: () => v("default", "requests-helper", [2, 0, 1, 5], (() => j.e(873).then((() => () => j(873))))),
+        993: () => h("default", "@jupyterlab/coreutils", [1, 6, 0, 2])
+    }, g = {
+        568: [164, 262, 350, 554, 760, 993]
+    }, j.f.consumes = (e, r) => {
+        j.o(g, e) && g[e].forEach((e => {
+            if (j.o(m, e)) return r.push(m[e]);
             var t = r => {
-                    v[e] = 0, w.m[e] = t => {
-                        delete w.c[e], t.exports = r()
+                    m[e] = 0, j.m[e] = t => {
+                        delete j.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete v[e], w.m[e] = t => {
-                        throw delete w.c[e], r
+                    delete m[e], j.m[e] = t => {
+                        throw delete j.c[e], r
                     }
                 };
             try {
-                var a = b[e]();
-                a.then ? r.push(v[e] = a.then(t).catch(n)) : t(a)
+                var o = b[e]();
+                o.then ? r.push(m[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             129: 0
         };
-        w.f.j = (r, t) => {
-            var n = w.o(e, r) ? e[r] : void 0;
+        j.f.j = (r, t) => {
+            var n = j.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
-                    var a = new Promise(((t, a) => n = e[r] = [t, a]));
-                    t.push(n[2] = a);
-                    var o = w.p + w.u(r),
+                    var o = new Promise(((t, o) => n = e[r] = [t, o]));
+                    t.push(n[2] = o);
+                    var a = j.p + j.u(r),
                         i = new Error;
-                    w.l(o, (t => {
-                        if (w.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                            var a = t && ("load" === t.type ? "missing" : t.type),
-                                o = t && t.target && t.target.src;
-                            i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
+                    j.l(a, (t => {
+                        if (j.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                            var o = t && ("load" === t.type ? "missing" : t.type),
+                                a = t && t.target && t.target.src;
+                            i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, a, [o, i, u] = t,
+                var n, o, [a, i, u] = t,
                     l = 0;
-                if (o.some((r => 0 !== e[r]))) {
-                    for (n in i) w.o(i, n) && (w.m[n] = i[n]);
-                    u && u(w)
+                if (a.some((r => 0 !== e[r]))) {
+                    for (n in i) j.o(i, n) && (j.m[n] = i[n]);
+                    u && u(j)
                 }
-                for (r && r(t); l < o.length; l++) a = o[l], w.o(e, a) && e[a] && e[a][0](), e[o[l]] = 0
+                for (r && r(t); l < a.length; l++) o = a[l], j.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkjupyterlab_commands = self.webpackChunkjupyterlab_commands || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })();
-    var j = w(305);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).jupyterlab_commands = j
+    })(), j.nc = void 0;
+    var S = j(822);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).jupyterlab_commands = S
 })();
```

### Comparing `jupyterlab_commands-0.3.4/jupyterlab_commands/labextension/static/third-party-licenses.json` & `jupyterlab_commands-0.4.0/jupyterlab_commands/labextension/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333333%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '6.8.1'}, 2: {'versionInfo': '3.3.3'}}"}*

```diff
@@ -1,22 +1,22 @@
 {
     "packages": [
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
-            "versionInfo": "5.2.7"
+            "versionInfo": "6.8.1"
         },
         {
             "extractedText": "Mozilla Public License Version 2.0\n==================================\n\n1. Definitions\n--------------\n\n1.1. \"Contributor\"\n    means each individual or legal entity that creates, contributes to\n    the creation of, or owns Covered Software.\n\n1.2. \"Contributor Version\"\n    means the combination of the Contributions of others (if any) used\n    by a Contributor and that particular Contributor's Contribution.\n\n1.3. \"Contribution\"\n    means Covered Software of a particular Contributor.\n\n1.4. \"Covered Software\"\n    means Source Code Form to which the initial Contributor has attached\n    the notice in Exhibit A, the Executable Form of such Source Code\n    Form, and Modifications of such Source Code Form, in each case\n    including portions thereof.\n\n1.5. \"Incompatible With Secondary Licenses\"\n    means\n\n    (a) that the initial Contributor has attached the notice described\n        in Exhibit B to the Covered Software; or\n\n    (b) that the Covered Software was made available under the terms of\n        version 1.1 or earlier of the License, but not also under the\n        terms of a Secondary License.\n\n1.6. \"Executable Form\"\n    means any form of the work other than Source Code Form.\n\n1.7. \"Larger Work\"\n    means a work that combines Covered Software with other material, in\n    a separate file or files, that is not Covered Software.\n\n1.8. \"License\"\n    means this document.\n\n1.9. \"Licensable\"\n    means having the right to grant, to the maximum extent possible,\n    whether at the time of the initial grant or subsequently, any and\n    all of the rights conveyed by this License.\n\n1.10. \"Modifications\"\n    means any of the following:\n\n    (a) any file in Source Code Form that results from an addition to,\n        deletion from, or modification of the contents of Covered\n        Software; or\n\n    (b) any new file in Source Code Form that contains any Covered\n        Software.\n\n1.11. \"Patent Claims\" of a Contributor\n    means any patent claim(s), including without limitation, method,\n    process, and apparatus claims, in any patent Licensable by such\n    Contributor that would be infringed, but for the grant of the\n    License, by the making, using, selling, offering for sale, having\n    made, import, or transfer of either its Contributions or its\n    Contributor Version.\n\n1.12. \"Secondary License\"\n    means either the GNU General Public License, Version 2.0, the GNU\n    Lesser General Public License, Version 2.1, the GNU Affero General\n    Public License, Version 3.0, or any later versions of those\n    licenses.\n\n1.13. \"Source Code Form\"\n    means the form of the work preferred for making modifications.\n\n1.14. \"You\" (or \"Your\")\n    means an individual or a legal entity exercising rights under this\n    License. For legal entities, \"You\" includes any entity that\n    controls, is controlled by, or is under common control with You. For\n    purposes of this definition, \"control\" means (a) the power, direct\n    or indirect, to cause the direction or management of such entity,\n    whether by contract or otherwise, or (b) ownership of more than\n    fifty percent (50%) of the outstanding shares or beneficial\n    ownership of such entity.\n\n2. License Grants and Conditions\n--------------------------------\n\n2.1. Grants\n\nEach Contributor hereby grants You a world-wide, royalty-free,\nnon-exclusive license:\n\n(a) under intellectual property rights (other than patent or trademark)\n    Licensable by such Contributor to use, reproduce, make available,\n    modify, display, perform, distribute, and otherwise exploit its\n    Contributions, either on an unmodified basis, with Modifications, or\n    as part of a Larger Work; and\n\n(b) under Patent Claims of such Contributor to make, use, sell, offer\n    for sale, have made, import, and otherwise transfer either its\n    Contributions or its Contributor Version.\n\n2.2. Effective Date\n\nThe licenses granted in Section 2.1 with respect to any Contribution\nbecome effective for each Contribution on the date the Contributor first\ndistributes such Contribution.\n\n2.3. Limitations on Grant Scope\n\nThe licenses granted in this Section 2 are the only rights granted under\nthis License. No additional rights or licenses will be implied from the\ndistribution or licensing of Covered Software under this License.\nNotwithstanding Section 2.1(b) above, no patent license is granted by a\nContributor:\n\n(a) for any code that a Contributor has removed from Covered Software;\n    or\n\n(b) for infringements caused by: (i) Your and any other third party's\n    modifications of Covered Software, or (ii) the combination of its\n    Contributions with other software (except as part of its Contributor\n    Version); or\n\n(c) under Patent Claims infringed by Covered Software in the absence of\n    its Contributions.\n\nThis License does not grant any rights in the trademarks, service marks,\nor logos of any Contributor (except as may be necessary to comply with\nthe notice requirements in Section 3.4).\n\n2.4. Subsequent Licenses\n\nNo Contributor makes additional grants as a result of Your choice to\ndistribute the Covered Software under a subsequent version of this\nLicense (see Section 10.2) or under the terms of a Secondary License (if\npermitted under the terms of Section 3.3).\n\n2.5. Representation\n\nEach Contributor represents that the Contributor believes its\nContributions are its original creation(s) or it has sufficient rights\nto grant the rights to its Contributions conveyed by this License.\n\n2.6. Fair Use\n\nThis License is not intended to limit any rights You have under\napplicable copyright doctrines of fair use, fair dealing, or other\nequivalents.\n\n2.7. Conditions\n\nSections 3.1, 3.2, 3.3, and 3.4 are conditions of the licenses granted\nin Section 2.1.\n\n3. Responsibilities\n-------------------\n\n3.1. Distribution of Source Form\n\nAll distribution of Covered Software in Source Code Form, including any\nModifications that You create or to which You contribute, must be under\nthe terms of this License. You must inform recipients that the Source\nCode Form of the Covered Software is governed by the terms of this\nLicense, and how they can obtain a copy of this License. You may not\nattempt to alter or restrict the recipients' rights in the Source Code\nForm.\n\n3.2. Distribution of Executable Form\n\nIf You distribute Covered Software in Executable Form then:\n\n(a) such Covered Software must also be made available in Source Code\n    Form, as described in Section 3.1, and You must inform recipients of\n    the Executable Form how they can obtain a copy of such Source Code\n    Form by reasonable means in a timely manner, at a charge no more\n    than the cost of distribution to the recipient; and\n\n(b) You may distribute such Executable Form under the terms of this\n    License, or sublicense it under different terms, provided that the\n    license for the Executable Form does not attempt to limit or alter\n    the recipients' rights in the Source Code Form under this License.\n\n3.3. Distribution of a Larger Work\n\nYou may create and distribute a Larger Work under terms of Your choice,\nprovided that You also comply with the requirements of this License for\nthe Covered Software. If the Larger Work is a combination of Covered\nSoftware with a work governed by one or more Secondary Licenses, and the\nCovered Software is not Incompatible With Secondary Licenses, this\nLicense permits You to additionally distribute such Covered Software\nunder the terms of such Secondary License(s), so that the recipient of\nthe Larger Work may, at their option, further distribute the Covered\nSoftware under the terms of either this License or such Secondary\nLicense(s).\n\n3.4. Notices\n\nYou may not remove or alter the substance of any license notices\n(including copyright notices, patent notices, disclaimers of warranty,\nor limitations of liability) contained within the Source Code Form of\nthe Covered Software, except that You may alter any license notices to\nthe extent required to remedy known factual inaccuracies.\n\n3.5. Application of Additional Terms\n\nYou may choose to offer, and to charge a fee for, warranty, support,\nindemnity or liability obligations to one or more recipients of Covered\nSoftware. However, You may do so only on Your own behalf, and not on\nbehalf of any Contributor. You must make it absolutely clear that any\nsuch warranty, support, indemnity, or liability obligation is offered by\nYou alone, and You hereby agree to indemnify every Contributor for any\nliability incurred by such Contributor as a result of warranty, support,\nindemnity or liability terms You offer. You may include additional\ndisclaimers of warranty and limitations of liability specific to any\njurisdiction.\n\n4. Inability to Comply Due to Statute or Regulation\n---------------------------------------------------\n\nIf it is impossible for You to comply with any of the terms of this\nLicense with respect to some or all of the Covered Software due to\nstatute, judicial order, or regulation then You must: (a) comply with\nthe terms of this License to the maximum extent possible; and (b)\ndescribe the limitations and the code they affect. Such description must\nbe placed in a text file included with all distributions of the Covered\nSoftware under this License. Except to the extent prohibited by statute\nor regulation, such description must be sufficiently detailed for a\nrecipient of ordinary skill to be able to understand it.\n\n5. Termination\n--------------\n\n5.1. The rights granted under this License will terminate automatically\nif You fail to comply with any of its terms. However, if You become\ncompliant, then the rights granted under this License from a particular\nContributor are reinstated (a) provisionally, unless and until such\nContributor explicitly and finally terminates Your grants, and (b) on an\nongoing basis, if such Contributor fails to notify You of the\nnon-compliance by some reasonable means prior to 60 days after You have\ncome back into compliance. Moreover, Your grants from a particular\nContributor are reinstated on an ongoing basis if such Contributor\nnotifies You of the non-compliance by some reasonable means, this is the\nfirst time You have received notice of non-compliance with this License\nfrom such Contributor, and You become compliant prior to 30 days after\nYour receipt of the notice.\n\n5.2. If You initiate litigation against any entity by asserting a patent\ninfringement claim (excluding declaratory judgment actions,\ncounter-claims, and cross-claims) alleging that a Contributor Version\ndirectly or indirectly infringes any patent, then the rights granted to\nYou by any and all Contributors for the Covered Software under Section\n2.1 of this License shall terminate.\n\n5.3. In the event of termination under Sections 5.1 or 5.2 above, all\nend user license agreements (excluding distributors and resellers) which\nhave been validly granted by You or Your distributors under this License\nprior to termination shall survive termination.\n\n************************************************************************\n*                                                                      *\n*  6. Disclaimer of Warranty                                           *\n*  -------------------------                                           *\n*                                                                      *\n*  Covered Software is provided under this License on an \"as is\"       *\n*  basis, without warranty of any kind, either expressed, implied, or  *\n*  statutory, including, without limitation, warranties that the       *\n*  Covered Software is free of defects, merchantable, fit for a        *\n*  particular purpose or non-infringing. The entire risk as to the     *\n*  quality and performance of the Covered Software is with You.        *\n*  Should any Covered Software prove defective in any respect, You     *\n*  (not any Contributor) assume the cost of any necessary servicing,   *\n*  repair, or correction. This disclaimer of warranty constitutes an   *\n*  essential part of this License. No use of any Covered Software is   *\n*  authorized under this License except under this disclaimer.         *\n*                                                                      *\n************************************************************************\n\n************************************************************************\n*                                                                      *\n*  7. Limitation of Liability                                          *\n*  --------------------------                                          *\n*                                                                      *\n*  Under no circumstances and under no legal theory, whether tort      *\n*  (including negligence), contract, or otherwise, shall any           *\n*  Contributor, or anyone who distributes Covered Software as          *\n*  permitted above, be liable to You for any direct, indirect,         *\n*  special, incidental, or consequential damages of any character      *\n*  including, without limitation, damages for lost profits, loss of    *\n*  goodwill, work stoppage, computer failure or malfunction, or any    *\n*  and all other commercial damages or losses, even if such party      *\n*  shall have been informed of the possibility of such damages. This   *\n*  limitation of liability shall not apply to liability for death or   *\n*  personal injury resulting from such party's negligence to the       *\n*  extent applicable law prohibits such limitation. Some               *\n*  jurisdictions do not allow the exclusion or limitation of           *\n*  incidental or consequential damages, so this exclusion and          *\n*  limitation may not apply to You.                                    *\n*                                                                      *\n************************************************************************\n\n8. Litigation\n-------------\n\nAny litigation relating to this License may be brought only in the\ncourts of a jurisdiction where the defendant maintains its principal\nplace of business and such litigation shall be governed by laws of that\njurisdiction, without reference to its conflict-of-law provisions.\nNothing in this Section shall prevent a party's ability to bring\ncross-claims or counter-claims.\n\n9. Miscellaneous\n----------------\n\nThis License represents the complete agreement concerning the subject\nmatter hereof. If any provision of this License is held to be\nunenforceable, such provision shall be reformed only to the extent\nnecessary to make it enforceable. Any law or regulation which provides\nthat the language of a contract shall be construed against the drafter\nshall not be used to construe this License against a Contributor.\n\n10. Versions of the License\n---------------------------\n\n10.1. New Versions\n\nMozilla Foundation is the license steward. Except as provided in Section\n10.3, no one other than the license steward has the right to modify or\npublish new versions of this License. Each version will be given a\ndistinguishing version number.\n\n10.2. Effect of New Versions\n\nYou may distribute the Covered Software under the terms of the version\nof the License under which You originally received the Covered Software,\nor under the terms of any subsequent version published by the license\nsteward.\n\n10.3. Modified Versions\n\nIf you create software not governed by this License, and you want to\ncreate a new license for such software, you may create and use a\nmodified version of this License if you rename the license and remove\nany references to the name of the license steward (except to note that\nsuch modified license differs from this License).\n\n10.4. Distributing Source Code Form that is Incompatible With Secondary\nLicenses\n\nIf You choose to distribute Source Code Form that is Incompatible With\nSecondary Licenses under the terms of this version of the License, the\nnotice described in Exhibit B of this License must be attached.\n\nExhibit A - Source Code Form License Notice\n-------------------------------------------\n\n  This Source Code Form is subject to the terms of the Mozilla Public\n  License, v. 2.0. If a copy of the MPL was not distributed with this\n  file, You can obtain one at http://mozilla.org/MPL/2.0/.\n\nIf it is not possible or desirable to put the notice in a particular\nfile, then You may include the notice in a location (such as a LICENSE\nfile in a relevant directory) where a recipient would be likely to look\nfor such a notice.\n\nYou may add additional accurate notices of copyright ownership.\n\nExhibit B - \"Incompatible With Secondary Licenses\" Notice\n---------------------------------------------------------\n\n  This Source Code Form is \"Incompatible With Secondary Licenses\", as\n  defined by the Mozilla Public License, v. 2.0.\n",
             "licenseId": "Apache-2.0",
             "name": "requests-helper",
             "versionInfo": "0.1.5"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "style-loader",
-            "versionInfo": "2.0.0"
+            "versionInfo": "3.3.3"
         }
     ]
 }
```

### Comparing `jupyterlab_commands-0.3.4/setup.cfg` & `jupyterlab_commands-0.4.0/.bumpversion.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,20 @@
 [bumpversion]
-current_version = 0.3.4
+current_version = 0.4.0
 commit = True
 tag = False
 
-[bdist_wheel]
-universal = 1
-
-[metadata]
-description_file = README.md
-long_description_content_type = text/markdown
-
-[flake8]
-ignore = E203, W503
-max-line-length = 200
-exclude = jupyterlab_commands/tests
-per-file-ignores = 
-	jupyterlab_commands/__init__.py:F401, F403
-
-[tool:pytest]
-junit_family = xunit2
-
 [bumpversion:file:jupyterlab_commands/_version.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
-[bumpversion:file:setup.py]
-search = version="{current_version}"
-replace = version="{new_version}"
+[bumpversion:file:pyproject.toml]
+search = version = "{current_version}"
+replace = version = "{new_version}"
 
 [bumpversion:file:js/package.json]
 search = "version": "{current_version}"
 replace = "version": "{new_version}"
 
-[bumpversion:file:docs/conf.py]
-search = version = "{current_version}"
-replace = version = "{new_version}"
-
-[check-manifest]
-ignore = 
-	jupyterlab_commands/labextension/**
-	js/**
-
-[egg_info]
-tag_build = 
-tag_date = 0
-
+[bumpversion:file:binder/requirements.txt]
+search = jupyterlab_commands=={current_version}
+replace = jupyterlab_commands=={new_version}
```

