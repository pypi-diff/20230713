# Comparing `tmp/texplain-0.8.3.tar.gz` & `tmp/texplain-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texplain-0.8.3.tar", last modified: Fri Jul  7 14:52:52 2023, max compression
+gzip compressed data, was "texplain-0.8.4.tar", last modified: Thu Jul 13 07:25:26 2023, max compression
```

## Comparing `texplain-0.8.3.tar` & `texplain-0.8.4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:52:52.232801 texplain-0.8.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:52:52.228801 texplain-0.8.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:52:52.228801 texplain-0.8.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-07 14:52:34.000000 texplain-0.8.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-07 14:52:34.000000 texplain-0.8.3/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-07 14:52:34.000000 texplain-0.8.3/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-07 14:52:34.000000 texplain-0.8.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-07 14:52:34.000000 texplain-0.8.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-07 14:52:34.000000 texplain-0.8.3/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-07 14:52:34.000000 texplain-0.8.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 14:52:34.000000 texplain-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-07 14:52:52.232801 texplain-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-07 14:52:34.000000 texplain-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:52:52.228801 texplain-0.8.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 14:52:34.000000 texplain-0.8.3/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 14:52:34.000000 texplain-0.8.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-07 14:52:34.000000 texplain-0.8.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-07 14:52:34.000000 texplain-0.8.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-07 14:52:34.000000 texplain-0.8.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-07 14:52:34.000000 texplain-0.8.3/docs/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 14:52:34.000000 texplain-0.8.3/docs/pre-commit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-07 14:52:34.000000 texplain-0.8.3/docs/tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-07 14:52:34.000000 texplain-0.8.3/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 14:52:34.000000 texplain-0.8.3/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-07 14:52:34.000000 texplain-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 14:52:52.232801 texplain-0.8.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:52:52.228801 texplain-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:52:52.228801 texplain-0.8.3/tests/input1/
--rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/input1/apalike.bst
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/input1/example.tex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:52:52.232801 texplain-0.8.3/tests/input1/figures/
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/input1/figures/Diverging.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/input1/figures/Sequential.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/input1/goose-article.cls
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/input1/refs.bib
--rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/input1/unsrtnat.bst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:52:52.232801 texplain-0.8.3/tests/output1/
--rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/output1/apalike.bst
--rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/output1/figure_1.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/output1/figure_2.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/output1/goose-article.cls
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/output1/library.bib
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/output1/main.tex
--rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/output1/unsrtnat.bst
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/test_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/test_find_command.py
--rw-r--r--   0 runner    (1001) docker     (123)   167299 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/test_indent_long.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/test_indent_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/test_indent_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/test_indent_texindent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/test_placeholders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-07 14:52:34.000000 texplain-0.8.3/tests/test_texplain_example1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:52:52.232801 texplain-0.8.3/texplain/
--rw-r--r--   0 runner    (1001) docker     (123)    88674 2023-07-07 14:52:34.000000 texplain-0.8.3/texplain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-07 14:52:52.000000 texplain-0.8.3/texplain/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:52:52.232801 texplain-0.8.3/texplain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-07 14:52:52.000000 texplain-0.8.3/texplain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-07 14:52:52.000000 texplain-0.8.3/texplain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:52:52.000000 texplain-0.8.3/texplain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-07 14:52:52.000000 texplain-0.8.3/texplain.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 14:52:52.000000 texplain-0.8.3/texplain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 14:52:52.000000 texplain-0.8.3/texplain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:26.947025 texplain-0.8.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:26.939025 texplain-0.8.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:26.943025 texplain-0.8.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-13 07:25:17.000000 texplain-0.8.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-13 07:25:17.000000 texplain-0.8.4/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-13 07:25:17.000000 texplain-0.8.4/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-13 07:25:17.000000 texplain-0.8.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-13 07:25:17.000000 texplain-0.8.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-13 07:25:17.000000 texplain-0.8.4/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-13 07:25:17.000000 texplain-0.8.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-13 07:25:17.000000 texplain-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-13 07:25:26.947025 texplain-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-13 07:25:17.000000 texplain-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:26.943025 texplain-0.8.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 07:25:17.000000 texplain-0.8.4/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-13 07:25:17.000000 texplain-0.8.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-13 07:25:17.000000 texplain-0.8.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-13 07:25:17.000000 texplain-0.8.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-13 07:25:17.000000 texplain-0.8.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-13 07:25:17.000000 texplain-0.8.4/docs/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-13 07:25:17.000000 texplain-0.8.4/docs/pre-commit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-13 07:25:17.000000 texplain-0.8.4/docs/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-13 07:25:17.000000 texplain-0.8.4/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 07:25:17.000000 texplain-0.8.4/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-13 07:25:17.000000 texplain-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 07:25:26.947025 texplain-0.8.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:26.943025 texplain-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:26.943025 texplain-0.8.4/tests/input1/
+-rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/input1/apalike.bst
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/input1/example.tex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:26.943025 texplain-0.8.4/tests/input1/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/input1/figures/Diverging.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/input1/figures/Sequential.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/input1/goose-article.cls
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/input1/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/input1/unsrtnat.bst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:26.943025 texplain-0.8.4/tests/output1/
+-rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/output1/apalike.bst
+-rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/output1/figure_1.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/output1/figure_2.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/output1/goose-article.cls
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/output1/library.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/output1/main.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/output1/unsrtnat.bst
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/test_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/test_find_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)   167299 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/test_indent_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/test_indent_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/test_indent_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/test_indent_texindent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/test_placeholders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-13 07:25:17.000000 texplain-0.8.4/tests/test_texplain_example1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:26.947025 texplain-0.8.4/texplain/
+-rw-r--r--   0 runner    (1001) docker     (123)    88194 2023-07-13 07:25:17.000000 texplain-0.8.4/texplain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-13 07:25:26.000000 texplain-0.8.4/texplain/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:25:26.947025 texplain-0.8.4/texplain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-13 07:25:26.000000 texplain-0.8.4/texplain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-13 07:25:26.000000 texplain-0.8.4/texplain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 07:25:26.000000 texplain-0.8.4/texplain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-13 07:25:26.000000 texplain-0.8.4/texplain.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 07:25:26.000000 texplain-0.8.4/texplain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 07:25:26.000000 texplain-0.8.4/texplain.egg-info/top_level.txt
```

### Comparing `texplain-0.8.3/.github/workflows/ci.yml` & `texplain-0.8.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/.github/workflows/pythonpublish.yml` & `texplain-0.8.4/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/.gitignore` & `texplain-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/.pre-commit-config.yaml` & `texplain-0.8.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/LICENSE` & `texplain-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/PKG-INFO` & `texplain-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texplain
-Version: 0.8.3
+Version: 0.8.4
 Summary: TeX file formatting
 Author-email: Tom de Geus <tom@geus.me>
 Project-URL: Source, https://github.com/tdegeus/texplain
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `texplain-0.8.3/README.md` & `texplain-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/docs/Makefile` & `texplain-0.8.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/docs/make.bat` & `texplain-0.8.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/docs/module.rst` & `texplain-0.8.4/docs/module.rst`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/pyproject.toml` & `texplain-0.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/input1/apalike.bst` & `texplain-0.8.4/tests/input1/apalike.bst`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/input1/example.tex` & `texplain-0.8.4/tests/input1/example.tex`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/input1/figures/Diverging.pdf` & `texplain-0.8.4/tests/input1/figures/Diverging.pdf`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/input1/figures/Sequential.pdf` & `texplain-0.8.4/tests/input1/figures/Sequential.pdf`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/input1/goose-article.cls` & `texplain-0.8.4/tests/input1/goose-article.cls`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/input1/refs.bib` & `texplain-0.8.4/tests/input1/refs.bib`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/input1/unsrtnat.bst` & `texplain-0.8.4/tests/input1/unsrtnat.bst`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/output1/apalike.bst` & `texplain-0.8.4/tests/output1/apalike.bst`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/output1/figure_1.pdf` & `texplain-0.8.4/tests/output1/figure_1.pdf`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/output1/figure_2.pdf` & `texplain-0.8.4/tests/output1/figure_2.pdf`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/output1/goose-article.cls` & `texplain-0.8.4/tests/output1/goose-article.cls`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/output1/library.bib` & `texplain-0.8.4/tests/output1/library.bib`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/output1/main.tex` & `texplain-0.8.4/tests/output1/main.tex`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/output1/unsrtnat.bst` & `texplain-0.8.4/tests/output1/unsrtnat.bst`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/test_align.py` & `texplain-0.8.4/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/test_find_command.py` & `texplain-0.8.4/tests/test_find_command.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/test_indent_long.py` & `texplain-0.8.4/tests/test_indent_long.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/test_indent_options.py` & `texplain-0.8.4/tests/test_indent_options.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/test_indent_simple.py` & `texplain-0.8.4/tests/test_indent_simple.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/test_indent_texindent.py` & `texplain-0.8.4/tests/test_indent_texindent.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/test_placeholders.py` & `texplain-0.8.4/tests/test_placeholders.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/test_simple.py` & `texplain-0.8.4/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/tests/test_texplain_example1.py` & `texplain-0.8.4/tests/test_texplain_example1.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.3/texplain/__init__.py` & `texplain-0.8.4/texplain/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1808,159 +1808,141 @@
             parts[i] = "\n".join([parts[i][0], body, parts[i][-1]])
 
     return "".join(parts)
 
 
 def _classify_for_label(text: str) -> tuple[list[str], NDArray[np.int_]]:
     """
-    Classify characters to identify to which environment a label belongs.
+    Classify each character.
+    This can be used for example to figure out to which environment a label belongs.
 
     :param text: The text to classify.
     :return:
-        ``(categories, classification)`` where ``categories`` is the list of label categories
-        ``"eq"``, ``"fig"``, etc.) and ``classification`` is an array of the same length as ``text``
-        where each element is the index of the category to which the character belongs.
+        ``(categories, classification)`` where ``categories`` is the list of categories
+        (``"eq"``, ``"fig"``, etc.; with ``"misc"`` for unknown) and ``classification`` is an array
+        of the same length as ``text`` where each element is the index in ``categories`` to which
+        the character belongs.
     """
 
     categories = ["misc", "eq", "item", "note", "sec", "ch", "fig", "tab"]
-    classification = np.zeros(len(text), dtype=int)
+    starting = -1 * np.ones((len(text), len(categories)), dtype=int)
     braces = find_matching(text, "{", "}", ignore_escaped=True)
 
-    # ---
-
-    r = -1
-
-    for match in re.finditer(r"(\s*\\label\s*\{)", text):
-        i = match.span()[0]
-        j = braces[match.span()[1] - 1]
-        classification[i:j] = r
-        r -= 1
-
-    # ---
+    # "eq"
 
     r = categories.index("eq")
 
     index = find_matching(
         text,
         r"\\begin\{equation\*?\}",
         r"\\end\{equation\*?\}",
         escape=False,
         closing_match=1,
     )
     for i, j in index.items():
-        classification[i:j] = r
+        starting[i:j, r] = i
 
     index = find_matching(
         text,
         r"\\begin\{align\*?\}",
         r"\\end\{align\*?\}",
         escape=False,
         closing_match=1,
     )
     for i, j in index.items():
-        classification[i:j] = r
+        starting[i:j, r] = i
 
     index = find_matching(
         text,
         r"\\begin\{eqnarray\*?\}",
         r"\\end\{eqnarray\*?\}",
         escape=False,
         closing_match=1,
     )
     for i, j in index.items():
-        classification[i:j] = r
+        starting[i:j, r] = i
 
-    # ---
+    # "fig"
 
     r = categories.index("fig")
 
     index = find_matching(
         text,
         r"\begin{figure}",
         r"\end{figure}",
         escape=True,
         closing_match=1,
     )
     for i, j in index.items():
-        classification[i:j] = r
+        starting[i:j, r] = i
 
-    # ---
+    # "tab"
 
     r = categories.index("tab")
 
     index = find_matching(
         text,
         r"\begin{table}",
         r"\end{table}",
         escape=True,
         closing_match=1,
     )
     for i, j in index.items():
-        classification[i:j] = r
+        starting[i:j, r] = i
 
-    # ---
+    # "item"
 
     r = categories.index("item")
 
     index = find_matching(
         text,
         r"\begin{itemize}",
         r"\end{itemize}",
         escape=True,
         closing_match=1,
     )
     for i, j in index.items():
-        classification[i:j] = r
+        starting[i:j, r] = i
 
     index = find_matching(
         text,
         r"\begin{enumerate}",
         r"\end{enumerate}",
         escape=True,
         closing_match=1,
     )
     for i, j in index.items():
-        classification[i:j] = r
+        starting[i:j, r] = i
 
-    # ---
+    # "note"
 
     r = categories.index("note")
 
     for match in re.finditer(r"(\\footnote\s*\{)", text):
         i = match.span()[0]
         j = braces[match.span()[1] - 1]
-        classification[i:j] = r
+        starting[i:j, r] = i
 
-    # ---
+    # "sec"
 
     r = categories.index("sec")
 
     for match in re.finditer(r"(\\)(sub)*(section\s*\{)", text):
         i = match.span()[0]
-        j = braces[match.span()[1] - 1]
-        classification[i:j] = r
-
-        if classification[j + 1] < 0:
-            classification[classification == classification[j + 1]] = r
+        starting[i:, r] = i
 
-    # ---
+    # "ch"
 
     r = categories.index("ch")
 
     for match in re.finditer(r"(\\)(chapter\s*\{)", text):
         i = match.span()[0]
-        j = braces[match.span()[1] - 1]
-        classification[i:j] = r
-
-        if classification[j + 1] < 0:
-            classification[classification == classification[j + 1]] = r
-
-    # ---
+        starting[i:, r] = i
 
-    return categories, np.where(classification < 0, categories.index("misc"), classification)
+    return categories, np.argmax(starting, axis=1)
 
 
 class TeX:
     """
     Interpret TeX file to allow simple manipulations.
     The manipulations are the member functions.
```

### Comparing `texplain-0.8.3/texplain.egg-info/PKG-INFO` & `texplain-0.8.4/texplain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texplain
-Version: 0.8.3
+Version: 0.8.4
 Summary: TeX file formatting
 Author-email: Tom de Geus <tom@geus.me>
 Project-URL: Source, https://github.com/tdegeus/texplain
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `texplain-0.8.3/texplain.egg-info/SOURCES.txt` & `texplain-0.8.4/texplain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

