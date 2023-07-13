# Comparing `tmp/robust_deid-0.3.0.tar.gz` & `tmp/robust_deid-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/pk621/Desktop/projects/ehr_deidentification/dist/tmpdwmgvvvo/robust_deid-0.3.0.tar", last modified: Wed Aug 31 21:06:24 2022, max compression
+gzip compressed data, was "/Users/pk621/Desktop/projects/public/ehr_deidentification/dist/.tmp-gcqu9fpf/robust_deid-0.3.1.tar", last modified: Thu Jul 13 19:52:39 2023, max compression
```

## Comparing `robust_deid-0.3.0.tar` & `robust_deid-0.3.1.tar`

### file list

```diff
@@ -1,109 +1,111 @@
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.211500 robust_deid-0.3.0/
--rw-r--r--   0 pk621      (503) staff       (20)     1070 2022-08-29 20:52:22.000000 robust_deid-0.3.0/LICENSE
--rw-r--r--   0 pk621      (503) staff       (20)      971 2022-08-30 21:29:31.000000 robust_deid-0.3.0/MANIFEST.in
--rw-r--r--   0 pk621      (503) staff       (20)    31365 2022-08-31 21:06:24.211730 robust_deid-0.3.0/PKG-INFO
--rw-r--r--   0 pk621      (503) staff       (20)    30322 2022-08-30 21:29:31.000000 robust_deid-0.3.0/README.md
--rw-r--r--   0 pk621      (503) staff       (20)      103 2022-08-30 21:29:32.000000 robust_deid-0.3.0/pyproject.toml
--rw-r--r--   0 pk621      (503) staff       (20)     1261 2022-08-31 21:06:24.212844 robust_deid-0.3.0/setup.cfg
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.142638 robust_deid-0.3.0/src/
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.155840 robust_deid-0.3.0/src/robust_deid/
--rw-r--r--   0 pk621      (503) staff       (20)        0 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/__init__.py
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.162068 robust_deid-0.3.0/src/robust_deid/arguments/
--rw-r--r--   0 pk621      (503) staff       (20)      157 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/arguments/__init__.py
--rw-r--r--   0 pk621      (503) staff       (20)     5838 2022-08-31 18:24:51.000000 robust_deid-0.3.0/src/robust_deid/arguments/data_training_arguments.py
--rw-r--r--   0 pk621      (503) staff       (20)     2181 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/arguments/model_arguments.py
--rw-r--r--   0 pk621      (503) staff       (20)    11627 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/dataset_splitter.py
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.164653 robust_deid-0.3.0/src/robust_deid/deidentification/
--rw-r--r--   0 pk621      (503) staff       (20)      228 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/deidentification/__init__.py
--rw-r--r--   0 pk621      (503) staff       (20)      180 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/deidentification/deidentification_types.py
--rw-r--r--   0 pk621      (503) staff       (20)    13135 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/deidentification/text_deidentification.py
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.166668 robust_deid-0.3.0/src/robust_deid/metrics/
--rw-r--r--   0 pk621      (503) staff       (20)       76 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/metrics/__init__.py
--rw-r--r--   0 pk621      (503) staff       (20)     3950 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/metrics/sequence_metrics.py
--rw-r--r--   0 pk621      (503) staff       (20)     7008 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/metrics/token_evaluation.py
--rw-r--r--   0 pk621      (503) staff       (20)     6272 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/model_helpers.py
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.168709 robust_deid-0.3.0/src/robust_deid/model_outputs/
--rw-r--r--   0 pk621      (503) staff       (20)      165 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/model_outputs/__init__.py
--rw-r--r--   0 pk621      (503) staff       (20)     3151 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/model_outputs/note_aggregate.py
--rw-r--r--   0 pk621      (503) staff       (20)    16234 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/model_outputs/post_process.py
--rw-r--r--   0 pk621      (503) staff       (20)     2119 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/recall_threshold.py
--rw-r--r--   0 pk621      (503) staff       (20)    11027 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_dataset.py
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.169375 robust_deid-0.3.0/src/robust_deid/sequence_datasets/
--rw-r--r--   0 pk621      (503) staff       (20)        0 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/__init__.py
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.170914 robust_deid-0.3.0/src/robust_deid/sequence_datasets/builder/
--rw-r--r--   0 pk621      (503) staff       (20)      138 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/builder/__init__.py
--rw-r--r--   0 pk621      (503) staff       (20)     5647 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/builder/dataset_builder.py
--rw-r--r--   0 pk621      (503) staff       (20)     3567 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/builder/sequence_dataset.py
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.174756 robust_deid-0.3.0/src/robust_deid/sequence_datasets/labels/
--rw-r--r--   0 pk621      (503) staff       (20)      173 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/labels/__init__.py
--rw-r--r--   0 pk621      (503) staff       (20)      193 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/labels/align.py
--rw-r--r--   0 pk621      (503) staff       (20)     9008 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/labels/align_token_labels.py
--rw-r--r--   0 pk621      (503) staff       (20)     3013 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/labels/label_info.py
--rw-r--r--   0 pk621      (503) staff       (20)      326 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/labels/mismatch_error.py
--rw-r--r--   0 pk621      (503) staff       (20)    13570 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/labels/span_fixer.py
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.177338 robust_deid-0.3.0/src/robust_deid/sequence_datasets/sequences/
--rw-r--r--   0 pk621      (503) staff       (20)       76 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/sequences/__init__.py
--rw-r--r--   0 pk621      (503) staff       (20)    20919 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/sequences/sequence_chunker.py
--rw-r--r--   0 pk621      (503) staff       (20)     6263 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/sequences/utils.py
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.179247 robust_deid-0.3.0/src/robust_deid/sequence_datasets/setup/
--rw-r--r--   0 pk621      (503) staff       (20)        0 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/setup/__init__.py
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.181991 robust_deid-0.3.0/src/robust_deid/sequence_datasets/setup/distribution/
--rw-r--r--   0 pk621      (503) staff       (20)      203 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/setup/distribution/__init__.py
--rw-r--r--   0 pk621      (503) staff       (20)    12469 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/setup/distribution/dataset_splits.py
--rw-r--r--   0 pk621      (503) staff       (20)     2307 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/setup/distribution/ner_distribution.py
--rw-r--r--   0 pk621      (503) staff       (20)     2133 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/setup/distribution/print_distribution.py
--rw-r--r--   0 pk621      (503) staff       (20)     1652 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/setup/merge_files.py
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.185524 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_tokenizers/
--rw-r--r--   0 pk621      (503) staff       (20)      148 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_tokenizers/__init__.py
--rw-r--r--   0 pk621      (503) staff       (20)     1525 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_tokenizers/hf_subword_tokenizer.py
--rw-r--r--   0 pk621      (503) staff       (20)     2041 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_tokenizers/spacy_tokenizer.py
--rw-r--r--   0 pk621      (503) staff       (20)      335 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_tokenizers/subword_tokenizer.py
--rw-r--r--   0 pk621      (503) staff       (20)     1125 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_tokenizers/tokenizer.py
--rw-r--r--   0 pk621      (503) staff       (20)      582 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_tokenizers/utils.py
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.186650 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/
--rw-r--r--   0 pk621      (503) staff       (20)       70 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/__init__.py
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.187472 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/
--rw-r--r--   0 pk621      (503) staff       (20)        0 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/__init__.py
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.188434 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/noise/
--rw-r--r--   0 pk621      (503) staff       (20)       95 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/noise/__init__.py
--rw-r--r--   0 pk621      (503) staff       (20)     2144 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/noise/character_noise_augment.py
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.200772 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/
--rw-r--r--   0 pk621      (503) staff       (20)      805 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/__init__.py
--rw-r--r--   0 pk621      (503) staff       (20)     6177 2022-08-31 18:25:30.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/age_augment.py
--rw-r--r--   0 pk621      (503) staff       (20)      119 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/augment_type.py
--rw-r--r--   0 pk621      (503) staff       (20)    16590 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/augmenter.py
--rw-r--r--   0 pk621      (503) staff       (20)     3166 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/date_augment.py
--rw-r--r--   0 pk621      (503) staff       (20)    20197 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/date_patterns.py
--rw-r--r--   0 pk621      (503) staff       (20)     1081 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/email_augment.py
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.208914 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/hospital/
--rw-r--r--   0 pk621      (503) staff       (20)     2547 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/hospital/acronyms.json
--rw-r--r--   0 pk621      (503) staff       (20)      953 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/hospital/assisted_living.json
--rw-r--r--   0 pk621      (503) staff       (20)    18979 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/hospital/hospitals.json
--rw-r--r--   0 pk621      (503) staff       (20)   190174 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/hospital/hospitals_full.json
--rw-r--r--   0 pk621      (503) staff       (20)     1694 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/hospital/ids.json
--rw-r--r--   0 pk621      (503) staff       (20)      613 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/hospital/location_ids.json
--rw-r--r--   0 pk621      (503) staff       (20)     1111 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/hospital/locations.json
--rw-r--r--   0 pk621      (503) staff       (20)      767 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/hospital/pharmacies.json
--rw-r--r--   0 pk621      (503) staff       (20)    11918 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/hospital_augment.py
--rw-r--r--   0 pk621      (503) staff       (20)     4545 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/id_augment.py
--rw-r--r--   0 pk621      (503) staff       (20)    23590 2022-08-31 20:48:49.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/location_augment.py
--rw-r--r--   0 pk621      (503) staff       (20)     8378 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/name_augment.py
--rw-r--r--   0 pk621      (503) staff       (20)     4553 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/other_phi_augment.py
--rw-r--r--   0 pk621      (503) staff       (20)      137 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/patient_augment.py
--rw-r--r--   0 pk621      (503) staff       (20)    36836 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/patorg.txt
--rw-r--r--   0 pk621      (503) staff       (20)     1864 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/patorg_augment.py
--rw-r--r--   0 pk621      (503) staff       (20)     4139 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/phone_augment.py
--rw-r--r--   0 pk621      (503) staff       (20)     4696 2022-08-31 20:57:21.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/staff_augment.py
--rw-r--r--   0 pk621      (503) staff       (20)     2563 2022-08-31 20:40:06.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/augmentations/phi/utils.py
--rw-r--r--   0 pk621      (503) staff       (20)    16660 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_datasets/text_transformations/text_transform.py
--rw-r--r--   0 pk621      (503) staff       (20)    35108 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/sequence_tagger.py
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.210651 robust_deid-0.3.0/src/robust_deid/training/
--rw-r--r--   0 pk621      (503) staff       (20)       54 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/training/__init__.py
--rw-r--r--   0 pk621      (503) staff       (20)     3405 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/training/training.py
--rw-r--r--   0 pk621      (503) staff       (20)     7309 2022-08-30 21:29:32.000000 robust_deid-0.3.0/src/robust_deid/utils.py
-drwxr-xr-x   0 pk621      (503) staff       (20)        0 2022-08-31 21:06:24.159590 robust_deid-0.3.0/src/robust_deid.egg-info/
--rw-r--r--   0 pk621      (503) staff       (20)    31365 2022-08-31 21:06:24.000000 robust_deid-0.3.0/src/robust_deid.egg-info/PKG-INFO
--rw-r--r--   0 pk621      (503) staff       (20)     5425 2022-08-31 21:06:24.000000 robust_deid-0.3.0/src/robust_deid.egg-info/SOURCES.txt
--rw-r--r--   0 pk621      (503) staff       (20)        1 2022-08-31 21:06:24.000000 robust_deid-0.3.0/src/robust_deid.egg-info/dependency_links.txt
--rw-r--r--   0 pk621      (503) staff       (20)        1 2022-08-30 18:23:18.000000 robust_deid-0.3.0/src/robust_deid.egg-info/not-zip-safe
--rw-r--r--   0 pk621      (503) staff       (20)       12 2022-08-31 21:06:24.000000 robust_deid-0.3.0/src/robust_deid.egg-info/top_level.txt
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.249020 robust_deid-0.3.1/
+-rw-r--r--   0 pk621      (503) staff       (20)     1070 2023-07-13 15:15:12.000000 robust_deid-0.3.1/LICENSE
+-rw-r--r--   0 pk621      (503) staff       (20)      132 2023-07-13 15:15:12.000000 robust_deid-0.3.1/MANIFEST.in
+-rw-r--r--   0 pk621      (503) staff       (20)    10972 2023-07-13 19:52:39.249260 robust_deid-0.3.1/PKG-INFO
+-rw-r--r--   0 pk621      (503) staff       (20)    10091 2023-07-13 15:15:12.000000 robust_deid-0.3.1/README.md
+-rw-r--r--   0 pk621      (503) staff       (20)      103 2023-07-13 15:15:12.000000 robust_deid-0.3.1/pyproject.toml
+-rw-r--r--   0 pk621      (503) staff       (20)     1637 2023-07-13 19:52:39.250515 robust_deid-0.3.1/setup.cfg
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.161947 robust_deid-0.3.1/src/
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.173267 robust_deid-0.3.1/src/robust_deid/
+-rw-r--r--   0 pk621      (503) staff       (20)      363 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/__init__.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.180602 robust_deid-0.3.1/src/robust_deid/data_processing/
+-rw-r--r--   0 pk621      (503) staff       (20)       61 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/data_processing/__init__.py
+-rw-r--r--   0 pk621      (503) staff       (20)     7272 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/data_processing/data_loader.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.183779 robust_deid-0.3.1/src/robust_deid/deid/
+-rw-r--r--   0 pk621      (503) staff       (20)       55 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/deid/__init__.py
+-rw-r--r--   0 pk621      (503) staff       (20)    12268 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/deid/text_deid.py
+-rw-r--r--   0 pk621      (503) staff       (20)     1166 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/deid/utils.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.188759 robust_deid-0.3.1/src/robust_deid/ner_datasets/
+-rw-r--r--   0 pk621      (503) staff       (20)      247 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/__init__.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.191364 robust_deid-0.3.1/src/robust_deid/ner_datasets/dataset_builder/
+-rw-r--r--   0 pk621      (503) staff       (20)      116 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/dataset_builder/__init__.py
+-rw-r--r--   0 pk621      (503) staff       (20)     6725 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/dataset_builder/dataset.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.195041 robust_deid-0.3.1/src/robust_deid/ner_datasets/dataset_builder/labels/
+-rw-r--r--   0 pk621      (503) staff       (20)      215 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/dataset_builder/labels/__init__.py
+-rw-r--r--   0 pk621      (503) staff       (20)      326 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/dataset_builder/labels/mismatch_error.py
+-rw-r--r--   0 pk621      (503) staff       (20)     1072 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/dataset_builder/labels/ner_predict_token_labels.py
+-rw-r--r--   0 pk621      (503) staff       (20)     7807 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/dataset_builder/labels/ner_token_labels.py
+-rw-r--r--   0 pk621      (503) staff       (20)    24484 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/dataset_builder/sentence_dataset.py
+-rw-r--r--   0 pk621      (503) staff       (20)    14441 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/dataset_creator.py
+-rw-r--r--   0 pk621      (503) staff       (20)    11387 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/dataset_splitter.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.199063 robust_deid-0.3.1/src/robust_deid/ner_datasets/distribution/
+-rw-r--r--   0 pk621      (503) staff       (20)      203 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/distribution/__init__.py
+-rw-r--r--   0 pk621      (503) staff       (20)    12442 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/distribution/dataset_splits.py
+-rw-r--r--   0 pk621      (503) staff       (20)     2300 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/distribution/ner_distribution.py
+-rw-r--r--   0 pk621      (503) staff       (20)     2129 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/distribution/print_distribution.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.201753 robust_deid-0.3.1/src/robust_deid/ner_datasets/preprocessing/
+-rw-r--r--   0 pk621      (503) staff       (20)       88 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/preprocessing/__init__.py
+-rw-r--r--   0 pk621      (503) staff       (20)     2229 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/preprocessing/preprocessing_loader.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.208139 robust_deid-0.3.1/src/robust_deid/ner_datasets/preprocessing/sentencizers/
+-rw-r--r--   0 pk621      (503) staff       (20)      141 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/preprocessing/sentencizers/__init__.py
+-rw-r--r--   0 pk621      (503) staff       (20)     1112 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/preprocessing/sentencizers/note_sentencizer.py
+-rw-r--r--   0 pk621      (503) staff       (20)     1317 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/preprocessing/sentencizers/spacy_sentencizer.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.211809 robust_deid-0.3.1/src/robust_deid/ner_datasets/preprocessing/tokenizers/
+-rw-r--r--   0 pk621      (503) staff       (20)      226 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/preprocessing/tokenizers/__init__.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.214323 robust_deid-0.3.1/src/robust_deid/ner_datasets/preprocessing/tokenizers/abbreviations/
+-rw-r--r--   0 pk621      (503) staff       (20)        0 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/preprocessing/tokenizers/abbreviations/__init__.py
+-rw-r--r--   0 pk621      (503) staff       (20)     3281 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/preprocessing/tokenizers/abbreviations/medical_abbreviations.txt
+-rw-r--r--   0 pk621      (503) staff       (20)     3505 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/preprocessing/tokenizers/clinical_spacy_tokenizer.py
+-rw-r--r--   0 pk621      (503) staff       (20)     2306 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/preprocessing/tokenizers/core_nlp_tokenizer.py
+-rw-r--r--   0 pk621      (503) staff       (20)     1874 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/preprocessing/tokenizers/spacy_tokenizer.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.217684 robust_deid-0.3.1/src/robust_deid/ner_datasets/preprocessing/tokenizers/utils/
+-rw-r--r--   0 pk621      (503) staff       (20)      164 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/preprocessing/tokenizers/utils/__init__.py
+-rw-r--r--   0 pk621      (503) staff       (20)     3180 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/preprocessing/tokenizers/utils/clean_regex.py
+-rw-r--r--   0 pk621      (503) staff       (20)    14490 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/preprocessing/tokenizers/utils/clinical_regex.py
+-rw-r--r--   0 pk621      (503) staff       (20)     3672 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/preprocessing/tokenizers/utils/date_regex.py
+-rw-r--r--   0 pk621      (503) staff       (20)    18518 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/span_fixer.py
+-rw-r--r--   0 pk621      (503) staff       (20)     3278 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/ner_datasets/span_validation.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.220227 robust_deid-0.3.1/src/robust_deid/sequence_tagging/
+-rw-r--r--   0 pk621      (503) staff       (20)      144 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/__init__.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.223888 robust_deid-0.3.1/src/robust_deid/sequence_tagging/arguments/
+-rw-r--r--   0 pk621      (503) staff       (20)      249 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/arguments/__init__.py
+-rw-r--r--   0 pk621      (503) staff       (20)     4188 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/arguments/data_training_arguments.py
+-rw-r--r--   0 pk621      (503) staff       (20)     1036 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/arguments/evaluation_arguments.py
+-rw-r--r--   0 pk621      (503) staff       (20)     1550 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/arguments/model_arguments.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.227822 robust_deid-0.3.1/src/robust_deid/sequence_tagging/dataset_builder/
+-rw-r--r--   0 pk621      (503) staff       (20)      226 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/dataset_builder/__init__.py
+-rw-r--r--   0 pk621      (503) staff       (20)    10148 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/dataset_builder/dataset_tokenizer.py
+-rw-r--r--   0 pk621      (503) staff       (20)     4155 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/dataset_builder/label_mapper.py
+-rw-r--r--   0 pk621      (503) staff       (20)     3777 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/dataset_builder/ner_dataset.py
+-rw-r--r--   0 pk621      (503) staff       (20)     2937 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/dataset_builder/ner_labels.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.229266 robust_deid-0.3.1/src/robust_deid/sequence_tagging/evaluation/
+-rw-r--r--   0 pk621      (503) staff       (20)       43 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/evaluation/__init__.py
+-rw-r--r--   0 pk621      (503) staff       (20)    11907 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/evaluation/metrics_compute.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.234898 robust_deid-0.3.1/src/robust_deid/sequence_tagging/evaluation/note_evaluation/
+-rw-r--r--   0 pk621      (503) staff       (20)        0 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/evaluation/note_evaluation/__init__.py
+-rw-r--r--   0 pk621      (503) staff       (20)    10658 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/evaluation/note_evaluation/note_evaluation.py
+-rw-r--r--   0 pk621      (503) staff       (20)    25633 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/evaluation/note_evaluation/note_sequence_evaluation.py
+-rw-r--r--   0 pk621      (503) staff       (20)     6684 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/evaluation/note_evaluation/note_token_evaluation.py
+-rw-r--r--   0 pk621      (503) staff       (20)     4537 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/evaluation/note_evaluation/violations.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.236544 robust_deid-0.3.1/src/robust_deid/sequence_tagging/evaluation/results/
+-rw-r--r--   0 pk621      (503) staff       (20)       76 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/evaluation/results/__init__.py
+-rw-r--r--   0 pk621      (503) staff       (20)     2626 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/evaluation/results/results_formatter.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.237357 robust_deid-0.3.1/src/robust_deid/sequence_tagging/models/
+-rw-r--r--   0 pk621      (503) staff       (20)        0 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/models/__init__.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.238645 robust_deid-0.3.1/src/robust_deid/sequence_tagging/models/hf/
+-rw-r--r--   0 pk621      (503) staff       (20)       61 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/models/hf/__init__.py
+-rw-r--r--   0 pk621      (503) staff       (20)     2195 2023-07-13 19:24:48.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/models/hf/model_picker.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.240517 robust_deid-0.3.1/src/robust_deid/sequence_tagging/note_aggregate/
+-rw-r--r--   0 pk621      (503) staff       (20)       88 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/note_aggregate/__init__.py
+-rw-r--r--   0 pk621      (503) staff       (20)     8473 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/note_aggregate/note_level_aggregator.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.241715 robust_deid-0.3.1/src/robust_deid/sequence_tagging/post_process/
+-rw-r--r--   0 pk621      (503) staff       (20)        0 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/post_process/__init__.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.248429 robust_deid-0.3.1/src/robust_deid/sequence_tagging/post_process/model_outputs/
+-rw-r--r--   0 pk621      (503) staff       (20)       80 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/post_process/model_outputs/__init__.py
+-rw-r--r--   0 pk621      (503) staff       (20)     2440 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/post_process/model_outputs/argmax_process.py
+-rw-r--r--   0 pk621      (503) staff       (20)     1118 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/post_process/model_outputs/crf_argmax_process.py
+-rw-r--r--   0 pk621      (503) staff       (20)     4121 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/post_process/model_outputs/crf_process.py
+-rw-r--r--   0 pk621      (503) staff       (20)     2283 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/post_process/model_outputs/logits_process.py
+-rw-r--r--   0 pk621      (503) staff       (20)     2647 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/post_process/model_outputs/post_process_picker.py
+-rw-r--r--   0 pk621      (503) staff       (20)     2445 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/post_process/model_outputs/threshold_process_max.py
+-rw-r--r--   0 pk621      (503) staff       (20)     2360 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/post_process/model_outputs/threshold_process_sum.py
+-rw-r--r--   0 pk621      (503) staff       (20)      675 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/post_process/model_outputs/utils.py
+-rw-r--r--   0 pk621      (503) staff       (20)     5209 2023-07-13 15:15:12.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/recall_thresholder.py
+-rw-r--r--   0 pk621      (503) staff       (20)    26316 2023-07-13 19:24:48.000000 robust_deid-0.3.1/src/robust_deid/sequence_tagging/sequence_tagger.py
+drwxr-xr-x   0 pk621      (503) staff       (20)        0 2023-07-13 19:52:39.178829 robust_deid-0.3.1/src/robust_deid.egg-info/
+-rw-r--r--   0 pk621      (503) staff       (20)    10972 2023-07-13 19:52:39.000000 robust_deid-0.3.1/src/robust_deid.egg-info/PKG-INFO
+-rw-r--r--   0 pk621      (503) staff       (20)     4999 2023-07-13 19:52:39.000000 robust_deid-0.3.1/src/robust_deid.egg-info/SOURCES.txt
+-rw-r--r--   0 pk621      (503) staff       (20)        1 2023-07-13 19:52:39.000000 robust_deid-0.3.1/src/robust_deid.egg-info/dependency_links.txt
+-rw-r--r--   0 pk621      (503) staff       (20)      494 2023-07-13 19:52:39.000000 robust_deid-0.3.1/src/robust_deid.egg-info/entry_points.txt
+-rw-r--r--   0 pk621      (503) staff       (20)        1 2023-07-13 19:52:38.000000 robust_deid-0.3.1/src/robust_deid.egg-info/not-zip-safe
+-rw-r--r--   0 pk621      (503) staff       (20)       12 2023-07-13 19:52:39.000000 robust_deid-0.3.1/src/robust_deid.egg-info/top_level.txt
```

### Comparing `robust_deid-0.3.0/LICENSE` & `robust_deid-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robust_deid-0.3.0/src/robust_deid/arguments/data_training_arguments.py` & `robust_deid-0.3.1/src/robust_deid/sequence_tagging/arguments/data_training_arguments.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,107 +1,84 @@
-from dataclasses import field, dataclass
 from typing import Optional
-
+from dataclasses import dataclass, field
 
 @dataclass
 class DataTrainingArguments:
     """
     Arguments pertaining to what data we are going to input our model for training and eval.
     """
+    task_name: Optional[str] = field(
+        default="ner",
+        metadata={"help": "The name of the task (ner, pos...)."}
+    )
     notation: str = field(
         default="BIO",
         metadata={"help": "NER notation e.g BIO"},
     )
     ner_types: Optional[str] = field(
         default=None,
         metadata={"help": "Pass a list of NER types"},
     )
-    ner_priorities: Optional[str] = field(
-        default=None,
-        metadata={"help": "Pass a list of NER priorities - that indicate the importance of the ner types - needs to "
-                          "be in the same order as the ner_types list"
-                  },
-    )
-    ner_type_maps: Optional[str] = field(
-        default=None,
-        metadata={
-            "help": "List that contains the mappings between the original NER types to another set of NER types. Used "
-                    "mainly for evaluation. to map ner token labels to another set of ner token"
-        },
-    )
-    fix_spans: bool = field(
-        default=True,
-        metadata={
-            "help": "Whether to fix token span alignments. Required to align tokens and labels (token level)"
-        },
-    )
-    ner_augment: Optional[str] = field(
-        default=None,
-        metadata={
-            "help": "Whether to replace/augment NER tokens (augment data)"
-        },
-    )
-    character_noise_augment: Optional[float] = field(
-        default=None,
-        metadata={
-            "help": "Add noise by replacing a character in a token"
-        },
-    )
     train_file: Optional[str] = field(
         default=None,
-        metadata={"help": "The input training data file (a text file)."}
+        metadata={"help": "The input training data file (a csv or JSON file)."}
     )
     validation_file: Optional[str] = field(
         default=None,
-        metadata={"help": "An optional input evaluation data file to evaluate the perplexity on (a text file)."},
+        metadata={"help": "An optional input evaluation data file to evaluate on (a csv or JSON file)."},
     )
     test_file: Optional[str] = field(
         default=None,
-        metadata={"help": "An optional input evaluation data file to evaluate the perplexity on (a text file)."},
+        metadata={"help": "An optional input test data file to predict on (a csv or JSON file)."},
     )
-    train_on_fly: Optional[str] = field(
-        default=True,
-        metadata={"help": "Whether to run text transformations (e.g tokenization) on the fly"}
+    output_predictions_file: Optional[str] = field(
+        default=None,
+        metadata={"help": "A location where to write the output of the test data"},
     )
-    validation_on_fly: Optional[str] = field(
-        default=False,
-        metadata={"help": "Whether to run text transformations (e.g tokenization) on the fly"}
+    text_column_name: Optional[str] = field(
+        default='tokens',
+        metadata={"help": "The column name of text to input in the file (a csv or JSON file)."}
     )
-    test_on_fly: Optional[str] = field(
-        default=False,
-        metadata={"help": "Whether to run text transformations (e.g tokenization) on the fly"}
+    label_column_name: Optional[str] = field(
+        default='labels',
+        metadata={"help": "The column name of label to input in the file (a csv or JSON file)."}
     )
     overwrite_cache: bool = field(
-        default=False, metadata={"help": "Overwrite the cached training and evaluation sets"}
-    )
-    max_seq_length: Optional[int] = field(
-        default=None,
-        metadata={
-            "help": "The maximum total input sequence length after tokenization. Sequences longer "
-            "than this will be truncated."
-        },
+        default=False,
+        metadata={"help": "Overwrite the cached training and evaluation sets"}
     )
     preprocessing_num_workers: Optional[int] = field(
         default=None,
         metadata={"help": "The number of processes to use for the preprocessing."},
     )
     pad_to_max_length: bool = field(
+        default=False,
+        metadata={
+            "help": "Whether to pad all samples to model maximum sentence length. "
+            "If False, will pad the samples dynamically when batching to the maximum length in the batch. More "
+            "efficient on GPU but very bad for TPU."
+        },
+    )
+    truncation: bool = field(
         default=True,
         metadata={
-            "help": "Whether to pad all samples to `max_seq_length`. "
-            "If False, will pad the samples dynamically when batching to the maximum length in the batch."
+            "help": "Activates and controls truncation"
         },
     )
-    text_column_name: Optional[str] = field(
-        default=None,
-        metadata={"help": "The column that contains the ICD10 codes"}
+    max_length: int = field(
+        default=512,
+        metadata={
+            "help": "Controls the maximum length to use by one of the truncation/padding parameters."
+        },
     )
-    note_id_column_name: Optional[str] = field(
-        default=None,
-        metadata={"help": "The column that contains the note ids"}
+    do_lower_case: bool = field(
+        default=False,
+        metadata={
+            "help": "Whether to lowercase the text"
+        },
     )
     max_train_samples: Optional[int] = field(
         default=None,
         metadata={
             "help": "For debugging purposes or quicker training, truncate the number of training examples to this "
             "value if set."
         },
@@ -112,40 +89,27 @@
             "help": "For debugging purposes or quicker training, truncate the number of evaluation examples to this "
             "value if set."
         },
     )
     max_predict_samples: Optional[int] = field(
         default=None,
         metadata={
-            "help": "For debugging purposes or quicker training, truncate the number of test examples to this "
-                    "value if set."
+            "help": "For debugging purposes or quicker training, truncate the number of prediction examples to this "
+            "value if set."
         },
     )
     label_all_tokens: bool = field(
         default=False,
         metadata={
-            "help": (
-                "Whether to put the label for one word on all tokens of generated by that word or just on the "
-                "one (in which case the other tokens will have a padding index)."
-            )
+            "help": "Whether to put the label for one word on all tokens of generated by that word or just on the "
+            "one (in which case the other tokens will have a padding index)."
         },
     )
     return_entity_level_metrics: bool = field(
         default=True,
         metadata={"help": "Whether to return all the entity levels during evaluation or just the overall ones."},
     )
-
-    def __post_init__(self):
-        if self.train_file is not None:
-            if type(self.train_file) == list:
-                extension = self.train_file[0].split(".")[-1]
-            else:
-                extension = self.train_file.split(".")[-1]
-            if extension not in ["csv", "json", "txt", "parquet", "zst", "jsonl"]:
-                raise ValueError("`train_file` should be a csv, a parquet, a json or a txt file.")
-        if self.validation_file is not None:
-            if type(self.validation_file) == list:
-                extension = self.validation_file[0].split(".")[-1]
-            else:
-                extension = self.validation_file.split(".")[-1]
-            if extension not in ["csv", "json", "txt", "parquet", "zst", "jsonl"]:
-                raise ValueError("`validation_file` should be a csv, a parquet, a json or a txt file.")
+    token_ignore_label: str = field(
+        default='NA',
+        metadata={"help": "The label that indicates where the tokens will be ignored in loss computation. Used for "
+                          "indicating context tokens to the model"}
+    )
```

### Comparing `robust_deid-0.3.0/src/robust_deid/arguments/model_arguments.py` & `robust_deid-0.3.1/src/robust_deid/sequence_tagging/arguments/model_arguments.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,43 @@
-from dataclasses import dataclass, field
 from typing import Optional
+from dataclasses import dataclass, field
 
 
 @dataclass
 class ModelArguments:
     """
-    Arguments pertaining to which model/config/tokenizer we are going to fine-tune, or train from scratch.
+    Arguments pertaining to which model/config/tokenizer we are going to fine-tune from.
     """
-    model_name_or_path: Optional[str] = field(
-        default=None,
-        metadata={
-            "help": "The model checkpoint for weights initialization."
-                    "Don't set if you want to train a model from scratch."
-        },
-    )
-    config_overrides: Optional[str] = field(
-        default=None,
-        metadata={
-            "help": "Override some existing default config settings when a model is trained from scratch. Example: "
-                    "n_embd=10,resid_pdrop=0.2,scale_attn_weights=false,summary_type=cls_index"
-        },
+    model_name_or_path: str = field(
+        metadata={"help": "Path to pretrained model or model identifier from huggingface.co/models"}
     )
     config_name: Optional[str] = field(
-        default=None, metadata={"help": "Pretrained config name or path if not the same as model_name"}
+        default=None,
+        metadata={"help": "Pretrained config name or path if not the same as model_name"}
     )
     tokenizer_name: Optional[str] = field(
-        default=None, metadata={"help": "Pretrained tokenizer name or path if not the same as model_name"}
-    )
-    spacy_model: Optional[str] = field(
         default=None,
-        metadata={
-            "help": "The spacy model to use for tokenization"
-        },
+        metadata={"help": "Pretrained tokenizer name or path if not the same as model_name"}
     )
     cache_dir: Optional[str] = field(
         default=None,
         metadata={"help": "Where do you want to store the pretrained models downloaded from huggingface.co"},
     )
-    use_fast_tokenizer: bool = field(
-        default=True,
-        metadata={"help": "Whether to use one of the fast tokenizer (backed by the tokenizers library) or not."},
-    )
     model_revision: str = field(
         default="main",
         metadata={"help": "The specific model version to use (can be a branch name, tag name or commit id)."},
     )
     use_auth_token: bool = field(
         default=False,
         metadata={
             "help": "Will use the token generated when running `transformers-cli login` (necessary to use this script "
                     "with private models)."
         },
     )
-    recall_threshold: Optional[float] = field(
+    post_process: str = field(
+        default='argmax',
+        metadata={"help": "What post processing to use on the model logits"},
+    )
+    threshold: Optional[float] = field(
         default=None,
         metadata={"help": "Threshold cutoff for softmax"},
     )
```

### Comparing `robust_deid-0.3.0/src/robust_deid/dataset_splitter.py` & `robust_deid-0.3.1/src/robust_deid/ner_datasets/dataset_splitter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-# Prepare dataset splits - training, validation & testing splits.
-# Write the splits to a file, so that they can be used later.
-
 import json
 import random
 from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
 from collections import Counter
 from typing import NoReturn, List
 
-from .sequence_datasets.setup.distribution import NERDistribution, DatasetSplits, PrintDistribution
+from .distribution import NERDistribution, DatasetSplits, PrintDistribution
 
 random.seed(41)
 
 
 class DatasetSplitter(object):
     """
     Prepare dataset splits - training, validation & testing splits
@@ -21,158 +18,139 @@
     Based on this distribution and whether we want to keep certain notes
     grouped (e.g by patient) we assign notes to a split, such that the
     final ner type distribution in each split is similar.
     """
 
     def __init__(
             self,
-            train_proportion: int = 80,
-            validation_proportion: int = 10,
-            test_proportion: int = 10
+            train_proportion: int = 70,
+            validation_proportion: int = 15,
+            test_proportion: int = 15
     ) -> NoReturn:
         """
         Initialize the proportions of the splits.
-
         Args:
-            train_proportion (int, defaults to `80`): Ratio of train dataset
-            validation_proportion (int, defaults to `10`): Ratio of validation dataset
-            test_proportion (int, defaults to `10`): Ratio of test dataset
+            train_proportion (int): Ratio of train dataset
+            validation_proportion (int): Ratio of validation dataset
+            test_proportion (int): Ratio of test dataset
         """
-
         self._train_proportion = train_proportion
         self._validation_proportion = validation_proportion
         self._test_proportion = test_proportion
         self._split = None
         self._lookup_split = dict()
 
     def get_split(self, split: str) -> List[str]:
-        """
-        Get the data associated with the specified split
-
-        Args:
-            split (str): The split
-
-        Returns:
-            (List[str]): The list of data elements associated with the specified split
-        """
-
         return [key for key in self._lookup_split[split].keys()]
 
     def set_split(self, split: str) -> NoReturn:
         """
         Set the split that you are currently checking/processing.
         Based on the split you can perform certain checks and
         computation. Once the split is set, read the information
         present in the split_info_path. Extract only the information
         belonging to the split. Create a hash map where we have
         the keys as the note_ids/patient ids that belong to the split. This hashmap
         can then be used to check if a particular note belongs to this
         split.
-
         Args:
             split (str): The split - train, test etc (depends on how you named it)
         """
-
         if split not in ['train', 'validation', 'test']:
             raise ValueError('Invalid split')
         self._split = split
 
     def __update_split(self, key: str) -> NoReturn:
         """
         Update the hash map where we have
         the keys (e.g note_id) that belong to the split. This hashmap
         can then be used to check if a particular note belongs to this
         split.
-
         Args:
             key (str): The key that identify the note belonging to the split
         """
-
         self._lookup_split[self._split][key] = 1
 
     def check_note(self, key: str) -> bool:
         """
         Use the hash map created in the __get_i2b2_filter_map function
         to check if the note (note_info) belongs to this split (train,
         val, test etc). If it does, return true, else false
-
         Args:
             key (str): The key that identify the note belonging to the split
-
         Returns:
             (bool): True if the note belongs to the split, false otherwise
         """
-
         if self._split is None:
             raise ValueError('Split not set')
         if self._lookup_split[self._split].get(key, False):
             return True
         else:
             return False
 
     def assign_splits(
             self,
             input_file: str,
             spans_key: str = 'spans',
+            metadata_key: str = 'meta',
             group_key: str = 'note_id',
             margin: float = 0.3
     ) -> NoReturn:
         """
         Get the dataset splits - training, validation & testing splits
         Based on the NER distribution and whether we want to keep certain
         notes grouped (e.g by patient). Return an iterable that contains
         a tuple that contains the note_id and the split. This can be used
         to filter notes based on the splits.
-
         Args:
             input_file (str): The input file
-            spans_key (str, defaults to `spans`): The key where the note spans are present
-            group_key (str, defaults to `note_id`): The key where the note group (e.g note_id or patient id etc)
-            is present. This field is what the notes will be grouped by, and all notes belonging to this grouping
-            will be in the same split
-            margin (float, defaults to `0.3`): Margin of error when maintaining proportions in the splits
+            spans_key (str): The key where the note spans are present
+            metadata_key (str): The key where the note metadata is present
+            group_key (str): The key where the note group (e.g note_id or patient id etc) is present.
+                             This field is what the notes will be grouped by, and all notes belonging
+                             to this grouping will be in the same split
+            margin (float): Margin of error when maintaining proportions in the splits
         """
-
         # Compute the distribution of NER types in the grouped notes.
         # For example the distribution of NER types in all notes belonging to a
         # particular patient
         self._lookup_split = {
             'train': dict(),
             'validation': dict(),
             'test': dict()
         }
         ner_distribution = NERDistribution()
         for line in open(input_file, 'r'):
             note = json.loads(line)
-            key = note[group_key]
+            key = note[metadata_key][group_key]
             ner_distribution.update_distribution(spans=note[spans_key], key=key)
         # Initialize the dataset splits object
         dataset_splits = DatasetSplits(
             ner_distribution=ner_distribution,
             train_proportion=self._train_proportion,
             validation_proportion=self._validation_proportion,
             test_proportion=self._test_proportion,
             margin=margin
         )
         # Check the note and assign it to a split
         for line in open(input_file, 'r'):
             note = json.loads(line)
-            key = note[group_key]
+            key = note[metadata_key][group_key]
             split = dataset_splits.get_split(key=key)
             self.set_split(split)
             self.__update_split(key)
         return None
 
 
 def main() -> NoReturn:
     """
     Prepare dataset splits - training, validation & testing splits
     Compute ner distributions in our dataset. Based on this distribution
     and whether we want to keep certain notes grouped (e.g by patient)
-    we assign notes to a split, such that the final ner type distribution
+    we assign notes to a split, such that the final ner type distribution 
     in each split is similar.
     """
     # Compute the distribution of NER types in the grouped notes.
     # For example the distribution of NER types in all notes belonging to a
     # particular patient
     # The following code sets up the arguments to be passed via CLI or via a JSON file
     cli_parser = ArgumentParser(
@@ -188,14 +166,20 @@
     cli_parser.add_argument(
         '--spans_key',
         type=str,
         default='spans',
         help='the key where the note spans is present in the json object'
     )
     cli_parser.add_argument(
+        '--metadata_key',
+        type=str,
+        default='meta',
+        help='the key where the note metadata is present in the json object'
+    )
+    cli_parser.add_argument(
         '--group_key',
         type=str,
         default='note_id',
         help='the key to group notes by in the json object'
     )
     cli_parser.add_argument(
         '--train_proportion',
@@ -241,67 +225,61 @@
     )
     cli_parser.add_argument(
         '--print_dist',
         action='store_true',
         help='whether to print the label distribution in the splits'
     )
     args = cli_parser.parse_args()
-
-    # Load the dataset splitter object
     dataset_splitter = DatasetSplitter(
         train_proportion=args.train_proportion,
         validation_proportion=args.validation_proportion,
         test_proportion=args.test_proportion
     )
-
-    # Assign note_ids to each splits
     dataset_splitter.assign_splits(
         input_file=args.input_file,
         spans_key=args.spans_key,
+        metadata_key=args.metadata_key,
         group_key=args.group_key,
         margin=args.margin
     )
 
-    # Write the train split to a file
     if args.train_proportion > 0:
         with open(args.train_file, 'w') as file:
             for line in open(args.input_file, 'r'):
                 note = json.loads(line)
-                key = note[args.group_key]
+                key = note[args.metadata_key][args.group_key]
                 dataset_splitter.set_split('train')
                 if dataset_splitter.check_note(key):
                     file.write(json.dumps(note) + '\n')
 
-    # Write the validation split to a file
     if args.validation_proportion > 0:
         with open(args.validation_file, 'w') as file:
             for line in open(args.input_file, 'r'):
                 note = json.loads(line)
-                key = note[args.group_key]
+                key = note[args.metadata_key][args.group_key]
                 dataset_splitter.set_split('validation')
                 if dataset_splitter.check_note(key):
                     file.write(json.dumps(note) + '\n')
 
-    # Write the test split to a file
     if args.test_proportion > 0:
         with open(args.test_file, 'w') as file:
             for line in open(args.input_file, 'r'):
                 note = json.loads(line)
-                key = note[args.group_key]
+                key = note[args.metadata_key][args.group_key]
                 dataset_splitter.set_split('test')
                 if dataset_splitter.check_note(key):
                     file.write(json.dumps(note) + '\n')
 
     if args.print_dist:
         # Read the dataset splits file and compute the NER type distribution
         key_counts = Counter()
         ner_distribution = NERDistribution()
         for line in open(args.input_file, 'r'):
             note = json.loads(line)
-            key = note[args.group_key]
+            key = note[args.metadata_key][args.group_key]
             key_counts[key] += 1
             ner_distribution.update_distribution(spans=note[args.spans_key], key=key)
         print_distribution = PrintDistribution(ner_distribution=ner_distribution, key_counts=key_counts)
         train_splits = dataset_splitter.get_split('train')
         validation_splits = dataset_splitter.get_split('validation')
         test_splits = dataset_splitter.get_split('test')
         all_splits = train_splits + validation_splits + test_splits
```

### Comparing `robust_deid-0.3.0/src/robust_deid/metrics/token_evaluation.py` & `robust_deid-0.3.1/src/robust_deid/sequence_tagging/evaluation/note_evaluation/note_token_evaluation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,159 +1,134 @@
 from collections import Counter
 from typing import Sequence, List, Tuple, Union, Type, Optional
 
 from seqeval.reporters import DictReporter
 from sklearn.metrics import precision_score, recall_score, f1_score, confusion_matrix
 
 
-class TokenEvaluation(object):
+class NoteTokenEvaluation(object):
     """
     This class is used to evaluate token level precision, recall and F1 scores.
     Script to evaluate at a token level. Calculate precision, recall, and f1 metrics
     at the token level rather than the span level.
     """
 
     @staticmethod
     def unpack_nested_list(nested_list: Sequence[Sequence[str]]) -> List[str]:
         """
         Use this function to unpack a nested list and also for token level evaluation we dont
         need to consider the B, I prefixes (depending on the NER notation, so remove that as well.
-
         Args:
             nested_list (Sequence[Sequence[str]]): A nested list of predictions/labels
-
         Returns:
             (List[str]): Unpacked nested list of predictions/labels
         """
-
         return [inner if inner == 'O' else inner[2:] for nested in nested_list for inner in nested]
 
     @staticmethod
     def get_counts(sequence: Sequence[str], ner_types: Sequence[str]) -> List[int]:
         """
-        Use this function to get the counts for each NER type.
-
+        Use this function to get the counts for each NER type
         Args:
-            sequence (Sequence[str]): Sequence of values that we want to calculate counts of unique values.
-            ner_types (Sequence[str]): A list of the NER types.
-
+            ner_list (Sequence[str]): A list of the NER labels/predicitons
         Returns:
             (List[int]): Position 0 contains the counts for the NER type that corresponds to position 0
         """
-
         counts = Counter()
         counts.update(sequence)
         return [counts[ner_type] for ner_type in ner_types]
 
     @staticmethod
     def precision_recall_fscore(
             labels: Sequence[str],
             predictions: Sequence[str],
             ner_types: Sequence[str],
             average: Optional[str] = None
     ) -> Tuple[Union[float, List[float]], Union[float, List[float]], Union[float, List[float]], Union[int, List[int]]]:
         """
-        Use this function to get the token level precision, recall and f-score. Internally we use the
+        Use this function to get the token level precision, recall and fscore. Internally we use the
         sklearn precision_score, recall_score and f1 score functions. Also return the count of each
         NER type.
-
         Args:
-            labels (Sequence[str]): A list of the gold standard NER labels.
-            predictions (Sequence[str]): A list of the predicted NER labels.
-            ner_types (Sequence[str]): A list of the NER types.
-            average (Optional[str], defaults to `None`): None for per NER types scores, or pass an appropriate average
-            value.
-
+            labels (Sequence[str]): A list of the gold standard NER labels
+            predictions (Sequence[str]): A list of the predicted NER labels
+            average (Optional[str]): None for per NER types scores, or pass an appropriate average value
         Returns:
             eval_precision (Union[float, List[float]]): precision score (averaged or per ner type)
             eval_precision (Union[float, List[float]]): recall score (averaged or per ner type)
             eval_precision (Union[float, List[float]]): F1 score (averaged or per ner type)
             counts (Union[int, List[int]]): Counts (total or per ner type)
         """
-
         eval_precision = precision_score(y_true=labels, y_pred=predictions, labels=ner_types, average=average)
         eval_recall = recall_score(y_true=labels, y_pred=predictions, labels=ner_types, average=average)
         eval_f1 = f1_score(y_true=labels, y_pred=predictions, labels=ner_types, average=average)
-        counts = TokenEvaluation.get_counts(sequence=labels, ner_types=ner_types)
-        if average is None:
+        counts = NoteTokenEvaluation.get_counts(sequence=labels, ner_types=ner_types)
+        if (average == None):
             eval_precision = list(eval_precision)
             eval_recall = list(eval_recall)
             eval_f1 = list(eval_f1)
         else:
             counts = sum(counts)
         return eval_precision, eval_recall, eval_f1, counts
 
     @staticmethod
-    def get_confusion_matrix(labels: List[str], predictions: List[str], ner_types: List[str]):
+    def get_confusion_matrix(labels: Sequence[str], predictions: Sequence[str], ner_types: Sequence[str]):
         """
-        Use this function to get the token level precision, recall and f-score per NER type
+        Use this function to get the token level precision, recall and fscore per NER type
         and also the micro, macro and weighted averaged precision, recall and f scores.
         Essentially we return a classification report
-
         Args:
             labels (Sequence[str]): A list of the gold standard NER labels
             predictions (Sequence[str]): A list of the predicted NER labels
-            ner_types (List[str]): A list of the NER types.
-
         Returns:
             (Type[DictReporter]): Classification report
         """
-
-        labels = TokenEvaluation.unpack_nested_list(labels)
-        predictions = TokenEvaluation.unpack_nested_list(predictions)
+        labels = NoteTokenEvaluation.unpack_nested_list(labels)
+        predictions = NoteTokenEvaluation.unpack_nested_list(predictions)
         return confusion_matrix(y_true=labels, y_pred=predictions, labels=ner_types + ['O', ])
 
     @staticmethod
     def classification_report(
             labels: Sequence[Sequence[str]],
             predictions: Sequence[Sequence[str]],
             ner_types: Sequence[str]
     ) -> Type[DictReporter]:
         """
-        Use this function to get the token level precision, recall and f-score per NER type
+        Use this function to get the token level precision, recall and fscore per NER type
         and also the micro, macro and weighted averaged precision, recall and f scores.
         Essentially we return a classification report which contains all this information
-
         Args:
             labels (Sequence[Sequence[str]]): A list of the gold standard NER labels for each note
             predictions (Sequence[Sequence[str]]): A list of the predicted NER labels for each note
-            ner_types (Sequence[str]): A list of the NER types.
-
         Returns:
             (Type[DictReporter]): Classification report that contains the token level metric scores
         """
-
         # Unpack the nested lists (labels and predictions) before running the evaluation metrics
-        labels = TokenEvaluation.unpack_nested_list(nested_list=labels)
-        predictions = TokenEvaluation.unpack_nested_list(nested_list=predictions)
-
+        labels = NoteTokenEvaluation.unpack_nested_list(nested_list=labels)
+        predictions = NoteTokenEvaluation.unpack_nested_list(nested_list=predictions)
         # Store results in this and return this object
         reporter = DictReporter()
         # Calculate precision, recall and f1 for each NER type
-        eval_precision, eval_recall, eval_f1, counts = TokenEvaluation.precision_recall_fscore(
+        eval_precision, eval_recall, eval_f1, counts = NoteTokenEvaluation.precision_recall_fscore(
             labels=labels,
             predictions=predictions,
             ner_types=ner_types,
             average=None
         )
-
         # Store the results
         for row in zip(ner_types, eval_precision, eval_recall, eval_f1, counts):
             reporter.write(*row)
         reporter.write_blank()
-
         # Calculate the overall precision, recall and f1 - based on the defined averages
         average_options = ('micro', 'macro', 'weighted')
         for average in average_options:
-            eval_precision, eval_recall, eval_f1, counts = TokenEvaluation.precision_recall_fscore(
+            eval_precision, eval_recall, eval_f1, counts = NoteTokenEvaluation.precision_recall_fscore(
                 labels=labels,
                 predictions=predictions,
                 ner_types=ner_types,
                 average=average
             )
             # Store the results
             reporter.write('{} avg'.format(average), eval_precision, eval_recall, eval_f1, counts)
-
-        # Add a blank line
         reporter.write_blank()
         # Return the token level results
         return reporter.report()
```

### Comparing `robust_deid-0.3.0/src/robust_deid/sequence_datasets/builder/sequence_dataset.py` & `robust_deid-0.3.1/src/robust_deid/sequence_tagging/dataset_builder/ner_dataset.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,102 @@
-from typing import Optional
+from typing import Sequence, Optional, NoReturn
 
-from datasets import DatasetDict, Dataset
+from datasets import load_dataset, Dataset
 
 
-class SequenceDataset(object):
+class NERDataset(object):
     """
-    Class that outlines the functions that can be used to prepare the datasets
-    for training and evaluation, and run the training and evaluation of the models
+    This class is a wrapper around the huggingface datasets library
+    It maintains the train, validation and test datasets based on the
+    train, validation and test files passed by loading the dataset object
+    from the file and provides a get function to access each of the datasets. 
     """
 
     def __init__(
             self,
-            sentence_datasets: DatasetDict,
-    ):
+            train_file: Optional[Sequence[str]] = None,
+            validation_file: Optional[Sequence[str]] = None,
+            test_file: Optional[Sequence[str]] = None,
+            extension: str = 'json',
+            shuffle: bool = True,
+            seed: int = 41
+    ) -> NoReturn:
         """
-        Initialize the Huggingface DatasetDict object that contains the train, eval and test splits
-
+        Load the train, validation and test datasets from the files passed. Read the files and convert
+        it into a huggingface dataset.
         Args:
-            sentence_datasets (DatasetDict): The dataset object that contains the data for each split (train, val etc)
+            train_file (Optional[Sequence[str]]): The list of files that contain train data
+            validation_file (Optional[Sequence[str]]): The list of files that contain validation data
+            test_file (Optional[Sequence[str]]): The list of files that contain test data
+            shuffle (bool): Whether to shuffle the dataset
+            seed (int): Shuffle seed
+       
+        """
+        self._datasets = NERDataset.__prepare_data(
+            train_file,
+            validation_file,
+            test_file,
+            extension,
+            shuffle,
+            seed
+        )
+
+    @staticmethod
+    def __prepare_data(
+            train_file: Optional[Sequence[str]],
+            validation_file: Optional[Sequence[str]],
+            test_file: Optional[Sequence[str]],
+            extension: str,
+            shuffle: bool,
+            seed: int
+    ) -> Dataset:
         """
-
-        self._sentence_datasets = sentence_datasets
-
-    def get_train_dataset(self, max_train_samples: Optional[int]) -> Optional[Dataset]:
-        """
-        Return the train split of the dataset object.
-
+        Get the train, validation and test datasets from the files passed. Read the files and convert
+        it into a huggingface dataset.
         Args:
-            max_train_samples (Optional[int]): For debugging purposes or quicker training, truncate the number of
-            training examples to this value if set.
-
+            train_file (Optional[Sequence[str]]): The list of files that contain train data
+            validation_file (Optional[Sequence[str]]): The list of files that contain validation data
+            test_file (Optional[Sequence[str]]): The list of files that contain test data
+            shuffle (bool): Whether to shuffle the dataset
+            seed (int): Shuffle seed
         Returns:
-            train_dataset (Optional[Dataset]): The training dataset. Returns None if train split does not exist.
+            (Dataset): The huggingface dataset with train, validation, test splits (if included)
         """
+        # Read the datasets (train, validation, test etc).
+        data_files = {}
+        if train_file is not None:
+            data_files['train'] = train_file
+        if validation_file is not None:
+            data_files['validation'] = validation_file
+        if test_file is not None:
+            data_files['test'] = test_file
+        # Shuffle the dataset
+        if shuffle:
+            datasets = load_dataset(extension, data_files=data_files).shuffle(seed=seed)
+        else:
+            # Don't shuffle the dataset
+            datasets = load_dataset(extension, data_files=data_files)
+        return datasets
 
-        # Check if the DatasetDict object contains the train split
-        if "train" not in self._sentence_datasets:
-            return None
-        train_dataset = self._sentence_datasets["train"]
-        # Select only a subset of training examples if desired.
-        if max_train_samples is not None:
-            max_train_samples = min(len(train_dataset), max_train_samples)
-            train_dataset = train_dataset.select(range(max_train_samples))
-        return train_dataset
-
-    def get_eval_dataset(self, max_eval_samples: Optional[int]) -> Optional[Dataset]:
+    def get_train_dataset(self) -> Dataset:
         """
-        Return the validation split of the dataset object.
-
-        Args:
-            max_eval_samples (Optional[int]): For debugging purposes or quicker training, truncate the number of
-            validation examples to this value if set.
-
+        Return the train dataset
         Returns:
-            eval_dataset (Optional[Dataset]): The validation dataset. Returns None if validation split does not exist.
+            (Dataset): The huggingface dataset - train split
         """
+        return self._datasets['train']
 
-        # Check if the DatasetDict object contains the validation split
-        if "validation" not in self._sentence_datasets:
-            return None
-        # Select only a subset of validation examples if desired.
-        eval_dataset = self._sentence_datasets["validation"]
-        if max_eval_samples is not None:
-            max_eval_samples = min(len(eval_dataset), max_eval_samples)
-            eval_dataset = eval_dataset.select(range(max_eval_samples))
-        return eval_dataset
-
-    def get_test_dataset(self, max_test_samples: Optional[int]) -> Optional[Dataset]:
+    def get_validation_dataset(self) -> Dataset:
         """
-        Return the test split of the dataset object.
-
-        Args:
-            max_test_samples (Optional[int]): For debugging purposes or quicker training, truncate the number of test
-            examples to this value if set.
-
+        Return the validation dataset
         Returns:
-            test_dataset (Optional[Dataset]): The test dataset. Returns None if test split does not exist.
+            (Dataset): The huggingface dataset - validation split
         """
+        return self._datasets['validation']
 
-        # Check if the DatasetDict object contains the test split
-        if "test" not in self._sentence_datasets:
-            return None
-        test_dataset = self._sentence_datasets["test"]
-        # Select only a subset of validation examples if desired.
-        if max_test_samples is not None:
-            max_test_samples = min(len(test_dataset), max_test_samples)
-            test_dataset = test_dataset.select(range(max_test_samples))
-        return test_dataset
+    def get_test_dataset(self) -> Dataset:
+        """
+        Return the test dataset
+        Returns:
+            (Dataset): The huggingface dataset - test split
+        """
+        return self._datasets['test']
```

### Comparing `robust_deid-0.3.0/src/robust_deid/sequence_datasets/labels/label_info.py` & `robust_deid-0.3.1/src/robust_deid/sequence_tagging/dataset_builder/ner_labels.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,79 +1,67 @@
-from typing import Sequence, List, Dict
+from typing import Sequence, List, NoReturn, Dict
 
 
-class LabelInfo(object):
+class NERLabels(object):
     """
     Prepare the labels that will be used by the model. Parse the NER types
     and prepare the NER labels. For example - NER Types: [AGE, DATE],
     it will create a list like this (for BIO notation) [B-AGE, I-AGE, B-DATE, I-DATE, O]
     These are the labels that will be assigned to the tokens based on the PHI type.
     Say we had the following NER types: NAME, AGE, HOSP
     The NER labels in the BIO notation would be B-AGE, B-HOSP, B-NAME, I-AGE, I-HOSP, I-NAME, O
     This script creates a list of the NER labels ([B-AGE, B-HOSP, B-NAME, I-AGE, I-HOSP, I-NAME, O])
     based on the NER types (NAME, AGE, HOSP) that have been defined. Labels have been sorted.
     The script also returns the number of labels, the label_to_id mapping, the id_to_label mapping
     Label_id_mapping: {B-AGE:0, B-HOSP:1, B-NAME:2, I-AGE:3, I-HOSP:4, I-NAME:5, O:6}
     This information will be used  during training, evaluation and prediction.
     """
 
-    def __init__(self, notation: str, ner_types: Sequence[str]):
+    def __init__(self, notation: str, ner_types: Sequence[str]) -> NoReturn:
         """
-        Initialize the notation that we are using for the NER task.
-
+        Initialize the notation that we are using for the NER task
         Args:
-            notation (str): The notation that will be used for the NER labels.
-            ner_types (Sequence[str]): The list of NER categories (e.g AGE, PHONE etc.).
+            notation (str): The notation that will be used for the NER labels
+            ner_types (Sequence[str]): The list of NER categories
         """
-
         self._notation = notation
         self._ner_types = ner_types
 
     def get_label_list(self) -> List[str]:
         """
         Given the NER types return the NER labels.
-        NER Types: [AGE, DATE] -> return a list like this (for BIO notation)
-        [B-AGE, I-AGE, B-DATE, I-DATE, O].
-
+        NER Types: [AGE, DATE] -> return a list like this (for BIO notation) [B-AGE, I-AGE, B-DATE, I-DATE, O]
         Returns:
-            ner_labels (List[str]): The list of NER labels based on the NER notation (e.g BIO).
+            ner_labels (List[str]): The list of NER labels based on the NER notation (e.g BIO)
         """
-
         # Add the 'O' (Outside - Non-phi) label to the list
         if 'O' not in self._ner_types:
             ner_labels = ['O']
         else:
             ner_labels = list()
-
         # Go through each label and prefix it based on the notation (e.g - B, I etc)
         for ner_type in self._ner_types:
             for ner_tag in list(self._notation):
                 if ner_tag != 'O':
                     ner_labels.append(ner_tag + '-' + ner_type)
-
-        # Sort the labels - make it deterministic
         ner_labels.sort()
         return ner_labels
 
     def get_label_to_id(self) -> Dict[str, int]:
         """
-        Return a label to id mapping.
-
+        Return a label to id mapping
         Returns:
             label_to_id (Dict[str, int]): label to id mapping
         """
-
         labels = self.get_label_list()
         label_to_id = {label: index_id for index_id, label in enumerate(labels)}
         return label_to_id
 
     def get_id_to_label(self) -> Dict[int, str]:
         """
-        Return a id to label mapping.
-
+        Return a id to label mapping
         Returns:
-            id_to_label (Dict[int, str]): id to label mapping.
+            id_to_label (Dict[int, str]): id to label mapping
         """
-
         labels = self.get_label_list()
         id_to_label = {index_id: label for index_id, label in enumerate(labels)}
         return id_to_label
```

### Comparing `robust_deid-0.3.0/src/robust_deid/sequence_datasets/sequences/sequence_chunker.py` & `robust_deid-0.3.1/src/robust_deid/ner_datasets/dataset_builder/sentence_dataset.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,212 +1,167 @@
 from collections import deque
-from typing import Deque, List, Sequence, Iterable, Optional, NoReturn, Dict, Tuple, Any
+from typing import Deque, List, Sequence, Iterable, Optional, NoReturn, Dict, Mapping, Union, Tuple
 
 
-class SequenceChunker(object):
+class SentenceDataset(object):
     """
     When we mention previous sentence and next sentence, we don't mean exactly one sentence
     but rather a previous chunk and a next chunk. This can include one or more sentences and
     it does not mean that the sentence has to be complete (it can be cutoff in between) - hence a chunk
-    This class is used to build a dataset at the sentence level. It takes as input all the tokenized
-    sentences in the note. So the input is a list of lists where the outer list represents the sentences
-    in the note and the inner list is a list of tokens in the sentence. It then returns a dataset where
-    each element in the list contains the tokens that form the previous chunk, the current chunk
-    and the next chunk. This is done so that when we build a model we can use the previous and next chunks
-    to add context to the sentence/model. We could have different sizes of previous and next chunks
+    This class is used to build a dataset at the sentence
+    level. It takes as input all the tokenized sentences in the note. So the input is
+    a list of lists where the outer list represents the sentences in the note and the inner list
+    is a list of tokens in the sentence. It then returns a dataset where each sentence is 
+    concatenated with the previous and a next chunk. This is done so that when we build a model
+    we can use the previous and next chunks to add context to the sentence/model. The weights and loss etc
+    will be computed and updated based on the current sentence. The previous and next chunks will
+    only be used to add context. We could have different sizes of previous and next chunks
     depending on the position of the sentence etc. Essentially we build a sentence level dataset
     where we can also provide context to the sentence by including the previous and next chunks
     """
 
     def __init__(
             self,
             max_tokens: int,
-            max_prev_sentence_tokens: int,
-            max_next_sentence_tokens: int,
+            max_prev_sentence_token: int,
+            max_next_sentence_token: int,
             default_chunk_size: int,
+            ignore_label: str
     ) -> NoReturn:
         """
         Set the maximum token length a given training example (sentence level) can have.
         That is the total length of the current sentence + previous chunk + next chunk
         We also set the the maximum length of the previous and next chunks. That is how many
         tokens can be in these chunks. However if the total length exceeds, tokens in the
         previous and next chunks will be dropped to ensure that the total length is < max_tokens
         The default chunk size ensures that the length of the chunks will be a minimum number of
         tokens based on the value passed. For example is default_chunk_size=10, the length
         of the previous chunks and next chunks will be at least 10 tokens.
-
         Args:
-            max_tokens (int): The maximum token length a given training example (sentence level) can have.
-            max_prev_sentence_tokens (int): The max chunk size for the previous chunks for a given sentence
-            (training/prediction example) in the note can have.
-            max_next_sentence_tokens (int): The max chunk size for the next chunks for a given sentence
-            (training/prediction example) in the note can have.
+            max_tokens (int): maximum token length a given training example (sentence level) can have
+            max_prev_sentence_token (int): The max chunk size for the previous chunks for a given sentence 
+                                           (training/prediction example) in the note can have
+            max_next_sentence_token (int): The max chunk size for the next chunks for a given sentence 
+                                           (training/prediction example) in the note can have
             default_chunk_size (int): the training example will always include a chunk of this length
-            as part of the previous and next chunks.
+                                      as part of the previous and next chunks
+            ignore_label (str): The label assigned to the previous and next chunks to distinguish
+                                from the current sentence
         """
-
         self._id_num = None
         self._max_tokens = max_tokens
-        self._max_prev_sentence_tokens = max_prev_sentence_tokens
-        self._max_next_sentence_tokens = max_next_sentence_tokens
+        self._max_prev_sentence_token = max_prev_sentence_token
+        self._max_next_sentence_token = max_next_sentence_token
         self._default_chunk_size = default_chunk_size
+        self._ignore_label = ignore_label
 
     @staticmethod
-    def _get_chunks(
-            seq: List[Tuple[Any, int]],
+    def chunker(
+            seq: Sequence[Mapping[str, Union[str, int]]],
             size: int
-    ) -> Iterable[List[Tuple[Any, int]]]:
+    ) -> Iterable[Sequence[Mapping[str, Union[str, int]]]]:
         """
         Return chunks of the sequence. The size of each chunk will be based
         on the value passed to the size argument.
-
         Args:
-            seq (List[Tuple[Any, int]]): The sequence to be chunked.
-            size (int): The max chunk size for the chunks.
-
-        Returns:
-            (Iterable[List[Tuple[Any, int]]]): Iterable that iterates through fixed size chunks of
-            the input sequence chunked version of the sequence.
+            seq (Sequence): maximum token length a given training example (sentence level) can have
+            size (int): The max chunk size for the chunks
+        Return:
+            (Iterable[Sequence[Mapping[str, Union[str, int]]]]): Iterable that iterates through fixed size chunks of
+                                                                 the input sequence chunked version of the sequence
+                         
         """
+        return (seq[pos:pos + size] for pos in range(0, len(seq), size))
 
-        count = 0
-        chunked_seq = list()
-        for token in seq:
-            # Append when the size of the chunk is less than maximum size
-            if count + token[1] <= size:
-                count += token[1]
-                chunked_seq.append(token)
-            # Return the chunk when it has reached the maximum size
-            else:
-                yield chunked_seq
-                chunked_seq = list()
-                count = token[1]
-                chunked_seq.append(token)
-        # Return the final chunk
-        if len(chunked_seq) != 0:
-            yield chunked_seq
-
-    @staticmethod
-    def _get_sentence_length(sentence: Sequence[Tuple[Any, int]]) -> int:
-        """
-        Get the number of subwords in the sentence.
-
-        Args:
-            sentence (Sequence[Tuple[Any, int]]): A list of tuples that contains token object, and how many
-            subwords the token contains.
-
-        Returns:
-            (int): The total number of subwords in the sequence
-        """
-
-        count = 0
-        for token in sentence:
-            # The token is a tuple where the second element contains the number of
-            # subwords for that token
-            count += token[1]
-        return count
-
-    def get_previous_sentences(
-            self,
-            sent_tokens: Sequence[Sequence[Tuple[Any, int]]]
-    ) -> List[Deque]:
+    def get_previous_sentences(self, sent_tokens: Sequence[Sequence[Mapping[str, Union[str, int]]]]) -> List[Deque]:
         """
         Go through all the sentences in the medical note and create a list of
         previous sentences. The output of this function will be a list of chunks
         where each index of the list contains the sentences (chunks) - (tokens) present before
         the sentence at that index in the medical note. For example prev_sent[0] will
         be empty since there is no sentence before the first sentence in the note
         prev_sent[1] will be equal to sent[0], that is the previous sentence of the
         second sentence will be the first sentence. We make use of deque, where we
         start to deque elements when it start to exceed max_prev_sentence_token. This
         list of previous sentences will be used to define the previous chunks
-
         Args:
-            sent_tokens (Sequence[Sequence[Tuple[Any, int]]]): Sentences in the note and each element of the list
-            contains a list of tokens in that sentence.
-
+            sent_tokens (Sequence[str]): Sentences in the note and 
+                                         each element of the list contains a
+                                         list of tokens in that sentence
         Returns:
-            previous_sentences (List[deque]): A list of deque objects where each index contains a list (queue) of
-            previous tokens (chunk) with respect to the sentence represented by that index in the note.
+            previous_sentences (List[deque]): A list of deque objects where each index contains a 
+                                              list (queue) of previous tokens (chunk) with respect 
+                                              to the sentence represented by that index in the note
         """
-
         previous_sentences = list()
-
         # Create a queue and specify the capacity of the queue
         # Tokens will be popped from the queue when the capacity is exceeded
-        prev_sentence = deque(maxlen=self._max_prev_sentence_tokens)
-
+        prev_sentence = deque(maxlen=self._max_prev_sentence_token)
         # The first previous chunk is empty since the first sentence in the note does not have
         # anything before it
         previous_sentences.append(prev_sentence.copy())
-
         # As we iterate through the list of sentences in the not, we add the tokens from the previous chunks
         # to the the queue. Since we have a queue, as soon as the capacity is exceeded we pop tokens from
         # the queue
         for sent_token in sent_tokens[:-1]:
             for token in sent_token:
                 prev_sentence.append(token)
             # As soon as each sentence in the list is processed
             # We add a copy of the current queue to a list - this list keeps track of the
             # previous chunks for a sentence
             previous_sentences.append(prev_sentence.copy())
 
         return previous_sentences
 
-    def get_next_sentences(
-            self,
-            sent_tokens: Sequence[Sequence[Tuple[Any, int]]]
-    ) -> List[Deque]:
+    def get_next_sentences(self, sent_tokens: Sequence[Sequence[Mapping[str, Union[str, int]]]]) -> List[Deque]:
         """
         Go through all the sentences in the medical note and create a list of
         next sentences. The output of this function will be a list of lists
         where each index of the list contains the list of sentences present after
         the sentence at that index in the medical note. For example next_sent[-] will
         be empty since there is no sentence after the last sentence in the note
         next_sent[0] will be equal to sent[1:], that is the next sentence of the
         first sentence will be the subsequent sentences. We make use of deque, where we
         start to deque elements when it start to exceed max_next_sentence_token. This
         list of previous sentences will be used to define the previous chunks
-
         Args:
-            sent_tokens (Sequence[Sequence[Tuple[Any, int]]]): Sentences in the note and each element of the list
-            contains a list of tokens in that sentence
-
+            sent_tokens (Sequence[str]): Sentences in the note and each 
+                                         element of the list contains a
+                                         list of tokens in that sentence
         Returns:
-            next_sentences (List[deque]): A list of deque objects where each index contains a list (queue) of
-            next tokens (chunk) with respect to the sentence represented by that index in the note
+            next_sentences (List[deque]): A list of deque objects where each index contains a list (queue) 
+                                          of next tokens (chunk) with respect to the sentence represented 
+                                          by that index in the note
         """
-
         # A list of next sentences is first created and reversed
         next_sentences = list()
-
         # Create a queue and specify the capacity of the queue
         # Tokens will be popped from the queue when the capacity is exceeded
-        next_sentence = deque(maxlen=self._max_next_sentence_tokens)
-
+        next_sentence = deque(maxlen=self._max_next_sentence_token)
         # The first (which becomes the last chunk when we reverse this list) next chunk is empty since
         # the last sentence in the note does not have
         # anything after it
         next_sentences.append(next_sentence.copy())
         for sent_token in reversed(sent_tokens[1:]):
             for token in reversed(sent_token):
                 next_sentence.appendleft(token)
             next_sentences.append(next_sentence.copy())
-
         # The list is reversed - since we went through the sentences in the reverse order in
         # the earlier steps
         return [next_sent for next_sent in reversed(next_sentences)]
 
-    def get_sentence_chunks(
+    def get_sentences(
             self,
-            sentence_tokens: List[List[Tuple[Any, int]]],
-            start_chunk: Optional[List[Tuple[Any, int]]] = None,
-            end_chunk: Optional[List[Tuple[Any, int]]] = None,
+            sent_tokens: Sequence[Sequence[Mapping[str, Union[str, int]]]],
+            token_text_key: str = 'text',
+            label_key: str = 'label',
+            start_chunk: Optional[Sequence[Mapping[str, Union[str, int]]]] = None,
+            end_chunk: Optional[Sequence[Mapping[str, Union[str, int]]]] = None,
             sub: bool = False
-    ) -> Iterable[Tuple[str, Dict[str, List[Tuple[Any, int]]]]]:
+    ) -> Iterable[Tuple[int, Dict[str, Union[List[Dict[str, Union[str, int]]], List[str]]]]]:
         """
         When we mention previous sentence and next sentence, we don't mean exactly one sentence
         but rather a previous chunk and a next chunk. This can include one or more sentences and
         it does not mean that the sentence has to be complete (it can be cutoff in between) - hence a chunk
         We iterate through all the tokenized sentences in the note. So the input is
         a list of lists where the outer list represents the sentences in the note and the inner list
         is a list of tokens in the sentence. It then returns a dataset where each sentence is
@@ -214,129 +169,158 @@
         we can use the previous and next sentence to add context to the model. The weights and loss etc
         will be computed and updated based on the current sentence. The previous and next sentence will
         only be used to add context. We could have different sizes of previous and next chunks
         depending on the position of the sentence etc. Since we split a note in several sentences which are
         then used as training data.
         ignore_label is used to differentiate between the current sentence and the previous and next
         chunks. The chunks will have the label NA so that and the current sentence
-        will have the label (DATE, AGE etc) so that they can be distinguished.
+        will have the label (DATE, AGE etc) so that they can be distinguished. 
         If however we are building a dataset for predictions
         the current sentence will have the default label O, but the next and previous chunks will still
         have the label NA. However if the total length exceeds, tokens in the
         previous and next chunks will be dropped to ensure that the total length is < max_tokens
         The default chunk size ensures that the length of the chunks will be a minimum number of
         tokens based on the value passed. For example is default_chunk_size=10, the length
         of the previous chunks and next chunks will be at least 10 tokens. If the total length > max tokens
-        even after decreasing the sizes of the previous and next chunks, then we split this long
+        even after decreasing the sizes of the previous and next chunks, then we split this long 
         sentence into sub sentences and repeat the process described above.
-
         Args:
-            sentence_tokens (List[List[Tuple[Any, int]]]): Sentences in the note and each sentence contain
-            the tokens (dict) in that sentence the token dict object contains the token text, start, end etc.
-            start_chunk (Optional[List[Tuple[Any, int]]]): Prefix the first sentence of with some
-            pre-defined chunk
-            end_chunk (Optional[List[Tuple[Any, int]]]): Suffix the last sentence of with some
-            pre-defined chunk
-            sub (bool): Whether the function is called to process sub-sentences (used when we are splitting
-            long sentences into smaller sub sentences to keep sentence length < max_tokens
-
+            sent_tokens (Sequence[Sequence[Mapping[str, Union[str, int]]]]): Sentences in the note and each sentence 
+                                                                             contains the tokens (dict) in that sentence
+                                                                             the token dict object contains the
+                                                                             token text, start, end etc
+            token_text_key (str): Each sentence contains a list of tokens where each token is a dict. We use the text
+                                  key to extract the text of the token from the dictionary
+            label_key (str): Each sentence contains a list of tokens where each token is a dict. We use the label_key
+                             key to extract the label of the token from the dictionary. (if it does not have a label
+                             the default label will be assigned)
+            start_chunk (Optional[Sequence[Mapping[str, Union[str, int]]]]): Prefix the first sentence of with some
+                                                                             pre-defined chunk
+            end_chunk (Optional[Sequence[Mapping[str, Union[str, int]]]]): Suffix the last sentence of with some
+                                                                            pre-defined chunk
+            sub (bool): Whether the function is called to process sub-sentences (used when we are splitting 
+                        long sentences into smaller sub sentences to keep sentence length < max_tokens
         Returns:
-            (Iterable[Tuple[str, Dict[str, List[Tuple[Any, int]]]]]): Iterate through the returned sentences, where
-            each sentence has the previous chunks and next chunks attached to it.
+            (Iterable[Tuple[int, Dict[str, Union[List[Dict[str, Union[str, int]]], List[str]]]]]): Iterate through the
+                                                                                                   returned sentences,
+                                                                                                   where each sentence
+                                                                                                   has the previous
+                                                                                                   chunks and next
+                                                                                                   chunks attached
+                                                                                                   to it.
         """
-
         # Id num keeps track of the id of the sentence - that is the position the sentence occurs in
         # the note. We keep the id of sub sentences the same as the sentence, so that the user
         # knows that these sub sentences are chunked from a longer sentence.
         # <SENT 0> <SENT 1>. Say length of sent 0 with the previous and next chunks is less than max_tokens
         # we return sent 0 with id 0. For sent 1, say the length is longer, we split it into sub
         # sentences - <SUB 1><SUB 2> - we return SUB 1, and SUB 2 with id 1 - so we know that it belongs
         # to <SENT 1> in the note.
         if not sub:
             self._id_num = -1
-
         # Initialize the object that will take all the sentences in the note and return
         # a dataset where each row represents a sentence in the note. The sentence in each
         # row will also contain a previous chunk and next chunk (tokens) that will act as context
         # when training the mode
         # [ps1, ps 2, ps 3...ps-i], [cs1, cs2, ... cs-j], [ns, ns, ... ns-k] - as you can see the current sentence
         # which is the sentence we train on (or predict on) will be in the middle - the surrounding tokens will
         # provide context to the current sentence
         # Get the previous sentences (chunks) for each sentence in the note
-        previous_chunks_tokens = self.get_previous_sentences(sentence_tokens)
+        previous_sentences = self.get_previous_sentences(sent_tokens)
         # Get the next sentences (chunks) for each sentence in the note
-        next_chunks_tokens = self.get_next_sentences(sentence_tokens)
-
+        next_sentences = self.get_next_sentences(sent_tokens)
         # For the note we are going to iterate through all the sentences in the note and
         # concatenate each sentence with the previous and next chunks. (This forms the data that
         # will be used for training/predictions) Each sentence with the concatenated chunks will be
         # a training sample. We would do the same thing for getting predictions on a sentence as well
         # The only difference would be the labels that are used. We would use the default label O for
         # prediction and the annotated labels for prediction
-        if len(sentence_tokens) != len(previous_chunks_tokens) or len(sentence_tokens) != len(next_chunks_tokens):
+        if len(sent_tokens) != len(previous_sentences) or len(sent_tokens) != len(next_sentences):
             raise ValueError('Sentence length mismatch')
-        for index, (previous_chunk_tokens, current_sentence_tokens, next_chunk_tokens) in enumerate(
-                zip(previous_chunks_tokens, sentence_tokens, next_chunks_tokens)
-        ):
+        for index, (previous_sent, current_sent, next_sent) in enumerate(
+                zip(previous_sentences, sent_tokens, next_sentences)):
+            sent_tokens_text = list()
+            sent_labels = list()
+            sent_toks = list()
+            # Get the tokens and labels for the current sentence
+            for token in current_sent:
+                # We store this, if we need to process sub sentences when a sentence exceeds max_tokens
+                sent_toks.append(token)
+                sent_tokens_text.append(token[token_text_key])
+                sent_labels.append(token[label_key])
             # We check if the number of tokens in teh current sentence + previous chunk
             # + next chunk exceeds max tokens. If it does we start popping tokens from the previous and next chunks
             # until the number of tokens is equal to max tokens
-            previous_chunk_length = self._get_sentence_length(previous_chunk_tokens)
-            current_sentence_length = self._get_sentence_length(current_sentence_tokens)
-            next_sentence_length = self._get_sentence_length(next_chunk_tokens)
-            total_length = previous_chunk_length + current_sentence_length + next_sentence_length
-
+            previous_sent_length = len(previous_sent)
+            current_sent_length = len(sent_tokens_text)
+            next_sent_length = len(next_sent)
+            total_length = previous_sent_length + current_sent_length + next_sent_length
             # If the length of the current sentence plus the length of the previous and next
             # chunks exceeds the max_tokens, start popping tokens from the previous and next
             # chunks until either total length < max_tokens or the number of tokens in the previous and
             # next chunks goes below the default chunk size
-            while (
-                    total_length > self._max_tokens and
-                    (next_sentence_length > self._default_chunk_size or
-                     previous_chunk_length > self._default_chunk_size)
-            ):
-                if next_sentence_length >= previous_chunk_length:
-                    _, length = next_chunk_tokens.pop()
-                    next_sentence_length -= length
-                    total_length -= length
-                elif previous_chunk_length > next_sentence_length:
-                    _, length = previous_chunk_tokens.popleft()
-                    previous_chunk_length -= length
-                    total_length -= length
-
+            while total_length > self._max_tokens and \
+                    (next_sent_length > self._default_chunk_size or previous_sent_length > self._default_chunk_size):
+                if next_sent_length >= previous_sent_length:
+                    next_sent.pop()
+                    next_sent_length -= 1
+                    total_length -= 1
+                elif previous_sent_length > next_sent_length:
+                    previous_sent.popleft()
+                    previous_sent_length -= 1
+                    total_length -= 1
             # If this is not a sub sentence, increment the ID to
             # indicate the processing of the next sentence of the note
             # If it is a sub sentence, keep the ID the same, to indicate
             # it belongs to a larger sentence
             if not sub:
                 self._id_num += 1
-
             # If total length < max_tokens - process the sentence with the current sentence
             # and add on the previous and next chunks and return
             if total_length <= self._max_tokens:
                 # Check if we want to add a pre-defined chunk for the first sentence in the note
                 if index == 0 and start_chunk is not None:
-                    previous_chunk = start_chunk + list(previous_chunk_tokens)
+                    previous_sent_tokens = [chunk[token_text_key] for chunk in start_chunk] + \
+                                           [prev_token[token_text_key] for prev_token in list(previous_sent)]
                 else:
-                    previous_chunk = list(previous_chunk_tokens)
+                    previous_sent_tokens = [prev_token[token_text_key] for prev_token in list(previous_sent)]
                 # Check if we want to add a pre-defined chunk for the last sentence in the note
-                if index == len(sentence_tokens) - 1 and end_chunk is not None:
-                    next_chunk = list(next_chunk_tokens) + end_chunk
+                if index == len(sent_tokens) - 1 and end_chunk is not None:
+                    next_sent_tokens = [next_token[token_text_key] for next_token in list(next_sent)] + \
+                                       [chunk[token_text_key] for chunk in end_chunk]
                 else:
-                    next_chunk = list(next_chunk_tokens)
+                    next_sent_tokens = [next_token[token_text_key] for next_token in list(next_sent)]
+                previous_sent_length = len(previous_sent_tokens)
+                next_sent_length = len(next_sent_tokens)
+                # Store information about the current sentence - start and end pos etc
+                # this can be used to distinguish from the next and previous chunks
+                # current_sent_info = {'token_info':current_sent}
+                # Assign an different label (the ignore label) to the chunks - since they are used only for context
+                previous_sent_labels = list()
+                next_sent_labels = list()
+                if self._ignore_label == 'NA':
+                    previous_sent_labels = [self._ignore_label] * previous_sent_length
+                    next_sent_labels = [self._ignore_label] * next_sent_length
+                elif self._ignore_label == 'label':
+                    if index == 0 and start_chunk is not None:
+                        previous_sent_labels = [chunk[label_key] for chunk in start_chunk] + \
+                                               [prev_token[label_key] for prev_token in list(previous_sent)]
+                    else:
+                        previous_sent_labels = [prev_token[label_key] for prev_token in list(previous_sent)]
+                    if index == len(sent_tokens) - 1 and end_chunk is not None:
+                        next_sent_labels = [next_token[label_key] for next_token in list(next_sent)] + \
+                                           [chunk[label_key] for chunk in end_chunk]
+                    else:
+                        next_sent_labels = [next_token[label_key] for next_token in list(next_sent)]
+                # Concatenate the chunks and the sentence
+                # sent_tokens_text.append(token[token_text_key])
+                tokens_data = previous_sent_tokens + sent_tokens_text + next_sent_tokens
+                labels_data = previous_sent_labels + sent_labels + next_sent_labels
                 # Return processed sentences
-                yield (
-                    self._id_num,
-                    {
-                        'previous_chunk': previous_chunk,
-                        'current_chunk': current_sentence_tokens,
-                        'next_chunk': next_chunk
-                    }
-                )
-
+                yield self._id_num, {'tokens': tokens_data, 'labels': labels_data, 'current_sent_info': current_sent}
             # Process the sub sentences - we take a long sentence
             # and split it into smaller chunks - and we recursively call the function on this list
             # of smaller chunks - as mentioned before the smaller chunks (sub sentences) will have the
             # same ID as the original sentence
             else:
                 # Store the smaller chunks - say <SENT1> is too long
                 # <PREV CHUNK><SENT1><NEXT CHUNK>
@@ -349,24 +333,23 @@
                 # we include the previous_sent_tokens and next_sent_tokens as the start chunk
                 # and the next chunk in the function call below
                 # <PREV CHUNK><SUB1><NEXT SUB1>, id = x
                 # <PREV SUB2><SUB2><NEXT SUB2>, id = x
                 # <PREV SUB3><SUB3><NEXT CHUNK>, id = x
                 sub_sentences = list()
                 # Prefix the first sentence in these smaller chunks
-                previous_chunk = list(previous_chunk_tokens)
+                previous_sent_tokens = list(previous_sent)
                 # Suffix the last sentence in these smaller chunks
-                next_chunk = list(next_chunk_tokens)
+                next_sent_tokens = list(next_sent)
                 # Get chunks
-                for chunk in self._get_chunks(
-                        current_sentence_tokens, self._max_tokens - (2 * self._default_chunk_size)
-                ):
+                for chunk in SentenceDataset.chunker(sent_toks, self._max_tokens - (2 * self._default_chunk_size)):
                     sub_sentences.append(chunk)
-
                 # Process list of smaller chunks
-                for sub_sent in self.get_sentence_chunks(
+                for sub_sent in self.get_sentences(
                         sub_sentences,
-                        start_chunk=previous_chunk,
-                        end_chunk=next_chunk,
+                        token_text_key,
+                        label_key,
+                        start_chunk=previous_sent_tokens,
+                        end_chunk=next_sent_tokens,
                         sub=True
                 ):
                     yield sub_sent
```

### Comparing `robust_deid-0.3.0/src/robust_deid/sequence_datasets/setup/distribution/dataset_splits.py` & `robust_deid-0.3.1/src/robust_deid/ner_datasets/distribution/dataset_splits.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 
 class DatasetSplits(object):
     """
     Prepare dataset splits - training, validation & testing splits
     Compute ner distributions in the dataset. Based on this we assign
     notes to different splits and at the same time, we keep the distribution of
-    NER types in each split similar. Keep track of the split information - which
-    notes are present in which split. The label distribution in each split, the
-    number of notes in each split.
+    NER types in each split similar. .
+    Keep track of the split information - which notes are present in which split.
+    The label distribution in each split, the number of notes in each split.
     """
 
     def __init__(
             self,
             ner_distribution: NERDistribution,
             train_proportion: int,
             validation_proportion: int,
@@ -33,23 +33,21 @@
         Keep track of the dataset splits and the counts in each split etc.
         These will be used to assign the different notes to different
         splits while keeping the proportion of ner similar in each split.
         Get the maximum number of ner that can be present in the train,
         validation and test split. The total count will be used to
         calculate the current proportion of ner in the split. This can be used
         to keep the proportion of ner types consistent among different splits
-
         Args:
-            ner_distribution (NERDistribution): The NER distribution in the dataset.
-            train_proportion (int): Ratio of train dataset.
-            validation_proportion (int): Ratio of validation dataset.
-            test_proportion (int): Ratio of test dataset.
-            margin (float): Margin by which the label distribution can be exceeded in the split.
+            ner_distribution (NERDistribution): The NER distribution in the dataset
+            train_proportion (int): Ratio of train dataset
+            validation_proportion (int): Ratio of validation dataset
+            test_proportion (int): Ratio of test dataset
+            margin (float): Margin by which the label distribution can be exceeded in the split
         """
-
         self._ner_distribution = ner_distribution
         # Compute the counts of NER types in the entire dataset
         total_distribution = Counter()
         for key, counts in ner_distribution.get_ner_distribution().items():
             for label, count in counts.items():
                 total_distribution[label] += count
         # Compute the percentages of NER types in the entire dataset
@@ -59,39 +57,35 @@
             for ner_type, count in total_distribution.items()
         }
         self._margin = margin
         # The three splits
         self._splits = ['train', 'validation', 'test']
         self._split_weights = None
         self._splits_info = None
-
         # Keep track of the patient_ids that have been processed.
         # Since a patient can have multiple notes and we already know the
         # ner distribution for this patient across all the notes (i.e the ner types
         # and count that appear in all the notes associated with this patient)
         # We also keep all the notes associated with a patient in the same split
         # So we check if adding all the notes associated with this patient will
         # disturb the ner distribution (proportions) as mentioned before.
         self._processed_keys = dict()
-
         # Based on these proportions we compute train_ner_count, validation_ner_count, test_ner_count
         # Say the proportion are 85, 10, 5
         # The train split will have a maximum of 85% of the overall ner, validation will have 10 and test will 5
         # That is if there are total count of all ner is 100, on splitting the datasets
         # the train split will have a total of 85 ner, validation split will have a total of 10 ner and the
         # test split will have a total of 5 ner
         train_ner_count = int(train_proportion * self._total_ner / 100)
         validation_ner_count = int(validation_proportion * self._total_ner / 100)
         test_ner_count = int(test_proportion * self._total_ner / 100)
-
         # So based on this, we check if adding a note keeps the balance in proportion or not
         # If it does not, we check the splits given in the "remain" field of the dict (which is
         # the 2 other splits
         self._split_weights = [train_proportion, validation_proportion, test_proportion]
-
         # Based on the split proportions, ner counts and ner distribution
         # we need to split our dataset into train, validation and test split
         # For each split we try and maintain the same distribution (proportions) between ner types
         # that we computed from the entire dataset (given by - ner_distribution)
         # If the entire dataset had AGE:50%, DATE:30%, LOC:20%, we want the same proportions
         # in each of the train, validation and test splits
         # So based on this, we check if adding a note keeps the balance in proportion or not
@@ -111,63 +105,54 @@
                                       'groups': list(), 'number_of_notes': 0, 'label_dist': Counter()}}
 
     def __set_split(self, split: str) -> NoReturn:
         """
         Set the split that you are currently checking/processing. 
         Based on the split you can perform certain checks and 
         computation for that split.
-
         Args:
-            split (str): The split - train, validation or test.
+            split (str): The split - train, validation or test
         """
-
         self._split = split
 
     def __update_label_dist(self, distribution: Counter) -> NoReturn:
         """
         Once we have determined that a note can be added to the split we need to 
         update the current count of the ner types in the split. So we pass the ner counts 
         in the note that will be updated and update the counts of the ner types in the split.
-
         Args:
-            distribution (Counter): Contains the ner type and it's counts (distribution).
+            distribution (Counter): Contains the ner type and it's counts (distribution)
         """
-
         self._splits_info[self._split]['label_dist'].update(distribution)
 
     def __update_groups(self, note_group_key: str) -> NoReturn:
         """
         Once we have determined that a note can be added to the split, we append
         to a list some distinct element of the note (e.g note_id). This list will
         contain the note_ids of the notes that belong to this split.
-
         Args:
-            note_group_key (str): Contains the note metadata - e.g note_id, institute etc.
+            note_group_key (str): Contains the note metadata - e.g note_id, institute etc
         """
-
         self._processed_keys[note_group_key] = self._split
         self._splits_info[self._split]['groups'].append(note_group_key)
 
     def __check_split(self, distribution: Counter) -> bool:
         """
         This function is used to check the resulting ner distribution in the split on adding this
         note to the split. We check how the proportion of ner changes if this note is added to
         the split. If the proportion exceeds the desired proportion then we return false
         to indicate that adding this note will upset the ner distribution across splits, so we should
         instead check adding this note to another split. If it does not update the balance then we return
         True, which means we can add this note to this split. The desired proportion of ner is passed
         in the percentages argument - where we have the desired proportion for each ner type.
-
         Args:
-            distribution (Counter): Contains the mapping between ner type and count.
-
+            distribution (Counter): Contains the mapping between ner type and count
         Returns:
-            (bool): True if the note can be added to the split, false otherwise.
+            (bool): True if the note can be added to the split, false otherwise
         """
-
         # Get the current ner types and counts in the split
         split_label_dist = self._splits_info[self._split]['label_dist']
         # Get the max ner count that can be present in the split
         # This will be used to compute the ner proportions in the split
         split_total = self._splits_info[self._split]['total']
         # Check if the proportion of the split picked in zero
         # and return False because we cant add any note to this split
@@ -184,28 +169,24 @@
 
     def get_split(self, key: str) -> str:
         """
         Assign a split to the note - based on the distribution of ner types in the note
         and the distribution of ner types in the split. Essentially assign a note to a split
         such that the distribution of ner types in each split is similar, once all notes have
         been assigned to their respective splits.
-
         Args:
             key (str): The note id or patient id of the note (some grouping key)
-
         Returns:
             (str): The split
         """
-
         current_splits = self._splits
         current_weights = self._split_weights
         distribution = self._ner_distribution.get_group_distribution(key=key)
         if self._processed_keys.get(key, False):
             return self._processed_keys[key]
-
         while True:
             # Pick and set the split
             check_split = random.choices(current_splits, current_weights)[0]
             self.__set_split(check_split)
             # Get the ner distribution for this particular patient (across all the notes associated
             # with this patient) and check if the notes can be added to this split.
             # The margin of error for the ner proportions. As we said above we try and keep the proportions
```

### Comparing `robust_deid-0.3.0/src/robust_deid/sequence_datasets/setup/distribution/ner_distribution.py` & `robust_deid-0.3.1/src/robust_deid/ner_datasets/distribution/ner_distribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,53 +9,46 @@
     the distribution when spans related to that key is passed
     """
 
     def __init__(self) -> NoReturn:
         """
         Initialize the NER type - count mapping
         """
-
         # Counter the captures the ner types and counts per patient/note_id in the dataset
         # Depending on what we set the group_key as. Basically gather counts with respect
         # to some grouping of the notes
         # E.g - {{PATIENT 1: {AGE: 99, DATE: 55, ...}, {PATIENT 2: {AGE: 5, DATE: 9, ...} ... }
         self._ner_distribution = defaultdict(Counter)
 
     def update_distribution(self, spans: Sequence[Mapping[str, str]], key: str) -> NoReturn:
         """
         Update the distribution of ner types for the given key
-
         Args:
             spans (Sequence[Mapping[str, str]]): The list of spans in the note
             key (str): The note id or patient id of the note (some grouping)
         """
-
         # Go through the spans in the note and compute the ner distribution
         # Compute both the overall ner distribution and ner distribution per
         # patient (i.e the ner types in all the notes associated with the patient)
         if not self._ner_distribution.get(key, False):
             self._ner_distribution[key] = Counter()
         for span in spans:
             self._ner_distribution[key][span['label']] += 1
 
     def get_ner_distribution(self) -> defaultdict:
         """
         Return overall ner distribution. The NER type distribution for every key.
-
         Returns:
             ner_distribution (defaultdict(Counter)): Overall NER type distribution for all keys
         """
-
         return self._ner_distribution
 
     def get_group_distribution(self, key: str) -> Counter:
         """
         Return the NER type distribution for the given key
-
         Returns:
             (Counter): ner distribution w.r.t some grouping (key)
         """
-
         if key in self._ner_distribution.keys():
             return self._ner_distribution[key]
         else:
             raise ValueError('Key not found')
```

### Comparing `robust_deid-0.3.0/src/robust_deid/sequence_datasets/setup/distribution/print_distribution.py` & `robust_deid-0.3.1/src/robust_deid/ner_datasets/distribution/print_distribution.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,32 +8,28 @@
     """
     This class is used to print the distribution of NER types
     """
 
     def __init__(self, ner_distribution: NERDistribution, key_counts: Counter) -> NoReturn:
         """
         Initialize
-
         Args:
             ner_distribution (NERDistribution): NERDistribution object that keeps track of the NER type distributions
             key_counts (Counter): Number of keys/groups (e.g note_ids, patient ids etc)
         """
-
         self._ner_distribution = ner_distribution
         self._key_counts = key_counts
 
     def split_distribution(self, split: str, split_info: Sequence[str]) -> NoReturn:
         """
         Print NER type distribution
-
         Args:
             split (str): The dataset split
             split_info (Sequence[str]): The keys belonging to that split
         """
-
         split_distribution = Counter()
         number_of_notes = 0
         for key in split_info:
             number_of_notes += self._key_counts[key]
             split_distribution.update(self._ner_distribution.get_group_distribution(key))
         total_ner = sum(split_distribution.values())
         percentages = {ner_type: float(count) / total_ner * 100 if total_ner else 0
```

