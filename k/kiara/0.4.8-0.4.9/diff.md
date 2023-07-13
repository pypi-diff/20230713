# Comparing `tmp/kiara-0.4.8.tar.gz` & `tmp/kiara-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara-0.4.8.tar", last modified: Mon May 23 10:25:38 2022, max compression
+gzip compressed data, was "kiara-0.4.9.tar", last modified: Mon May 23 11:51:33 2022, max compression
```

## Comparing `kiara-0.4.8.tar` & `kiara-0.4.9.tar`

### file list

```diff
@@ -1,389 +1,389 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.873853 kiara-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-05-23 10:24:56.000000 kiara-0.4.8/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-05-23 10:24:56.000000 kiara-0.4.8/.envrc.bak
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-05-23 10:24:56.000000 kiara-0.4.8/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-05-23 10:24:56.000000 kiara-0.4.8/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-05-23 10:24:56.000000 kiara-0.4.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.845852 kiara-0.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.845852 kiara-0.4.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-05-23 10:24:56.000000 kiara-0.4.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-05-23 10:24:56.000000 kiara-0.4.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-05-23 10:24:56.000000 kiara-0.4.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.849853 kiara-0.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-05-23 10:24:56.000000 kiara-0.4.8/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     8718 2022-05-23 10:24:56.000000 kiara-0.4.8/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-05-23 10:24:56.000000 kiara-0.4.8/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      763 2022-05-23 10:24:56.000000 kiara-0.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-05-23 10:24:56.000000 kiara-0.4.8/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-05-23 10:24:56.000000 kiara-0.4.8/.kiara_complete.zsh
--rw-r--r--   0 runner    (1001) docker     (121)     1883 2022-05-23 10:24:56.000000 kiara-0.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-05-23 10:24:56.000000 kiara-0.4.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10721 2022-05-23 10:24:56.000000 kiara-0.4.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)    16756 2022-05-23 10:24:56.000000 kiara-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-05-23 10:24:56.000000 kiara-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2352 2022-05-23 10:24:56.000000 kiara-0.4.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     4077 2022-05-23 10:25:38.873853 kiara-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3210 2022-05-23 10:24:56.000000 kiara-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.841853 kiara-0.4.8/ci/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.849853 kiara-0.4.8/ci/build/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-05-23 10:24:56.000000 kiara-0.4.8/ci/build/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.849853 kiara-0.4.8/ci/conda/
--rwxr-xr-x   0 runner    (1001) docker     (121)     7458 2022-05-23 10:24:56.000000 kiara-0.4.8/ci/conda/build-conda-packages.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.849853 kiara-0.4.8/ci/conda/kiara/
--rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-05-23 10:24:56.000000 kiara-0.4.8/ci/conda/kiara/meta.yaml.template
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.849853 kiara-0.4.8/ci/docker/
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-05-23 10:24:56.000000 kiara-0.4.8/ci/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-05-23 10:24:56.000000 kiara-0.4.8/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.849853 kiara-0.4.8/dev/
--rw-r--r--   0 runner    (1001) docker     (121)   134752 2022-05-23 10:24:56.000000 kiara-0.4.8/dev/dev.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 10:24:56.000000 kiara-0.4.8/dev/network_analysis.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     4063 2022-05-23 10:24:56.000000 kiara-0.4.8/dev/script.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.849853 kiara-0.4.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/SUMMARY.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.849853 kiara-0.4.8/docs/architecture/
--rw-r--r--   0 runner    (1001) docker     (121)     2141 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/assumptions.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.849853 kiara-0.4.8/docs/architecture/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.849853 kiara-0.4.8/docs/architecture/data/.ipynb_checkpoints/
--rw-r--r--   0 runner    (1001) docker     (121)    68007 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/data/.ipynb_checkpoints/data_formats-checkpoint.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   105053 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/data/.ipynb_checkpoints/requirements-checkpoint.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      878 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/data/data_centric_approach.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    67993 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/data/data_formats.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/data/dev.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     6152 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/data/index.md
--rw-r--r--   0 runner    (1001) docker     (121)    20616 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/data/persistence.md
--rw-r--r--   0 runner    (1001) docker     (121)   105120 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/data/requirements.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    17509 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/data/result_tree.png
--rw-r--r--   0 runner    (1001) docker     (121)     5724 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/decisions.md
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/index.md
--rw-r--r--   0 runner    (1001) docker     (121)     3399 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/metadata.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.849853 kiara-0.4.8/docs/architecture/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)    18476 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/workflows/index.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.849853 kiara-0.4.8/docs/architecture/workflows/modularity/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.849853 kiara-0.4.8/docs/architecture/workflows/modularity/.ipynb_checkpoints/
--rw-r--r--   0 runner    (1001) docker     (121)    63891 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/workflows/modularity/.ipynb_checkpoints/modularity-checkpoint.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    53034 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/workflows/modularity/.ipynb_checkpoints/modularity_2-checkpoint.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    63106 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/workflows/modularity/modularity.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    53370 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/workflows/modularity/modularity_2.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.849853 kiara-0.4.8/docs/architecture/workflows/modularity/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/workflows/modularity/workflows/corpus_processing.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/workflows/modularity/workflows/corpus_processing_simple.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      597 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/architecture/workflows/modularity/workflows/input_files_processing.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.849853 kiara-0.4.8/docs/included_components/
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/included_components/index.md
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/install.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.853853 kiara-0.4.8/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-05-23 10:24:56.000000 kiara-0.4.8/docs/stylesheets/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.841853 kiara-0.4.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.853853 kiara-0.4.8/examples/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.853853 kiara-0.4.8/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (121)     2989 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (121)    33398 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/journals/Readme.md
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/journals/query.graphql
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.853853 kiara-0.4.8/examples/data/text_corpus/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.853853 kiara-0.4.8/examples/data/text_corpus/La_Ragione/
--rw-r--r--   0 runner    (1001) docker     (121)    16613 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (121)    16679 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (121)    16793 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-3_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (121)    16235 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-4_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (121)    18346 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (121)    18474 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (121)    18280 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-3_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (121)    18481 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-4_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (121)    18620 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (121)    18698 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (121)    18540 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-3_seq-1_ocr.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.853853 kiara-0.4.8/examples/data/text_corpus/La_Rassegna/
--rw-r--r--   0 runner    (1001) docker     (121)    19397 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-07_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (121)    20647 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-14_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (121)    20650 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-14_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (121)    21017 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-21_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (121)    20982 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-21_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-05-23 10:24:56.000000 kiara-0.4.8/examples/data/text_corpus/Readme.md
--rw-r--r--   0 runner    (1001) docker     (121)     1385 2022-05-23 10:24:56.000000 kiara-0.4.8/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-05-23 10:24:56.000000 kiara-0.4.8/onboarding.folder_to_table.json
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-05-23 10:24:56.000000 kiara-0.4.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.841853 kiara-0.4.8/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.853853 kiara-0.4.8/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-05-23 10:24:56.000000 kiara-0.4.8/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-05-23 10:24:56.000000 kiara-0.4.8/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (121)     2190 2022-05-23 10:24:56.000000 kiara-0.4.8/scripts/documentation/gen_schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)    10829 2022-05-23 10:25:38.873853 kiara-0.4.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     2008 2022-05-23 10:24:56.000000 kiara-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.845852 kiara-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.853853 kiara-0.4.8/src/kiara/
--rw-r--r--   0 runner    (1001) docker     (121)     3534 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.857853 kiara-0.4.8/src/kiara/context/
--rw-r--r--   0 runner    (1001) docker     (121)    21677 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27984 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/context/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     6072 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/context/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.857853 kiara-0.4.8/src/kiara/data_types/
--rw-r--r--   0 runner    (1001) docker     (121)    18376 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/data_types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.857853 kiara-0.4.8/src/kiara/data_types/included_core_types/
--rw-r--r--   0 runner    (1001) docker     (121)     6456 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/data_types/included_core_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8052 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/data_types/included_core_types/filesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.857853 kiara-0.4.8/src/kiara/data_types/included_core_types/internal/
--rw-r--r--   0 runner    (1001) docker     (121)     5687 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/data_types/included_core_types/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3464 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/data_types/included_core_types/internal/render_value.py
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/data_types/included_core_types/serialization.py
--rw-r--r--   0 runner    (1001) docker     (121)     7067 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.857853 kiara-0.4.8/src/kiara/doc/
--rw-r--r--   0 runner    (1001) docker     (121)     3436 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/doc/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (121)     2227 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/doc/generate_api_doc.py
--rw-r--r--   0 runner    (1001) docker     (121)     6488 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/doc/mkdocs_macros_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     6029 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/doc/mkdocs_macros_kiara.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.857853 kiara-0.4.8/src/kiara/doc/mkdocstrings/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/doc/mkdocstrings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2565 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/doc/mkdocstrings/collector.py
--rw-r--r--   0 runner    (1001) docker     (121)     2942 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/doc/mkdocstrings/handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/doc/mkdocstrings/renderer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6242 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.857853 kiara-0.4.8/src/kiara/interfaces/
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.857853 kiara-0.4.8/src/kiara/interfaces/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     3796 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.857853 kiara-0.4.8/src/kiara/interfaces/cli/context/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/cli/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7488 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/cli/context/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.857853 kiara-0.4.8/src/kiara/interfaces/cli/data/
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/cli/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9913 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/cli/data/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.857853 kiara-0.4.8/src/kiara/interfaces/cli/dev/
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/cli/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1425 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/cli/dev/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.857853 kiara-0.4.8/src/kiara/interfaces/cli/module/
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/cli/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3854 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/cli/module/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.857853 kiara-0.4.8/src/kiara/interfaces/cli/operation/
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/cli/operation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4570 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/cli/operation/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.857853 kiara-0.4.8/src/kiara/interfaces/cli/pipeline/
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/cli/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8010 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/cli/pipeline/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     8960 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/cli/run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.857853 kiara-0.4.8/src/kiara/interfaces/cli/service/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/cli/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/cli/service/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.857853 kiara-0.4.8/src/kiara/interfaces/cli/type/
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/cli/type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3910 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/cli/type/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.857853 kiara-0.4.8/src/kiara/interfaces/python_api/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/python_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5481 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/python_api/batch.py
--rw-r--r--   0 runner    (1001) docker     (121)    12162 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/python_api/operation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1431 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/python_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1509 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/python_api/value.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.857853 kiara-0.4.8/src/kiara/interfaces/tui/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3629 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/interfaces/tui/pager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.861853 kiara-0.4.8/src/kiara/models/
--rw-r--r--   0 runner    (1001) docker     (121)     9203 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.861853 kiara-0.4.8/src/kiara/models/aliases/
--rw-r--r--   0 runner    (1001) docker     (121)    12722 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/aliases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7524 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/archives.py
--rw-r--r--   0 runner    (1001) docker     (121)     8728 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     7074 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/documentation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.861853 kiara-0.4.8/src/kiara/models/events/
--rw-r--r--   0 runner    (1001) docker     (121)      776 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/events/alias_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1560 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/events/data_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/events/destiny_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/events/job_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     7919 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/events/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)    16224 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (121)     9019 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.861853 kiara-0.4.8/src/kiara/models/module/
--rw-r--r--   0 runner    (1001) docker     (121)    11745 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6266 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/module/destiniy.py
--rw-r--r--   0 runner    (1001) docker     (121)     7029 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/module/jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4019 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/module/manifest.py
--rw-r--r--   0 runner    (1001) docker     (121)    21780 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/module/operation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/module/persistence.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.861853 kiara-0.4.8/src/kiara/models/module/pipeline/
--rw-r--r--   0 runner    (1001) docker     (121)    17501 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/module/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6417 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/module/pipeline/controller.py
--rw-r--r--   0 runner    (1001) docker     (121)    38997 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/module/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)    25750 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/module/pipeline/structure.py
--rw-r--r--   0 runner    (1001) docker     (121)     6794 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/module/pipeline/value_refs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2495 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/python_class.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.861853 kiara-0.4.8/src/kiara/models/render_value/
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/render_value/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.861853 kiara-0.4.8/src/kiara/models/runtime_environment/
--rw-r--r--   0 runner    (1001) docker     (121)     2467 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/runtime_environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1944 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/runtime_environment/kiara.py
--rw-r--r--   0 runner    (1001) docker     (121)     2097 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/runtime_environment/operating_system.py
--rw-r--r--   0 runner    (1001) docker     (121)     2416 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/runtime_environment/python.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.861853 kiara-0.4.8/src/kiara/models/values/
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/values/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8686 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/values/data_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    10418 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/values/info.py
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/values/lineage.py
--rw-r--r--   0 runner    (1001) docker     (121)    47155 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/values/value.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.861853 kiara-0.4.8/src/kiara/models/values/value_metadata/
--rw-r--r--   0 runner    (1001) docker     (121)     4146 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/values/value_metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.861853 kiara-0.4.8/src/kiara/models/values/value_metadata/included_metadata_types/
--rw-r--r--   0 runner    (1001) docker     (121)     2148 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/values/value_metadata/included_metadata_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2943 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/models/values/value_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.861853 kiara-0.4.8/src/kiara/modules/
--rw-r--r--   0 runner    (1001) docker     (121)    16068 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/modules/included_core_modules/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/modules/included_core_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4614 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/modules/included_core_modules/create_from.py
--rw-r--r--   0 runner    (1001) docker     (121)     8752 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/modules/included_core_modules/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (121)     2926 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/modules/included_core_modules/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     2362 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/modules/included_core_modules/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)     5934 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/modules/included_core_modules/pretty_print.py
--rw-r--r--   0 runner    (1001) docker     (121)     4444 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/modules/included_core_modules/render_value.py
--rw-r--r--   0 runner    (1001) docker     (121)    12509 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/modules/included_core_modules/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/operations/
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/operations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/operations/included_core_operations/
--rw-r--r--   0 runner    (1001) docker     (121)     3521 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/operations/included_core_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7177 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/operations/included_core_operations/create_from.py
--rw-r--r--   0 runner    (1001) docker     (121)     6069 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/operations/included_core_operations/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     7790 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/operations/included_core_operations/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)     9523 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/operations/included_core_operations/pretty_print.py
--rw-r--r--   0 runner    (1001) docker     (121)     7247 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/operations/included_core_operations/render_value.py
--rw-r--r--   0 runner    (1001) docker     (121)    10007 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/operations/included_core_operations/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/processing/
--rw-r--r--   0 runner    (1001) docker     (121)     8967 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/processing/synchronous.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/registries/
--rw-r--r--   0 runner    (1001) docker     (121)     3848 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/registries/aliases/
--rw-r--r--   0 runner    (1001) docker     (121)    11617 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/aliases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4649 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/aliases/archives.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/registries/data/
--rw-r--r--   0 runner    (1001) docker     (121)    32526 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/registries/data/data_store/
--rw-r--r--   0 runner    (1001) docker     (121)    16799 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/data/data_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16191 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/data/data_store/filesystem_store.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/registries/destinies/
--rw-r--r--   0 runner    (1001) docker     (121)     1319 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/destinies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6003 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/destinies/filesystem_store.py
--rw-r--r--   0 runner    (1001) docker     (121)    10204 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/destinies/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/registries/environment/
--rw-r--r--   0 runner    (1001) docker     (121)     4878 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/registries/events/
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3081 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/events/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     3099 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/events/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/registries/ids/
--rw-r--r--   0 runner    (1001) docker     (121)     1956 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/ids/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/registries/jobs/
--rw-r--r--   0 runner    (1001) docker     (121)    11381 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/jobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/registries/jobs/job_store/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/jobs/job_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4501 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/jobs/job_store/filesystem_store.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/registries/models/
--rw-r--r--   0 runner    (1001) docker     (121)     2998 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/registries/modules/
--rw-r--r--   0 runner    (1001) docker     (121)     3931 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/registries/operations/
--rw-r--r--   0 runner    (1001) docker     (121)    16106 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/operations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/registries/types/
--rw-r--r--   0 runner    (1001) docker     (121)     9553 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/registries/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/resources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/resources/database/
--rw-r--r--   0 runner    (1001) docker     (121)     2910 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/resources/database/alembic.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/resources/database/kiara/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/resources/database/kiara/README
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/resources/database/kiara/env.py
--rw-r--r--   0 runner    (1001) docker     (121)      541 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/resources/database/kiara/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.865853 kiara-0.4.8/src/kiara/resources/database/kiara/versions/
--rw-r--r--   0 runner    (1001) docker     (121)     9033 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/resources/database/kiara/versions/e90a32e90839_create_the_example_database.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      391 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/resources/database/reinit.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.845852 kiara-0.4.8/src/kiara/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.869853 kiara-0.4.8/src/kiara/resources/templates/doc_gen/
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/resources/templates/doc_gen/info_listing.j2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.869853 kiara-0.4.8/src/kiara/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     7740 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22057 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/utils/class_loading.py
--rw-r--r--   0 runner    (1001) docker     (121)     8169 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      825 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/utils/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (121)     3153 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2408 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/utils/db.py
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/utils/doc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/utils/global_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/utils/graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.869853 kiara-0.4.8/src/kiara/utils/hashfs/
--rw-r--r--   0 runner    (1001) docker     (121)    16435 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/utils/hashfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1615 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/utils/hashing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/utils/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/utils/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     3868 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1838 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/utils/operations.py
--rw-r--r--   0 runner    (1001) docker     (121)    26338 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/utils/output.py
--rw-r--r--   0 runner    (1001) docker     (121)     4634 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/utils/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (121)     4280 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/utils/string_vars.py
--rw-r--r--   0 runner    (1001) docker     (121)     3998 2022-05-23 10:24:56.000000 kiara-0.4.8/src/kiara/utils/values.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.853853 kiara-0.4.8/src/kiara.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4077 2022-05-23 10:25:38.000000 kiara-0.4.8/src/kiara.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11545 2022-05-23 10:25:38.000000 kiara-0.4.8/src/kiara.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-23 10:25:38.000000 kiara-0.4.8/src/kiara.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4581 2022-05-23 10:25:38.000000 kiara-0.4.8/src/kiara.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-23 10:25:33.000000 kiara-0.4.8/src/kiara.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-05-23 10:25:38.000000 kiara-0.4.8/src/kiara.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-23 10:25:38.000000 kiara-0.4.8/src/kiara.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.845852 kiara-0.4.8/src/mkdocstrings_handlers/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.869853 kiara-0.4.8/src/mkdocstrings_handlers/kiara/
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-05-23 10:24:56.000000 kiara-0.4.8/src/mkdocstrings_handlers/kiara/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.845852 kiara-0.4.8/src/mkdocstrings_handlers/kiara/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.869853 kiara-0.4.8/src/mkdocstrings_handlers/kiara/templates/material/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 10:24:56.000000 kiara-0.4.8/src/mkdocstrings_handlers/kiara/templates/material/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.869853 kiara-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3807 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.845852 kiara-0.4.8/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.869853 kiara-0.4.8/tests/resources/invalid_pipelines/
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/resources/invalid_pipelines/logic_4.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.869853 kiara-0.4.8/tests/resources/module_configs/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/resources/module_configs/and.json
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/resources/module_configs/and_wrapped.json
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/resources/module_configs/table_load.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.869853 kiara-0.4.8/tests/resources/pipelines/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.869853 kiara-0.4.8/tests/resources/pipelines/dummy/
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/resources/pipelines/dummy/dummy_1.json
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/resources/pipelines/dummy/dummy_1_delay.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.873853 kiara-0.4.8/tests/resources/pipelines/logic/
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/resources/pipelines/logic/logic_1.json
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/resources/pipelines/logic/logic_2.json
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/resources/pipelines/logic/logic_3.json
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/resources/pipelines/logic/logic_4.json
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/resources/pipelines/table_import.json
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/resources/pipelines/test_preseed_1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.873853 kiara-0.4.8/tests/test_cli/
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2289 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_cli/test_data_subcommands.py
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_cli/test_info_subcommands.py
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_cli/test_metadata_subcommands.py
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_cli/test_misc_commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     1385 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_cli/test_module_subcommands.py
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_cli/test_operation_subcommands.py
--rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_cli/test_pipeline_subcommands.py
--rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_cli/test_run_subcommand.py
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_kiara_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     3181 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_module_instances.py
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_module_types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.873853 kiara-0.4.8/tests/test_modules/
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_modules/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_modules/test_simple_module_exec.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.873853 kiara-0.4.8/tests/test_operation_types/
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_operation_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_operation_types/test_extract_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_operation_types/test_persist_value.py
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_operation_types/test_render_value.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2579 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_pipeline_creation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2309 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (121)     1593 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_rendering.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:25:38.873853 kiara-0.4.8/tests/test_values/
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_values/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2897 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/test_values/test_values.py
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-05-23 10:24:56.000000 kiara-0.4.8/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.215277 kiara-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-05-23 11:50:46.000000 kiara-0.4.9/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2022-05-23 11:50:46.000000 kiara-0.4.9/.envrc.bak
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2022-05-23 11:50:46.000000 kiara-0.4.9/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-05-23 11:50:46.000000 kiara-0.4.9/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-05-23 11:50:46.000000 kiara-0.4.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.171274 kiara-0.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.171274 kiara-0.4.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      829 2022-05-23 11:50:46.000000 kiara-0.4.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (121)      595 2022-05-23 11:50:46.000000 kiara-0.4.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2022-05-23 11:50:46.000000 kiara-0.4.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.171274 kiara-0.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-05-23 11:50:46.000000 kiara-0.4.9/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     8718 2022-05-23 11:50:46.000000 kiara-0.4.9/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-05-23 11:50:46.000000 kiara-0.4.9/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      763 2022-05-23 11:50:46.000000 kiara-0.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      934 2022-05-23 11:50:46.000000 kiara-0.4.9/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      851 2022-05-23 11:50:46.000000 kiara-0.4.9/.kiara_complete.zsh
+-rw-r--r--   0 runner    (1001) docker     (121)     1883 2022-05-23 11:50:46.000000 kiara-0.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-05-23 11:50:46.000000 kiara-0.4.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10721 2022-05-23 11:50:46.000000 kiara-0.4.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)    16756 2022-05-23 11:50:46.000000 kiara-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2022-05-23 11:50:46.000000 kiara-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2352 2022-05-23 11:50:46.000000 kiara-0.4.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     4077 2022-05-23 11:51:33.215277 kiara-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3210 2022-05-23 11:50:46.000000 kiara-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.163273 kiara-0.4.9/ci/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.171274 kiara-0.4.9/ci/build/
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-05-23 11:50:46.000000 kiara-0.4.9/ci/build/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.171274 kiara-0.4.9/ci/conda/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7458 2022-05-23 11:50:46.000000 kiara-0.4.9/ci/conda/build-conda-packages.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.171274 kiara-0.4.9/ci/conda/kiara/
+-rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-05-23 11:50:46.000000 kiara-0.4.9/ci/conda/kiara/meta.yaml.template
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.171274 kiara-0.4.9/ci/docker/
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2022-05-23 11:50:46.000000 kiara-0.4.9/ci/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-05-23 11:50:46.000000 kiara-0.4.9/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.175274 kiara-0.4.9/dev/
+-rw-r--r--   0 runner    (1001) docker     (121)   134752 2022-05-23 11:50:46.000000 kiara-0.4.9/dev/dev.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 11:50:46.000000 kiara-0.4.9/dev/network_analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     4063 2022-05-23 11:50:46.000000 kiara-0.4.9/dev/script.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.175274 kiara-0.4.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.175274 kiara-0.4.9/docs/architecture/
+-rw-r--r--   0 runner    (1001) docker     (121)     2141 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/assumptions.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.175274 kiara-0.4.9/docs/architecture/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.175274 kiara-0.4.9/docs/architecture/data/.ipynb_checkpoints/
+-rw-r--r--   0 runner    (1001) docker     (121)    68007 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/data/.ipynb_checkpoints/data_formats-checkpoint.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   105053 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/data/.ipynb_checkpoints/requirements-checkpoint.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)      878 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/data/data_centric_approach.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    67993 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/data/data_formats.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)      592 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/data/dev.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     6152 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/data/index.md
+-rw-r--r--   0 runner    (1001) docker     (121)    20616 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/data/persistence.md
+-rw-r--r--   0 runner    (1001) docker     (121)   105120 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/data/requirements.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    17509 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/data/result_tree.png
+-rw-r--r--   0 runner    (1001) docker     (121)     5724 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/decisions.md
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/index.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3399 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/metadata.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.175274 kiara-0.4.9/docs/architecture/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)    18476 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/workflows/index.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.175274 kiara-0.4.9/docs/architecture/workflows/modularity/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.175274 kiara-0.4.9/docs/architecture/workflows/modularity/.ipynb_checkpoints/
+-rw-r--r--   0 runner    (1001) docker     (121)    63891 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/workflows/modularity/.ipynb_checkpoints/modularity-checkpoint.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    53034 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/workflows/modularity/.ipynb_checkpoints/modularity_2-checkpoint.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    63106 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/workflows/modularity/modularity.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    53370 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/workflows/modularity/modularity_2.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.175274 kiara-0.4.9/docs/architecture/workflows/modularity/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      740 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/workflows/modularity/workflows/corpus_processing.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/workflows/modularity/workflows/corpus_processing_simple.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      597 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/architecture/workflows/modularity/workflows/input_files_processing.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.175274 kiara-0.4.9/docs/included_components/
+-rw-r--r--   0 runner    (1001) docker     (121)      287 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/included_components/index.md
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (121)      839 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/install.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.179274 kiara-0.4.9/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2022-05-23 11:50:46.000000 kiara-0.4.9/docs/stylesheets/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.163273 kiara-0.4.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.179274 kiara-0.4.9/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.179274 kiara-0.4.9/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (121)     2989 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    33398 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/journals/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/journals/query.graphql
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.179274 kiara-0.4.9/examples/data/text_corpus/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.179274 kiara-0.4.9/examples/data/text_corpus/La_Ragione/
+-rw-r--r--   0 runner    (1001) docker     (121)    16613 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    16679 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    16793 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-3_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    16235 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-4_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    18346 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    18474 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    18280 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-3_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    18481 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-4_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    18620 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    18698 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    18540 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-3_seq-1_ocr.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.179274 kiara-0.4.9/examples/data/text_corpus/La_Rassegna/
+-rw-r--r--   0 runner    (1001) docker     (121)    19397 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-07_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    20647 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-14_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    20650 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-14_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    21017 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-21_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    20982 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-21_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2022-05-23 11:50:46.000000 kiara-0.4.9/examples/data/text_corpus/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1385 2022-05-23 11:50:46.000000 kiara-0.4.9/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2022-05-23 11:50:46.000000 kiara-0.4.9/onboarding.folder_to_table.json
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-05-23 11:50:46.000000 kiara-0.4.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.163273 kiara-0.4.9/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.179274 kiara-0.4.9/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (121)      926 2022-05-23 11:50:46.000000 kiara-0.4.9/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (121)      471 2022-05-23 11:50:46.000000 kiara-0.4.9/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2190 2022-05-23 11:50:46.000000 kiara-0.4.9/scripts/documentation/gen_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10829 2022-05-23 11:51:33.219277 kiara-0.4.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2008 2022-05-23 11:50:46.000000 kiara-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.167274 kiara-0.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.179274 kiara-0.4.9/src/kiara/
+-rw-r--r--   0 runner    (1001) docker     (121)     3534 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.187275 kiara-0.4.9/src/kiara/context/
+-rw-r--r--   0 runner    (1001) docker     (121)    21677 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27984 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/context/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6072 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/context/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.187275 kiara-0.4.9/src/kiara/data_types/
+-rw-r--r--   0 runner    (1001) docker     (121)    18376 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/data_types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.187275 kiara-0.4.9/src/kiara/data_types/included_core_types/
+-rw-r--r--   0 runner    (1001) docker     (121)     6456 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/data_types/included_core_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8052 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/data_types/included_core_types/filesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.187275 kiara-0.4.9/src/kiara/data_types/included_core_types/internal/
+-rw-r--r--   0 runner    (1001) docker     (121)     5687 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/data_types/included_core_types/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3464 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/data_types/included_core_types/internal/render_value.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/data_types/included_core_types/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7067 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.191275 kiara-0.4.9/src/kiara/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)     3436 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/doc/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2227 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/doc/generate_api_doc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6488 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/doc/mkdocs_macros_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6029 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/doc/mkdocs_macros_kiara.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.191275 kiara-0.4.9/src/kiara/doc/mkdocstrings/
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/doc/mkdocstrings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2565 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/doc/mkdocstrings/collector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2942 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/doc/mkdocstrings/handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      844 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/doc/mkdocstrings/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6242 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.191275 kiara-0.4.9/src/kiara/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (121)      852 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.191275 kiara-0.4.9/src/kiara/interfaces/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)     3796 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.191275 kiara-0.4.9/src/kiara/interfaces/cli/context/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/cli/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7488 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/cli/context/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.191275 kiara-0.4.9/src/kiara/interfaces/cli/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/cli/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9913 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/cli/data/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.191275 kiara-0.4.9/src/kiara/interfaces/cli/dev/
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/cli/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1425 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/cli/dev/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.191275 kiara-0.4.9/src/kiara/interfaces/cli/module/
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/cli/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3854 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/cli/module/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.191275 kiara-0.4.9/src/kiara/interfaces/cli/operation/
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/cli/operation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4570 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/cli/operation/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.191275 kiara-0.4.9/src/kiara/interfaces/cli/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/cli/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8010 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/cli/pipeline/commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8960 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.191275 kiara-0.4.9/src/kiara/interfaces/cli/service/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/cli/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/cli/service/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.195276 kiara-0.4.9/src/kiara/interfaces/cli/type/
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/cli/type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3910 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/cli/type/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.195276 kiara-0.4.9/src/kiara/interfaces/python_api/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/python_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5481 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/python_api/batch.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12162 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/python_api/operation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1431 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/python_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1509 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/python_api/value.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.195276 kiara-0.4.9/src/kiara/interfaces/tui/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3629 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/interfaces/tui/pager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.195276 kiara-0.4.9/src/kiara/models/
+-rw-r--r--   0 runner    (1001) docker     (121)     9203 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.195276 kiara-0.4.9/src/kiara/models/aliases/
+-rw-r--r--   0 runner    (1001) docker     (121)    12722 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/aliases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7524 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/archives.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8728 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7074 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/documentation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.195276 kiara-0.4.9/src/kiara/models/events/
+-rw-r--r--   0 runner    (1001) docker     (121)      776 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/events/alias_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1560 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/events/data_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)      741 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/events/destiny_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/events/job_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7919 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/events/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16224 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9019 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/info.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.199276 kiara-0.4.9/src/kiara/models/module/
+-rw-r--r--   0 runner    (1001) docker     (121)    11745 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6266 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/module/destiniy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7029 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/module/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4019 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/module/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21780 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/module/operation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/module/persistence.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.199276 kiara-0.4.9/src/kiara/models/module/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (121)    17501 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/module/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6417 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/module/pipeline/controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38997 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/module/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25750 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/module/pipeline/structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6794 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/module/pipeline/value_refs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2495 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/python_class.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.199276 kiara-0.4.9/src/kiara/models/render_value/
+-rw-r--r--   0 runner    (1001) docker     (121)      955 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/render_value/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.199276 kiara-0.4.9/src/kiara/models/runtime_environment/
+-rw-r--r--   0 runner    (1001) docker     (121)     2467 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/runtime_environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1944 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/runtime_environment/kiara.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2097 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/runtime_environment/operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2416 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/runtime_environment/python.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.199276 kiara-0.4.9/src/kiara/models/values/
+-rw-r--r--   0 runner    (1001) docker     (121)      385 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8686 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/values/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10418 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/values/info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/values/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (121)    47172 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/values/value.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.203276 kiara-0.4.9/src/kiara/models/values/value_metadata/
+-rw-r--r--   0 runner    (1001) docker     (121)     4146 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/values/value_metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.203276 kiara-0.4.9/src/kiara/models/values/value_metadata/included_metadata_types/
+-rw-r--r--   0 runner    (1001) docker     (121)     2148 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/values/value_metadata/included_metadata_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2943 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/models/values/value_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.203276 kiara-0.4.9/src/kiara/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)    16068 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.203276 kiara-0.4.9/src/kiara/modules/included_core_modules/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/modules/included_core_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4614 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/modules/included_core_modules/create_from.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8752 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/modules/included_core_modules/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2926 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/modules/included_core_modules/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2362 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/modules/included_core_modules/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6141 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/modules/included_core_modules/pretty_print.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4443 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/modules/included_core_modules/render_value.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12509 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/modules/included_core_modules/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.203276 kiara-0.4.9/src/kiara/operations/
+-rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/operations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.203276 kiara-0.4.9/src/kiara/operations/included_core_operations/
+-rw-r--r--   0 runner    (1001) docker     (121)     3521 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/operations/included_core_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7177 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/operations/included_core_operations/create_from.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6069 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/operations/included_core_operations/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7790 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/operations/included_core_operations/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9523 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/operations/included_core_operations/pretty_print.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7247 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/operations/included_core_operations/render_value.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10007 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/operations/included_core_operations/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.203276 kiara-0.4.9/src/kiara/processing/
+-rw-r--r--   0 runner    (1001) docker     (121)     8967 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/processing/synchronous.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.203276 kiara-0.4.9/src/kiara/registries/
+-rw-r--r--   0 runner    (1001) docker     (121)     3848 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.203276 kiara-0.4.9/src/kiara/registries/aliases/
+-rw-r--r--   0 runner    (1001) docker     (121)    11617 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/aliases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4649 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/aliases/archives.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.203276 kiara-0.4.9/src/kiara/registries/data/
+-rw-r--r--   0 runner    (1001) docker     (121)    32526 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.207277 kiara-0.4.9/src/kiara/registries/data/data_store/
+-rw-r--r--   0 runner    (1001) docker     (121)    16799 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/data/data_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16191 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/data/data_store/filesystem_store.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.207277 kiara-0.4.9/src/kiara/registries/destinies/
+-rw-r--r--   0 runner    (1001) docker     (121)     1319 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/destinies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6003 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/destinies/filesystem_store.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10204 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/destinies/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.207277 kiara-0.4.9/src/kiara/registries/environment/
+-rw-r--r--   0 runner    (1001) docker     (121)     4878 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.207277 kiara-0.4.9/src/kiara/registries/events/
+-rw-r--r--   0 runner    (1001) docker     (121)      644 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3081 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/events/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3099 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/events/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.207277 kiara-0.4.9/src/kiara/registries/ids/
+-rw-r--r--   0 runner    (1001) docker     (121)     1956 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/ids/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.207277 kiara-0.4.9/src/kiara/registries/jobs/
+-rw-r--r--   0 runner    (1001) docker     (121)    11381 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/jobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.207277 kiara-0.4.9/src/kiara/registries/jobs/job_store/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/jobs/job_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4501 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/jobs/job_store/filesystem_store.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.207277 kiara-0.4.9/src/kiara/registries/models/
+-rw-r--r--   0 runner    (1001) docker     (121)     2998 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.207277 kiara-0.4.9/src/kiara/registries/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)     3931 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.207277 kiara-0.4.9/src/kiara/registries/operations/
+-rw-r--r--   0 runner    (1001) docker     (121)    16106 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/operations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.207277 kiara-0.4.9/src/kiara/registries/types/
+-rw-r--r--   0 runner    (1001) docker     (121)     9553 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/registries/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.207277 kiara-0.4.9/src/kiara/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.207277 kiara-0.4.9/src/kiara/resources/database/
+-rw-r--r--   0 runner    (1001) docker     (121)     2910 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/resources/database/alembic.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.207277 kiara-0.4.9/src/kiara/resources/database/kiara/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/resources/database/kiara/README
+-rw-r--r--   0 runner    (1001) docker     (121)     2374 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/resources/database/kiara/env.py
+-rw-r--r--   0 runner    (1001) docker     (121)      541 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/resources/database/kiara/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.207277 kiara-0.4.9/src/kiara/resources/database/kiara/versions/
+-rw-r--r--   0 runner    (1001) docker     (121)     9033 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/resources/database/kiara/versions/e90a32e90839_create_the_example_database.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      391 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/resources/database/reinit.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.167274 kiara-0.4.9/src/kiara/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.207277 kiara-0.4.9/src/kiara/resources/templates/doc_gen/
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/resources/templates/doc_gen/info_listing.j2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.211277 kiara-0.4.9/src/kiara/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     7740 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22057 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/utils/class_loading.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8169 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)      825 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/utils/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3153 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2408 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/utils/db.py
+-rw-r--r--   0 runner    (1001) docker     (121)      599 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/utils/doc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/utils/global_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/utils/graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.211277 kiara-0.4.9/src/kiara/utils/hashfs/
+-rw-r--r--   0 runner    (1001) docker     (121)    16435 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/utils/hashfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1615 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/utils/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/utils/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/utils/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3868 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1838 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/utils/operations.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26338 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/utils/output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4634 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/utils/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4280 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/utils/string_vars.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3998 2022-05-23 11:50:46.000000 kiara-0.4.9/src/kiara/utils/values.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.187275 kiara-0.4.9/src/kiara.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4077 2022-05-23 11:51:33.000000 kiara-0.4.9/src/kiara.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    11545 2022-05-23 11:51:33.000000 kiara-0.4.9/src/kiara.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-23 11:51:33.000000 kiara-0.4.9/src/kiara.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4581 2022-05-23 11:51:33.000000 kiara-0.4.9/src/kiara.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-23 11:51:26.000000 kiara-0.4.9/src/kiara.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-05-23 11:51:33.000000 kiara-0.4.9/src/kiara.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-23 11:51:33.000000 kiara-0.4.9/src/kiara.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.167274 kiara-0.4.9/src/mkdocstrings_handlers/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.211277 kiara-0.4.9/src/mkdocstrings_handlers/kiara/
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-05-23 11:50:46.000000 kiara-0.4.9/src/mkdocstrings_handlers/kiara/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.167274 kiara-0.4.9/src/mkdocstrings_handlers/kiara/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.211277 kiara-0.4.9/src/mkdocstrings_handlers/kiara/templates/material/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 11:50:46.000000 kiara-0.4.9/src/mkdocstrings_handlers/kiara/templates/material/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.211277 kiara-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3807 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.167274 kiara-0.4.9/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.211277 kiara-0.4.9/tests/resources/invalid_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/resources/invalid_pipelines/logic_4.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.215277 kiara-0.4.9/tests/resources/module_configs/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/resources/module_configs/and.json
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/resources/module_configs/and_wrapped.json
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/resources/module_configs/table_load.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.215277 kiara-0.4.9/tests/resources/pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.215277 kiara-0.4.9/tests/resources/pipelines/dummy/
+-rw-r--r--   0 runner    (1001) docker     (121)      437 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/resources/pipelines/dummy/dummy_1.json
+-rw-r--r--   0 runner    (1001) docker     (121)      506 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/resources/pipelines/dummy/dummy_1_delay.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.215277 kiara-0.4.9/tests/resources/pipelines/logic/
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/resources/pipelines/logic/logic_1.json
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/resources/pipelines/logic/logic_2.json
+-rw-r--r--   0 runner    (1001) docker     (121)      383 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/resources/pipelines/logic/logic_3.json
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/resources/pipelines/logic/logic_4.json
+-rw-r--r--   0 runner    (1001) docker     (121)      310 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/resources/pipelines/table_import.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1858 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/resources/pipelines/test_preseed_1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.215277 kiara-0.4.9/tests/test_cli/
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2289 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_cli/test_data_subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (121)      377 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_cli/test_info_subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_cli/test_metadata_subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (121)      847 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_cli/test_misc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1385 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_cli/test_module_subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (121)      978 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_cli/test_operation_subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_cli/test_pipeline_subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_cli/test_run_subcommand.py
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_kiara_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3181 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_module_instances.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_module_types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.215277 kiara-0.4.9/tests/test_modules/
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_modules/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_modules/test_simple_module_exec.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.215277 kiara-0.4.9/tests/test_operation_types/
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_operation_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_operation_types/test_extract_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_operation_types/test_persist_value.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_operation_types/test_render_value.py
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2579 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_pipeline_creation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2309 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1593 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_rendering.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 11:51:33.215277 kiara-0.4.9/tests/test_values/
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2897 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/test_values/test_values.py
+-rw-r--r--   0 runner    (1001) docker     (121)      733 2022-05-23 11:50:46.000000 kiara-0.4.9/tests/utils.py
```

### Comparing `kiara-0.4.8/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara-0.4.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/.github/ISSUE_TEMPLATE/feature_request.md` & `kiara-0.4.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/.github/workflows/build-darwin.yaml` & `kiara-0.4.9/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/.github/workflows/build-linux.yaml` & `kiara-0.4.9/.github/workflows/build-linux.yaml`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/.github/workflows/build-windows.yaml` & `kiara-0.4.9/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/.gitignore` & `kiara-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/.gitlab-ci.yml` & `kiara-0.4.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/.kiara_complete.zsh` & `kiara-0.4.9/.kiara_complete.zsh`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/.pre-commit-config.yaml` & `kiara-0.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/CHANGELOG.md` & `kiara-0.4.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/LICENSE` & `kiara-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/Makefile` & `kiara-0.4.9/Makefile`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/PKG-INFO` & `kiara-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara
-Version: 0.4.8
+Version: 0.4.9
 Summary: Data-centric workflow orchestration.
 Home-page: https://github.com/DHARPA-Project/kiara
 Author: Markus Binsteiner
 Author-email: markus@frkl.io
 License: MPL-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kiara-0.4.8/README.md` & `kiara-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/ci/conda/build-conda-packages.sh` & `kiara-0.4.9/ci/conda/build-conda-packages.sh`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/ci/conda/kiara/meta.yaml.template` & `kiara-0.4.9/ci/conda/kiara/meta.yaml.template`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/dev/dev.ipynb` & `kiara-0.4.9/dev/dev.ipynb`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/dev/script.py` & `kiara-0.4.9/dev/script.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/docs/architecture/assumptions.md` & `kiara-0.4.9/docs/architecture/assumptions.md`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/docs/architecture/data/.ipynb_checkpoints/data_formats-checkpoint.ipynb` & `kiara-0.4.9/docs/architecture/data/.ipynb_checkpoints/data_formats-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/docs/architecture/data/.ipynb_checkpoints/requirements-checkpoint.ipynb` & `kiara-0.4.9/docs/architecture/data/.ipynb_checkpoints/requirements-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/docs/architecture/data/data_centric_approach.ipynb` & `kiara-0.4.9/docs/architecture/data/data_centric_approach.ipynb`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/docs/architecture/data/data_formats.ipynb` & `kiara-0.4.9/docs/architecture/data/data_formats.ipynb`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/docs/architecture/data/dev.ipynb` & `kiara-0.4.9/docs/architecture/data/dev.ipynb`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/docs/architecture/data/index.md` & `kiara-0.4.9/docs/architecture/data/index.md`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/docs/architecture/data/persistence.md` & `kiara-0.4.9/docs/architecture/data/persistence.md`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/docs/architecture/data/requirements.ipynb` & `kiara-0.4.9/docs/architecture/data/requirements.ipynb`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/docs/architecture/data/result_tree.png` & `kiara-0.4.9/docs/architecture/data/result_tree.png`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/docs/architecture/decisions.md` & `kiara-0.4.9/docs/architecture/decisions.md`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/docs/architecture/metadata.md` & `kiara-0.4.9/docs/architecture/metadata.md`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/docs/architecture/workflows/index.md` & `kiara-0.4.9/docs/architecture/workflows/index.md`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/docs/architecture/workflows/modularity/.ipynb_checkpoints/modularity-checkpoint.ipynb` & `kiara-0.4.9/docs/architecture/workflows/modularity/.ipynb_checkpoints/modularity-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/docs/architecture/workflows/modularity/.ipynb_checkpoints/modularity_2-checkpoint.ipynb` & `kiara-0.4.9/docs/architecture/workflows/modularity/.ipynb_checkpoints/modularity_2-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/docs/architecture/workflows/modularity/modularity.ipynb` & `kiara-0.4.9/docs/architecture/workflows/modularity/modularity.ipynb`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/docs/architecture/workflows/modularity/modularity_2.ipynb` & `kiara-0.4.9/docs/architecture/workflows/modularity/modularity_2.ipynb`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/docs/architecture/workflows/modularity/workflows/corpus_processing.yaml` & `kiara-0.4.9/docs/architecture/workflows/modularity/workflows/corpus_processing.yaml`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/docs/architecture/workflows/modularity/workflows/input_files_processing.yaml` & `kiara-0.4.9/docs/architecture/workflows/modularity/workflows/input_files_processing.yaml`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/docs/install.md` & `kiara-0.4.9/docs/install.md`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/examples/data/journals/JournalEdges1902.csv` & `kiara-0.4.9/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/examples/data/journals/JournalNodes1902.csv` & `kiara-0.4.9/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-1_seq-1_ocr.txt` & `kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-2_seq-1_ocr.txt` & `kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-3_seq-1_ocr.txt` & `kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-3_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-4_seq-1_ocr.txt` & `kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-04-25_ed-4_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-1_seq-1_ocr.txt` & `kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-2_seq-1_ocr.txt` & `kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-3_seq-1_ocr.txt` & `kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-3_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-4_seq-1_ocr.txt` & `kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-05_ed-4_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-1_seq-1_ocr.txt` & `kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-2_seq-1_ocr.txt` & `kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-3_seq-1_ocr.txt` & `kiara-0.4.9/examples/data/text_corpus/La_Ragione/sn84037024_1917-05-16_ed-3_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-07_ed-1_seq-1_ocr.txt` & `kiara-0.4.9/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-07_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-14_ed-1_seq-1_ocr.txt` & `kiara-0.4.9/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-14_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-14_ed-2_seq-1_ocr.txt` & `kiara-0.4.9/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-14_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-21_ed-1_seq-1_ocr.txt` & `kiara-0.4.9/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-21_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-21_ed-2_seq-1_ocr.txt` & `kiara-0.4.9/examples/data/text_corpus/La_Rassegna/sn84037025_1917-04-21_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/mkdocs.yml` & `kiara-0.4.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/scripts/documentation/gen_api_doc_pages.py` & `kiara-0.4.9/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/scripts/documentation/gen_schemas.py` & `kiara-0.4.9/scripts/documentation/gen_schemas.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/setup.cfg` & `kiara-0.4.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/setup.py` & `kiara-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/__init__.py` & `kiara-0.4.9/src/kiara/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/context/__init__.py` & `kiara-0.4.9/src/kiara/context/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/context/config.py` & `kiara-0.4.9/src/kiara/context/config.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/context/orm.py` & `kiara-0.4.9/src/kiara/context/orm.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/data_types/__init__.py` & `kiara-0.4.9/src/kiara/data_types/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/data_types/included_core_types/__init__.py` & `kiara-0.4.9/src/kiara/data_types/included_core_types/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/data_types/included_core_types/filesystem.py` & `kiara-0.4.9/src/kiara/data_types/included_core_types/filesystem.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/data_types/included_core_types/internal/__init__.py` & `kiara-0.4.9/src/kiara/data_types/included_core_types/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/data_types/included_core_types/internal/render_value.py` & `kiara-0.4.9/src/kiara/data_types/included_core_types/internal/render_value.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/data_types/included_core_types/serialization.py` & `kiara-0.4.9/src/kiara/data_types/included_core_types/serialization.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/defaults.py` & `kiara-0.4.9/src/kiara/defaults.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/doc/__init__.py` & `kiara-0.4.9/src/kiara/doc/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/doc/gen_info_pages.py` & `kiara-0.4.9/src/kiara/doc/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/doc/generate_api_doc.py` & `kiara-0.4.9/src/kiara/doc/generate_api_doc.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/doc/mkdocs_macros_cli.py` & `kiara-0.4.9/src/kiara/doc/mkdocs_macros_cli.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/doc/mkdocs_macros_kiara.py` & `kiara-0.4.9/src/kiara/doc/mkdocs_macros_kiara.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/doc/mkdocstrings/collector.py` & `kiara-0.4.9/src/kiara/doc/mkdocstrings/collector.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/doc/mkdocstrings/handler.py` & `kiara-0.4.9/src/kiara/doc/mkdocstrings/handler.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/doc/mkdocstrings/renderer.py` & `kiara-0.4.9/src/kiara/doc/mkdocstrings/renderer.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/exceptions.py` & `kiara-0.4.9/src/kiara/exceptions.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/interfaces/__init__.py` & `kiara-0.4.9/src/kiara/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/interfaces/cli/__init__.py` & `kiara-0.4.9/src/kiara/interfaces/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/interfaces/cli/context/commands.py` & `kiara-0.4.9/src/kiara/interfaces/cli/context/commands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/interfaces/cli/data/commands.py` & `kiara-0.4.9/src/kiara/interfaces/cli/data/commands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/interfaces/cli/dev/commands.py` & `kiara-0.4.9/src/kiara/interfaces/cli/dev/commands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/interfaces/cli/module/commands.py` & `kiara-0.4.9/src/kiara/interfaces/cli/module/commands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/interfaces/cli/operation/commands.py` & `kiara-0.4.9/src/kiara/interfaces/cli/operation/commands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/interfaces/cli/pipeline/commands.py` & `kiara-0.4.9/src/kiara/interfaces/cli/pipeline/commands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/interfaces/cli/run.py` & `kiara-0.4.9/src/kiara/interfaces/cli/run.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/interfaces/cli/type/commands.py` & `kiara-0.4.9/src/kiara/interfaces/cli/type/commands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/interfaces/python_api/__init__.py` & `kiara-0.4.9/src/kiara/interfaces/python_api/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/interfaces/python_api/batch.py` & `kiara-0.4.9/src/kiara/interfaces/python_api/batch.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/interfaces/python_api/operation.py` & `kiara-0.4.9/src/kiara/interfaces/python_api/operation.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/interfaces/python_api/utils.py` & `kiara-0.4.9/src/kiara/interfaces/python_api/utils.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/interfaces/python_api/value.py` & `kiara-0.4.9/src/kiara/interfaces/python_api/value.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/interfaces/tui/pager.py` & `kiara-0.4.9/src/kiara/interfaces/tui/pager.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/__init__.py` & `kiara-0.4.9/src/kiara/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/aliases/__init__.py` & `kiara-0.4.9/src/kiara/models/aliases/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/archives.py` & `kiara-0.4.9/src/kiara/models/archives.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/context.py` & `kiara-0.4.9/src/kiara/models/context.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/documentation.py` & `kiara-0.4.9/src/kiara/models/documentation.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/events/__init__.py` & `kiara-0.4.9/src/kiara/models/events/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/events/alias_registry.py` & `kiara-0.4.9/src/kiara/models/events/alias_registry.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/events/data_registry.py` & `kiara-0.4.9/src/kiara/models/events/data_registry.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/events/destiny_registry.py` & `kiara-0.4.9/src/kiara/models/events/destiny_registry.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/events/job_registry.py` & `kiara-0.4.9/src/kiara/models/events/job_registry.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/events/pipeline.py` & `kiara-0.4.9/src/kiara/models/events/pipeline.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/filesystem.py` & `kiara-0.4.9/src/kiara/models/filesystem.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/info.py` & `kiara-0.4.9/src/kiara/models/info.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/module/__init__.py` & `kiara-0.4.9/src/kiara/models/module/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/module/destiniy.py` & `kiara-0.4.9/src/kiara/models/module/destiniy.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/module/jobs.py` & `kiara-0.4.9/src/kiara/models/module/jobs.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/module/manifest.py` & `kiara-0.4.9/src/kiara/models/module/manifest.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/module/operation.py` & `kiara-0.4.9/src/kiara/models/module/operation.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/module/persistence.py` & `kiara-0.4.9/src/kiara/models/module/persistence.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/module/pipeline/__init__.py` & `kiara-0.4.9/src/kiara/models/module/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/module/pipeline/controller.py` & `kiara-0.4.9/src/kiara/models/module/pipeline/controller.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/module/pipeline/pipeline.py` & `kiara-0.4.9/src/kiara/models/module/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/module/pipeline/structure.py` & `kiara-0.4.9/src/kiara/models/module/pipeline/structure.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/module/pipeline/value_refs.py` & `kiara-0.4.9/src/kiara/models/module/pipeline/value_refs.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/python_class.py` & `kiara-0.4.9/src/kiara/models/python_class.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/render_value/__init__.py` & `kiara-0.4.9/src/kiara/models/render_value/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/runtime_environment/__init__.py` & `kiara-0.4.9/src/kiara/models/runtime_environment/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/runtime_environment/kiara.py` & `kiara-0.4.9/src/kiara/models/runtime_environment/kiara.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/runtime_environment/operating_system.py` & `kiara-0.4.9/src/kiara/models/runtime_environment/operating_system.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/runtime_environment/python.py` & `kiara-0.4.9/src/kiara/models/runtime_environment/python.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/values/data_type.py` & `kiara-0.4.9/src/kiara/models/values/data_type.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/values/info.py` & `kiara-0.4.9/src/kiara/models/values/info.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/values/lineage.py` & `kiara-0.4.9/src/kiara/models/values/lineage.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/values/value.py` & `kiara-0.4.9/src/kiara/models/values/value.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,16 @@
     )
     _json_cache: Optional[bytes] = PrivateAttr(default=None)
 
     def as_json(self) -> bytes:
         assert self.inline_data is not None
         if self._json_cache is None:
             self._json_cache = orjson.dumps(
-                self.inline_data, option=orjson.OPT_NON_STR_KEYS
+                self.inline_data,
+                option=orjson.OPT_NON_STR_KEYS,
             )
         return self._json_cache
 
     def get_chunks(
         self, as_files: Union[bool, str, Sequence[str]] = True, symlink_ok: bool = True
     ) -> Iterable[Union[str, BytesLike]]:
```

### Comparing `kiara-0.4.8/src/kiara/models/values/value_metadata/__init__.py` & `kiara-0.4.9/src/kiara/models/values/value_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/values/value_metadata/included_metadata_types/__init__.py` & `kiara-0.4.9/src/kiara/models/values/value_metadata/included_metadata_types/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/models/values/value_schema.py` & `kiara-0.4.9/src/kiara/models/values/value_schema.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/modules/__init__.py` & `kiara-0.4.9/src/kiara/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/modules/included_core_modules/create_from.py` & `kiara-0.4.9/src/kiara/modules/included_core_modules/create_from.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/modules/included_core_modules/filesystem.py` & `kiara-0.4.9/src/kiara/modules/included_core_modules/filesystem.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/modules/included_core_modules/metadata.py` & `kiara-0.4.9/src/kiara/modules/included_core_modules/metadata.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/modules/included_core_modules/pipeline.py` & `kiara-0.4.9/src/kiara/modules/included_core_modules/pipeline.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/modules/included_core_modules/pretty_print.py` & `kiara-0.4.9/src/kiara/modules/included_core_modules/pretty_print.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,19 @@
         self,
     ) -> Mapping[str, Union[ValueSchema, Mapping[str, Any]]]:
 
         source_type = self.get_config_value("source_type")
         assert source_type not in ["target", "base_name"]
 
         schema = {
-            source_type: {"type": source_type, "doc": "The value to render."},
+            source_type: {
+                "type": source_type,
+                "doc": "The value to render.",
+                "optional": True,
+            },
             "render_config": {
                 "type": "any",
                 "doc": "Value type dependent render configuration.",
                 "optional": True,
             },
         }
 
@@ -141,14 +145,18 @@
 
         source_type = self.get_config_value("source_type")
         target_type = self.get_config_value("target_type")
 
         source_value = inputs.get_value_obj(source_type)
         render_config = inputs.get_value_obj("render_config")
 
+        if not source_value.is_set:
+            outputs.set_value("rendered_value", "-- none/not set --")
+            return
+
         data_type_cls = source_value.data_type_class.get_class()
         data_type = data_type_cls(**source_value.value_schema.type_config)
 
         func_name = f"pretty_print_as__{target_type}"
         func = getattr(data_type, func_name)
 
         render_config_dict = render_config.data
```

### Comparing `kiara-0.4.8/src/kiara/modules/included_core_modules/render_value.py` & `kiara-0.4.9/src/kiara/modules/included_core_modules/render_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         data_type_name = instr_model_cls.retrieve_source_type()
         assert data_type_name
 
         inputs = {
             data_type_name: {
                 "type": data_type_name,
                 "doc": f"A value of type '{data_type_name}'",
-                "optional": False,
+                "optional": True,
             },
             "render_instruction": {
                 "type": "render_instruction",
                 "doc": "Instructions/config on how (or what) to render the provided value.",
                 "optional": False,
                 "default": {"number_of_rows": 20, "row_offset": 0, "columns": None},
             },
```

### Comparing `kiara-0.4.8/src/kiara/modules/included_core_modules/serialization.py` & `kiara-0.4.9/src/kiara/modules/included_core_modules/serialization.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/operations/__init__.py` & `kiara-0.4.9/src/kiara/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/operations/included_core_operations/__init__.py` & `kiara-0.4.9/src/kiara/operations/included_core_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/operations/included_core_operations/create_from.py` & `kiara-0.4.9/src/kiara/operations/included_core_operations/create_from.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/operations/included_core_operations/metadata.py` & `kiara-0.4.9/src/kiara/operations/included_core_operations/metadata.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/operations/included_core_operations/pipeline.py` & `kiara-0.4.9/src/kiara/operations/included_core_operations/pipeline.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/operations/included_core_operations/pretty_print.py` & `kiara-0.4.9/src/kiara/operations/included_core_operations/pretty_print.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/operations/included_core_operations/render_value.py` & `kiara-0.4.9/src/kiara/operations/included_core_operations/render_value.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/operations/included_core_operations/serialize.py` & `kiara-0.4.9/src/kiara/operations/included_core_operations/serialize.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/processing/__init__.py` & `kiara-0.4.9/src/kiara/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/processing/synchronous.py` & `kiara-0.4.9/src/kiara/processing/synchronous.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/registries/__init__.py` & `kiara-0.4.9/src/kiara/registries/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/registries/aliases/__init__.py` & `kiara-0.4.9/src/kiara/registries/aliases/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/registries/aliases/archives.py` & `kiara-0.4.9/src/kiara/registries/aliases/archives.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/registries/data/__init__.py` & `kiara-0.4.9/src/kiara/registries/data/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/registries/data/data_store/__init__.py` & `kiara-0.4.9/src/kiara/registries/data/data_store/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/registries/data/data_store/filesystem_store.py` & `kiara-0.4.9/src/kiara/registries/data/data_store/filesystem_store.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/registries/destinies/__init__.py` & `kiara-0.4.9/src/kiara/registries/destinies/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/registries/destinies/filesystem_store.py` & `kiara-0.4.9/src/kiara/registries/destinies/filesystem_store.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/registries/destinies/registry.py` & `kiara-0.4.9/src/kiara/registries/destinies/registry.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/registries/environment/__init__.py` & `kiara-0.4.9/src/kiara/registries/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/registries/events/__init__.py` & `kiara-0.4.9/src/kiara/registries/events/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/registries/events/metadata.py` & `kiara-0.4.9/src/kiara/registries/events/metadata.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/registries/events/registry.py` & `kiara-0.4.9/src/kiara/registries/events/registry.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/registries/ids/__init__.py` & `kiara-0.4.9/src/kiara/registries/ids/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/registries/jobs/__init__.py` & `kiara-0.4.9/src/kiara/registries/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/registries/jobs/job_store/filesystem_store.py` & `kiara-0.4.9/src/kiara/registries/jobs/job_store/filesystem_store.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/registries/models/__init__.py` & `kiara-0.4.9/src/kiara/registries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/registries/modules/__init__.py` & `kiara-0.4.9/src/kiara/registries/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/registries/operations/__init__.py` & `kiara-0.4.9/src/kiara/registries/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/registries/types/__init__.py` & `kiara-0.4.9/src/kiara/registries/types/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/resources/database/alembic.ini` & `kiara-0.4.9/src/kiara/resources/database/alembic.ini`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/resources/database/kiara/env.py` & `kiara-0.4.9/src/kiara/resources/database/kiara/env.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/resources/database/kiara/script.py.mako` & `kiara-0.4.9/src/kiara/resources/database/kiara/script.py.mako`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/resources/database/kiara/versions/e90a32e90839_create_the_example_database.py` & `kiara-0.4.9/src/kiara/resources/database/kiara/versions/e90a32e90839_create_the_example_database.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/utils/__init__.py` & `kiara-0.4.9/src/kiara/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/utils/class_loading.py` & `kiara-0.4.9/src/kiara/utils/class_loading.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/utils/cli.py` & `kiara-0.4.9/src/kiara/utils/cli.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/utils/concurrency.py` & `kiara-0.4.9/src/kiara/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/utils/data.py` & `kiara-0.4.9/src/kiara/utils/data.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/utils/db.py` & `kiara-0.4.9/src/kiara/utils/db.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/utils/doc.py` & `kiara-0.4.9/src/kiara/utils/doc.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/utils/global_metadata.py` & `kiara-0.4.9/src/kiara/utils/global_metadata.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/utils/graphs.py` & `kiara-0.4.9/src/kiara/utils/graphs.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/utils/hashfs/__init__.py` & `kiara-0.4.9/src/kiara/utils/hashfs/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/utils/hashing.py` & `kiara-0.4.9/src/kiara/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/utils/jupyter.py` & `kiara-0.4.9/src/kiara/utils/jupyter.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/utils/metadata.py` & `kiara-0.4.9/src/kiara/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/utils/models.py` & `kiara-0.4.9/src/kiara/utils/models.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/utils/operations.py` & `kiara-0.4.9/src/kiara/utils/operations.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/utils/output.py` & `kiara-0.4.9/src/kiara/utils/output.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/utils/pipelines.py` & `kiara-0.4.9/src/kiara/utils/pipelines.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/utils/string_vars.py` & `kiara-0.4.9/src/kiara/utils/string_vars.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara/utils/values.py` & `kiara-0.4.9/src/kiara/utils/values.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara.egg-info/PKG-INFO` & `kiara-0.4.9/src/kiara.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara
-Version: 0.4.8
+Version: 0.4.9
 Summary: Data-centric workflow orchestration.
 Home-page: https://github.com/DHARPA-Project/kiara
 Author: Markus Binsteiner
 Author-email: markus@frkl.io
 License: MPL-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kiara-0.4.8/src/kiara.egg-info/SOURCES.txt` & `kiara-0.4.9/src/kiara.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara.egg-info/entry_points.txt` & `kiara-0.4.9/src/kiara.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/src/kiara.egg-info/requires.txt` & `kiara-0.4.9/src/kiara.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -40,46 +40,46 @@
 [:python_version <= "3.8"]
 importlib-metadata>=3.0.0.0
 
 [all]
 click>=7.0.0
 
 [all_dev]
-mkdocs-material>=8.0.0
-pip-licenses>=3.3.0
-types-Deprecated
-types-pkg-resources
-mkdocs-section-index>0.3.0
-types-PyYAML
-mkdocs-awesome-pages-plugin>=2.5.0
-coveralls>=3.2.0
-mkdocstrings-python-legacy
-tox>=3.21.2
-click>=7.0.0
 wheel
+flake8>=3.8.4
+mkdocs-awesome-pages-plugin>=2.5.0
+pre-commit>=2.9.3
+watchgod>=0.6
+jsonschema>=4.0.0
+pip-licenses>=3.3.0
+black
+mike>=1.0.1
+mkdocs-material>=8.0.0
+icecream>=2.1.0
+types-python-slugify
 ipython
+tox>=3.21.2
+pytest-html>=3.1.0
+types-pkg-resources
 mknotebooks>=0.7.0
-mkdocs-macros-plugin<0.6.0,>=0.5.0
 setup-cfg-fmt>=1.16.0
+mkdocs-macros-plugin<0.6.0,>=0.5.0
+mkdocstrings-python-legacy
+types-Deprecated
+click>=7.0.0
+pytest>=6.2.2
 sqlalchemy-stubs
 types-python-dateutil
-mypy>=0.800
-pytest-html>=3.1.0
 jupyter
-mike>=1.0.1
-black
+mypy>=0.800
+coveralls>=3.2.0
 types-tzlocal
-flake8>=3.8.4
-types-python-slugify
-pre-commit>=2.9.3
-watchgod>=0.6
-icecream>=2.1.0
-pytest>=6.2.2
 mkdocs-literate-nav>=0.4.0
-jsonschema>=4.0.0
+types-PyYAML
+mkdocs-section-index>0.3.0
 pytest-cov>=2.11.1
 
 [all_dev:python_version >= "3.7"]
 mkdocs-gen-files>=0.3.1
 
 [cli]
 click>=7.0.0
```

### Comparing `kiara-0.4.8/tests/conftest.py` & `kiara-0.4.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/resources/pipelines/test_preseed_1.yaml` & `kiara-0.4.9/tests/resources/pipelines/test_preseed_1.yaml`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/test_cli/test_data_subcommands.py` & `kiara-0.4.9/tests/test_cli/test_data_subcommands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/test_cli/test_metadata_subcommands.py` & `kiara-0.4.9/tests/test_cli/test_metadata_subcommands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/test_cli/test_misc_commands.py` & `kiara-0.4.9/tests/test_cli/test_misc_commands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/test_cli/test_module_subcommands.py` & `kiara-0.4.9/tests/test_cli/test_module_subcommands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/test_cli/test_operation_subcommands.py` & `kiara-0.4.9/tests/test_cli/test_operation_subcommands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/test_cli/test_pipeline_subcommands.py` & `kiara-0.4.9/tests/test_cli/test_pipeline_subcommands.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/test_cli/test_run_subcommand.py` & `kiara-0.4.9/tests/test_cli/test_run_subcommand.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/test_kiara_context.py` & `kiara-0.4.9/tests/test_kiara_context.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/test_module_instances.py` & `kiara-0.4.9/tests/test_module_instances.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/test_module_types.py` & `kiara-0.4.9/tests/test_module_types.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/test_modules/test_operations.py` & `kiara-0.4.9/tests/test_modules/test_operations.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/test_modules/test_simple_module_exec.py` & `kiara-0.4.9/tests/test_modules/test_simple_module_exec.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/test_operation_types/test_extract_metadata.py` & `kiara-0.4.9/tests/test_operation_types/test_extract_metadata.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/test_operation_types/test_persist_value.py` & `kiara-0.4.9/tests/test_operation_types/test_persist_value.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/test_operation_types/test_render_value.py` & `kiara-0.4.9/tests/test_operation_types/test_render_value.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/test_operations.py` & `kiara-0.4.9/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/test_pipeline_creation.py` & `kiara-0.4.9/tests/test_pipeline_creation.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/test_pipelines.py` & `kiara-0.4.9/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/test_rendering.py` & `kiara-0.4.9/tests/test_rendering.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/test_values/test_values.py` & `kiara-0.4.9/tests/test_values/test_values.py`

 * *Files identical despite different names*

### Comparing `kiara-0.4.8/tests/utils.py` & `kiara-0.4.9/tests/utils.py`

 * *Files identical despite different names*

