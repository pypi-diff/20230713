# Comparing `tmp/graph-part-1.0.1.tar.gz` & `tmp/graph-part-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph-part-1.0.1.tar", last modified: Sun Jul  2 18:28:49 2023, max compression
+gzip compressed data, was "graph-part-1.0.2.tar", last modified: Thu Jul 13 11:32:53 2023, max compression
```

## Comparing `graph-part-1.0.1.tar` & `graph-part-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:28:49.178811 graph-part-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-02 18:28:38.000000 graph-part-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17029 2023-07-02 18:28:49.178811 graph-part-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16735 2023-07-02 18:28:38.000000 graph-part-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:28:49.178811 graph-part-1.0.1/graph_part/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13608 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13160 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    30192 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/graph_part.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/mmseqs_fake_prefilter.sh
--rw-r--r--   0 runner    (1001) docker     (123)    17171 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/mmseqs_needle_combined_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/mmseqs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/molecules.py
--rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/needle_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/precomputed_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/train_val_test_split.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:28:49.178811 graph-part-1.0.1/graph_part.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17029 2023-07-02 18:28:49.000000 graph-part-1.0.1/graph_part.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-02 18:28:49.000000 graph-part-1.0.1/graph_part.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 18:28:49.000000 graph-part-1.0.1/graph_part.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-02 18:28:49.000000 graph-part-1.0.1/graph_part.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-02 18:28:49.000000 graph-part-1.0.1/graph_part.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 18:28:49.000000 graph-part-1.0.1/graph_part.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 18:28:49.178811 graph-part-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-02 18:28:38.000000 graph-part-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:32:53.294897 graph-part-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-13 11:32:35.000000 graph-part-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17163 2023-07-13 11:32:53.294897 graph-part-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16869 2023-07-13 11:32:35.000000 graph-part-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:32:53.294897 graph-part-1.0.2/graph_part/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-13 11:32:36.000000 graph-part-1.0.2/graph_part/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:32:36.000000 graph-part-1.0.2/graph_part/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-07-13 11:32:36.000000 graph-part-1.0.2/graph_part/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12523 2023-07-13 11:32:36.000000 graph-part-1.0.2/graph_part/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28365 2023-07-13 11:32:36.000000 graph-part-1.0.2/graph_part/graph_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-13 11:32:36.000000 graph-part-1.0.2/graph_part/mmseqs_fake_prefilter.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    17171 2023-07-13 11:32:36.000000 graph-part-1.0.2/graph_part/mmseqs_needle_combined_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-13 11:32:36.000000 graph-part-1.0.2/graph_part/mmseqs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-07-13 11:32:36.000000 graph-part-1.0.2/graph_part/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-07-13 11:32:36.000000 graph-part-1.0.2/graph_part/needle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-13 11:32:36.000000 graph-part-1.0.2/graph_part/precomputed_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-07-13 11:32:36.000000 graph-part-1.0.2/graph_part/train_val_test_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-13 11:32:36.000000 graph-part-1.0.2/graph_part/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:32:53.294897 graph-part-1.0.2/graph_part.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17163 2023-07-13 11:32:53.000000 graph-part-1.0.2/graph_part.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-13 11:32:53.000000 graph-part-1.0.2/graph_part.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:32:53.000000 graph-part-1.0.2/graph_part.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-13 11:32:53.000000 graph-part-1.0.2/graph_part.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-13 11:32:53.000000 graph-part-1.0.2/graph_part.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 11:32:53.000000 graph-part-1.0.2/graph_part.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 11:32:53.294897 graph-part-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-13 11:32:36.000000 graph-part-1.0.2/setup.py
```

### Comparing `graph-part-1.0.1/LICENSE` & `graph-part-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `graph-part-1.0.1/PKG-INFO` & `graph-part-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graph-part
-Version: 1.0.1
+Version: 1.0.2
 Summary: Graph-based partitioning of biological sequence data
 Home-page: https://github.com/graph-part/graph-part
 Author: F. Teufel and M.H. Gislason
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -99,17 +99,18 @@
 graphpart ALIGNMENT_MODE -ff FASTAFILE.fasta -th 0.3
 ```
 
 ### Supported aligners
 
 Alignment mode  | Description
 ----------------|----------------------
-`needle`        | Use EMBOSS needleall to compute exact pairwise global Needleman-Wunsch identities for all sequences.
-`mmseqs2`       | Use MMseqs2 to compute fast identities from local alignments. Use with caution for nucleotides, as there it cannot be guaranteed that MMseqs2 computes all pairwise alignments.
-`precomputed`   | Use a list of precomputed identities or other similarity/distance metrics.
+[`needle`](#needle)        | Use EMBOSS needleall to compute exact pairwise global Needleman-Wunsch (NW) identities for all sequences.
+[`mmseqs2`](#mmseqs2)       | Use MMseqs2 to compute fast identities from local alignments. Use with caution for nucleotides, as there it cannot be guaranteed that MMseqs2 computes all pairwise alignments.
+[`precomputed`](#precomputed)   | Use a list of precomputed identities or other similarity/distance metrics.
+[`mmseqs2needle`](#mmseqs2needle) | Uses MMseqs2 to compute fast identities, followed by recomputation of NW identities of all identities between the separation threshold and an user-defined lower threshold.
 
 ### Arguments
 
 #### Shared
 
 Long                    | Short | Description
 ------------------------|-------|------------
@@ -118,31 +119,30 @@
 `--threshold`           |`-th`  | The desired partitioning threshold, should be within the bounds defined by the metric.
 `--partitions`          |`-pa`  | Number of partitions to generate. Defaults to 5.
 `--transformation`      |`-tf`  | Transformation to apply to the similarity/distance metric. GraphPart operates on distances, therefore similarity metrics need to be transformed. Can be any of `one-minus`, `inverse`, `square`, `log`, `None`. See the [source](graph_part/transformations.py) for definitions. As an example, when operating with sequence identities ranging from 0 to 1, the transformation `one-minus` yields corresponding distances. Defaults to `one-minus`.
 `--priority-name`       |`-pn`  | The name of the retention priority in the meta file. Is either `=0` or `=1`. If specified, the algorithm first tries to reach the treshold by removing/moving low-priority (`0`) samples before proceeding to `1` samples.
 `--labels-name`         |`-ln`  | The name of the label in the meta file. Used for balancing partitions.
 `--initialization-mode` |`-im`  | Use either slow or fast restricted nearest neighbor linkage or no initialization. Can be any of `slow-nn`, `fast-nn`, `simple`. Defaults to `slow-nn`.
 `--no-moving`           |`-nm`  | By default, the removing procedure tries to relocate sequences to another partition if it finds more within-threshold neighbours in any. This flag disallows moving. In high-redundancy datasets, moving can lead to imbalanced partitions and should be disabled.
-`--remove-same`         |`-rs`  | This here is the inverse of removal_type (has default True) DO @Magnus can you describe it in one sentence?
 `--save-checkpoint-path`|`-sc`  | Optional path to save the computed identities above the chosen threshold as an edge list. Can be used to quickstart runs in the `precomputed` mode. Defaults to `None` with no file saved.
 `--test-ratio`          | `-te` | Make a train-val-test split instead of partitions for cross-validation. Overrides `--partitions` when specified. Defaults to 0. Needs to be a multiple of 0.05.
 `--val-ratio`           | `-va` |Make a train-val-test split instead of partitions for cross-validation. Overrides `--partitions` when specified. Defaults to 0. Needs to be a multiple of 0.05.
 
 #### needle
 
 Long                    | Short | Description
 ------------------------|-------|------------
 `--denominator`         |`-dn`  | Denominator to use for percent sequence identity computation. The number of perfect matching positions is divided by the result of this operation. Can be any of `shortest`, `longest`, `mean`, `full`, `no_gaps`. The first three options are computed from the original lengths of the aligned sequences. `full` refers to the full length of the alignment, including gaps, and is the default. `no_gaps` subtracts gaps from the full alignment length.
 `--threads`             |`-nt`  | The number of threads to run in parallel. If `-1`, will use all available resources. Defaults to 1.
 `--chunks`              |`-nc`  | The number of chunks into which to split the fasta file for multithreaded alignment. Defaults to 10.
-`--parallel-mode`       |`-pm`  | The Python parallelization strategy to use. `multithread` or `multiprocess`. Multiprocessing is potentially faster (especially for short sequences), but increases memory usage.
+`--parallel-mode`       |`-pm`  | The Python parallelization strategy to use. `multithread` or `multiprocess`. Multiprocessing is potentially faster (especially for short sequences), but increases memory usage. Defaults to `multithread`
 `--nucleotide`          |`-nu`  | Use this flag if the input contains nucleotide sequences. By default, assumes proteins.
 `--triangular`          |`-tr`  | Only compute triangular of the full distance matrix. Twice as fast, but can yield slightly different results if an alignment has two different solutions with the same score, but different identities. In some cases, a pairwise identity can be slightly above the threshold in one solution, and slightly below in another (e.g A:B = 29.8%, B:A = 30.4%).
 `--gapopen`             |`-gapopen`     | [10.0 for any sequence] The gap open penalty is the score taken away when a gap is created. The best value depends on the choice of comparison matrix. The default value assumes you are using the EBLOSUM62 matrix. (Floating point number from 1.0 to 100.0)
-`--gapextend`           |`-gapextend`   | [0.5 for any sequence] The gap extension penalty is added to the standard gap penalty for each base or residue in the gap. This is how long gaps are penalized. Usually you will expect a few long gaps rather than many short gaps, so the gap extension penalty should be lower than the gap penalty. An exception is where one or both sequences are single reads with possible sequencing errors in which case you would expect many single base gaps. You can get this result by setting the gap open penalty to zero (or very low) and using the gap extension penalty to control gap scoring. (Floating point number from 0.0 to 10.0)
+`--gapextend`           |`-gapextend`   | [0.5 for any sequence] The gap extension penalty is added to the standard gap penalty for each base or residue in the gap. This is how long gaps are penalized. Usually you will expect a few long gaps rather than many short gaps, so the gap extension penalty should be lower than the gap penalty. An exception is where one or both sequences are single reads with possible sequencing errors in which case you would expect many single base gaps. You can get this result by setting the gap open penalty to a very low value and using the gap extension penalty to control gap scoring. (Floating point number from 0.0 to 10.0)
 `--endextend`           |`-endextend`   | [0.5 for any sequence] The end gap extension, penalty is added to the end gap penalty for each base or residue in the end gap. This is how long end gaps are penalized. (Floating point number from 0.0 to 10.0)
 `--endweight`           |`-endweight`   | Flag. Apply end gap penalties.
 `--endopen`             |`-endopen`     | [10.0 for any sequence] The end gap open penalty is the score taken away when an end gap is created. The best value depends on the choice of comparison matrix. The default value assumes you are using the EBLOSUM62 matrix for protein sequences. (Floating point number from 1.0 to 100.0)
 `--matrix`              |`-datafile`    | This is the scoring matrix file used when comparing sequences. By default it is the file 'EBLOSUM62'. These files are found in the 'data' directory of the EMBOSS installation.
 
 
 #### mmseqs2
```

### Comparing `graph-part-1.0.1/README.md` & `graph-part-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -89,17 +89,18 @@
 graphpart ALIGNMENT_MODE -ff FASTAFILE.fasta -th 0.3
 ```
 
 ### Supported aligners
 
 Alignment mode  | Description
 ----------------|----------------------
-`needle`        | Use EMBOSS needleall to compute exact pairwise global Needleman-Wunsch identities for all sequences.
-`mmseqs2`       | Use MMseqs2 to compute fast identities from local alignments. Use with caution for nucleotides, as there it cannot be guaranteed that MMseqs2 computes all pairwise alignments.
-`precomputed`   | Use a list of precomputed identities or other similarity/distance metrics.
+[`needle`](#needle)        | Use EMBOSS needleall to compute exact pairwise global Needleman-Wunsch (NW) identities for all sequences.
+[`mmseqs2`](#mmseqs2)       | Use MMseqs2 to compute fast identities from local alignments. Use with caution for nucleotides, as there it cannot be guaranteed that MMseqs2 computes all pairwise alignments.
+[`precomputed`](#precomputed)   | Use a list of precomputed identities or other similarity/distance metrics.
+[`mmseqs2needle`](#mmseqs2needle) | Uses MMseqs2 to compute fast identities, followed by recomputation of NW identities of all identities between the separation threshold and an user-defined lower threshold.
 
 ### Arguments
 
 #### Shared
 
 Long                    | Short | Description
 ------------------------|-------|------------
@@ -108,31 +109,30 @@
 `--threshold`           |`-th`  | The desired partitioning threshold, should be within the bounds defined by the metric.
 `--partitions`          |`-pa`  | Number of partitions to generate. Defaults to 5.
 `--transformation`      |`-tf`  | Transformation to apply to the similarity/distance metric. GraphPart operates on distances, therefore similarity metrics need to be transformed. Can be any of `one-minus`, `inverse`, `square`, `log`, `None`. See the [source](graph_part/transformations.py) for definitions. As an example, when operating with sequence identities ranging from 0 to 1, the transformation `one-minus` yields corresponding distances. Defaults to `one-minus`.
 `--priority-name`       |`-pn`  | The name of the retention priority in the meta file. Is either `=0` or `=1`. If specified, the algorithm first tries to reach the treshold by removing/moving low-priority (`0`) samples before proceeding to `1` samples.
 `--labels-name`         |`-ln`  | The name of the label in the meta file. Used for balancing partitions.
 `--initialization-mode` |`-im`  | Use either slow or fast restricted nearest neighbor linkage or no initialization. Can be any of `slow-nn`, `fast-nn`, `simple`. Defaults to `slow-nn`.
 `--no-moving`           |`-nm`  | By default, the removing procedure tries to relocate sequences to another partition if it finds more within-threshold neighbours in any. This flag disallows moving. In high-redundancy datasets, moving can lead to imbalanced partitions and should be disabled.
-`--remove-same`         |`-rs`  | This here is the inverse of removal_type (has default True) DO @Magnus can you describe it in one sentence?
 `--save-checkpoint-path`|`-sc`  | Optional path to save the computed identities above the chosen threshold as an edge list. Can be used to quickstart runs in the `precomputed` mode. Defaults to `None` with no file saved.
 `--test-ratio`          | `-te` | Make a train-val-test split instead of partitions for cross-validation. Overrides `--partitions` when specified. Defaults to 0. Needs to be a multiple of 0.05.
 `--val-ratio`           | `-va` |Make a train-val-test split instead of partitions for cross-validation. Overrides `--partitions` when specified. Defaults to 0. Needs to be a multiple of 0.05.
 
 #### needle
 
 Long                    | Short | Description
 ------------------------|-------|------------
 `--denominator`         |`-dn`  | Denominator to use for percent sequence identity computation. The number of perfect matching positions is divided by the result of this operation. Can be any of `shortest`, `longest`, `mean`, `full`, `no_gaps`. The first three options are computed from the original lengths of the aligned sequences. `full` refers to the full length of the alignment, including gaps, and is the default. `no_gaps` subtracts gaps from the full alignment length.
 `--threads`             |`-nt`  | The number of threads to run in parallel. If `-1`, will use all available resources. Defaults to 1.
 `--chunks`              |`-nc`  | The number of chunks into which to split the fasta file for multithreaded alignment. Defaults to 10.
-`--parallel-mode`       |`-pm`  | The Python parallelization strategy to use. `multithread` or `multiprocess`. Multiprocessing is potentially faster (especially for short sequences), but increases memory usage.
+`--parallel-mode`       |`-pm`  | The Python parallelization strategy to use. `multithread` or `multiprocess`. Multiprocessing is potentially faster (especially for short sequences), but increases memory usage. Defaults to `multithread`
 `--nucleotide`          |`-nu`  | Use this flag if the input contains nucleotide sequences. By default, assumes proteins.
 `--triangular`          |`-tr`  | Only compute triangular of the full distance matrix. Twice as fast, but can yield slightly different results if an alignment has two different solutions with the same score, but different identities. In some cases, a pairwise identity can be slightly above the threshold in one solution, and slightly below in another (e.g A:B = 29.8%, B:A = 30.4%).
 `--gapopen`             |`-gapopen`     | [10.0 for any sequence] The gap open penalty is the score taken away when a gap is created. The best value depends on the choice of comparison matrix. The default value assumes you are using the EBLOSUM62 matrix. (Floating point number from 1.0 to 100.0)
-`--gapextend`           |`-gapextend`   | [0.5 for any sequence] The gap extension penalty is added to the standard gap penalty for each base or residue in the gap. This is how long gaps are penalized. Usually you will expect a few long gaps rather than many short gaps, so the gap extension penalty should be lower than the gap penalty. An exception is where one or both sequences are single reads with possible sequencing errors in which case you would expect many single base gaps. You can get this result by setting the gap open penalty to zero (or very low) and using the gap extension penalty to control gap scoring. (Floating point number from 0.0 to 10.0)
+`--gapextend`           |`-gapextend`   | [0.5 for any sequence] The gap extension penalty is added to the standard gap penalty for each base or residue in the gap. This is how long gaps are penalized. Usually you will expect a few long gaps rather than many short gaps, so the gap extension penalty should be lower than the gap penalty. An exception is where one or both sequences are single reads with possible sequencing errors in which case you would expect many single base gaps. You can get this result by setting the gap open penalty to a very low value and using the gap extension penalty to control gap scoring. (Floating point number from 0.0 to 10.0)
 `--endextend`           |`-endextend`   | [0.5 for any sequence] The end gap extension, penalty is added to the end gap penalty for each base or residue in the end gap. This is how long end gaps are penalized. (Floating point number from 0.0 to 10.0)
 `--endweight`           |`-endweight`   | Flag. Apply end gap penalties.
 `--endopen`             |`-endopen`     | [10.0 for any sequence] The end gap open penalty is the score taken away when an end gap is created. The best value depends on the choice of comparison matrix. The default value assumes you are using the EBLOSUM62 matrix for protein sequences. (Floating point number from 1.0 to 100.0)
 `--matrix`              |`-datafile`    | This is the scoring matrix file used when comparing sequences. By default it is the file 'EBLOSUM62'. These files are found in the 'data' directory of the EMBOSS installation.
 
 
 #### mmseqs2
```

### Comparing `graph-part-1.0.1/graph_part/api.py` & `graph-part-1.0.2/graph_part/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     partition_assignment_df = run_partitioning(config, write_output_file=False, write_json_report=False, verbose=False)
     os.remove(config['fasta_file'])
 
     # 4. Make output lists.
     partition_assignment_df = partition_assignment_df.reset_index()
 
     # 'AC' will be type string. But potentially the original 'AC' were ints.
-    if type(next(sequences.keys())) == int:
+    if type(list(sequences.keys())[0]) == int:
         try:
             partition_assignment_df['AC'] = partition_assignment_df['AC'].astype(int)
         except:
             pass
 
     outs = []
     # iterate over all created folds and add to the output list.
@@ -313,15 +313,15 @@
     partition_assignment_df = run_partitioning(config, write_output_file=False, write_json_report=False, verbose=False)
     os.remove(config['fasta_file'])
 
     # 4. Make output lists.
     partition_assignment_df = partition_assignment_df.reset_index()
 
     # 'AC' will be type string. But potentially the original 'AC' were ints.
-    if type(next(sequences.keys())) == int:
+    if type(list(sequences.keys())[0]) == int:
         try:
             partition_assignment_df['AC'] = partition_assignment_df['AC'].astype(int)
         except:
             pass
 
     outs = []
     # iterate over all created folds and add to the output list.
```

### Comparing `graph-part-1.0.1/graph_part/cli.py` & `graph-part-1.0.2/graph_part/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,21 +52,14 @@
                         default='slow-nn', 
                         choices=['slow-nn', 'fast-nn', 'simple'],
                         )
     core_parser.add_argument("-nm","--no-moving",action='store_true', help='''Disallows the removing procedure to relocate
                                                                             entities if it finds more within threshold 
                                                                             neighbours in another partition.'''
                         )
-    core_parser.add_argument("-rs","--remove-same",action='store_true', help='''Activate if you also want to remove
-                                      based on the within threshold interconnectivity
-                                      between within threshold neighbours in other
-                                      partitions and within threshold neighbours 
-                                      in the same partition. The default removes based on the number
-                                      of within threshold neighbours in other partitions.'''
-                        )
     
     # train-val-test splits.
     core_parser.add_argument("-te","--test-ratio",type=float, default=0.0, help='The fraction of the data to use for testing. Incompatible with `partitions`.')
     core_parser.add_argument("-va","--val-ratio",type=float, default=0.0,help='The fraction of the data to use for validation. Incompatible with `partitions`.')
     
     #checkpointing
     core_parser.add_argument('--save-checkpoint-path', '-sc', type=str, default=None, help='''Path to save the computed similarities above the threshold. 
@@ -195,13 +188,12 @@
 
 def main():
 
     
     args = get_args()
     config = vars(args)
     config['allow_moving'] = not args.no_moving
-    config['removal_type'] = not args.remove_same
 
     if 'matrix' in config and config['matrix'] == 'EBLOSUM62' and config['nucleotide']:
         config['matrix'] = 'EDNAFULL'
 
     run_partitioning(config, write_output_file=True, write_json_report=True)
```

### Comparing `graph-part-1.0.1/graph_part/graph_part.py` & `graph-part-1.0.2/graph_part/graph_part.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import time
 
 from tqdm import tqdm
 
 from .transformations import TRANSFORMATIONS
 from .train_val_test_split import train_val_test_split
 
-#TODO update new arg names here
 """
 This program partitions an entity set according to a single pairwise distance metric
 and some desired threshold the partitions should fullfill.
 The program seeks maximum distance between partitions. If the metric and desired 
 threshold imply minimization you should designate the ('-tf', '--transformation')
 parameter and specify either the one-minus or inverse transformation. The program 
 converts the designated threshold the same way as the metric.
@@ -29,43 +28,19 @@
 The entity/meta file can contain a priority designator and a label designator 
 For example:
 >entity_identifier1|exp=1|class=label1
 >entity_identifier2|exp=0|class=label2
 the priority name and label name should be designated using the appropriate parameters.
 In this case you would specify the priority name -pn experimental and the label name 
 -ln class
-For the full list of parameters, run graph_part.py --help
-Example usage:
-python graph_part.py 
-    -ff ../../data/sequences/raw_data.fasta 
-    -ef ../../data/edgefiles/ggs_default_gpia2_edges 
-    -mc 2
-    -th 0.31 
-    -pa 5 
-    -tf one-minus 
-    -pn experimental
-    -ln positive 
-    -of gpia_gps_part_identity2.csv
+    
 Author(s): Magnús Halldór Gíslason.
+           Felix Teufel
            Developed in close collaboration with 
            José Juan Almagro Armenteros and Henrik Nielsen.
-For bug reporting contact mhgislason@gmail.com
-(CC BY-NC 4.0) 
-You are free to:
-Share — copy and redistribute the material in any medium or format
-Adapt — remix, transform, and build upon the material
-Under the following terms:
-Attribution — You must give appropriate credit, provide a link to the license, and indicate if changes were made. 
-You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
-NonCommercial — You may not use the material for commercial purposes.
-No additional restrictions — You may not apply legal terms or technological measures that legally restrict others 
-from doing anything the license permits.
-see:
-https://creativecommons.org/licenses/by-nc/4.0/
-https://creativecommons.org/licenses/by-nc/4.0/legalcode
 """
 
 
 def process_csv(line: str) -> Tuple[str, dict]:
     """ NOT IMPLEMENTED """
     raise NotImplementedError('Graph-Part does not support starting from .csv yet.')
     yield None, None
@@ -290,22 +265,21 @@
     partitioning = partition_assignment(clusters, labels, nr_of_parts, len(np.unique(labels)))
     for ind, p in enumerate(partitioning):
         attr = part_graph.nodes[acs[ind]]
         attr['cluster'] = p
         nx.set_node_attributes(part_graph,{acs[ind]:attr})
 
 
-def remover(full_graph: nx.classes.graph.Graph, 
-            part_graph: nx.classes.graph.Graph, 
-            threshold:float, 
-            json_dict: Dict[str, Any],
-            move_to_most_neighbourly:bool = True, 
-            ignore_priority:bool = True,
-            simplistic_removal:bool = True,
-            verbose: bool = True):
+def remover( full_graph: nx.classes.graph.Graph, 
+             part_graph: nx.classes.graph.Graph, 
+             threshold:float, 
+             json_dict: Dict[str, Any],
+             move_to_most_neighbourly:bool = True, 
+             ignore_priority:bool = True,
+             verbose: bool = True ):
 
     if ignore_priority:
         json_dict['removal_step_1'] = {}
         dict_key = 'removal_step_1'
     else:
         json_dict['removal_step_2'] = {}
         dict_key = 'removal_step_2'
@@ -317,15 +291,14 @@
         between_connectivity = {}
         min_oc_wth= 1
         number_moved = 0
         for n,d in full_graph.nodes(data=True):
             neighbours = nx.neighbors(full_graph,n)
             neighbour_clusters = Counter((part_graph.nodes[nb]['cluster'] for nb in nx.neighbors(full_graph,n) if full_graph[n][nb]['metric'] < threshold))
             cluster = part_graph.nodes[n]['cluster']
-            nb_sc_wth = []
             nb_oc_wth = []
             
             ## FIRST MOVE NODE TO CLUSTER WITH MOST NEIGHBOURS
             if move_to_most_neighbourly:
                 if len(neighbour_clusters) > 0:
                     most_neighbourly_cluster = max(neighbour_clusters.items(), key=lambda x:x[1])[0]
                     if most_neighbourly_cluster != cluster:
@@ -334,27 +307,19 @@
             
             if ignore_priority and full_graph.nodes[n]['priority']:
                 between_connectivity[n] = 0
                 continue
 
             for neighbour in neighbours:
                 nb_cluster = part_graph.nodes[neighbour]['cluster']
-                if nb_cluster == cluster and full_graph[n][neighbour]['metric'] < threshold and not simplistic_removal:
-                    ## The more complex removal criterion. This was worse for GPI anchors. Haven't checked for Subnuclear
-                    nb_sc_wth.append(full_graph[n][neighbour]['metric'])
-                elif nb_cluster != cluster and full_graph[n][neighbour]['metric'] < threshold:
+                if nb_cluster != cluster and full_graph[n][neighbour]['metric'] < threshold:
                     min_oc_wth = min(min_oc_wth, full_graph[n][neighbour]['metric'])
                     nb_oc_wth.append(full_graph[n][neighbour]['metric'])
 
-            ## The more complex additional connectivity criterion, will be empty with simple_removal == True        
-            distances = [x for x in (sum(x_) for x_ in product(nb_sc_wth, nb_oc_wth)) if x >= threshold] 
-            
-            distances += nb_oc_wth
-
-            between_connectivity[n] = len(distances)
+            between_connectivity[n] = len(nb_oc_wth)
             
         nx.set_node_attributes(full_graph, between_connectivity, 'between_connectivity')
         bc_sum = np.sum(np.fromiter((d['between_connectivity'] for n,d in full_graph.nodes(data=True)),int))
         bc_count = np.sum(np.fromiter((1 for n,d in full_graph.nodes(data=True) if d['between_connectivity'] > 0),int))
 
         removing_round += 1
         number_to_remove = int(bc_count*np.log10(removing_round)/100)+1 # int(bc_count*0.01)+1
@@ -569,19 +534,19 @@
     json_dict['score_pre_removal'] = score_partitioning(result[range(config['partitions'])])
 
     
     ## Check if we need to remove any
     if removal_needed(part_graph, full_graph, threshold):     
         print('Need to remove! Currently have this many samples:', full_graph.number_of_nodes())
 
-        remover(full_graph, part_graph, threshold, json_dict, config['allow_moving'], True, config['removal_type'], verbose=verbose)    
+        remover(full_graph, part_graph, threshold, json_dict, config['allow_moving'], True, verbose=verbose)    
 
     if removal_needed(part_graph, full_graph, threshold):   
         print('Need to remove priority! Currently have this many samples:', full_graph.number_of_nodes())
-        remover(full_graph, part_graph, threshold, json_dict, config['allow_moving'], False, config['removal_type'], verbose=verbose)    
+        remover(full_graph, part_graph, threshold, json_dict, config['allow_moving'], False, verbose=verbose)    
 
     print('After removal we have this many samples:', full_graph.number_of_nodes())
 
 
     df, result = display_results(part_graph, full_graph, labels, config['partitions'], verbose=verbose)
 
     json_dict['partitioning_after_removal'] = result.to_json()
```

### Comparing `graph-part-1.0.1/graph_part/mmseqs_fake_prefilter.sh` & `graph-part-1.0.2/graph_part/mmseqs_fake_prefilter.sh`

 * *Files identical despite different names*

### Comparing `graph-part-1.0.1/graph_part/mmseqs_needle_combined_utils.py` & `graph-part-1.0.2/graph_part/mmseqs_needle_combined_utils.py`

 * *Files identical despite different names*

### Comparing `graph-part-1.0.1/graph_part/mmseqs_utils.py` & `graph-part-1.0.2/graph_part/mmseqs_utils.py`

 * *Files identical despite different names*

### Comparing `graph-part-1.0.1/graph_part/molecules.py` & `graph-part-1.0.2/graph_part/molecules.py`

 * *Files identical despite different names*

### Comparing `graph-part-1.0.1/graph_part/needle_utils.py` & `graph-part-1.0.2/graph_part/needle_utils.py`

 * *Files identical despite different names*

### Comparing `graph-part-1.0.1/graph_part/precomputed_utils.py` & `graph-part-1.0.2/graph_part/precomputed_utils.py`

 * *Files identical despite different names*

### Comparing `graph-part-1.0.1/graph_part/train_val_test_split.py` & `graph-part-1.0.2/graph_part/train_val_test_split.py`

 * *Files identical despite different names*

### Comparing `graph-part-1.0.1/graph_part/transformations.py` & `graph-part-1.0.2/graph_part/transformations.py`

 * *Files identical despite different names*

### Comparing `graph-part-1.0.1/graph_part.egg-info/PKG-INFO` & `graph-part-1.0.2/graph_part.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graph-part
-Version: 1.0.1
+Version: 1.0.2
 Summary: Graph-based partitioning of biological sequence data
 Home-page: https://github.com/graph-part/graph-part
 Author: F. Teufel and M.H. Gislason
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -99,17 +99,18 @@
 graphpart ALIGNMENT_MODE -ff FASTAFILE.fasta -th 0.3
 ```
 
 ### Supported aligners
 
 Alignment mode  | Description
 ----------------|----------------------
-`needle`        | Use EMBOSS needleall to compute exact pairwise global Needleman-Wunsch identities for all sequences.
-`mmseqs2`       | Use MMseqs2 to compute fast identities from local alignments. Use with caution for nucleotides, as there it cannot be guaranteed that MMseqs2 computes all pairwise alignments.
-`precomputed`   | Use a list of precomputed identities or other similarity/distance metrics.
+[`needle`](#needle)        | Use EMBOSS needleall to compute exact pairwise global Needleman-Wunsch (NW) identities for all sequences.
+[`mmseqs2`](#mmseqs2)       | Use MMseqs2 to compute fast identities from local alignments. Use with caution for nucleotides, as there it cannot be guaranteed that MMseqs2 computes all pairwise alignments.
+[`precomputed`](#precomputed)   | Use a list of precomputed identities or other similarity/distance metrics.
+[`mmseqs2needle`](#mmseqs2needle) | Uses MMseqs2 to compute fast identities, followed by recomputation of NW identities of all identities between the separation threshold and an user-defined lower threshold.
 
 ### Arguments
 
 #### Shared
 
 Long                    | Short | Description
 ------------------------|-------|------------
@@ -118,31 +119,30 @@
 `--threshold`           |`-th`  | The desired partitioning threshold, should be within the bounds defined by the metric.
 `--partitions`          |`-pa`  | Number of partitions to generate. Defaults to 5.
 `--transformation`      |`-tf`  | Transformation to apply to the similarity/distance metric. GraphPart operates on distances, therefore similarity metrics need to be transformed. Can be any of `one-minus`, `inverse`, `square`, `log`, `None`. See the [source](graph_part/transformations.py) for definitions. As an example, when operating with sequence identities ranging from 0 to 1, the transformation `one-minus` yields corresponding distances. Defaults to `one-minus`.
 `--priority-name`       |`-pn`  | The name of the retention priority in the meta file. Is either `=0` or `=1`. If specified, the algorithm first tries to reach the treshold by removing/moving low-priority (`0`) samples before proceeding to `1` samples.
 `--labels-name`         |`-ln`  | The name of the label in the meta file. Used for balancing partitions.
 `--initialization-mode` |`-im`  | Use either slow or fast restricted nearest neighbor linkage or no initialization. Can be any of `slow-nn`, `fast-nn`, `simple`. Defaults to `slow-nn`.
 `--no-moving`           |`-nm`  | By default, the removing procedure tries to relocate sequences to another partition if it finds more within-threshold neighbours in any. This flag disallows moving. In high-redundancy datasets, moving can lead to imbalanced partitions and should be disabled.
-`--remove-same`         |`-rs`  | This here is the inverse of removal_type (has default True) DO @Magnus can you describe it in one sentence?
 `--save-checkpoint-path`|`-sc`  | Optional path to save the computed identities above the chosen threshold as an edge list. Can be used to quickstart runs in the `precomputed` mode. Defaults to `None` with no file saved.
 `--test-ratio`          | `-te` | Make a train-val-test split instead of partitions for cross-validation. Overrides `--partitions` when specified. Defaults to 0. Needs to be a multiple of 0.05.
 `--val-ratio`           | `-va` |Make a train-val-test split instead of partitions for cross-validation. Overrides `--partitions` when specified. Defaults to 0. Needs to be a multiple of 0.05.
 
 #### needle
 
 Long                    | Short | Description
 ------------------------|-------|------------
 `--denominator`         |`-dn`  | Denominator to use for percent sequence identity computation. The number of perfect matching positions is divided by the result of this operation. Can be any of `shortest`, `longest`, `mean`, `full`, `no_gaps`. The first three options are computed from the original lengths of the aligned sequences. `full` refers to the full length of the alignment, including gaps, and is the default. `no_gaps` subtracts gaps from the full alignment length.
 `--threads`             |`-nt`  | The number of threads to run in parallel. If `-1`, will use all available resources. Defaults to 1.
 `--chunks`              |`-nc`  | The number of chunks into which to split the fasta file for multithreaded alignment. Defaults to 10.
-`--parallel-mode`       |`-pm`  | The Python parallelization strategy to use. `multithread` or `multiprocess`. Multiprocessing is potentially faster (especially for short sequences), but increases memory usage.
+`--parallel-mode`       |`-pm`  | The Python parallelization strategy to use. `multithread` or `multiprocess`. Multiprocessing is potentially faster (especially for short sequences), but increases memory usage. Defaults to `multithread`
 `--nucleotide`          |`-nu`  | Use this flag if the input contains nucleotide sequences. By default, assumes proteins.
 `--triangular`          |`-tr`  | Only compute triangular of the full distance matrix. Twice as fast, but can yield slightly different results if an alignment has two different solutions with the same score, but different identities. In some cases, a pairwise identity can be slightly above the threshold in one solution, and slightly below in another (e.g A:B = 29.8%, B:A = 30.4%).
 `--gapopen`             |`-gapopen`     | [10.0 for any sequence] The gap open penalty is the score taken away when a gap is created. The best value depends on the choice of comparison matrix. The default value assumes you are using the EBLOSUM62 matrix. (Floating point number from 1.0 to 100.0)
-`--gapextend`           |`-gapextend`   | [0.5 for any sequence] The gap extension penalty is added to the standard gap penalty for each base or residue in the gap. This is how long gaps are penalized. Usually you will expect a few long gaps rather than many short gaps, so the gap extension penalty should be lower than the gap penalty. An exception is where one or both sequences are single reads with possible sequencing errors in which case you would expect many single base gaps. You can get this result by setting the gap open penalty to zero (or very low) and using the gap extension penalty to control gap scoring. (Floating point number from 0.0 to 10.0)
+`--gapextend`           |`-gapextend`   | [0.5 for any sequence] The gap extension penalty is added to the standard gap penalty for each base or residue in the gap. This is how long gaps are penalized. Usually you will expect a few long gaps rather than many short gaps, so the gap extension penalty should be lower than the gap penalty. An exception is where one or both sequences are single reads with possible sequencing errors in which case you would expect many single base gaps. You can get this result by setting the gap open penalty to a very low value and using the gap extension penalty to control gap scoring. (Floating point number from 0.0 to 10.0)
 `--endextend`           |`-endextend`   | [0.5 for any sequence] The end gap extension, penalty is added to the end gap penalty for each base or residue in the end gap. This is how long end gaps are penalized. (Floating point number from 0.0 to 10.0)
 `--endweight`           |`-endweight`   | Flag. Apply end gap penalties.
 `--endopen`             |`-endopen`     | [10.0 for any sequence] The end gap open penalty is the score taken away when an end gap is created. The best value depends on the choice of comparison matrix. The default value assumes you are using the EBLOSUM62 matrix for protein sequences. (Floating point number from 1.0 to 100.0)
 `--matrix`              |`-datafile`    | This is the scoring matrix file used when comparing sequences. By default it is the file 'EBLOSUM62'. These files are found in the 'data' directory of the EMBOSS installation.
 
 
 #### mmseqs2
```

### Comparing `graph-part-1.0.1/graph_part.egg-info/SOURCES.txt` & `graph-part-1.0.2/graph_part.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graph-part-1.0.1/setup.py` & `graph-part-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 
 
 
 
 setup(
     name="graph-part",
-    version='1.0.1',
+    version='1.0.2',
     description="Graph-based partitioning of biological sequence data",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/graph-part/graph-part",
     author="F. Teufel and M.H. Gislason",
     packages=['graph_part'],
     python_requires=">=3.6, <4",
```

