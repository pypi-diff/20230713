# Comparing `tmp/texplain-0.8.4.tar.gz` & `tmp/texplain-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texplain-0.8.4.tar", last modified: Thu Jul 13 07:25:26 2023, max compression
+gzip compressed data, was "texplain-0.8.5.tar", last modified: Thu Jul 13 07:37:33 2023, max compression
```

## Comparing `texplain-0.8.4.tar` & `texplain-0.8.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:26.947025 texplain-0.8.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:26.939025 texplain-0.8.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:26.943025 texplain-0.8.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-13 07:25:17.000000 texplain-0.8.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-13 07:25:17.000000 texplain-0.8.4/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-13 07:25:17.000000 texplain-0.8.4/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-13 07:25:17.000000 texplain-0.8.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-13 07:25:17.000000 texplain-0.8.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-13 07:25:17.000000 texplain-0.8.4/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-13 07:25:17.000000 texplain-0.8.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-13 07:25:17.000000 texplain-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-13 07:25:26.947025 texplain-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-13 07:25:17.000000 texplain-0.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:26.943025 texplain-0.8.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 07:25:17.000000 texplain-0.8.4/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-13 07:25:17.000000 texplain-0.8.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-13 07:25:17.000000 texplain-0.8.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-13 07:25:17.000000 texplain-0.8.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-13 07:25:17.000000 texplain-0.8.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-13 07:25:17.000000 texplain-0.8.4/docs/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-13 07:25:17.000000 texplain-0.8.4/docs/pre-commit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-13 07:25:17.000000 texplain-0.8.4/docs/tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-13 07:25:17.000000 texplain-0.8.4/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 07:25:17.000000 texplain-0.8.4/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-13 07:25:17.000000 texplain-0.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 07:25:26.947025 texplain-0.8.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:26.943025 texplain-0.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:26.943025 texplain-0.8.4/tests/input1/
--rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/input1/apalike.bst
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/input1/example.tex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:26.943025 texplain-0.8.4/tests/input1/figures/
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/input1/figures/Diverging.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/input1/figures/Sequential.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/input1/goose-article.cls
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/input1/refs.bib
--rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/input1/unsrtnat.bst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:26.943025 texplain-0.8.4/tests/output1/
--rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/output1/apalike.bst
--rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/output1/figure_1.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/output1/figure_2.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/output1/goose-article.cls
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/output1/library.bib
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/output1/main.tex
--rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/output1/unsrtnat.bst
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/test_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/test_find_command.py
--rw-r--r--   0 runner    (1001) docker     (123)   167299 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/test_indent_long.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/test_indent_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/test_indent_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/test_indent_texindent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/test_placeholders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/test_texplain_example1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:26.947025 texplain-0.8.4/texplain/
--rw-r--r--   0 runner    (1001) docker     (123)    88194 2023-07-13 07:25:17.000000 texplain-0.8.4/texplain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-13 07:25:26.000000 texplain-0.8.4/texplain/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:26.947025 texplain-0.8.4/texplain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-13 07:25:26.000000 texplain-0.8.4/texplain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-13 07:25:26.000000 texplain-0.8.4/texplain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 07:25:26.000000 texplain-0.8.4/texplain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-13 07:25:26.000000 texplain-0.8.4/texplain.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 07:25:26.000000 texplain-0.8.4/texplain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 07:25:26.000000 texplain-0.8.4/texplain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:37:33.801238 texplain-0.8.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:37:33.789238 texplain-0.8.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:37:33.797238 texplain-0.8.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-13 07:37:23.000000 texplain-0.8.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-13 07:37:23.000000 texplain-0.8.5/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-13 07:37:23.000000 texplain-0.8.5/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-13 07:37:23.000000 texplain-0.8.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-13 07:37:23.000000 texplain-0.8.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-13 07:37:23.000000 texplain-0.8.5/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-13 07:37:23.000000 texplain-0.8.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-13 07:37:23.000000 texplain-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-13 07:37:33.801238 texplain-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-13 07:37:23.000000 texplain-0.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:37:33.797238 texplain-0.8.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 07:37:23.000000 texplain-0.8.5/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-13 07:37:23.000000 texplain-0.8.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-13 07:37:23.000000 texplain-0.8.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-13 07:37:23.000000 texplain-0.8.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-13 07:37:23.000000 texplain-0.8.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-13 07:37:23.000000 texplain-0.8.5/docs/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-13 07:37:23.000000 texplain-0.8.5/docs/pre-commit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-13 07:37:23.000000 texplain-0.8.5/docs/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-13 07:37:23.000000 texplain-0.8.5/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 07:37:23.000000 texplain-0.8.5/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-13 07:37:23.000000 texplain-0.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 07:37:33.801238 texplain-0.8.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:37:33.797238 texplain-0.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:37:33.801238 texplain-0.8.5/tests/input1/
+-rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/input1/apalike.bst
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/input1/example.tex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:37:33.801238 texplain-0.8.5/tests/input1/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/input1/figures/Diverging.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/input1/figures/Sequential.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/input1/goose-article.cls
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/input1/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/input1/unsrtnat.bst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:37:33.801238 texplain-0.8.5/tests/output1/
+-rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/output1/apalike.bst
+-rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/output1/figure_1.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/output1/figure_2.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/output1/goose-article.cls
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/output1/library.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/output1/main.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/output1/unsrtnat.bst
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/test_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/test_find_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)   167299 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/test_indent_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/test_indent_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21031 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/test_indent_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/test_indent_texindent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/test_placeholders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-13 07:37:23.000000 texplain-0.8.5/tests/test_texplain_example1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:37:33.801238 texplain-0.8.5/texplain/
+-rw-r--r--   0 runner    (1001) docker     (123)    88197 2023-07-13 07:37:23.000000 texplain-0.8.5/texplain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-13 07:37:33.000000 texplain-0.8.5/texplain/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:37:33.801238 texplain-0.8.5/texplain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-13 07:37:33.000000 texplain-0.8.5/texplain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-13 07:37:33.000000 texplain-0.8.5/texplain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 07:37:33.000000 texplain-0.8.5/texplain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-13 07:37:33.000000 texplain-0.8.5/texplain.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 07:37:33.000000 texplain-0.8.5/texplain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 07:37:33.000000 texplain-0.8.5/texplain.egg-info/top_level.txt
```

### Comparing `texplain-0.8.4/.github/workflows/ci.yml` & `texplain-0.8.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/.github/workflows/pythonpublish.yml` & `texplain-0.8.5/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/.gitignore` & `texplain-0.8.5/.gitignore`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/.pre-commit-config.yaml` & `texplain-0.8.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/LICENSE` & `texplain-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/PKG-INFO` & `texplain-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texplain
-Version: 0.8.4
+Version: 0.8.5
 Summary: TeX file formatting
 Author-email: Tom de Geus <tom@geus.me>
 Project-URL: Source, https://github.com/tdegeus/texplain
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `texplain-0.8.4/README.md` & `texplain-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/docs/Makefile` & `texplain-0.8.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/docs/make.bat` & `texplain-0.8.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/docs/module.rst` & `texplain-0.8.5/docs/module.rst`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/pyproject.toml` & `texplain-0.8.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/input1/apalike.bst` & `texplain-0.8.5/tests/input1/apalike.bst`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/input1/example.tex` & `texplain-0.8.5/tests/input1/example.tex`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/input1/figures/Diverging.pdf` & `texplain-0.8.5/tests/input1/figures/Diverging.pdf`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/input1/figures/Sequential.pdf` & `texplain-0.8.5/tests/input1/figures/Sequential.pdf`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/input1/goose-article.cls` & `texplain-0.8.5/tests/input1/goose-article.cls`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/input1/refs.bib` & `texplain-0.8.5/tests/input1/refs.bib`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/input1/unsrtnat.bst` & `texplain-0.8.5/tests/input1/unsrtnat.bst`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/output1/apalike.bst` & `texplain-0.8.5/tests/output1/apalike.bst`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/output1/figure_1.pdf` & `texplain-0.8.5/tests/output1/figure_1.pdf`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/output1/figure_2.pdf` & `texplain-0.8.5/tests/output1/figure_2.pdf`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/output1/goose-article.cls` & `texplain-0.8.5/tests/output1/goose-article.cls`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/output1/library.bib` & `texplain-0.8.5/tests/output1/library.bib`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/output1/main.tex` & `texplain-0.8.5/tests/output1/main.tex`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/output1/unsrtnat.bst` & `texplain-0.8.5/tests/output1/unsrtnat.bst`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/test_align.py` & `texplain-0.8.5/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/test_classify.py` & `texplain-0.8.5/tests/test_classify.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/test_find_command.py` & `texplain-0.8.5/tests/test_find_command.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/test_indent_long.py` & `texplain-0.8.5/tests/test_indent_long.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/test_indent_options.py` & `texplain-0.8.5/tests/test_indent_options.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/test_indent_simple.py` & `texplain-0.8.5/tests/test_indent_simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -410,14 +410,36 @@
     \item e
 \end{itemize}
         """
 
         ret = texplain.indent(text)
         self.assertEqual(ret.strip(), formatted.strip())
 
+    def test_newline(self):
+        text = r"""
+\begin{itemize} \item a \item b
+
+\item c \item d
+\item e \end{itemize}
+        """
+
+        formatted = r"""
+\begin{itemize}
+    \item a
+    \item b
+
+    \item c
+    \item d
+    \item e
+\end{itemize}
+        """
+
+        ret = texplain.indent(text)
+        self.assertEqual(ret.strip(), formatted.strip())
+
     def test_multiline(self):
         text = r"""
 \begin{itemize} \item a \item b has a long
 text that spans multiple lines. But also multiple
 sentences.
 
 With even
```

### Comparing `texplain-0.8.4/tests/test_indent_texindent.py` & `texplain-0.8.5/tests/test_indent_texindent.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/test_placeholders.py` & `texplain-0.8.5/tests/test_placeholders.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/test_simple.py` & `texplain-0.8.5/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/tests/test_texplain_example1.py` & `texplain-0.8.5/tests/test_texplain_example1.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.4/texplain/__init__.py` & `texplain-0.8.5/texplain/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1523,15 +1523,15 @@
 
     # \\ ends on line
     if linebreak:
         text = re.sub(r"(?<!\\)(\\\\)(\ *\n?)", r"\1\n", text)
 
     # \item starts on a new line
     if itemize:
-        text = re.sub(r"(\s*)(?<!\\)(\\item)", r"\n\2", text)
+        text = re.sub(r"(\n?\ *)(?<!\\)(\\item)", r"\n\2", text)
 
     # format tables: align if possible
     if alignment:
         text, placeholders_table = text_to_placeholders(text, [PlaceholderType.tabular])
         for placeholder in placeholders_table:
             placeholder.content = _align(placeholder.content)
         text = text_from_placeholders(text, placeholders_table)
```

### Comparing `texplain-0.8.4/texplain.egg-info/PKG-INFO` & `texplain-0.8.5/texplain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texplain
-Version: 0.8.4
+Version: 0.8.5
 Summary: TeX file formatting
 Author-email: Tom de Geus <tom@geus.me>
 Project-URL: Source, https://github.com/tdegeus/texplain
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `texplain-0.8.4/texplain.egg-info/SOURCES.txt` & `texplain-0.8.5/texplain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

