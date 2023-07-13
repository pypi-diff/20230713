# Comparing `tmp/napari-tomotwin-0.2.0b0.tar.gz` & `tmp/napari-tomotwin-0.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-tomotwin-0.2.0b0.tar", last modified: Tue Jul 11 15:21:53 2023, max compression
+gzip compressed data, was "napari-tomotwin-0.2.0b1.tar", last modified: Thu Jul 13 15:23:53 2023, max compression
```

## Comparing `napari-tomotwin-0.2.0b0.tar` & `napari-tomotwin-0.2.0b1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:21:53.807930 napari-tomotwin-0.2.0b0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:21:53.787928 napari-tomotwin-0.2.0b0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:21:53.799929 napari-tomotwin-0.2.0b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-11 15:21:33.000000 napari-tomotwin-0.2.0b0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-11 15:21:33.000000 napari-tomotwin-0.2.0b0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:21:53.799929 napari-tomotwin-0.2.0b0/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-11 15:21:33.000000 napari-tomotwin-0.2.0b0/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-11 15:21:33.000000 napari-tomotwin-0.2.0b0/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-11 15:21:33.000000 napari-tomotwin-0.2.0b0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-07-11 15:21:33.000000 napari-tomotwin-0.2.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-11 15:21:33.000000 napari-tomotwin-0.2.0b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-11 15:21:53.807930 napari-tomotwin-0.2.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-11 15:21:33.000000 napari-tomotwin-0.2.0b0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-11 15:21:33.000000 napari-tomotwin-0.2.0b0/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-11 15:21:33.000000 napari-tomotwin-0.2.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-11 15:21:33.000000 napari-tomotwin-0.2.0b0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-11 15:21:53.807930 napari-tomotwin-0.2.0b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:21:53.799929 napari-tomotwin-0.2.0b0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:21:33.000000 napari-tomotwin-0.2.0b0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:21:53.803929 napari-tomotwin-0.2.0b0/src/napari_tomotwin/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 15:21:33.000000 napari-tomotwin-0.2.0b0/src/napari_tomotwin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:21:53.807930 napari-tomotwin-0.2.0b0/src/napari_tomotwin/_qt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:21:33.000000 napari-tomotwin-0.2.0b0/src/napari_tomotwin/_qt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:21:53.807930 napari-tomotwin-0.2.0b0/src/napari_tomotwin/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:21:33.000000 napari-tomotwin-0.2.0b0/src/napari_tomotwin/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 15:21:33.000000 napari-tomotwin-0.2.0b0/src/napari_tomotwin/_tests/test_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-11 15:21:53.000000 napari-tomotwin-0.2.0b0/src/napari_tomotwin/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-11 15:21:33.000000 napari-tomotwin-0.2.0b0/src/napari_tomotwin/load_umap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-11 15:21:33.000000 napari-tomotwin-0.2.0b0/src/napari_tomotwin/make_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-11 15:21:33.000000 napari-tomotwin-0.2.0b0/src/napari_tomotwin/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:21:53.807930 napari-tomotwin-0.2.0b0/src/napari_tomotwin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-11 15:21:53.000000 napari-tomotwin-0.2.0b0/src/napari_tomotwin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-11 15:21:53.000000 napari-tomotwin-0.2.0b0/src/napari_tomotwin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:21:53.000000 napari-tomotwin-0.2.0b0/src/napari_tomotwin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 15:21:53.000000 napari-tomotwin-0.2.0b0/src/napari_tomotwin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-11 15:21:53.000000 napari-tomotwin-0.2.0b0/src/napari_tomotwin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 15:21:53.000000 napari-tomotwin-0.2.0b0/src/napari_tomotwin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-11 15:21:33.000000 napari-tomotwin-0.2.0b0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:23:53.593481 napari-tomotwin-0.2.0b1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:23:53.589481 napari-tomotwin-0.2.0b1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:23:53.593481 napari-tomotwin-0.2.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-13 15:23:33.000000 napari-tomotwin-0.2.0b1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-13 15:23:33.000000 napari-tomotwin-0.2.0b1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:23:53.593481 napari-tomotwin-0.2.0b1/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-13 15:23:33.000000 napari-tomotwin-0.2.0b1/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-13 15:23:33.000000 napari-tomotwin-0.2.0b1/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-13 15:23:33.000000 napari-tomotwin-0.2.0b1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-07-13 15:23:33.000000 napari-tomotwin-0.2.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 15:23:33.000000 napari-tomotwin-0.2.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-13 15:23:53.593481 napari-tomotwin-0.2.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-13 15:23:33.000000 napari-tomotwin-0.2.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-13 15:23:33.000000 napari-tomotwin-0.2.0b1/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-13 15:23:33.000000 napari-tomotwin-0.2.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-13 15:23:33.000000 napari-tomotwin-0.2.0b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-13 15:23:53.593481 napari-tomotwin-0.2.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:23:53.593481 napari-tomotwin-0.2.0b1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:23:33.000000 napari-tomotwin-0.2.0b1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:23:53.593481 napari-tomotwin-0.2.0b1/src/napari_tomotwin/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-13 15:23:33.000000 napari-tomotwin-0.2.0b1/src/napari_tomotwin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:23:53.593481 napari-tomotwin-0.2.0b1/src/napari_tomotwin/_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:23:33.000000 napari-tomotwin-0.2.0b1/src/napari_tomotwin/_qt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:23:53.593481 napari-tomotwin-0.2.0b1/src/napari_tomotwin/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:23:33.000000 napari-tomotwin-0.2.0b1/src/napari_tomotwin/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 15:23:33.000000 napari-tomotwin-0.2.0b1/src/napari_tomotwin/_tests/test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-13 15:23:53.000000 napari-tomotwin-0.2.0b1/src/napari_tomotwin/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-13 15:23:33.000000 napari-tomotwin-0.2.0b1/src/napari_tomotwin/load_umap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-13 15:23:33.000000 napari-tomotwin-0.2.0b1/src/napari_tomotwin/make_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-13 15:23:33.000000 napari-tomotwin-0.2.0b1/src/napari_tomotwin/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:23:53.593481 napari-tomotwin-0.2.0b1/src/napari_tomotwin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-13 15:23:53.000000 napari-tomotwin-0.2.0b1/src/napari_tomotwin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-13 15:23:53.000000 napari-tomotwin-0.2.0b1/src/napari_tomotwin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:23:53.000000 napari-tomotwin-0.2.0b1/src/napari_tomotwin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-13 15:23:53.000000 napari-tomotwin-0.2.0b1/src/napari_tomotwin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-13 15:23:53.000000 napari-tomotwin-0.2.0b1/src/napari_tomotwin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 15:23:53.000000 napari-tomotwin-0.2.0b1/src/napari_tomotwin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-13 15:23:33.000000 napari-tomotwin-0.2.0b1/tox.ini
```

### Comparing `napari-tomotwin-0.2.0b0/.github/workflows/test_and_deploy.yml` & `napari-tomotwin-0.2.0b1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.2.0b0/.gitignore` & `napari-tomotwin-0.2.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.2.0b0/.napari-hub/config.yml` & `napari-tomotwin-0.2.0b1/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.2.0b0/.pre-commit-config.yaml` & `napari-tomotwin-0.2.0b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.2.0b0/LICENSE` & `napari-tomotwin-0.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.2.0b0/PKG-INFO` & `napari-tomotwin-0.2.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-tomotwin
-Version: 0.2.0b0
+Version: 0.2.0b1
 Summary: Several tools for the work with TomoTwin
 Home-page: https://github.com/MPI-Dortmund/napari-tomotwin
 Author: Thorsten Wagner
 Author-email: twa1@posteo.de
 License: MPL-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari-tomotwin-0.2.0b0/README.md` & `napari-tomotwin-0.2.0b1/README.md`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.2.0b0/setup.cfg` & `napari-tomotwin-0.2.0b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.2.0b0/src/napari_tomotwin/load_umap.py` & `napari-tomotwin-0.2.0b1/src/napari_tomotwin/load_umap.py`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.2.0b0/src/napari_tomotwin/make_targets.py` & `napari-tomotwin-0.2.0b1/src/napari_tomotwin/make_targets.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,23 @@
     sample = embeddings
     if len(sample)>max_embeddings:
         # For samples more than 50k it's way to slow and memory hungry.
         sample = embeddings.sample(max_embeddings)
         print(f"Your cluster size ({len(embeddings)}) is bigger then {max_embeddings}. Make a random sample to calculate medoid.")
     distance_matrix=cdist(sample,sample,metric='cosine') # its not the cosine similarity, rather a distance (its 0 in case of same embeddings)
     medoid_index = np.argmin(np.sum(distance_matrix,axis=0))
-    return embeddings.iloc[medoid_index,:]
+    return sample.iloc[medoid_index,:]
 
 def _get_avg_embedding(embeddings: pd.DataFrame) -> pd.DataFrame:
     target = embeddings.mean(axis=0)
     return target
 
 
 def _make_targets(embeddings: pd.DataFrame, clusters: pd.DataFrame, avg_func: Callable[[pd.DataFrame], npt.ArrayLike]) -> Tuple[pd.DataFrame, List[pd.DataFrame]]:
+    print("MEDOID!!!")
     targets = []
     sub_embeddings = []
     target_names = []
     for cluster in set(clusters):
         if cluster == 0:
             continue
         cluster_embeddings = embeddings.drop(columns=["X", "Y", "Z", "filepath"], errors="ignore").loc[clusters == cluster, :].astype(np.float32)
```

### Comparing `napari-tomotwin-0.2.0b0/src/napari_tomotwin/napari.yaml` & `napari-tomotwin-0.2.0b1/src/napari_tomotwin/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.2.0b0/src/napari_tomotwin.egg-info/PKG-INFO` & `napari-tomotwin-0.2.0b1/src/napari_tomotwin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-tomotwin
-Version: 0.2.0b0
+Version: 0.2.0b1
 Summary: Several tools for the work with TomoTwin
 Home-page: https://github.com/MPI-Dortmund/napari-tomotwin
 Author: Thorsten Wagner
 Author-email: twa1@posteo.de
 License: MPL-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari-tomotwin-0.2.0b0/src/napari_tomotwin.egg-info/SOURCES.txt` & `napari-tomotwin-0.2.0b1/src/napari_tomotwin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.2.0b0/tox.ini` & `napari-tomotwin-0.2.0b1/tox.ini`

 * *Files identical despite different names*

