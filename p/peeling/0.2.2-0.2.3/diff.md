# Comparing `tmp/peeling-0.2.2.tar.gz` & `tmp/peeling-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peeling-0.2.2.tar", last modified: Thu Jun 29 20:34:55 2023, max compression
+gzip compressed data, was "peeling-0.2.3.tar", last modified: Thu Jul 13 01:59:13 2023, max compression
```

## Comparing `peeling-0.2.2.tar` & `peeling-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 clementsj   (503) staff       (20)        0 2023-06-29 20:34:55.727373 peeling-0.2.2/
--rw-r--r--   0 clementsj   (503) staff       (20)     1518 2023-05-16 19:45:54.000000 peeling-0.2.2/LICENSE
--rw-r--r--   0 clementsj   (503) staff       (20)     9140 2023-06-29 20:34:55.727216 peeling-0.2.2/PKG-INFO
--rw-r--r--   0 clementsj   (503) staff       (20)     7008 2023-06-29 19:26:11.000000 peeling-0.2.2/README.md
-drwxr-xr-x   0 clementsj   (503) staff       (20)        0 2023-06-29 20:34:55.725899 peeling-0.2.2/peeling/
--rw-r--r--   0 clementsj   (503) staff       (20)        0 2023-05-16 19:45:54.000000 peeling-0.2.2/peeling/__init__.py
--rw-r--r--   0 clementsj   (503) staff       (20)     3169 2023-06-07 13:14:59.000000 peeling-0.2.2/peeling/cellular_compartments.py
--rw-r--r--   0 clementsj   (503) staff       (20)     1337 2023-06-07 13:14:59.000000 peeling-0.2.2/peeling/clipantherprocessor.py
--rwxr-xr-x   0 clementsj   (503) staff       (20)     6492 2023-06-07 13:14:59.000000 peeling-0.2.2/peeling/cliprocessor.py
--rwxr-xr-x   0 clementsj   (503) staff       (20)      267 2023-06-07 13:14:59.000000 peeling-0.2.2/peeling/cliuniprotcommunicator.py
--rwxr-xr-x   0 clementsj   (503) staff       (20)     3606 2023-06-29 18:22:08.000000 peeling-0.2.2/peeling/cliuserinputreader.py
--rwxr-xr-x   0 clementsj   (503) staff       (20)     4798 2023-06-28 14:01:23.000000 peeling-0.2.2/peeling/main.py
--rw-r--r--   0 clementsj   (503) staff       (20)     6156 2023-06-07 13:14:59.000000 peeling-0.2.2/peeling/pantherprocessor.py
--rw-r--r--   0 clementsj   (503) staff       (20)    10929 2023-06-29 18:18:33.000000 peeling-0.2.2/peeling/processor.py
--rw-r--r--   0 clementsj   (503) staff       (20)    12249 2023-06-07 13:14:59.000000 peeling-0.2.2/peeling/uniprotcommunicator.py
--rw-r--r--   0 clementsj   (503) staff       (20)     2256 2023-06-07 13:14:59.000000 peeling-0.2.2/peeling/userinputreader.py
--rw-r--r--   0 clementsj   (503) staff       (20)     1595 2023-06-07 13:14:59.000000 peeling-0.2.2/peeling/webpantherprocessor.py
--rwxr-xr-x   0 clementsj   (503) staff       (20)     5478 2023-06-29 18:37:23.000000 peeling-0.2.2/peeling/webprocessor.py
--rwxr-xr-x   0 clementsj   (503) staff       (20)     6498 2023-06-07 13:14:59.000000 peeling-0.2.2/peeling/webuniprotcommunicator.py
--rwxr-xr-x   0 clementsj   (503) staff       (20)     1110 2023-06-07 18:42:16.000000 peeling-0.2.2/peeling/webuserinputreader.py
-drwxr-xr-x   0 clementsj   (503) staff       (20)        0 2023-06-29 20:34:55.726774 peeling-0.2.2/peeling.egg-info/
--rw-r--r--   0 clementsj   (503) staff       (20)     9140 2023-06-29 20:34:55.000000 peeling-0.2.2/peeling.egg-info/PKG-INFO
--rw-r--r--   0 clementsj   (503) staff       (20)      647 2023-06-29 20:34:55.000000 peeling-0.2.2/peeling.egg-info/SOURCES.txt
--rw-r--r--   0 clementsj   (503) staff       (20)        1 2023-06-29 20:34:55.000000 peeling-0.2.2/peeling.egg-info/dependency_links.txt
--rw-r--r--   0 clementsj   (503) staff       (20)       46 2023-06-29 20:34:55.000000 peeling-0.2.2/peeling.egg-info/entry_points.txt
--rw-r--r--   0 clementsj   (503) staff       (20)      522 2023-06-29 20:34:55.000000 peeling-0.2.2/peeling.egg-info/requires.txt
--rw-r--r--   0 clementsj   (503) staff       (20)        8 2023-06-29 20:34:55.000000 peeling-0.2.2/peeling.egg-info/top_level.txt
--rw-r--r--   0 clementsj   (503) staff       (20)     1479 2023-06-29 18:44:27.000000 peeling-0.2.2/pyproject.toml
--rw-r--r--   0 clementsj   (503) staff       (20)       38 2023-06-29 20:34:55.727410 peeling-0.2.2/setup.cfg
-drwxr-xr-x   0 clementsj   (503) staff       (20)        0 2023-06-29 20:34:55.726899 peeling-0.2.2/test/
--rw-r--r--   0 clementsj   (503) staff       (20)    15513 2023-05-16 19:45:54.000000 peeling-0.2.2/test/test.py
+drwxr-xr-x   0 pengxi     (501) staff       (20)        0 2023-07-13 01:59:13.155089 peeling-0.2.3/
+-rw-r--r--   0 pengxi     (501) staff       (20)     1518 2023-07-07 14:15:58.000000 peeling-0.2.3/LICENSE
+-rw-r--r--   0 pengxi     (501) staff       (20)     8600 2023-07-13 01:59:13.154709 peeling-0.2.3/PKG-INFO
+-rw-r--r--   0 pengxi     (501) staff       (20)     6468 2023-07-12 23:15:27.000000 peeling-0.2.3/README.md
+drwxr-xr-x   0 pengxi     (501) staff       (20)        0 2023-07-13 01:59:13.152118 peeling-0.2.3/peeling/
+-rw-r--r--   0 pengxi     (501) staff       (20)        0 2023-07-07 14:15:58.000000 peeling-0.2.3/peeling/__init__.py
+-rw-r--r--   0 pengxi     (501) staff       (20)     3169 2023-07-07 14:15:58.000000 peeling-0.2.3/peeling/cellular_compartments.py
+-rw-r--r--   0 pengxi     (501) staff       (20)     1337 2023-07-07 14:15:58.000000 peeling-0.2.3/peeling/clipantherprocessor.py
+-rwxr-xr-x   0 pengxi     (501) staff       (20)     6492 2023-07-07 14:15:58.000000 peeling-0.2.3/peeling/cliprocessor.py
+-rwxr-xr-x   0 pengxi     (501) staff       (20)      267 2023-07-07 14:15:58.000000 peeling-0.2.3/peeling/cliuniprotcommunicator.py
+-rwxr-xr-x   0 pengxi     (501) staff       (20)     3606 2023-07-07 14:15:58.000000 peeling-0.2.3/peeling/cliuserinputreader.py
+-rwxr-xr-x   0 pengxi     (501) staff       (20)     4798 2023-07-12 23:46:02.000000 peeling-0.2.3/peeling/main.py
+-rw-r--r--   0 pengxi     (501) staff       (20)     6156 2023-07-07 14:15:58.000000 peeling-0.2.3/peeling/pantherprocessor.py
+-rw-r--r--   0 pengxi     (501) staff       (20)    10929 2023-07-07 14:15:58.000000 peeling-0.2.3/peeling/processor.py
+-rw-r--r--   0 pengxi     (501) staff       (20)    12249 2023-07-07 14:15:58.000000 peeling-0.2.3/peeling/uniprotcommunicator.py
+-rw-r--r--   0 pengxi     (501) staff       (20)     2256 2023-07-07 14:15:58.000000 peeling-0.2.3/peeling/userinputreader.py
+-rw-r--r--   0 pengxi     (501) staff       (20)     1595 2023-07-07 14:15:58.000000 peeling-0.2.3/peeling/webpantherprocessor.py
+-rwxr-xr-x   0 pengxi     (501) staff       (20)     5478 2023-07-07 14:15:58.000000 peeling-0.2.3/peeling/webprocessor.py
+-rwxr-xr-x   0 pengxi     (501) staff       (20)     6527 2023-07-13 01:08:50.000000 peeling-0.2.3/peeling/webuniprotcommunicator.py
+-rwxr-xr-x   0 pengxi     (501) staff       (20)     1110 2023-07-07 14:15:58.000000 peeling-0.2.3/peeling/webuserinputreader.py
+drwxr-xr-x   0 pengxi     (501) staff       (20)        0 2023-07-13 01:59:13.153723 peeling-0.2.3/peeling.egg-info/
+-rw-r--r--   0 pengxi     (501) staff       (20)     8600 2023-07-13 01:59:13.000000 peeling-0.2.3/peeling.egg-info/PKG-INFO
+-rw-r--r--   0 pengxi     (501) staff       (20)      647 2023-07-13 01:59:13.000000 peeling-0.2.3/peeling.egg-info/SOURCES.txt
+-rw-r--r--   0 pengxi     (501) staff       (20)        1 2023-07-13 01:59:13.000000 peeling-0.2.3/peeling.egg-info/dependency_links.txt
+-rw-r--r--   0 pengxi     (501) staff       (20)       46 2023-07-13 01:59:13.000000 peeling-0.2.3/peeling.egg-info/entry_points.txt
+-rw-r--r--   0 pengxi     (501) staff       (20)      522 2023-07-13 01:59:13.000000 peeling-0.2.3/peeling.egg-info/requires.txt
+-rw-r--r--   0 pengxi     (501) staff       (20)        8 2023-07-13 01:59:13.000000 peeling-0.2.3/peeling.egg-info/top_level.txt
+-rw-r--r--   0 pengxi     (501) staff       (20)     1479 2023-07-13 01:29:07.000000 peeling-0.2.3/pyproject.toml
+-rw-r--r--   0 pengxi     (501) staff       (20)       38 2023-07-13 01:59:13.155171 peeling-0.2.3/setup.cfg
+drwxr-xr-x   0 pengxi     (501) staff       (20)        0 2023-07-13 01:59:13.153993 peeling-0.2.3/test/
+-rw-r--r--   0 pengxi     (501) staff       (20)    15513 2023-07-07 14:15:58.000000 peeling-0.2.3/test/test.py
```

### Comparing `peeling-0.2.2/LICENSE` & `peeling-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `peeling-0.2.2/PKG-INFO` & `peeling-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peeling
-Version: 0.2.2
+Version: 0.2.3
 Author-email: HHMI Janelia <peeling@janelia.hhmi.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Howard Hughes Medical Institute
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -40,19 +40,25 @@
 
 # PEELing
 
 
 ### Introduction
 Molecular compartmentalization is vital for cellular physiology. Spatially-resolved proteomics allows biologists to survey protein composition and dynamics with subcellular resolution. Here, we present **PEELing** (***p***roteome ***e***xtraction from ***e***nzymatic ***l***abel***ing*** data), an integrated package and user-friendly web service for analyzing spatially-resolved proteomics data. PEELing assesses data quality using curated or user-defined references, performs cutoff analysis to remove contaminants, connects to databases for functional annotation, and generates data visualizations—providing a streamlined and reproducible workflow to explore spatially-resolved proteomics data.
 
-This `PEELing` program provides an automated, standardized, and easy-to-use analysis pipeline for iPEEL or any other cell-surface proteomics data. PEELing evaluates data quality using curated [Swiss-Prot](https://www.sib.swiss/swiss-prot)  references, performs cut-off analysis to remove contaminants (modified from [Hung et al., 2014](https://pubmed.ncbi.nlm.nih.gov/25002142/) — `PMID:  25002142`), connects to [UniProt](https://www.uniprot.org/) and [Panther](http://www.pantherdb.org/) databases for functional annotation, and generates data visualizations. Together with iPEEL transgenic tools (The Jackson Laboratory: 037697, 037698; Bloomington Drosophila Stock Center: 8763, 9906, 9908), PEELing enables a complete pipeline, from wet lab method to data analysis, for in situ cell-surface proteomics.
-
 `PEELing` also provides a web portal. Please refer to [link](http://peeling.janelia.org)
 
 
+
+### Citation
+Manuscript preprint: [https://www.biorxiv.org/content/10.1101/2023.04.21.537871](https://www.biorxiv.org/content/10.1101/2023.04.21.537871)
+
+Please note that this bioRxiv preprint will be updated as we add new functionalities to PEELing.
+
+
+
 ### Installation
 ```
 pip install peeling
 ```
 
 
 ### Basic Usage
@@ -70,23 +76,23 @@
 ##### Mass Spec Data Example (e.g., 2 non-labelled controls and 3 labelled replicates)
 | UniProt_IDs  | Ratio_Labelled-Rep1_Over_Ctrl1 | Ratio_Labelled-Rep2_Over_Ctrl1 | Ratio_Labelled-Rep3_Over_Ctrl1 | Ratio_Labelled-Rep1_Over_Ctrl2 | Ratio_Labelled-Rep2_Over_Ctrl2 | Ratio_Labelled-Rep3_Over_Ctrl2 |
 | ------------ | ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ |
 | Content Cell |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |
 | Content Cell |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |
 
 #### Note
-The basic usage will communicate with the UniProt website to map the provided IDs to their latest version, and get the annotation data of surface proteins (TP) and introcellular proteins (FP). Our testing shows that this can take dozens of seconds or minutes to complete.
+The basic usage will communicate with the UniProt website to map the provided IDs to their latest version, and get the annotation data of true positive proteins (TP) and false positive proteins (FP). Our testing shows that this can take dozens of seconds or minutes to complete.
 
 Therefore, it is recommended to save the retrieved data after the first run, and use the locally saved data for the following runs, which will reduce the run time to seconds. If using local annotation files, PEELing does id mapping by default. To disable id mapping for local annotation files specify -n/--nomap. Note: Remember to update the retrieved data periodically.
 ```
 # To save the retrieved data, specify -a/--cache
 peeling mass_spec_dir num_of_nonlabelled_controls num_of_labelled_replicates --cache
 
 # To use locally saved data, specify the directories
-peeling mass_spec_dir num_of_nonlabelled_controls num_of_labelled_replicates --ids latest_ids_dir --surface annotation_surface_dir --cyto annotation_cyto_dir --nomap
+peeling mass_spec_dir num_of_nonlabelled_controls num_of_labelled_replicates --ids latest_ids_dir --tp annotation_true_positive_dir --fp annotation_false_positive_dir --nomap
 ```
 
 
 ### Panther analysis
 PEELing provides the functionality to perform protein ontology and pathway analyses of the post-cutoff proteome using the [Panther](http://www.pantherdb.org/) API. Top 10 terms based on false discovery rate (FDR) are listed for protein localization (Panther GO Slim Cellular Component), function (Panther GO Slim Biological Process), and pathway (Reactome).
 
 To run this analysis, specify `-p/--panther` and provide the organism from which the mass spec data is made. Please refer to Panther's API [page](http://pantherdb.org/services/oai/pantherdb/supportedgenomes) for supported organism. Choose the corresponding 'long_names', and wrap it by quotes if there is white space inside the name, e.g. 'Homo sapiens'
```

### Comparing `peeling-0.2.2/README.md` & `peeling-0.2.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 # PEELing
 
 
 ### Introduction
 Molecular compartmentalization is vital for cellular physiology. Spatially-resolved proteomics allows biologists to survey protein composition and dynamics with subcellular resolution. Here, we present **PEELing** (***p***roteome ***e***xtraction from ***e***nzymatic ***l***abel***ing*** data), an integrated package and user-friendly web service for analyzing spatially-resolved proteomics data. PEELing assesses data quality using curated or user-defined references, performs cutoff analysis to remove contaminants, connects to databases for functional annotation, and generates data visualizations—providing a streamlined and reproducible workflow to explore spatially-resolved proteomics data.
 
-This `PEELing` program provides an automated, standardized, and easy-to-use analysis pipeline for iPEEL or any other cell-surface proteomics data. PEELing evaluates data quality using curated [Swiss-Prot](https://www.sib.swiss/swiss-prot)  references, performs cut-off analysis to remove contaminants (modified from [Hung et al., 2014](https://pubmed.ncbi.nlm.nih.gov/25002142/) — `PMID:  25002142`), connects to [UniProt](https://www.uniprot.org/) and [Panther](http://www.pantherdb.org/) databases for functional annotation, and generates data visualizations. Together with iPEEL transgenic tools (The Jackson Laboratory: 037697, 037698; Bloomington Drosophila Stock Center: 8763, 9906, 9908), PEELing enables a complete pipeline, from wet lab method to data analysis, for in situ cell-surface proteomics.
-
 `PEELing` also provides a web portal. Please refer to [link](http://peeling.janelia.org)
 
 
+
+### Citation
+Manuscript preprint: [https://www.biorxiv.org/content/10.1101/2023.04.21.537871](https://www.biorxiv.org/content/10.1101/2023.04.21.537871)
+
+Please note that this bioRxiv preprint will be updated as we add new functionalities to PEELing.
+
+
+
 ### Installation
 ```
 pip install peeling
 ```
 
 
 ### Basic Usage
@@ -30,23 +36,23 @@
 ##### Mass Spec Data Example (e.g., 2 non-labelled controls and 3 labelled replicates)
 | UniProt_IDs  | Ratio_Labelled-Rep1_Over_Ctrl1 | Ratio_Labelled-Rep2_Over_Ctrl1 | Ratio_Labelled-Rep3_Over_Ctrl1 | Ratio_Labelled-Rep1_Over_Ctrl2 | Ratio_Labelled-Rep2_Over_Ctrl2 | Ratio_Labelled-Rep3_Over_Ctrl2 |
 | ------------ | ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ |
 | Content Cell |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |
 | Content Cell |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |
 
 #### Note
-The basic usage will communicate with the UniProt website to map the provided IDs to their latest version, and get the annotation data of surface proteins (TP) and introcellular proteins (FP). Our testing shows that this can take dozens of seconds or minutes to complete.
+The basic usage will communicate with the UniProt website to map the provided IDs to their latest version, and get the annotation data of true positive proteins (TP) and false positive proteins (FP). Our testing shows that this can take dozens of seconds or minutes to complete.
 
 Therefore, it is recommended to save the retrieved data after the first run, and use the locally saved data for the following runs, which will reduce the run time to seconds. If using local annotation files, PEELing does id mapping by default. To disable id mapping for local annotation files specify -n/--nomap. Note: Remember to update the retrieved data periodically.
 ```
 # To save the retrieved data, specify -a/--cache
 peeling mass_spec_dir num_of_nonlabelled_controls num_of_labelled_replicates --cache
 
 # To use locally saved data, specify the directories
-peeling mass_spec_dir num_of_nonlabelled_controls num_of_labelled_replicates --ids latest_ids_dir --surface annotation_surface_dir --cyto annotation_cyto_dir --nomap
+peeling mass_spec_dir num_of_nonlabelled_controls num_of_labelled_replicates --ids latest_ids_dir --tp annotation_true_positive_dir --fp annotation_false_positive_dir --nomap
 ```
 
 
 ### Panther analysis
 PEELing provides the functionality to perform protein ontology and pathway analyses of the post-cutoff proteome using the [Panther](http://www.pantherdb.org/) API. Top 10 terms based on false discovery rate (FDR) are listed for protein localization (Panther GO Slim Cellular Component), function (Panther GO Slim Biological Process), and pathway (Reactome).
 
 To run this analysis, specify `-p/--panther` and provide the organism from which the mass spec data is made. Please refer to Panther's API [page](http://pantherdb.org/services/oai/pantherdb/supportedgenomes) for supported organism. Choose the corresponding 'long_names', and wrap it by quotes if there is white space inside the name, e.g. 'Homo sapiens'
```

### Comparing `peeling-0.2.2/peeling/cellular_compartments.py` & `peeling-0.2.3/peeling/cellular_compartments.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.2/peeling/clipantherprocessor.py` & `peeling-0.2.3/peeling/clipantherprocessor.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.2/peeling/cliprocessor.py` & `peeling-0.2.3/peeling/cliprocessor.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.2/peeling/cliuserinputreader.py` & `peeling-0.2.3/peeling/cliuserinputreader.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.2/peeling/main.py` & `peeling-0.2.3/peeling/main.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.2/peeling/pantherprocessor.py` & `peeling-0.2.3/peeling/pantherprocessor.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.2/peeling/processor.py` & `peeling-0.2.3/peeling/processor.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.2/peeling/uniprotcommunicator.py` & `peeling-0.2.3/peeling/uniprotcommunicator.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.2/peeling/userinputreader.py` & `peeling-0.2.3/peeling/userinputreader.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.2/peeling/webpantherprocessor.py` & `peeling-0.2.3/peeling/webpantherprocessor.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.2/peeling/webprocessor.py` & `peeling-0.2.3/peeling/webprocessor.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.2/peeling/webuniprotcommunicator.py` & `peeling-0.2.3/peeling/webuniprotcommunicator.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import os
 from peeling.uniprotcommunicator import UniProtCommunicator
 
 logger = logging.getLogger('peeling')
 
 
 class WebUniProtCommunicator(UniProtCommunicator):
-    def __init__(self, cache, cellular_compartment, tp_data=None, fp_data=None):
+    def __init__(self, cache, cellular_compartment, track_update, tp_data=None, fp_data=None):
         super().__init__(cache, cellular_compartment)
         self.__ids = None
-        self.__track_update = 0
+        self.__track_update = track_update
         if isinstance(tp_data, pd.DataFrame) and isinstance(fp_data, pd.DataFrame):
             self._annotation_true_positive = tp_data
             self._annotation_false_positive = fp_data
         else:
             self.__init_annotations()
 
 
@@ -106,15 +106,15 @@
 
 
     async def update_data(self):
         start_time = datetime.now()
         if self.__track_update == 0:
             try:
                 await self.__initialize()
-                self.__track_update += 1
+                # self.__track_update += 1
             except Exception as e:
                 logger.error(e)
         else:
             logger.info('Updating data...')
             try:
                 meta={}
                 if self.__ids is not None:
@@ -129,15 +129,15 @@
                 true_positive = await self.get_annotation('true_positive')
                 true_positive.to_csv(f'../retrieved_data/{self._cc_code}_annotation_true_positive.tsv', sep='\t', index=False)
                 false_positive = await self.get_annotation('false_positive')
                 false_positive.to_csv(f'../retrieved_data/{self._cc_code}_annotation_false_positive.tsv', sep='\t', index=False)
                 logger.info(f'Annotation files saved')
                 end_time = datetime.now()
                 logger.info(f'Update is done. Time: {end_time-start_time}')
-                self.__track_update += 1
+                # self.__track_update += 1
             except Exception as e:
                 logger.error(e)
 
 
     # called in main.py, to export cached ids by api instead of waiting for update
     def get_ids(self):
         return self.__ids
```

### Comparing `peeling-0.2.2/peeling/webuserinputreader.py` & `peeling-0.2.3/peeling/webuserinputreader.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.2/peeling.egg-info/PKG-INFO` & `peeling-0.2.3/peeling.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peeling
-Version: 0.2.2
+Version: 0.2.3
 Author-email: HHMI Janelia <peeling@janelia.hhmi.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Howard Hughes Medical Institute
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -40,19 +40,25 @@
 
 # PEELing
 
 
 ### Introduction
 Molecular compartmentalization is vital for cellular physiology. Spatially-resolved proteomics allows biologists to survey protein composition and dynamics with subcellular resolution. Here, we present **PEELing** (***p***roteome ***e***xtraction from ***e***nzymatic ***l***abel***ing*** data), an integrated package and user-friendly web service for analyzing spatially-resolved proteomics data. PEELing assesses data quality using curated or user-defined references, performs cutoff analysis to remove contaminants, connects to databases for functional annotation, and generates data visualizations—providing a streamlined and reproducible workflow to explore spatially-resolved proteomics data.
 
-This `PEELing` program provides an automated, standardized, and easy-to-use analysis pipeline for iPEEL or any other cell-surface proteomics data. PEELing evaluates data quality using curated [Swiss-Prot](https://www.sib.swiss/swiss-prot)  references, performs cut-off analysis to remove contaminants (modified from [Hung et al., 2014](https://pubmed.ncbi.nlm.nih.gov/25002142/) — `PMID:  25002142`), connects to [UniProt](https://www.uniprot.org/) and [Panther](http://www.pantherdb.org/) databases for functional annotation, and generates data visualizations. Together with iPEEL transgenic tools (The Jackson Laboratory: 037697, 037698; Bloomington Drosophila Stock Center: 8763, 9906, 9908), PEELing enables a complete pipeline, from wet lab method to data analysis, for in situ cell-surface proteomics.
-
 `PEELing` also provides a web portal. Please refer to [link](http://peeling.janelia.org)
 
 
+
+### Citation
+Manuscript preprint: [https://www.biorxiv.org/content/10.1101/2023.04.21.537871](https://www.biorxiv.org/content/10.1101/2023.04.21.537871)
+
+Please note that this bioRxiv preprint will be updated as we add new functionalities to PEELing.
+
+
+
 ### Installation
 ```
 pip install peeling
 ```
 
 
 ### Basic Usage
@@ -70,23 +76,23 @@
 ##### Mass Spec Data Example (e.g., 2 non-labelled controls and 3 labelled replicates)
 | UniProt_IDs  | Ratio_Labelled-Rep1_Over_Ctrl1 | Ratio_Labelled-Rep2_Over_Ctrl1 | Ratio_Labelled-Rep3_Over_Ctrl1 | Ratio_Labelled-Rep1_Over_Ctrl2 | Ratio_Labelled-Rep2_Over_Ctrl2 | Ratio_Labelled-Rep3_Over_Ctrl2 |
 | ------------ | ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ |
 | Content Cell |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |
 | Content Cell |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |          Content Cell          |
 
 #### Note
-The basic usage will communicate with the UniProt website to map the provided IDs to their latest version, and get the annotation data of surface proteins (TP) and introcellular proteins (FP). Our testing shows that this can take dozens of seconds or minutes to complete.
+The basic usage will communicate with the UniProt website to map the provided IDs to their latest version, and get the annotation data of true positive proteins (TP) and false positive proteins (FP). Our testing shows that this can take dozens of seconds or minutes to complete.
 
 Therefore, it is recommended to save the retrieved data after the first run, and use the locally saved data for the following runs, which will reduce the run time to seconds. If using local annotation files, PEELing does id mapping by default. To disable id mapping for local annotation files specify -n/--nomap. Note: Remember to update the retrieved data periodically.
 ```
 # To save the retrieved data, specify -a/--cache
 peeling mass_spec_dir num_of_nonlabelled_controls num_of_labelled_replicates --cache
 
 # To use locally saved data, specify the directories
-peeling mass_spec_dir num_of_nonlabelled_controls num_of_labelled_replicates --ids latest_ids_dir --surface annotation_surface_dir --cyto annotation_cyto_dir --nomap
+peeling mass_spec_dir num_of_nonlabelled_controls num_of_labelled_replicates --ids latest_ids_dir --tp annotation_true_positive_dir --fp annotation_false_positive_dir --nomap
 ```
 
 
 ### Panther analysis
 PEELing provides the functionality to perform protein ontology and pathway analyses of the post-cutoff proteome using the [Panther](http://www.pantherdb.org/) API. Top 10 terms based on false discovery rate (FDR) are listed for protein localization (Panther GO Slim Cellular Component), function (Panther GO Slim Biological Process), and pathway (Reactome).
 
 To run this analysis, specify `-p/--panther` and provide the organism from which the mass spec data is made. Please refer to Panther's API [page](http://pantherdb.org/services/oai/pantherdb/supportedgenomes) for supported organism. Choose the corresponding 'long_names', and wrap it by quotes if there is white space inside the name, e.g. 'Homo sapiens'
```

### Comparing `peeling-0.2.2/peeling.egg-info/SOURCES.txt` & `peeling-0.2.3/peeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peeling-0.2.2/peeling.egg-info/requires.txt` & `peeling-0.2.3/peeling.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `peeling-0.2.2/pyproject.toml` & `peeling-0.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "peeling"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="HHMI Janelia", email="peeling@janelia.hhmi.org" },
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `peeling-0.2.2/test/test.py` & `peeling-0.2.3/test/test.py`

 * *Files identical despite different names*

