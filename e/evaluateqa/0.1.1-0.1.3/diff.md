# Comparing `tmp/evaluateqa-0.1.1.tar.gz` & `tmp/evaluateqa-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evaluateqa-0.1.1.tar", max compression
+gzip compressed data, was "evaluateqa-0.1.3.tar", max compression
```

## Comparing `evaluateqa-0.1.1.tar` & `evaluateqa-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-04-24 12:38:02.469440 evaluateqa-0.1.1/LICENSE
--rw-r--r--   0        0        0      623 2023-04-24 14:40:56.945341 evaluateqa-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-24 13:26:29.451612 evaluateqa-0.1.1/evaluateqa/__init__.py
--rw-r--r--   0        0        0       65 2023-04-24 14:38:40.097600 evaluateqa-0.1.1/evaluateqa/mintaka/__init__.py
--rw-r--r--   0        0        0    11305 2023-04-26 12:08:17.595709 evaluateqa-0.1.1/evaluateqa/mintaka/evaluate.py
--rw-r--r--   0        0        0      498 2023-04-26 12:10:11.669847 evaluateqa-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1426 1970-01-01 00:00:00.000000 evaluateqa-0.1.1/setup.py
--rw-r--r--   0        0        0     1477 1970-01-01 00:00:00.000000 evaluateqa-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-13 14:56:58.033887 evaluateqa-0.1.3/LICENSE
+-rw-r--r--   0        0        0      623 2023-07-13 14:56:58.033887 evaluateqa-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 14:56:58.033887 evaluateqa-0.1.3/evaluateqa/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-13 14:56:58.033887 evaluateqa-0.1.3/evaluateqa/mintaka/__init__.py
+-rw-r--r--   0        0        0    12519 2023-07-13 15:42:08.320447 evaluateqa-0.1.3/evaluateqa/mintaka/evaluate.py
+-rw-r--r--   0        0        0      497 2023-07-13 15:43:27.471813 evaluateqa-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1476 1970-01-01 00:00:00.000000 evaluateqa-0.1.3/PKG-INFO
```

### Comparing `evaluateqa-0.1.1/LICENSE` & `evaluateqa-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `evaluateqa-0.1.1/README.md` & `evaluateqa-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `evaluateqa-0.1.1/evaluateqa/mintaka/evaluate.py` & `evaluateqa-0.1.3/evaluateqa/mintaka/evaluate.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,21 +36,25 @@
 
 
 def _validate_mode(mode: str):
     if mode not in ["kg", "text"]:
         raise ValueError(f"mode must be kg or text, but {mode} was passed")
 
 
-def _validate_predictions(predictions: Dict[str, Union[str, int, float, List]]):
+def _validate_predictions(
+    predictions: Dict[str, Union[str, int, float, List]], mode: str
+):
     for key, val in predictions.items():
-        if not isinstance(key, str):
+        if mode == "text" and not isinstance(key, str):
             raise ValueError(
                 f"MINTAKA predictions keys must be str, but {key} was passed"
             )
-        if not (val is None or isinstance(val, (str, int, float, list))):
+        if mode == "kg" and not (
+            val is None or isinstance(val, (str, int, float, list))
+        ):
             raise ValueError(
                 f"MINTAKA predictions values must be str, int, float, list or None, but {val} was passed"
             )
 
 
 @MEMORY.cache
 def _load_mintaka_data(split: str) -> Dict:
@@ -86,15 +90,15 @@
     -------
     pd.DataFrame
         DataFrame with at least 6 columns: id, answer, pred, exact_match, f1 and hits1
     """
     _validate_data_split(split)
     _validate_lang(lang)
     _validate_mode(mode)
-    _validate_predictions(predictions)
+    _validate_predictions(predictions, mode)
 
     target_data = _load_mintaka_data(split)
     target_df = pd.DataFrame(target_data)
     target_df["answer"] = target_df["answer"].apply(
         lambda answer: _format_answers(answer, mode, lang)
     )
 
@@ -115,74 +119,93 @@
 
 def evaluate(
     predictions: Optional[Dict[str, Union[str, int, float, List, None]]] = None,
     df_with_predictions: Optional[pd.DataFrame] = None,
     split: str = "test",
     mode: str = "text",
     lang: Optional[str] = "en",
+    groupbycols: List[str] = ["complexityType", "category"],
 ) -> Dict[str, float]:
     """evaluate - main method for evaluate your predicions
 
     Parameters
     ----------
     predictions : Optional[Dict[str, Union[str, int, float, List, None]]], optional
         Dict with key - id of question and value - your answer.
         For kg mode it can be entity id, number, string or list of all prevous types,
         by default None
     df_with_predictions : Optional[pd.DataFrame], optional
-        Instead of predictions, can be used precomputed dataframe with dataset 
+        Instead of predictions, can be used precomputed dataframe with dataset
         and prediciton that can be calculated in calculate_metrics_for_prediction method,
         by default None
     split : str, optional
         train, validation or test, by default "test"
     mode : str, optional
         'kg' or 'text' for Knowledge Graph or open question text mode,
         by default "text"
     lang : Optional[str], optional
         Language of used questions,
         can be "en", "ar", "de", "es", "fr", "hi", "it", "ja" or "pt"
         by default "en"
+    groupbycols : list[str], optional
+        List of df_with_predictions columns that was used for grouping results and calculate metrics for different groups.
 
     Returns
     -------
     Dict[str, float]
         Dict with computed metrics. For all dataset in 'All' field,
         for different splits in corresponding fields: complexityType and category
     """
     if predictions is None and df_with_predictions is None:
-        raise ValueError('predictions or df_with_predictions argumet must be provided')
+        raise ValueError("predictions or df_with_predictions argumet must be provided")
     elif predictions is not None and df_with_predictions is None:
         df_with_predictions = calculate_metrics_for_prediction(
             predictions,
             split,
             mode,
             lang,
         )
     elif predictions is not None and df_with_predictions is not None:
-        raise ValueError('predictions and df_with_predictions can not be used at the same call')
+        raise ValueError(
+            "predictions and df_with_predictions can not be used at the same call"
+        )
 
     results = {
         "All": {
             "exact_match": df_with_predictions["exact_match"].mean(),
+            "exact_match Number Correct Answer Of": (
+                df_with_predictions["exact_match"].sum(),
+                df_with_predictions["exact_match"].index.size,
+            ),
             "f1": df_with_predictions["f1"].mean(),
             "hits1": df_with_predictions["hits1"].mean(),
+            "hits1 Number Correct Answer Of": (
+                df_with_predictions["hits1"].sum(),
+                df_with_predictions["hits1"].index.size,
+            ),
         }
     }
-    results["complexityType"] = (
-        df_with_predictions.groupby("complexityType")[["exact_match", "f1", "hits1"]]
-        .mean()
-        .transpose()
-        .to_dict()
-    )
-    results["category"] = (
-        df_with_predictions.groupby("category")[["exact_match", "f1", "hits1"]]
-        .mean()
-        .transpose()
-        .to_dict()
-    )
+    for groupbycol in groupbycols:
+        results[groupbycol] = {}
+        for group_name, group in df_with_predictions.groupby(groupbycol):
+            results_type_metric = {}
+            results_type_metric["exact_match"] = group["exact_match"].mean()
+            results_type_metric["exact_match Number Correct Answer Of"] = (
+                group["exact_match"].sum(),
+                group["exact_match"].count(),
+            )
+            results_type_metric["f1"] = group["f1"].mean()
+            results_type_metric["hits1"] = group["hits1"].mean()
+            results_type_metric["hits1 Number Correct Answer Of"] = (
+                group["hits1"].sum(),
+                group["hits1"].count(),
+            )
+
+            results[groupbycol][group_name] = results_type_metric
+
     return results
 
 
 def _format_answers(answer: dict, mode: str, lang: str) -> Union[list, str, None]:
     """
     Formats answers from the Mintaka test set based on evaluation mode (kg or text)
     Args:
@@ -263,14 +286,16 @@
     Args:
         pred: predicted answer from a model
         answer: answer from the Mintaka test set
         mode: mode of evaluation (kg or text)
     Returns:
         1 if the prediction exactly matches the answer, else 0
     """
+    if pd.isnull(pred):
+        return False
     if mode == "text" and pred and answer:
         pred = normalize_and_tokenize_text(pred)
         answer = normalize_and_tokenize_text(answer)
         for i in range(0, len(pred) - len(answer) + 1):
             if answer == pred[i : i + len(answer)]:
                 return True
         return False
@@ -284,14 +309,16 @@
     Args:
         pred: predicted answer from a model
         answer: answer from the Mintaka test set
         mode: mode of evaluation (kg or text)
     Returns:
         An F1 score based on the tokens in a text answer or the list elements in a KG answer
     """
+    if pd.isnull(pred):
+        return False
     if not answer or not pred:
         return int(answer == pred)
     if mode == "text":
         pred = pred.split()
         answer = answer.split()
     common = collections.Counter(pred) & collections.Counter(answer)
     num_same = sum(common.values())
```

### Comparing `evaluateqa-0.1.1/PKG-INFO` & `evaluateqa-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evaluateqa
-Version: 0.1.1
+Version: 0.1.3
 Summary: 
 Home-page: https://github.com/MihailSalnikov/EvaluateQA
 License: MIT
 Keywords: QA,KGQA,ODQA,Evaluate
 Author: Mikhail Salnikov
 Author-email: 2613180+MihailSalnikov@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: joblib (>=1.2.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
-Requires-Dist: regex (>=2023.3.23,<2024.0.0)
+Requires-Dist: regex (>=2023.6.3,<2024.0.0)
 Requires-Dist: ujson (>=5.7.0,<6.0.0)
 Project-URL: Repository, https://github.com/MihailSalnikov/EvaluateQA
 Description-Content-Type: text/markdown
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # EvaluateQA
```

