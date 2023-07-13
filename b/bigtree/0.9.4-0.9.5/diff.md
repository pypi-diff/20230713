# Comparing `tmp/bigtree-0.9.4.tar.gz` & `tmp/bigtree-0.9.5.tar.gz`

## Comparing `bigtree-0.9.4.tar` & `bigtree-0.9.5.tar`

### file list

```diff
@@ -1,109 +1,113 @@
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 bigtree-0.9.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 bigtree-0.9.4/.readthedocs.yaml
--rw-r--r--   0        0        0    13366 2020-02-02 00:00:00.000000 bigtree-0.9.4/CHANGELOG.md
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bigtree-0.9.4/CONTRIBUTING.md
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 bigtree-0.9.4/SECURITY.md
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 bigtree-0.9.4/.github/workflows/codecov.yml
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 bigtree-0.9.4/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 bigtree-0.9.4/.github/workflows/pytest.yml
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 bigtree-0.9.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0   757076 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/DejaVuSans.ttf
--rw-r--r--   0        0        0    20084 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/binarytree.png
--rw-r--r--   0        0        0    11224 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/custom_tree.png
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/dag_construct.png
--rw-r--r--   0        0        0    12108 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/demo.png
--rw-r--r--   0        0        0    17554 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/demo_binarytree.png
--rw-r--r--   0        0        0    19320 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/demo_dag.png
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/demo_pillow.png
--rw-r--r--   0        0        0    10235 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/demo_tree.png
--rw-r--r--   0        0        0   313013 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/modify_advanced.png
--rw-r--r--   0        0        0   180588 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/modify_shift_and_copy.png
--rw-r--r--   0        0        0    67777 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/tree_construct.png
--rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 bigtree-0.9.4/assets/weighted_tree.png
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/py.typed
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/binarytree/construct.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/dag/__init__.py
--rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/dag/construct.py
--rw-r--r--   0        0        0    10007 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/dag/export.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/node/__init__.py
--rw-r--r--   0        0        0    21937 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/node/basenode.py
--rw-r--r--   0        0        0    13630 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/node/binarynode.py
--rw-r--r--   0        0        0    18188 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/node/dagnode.py
--rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/node/node.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/tree/__init__.py
--rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/tree/construct.py
--rw-r--r--   0        0        0    30268 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/tree/export.py
--rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/tree/helper.py
--rw-r--r--   0        0        0    33168 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/tree/modify.py
--rw-r--r--   0        0        0    12597 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/tree/search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/utils/__init__.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/utils/exceptions.py
--rw-r--r--   0        0        0    13884 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/utils/iterators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/workflows/__init__.py
--rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/workflows/app_calendar.py
--rw-r--r--   0        0        0     8516 2020-02-02 00:00:00.000000 bigtree-0.9.4/bigtree/workflows/app_todo.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/make.bat
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/requirements.txt
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/binarytree.rst
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/conf.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/dag.rst
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/index.rst
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/node.rst
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/others.rst
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/tree.rst
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/utils.rst
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/workflows.rst
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/_static/custom.css
--rw-r--r--   0        0        0    27138 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/_static/favicon.ico
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/_templates/layout.html
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/binarytree/construct.rst
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/dag/construct.rst
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/dag/export.rst
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/node/basenode.rst
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/node/binarynode.rst
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/node/dagnode.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/node/node.rst
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/tree/construct.rst
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/tree/export.rst
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/tree/helper.rst
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/tree/modify.rst
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/tree/search.rst
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/utils/iterators.rst
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/workflows/app_calendar.rst
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/bigtree/workflows/app_todo.rst
--rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/others/contributing.rst
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/others/list_dir.md
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/others/merging_trees.md
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/others/nodes.md
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/others/tips.rst
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 bigtree-0.9.4/docs/source/others/weighted_trees.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/__init__.py
--rw-r--r--   0        0        0     9434 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/conftest.py
--rw-r--r--   0        0        0     6308 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/binarytree/__init__.py
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/binarytree/test_construct.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/binarytree/test_export.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/binarytree/test_helper.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/binarytree/test_search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/dag/__init__.py
--rw-r--r--   0        0        0     8922 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/dag/test_construct.py
--rw-r--r--   0        0        0    15751 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/dag/test_export.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/node/__init__.py
--rw-r--r--   0        0        0    32428 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/node/test_basenode.py
--rw-r--r--   0        0        0    36915 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/node/test_binarynode.py
--rw-r--r--   0        0        0    32596 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/node/test_dagnode.py
--rw-r--r--   0        0        0    14179 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/node/test_node.py
--rw-r--r--   0        0        0    66656 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/tree/test_construct.py
--rw-r--r--   0        0        0    37681 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/tree/test_export.py
--rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/tree/test_helper.py
--rw-r--r--   0        0        0    67494 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/tree/test_modify.py
--rw-r--r--   0        0        0    18425 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/tree/test_search.py
--rw-r--r--   0        0        0    13544 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/utils/test_iterators.py
--rw-r--r--   0        0        0    18086 2020-02-02 00:00:00.000000 bigtree-0.9.4/tests/workflows/test_todo.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 bigtree-0.9.4/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bigtree-0.9.4/LICENSE
--rw-r--r--   0        0        0    25288 2020-02-02 00:00:00.000000 bigtree-0.9.4/README.md
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 bigtree-0.9.4/pyproject.toml
--rw-r--r--   0        0        0    26396 2020-02-02 00:00:00.000000 bigtree-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 bigtree-0.9.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 bigtree-0.9.5/.readthedocs.yaml
+-rw-r--r--   0        0        0    13772 2020-02-02 00:00:00.000000 bigtree-0.9.5/CHANGELOG.md
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bigtree-0.9.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 bigtree-0.9.5/SECURITY.md
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 bigtree-0.9.5/.github/workflows/codecov.yml
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 bigtree-0.9.5/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 bigtree-0.9.5/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 bigtree-0.9.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0   757076 2020-02-02 00:00:00.000000 bigtree-0.9.5/assets/DejaVuSans.ttf
+-rw-r--r--   0        0        0    20084 2020-02-02 00:00:00.000000 bigtree-0.9.5/assets/binarytree.png
+-rw-r--r--   0        0        0    11224 2020-02-02 00:00:00.000000 bigtree-0.9.5/assets/custom_tree.png
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 bigtree-0.9.5/assets/dag_construct.png
+-rw-r--r--   0        0        0    12108 2020-02-02 00:00:00.000000 bigtree-0.9.5/assets/demo.png
+-rw-r--r--   0        0        0    17554 2020-02-02 00:00:00.000000 bigtree-0.9.5/assets/demo_binarytree.png
+-rw-r--r--   0        0        0    19320 2020-02-02 00:00:00.000000 bigtree-0.9.5/assets/demo_dag.png
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 bigtree-0.9.5/assets/demo_pillow.png
+-rw-r--r--   0        0        0    10235 2020-02-02 00:00:00.000000 bigtree-0.9.5/assets/demo_tree.png
+-rw-r--r--   0        0        0   313013 2020-02-02 00:00:00.000000 bigtree-0.9.5/assets/modify_advanced.png
+-rw-r--r--   0        0        0   180588 2020-02-02 00:00:00.000000 bigtree-0.9.5/assets/modify_shift_and_copy.png
+-rw-r--r--   0        0        0    67777 2020-02-02 00:00:00.000000 bigtree-0.9.5/assets/tree_construct.png
+-rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 bigtree-0.9.5/assets/weighted_tree.png
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/binarytree/__init__.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/binarytree/construct.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/dag/__init__.py
+-rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/dag/construct.py
+-rw-r--r--   0        0        0    10007 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/dag/export.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/node/__init__.py
+-rw-r--r--   0        0        0    22023 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/node/basenode.py
+-rw-r--r--   0        0        0    13630 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/node/binarynode.py
+-rw-r--r--   0        0        0    18228 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/node/dagnode.py
+-rw-r--r--   0        0        0     6717 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/node/node.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/tree/__init__.py
+-rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/tree/construct.py
+-rw-r--r--   0        0        0    30268 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/tree/export.py
+-rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/tree/helper.py
+-rw-r--r--   0        0        0    33168 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/tree/modify.py
+-rw-r--r--   0        0        0    12597 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/tree/search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/utils/__init__.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/utils/exceptions.py
+-rw-r--r--   0        0        0    13884 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/utils/iterators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/workflows/__init__.py
+-rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/workflows/app_calendar.py
+-rw-r--r--   0        0        0     8516 2020-02-02 00:00:00.000000 bigtree-0.9.5/bigtree/workflows/app_todo.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/make.bat
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/requirements.txt
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/binarytree.rst
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/conf.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/dag.rst
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/index.rst
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/node.rst
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/others.rst
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/tree.rst
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/utils.rst
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/workflows.rst
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/_static/custom.css
+-rw-r--r--   0        0        0    27138 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/_static/favicon.ico
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/_templates/layout.html
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/bigtree/binarytree/construct.rst
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/bigtree/dag/construct.rst
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/bigtree/dag/export.rst
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/bigtree/node/basenode.rst
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/bigtree/node/binarynode.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/bigtree/node/dagnode.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/bigtree/node/node.rst
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/bigtree/tree/construct.rst
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/bigtree/tree/export.rst
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/bigtree/tree/helper.rst
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/bigtree/tree/modify.rst
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/bigtree/tree/search.rst
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/bigtree/utils/iterators.rst
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/bigtree/workflows/app_calendar.rst
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/bigtree/workflows/app_todo.rst
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/others/contributing.rst
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/others/list_dir.md
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/others/merging_trees.md
+-rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/others/nodes.md
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/others/tips.rst
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 bigtree-0.9.5/docs/source/others/weighted_trees.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/__init__.py
+-rw-r--r--   0        0        0     9434 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/conftest.py
+-rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/binarytree/__init__.py
+-rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/binarytree/test_construct.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/binarytree/test_export.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/binarytree/test_helper.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/binarytree/test_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/dag/__init__.py
+-rw-r--r--   0        0        0     8922 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/dag/test_construct.py
+-rw-r--r--   0        0        0    15751 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/dag/test_export.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/node/__init__.py
+-rw-r--r--   0        0        0    33197 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/node/test_basenode.py
+-rw-r--r--   0        0        0    36915 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/node/test_binarynode.py
+-rw-r--r--   0        0        0    33315 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/node/test_dagnode.py
+-rw-r--r--   0        0        0    14179 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/node/test_node.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/tree/__init__.py
+-rw-r--r--   0        0        0    66656 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/tree/test_construct.py
+-rw-r--r--   0        0        0    37681 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/tree/test_export.py
+-rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/tree/test_helper.py
+-rw-r--r--   0        0        0    67494 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/tree/test_modify.py
+-rw-r--r--   0        0        0    18425 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/tree/test_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/utils/__init__.py
+-rw-r--r--   0        0        0    13544 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/utils/test_iterators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/workflows/__init__.py
+-rw-r--r--   0        0        0    18086 2020-02-02 00:00:00.000000 bigtree-0.9.5/tests/workflows/test_todo.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 bigtree-0.9.5/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bigtree-0.9.5/LICENSE
+-rw-r--r--   0        0        0    25351 2020-02-02 00:00:00.000000 bigtree-0.9.5/README.md
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 bigtree-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0    26531 2020-02-02 00:00:00.000000 bigtree-0.9.5/PKG-INFO
```

### Comparing `bigtree-0.9.4/.pre-commit-config.yaml` & `bigtree-0.9.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/CHANGELOG.md` & `bigtree-0.9.5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.9.5] - 2023-07-13
+### Added
+- Misc: Added init files, add link to discussions to README and pyproject, add sphinx coverage shortcuts.
+### Fixed
+- [#66] DAGNode/Node: Children constructor to allow Iterable types, fixed issue of lists being mutable.
+- [#67] Node: `path_name` to reduce number of recursive calls to root node for `sep`.
+
 ## [0.9.4] - 2023-06-18
 ### Added
 - Tree Constructor: `list_to_tree_by_relation` and `dataframe_to_tree_by_relation` method to allow duplicate intermediate nodes (default is false).
 - DAG Exporter: Added `node_shape` parameter in `dag_to_dot` export function for easier way to customize node shape.
 - Misc: More test cases.
 - Misc: Added security instructions on how to raise vulnerabilities.
 - Misc: Added Calendar workflow to documentation.
@@ -273,14 +280,15 @@
 - Tree Exporter: To list, nested dictionary, pandas DataFrame.
 - Tree Helper: Cloning, pruning trees, get difference between two trees.
 - Tree Modifier: Shift and copy nodes within tree and between trees.
 - Tree Search: Find single or multiple nodes based on name, attribute, or custom criteria.
 - Utility Iterator: Tree traversal methods.
 - Workflow To Do App: Tree use case with to-do list implementation.
 
+[0.9.5]: https://github.com/kayjan/bigtree/compare/0.9.4...0.9.5
 [0.9.4]: https://github.com/kayjan/bigtree/compare/0.9.3...0.9.4
 [0.9.3]: https://github.com/kayjan/bigtree/compare/0.9.2...0.9.3
 [0.9.2]: https://github.com/kayjan/bigtree/compare/0.9.1...0.9.2
 [0.9.1]: https://github.com/kayjan/bigtree/compare/0.9.0...0.9.1
 [0.9.0]: https://github.com/kayjan/bigtree/compare/0.8.4...0.9.0
 [0.8.4]: https://github.com/kayjan/bigtree/compare/0.8.3...0.8.4
 [0.8.3]: https://github.com/kayjan/bigtree/compare/0.8.2...0.8.3
```

### Comparing `bigtree-0.9.4/SECURITY.md` & `bigtree-0.9.5/SECURITY.md`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/.github/workflows/codecov.yml` & `bigtree-0.9.5/.github/workflows/codecov.yml`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/.github/workflows/docs.yml` & `bigtree-0.9.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/.github/workflows/pytest.yml` & `bigtree-0.9.5/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/.github/workflows/python-publish.yml` & `bigtree-0.9.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/assets/DejaVuSans.ttf` & `bigtree-0.9.5/assets/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/assets/binarytree.png` & `bigtree-0.9.5/assets/binarytree.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/assets/custom_tree.png` & `bigtree-0.9.5/assets/custom_tree.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/assets/dag_construct.png` & `bigtree-0.9.5/assets/dag_construct.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/assets/demo.png` & `bigtree-0.9.5/assets/demo.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/assets/demo_binarytree.png` & `bigtree-0.9.5/assets/demo_binarytree.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/assets/demo_dag.png` & `bigtree-0.9.5/assets/demo_dag.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/assets/demo_pillow.png` & `bigtree-0.9.5/assets/demo_pillow.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/assets/demo_tree.png` & `bigtree-0.9.5/assets/demo_tree.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/assets/modify_advanced.png` & `bigtree-0.9.5/assets/modify_advanced.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/assets/modify_shift_and_copy.png` & `bigtree-0.9.5/assets/modify_shift_and_copy.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/assets/tree_construct.png` & `bigtree-0.9.5/assets/tree_construct.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/assets/weighted_tree.png` & `bigtree-0.9.5/assets/weighted_tree.png`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/bigtree/__init__.py` & `bigtree-0.9.5/bigtree/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.4"
+__version__ = "0.9.5"
 
 from bigtree.binarytree.construct import list_to_binarytree
 from bigtree.dag.construct import dataframe_to_dag, dict_to_dag, list_to_dag
 from bigtree.dag.export import dag_to_dataframe, dag_to_dict, dag_to_dot, dag_to_list
 from bigtree.node.basenode import BaseNode
 from bigtree.node.binarynode import BinaryNode
 from bigtree.node.dagnode import DAGNode
```

### Comparing `bigtree-0.9.4/bigtree/binarytree/construct.py` & `bigtree-0.9.5/bigtree/binarytree/construct.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/bigtree/dag/construct.py` & `bigtree-0.9.5/bigtree/dag/construct.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/bigtree/dag/export.py` & `bigtree-0.9.5/bigtree/dag/export.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/bigtree/node/basenode.py` & `bigtree-0.9.5/bigtree/node/basenode.py`

 * *Files 6% similar despite different names*

```diff
@@ -246,30 +246,30 @@
         """Do not allow `parents` attribute to be set
 
         Args:
             new_parent (Self): parent node
         """
         raise ValueError("Attempting to set `parents` attribute, do you mean `parent`?")
 
-    def __check_children_type(self: T, new_children: List[T]) -> None:
+    def __check_children_type(self: T, new_children: Iterable[T]) -> None:
         """Check child type
 
         Args:
-            new_children (List[Self]): child node
+            new_children (Iterable[Self]): child node
         """
-        if not isinstance(new_children, list):
+        if not isinstance(new_children, Iterable):
             raise TypeError(
-                f"Children input should be list type, received input type {type(new_children)}"
+                f"Children input should be Iterable type, received input type {type(new_children)}"
             )
 
-    def __check_children_loop(self: T, new_children: List[T]) -> None:
+    def __check_children_loop(self: T, new_children: Iterable[T]) -> None:
         """Check child loop
 
         Args:
-            new_children (List[Self]): child node
+            new_children (Iterable[Self]): child node
         """
         seen_children = []
         for new_child in new_children:
             # Check type
             if not isinstance(new_child, BaseNode):
                 raise TypeError(
                     f"Expect input to be BaseNode type, received input type {type(new_child)}"
@@ -297,22 +297,23 @@
 
         Returns:
             (Tuple[Self, ...])
         """
         return tuple(self.__children)
 
     @children.setter
-    def children(self: T, new_children: List[T]) -> None:
+    def children(self: T, new_children: Iterable[T]) -> None:
         """Set child nodes
 
         Args:
             new_children (List[Self]): child node
         """
         self.__check_children_type(new_children)
         self.__check_children_loop(new_children)
+        new_children = list(new_children)
 
         current_new_children = {
             new_child: (new_child.parent.__children.index(new_child), new_child.parent)
             for new_child in new_children
             if new_child.parent is not None
         }
         current_new_orphan = [
@@ -351,29 +352,29 @@
     @children.deleter
     def children(self) -> None:
         """Delete child node(s)"""
         for child in self.children:
             child.parent.__children.remove(child)  # type: ignore
             child.__parent = None
 
-    def __pre_assign_children(self: T, new_children: List[T]) -> None:
+    def __pre_assign_children(self: T, new_children: Iterable[T]) -> None:
         """Custom method to check before attaching children
         Can be overriden with `_BaseNode__pre_assign_children()`
 
         Args:
-            new_children (List[Self]): new children to be added
+            new_children (Iterable[Self]): new children to be added
         """
         pass
 
-    def __post_assign_children(self: T, new_children: List[T]) -> None:
+    def __post_assign_children(self: T, new_children: Iterable[T]) -> None:
         """Custom method to check after attaching children
         Can be overriden with `_BaseNode__post_assign_children()`
 
         Args:
-            new_children (List[Self]): new children to be added
+            new_children (Iterable[Self]): new children to be added
         """
         pass
 
     @property
     def ancestors(self: T) -> Iterable[T]:
         """Get iterator to yield all ancestors of self, does not include self
```

### Comparing `bigtree-0.9.4/bigtree/node/binarynode.py` & `bigtree-0.9.5/bigtree/node/binarynode.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/bigtree/node/dagnode.py` & `bigtree-0.9.5/bigtree/node/dagnode.py`

 * *Files 4% similar despite different names*

```diff
@@ -236,30 +236,30 @@
         Can be overriden with `_DAGNode__post_assign_parent()`
 
         Args:
             new_parents (List[Self]): new parents to be added
         """
         pass
 
-    def __check_children_type(self: T, new_children: List[T]) -> None:
+    def __check_children_type(self: T, new_children: Iterable[T]) -> None:
         """Check child type
 
         Args:
-            new_children (List[Self]): child node
+            new_children (Iterable[Self]): child node
         """
-        if not isinstance(new_children, list):
+        if not isinstance(new_children, Iterable):
             raise TypeError(
-                f"Children input should be list type, received input type {type(new_children)}"
+                f"Children input should be Iterable type, received input type {type(new_children)}"
             )
 
-    def __check_children_loop(self: T, new_children: List[T]) -> None:
+    def __check_children_loop(self: T, new_children: Iterable[T]) -> None:
         """Check child loop
 
         Args:
-            new_children (List[Self]): child node
+            new_children (Iterable[Self]): child node
         """
         seen_children = []
         for new_child in new_children:
             # Check type
             if not isinstance(new_child, DAGNode):
                 raise TypeError(
                     f"Expect input to be DAGNode type, received input type {type(new_child)}"
@@ -287,19 +287,19 @@
 
         Returns:
             (Iterable[Self])
         """
         return tuple(self.__children)
 
     @children.setter
-    def children(self: T, new_children: List[T]) -> None:
+    def children(self: T, new_children: Iterable[T]) -> None:
         """Set child nodes
 
         Args:
-            new_children (List[Self]): child node
+            new_children (Iterable[Self]): child node
         """
         self.__check_children_type(new_children)
         self.__check_children_loop(new_children)
 
         current_children = list(self.children)
 
         # Assign new children - rollback if error
@@ -315,24 +315,24 @@
             # Reassign old children to self
             for new_child in new_children:
                 if new_child not in current_children:
                     new_child.__parents.remove(self)
                     self.__children.remove(new_child)
             raise TreeError(exc_info)
 
-    def __pre_assign_children(self: T, new_children: List[T]) -> None:
+    def __pre_assign_children(self: T, new_children: Iterable[T]) -> None:
         """Custom method to check before attaching children
         Can be overriden with `_DAGNode__pre_assign_children()`
 
         Args:
             new_children (List[Self]): new children to be added
         """
         pass
 
-    def __post_assign_children(self: T, new_children: List[T]) -> None:
+    def __post_assign_children(self: T, new_children: Iterable[T]) -> None:
         """Custom method to check after attaching children
         Can be overriden with `_DAGNode__post_assign_children()`
 
         Args:
             new_children (List[Self]): new children to be added
         """
         pass
```

### Comparing `bigtree-0.9.4/bigtree/node/node.py` & `bigtree-0.9.5/bigtree/node/node.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,17 +110,17 @@
     @property
     def path_name(self) -> str:
         """Get path name, separated by self.sep
 
         Returns:
             (str)
         """
-        if self.parent is None:
-            return f"{self.sep}{self.name}"
-        return f"{self.parent.path_name}{self.sep}{self.name}"
+        ancestors = [self] + list(self.ancestors)
+        sep = ancestors[-1].sep
+        return sep + sep.join([node.name for node in reversed(ancestors)])
 
     def __pre_assign_children(self: T, new_children: List[T]) -> None:
         """Custom method to check before attaching children
         Can be overriden with `_Node__pre_assign_children()`
 
         Args:
             new_children (List[Self]): new children to be added
```

### Comparing `bigtree-0.9.4/bigtree/tree/construct.py` & `bigtree-0.9.5/bigtree/tree/construct.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/bigtree/tree/export.py` & `bigtree-0.9.5/bigtree/tree/export.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/bigtree/tree/helper.py` & `bigtree-0.9.5/bigtree/tree/helper.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/bigtree/tree/modify.py` & `bigtree-0.9.5/bigtree/tree/modify.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/bigtree/tree/search.py` & `bigtree-0.9.5/bigtree/tree/search.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/bigtree/utils/iterators.py` & `bigtree-0.9.5/bigtree/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/bigtree/workflows/app_calendar.py` & `bigtree-0.9.5/bigtree/workflows/app_calendar.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/bigtree/workflows/app_todo.py` & `bigtree-0.9.5/bigtree/workflows/app_todo.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/docs/Makefile` & `bigtree-0.9.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/docs/make.bat` & `bigtree-0.9.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/docs/source/conf.py` & `bigtree-0.9.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/docs/source/index.rst` & `bigtree-0.9.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/docs/source/_static/custom.css` & `bigtree-0.9.5/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/docs/source/_static/favicon.ico` & `bigtree-0.9.5/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/docs/source/_templates/layout.html` & `bigtree-0.9.5/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/docs/source/bigtree/dag/construct.rst` & `bigtree-0.9.5/docs/source/bigtree/dag/construct.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/docs/source/bigtree/dag/export.rst` & `bigtree-0.9.5/docs/source/bigtree/dag/export.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/docs/source/bigtree/tree/construct.rst` & `bigtree-0.9.5/docs/source/bigtree/tree/construct.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/docs/source/bigtree/tree/export.rst` & `bigtree-0.9.5/docs/source/bigtree/tree/export.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/docs/source/bigtree/tree/modify.rst` & `bigtree-0.9.5/docs/source/bigtree/tree/modify.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/docs/source/bigtree/tree/search.rst` & `bigtree-0.9.5/docs/source/bigtree/tree/search.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/docs/source/bigtree/utils/iterators.rst` & `bigtree-0.9.5/docs/source/bigtree/utils/iterators.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/docs/source/others/contributing.rst` & `bigtree-0.9.5/docs/source/others/contributing.rst`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/docs/source/others/merging_trees.md` & `bigtree-0.9.5/docs/source/others/merging_trees.md`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/docs/source/others/nodes.md` & `bigtree-0.9.5/docs/source/others/nodes.md`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/docs/source/others/weighted_trees.md` & `bigtree-0.9.5/docs/source/others/weighted_trees.md`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/tests/conftest.py` & `bigtree-0.9.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/tests/constants.py` & `bigtree-0.9.5/tests/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     ERROR_SET_DUPLICATE_CHILD = (
         "Error setting child: Node cannot be added multiple times as a child"
     )
     ERROR_SET_DUPLICATE_PARENT = (
         "Error setting parent: Node cannot be added multiple times as a parent"
     )
 
-    ERROR_CHILDREN_TYPE = "Children input should be list type, received input type"
+    ERROR_CHILDREN_TYPE = "Children input should be Iterable type, received input type"
     ERROR_BASENODE_CHILDREN_TYPE = (
         "Expect input to be BaseNode type, received input type"
     )
     ERROR_BASENODE_PARENT_TYPE = (
         "Expect input to be BaseNode type or NoneType, received input type"
     )
```

### Comparing `bigtree-0.9.4/tests/binarytree/test_construct.py` & `bigtree-0.9.5/tests/binarytree/test_construct.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/tests/binarytree/test_export.py` & `bigtree-0.9.5/tests/binarytree/test_export.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/tests/binarytree/test_helper.py` & `bigtree-0.9.5/tests/binarytree/test_helper.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/tests/binarytree/test_search.py` & `bigtree-0.9.5/tests/binarytree/test_search.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/tests/dag/test_construct.py` & `bigtree-0.9.5/tests/dag/test_construct.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/tests/dag/test_export.py` & `bigtree-0.9.5/tests/dag/test_export.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/tests/node/test_basenode.py` & `bigtree-0.9.5/tests/node/test_basenode.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,14 +363,34 @@
 
         with pytest.raises(LoopError) as exc_info:
             self.b.parent = self.a
             self.c.parent = self.b
             self.a.parent = self.c
         assert str(exc_info.value) == Constants.ERROR_LOOP_ANCESTOR
 
+    def test_set_children_mutable_list(self):
+        children_list = [self.b, self.c, self.d]
+        self.a.children = children_list
+        children_list.pop()
+        actual_children = self.a.children
+        expected_children = (self.b, self.c, self.d)
+        assert (
+            actual_children == expected_children
+        ), f"Expected {expected_children}, Received {actual_children}"
+
+    def test_set_children_iterable(self):
+        self.a.children = (self.b, self.c)
+        self.b.children = {self.d: 0, self.e: 0}
+        self.c.children = {self.f}
+        self.e.children = (self.g, self.h)
+
+        assert_tree_structure_basenode_root(self.a)
+        assert_tree_structure_basenode_root_attr(self.a)
+        assert_tree_structure_basenode_self(self)
+
     def test_set_children_type_error(self):
         with pytest.raises(TypeError) as exc_info:
             self.a.children = [self.b, 1]
         assert str(exc_info.value).startswith(Constants.ERROR_BASENODE_CHILDREN_TYPE)
 
         with pytest.raises(TypeError) as exc_info:
             self.a.children = [self.b, None]
```

### Comparing `bigtree-0.9.4/tests/node/test_binarynode.py` & `bigtree-0.9.5/tests/node/test_binarynode.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/tests/node/test_dagnode.py` & `bigtree-0.9.5/tests/node/test_dagnode.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,14 +303,34 @@
         assert str(exc_info.value).startswith(Constants.ERROR_LOOP_ANCESTOR)
 
     def test_set_duplicate_parent_error(self):
         with pytest.raises(TreeError) as exc_info:
             self.a.parents = [self.b, self.b]
         assert str(exc_info.value).startswith(Constants.ERROR_SET_DUPLICATE_PARENT)
 
+    def test_set_children_mutable_list(self):
+        children_list = [self.c, self.d]
+        self.a.children = children_list
+        children_list.pop()
+        actual_children = self.a.children
+        expected_children = (self.c, self.d)
+        assert (
+            actual_children == expected_children
+        ), f"Expected {expected_children}, Received {actual_children}"
+
+    def test_set_children_iterable(self):
+        self.a.children = (self.c, self.d)
+        self.b.children = {self.c}
+        self.c.children = (self.d, self.f, self.g)
+        self.d.children = {self.e: 0, self.f: 0}
+        self.g.children = {self.h}
+
+        assert_dag_structure_self(self)
+        assert_dag_structure_root(self.a)
+
     def test_set_children_type_error(self):
         with pytest.raises(TypeError) as exc_info:
             self.a.children = 1
         assert str(exc_info.value).startswith(Constants.ERROR_CHILDREN_TYPE)
 
         with pytest.raises(TypeError) as exc_info:
             self.a.children = [self.b, 1]
```

### Comparing `bigtree-0.9.4/tests/node/test_node.py` & `bigtree-0.9.5/tests/node/test_node.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/tests/tree/test_construct.py` & `bigtree-0.9.5/tests/tree/test_construct.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/tests/tree/test_export.py` & `bigtree-0.9.5/tests/tree/test_export.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/tests/tree/test_helper.py` & `bigtree-0.9.5/tests/tree/test_helper.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/tests/tree/test_modify.py` & `bigtree-0.9.5/tests/tree/test_modify.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/tests/tree/test_search.py` & `bigtree-0.9.5/tests/tree/test_search.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/tests/utils/test_iterators.py` & `bigtree-0.9.5/tests/utils/test_iterators.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/tests/workflows/test_todo.py` & `bigtree-0.9.5/tests/workflows/test_todo.py`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/LICENSE` & `bigtree-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bigtree-0.9.4/README.md` & `bigtree-0.9.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ----
 
 Related Links:
 - [Documentation](https://bigtree.readthedocs.io/en/latest/)
 - [GitHub](https://github.com/kayjan/bigtree/)
 - [Changelog](https://github.com/kayjan/bigtree/blob/master/CHANGELOG.md)
 - [Issues](https://github.com/kayjan/bigtree/issues)
+- [Discussions](https://github.com/kayjan/bigtree/discussions)
 - [Contributing](https://bigtree.readthedocs.io/en/latest/others/contributing.html)
 - [PyPI](https://pypi.org/project/bigtree/)
 - Articles
   - [Python Tree Implementation with BigTree](https://towardsdatascience.com/python-tree-implementation-with-bigtree-13cdabd77adc#245a-94ae81f0b3f1)
 - <div><p>If you want to support bigtree, <a href="https://www.buymeacoffee.com/kayjan"><img src="https://img.shields.io/badge/Buy_Me_A_Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black" alt="Buy Me a Coffee" style="vertical-align:middle"></a></p></div>
 
 ----
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
 # Big Tree Python Package Tree Implementation for Python, integrated with
 Python list, dictionary, and pandas DataFrame. It is pythonic, making it easy
 to learn and extendable to many types of workflows. ---- Related Links: -
 [Documentation](https://bigtree.readthedocs.io/en/latest/) - [GitHub](https://
 github.com/kayjan/bigtree/) - [Changelog](https://github.com/kayjan/bigtree/
 blob/master/CHANGELOG.md) - [Issues](https://github.com/kayjan/bigtree/issues)
-- [Contributing](https://bigtree.readthedocs.io/en/latest/others/
-contributing.html) - [PyPI](https://pypi.org/project/bigtree/) - Articles -
-[Python Tree Implementation with BigTree](https://towardsdatascience.com/
-python-tree-implementation-with-bigtree-13cdabd77adc#245a-94ae81f0b3f1) -
+- [Discussions](https://github.com/kayjan/bigtree/discussions) - [Contributing]
+(https://bigtree.readthedocs.io/en/latest/others/contributing.html) - [PyPI]
+(https://pypi.org/project/bigtree/) - Articles - [Python Tree Implementation
+with BigTree](https://towardsdatascience.com/python-tree-implementation-with-
+bigtree-13cdabd77adc#245a-94ae81f0b3f1) -
 If you want to support bigtree, [Buy_Me_a_Coffee]
 ---- ## Components There are 3 segments to Big Tree consisting of Tree, Binary
 Tree, and Directed Acyclic Graph (DAG) implementation. For **Tree**
 implementation, there are 8 main components. 1. [**Node**](https://
 bigtree.readthedocs.io/en/latest/node.html) 1. ``BaseNode``, extendable class
 2. ``Node``, BaseNode with node name attribute 2. [**Constructing Tree**]
 (https://bigtree.readthedocs.io/en/latest/bigtree/tree/construct.html) 1. From
```

### Comparing `bigtree-0.9.4/pyproject.toml` & `bigtree-0.9.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
   "pandas",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://bigtree.readthedocs.io"
 Issues = "https://github.com/kayjan/bigtree/issues"
+Discussions = "https://github.com/kayjan/bigtree/discussions"
 Source = "https://github.com/kayjan/bigtree"
 
 [project.optional-dependencies]
 image = [
   "pydot",
   "Pillow",
 ]
@@ -71,14 +72,15 @@
   "myst-parser==0.18.1",
   "pandas==1.5.1",
   "sphinxemoji==0.2.0"
 ]
 
 [tool.hatch.envs.docs.scripts]
 html = "sphinx-build -M html docs/source docs/build"
+coverage = "sphinx-build -v -b coverage docs/source docs/build/coverage"
 clean = "sphinx-build -M clean docs/source docs/build"
 clean-html = "sphinx-build -M html docs/source docs/build & sphinx-build -M clean docs/source docs/build"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["37", "38", "39", "310", "311"]
 
 [tool.coverage.run]
```

### Comparing `bigtree-0.9.4/PKG-INFO` & `bigtree-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: bigtree
-Version: 0.9.4
+Version: 0.9.5
 Summary: Tree Implementation for Python, integrated with Python list, dictionary, and pandas DataFrame.
 Project-URL: Documentation, https://bigtree.readthedocs.io
 Project-URL: Issues, https://github.com/kayjan/bigtree/issues
+Project-URL: Discussions, https://github.com/kayjan/bigtree/discussions
 Project-URL: Source, https://github.com/kayjan/bigtree
 Author-email: Kay Jan <kayjanw@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: bigtree,tree
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -34,14 +35,15 @@
 ----
 
 Related Links:
 - [Documentation](https://bigtree.readthedocs.io/en/latest/)
 - [GitHub](https://github.com/kayjan/bigtree/)
 - [Changelog](https://github.com/kayjan/bigtree/blob/master/CHANGELOG.md)
 - [Issues](https://github.com/kayjan/bigtree/issues)
+- [Discussions](https://github.com/kayjan/bigtree/discussions)
 - [Contributing](https://bigtree.readthedocs.io/en/latest/others/contributing.html)
 - [PyPI](https://pypi.org/project/bigtree/)
 - Articles
   - [Python Tree Implementation with BigTree](https://towardsdatascience.com/python-tree-implementation-with-bigtree-13cdabd77adc#245a-94ae81f0b3f1)
 - <div><p>If you want to support bigtree, <a href="https://www.buymeacoffee.com/kayjan"><img src="https://img.shields.io/badge/Buy_Me_A_Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black" alt="Buy Me a Coffee" style="vertical-align:middle"></a></p></div>
 
 ----
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
-Metadata-Version: 2.1 Name: bigtree Version: 0.9.4 Summary: Tree Implementation
+Metadata-Version: 2.1 Name: bigtree Version: 0.9.5 Summary: Tree Implementation
 for Python, integrated with Python list, dictionary, and pandas DataFrame.
 Project-URL: Documentation, https://bigtree.readthedocs.io Project-URL: Issues,
-https://github.com/kayjan/bigtree/issues Project-URL: Source, https://
-github.com/kayjan/bigtree Author-email: Kay Jan
+https://github.com/kayjan/bigtree/issues Project-URL: Discussions, https://
+github.com/kayjan/bigtree/discussions Project-URL: Source, https://github.com/
+kayjan/bigtree Author-email: Kay Jan
 gmail.com> License-Expression: MIT License-File: LICENSE Keywords: bigtree,tree
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: Implementation :: CPython Classifier: Programming Language :: Python
@@ -15,18 +16,19 @@
 pydot; extra == 'image' Description-Content-Type: text/markdown # Big Tree
 Python Package Tree Implementation for Python, integrated with Python list,
 dictionary, and pandas DataFrame. It is pythonic, making it easy to learn and
 extendable to many types of workflows. ---- Related Links: - [Documentation]
 (https://bigtree.readthedocs.io/en/latest/) - [GitHub](https://github.com/
 kayjan/bigtree/) - [Changelog](https://github.com/kayjan/bigtree/blob/master/
 CHANGELOG.md) - [Issues](https://github.com/kayjan/bigtree/issues) -
-[Contributing](https://bigtree.readthedocs.io/en/latest/others/
-contributing.html) - [PyPI](https://pypi.org/project/bigtree/) - Articles -
-[Python Tree Implementation with BigTree](https://towardsdatascience.com/
-python-tree-implementation-with-bigtree-13cdabd77adc#245a-94ae81f0b3f1) -
+[Discussions](https://github.com/kayjan/bigtree/discussions) - [Contributing]
+(https://bigtree.readthedocs.io/en/latest/others/contributing.html) - [PyPI]
+(https://pypi.org/project/bigtree/) - Articles - [Python Tree Implementation
+with BigTree](https://towardsdatascience.com/python-tree-implementation-with-
+bigtree-13cdabd77adc#245a-94ae81f0b3f1) -
 If you want to support bigtree, [Buy_Me_a_Coffee]
 ---- ## Components There are 3 segments to Big Tree consisting of Tree, Binary
 Tree, and Directed Acyclic Graph (DAG) implementation. For **Tree**
 implementation, there are 8 main components. 1. [**Node**](https://
 bigtree.readthedocs.io/en/latest/node.html) 1. ``BaseNode``, extendable class
 2. ``Node``, BaseNode with node name attribute 2. [**Constructing Tree**]
 (https://bigtree.readthedocs.io/en/latest/bigtree/tree/construct.html) 1. From
```

