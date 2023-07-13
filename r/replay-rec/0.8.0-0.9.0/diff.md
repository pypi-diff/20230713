# Comparing `tmp/replay-rec-0.8.0.tar.gz` & `tmp/replay-rec-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replay-rec-0.8.0.tar", max compression
+gzip compressed data, was "replay-rec-0.9.0.tar", max compression
```

## Comparing `replay-rec-0.8.0.tar` & `replay-rec-0.9.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0    11344 2021-12-06 14:15:54.516529 replay-rec-0.8.0/LICENSE
--rw-r--r--   0        0        0      628 2021-12-06 14:15:54.516737 replay-rec-0.8.0/README.md
--rw-r--r--   0        0        0     1767 2021-12-06 14:17:33.786925 replay-rec-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      112 2021-12-06 14:15:54.625561 replay-rec-0.8.0/replay/__init__.py
--rw-r--r--   0        0        0     1240 2021-12-06 14:15:54.625794 replay-rec-0.8.0/replay/constants.py
--rw-r--r--   0        0        0    14159 2021-12-06 14:15:54.626054 replay-rec-0.8.0/replay/data_preparator.py
--rw-r--r--   0        0        0     2668 2021-12-06 14:15:54.626222 replay-rec-0.8.0/replay/distributions.py
--rw-r--r--   0        0        0     7158 2021-12-06 14:15:54.626398 replay-rec-0.8.0/replay/experiment.py
--rw-r--r--   0        0        0    14031 2021-12-06 14:15:54.626584 replay-rec-0.8.0/replay/filters.py
--rw-r--r--   0        0        0     1574 2021-12-06 14:15:54.626769 replay-rec-0.8.0/replay/metrics/__init__.py
--rwxr-xr-x   0        0        0     9277 2021-12-06 14:15:54.626983 replay-rec-0.8.0/replay/metrics/base_metric.py
--rw-r--r--   0        0        0     3194 2021-12-06 14:15:54.627164 replay-rec-0.8.0/replay/metrics/coverage.py
--rw-r--r--   0        0        0      679 2021-12-06 14:15:54.627318 replay-rec-0.8.0/replay/metrics/hitrate.py
--rw-r--r--   0        0        0      984 2021-12-06 14:15:54.627495 replay-rec-0.8.0/replay/metrics/map.py
--rw-r--r--   0        0        0      878 2021-12-06 14:15:54.627635 replay-rec-0.8.0/replay/metrics/mrr.py
--rw-r--r--   0        0        0     1925 2021-12-06 14:15:54.627764 replay-rec-0.8.0/replay/metrics/ndcg.py
--rw-r--r--   0        0        0      679 2021-12-06 14:15:54.627948 replay-rec-0.8.0/replay/metrics/precision.py
--rw-r--r--   0        0        0      722 2021-12-06 14:15:54.628095 replay-rec-0.8.0/replay/metrics/recall.py
--rw-r--r--   0        0        0     2085 2021-12-06 14:15:54.628207 replay-rec-0.8.0/replay/metrics/rocauc.py
--rw-r--r--   0        0        0     2635 2021-12-06 14:15:54.628352 replay-rec-0.8.0/replay/metrics/surprisal.py
--rw-r--r--   0        0        0     2679 2021-12-06 14:15:54.628523 replay-rec-0.8.0/replay/metrics/unexpectedness.py
--rw-r--r--   0        0        0     2685 2021-12-06 14:15:54.628636 replay-rec-0.8.0/replay/model_handler.py
--rw-r--r--   0        0        0     1110 2021-12-06 14:15:54.628804 replay-rec-0.8.0/replay/models/__init__.py
--rw-r--r--   0        0        0     6105 2021-12-06 14:15:54.628990 replay-rec-0.8.0/replay/models/admm_slim.py
--rw-r--r--   0        0        0     3916 2021-12-06 14:15:54.629149 replay-rec-0.8.0/replay/models/als.py
--rw-r--r--   0        0        0     9444 2021-12-06 14:15:54.629300 replay-rec-0.8.0/replay/models/association_rules.py
--rw-r--r--   0        0        0    55633 2021-12-06 14:15:54.629774 replay-rec-0.8.0/replay/models/base_rec.py
--rw-r--r--   0        0        0    10396 2021-12-06 14:15:54.630009 replay-rec-0.8.0/replay/models/base_torch_rec.py
--rw-r--r--   0        0        0     3536 2021-12-06 14:15:54.630163 replay-rec-0.8.0/replay/models/cluster.py
--rw-r--r--   0        0        0     2783 2021-12-06 14:15:54.630304 replay-rec-0.8.0/replay/models/implicit_wrap.py
--rw-r--r--   0        0        0     4386 2021-12-06 14:15:54.630476 replay-rec-0.8.0/replay/models/knn.py
--rw-r--r--   0        0        0    11488 2021-12-06 14:15:54.630706 replay-rec-0.8.0/replay/models/lightfm_wrap.py
--rw-r--r--   0        0        0    12395 2021-12-06 14:15:54.630891 replay-rec-0.8.0/replay/models/mult_vae.py
--rw-r--r--   0        0        0    14998 2021-12-06 14:15:54.631118 replay-rec-0.8.0/replay/models/neuromf.py
--rw-r--r--   0        0        0     5105 2021-12-06 14:15:54.631242 replay-rec-0.8.0/replay/models/pop_rec.py
--rw-r--r--   0        0        0     8984 2021-12-06 14:15:54.631411 replay-rec-0.8.0/replay/models/random_rec.py
--rw-r--r--   0        0        0     3299 2021-12-06 14:15:54.631577 replay-rec-0.8.0/replay/models/slim.py
--rw-r--r--   0        0        0     4122 2021-12-06 14:15:54.631725 replay-rec-0.8.0/replay/models/user_pop_rec.py
--rw-r--r--   0        0        0     2294 2021-12-06 14:15:54.631857 replay-rec-0.8.0/replay/models/wilson.py
--rw-r--r--   0        0        0     6604 2021-12-06 14:15:54.631997 replay-rec-0.8.0/replay/models/word2vec.py
--rw-r--r--   0        0        0     4303 2021-12-06 14:15:54.632237 replay-rec-0.8.0/replay/optuna_objective.py
--rw-r--r--   0        0        0      338 2021-12-06 14:15:54.632467 replay-rec-0.8.0/replay/scenarios/__init__.py
--rw-r--r--   0        0        0     8739 2021-12-06 14:15:54.632634 replay-rec-0.8.0/replay/scenarios/basescenario.py
--rw-r--r--   0        0        0     5278 2021-12-06 14:15:54.632808 replay-rec-0.8.0/replay/scenarios/fallback.py
--rw-r--r--   0        0        0    17362 2021-12-06 14:15:54.633139 replay-rec-0.8.0/replay/scenarios/two_stages/feature_processor.py
--rw-r--r--   0        0        0    34781 2021-12-06 14:15:54.633565 replay-rec-0.8.0/replay/scenarios/two_stages/two_stages_scenario.py
--rw-r--r--   0        0        0     3590 2021-12-06 14:15:54.633770 replay-rec-0.8.0/replay/session_handler.py
--rw-r--r--   0        0        0      329 2021-12-06 14:15:54.633954 replay-rec-0.8.0/replay/splitters/__init__.py
--rw-r--r--   0        0        0     2914 2021-12-06 14:15:54.634109 replay-rec-0.8.0/replay/splitters/base_splitter.py
--rw-r--r--   0        0        0     7475 2021-12-06 14:15:54.634268 replay-rec-0.8.0/replay/splitters/log_splitter.py
--rw-r--r--   0        0        0    10377 2021-12-06 14:15:54.634469 replay-rec-0.8.0/replay/splitters/user_log_splitter.py
--rw-r--r--   0        0        0     8752 2021-12-06 14:15:54.634626 replay-rec-0.8.0/replay/time.py
--rw-r--r--   0        0        0    20832 2021-12-06 14:15:54.634863 replay-rec-0.8.0/replay/utils.py
--rw-r--r--   0        0        0     1606 2021-12-06 14:18:54.158533 replay-rec-0.8.0/setup.py
--rw-r--r--   0        0        0     1864 2021-12-06 14:18:54.158852 replay-rec-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11344 2022-04-13 12:55:01.843959 replay-rec-0.9.0/LICENSE
+-rw-r--r--   0        0        0      813 2022-04-13 12:55:01.844101 replay-rec-0.9.0/README.md
+-rw-r--r--   0        0        0     1776 2022-04-13 12:58:45.561827 replay-rec-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      112 2022-04-13 12:55:02.055666 replay-rec-0.9.0/replay/__init__.py
+-rw-r--r--   0        0        0      912 2022-04-13 12:55:02.055825 replay-rec-0.9.0/replay/constants.py
+-rw-r--r--   0        0        0    14705 2022-04-13 12:55:02.056085 replay-rec-0.9.0/replay/data_preparator.py
+-rw-r--r--   0        0        0     2676 2022-04-13 12:55:02.056273 replay-rec-0.9.0/replay/distributions.py
+-rw-r--r--   0        0        0     7049 2022-04-13 12:55:02.056467 replay-rec-0.9.0/replay/experiment.py
+-rw-r--r--   0        0        0    14232 2022-04-13 12:55:02.056739 replay-rec-0.9.0/replay/filters.py
+-rw-r--r--   0        0        0    19532 2022-04-13 12:55:02.056975 replay-rec-0.9.0/replay/history_based_fp.py
+-rw-r--r--   0        0        0     1574 2022-04-13 12:55:02.057206 replay-rec-0.9.0/replay/metrics/__init__.py
+-rwxr-xr-x   0        0        0     8567 2022-04-13 12:55:02.057447 replay-rec-0.9.0/replay/metrics/base_metric.py
+-rw-r--r--   0        0        0     3198 2022-04-13 12:55:02.057639 replay-rec-0.9.0/replay/metrics/coverage.py
+-rw-r--r--   0        0        0      679 2022-04-13 12:55:02.057772 replay-rec-0.9.0/replay/metrics/hitrate.py
+-rw-r--r--   0        0        0      984 2022-04-13 12:55:02.057994 replay-rec-0.9.0/replay/metrics/map.py
+-rw-r--r--   0        0        0      882 2022-04-13 12:55:02.058195 replay-rec-0.9.0/replay/metrics/mrr.py
+-rw-r--r--   0        0        0     1929 2022-04-13 12:55:02.058356 replay-rec-0.9.0/replay/metrics/ndcg.py
+-rw-r--r--   0        0        0      679 2022-04-13 12:55:02.058521 replay-rec-0.9.0/replay/metrics/precision.py
+-rw-r--r--   0        0        0      722 2022-04-13 12:55:02.058670 replay-rec-0.9.0/replay/metrics/recall.py
+-rw-r--r--   0        0        0     2089 2022-04-13 12:55:02.058808 replay-rec-0.9.0/replay/metrics/rocauc.py
+-rw-r--r--   0        0        0     2630 2022-04-13 12:55:02.058952 replay-rec-0.9.0/replay/metrics/surprisal.py
+-rw-r--r--   0        0        0     2692 2022-04-13 12:55:02.059087 replay-rec-0.9.0/replay/metrics/unexpectedness.py
+-rw-r--r--   0        0        0     3757 2022-04-13 12:55:02.059233 replay-rec-0.9.0/replay/model_handler.py
+-rw-r--r--   0        0        0     1110 2022-04-13 12:55:02.059477 replay-rec-0.9.0/replay/models/__init__.py
+-rw-r--r--   0        0        0     6098 2022-04-13 12:55:02.059678 replay-rec-0.9.0/replay/models/admm_slim.py
+-rw-r--r--   0        0        0     3916 2022-04-13 12:55:02.059840 replay-rec-0.9.0/replay/models/als.py
+-rw-r--r--   0        0        0    10811 2022-04-13 12:55:02.059992 replay-rec-0.9.0/replay/models/association_rules.py
+-rw-r--r--   0        0        0    50794 2022-04-13 12:55:02.060656 replay-rec-0.9.0/replay/models/base_rec.py
+-rw-r--r--   0        0        0     7697 2022-04-13 12:55:02.061020 replay-rec-0.9.0/replay/models/base_torch_rec.py
+-rw-r--r--   0        0        0     3585 2022-04-13 12:55:02.061249 replay-rec-0.9.0/replay/models/cluster.py
+-rw-r--r--   0        0        0     2861 2022-04-13 12:55:02.061471 replay-rec-0.9.0/replay/models/implicit_wrap.py
+-rw-r--r--   0        0        0     4986 2022-04-13 12:55:02.061778 replay-rec-0.9.0/replay/models/knn.py
+-rw-r--r--   0        0        0    11032 2022-04-13 12:55:02.062139 replay-rec-0.9.0/replay/models/lightfm_wrap.py
+-rw-r--r--   0        0        0    12364 2022-04-13 12:55:02.062443 replay-rec-0.9.0/replay/models/mult_vae.py
+-rw-r--r--   0        0        0    15300 2022-04-13 12:55:02.062833 replay-rec-0.9.0/replay/models/neuromf.py
+-rw-r--r--   0        0        0     4992 2022-04-13 12:55:02.063101 replay-rec-0.9.0/replay/models/pop_rec.py
+-rw-r--r--   0        0        0     9006 2022-04-13 12:55:02.063419 replay-rec-0.9.0/replay/models/random_rec.py
+-rw-r--r--   0        0        0     3315 2022-04-13 12:55:02.063700 replay-rec-0.9.0/replay/models/slim.py
+-rw-r--r--   0        0        0     4159 2022-04-13 12:55:02.063956 replay-rec-0.9.0/replay/models/user_pop_rec.py
+-rw-r--r--   0        0        0     2402 2022-04-13 12:55:02.064145 replay-rec-0.9.0/replay/models/wilson.py
+-rw-r--r--   0        0        0     6644 2022-04-13 12:55:02.064350 replay-rec-0.9.0/replay/models/word2vec.py
+-rw-r--r--   0        0        0     7224 2022-04-13 12:55:02.064560 replay-rec-0.9.0/replay/optuna_objective.py
+-rw-r--r--   0        0        0      242 2022-04-13 12:55:02.064880 replay-rec-0.9.0/replay/scenarios/__init__.py
+-rw-r--r--   0        0        0     8531 2022-04-13 12:55:02.065132 replay-rec-0.9.0/replay/scenarios/basescenario.py
+-rw-r--r--   0        0        0     7648 2022-04-13 12:55:02.065413 replay-rec-0.9.0/replay/scenarios/fallback.py
+-rw-r--r--   0        0        0     4247 2022-04-13 12:55:02.065734 replay-rec-0.9.0/replay/scenarios/two_stages/reranker.py
+-rw-r--r--   0        0        0    30830 2022-04-13 12:55:02.066270 replay-rec-0.9.0/replay/scenarios/two_stages/two_stages_scenario.py
+-rw-r--r--   0        0        0     3590 2022-04-13 12:55:02.066594 replay-rec-0.9.0/replay/session_handler.py
+-rw-r--r--   0        0        0      329 2022-04-13 12:55:02.066901 replay-rec-0.9.0/replay/splitters/__init__.py
+-rw-r--r--   0        0        0     2902 2022-04-13 12:55:02.067152 replay-rec-0.9.0/replay/splitters/base_splitter.py
+-rw-r--r--   0        0        0     7533 2022-04-13 12:55:02.067417 replay-rec-0.9.0/replay/splitters/log_splitter.py
+-rw-r--r--   0        0        0    10566 2022-04-13 12:55:02.067741 replay-rec-0.9.0/replay/splitters/user_log_splitter.py
+-rw-r--r--   0        0        0     8831 2022-04-13 12:55:02.067992 replay-rec-0.9.0/replay/time.py
+-rw-r--r--   0        0        0    20908 2022-04-13 12:55:02.068284 replay-rec-0.9.0/replay/utils.py
+-rw-r--r--   0        0        0     1792 2022-04-13 12:58:50.424157 replay-rec-0.9.0/setup.py
+-rw-r--r--   0        0        0     2052 2022-04-13 12:58:50.424546 replay-rec-0.9.0/PKG-INFO
```

### Comparing `replay-rec-0.8.0/LICENSE` & `replay-rec-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `replay-rec-0.8.0/README.md` & `replay-rec-0.9.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 ## Docs
 
 [Documentation](https://sberbank-ai-lab.github.io/RePlay/)
 
 
 ### Installation
 
-Use Linux machine with Python 3.7+ and Java 8+. 
+Use Linux machine with Python 3.7+, Java 8+ and C++ compiler. 
 
 ```bash
 pip install replay-rec
 ```
 
 It is preferable to use a virtual environment for your installation.
+
+If you encounter an error during RePlay installation, check the [troubleshooting](https://sberbank-ai-lab.github.io/RePlay/pages/installation.html#troubleshooting) guide.
```

### Comparing `replay-rec-0.8.0/pyproject.toml` & `replay-rec-0.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "replay-rec"
-version = "0.8.0"
+version = "0.9.0"
 description = "RecSys Library"
 authors = ["AI Lab, Sber",
            "Alexey Vasilev <AVaVasilyev@sberbank.ru>",
            "Yan-Martin Tamm <YYTamm@sberbank.ru>",
            "Anna Volodkevich <AAVolodkevich@sberbank.ru>",
            "Boris Shminke",
            "Alexander Sidorenko",
@@ -31,23 +31,23 @@
 pytorch-ignite = "*"
 lightfm = "*"
 lightautoml = ">=0.3.1"
 numpy = ">=1.20.0"
 optuna = "*"
 pandas = "*"
 psutil = "*"
-pyspark = "^3.0.0"
+pyspark = ">=3.0, < 3.2"
 scipy = "*"
 scikit-learn = "*"
 torch = "*"
 numba = ">=0.50"
 llvmlite = ">=0.32.1"
 seaborn = "*"
 pyarrow = "*"
-implicit = "*"
+implicit = "<0.5"
 
 [tool.poetry.dev-dependencies]
 # dev only
 # visualization
 jupyter = "*"
 jupyterlab = "*"
 matplotlib = "*"
```

### Comparing `replay-rec-0.8.0/replay/constants.py` & `replay-rec-0.9.0/replay/constants.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,55 +4,39 @@
 from typing import Iterable, Union
 
 import pandas as pd
 from pyspark.sql import DataFrame
 from pyspark.sql.types import (
     DoubleType,
     IntegerType,
-    StringType,
     StructField,
     StructType,
     TimestampType,
 )
 
 LOG_SCHEMA = StructType(
     [
-        StructField("user_id", StringType()),
-        StructField("item_id", StringType()),
+        StructField("user_idx", IntegerType()),
+        StructField("item_idx", IntegerType()),
         StructField("timestamp", TimestampType()),
         StructField("relevance", DoubleType()),
     ]
 )
 
 REC_SCHEMA = StructType(
     [
-        StructField("user_id", StringType()),
-        StructField("item_id", StringType()),
-        StructField("relevance", DoubleType()),
-    ]
-)
-
-BASE_SCHEMA = StructType(
-    [
-        StructField("user_id", StringType()),
-        StructField("item_id", StringType()),
-    ]
-)
-
-IDX_SCHEMA = StructType(
-    [
         StructField("user_idx", IntegerType()),
         StructField("item_idx", IntegerType()),
+        StructField("relevance", DoubleType()),
     ]
 )
 
-IDX_REC_SCHEMA = StructType(
+BASE_SCHEMA = StructType(
     [
         StructField("user_idx", IntegerType()),
         StructField("item_idx", IntegerType()),
-        StructField("relevance", DoubleType()),
     ]
 )
 
 IntOrList = Union[Iterable[int], int]
 NumType = Union[int, float]
 AnyDataFrame = Union[DataFrame, pd.DataFrame]
```

### Comparing `replay-rec-0.8.0/replay/experiment.py` & `replay-rec-0.9.0/replay/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 
     Results are available with ``pandas_df`` attribute.
 
     Example:
 
     >>> import pandas as pd
     >>> from replay.metrics import Coverage, NDCG, Precision, Surprisal
-    >>> log = pd.DataFrame({"user_id": [2, 2, 2, 1], "item_id": [1, 2, 3, 3], "relevance": [5, 5, 5, 5]})
-    >>> test = pd.DataFrame({"user_id": [1, 1, 1], "item_id": [1, 2, 3], "relevance": [5, 3, 4]})
-    >>> pred = pd.DataFrame({"user_id": [1, 1, 1], "item_id": [4, 1, 3], "relevance": [5, 4, 5]})
-    >>> recs = pd.DataFrame({"user_id": [1, 1, 1], "item_id": [1, 4, 5], "relevance": [5, 4, 5]})
+    >>> log = pd.DataFrame({"user_idx": [2, 2, 2, 1], "item_idx": [1, 2, 3, 3], "relevance": [5, 5, 5, 5]})
+    >>> test = pd.DataFrame({"user_idx": [1, 1, 1], "item_idx": [1, 2, 3], "relevance": [5, 3, 4]})
+    >>> pred = pd.DataFrame({"user_idx": [1, 1, 1], "item_idx": [4, 1, 3], "relevance": [5, 4, 5]})
+    >>> recs = pd.DataFrame({"user_idx": [1, 1, 1], "item_idx": [1, 4, 5], "relevance": [5, 4, 5]})
     >>> ex = Experiment(test, {NDCG(): [2, 3], Surprisal(log): 3})
     >>> ex.add_result("baseline", recs)
     >>> ex.add_result("model", pred)
     >>> ex.results
                 NDCG@2    NDCG@3  Surprisal@3
     baseline  0.613147  0.469279     1.000000
     model     0.386853  0.530721     0.666667
@@ -83,25 +83,23 @@
         :param name: name of the run to store in the resulting DataFrame
         :param pred: model recommendations
         """
         recs = get_enriched_recommendations(pred, self.test).cache()
         for metric, k_list in sorted(
             self.metrics.items(), key=lambda x: str(x[0])
         ):
+            enriched = None
             if isinstance(metric, RecOnlyMetric):
                 enriched = metric._get_enriched_recommendations(
                     pred, self.test
                 )
-                values, median, conf_interval = self._calculate(
-                    metric, enriched, k_list
-                )
-            else:
-                values, median, conf_interval = self._calculate(
-                    metric, recs, k_list
-                )
+
+            values, median, conf_interval = self._calculate(
+                metric, enriched or recs, k_list
+            )
 
             if isinstance(k_list, int):
                 self._add_metric(  # type: ignore
                     name,
                     metric,
                     k_list,
                     values,  # type: ignore
```

### Comparing `replay-rec-0.8.0/replay/filters.py` & `replay-rec-0.9.0/replay/filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,38 +13,37 @@
 
 
 def min_entries(data_frame: AnyDataFrame, num_entries: int) -> DataFrame:
     """
     Remove users with less than ``num_entries`` ratings.
 
     >>> import pandas as pd
-    >>> data_frame = pd.DataFrame({"user_id": [1, 1, 2]})
+    >>> data_frame = pd.DataFrame({"user_idx": [1, 1, 2]})
     >>> min_entries(data_frame, 2).toPandas()
-       user_id
-    0        1
-    1        1
+       user_idx
+    0         1
+    1         1
     """
     data_frame = convert2spark(data_frame)
     input_count = data_frame.count()
-    entries_by_user = data_frame.groupBy("user_id").count()  # type: ignore
+    entries_by_user = data_frame.groupBy("user_idx").count()  # type: ignore
     remaining_users = entries_by_user.filter(
         entries_by_user["count"] >= num_entries
-    )[["user_id"]]
+    )[["user_idx"]]
     data_frame = data_frame.join(
-        remaining_users, on="user_id", how="inner"
+        remaining_users, on="user_idx", how="inner"
     )  # type: ignore
     output_count = data_frame.count()
     diff = (input_count - output_count) / input_count
     if diff > 0.5:
         logger_level = State().logger.warning
     else:
         logger_level = State().logger.info
     logger_level(
-        "current threshold removes %s%% of data",
-        diff,
+        "current threshold removes %s%% of data", diff,
     )
     return data_frame
 
 
 def min_rating(
     data_frame: AnyDataFrame, value: float, column="relevance"
 ) -> DataFrame:
@@ -65,76 +64,76 @@
 
 # pylint: disable=too-many-arguments,
 def filter_user_interactions(
     log: DataFrame,
     num_interactions: int = 10,
     first: bool = True,
     date_col: str = "timestamp",
-    user_col: str = "user_id",
-    item_col: Optional[str] = "item_id",
+    user_col: str = "user_idx",
+    item_col: Optional[str] = "item_idx",
 ) -> DataFrame:
     """
      Get first/last ``num_interactions`` interactions for each user.
 
     >>> import pandas as pd
     >>> from replay.utils import convert2spark
-    >>> log_pd = pd.DataFrame({"user_id": ["u1", "u2", "u2", "u3", "u3", "u3"],
-    ...                     "item_id": ["i1", "i2","i3", "i1", "i2","i3"],
+    >>> log_pd = pd.DataFrame({"user_idx": ["u1", "u2", "u2", "u3", "u3", "u3"],
+    ...                     "item_idx": ["i1", "i2","i3", "i1", "i2","i3"],
     ...                     "rel": [1., 0.5, 3, 1, 0, 1],
     ...                     "timestamp": ["2020-01-01 23:59:59", "2020-02-01",
     ...                                   "2020-02-01", "2020-01-01 00:04:15",
     ...                                   "2020-01-02 00:04:14", "2020-01-05 23:59:59"]},
     ...             )
     >>> log_pd["timestamp"] = pd.to_datetime(log_pd["timestamp"])
     >>> log_sp = convert2spark(log_pd)
     >>> log_sp.show()
-    +-------+-------+---+-------------------+
-    |user_id|item_id|rel|          timestamp|
-    +-------+-------+---+-------------------+
-    |     u1|     i1|1.0|2020-01-01 23:59:59|
-    |     u2|     i2|0.5|2020-02-01 00:00:00|
-    |     u2|     i3|3.0|2020-02-01 00:00:00|
-    |     u3|     i1|1.0|2020-01-01 00:04:15|
-    |     u3|     i2|0.0|2020-01-02 00:04:14|
-    |     u3|     i3|1.0|2020-01-05 23:59:59|
-    +-------+-------+---+-------------------+
+    +--------+--------+---+-------------------+
+    |user_idx|item_idx|rel|          timestamp|
+    +--------+--------+---+-------------------+
+    |      u1|      i1|1.0|2020-01-01 23:59:59|
+    |      u2|      i2|0.5|2020-02-01 00:00:00|
+    |      u2|      i3|3.0|2020-02-01 00:00:00|
+    |      u3|      i1|1.0|2020-01-01 00:04:15|
+    |      u3|      i2|0.0|2020-01-02 00:04:14|
+    |      u3|      i3|1.0|2020-01-05 23:59:59|
+    +--------+--------+---+-------------------+
     <BLANKLINE>
 
     Only first interaction:
 
-    >>> filter_user_interactions(log_sp, 1, True).orderBy('user_id').show()
-    +-------+-------+---+-------------------+
-    |user_id|item_id|rel|          timestamp|
-    +-------+-------+---+-------------------+
-    |     u1|     i1|1.0|2020-01-01 23:59:59|
-    |     u2|     i2|0.5|2020-02-01 00:00:00|
-    |     u3|     i1|1.0|2020-01-01 00:04:15|
-    +-------+-------+---+-------------------+
+    >>> filter_user_interactions(log_sp, 1, True).orderBy('user_idx').show()
+    +--------+--------+---+-------------------+
+    |user_idx|item_idx|rel|          timestamp|
+    +--------+--------+---+-------------------+
+    |      u1|      i1|1.0|2020-01-01 23:59:59|
+    |      u2|      i2|0.5|2020-02-01 00:00:00|
+    |      u3|      i1|1.0|2020-01-01 00:04:15|
+    +--------+--------+---+-------------------+
     <BLANKLINE>
 
     Only last interaction:
 
-    >>> filter_user_interactions(log_sp, 1, False, item_col=None).orderBy('user_id').show()
-    +-------+-------+---+-------------------+
-    |user_id|item_id|rel|          timestamp|
-    +-------+-------+---+-------------------+
-    |     u1|     i1|1.0|2020-01-01 23:59:59|
-    |     u2|     i2|0.5|2020-02-01 00:00:00|
-    |     u3|     i3|1.0|2020-01-05 23:59:59|
-    +-------+-------+---+-------------------+
-    <BLANKLINE>
-
-    >>> filter_user_interactions(log_sp, 1, False).orderBy('user_id').show()
-    +-------+-------+---+-------------------+
-    |user_id|item_id|rel|          timestamp|
-    +-------+-------+---+-------------------+
-    |     u1|     i1|1.0|2020-01-01 23:59:59|
-    |     u2|     i3|3.0|2020-02-01 00:00:00|
-    |     u3|     i3|1.0|2020-01-05 23:59:59|
-    +-------+-------+---+-------------------+
+    >>> filter_user_interactions(log_sp, 1, False, item_col=None).orderBy('user_idx').show()
+    +--------+--------+---+-------------------+
+    |user_idx|item_idx|rel|          timestamp|
+    +--------+--------+---+-------------------+
+    |      u1|      i1|1.0|2020-01-01 23:59:59|
+    |      u2|      i2|0.5|2020-02-01 00:00:00|
+    |      u3|      i3|1.0|2020-01-05 23:59:59|
+    +--------+--------+---+-------------------+
+    <BLANKLINE>
+
+    >>> filter_user_interactions(log_sp, 1, False).orderBy('user_idx').show()
+    +--------+--------+---+-------------------+
+    |user_idx|item_idx|rel|          timestamp|
+    +--------+--------+---+-------------------+
+    |      u1|      i1|1.0|2020-01-01 23:59:59|
+    |      u2|      i3|3.0|2020-02-01 00:00:00|
+    |      u3|      i3|1.0|2020-01-05 23:59:59|
+    +--------+--------+---+-------------------+
     <BLANKLINE>
 
     :param log: historical interactions DataFrame
     :param num_interactions: number of interactions to leave per user
     :param first: take either first ``num_interactions`` or last.
     :param date_col: date column
     :param user_col: user column
@@ -159,68 +158,68 @@
 
 
 def filter_by_user_duration(
     log: DataFrame,
     days: int = 10,
     first: bool = True,
     date_col: str = "timestamp",
-    user_col: str = "user_id",
+    user_col: str = "user_idx",
 ) -> DataFrame:
     """
     Get first/last ``days`` of user interactions.
 
     >>> import pandas as pd
     >>> from replay.utils import convert2spark
-    >>> log_pd = pd.DataFrame({"user_id": ["u1", "u2", "u2", "u3", "u3", "u3"],
-    ...                     "item_id": ["i1", "i2","i3", "i1", "i2","i3"],
+    >>> log_pd = pd.DataFrame({"user_idx": ["u1", "u2", "u2", "u3", "u3", "u3"],
+    ...                     "item_idx": ["i1", "i2","i3", "i1", "i2","i3"],
     ...                     "rel": [1., 0.5, 3, 1, 0, 1],
     ...                     "timestamp": ["2020-01-01 23:59:59", "2020-02-01",
     ...                                   "2020-02-01", "2020-01-01 00:04:15",
     ...                                   "2020-01-02 00:04:14", "2020-01-05 23:59:59"]},
     ...             )
     >>> log_pd["timestamp"] = pd.to_datetime(log_pd["timestamp"])
     >>> log_sp = convert2spark(log_pd)
-    >>> log_sp.orderBy('user_id', 'item_id').show()
-    +-------+-------+---+-------------------+
-    |user_id|item_id|rel|          timestamp|
-    +-------+-------+---+-------------------+
-    |     u1|     i1|1.0|2020-01-01 23:59:59|
-    |     u2|     i2|0.5|2020-02-01 00:00:00|
-    |     u2|     i3|3.0|2020-02-01 00:00:00|
-    |     u3|     i1|1.0|2020-01-01 00:04:15|
-    |     u3|     i2|0.0|2020-01-02 00:04:14|
-    |     u3|     i3|1.0|2020-01-05 23:59:59|
-    +-------+-------+---+-------------------+
+    >>> log_sp.orderBy('user_idx', 'item_idx').show()
+    +--------+--------+---+-------------------+
+    |user_idx|item_idx|rel|          timestamp|
+    +--------+--------+---+-------------------+
+    |      u1|      i1|1.0|2020-01-01 23:59:59|
+    |      u2|      i2|0.5|2020-02-01 00:00:00|
+    |      u2|      i3|3.0|2020-02-01 00:00:00|
+    |      u3|      i1|1.0|2020-01-01 00:04:15|
+    |      u3|      i2|0.0|2020-01-02 00:04:14|
+    |      u3|      i3|1.0|2020-01-05 23:59:59|
+    +--------+--------+---+-------------------+
     <BLANKLINE>
 
     Get first day:
 
-    >>> filter_by_user_duration(log_sp, 1, True).orderBy('user_id', 'item_id').show()
-    +-------+-------+---+-------------------+
-    |user_id|item_id|rel|          timestamp|
-    +-------+-------+---+-------------------+
-    |     u1|     i1|1.0|2020-01-01 23:59:59|
-    |     u2|     i2|0.5|2020-02-01 00:00:00|
-    |     u2|     i3|3.0|2020-02-01 00:00:00|
-    |     u3|     i1|1.0|2020-01-01 00:04:15|
-    |     u3|     i2|0.0|2020-01-02 00:04:14|
-    +-------+-------+---+-------------------+
+    >>> filter_by_user_duration(log_sp, 1, True).orderBy('user_idx', 'item_idx').show()
+    +--------+--------+---+-------------------+
+    |user_idx|item_idx|rel|          timestamp|
+    +--------+--------+---+-------------------+
+    |      u1|      i1|1.0|2020-01-01 23:59:59|
+    |      u2|      i2|0.5|2020-02-01 00:00:00|
+    |      u2|      i3|3.0|2020-02-01 00:00:00|
+    |      u3|      i1|1.0|2020-01-01 00:04:15|
+    |      u3|      i2|0.0|2020-01-02 00:04:14|
+    +--------+--------+---+-------------------+
     <BLANKLINE>
 
     Get last day:
 
-    >>> filter_by_user_duration(log_sp, 1, False).orderBy('user_id', 'item_id').show()
-    +-------+-------+---+-------------------+
-    |user_id|item_id|rel|          timestamp|
-    +-------+-------+---+-------------------+
-    |     u1|     i1|1.0|2020-01-01 23:59:59|
-    |     u2|     i2|0.5|2020-02-01 00:00:00|
-    |     u2|     i3|3.0|2020-02-01 00:00:00|
-    |     u3|     i3|1.0|2020-01-05 23:59:59|
-    +-------+-------+---+-------------------+
+    >>> filter_by_user_duration(log_sp, 1, False).orderBy('user_idx', 'item_idx').show()
+    +--------+--------+---+-------------------+
+    |user_idx|item_idx|rel|          timestamp|
+    +--------+--------+---+-------------------+
+    |      u1|      i1|1.0|2020-01-01 23:59:59|
+    |      u2|      i2|0.5|2020-02-01 00:00:00|
+    |      u2|      i3|3.0|2020-02-01 00:00:00|
+    |      u3|      i3|1.0|2020-01-05 23:59:59|
+    +--------+--------+---+-------------------+
     <BLANKLINE>
 
     :param log: historical DataFrame
     :param days: how many days to return per user
     :param first: take either first ``days`` or last
     :param date_col: date column
     :param user_col: user column
@@ -236,16 +235,15 @@
             )
             .drop("min_date")
         )
 
     return (
         log.withColumn("max_date", sf.max(col(date_col)).over(window))
         .filter(
-            col(date_col)
-            > col("max_date") - sf.expr(f"INTERVAL {days} days")
+            col(date_col) > col("max_date") - sf.expr(f"INTERVAL {days} days")
         )
         .drop("max_date")
     )
 
 
 def filter_between_dates(
     log: DataFrame,
@@ -254,43 +252,43 @@
     date_column: str = "timestamp",
 ) -> DataFrame:
     """
     Select a part of data between ``[start_date, end_date)``.
 
     >>> import pandas as pd
     >>> from replay.utils import convert2spark
-    >>> log_pd = pd.DataFrame({"user_id": ["u1", "u2", "u2", "u3", "u3", "u3"],
-    ...                     "item_id": ["i1", "i2","i3", "i1", "i2","i3"],
+    >>> log_pd = pd.DataFrame({"user_idx": ["u1", "u2", "u2", "u3", "u3", "u3"],
+    ...                     "item_idx": ["i1", "i2","i3", "i1", "i2","i3"],
     ...                     "rel": [1., 0.5, 3, 1, 0, 1],
     ...                     "timestamp": ["2020-01-01 23:59:59", "2020-02-01",
     ...                                   "2020-02-01", "2020-01-01 00:04:15",
     ...                                   "2020-01-02 00:04:14", "2020-01-05 23:59:59"]},
     ...             )
     >>> log_pd["timestamp"] = pd.to_datetime(log_pd["timestamp"])
     >>> log_sp = convert2spark(log_pd)
     >>> log_sp.show()
-    +-------+-------+---+-------------------+
-    |user_id|item_id|rel|          timestamp|
-    +-------+-------+---+-------------------+
-    |     u1|     i1|1.0|2020-01-01 23:59:59|
-    |     u2|     i2|0.5|2020-02-01 00:00:00|
-    |     u2|     i3|3.0|2020-02-01 00:00:00|
-    |     u3|     i1|1.0|2020-01-01 00:04:15|
-    |     u3|     i2|0.0|2020-01-02 00:04:14|
-    |     u3|     i3|1.0|2020-01-05 23:59:59|
-    +-------+-------+---+-------------------+
+    +--------+--------+---+-------------------+
+    |user_idx|item_idx|rel|          timestamp|
+    +--------+--------+---+-------------------+
+    |      u1|      i1|1.0|2020-01-01 23:59:59|
+    |      u2|      i2|0.5|2020-02-01 00:00:00|
+    |      u2|      i3|3.0|2020-02-01 00:00:00|
+    |      u3|      i1|1.0|2020-01-01 00:04:15|
+    |      u3|      i2|0.0|2020-01-02 00:04:14|
+    |      u3|      i3|1.0|2020-01-05 23:59:59|
+    +--------+--------+---+-------------------+
     <BLANKLINE>
 
     >>> filter_between_dates(log_sp, start_date="2020-01-01 14:00:00", end_date=datetime(2020, 1, 3, 0, 0, 0)).show()
-    +-------+-------+---+-------------------+
-    |user_id|item_id|rel|          timestamp|
-    +-------+-------+---+-------------------+
-    |     u1|     i1|1.0|2020-01-01 23:59:59|
-    |     u3|     i2|0.0|2020-01-02 00:04:14|
-    +-------+-------+---+-------------------+
+    +--------+--------+---+-------------------+
+    |user_idx|item_idx|rel|          timestamp|
+    +--------+--------+---+-------------------+
+    |      u1|      i1|1.0|2020-01-01 23:59:59|
+    |      u3|      i2|0.0|2020-01-02 00:04:14|
+    +--------+--------+---+-------------------+
     <BLANKLINE>
 
     :param log: historical DataFrame
     :param start_date: datetime or str with format "yyyy-MM-dd HH:mm:ss".
     :param end_date: datetime or str with format "yyyy-MM-dd HH:mm:ss".
     :param date_column: date column
     """
@@ -314,53 +312,53 @@
     date_column: str = "timestamp",
 ) -> DataFrame:
     """
     Select first/last days from ``log``.
 
     >>> import pandas as pd
     >>> from replay.utils import convert2spark
-    >>> log_pd = pd.DataFrame({"user_id": ["u1", "u2", "u2", "u3", "u3", "u3"],
-    ...                     "item_id": ["i1", "i2","i3", "i1", "i2","i3"],
+    >>> log_pd = pd.DataFrame({"user_idx": ["u1", "u2", "u2", "u3", "u3", "u3"],
+    ...                     "item_idx": ["i1", "i2","i3", "i1", "i2","i3"],
     ...                     "rel": [1., 0.5, 3, 1, 0, 1],
     ...                     "timestamp": ["2020-01-01 23:59:59", "2020-02-01",
     ...                                   "2020-02-01", "2020-01-01 00:04:15",
     ...                                   "2020-01-02 00:04:14", "2020-01-05 23:59:59"]},
     ...             )
     >>> log_pd["timestamp"] = pd.to_datetime(log_pd["timestamp"])
     >>> log_sp = convert2spark(log_pd)
     >>> log_sp.show()
-    +-------+-------+---+-------------------+
-    |user_id|item_id|rel|          timestamp|
-    +-------+-------+---+-------------------+
-    |     u1|     i1|1.0|2020-01-01 23:59:59|
-    |     u2|     i2|0.5|2020-02-01 00:00:00|
-    |     u2|     i3|3.0|2020-02-01 00:00:00|
-    |     u3|     i1|1.0|2020-01-01 00:04:15|
-    |     u3|     i2|0.0|2020-01-02 00:04:14|
-    |     u3|     i3|1.0|2020-01-05 23:59:59|
-    +-------+-------+---+-------------------+
+    +--------+--------+---+-------------------+
+    |user_idx|item_idx|rel|          timestamp|
+    +--------+--------+---+-------------------+
+    |      u1|      i1|1.0|2020-01-01 23:59:59|
+    |      u2|      i2|0.5|2020-02-01 00:00:00|
+    |      u2|      i3|3.0|2020-02-01 00:00:00|
+    |      u3|      i1|1.0|2020-01-01 00:04:15|
+    |      u3|      i2|0.0|2020-01-02 00:04:14|
+    |      u3|      i3|1.0|2020-01-05 23:59:59|
+    +--------+--------+---+-------------------+
     <BLANKLINE>
 
     >>> filter_by_duration(log_sp, 1).show()
-    +-------+-------+---+-------------------+
-    |user_id|item_id|rel|          timestamp|
-    +-------+-------+---+-------------------+
-    |     u1|     i1|1.0|2020-01-01 23:59:59|
-    |     u3|     i1|1.0|2020-01-01 00:04:15|
-    |     u3|     i2|0.0|2020-01-02 00:04:14|
-    +-------+-------+---+-------------------+
+    +--------+--------+---+-------------------+
+    |user_idx|item_idx|rel|          timestamp|
+    +--------+--------+---+-------------------+
+    |      u1|      i1|1.0|2020-01-01 23:59:59|
+    |      u3|      i1|1.0|2020-01-01 00:04:15|
+    |      u3|      i2|0.0|2020-01-02 00:04:14|
+    +--------+--------+---+-------------------+
     <BLANKLINE>
 
     >>> filter_by_duration(log_sp, 1, first=False).show()
-    +-------+-------+---+-------------------+
-    |user_id|item_id|rel|          timestamp|
-    +-------+-------+---+-------------------+
-    |     u2|     i2|0.5|2020-02-01 00:00:00|
-    |     u2|     i3|3.0|2020-02-01 00:00:00|
-    +-------+-------+---+-------------------+
+    +--------+--------+---+-------------------+
+    |user_idx|item_idx|rel|          timestamp|
+    +--------+--------+---+-------------------+
+    |      u2|      i2|0.5|2020-02-01 00:00:00|
+    |      u2|      i3|3.0|2020-02-01 00:00:00|
+    +--------+--------+---+-------------------+
     <BLANKLINE>
 
     :param log: historical DataFrame
     :param duration_days: length of selected data in days
     :param first: take either first ``duration_days`` or last
     :param date_column: date column
     """
```

### Comparing `replay-rec-0.8.0/replay/metrics/__init__.py` & `replay-rec-0.9.0/replay/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `replay-rec-0.8.0/replay/metrics/base_metric.py` & `replay-rec-0.9.0/replay/metrics/base_metric.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,49 +35,66 @@
     return list_res
 
 
 def get_enriched_recommendations(
     recommendations: AnyDataFrame, ground_truth: AnyDataFrame
 ) -> DataFrame:
     """
-    Adds additional info to recommendations.
-    By default adds column containing number of elements user interacted with.
+    Merge recommendations and ground truth into a single DataFrame
+    and aggregate items into lists so that each user has only one record.
 
     :param recommendations: recommendation list
     :param ground_truth: test data
-    :return: recommendations with additional columns,
-        spark DataFrame ``[user_id, item_id, relevance, *columns]``
+    :return:  ``[user_id, pred, ground_truth]``
     """
     recommendations = convert2spark(recommendations)
     ground_truth = convert2spark(ground_truth)
-    true_items_by_users = ground_truth.groupby("user_id").agg(
-        sf.collect_set("item_id").alias("ground_truth")
+    true_items_by_users = ground_truth.groupby("user_idx").agg(
+        sf.collect_set("item_idx").alias("ground_truth")
     )
     sort_udf = sf.udf(
         sorter,
-        returnType=st.ArrayType(ground_truth.schema["item_id"].dataType),
+        returnType=st.ArrayType(ground_truth.schema["item_idx"].dataType),
     )
     recommendations = (
-        recommendations.groupby("user_id")
-        .agg(sf.collect_list(sf.struct("relevance", "item_id")).alias("pred"))
-        .select("user_id", sort_udf(sf.col("pred")).alias("pred"))
-        .join(true_items_by_users, how="right", on=["user_id"])
+        recommendations.groupby("user_idx")
+        .agg(sf.collect_list(sf.struct("relevance", "item_idx")).alias("pred"))
+        .select("user_idx", sort_udf(sf.col("pred")).alias("pred"))
+        .join(true_items_by_users, how="right", on=["user_idx"])
     )
 
     return recommendations.withColumn(
         "pred",
         sf.coalesce(
             "pred",
             sf.array().cast(
-                st.ArrayType(ground_truth.schema["item_id"].dataType)
+                st.ArrayType(ground_truth.schema["item_idx"].dataType)
             ),
         ),
     )
 
 
+def process_k(func):
+    """Decorator that converts k to list and unpacks result"""
+
+    def wrap(self, recs: DataFrame, k: IntOrList, *args):
+        if isinstance(k, int):
+            k_list = [k]
+        else:
+            k_list = k
+
+        res = func(self, recs, k_list, *args)
+
+        if isinstance(k, int):
+            return res[k]
+        return res
+
+    return wrap
+
+
 class Metric(ABC):
     """Base metric class"""
 
     def __str__(self):
         return type(self).__name__
 
     def __call__(
@@ -93,121 +110,76 @@
             ``[user_id, item_id, timestamp, relevance]``
         :param k: depth cut-off. Truncates recommendation lists to top-k items.
         :return: metric value
         """
         recs = get_enriched_recommendations(recommendations, ground_truth)
         return self._mean(recs, k)
 
-    def _conf_interval(self, recs: DataFrame, k: IntOrList, alpha: float):
-        distribution = self._get_metric_distribution(recs, k)
-        total_metric = (
-            distribution.groupby("k")
-            .agg(
-                sf.stddev("cum_agg").alias("std"),
-                sf.count("cum_agg").alias("count"),
-            )
-            .select(
-                sf.when(sf.isnan(sf.col("std")), sf.lit(0.0))
-                .otherwise(sf.col("std"))
-                .cast("float")
-                .alias("std"),
-                "count",
-                "k",
-            )
-            .collect()
-        )
+    @process_k
+    def _conf_interval(self, recs: DataFrame, k_list: list, alpha: float):
+        res = {}
         quantile = norm.ppf((1 + alpha) / 2)
-        res = {
-            row["k"]: quantile * row["std"] / (row["count"] ** 0.5)
-            for row in total_metric
-        }
-
-        return self._unpack_if_int(res, k)
-
-    def _median(self, recs: DataFrame, k: IntOrList):
-        distribution = self._get_metric_distribution(recs, k)
-        total_metric = (
-            distribution.groupby("k")
-            .agg(
-                sf.expr("percentile_approx(cum_agg, 0.5)").alias(
-                    "total_metric"
+        for k in k_list:
+            distribution = self._get_metric_distribution(recs, k)
+            value = (
+                distribution.agg(
+                    sf.stddev("value").alias("std"),
+                    sf.count("value").alias("count"),
+                )
+                .select(
+                    sf.when(sf.isnan(sf.col("std")), sf.lit(0.0))
+                    .otherwise(sf.col("std"))
+                    .cast("float")
+                    .alias("std"),
+                    "count",
                 )
+                .first()
             )
-            .select("total_metric", "k")
-            .collect()
-        )
-        res = {row["k"]: row["total_metric"] for row in total_metric}
-        return self._unpack_if_int(res, k)
+            res[k] = quantile * value["std"] / (value["count"] ** 0.5)
+        return res
 
-    @staticmethod
-    def _unpack_if_int(res: Dict, k: IntOrList) -> Union[Dict, float]:
-        if isinstance(k, int):
-            return res[k]
+    @process_k
+    def _median(self, recs: DataFrame, k_list: list):
+        res = {}
+        for k in k_list:
+            distribution = self._get_metric_distribution(recs, k)
+            value = distribution.agg(
+                sf.expr("percentile_approx(value, 0.5)").alias("value")
+            ).first()["value"]
+            res[k] = value
         return res
 
-    def _mean(self, recs: DataFrame, k: IntOrList):
-        distribution = self._get_metric_distribution(recs, k)
-        total_metric = (
-            distribution.groupby("k")
-            .agg(sf.avg("cum_agg").alias("total_metric"))
-            .select("total_metric", "k")
-            .collect()
-        )
-        res = {row["k"]: row["total_metric"] for row in total_metric}
-        return self._unpack_if_int(res, k)
+    @process_k
+    def _mean(self, recs: DataFrame, k_list: list):
+        res = {}
+        for k in k_list:
+            distribution = self._get_metric_distribution(recs, k)
+            value = distribution.agg(sf.avg("value").alias("value")).first()[
+                "value"
+            ]
+            res[k] = value
+        return res
 
-    def _get_metric_distribution(
-        self,
-        recs: DataFrame,
-        k: IntOrList,
-    ) -> DataFrame:
+    def _get_metric_distribution(self, recs: DataFrame, k: int) -> DataFrame:
         """
         :param recs: recommendations
-        :param k: one or more depth cut-offs
+        :param k: depth cut-off
         :return: metric distribution for different cut-offs and users
         """
-
-        if isinstance(k, int):
-            k_set = {k}
-        else:
-            k_set = set(k)
         cur_class = self.__class__
         distribution = recs.rdd.flatMap(
             # pylint: disable=protected-access
-            lambda x: cur_class._get_metric_value_by_user_all_k(k_set, *x)
+            lambda x: [
+                (x[0], float(cur_class._get_metric_value_by_user(k, *x[1:])))
+            ]
         ).toDF(
-            f"""user_id {recs.schema["user_id"].dataType.typeName()},
-cum_agg double, k long"""
+            f"user_idx {recs.schema['user_idx'].dataType.typeName()}, value double"
         )
-
         return distribution
 
-    @classmethod
-    def _get_metric_value_by_user_all_k(cls, k_set, user_id, *args):
-        """
-        Calculate metric using multiple depth cut-offs.
-
-        :param k_set: depth cut-offs
-        :param user_id: user identificator
-        :param *args: extra parameters, returned by
-            '''self._get_enriched_recommendations''' method
-        :return: metric values for all users at each cut-off
-        """
-        result = []
-        for k in k_set:
-            result.append(
-                (
-                    user_id,
-                    # pylint: disable=no-value-for-parameter
-                    float(cls._get_metric_value_by_user(k, *args)),
-                    k,
-                )
-            )
-        return result
-
     @staticmethod
     @abstractmethod
     def _get_metric_value_by_user(k, pred, ground_truth) -> float:
         """
         Metric calculation for one user.
 
         :param k: depth cut-off
@@ -229,45 +201,52 @@
         :param log: history DataFrame to calculate number of ratings per user
         :param recommendations: prediction DataFrame
         :param ground_truth: test data
         :param k: depth cut-off
         :return: pandas DataFrame
         """
         log = convert2spark(log)
-        count = log.groupBy("user_id").count()
+        count = log.groupBy("user_idx").count()
         if hasattr(self, "_get_enriched_recommendations"):
             recs = self._get_enriched_recommendations(
                 recommendations, ground_truth
             )
         else:
             recs = get_enriched_recommendations(recommendations, ground_truth)
-        dist = self._get_metric_distribution(recs, k)
-        res = count.join(dist, on="user_id")
-        res = (
-            res.groupBy("k", "count")
-            .agg(sf.avg("cum_agg").alias("value"))
-            .orderBy(["k", "count"])
-            .select("k", "count", "value")
-            .toPandas()
-        )
+        if isinstance(k, int):
+            k_list = [k]
+        else:
+            k_list = k
+        res = pd.DataFrame()
+        for cut_off in k_list:
+            dist = self._get_metric_distribution(recs, cut_off)
+            val = count.join(dist, on="user_idx")
+            val = (
+                val.groupBy("count")
+                .agg(sf.avg("value").alias("value"))
+                .orderBy(["count"])
+                .select("count", "value")
+                .toPandas()
+            )
+            res = res.append(val, ignore_index=True)
         return res
 
 
 # pylint: disable=too-few-public-methods
 class RecOnlyMetric(Metric):
     """Base class for metrics that do not need holdout data"""
 
     @abstractmethod
     def __init__(self, log: AnyDataFrame, *args, **kwargs):
         pass
 
-    @staticmethod
+    # pylint: disable=no-self-use
     @abstractmethod
     def _get_enriched_recommendations(
-        recommendations: AnyDataFrame, ground_truth: AnyDataFrame
+        self, recommendations: AnyDataFrame, ground_truth: AnyDataFrame
     ) -> DataFrame:
         pass
 
     def __call__(  # type: ignore
         self, recommendations: AnyDataFrame, k: IntOrList
     ) -> Union[Dict[int, NumType], NumType]:
         """
```

### Comparing `replay-rec-0.8.0/replay/metrics/coverage.py` & `replay-rec-0.9.0/replay/metrics/coverage.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Dict, Union
 
 from pyspark.sql import Window, DataFrame
 from pyspark.sql import functions as sf
 
 from replay.constants import AnyDataFrame, IntOrList, NumType
 from replay.utils import convert2spark
-from replay.metrics.base_metric import RecOnlyMetric
+from replay.metrics.base_metric import RecOnlyMetric, process_k
 
 
 # pylint: disable=too-few-public-methods, arguments-differ, unused-argument
 class Coverage(RecOnlyMetric):
     """
     Metric calculation is as follows:
 
@@ -24,86 +24,84 @@
         self, log: AnyDataFrame
     ):  # pylint: disable=super-init-not-called
         """
         :param log: pandas or Spark DataFrame
                     It is important for ``log`` to contain all available items.
         """
         self.items = (
-            convert2spark(log).select("item_id").distinct()  # type: ignore
+            convert2spark(log).select("item_idx").distinct()  # type: ignore
         )
         self.item_count = self.items.count()
         self.logger = logging.getLogger("replay")
 
     @staticmethod
     def _get_metric_value_by_user(k, *args):
         # not averaged by users
         pass
 
-    @staticmethod
+    # pylint: disable=no-self-use
     def _get_enriched_recommendations(
-        recommendations: AnyDataFrame, ground_truth: AnyDataFrame
+        self, recommendations: AnyDataFrame, ground_truth: AnyDataFrame
     ) -> DataFrame:
         return convert2spark(recommendations)
 
     def _conf_interval(
         self,
         recs: AnyDataFrame,
-        k: IntOrList,
+        k_list: IntOrList,
         alpha: float = 0.95,
     ) -> Union[Dict[int, float], float]:
-        if isinstance(k, int):
+        if isinstance(k_list, int):
             return 0.0
-        return {i: 0.0 for i in k}
+        return {i: 0.0 for i in k_list}
 
     def _median(
         self,
         recs: AnyDataFrame,
-        k: IntOrList,
+        k_list: IntOrList,
     ) -> Union[Dict[int, NumType], NumType]:
-        return self._mean(recs, k)
+        return self._mean(recs, k_list)
 
+    @process_k
     def _mean(
         self,
         recs: DataFrame,
-        k: IntOrList,
+        k_list: list,
     ) -> Union[Dict[int, NumType], NumType]:
         unknown_item_count = (
-            recs.select("item_id")  # type: ignore
+            recs.select("item_idx")  # type: ignore
             .distinct()
             .exceptAll(self.items)
             .count()
         )
         if unknown_item_count > 0:
             self.logger.warning(
                 "Recommendations contain items that were not present in the log. "
                 "The resulting metric value can be more than 1.0 ¯\_(ツ)_/¯"
             )
 
         best_positions = (
             recs.withColumn(
                 "row_num",
                 sf.row_number().over(
-                    Window.partitionBy("user_id").orderBy(sf.desc("relevance"))
+                    Window.partitionBy("user_idx").orderBy(
+                        sf.desc("relevance")
+                    )
                 ),
             )
-            .select("item_id", "row_num")
-            .groupBy("item_id")
+            .select("item_idx", "row_num")
+            .groupBy("item_idx")
             .agg(sf.min("row_num").alias("best_position"))
             .cache()
         )
 
-        if isinstance(k, int):
-            k_set = {k}
-        else:
-            k_set = set(k)
-
         res = {}
-        for current_k in k_set:
+        for current_k in k_list:
             res[current_k] = (
                 best_positions.filter(
                     sf.col("best_position") <= current_k
                 ).count()
                 / self.item_count
             )
 
         best_positions.unpersist()
-        return self._unpack_if_int(res, k)
+        return res
```

### Comparing `replay-rec-0.8.0/replay/metrics/hitrate.py` & `replay-rec-0.9.0/replay/metrics/hitrate.py`

 * *Files identical despite different names*

### Comparing `replay-rec-0.8.0/replay/metrics/map.py` & `replay-rec-0.9.0/replay/metrics/map.py`

 * *Files identical despite different names*

### Comparing `replay-rec-0.8.0/replay/metrics/mrr.py` & `replay-rec-0.9.0/replay/metrics/mrr.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 class MRR(Metric):
     """
     Mean Reciprocal Rank --
     Reciprocal Rank is the inverse position of the first relevant item among top-k recommendations,
     :math:`\\frac {1}{rank_i}`. This value is averaged by all users.
 
     >>> import pandas as pd
-    >>> pred = pd.DataFrame({"user_id": [1, 1, 1], "item_id": [3, 2, 1], "relevance": [5 ,5, 5]})
-    >>> true = pd.DataFrame({"user_id": [1, 1, 1], "item_id": [2, 4, 5], "relevance": [5, 5, 5]})
+    >>> pred = pd.DataFrame({"user_idx": [1, 1, 1], "item_idx": [3, 2, 1], "relevance": [5 ,5, 5]})
+    >>> true = pd.DataFrame({"user_idx": [1, 1, 1], "item_idx": [2, 4, 5], "relevance": [5, 5, 5]})
     >>> MRR()(pred, true, 3)
     0.5
     >>> MRR()(pred, true, 1)
     0.0
     >>> MRR()(true, pred, 1)
     1.0
     """
```

### Comparing `replay-rec-0.8.0/replay/metrics/ndcg.py` & `replay-rec-0.9.0/replay/metrics/ndcg.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 
     Metric is averaged by users.
 
     .. math::
         nDCG@K = \\frac {\sum_{i=1}^{N}nDCG@K(i)}{N}
 
     >>> import pandas as pd
-    >>> pred=pd.DataFrame({"user_id": [1, 1, 2, 2],
-    ...                    "item_id": [4, 5, 6, 7],
+    >>> pred=pd.DataFrame({"user_idx": [1, 1, 2, 2],
+    ...                    "item_idx": [4, 5, 6, 7],
     ...                    "relevance": [1, 1, 1, 1]})
-    >>> true=pd.DataFrame({"user_id": [1, 1, 1, 1, 1, 2],
-    ...                    "item_id": [1, 2, 3, 4, 5, 8],
+    >>> true=pd.DataFrame({"user_idx": [1, 1, 1, 1, 1, 2],
+    ...                    "item_idx": [1, 2, 3, 4, 5, 8],
     ...                    "relevance": [0.5, 0.1, 0.25, 0.6, 0.2, 0.3]})
     >>> ndcg = NDCG()
     >>> ndcg(pred, true, 2)
     0.5
     """
 
     @staticmethod
```

### Comparing `replay-rec-0.8.0/replay/metrics/precision.py` & `replay-rec-0.9.0/replay/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `replay-rec-0.8.0/replay/metrics/recall.py` & `replay-rec-0.9.0/replay/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `replay-rec-0.8.0/replay/metrics/rocauc.py` & `replay-rec-0.9.0/replay/metrics/rocauc.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 
     Metric is averaged by all users.
 
     .. math::
         ROCAUC@K = \\frac {\sum_{i=1}^{N}ROCAUC@K(i)}{N}
 
     >>> import pandas as pd
-    >>> true=pd.DataFrame({"user_id": 1,
-    ...                    "item_id": [4, 5, 6],
+    >>> true=pd.DataFrame({"user_idx": 1,
+    ...                    "item_idx": [4, 5, 6],
     ...                    "relevance": [1, 1, 1]})
-    >>> pred=pd.DataFrame({"user_id": 1,
-    ...                    "item_id": [1, 2, 3, 4, 5, 6, 7],
+    >>> pred=pd.DataFrame({"user_idx": 1,
+    ...                    "item_idx": [1, 2, 3, 4, 5, 6, 7],
     ...                    "relevance": [0.5, 0.1, 0.25, 0.6, 0.2, 0.3, 0]})
     >>> roc = RocAuc()
     >>> roc(pred, true, 7)
     0.75
 
     """
```

### Comparing `replay-rec-0.8.0/replay/metrics/surprisal.py` & `replay-rec-0.9.0/replay/metrics/surprisal.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,41 +45,40 @@
     ):  # pylint: disable=super-init-not-called
         """
         Here we calculate self-information for each item
 
         :param log: historical data
         """
         self.log = convert2spark(log)
-        n_users = self.log.select("user_id").distinct().count()  # type: ignore
-        self.item_weights = self.log.groupby("item_id").agg(
+        n_users = self.log.select("user_idx").distinct().count()  # type: ignore
+        self.item_weights = self.log.groupby("item_idx").agg(
             (
-                sf.log2(n_users / sf.countDistinct("user_id"))  # type: ignore
+                sf.log2(n_users / sf.countDistinct("user_idx"))  # type: ignore
                 / np.log2(n_users)
             ).alias("rec_weight")
         )
 
     @staticmethod
     def _get_metric_value_by_user(k, *args):
         weigths = args[0]
         return sum(weigths[:k]) / k
 
     def _get_enriched_recommendations(
         self, recommendations: DataFrame, ground_truth: DataFrame
     ) -> DataFrame:
         recommendations = convert2spark(recommendations)
         sort_udf = sf.udf(
-            partial(sorter, index=2),
-            returnType=st.ArrayType(st.DoubleType()),
+            partial(sorter, index=2), returnType=st.ArrayType(st.DoubleType()),
         )
         return (
-            recommendations.join(self.item_weights, on="item_id", how="left")
+            recommendations.join(self.item_weights, on="item_idx", how="left")
             .fillna(1)
-            .groupby("user_id")
+            .groupby("user_idx")
             .agg(
                 sf.collect_list(
-                    sf.struct("relevance", "item_id", "rec_weight")
+                    sf.struct("relevance", "item_idx", "rec_weight")
                 ).alias("rec_weight")
             )
             .select(
-                "user_id", sort_udf(sf.col("rec_weight")).alias("rec_weight")
+                "user_idx", sort_udf(sf.col("rec_weight")).alias("rec_weight")
             )
         )
```

### Comparing `replay-rec-0.8.0/replay/metrics/unexpectedness.py` & `replay-rec-0.9.0/replay/metrics/unexpectedness.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     Fraction of recommended items that are not present in some baseline recommendations.
 
     >>> import pandas as pd
     >>> from replay.session_handler import get_spark_session, State
     >>> spark = get_spark_session(1, 1)
     >>> state = State(spark)
 
-    >>> log = pd.DataFrame({"user_id": [1, 1, 1], "item_id": [1, 2, 3], "relevance": [5, 5, 5], "timestamp": [1, 1, 1]})
-    >>> recs = pd.DataFrame({"user_id": [1, 1, 1], "item_id": [0, 0, 1], "relevance": [5, 5, 5], "timestamp": [1, 1, 1]})
+    >>> log = pd.DataFrame({"user_idx": [1, 1, 1], "item_idx": [1, 2, 3], "relevance": [5, 5, 5], "timestamp": [1, 1, 1]})
+    >>> recs = pd.DataFrame({"user_idx": [1, 1, 1], "item_idx": [0, 0, 1], "relevance": [5, 5, 5], "timestamp": [1, 1, 1]})
     >>> metric = Unexpectedness(log)
     >>> round(metric(recs, 3), 2)
     0.67
     """
 
     def __init__(
         self, pred: AnyDataFrame
@@ -43,40 +43,40 @@
     def _get_enriched_recommendations(
         self, recommendations: DataFrame, ground_truth: DataFrame
     ) -> DataFrame:
         recommendations = convert2spark(recommendations)
         base_pred = self.pred
         sort_udf = sf.udf(
             sorter,
-            returnType=st.ArrayType(base_pred.schema["item_id"].dataType),
+            returnType=st.ArrayType(base_pred.schema["item_idx"].dataType),
         )
         base_recs = (
-            base_pred.groupby("user_id")
+            base_pred.groupby("user_idx")
             .agg(
-                sf.collect_list(sf.struct("relevance", "item_id")).alias(
+                sf.collect_list(sf.struct("relevance", "item_idx")).alias(
                     "base_pred"
                 )
             )
             .select(
-                "user_id", sort_udf(sf.col("base_pred")).alias("base_pred")
+                "user_idx", sort_udf(sf.col("base_pred")).alias("base_pred")
             )
         )
 
         recommendations = (
-            recommendations.groupby("user_id")
+            recommendations.groupby("user_idx")
             .agg(
-                sf.collect_list(sf.struct("relevance", "item_id")).alias(
+                sf.collect_list(sf.struct("relevance", "item_idx")).alias(
                     "pred"
                 )
             )
-            .select("user_id", sort_udf(sf.col("pred")).alias("pred"))
-            .join(base_recs, how="right", on=["user_id"])
+            .select("user_idx", sort_udf(sf.col("pred")).alias("pred"))
+            .join(base_recs, how="right", on=["user_idx"])
         )
         return recommendations.withColumn(
             "pred",
             sf.coalesce(
                 "pred",
                 sf.array().cast(
-                    st.ArrayType(base_pred.schema["item_id"].dataType)
+                    st.ArrayType(base_pred.schema["item_idx"].dataType)
                 ),
             ),
         )
```

### Comparing `replay-rec-0.8.0/replay/model_handler.py` & `replay-rec-0.9.0/replay/model_handler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # pylint: disable=wildcard-import,invalid-name,unused-wildcard-import,unspecified-encoding
 import os
 import json
 import shutil
 from inspect import getfullargspec
 
-from pyspark.ml.feature import StringIndexerModel, IndexToString
+import joblib
 from os.path import exists, join
 
+from pyspark.ml.feature import StringIndexerModel, IndexToString
+
+from replay.data_preparator import Indexer
 from replay.models import *
 from replay.models.base_rec import BaseRecommender
 from replay.session_handler import State
 
 
 def save(model: BaseRecommender, path: str):
     """
@@ -26,24 +29,70 @@
     model._save_model(join(path, "model"))
 
     init_args = model._init_args
     init_args["_model_name"] = str(model)
     with open(join(path, "init_args.json"), "w") as json_file:
         json.dump(init_args, json_file)
 
-    model.user_indexer.save(join(path, "user_indexer"))
-    model.item_indexer.save(join(path, "item_indexer"))
-    model.inv_user_indexer.save(join(path, "inv_user_indexer"))
-    model.inv_item_indexer.save(join(path, "inv_item_indexer"))
-
     dataframes = model._dataframes
     df_path = join(path, "dataframes")
     os.makedirs(df_path)
     for name, df in dataframes.items():
         df.write.parquet(join(df_path, name))
+    model.fit_users.write.parquet(join(df_path, "fit_users"))
+    model.fit_items.write.parquet(join(df_path, "fit_items"))
+
+    joblib.dump(model.study, join(path, "study"))
+
+
+def save_indexer(indexer: Indexer, path: str):
+    """
+    Save fitted indexer to disk as a folder
+
+    :param indexer: Trained indexer
+    :param path: destination where indexer files will be stored
+    :return:
+    """
+    if exists(path):
+        shutil.rmtree(path)
+    os.makedirs(path)
+
+    init_args = indexer._init_args
+    with open(join(path, "init_args.json"), "w") as json_file:
+        json.dump(init_args, json_file)
+
+    indexer.user_indexer.save(join(path, "user_indexer"))
+    indexer.item_indexer.save(join(path, "item_indexer"))
+    indexer.inv_user_indexer.save(join(path, "inv_user_indexer"))
+    indexer.inv_item_indexer.save(join(path, "inv_item_indexer"))
+
+
+def load_indexer(path: str):
+    """
+    Load saved indexer from disk
+
+    :param path: path to folder
+    :return: Restored trained model
+    """
+    State()
+    with open(join(path, "init_args.json"), "r") as json_file:
+        args = json.load(json_file)
+
+    indexer = Indexer(**args)
+
+    indexer.user_indexer = StringIndexerModel.load(join(path, "user_indexer"))
+    indexer.item_indexer = StringIndexerModel.load(join(path, "item_indexer"))
+    indexer.inv_user_indexer = IndexToString.load(
+        join(path, "inv_user_indexer")
+    )
+    indexer.inv_item_indexer = IndexToString.load(
+        join(path, "inv_item_indexer")
+    )
+
+    return indexer
 
 
 def load(path: str):
     """
     Load saved model from disk
 
     :param path: path to model folder
@@ -66,20 +115,16 @@
         init_args = args
         extra_args = {}
 
     model = model_class(**init_args)
     for arg in extra_args:
         model.arg = extra_args[arg]
 
-    model.user_indexer = StringIndexerModel.load(join(path, "user_indexer"))
-    model.item_indexer = StringIndexerModel.load(join(path, "item_indexer"))
-    model.inv_user_indexer = IndexToString.load(join(path, "inv_user_indexer"))
-    model.inv_item_indexer = IndexToString.load(join(path, "inv_item_indexer"))
-
     df_path = join(path, "dataframes")
     dataframes = os.listdir(df_path)
     for name in dataframes:
         df = spark.read.parquet(join(df_path, name))
         setattr(model, name, df)
 
     model._load_model(join(path, "model"))
+    model.study = joblib.load(join(path, "study"))
     return model
```

### Comparing `replay-rec-0.8.0/replay/models/__init__.py` & `replay-rec-0.9.0/replay/models/__init__.py`

 * *Files identical despite different names*

### Comparing `replay-rec-0.8.0/replay/models/admm_slim.py` & `replay-rec-0.9.0/replay/models/admm_slim.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ):  # pragma: no cover
 
     # calculate mat_b
     mat_b = p_x + np.dot(inv_matrix, rho * mat_c - mat_gamma)
     vec_gamma = np.diag(mat_b) / np.diag(inv_matrix)
     mat_b -= inv_matrix * vec_gamma
 
-    # calculate mat_с
+    # calculate mat_c
     prev_mat_c = mat_c
     mat_c = mat_b + mat_gamma / rho
     coef = lambda_1 / rho
     mat_c = np.maximum(mat_c - coef, 0.0) - np.maximum(-mat_c - coef, 0.0)
 
     # calculate mat_gamma
     mat_gamma += rho * (mat_b - mat_c)
@@ -124,25 +124,25 @@
         self.logger.debug("Fitting ADMM SLIM")
         pandas_log = log.select("user_idx", "item_idx", "relevance").toPandas()
         interactions_matrix = csr_matrix(
             (
                 pandas_log["relevance"],
                 (pandas_log["user_idx"], pandas_log["item_idx"]),
             ),
-            shape=(self.users_count, self.items_count),
+            shape=(self._user_dim, self._item_dim),
         )
         self.logger.debug("Gram matrix")
         xtx = (interactions_matrix.T @ interactions_matrix).toarray()
         self.logger.debug("Inverse matrix")
         inv_matrix = np.linalg.inv(
-            xtx + (self.lambda_2 + self.rho) * np.eye(self.items_count)
+            xtx + (self.lambda_2 + self.rho) * np.eye(self._item_dim)
         )
         self.logger.debug("Main calculations")
         p_x = inv_matrix @ xtx
-        mat_b, mat_c, mat_gamma = self._init_matrix(self.items_count)
+        mat_b, mat_c, mat_gamma = self._init_matrix(self._item_dim)
         r_primal = np.linalg.norm(mat_b - mat_c)
         r_dual = np.linalg.norm(self.rho * mat_c)
         eps_primal, eps_dual = 0.0, 0.0
         iteration = 0
         while (
             r_primal > eps_primal or r_dual > eps_dual
         ) and iteration < self.max_iteration:
@@ -162,36 +162,36 @@
                 mat_b,
                 mat_c,
                 mat_gamma,
                 self.rho,
                 self.eps_abs,
                 self.eps_rel,
                 self.lambda_1,
-                self.items_count,
+                self._item_dim,
                 self.threshold,
                 self.multiplicator,
             )
             result_message = (
                 f"Iteration: {iteration}. primal gap: "
                 f"{r_primal - eps_primal:.5}; dual gap: "
                 f" {r_dual - eps_dual:.5}; rho: {self.rho}"
             )
             self.logger.debug(result_message)
 
         mat_c_sparse = coo_matrix(mat_c)
         mat_c_pd = pd.DataFrame(
             {
-                "item_id_one": mat_c_sparse.row.astype(np.int32),
-                "item_id_two": mat_c_sparse.col.astype(np.int32),
+                "item_idx_one": mat_c_sparse.row.astype(np.int32),
+                "item_idx_two": mat_c_sparse.col.astype(np.int32),
                 "similarity": mat_c_sparse.data,
             }
         )
         self.similarity = State().session.createDataFrame(
             mat_c_pd,
-            schema="item_id_one int, item_id_two int, similarity double",
+            schema="item_idx_one int, item_idx_two int, similarity double",
         )
         self.similarity.cache()
 
     def _init_matrix(
         self, size: int
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """Matrix initialization"""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `replay-rec-0.8.0/replay/models/als.py` & `replay-rec-0.9.0/replay/models/als.py`

 * *Files identical despite different names*

### Comparing `replay-rec-0.8.0/replay/models/association_rules.py` & `replay-rec-0.9.0/replay/models/association_rules.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,116 +11,158 @@
 
 
 class AssociationRulesItemRec(Recommender):
     """
     Item-to-item recommender based on association rules.
     Calculate pairs confidence, lift and confidence_gain defined as
     confidence(a, b)/confidence(!a, b) to get top-k associated items.
+
+    Classical model uses items co-occurrence in sessions for
+    confidence, lift and confidence_gain calculation
+    but relevance could also be passed to the model, e.g.
+    if you want to apply time smoothing and treat old sessions as less important.
+    In this case all items in sessions should have the same relevance.
     """
 
     can_predict_item_to_item = True
     item_to_item_metrics: List[str] = ["lift", "confidence_gain"]
     pair_metrics: DataFrame
 
+    # pylint: disable=too-many-arguments,
     def __init__(
         self,
         session_col: Optional[str] = None,
         min_item_count: int = 5,
         min_pair_count: int = 5,
         num_neighbours: Optional[int] = 1000,
+        use_relevance: bool = False,
     ) -> None:
         """
         :param session_col: name of column to group sessions.
             Items are combined by the ``user_id`` column if ``session_col`` is not defined.
         :param min_item_count: items with fewer sessions will be filtered out
         :param min_pair_count: pairs with fewer sessions will be filtered out
         :param num_neighbours: maximal number of neighbours to save for each item
+        :param use_relevance: flag to use relevance values instead of co-occurrence count
+            If true, pair relevance in session is minimal relevance of item in pair.
+            Item relevance is sum of relevance in all sessions.
         """
         self.session_col = (
             session_col if session_col is not None else "user_idx"
         )
         self.min_item_count = min_item_count
         self.min_pair_count = min_pair_count
         self.num_neighbours = num_neighbours
+        self.use_relevance = use_relevance
 
     @property
     def _init_args(self):
         return {
             "session_col": self.session_col,
             "min_item_count": self.min_item_count,
             "min_pair_count": self.min_pair_count,
             "num_neighbours": self.num_neighbours,
+            "use_relevance": self.use_relevance,
         }
 
     def _fit(
         self,
         log: DataFrame,
         user_features: Optional[DataFrame] = None,
         item_features: Optional[DataFrame] = None,
     ) -> None:
         """
         1) Filter log items by ``min_item_count`` threshold
         2) Calculate items support, pairs confidence, lift and confidence_gain defined as
             confidence(a, b)/confidence(!a, b).
         """
-        log = log.select(self.session_col, "item_idx").distinct()
+        rel_col = sf.col("relevance") if self.use_relevance else sf.lit(1)
+        log = log.select(
+            self.session_col, "item_idx", rel_col.alias("relevance")
+        ).distinct()
         num_sessions = log.select(self.session_col).distinct().count()
 
-        frequent_items = (
+        frequent_items_cached = (
             log.groupBy("item_idx")
-            .agg(sf.count("item_idx").alias("item_count"))
+            .agg(
+                sf.count("item_idx").alias("item_count"),
+                sf.sum("relevance").alias("item_relevance"),
+            )
             .filter(sf.col("item_count") >= self.min_item_count)
+            .drop("item_count")
         ).cache()
 
         frequent_items_log = log.join(
-            frequent_items.select("item_idx"), on="item_idx"
+            frequent_items_cached.select("item_idx"), on="item_idx"
         )
 
         frequent_item_pairs = (
             frequent_items_log.withColumnRenamed("item_idx", "antecedent")
+            .withColumnRenamed("relevance", "antecedent_rel")
             .join(
                 frequent_items_log.withColumnRenamed(
                     self.session_col, self.session_col + "_cons"
-                ).withColumnRenamed("item_idx", "consequent"),
+                )
+                .withColumnRenamed("item_idx", "consequent")
+                .withColumnRenamed("relevance", "consequent_rel"),
                 on=[
                     sf.col(self.session_col)
                     == sf.col(self.session_col + "_cons"),
                     sf.col("antecedent") < sf.col("consequent"),
                 ],
             )
-            .drop(self.session_col + "_cons")
+            # taking minimal relevance of item for pair
+            .withColumn(
+                "relevance",
+                sf.least(sf.col("consequent_rel"), sf.col("antecedent_rel")),
+            )
+            .drop(
+                self.session_col + "_cons", "consequent_rel", "antecedent_rel"
+            )
         )
+
         pairs_count = (
             frequent_item_pairs.groupBy("antecedent", "consequent")
-            .agg(sf.count("consequent").alias("pair_count"))
+            .agg(
+                sf.count("consequent").alias("pair_count"),
+                sf.sum("relevance").alias("pair_relevance"),
+            )
             .filter(sf.col("pair_count") >= self.min_pair_count)
-        )
+        ).drop("pair_count")
 
         pairs_metrics = pairs_count.unionByName(
             pairs_count.select(
                 sf.col("consequent").alias("antecedent"),
                 sf.col("antecedent").alias("consequent"),
-                sf.col("pair_count"),
+                sf.col("pair_relevance"),
             )
         )
+
         pairs_metrics = pairs_metrics.join(
-            frequent_items.withColumnRenamed("item_count", "antecedent_count"),
+            frequent_items_cached.withColumnRenamed(
+                "item_relevance", "antecedent_relevance"
+            ),
             on=[sf.col("antecedent") == sf.col("item_idx")],
         ).drop("item_idx")
 
         pairs_metrics = pairs_metrics.join(
-            frequent_items.withColumnRenamed("item_count", "consequent_count"),
+            frequent_items_cached.withColumnRenamed(
+                "item_relevance", "consequent_relevance"
+            ),
             on=[sf.col("consequent") == sf.col("item_idx")],
         ).drop("item_idx")
 
         pairs_metrics = pairs_metrics.withColumn(
-            "confidence", sf.col("pair_count") / sf.col("antecedent_count")
+            "confidence",
+            sf.col("pair_relevance") / sf.col("antecedent_relevance"),
         ).withColumn(
             "lift",
-            num_sessions * sf.col("confidence") / sf.col("consequent_count"),
+            num_sessions
+            * sf.col("confidence")
+            / sf.col("consequent_relevance"),
         )
 
         if self.num_neighbours is not None:
             pairs_metrics = (
                 pairs_metrics.withColumn(
                     "similarity_order",
                     sf.row_number().over(
@@ -133,31 +175,36 @@
                 .drop("similarity_order")
             )
 
         self.pair_metrics = (
             pairs_metrics.withColumn(
                 "confidence_gain",
                 sf.when(
-                    sf.col("consequent_count") - sf.col("pair_count") == 0,
+                    sf.col("consequent_relevance") - sf.col("pair_relevance")
+                    == 0,
                     sf.lit(np.inf),
                 ).otherwise(
                     sf.col("confidence")
-                    * (num_sessions - sf.col("antecedent_count"))
-                    / (sf.col("consequent_count") - sf.col("pair_count"))
+                    * (num_sessions - sf.col("antecedent_relevance"))
+                    / (
+                        sf.col("consequent_relevance")
+                        - sf.col("pair_relevance")
+                    )
                 ),
             )
             .select(
                 "antecedent",
                 "consequent",
                 "confidence",
                 "lift",
                 "confidence_gain",
             )
             .cache()
         )
+        frequent_items_cached.unpersist()
 
     # pylint: disable=too-many-arguments
     def _predict(
         self,
         log: DataFrame,
         k: int,
         users: DataFrame,
@@ -167,35 +214,21 @@
         filter_seen_items: bool = True,
     ) -> None:
         raise NotImplementedError(
             f"item-to-user predict is not implemented for {self.__str__()}, "
             f"use get_nearest_items method to get item-to-item recommendations"
         )
 
+    @property
     def get_pair_metrics(self):
         """
         Return matrix with calculated confidence, lift and confidence gain.
         :return: association rules measures calculated during ``fit`` stage
         """
-        res = (
-            self.inv_item_indexer.transform(
-                self.pair_metrics.withColumnRenamed("antecedent", "item_idx")
-            )
-            .drop("item_idx")
-            .withColumnRenamed("item_id", "antecedent")
-        )
-
-        res = (
-            self.inv_item_indexer.transform(
-                res.withColumnRenamed("consequent", "item_idx")
-            )
-            .drop("item_idx")
-            .withColumnRenamed("item_id", "consequent")
-        )
-        return res
+        return self.pair_metrics
 
     def get_nearest_items(
         self,
         items: Union[DataFrame, Iterable],
         k: int,
         metric: Optional[str] = "lift",
         candidates: Optional[Union[DataFrame, Iterable]] = None,
@@ -244,21 +277,21 @@
                 sf.broadcast(
                     candidates.withColumnRenamed("item_idx", "consequent")
                 ),
                 on="consequent",
             )
 
         return (
-            pairs_to_consider.withColumnRenamed("antecedent", "item_id_one")
-            .withColumnRenamed("consequent", "item_id_two")
+            pairs_to_consider.withColumnRenamed("antecedent", "item_idx_one")
+            .withColumnRenamed("consequent", "item_idx_two")
             .join(
                 sf.broadcast(
-                    items.withColumnRenamed("item_idx", "item_id_one")
+                    items.withColumnRenamed("item_idx", "item_idx_one")
                 ),
-                on="item_id_one",
+                on="item_idx_one",
             )
         )
 
     def _clear_cache(self):
         if hasattr(self, "pair_metrics"):
             unpersist_if_exists(self.pair_metrics)
```

### Comparing `replay-rec-0.8.0/replay/models/base_rec.py` & `replay-rec-0.9.0/replay/models/base_rec.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,58 +14,60 @@
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from typing import Any, Dict, Iterable, List, Optional, Union, Sequence, Tuple
 
 import pandas as pd
 from optuna import create_study
 from optuna.samplers import TPESampler
-from pyspark.ml.feature import IndexToString, StringIndexer, StringIndexerModel
 from pyspark.sql import DataFrame, Window
 from pyspark.sql import functions as sf
 from pyspark.sql.column import Column
 
-from replay.constants import AnyDataFrame
 from replay.metrics import Metric, NDCG
 from replay.optuna_objective import SplitData, MainObjective
 from replay.session_handler import State
 from replay.utils import (
     convert2spark,
     cosine_similarity,
     get_top_k,
     get_top_k_recs,
     vector_euclidean_distance_similarity,
     vector_dot,
 )
 
 
+# pylint: disable=too-many-instance-attributes
 class BaseRecommender(ABC):
     """Base recommender"""
 
     model: Any
-    user_indexer: StringIndexerModel
-    item_indexer: StringIndexerModel
-    inv_user_indexer: IndexToString
-    inv_item_indexer: IndexToString
     _logger: Optional[logging.Logger] = None
     can_predict_cold_users: bool = False
     can_predict_cold_items: bool = False
     can_predict_item_to_item: bool = False
     _search_space: Optional[
         Dict[str, Union[str, Sequence[Union[str, int, float]]]]
     ] = None
     _objective = MainObjective
     study = None
+    fit_users: DataFrame
+    fit_items: DataFrame
+    fit_statistics: Optional[Dict[str, int]]
+    _num_users: int
+    _num_items: int
+    _user_dim_size: int
+    _item_dim_size: int
 
     # pylint: disable=too-many-arguments, too-many-locals, no-member
     def optimize(
         self,
-        train: AnyDataFrame,
-        test: AnyDataFrame,
-        user_features: Optional[AnyDataFrame] = None,
-        item_features: Optional[AnyDataFrame] = None,
+        train: DataFrame,
+        test: DataFrame,
+        user_features: Optional[DataFrame] = None,
+        item_features: Optional[DataFrame] = None,
         param_borders: Optional[Dict[str, List[Any]]] = None,
         criterion: Metric = NDCG(),
         k: int = 10,
         budget: int = 10,
         new_study: bool = True,
     ) -> Optional[Dict[str, Any]]:
         """
@@ -206,38 +208,36 @@
                 Hyper parameter {param} is numerical
                  but bounds are not in ([lower, upper]) format
                 """
             )
 
     def _prepare_split_data(
         self,
-        train: AnyDataFrame,
-        test: AnyDataFrame,
-        user_features: Optional[AnyDataFrame] = None,
-        item_features: Optional[AnyDataFrame] = None,
+        train: DataFrame,
+        test: DataFrame,
+        user_features: Optional[DataFrame] = None,
+        item_features: Optional[DataFrame] = None,
     ) -> SplitData:
         """
         This method converts data to spark and packs it into a named tuple to pass into optuna.
 
         :param train: train data
         :param test: test data
         :param user_features: user features
         :param item_features: item features
         :return: packed PySpark DataFrames
         """
-        train = convert2spark(train)
-        test = convert2spark(test)
         user_features_train, user_features_test = self._train_test_features(
-            train, test, user_features, "user_id"
+            train, test, user_features, "user_idx"
         )
         item_features_train, item_features_test = self._train_test_features(
-            train, test, item_features, "item_id"
+            train, test, item_features, "item_idx"
         )
-        users = test.select("user_id").distinct()
-        items = test.select("item_id").distinct()
+        users = test.select("user_idx").distinct()
+        items = test.select("item_idx").distinct()
         split_data = SplitData(
             train,
             test,
             users,
             items,
             user_features_train,
             user_features_test,
@@ -256,29 +256,28 @@
     def _load_model(self, path: str):
         pass
 
     @staticmethod
     def _train_test_features(
         train: DataFrame,
         test: DataFrame,
-        features: Optional[AnyDataFrame],
+        features: Optional[DataFrame],
         column: Union[str, Column],
     ) -> Tuple[Optional[DataFrame], Optional[DataFrame]]:
         """
         split dataframe with features into two dataframes representing
         features for train and tests subset entities, defined by `column`
 
         :param train: spark dataframe with the train subset
         :param test: spark dataframe with the train subset
         :param features: spark dataframe with users'/items' features
-        :param column: column name to use as a key for join (e.g., user_id or item_id)
+        :param column: column name to use as a key for join (e.g., user_idx or item_idx)
         :return: features for train and test subsets
         """
         if features is not None:
-            features = convert2spark(features)
             features_train = features.join(
                 train.select(column).distinct(), on=column
             )
             features_test = features.join(
                 test.select(column).distinct(), on=column
             )
         else:
@@ -298,160 +297,175 @@
         self._clear_cache()
 
     def __str__(self):
         return type(self).__name__
 
     def _fit_wrap(
         self,
-        log: AnyDataFrame,
-        user_features: Optional[AnyDataFrame] = None,
-        item_features: Optional[AnyDataFrame] = None,
-        force_reindex: bool = True,
+        log: DataFrame,
+        user_features: Optional[DataFrame] = None,
+        item_features: Optional[DataFrame] = None,
     ) -> None:
         """
         Wrapper for fit to allow for fewer arguments in a model.
 
         :param log: historical log of interactions
-            ``[user_id, item_id, timestamp, relevance]``
+            ``[user_idx, item_idx, timestamp, relevance]``
         :param user_features: user features
-            ``[user_id, timestamp]`` + feature columns
+            ``[user_idx, timestamp]`` + feature columns
         :param item_features: item features
-            ``[item_id, timestamp]`` + feature columns
-        :param force_reindex: create indexers again, even if they were created previously
+            ``[item_idx, timestamp]`` + feature columns
         :return:
         """
         self.logger.debug("Starting fit %s", type(self).__name__)
-        log, user_features, item_features = [
-            convert2spark(df) for df in [log, user_features, item_features]
-        ]
-
-        if "user_indexer" not in self.__dict__ or force_reindex:
-            self.logger.debug("Creating indexers")
-            self._create_indexers(log, user_features, item_features)
-        self.logger.debug("Main fit stage")
-
-        log, user_features, item_features = [
-            self._convert_index(df)
-            for df in [log, user_features, item_features]
-        ]
-        self._fit(log, user_features, item_features)
-
-    def _create_indexers(
-        self,
-        log: DataFrame,
-        user_features: Optional[DataFrame] = None,
-        item_features: Optional[DataFrame] = None,
-    ) -> None:
-        """
-        Creates indexers to map raw id to numerical idx so that spark can handle them.
-        :param log: historical log of interactions
-            ``[user_id, item_id, timestamp, relevance]``
-        :param user_features: user features (must have ``user_id``)
-        :param item_features: item features (must have ``item_id``)
-        :return:
-        """
         if user_features is None:
-            users = log.select("user_id")
+            users = log.select("user_idx").distinct()
         else:
-            users = log.select("user_id").union(
-                user_features.select("user_id")
+            users = (
+                log.select("user_idx")
+                .union(user_features.select("user_idx"))
+                .distinct()
             )
         if item_features is None:
-            items = log.select("item_id")
+            items = log.select("item_idx").distinct()
         else:
-            items = log.select("item_id").union(
-                item_features.select("item_id")
-            )
-        self.user_indexer = StringIndexer(
-            inputCol="user_id", outputCol="user_idx"
-        ).fit(users)
-        self.item_indexer = StringIndexer(
-            inputCol="item_id", outputCol="item_idx"
-        ).fit(items)
-        self.inv_user_indexer = IndexToString(
-            inputCol="user_idx",
-            outputCol="user_id",
-            labels=self.user_indexer.labels,
-        )
-        self.inv_item_indexer = IndexToString(
-            inputCol="item_idx",
-            outputCol="item_id",
-            labels=self.item_indexer.labels,
+            items = (
+                log.select("item_idx")
+                .union(item_features.select("item_idx"))
+                .distinct()
+            )
+        self.fit_users = users.cache()
+        self.fit_items = items.cache()
+        self._num_users = self.fit_users.count()
+        self._num_items = self.fit_items.count()
+        self._user_dim_size = (
+            self.fit_users.agg({"user_idx": "max"}).collect()[0][0] + 1
         )
+        self._item_dim_size = (
+            self.fit_items.agg({"item_idx": "max"}).collect()[0][0] + 1
+        )
+        self._fit(log, user_features, item_features)
 
     @abstractmethod
     def _fit(
         self,
         log: DataFrame,
         user_features: Optional[DataFrame] = None,
         item_features: Optional[DataFrame] = None,
     ) -> None:
         """
         Inner method where model actually fits.
 
         :param log: historical log of interactions
-            ``[user_id, item_id, timestamp, relevance]``
+            ``[user_idx, item_idx, timestamp, relevance]``
         :param user_features: user features
-            ``[user_id, timestamp]`` + feature columns
+            ``[user_idx, timestamp]`` + feature columns
         :param item_features: item features
-            ``[item_id, timestamp]`` + feature columns
+            ``[item_idx, timestamp]`` + feature columns
         :return:
         """
 
+    @staticmethod
+    def _filter_seen(
+        recs: DataFrame, log: DataFrame, k: int, users: DataFrame
+    ):
+        """
+        Filter seen items (presented in log) out of the users' recommendations.
+        For each user return from `k` to `k + number of seen by user` recommendations.
+        """
+
+        users_log = log.join(users, on="user_idx").cache()
+        num_seen = (
+            users_log.groupBy("user_idx").agg(
+                sf.count("item_idx").alias("seen_count")
+            )
+        ).cache()
+
+        # count maximal number of items seen by users
+        max_seen = 0
+        if num_seen.count() > 0:
+            max_seen = num_seen.select(sf.max("seen_count")).collect()[0][0]
+
+        # crop recommendations to first k + max_seen items for each user
+        recs = recs.withColumn(
+            "temp_rank",
+            sf.row_number().over(
+                Window.partitionBy("user_idx").orderBy(
+                    sf.col("relevance").desc()
+                )
+            ),
+        ).filter(sf.col("temp_rank") <= sf.lit(max_seen + k))
+
+        # leave k + number of items seen by user recommendations in recs
+        recs = (
+            recs.join(num_seen, on="user_idx", how="left")
+            .fillna(0)
+            .filter(sf.col("temp_rank") <= sf.col("seen_count") + sf.lit(k))
+            .drop("temp_rank", "seen_count")
+        )
+
+        # filter recommendations presented in interactions log
+        recs = recs.join(
+            users_log.withColumnRenamed("item_idx", "item")
+            .withColumnRenamed("user_idx", "user")
+            .select("user", "item"),
+            on=(sf.col("user_idx") == sf.col("user"))
+            & (sf.col("item_idx") == sf.col("item")),
+            how="anti",
+        ).drop("user", "item")
+
+        users_log.unpersist()
+        num_seen.unpersist()
+
+        return recs
+
     # pylint: disable=too-many-arguments
     def _predict_wrap(
         self,
-        log: Optional[AnyDataFrame],
+        log: Optional[DataFrame],
         k: int,
-        users: Optional[Union[AnyDataFrame, Iterable]] = None,
-        items: Optional[Union[AnyDataFrame, Iterable]] = None,
-        user_features: Optional[AnyDataFrame] = None,
-        item_features: Optional[AnyDataFrame] = None,
+        users: Optional[Union[DataFrame, Iterable]] = None,
+        items: Optional[Union[DataFrame, Iterable]] = None,
+        user_features: Optional[DataFrame] = None,
+        item_features: Optional[DataFrame] = None,
         filter_seen_items: bool = True,
     ) -> DataFrame:
         """
         Predict wrapper to allow for fewer parameters in models
 
         :param log: historical log of interactions
-            ``[user_id, item_id, timestamp, relevance]``
-        :param k: length of recommendation lists, should be less that the total number of ``items``
+            ``[user_idx, item_idx, timestamp, relevance]``
+        :param k: number of recommendations for each user
         :param users: users to create recommendations for
-            dataframe containing ``[user_id]`` or ``array-like``;
+            dataframe containing ``[user_idx]`` or ``array-like``;
             if ``None``, recommend to all users from ``log``
         :param items: candidate items for recommendations
-            dataframe containing ``[item_id]`` or ``array-like``;
+            dataframe containing ``[item_idx]`` or ``array-like``;
             if ``None``, take all items from ``log``.
             If it contains new items, ``relevance`` for them will be ``0``.
         :param user_features: user features
-            ``[user_id , timestamp]`` + feature columns
+            ``[user_idx , timestamp]`` + feature columns
         :param item_features: item features
-            ``[item_id , timestamp]`` + feature columns
+            ``[item_idx , timestamp]`` + feature columns
         :param filter_seen_items: flag to remove seen items from recommendations based on ``log``.
         :return: recommendation dataframe
-            ``[user_id, item_id, relevance]``
+            ``[user_idx, item_idx, relevance]``
         """
         self.logger.debug("Starting predict %s", type(self).__name__)
-
-        log, user_features, item_features = [
-            convert2spark(df) for df in [log, user_features, item_features]
-        ]
-
-        user_data = users or log or user_features or self.user_indexer.labels
-        users = self._get_ids(user_data, "user_id")
-
-        item_data = items or log or item_features or self.item_indexer.labels
-        items = self._get_ids(item_data, "item_id")
-
-        users_type = users.schema["user_id"].dataType
-        items_type = items.schema["item_id"].dataType
-
-        log, user_features, item_features, users, items = [
-            self._convert_index(df)
-            for df in [log, user_features, item_features, users, items]
-        ]
+        user_data = users or log or user_features or self.fit_users
+        users = self._get_ids(user_data, "user_idx")
+        users = self._filter_ids(users, "user_idx")
+
+        item_data = items or self.fit_items
+        items = self._get_ids(item_data, "item_idx")
+        items = self._filter_ids(items, "item_idx")
+
+        if log is not None:
+            log = self._filter_ids(log, "user_idx")
+            log = self._filter_ids(log, "item_idx")
 
         num_items = items.count()
         if num_items < k:
             message = f"k = {k} > number of items = {num_items}"
             self.logger.debug(message)
 
         recs = self._predict(
@@ -460,141 +474,23 @@
             users,
             items,
             user_features,
             item_features,
             filter_seen_items,
         )
         if filter_seen_items and log:
-            num_of_seen = (
-                log.groupBy("user_idx")
-                .agg(sf.count("item_idx").alias("seen_count"))
-                .cache()
-            )
-
-            max_seen = num_of_seen.select(sf.max("seen_count")).collect()[0][0]
-
-            recs = recs.withColumn(
-                "temp_rank",
-                sf.row_number().over(
-                    Window.partitionBy("user_idx").orderBy(
-                        sf.col("relevance").desc()
-                    )
-                ),
-            ).filter(sf.col("temp_rank") <= sf.lit(max_seen + k))
-
-            recs = (
-                recs.join(sf.broadcast(num_of_seen), on="user_idx", how="left")
-                .fillna(0)
-                .filter(
-                    sf.col("temp_rank") <= sf.col("seen_count") + sf.lit(k)
-                )
-                .drop("temp_rank", "seen_count")
-            )
-            num_of_seen.unpersist()
-
-            recs = recs.join(
-                log.withColumnRenamed("item_idx", "item")
-                .withColumnRenamed("user_idx", "user")
-                .select("user", "item"),
-                on=(sf.col("user_idx") == sf.col("user"))
-                & (sf.col("item_idx") == sf.col("item")),
-                how="anti",
-            ).drop("user", "item")
+            recs = self._filter_seen(recs=recs, log=log, users=users, k=k)
 
-        recs = self._convert_back(recs, users_type, items_type).select(
-            "user_id", "item_id", "relevance"
-        )
-        return get_top_k_recs(recs, k=k)
-
-    def _convert_index(
-        self, data_frame: Optional[DataFrame]
-    ) -> Optional[DataFrame]:
-        """
-        Convert raw ``user_id`` and ``item_id`` to numerical ``user_idx`` and ``item_idx``
-
-        :param data_frame: dataframe with raw indexes
-        :return: dataframe with converted indexes
-        """
-        if data_frame is None:
-            return None
-        if "user_id" in data_frame.columns:
-            self._reindex("user", data_frame)
-            data_frame = self.user_indexer.transform(data_frame).drop(
-                "user_id"
-            )
-            data_frame = data_frame.withColumn(
-                "user_idx", sf.col("user_idx").cast("int")
-            )
-        if "item_id" in data_frame.columns:
-            self._reindex("item", data_frame)
-            data_frame = self.item_indexer.transform(data_frame).drop(
-                "item_id"
-            )
-            data_frame = data_frame.withColumn(
-                "item_idx", sf.col("item_idx").cast("int")
-            )
-        return data_frame
-
-    def _convert_back(self, log, user_type, item_type):
-        res = log
-        if "user_idx" in log.columns:
-            res = (
-                self.inv_user_indexer.transform(res)
-                .drop("user_idx")
-                .withColumn("user_id", sf.col("user_id").cast(user_type))
-            )
-        if "item_idx" in log.columns:
-            res = (
-                self.inv_item_indexer.transform(res)
-                .drop("item_idx")
-                .withColumn("item_id", sf.col("item_id").cast(item_type))
-            )
-        return res
-
-    def _reindex(self, entity: str, objects: DataFrame):
-        """
-        Reindex users or items. If recommender can process cold entities,
-        indexer is updated with new entries.
-
-        :param entity: user or item
-        :param objects: unique users/items
-        """
-        indexer = getattr(self, f"{entity}_indexer")
-        inv_indexer = getattr(self, f"inv_{entity}_indexer")
-        can_reindex = getattr(self, f"can_predict_cold_{entity}s")
-        new_objects = set(
-            map(
-                str,
-                objects.select(sf.collect_list(indexer.getInputCol())).first()[
-                    0
-                ],
-            )
-        ).difference(indexer.labels)
-        if new_objects:
-            if can_reindex:
-                new_labels = indexer.labels + list(new_objects)
-                setattr(
-                    self,
-                    f"{entity}_indexer",
-                    indexer.from_labels(
-                        new_labels,
-                        inputCol=indexer.getInputCol(),
-                        outputCol=indexer.getOutputCol(),
-                        handleInvalid="error",
-                    ),
-                )
-                inv_indexer.setLabels(new_labels)
-            else:
-                message = f"{entity} contains cold elements, recommendations won't be complete."
-                self.logger.warning(message)
-                indexer.setHandleInvalid("skip")
+        recs = get_top_k_recs(recs, k=k)
+        return recs.select("user_idx", "item_idx", "relevance")
 
     @staticmethod
     def _get_ids(
-        log: Union[Iterable, AnyDataFrame], column: str,
+        log: Union[Iterable, DataFrame],
+        column: str,
     ) -> DataFrame:
         """
         Get unique values from ``array`` and put them into dataframe with column ``column``.
         """
         spark = State().session
         if isinstance(log, DataFrame):
             unique = log.select(column).distinct()
@@ -602,14 +498,27 @@
             unique = spark.createDataFrame(
                 data=pd.DataFrame(pd.unique(list(log)), columns=[column])
             )
         else:
             raise ValueError(f"Wrong type {type(log)}")
         return unique
 
+    def _filter_ids(self, log: DataFrame, column: str) -> DataFrame:
+        """
+        Filter out new ids if the model cannot predict cold items
+        """
+        entity = column.split("_")[0]
+        if getattr(self, f"can_predict_cold_{entity}s"):
+            return log
+        self.logger.warning(
+            "This model can't predict cold %ss, they will be ignored", entity
+        )
+        res = log.join(getattr(self, f"fit_{entity}s"), on=column, how="inner")
+        return res
+
     # pylint: disable=too-many-arguments
     @abstractmethod
     def _predict(
         self,
         log: DataFrame,
         k: int,
         users: DataFrame,
@@ -618,77 +527,101 @@
         item_features: Optional[DataFrame] = None,
         filter_seen_items: bool = True,
     ) -> DataFrame:
         """
         Inner method where model actually predicts.
 
         :param log: historical log of interactions
-            ``[user_id, item_id, timestamp, relevance]``
-        :param k: length of recommendation lists, should be less that the total number of ``items``
+            ``[user_idx, item_idx, timestamp, relevance]``
+        :param k: number of recommendations for each user
         :param users: users to create recommendations for
-            dataframe containing ``[user_id]`` or ``array-like``;
+            dataframe containing ``[user_idx]`` or ``array-like``;
             if ``None``, recommend to all users from ``log``
         :param items: candidate items for recommendations
-            dataframe containing ``[item_id]`` or ``array-like``;
+            dataframe containing ``[item_idx]`` or ``array-like``;
             if ``None``, take all items from ``log``.
             If it contains new items, ``relevance`` for them will be ``0``.
         :param user_features: user features
-            ``[user_id , timestamp]`` + feature columns
+            ``[user_idx , timestamp]`` + feature columns
         :param item_features: item features
-            ``[item_id , timestamp]`` + feature columns
+            ``[item_idx , timestamp]`` + feature columns
         :param filter_seen_items: flag to remove seen items from recommendations based on ``log``.
         :return: recommendation dataframe
-            ``[user_id, item_id, relevance]``
+            ``[user_idx, item_idx, relevance]``
         """
 
     @property
     def logger(self) -> logging.Logger:
         """
         :returns: get library logger
         """
         if self._logger is None:
             self._logger = logging.getLogger("replay")
         return self._logger
 
+    def _get_fit_counts(self, entity: str) -> int:
+        if not hasattr(self, f"_num_{entity}s"):
+            setattr(
+                self,
+                f"_num_{entity}s",
+                getattr(self, f"fit_{entity}s").count(),
+            )
+        return getattr(self, f"_num_{entity}s")
+
     @property
     def users_count(self) -> int:
         """
         :returns: number of users the model was trained on
         """
-        try:
-            return len(self.user_indexer.labels)
-        except AttributeError as error:
-            raise AttributeError(
-                "Must run fit before calling this method"
-            ) from error
+        return self._get_fit_counts("user")
 
     @property
     def items_count(self) -> int:
         """
         :returns: number of items the model was trained on
         """
-        try:
-            return len(self.item_indexer.labels)
-        except AttributeError as error:
-            raise AttributeError(
-                "Must run fit before calling this method"
-            ) from error
+        return self._get_fit_counts("item")
+
+    def _get_fit_dims(self, entity: str) -> int:
+        if not hasattr(self, f"_{entity}_dim_size"):
+            setattr(
+                self,
+                f"_{entity}_dim_size",
+                getattr(self, f"fit_{entity}s")
+                .agg({f"{entity}_idx": "max"})
+                .collect()[0][0]
+                + 1,
+            )
+        return getattr(self, f"_{entity}_dim_size")
+
+    @property
+    def _user_dim(self) -> int:
+        """
+        :returns: dimension of users matrix (maximal user idx + 1)
+        """
+        return self._get_fit_dims("user")
+
+    @property
+    def _item_dim(self) -> int:
+        """
+        :returns: dimension of items matrix (maximal item idx + 1)
+        """
+        return self._get_fit_dims("item")
 
     def _fit_predict(
         self,
-        log: AnyDataFrame,
+        log: DataFrame,
         k: int,
-        users: Optional[Union[AnyDataFrame, Iterable]] = None,
-        items: Optional[Union[AnyDataFrame, Iterable]] = None,
-        user_features: Optional[AnyDataFrame] = None,
-        item_features: Optional[AnyDataFrame] = None,
+        users: Optional[Union[DataFrame, Iterable]] = None,
+        items: Optional[Union[DataFrame, Iterable]] = None,
+        user_features: Optional[DataFrame] = None,
+        item_features: Optional[DataFrame] = None,
         filter_seen_items: bool = True,
-        force_reindex: bool = True,
     ) -> DataFrame:
-        self._fit_wrap(log, user_features, item_features, force_reindex)
+        self._fit_wrap(log, user_features, item_features)
         return self._predict_wrap(
             log,
             k,
             users,
             items,
             user_features,
             item_features,
@@ -698,60 +631,55 @@
     def _clear_cache(self):
         """
         Clear spark cache
         """
 
     def _predict_pairs_wrap(
         self,
-        pairs: AnyDataFrame,
-        log: Optional[AnyDataFrame] = None,
-        user_features: Optional[AnyDataFrame] = None,
-        item_features: Optional[AnyDataFrame] = None,
+        pairs: DataFrame,
+        log: Optional[DataFrame] = None,
+        user_features: Optional[DataFrame] = None,
+        item_features: Optional[DataFrame] = None,
     ) -> DataFrame:
         """
         This method
         1) converts data to spark
         2) converts indexes
         3) calls inner _predict_pairs method of a model
         4) converts indexes back
 
         :param pairs: user-item pairs to get relevance for,
-            dataframe containing``[user_id, item_id]``.
+            dataframe containing``[user_idx, item_idx]``.
         :param log: train data
-            ``[user_id, item_id, timestamp, relevance]``.
+            ``[user_idx, item_idx, timestamp, relevance]``.
         :return: recommendations
-            ``[user_id, item_id, relevance]`` for given pairs
+            ``[user_idx, item_idx, relevance]`` for given pairs
         """
         log, user_features, item_features, pairs = [
             convert2spark(df)
             for df in [log, user_features, item_features, pairs]
         ]
-        if sorted(pairs.columns) != ["item_id", "user_id"]:
+        if sorted(pairs.columns) != ["item_idx", "user_idx"]:
             raise ValueError(
-                "pairs must be a dataframe with columns strictly [user_id, item_id]"
+                "pairs must be a dataframe with columns strictly [user_idx, item_idx]"
             )
 
-        users_type = pairs.schema["user_id"].dataType
-        items_type = pairs.schema["item_id"].dataType
-
-        log, user_features, item_features, pairs = [
-            self._convert_index(df)
-            for df in [log, user_features, item_features, pairs]
-        ]
+        if log is not None:
+            log = self._filter_ids(log, "user_idx")
+            log = self._filter_ids(log, "item_idx")
+        pairs = self._filter_ids(pairs, "item_idx")
+        pairs = self._filter_ids(pairs, "user_idx")
 
         pred = self._predict_pairs(
             pairs=pairs,
             log=log,
             user_features=user_features,
             item_features=item_features,
         )
 
-        pred = self._convert_back(pred, users_type, items_type).select(
-            "user_id", "item_id", "relevance"
-        )
         return pred
 
     def _predict_pairs(
         self,
         pairs: DataFrame,
         log: Optional[DataFrame] = None,
         user_features: Optional[DataFrame] = None,
@@ -792,29 +720,17 @@
             how="inner",
         )
         return pred
 
     def _get_features_wrap(
         self, ids: DataFrame, features: Optional[DataFrame]
     ) -> Optional[Tuple[DataFrame, int]]:
-        if "user_id" not in ids.columns and "item_id" not in ids.columns:
-            raise ValueError("user_id or item_id missing")
-
-        idx_col_name = "item_id" if "item_id" in ids.columns else "user_id"
-
-        ids_type = ids.schema[idx_col_name].dataType
-        ids, features = [self._convert_index(df) for df in [ids, features]]
-
+        if "user_idx" not in ids.columns and "item_idx" not in ids.columns:
+            raise ValueError("user_idx or item_idx missing")
         vectors, rank = self._get_features(ids, features)
-        vectors = self._convert_back(
-            log=vectors,
-            user_type=ids_type if idx_col_name == "user_id" else None,
-            item_type=ids_type if idx_col_name == "item_id" else None,
-        )
-
         return vectors, rank
 
     # pylint: disable=unused-argument
     def _get_features(
         self, ids: DataFrame, features: Optional[DataFrame]
     ) -> Tuple[Optional[DataFrame], Optional[int]]:
         """
@@ -822,15 +738,16 @@
 
         :param ids: id ids to get embeddings for Spark DataFrame containing user_idx or item_idx
         :param features: user or item features
         :return: DataFrame with biases and embeddings, and vector size
         """
 
         self.logger.info(
-            "Метод реализован только для моделей ALS и LightFMWrap. Признаки не будут возвращены"
+            "get_features method is not defined for the model %s. Features will not be returned.",
+            self.__str__(),
         )
         return None, None
 
     def get_nearest_items(
         self,
         items: Union[DataFrame, Iterable],
         k: int,
@@ -844,25 +761,28 @@
         :param k: number of neighbors
         :param metric: 'euclidean_distance_sim', 'cosine_similarity', 'dot_product'
         :param candidates: spark dataframe or list of items
             to consider as similar, e.g. popular/new items. If None,
             all items presented during model training are used.
         :return: dataframe with the most similar items an distance,
             where bigger value means greater similarity.
-            spark-dataframe with columns ``[item_id, neighbour_item_id, similarity]``
+            spark-dataframe with columns ``[item_idx, neighbour_item_idx, similarity]``
         """
         if metric is None:
             raise ValueError(
                 f"Distance metric is required to get nearest items with "
                 f"{self.__str__()} model"
             )
 
         if self.can_predict_item_to_item:
             return self._get_nearest_items_wrap(
-                items=items, k=k, metric=metric, candidates=candidates,
+                items=items,
+                k=k,
+                metric=metric,
+                candidates=candidates,
             )
 
         raise ValueError(
             "Use models with attribute 'can_predict_item_to_item' set to True to get nearest items"
         )
 
     def _get_nearest_items_wrap(
@@ -871,49 +791,40 @@
         k: int,
         metric: Optional[str] = "cosine_similarity",
         candidates: Optional[Union[DataFrame, Iterable]] = None,
     ) -> Optional[DataFrame]:
         """
         Convert indexes and leave top-k nearest items for each item in `items`.
         """
-        items = self._get_ids(items, "item_id")
+        items = self._get_ids(items, "item_idx")
         if candidates is not None:
-            candidates = self._get_ids(candidates, "item_id")
-
-        items_type = items.schema["item_id"].dataType
-
-        items, candidates = [
-            self._convert_index(df) for df in [items, candidates]
-        ]
+            candidates = self._get_ids(candidates, "item_idx")
 
         nearest_items_to_filter = self._get_nearest_items(
-            items=items, metric=metric, candidates=candidates,
+            items=items,
+            metric=metric,
+            candidates=candidates,
         )
 
         rel_col_name = metric if metric is not None else "similarity"
         nearest_items = get_top_k(
             dataframe=nearest_items_to_filter,
-            partition_by_col=sf.col("item_id_one"),
+            partition_by_col=sf.col("item_idx_one"),
             order_by_col=[
                 sf.col(rel_col_name).desc(),
-                sf.col("item_id_two").desc(),
+                sf.col("item_idx_two").desc(),
             ],
             k=k,
         )
 
-        nearest_items = self._convert_back(
-            nearest_items.withColumnRenamed("item_id_two", "item_idx"),
-            None,
-            items_type,
-        ).withColumnRenamed("item_id", "neighbour_item_id")
-
-        nearest_items = self._convert_back(
-            nearest_items.withColumnRenamed("item_id_one", "item_idx"),
-            None,
-            items_type,
+        nearest_items = nearest_items.withColumnRenamed(
+            "item_idx_two", "neighbour_item_idx"
+        )
+        nearest_items = nearest_items.withColumnRenamed(
+            "item_idx_one", "item_idx"
         )
         return nearest_items
 
     def _get_nearest_items(
         self,
         items: DataFrame,
         metric: Optional[str] = None,
@@ -963,202 +874,196 @@
 
         :param items: ids to find neighbours, spark dataframe with column ``item_idx``
         :param metric: 'euclidean_distance_sim' calculated as 1/(1 + euclidean_distance),
             'cosine_similarity', 'dot_product'
         :param candidates: items among which we are looking for similar,
             e.g. popular/new items. If None, all items presented during model training are used.
         :return: dataframe with neighbours,
-            spark-dataframe with columns ``[item_id_one, item_id_two, similarity]``
+            spark-dataframe with columns ``[item_idx_one, item_idx_two, similarity]``
         """
         dist_function = cosine_similarity
         if metric == "euclidean_distance_sim":
             dist_function = vector_euclidean_distance_similarity
         elif metric == "dot_product":
             dist_function = vector_dot
         elif metric != "cosine_similarity":
             raise NotImplementedError(
                 f"{metric} metric is not implemented, valid metrics are "
                 "'euclidean_distance_sim', 'cosine_similarity', 'dot_product'"
             )
 
         items_vectors = self._get_item_vectors()
         left_part = (
-            items_vectors.withColumnRenamed("item_idx", "item_id_one")
+            items_vectors.withColumnRenamed("item_idx", "item_idx_one")
             .withColumnRenamed("item_vector", "item_vector_one")
             .join(
-                items.select(sf.col("item_idx").alias("item_id_one")),
-                on="item_id_one",
+                items.select(sf.col("item_idx").alias("item_idx_one")),
+                on="item_idx_one",
             )
         )
 
         right_part = items_vectors.withColumnRenamed(
-            "item_idx", "item_id_two"
+            "item_idx", "item_idx_two"
         ).withColumnRenamed("item_vector", "item_vector_two")
 
         if candidates is not None:
             right_part = right_part.join(
-                candidates.withColumnRenamed("item_idx", "item_id_two"),
-                on="item_id_two",
+                candidates.withColumnRenamed("item_idx", "item_idx_two"),
+                on="item_idx_two",
             )
 
         joined_factors = left_part.join(
-            right_part, on=sf.col("item_id_one") != sf.col("item_id_two")
+            right_part, on=sf.col("item_idx_one") != sf.col("item_idx_two")
         )
 
         joined_factors = joined_factors.withColumn(
             metric,
             dist_function(
                 sf.col("item_vector_one"), sf.col("item_vector_two")
             ),
         )
 
         similarity_matrix = joined_factors.select(
-            "item_id_one", "item_id_two", metric
+            "item_idx_one", "item_idx_two", metric
         )
 
         return similarity_matrix
 
 
 # pylint: disable=abstract-method
 class HybridRecommender(BaseRecommender, ABC):
     """Base class for models that can use extra features"""
 
     def fit(
         self,
-        log: AnyDataFrame,
-        user_features: Optional[AnyDataFrame] = None,
-        item_features: Optional[AnyDataFrame] = None,
-        force_reindex: bool = True,
+        log: DataFrame,
+        user_features: Optional[DataFrame] = None,
+        item_features: Optional[DataFrame] = None,
     ) -> None:
         """
         Fit a recommendation model
 
         :param log: historical log of interactions
-            ``[user_id, item_id, timestamp, relevance]``
+            ``[user_idx, item_idx, timestamp, relevance]``
         :param user_features: user features
-            ``[user_id, timestamp]`` + feature columns
+            ``[user_idx, timestamp]`` + feature columns
         :param item_features: item features
-            ``[item_id, timestamp]`` + feature columns
-        :param force_reindex: create indexers again, even if they were created previously
+            ``[item_idx, timestamp]`` + feature columns
         :return:
         """
         self._fit_wrap(
             log=log,
             user_features=user_features,
             item_features=item_features,
-            force_reindex=force_reindex,
         )
 
     # pylint: disable=too-many-arguments
     def predict(
         self,
-        log: AnyDataFrame,
+        log: DataFrame,
         k: int,
-        users: Optional[Union[AnyDataFrame, Iterable]] = None,
-        items: Optional[Union[AnyDataFrame, Iterable]] = None,
-        user_features: Optional[AnyDataFrame] = None,
-        item_features: Optional[AnyDataFrame] = None,
+        users: Optional[Union[DataFrame, Iterable]] = None,
+        items: Optional[Union[DataFrame, Iterable]] = None,
+        user_features: Optional[DataFrame] = None,
+        item_features: Optional[DataFrame] = None,
         filter_seen_items: bool = True,
     ) -> DataFrame:
         """
         Get recommendations
 
         :param log: historical log of interactions
-            ``[user_id, item_id, timestamp, relevance]``
-        :param k: length of recommendation lists, should be less that the total number of ``items``
+            ``[user_idx, item_idx, timestamp, relevance]``
+        :param k: number of recommendations for each user
         :param users: users to create recommendations for
-            dataframe containing ``[user_id]`` or ``array-like``;
+            dataframe containing ``[user_idx]`` or ``array-like``;
             if ``None``, recommend to all users from ``log``
         :param items: candidate items for recommendations
-            dataframe containing ``[item_id]`` or ``array-like``;
+            dataframe containing ``[item_idx]`` or ``array-like``;
             if ``None``, take all items from ``log``.
             If it contains new items, ``relevance`` for them will be ``0``.
         :param user_features: user features
-            ``[user_id , timestamp]`` + feature columns
+            ``[user_idx , timestamp]`` + feature columns
         :param item_features: item features
-            ``[item_id , timestamp]`` + feature columns
+            ``[item_idx , timestamp]`` + feature columns
         :param filter_seen_items: flag to remove seen items from recommendations based on ``log``.
         :return: recommendation dataframe
-            ``[user_id, item_id, relevance]``
+            ``[user_idx, item_idx, relevance]``
         """
         return self._predict_wrap(
             log=log,
             k=k,
             users=users,
             items=items,
             user_features=user_features,
             item_features=item_features,
             filter_seen_items=filter_seen_items,
         )
 
     def fit_predict(
         self,
-        log: AnyDataFrame,
+        log: DataFrame,
         k: int,
-        users: Optional[Union[AnyDataFrame, Iterable]] = None,
-        items: Optional[Union[AnyDataFrame, Iterable]] = None,
-        user_features: Optional[AnyDataFrame] = None,
-        item_features: Optional[AnyDataFrame] = None,
+        users: Optional[Union[DataFrame, Iterable]] = None,
+        items: Optional[Union[DataFrame, Iterable]] = None,
+        user_features: Optional[DataFrame] = None,
+        item_features: Optional[DataFrame] = None,
         filter_seen_items: bool = True,
-        force_reindex: bool = True,
     ) -> DataFrame:
         """
         Fit model and get recommendations
 
         :param log: historical log of interactions
-            ``[user_id, item_id, timestamp, relevance]``
-        :param k: length of recommendation lists, should be less that the total number of ``items``
+            ``[user_idx, item_idx, timestamp, relevance]``
+        :param k: number of recommendations for each user
         :param users: users to create recommendations for
-            dataframe containing ``[user_id]`` or ``array-like``;
+            dataframe containing ``[user_idx]`` or ``array-like``;
             if ``None``, recommend to all users from ``log``
         :param items: candidate items for recommendations
-            dataframe containing ``[item_id]`` or ``array-like``;
+            dataframe containing ``[item_idx]`` or ``array-like``;
             if ``None``, take all items from ``log``.
             If it contains new items, ``relevance`` for them will be ``0``.
         :param user_features: user features
-            ``[user_id , timestamp]`` + feature columns
+            ``[user_idx , timestamp]`` + feature columns
         :param item_features: item features
-            ``[item_id , timestamp]`` + feature columns
+            ``[item_idx , timestamp]`` + feature columns
         :param filter_seen_items: flag to remove seen items from recommendations based on ``log``.
-        :param force_reindex: replace existing user and item indexers
         :return: recommendation dataframe
-            ``[user_id, item_id, relevance]``
+            ``[user_idx, item_idx, relevance]``
         """
         return self._fit_predict(
             log=log,
             k=k,
             users=users,
             items=items,
             user_features=user_features,
             item_features=item_features,
             filter_seen_items=filter_seen_items,
-            force_reindex=force_reindex,
         )
 
     def predict_pairs(
         self,
-        pairs: AnyDataFrame,
-        log: Optional[AnyDataFrame] = None,
-        user_features: Optional[AnyDataFrame] = None,
-        item_features: Optional[AnyDataFrame] = None,
+        pairs: DataFrame,
+        log: Optional[DataFrame] = None,
+        user_features: Optional[DataFrame] = None,
+        item_features: Optional[DataFrame] = None,
     ) -> DataFrame:
         """
         Get recommendations for specific user-item ``pairs``.
         If a model can't produce recommendation
         for specific pair it is removed from the resulting dataframe.
 
-        :param pairs: dataframe with pairs to calculate relevance for, ``[user_id, item_id]``.
+        :param pairs: dataframe with pairs to calculate relevance for, ``[user_idx, item_idx]``.
         :param log: historical log of interactions
-            ``[user_id, item_id, timestamp, relevance]``
+            ``[user_idx, item_idx, timestamp, relevance]``
         :param user_features: user features
-            ``[user_id , timestamp]`` + feature columns
+            ``[user_idx , timestamp]`` + feature columns
         :param item_features: item features
-            ``[item_id , timestamp]`` + feature columns
+            ``[item_idx , timestamp]`` + feature columns
         :return: recommendation dataframe
-            ``[user_id, item_id, relevance]``
+            ``[user_idx, item_idx, relevance]``
         """
         return self._predict_pairs_wrap(
             pairs, log, user_features, item_features
         )
 
     def get_features(
         self, ids: DataFrame, features: Optional[DataFrame]
@@ -1173,119 +1078,114 @@
         return self._get_features_wrap(ids, features)
 
 
 # pylint: disable=abstract-method
 class Recommender(BaseRecommender, ABC):
     """Usual recommender class for models without features."""
 
-    def fit(self, log: AnyDataFrame, force_reindex: bool = True) -> None:
+    def fit(self, log: DataFrame) -> None:
         """
         Fit a recommendation model
 
         :param log: historical log of interactions
-            ``[user_id, item_id, timestamp, relevance]``
-        :param force_reindex: create indexers again, even if they were created previously
+            ``[user_idx, item_idx, timestamp, relevance]``
         :return:
         """
         self._fit_wrap(
             log=log,
             user_features=None,
             item_features=None,
-            force_reindex=force_reindex,
         )
 
     # pylint: disable=too-many-arguments
     def predict(
         self,
-        log: AnyDataFrame,
+        log: DataFrame,
         k: int,
-        users: Optional[Union[AnyDataFrame, Iterable]] = None,
-        items: Optional[Union[AnyDataFrame, Iterable]] = None,
+        users: Optional[Union[DataFrame, Iterable]] = None,
+        items: Optional[Union[DataFrame, Iterable]] = None,
         filter_seen_items: bool = True,
     ) -> DataFrame:
         """
         Get recommendations
 
         :param log: historical log of interactions
-            ``[user_id, item_id, timestamp, relevance]``
-        :param k: length of recommendation lists, should be less that the total number of ``items``
+            ``[user_idx, item_idx, timestamp, relevance]``
+        :param k: number of recommendations for each user
         :param users: users to create recommendations for
-            dataframe containing ``[user_id]`` or ``array-like``;
+            dataframe containing ``[user_idx]`` or ``array-like``;
             if ``None``, recommend to all users from ``log``
         :param items: candidate items for recommendations
-            dataframe containing ``[item_id]`` or ``array-like``;
+            dataframe containing ``[item_idx]`` or ``array-like``;
             if ``None``, take all items from ``log``.
             If it contains new items, ``relevance`` for them will be ``0``.
         :param filter_seen_items: flag to remove seen items from recommendations based on ``log``.
         :return: recommendation dataframe
-            ``[user_id, item_id, relevance]``
+            ``[user_idx, item_idx, relevance]``
         """
         return self._predict_wrap(
             log=log,
             k=k,
             users=users,
             items=items,
             user_features=None,
             item_features=None,
             filter_seen_items=filter_seen_items,
         )
 
     def predict_pairs(
-        self, pairs: AnyDataFrame, log: Optional[AnyDataFrame] = None
+        self, pairs: DataFrame, log: Optional[DataFrame] = None
     ) -> DataFrame:
         """
         Get recommendations for specific user-item ``pairs``.
         If a model can't produce recommendation
         for specific pair it is removed from the resulting dataframe.
 
-        :param pairs: dataframe with pairs to calculate relevance for, ``[user_id, item_id]``.
+        :param pairs: dataframe with pairs to calculate relevance for, ``[user_idx, item_idx]``.
         :param log: historical log of interactions
-            ``[user_id, item_id, timestamp, relevance]``
+            ``[user_idx, item_idx, timestamp, relevance]``
         :return: recommendation dataframe
-            ``[user_id, item_id, relevance]``
+            ``[user_idx, item_idx, relevance]``
         """
         return self._predict_pairs_wrap(pairs, log, None, None)
 
     # pylint: disable=too-many-arguments
     def fit_predict(
         self,
-        log: AnyDataFrame,
+        log: DataFrame,
         k: int,
-        users: Optional[Union[AnyDataFrame, Iterable]] = None,
-        items: Optional[Union[AnyDataFrame, Iterable]] = None,
+        users: Optional[Union[DataFrame, Iterable]] = None,
+        items: Optional[Union[DataFrame, Iterable]] = None,
         filter_seen_items: bool = True,
-        force_reindex: bool = True,
     ) -> DataFrame:
         """
         Fit model and get recommendations
 
         :param log: historical log of interactions
-            ``[user_id, item_id, timestamp, relevance]``
-        :param k: length of recommendation lists, should be less that the total number of ``items``
+            ``[user_idx, item_idx, timestamp, relevance]``
+        :param k: number of recommendations for each user
         :param users: users to create recommendations for
-            dataframe containing ``[user_id]`` or ``array-like``;
+            dataframe containing ``[user_idx]`` or ``array-like``;
             if ``None``, recommend to all users from ``log``
         :param items: candidate items for recommendations
-            dataframe containing ``[item_id]`` or ``array-like``;
+            dataframe containing ``[item_idx]`` or ``array-like``;
             if ``None``, take all items from ``log``.
             If it contains new items, ``relevance`` for them will be ``0``.
         :param filter_seen_items: flag to remove seen items from recommendations based on ``log``.
-        :param force_reindex: replace existing user and item indexers
         :return: recommendation dataframe
-            ``[user_id, item_id, relevance]``
+            ``[user_idx, item_idx, relevance]``
         """
         return self._fit_predict(
             log=log,
             k=k,
             users=users,
             items=items,
             user_features=None,
             item_features=None,
             filter_seen_items=filter_seen_items,
-            force_reindex=force_reindex,
         )
 
     def get_features(self, ids: DataFrame) -> Optional[Tuple[DataFrame, int]]:
         """
         Returns user or item feature vectors as a Column with type ArrayType
 
         :param ids: Spark DataFrame with unique ids
@@ -1297,88 +1197,84 @@
 
 class UserRecommender(BaseRecommender, ABC):
     """Base class for models that use user features
     but not item features. ``log`` is not required for this class."""
 
     def fit(
         self,
-        log: AnyDataFrame,
-        user_features: AnyDataFrame,
-        force_reindex: bool = True,
+        log: DataFrame,
+        user_features: DataFrame,
     ) -> None:
         """
         Finds user clusters and calculates item similarity in that clusters.
 
         :param log: historical log of interactions
-            ``[user_id, item_id, timestamp, relevance]``
+            ``[user_idx, item_idx, timestamp, relevance]``
         :param user_features: user features
-            ``[user_id, timestamp]`` + feature columns
-        :param force_reindex: create indexers again, even if they were created previously
+            ``[user_idx, timestamp]`` + feature columns
         :return:
         """
-        self._fit_wrap(
-            log=log, user_features=user_features, force_reindex=force_reindex
-        )
+        self._fit_wrap(log=log, user_features=user_features)
 
     # pylint: disable=too-many-arguments
     def predict(
         self,
-        user_features: AnyDataFrame,
+        user_features: DataFrame,
         k: int,
-        log: Optional[AnyDataFrame] = None,
-        users: Optional[Union[AnyDataFrame, Iterable]] = None,
-        items: Optional[Union[AnyDataFrame, Iterable]] = None,
+        log: Optional[DataFrame] = None,
+        users: Optional[Union[DataFrame, Iterable]] = None,
+        items: Optional[Union[DataFrame, Iterable]] = None,
         filter_seen_items: bool = True,
     ) -> DataFrame:
         """
         Get recommendations
 
         :param log: historical log of interactions
-            ``[user_id, item_id, timestamp, relevance]``
-        :param k: length of recommendation lists, should be less that the total number of ``items``
+            ``[user_idx, item_idx, timestamp, relevance]``
+        :param k: number of recommendations for each user
         :param users: users to create recommendations for
-            dataframe containing ``[user_id]`` or ``array-like``;
+            dataframe containing ``[user_idx]`` or ``array-like``;
             if ``None``, recommend to all users from ``log``
         :param items: candidate items for recommendations
-            dataframe containing ``[item_id]`` or ``array-like``;
+            dataframe containing ``[item_idx]`` or ``array-like``;
             if ``None``, take all items from ``log``.
             If it contains new items, ``relevance`` for them will be ``0``.
         :param user_features: user features
-            ``[user_id , timestamp]`` + feature columns
+            ``[user_idx , timestamp]`` + feature columns
         :param filter_seen_items: flag to remove seen items from recommendations based on ``log``.
         :return: recommendation dataframe
-            ``[user_id, item_id, relevance]``
+            ``[user_idx, item_idx, relevance]``
         """
         return self._predict_wrap(
             log=log,
             user_features=user_features,
             k=k,
             filter_seen_items=filter_seen_items,
             users=users,
             items=items,
         )
 
     def predict_pairs(
         self,
-        pairs: AnyDataFrame,
-        log: Optional[AnyDataFrame] = None,
-        user_features: Optional[AnyDataFrame] = None,
+        pairs: DataFrame,
+        log: Optional[DataFrame] = None,
+        user_features: Optional[DataFrame] = None,
     ) -> DataFrame:
         """
         Get recommendations for specific user-item ``pairs``.
         If a model can't produce recommendation
         for specific pair it is removed from the resulting dataframe.
 
-        :param pairs: dataframe with pairs to calculate relevance for, ``[user_id, item_id]``.
+        :param pairs: dataframe with pairs to calculate relevance for, ``[user_idx, item_idx]``.
         :param log: historical log of interactions
-            ``[user_id, item_id, timestamp, relevance]``
+            ``[user_idx, item_idx, timestamp, relevance]``
         :param user_features: user features
-            ``[user_id , timestamp]`` + feature columns
+            ``[user_idx , timestamp]`` + feature columns
         :return: recommendation dataframe
-            ``[user_id, item_id, relevance]``
+            ``[user_idx, item_idx, relevance]``
         """
         return self._predict_pairs_wrap(pairs, log, user_features, None)
 
 
 class NeighbourRec(Recommender, ABC):
     """Base class that requires log at prediction time"""
 
@@ -1420,20 +1316,24 @@
             )
 
         recs = (
             log.join(users, how="inner", on="user_idx")
             .join(
                 self.similarity,
                 how="inner",
-                on=sf.col("item_idx") == sf.col("item_id_one"),
+                on=sf.col("item_idx") == sf.col("item_idx_one"),
+            )
+            .join(
+                filter_df,
+                how="inner",
+                on=condition,
             )
-            .join(filter_df, how="inner", on=condition,)
-            .groupby("user_idx", "item_id_two")
+            .groupby("user_idx", "item_idx_two")
             .agg(sf.sum("similarity").alias("relevance"))
-            .withColumnRenamed("item_id_two", "item_idx")
+            .withColumnRenamed("item_idx_two", "item_idx")
         )
         return recs
 
     # pylint: disable=too-many-arguments
     def _predict(
         self,
         log: DataFrame,
@@ -1443,15 +1343,15 @@
         user_features: Optional[DataFrame] = None,
         item_features: Optional[DataFrame] = None,
         filter_seen_items: bool = True,
     ) -> DataFrame:
         return self._predict_pairs_inner(
             log=log,
             filter_df=items.withColumnRenamed("item_idx", "item_idx_filter"),
-            condition=sf.col("item_id_two") == sf.col("item_idx_filter"),
+            condition=sf.col("item_idx_two") == sf.col("item_idx_filter"),
             users=users,
         )
 
     def _predict_pairs(
         self,
         pairs: DataFrame,
         log: Optional[DataFrame] = None,
@@ -1462,15 +1362,15 @@
             log=log,
             filter_df=(
                 pairs.withColumnRenamed(
                     "user_idx", "user_idx_filter"
                 ).withColumnRenamed("item_idx", "item_idx_filter")
             ),
             condition=(sf.col("user_idx") == sf.col("user_idx_filter"))
-            & (sf.col("item_id_two") == sf.col("item_idx_filter")),
+            & (sf.col("item_idx_two") == sf.col("item_idx_filter")),
             users=pairs.select("user_idx").distinct(),
         )
 
     def get_nearest_items(
         self,
         items: Union[DataFrame, Iterable],
         k: int,
@@ -1485,40 +1385,43 @@
         :param metric: metric is not used to find neighbours in NeighbourRec,
             the parameter is ignored
         :param candidates: spark dataframe or list of items
             to consider as similar, e.g. popular/new items. If None,
             all items presented during model training are used.
         :return: dataframe with the most similar items an distance,
             where bigger value means greater similarity.
-            spark-dataframe with columns ``[item_id, neighbour_item_id, similarity]``
+            spark-dataframe with columns ``[item_idx, neighbour_item_idx, similarity]``
         """
         if metric is not None:
             self.logger.debug(
                 "Metric is not used to determine nearest items in %s model",
                 self.__str__(),
             )
 
         return self._get_nearest_items_wrap(
-            items=items, k=k, metric=None, candidates=candidates,
+            items=items,
+            k=k,
+            metric=None,
+            candidates=candidates,
         )
 
     def _get_nearest_items(
         self,
         items: DataFrame,
         metric: Optional[str] = None,
         candidates: Optional[DataFrame] = None,
     ) -> DataFrame:
 
         similarity_filtered = self.similarity.join(
-            items.withColumnRenamed("item_idx", "item_id_one"),
-            on="item_id_one",
+            items.withColumnRenamed("item_idx", "item_idx_one"),
+            on="item_idx_one",
         )
 
         if candidates is not None:
             similarity_filtered = similarity_filtered.join(
-                candidates.withColumnRenamed("item_idx", "item_id_two"),
-                on="item_id_two",
+                candidates.withColumnRenamed("item_idx", "item_idx_two"),
+                on="item_idx_two",
             )
 
         return similarity_filtered.select(
-            "item_id_one", "item_id_two", "similarity"
+            "item_idx_one", "item_idx_two", "similarity"
         )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `replay-rec-0.8.0/replay/models/cluster.py` & `replay-rec-0.9.0/replay/models/cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,15 +88,17 @@
         users: DataFrame,
         items: DataFrame,
         user_features: Optional[DataFrame] = None,
         item_features: Optional[DataFrame] = None,
         filter_seen_items: bool = True,
     ) -> DataFrame:
 
-        user_features_vector = self._transform_features(user_features)
+        user_features_vector = self._transform_features(
+            user_features.join(users, on="user_idx")
+        )
         user_clusters = (
             self.model.transform(user_features_vector)
             .select("user_idx", "prediction")
             .withColumnRenamed("prediction", "cluster")
         )
         filtered_items = self.item_rel_in_cluster.join(items, on="item_idx")
         pred = user_clusters.join(filtered_items, on="cluster").drop("cluster")
```

### Comparing `replay-rec-0.8.0/replay/models/implicit_wrap.py` & `replay-rec-0.9.0/replay/models/implicit_wrap.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import joblib
 import pandas as pd
 from pyspark.sql import DataFrame
 
 from replay.models.base_rec import Recommender
 from replay.utils import to_csr
-from replay.constants import IDX_REC_SCHEMA
+from replay.constants import REC_SCHEMA
 
 
 class ImplicitWrap(Recommender):
     """Wrapper for `implicit
     <https://github.com/benfred/implicit>`_
 
     Example:
@@ -19,18 +19,20 @@
     >>> model = implicit.als.AlternatingLeastSquares(factors=5)
     >>> als = ImplicitWrap(model)
 
     This way you can use implicit models as any other in replay
     with conversions made under the hood.
 
     >>> import pandas as pd
-    >>> df = pd.DataFrame({"user_id": [1, 1, 2, 2], "item_id": [1, 2, 2, 3], "relevance": [1, 1, 1, 1]})
-    >>> als.fit_predict(df, 1, users=[1])[["user_id", "item_id"]].toPandas()
-       user_id  item_id
-    0        1        3
+    >>> from replay.utils import convert2spark
+    >>> df = pd.DataFrame({"user_idx": [1, 1, 2, 2], "item_idx": [1, 2, 2, 3], "relevance": [1, 1, 1, 1]})
+    >>> df = convert2spark(df)
+    >>> als.fit_predict(df, 1, users=[1])[["user_idx", "item_idx"]].toPandas()
+       user_idx  item_idx
+    0         1         3
     """
 
     def __init__(self, model):
         """Provide initialized ``implicit`` model."""
         self.model = model
         self.logger.info(
             "The model is a wrapper of a non-distributed model which may affect performance"
@@ -87,9 +89,9 @@
             .item_idx.to_list()
         )
         user_item_data = to_csr(log).tocsr()
         model = self.model
         return (
             users.select("user_idx")
             .groupby("user_idx")
-            .applyInPandas(predict_by_user, IDX_REC_SCHEMA)
+            .applyInPandas(predict_by_user, REC_SCHEMA)
         )
```

### Comparing `replay-rec-0.8.0/replay/models/knn.py` & `replay-rec-0.9.0/replay/models/knn.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from typing import Optional
 
 from pyspark.sql import DataFrame
 from pyspark.sql import functions as sf
 from pyspark.sql.window import Window
 
 from replay.models.base_rec import NeighbourRec
+from replay.optuna_objective import KNNObjective
 
 
 class KNN(NeighbourRec):
     """Item-based KNN with modified cosine similarity measure."""
 
     all_items: Optional[DataFrame]
     dot_products: Optional[DataFrame]
     item_norms: Optional[DataFrame]
+    _objective = KNNObjective
     _search_space = {
         "num_neighbours": {"type": "int", "args": [1, 100]},
         "shrink": {"type": "int", "args": [0, 100]},
     }
 
     def __init__(
         self,
@@ -37,33 +39,53 @@
     def _init_args(self):
         return {
             "shrink": self.shrink,
             "use_relevance": self.use_relevance,
             "num_neighbours": self.num_neighbours,
         }
 
+    @staticmethod
+    def _shrink(dot_products: DataFrame, shrink: float) -> DataFrame:
+        return dot_products.withColumn(
+            "similarity",
+            sf.col("dot_product")
+            / (sf.col("norm1") * sf.col("norm2") + shrink),
+        ).select("item_idx_one", "item_idx_two", "similarity")
+
     def _get_similarity(self, log: DataFrame) -> DataFrame:
         """
         Calculate item similarities
 
         :param log: DataFrame with interactions, `[user_idx, item_idx, relevance]`
-        :return: similarity matrix `[item_id_one, item_id_two, similarity]`
+        :return: similarity matrix `[item_idx_one, item_idx_two, similarity]`
+        """
+        dot_products = self._get_products(log)
+        similarity = self._shrink(dot_products, self.shrink)
+        return similarity
+
+    @staticmethod
+    def _get_products(log: DataFrame) -> DataFrame:
+        """
+        Calculate item dot products
+
+        :param log: DataFrame with interactions, `[user_idx, item_idx, relevance]`
+        :return: similarity matrix `[item_idx_one, item_idx_two, norm1, norm2]`
         """
         left = log.withColumnRenamed(
-            "item_idx", "item_id_one"
+            "item_idx", "item_idx_one"
         ).withColumnRenamed("relevance", "rel_one")
         right = log.withColumnRenamed(
-            "item_idx", "item_id_two"
+            "item_idx", "item_idx_two"
         ).withColumnRenamed("relevance", "rel_two")
 
         dot_products = (
             left.join(right, how="inner", on="user_idx")
-            .filter(sf.col("item_id_one") != sf.col("item_id_two"))
+            .filter(sf.col("item_idx_one") != sf.col("item_idx_two"))
             .withColumn("relevance", sf.col("rel_one") * sf.col("rel_two"))
-            .groupBy("item_id_one", "item_id_two")
+            .groupBy("item_idx_one", "item_idx_two")
             .agg(sf.sum("relevance").alias("dot_product"))
         )
 
         item_norms = (
             log.withColumn("relevance", sf.col("relevance") ** 2)
             .groupBy("item_idx")
             .agg(sf.sum("relevance").alias("square_norm"))
@@ -74,41 +96,36 @@
             "item_idx", "item_id1"
         ).withColumnRenamed("norm", "norm1")
         norm2 = item_norms.withColumnRenamed(
             "item_idx", "item_id2"
         ).withColumnRenamed("norm", "norm2")
 
         dot_products = dot_products.join(
-            norm1, how="inner", on=sf.col("item_id1") == sf.col("item_id_one")
+            norm1, how="inner", on=sf.col("item_id1") == sf.col("item_idx_one")
         )
         dot_products = dot_products.join(
-            norm2, how="inner", on=sf.col("item_id2") == sf.col("item_id_two")
+            norm2, how="inner", on=sf.col("item_id2") == sf.col("item_idx_two")
         )
 
-        dot_products = dot_products.withColumn(
-            "similarity",
-            sf.col("dot_product")
-            / (sf.col("norm1") * sf.col("norm2") + self.shrink),
-        ).select("item_id_one", "item_id_two", "similarity")
         return dot_products
 
     def _get_k_most_similar(self, similarity_matrix: DataFrame) -> DataFrame:
         """
         Leaves only top-k neighbours for each item
 
-        :param similarity_matrix: dataframe `[item_id_one, item_id_two, similarity]`
+        :param similarity_matrix: dataframe `[item_idx_one, item_idx_two, similarity]`
         :return: cropped similarity matrix
         """
         return (
             similarity_matrix.withColumn(
                 "similarity_order",
                 sf.row_number().over(
-                    Window.partitionBy("item_id_one").orderBy(
+                    Window.partitionBy("item_idx_one").orderBy(
                         sf.col("similarity").desc(),
-                        sf.col("item_id_two").desc(),
+                        sf.col("item_idx_two").desc(),
                     )
                 ),
             )
             .filter(sf.col("similarity_order") <= self.num_neighbours)
             .drop("similarity_order")
         )
```

### Comparing `replay-rec-0.8.0/replay/models/lightfm_wrap.py` & `replay-rec-0.9.0/replay/models/lightfm_wrap.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import pyspark.sql.functions as sf
 
 from lightfm import LightFM
 from pyspark.sql import DataFrame
 from scipy.sparse import csr_matrix, hstack, diags
 from sklearn.preprocessing import MinMaxScaler
 
-from replay.constants import IDX_REC_SCHEMA
+from replay.constants import REC_SCHEMA
 from replay.models.base_rec import HybridRecommender
 from replay.utils import to_csr, check_numeric
 from replay.session_handler import State
 
 
 # pylint: disable=too-many-locals, too-many-instance-attributes
 class LightFMWrap(HybridRecommender):
@@ -28,41 +28,34 @@
             "type": "categorical",
             "args": ["logistic", "bpr", "warp", "warp-kos"],
         },
         "no_components": {"type": "loguniform_int", "args": [8, 512]},
     }
     user_feat_scaler: Optional[MinMaxScaler] = None
     item_feat_scaler: Optional[MinMaxScaler] = None
-    num_of_warm_users: int
-    num_of_warm_items: int
 
     def __init__(
         self,
         no_components: int = 128,
         loss: str = "warp",
         random_state: Optional[int] = None,
     ):  # pylint: disable=too-many-arguments
         np.random.seed(42)
         self.no_components = no_components
         self.loss = loss
         self.random_state = random_state
         cpu_count = os.cpu_count()
         self.num_threads = cpu_count if cpu_count is not None else 1
-        # number of columns in identity matrix used for building feature matrix
-        self.num_of_warm_items = None
-        self.num_of_warm_users = None
 
     @property
     def _init_args(self):
         return {
             "no_components": self.no_components,
             "loss": self.loss,
             "random_state": self.random_state,
-            "num_of_warm_items": self.num_of_warm_items,
-            "num_of_warm_users": self.num_of_warm_users,
         }
 
     def _save_model(self, path: str):
         os.makedirs(path)
         joblib.dump(self.model, join(path, "model"))
         joblib.dump(self.user_feat_scaler, join(path, "user_feat_scaler"))
         joblib.dump(self.item_feat_scaler, join(path, "item_feat_scaler"))
@@ -102,17 +95,17 @@
         idx_col_name = f"{entity}_idx"
 
         # filter features by log
         feature_table = feature_table.join(
             log_ids_list, on=idx_col_name, how="inner"
         )
 
-        num_entities_in_fit = getattr(self, f"num_of_warm_{entity}s")
+        fit_dim = getattr(self, f"_{entity}_dim")
         matrix_height = max(
-            num_entities_in_fit,
+            fit_dim,
             log_ids_list.select(sf.max(idx_col_name)).collect()[0][0] + 1,
         )
         if not feature_table.rdd.isEmpty():
             matrix_height = max(
                 matrix_height,
                 feature_table.select(sf.max(idx_col_name)).collect()[0][0] + 1,
             )
@@ -135,22 +128,22 @@
             .to_numpy()
         )
         entities_ids = features_np[:, 0]
         features_np = features_np[:, 1:]
         number_of_features = features_np.shape[1]
 
         all_ids_list = log_ids_list.toPandas().to_numpy().ravel()
-        entities_seen_in_fit = all_ids_list[all_ids_list < num_entities_in_fit]
+        entities_seen_in_fit = all_ids_list[all_ids_list < fit_dim]
 
         entity_id_features = csr_matrix(
             (
                 [1.0] * entities_seen_in_fit.shape[0],
                 (entities_seen_in_fit, entities_seen_in_fit),
             ),
-            shape=(matrix_height, num_entities_in_fit),
+            shape=(matrix_height, fit_dim),
         )
 
         scaler_name = f"{entity}_feat_scaler"
         if getattr(self, scaler_name) is None:
             if not features_np.size:
                 raise ValueError(f"features for {entity}s from log are absent")
             setattr(self, scaler_name, MinMaxScaler().fit(features_np))
@@ -185,18 +178,15 @@
         log: DataFrame,
         user_features: Optional[DataFrame] = None,
         item_features: Optional[DataFrame] = None,
     ) -> None:
         self.user_feat_scaler = None
         self.item_feat_scaler = None
 
-        self.num_of_warm_items = len(self.item_indexer.labels)
-        self.num_of_warm_users = len(self.user_indexer.labels)
-
-        interactions_matrix = to_csr(log, self.users_count, self.items_count)
+        interactions_matrix = to_csr(log, self._user_dim, self._item_dim)
         csr_item_features = self._feature_table_to_csr(
             log.select("item_idx").distinct(), item_features
         )
         csr_user_features = self._feature_table_to_csr(
             log.select("user_idx").distinct(), user_features
         )
 
@@ -243,15 +233,15 @@
             pairs.select("item_idx").distinct(), item_features
         )
         csr_user_features = self._feature_table_to_csr(
             pairs.select("user_idx").distinct(), user_features
         )
 
         return pairs.groupby("user_idx").applyInPandas(
-            predict_by_user, IDX_REC_SCHEMA
+            predict_by_user, REC_SCHEMA
         )
 
     # pylint: disable=too-many-arguments
     def _predict(
         self,
         log: DataFrame,
         k: int,
@@ -282,25 +272,28 @@
         """
         Get features from LightFM.
         LightFM has methods get_item_representations/get_user_representations,
         which accept object matrix and return features.
 
         :param ids: id item_idx/user_idx to get features for
         :param features: features for item_idx/user_idx
-        :return: spark-dataframe с bias и векторами пользователей/объектов, размерность вектора
+        :return: spark-dataframe with biases and vectors for users/items and vector size
         """
         entity = "item" if "item_idx" in ids.columns else "user"
         ids_list = ids.toPandas()[f"{entity}_idx"]
 
         # models without features use sparse matrix
         if features is None:
-            matrix_width = getattr(self, f"num_of_warm_{entity}s")
+            matrix_width = getattr(self, f"fit_{entity}s").count()
             warm_ids = ids_list[ids_list < matrix_width]
             sparse_features = csr_matrix(
-                ([1] * warm_ids.shape[0], (warm_ids, warm_ids),),
+                (
+                    [1] * warm_ids.shape[0],
+                    (warm_ids, warm_ids),
+                ),
                 shape=(ids_list.max() + 1, matrix_width),
             )
         else:
             sparse_features = self._feature_table_to_csr(ids, features)
 
         biases, vectors = getattr(self.model, f"get_{entity}_representations")(
             sparse_features
@@ -311,10 +304,14 @@
                 ids_list,
                 biases[ids_list].tolist(),
                 vectors[ids_list].tolist(),
             )
         )
         lightfm_factors = State().session.createDataFrame(
             embed_list,
-            schema=[f"{entity}_idx", f"{entity}_bias", f"{entity}_factors",],
+            schema=[
+                f"{entity}_idx",
+                f"{entity}_bias",
+                f"{entity}_factors",
+            ],
         )
         return lightfm_factors, self.model.no_components
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `replay-rec-0.8.0/replay/models/mult_vae.py` & `replay-rec-0.9.0/replay/models/mult_vae.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 MultVAE implementation
 (Variational Autoencoders for Collaborative Filtering)
 """
 from typing import Optional, Tuple
 
 import numpy as np
 import pandas as pd
+import torch
+import torch.nn.functional as F
 from pyspark.sql import DataFrame
 from scipy.sparse import csr_matrix
 from sklearn.model_selection import GroupShuffleSplit
-import torch
 from torch import nn
-import torch.nn.functional as F
 from torch.optim import Adam
 from torch.optim.lr_scheduler import ReduceLROnPlateau
 from torch.utils.data import DataLoader, TensorDataset
 
 from replay.models.base_torch_rec import TorchRecommender
-from replay.session_handler import State
 
 
 class VAE(nn.Module):
     """Base variational autoencoder"""
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes
     def __init__(
@@ -143,75 +142,79 @@
         "learning_rate": {"type": "loguniform", "args": [0.0001, 0.5]},
         "epochs": {"type": "int", "args": [100, 100]},
         "latent_dim": {"type": "int", "args": [200, 200]},
         "hidden_dim": {"type": "int", "args": [600, 600]},
         "dropout": {"type": "uniform", "args": [0, 0.5]},
         "anneal": {"type": "uniform", "args": [0.2, 1]},
         "l2_reg": {"type": "loguniform", "args": [1e-9, 5]},
-        "gamma": {"type": "uniform", "args": [0.8, 0.99]},
+        "factor": {"type": "float", "args": [0.2, 0.2]},
+        "patience": {"type": "int", "args": [3, 3]},
     }
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         learning_rate: float = 0.01,
         epochs: int = 100,
         latent_dim: int = 200,
         hidden_dim: int = 600,
         dropout: float = 0.3,
         anneal: float = 0.1,
         l2_reg: float = 0,
-        gamma: float = 0.99,
+        factor: float = 0.2,
+        patience: int = 3,
     ):
         """
         :param learning_rate: learning rate
         :param epochs: number of epochs to train model
         :param latent_dim: latent dimension size for user vectors
         :param hidden_dim: hidden dimension size for encoder and decoder
         :param dropout: dropout coefficient
         :param anneal: anneal coefficient [0,1]
         :param l2_reg: l2 regularization term
-        :param gamma: reduce learning rate by this coefficient per epoch
+        :param factor: ReduceLROnPlateau reducing factor. new_lr = lr * factor
+        :param patience: number of non-improved epochs before reducing lr
         """
         super().__init__()
-        self.device = State().device
         self.learning_rate = learning_rate
         self.epochs = epochs
         self.latent_dim = latent_dim
         self.hidden_dim = hidden_dim
         self.dropout = dropout
         self.anneal = anneal
         self.l2_reg = l2_reg
-        self.gamma = gamma
+        self.factor = factor
+        self.patience = patience
 
     @property
     def _init_args(self):
         return {
             "learning_rate": self.learning_rate,
             "epochs": self.epochs,
             "latent_dim": self.latent_dim,
             "hidden_dim": self.hidden_dim,
             "dropout": self.dropout,
             "anneal": self.anneal,
             "l2_reg": self.l2_reg,
-            "gamma": self.gamma,
+            "factor": self.factor,
+            "patience": self.patience,
         }
 
     def _get_data_loader(
         self, data: pd.DataFrame, shuffle: bool = True
     ) -> Tuple[csr_matrix, DataLoader, np.ndarray]:
         """get data loader and matrix with data"""
         users_count = data["user_idx"].value_counts().count()
         user_idx = data["user_idx"].astype("category").cat  # type: ignore
         user_batch = csr_matrix(
             (
                 np.ones(len(data["user_idx"])),
                 ([user_idx.codes.values, data["item_idx"].values]),
             ),
-            shape=(users_count, self.items_count),
+            shape=(users_count, self._item_dim),
         )
         data_loader = DataLoader(
             TensorDataset(torch.arange(users_count).long()),
             batch_size=self.batch_size_users,
             shuffle=shuffle,
             num_workers=self.num_workers,
         )
@@ -221,15 +224,15 @@
     # pylint: disable=too-many-locals
     def _fit(
         self,
         log: DataFrame,
         user_features: Optional[DataFrame] = None,
         item_features: Optional[DataFrame] = None,
     ) -> None:
-        self.logger.debug("Creating batch:")
+        self.logger.debug("Creating batch")
         data = log.select("user_idx", "item_idx").toPandas()
         splitter = GroupShuffleSplit(
             n_splits=1, test_size=self.valid_split_size, random_state=self.seed
         )
         train_idx, valid_idx = next(
             splitter.split(data, groups=data["user_idx"])
         )
@@ -240,37 +243,37 @@
         )
         self.valid_user_batch, valid_data_loader, _ = self._get_data_loader(
             valid_data, False
         )
 
         self.logger.debug("Training VAE")
         self.model = VAE(
-            item_count=self.items_count,
+            item_count=self._item_dim,
             latent_dim=self.latent_dim,
             hidden_dim=self.hidden_dim,
             dropout=self.dropout,
         ).to(self.device)
-
         optimizer = Adam(
             self.model.parameters(),
             lr=self.learning_rate,
             weight_decay=self.l2_reg / self.batch_size_users,
         )
-        lr_scheduler = ReduceLROnPlateau(optimizer, factor=0.5, patience=3)
+        lr_scheduler = ReduceLROnPlateau(
+            optimizer, factor=self.factor, patience=self.patience
+        )
 
-        vae_trainer, _ = self._create_trainer_evaluator(
-            optimizer,
+        self.train(
+            train_data_loader,
             valid_data_loader,
+            optimizer,
             lr_scheduler,
-            self.patience,
-            self.n_saved,
+            self.epochs,
+            "multvae",
         )
 
-        vae_trainer.run(train_data_loader, max_epochs=self.epochs)
-
     # pylint: disable=arguments-differ
     def _loss(self, y_pred, y_true, mu_latent, logvar_latent):
         log_softmax_var = F.log_softmax(y_pred, dim=1)
         bce = -(log_softmax_var * y_true).sum(dim=1).mean()
         kld = (
             -0.5
             * torch.sum(
@@ -287,19 +290,20 @@
             full_batch = self.valid_user_batch
         user_batch = torch.FloatTensor(full_batch[batch[0]].toarray()).to(
             self.device
         )
         pred_user_batch, latent_mu, latent_logvar = self.model.forward(
             user_batch
         )
-        return (
-            pred_user_batch,
-            user_batch,
-            {"mu_latent": latent_mu, "logvar_latent": latent_logvar},
-        )
+        return {
+            "y_pred": pred_user_batch,
+            "y_true": user_batch,
+            "mu_latent": latent_mu,
+            "logvar_latent": latent_logvar,
+        }
 
     @staticmethod
     def _predict_pairs_inner(
         model: nn.Module,
         user_idx: int,
         items_np_history: np.ndarray,
         items_np_to_pred: np.ndarray,
@@ -343,36 +347,29 @@
             items_np_to_pred=items_np,
             item_count=item_count,
             cnt=min(len(pandas_df) + k, len(items_np)),
         )
 
     @staticmethod
     def _predict_by_user_pairs(
-        pandas_df: pd.DataFrame, model: nn.Module, item_count: int,
+        pandas_df: pd.DataFrame,
+        model: nn.Module,
+        item_count: int,
     ) -> pd.DataFrame:
-
-        items_np_history = np.array(
-            (
-                pandas_df["item_idx_history"][0]
-                if pandas_df["item_idx_history"][0] is not None
-                else []
-            )
-        )
-
         return MultVAE._predict_pairs_inner(
             model=model,
             user_idx=pandas_df["user_idx"][0],
-            items_np_history=items_np_history,
+            items_np_history=np.array(pandas_df["item_idx_history"][0]),
             items_np_to_pred=np.array(pandas_df["item_idx_to_pred"][0]),
             item_count=item_count,
             cnt=None,
         )
 
     def _load_model(self, path: str):
         self.model = VAE(
-            item_count=self.items_count,
+            item_count=self._item_dim,
             latent_dim=self.latent_dim,
             hidden_dim=self.hidden_dim,
             dropout=self.dropout,
         ).to(self.device)
         self.model.load_state_dict(torch.load(path))
         self.model.eval()
```

### Comparing `replay-rec-0.8.0/replay/models/neuromf.py` & `replay-rec-0.9.0/replay/models/neuromf.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 Multi-Layer Perceptron (MLP),
 Neural Matrix Factorization (MLP + GMF).
 """
 from typing import List, Optional
 
 import numpy as np
 import pandas as pd
+import torch
 import torch.nn.functional as F
-import torch.optim
-from ignite.engine import Engine
 from pyspark.sql import DataFrame
 from sklearn.model_selection import train_test_split
 from torch import LongTensor, Tensor, nn
-from torch.optim.lr_scheduler import ExponentialLR
+from torch.optim import Adam
+from torch.optim.lr_scheduler import ReduceLROnPlateau
 from torch.utils.data import DataLoader, TensorDataset
 
 from replay.models.base_torch_rec import TorchRecommender
-from replay.session_handler import State
 
 EMBED_DIM = 128
 
 
 def xavier_init_(layer: nn.Module):
     """
     Xavier initialization
@@ -202,15 +201,15 @@
 
         if self.mlp:
             mlp_vector = self.mlp(user, item)
         else:
             mlp_vector = torch.zeros(batch_size, 0).to(user.device)
 
         merged_vector = torch.cat([gmf_vector, mlp_vector], dim=1)
-        merged_vector = self.last_layer(merged_vector).squeeze()
+        merged_vector = self.last_layer(merged_vector).squeeze(dim=1)
         merged_vector = torch.sigmoid(merged_vector)
 
         return merged_vector
 
 
 # pylint: disable=too-many-instance-attributes
 class NeuroMF(TorchRecommender):
@@ -218,87 +217,89 @@
     Neural Matrix Factorization model (NeuMF, NCF).
 
     In this implementation MLP and GMF modules are optional.
     """
 
     num_workers: int = 0
     batch_size_users: int = 100000
-    trainer: Engine
-    val_evaluator: Engine
     patience: int = 3
     n_saved: int = 2
     valid_split_size: float = 0.1
     seed: int = 42
     _search_space = {
         "embedding_gmf_dim": {"type": "int", "args": [EMBED_DIM, EMBED_DIM]},
         "embedding_mlp_dim": {"type": "int", "args": [EMBED_DIM, EMBED_DIM]},
         "learning_rate": {"type": "loguniform", "args": [0.0001, 0.5]},
         "l2_reg": {"type": "loguniform", "args": [1e-9, 5]},
-        "gamma": {"type": "uniform", "args": [0.8, 0.99]},
         "count_negative_sample": {"type": "int", "args": [1, 20]},
+        "factor": {"type": "float", "args": [0.2, 0.2]},
+        "patience": {"type": "int", "args": [3, 3]},
     }
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         learning_rate: float = 0.05,
         epochs: int = 20,
         embedding_gmf_dim: Optional[int] = None,
         embedding_mlp_dim: Optional[int] = None,
         hidden_mlp_dims: Optional[List[int]] = None,
         l2_reg: float = 0,
-        gamma: float = 0.99,
         count_negative_sample: int = 1,
+        factor: float = 0.2,
+        patience: int = 3,
     ):
         """
         MLP or GMF model can be ignored if
         its embedding size (embedding_mlp_dim or embedding_gmf_dim) is set to ``None``.
         Default variant is MLP + GMF with embedding size 128.
 
         :param learning_rate: learning rate
         :param epochs: number of epochs to train model
         :param embedding_gmf_dim: embedding size for gmf
         :param embedding_mlp_dim: embedding size for mlp
         :param hidden_mlp_dims: list of hidden dimension sized for mlp
         :param l2_reg: l2 regularization term
-        :param gamma: decrease learning rate by this coefficient per epoch
         :param count_negative_sample: number of negative samples to use
+        :param factor: ReduceLROnPlateau reducing factor. new_lr = lr * factor
+        :param patience: number of non-improved epochs before reducing lr
         """
         super().__init__()
         if not embedding_gmf_dim and not embedding_mlp_dim:
             embedding_gmf_dim, embedding_mlp_dim = EMBED_DIM, EMBED_DIM
 
         if (embedding_gmf_dim is None or embedding_gmf_dim < 0) and (
             embedding_mlp_dim is None or embedding_mlp_dim < 0
         ):
             raise ValueError(
                 "embedding_gmf_dim and embedding_mlp_dim must be positive"
             )
 
-        self.device = State().device
         self.learning_rate = learning_rate
         self.epochs = epochs
         self.embedding_gmf_dim = embedding_gmf_dim
         self.embedding_mlp_dim = embedding_mlp_dim
         self.hidden_mlp_dims = hidden_mlp_dims
         self.l2_reg = l2_reg
-        self.gamma = gamma
         self.count_negative_sample = count_negative_sample
+        self.factor = factor
+        self.patience = patience
 
     @property
     def _init_args(self):
         return {
             "learning_rate": self.learning_rate,
             "epochs": self.epochs,
             "embedding_gmf_dim": self.embedding_gmf_dim,
             "embedding_mlp_dim": self.embedding_mlp_dim,
             "hidden_mlp_dims": self.hidden_mlp_dims,
             "l2_reg": self.l2_reg,
-            "gamma": self.gamma,
             "count_negative_sample": self.count_negative_sample,
+            "factor": self.factor,
+            "patience": self.patience,
         }
 
     def _data_loader(
         self, data: pd.DataFrame, shuffle: bool = True
     ) -> DataLoader:
 
         user_batch = LongTensor(data["user_idx"].values)  # type: ignore
@@ -311,64 +312,69 @@
             batch_size=self.batch_size_users,
             shuffle=shuffle,
             num_workers=self.num_workers,
         )
         return loader
 
     def _get_neg_batch(self, batch: Tensor) -> Tensor:
-        negative_items = torch.randint(
-            0,
-            self.items_count - 1,
-            (batch.shape[0] * self.count_negative_sample,),
+        return torch.from_numpy(
+            np.random.choice(
+                self._fit_items_np, batch.shape[0] * self.count_negative_sample
+            )
         )
-        return negative_items
 
     def _fit(
         self,
         log: DataFrame,
         user_features: Optional[DataFrame] = None,
         item_features: Optional[DataFrame] = None,
     ) -> None:
-        self.model = NMF(
-            user_count=self.users_count,
-            item_count=self.items_count,
-            embedding_gmf_dim=self.embedding_gmf_dim,
-            embedding_mlp_dim=self.embedding_mlp_dim,
-            hidden_mlp_dims=self.hidden_mlp_dims,
-        ).to(self.device)
-
-        self.logger.debug("Create batch")
+        self.logger.debug("Create DataLoaders")
         tensor_data = log.select("user_idx", "item_idx").toPandas()
         train_tensor_data, valid_tensor_data = train_test_split(
             tensor_data,
             test_size=self.valid_split_size,
             random_state=self.seed,
         )
         train_data_loader = self._data_loader(train_tensor_data)
-        val_data_loader = self._data_loader(valid_tensor_data)
+        valid_data_loader = self._data_loader(valid_tensor_data)
+        # pylint: disable=attribute-defined-outside-init
+        self._fit_items_np = self.fit_items.toPandas().to_numpy().ravel()
 
-        self.logger.debug("Train NeuroMF")
-        optimizer = torch.optim.Adam(
+        self.logger.debug("Training NeuroMF")
+        self.model = NMF(
+            user_count=self._user_dim,
+            item_count=self._item_dim,
+            embedding_gmf_dim=self.embedding_gmf_dim,
+            embedding_mlp_dim=self.embedding_mlp_dim,
+            hidden_mlp_dims=self.hidden_mlp_dims,
+        ).to(self.device)
+        optimizer = Adam(
             self.model.parameters(),
             lr=self.learning_rate,
             weight_decay=self.l2_reg / self.batch_size_users,
         )
-        lr_scheduler = ExponentialLR(optimizer, gamma=self.gamma)
-        nmf_trainer, _ = self._create_trainer_evaluator(
+        lr_scheduler = ReduceLROnPlateau(
+            optimizer, factor=self.factor, patience=self.patience
+        )
+
+        self.train(
+            train_data_loader,
+            valid_data_loader,
             optimizer,
-            val_data_loader,
             lr_scheduler,
-            self.patience,
-            self.n_saved,
+            self.epochs,
+            "neuromf",
         )
 
-        nmf_trainer.run(train_data_loader, max_epochs=self.epochs)
+        del self._fit_items_np
 
     # pylint: disable=arguments-differ
-    def _loss(self, y_pred, y_true):
+    @staticmethod
+    def _loss(y_pred, y_true):
         return F.binary_cross_entropy(y_pred, y_true).mean()
 
     def _batch_pass(self, batch, model):
         user_batch, pos_item_batch = batch
         neg_item_batch = self._get_neg_batch(user_batch)
         pos_relevance = model(
             user_batch.to(self.device), pos_item_batch.to(self.device)
@@ -378,29 +384,32 @@
             neg_item_batch.to(self.device),
         )
         y_pred = torch.cat((pos_relevance, neg_relevance), 0)
         y_true_pos = torch.ones_like(pos_item_batch).to(self.device)
         y_true_neg = torch.zeros_like(neg_item_batch).to(self.device)
         y_true = torch.cat((y_true_pos, y_true_neg), 0).float()
 
-        return y_pred, y_true
+        return {"y_pred": y_pred, "y_true": y_true}
 
     @staticmethod
     def _predict_pairs_inner(
         model: nn.Module,
         user_idx: int,
         items_np: np.ndarray,
         cnt: Optional[int] = None,
     ) -> DataFrame:
         model.eval()
         with torch.no_grad():
             user_batch = LongTensor([user_idx] * len(items_np))
             item_batch = LongTensor(items_np)
             user_recs = torch.reshape(
-                model(user_batch, item_batch).detach(), [-1,],
+                model(user_batch, item_batch).detach(),
+                [
+                    -1,
+                ],
             )
             if cnt is not None:
                 best_item_idx = (
                     torch.argsort(user_recs, descending=True)[:cnt]
                 ).numpy()
                 user_recs = user_recs[best_item_idx]
                 items_np = items_np[best_item_idx]
@@ -437,15 +446,15 @@
             user_idx=pandas_df["user_idx"][0],
             items_np=np.array(pandas_df["item_idx_to_pred"][0]),
             cnt=None,
         )
 
     def _load_model(self, path: str):
         self.model = NMF(
-            user_count=self.users_count,
-            item_count=self.items_count,
+            user_count=self._user_dim,
+            item_count=self._item_dim,
             embedding_gmf_dim=self.embedding_gmf_dim,
             embedding_mlp_dim=self.embedding_mlp_dim,
             hidden_mlp_dims=self.hidden_mlp_dims,
         ).to(self.device)
         self.model.load_state_dict(torch.load(path))
         self.model.eval()
```

### Comparing `replay-rec-0.8.0/replay/models/pop_rec.py` & `replay-rec-0.9.0/replay/models/pop_rec.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,47 +16,50 @@
         Popularity(i) = \\dfrac{N_i}{N}
 
     :math:`N_i` - number of users who rated item :math:`i`
 
     :math:`N` - total number of users
 
     >>> import pandas as pd
-    >>> data_frame = pd.DataFrame({"user_id": [1, 1, 2, 2, 3, 4], "item_id": [1, 2, 2, 3, 3, 3], "relevance": [0.5, 1, 0.1, 0.8, 0.7, 1]})
+    >>> data_frame = pd.DataFrame({"user_idx": [1, 1, 2, 2, 3, 4], "item_idx": [1, 2, 2, 3, 3, 3], "relevance": [0.5, 1, 0.1, 0.8, 0.7, 1]})
     >>> data_frame
-       user_id  item_id  relevance
-    0        1        1        0.5
-    1        1        2        1.0
-    2        2        2        0.1
-    3        2        3        0.8
-    4        3        3        0.7
-    5        4        3        1.0
+       user_idx  item_idx  relevance
+    0         1         1        0.5
+    1         1         2        1.0
+    2         2         2        0.1
+    3         2         3        0.8
+    4         3         3        0.7
+    5         4         3        1.0
+
+    >>> from replay.utils import convert2spark
+    >>> data_frame = convert2spark(data_frame)
 
     >>> res = PopRec().fit_predict(data_frame, 1)
-    >>> res.toPandas().sort_values("user_id", ignore_index=True)
-       user_id  item_id  relevance
-    0        1        3       0.75
-    1        2        1       0.25
-    2        3        2       0.50
-    3        4        2       0.50
+    >>> res.toPandas().sort_values("user_idx", ignore_index=True)
+       user_idx  item_idx  relevance
+    0         1         3       0.75
+    1         2         1       0.25
+    2         3         2       0.50
+    3         4         2       0.50
 
     >>> res = PopRec().fit_predict(data_frame, 1, filter_seen_items=False)
-    >>> res.toPandas().sort_values("user_id", ignore_index=True)
-       user_id  item_id  relevance
-    0        1        3       0.75
-    1        2        3       0.75
-    2        3        3       0.75
-    3        4        3       0.75
+    >>> res.toPandas().sort_values("user_idx", ignore_index=True)
+       user_idx  item_idx  relevance
+    0         1         3       0.75
+    1         2         3       0.75
+    2         3         3       0.75
+    3         4         3       0.75
 
     >>> res = PopRec(use_relevance=True).fit_predict(data_frame, 1)
-    >>> res.toPandas().sort_values("user_id", ignore_index=True)
-       user_id  item_id  relevance
-    0        1        3      0.625
-    1        2        1      0.125
-    2        3        2      0.275
-    3        4        2      0.275
+    >>> res.toPandas().sort_values("user_idx", ignore_index=True)
+       user_idx  item_idx  relevance
+    0         1         3      0.625
+    1         2         1      0.125
+    2         3         2      0.275
+    3         4         2      0.275
 
     """
 
     item_popularity: DataFrame
     can_predict_cold_users = True
 
     def __init__(self, use_relevance: bool = False):
@@ -112,46 +115,40 @@
         users: DataFrame,
         items: DataFrame,
         user_features: Optional[DataFrame] = None,
         item_features: Optional[DataFrame] = None,
         filter_seen_items: bool = True,
     ) -> DataFrame:
         selected_item_popularity = self.item_popularity.join(
-            items, on="item_idx", how="inner",
+            items,
+            on="item_idx",
+            how="inner",
         ).withColumn(
             "rank",
             sf.row_number().over(Window.orderBy(sf.col("relevance").desc())),
         )
 
-        if not filter_seen_items:
-            return users.crossJoin(
-                selected_item_popularity.filter(sf.col("rank") <= k)
-            ).drop("rank")
-
-        log_by_user = (
-            log.join(users, on="user_idx")
-            .groupBy("user_idx")
-            .agg(sf.countDistinct("item_idx").alias("items_count"))
-        )
-        max_history_len = log_by_user.select(sf.max("items_count")).collect()[
-            0
-        ][0]
-        cropped_item_popularity = selected_item_popularity.filter(
-            sf.col("rank") <= max_history_len + k
-        )
-
-        log_by_user_with_new_users = log_by_user.join(
-            users, on="user_idx", how="right"
-        ).fillna(0)
-        recs = log_by_user_with_new_users.join(
-            cropped_item_popularity,
-            on=sf.col("rank") <= sf.col("items_count") + sf.lit(k),
-        ).drop("rank", "items_count")
-
-        return recs
+        max_hist_len = 0
+        if filter_seen_items:
+            max_hist_len = (
+                (
+                    log.join(users, on="user_idx")
+                    .groupBy("user_idx")
+                    .agg(sf.countDistinct("item_idx").alias("items_count"))
+                )
+                .select(sf.max("items_count"))
+                .collect()[0][0]
+            )
+            # all users have empty history
+            if max_hist_len is None:
+                max_hist_len = 0
+
+        return users.crossJoin(
+            selected_item_popularity.filter(sf.col("rank") <= k + max_hist_len)
+        ).drop("rank")
 
     def _predict_pairs(
         self,
         pairs: DataFrame,
         log: Optional[DataFrame] = None,
         user_features: Optional[DataFrame] = None,
         item_features: Optional[DataFrame] = None,
```

### Comparing `replay-rec-0.8.0/replay/models/random_rec.py` & `replay-rec-0.9.0/replay/models/random_rec.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pandas as pd
 
 from numpy.random import default_rng
 from pyspark.sql import DataFrame
 from pyspark.sql import functions as sf
 
 from replay.models.base_rec import Recommender
-from replay.constants import IDX_REC_SCHEMA
+from replay.constants import REC_SCHEMA
 
 
 class RandomRec(Recommender):
     """
     Recommend random items, either weighted by item popularity or uniform.
 
     .. math::
@@ -27,28 +27,28 @@
     >>> spark = get_spark_session(1, 1)
     >>> state = State(spark)
 
     >>> import pandas as pd
     >>> from replay.utils import convert2spark
     >>>
     >>> log = convert2spark(pd.DataFrame({
-    ...     "user_id": ["1", "1", "2", "2", "3", "4"],
-    ...     "item_id": ["1", "2", "2", "3", "3", "3"]
+    ...     "user_idx": [1, 1, 2, 2, 3, 4],
+    ...     "item_idx": [1, 2, 2, 3, 3, 3]
     ... }))
     >>> log.show()
-    +-------+-------+
-    |user_id|item_id|
-    +-------+-------+
-    |      1|      1|
-    |      1|      2|
-    |      2|      2|
-    |      2|      3|
-    |      3|      3|
-    |      4|      3|
-    +-------+-------+
+    +--------+--------+
+    |user_idx|item_idx|
+    +--------+--------+
+    |       1|       1|
+    |       1|       2|
+    |       2|       2|
+    |       2|       3|
+    |       3|       3|
+    |       4|       3|
+    +--------+--------+
     <BLANKLINE>
     >>> random_pop = RandomRec(distribution="popular_based", alpha=-1)
     Traceback (most recent call last):
      ...
     ValueError: alpha must be bigger than -1
 
     >>> random_pop = RandomRec(distribution="abracadabra")
@@ -58,50 +58,50 @@
 
     >>> random_pop = RandomRec(distribution="popular_based", alpha=1.0, seed=777)
     >>> random_pop.fit(log)
     >>> random_pop.item_popularity.show()
     +--------+-----------+
     |item_idx|probability|
     +--------+-----------+
-    |       2|        2.0|
-    |       1|        3.0|
-    |       0|        4.0|
+    |       1|        2.0|
+    |       2|        3.0|
+    |       3|        4.0|
     +--------+-----------+
     <BLANKLINE>
     >>> recs = random_pop.predict(log, 2)
     >>> recs.show()
-    +-------+-------+------------------+
-    |user_id|item_id|         relevance|
-    +-------+-------+------------------+
-    |      1|      3|               1.0|
-    |      2|      1|               0.5|
-    |      3|      2|               1.0|
-    |      3|      1|               0.5|
-    |      4|      2|               1.0|
-    |      4|      1|0.3333333333333333|
-    +-------+-------+------------------+
+    +--------+--------+------------------+
+    |user_idx|item_idx|         relevance|
+    +--------+--------+------------------+
+    |       1|       3|0.3333333333333333|
+    |       2|       1|               0.5|
+    |       3|       2|               1.0|
+    |       3|       1|0.3333333333333333|
+    |       4|       2|               1.0|
+    |       4|       1|               0.5|
+    +--------+--------+------------------+
     <BLANKLINE>
     >>> recs = random_pop.predict(log, 2, users=[1], items=[7, 8])
     >>> recs.show()
-    +-------+-------+---------+
-    |user_id|item_id|relevance|
-    +-------+-------+---------+
-    |      1|      8|      1.0|
-    |      1|      7|      0.5|
-    +-------+-------+---------+
+    +--------+--------+---------+
+    |user_idx|item_idx|relevance|
+    +--------+--------+---------+
+    |       1|       7|      1.0|
+    |       1|       8|      0.5|
+    +--------+--------+---------+
     <BLANKLINE>
     >>> random_pop = RandomRec(seed=555)
     >>> random_pop.fit(log)
     >>> random_pop.item_popularity.show()
     +--------+-----------+
     |item_idx|probability|
     +--------+-----------+
-    |       2|        1.0|
     |       1|        1.0|
-    |       0|        1.0|
+    |       2|        1.0|
+    |       3|        1.0|
     +--------+-----------+
     <BLANKLINE>
     """
 
     can_predict_cold_users = True
     can_predict_cold_items = True
     _search_space = {
@@ -272,11 +272,11 @@
             .select("user_idx", "item_idx")
             .groupby("user_idx")
             .agg(sf.countDistinct("item_idx").alias("cnt"))
             .selectExpr(
                 "user_idx", f"LEAST(cnt + {k}, {items_np.shape[0]}) AS cnt",
             )
             .groupby("user_idx")
-            .applyInPandas(grouped_map, IDX_REC_SCHEMA)
+            .applyInPandas(grouped_map, REC_SCHEMA)
         )
 
         return recs
```

### Comparing `replay-rec-0.8.0/replay/models/slim.py` & `replay-rec-0.9.0/replay/models/slim.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,20 +47,20 @@
         user_features: Optional[DataFrame] = None,
         item_features: Optional[DataFrame] = None,
     ) -> None:
         pandas_log = log.select("user_idx", "item_idx", "relevance").toPandas()
 
         interactions_matrix = csc_matrix(
             (pandas_log.relevance, (pandas_log.user_idx, pandas_log.item_idx)),
-            shape=(self.users_count, self.items_count),
+            shape=(self._user_dim, self._item_dim),
         )
         similarity = (
             State()
             .session.createDataFrame(pandas_log.item_idx, st.IntegerType())
-            .withColumnRenamed("value", "item_id_one")
+            .withColumnRenamed("value", "item_idx_one")
         )
 
         alpha = self.beta + self.lambda_
         l1_ratio = self.lambda_ / alpha
 
         regression = ElasticNet(
             alpha=alpha,
@@ -74,29 +74,30 @@
 
         def slim_column(pandas_df: pd.DataFrame) -> pd.DataFrame:
             """
             fit similarity matrix with ElasticNet
             :param pandas_df: pd.Dataframe
             :return: pd.Dataframe
             """
-            idx = int(pandas_df["item_id_one"][0])
+            idx = int(pandas_df["item_idx_one"][0])
             column = interactions_matrix[:, idx]
             column_arr = column.toarray().ravel()
             interactions_matrix[
                 interactions_matrix[:, idx].nonzero()[0], idx
             ] = 0
 
             regression.fit(interactions_matrix, column_arr)
             interactions_matrix[:, idx] = column
             good_idx = np.argwhere(regression.coef_ > 0).reshape(-1)
             good_values = regression.coef_[good_idx]
             similarity_row = {
-                "item_id_one": good_idx,
-                "item_id_two": idx,
+                "item_idx_one": good_idx,
+                "item_idx_two": idx,
                 "similarity": good_values,
             }
             return pd.DataFrame(data=similarity_row)
 
-        self.similarity = similarity.groupby("item_id_one").applyInPandas(
-            slim_column, "item_id_one int, item_id_two int, similarity double"
+        self.similarity = similarity.groupby("item_idx_one").applyInPandas(
+            slim_column,
+            "item_idx_one int, item_idx_two int, similarity double",
         )
         self.similarity.cache()
```

### Comparing `replay-rec-0.8.0/replay/models/user_pop_rec.py` & `replay-rec-0.9.0/replay/models/user_pop_rec.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,29 +18,31 @@
     .. math::
         Popularity(i_u) = \\dfrac{N_iu}{N_u}
 
     :math:`N_iu` - number of interactions of user :math:`u` with item :math:`i`.
     :math:`N_u` - total number of interactions of user :math:`u`.
 
     >>> import pandas as pd
-    >>> data_frame = pd.DataFrame({"user_id": [1, 1, 3], "item_id": [1, 2, 3], "relevance": [2, 1, 1]})
+    >>> data_frame = pd.DataFrame({"user_idx": [1, 1, 3], "item_idx": [1, 2, 3], "relevance": [2, 1, 1]})
     >>> data_frame
-       user_id  item_id  relevance
-    0        1        1          2
-    1        1        2          1
-    2        3        3          1
+       user_idx  item_idx  relevance
+    0         1         1          2
+    1         1         2          1
+    2         3         3          1
 
+    >>> from replay.utils import convert2spark
+    >>> data_frame = convert2spark(data_frame)
     >>> model = UserPopRec()
     >>> res = model.fit_predict(data_frame, 1, filter_seen_items=False)
     >>> model.user_item_popularity.count()
     3
-    >>> res.toPandas().sort_values("user_id", ignore_index=True)
-       user_id  item_id  relevance
-    0        1        1   0.666667
-    1        3        3   1.000000
+    >>> res.toPandas().sort_values("user_idx", ignore_index=True)
+       user_idx  item_idx  relevance
+    0         1         1   0.666667
+    1         3         3   1.000000
     """
 
     user_item_popularity: DataFrame
 
     @property
     def _init_args(self):
         return {}
@@ -108,19 +110,16 @@
     def fit_predict(
         self,
         log: AnyDataFrame,
         k: int,
         users: Optional[Union[AnyDataFrame, Iterable]] = None,
         items: Optional[Union[AnyDataFrame, Iterable]] = None,
         filter_seen_items: bool = False,
-        force_reindex: bool = False,
     ) -> DataFrame:
-        return super().fit_predict(
-            log, k, users, items, filter_seen_items, force_reindex
-        )
+        return super().fit_predict(log, k, users, items, filter_seen_items)
 
     # pylint: disable=too-many-arguments
     def predict(
         self,
         log: AnyDataFrame,
         k: int,
         users: Optional[Union[AnyDataFrame, Iterable]] = None,
```

### Comparing `replay-rec-0.8.0/replay/models/wilson.py` & `replay-rec-0.9.0/replay/models/wilson.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,20 +11,22 @@
     """
     Calculates lower confidence bound for the confidence interval
     of true fraction of positive ratings.
 
     ``relevance`` must be converted to binary 0-1 form.
 
     >>> import pandas as pd
-    >>> data_frame = pd.DataFrame({"user_id": [1, 2], "item_id": [1, 2], "relevance": [1, 1]})
+    >>> data_frame = pd.DataFrame({"user_idx": [1, 2], "item_idx": [1, 2], "relevance": [1, 1]})
+    >>> from replay.utils import convert2spark
+    >>> data_frame = convert2spark(data_frame)
     >>> model = Wilson()
     >>> model.fit_predict(data_frame,k=1).toPandas()
-      user_id item_id  relevance
-    0       1       2   0.206549
-    1       2       1   0.206549
+       user_idx  item_idx  relevance
+    0         1         2   0.206549
+    1         2         1   0.206549
 
     """
 
     def __init__(self, alpha=0.05):
         """
         :param alpha: significance level, default 0.05
         """
```

### Comparing `replay-rec-0.8.0/replay/models/word2vec.py` & `replay-rec-0.9.0/replay/models/word2vec.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     ) -> None:
         self.idf = (
             log.groupBy("item_idx")
             .agg(sf.countDistinct("user_idx").alias("count"))
             .select(
                 "item_idx",
                 (
-                    sf.log(self.users_count / sf.col("count"))
+                    sf.log(sf.lit(self.users_count) / sf.col("count"))
                     if self.use_idf
                     else sf.lit(1.0)
                 ).alias("idf"),
             )
         )
         self.idf.cache()
 
@@ -130,15 +130,17 @@
             self.vectors.unpersist()
 
     @property
     def _dataframes(self):
         return {"idf": self.idf, "vectors": self.vectors}
 
     def _get_user_vectors(
-        self, users: DataFrame, log: DataFrame,
+        self,
+        users: DataFrame,
+        log: DataFrame,
     ) -> DataFrame:
         """
         :param users: user ids, dataframe ``[user_idx]``
         :param log: interaction dataframe
             ``[user_idx, item_idx, timestamp, relevance]``
         :return: user embeddings dataframe
             ``[user_idx, user_vector]``
@@ -157,15 +159,17 @@
                     vector_mult(sf.col("idf"), sf.col("vector"))
                 ).alias("user_vector")
             )
             .select("user_idx", "user_vector")
         )
 
     def _predict_pairs_inner(
-        self, pairs: DataFrame, log: DataFrame,
+        self,
+        pairs: DataFrame,
+        log: DataFrame,
     ) -> DataFrame:
         if log is None:
             raise ValueError(
                 f"log is not provided, {self.__str__()} predict requires log."
             )
 
         user_vectors = self._get_user_vectors(
```

### Comparing `replay-rec-0.8.0/replay/optuna_objective.py` & `replay-rec-0.9.0/replay/optuna_objective.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 import collections
 import logging
 from functools import partial
 from typing import Any, Dict, List, Optional, Callable, Union
 
 from optuna import Trial
+from pyspark.sql import functions as sf
 
 from replay.metrics.base_metric import Metric
 
 SplitData = collections.namedtuple(
     "SplitData",
     "train test users items user_features_train "
     "user_features_test item_features_train item_features_test",
@@ -90,15 +91,14 @@
     logger = logging.getLogger("replay")
     logger.debug("Fitting model inside optimization")
     # pylint: disable=protected-access
     recommender._fit_wrap(
         split_data.train,
         split_data.user_features_train,
         split_data.item_features_train,
-        False,
     )
     logger.debug("Predicting inside optimization")
     recs = recommender._predict_wrap(
         log=split_data.train,
         k=k,
         users=split_data.users,
         items=split_data.items,
@@ -134,7 +134,87 @@
     recommender.set_params(**params_for_trial)
     return eval_quality(split_data, recommender, criterion, k)
 
 
 MainObjective = partial(
     ObjectiveWrapper, objective_calculator=scenario_objective_calculator
 )
+
+
+# pylint: disable=too-few-public-methods
+class KNNObjective:
+    """
+    This class is implemented according to
+    `instruction <https://optuna.readthedocs.io/en/stable/faq.html#how-to-define-objective-functions-that-have-own-arguments>`_
+    on integration with ``optuna``.
+
+    Criterion is calculated with ``__call__``,
+    other arguments are passed into ``__init__``.
+    """
+
+    # pylint: disable=too-many-arguments,too-many-instance-attributes
+
+    def __init__(self, **kwargs: Any):
+        self.kwargs = kwargs
+        max_neighbours = self.kwargs["search_space"]["num_neighbours"]["args"][
+            1
+        ]
+        model = self.kwargs["recommender"]
+        split_data = self.kwargs["split_data"]
+        train = split_data.train
+        model.num_neighbours = max_neighbours
+
+        df = train.select("user_idx", "item_idx", "relevance")
+        if not model.use_relevance:
+            df = df.withColumn("relevance", sf.lit(1))
+
+        self.dot_products = model._get_products(df).cache()
+
+    def objective_calculator(
+        self,
+        trial: Trial,
+        search_space: Dict[str, List[Optional[Any]]],
+        split_data: SplitData,
+        recommender,
+        criterion: Metric,
+        k: int,
+    ) -> float:
+        """
+        Sample parameters and calculate criterion value
+        :param trial: optuna trial
+        :param search_space: hyper parameter search space
+        :param split_data: data to train and test model
+        :param recommender: recommender model
+        :param criterion: optimization metric
+        :param k: length of a recommendation list
+        :return: criterion value
+        """
+        params_for_trial = suggest_params(trial, search_space)
+        recommender.set_params(**params_for_trial)
+        recommender.fit_users = split_data.train.select("user_idx").distinct()
+        recommender.fit_items = split_data.train.select("item_idx").distinct()
+        similarity = recommender._shrink(self.dot_products, recommender.shrink)
+        recommender.similarity = recommender._get_k_most_similar(
+            similarity
+        ).cache()
+        recs = recommender._predict_wrap(
+            log=split_data.train,
+            k=k,
+            users=split_data.users,
+            items=split_data.items,
+            user_features=split_data.user_features_test,
+            item_features=split_data.item_features_test,
+        )
+        logger = logging.getLogger("replay")
+        logger.debug("Calculating criterion")
+        criterion_value = criterion(recs, split_data.test, k)
+        logger.debug("%s=%.6f", criterion, criterion_value)
+        return criterion_value
+
+    def __call__(self, trial: Trial) -> float:
+        """
+        Calculate criterion for ``optuna``.
+
+        :param trial: current trial
+        :return: criterion value
+        """
+        return self.objective_calculator(trial=trial, **self.kwargs)
```

### Comparing `replay-rec-0.8.0/replay/scenarios/basescenario.py` & `replay-rec-0.9.0/replay/scenarios/basescenario.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,29 +23,25 @@
         self.hot_users = None
 
     def fit(
         self,
         log: AnyDataFrame,
         user_features: Optional[AnyDataFrame] = None,
         item_features: Optional[AnyDataFrame] = None,
-        force_reindex: bool = True,
     ) -> None:
         """
         :param log: input DataFrame ``[user_id, item_id, timestamp, relevance]``
         :param user_features: user features ``[user_id, timestamp]`` + feature columns
         :param item_features: item features ``[item_id, timestamp]`` + feature columns
-        :param force_reindex: create indexers even if they exist
         :return:
         """
         hot_data = min_entries(log, self.threshold)
-        self.hot_users = hot_data.select("user_id").distinct()
-        self._fit_wrap(hot_data, user_features, item_features, force_reindex)
-        self.cold_model._fit_wrap(
-            log, user_features, item_features, force_reindex
-        )
+        self.hot_users = hot_data.select("user_idx").distinct()
+        self._fit_wrap(hot_data, user_features, item_features)
+        self.cold_model._fit_wrap(log, user_features, item_features)
 
     # pylint: disable=too-many-arguments
     def predict(
         self,
         log: AnyDataFrame,
         k: int,
         users: Optional[Union[AnyDataFrame, Iterable]] = None,
@@ -72,36 +68,36 @@
         :param item_features: item features
             ``[item_id , timestamp]`` + feature columns
         :param filter_seen_items: flag to remove seen items from recommendations based on ``log``.
         :return: recommendation dataframe
             ``[user_id, item_id, relevance]``
         """
         log = convert2spark(log)
-        users = users or log or user_features or self.user_indexer.labels
-        users = self._get_ids(users, "user_id")
+        users = users or log or user_features or self.fit_users
+        users = self._get_ids(users, "user_idx")
         hot_data = min_entries(log, self.threshold)
-        hot_users = hot_data.select("user_id").distinct()
+        hot_users = hot_data.select("user_idx").distinct()
         if not self.can_predict_cold_users:
             hot_users = hot_users.join(self.hot_users)
-        hot_users = hot_users.join(users, on="user_id", how="inner")
+        hot_users = hot_users.join(users, on="user_idx", how="inner")
 
         hot_pred = self._predict_wrap(
             log=hot_data,
             k=k,
             users=hot_users,
             items=items,
             user_features=user_features,
             item_features=item_features,
             filter_seen_items=filter_seen_items,
         )
         if log is not None:
-            cold_data = log.join(self.hot_users, how="anti", on="user_id")
+            cold_data = log.join(self.hot_users, how="anti", on="user_idx")
         else:
             cold_data = None
-        cold_users = users.join(self.hot_users, how="anti", on="user_id")
+        cold_users = users.join(self.hot_users, how="anti", on="user_idx")
         cold_pred = self.cold_model._predict_wrap(
             log=cold_data,
             k=k,
             users=cold_users,
             items=items,
             user_features=user_features,
             item_features=item_features,
@@ -114,15 +110,14 @@
         log: AnyDataFrame,
         k: int,
         users: Optional[Union[AnyDataFrame, Iterable]] = None,
         items: Optional[Union[AnyDataFrame, Iterable]] = None,
         user_features: Optional[AnyDataFrame] = None,
         item_features: Optional[AnyDataFrame] = None,
         filter_seen_items: bool = True,
-        force_reindex: bool = True,
     ) -> DataFrame:
         """
         Train and get recommendations
 
         :param log: historical log of interactions
             ``[user_id, item_id, timestamp, relevance]``
         :param k: length of recommendation lists, should be less that the total number of ``items``
@@ -137,15 +132,15 @@
             ``[user_id , timestamp]`` + feature columns
         :param item_features: item features
             ``[item_id , timestamp]`` + feature columns
         :param filter_seen_items: flag to remove seen items from recommendations based on ``log``.
         :return: recommendation dataframe
             ``[user_id, item_id, relevance]``
         """
-        self.fit(log, user_features, item_features, force_reindex)
+        self.fit(log, user_features, item_features)
         return self.predict(
             log,
             k,
             users,
             items,
             user_features,
             item_features,
```

### Comparing `replay-rec-0.8.0/replay/scenarios/two_stages/feature_processor.py` & `replay-rec-0.9.0/replay/history_based_fp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,471 +1,529 @@
-from typing import Dict, Optional, Tuple, List
+"""
+Contains classes for users' and items' features generation based on interactions history.
+
+``LogStatFeaturesProcessor`` to generate users' and items' features based on log.
+``ConditionalPopularityProcessor`` to generate popularity among users and items
+    conditioned on categorical feature value
+``HistoryBasedFeaturesProcessor`` applies LogStatFeaturesProcessor
+    and ConditionalPopularityProcessor as a pipeline.
+"""
+
+from typing import Dict, Optional, List
 
 import pyspark.sql.functions as sf
+
+from datetime import datetime
 from pyspark.sql import DataFrame
-from pyspark.sql.types import NumericType
+from pyspark.sql.types import TimestampType
 
-from replay.data_preparator import CatFeaturesTransformer
-from replay.session_handler import State
 from replay.utils import join_or_return, ugly_join, unpersist_if_exists
 
 
-class FirstLevelFeaturesProcessor:
-    """Transform features for first level"""
-
-    cat_feat_transformer: Optional[CatFeaturesTransformer]
-    cols_to_one_hot: Optional[List]
-    cols_to_del: Optional[List]
-    all_columns: Optional[List]
-
-    def __init__(self, threshold: Optional[int] = 100):
-        self.threshold = threshold
-        self.fitted = False
-
-    def fit(self, spark_df: Optional[DataFrame]) -> None:
-        """
-        Determine categorical columns for one-hot encoding.
-        Non categorical columns with more values than threshold will be deleted.
-        Saves categories for each column.
-        :param spark_df: input DataFrame
-        """
-        self.cat_feat_transformer = None
-        if spark_df is None:
-            return
-
-        self.all_columns = sorted(spark_df.columns)
-        self.cols_to_del = []
-        idx_cols_set = {"user_idx", "item_idx", "user_id", "item_id"}
-
-        spark_df_non_numeric = spark_df.select(
-            *[
-                col
-                for col in spark_df.columns
-                if (not isinstance(spark_df.schema[col].dataType, NumericType))
-                and (col not in idx_cols_set)
-            ]
-        )
-        if self.threshold is None:
-            self.cols_to_one_hot = spark_df_non_numeric.columns
-        else:
-            counts_pd = (
-                spark_df.agg(
-                    *[
-                        sf.approx_count_distinct(sf.col(c)).alias(c)
-                        for c in spark_df_non_numeric.columns
-                    ]
-                )
-                .toPandas()
-                .T
-            )
-            self.cols_to_one_hot = (
-                counts_pd[counts_pd[0] <= self.threshold]
-            ).index.values
-            self.cols_to_del = [
-                col
-                for col in spark_df_non_numeric.columns
-                if col not in set(self.cols_to_one_hot)
-            ]
-            if self.cols_to_del:
-                State().logger.warning(
-                    "%s columns contain more that threshold unique "
-                    "values and will be deleted",
-                    self.cols_to_del,
-                )
-
-        self.cat_feat_transformer = CatFeaturesTransformer(
-            cat_cols_list=self.cols_to_one_hot, threshold=None
-        )
-        self.cat_feat_transformer.fit(spark_df.drop(*self.cols_to_del))
+class EmptyFeatureProcessor:
+    """Do not perform any transformations on the dataframe"""
 
-    def transform(self, spark_df: Optional[DataFrame]) -> Optional[DataFrame]:
+    def fit(self, log: DataFrame, features: DataFrame) -> None:
         """
-        Transform categorical features.
-        Use one hot encoding for columns with the amount of unique values smaller than threshold and delete other columns.
-        :param spark_df: input DataFrame
-        :return: processed DataFrame
+        :param log: input DataFrame ``[user_idx, item_idx, timestamp, relevance]``
+        :param features: DataFrame with ``user_idx/item_idx`` and feature columns
         """
-        if spark_df is None or self.cat_feat_transformer is None:
-            return None
 
-        if sorted(spark_df.columns) != self.all_columns:
-            raise ValueError(
-                "Columns from fit do not match "
-                "columns in transform. "
-                "Fit columns: %s,"
-                "Transform columns: %s"
-                % (self.all_columns, sorted(spark_df.columns)),
-            )
-
-        return self.cat_feat_transformer.transform(
-            spark_df.drop(*self.cols_to_del)
-        )
-
-    def fit_transform(self, spark_df: DataFrame) -> DataFrame:
+    # pylint: disable=no-self-use
+    def transform(self, log: DataFrame) -> DataFrame:
         """
-        :param spark_df: input DataFrame
-        :return: output DataFrame
+        Return log without any transformations
+        :param log: spark DataFrame
         """
-        self.fit(spark_df)
-        return self.transform(spark_df)
+        return log
 
 
-# pylint: disable=too-many-instance-attributes, too-many-arguments
-class SecondLevelFeaturesProcessor:
+class LogStatFeaturesProcessor(EmptyFeatureProcessor):
     """
-    Calculate extra features for two stages scenario
+    Calculate user and item features based on interactions log:
+        Based on the number of interactions:
+        - log number of interactions (1)
+        - average log number of interactions by users interacted with item and vice versa (2)
+        - difference between number of interactions by user/item (1)
+        and average number of interactions (2)
+
+        Based on timestamp (if present and has a TimestampType):
+        - min and max interaction timestamp for user/item
+        - history length (max - min timestamp)
+        - log number of interactions' days
+        - difference in days between last date in log and last interaction of the user/item
+
+        Based or ratings/relevance:
+        - relevance mean and std
+        - relevance approximate quantiles (0.05, 0.5, 0.95)
+        - abnormality of user's preferences https://hal.inria.fr/hal-01254172/document
     """
 
-    def __init__(
-        self,
-        use_log_features: bool = True,
-        use_conditional_popularity: bool = True,
-        use_cooccurrence: bool = False,
-        user_id: str = "user_idx",
-        item_id: str = "item_idx",
-    ):
-        self.use_log_features = use_log_features
-        self.use_conditional_popularity = use_conditional_popularity
-        self.use_cooccurrence = use_cooccurrence
-        self.user_id = user_id
-        self.item_id = item_id
-        self.fitted: bool = False
-        self.user_log_features_cached: Optional[DataFrame] = None
-        self.item_log_features_cached: Optional[DataFrame] = None
-        self.item_cond_dist_cat_feat_c: Optional[Dict[str, DataFrame]] = None
-        self.user_cond_dist_cat_feat_c: Optional[Dict[str, DataFrame]] = None
+    calc_timestamp_based: bool = False
+    calc_relevance_based: bool = False
+    user_log_features: Optional[DataFrame] = None
+    item_log_features: Optional[DataFrame] = None
 
-    @staticmethod
-    def _create_cols_list(log: DataFrame, agg_col: str = "user_idx") -> List:
+    def _create_log_aggregates(self, agg_col: str = "user_idx") -> List:
         """
         Create features based on relevance type
         (binary or not) and whether timestamp is present.
-        :param log: input DataFrame ``[user_id(x), item_id(x), timestamp, relevance]``
-        :param agg_col: column to create features for, user_id(x) or item_id(x)
+        :param agg_col: column to create features for, user_idx or item_idx
         :return: list of columns to pass into pyspark agg
         """
         prefix = agg_col[:1]
 
         aggregates = [
             sf.log(sf.count(sf.col("relevance"))).alias(
-                "{}_log_ratings_count".format(prefix)
+                f"{prefix}_log_num_interact"
             )
         ]
 
-        if (
-            log.select(sf.countDistinct(sf.col("timestamp"))).collect()[0][0]
-            > 1
-        ):
+        if self.calc_timestamp_based:
             aggregates.extend(
                 [
-                    sf.log(sf.countDistinct(sf.col("timestamp"))).alias(
-                        "{}_log_rating_dates_count".format(prefix)
-                    ),
+                    sf.log(
+                        sf.countDistinct(
+                            sf.date_trunc("dd", sf.col("timestamp"))
+                        )
+                    ).alias(f"{prefix}_log_interact_days_count"),
                     sf.min(sf.col("timestamp")).alias(
-                        "{}_min_rating_date".format(prefix)
+                        f"{prefix}_min_interact_date"
                     ),
                     sf.max(sf.col("timestamp")).alias(
-                        "{}_max_rating_date".format(prefix)
+                        f"{prefix}_max_interact_date"
                     ),
                 ]
             )
 
-        if (
-            log.select(sf.countDistinct(sf.col("relevance"))).collect()[0][0]
-            > 1
-        ):
+        if self.calc_relevance_based:
             aggregates.extend(
                 [
                     (
                         sf.when(
                             sf.stddev(sf.col("relevance")).isNull()
                             | sf.isnan(sf.stddev(sf.col("relevance"))),
                             0,
                         )
                         .otherwise(sf.stddev(sf.col("relevance")))
-                        .alias("{}_std".format(prefix))
-                    ),
-                    sf.mean(sf.col("relevance")).alias(
-                        "{}_mean".format(prefix)
+                        .alias(f"{prefix}_std")
                     ),
+                    sf.mean(sf.col("relevance")).alias(f"{prefix}_mean"),
                 ]
             )
             for percentile in [0.05, 0.5, 0.95]:
                 aggregates.append(
                     sf.expr(
-                        "percentile_approx({}, {})".format(
-                            "relevance", percentile
-                        )
-                    ).alias(
-                        "{}_quantile_{}".format(prefix, str(percentile)[2:])
-                    )
+                        f"percentile_approx(relevance, {percentile})"
+                    ).alias(f"{prefix}_quantile_{str(percentile)[2:]}")
                 )
 
         return aggregates
 
-    def _calc_log_features(
-        self, log: DataFrame
-    ) -> Tuple[DataFrame, DataFrame]:
-        user_aggs = self._create_cols_list(log, agg_col=self.user_id)
-        user_log_features = log.groupBy(self.user_id).agg(*user_aggs)
-
-        item_aggs = self._create_cols_list(log, agg_col=self.item_id)
-        item_log_features = log.groupBy(self.item_id).agg(*item_aggs)
-
-        mean_log_rating_of_user_items = log.join(
-            item_log_features.select(self.item_id, "i_log_ratings_count"),
-            on=self.item_id,
+    @staticmethod
+    def _add_ts_based(
+        features: DataFrame, max_log_date: datetime, prefix: str
+    ) -> DataFrame:
+        """
+        Add history length (max - min timestamp) and difference in days between
+        last date in log and last interaction of the user/item
+
+        :param features: dataframe with calculated log-based features
+        :param max_log_date: max timestamp in log used for features calculation
+        :param prefix: identifier used as a part of column name
+        :return: features dataframe with new timestamp-based columns
+        """
+        return features.withColumn(
+            f"{prefix}_history_length_days",
+            sf.datediff(
+                sf.col(f"{prefix}_max_interact_date"),
+                sf.col(f"{prefix}_min_interact_date"),
+            ),
+        ).withColumn(
+            f"{prefix}_last_interaction_gap_days",
+            sf.datediff(
+                sf.lit(max_log_date), sf.col(f"{prefix}_max_interact_date")
+            ),
+        )
+
+    @staticmethod
+    def _cals_cross_interactions_count(
+        log: DataFrame, features: DataFrame
+    ) -> DataFrame:
+        """
+        Calculate difference between the log number of interactions by the user
+        and average log number of interactions users interacted with the item has.
+
+        :param log: dataframe with calculated log-based features
+        :param features: dataframe with calculated log-based features
+        :return: features dataframe with new columns
+        """
+        if "user_idx" in features.columns:
+            new_feature_entity, calc_by_entity = "item_idx", "user_idx"
+        else:
+            new_feature_entity, calc_by_entity = "user_idx", "item_idx"
+
+        mean_log_num_interact = log.join(
+            features.select(
+                calc_by_entity, f"{calc_by_entity[0]}_log_num_interact"
+            ),
+            on=calc_by_entity,
             how="left",
         )
-        mean_log_rating_of_user_items = mean_log_rating_of_user_items.groupBy(
-            self.user_id
-        ).agg(
-            sf.mean("i_log_ratings_count").alias(
-                "u_mean_log_items_ratings_count"
+        return mean_log_num_interact.groupBy(new_feature_entity).agg(
+            sf.mean(f"{calc_by_entity[0]}_log_num_interact").alias(
+                f"{new_feature_entity[0]}_mean_{calc_by_entity[0]}_log_num_interact"
             )
         )
 
-        user_log_features = ugly_join(
-            left=user_log_features,
-            right=mean_log_rating_of_user_items,
-            on_col_name=self.user_id,
+    @staticmethod
+    def _calc_abnormality(
+        log: DataFrame, item_features: DataFrame
+    ) -> DataFrame:
+        """
+        Calculate  discrepancy between a rating on a resource
+        and the average rating of this resource (Abnormality) and
+        abnormality taking controversy of the item into account (AbnormalityCR).
+        https://hal.inria.fr/hal-01254172/document
+
+        :param log: dataframe with calculated log-based features
+        :param item_features: dataframe with calculated log-based features
+        :return: features dataframe with new columns
+        """
+        # Abnormality
+        abnormality_df = ugly_join(
+            left=log,
+            right=item_features.select("item_idx", "i_mean", "i_std"),
+            on_col_name="item_idx",
             how="left",
         )
-
-        mean_log_rating_of_item_users = log.join(
-            user_log_features.select(self.user_id, "u_log_ratings_count"),
-            on=self.user_id,
-            how="left",
+        abnormality_df = abnormality_df.withColumn(
+            "abnormality", sf.abs(sf.col("relevance") - sf.col("i_mean"))
         )
-        mean_log_rating_of_item_users = mean_log_rating_of_item_users.groupBy(
-            self.item_id
-        ).agg(
-            sf.mean("u_log_ratings_count").alias(
-                "i_mean_log_users_ratings_count"
+
+        abnormality_aggs = [
+            sf.mean(sf.col("abnormality")).alias("abnormality")
+        ]
+
+        # Abnormality CR:
+        max_std = item_features.select(sf.max("i_std")).collect()[0][0]
+        min_std = item_features.select(sf.min("i_std")).collect()[0][0]
+        if max_std - min_std != 0:
+            abnormality_df = abnormality_df.withColumn(
+                "controversy",
+                1
+                - (sf.col("i_std") - sf.lit(min_std))
+                / (sf.lit(max_std - min_std)),
             )
+            abnormality_df = abnormality_df.withColumn(
+                "abnormalityCR",
+                (sf.col("abnormality") * sf.col("controversy")) ** 2,
+            )
+            abnormality_aggs.append(
+                sf.mean(sf.col("abnormalityCR")).alias("abnormalityCR")
+            )
+
+        return abnormality_df.groupBy("user_idx").agg(*abnormality_aggs)
+
+    def fit(
+        self, log: DataFrame, features: Optional[DataFrame] = None
+    ) -> None:
+        """
+        Calculate log-based features for users and items
+
+         :param log: input DataFrame ``[user_idx, item_idx, timestamp, relevance]``
+         :param features: not required
+        """
+        self.calc_timestamp_based = (
+            isinstance(log.schema["timestamp"].dataType, TimestampType)
+        ) & (
+            log.select(sf.countDistinct(sf.col("timestamp"))).collect()[0][0]
+            > 1
+        )
+        self.calc_relevance_based = (
+            log.select(sf.countDistinct(sf.col("relevance"))).collect()[0][0]
+            > 1
         )
 
-        item_log_features = ugly_join(
+        user_log_features = log.groupBy("user_idx").agg(
+            *self._create_log_aggregates(agg_col="user_idx")
+        )
+        item_log_features = log.groupBy("item_idx").agg(
+            *self._create_log_aggregates(agg_col="item_idx")
+        )
+
+        if self.calc_timestamp_based:
+            last_date = log.select(sf.max("timestamp")).collect()[0][0]
+            user_log_features = self._add_ts_based(
+                features=user_log_features, max_log_date=last_date, prefix="u"
+            )
+
+            item_log_features = self._add_ts_based(
+                features=item_log_features, max_log_date=last_date, prefix="i"
+            )
+
+        if self.calc_relevance_based:
+            user_log_features = user_log_features.join(
+                self._calc_abnormality(
+                    log=log, item_features=item_log_features
+                ),
+                on="user_idx",
+                how="left",
+            ).cache()
+
+        self.user_log_features = ugly_join(
+            left=user_log_features,
+            right=self._cals_cross_interactions_count(
+                log=log, features=item_log_features
+            ),
+            on_col_name="user_idx",
+            how="left",
+        ).cache()
+
+        self.item_log_features = ugly_join(
             left=item_log_features,
-            right=mean_log_rating_of_item_users,
-            on_col_name=self.item_id,
+            right=self._cals_cross_interactions_count(
+                log=log, features=user_log_features
+            ),
+            on_col_name="item_idx",
             how="left",
         ).cache()
 
-        if "i_mean" in item_log_features.columns:
-            # Abnormality: https://hal.inria.fr/hal-01254172/document
-            abnormality_df = ugly_join(
-                left=log,
-                right=sf.broadcast(
-                    item_log_features.select(self.item_id, "i_mean", "i_std")
-                ),
-                on_col_name=self.item_id,
+    def transform(self, log: DataFrame) -> DataFrame:
+        """
+        Add log-based features for users and items
+
+        :param log: input DataFrame with
+            ``[user_idx, item_idx, <features columns>]`` columns
+        :return: log with log-based feature columns
+        """
+        joined = (
+            log.join(
+                self.user_log_features,
+                on="user_idx",
                 how="left",
             )
-            abnormality_df = abnormality_df.withColumn(
-                "abnormality", sf.abs(sf.col("relevance") - sf.col("i_mean"))
+            .join(
+                self.item_log_features,
+                on="item_idx",
+                how="left",
+            )
+            .withColumn(
+                "na_u_log_features",
+                sf.when(sf.col("u_log_num_interact").isNull(), 1.0).otherwise(
+                    0.0
+                ),
+            )
+            .withColumn(
+                "na_i_log_features",
+                sf.when(sf.col("i_log_num_interact").isNull(), 1.0).otherwise(
+                    0.0
+                ),
+            )
+            # TO DO std и date diff заменяем на inf, date features - будут ли работать корректно?
+            # если не заменять, будет ли работать корректно?
+            .fillna(
+                {
+                    col_name: 0
+                    for col_name in self.user_log_features.columns
+                    + self.item_log_features.columns
+                }
             )
+        )
 
-            abnormality_aggs = [
-                sf.mean(sf.col("abnormality")).alias("abnormality")
-            ]
-
-            # Abnormality CR: https://hal.inria.fr/hal-01254172/document
-            max_std = item_log_features.select(sf.max("i_std")).collect()[0][0]
-            min_std = item_log_features.select(sf.min("i_std")).collect()[0][0]
-            if max_std - min_std != 0:
-                abnormality_df = abnormality_df.withColumn(
-                    "controversy",
-                    1
-                    - (sf.col("i_std") - sf.lit(min_std))
-                    / (sf.lit(max_std - min_std)),
-                )
-                abnormality_df = abnormality_df.withColumn(
-                    "abnormalityCR",
-                    (sf.col("abnormality") * sf.col("controversy")) ** 2,
-                )
-                abnormality_aggs.append(
-                    sf.mean(sf.col("abnormalityCR")).alias("abnormalityCR")
-                )
+        joined = joined.withColumn(
+            "u_i_log_num_interact_diff",
+            sf.col("u_log_num_interact") - sf.col("i_mean_u_log_num_interact"),
+        ).withColumn(
+            "i_u_log_num_interact_diff",
+            sf.col("i_log_num_interact") - sf.col("u_mean_i_log_num_interact"),
+        )
 
-            abnormality_res = abnormality_df.groupBy(self.user_id).agg(
-                *abnormality_aggs
-            )
-            user_log_features = user_log_features.join(
-                sf.broadcast(abnormality_res), on=self.user_id, how="left"
-            ).cache()
+        return joined
+
+    def __del__(self):
+        unpersist_if_exists(self.user_log_features)
+        unpersist_if_exists(self.item_log_features)
+
+
+class ConditionalPopularityProcessor(EmptyFeatureProcessor):
+    """
+    Calculate popularity based on user or item categorical features
+    (for example movie popularity among users of the same age group).
+    If user features are provided, item features will be generated and vice versa.
+    """
 
-        return user_log_features, item_log_features
+    conditional_pop_dict: Optional[Dict[str, DataFrame]]
+    entity_name: str
 
-    def _add_cond_distr_feat(
-        self, cat_cols: List[str], log: DataFrame, features_df: DataFrame
-    ) -> Dict[str, DataFrame]:
-        """
-        Calculate item popularity based on user or item categorical features.
-        For example movie popularity among users of the same age.
-        If user features are provided, result will contain item features and vice versa.
-
-        :param cat_cols: list of categorical columns
-        :param log: input DataFrame ``[user_id(x), item_id(x), timestamp, relevance]``
-        :param features_df: DataFrame with user or item features
-        :return: dictionary "categorical feature name - DataFrame with popularity by id and category values"
+    def __init__(
+        self,
+        cat_features_list: List,
+    ):
         """
-        if self.item_id in features_df.columns:
-            join_col, agg_col = self.item_id, self.user_id
-        else:
-            join_col, agg_col = self.user_id, self.item_id
+        :param cat_features_list: List of columns with categorical features to use
+            for conditional popularity calculation
+        """
+        self.cat_features_list = cat_features_list
 
-        conditional_dist = dict()
-        log_with_features = log.join(features_df, on=join_col, how="left")
-        count_by_agg_col_name = "count_by_{}".format(agg_col)
-        count_by_agg_col = log_with_features.groupBy(agg_col).agg(
-            sf.count("relevance").alias(count_by_agg_col_name)
-        )
-        for cat_col in cat_cols:
-            col_name = "{}_pop_by_{}".format(agg_col[:4], cat_col)
-            intermediate_df = log_with_features.groupBy(agg_col, cat_col).agg(
-                sf.count("relevance").alias(col_name)
+    def fit(self, log: DataFrame, features: DataFrame) -> None:
+        """
+        Calculate conditional popularity for id and categorical features
+        defined in `cat_features_list`
+
+        :param log: input DataFrame ``[user_idx, item_idx, timestamp, relevance]``
+        :param features: DataFrame with ``user_idx/item_idx`` and feature columns
+        """
+        if len(
+            set(self.cat_features_list).intersection(features.columns)
+        ) != len(self.cat_features_list):
+            raise ValueError(
+                f"Columns {set(self.cat_features_list).difference(features.columns)} "
+                f"defined in `cat_features_list` are absent in features. "
+                f"features columns are: {features.columns}."
             )
+
+        join_col, self.entity_name = (
+            ("item_idx", "user_idx")
+            if "item_idx" in features.columns
+            else ("user_idx", "item_idx")
+        )
+
+        self.conditional_pop_dict = {}
+        log_with_features = log.join(features, on=join_col, how="left")
+        count_by_entity_col_name = f"count_by_{self.entity_name}"
+
+        count_by_entity_col = log_with_features.groupBy(self.entity_name).agg(
+            sf.count("relevance").alias(count_by_entity_col_name)
+        )
+
+        for cat_col in self.cat_features_list:
+            col_name = f"{self.entity_name[0]}_pop_by_{cat_col}"
+            intermediate_df = log_with_features.groupBy(
+                self.entity_name, cat_col
+            ).agg(sf.count("relevance").alias(col_name))
             intermediate_df = intermediate_df.join(
-                sf.broadcast(count_by_agg_col), on=agg_col, how="left"
+                sf.broadcast(count_by_entity_col),
+                on=self.entity_name,
+                how="left",
+            )
+            self.conditional_pop_dict[cat_col] = intermediate_df.withColumn(
+                col_name, sf.col(col_name) / sf.col(count_by_entity_col_name)
+            ).drop(count_by_entity_col_name)
+            self.conditional_pop_dict[cat_col].cache()
+
+    def transform(self, log: DataFrame) -> DataFrame:
+        """
+        Add conditional popularity features
+
+        :param log: input DataFrame with
+            ``[user_idx, item_idx, <features columns>]`` columns
+        :return: log with conditional popularity feature columns
+        """
+
+        joined = log
+        for (
+            key,
+            value,
+        ) in self.conditional_pop_dict.items():
+            joined = join_or_return(
+                joined,
+                sf.broadcast(value),
+                on=[self.entity_name, key],
+                how="left",
+            ).withColumn(
+                f"na_{self.entity_name[0]}_pop_by_{key}",
+                sf.when(
+                    sf.col(f"{self.entity_name[0]}_pop_by_{key}").isNull(),
+                    True,
+                ).otherwise(False),
             )
-            conditional_dist[cat_col] = intermediate_df.withColumn(
-                col_name, sf.col(col_name) / sf.col(count_by_agg_col_name)
-            ).drop(count_by_agg_col_name)
-            conditional_dist[cat_col].cache()
+            joined = joined.fillna({f"{self.entity_name[0]}_pop_by_{key}": 0})
+        return joined
+
+    def __del__(self):
+        for df in self.conditional_pop_dict.values():
+            unpersist_if_exists(df)
+
+
+# pylint: disable=too-many-instance-attributes, too-many-arguments
+class HistoryBasedFeaturesProcessor:
+    """
+    Calculate user and item features based on interactions history (log).
+    calculated features includes numbers of interactions, rating and timestamp distribution features
+    and conditional popularity for pairs `user_idx/item_idx - categorical feature`.
+
+    See LogStatFeaturesProcessor and ConditionalPopularityProcessor documentation
+    for detailed description of generated features.
+    """
 
-        return conditional_dist
+    log_proc = EmptyFeatureProcessor()
+    user_cond_pop_proc = EmptyFeatureProcessor()
+    item_cond_pop_proc = EmptyFeatureProcessor()
+
+    def __init__(
+        self,
+        use_log_features: bool = True,
+        use_conditional_popularity: bool = True,
+        user_cat_features_list: Optional[List] = None,
+        item_cat_features_list: Optional[List] = None,
+    ):
+        """
+        :param use_log_features: if add statistical log-based features
+            generated by LogStatFeaturesProcessor
+        :param use_conditional_popularity: if add conditional popularity
+            features generated by ConditionalPopularityProcessor
+        :param user_cat_features_list: list of user categorical features
+            used to calculate item conditional popularity features
+        :param item_cat_features_list: list of item categorical features
+            used to calculate user conditional popularity features
+        """
+        if use_log_features:
+            self.log_processor = LogStatFeaturesProcessor()
+        if use_conditional_popularity and user_cat_features_list:
+            if user_cat_features_list:
+                self.user_cond_pop_proc = ConditionalPopularityProcessor(
+                    cat_features_list=user_cat_features_list
+                )
+            if item_cat_features_list:
+                self.item_cond_pop_proc = ConditionalPopularityProcessor(
+                    cat_features_list=item_cat_features_list
+                )
+        self.fitted: bool = False
 
     def fit(
         self,
         log: DataFrame,
         user_features: Optional[DataFrame] = None,
         item_features: Optional[DataFrame] = None,
-        user_cat_features_list: Optional[List] = None,
-        item_cat_features_list: Optional[List] = None,
     ) -> None:
         """
-        Calculate features for users and items, and popularity based on categorical features.
+        Calculate log and conditional popularity features.
 
-        :param log: input DataFrame ``[user_id(x), item_id(x), timestamp, relevance]``
-        :param user_features: DataFrame with ``user_id(x)`` and feature columns
-        :param item_features: DataFrame with ``item_id(x)`` and feature columns
-        :param user_cat_features_list: list of user categorical features used to calculate item popularity features,
-            such as movie popularity among certain age group
-        :param item_cat_features_list: list of item categorical features
+        :param log: input DataFrame ``[user_idx, item_idx, timestamp, relevance]``
+        :param user_features: DataFrame with ``user_idx`` and feature columns
+        :param item_features: DataFrame with ``item_idx`` and feature columns
         """
         log = log.cache()
-        if self.use_cooccurrence:
-            raise NotImplementedError("co-occurrence will be implemented soon")
-
-        if self.use_log_features:
-            (
-                self.user_log_features_cached,
-                self.item_log_features_cached,
-            ) = self._calc_log_features(log)
-
-        if self.use_conditional_popularity:
-            if (
-                user_features is not None
-                and user_cat_features_list is not None
-            ):
-                self.item_cond_dist_cat_feat_c = self._add_cond_distr_feat(
-                    user_cat_features_list, log, user_features
-                )
-
-            if (
-                item_features is not None
-                and item_cat_features_list is not None
-            ):
-                self.user_cond_dist_cat_feat_c = self._add_cond_distr_feat(
-                    item_cat_features_list, log, item_features
-                )
-
+        self.log_processor.fit(log=log)
+        self.user_cond_pop_proc.fit(log=log, features=user_features)
+        self.item_cond_pop_proc.fit(log=log, features=item_features)
         self.fitted = True
         log.unpersist()
 
     def transform(
         self,
         log: DataFrame,
     ):
         """
         Add features
-        :param log: input DataFrame ``[user_id(x), item_id(x), ...]``
+        :param log: input DataFrame with
+            ``[user_idx, item_idx, <features columns>]`` columns
         :return: augmented DataFrame
         """
         if not self.fitted:
             raise AttributeError("Call fit before running transform")
-        joined = log
-
-        if self.use_log_features:
-            joined = (
-                joined.join(
-                    sf.broadcast(self.user_log_features_cached),
-                    on=self.user_id,
-                    how="left",
-                )
-                .join(
-                    sf.broadcast(self.item_log_features_cached),
-                    on=self.item_id,
-                    how="left",
-                )
-                .fillna(
-                    {
-                        col_name: 0
-                        for col_name in self.user_log_features_cached.columns
-                        + self.item_log_features_cached.columns
-                    }
-                )
-            )
+        joined = self.log_processor.transform(log)
+        joined = self.user_cond_pop_proc.transform(joined)
+        joined = self.item_cond_pop_proc.transform(joined)
 
-            joined = joined.withColumn(
-                "u_log_ratings_count_diff",
-                sf.col("u_log_ratings_count")
-                - sf.col("i_mean_log_users_ratings_count"),
-            ).withColumn(
-                "i_log_ratings_count_diff",
-                sf.col("i_log_ratings_count")
-                - sf.col("u_mean_log_items_ratings_count"),
-            )
-
-        if self.use_conditional_popularity:
-            if self.user_cond_dist_cat_feat_c is not None:
-                for (
-                    key,
-                    value,
-                ) in self.user_cond_dist_cat_feat_c.items():
-                    joined = join_or_return(
-                        joined,
-                        sf.broadcast(value),
-                        on=[self.user_id, key],
-                        how="left",
-                    )
-                    joined = joined.fillna({"user_pop_by_" + key: 0})
-
-            if self.item_cond_dist_cat_feat_c is not None:
-                for (
-                    key,
-                    value,
-                ) in self.item_cond_dist_cat_feat_c.items():
-                    joined = join_or_return(
-                        joined,
-                        sf.broadcast(value),
-                        on=[self.item_id, key],
-                        how="left",
-                    )
-                    joined = joined.fillna({"item_pop_by_" + key: 0})
         return joined
-
-    def __del__(self):
-        for log_feature in [
-            self.user_log_features_cached,
-            self.item_log_features_cached,
-        ]:
-            unpersist_if_exists(log_feature)
-
-        for conditional_feature in [
-            self.user_cond_dist_cat_feat_c,
-            self.item_cond_dist_cat_feat_c,
-        ]:
-            if conditional_feature is not None:
-                for value in conditional_feature.values():
-                    unpersist_if_exists(value)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `replay-rec-0.8.0/replay/scenarios/two_stages/two_stages_scenario.py` & `replay-rec-0.9.0/replay/scenarios/two_stages/two_stages_scenario.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 # pylint: disable=too-many-lines
 from collections.abc import Iterable
 from typing import Dict, Optional, Tuple, List, Union, Any
 
 import pyspark.sql.functions as sf
 from pyspark.sql import DataFrame
 
-from lightautoml.automl.presets.tabular_presets import TabularAutoML
-from lightautoml.tasks import Task
-
 from replay.constants import AnyDataFrame
+from replay.data_preparator import ToNumericFeatureTransformer
+from replay.history_based_fp import HistoryBasedFeaturesProcessor
 from replay.metrics import Metric, Precision
 from replay.models import ALSWrap, RandomRec, PopRec
 from replay.models.base_rec import BaseRecommender, HybridRecommender
-from replay.scenarios.two_stages.feature_processor import (
-    SecondLevelFeaturesProcessor,
-    FirstLevelFeaturesProcessor,
-)
+from replay.scenarios.two_stages.reranker import LamaWrap
 
 from replay.session_handler import State
 from replay.splitters import Splitter, UserSplitter
 from replay.utils import (
     array_mult,
     cache_if_exists,
-    convert2spark,
     fallback,
     get_log_info,
     get_top_k_recs,
     horizontal_explode,
     join_or_return,
     ugly_join,
     unpersist_if_exists,
@@ -41,48 +36,41 @@
     item_features: Optional[DataFrame] = None,
     add_factors_mult: bool = True,
     prefix: str = "",
 ) -> DataFrame:
     """
     Get user and item embeddings from replay model.
     Can also compute elementwise multiplication between them with ``add_factors_mult`` parameter.
-    Zero verctors are returned if a model does not have embeddings for specific users/items.
+    Zero vectors are returned if a model does not have embeddings for specific users/items.
 
     :param model: trained model
     :param pairs: user-item pairs to get vectors for `[user_id/user_idx, item_id/item_id]`
     :param user_features: user features `[user_id/user_idx, feature_1, ....]`
     :param item_features: item features `[item_id/item_idx, feature_1, ....]`
     :param add_factors_mult: flag to add elementwise multiplication
     :param prefix: name to add to the columns
     :return: DataFrame
     """
-    if "user_id" in pairs.columns:
-        func_name = "_get_features_wrap"
-        id_type = "id"
-    else:
-        func_name = "_get_features"
-        id_type = "idx"
-
-    users = pairs.select("user_{}".format(id_type)).distinct()
-    items = pairs.select("item_{}".format(id_type)).distinct()
-    user_factors, user_vector_len = getattr(model, func_name)(
+    users = pairs.select("user_idx").distinct()
+    items = pairs.select("item_idx").distinct()
+    user_factors, user_vector_len = model._get_features_wrap(
         users, user_features
     )
-    item_factors, item_vector_len = getattr(model, func_name)(
+    item_factors, item_vector_len = model._get_features_wrap(
         items, item_features
     )
 
     pairs_with_features = join_or_return(
-        pairs, user_factors, how="left", on="user_{}".format(id_type)
+        pairs, user_factors, how="left", on="user_idx"
     )
     pairs_with_features = join_or_return(
         pairs_with_features,
         item_factors,
         how="left",
-        on="item_{}".format(id_type),
+        on="item_idx",
     )
 
     factors_to_explode = []
     if user_factors is not None:
         pairs_with_features = pairs_with_features.withColumn(
             "user_factors",
             sf.coalesce(
@@ -101,16 +89,16 @@
             ),
         )
         factors_to_explode.append(("item_factors", "if"))
 
     if model.__str__() == "LightFMWrap":
         pairs_with_features = (
             pairs_with_features.fillna({"user_bias": 0, "item_bias": 0})
-            .withColumnRenamed("user_bias", "{}_user_bias".format(prefix))
-            .withColumnRenamed("item_bias", "{}_item_bias".format(prefix))
+            .withColumnRenamed("user_bias", f"{prefix}_user_bias")
+            .withColumnRenamed("item_bias", f"{prefix}_item_bias")
         )
 
     if (
         add_factors_mult
         and user_factors is not None
         and item_factors is not None
     ):
@@ -123,17 +111,15 @@
     for col_name, feature_prefix in factors_to_explode:
         col_set = set(pairs_with_features.columns)
         col_set.remove(col_name)
         pairs_with_features = horizontal_explode(
             data_frame=pairs_with_features,
             column_to_explode=col_name,
             other_columns=[sf.col(column) for column in sorted(list(col_set))],
-            prefix="{general_prefix}_{feature_prefix}".format(
-                general_prefix=prefix, feature_prefix=feature_prefix
-            ),
+            prefix=f"{prefix}_{feature_prefix}",
         )
 
     return pairs_with_features
 
 
 # pylint: disable=too-many-instance-attributes
 class TwoStagesScenario(HybridRecommender):
@@ -184,15 +170,15 @@
         second_model_params: Optional[Union[Dict, str]] = None,
         second_model_config_path: Optional[str] = None,
         num_negatives: int = 100,
         negatives_type: str = "first_level",
         use_generated_features: bool = False,
         user_cat_features_list: Optional[List] = None,
         item_cat_features_list: Optional[List] = None,
-        custom_features_processor: SecondLevelFeaturesProcessor = None,
+        custom_features_processor: HistoryBasedFeaturesProcessor = None,
         seed: int = 123,
     ) -> None:
         """
         :param train_splitter: splitter to get ``first_level_train`` and ``second_level_train``.
             Default is random 50% split.
         :param first_level_models: model or a list of models
         :param fallback_model: model used to fill missing recommendations at first level models
@@ -215,79 +201,62 @@
 
         self.first_level_models = (
             first_level_models
             if isinstance(first_level_models, Iterable)
             else [first_level_models]
         )
 
-        self.first_level_item_indexer_len = 0
-        self.first_level_user_indexer_len = 0
+        self.first_level_item_len = 0
+        self.first_level_user_len = 0
 
         self.random_model = RandomRec(seed=seed)
         self.fallback_model = fallback_model
         self.first_level_user_features_transformer = (
-            FirstLevelFeaturesProcessor()
+            ToNumericFeatureTransformer()
         )
         self.first_level_item_features_transformer = (
-            FirstLevelFeaturesProcessor()
+            ToNumericFeatureTransformer()
         )
 
         if isinstance(use_first_level_models_feat, bool):
             self.use_first_level_models_feat = [
                 use_first_level_models_feat
             ] * len(self.first_level_models)
         else:
             if len(self.first_level_models) != len(
                 use_first_level_models_feat
             ):
                 raise ValueError(
-                    "For each model from first_level_models specify "
-                    "flag to use first level features."
-                    "Length of first_level_models is {}, "
-                    "Length of use_first_level_models_feat is {}".format(
-                        len(first_level_models),
-                        len(use_first_level_models_feat),
-                    )
+                    f"For each model from first_level_models specify "
+                    f"flag to use first level features."
+                    f"Length of first_level_models is {len(first_level_models)}, "
+                    f"Length of use_first_level_models_feat is {len(use_first_level_models_feat)}"
                 )
 
             self.use_first_level_models_feat = use_first_level_models_feat
 
-        if (
-            second_model_config_path is not None
-            or second_model_params is not None
-        ):
-            second_model_params = (
-                dict() if second_model_params is None else second_model_params
-            )
-            self.second_stage_model = TabularAutoML(
-                config_path=second_model_config_path,
-                task=Task("binary"),
-                **second_model_params
-            )
-        else:
-            # CHECK! ask about parameters
-            self.second_stage_model = TabularAutoML(
-                task=Task("binary"),
-                reader_params={"cv": 5, "random_state": seed},
-            )
+        self.second_stage_model = LamaWrap(
+            params=second_model_params, config_path=second_model_config_path
+        )
 
         self.num_negatives = num_negatives
         if negatives_type not in ["random", "first_level"]:
             raise ValueError(
-                "Invalid negatives_type value: {}. Use 'random' or 'first_level'"
+                f"Invalid negatives_type value: {negatives_type}. Use 'random' or 'first_level'"
             )
         self.negatives_type = negatives_type
 
         self.use_generated_features = use_generated_features
-        self.user_cat_features_list = user_cat_features_list
-        self.item_cat_features_list = item_cat_features_list
         self.features_processor = (
             custom_features_processor
             if custom_features_processor
-            else SecondLevelFeaturesProcessor()
+            else HistoryBasedFeaturesProcessor(
+                user_cat_features_list=user_cat_features_list,
+                item_cat_features_list=item_cat_features_list,
+            )
         )
         self.seed = seed
 
     # pylint: disable=too-many-locals
     def _add_features_for_second_level(
         self,
         log_to_add_features: DataFrame,
@@ -321,30 +290,30 @@
         for idx, model in enumerate(self.first_level_models):
             current_pred = self._predict_pairs_with_first_level_model(
                 model=model,
                 log=log_for_first_level_models,
                 pairs=pairs,
                 user_features=first_level_user_features_cached,
                 item_features=first_level_item_features_cached,
-            ).withColumnRenamed("relevance", "rel_{}_{}".format(idx, model))
+            ).withColumnRenamed("relevance", f"rel_{idx}_{model}")
             full_second_level_train = full_second_level_train.join(
                 sf.broadcast(current_pred),
                 on=["user_idx", "item_idx"],
                 how="left",
             )
 
             if self.use_first_level_models_feat[idx]:
                 features = get_first_level_model_features(
                     model=model,
                     pairs=full_second_level_train.select(
                         "user_idx", "item_idx"
                     ),
                     user_features=first_level_user_features_cached,
                     item_features=first_level_item_features_cached,
-                    prefix="m_{}".format(idx),
+                    prefix=f"m_{idx}",
                 )
                 full_second_level_train = ugly_join(
                     left=full_second_level_train,
                     right=features,
                     on_col_name=["user_idx", "item_idx"],
                     how="left",
                 )
@@ -360,25 +329,26 @@
         full_second_level_train = join_or_return(
             full_second_level_train_cached,
             user_features,
             on="user_idx",
             how="left",
         )
         full_second_level_train = join_or_return(
-            full_second_level_train, item_features, on="item_idx", how="left",
+            full_second_level_train,
+            item_features,
+            on="item_idx",
+            how="left",
         )
 
         if self.use_generated_features:
             if not self.features_processor.fitted:
                 self.features_processor.fit(
                     log=log_for_first_level_models,
                     user_features=user_features,
                     item_features=item_features,
-                    user_cat_features_list=self.user_cat_features_list,
-                    item_cat_features_list=self.item_cat_features_list,
                 )
             self.logger.info("Adding generated features")
             full_second_level_train = self.features_processor.transform(
                 log=full_second_level_train
             )
 
         self.logger.info(
@@ -396,26 +366,14 @@
             "first_level_train info: %s", get_log_info(first_level_train)
         )
         State().logger.debug(
             "second_level_train info: %s", get_log_info(second_level_train)
         )
         return first_level_train, second_level_train
 
-    def _fit_wrap(
-        self,
-        log: AnyDataFrame,
-        user_features: Optional[AnyDataFrame] = None,
-        item_features: Optional[AnyDataFrame] = None,
-        force_reindex: bool = True,
-    ) -> None:
-        log, user_features, item_features = [
-            convert2spark(df) for df in [log, user_features, item_features]
-        ]
-        self._fit(log, user_features, item_features)
-
     @staticmethod
     def _filter_or_return(dataframe, condition):
         if dataframe is None:
             return dataframe
         return dataframe.filter(condition)
 
     def _predict_with_first_level_model(
@@ -432,61 +390,61 @@
         """
         Filter users and items using can_predict_cold_items and can_predict_cold_users, and predict
         """
         if not model.can_predict_cold_items:
             log, items, item_features = [
                 self._filter_or_return(
                     dataframe=df,
-                    condition=sf.col("item_idx")
-                    < self.first_level_item_indexer_len,
+                    condition=sf.col("item_idx") < self.first_level_item_len,
                 )
                 for df in [log, items, item_features]
             ]
         if not model.can_predict_cold_users:
             log, users, user_features = [
                 self._filter_or_return(
                     dataframe=df,
-                    condition=sf.col("user_idx")
-                    < self.first_level_user_indexer_len,
+                    condition=sf.col("user_idx") < self.first_level_user_len,
                 )
                 for df in [log, users, user_features]
             ]
 
-        max_positives_to_filter = min(
-            [
-                log_to_filter.groupBy("user_idx")
+        log_to_filter_cached = ugly_join(
+            left=log_to_filter,
+            right=users,
+            on_col_name="user_idx",
+        ).cache()
+        max_positives_to_filter = 0
+
+        if log_to_filter_cached.count() > 0:
+            max_positives_to_filter = (
+                log_to_filter_cached.groupBy("user_idx")
                 .agg(sf.count("item_idx").alias("num_positives"))
                 .select(sf.max("num_positives"))
-                .collect()[0][0],
-                log.select("item_idx").distinct().count() - k,
-                items.select("item_idx").distinct().count() - k,
-            ]
-        )
+                .collect()[0][0]
+            )
 
         pred = model._predict(
             log,
             k=k + max_positives_to_filter,
             users=users,
             items=items,
             user_features=user_features,
             item_features=item_features,
             filter_seen_items=False,
         )
 
-        # TO DO: это неоптимально, можно попробовать для каждого пользователя определять
-        # свое k до фильтрации просмотренных,
-        # фильтровать top-k, а потом исключать просмотренных,
-        # чтобы сделать anti-join не таким объемным
         pred = pred.join(
-            log_to_filter.select("user_idx", "item_idx"),
+            log_to_filter_cached.select("user_idx", "item_idx"),
             on=["user_idx", "item_idx"],
             how="anti",
         ).drop("user", "item")
 
-        return get_top_k_recs(pred, k, id_type="idx")
+        log_to_filter_cached.unpersist()
+
+        return get_top_k_recs(pred, k)
 
     def _predict_pairs_with_first_level_model(
         self,
         model: BaseRecommender,
         log: DataFrame,
         pairs: DataFrame,
         user_features: DataFrame,
@@ -495,25 +453,23 @@
         """
         Get relevance for selected user-item pairs.
         """
         if not model.can_predict_cold_items:
             log, pairs, item_features = [
                 self._filter_or_return(
                     dataframe=df,
-                    condition=sf.col("item_idx")
-                    < self.first_level_item_indexer_len,
+                    condition=sf.col("item_idx") < self.first_level_item_len,
                 )
                 for df in [log, pairs, item_features]
             ]
         if not model.can_predict_cold_users:
             log, pairs, user_features = [
                 self._filter_or_return(
                     dataframe=df,
-                    condition=sf.col("user_idx")
-                    < self.first_level_user_indexer_len,
+                    condition=sf.col("user_idx") < self.first_level_user_len,
                 )
                 for df in [log, pairs, user_features]
             ]
 
         return model._predict_pairs(
             pairs=pairs,
             log=log,
@@ -538,62 +494,61 @@
         predictions.
         """
         passed_arguments = locals()
         passed_arguments.pop("self")
         candidates = self._predict_with_first_level_model(**passed_arguments)
 
         if self.fallback_model is not None:
+            passed_arguments.pop("model")
             fallback_candidates = self._predict_with_first_level_model(
-                **passed_arguments
+                model=self.fallback_model, **passed_arguments
             )
 
             candidates = fallback(
                 base=candidates,
                 fill=fallback_candidates,
                 k=self.num_negatives,
-                id_type="idx",
             )
         return candidates
 
     # pylint: disable=too-many-locals,too-many-statements
     def _fit(
         self,
         log: DataFrame,
         user_features: Optional[DataFrame] = None,
         item_features: Optional[DataFrame] = None,
     ) -> None:
 
         self.cached_list = []
 
         self.logger.info("Data split")
-        first_level_train, second_level_train = self._split_data(log)
-        self.logger.info("Create indexers")
-        self._create_indexers(first_level_train, None, None)
-
-        self.first_level_item_indexer_len = len(self.item_indexer.labels)
-        self.first_level_user_indexer_len = len(self.user_indexer.labels)
-
-        for model in self.first_level_models + [self.fallback_model]:
-            model.user_indexer = self.user_indexer.copy()
-            model.item_indexer = self.item_indexer.copy()
-            model.inv_user_indexer = self.inv_user_indexer.copy()
-            model.inv_item_indexer = self.inv_item_indexer.copy()
-
-        log, first_level_train, second_level_train = [
-            self._convert_index(df).cache()
-            for df in [log, first_level_train, second_level_train]
-        ]
-        self.cached_list.extend([log, first_level_train, second_level_train])
+        first_level_train, second_level_positive = self._split_data(log)
+        # second_level_positive = second_level_positive
+        # .join(first_level_train.select("user_idx"), on="user_idx", how="left")
+
+        self.first_level_item_len = (
+            first_level_train.select("item_idx").distinct().count()
+        )
+        self.first_level_user_len = (
+            first_level_train.select("user_idx").distinct().count()
+        )
+
+        log.cache()
+        first_level_train.cache()
+        second_level_positive.cache()
+        self.cached_list.extend(
+            [log, first_level_train, second_level_positive]
+        )
 
         if user_features is not None:
-            user_features = self._convert_index(user_features).cache()
+            user_features.cache()
             self.cached_list.append(user_features)
 
         if item_features is not None:
-            item_features = self._convert_index(item_features).cache()
+            item_features.cache()
             self.cached_list.append(item_features)
 
         self.first_level_item_features_transformer.fit(item_features)
         self.first_level_user_features_transformer.fit(user_features)
 
         first_level_item_features = cache_if_exists(
             self.first_level_item_features_transformer.transform(item_features)
@@ -603,103 +558,87 @@
         )
 
         for base_model in [
             *self.first_level_models,
             self.random_model,
             self.fallback_model,
         ]:
-            base_model._fit(
+            base_model._fit_wrap(
                 log=first_level_train,
                 user_features=first_level_user_features.filter(
-                    sf.col("user_idx") < self.first_level_user_indexer_len
+                    sf.col("user_idx") < self.first_level_user_len
                 ),
                 item_features=first_level_item_features.filter(
-                    sf.col("item_idx") < self.first_level_item_indexer_len
+                    sf.col("item_idx") < self.first_level_item_len
                 ),
             )
 
         self.logger.info("Generate negative examples")
         negatives_source = (
             self.first_level_models[0]
             if self.negatives_type == "first_level"
             else self.random_model
         )
 
-        negatives = self._get_first_level_candidates(
+        first_level_candidates = self._get_first_level_candidates(
             model=negatives_source,
             log=first_level_train,
             k=self.num_negatives,
             users=log.select("user_idx").distinct(),
             items=log.select("item_idx").distinct(),
             user_features=first_level_user_features,
             item_features=first_level_item_features,
-            log_to_filter=log,
-        ).withColumn("relevance", sf.lit(0))
+            log_to_filter=first_level_train,
+        ).select("user_idx", "item_idx")
 
         unpersist_if_exists(first_level_user_features)
         unpersist_if_exists(first_level_item_features)
 
         self.logger.info("Crate train dataset for second level")
-        full_second_level_train = (
-            second_level_train.select("user_idx", "item_idx", "relevance")
-            .withColumn("relevance", sf.lit(1))
-            .unionByName(negatives)
-            .cache()
-        )
-
-        self.cached_list.append(full_second_level_train)
-
-        dataset_class_sizes = (
-            full_second_level_train.groupBy("relevance")
-            .agg(sf.count(sf.col("relevance")).alias("count_for_class"))
-            .toPandas()
-        )
-
-        self.logger.info("В train для модели второго уровня:")
-        for row_num in range(2):
-            self.logger.info(
-                "\t%s объектов класса %s",
-                dataset_class_sizes.loc[row_num, "count_for_class"],
-                dataset_class_sizes.loc[row_num, "relevance"],
-            )
+
+        second_level_train = (
+            first_level_candidates.join(
+                second_level_positive.select(
+                    "user_idx", "item_idx"
+                ).withColumn("target", sf.lit(1.0)),
+                on=["user_idx", "item_idx"],
+                how="left",
+            ).fillna(0.0, subset="target")
+        ).cache()
+
+        self.cached_list.append(second_level_train)
+
+        self.logger.info(
+            "Distribution of classes in second-level train dataset:/n %s",
+            (
+                second_level_train.groupBy("target")
+                .agg(sf.count(sf.col("target")).alias("count_for_class"))
+                .take(2)
+            ),
+        )
 
         self.features_processor.fit(
             log=first_level_train,
             user_features=user_features,
             item_features=item_features,
-            user_cat_features_list=self.user_cat_features_list,
-            item_cat_features_list=self.item_cat_features_list,
         )
 
-        self.logger.info("Дополнение train модели второго уровня признаками")
-        full_second_level_train = self._add_features_for_second_level(
-            log_to_add_features=full_second_level_train,
+        self.logger.info("Adding features to second-level train dataset")
+        second_level_train_to_convert = self._add_features_for_second_level(
+            log_to_add_features=second_level_train,
             log_for_first_level_models=first_level_train,
             user_features=user_features,
             item_features=item_features,
-        )
+        ).cache()
 
-        full_second_level_train = full_second_level_train.drop(
-            "user_idx", "item_idx"
-        )
-        self.logger.info("Converting to pandas")
-        full_second_level_train.cache()
-        full_second_level_train_pd = full_second_level_train.toPandas()
-        full_second_level_train.unpersist()
+        self.cached_list.append(second_level_train_to_convert)
+        self.second_stage_model.fit(second_level_train_to_convert)
         for dataframe in self.cached_list:
             unpersist_if_exists(dataframe)
 
-        self.second_stage_model.fit_predict(
-            full_second_level_train_pd, roles={"target": "relevance"}
-        )
-
-        # TO DO: узнать у коллег, как достать какие-нибудь
-        # понятные важности признаков (не от одной модели)
-        self.logger.info("Second level is trained")
-
     # pylint: disable=too-many-arguments
     def _predict(
         self,
         log: DataFrame,
         k: int,
         users: DataFrame,
         items: DataFrame,
@@ -722,15 +661,15 @@
             log=log,
             k=self.num_negatives,
             users=users,
             items=items,
             user_features=first_level_user_features,
             item_features=first_level_item_features,
             log_to_filter=log,
-        )
+        ).select("user_idx", "item_idx")
 
         candidates_cached = candidates.cache()
         unpersist_if_exists(first_level_user_features)
         unpersist_if_exists(first_level_item_features)
         self.logger.info("Adding features")
         candidates_features = self._add_features_for_second_level(
             log_to_add_features=candidates_cached,
@@ -741,62 +680,37 @@
         candidates_features.cache()
         candidates_cached.unpersist()
         self.logger.info(
             "Generated %s candidates for %s users",
             candidates_features.count(),
             candidates_features.select("user_idx").distinct().count(),
         )
-        candidates_features_pd = candidates_features.toPandas()
-        candidates_features.unpersist()
-        candidates_ids = candidates_features_pd[
-            ["user_idx", "item_idx", "relevance"]
-        ]
-        candidates_features_pd.drop(
-            columns=["user_idx", "item_idx"], inplace=True
-        )
-
-        self.logger.info("Starting reranking")
-        candidates_pred = self.second_stage_model.predict(
-            candidates_features_pd
-        )
-        candidates_ids["relevance"] = candidates_pred.data[:, 0]
-        self.logger.info(
-            "%s candidates rated for %s users",
-            candidates_ids.shape[0],
-            candidates.select("user_idx").distinct().count(),
-        )
-
-        self.logger.info("top-k")
-        return get_top_k_recs(
-            recs=convert2spark(candidates_ids), k=k, id_type="idx"
-        )
+        return self.second_stage_model.predict(data=candidates_features, k=k)
 
     def fit_predict(
         self,
         log: AnyDataFrame,
         k: int,
         users: Optional[Union[AnyDataFrame, Iterable]] = None,
         items: Optional[Union[AnyDataFrame, Iterable]] = None,
         user_features: Optional[AnyDataFrame] = None,
         item_features: Optional[AnyDataFrame] = None,
         filter_seen_items: bool = True,
-        force_reindex: bool = True,
     ) -> DataFrame:
         """
         :param log: input DataFrame ``[user_id, item_id, timestamp, relevance]``
         :param k: length of a recommendation list, must be smaller than the number of ``items``
         :param users: users to get recommendations for
         :param items: items to get recommendations for
         :param user_features: user features``[user_id]`` + feature columns
         :param item_features: item features``[item_id]`` + feature columns
         :param filter_seen_items: flag to removed seen items from recommendations
-        :param force_reindex: create indexers even if they were created
         :return: DataFrame ``[user_id, item_id, relevance]``
         """
-        self.fit(log, user_features, item_features, force_reindex)
+        self.fit(log, user_features, item_features)
         return self.predict(
             log,
             k,
             users,
             items,
             user_features,
             item_features,
@@ -862,19 +776,19 @@
         if self.fallback_model is not None:
             number_of_models += 1
         if number_of_models != len(param_borders):
             raise ValueError(
                 "Provide search grid or None for every first level model"
             )
 
-        first_level_user_features_tr = FirstLevelFeaturesProcessor()
+        first_level_user_features_tr = ToNumericFeatureTransformer()
         first_level_user_features = first_level_user_features_tr.fit_transform(
             user_features
         )
-        first_level_item_features_tr = FirstLevelFeaturesProcessor()
+        first_level_item_features_tr = ToNumericFeatureTransformer()
         first_level_item_features = first_level_item_features_tr.fit_transform(
             item_features
         )
 
         first_level_user_features = cache_if_exists(first_level_user_features)
         first_level_item_features = cache_if_exists(first_level_item_features)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `replay-rec-0.8.0/replay/session_handler.py` & `replay-rec-0.9.0/replay/session_handler.py`

 * *Files identical despite different names*

### Comparing `replay-rec-0.8.0/replay/splitters/base_splitter.py` & `replay-rec-0.9.0/replay/splitters/base_splitter.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 
 
 # pylint: disable=too-few-public-methods
 class Splitter(ABC):
     """Base class"""
 
     def __init__(
-        self,
-        drop_cold_items: bool,
-        drop_cold_users: bool,
+        self, drop_cold_items: bool, drop_cold_users: bool,
     ):
         """
         :param drop_cold_items: flag to remove items that are not in train data
         :param drop_cold_users: flag to remove users that are not in train data
         """
         self.drop_cold_users = drop_cold_users
         self.drop_cold_items = drop_cold_items
@@ -50,25 +48,25 @@
         :param test: DataFrame like train
         :param drop_cold_items: flag to remove cold items
         :param drop_cold_users: flag to remove cold users
         :return: filtered DataFrame
         """
         if drop_cold_items:
             train_tmp = train.select(
-                sf.col("item_id").alias("item")
+                sf.col("item_idx").alias("item")
             ).distinct()
-            test = test.join(train_tmp, train_tmp.item == test.item_id).drop(
+            test = test.join(train_tmp, train_tmp.item == test.item_idx).drop(
                 "item"
             )
 
         if drop_cold_users:
             train_tmp = train.select(
-                sf.col("user_id").alias("user")
+                sf.col("user_idx").alias("user")
             ).distinct()
-            test = test.join(train_tmp, train_tmp.user == test.user_id).drop(
+            test = test.join(train_tmp, train_tmp.user == test.user_idx).drop(
                 "user"
             )
         return test
 
     @abstractmethod
     def _core_split(self, log: DataFrame) -> SplitterReturnType:
         """
```

### Comparing `replay-rec-0.8.0/replay/splitters/log_splitter.py` & `replay-rec-0.9.0/replay/splitters/log_splitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,55 +98,55 @@
     """
     Only new users will be assigned to test set.
     Splits log by timestamp so that test has `test_size` fraction of most recent users.
 
 
     >>> from replay.splitters import NewUsersSplitter
     >>> import pandas as pd
-    >>> data_frame = pd.DataFrame({"user_id": [1,1,2,2,3,4],
-    ...    "item_id": [1,2,3,1,2,3],
+    >>> data_frame = pd.DataFrame({"user_idx": [1,1,2,2,3,4],
+    ...    "item_idx": [1,2,3,1,2,3],
     ...    "relevance": [1,2,3,4,5,6],
     ...    "timestamp": [20,40,20,30,10,40]})
     >>> data_frame
-       user_id  item_id  relevance  timestamp
-    0        1        1          1         20
-    1        1        2          2         40
-    2        2        3          3         20
-    3        2        1          4         30
-    4        3        2          5         10
-    5        4        3          6         40
+       user_idx  item_idx  relevance  timestamp
+    0         1         1          1         20
+    1         1         2          2         40
+    2         2         3          3         20
+    3         2         1          4         30
+    4         3         2          5         10
+    5         4         3          6         40
     >>> train, test = NewUsersSplitter(test_size=0.1).split(data_frame)
     >>> train.show()
-    +-------+-------+---------+---------+
-    |user_id|item_id|relevance|timestamp|
-    +-------+-------+---------+---------+
-    |      1|      1|        1|       20|
-    |      2|      3|        3|       20|
-    |      2|      1|        4|       30|
-    |      3|      2|        5|       10|
-    +-------+-------+---------+---------+
+    +--------+--------+---------+---------+
+    |user_idx|item_idx|relevance|timestamp|
+    +--------+--------+---------+---------+
+    |       1|       1|        1|       20|
+    |       2|       3|        3|       20|
+    |       2|       1|        4|       30|
+    |       3|       2|        5|       10|
+    +--------+--------+---------+---------+
     <BLANKLINE>
     >>> test.show()
-    +-------+-------+---------+---------+
-    |user_id|item_id|relevance|timestamp|
-    +-------+-------+---------+---------+
-    |      4|      3|        6|       40|
-    +-------+-------+---------+---------+
+    +--------+--------+---------+---------+
+    |user_idx|item_idx|relevance|timestamp|
+    +--------+--------+---------+---------+
+    |       4|       3|        6|       40|
+    +--------+--------+---------+---------+
     <BLANKLINE>
 
     Train DataFrame can be drastically reduced even with moderate
     `test_size` if the amount of new users is small.
 
     >>> train, test = NewUsersSplitter(test_size=0.3).split(data_frame)
     >>> train.show()
-    +-------+-------+---------+---------+
-    |user_id|item_id|relevance|timestamp|
-    +-------+-------+---------+---------+
-    |      3|      2|        5|       10|
-    +-------+-------+---------+---------+
+    +--------+--------+---------+---------+
+    |user_idx|item_idx|relevance|timestamp|
+    +--------+--------+---------+---------+
+    |       3|       2|        5|       10|
+    +--------+--------+---------+---------+
     <BLANKLINE>
     """
 
     def __init__(self, test_size: float, drop_cold_items: bool = False):
         """
         :param test_size: test size 0 to 1
         :param drop_cold_items: flag to drop cold items from test
@@ -155,20 +155,20 @@
             drop_cold_items=drop_cold_items, drop_cold_users=False
         )
         self.test_size = test_size
         if test_size < 0 or test_size > 1:
             raise ValueError("test_size must be 0 to 1")
 
     def _core_split(self, log: DataFrame) -> SplitterReturnType:
-        start_date_by_user = log.groupby("user_id").agg(
+        start_date_by_user = log.groupby("user_idx").agg(
             sf.min("timestamp").alias("start_dt")
         )
         test_start_date = (
             start_date_by_user.groupby("start_dt")
-            .agg(sf.count("user_id").alias("cnt"))
+            .agg(sf.count("user_idx").alias("cnt"))
             .select(
                 "start_dt",
                 sf.sum("cnt")
                 .over(Window.orderBy(sf.desc("start_dt")))
                 .alias("cnt"),
                 sf.sum("cnt").over(Window.orderBy(sf.lit(1))).alias("total"),
             )
@@ -178,15 +178,15 @@
         )
 
         train = log.filter(sf.col("timestamp") < test_start_date)
 
         test = log.join(
             start_date_by_user.filter(sf.col("start_dt") >= test_start_date),
             how="inner",
-            on="user_id",
+            on="user_idx",
         ).drop("start_dt")
         return train, test
 
 
 # pylint: disable=too-few-public-methods
 class ColdUserRandomSplitter(Splitter):
     """
@@ -209,14 +209,14 @@
         """
         super().__init__(
             drop_cold_items=drop_cold_items, drop_cold_users=drop_cold_users
         )
         self.test_size = test_size
 
     def _core_split(self, log: DataFrame) -> SplitterReturnType:
-        users = log.select("user_id").distinct()
+        users = log.select("user_idx").distinct()
         train_users, test_users = users.randomSplit(
             [1 - self.test_size, self.test_size], seed=self.seed,
         )
-        train = log.join(train_users, on="user_id", how="inner")
-        test = log.join(test_users, on="user_id", how="inner")
+        train = log.join(train_users, on="user_idx", how="inner")
+        test = log.join(test_users, on="user_idx", how="inner")
         return train, test
```

### Comparing `replay-rec-0.8.0/replay/splitters/user_log_splitter.py` & `replay-rec-0.9.0/replay/splitters/user_log_splitter.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,67 +20,70 @@
 
     >>> from replay.session_handler import get_spark_session, State
     >>> spark = get_spark_session(1, 1)
     >>> state = State(spark)
 
     >>> from replay.splitters import UserSplitter
     >>> import pandas as pd
-    >>> data_frame = pd.DataFrame({"user_id": [1,1,1,2,2,2],
-    ...    "item_id": [1,2,3,1,2,3],
+    >>> data_frame = pd.DataFrame({"user_idx": [1,1,1,2,2,2],
+    ...    "item_idx": [1,2,3,1,2,3],
     ...    "relevance": [1,2,3,4,5,6],
     ...    "timestamp": [1,2,3,3,2,1]})
     >>> data_frame
-       user_id  item_id  relevance  timestamp
-    0        1        1          1          1
-    1        1        2          2          2
-    2        1        3          3          3
-    3        2        1          4          3
-    4        2        2          5          2
-    5        2        3          6          1
+       user_idx  item_idx  relevance  timestamp
+    0         1         1          1          1
+    1         1         2          2          2
+    2         1         3          3          3
+    3         2         1          4          3
+    4         2         2          5          2
+    5         2         3          6          1
+
+    >>> from replay.utils import convert2spark
+    >>> data_frame = convert2spark(data_frame)
 
     By default, test is one last item for each user
 
     >>> UserSplitter(seed=80083).split(data_frame)[-1].toPandas()
-       user_id  item_id  relevance  timestamp
-    0        1        3          3          3
-    1        2        1          4          3
+       user_idx  item_idx  relevance  timestamp
+    0         1         3          3          3
+    1         2         1          4          3
 
     Random records can be retrieved with ``shuffle``:
 
     >>> UserSplitter(shuffle=True, seed=80083).split(data_frame)[-1].toPandas()
-       user_id  item_id  relevance  timestamp
-    0        1        2          2          2
-    1        2        3          6          1
+       user_idx  item_idx  relevance  timestamp
+    0         1         2          2          2
+    1         2         3          6          1
 
     You can specify the number of items for each user:
 
     >>> UserSplitter(item_test_size=3, shuffle=True, seed=80083).split(data_frame)[-1].toPandas()
-       user_id  item_id  relevance  timestamp
-    0        1        2          2          2
-    1        1        3          3          3
-    2        1        1          1          1
-    3        2        3          6          1
-    4        2        2          5          2
-    5        2        1          4          3
+       user_idx  item_idx  relevance  timestamp
+    0         1         2          2          2
+    1         1         3          3          3
+    2         1         1          1          1
+    3         2         3          6          1
+    4         2         2          5          2
+    5         2         1          4          3
 
     Or a fraction:
 
     >>> UserSplitter(item_test_size=0.67, shuffle=True, seed=80083).split(data_frame)[-1].toPandas()
-       user_id  item_id  relevance  timestamp
-    0        1        2          2          2
-    1        1        3          3          3
-    2        2        3          6          1
-    3        2        2          5          2
+       user_idx  item_idx  relevance  timestamp
+    0         1         2          2          2
+    1         1         3          3          3
+    2         2         3          6          1
+    3         2         2          5          2
 
     `user_test_size` allows to put exact number of users into test set
 
-    >>> UserSplitter(user_test_size=1, item_test_size=2, seed=42).split(data_frame)[-1].toPandas().user_id.nunique()
+    >>> UserSplitter(user_test_size=1, item_test_size=2, seed=42).split(data_frame)[-1].toPandas().user_idx.nunique()
     1
 
-    >>> UserSplitter(user_test_size=0.5, item_test_size=2, seed=42).split(data_frame)[-1].toPandas().user_id.nunique()
+    >>> UserSplitter(user_test_size=0.5, item_test_size=2, seed=42).split(data_frame)[-1].toPandas().user_idx.nunique()
     1
 
     """
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
@@ -110,15 +113,15 @@
         self.seed = seed
 
     def _get_test_users(self, log: DataFrame,) -> DataFrame:
         """
         :param log: input DataFrame
         :return: Spark DataFrame with single column `user_id`
         """
-        all_users = log.select("user_id").distinct()
+        all_users = log.select("user_idx").distinct()
         user_count = all_users.count()
         if self.user_test_size is not None:
             value_error = False
             if isinstance(self.user_test_size, int):
                 if 1 <= self.user_test_size < user_count:
                     test_user_count = self.user_test_size
                 else:
@@ -150,28 +153,28 @@
         """
         Proportionate split
 
         :param log: input DataFrame `[timestamp, user_id, item_id, relevance]`
         :return: train and test DataFrames
         """
 
-        counts = log.groupBy("user_id").count()
+        counts = log.groupBy("user_idx").count()
         test_users = self._get_test_users(log).withColumn(
             "test_user", sf.lit(1)
         )
         if self.shuffle:
             res = self._add_random_partition(
-                log.join(test_users, how="left", on="user_id")
+                log.join(test_users, how="left", on="user_idx")
             )
         else:
             res = self._add_time_partition(
-                log.join(test_users, how="left", on="user_id")
+                log.join(test_users, how="left", on="user_idx")
             )
 
-        res = res.join(counts, on="user_id", how="left")
+        res = res.join(counts, on="user_idx", how="left")
         res = res.withColumn("frac", sf.col("row_num") / sf.col("count"))
         train = res.filter(
             f"""
                     frac > {self.item_test_size} OR
                     test_user IS NULL
                 """
         ).drop("rand", "row_num", "count", "frac", "test_user")
@@ -192,19 +195,19 @@
         """
 
         test_users = self._get_test_users(log).withColumn(
             "test_user", sf.lit(1)
         )
         if self.shuffle:
             res = self._add_random_partition(
-                log.join(test_users, how="left", on="user_id")
+                log.join(test_users, how="left", on="user_idx")
             )
         else:
             res = self._add_time_partition(
-                log.join(test_users, how="left", on="user_id")
+                log.join(test_users, how="left", on="user_idx")
             )
         train = res.filter(
             f"""
                     row_num > {self.item_test_size} OR
                     test_user IS NULL
                 """
         ).drop("rand", "row_num", "test_user")
@@ -237,15 +240,15 @@
         :param dataframe: input DataFrame with `user_id` column
         :returns: processed DataFrame
         """
         dataframe = dataframe.withColumn("rand", sf.rand(self.seed))
         dataframe = dataframe.withColumn(
             "row_num",
             sf.row_number().over(
-                Window.partitionBy("user_id").orderBy("rand")
+                Window.partitionBy("user_idx").orderBy("rand")
             ),
         )
         return dataframe
 
     @staticmethod
     def _add_time_partition(dataframe: DataFrame) -> DataFrame:
         """
@@ -253,15 +256,15 @@
 
         :param dataframe: input DataFrame with `[timestamp, user_id]`
         :returns: processed DataFrame
         """
         res = dataframe.withColumn(
             "row_num",
             sf.row_number().over(
-                Window.partitionBy("user_id").orderBy(
+                Window.partitionBy("user_idx").orderBy(
                     sf.col("timestamp").desc()
                 )
             ),
         )
         return res
 
 
@@ -282,14 +285,16 @@
     """
     if splitter not in {"user"}:
         raise ValueError(f"Wrong splitter parameter: {splitter}")
     if splitter == "user":
         dataframe = convert2spark(log).withColumn("rand", sf.rand(seed))
         dataframe = dataframe.withColumn(
             "fold",
-            sf.row_number().over(Window.partitionBy("user_id").orderBy("rand"))
+            sf.row_number().over(
+                Window.partitionBy("user_idx").orderBy("rand")
+            )
             % n_folds,
         ).drop("rand")
         for i in range(n_folds):
             train = dataframe.filter(f"fold != {i}").drop("fold")
             test = dataframe.filter(f"fold == {i}").drop("fold")
             yield train, test
```

### Comparing `replay-rec-0.8.0/replay/time.py` & `replay-rec-0.9.0/replay/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,77 +20,77 @@
     :param kind: type of smoothing, one of [power, exp, linear]
         Corresponding functions are ``power``: ``age^c``,
         ``exp``: ``c^age``, ``linear``: ``1-c*age``
     :return: DataFrame with item weights
 
     >>> import pandas as pd
     >>> d = {}
-    >>> d["item_id"] = [1, 1, 2, 3, 3]
+    >>> d["item_idx"] = [1, 1, 2, 3, 3]
     >>> d["timestamp"] = ["2099-03-19", "2099-03-20", "2099-03-22", "2099-03-27", "2099-03-25"]
     >>> d["relevance"] = [1, 1, 1, 1, 1]
     >>> df = pd.DataFrame(d)
     >>> df
-       item_id   timestamp  relevance
-    0        1  2099-03-19          1
-    1        1  2099-03-20          1
-    2        2  2099-03-22          1
-    3        3  2099-03-27          1
-    4        3  2099-03-25          1
+       item_idx   timestamp  relevance
+    0         1  2099-03-19          1
+    1         1  2099-03-20          1
+    2         2  2099-03-22          1
+    3         3  2099-03-27          1
+    4         3  2099-03-25          1
 
     Age in days is calculated for every item,
     which is transformed into a weight using some function.
     There are three types of smoothing types available: power, exp and linear.
     Each type calculates a parameter ``c`` based on the ``decay`` argument,
     so that an item with ``age==decay`` has weight 0.5.
 
     Power smoothing falls quickly in the beginning but decays slowly afterwards as ``age^c``.
 
-    >>> get_item_recency(df, kind="power").orderBy("item_id").show()
-    +-------+-------------------+------------------+
-    |item_id|          timestamp|         relevance|
-    +-------+-------------------+------------------+
-    |      1|2099-03-19 12:00:00|0.6632341020947187|
-    |      2|2099-03-22 00:00:00|0.7203662792445817|
-    |      3|2099-03-26 00:00:00|               1.0|
-    +-------+-------------------+------------------+
+    >>> get_item_recency(df, kind="power").orderBy("item_idx").show()
+    +--------+-------------------+------------------+
+    |item_idx|          timestamp|         relevance|
+    +--------+-------------------+------------------+
+    |       1|2099-03-19 12:00:00|0.6632341020947187|
+    |       2|2099-03-22 00:00:00|0.7203662792445817|
+    |       3|2099-03-26 00:00:00|               1.0|
+    +--------+-------------------+------------------+
     <BLANKLINE>
 
     Exponential smoothing is the other way around. Old objects decay more quickly as ``c^age``.
 
-    >>> get_item_recency(df, kind="exp").orderBy("item_id").show()
-    +-------+-------------------+------------------+
-    |item_id|          timestamp|         relevance|
-    +-------+-------------------+------------------+
-    |      1|2099-03-19 12:00:00|0.8605514372443298|
-    |      2|2099-03-22 00:00:00|0.9117224885582166|
-    |      3|2099-03-26 00:00:00|               1.0|
-    +-------+-------------------+------------------+
+    >>> get_item_recency(df, kind="exp").orderBy("item_idx").show()
+    +--------+-------------------+------------------+
+    |item_idx|          timestamp|         relevance|
+    +--------+-------------------+------------------+
+    |       1|2099-03-19 12:00:00|0.8605514372443298|
+    |       2|2099-03-22 00:00:00|0.9117224885582166|
+    |       3|2099-03-26 00:00:00|               1.0|
+    +--------+-------------------+------------------+
     <BLANKLINE>
 
     Last type is a linear smoothing: ``1 - c*age``.
 
-    >>> get_item_recency(df, kind="linear").orderBy("item_id").show()
-    +-------+-------------------+------------------+
-    |item_id|          timestamp|         relevance|
-    +-------+-------------------+------------------+
-    |      1|2099-03-19 12:00:00|0.8916666666666666|
-    |      2|2099-03-22 00:00:00|0.9333333333333333|
-    |      3|2099-03-26 00:00:00|               1.0|
-    +-------+-------------------+------------------+
+    >>> get_item_recency(df, kind="linear").orderBy("item_idx").show()
+    +--------+-------------------+------------------+
+    |item_idx|          timestamp|         relevance|
+    +--------+-------------------+------------------+
+    |       1|2099-03-19 12:00:00|0.8916666666666666|
+    |       2|2099-03-22 00:00:00|0.9333333333333333|
+    |       3|2099-03-26 00:00:00|               1.0|
+    +--------+-------------------+------------------+
     <BLANKLINE>
 
     This function **does not** take relevance values of interactions into account.
     Only item age is used.
     """
     log = convert2spark(log)
     items = log.select(
-        "item_id",
+        "item_idx",
         sf.unix_timestamp(sf.to_timestamp("timestamp")).alias("timestamp"),
     )
-    items = items.groupBy("item_id").agg(
+    items = items.groupBy("item_idx").agg(
         sf.mean("timestamp").alias("timestamp")
     )
     items = items.withColumn("relevance", sf.lit(1))
     items = smoothe_time(items, decay, limit, kind)
     return items
 
 
@@ -109,89 +109,89 @@
     :param kind: type of smoothing, one of [power, exp, linear].
         Corresponding functions are ``power``: ``age^c``,
         ``exp``: ``c^age``, ``linear``: ``1-c*age``
     :return: modified DataFrame
 
     >>> import pandas as pd
     >>> d = {}
-    >>> d["item_id"] = [1, 1, 2, 3, 3]
+    >>> d["item_idx"] = [1, 1, 2, 3, 3]
     >>> d["timestamp"] = ["2099-03-19", "2099-03-20", "2099-03-22", "2099-03-27", "2099-03-25"]
     >>> d["relevance"] = [1, 1, 1, 1, 1]
     >>> df = pd.DataFrame(d)
     >>> df
-       item_id   timestamp  relevance
-    0        1  2099-03-19          1
-    1        1  2099-03-20          1
-    2        2  2099-03-22          1
-    3        3  2099-03-27          1
-    4        3  2099-03-25          1
+       item_idx   timestamp  relevance
+    0         1  2099-03-19          1
+    1         1  2099-03-20          1
+    2         2  2099-03-22          1
+    3         3  2099-03-27          1
+    4         3  2099-03-25          1
 
     Power smoothing falls quickly in the beginning but decays slowly afterwards as ``age^c``.
 
     >>> smoothe_time(df, kind="power").orderBy("timestamp").show()
-    +-------+-------------------+------------------+
-    |item_id|          timestamp|         relevance|
-    +-------+-------------------+------------------+
-    |      1|2099-03-19 00:00:00|0.6390430306850825|
-    |      1|2099-03-20 00:00:00| 0.654567945027101|
-    |      2|2099-03-22 00:00:00|0.6940913454809814|
-    |      3|2099-03-25 00:00:00|0.7994016704292545|
-    |      3|2099-03-27 00:00:00|               1.0|
-    +-------+-------------------+------------------+
+    +--------+-------------------+------------------+
+    |item_idx|          timestamp|         relevance|
+    +--------+-------------------+------------------+
+    |       1|2099-03-19 00:00:00|0.6390430306850825|
+    |       1|2099-03-20 00:00:00| 0.654567945027101|
+    |       2|2099-03-22 00:00:00|0.6940913454809814|
+    |       3|2099-03-25 00:00:00|0.7994016704292545|
+    |       3|2099-03-27 00:00:00|               1.0|
+    +--------+-------------------+------------------+
     <BLANKLINE>
 
     Exponential smoothing is the other way around. Old objects decay more quickly as ``c^age``.
 
     >>> smoothe_time(df, kind="exp").orderBy("timestamp").show()
-    +-------+-------------------+------------------+
-    |item_id|          timestamp|         relevance|
-    +-------+-------------------+------------------+
-    |      1|2099-03-19 00:00:00|0.8312378961427874|
-    |      1|2099-03-20 00:00:00|0.8506671609508554|
-    |      2|2099-03-22 00:00:00| 0.890898718140339|
-    |      3|2099-03-25 00:00:00|0.9548416039104165|
-    |      3|2099-03-27 00:00:00|               1.0|
-    +-------+-------------------+------------------+
+    +--------+-------------------+------------------+
+    |item_idx|          timestamp|         relevance|
+    +--------+-------------------+------------------+
+    |       1|2099-03-19 00:00:00|0.8312378961427874|
+    |       1|2099-03-20 00:00:00|0.8506671609508554|
+    |       2|2099-03-22 00:00:00| 0.890898718140339|
+    |       3|2099-03-25 00:00:00|0.9548416039104165|
+    |       3|2099-03-27 00:00:00|               1.0|
+    +--------+-------------------+------------------+
     <BLANKLINE>
 
     Last type is a linear smoothing: ``1 - c*age``.
 
     >>> smoothe_time(df, kind="linear").orderBy("timestamp").show()
-    +-------+-------------------+------------------+
-    |item_id|          timestamp|         relevance|
-    +-------+-------------------+------------------+
-    |      1|2099-03-19 00:00:00|0.8666666666666667|
-    |      1|2099-03-20 00:00:00|0.8833333333333333|
-    |      2|2099-03-22 00:00:00|0.9166666666666666|
-    |      3|2099-03-25 00:00:00|0.9666666666666667|
-    |      3|2099-03-27 00:00:00|               1.0|
-    +-------+-------------------+------------------+
+    +--------+-------------------+------------------+
+    |item_idx|          timestamp|         relevance|
+    +--------+-------------------+------------------+
+    |       1|2099-03-19 00:00:00|0.8666666666666667|
+    |       1|2099-03-20 00:00:00|0.8833333333333333|
+    |       2|2099-03-22 00:00:00|0.9166666666666666|
+    |       3|2099-03-25 00:00:00|0.9666666666666667|
+    |       3|2099-03-27 00:00:00|               1.0|
+    +--------+-------------------+------------------+
     <BLANKLINE>
 
     These examples use constant relevance 1, so resulting weight equals the time dependent weight.
     But actually this value is an updated relevance.
 
     >>> d = {}
-    >>> d["item_id"] = [1, 2, 3]
+    >>> d["item_idx"] = [1, 2, 3]
     >>> d["timestamp"] = ["2099-03-19", "2099-03-20", "2099-03-22"]
     >>> d["relevance"] = [10, 3, 0.1]
     >>> df = pd.DataFrame(d)
     >>> df
-       item_id   timestamp  relevance
-    0        1  2099-03-19       10.0
-    1        2  2099-03-20        3.0
-    2        3  2099-03-22        0.1
+       item_idx   timestamp  relevance
+    0         1  2099-03-19       10.0
+    1         2  2099-03-20        3.0
+    2         3  2099-03-22        0.1
     >>> smoothe_time(df).orderBy("timestamp").show()
-    +-------+-------------------+------------------+
-    |item_id|          timestamp|         relevance|
-    +-------+-------------------+------------------+
-    |      1|2099-03-19 00:00:00| 9.330329915368074|
-    |      2|2099-03-20 00:00:00|2.8645248117312496|
-    |      3|2099-03-22 00:00:00|               0.1|
-    +-------+-------------------+------------------+
+    +--------+-------------------+------------------+
+    |item_idx|          timestamp|         relevance|
+    +--------+-------------------+------------------+
+    |       1|2099-03-19 00:00:00| 9.330329915368074|
+    |       2|2099-03-20 00:00:00|2.8645248117312496|
+    |       3|2099-03-22 00:00:00|               0.1|
+    +--------+-------------------+------------------+
     <BLANKLINE>
     """
     log = convert2spark(log)
     log = log.withColumn(
         "timestamp", sf.unix_timestamp(sf.to_timestamp("timestamp"))
     )
     last_date = (
```

### Comparing `replay-rec-0.8.0/replay/utils.py` & `replay-rec-0.9.0/replay/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
             ),
         )
         .filter(sf.col("temp_rank") <= k)
         .drop("temp_rank")
     )
 
 
-def get_top_k_recs(recs: DataFrame, k: int, id_type: str = "id") -> DataFrame:
+def get_top_k_recs(recs: DataFrame, k: int, id_type: str = "idx") -> DataFrame:
     """
     Get top k recommendations by `relevance`.
 
     :param recs: recommendations DataFrame
         `[user_id, item_id, relevance]`
     :param k: length of a recommendation list
     :param id_type: id or idx
@@ -246,33 +246,33 @@
 
 def get_log_info(log: DataFrame) -> str:
     """
     Basic log statistics
 
     >>> from replay.session_handler import State
     >>> spark = State().session
-    >>> log = spark.createDataFrame([(1, 2), (3, 4), (5, 2)]).toDF("user_id", "item_id")
+    >>> log = spark.createDataFrame([(1, 2), (3, 4), (5, 2)]).toDF("user_idx", "item_idx")
     >>> log.show()
-    +-------+-------+
-    |user_id|item_id|
-    +-------+-------+
-    |      1|      2|
-    |      3|      4|
-    |      5|      2|
-    +-------+-------+
+    +--------+--------+
+    |user_idx|item_idx|
+    +--------+--------+
+    |       1|       2|
+    |       3|       4|
+    |       5|       2|
+    +--------+--------+
     <BLANKLINE>
     >>> get_log_info(log)
     'total lines: 3, total users: 3, total items: 2'
 
-    :param log: interaction log containing ``user_id`` and ``item_id``
+    :param log: interaction log containing ``user_idx`` and ``item_idx``
     :returns: statistics string
     """
     cnt = log.count()
-    user_cnt = log.select("user_id").distinct().count()
-    item_cnt = log.select("item_id").distinct().count()
+    user_cnt = log.select("user_idx").distinct().count()
+    item_cnt = log.select("item_idx").distinct().count()
     return ", ".join(
         [
             f"total lines: {cnt}",
             f"total users: {user_cnt}",
             f"total items: {item_cnt}",
         ]
     )
@@ -304,15 +304,15 @@
     |      2|     1.0|      1|      1|        1|         1|
     |      3|     2.5|      3|      2|        2|         2|
     |      1|     2.0|      2|      2|        1|         2|
     +-------+--------+-------+-------+---------+----------+
     <BLANKLINE>
 
     :param log: spark DataFrame with ``user_id``, ``item_id`` and ``relevance`` columns
-    :param group_by: column to group data by, ``user_id`` или ``item_id``
+    :param group_by: column to group data by, ``user_id`` or ``item_id``
     :param target_column: column with interaction ratings
     :return: spark DataFrame with statistics
     """
     agg_functions = {
         "mean": sf.avg,
         "max": sf.max,
         "min": sf.min,
@@ -449,28 +449,30 @@
     """
     if second is None:
         return first
     return first.join(second, on=on, how=how)
 
 
 def fallback(
-    base: DataFrame, fill: DataFrame, k: int, id_type: str = "id"
+    base: DataFrame, fill: DataFrame, k: int, id_type: str = "idx"
 ) -> DataFrame:
     """
     Fill missing recommendations for users that have less than ``k`` recomended items.
     Score values for the fallback model may be decreased to preserve sorting.
 
     :param base: base recommendations that need to be completed
     :param fill: extra recommendations
     :param k: desired recommendation list lengths for each user
     :param id_type: id or idx
     :return: augmented recommendations
     """
     if fill is None:
         return base
+    if base.count() == 0:
+        return get_top_k_recs(fill, k, id_type)
     margin = 0.1
     min_in_base = base.agg({"relevance": "min"}).collect()[0][0]
     max_in_fill = fill.agg({"relevance": "max"}).collect()[0][0]
     diff = max_in_fill - min_in_base
     fill = fill.withColumnRenamed("relevance", "relevance_fallback")
     if diff >= 0:
         fill = fill.withColumn(
@@ -591,17 +593,15 @@
         )
         .drop("tmp")
     )
     return dataframe
 
 
 def process_timestamp_column(
-    dataframe: DataFrame,
-    column_name: str,
-    date_format: Optional[str] = None,
+    dataframe: DataFrame, column_name: str, date_format: Optional[str] = None,
 ) -> DataFrame:
     """
     Convert ``column_name`` column of numeric/string/timestamp type
     to TimestampType.
     Return original ``dataframe`` if the column has TimestampType.
     Treats numbers as unix timestamp, treats strings as
     a string representation of dates in ``date_format``.
@@ -624,16 +624,15 @@
     if isinstance(dataframe.schema[column_name].dataType, st.NumericType):
         return dataframe.withColumn(
             column_name, sf.to_timestamp(sf.from_unixtime(sf.col(column_name)))
         )
 
     # datetime in string format
     dataframe = dataframe.withColumn(
-        column_name,
-        sf.to_timestamp(sf.col(column_name), format=date_format),
+        column_name, sf.to_timestamp(sf.col(column_name), format=date_format),
     )
     return dataframe
 
 
 @sf.udf(returnType=VectorUDT())
 def list_to_vector_udf(array: st.ArrayType) -> DenseVector:
     """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `replay-rec-0.8.0/setup.py` & `replay-rec-0.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,36 +9,36 @@
  'replay.scenarios.two_stages',
  'replay.splitters']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['implicit',
+['implicit<0.5',
  'lightautoml>=0.3.1',
  'lightfm',
  'llvmlite>=0.32.1',
  'numba>=0.50',
  'numpy>=1.20.0',
  'optuna',
  'pandas',
  'psutil',
  'pyarrow',
- 'pyspark>=3.0.0,<4.0.0',
+ 'pyspark>=3.0,<3.2',
  'pytorch-ignite',
  'scikit-learn',
  'scipy',
  'seaborn',
  'torch']
 
 setup_kwargs = {
     'name': 'replay-rec',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'RecSys Library',
-    'long_description': '# RePlay\n\nRePlay is a library providing tools for all stages of creating a recommendation system, from data preprocessing to model evaluation and comparison.\n\nRePlay uses PySpark to handle big data.\n\nYou can\n\n- Filter and split data\n- Train models\n- Optimize hyper parameters\n- Evaluate predictions with metrics\n- Combine predictions from different models\n- Create a two-level model\n\n\n## Docs\n\n[Documentation](https://sberbank-ai-lab.github.io/RePlay/)\n\n\n### Installation\n\nUse Linux machine with Python 3.7+ and Java 8+. \n\n```bash\npip install replay-rec\n```\n\nIt is preferable to use a virtual environment for your installation.\n',
+    'long_description': '# RePlay\n\nRePlay is a library providing tools for all stages of creating a recommendation system, from data preprocessing to model evaluation and comparison.\n\nRePlay uses PySpark to handle big data.\n\nYou can\n\n- Filter and split data\n- Train models\n- Optimize hyper parameters\n- Evaluate predictions with metrics\n- Combine predictions from different models\n- Create a two-level model\n\n\n## Docs\n\n[Documentation](https://sberbank-ai-lab.github.io/RePlay/)\n\n\n### Installation\n\nUse Linux machine with Python 3.7+, Java 8+ and C++ compiler. \n\n```bash\npip install replay-rec\n```\n\nIt is preferable to use a virtual environment for your installation.\n\nIf you encounter an error during RePlay installation, check the [troubleshooting](https://sberbank-ai-lab.github.io/RePlay/pages/installation.html#troubleshooting) guide.',
     'author': 'AI Lab, Sber',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://sberbank-ai-lab.github.io/RePlay/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `replay-rec-0.8.0/PKG-INFO` & `replay-rec-0.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replay-rec
-Version: 0.8.0
+Version: 0.9.0
 Summary: RecSys Library
 Home-page: https://sberbank-ai-lab.github.io/RePlay/
 Author: AI Lab, Sber
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
@@ -12,25 +12,25 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Typing :: Typed
-Requires-Dist: implicit
+Requires-Dist: implicit (<0.5)
 Requires-Dist: lightautoml (>=0.3.1)
 Requires-Dist: lightfm
 Requires-Dist: llvmlite (>=0.32.1)
 Requires-Dist: numba (>=0.50)
 Requires-Dist: numpy (>=1.20.0)
 Requires-Dist: optuna
 Requires-Dist: pandas
 Requires-Dist: psutil
 Requires-Dist: pyarrow
-Requires-Dist: pyspark (>=3.0.0,<4.0.0)
+Requires-Dist: pyspark (>=3.0,<3.2)
 Requires-Dist: pytorch-ignite
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: seaborn
 Requires-Dist: torch
 Project-URL: Repository, https://github.com/sberbank-ai-lab/RePlay
 Description-Content-Type: text/markdown
@@ -54,15 +54,16 @@
 ## Docs
 
 [Documentation](https://sberbank-ai-lab.github.io/RePlay/)
 
 
 ### Installation
 
-Use Linux machine with Python 3.7+ and Java 8+. 
+Use Linux machine with Python 3.7+, Java 8+ and C++ compiler. 
 
 ```bash
 pip install replay-rec
 ```
 
 It is preferable to use a virtual environment for your installation.
 
+If you encounter an error during RePlay installation, check the [troubleshooting](https://sberbank-ai-lab.github.io/RePlay/pages/installation.html#troubleshooting) guide.
```

