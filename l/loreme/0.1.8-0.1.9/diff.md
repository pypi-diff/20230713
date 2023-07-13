# Comparing `tmp/loreme-0.1.8.tar.gz` & `tmp/loreme-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loreme-0.1.8.tar", last modified: Fri Jul  7 02:06:05 2023, max compression
+gzip compressed data, was "loreme-0.1.9.tar", last modified: Thu Jul 13 20:18:37 2023, max compression
```

## Comparing `loreme-0.1.8.tar` & `loreme-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-07 02:06:05.551694 loreme-0.1.8/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1520 2023-06-14 04:51:11.000000 loreme-0.1.8/LICENSE
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5245 2023-07-07 02:06:05.551141 loreme-0.1.8/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     4730 2023-06-14 04:58:53.000000 loreme-0.1.8/README.md
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-07 02:06:05.525699 loreme-0.1.8/loreme.egg-info/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5245 2023-07-07 02:06:05.000000 loreme-0.1.8/loreme.egg-info/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      763 2023-07-07 02:06:05.000000 loreme-0.1.8/loreme.egg-info/SOURCES.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-07-07 02:06:05.000000 loreme-0.1.8/loreme.egg-info/dependency_links.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       46 2023-07-07 02:06:05.000000 loreme-0.1.8/loreme.egg-info/entry_points.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       77 2023-07-07 02:06:05.000000 loreme-0.1.8/loreme.egg-info/requires.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        7 2023-07-07 02:06:05.000000 loreme-0.1.8/loreme.egg-info/top_level.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      918 2023-07-07 01:45:52.000000 loreme-0.1.8/pyproject.toml
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-07-07 02:06:05.551855 loreme-0.1.8/setup.cfg
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-07 02:06:05.518293 loreme-0.1.8/src/
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-07 02:06:05.550028 loreme-0.1.8/src/loreme/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1623 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/__init__.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2645 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/check_gpu_availability.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      396 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/check_tags.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3631 2023-07-03 21:29:32.000000 loreme-0.1.8/src/loreme/dorado.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     6099 2023-07-03 21:25:22.000000 loreme-0.1.8/src/loreme/download.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3907 2023-06-26 22:02:40.000000 loreme-0.1.8/src/loreme/env.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1496 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/export_bedgraph.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3440 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/gene_body_methylation.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1144 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/intersect.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)    37399 2023-07-06 23:58:13.000000 loreme-0.1.8/src/loreme/loreme.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5235 2023-06-14 05:31:42.000000 loreme-0.1.8/src/loreme/mean.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1690 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/merge.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      940 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/methylation_hist.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      376 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/modkit.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3054 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/parse_gff.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2219 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/pbcpg.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     6531 2023-06-14 05:32:28.000000 loreme-0.1.8/src/loreme/plot.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2563 2023-07-07 02:04:48.000000 loreme-0.1.8/src/loreme/plot_bedtools.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5087 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/plot_genes.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     4327 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/plot_repeats.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3433 2023-06-14 04:51:11.000000 loreme-0.1.8/src/loreme/promoter_methylation.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2023-07-07 01:45:55.000000 loreme-0.1.8/src/loreme/version.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-13 20:18:37.704452 loreme-0.1.9/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1520 2023-06-05 04:30:20.000000 loreme-0.1.9/LICENSE
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    10267 2023-07-13 20:18:37.704025 loreme-0.1.9/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     9752 2023-07-13 18:29:12.000000 loreme-0.1.9/README.md
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-13 20:18:37.680599 loreme-0.1.9/loreme.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    10267 2023-07-13 20:18:37.000000 loreme-0.1.9/loreme.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      763 2023-07-13 20:18:37.000000 loreme-0.1.9/loreme.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-07-13 20:18:37.000000 loreme-0.1.9/loreme.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       46 2023-07-13 20:18:37.000000 loreme-0.1.9/loreme.egg-info/entry_points.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       77 2023-07-13 20:18:37.000000 loreme-0.1.9/loreme.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        7 2023-07-13 20:18:37.000000 loreme-0.1.9/loreme.egg-info/top_level.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      918 2023-07-13 18:22:34.000000 loreme-0.1.9/pyproject.toml
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-07-13 20:18:37.704574 loreme-0.1.9/setup.cfg
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-13 20:18:37.675612 loreme-0.1.9/src/
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-07-13 20:18:37.703201 loreme-0.1.9/src/loreme/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1905 2023-07-13 18:22:34.000000 loreme-0.1.9/src/loreme/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2645 2023-06-05 04:30:20.000000 loreme-0.1.9/src/loreme/check_gpu_availability.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      396 2023-06-10 18:19:42.000000 loreme-0.1.9/src/loreme/check_tags.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3631 2023-06-13 05:56:48.000000 loreme-0.1.9/src/loreme/dorado.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     7715 2023-07-13 18:22:34.000000 loreme-0.1.9/src/loreme/download.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4291 2023-07-13 18:22:34.000000 loreme-0.1.9/src/loreme/env.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1496 2023-06-05 04:30:20.000000 loreme-0.1.9/src/loreme/export_bedgraph.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3440 2023-06-05 04:30:20.000000 loreme-0.1.9/src/loreme/gene_body_methylation.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1144 2023-06-05 04:30:20.000000 loreme-0.1.9/src/loreme/intersect.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    37948 2023-07-13 18:22:34.000000 loreme-0.1.9/src/loreme/loreme.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5235 2023-07-13 18:22:34.000000 loreme-0.1.9/src/loreme/mean.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1690 2023-06-05 04:30:20.000000 loreme-0.1.9/src/loreme/merge.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      940 2023-06-05 04:30:20.000000 loreme-0.1.9/src/loreme/methylation_hist.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      376 2023-06-10 17:48:02.000000 loreme-0.1.9/src/loreme/modkit.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3054 2023-06-05 04:30:20.000000 loreme-0.1.9/src/loreme/parse_gff.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2219 2023-06-10 18:20:20.000000 loreme-0.1.9/src/loreme/pbcpg.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     6531 2023-07-13 18:22:34.000000 loreme-0.1.9/src/loreme/plot.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2563 2023-07-13 18:22:34.000000 loreme-0.1.9/src/loreme/plot_bedtools.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5087 2023-06-05 04:30:20.000000 loreme-0.1.9/src/loreme/plot_genes.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4327 2023-06-05 04:30:20.000000 loreme-0.1.9/src/loreme/plot_repeats.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3433 2023-06-05 04:30:20.000000 loreme-0.1.9/src/loreme/promoter_methylation.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2023-07-13 18:22:34.000000 loreme-0.1.9/src/loreme/version.py
```

### Comparing `loreme-0.1.8/LICENSE` & `loreme-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `loreme-0.1.8/loreme.egg-info/SOURCES.txt` & `loreme-0.1.9/loreme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loreme-0.1.8/src/loreme/__init__.py` & `loreme-0.1.9/src/loreme/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 to `POD5 <https://github.com/nanoporetech/pod5-file-format>`_ format, then
 basecalled and aligned to a reference with `dorado <https://github.com/nanoporetech/dorado>`_ 
 (dorado alignment also uses minimap2 under the hood), and finally piled up with
 `modkit <https://github.com/nanoporetech/modkit/>`_ .
 
 3. Postprocessing and QC of methylation calls. Several functions are available
 to generate diagnostic statistics and plots.
+
+Other tools of interest: `methylartist <https://github.com/adamewing/methylartist>`_ , `modbamtools <https://github.com/rrazaghi/modbamtools>`_  (`modbamtools docs <https://rrazaghi.github.io/modbamtools/>`_), `methplotlib <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7214038/>`_
 """
 
 from loreme.version import __version__
 from loreme.env import PBCPG_MODEL
 from loreme.download import download_pbcpg, download_dorado
 from loreme.check_gpu_availability import check_gpu_availability
 from loreme.check_tags import check_tags
```

### Comparing `loreme-0.1.8/src/loreme/check_gpu_availability.py` & `loreme-0.1.9/src/loreme/check_gpu_availability.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.8/src/loreme/dorado.py` & `loreme-0.1.9/src/loreme/dorado.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.8/src/loreme/download.py` & `loreme-0.1.9/src/loreme/download.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 import os.path
 import ftplib
 import gzip
 import tarfile
 import subprocess
 import json
 from itertools import product
-from loreme.env import (PBCPG_URL, PBCPG_DIR, EXAMPLE_DATA_URLS, EXAMPLE_DATA_DIR, HG38_FTP,
+from loreme.env import (PBCPG_URL, PBCPG_DIR, PB_EXAMPLE_DATA_URLS, EXAMPLE_DATA_DIR, HG38_FTP,
                        HG38_GENOME_PATH, HG38_ANNOT_PATH, DORADO_DIR, DORADO_URL, DORADO_URL_024,
                        DORADO_MODEL_DIR, DORADO_CONFIG, DORADO_PATH, DORADO_PATH_024, MODKIT_URL,
-                       MODKIT_DIR)
+                       MODKIT_DIR, ONT_EXAMPLE_DATA_URL, KAZU_090722_GENOME_URL,
+                       KAZU_090722_ANNOT_URL)
 
 def download_pbcpg(directory: str = PBCPG_DIR):
     """Download pb-CpG-tools
 
     Parameters
     ----------
     directory : str
@@ -29,15 +30,15 @@
     http = urllib3.PoolManager()
     with http.request('GET', PBCPG_URL, preload_content=False) as r, open(dest_tarfile, 'wb') as f:
         shutil.copyfileobj(r, f)
     with tarfile.open(dest_tarfile) as tar:
         tar.extractall(path=directory)
 
 
-def download_example(directory: str = EXAMPLE_DATA_DIR, n_samples: int = 1):
+def download_pb_example(directory: str = EXAMPLE_DATA_DIR, n_samples: int = 1):
     """Download an example datatset
 
     Parameters
     ----------
     directory : str
         Destination directory for example data
     n_samples : int
@@ -63,23 +64,56 @@
         print(f'destination {hg38_annot_local_path} already exists')
     else:
         ftp = ftplib.FTP(HG38_FTP)
         ftp.login()
         with open(hg38_annot_local_path, 'wb') as f:
             ftp.retrbinary(f'RETR {HG38_ANNOT_PATH}', f.write)
     http = urllib3.PoolManager()
-    for example_data_url in EXAMPLE_DATA_URLS[:n_samples]:
+    for example_data_url in PB_EXAMPLE_DATA_URLS[:n_samples]:
         file_path = os.path.join(directory, os.path.basename(example_data_url))
         if os.path.exists(file_path):
             print(f'destination {file_path} already exists')
             continue
         with http.request('GET', example_data_url, preload_content=False) as r, open(file_path, 'wb') as out_file:
             shutil.copyfileobj(r, out_file)
 
 
+def download_ont_example(directory: str = EXAMPLE_DATA_DIR):
+    """Download an example datatset
+
+    Parameters
+    ----------
+    directory : str
+        Destination directory for example data
+    """
+
+    kazu_genome_local_path = os.path.join(directory, os.path.basename(KAZU_090722_GENOME_URL).replace('fna.gz', 'fa'))
+    kazu_annot_local_path = os.path.join(directory, os.path.basename(KAZU_090722_ANNOT_URL))
+    ont_example_data_local_path = os.path.join(directory, os.path.basename(ONT_EXAMPLE_DATA_URL))
+    http = urllib3.PoolManager()
+    if os.path.exists(kazu_genome_local_path):
+        print(f'destination {kazu_genome_local_path} already exists')
+    else:
+        with http.request('GET', KAZU_090722_GENOME_URL, preload_content=False) as r, \
+            open(kazu_genome_local_path, 'wb') as out_file:
+            shutil.copyfileobj(r, out_file)
+    if os.path.exists(kazu_annot_local_path):
+        print(f'destination {kazu_annot_local_path} already exists')
+    else:
+        with http.request('GET', KAZU_090722_ANNOT_URL, preload_content=False) as r, \
+            open(kazu_annot_local_path, 'wb') as out_file:
+            shutil.copyfileobj(r, out_file)
+    if os.path.exists(ont_example_data_local_path):
+        print(f'destination {ont_example_data_local_path} already exists')
+    else:
+        with http.request('GET', ONT_EXAMPLE_DATA_URL, preload_content=False) as r, \
+            open(ont_example_data_local_path, 'wb') as out_file:
+            shutil.copyfileobj(r, out_file)
+
+
 def download_dorado(pfm, directory=DORADO_DIR, model_dir=DORADO_MODEL_DIR,
                     dorado_config=DORADO_CONFIG):
     """Download dorado
 
     Parameters
     ----------
     pfm : str
```

### Comparing `loreme-0.1.8/src/loreme/env.py` & `loreme-0.1.9/src/loreme/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,26 @@
 PBCPG_DIR = os.environ.get('LOREME_PBCPG_DIR',
     os.path.join(os.path.dirname(__file__)))
 PBCPG_PATH = os.path.join(PBCPG_DIR, 'pb-CpG-tools-v2.3.1-x86_64-unknown-linux-gnu',
                          'bin', 'aligned_bam_to_cpg_scores')
 PBCPG_MODEL = os.path.join(PBCPG_DIR, 'pb-CpG-tools-v2.3.1-x86_64-unknown-linux-gnu',
                                'models', 'pileup_calling_model.v1.tflite')
 PBCPG_URL = 'https://github.com/PacificBiosciences/pb-CpG-tools/releases/download/v2.3.1/pb-CpG-tools-v2.3.1-x86_64-unknown-linux-gnu.tar.gz'
-EXAMPLE_DATA_URLS = (
+PB_EXAMPLE_DATA_URLS = (
     'https://downloads.pacbcloud.com/public/dataset/HG002-CpG-methylation-202202/m64011_190830_220126.hifi_reads.bam',
     'https://downloads.pacbcloud.com/public/dataset/HG002-CpG-methylation-202202/m64011_190901_095311.hifi_reads.bam',
     'https://downloads.pacbcloud.com/public/dataset/HG002-CpG-methylation-202202/m64012_190920_173625.hifi_reads.bam',
     'https://downloads.pacbcloud.com/public/dataset/HG002-CpG-methylation-202202/m64012_190921_234837.hifi_reads.bam',
 )
 HG38_FTP = 'ftp.ncbi.nlm.nih.gov'
 HG38_GENOME_PATH = 'genomes/all/GCA/000/001/405/GCA_000001405.15_GRCh38/seqs_for_alignment_pipelines.ucsc_ids/GCA_000001405.15_GRCh38_no_alt_analysis_set.fna.gz'
 HG38_ANNOT_PATH = 'genomes/all/GCA/000/001/405/GCA_000001405.15_GRCh38/seqs_for_alignment_pipelines.ucsc_ids/GCA_000001405.15_GRCh38_full_analysis_set.refseq_annotation.gff.gz'
+ONT_EXAMPLE_DATA_URL = 'https://salk-tm-pub.s3.us-west-2.amazonaws.com/LoReMe_example/Kazu_090722_95etoh_22C_6w_SRE1_deep.pod5'
+KAZU_090722_GENOME_URL = 'https://salk-tm-pub.s3.us-west-2.amazonaws.com/LoReMe_example/Kazu_090722.softmasked.fasta.gz'
+KAZU_090722_ANNOT_URL = 'https://salk-tm-pub.s3.us-west-2.amazonaws.com/LoReMe_example/Kazu_090722.primary_high_confidence.gff3.gz'
 EXAMPLE_DATA_DIR = os.environ.get('LOREME_EXAMPLE_DATA_DIR', os.path.dirname(__file__))
 
 DORADO_DIR = os.environ.get('LOREME_DORADO_DIR',
     os.path.join(os.path.dirname(__file__)))
 DORADO_CONFIG = os.environ.get('LOREME_DORADO_CONFIG',
     os.path.join(os.path.dirname(__file__), 'dorado-config.json'))
 if os.path.isfile(DORADO_CONFIG):
```

### Comparing `loreme-0.1.8/src/loreme/export_bedgraph.py` & `loreme-0.1.9/src/loreme/export_bedgraph.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.8/src/loreme/gene_body_methylation.py` & `loreme-0.1.9/src/loreme/gene_body_methylation.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.8/src/loreme/intersect.py` & `loreme-0.1.9/src/loreme/intersect.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.8/src/loreme/loreme.py` & `loreme-0.1.9/src/loreme/loreme.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 import os.path
 import platform
 import shutil
 from math import floor
 from loreme.env import (PBCPG_DIR, PBCPG_MODEL, EXAMPLE_DATA_DIR, DORADO_DIR,
                        DORADO_MODEL_DIR, DORADO_PLATFORM, MODKIT_DIR)
 from loreme.version import __version__
-from loreme.download import (download_pbcpg, download_example, download_dorado,
-                             download_modkit)
+from loreme.download import (download_pbcpg, download_pb_example,
+                             download_dorado, download_modkit,
+                             download_ont_example)
 from loreme.check_tags import check_tags
 from loreme.check_gpu_availability import check_gpu_availability
 from loreme.pbcpg import pbcpg_align_bams, pbcpg_pileup
 from loreme.dorado import CPU_COUNT, fast5_to_pod5, dorado_basecall, dorado_align
 from loreme.modkit import modkit_pileup
 from loreme.mean import calculate_mean, calculate_total_mean
 from loreme.gene_body_methylation import gene_body_methylation
@@ -90,16 +91,20 @@
         error_exit(f"Can't find index for bam file '{args.bam}'")
 
 
 def _download_pbcpg(args):
     download_pbcpg(directory=args.directory)
 
 
-def _download_example(args):
-    download_example(directory=args.directory, n_samples=args.n_samples)
+def _download_pb_example(args):
+    download_pb_example(directory=args.directory, n_samples=args.n_samples)
+
+
+def _download_ont_example(args):
+    download_ont_example(directory=args.directory)
 
 
 def _download_dorado(args):
     download_dorado(args.platform, directory=args.directory,
                     model_dir=args.model_dir)
 
 
@@ -306,21 +311,27 @@
     parser_download_modkit = subparsers.add_parser('download-modkit',
                                                   help='download modkit')
     parser_download_modkit.set_defaults(func=_download_modkit)
     parser_download_modkit.add_argument(
         '-d', '--directory', metavar='<directory/>', default=MODKIT_DIR,
         help=f'destination directory for pb-CpG-tools (default: {MODKIT_DIR})')
 
-    parser_download_example = subparsers.add_parser('download-example',
+    parser_download_pb_example = subparsers.add_parser('download-pb-example',
         help='download an example dataset for pbcpg')
-    parser_download_example.set_defaults(func=_download_example)
-    parser_download_example.add_argument( '-d', '--directory', metavar='<directory/>',
+    parser_download_pb_example.set_defaults(func=_download_pb_example)
+    parser_download_pb_example.add_argument( '-d', '--directory', metavar='<directory/>',
         default=EXAMPLE_DATA_DIR, help='destination directory for example data')
-    parser_download_example.add_argument('-n', '--n-samples', metavar='<int>',
+    parser_download_pb_example.add_argument('-n', '--n-samples', metavar='<int>',
         type=int, default=1, help='number of samples to download, max 4 (default: 1)')
+    
+    parser_download_ont_example = subparsers.add_parser('download-ont-example',
+        help='download an example dataset for dorado')
+    parser_download_ont_example.set_defaults(func=_download_ont_example)
+    parser_download_ont_example.add_argument( '-d', '--directory', metavar='<directory/>',
+        default=EXAMPLE_DATA_DIR, help='destination directory for example data')
 
     parser_check_tags = subparsers.add_parser('check-tags', help='check BAM for MM/ML tags')
     parser_check_tags.set_defaults(func=_check_tags)
     parser_check_tags.add_argument("bam", metavar="<reads.bam>",
         help="BAM file to check.")
     parser_check_tags.add_argument('-n', '--n-reads', metavar="<int>",
         type=int, default=1000, help="Number of reads to check (default: %(default)d].")
```

### Comparing `loreme-0.1.8/src/loreme/mean.py` & `loreme-0.1.9/src/loreme/mean.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.8/src/loreme/merge.py` & `loreme-0.1.9/src/loreme/merge.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.8/src/loreme/methylation_hist.py` & `loreme-0.1.9/src/loreme/methylation_hist.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.8/src/loreme/parse_gff.py` & `loreme-0.1.9/src/loreme/parse_gff.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.8/src/loreme/pbcpg.py` & `loreme-0.1.9/src/loreme/pbcpg.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.8/src/loreme/plot.py` & `loreme-0.1.9/src/loreme/plot.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.8/src/loreme/plot_bedtools.py` & `loreme-0.1.9/src/loreme/plot_bedtools.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.8/src/loreme/plot_genes.py` & `loreme-0.1.9/src/loreme/plot_genes.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.8/src/loreme/plot_repeats.py` & `loreme-0.1.9/src/loreme/plot_repeats.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.8/src/loreme/promoter_methylation.py` & `loreme-0.1.9/src/loreme/promoter_methylation.py`

 * *Files identical despite different names*

