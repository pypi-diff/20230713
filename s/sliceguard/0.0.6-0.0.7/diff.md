# Comparing `tmp/sliceguard-0.0.6.tar.gz` & `tmp/sliceguard-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliceguard-0.0.6.tar", last modified: Tue Jul 11 15:32:51 2023, max compression
+gzip compressed data, was "sliceguard-0.0.7.tar", last modified: Thu Jul 13 09:11:13 2023, max compression
```

## Comparing `sliceguard-0.0.6.tar` & `sliceguard-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 15:32:51.659112 sliceguard-0.0.6/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1065 2023-06-14 07:59:41.000000 sliceguard-0.0.6/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3862 2023-07-11 15:32:51.659112 sliceguard-0.0.6/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3207 2023-07-11 15:29:58.000000 sliceguard-0.0.6/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1086 2023-07-11 15:30:09.000000 sliceguard-0.0.6/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-11 15:32:51.659112 sliceguard-0.0.6/setup.cfg
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 15:32:51.659112 sliceguard-0.0.6/sliceguard/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       44 2023-07-05 08:28:25.000000 sliceguard-0.0.6/sliceguard/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     6129 2023-07-07 08:09:57.000000 sliceguard-0.0.6/sliceguard/detection.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2843 2023-07-11 15:29:58.000000 sliceguard-0.0.6/sliceguard/embedding_utils.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4378 2023-07-11 15:29:58.000000 sliceguard-0.0.6/sliceguard/explanation.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    10187 2023-07-11 15:29:58.000000 sliceguard-0.0.6/sliceguard/sliceguard.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     8224 2023-07-11 15:29:58.000000 sliceguard-0.0.6/sliceguard/utils.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 15:32:51.659112 sliceguard-0.0.6/sliceguard.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3862 2023-07-11 15:32:51.000000 sliceguard-0.0.6/sliceguard.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      374 2023-07-11 15:32:51.000000 sliceguard-0.0.6/sliceguard.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-11 15:32:51.000000 sliceguard-0.0.6/sliceguard.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      262 2023-07-11 15:32:51.000000 sliceguard-0.0.6/sliceguard.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       11 2023-07-11 15:32:51.000000 sliceguard-0.0.6/sliceguard.egg-info/top_level.txt
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 15:32:51.659112 sliceguard-0.0.6/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4742 2023-07-11 15:29:58.000000 sliceguard-0.0.6/tests/test_sliceguard.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 09:11:13.050232 sliceguard-0.0.7/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1065 2023-06-14 07:59:41.000000 sliceguard-0.0.7/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4146 2023-07-13 09:11:13.050232 sliceguard-0.0.7/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3491 2023-07-13 08:54:42.000000 sliceguard-0.0.7/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1064 2023-07-13 08:55:35.000000 sliceguard-0.0.7/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-13 09:11:13.050232 sliceguard-0.0.7/setup.cfg
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 09:11:13.050232 sliceguard-0.0.7/sliceguard/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       44 2023-07-05 08:28:25.000000 sliceguard-0.0.7/sliceguard/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6129 2023-07-07 08:09:57.000000 sliceguard-0.0.7/sliceguard/detection.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2843 2023-07-11 15:29:58.000000 sliceguard-0.0.7/sliceguard/embedding_utils.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4378 2023-07-11 15:29:58.000000 sliceguard-0.0.7/sliceguard/explanation.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    10671 2023-07-13 08:54:42.000000 sliceguard-0.0.7/sliceguard/sliceguard.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     8510 2023-07-13 08:54:42.000000 sliceguard-0.0.7/sliceguard/utils.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 09:11:13.050232 sliceguard-0.0.7/sliceguard.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4146 2023-07-13 09:11:13.000000 sliceguard-0.0.7/sliceguard.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      374 2023-07-13 09:11:13.000000 sliceguard-0.0.7/sliceguard.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-13 09:11:13.000000 sliceguard-0.0.7/sliceguard.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      247 2023-07-13 09:11:13.000000 sliceguard-0.0.7/sliceguard.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       11 2023-07-13 09:11:13.000000 sliceguard-0.0.7/sliceguard.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 09:11:13.050232 sliceguard-0.0.7/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4742 2023-07-11 15:29:58.000000 sliceguard-0.0.7/tests/test_sliceguard.py
```

### Comparing `sliceguard-0.0.6/LICENSE` & `sliceguard-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.6/PKG-INFO` & `sliceguard-0.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliceguard
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library for detecting critical data slices in structured and unstructured data based on features, metadata and model predictions.
 Author-email: Renumics GmbH <info@renumics.com>, Daniel Klitzke <daniel.klitzke@renumics.com>
 Project-URL: Homepage, https://github.com/Renumics/sliceguard
 Project-URL: Bug Tracker, https://github.com/Renumics/sliceguard/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -72,14 +72,17 @@
 
 [Evaluating automatic speech recognition models beyond global metrics — A tutorial using OpenAI’s Whisper as an example](https://medium.com/@daniel-klitzke/evaluating-automatic-speech-recognition-models-beyond-global-metrics-a-tutorial-using-openais-54b63c4dadbd)
 
 ## 🗺️ Public Roadmap
 - [x] Detection of problematic data slices
 - [x] Basic explanation of found issues via feature importances
 - [x] Limited embedding computation for images, audio, text
+- [x] Extended embedding support, e.g., more embedding models and allow precomputed embeddings
+- [ ] Speed up embedding computation using datasets library
+- [ ] Soft Dependencies for embedding computation as torch dependencies are large
+- [ ] Improve Spotlight report with embeddings in simmap and histogram for univariate analysis
 - [ ] Extensive documentation and examples for common cases
 - [ ] Data connectors for faster application on common data formats
 - [ ] Improved explanations for found issues, e.g., via SHAP
-- [ ] Extended embedding support, e.g., more embedding models and allow precomputed embeddings
 - [ ] Generation of a summary report doing predefined checks
 - [ ] Allow for control features in order to account for expected variations when running checks
-- [ ] Improved issue detection algorithm, avoiding duplicate detections of similar problems
+- [ ] Improved issue detection algorithm, avoiding duplicate detections of similar problems and outliers influencing the segment detection
```

### Comparing `sliceguard-0.0.6/README.md` & `sliceguard-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -58,14 +58,17 @@
 
 [Evaluating automatic speech recognition models beyond global metrics — A tutorial using OpenAI’s Whisper as an example](https://medium.com/@daniel-klitzke/evaluating-automatic-speech-recognition-models-beyond-global-metrics-a-tutorial-using-openais-54b63c4dadbd)
 
 ## 🗺️ Public Roadmap
 - [x] Detection of problematic data slices
 - [x] Basic explanation of found issues via feature importances
 - [x] Limited embedding computation for images, audio, text
+- [x] Extended embedding support, e.g., more embedding models and allow precomputed embeddings
+- [ ] Speed up embedding computation using datasets library
+- [ ] Soft Dependencies for embedding computation as torch dependencies are large
+- [ ] Improve Spotlight report with embeddings in simmap and histogram for univariate analysis
 - [ ] Extensive documentation and examples for common cases
 - [ ] Data connectors for faster application on common data formats
 - [ ] Improved explanations for found issues, e.g., via SHAP
-- [ ] Extended embedding support, e.g., more embedding models and allow precomputed embeddings
 - [ ] Generation of a summary report doing predefined checks
 - [ ] Allow for control features in order to account for expected variations when running checks
-- [ ] Improved issue detection algorithm, avoiding duplicate detections of similar problems
+- [ ] Improved issue detection algorithm, avoiding duplicate detections of similar problems and outliers influencing the segment detection
```

### Comparing `sliceguard-0.0.6/pyproject.toml` & `sliceguard-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sliceguard"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Renumics GmbH", email="info@renumics.com"},
   { name="Daniel Klitzke", email="daniel.klitzke@renumics.com"}
 ]
 description = "A library for detecting critical data slices in structured and unstructured data based on features, metadata and model predictions."
 readme = "README.md"
 requires-python = ">=3.7"
@@ -22,16 +22,15 @@
   "umap-learn >= 0.5.3",
   "transformers >= 4.30.2",
   "torch >= 2.0.1",
   "torchaudio >= 2.0.2",
   "sentence-transformers >= 2.2.1",
   "tqdm >= 4.65.0",
   "Pillow >= 9.5.0",
-  "renumics-spotlight >= 1.3.0rc3",
-  "pydantic < 2.0.0",
+  "renumics-spotlight >= 1.3.0rc4",
   "plotly >= 5.15.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Renumics/sliceguard"
 "Bug Tracker" = "https://github.com/Renumics/sliceguard/issues"
```

### Comparing `sliceguard-0.0.6/sliceguard/detection.py` & `sliceguard-0.0.7/sliceguard/detection.py`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.6/sliceguard/embedding_utils.py` & `sliceguard-0.0.7/sliceguard/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.6/sliceguard/explanation.py` & `sliceguard-0.0.7/sliceguard/explanation.py`

 * *Files identical despite different names*

### Comparing `sliceguard-0.0.6/sliceguard/sliceguard.py` & `sliceguard-0.0.7/sliceguard/sliceguard.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import pandas as pd
 import numpy as np
 import plotly.express as px
 
 from renumics import spotlight
 from renumics.spotlight.analysis.typing import DataIssue
+from renumics.spotlight import Embedding
 from renumics.spotlight import layout
 
 from .utils import infer_feature_types, encode_normalize_features
 from .detection import generate_metric_frames, detect_issues
 from .explanation import explain_clusters
 
 
@@ -165,14 +166,21 @@
         # Some basic checks
         assert self._issue_df is not None
         assert len(self._df) == len(self._issue_df)
         assert all(self._df.index == self._issue_df.index)
 
         df = pd.concat((self._df, self._issue_df), axis=1)
 
+        # Insert embeddings if they were computed
+        embedding_dtypes = {}
+        for embedding_col, embeddings in self.embeddings.items():
+            report_col_name = f"sg_emb_{embedding_col}"
+            df[report_col_name] = [e.tolist() for e in embeddings]
+            embedding_dtypes[report_col_name] = Embedding
+
         data_issue_severity = []
         data_issues = []
         for issue in self._issue_df["issue"].unique():
             if issue == -1:
                 continue
             issue_rows = np.where(self._issue_df["issue"] == issue)[
                 0
@@ -198,25 +206,26 @@
 
         data_issue_order = np.argsort(data_issue_severity)
         if self._metric_mode == "min":
             data_issue_order = data_issue_order[::-1]
 
         spotlight.show(
             df,
-            dtype=spotlight_dtype,
+            dtype={ **spotlight_dtype, **embedding_dtypes},
             issues=np.array(data_issues)[data_issue_order].tolist(),
             layout=layout.layout(
                 [
                     [layout.table()],
                     [layout.similaritymap()],
                     [layout.histogram()],
                 ],
                 [[layout.widgets.Inspector()], [layout.widgets.Issues()]],
             ),
         )
+        return df # Return the create report dataframe in case caller wants to process it
 
     def _plot_clustering_overview(self):
         """
         Debugging method to get an overview on the last clustering structure.
         """
         # for i in range(len(self._clustering_cols)):
         # cur_clustering_cols = self._clustering_cols[:i+1]
```

### Comparing `sliceguard-0.0.6/sliceguard/utils.py` & `sliceguard-0.0.7/sliceguard/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -117,60 +117,62 @@
             ordinal_data = ordinal_data / (
                 len(feature_order) - 1
             )  # normalize with unique category count to make compatible with range of one hot encoding
             encoded_data = np.concatenate((encoded_data, ordinal_data), axis=1)
         elif feature_type == "raw" or feature_type == "embedding":
             # Print model that will be used for computing embeddings
             if col in df.columns and col not in precomputed_embeddings:
-                model_name_param = (
-                    {"model_name": embedding_models[col]}
+                hf_model_params = (
+                    {
+                        "model_name": embedding_models[col],
+                        "hf_auth_token": hf_auth_token,
+                    }
                     if col in embedding_models
                     else {}
                 )
-                if "model_name" in model_name_param:
+                if "model_name" in hf_model_params:
                     print(
-                        f"Using {model_name_param['model_name']} for computing embeddings for feature {col}."
+                        f"Using {hf_model_params['model_name']} for computing embeddings for feature {col}."
                     )
                 else:
                     print(
                         f"Using default model for computing embeddings for feature {col}."
                     )
             # Set first entry as for checking type of raw data.
             if col in df.columns:
                 first_entry = df[col].iloc[0]
             if col in precomputed_embeddings:  # use precomputed embeddings when given
                 embeddings = precomputed_embeddings[col]
                 assert len(embeddings) == len(df)
+                raw_embeddings[col] = embeddings # also save them here as they are used in report
             elif first_entry.lower().endswith(
                 ".wav"
             ):  # TODO: Improve data type inference for raw data
                 embeddings = generate_audio_embeddings(
-                    df[col].values, **model_name_param
+                    df[col].values, **hf_model_params
                 )
                 raw_embeddings[col] = embeddings
             elif (
                 first_entry.lower().endswith(".jpg")
                 or first_entry.lower().endswith(".jpeg")
                 or first_entry.lower().endswith(".png")
             ):
                 embeddings = generate_image_embeddings(
-                    df[col].values, **model_name_param
+                    df[col].values, **hf_model_params
                 )
                 raw_embeddings[col] = embeddings
             else:  # Treat as text if nothing known
-                embeddings = generate_text_embeddings(
-                    df[col].values, **model_name_param
-                )
+                embeddings = generate_text_embeddings(df[col].values, **hf_model_params)
                 raw_embeddings[col] = embeddings
 
             # TODO: Potentially filter out entries without valid embedding or replace with mean?
             reduced_embeddings = umap.UMAP(
                 # n_neighbors=min(len(df) - 1, 30),
                 # min_dist=0.0,
-                n_components=2,
+                n_components=8, # TODO: Do not hardcode this, probably determine based on embedding size and variance. Also, check implications on normlization.
                 random_state=42,
             ).fit_transform(embeddings)
 
             # TODO: Check if normalization makes sense. Probably do not normalize dimensiosn indenpendently!
             # reduced_embeddings = RobustScaler(
             #     quantile_range=(2.5, 97.5)
             # ).fit_transform(
```

### Comparing `sliceguard-0.0.6/sliceguard.egg-info/PKG-INFO` & `sliceguard-0.0.7/sliceguard.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliceguard
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library for detecting critical data slices in structured and unstructured data based on features, metadata and model predictions.
 Author-email: Renumics GmbH <info@renumics.com>, Daniel Klitzke <daniel.klitzke@renumics.com>
 Project-URL: Homepage, https://github.com/Renumics/sliceguard
 Project-URL: Bug Tracker, https://github.com/Renumics/sliceguard/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -72,14 +72,17 @@
 
 [Evaluating automatic speech recognition models beyond global metrics — A tutorial using OpenAI’s Whisper as an example](https://medium.com/@daniel-klitzke/evaluating-automatic-speech-recognition-models-beyond-global-metrics-a-tutorial-using-openais-54b63c4dadbd)
 
 ## 🗺️ Public Roadmap
 - [x] Detection of problematic data slices
 - [x] Basic explanation of found issues via feature importances
 - [x] Limited embedding computation for images, audio, text
+- [x] Extended embedding support, e.g., more embedding models and allow precomputed embeddings
+- [ ] Speed up embedding computation using datasets library
+- [ ] Soft Dependencies for embedding computation as torch dependencies are large
+- [ ] Improve Spotlight report with embeddings in simmap and histogram for univariate analysis
 - [ ] Extensive documentation and examples for common cases
 - [ ] Data connectors for faster application on common data formats
 - [ ] Improved explanations for found issues, e.g., via SHAP
-- [ ] Extended embedding support, e.g., more embedding models and allow precomputed embeddings
 - [ ] Generation of a summary report doing predefined checks
 - [ ] Allow for control features in order to account for expected variations when running checks
-- [ ] Improved issue detection algorithm, avoiding duplicate detections of similar problems
+- [ ] Improved issue detection algorithm, avoiding duplicate detections of similar problems and outliers influencing the segment detection
```

### Comparing `sliceguard-0.0.6/tests/test_sliceguard.py` & `sliceguard-0.0.7/tests/test_sliceguard.py`

 * *Files identical despite different names*

