# Comparing `tmp/forust-0.2.8.tar.gz` & `tmp/forust-0.2.9.tar.gz`

## Comparing `forust-0.2.8.tar` & `forust-0.2.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 forust-0.2.8/local_dependencies/forust-ml/Cargo.toml
--rw-r--r--   0      501       20     5608 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/.github/workflows/CI.yml
--rw-r--r--   0      501       20      268 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/.gitignore
--rw-r--r--   0      501       20      320 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/.pre-commit-config.yaml
--rw-r--r--   0      501       20     3242 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/CONTRIBUTING.md
--rw-r--r--   0      501       20    11341 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/LICENSE
--rw-r--r--   0      501       20    15541 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/README.md
--rw-r--r--   0      501       20     4228 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/benches/forust_benchmarks.rs
--rw-r--r--   0      501       20   452243 2023-05-18 18:52:22.000000 forust-0.2.8/local_dependencies/forust-ml/dist/forust-0.2.8-cp39-cp39-macosx_10_7_x86_64.whl
--rw-r--r--   0      501       20   764121 2023-05-18 18:51:20.000000 forust-0.2.8/local_dependencies/forust-ml/dist/forust-0.2.8.tar.gz
--rw-r--r--   0      501       20    16121 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/resources/pdp_plot_age.png
--rw-r--r--   0      501       20    10758 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png
--rw-r--r--   0      501       20    57018 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/resources/titanic.csv
--rw-r--r--   0      501       20   655700 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/resources/tree-image-crop.png
--rw-r--r--   0      501       20     2556 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/rs-example.md
--rw-r--r--   0      501       20     1179 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/scripts/make_resources.py
--rw-r--r--   0      501       20       53 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/scripts/run-python-tests.ps1
--rw-r--r--   0      501       20       53 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/scripts/run-python-tests.sh
--rw-r--r--   0      501       20     5610 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/binning.rs
--rw-r--r--   0      501       20      248 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/constraints.rs
--rw-r--r--   0      501       20     9944 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/data.rs
--rw-r--r--   0      501       20      562 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/errors.rs
--rw-r--r--   0      501       20    36231 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/gradientbooster.rs
--rw-r--r--   0      501       20     9357 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/histogram.rs
--rw-r--r--   0      501       20      355 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/lib.rs
--rw-r--r--   0      501       20     8847 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/metric.rs
--rw-r--r--   0      501       20     6060 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/node.rs
--rw-r--r--   0      501       20     4868 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/objective.rs
--rw-r--r--   0      501       20     4018 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/partial_dependence.rs
--rw-r--r--   0      501       20     3458 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/sampler.rs
--rw-r--r--   0      501       20    34995 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/splitter.rs
--rw-r--r--   0      501       20    21713 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/tree.rs
--rw-r--r--   0      501       20    29703 2023-05-18 18:47:19.000000 forust-0.2.8/local_dependencies/forust-ml/src/utils.rs
--rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 forust-0.2.8/Cargo.toml
--rw-r--r--   0      501       20      685 2023-05-18 18:47:19.000000 forust-0.2.8/.gitignore
--rw-r--r--   0      501       20    15541 2023-05-18 18:48:09.000000 forust-0.2.8/README.md
--rw-r--r--   0      501       20    27199 2023-05-18 18:47:19.000000 forust-0.2.8/forust/__init__.py
--rw-r--r--   0      501       20      785 2023-05-18 18:47:19.000000 forust-0.2.8/pyproject.toml
--rw-r--r--   0      501       20     7353 2023-05-18 18:47:19.000000 forust-0.2.8/scratch.py
--rw-r--r--   0      501       20    12899 2023-05-18 18:47:19.000000 forust-0.2.8/src/lib.rs
--rw-r--r--   0      501       20    14838 2023-05-18 18:47:19.000000 forust-0.2.8/tests/test_booster.py
--rw-r--r--   0      501       20    11341 2023-05-18 18:48:09.000000 forust-0.2.8/LICENSE
--rw-r--r--   0      501       20    15541 2023-05-18 18:48:09.000000 forust-0.2.8/README.md
--rw-r--r--   0        0        0    16325 1970-01-01 00:00:00.000000 forust-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 forust-0.2.9/local_dependencies/forust-ml/Cargo.toml
+-rw-r--r--   0      501       20     5608 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      268 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/.gitignore
+-rw-r--r--   0      501       20      320 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/.pre-commit-config.yaml
+-rw-r--r--   0      501       20     3242 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/CONTRIBUTING.md
+-rw-r--r--   0      501       20    11341 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/LICENSE
+-rw-r--r--   0      501       20    15541 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/README.md
+-rw-r--r--   0      501       20     4228 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/benches/forust_benchmarks.rs
+-rw-r--r--   0      501       20   451958 2023-05-18 19:43:02.000000 forust-0.2.9/local_dependencies/forust-ml/dist/forust-0.2.9-cp310-cp310-macosx_10_7_x86_64.whl
+-rw-r--r--   0      501       20   764143 2023-05-18 19:41:56.000000 forust-0.2.9/local_dependencies/forust-ml/dist/forust-0.2.9.tar.gz
+-rw-r--r--   0      501       20    16121 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/resources/pdp_plot_age.png
+-rw-r--r--   0      501       20    10758 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png
+-rw-r--r--   0      501       20    57018 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/resources/titanic.csv
+-rw-r--r--   0      501       20   655700 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/resources/tree-image-crop.png
+-rw-r--r--   0      501       20     2556 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/rs-example.md
+-rw-r--r--   0      501       20     1179 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/scripts/make_resources.py
+-rw-r--r--   0      501       20       53 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/scripts/run-python-tests.ps1
+-rw-r--r--   0      501       20       53 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/scripts/run-python-tests.sh
+-rw-r--r--   0      501       20     5610 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/src/binning.rs
+-rw-r--r--   0      501       20      248 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/src/constraints.rs
+-rw-r--r--   0      501       20     9944 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/src/data.rs
+-rw-r--r--   0      501       20      562 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/src/errors.rs
+-rw-r--r--   0      501       20    36401 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/src/gradientbooster.rs
+-rw-r--r--   0      501       20     9357 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/src/histogram.rs
+-rw-r--r--   0      501       20      355 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/src/lib.rs
+-rw-r--r--   0      501       20     8847 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/src/metric.rs
+-rw-r--r--   0      501       20     6060 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/src/node.rs
+-rw-r--r--   0      501       20     4868 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/src/objective.rs
+-rw-r--r--   0      501       20     4018 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/src/partial_dependence.rs
+-rw-r--r--   0      501       20     3458 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/src/sampler.rs
+-rw-r--r--   0      501       20    34995 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/src/splitter.rs
+-rw-r--r--   0      501       20    21713 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/src/tree.rs
+-rw-r--r--   0      501       20    29703 2023-05-18 19:37:58.000000 forust-0.2.9/local_dependencies/forust-ml/src/utils.rs
+-rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 forust-0.2.9/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-05-18 19:37:58.000000 forust-0.2.9/.gitignore
+-rw-r--r--   0      501       20    15541 2023-05-18 19:38:32.000000 forust-0.2.9/README.md
+-rw-r--r--   0      501       20    27199 2023-05-18 19:37:58.000000 forust-0.2.9/forust/__init__.py
+-rw-r--r--   0      501       20      785 2023-05-18 19:37:58.000000 forust-0.2.9/pyproject.toml
+-rw-r--r--   0      501       20     7353 2023-05-18 19:37:58.000000 forust-0.2.9/scratch.py
+-rw-r--r--   0      501       20    12899 2023-05-18 19:37:58.000000 forust-0.2.9/src/lib.rs
+-rw-r--r--   0      501       20    14838 2023-05-18 19:37:58.000000 forust-0.2.9/tests/test_booster.py
+-rw-r--r--   0      501       20    11341 2023-05-18 19:38:32.000000 forust-0.2.9/LICENSE
+-rw-r--r--   0      501       20    15541 2023-05-18 19:38:32.000000 forust-0.2.9/README.md
+-rw-r--r--   0        0        0    16325 1970-01-01 00:00:00.000000 forust-0.2.9/PKG-INFO
```

### Comparing `forust-0.2.8/local_dependencies/forust-ml/Cargo.toml` & `forust-0.2.9/local_dependencies/forust-ml/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "forust-ml"
-version = "0.2.8"
+version = "0.2.9"
 edition = "2021"
 authors = ["James Inlow <james.d.inlow@gmail.com>"]
 homepage = "https://github.com/jinlow/forust"
 description = "A lightweight gradient boosting implementation in Rust."
 license-file = "LICENSE"
 readme = "README.md"
 repository = "https://github.com/jinlow/forust"
```

### Comparing `forust-0.2.8/local_dependencies/forust-ml/.github/workflows/CI.yml` & `forust-0.2.9/local_dependencies/forust-ml/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/local_dependencies/forust-ml/CONTRIBUTING.md` & `forust-0.2.9/local_dependencies/forust-ml/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/local_dependencies/forust-ml/LICENSE` & `forust-0.2.9/local_dependencies/forust-ml/LICENSE`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/local_dependencies/forust-ml/README.md` & `forust-0.2.9/local_dependencies/forust-ml/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.2.8"
+forust-ml = "0.2.9"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 understand the XGBoost algorithm, additionally to have a fun project to work on
 in rust, and because I wanted to be able to experiment with adding new features
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
 package can be installed directly from [pypi](https://pypi.org/project/forust/
 ). ```shell pip install forust ``` To use in a rust project add the following
-to your Cargo.toml file. ```toml forust-ml = "0.2.8" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.9" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
```

### Comparing `forust-0.2.8/local_dependencies/forust-ml/benches/forust_benchmarks.rs` & `forust-0.2.9/local_dependencies/forust-ml/benches/forust_benchmarks.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/local_dependencies/forust-ml/resources/pdp_plot_age.png` & `forust-0.2.9/local_dependencies/forust-ml/resources/pdp_plot_age.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png` & `forust-0.2.9/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/local_dependencies/forust-ml/resources/titanic.csv` & `forust-0.2.9/local_dependencies/forust-ml/resources/titanic.csv`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/local_dependencies/forust-ml/resources/tree-image-crop.png` & `forust-0.2.9/local_dependencies/forust-ml/resources/tree-image-crop.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/local_dependencies/forust-ml/rs-example.md` & `forust-0.2.9/local_dependencies/forust-ml/rs-example.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## A Complete Rust Example
 
 To run this example, add the following code to your `Cargo.toml` file.
 ```toml
 [dependencies]
-forust-ml = "0.2.8"
+forust-ml = "0.2.9"
 polars = "0.24"
 reqwest = { version = "0.11", features = ["blocking"] }
 ```
 
 The following is a runable example using `polars` for data processing. The actual data manipulation can be performed with any tool, the only vital part, is the data be in column major format.
 ```rust
 use forust_ml::{GradientBooster, Matrix};
```

### Comparing `forust-0.2.8/local_dependencies/forust-ml/scripts/make_resources.py` & `forust-0.2.9/local_dependencies/forust-ml/scripts/make_resources.py`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/local_dependencies/forust-ml/src/binning.rs` & `forust-0.2.9/local_dependencies/forust-ml/src/binning.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/local_dependencies/forust-ml/src/data.rs` & `forust-0.2.9/local_dependencies/forust-ml/src/data.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/local_dependencies/forust-ml/src/errors.rs` & `forust-0.2.9/local_dependencies/forust-ml/src/errors.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/local_dependencies/forust-ml/src/gradientbooster.rs` & `forust-0.2.9/local_dependencies/forust-ml/src/gradientbooster.rs`

 * *Files 1% similar despite different names*

```diff
@@ -75,57 +75,63 @@
     pub min_leaf_weight: f32,
     pub base_score: f64,
     pub nbins: u16,
     pub parallel: bool,
     pub allow_missing_splits: bool,
     pub monotone_constraints: Option<ConstraintMap>,
     pub subsample: f32,
+    #[serde(default = "default_top_rate")]
     pub top_rate: f64,
+    #[serde(default = "default_other_rate")]
     pub other_rate: f64,
     pub seed: u64,
     #[serde(deserialize_with = "parse_missing")]
     pub missing: f64,
     pub create_missing_branch: bool,
     #[serde(default = "default_sample_method")]
     pub sample_method: SampleMethod,
     #[serde(default = "default_evaluation_metric")]
     pub evaluation_metric: Option<Metric>,
     #[serde(default = "default_early_stopping_rounds")]
     pub early_stopping_rounds: Option<usize>,
     #[serde(default = "default_evaluation_history")]
     pub evaluation_history: Option<RowMajorMatrix<f64>>,
-    #[serde(default = "default_prediction_iteration")]
+    #[serde(default = "default_best_iteration")]
     pub best_iteration: Option<usize>,
     /// number of trees to use when predicting,
     /// defaults to best_iteration if this is defined.
-    #[serde(default = "default_best_iteration")]
+    #[serde(default = "default_prediction_iteration")]
     pub prediction_iteration: Option<usize>,
     // Members internal to the booster object, and not parameters set by the user.
     // Trees is public, just to interact with it directly in the python wrapper.
     pub trees: Vec<Tree>,
     metadata: HashMap<String, String>,
 }
 
+fn default_top_rate() -> f64 {
+    0.1
+}
+fn default_other_rate() -> f64 {
+    0.2
+}
 fn default_sample_method() -> SampleMethod {
     SampleMethod::None
 }
 fn default_evaluation_metric() -> Option<Metric> {
     None
 }
 fn default_early_stopping_rounds() -> Option<usize> {
     None
 }
 fn default_evaluation_history() -> Option<RowMajorMatrix<f64>> {
     None
 }
-
 fn default_best_iteration() -> Option<usize> {
     None
 }
-
 fn default_prediction_iteration() -> Option<usize> {
     None
 }
 
 fn parse_missing<'de, D>(d: D) -> Result<f64, D::Error>
 where
     D: Deserializer<'de>,
```

### Comparing `forust-0.2.8/local_dependencies/forust-ml/src/histogram.rs` & `forust-0.2.9/local_dependencies/forust-ml/src/histogram.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/local_dependencies/forust-ml/src/metric.rs` & `forust-0.2.9/local_dependencies/forust-ml/src/metric.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/local_dependencies/forust-ml/src/node.rs` & `forust-0.2.9/local_dependencies/forust-ml/src/node.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/local_dependencies/forust-ml/src/objective.rs` & `forust-0.2.9/local_dependencies/forust-ml/src/objective.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/local_dependencies/forust-ml/src/partial_dependence.rs` & `forust-0.2.9/local_dependencies/forust-ml/src/partial_dependence.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/local_dependencies/forust-ml/src/sampler.rs` & `forust-0.2.9/local_dependencies/forust-ml/src/sampler.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/local_dependencies/forust-ml/src/splitter.rs` & `forust-0.2.9/local_dependencies/forust-ml/src/splitter.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/local_dependencies/forust-ml/src/tree.rs` & `forust-0.2.9/local_dependencies/forust-ml/src/tree.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/local_dependencies/forust-ml/src/utils.rs` & `forust-0.2.9/local_dependencies/forust-ml/src/utils.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/.gitignore` & `forust-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/README.md` & `forust-0.2.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.2.8"
+forust-ml = "0.2.9"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 understand the XGBoost algorithm, additionally to have a fun project to work on
 in rust, and because I wanted to be able to experiment with adding new features
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
 package can be installed directly from [pypi](https://pypi.org/project/forust/
 ). ```shell pip install forust ``` To use in a rust project add the following
-to your Cargo.toml file. ```toml forust-ml = "0.2.8" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.9" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
```

### Comparing `forust-0.2.8/forust/__init__.py` & `forust-0.2.9/forust/__init__.py`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/pyproject.toml` & `forust-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/scratch.py` & `forust-0.2.9/scratch.py`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/src/lib.rs` & `forust-0.2.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/tests/test_booster.py` & `forust-0.2.9/tests/test_booster.py`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/LICENSE` & `forust-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `forust-0.2.8/PKG-INFO` & `forust-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forust
-Version: 0.2.8
+Version: 0.2.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy>=1.21
 Requires-Dist: pandas>=1.3
 Requires-Dist: maturin; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
@@ -43,15 +43,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.2.8"
+forust-ml = "0.2.9"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: forust Version: 0.2.8 Classifier: Programming
+Metadata-Version: 2.1 Name: forust Version: 0.2.9 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy>=1.21 Requires-Dist: pandas>=1.3 Requires-Dist: maturin;
 extra == 'dev' Requires-Dist: pytest; extra == 'dev' Requires-Dist: seaborn;
 extra == 'dev' Requires-Dist: xgboost==1.6.1; extra == 'dev' Requires-Dist:
 scikit-learn; extra == 'dev' Provides-Extra: dev License-File: LICENSE Summary:
 A lightweight gradient boosting implementation in Rust. Keywords:
@@ -24,15 +24,15 @@
 understand the XGBoost algorithm, additionally to have a fun project to work on
 in rust, and because I wanted to be able to experiment with adding new features
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
 package can be installed directly from [pypi](https://pypi.org/project/forust/
 ). ```shell pip install forust ``` To use in a rust project add the following
-to your Cargo.toml file. ```toml forust-ml = "0.2.8" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.9" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
```

