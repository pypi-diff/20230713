# Comparing `tmp/covigator-2.2.0.tar.gz` & `tmp/covigator-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covigator-2.2.0.tar", last modified: Thu Jul  6 08:20:31 2023, max compression
+gzip compressed data, was "covigator-2.2.1.tar", last modified: Thu Jul 13 11:34:42 2023, max compression
```

## Comparing `covigator-2.2.0.tar` & `covigator-2.2.1.tar`

### file list

```diff
@@ -1,166 +1,208 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.661650 covigator-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1066 2023-07-06 08:20:19.000000 covigator-2.2.0/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (122)      338 2023-07-06 08:20:19.000000 covigator-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6059 2023-07-06 08:20:31.661650 covigator-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5473 2023-07-06 08:20:19.000000 covigator-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.641650 covigator-2.2.0/covigator/
--rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.641650 covigator-2.2.0/covigator/accessor/
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/accessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1803 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/accessor/abstract_accessor.py
--rw-r--r--   0 runner    (1001) docker     (122)    17131 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/accessor/covid19_portal_accessor.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    10084 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/accessor/ena_accessor.py
--rw-r--r--   0 runner    (1001) docker     (122)     6726 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/command_line.py
--rw-r--r--   0 runner    (1001) docker     (122)     8414 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.641650 covigator-2.2.0/covigator/dashboard/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.645650 covigator-2.2.0/covigator/dashboard/assets/
--rw-r--r--   0 runner    (1001) docker     (122)    19683 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/2021_twitter_logo_blue.png
--rw-r--r--   0 runner    (1001) docker     (122)    40495 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CV19DP_logo_oneliner2.svg
--rw-r--r--   0 runner    (1001) docker     (122)    31369 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CoVigator_ico.png
--rw-r--r--   0 runner    (1001) docker     (122)   106477 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo.png
--rw-r--r--   0 runner    (1001) docker     (122)  1013129 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_ENA.png
--rw-r--r--   0 runner    (1001) docker     (122)    43957 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt.png
--rw-r--r--   0 runner    (1001) docker     (122)    46264 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_nobg.png
--rw-r--r--   0 runner    (1001) docker     (122)    47880 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_reg.png
--rw-r--r--   0 runner    (1001) docker     (122)    55075 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg.png
--rw-r--r--   0 runner    (1001) docker     (122)    75513 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_covid19_portal.png
--rw-r--r--   0 runner    (1001) docker     (122)   189872 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_covid19_portal.xcf
--rw-r--r--   0 runner    (1001) docker     (122)   165548 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_ena.xcf
--rw-r--r--   0 runner    (1001) docker     (122)    49347 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/ENA_logo_2021.png
--rw-r--r--   0 runner    (1001) docker     (122)    40828 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/ENA_logo_2021_wo_text.png
--rw-r--r--   0 runner    (1001) docker     (122)    31369 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)    23354 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/favicon___.ico
--rw-r--r--   0 runner    (1001) docker     (122)      326 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/resizing_script.js
--rw-r--r--   0 runner    (1001) docker     (122)    13254 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/s1.css
--rw-r--r--   0 runner    (1001) docker     (122)     1928 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/styles.css
--rwxr-xr-x   0 runner    (1001) docker     (122)    12110 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/tron_logo.png
--rw-r--r--   0 runner    (1001) docker     (122)    14215 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/tron_logo_no_bg.png
--rwxr-xr-x   0 runner    (1001) docker     (122)    61168 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/tron_logo_without_text.png
--rw-r--r--   0 runner    (1001) docker     (122)   344224 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/wordcloud.png
--rw-r--r--   0 runner    (1001) docker     (122)    17319 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.645650 covigator-2.2.0/covigator/dashboard/figures/
--rw-r--r--   0 runner    (1001) docker     (122)      278 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/figures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/figures/figures.py
--rw-r--r--   0 runner    (1001) docker     (122)    16413 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/figures/intrahost_mutations.py
--rw-r--r--   0 runner    (1001) docker     (122)    10781 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/figures/lineages.py
--rw-r--r--   0 runner    (1001) docker     (122)     7227 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/figures/mutation_stats.py
--rw-r--r--   0 runner    (1001) docker     (122)    42807 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/figures/recurrent_mutations.py
--rw-r--r--   0 runner    (1001) docker     (122)     4599 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/figures/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.649650 covigator-2.2.0/covigator/dashboard/tabs/
--rw-r--r--   0 runner    (1001) docker     (122)      551 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6156 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/acknowledgements.py
--rw-r--r--   0 runner    (1001) docker     (122)     7286 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/dataset_covid19_portal.py
--rw-r--r--   0 runner    (1001) docker     (122)    13437 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/dataset_ena.py
--rw-r--r--   0 runner    (1001) docker     (122)     3202 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/download.py
--rw-r--r--   0 runner    (1001) docker     (122)     3036 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/footer.py
--rw-r--r--   0 runner    (1001) docker     (122)    11070 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/intrahost_mutations.py
--rw-r--r--   0 runner    (1001) docker     (122)    10590 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/lineages.py
--rw-r--r--   0 runner    (1001) docker     (122)     6746 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/mutation_stats.py
--rw-r--r--   0 runner    (1001) docker     (122)     8570 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/overview.py
--rw-r--r--   0 runner    (1001) docker     (122)    15016 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/recurrent_mutations.py
--rw-r--r--   0 runner    (1001) docker     (122)     7496 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.649650 covigator-2.2.0/covigator/database/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4035 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/database/database.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    44182 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/database/model.py
--rw-r--r--   0 runner    (1001) docker     (122)    42544 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/database/queries.py
--rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.649650 covigator-2.2.0/covigator/misc/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2175 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/misc/backoff_retrier.py
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/misc/compression.py
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/misc/country_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.649650 covigator-2.2.0/covigator/pipeline/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3712 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/pipeline/covid19_portal_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (122)     2703 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/pipeline/downloader.py
--rw-r--r--   0 runner    (1001) docker     (122)     6261 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/pipeline/ena_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (122)      883 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/pipeline/runner.py
--rw-r--r--   0 runner    (1001) docker     (122)    13976 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/pipeline/vcf_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.649650 covigator-2.2.0/covigator/precomputations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/precomputations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5594 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/precomputations/load_cooccurrences.py
--rw-r--r--   0 runner    (1001) docker     (122)     5632 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/precomputations/load_ns_s_counts.py
--rw-r--r--   0 runner    (1001) docker     (122)     5544 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/precomputations/load_top_occurrences.py
--rw-r--r--   0 runner    (1001) docker     (122)     3453 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/precomputations/load_variants_per_lineage.py
--rw-r--r--   0 runner    (1001) docker     (122)    17548 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/precomputations/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.649650 covigator-2.2.0/covigator/processor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10544 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/processor/abstract_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)     3081 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/processor/covid19portal_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/processor/ena_downloader.py
--rw-r--r--   0 runner    (1001) docker     (122)     5762 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/processor/ena_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.653650 covigator-2.2.0/covigator/references/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/references/conservation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2965 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/references/domains_NS_S.csv
--rw-r--r--   0 runner    (1001) docker     (122)     3699 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/references/gene_annotations.py
--rw-r--r--   0 runner    (1001) docker     (122)      577 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/references/genes_NS_S.csv
--rw-r--r--   0 runner    (1001) docker     (122)    37762 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/references/lineage_annotation.py
--rw-r--r--   0 runner    (1001) docker     (122)   601324 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/references/sars_cov_2.json
--rw-r--r--   0 runner    (1001) docker     (122)   934358 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/references/wuhCor1.mutDepletionConsHMM.bed
--rw-r--r--   0 runner    (1001) docker     (122)   932961 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/references/wuhCor1.mutDepletionSarbecovirusConsHMM.bed
--rw-r--r--   0 runner    (1001) docker     (122)   931439 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/references/wuhCor1.mutDepletionVertebrateCoVConsHMM.bed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.653650 covigator-2.2.0/covigator/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.657650 covigator-2.2.0/covigator/tests/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/integration_tests/integration_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/integration_tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/integration_tests/test_gene_annotations.py
--rw-r--r--   0 runner    (1001) docker     (122)      827 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/integration_tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (122)      773 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/integration_tests/test_vcf_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.661650 covigator-2.2.0/covigator/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (122)    30427 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/MN908947.3.fa
--rw-r--r--   0 runner    (1001) docker     (122)    18016 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/Sars_cov_2.ASM985889v3.pep.all.fa
--rw-r--r--   0 runner    (1001) docker     (122)  1231182 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/Sars_cov_2.all_variants.snpeff.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/Sars_cov_2.all_variants.snpeff.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (122)     4422 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/domains_NS_S.csv
--rw-r--r--   0 runner    (1001) docker     (122)      577 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/genes_NS_S.csv
--rw-r--r--   0 runner    (1001) docker     (122)    13972 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/gisaid_allprot0526.fasta
--rw-r--r--   0 runner    (1001) docker     (122)    27733 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/gisaid_allprot1208.fasta
--rw-r--r--   0 runner    (1001) docker     (122)    27784 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/gisaid_allprot1208.with_mutations.fasta
--rw-r--r--   0 runner    (1001) docker     (122)   601324 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/sars_cov_2.json
--rw-r--r--   0 runner    (1001) docker     (122)      765 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/sars_cov_2_dn_ds.json
--rw-r--r--   0 runner    (1001) docker     (122)     7041 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/snpeff.vcf
--rw-r--r--   0 runner    (1001) docker     (122)     4041 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/snpeff_with_deletion.vcf
--rw-r--r--   0 runner    (1001) docker     (122)     4041 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/snpeff_with_insertion.vcf
--rw-r--r--   0 runner    (1001) docker     (122)     3877 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/snpeff_without_annotation.vcf
--rw-r--r--   0 runner    (1001) docker     (122)     4023 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/snpeff_without_dp4.vcf
--rw-r--r--   0 runner    (1001) docker     (122)      910 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/test.another_pangolin.csv
--rw-r--r--   0 runner    (1001) docker     (122)     2148 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/test.assembly.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/test.assembly.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/test.coverage.tsv
--rw-r--r--   0 runner    (1001) docker     (122)     3483 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/test.deduplication_metrics.txt
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/test.lofreq.pangolin.csv
--rw-r--r--   0 runner    (1001) docker     (122)      398 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/test.lofreq.pangolin.with_none.csv
--rw-r--r--   0 runner    (1001) docker     (122)     3357 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/test.lofreq.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/test.lofreq.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (122)    30247 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/test_data.fasta
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.661650 covigator-2.2.0/covigator/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/abstract_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3928 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/faked_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)     9533 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/mocked.py
--rw-r--r--   0 runner    (1001) docker     (122)      413 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_country_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     8228 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_database_initialisation.py
--rw-r--r--   0 runner    (1001) docker     (122)     3117 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (122)    27682 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_ena_accessor.py
--rw-r--r--   0 runner    (1001) docker     (122)     7491 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_figures.py
--rw-r--r--   0 runner    (1001) docker     (122)    10320 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_lineage_annotation.py
--rw-r--r--   0 runner    (1001) docker     (122)    10466 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_precomputer.py
--rw-r--r--   0 runner    (1001) docker     (122)     8107 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)    14924 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (122)    13056 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_vcf_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.641650 covigator-2.2.0/covigator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6059 2023-07-06 08:20:31.000000 covigator-2.2.0/covigator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6267 2023-07-06 08:20:31.000000 covigator-2.2.0/covigator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 08:20:31.000000 covigator-2.2.0/covigator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      524 2023-07-06 08:20:31.000000 covigator-2.2.0/covigator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      480 2023-07-06 08:20:31.000000 covigator-2.2.0/covigator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-06 08:20:31.000000 covigator-2.2.0/covigator.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)       79 2023-07-06 08:20:31.661650 covigator-2.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1862 2023-07-06 08:20:19.000000 covigator-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.565139 covigator-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1066 2023-07-13 11:34:24.000000 covigator-2.2.1/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (122)      338 2023-07-13 11:34:24.000000 covigator-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6059 2023-07-13 11:34:42.565139 covigator-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5473 2023-07-13 11:34:24.000000 covigator-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.533139 covigator-2.2.1/covigator/
+-rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.537139 covigator-2.2.1/covigator/accessor/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/accessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1803 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/accessor/abstract_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17131 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/accessor/covid19_portal_accessor.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10084 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/accessor/ena_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6726 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8414 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.537139 covigator-2.2.1/covigator/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.541139 covigator-2.2.1/covigator/dashboard/assets/
+-rw-r--r--   0 runner    (1001) docker     (122)    19683 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/2021_twitter_logo_blue.png
+-rw-r--r--   0 runner    (1001) docker     (122)    40495 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/CV19DP_logo_oneliner2.svg
+-rw-r--r--   0 runner    (1001) docker     (122)    31369 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/CoVigator_ico.png
+-rw-r--r--   0 runner    (1001) docker     (122)   106477 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/CoVigator_logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)  1013129 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/CoVigator_logo_ENA.png
+-rw-r--r--   0 runner    (1001) docker     (122)    43957 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/CoVigator_logo_txt.png
+-rw-r--r--   0 runner    (1001) docker     (122)    46264 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/CoVigator_logo_txt_nobg.png
+-rw-r--r--   0 runner    (1001) docker     (122)    47880 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/CoVigator_logo_txt_reg.png
+-rw-r--r--   0 runner    (1001) docker     (122)    55075 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg.png
+-rw-r--r--   0 runner    (1001) docker     (122)    75513 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_covid19_portal.png
+-rw-r--r--   0 runner    (1001) docker     (122)   189872 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_covid19_portal.xcf
+-rw-r--r--   0 runner    (1001) docker     (122)   165548 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_ena.xcf
+-rw-r--r--   0 runner    (1001) docker     (122)    49347 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/ENA_logo_2021.png
+-rw-r--r--   0 runner    (1001) docker     (122)    40828 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/ENA_logo_2021_wo_text.png
+-rw-r--r--   0 runner    (1001) docker     (122)    31369 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)    23354 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/favicon___.ico
+-rw-r--r--   0 runner    (1001) docker     (122)      326 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/resizing_script.js
+-rw-r--r--   0 runner    (1001) docker     (122)    13254 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/s1.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1928 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/styles.css
+-rwxr-xr-x   0 runner    (1001) docker     (122)    12110 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/tron_logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)    14215 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/tron_logo_no_bg.png
+-rwxr-xr-x   0 runner    (1001) docker     (122)    61168 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/tron_logo_without_text.png
+-rw-r--r--   0 runner    (1001) docker     (122)   344224 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/assets/wordcloud.png
+-rw-r--r--   0 runner    (1001) docker     (122)    17319 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.541139 covigator-2.2.1/covigator/dashboard/figures/
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/figures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/figures/figures.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16413 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/figures/intrahost_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10781 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/figures/lineages.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7227 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/figures/mutation_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42807 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/figures/recurrent_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4599 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/figures/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.545139 covigator-2.2.1/covigator/dashboard/tabs/
+-rw-r--r--   0 runner    (1001) docker     (122)      551 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6156 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/tabs/acknowledgements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7286 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/tabs/dataset_covid19_portal.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13437 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/tabs/dataset_ena.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3202 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/tabs/download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3036 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/tabs/footer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11070 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/tabs/intrahost_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10590 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/tabs/lineages.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6746 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/tabs/mutation_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8570 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/tabs/overview.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15016 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/tabs/recurrent_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7496 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/dashboard/tabs/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.545139 covigator-2.2.1/covigator/database/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4035 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/database/database.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    44182 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/database/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42544 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/database/queries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.545139 covigator-2.2.1/covigator/misc/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2175 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/misc/backoff_retrier.py
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/misc/compression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/misc/country_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.545139 covigator-2.2.1/covigator/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3712 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/pipeline/covid19_portal_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2703 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/pipeline/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6261 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/pipeline/ena_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)      883 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/pipeline/runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13976 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/pipeline/vcf_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.545139 covigator-2.2.1/covigator/precomputations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/precomputations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5594 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/precomputations/load_cooccurrences.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5632 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/precomputations/load_ns_s_counts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5544 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/precomputations/load_top_occurrences.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3453 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/precomputations/load_variants_per_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17548 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/precomputations/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.549139 covigator-2.2.1/covigator/processor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10544 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/processor/abstract_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3081 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/processor/covid19portal_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/processor/ena_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5762 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/processor/ena_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.553139 covigator-2.2.1/covigator/references/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/references/conservation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.533139 covigator-2.2.1/covigator/references/constellations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.533139 covigator-2.2.1/covigator/references/constellations/constellations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.553139 covigator-2.2.1/covigator/references/constellations/constellations/data/
+-rw-r--r--   0 runner    (1001) docker     (122)    33771 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/data/SARS-CoV-2.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.557139 covigator-2.2.1/covigator/references/constellations/constellations/definitions/
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cA.23.1+E484K.json
+-rw-r--r--   0 runner    (1001) docker     (122)      702 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cA.23.1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      555 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cAV1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cAY.4.2.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cAY.4.json
+-rw-r--r--   0 runner    (1001) docker     (122)      942 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cB.1.1.318.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cB.1.1.529.json
+-rw-r--r--   0 runner    (1001) docker     (122)      926 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cB.1.1.7+E484K.json
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cB.1.1.7.json
+-rw-r--r--   0 runner    (1001) docker     (122)      863 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cB.1.351.json
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cB.1.427.json
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cB.1.429.json
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cB.1.525.json
+-rw-r--r--   0 runner    (1001) docker     (122)      808 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cB.1.526.json
+-rw-r--r--   0 runner    (1001) docker     (122)      919 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cB.1.617.1.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cB.1.617.2+K417N.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cB.1.617.2.json
+-rw-r--r--   0 runner    (1001) docker     (122)      932 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cB.1.617.3.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1304 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cB.1.621.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cBA.1.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1353 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cBA.2.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1066 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cBA.3.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cBA.4.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1353 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cBA.5.json
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cC.37.json
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cP.1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cP.2.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cP.3.json
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cXBB-parent1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      568 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cXBB-parent2.json
+-rw-r--r--   0 runner    (1001) docker     (122)      707 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cXBB.1.16.json
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cXBB.1.5.json
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cXBB.1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      873 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cXBB.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cXE-parent1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      980 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cXE-parent2.json
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-07-13 11:34:25.000000 covigator-2.2.1/covigator/references/constellations/constellations/definitions/cXE.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2965 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/references/domains_NS_S.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     3699 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/references/gene_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      577 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/references/genes_NS_S.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    37762 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/references/lineage_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (122)   601324 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/references/sars_cov_2.json
+-rw-r--r--   0 runner    (1001) docker     (122)   934358 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/references/wuhCor1.mutDepletionConsHMM.bed
+-rw-r--r--   0 runner    (1001) docker     (122)   932961 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/references/wuhCor1.mutDepletionSarbecovirusConsHMM.bed
+-rw-r--r--   0 runner    (1001) docker     (122)   931439 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/references/wuhCor1.mutDepletionVertebrateCoVConsHMM.bed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.557139 covigator-2.2.1/covigator/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.557139 covigator-2.2.1/covigator/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/integration_tests/integration_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/integration_tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/integration_tests/test_gene_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/integration_tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/integration_tests/test_vcf_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.561139 covigator-2.2.1/covigator/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)    30427 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/MN908947.3.fa
+-rw-r--r--   0 runner    (1001) docker     (122)    18016 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/Sars_cov_2.ASM985889v3.pep.all.fa
+-rw-r--r--   0 runner    (1001) docker     (122)  1231182 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/Sars_cov_2.all_variants.snpeff.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/Sars_cov_2.all_variants.snpeff.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (122)     4422 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/domains_NS_S.csv
+-rw-r--r--   0 runner    (1001) docker     (122)      577 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/genes_NS_S.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    13972 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/gisaid_allprot0526.fasta
+-rw-r--r--   0 runner    (1001) docker     (122)    27733 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/gisaid_allprot1208.fasta
+-rw-r--r--   0 runner    (1001) docker     (122)    27784 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/gisaid_allprot1208.with_mutations.fasta
+-rw-r--r--   0 runner    (1001) docker     (122)   601324 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/sars_cov_2.json
+-rw-r--r--   0 runner    (1001) docker     (122)      765 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/sars_cov_2_dn_ds.json
+-rw-r--r--   0 runner    (1001) docker     (122)     7041 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/snpeff.vcf
+-rw-r--r--   0 runner    (1001) docker     (122)     4041 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/snpeff_with_deletion.vcf
+-rw-r--r--   0 runner    (1001) docker     (122)     4041 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/snpeff_with_insertion.vcf
+-rw-r--r--   0 runner    (1001) docker     (122)     3877 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/snpeff_without_annotation.vcf
+-rw-r--r--   0 runner    (1001) docker     (122)     4023 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/snpeff_without_dp4.vcf
+-rw-r--r--   0 runner    (1001) docker     (122)      910 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/test.another_pangolin.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     2148 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/test.assembly.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/test.assembly.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/test.coverage.tsv
+-rw-r--r--   0 runner    (1001) docker     (122)     3483 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/test.deduplication_metrics.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/test.lofreq.pangolin.csv
+-rw-r--r--   0 runner    (1001) docker     (122)      398 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/test.lofreq.pangolin.with_none.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     3357 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/test.lofreq.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/test.lofreq.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (122)    30247 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/resources/test_data.fasta
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.565139 covigator-2.2.1/covigator/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/unit_tests/abstract_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3928 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/unit_tests/faked_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9533 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/unit_tests/mocked.py
+-rw-r--r--   0 runner    (1001) docker     (122)      413 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/unit_tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/unit_tests/test_country_parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8228 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/unit_tests/test_database_initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3117 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/unit_tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27682 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/unit_tests/test_ena_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7491 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/unit_tests/test_figures.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10320 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/unit_tests/test_lineage_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10466 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/unit_tests/test_precomputer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8107 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/unit_tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14924 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/unit_tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13056 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/tests/unit_tests/test_vcf_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-13 11:34:24.000000 covigator-2.2.1/covigator/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 11:34:42.537139 covigator-2.2.1/covigator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6059 2023-07-13 11:34:42.000000 covigator-2.2.1/covigator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9182 2023-07-13 11:34:42.000000 covigator-2.2.1/covigator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-13 11:34:42.000000 covigator-2.2.1/covigator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      524 2023-07-13 11:34:42.000000 covigator-2.2.1/covigator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      480 2023-07-13 11:34:42.000000 covigator-2.2.1/covigator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-13 11:34:42.000000 covigator-2.2.1/covigator.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)       79 2023-07-13 11:34:42.565139 covigator-2.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1862 2023-07-13 11:34:24.000000 covigator-2.2.1/setup.py
```

### Comparing `covigator-2.2.0/LICENSE` & `covigator-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/PKG-INFO` & `covigator-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covigator
-Version: 2.2.0
+Version: 2.2.1
 Home-page: 
 Author: TRON - Translational Oncology at the University Medical Center of the Johannes Gutenberg University Mainz - Computational Medicine group
 Author-email: patrick.sorn@tron-mainz.de
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `covigator-2.2.0/README.md` & `covigator-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/__init__.py` & `covigator-2.2.1/covigator/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = "v2.2.0"
+VERSION = "v2.2.1"
 ANALYSIS_PIPELINE_VERSION = "v0.15.0"
 
 MISSENSE_VARIANT = "missense_variant"
 SYNONYMOUS_VARIANT = "synonymous_variant"
 INFRAME_DELETION = "inframe_deletion"
 INFRAME_INSERTION = "inframe_insertion"
 DISRUPTIVE_INFRAME_DELETION = "disruptive_inframe_deletion"
```

### Comparing `covigator-2.2.0/covigator/accessor/abstract_accessor.py` & `covigator-2.2.1/covigator/accessor/abstract_accessor.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/accessor/covid19_portal_accessor.py` & `covigator-2.2.1/covigator/accessor/covid19_portal_accessor.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/accessor/ena_accessor.py` & `covigator-2.2.1/covigator/accessor/ena_accessor.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/command_line.py` & `covigator-2.2.1/covigator/command_line.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/configuration.py` & `covigator-2.2.1/covigator/configuration.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/2021_twitter_logo_blue.png` & `covigator-2.2.1/covigator/dashboard/assets/2021_twitter_logo_blue.png`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/CV19DP_logo_oneliner2.svg` & `covigator-2.2.1/covigator/dashboard/assets/CV19DP_logo_oneliner2.svg`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/CoVigator_ico.png` & `covigator-2.2.1/covigator/dashboard/assets/CoVigator_ico.png`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo.png` & `covigator-2.2.1/covigator/dashboard/assets/CoVigator_logo.png`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_ENA.png` & `covigator-2.2.1/covigator/dashboard/assets/CoVigator_logo_ENA.png`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt.png` & `covigator-2.2.1/covigator/dashboard/assets/CoVigator_logo_txt.png`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_nobg.png` & `covigator-2.2.1/covigator/dashboard/assets/CoVigator_logo_txt_nobg.png`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_reg.png` & `covigator-2.2.1/covigator/dashboard/assets/CoVigator_logo_txt_reg.png`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg.png` & `covigator-2.2.1/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg.png`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_covid19_portal.png` & `covigator-2.2.1/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_covid19_portal.png`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_covid19_portal.xcf` & `covigator-2.2.1/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_covid19_portal.xcf`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_ena.xcf` & `covigator-2.2.1/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_ena.xcf`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/ENA_logo_2021.png` & `covigator-2.2.1/covigator/dashboard/assets/ENA_logo_2021.png`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/ENA_logo_2021_wo_text.png` & `covigator-2.2.1/covigator/dashboard/assets/ENA_logo_2021_wo_text.png`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/favicon.ico` & `covigator-2.2.1/covigator/dashboard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/favicon___.ico` & `covigator-2.2.1/covigator/dashboard/assets/favicon___.ico`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/s1.css` & `covigator-2.2.1/covigator/dashboard/assets/s1.css`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/styles.css` & `covigator-2.2.1/covigator/dashboard/assets/styles.css`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/tron_logo.png` & `covigator-2.2.1/covigator/dashboard/assets/tron_logo.png`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/tron_logo_no_bg.png` & `covigator-2.2.1/covigator/dashboard/assets/tron_logo_no_bg.png`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/tron_logo_without_text.png` & `covigator-2.2.1/covigator/dashboard/assets/tron_logo_without_text.png`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/assets/wordcloud.png` & `covigator-2.2.1/covigator/dashboard/assets/wordcloud.png`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/dashboard.py` & `covigator-2.2.1/covigator/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/figures/figures.py` & `covigator-2.2.1/covigator/dashboard/figures/figures.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/figures/intrahost_mutations.py` & `covigator-2.2.1/covigator/dashboard/figures/intrahost_mutations.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/figures/lineages.py` & `covigator-2.2.1/covigator/dashboard/figures/lineages.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/figures/mutation_stats.py` & `covigator-2.2.1/covigator/dashboard/figures/mutation_stats.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/figures/recurrent_mutations.py` & `covigator-2.2.1/covigator/dashboard/figures/recurrent_mutations.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/figures/samples.py` & `covigator-2.2.1/covigator/dashboard/figures/samples.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/tabs/__init__.py` & `covigator-2.2.1/covigator/dashboard/tabs/__init__.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/tabs/acknowledgements.py` & `covigator-2.2.1/covigator/dashboard/tabs/acknowledgements.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/tabs/dataset_covid19_portal.py` & `covigator-2.2.1/covigator/dashboard/tabs/dataset_covid19_portal.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/tabs/dataset_ena.py` & `covigator-2.2.1/covigator/dashboard/tabs/dataset_ena.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/tabs/download.py` & `covigator-2.2.1/covigator/dashboard/tabs/download.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/tabs/footer.py` & `covigator-2.2.1/covigator/dashboard/tabs/footer.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/tabs/intrahost_mutations.py` & `covigator-2.2.1/covigator/dashboard/tabs/intrahost_mutations.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/tabs/lineages.py` & `covigator-2.2.1/covigator/dashboard/tabs/lineages.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/tabs/mutation_stats.py` & `covigator-2.2.1/covigator/dashboard/tabs/mutation_stats.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/tabs/overview.py` & `covigator-2.2.1/covigator/dashboard/tabs/overview.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/tabs/recurrent_mutations.py` & `covigator-2.2.1/covigator/dashboard/tabs/recurrent_mutations.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/dashboard/tabs/samples.py` & `covigator-2.2.1/covigator/dashboard/tabs/samples.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/database/database.py` & `covigator-2.2.1/covigator/database/database.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/database/model.py` & `covigator-2.2.1/covigator/database/model.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/database/queries.py` & `covigator-2.2.1/covigator/database/queries.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/exceptions.py` & `covigator-2.2.1/covigator/exceptions.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/misc/backoff_retrier.py` & `covigator-2.2.1/covigator/misc/backoff_retrier.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/misc/country_parser.py` & `covigator-2.2.1/covigator/misc/country_parser.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/pipeline/covid19_portal_pipeline.py` & `covigator-2.2.1/covigator/pipeline/covid19_portal_pipeline.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/pipeline/downloader.py` & `covigator-2.2.1/covigator/pipeline/downloader.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/pipeline/ena_pipeline.py` & `covigator-2.2.1/covigator/pipeline/ena_pipeline.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/pipeline/runner.py` & `covigator-2.2.1/covigator/pipeline/runner.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/pipeline/vcf_loader.py` & `covigator-2.2.1/covigator/pipeline/vcf_loader.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/precomputations/load_cooccurrences.py` & `covigator-2.2.1/covigator/precomputations/load_cooccurrences.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/precomputations/load_ns_s_counts.py` & `covigator-2.2.1/covigator/precomputations/load_ns_s_counts.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/precomputations/load_top_occurrences.py` & `covigator-2.2.1/covigator/precomputations/load_top_occurrences.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/precomputations/load_variants_per_lineage.py` & `covigator-2.2.1/covigator/precomputations/load_variants_per_lineage.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/precomputations/loader.py` & `covigator-2.2.1/covigator/precomputations/loader.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/processor/abstract_processor.py` & `covigator-2.2.1/covigator/processor/abstract_processor.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/processor/covid19portal_processor.py` & `covigator-2.2.1/covigator/processor/covid19portal_processor.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/processor/ena_downloader.py` & `covigator-2.2.1/covigator/processor/ena_downloader.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/processor/ena_processor.py` & `covigator-2.2.1/covigator/processor/ena_processor.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/references/conservation.py` & `covigator-2.2.1/covigator/references/conservation.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/references/domains_NS_S.csv` & `covigator-2.2.1/covigator/references/domains_NS_S.csv`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/references/gene_annotations.py` & `covigator-2.2.1/covigator/references/gene_annotations.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/references/genes_NS_S.csv` & `covigator-2.2.1/covigator/references/genes_NS_S.csv`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/references/lineage_annotation.py` & `covigator-2.2.1/covigator/references/lineage_annotation.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/references/sars_cov_2.json` & `covigator-2.2.1/covigator/references/sars_cov_2.json`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/references/wuhCor1.mutDepletionConsHMM.bed` & `covigator-2.2.1/covigator/references/wuhCor1.mutDepletionConsHMM.bed`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/references/wuhCor1.mutDepletionSarbecovirusConsHMM.bed` & `covigator-2.2.1/covigator/references/wuhCor1.mutDepletionSarbecovirusConsHMM.bed`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/references/wuhCor1.mutDepletionVertebrateCoVConsHMM.bed` & `covigator-2.2.1/covigator/references/wuhCor1.mutDepletionVertebrateCoVConsHMM.bed`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/integration_tests/integration_tests.py` & `covigator-2.2.1/covigator/tests/integration_tests/integration_tests.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/integration_tests/test_downloader.py` & `covigator-2.2.1/covigator/tests/integration_tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/integration_tests/test_pipeline.py` & `covigator-2.2.1/covigator/tests/integration_tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/integration_tests/test_vcf_loader.py` & `covigator-2.2.1/covigator/tests/integration_tests/test_vcf_loader.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/resources/MN908947.3.fa` & `covigator-2.2.1/covigator/tests/resources/MN908947.3.fa`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/resources/Sars_cov_2.ASM985889v3.pep.all.fa` & `covigator-2.2.1/covigator/tests/resources/Sars_cov_2.ASM985889v3.pep.all.fa`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/resources/Sars_cov_2.all_variants.snpeff.vcf.gz` & `covigator-2.2.1/covigator/tests/resources/Sars_cov_2.all_variants.snpeff.vcf.gz`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/resources/domains_NS_S.csv` & `covigator-2.2.1/covigator/tests/resources/domains_NS_S.csv`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/resources/genes_NS_S.csv` & `covigator-2.2.1/covigator/tests/resources/genes_NS_S.csv`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/resources/gisaid_allprot0526.fasta` & `covigator-2.2.1/covigator/tests/resources/gisaid_allprot0526.fasta`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/resources/gisaid_allprot1208.fasta` & `covigator-2.2.1/covigator/tests/resources/gisaid_allprot1208.fasta`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/resources/gisaid_allprot1208.with_mutations.fasta` & `covigator-2.2.1/covigator/tests/resources/gisaid_allprot1208.with_mutations.fasta`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/resources/sars_cov_2.json` & `covigator-2.2.1/covigator/tests/resources/sars_cov_2.json`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/resources/sars_cov_2_dn_ds.json` & `covigator-2.2.1/covigator/tests/resources/sars_cov_2_dn_ds.json`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/resources/snpeff.vcf` & `covigator-2.2.1/covigator/tests/resources/snpeff.vcf`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/resources/snpeff_with_deletion.vcf` & `covigator-2.2.1/covigator/tests/resources/snpeff_with_deletion.vcf`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/resources/snpeff_with_insertion.vcf` & `covigator-2.2.1/covigator/tests/resources/snpeff_with_insertion.vcf`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/resources/snpeff_without_annotation.vcf` & `covigator-2.2.1/covigator/tests/resources/snpeff_without_annotation.vcf`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/resources/snpeff_without_dp4.vcf` & `covigator-2.2.1/covigator/tests/resources/snpeff_without_dp4.vcf`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/resources/test.another_pangolin.csv` & `covigator-2.2.1/covigator/tests/resources/test.another_pangolin.csv`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/resources/test.assembly.vcf.gz` & `covigator-2.2.1/covigator/tests/resources/test.assembly.vcf.gz`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/resources/test.deduplication_metrics.txt` & `covigator-2.2.1/covigator/tests/resources/test.deduplication_metrics.txt`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/resources/test.lofreq.vcf.gz` & `covigator-2.2.1/covigator/tests/resources/test.lofreq.vcf.gz`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/resources/test_data.fasta` & `covigator-2.2.1/covigator/tests/resources/test_data.fasta`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/unit_tests/abstract_test.py` & `covigator-2.2.1/covigator/tests/unit_tests/abstract_test.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/unit_tests/faked_objects.py` & `covigator-2.2.1/covigator/tests/unit_tests/faked_objects.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/unit_tests/mocked.py` & `covigator-2.2.1/covigator/tests/unit_tests/mocked.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/unit_tests/test_country_parser.py` & `covigator-2.2.1/covigator/tests/unit_tests/test_country_parser.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/unit_tests/test_database_initialisation.py` & `covigator-2.2.1/covigator/tests/unit_tests/test_database_initialisation.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/unit_tests/test_downloader.py` & `covigator-2.2.1/covigator/tests/unit_tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/unit_tests/test_ena_accessor.py` & `covigator-2.2.1/covigator/tests/unit_tests/test_ena_accessor.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/unit_tests/test_figures.py` & `covigator-2.2.1/covigator/tests/unit_tests/test_figures.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/unit_tests/test_lineage_annotation.py` & `covigator-2.2.1/covigator/tests/unit_tests/test_lineage_annotation.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/unit_tests/test_precomputer.py` & `covigator-2.2.1/covigator/tests/unit_tests/test_precomputer.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/unit_tests/test_processor.py` & `covigator-2.2.1/covigator/tests/unit_tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/unit_tests/test_queries.py` & `covigator-2.2.1/covigator/tests/unit_tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator/tests/unit_tests/test_vcf_loader.py` & `covigator-2.2.1/covigator/tests/unit_tests/test_vcf_loader.py`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/covigator.egg-info/PKG-INFO` & `covigator-2.2.1/covigator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covigator
-Version: 2.2.0
+Version: 2.2.1
 Home-page: 
 Author: TRON - Translational Oncology at the University Medical Center of the Johannes Gutenberg University Mainz - Computational Medicine group
 Author-email: patrick.sorn@tron-mainz.de
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `covigator-2.2.0/covigator.egg-info/entry_points.txt` & `covigator-2.2.1/covigator.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `covigator-2.2.0/setup.py` & `covigator-2.2.1/setup.py`

 * *Files identical despite different names*

